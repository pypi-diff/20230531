# Comparing `tmp/LumosWeb-0.0.9.tar.gz` & `tmp/LumosWeb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-0.0.9.tar", last modified: Tue May 30 11:48:13 2023, max compression
+gzip compressed data, was "LumosWeb-1.0.0.tar", last modified: Wed May 31 19:57:51 2023, max compression
```

## Comparing `LumosWeb-0.0.9.tar` & `LumosWeb-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:48:13.007133 LumosWeb-0.0.9/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:48:12.648828 LumosWeb-0.0.9/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.9/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4729 2023-05-30 11:47:49.000000 LumosWeb-0.0.9/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      596 2023-05-30 11:39:42.000000 LumosWeb-0.0.9/LumosWeb/cli.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.9/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.9/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:48:12.943995 LumosWeb-0.0.9/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-05-30 11:48:12.000000 LumosWeb-0.0.9/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:48:12.999585 LumosWeb-0.0.9/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3760 2023-05-29 14:14:31.000000 LumosWeb-0.0.9/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-30 11:48:13.009900 LumosWeb-0.0.9/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-05-30 11:48:07.000000 LumosWeb-0.0.9/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 19:57:51.768988 LumosWeb-1.0.0/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 19:57:51.410234 LumosWeb-1.0.0/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.0.0/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4872 2023-05-31 19:49:07.000000 LumosWeb-1.0.0/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      971 2023-05-31 15:15:46.000000 LumosWeb-1.0.0/LumosWeb/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.0.0/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.0.0/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 19:57:51.712358 LumosWeb-1.0.0/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4269 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4269 2023-05-31 19:57:51.762984 LumosWeb-1.0.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4098 2023-05-31 19:57:30.000000 LumosWeb-1.0.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-31 19:57:51.771209 LumosWeb-1.0.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-05-31 19:55:55.000000 LumosWeb-1.0.0/setup.py
```

### Comparing `LumosWeb-0.0.9/LumosWeb/api.py` & `LumosWeb-1.0.0/LumosWeb/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import socket
 from webob import Request
 from parse import parse
 import inspect
 from requests import Session as RequestsSession
 from wsgiadapter import WSGIAdapter as RequestsWSGIAdapter
+from wsgiref.simple_server import make_server
 import os
 from jinja2 import Environment, FileSystemLoader
 from whitenoise import WhiteNoise
 from .middleware import Middleware
 from .response import Response
-import http.server
-import socketserver
 
 class API:
     def __init__(self, templates_dir="templates", static_dir="static"):
         self.routes = {}  # dictionary of routes and handlers, path as keys and handlers as values
 
         self.templates_env = Environment(
             loader = FileSystemLoader(os.path.abspath(templates_dir))
@@ -102,24 +102,26 @@
         return self.templates_env.get_template(template_name).render(**context)
     
     def add_exception_handler(self, exception_handler):
         self.exception_handler = exception_handler
 
     def add_middleware(self, middleware_cls):
         self.middleware.add(middleware_cls)
+        
+    def run(self, host="localhost", port=8080):
+        while True:
+            try:
+                server = make_server(host, port, self)
+                break  # Exit the loop if the server is created successfully
+            except OSError as e:
+                if e.errno == socket.errno.EADDRINUSE:
+                    # Port is already in use, try another port
+                    port += 1
+                    print(f"Port {port-1} is not available, trying port {port}")
+                else:
+                    # Other error occurred, raise the exception
+                    raise
+
+        actual_port = server.server_port
+        print(f"Starting Lumos server on {host}:{actual_port}")
+        server.serve_forever()
 
-    def run_server(self):
-        # Assuming you have defined your app instance and configurations
-        app = self.create_app()
-        host = '127.0.0.1'
-        port = 8000
-
-        # Create a simple HTTP server and assign it to the specified host and port
-        server_address = (host, port)
-        httpd = socketserver.TCPServer(server_address, http.server.SimpleHTTPRequestHandler)
-
-        # Set the app as the server's request handler
-        httpd.set_app(app)
-
-        # Start the server
-        print(f"Serving Lumos app on http://{host}:{port} (Press CTRL+C to quit)")
-        httpd.serve_forever()
```

### Comparing `LumosWeb-0.0.9/LumosWeb/middleware.py` & `LumosWeb-1.0.0/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.9/LumosWeb/response.py` & `LumosWeb-1.0.0/LumosWeb/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,7 +26,8 @@
         if self.text is not None:
             self.body = self.text
             self.content_type = "text/plain"
 
         if self.html is not None:
             self.body = self.html.encode()
             self.content_type = "text/html"
+
```

### Comparing `LumosWeb-0.0.9/LumosWeb.egg-info/PKG-INFO` & `LumosWeb-1.0.0/LumosWeb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.9
+Version: 1.0.0
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
 ## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
+- To ensure compatibility and access the latest features and improvements, it is highly recommended to use version 1.0.0 or higher of the package. 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 - [PyPI Release](https://pypi.org/project/LumosWeb/)
 
 
 
 ## Installation
@@ -24,16 +25,23 @@
 e.g. pip install LumosWeb==0.0.2
 ```
 
 ## Getting Started
 
 ### Basic usage
 
+### Define App
+
+```python
+from LumosWeb.api import API()
+app = API()  # We created our api instance
+```
+
 ```python
-@app.route("/home", allowed_methods=["get"])
+@app.route("/home", allowed_methods=["get", "post", "put", "delete"])
 def home(request, response):
     if request.method == "get":
         response.text = "Hello from the HOME page"
     else:
         raise AttributeError("Method not allowed.")
 
 # Parameterized routes
@@ -45,14 +53,16 @@
 def handler(req, resp):
     resp.text = "We don't have to use decorators!"
 
 app.add_route("/sample", handler, allowed_methods=["get", "post"])
 
 
 ```
+### Run Server
+> Lumosweb --app <module_name> run
 
 ### Unit Test
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
 that you may want to use when writing unit tests with LumosWeb. The first one is `app` which is an instance of the main `API` class:
 ```python
 def test_basic_route_adding(api):
```

### Comparing `LumosWeb-0.0.9/PKG-INFO` & `LumosWeb-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.9
+Version: 1.0.0
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
 ## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
+- To ensure compatibility and access the latest features and improvements, it is highly recommended to use version 1.0.0 or higher of the package. 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 - [PyPI Release](https://pypi.org/project/LumosWeb/)
 
 
 
 ## Installation
@@ -24,16 +25,23 @@
 e.g. pip install LumosWeb==0.0.2
 ```
 
 ## Getting Started
 
 ### Basic usage
 
+### Define App
+
+```python
+from LumosWeb.api import API()
+app = API()  # We created our api instance
+```
+
 ```python
-@app.route("/home", allowed_methods=["get"])
+@app.route("/home", allowed_methods=["get", "post", "put", "delete"])
 def home(request, response):
     if request.method == "get":
         response.text = "Hello from the HOME page"
     else:
         raise AttributeError("Method not allowed.")
 
 # Parameterized routes
@@ -45,14 +53,16 @@
 def handler(req, resp):
     resp.text = "We don't have to use decorators!"
 
 app.add_route("/sample", handler, allowed_methods=["get", "post"])
 
 
 ```
+### Run Server
+> Lumosweb --app <module_name> run
 
 ### Unit Test
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
 that you may want to use when writing unit tests with LumosWeb. The first one is `app` which is an instance of the main `API` class:
 ```python
 def test_basic_route_adding(api):
```

### Comparing `LumosWeb-0.0.9/README.md` & `LumosWeb-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
+- To ensure compatibility and access the latest features and improvements, it is highly recommended to use version 1.0.0 or higher of the package. 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 - [PyPI Release](https://pypi.org/project/LumosWeb/)
 
 
 
 ## Installation
@@ -12,16 +13,23 @@
 e.g. pip install LumosWeb==0.0.2
 ```
 
 ## Getting Started
 
 ### Basic usage
 
+### Define App
+
+```python
+from LumosWeb.api import API()
+app = API()  # We created our api instance
+```
+
 ```python
-@app.route("/home", allowed_methods=["get"])
+@app.route("/home", allowed_methods=["get", "post", "put", "delete"])
 def home(request, response):
     if request.method == "get":
         response.text = "Hello from the HOME page"
     else:
         raise AttributeError("Method not allowed.")
 
 # Parameterized routes
@@ -33,14 +41,16 @@
 def handler(req, resp):
     resp.text = "We don't have to use decorators!"
 
 app.add_route("/sample", handler, allowed_methods=["get", "post"])
 
 
 ```
+### Run Server
+> Lumosweb --app <module_name> run
 
 ### Unit Test
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
 that you may want to use when writing unit tests with LumosWeb. The first one is `app` which is an instance of the main `API` class:
 ```python
 def test_basic_route_adding(api):
```

### Comparing `LumosWeb-0.0.9/setup.py` & `LumosWeb-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.9"
+VERSION = "1.0.0"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

