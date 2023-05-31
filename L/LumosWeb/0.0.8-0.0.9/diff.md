# Comparing `tmp/LumosWeb-0.0.8.tar.gz` & `tmp/LumosWeb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-0.0.8.tar", last modified: Tue May 30 11:43:55 2023, max compression
+gzip compressed data, was "LumosWeb-0.0.9.tar", last modified: Tue May 30 11:48:13 2023, max compression
```

## Comparing `LumosWeb-0.0.8.tar` & `LumosWeb-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:43:55.424037 LumosWeb-0.0.8/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:43:55.041694 LumosWeb-0.0.8/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.8/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4163 2023-05-30 11:21:23.000000 LumosWeb-0.0.8/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      596 2023-05-30 11:39:42.000000 LumosWeb-0.0.8/LumosWeb/cli.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.8/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.8/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:43:55.363523 LumosWeb-0.0.8/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:43:54.000000 LumosWeb-0.0.8/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-05-30 11:43:54.000000 LumosWeb-0.0.8/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-30 11:43:54.000000 LumosWeb-0.0.8/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-05-30 11:43:54.000000 LumosWeb-0.0.8/LumosWeb.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-30 11:43:54.000000 LumosWeb-0.0.8/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-30 11:43:54.000000 LumosWeb-0.0.8/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:43:55.417036 LumosWeb-0.0.8/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3760 2023-05-29 14:14:31.000000 LumosWeb-0.0.8/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-30 11:43:55.427670 LumosWeb-0.0.8/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-05-30 11:42:06.000000 LumosWeb-0.0.8/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:48:13.007133 LumosWeb-0.0.9/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:48:12.648828 LumosWeb-0.0.9/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.9/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4729 2023-05-30 11:47:49.000000 LumosWeb-0.0.9/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      596 2023-05-30 11:39:42.000000 LumosWeb-0.0.9/LumosWeb/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.9/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.9/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:48:12.943995 LumosWeb-0.0.9/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-05-30 11:48:12.000000 LumosWeb-0.0.9/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-30 11:48:11.000000 LumosWeb-0.0.9/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:48:12.999585 LumosWeb-0.0.9/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3760 2023-05-29 14:14:31.000000 LumosWeb-0.0.9/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-30 11:48:13.009900 LumosWeb-0.0.9/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-05-30 11:48:07.000000 LumosWeb-0.0.9/setup.py
```

### Comparing `LumosWeb-0.0.8/LumosWeb/api.py` & `LumosWeb-0.0.9/LumosWeb/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from requests import Session as RequestsSession
 from wsgiadapter import WSGIAdapter as RequestsWSGIAdapter
 import os
 from jinja2 import Environment, FileSystemLoader
 from whitenoise import WhiteNoise
 from .middleware import Middleware
 from .response import Response
-import sys
-import importlib
-from http.server import HTTPServer, SimpleHTTPRequestHandler
+import http.server
+import socketserver
 
 class API:
     def __init__(self, templates_dir="templates", static_dir="static"):
         self.routes = {}  # dictionary of routes and handlers, path as keys and handlers as values
 
         self.templates_env = Environment(
             loader = FileSystemLoader(os.path.abspath(templates_dir))
@@ -103,7 +102,24 @@
         return self.templates_env.get_template(template_name).render(**context)
     
     def add_exception_handler(self, exception_handler):
         self.exception_handler = exception_handler
 
     def add_middleware(self, middleware_cls):
         self.middleware.add(middleware_cls)
+
+    def run_server(self):
+        # Assuming you have defined your app instance and configurations
+        app = self.create_app()
+        host = '127.0.0.1'
+        port = 8000
+
+        # Create a simple HTTP server and assign it to the specified host and port
+        server_address = (host, port)
+        httpd = socketserver.TCPServer(server_address, http.server.SimpleHTTPRequestHandler)
+
+        # Set the app as the server's request handler
+        httpd.set_app(app)
+
+        # Start the server
+        print(f"Serving Lumos app on http://{host}:{port} (Press CTRL+C to quit)")
+        httpd.serve_forever()
```

### Comparing `LumosWeb-0.0.8/LumosWeb/cli.py` & `LumosWeb-0.0.9/LumosWeb/cli.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.8/LumosWeb/middleware.py` & `LumosWeb-0.0.9/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.8/LumosWeb/response.py` & `LumosWeb-0.0.9/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.8/LumosWeb.egg-info/PKG-INFO` & `LumosWeb-0.0.9/LumosWeb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.8
+Version: 0.0.9
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `LumosWeb-0.0.8/PKG-INFO` & `LumosWeb-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.8
+Version: 0.0.9
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `LumosWeb-0.0.8/README.md` & `LumosWeb-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.8/setup.py` & `LumosWeb-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

