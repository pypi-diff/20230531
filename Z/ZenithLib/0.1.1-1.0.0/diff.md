# Comparing `tmp/zenithlib-0.1.1.tar.gz` & `tmp/zenithlib-1.0.0.tar.gz`

## Comparing `zenithlib-0.1.1.tar` & `zenithlib-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,49 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.1.1/.gitattributes
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/Builder.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/Stylesheet.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/Web.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/__init__.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/ZenithLang.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/langAST.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/langParser.py
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/langTranspiler.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/__testing__/out.html
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/src/tests.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 zenithlib-0.1.1/docs/README.md
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 zenithlib-0.1.1/docs/STYLESHEETS.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 zenithlib-0.1.1/examples/server.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.1.1/scripts/bupload.sh
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.1.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.1.1/LICENSE
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 zenithlib-0.1.1/README.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 zenithlib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 zenithlib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.gitattributes
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 zenithlib-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Code_of_Conduct.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 zenithlib-1.0.0/SECURITY.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/Builder.py
+-rw-r--r--   0        0        0    14953 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/Stylesheet.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/Web.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/__init__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/ZenithLang.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/__init__.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/langAST.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/langParser.py
+-rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/langTranspiler.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/__testing__/out.html
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/src/tests.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Customs/MaterialButton.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Customs/MaterialSlider.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Customs/ZenithDecorator.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Packages/multiport.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Plugins/ToElectron.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Plugins/bugRenderer.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/ATTRIBUTES.md
+-rw-r--r--   0        0        0    14467 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/ELEMENTS.md
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/README.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/STYLESHEETS.md
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/api-reference.md
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/configuration.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/contributing.md
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/getting-started.md
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/installation.md
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/routing.md
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/usage.md
+-rw-r--r--   0        0        0   205818 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/images/Upscaled-Zenith.png
+-rw-r--r--   0        0        0   205818 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/images/Zenith.png
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 zenithlib-1.0.0/examples/server.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-1.0.0/scripts/bupload.sh
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zenithlib-1.0.0/scripts/placeholder.sh
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 zenithlib-1.0.0/README.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 zenithlib-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 zenithlib-1.0.0/PKG-INFO
```

### Comparing `zenithlib-0.1.1/Zenith/Builder.py` & `zenithlib-1.0.0/Zenith/Builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,15 +18,14 @@
             NAME = BUILD_ROUTE
             BUILD_PRE_BUILD_CONTENT = self.routes[BUILD_ROUTE]
             
             tokens = langParser.parse_string(BUILD_PRE_BUILD_CONTENT)
             ast = langAST.build_ast(tokens)
             transpiled = langTranspiler.transpile_to_html(ast)
             
-            print(transpiled)
             NEW_BUILDER_BUILT[NAME] = f"""{transpiled}"""
             
             return NEW_BUILDER_BUILT
             
     def getRoutes(self):
         ROUTES = []
         for ROUTE in self.routes:
```

### Comparing `zenithlib-0.1.1/Zenith/Web.py` & `zenithlib-1.0.0/Zenith/Web.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import datetime
 from http.server import BaseHTTPRequestHandler, HTTPServer
 
 class CustomServer(BaseHTTPRequestHandler):
+    
     HEADER_VALUE = "text/html"
     HEADER_TYPE = "Content-type"
     BUILT_ROUTES = {}
 
     def do_GET(self):
         self.send_response(200)
         self.send_header(self.HEADER_TYPE, self.HEADER_VALUE)
         self.end_headers()
 
         path = self.path[1:]  # Remove the leading '/' from the path
+        if path == "":
+            path = "/"  # Set the path to "/" for the home route
         if path in self.BUILT_ROUTES:
             response = self.BUILT_ROUTES[path]
             self.wfile.write(response.encode('utf-8'))
         else:
             self.send_response(404)
             self.wfile.write(b"<h1>404 Not Found</h1>")
 
+
 class WApp:
+    INITAL_ROUTE = "/"
     def __init__(self):
         self.port = 3000
         self.host = 'localhost'
         self.devServer = False
         self.static_url_path = "static"
         self.name = "Zenith App"
         self.logging = True
```

### Comparing `zenithlib-0.1.1/Zenith/lang/langAST.py` & `zenithlib-1.0.0/Zenith/lang/langAST.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,17 +25,21 @@
             # Handle open tags
             tag_parts = token[1:-1].split()
             tag_name = tag_parts.pop(0)
             node = ASTNode(tag_name)
 
             # Handle attributes
             for part in tag_parts:
-                attr_name, attr_value = part.split("=")
-                attr_value = attr_value.strip('"')
-                node.set_attribute(attr_name, attr_value)
+                if "=" in part:
+                    attr_name, attr_value = part.split("=")
+                    attr_value = attr_value.strip('"')
+                    node.set_attribute(attr_name, attr_value)
+                else:
+                    attr_name = part
+                    node.set_attribute(attr_name, "")
 
             if stack:
                 parent_node = stack[-1]
                 parent_node.add_child(node)
             else:
                 root = node
 
@@ -46,14 +50,15 @@
         else:
             # Handle text content
             node = stack[-1]
             node.set_content(token)
 
     return root
 
+
 def print_ast(node, indent=""):
     print(f"{indent}<{node.tag_name}>")
 
     for attr_name, attr_value in node.attributes.items():
         print(f"{indent}  - {attr_name}: {attr_value}")
 
     if node.content:
```

### Comparing `zenithlib-0.1.1/Zenith/lang/langTranspiler.py` & `zenithlib-1.0.0/Zenith/lang/langTranspiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 def transpile_to_html(node):
     casing_dict = {
+        "Title": "title",
         "Container": "div",
         "Header": "h1",
         "Block": "div",
         "Button": "button",
         "Paragraph": "p",
         "Span": "span",
         "Image": "img",
@@ -146,41 +147,34 @@
     for child_node in node.children:
         result += transpile_to_html(child_node)
 
     result += close_tag(casing_dict.get(node.tag_name, "div"))
 
     return result
 
-
 def open_tag(tag_name, attributes):
     result = f"<{tag_name}"
 
     for attr_name, attr_value in attributes.items():
         attr_name = transpile_attribute_name(attr_name)
         result += f' {attr_name}="{attr_value}"'
 
     result += ">"
 
     return result
 
-
 def process_content(content):
     return content or ""
-
-
 def close_tag(tag_name):
     return f"</{tag_name}>"
 
-
-
-
 def transpile_attribute_name(attribute_name):
     attribute_mapping = {
         "idName": "id",
-        "classType": "class",
+        "className": "class",
         "dataValue": "data-value",
         "hrefLink": "href",
         "srcUrl": "src",
         "altText": "alt",
         "forElement": "for",
         "ariaLabel": "aria-label",
         "ariaHidden": "aria-hidden",
```

### Comparing `zenithlib-0.1.1/.gitignore` & `zenithlib-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zenithlib-0.1.1/LICENSE` & `zenithlib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zenithlib-0.1.1/pyproject.toml` & `zenithlib-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ZenithLib"
-version = "0.1.1"
+version = "1.0.0"
 authors = [
   { name="Ryan Rudd", email="rsrudd@gmail.com" },
 ]
 description = "Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zenithlib-0.1.1/PKG-INFO` & `zenithlib-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: ZenithLib
-Version: 0.1.1
+Version: 1.0.0
 Summary: Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites.
 Project-URL: Homepage, https://github.com/Ryan-Rudd/Zenith
 Project-URL: Bug Tracker, https://github.com/Ryan-Rudd/Zenith/issues
 Author-email: Ryan Rudd <rsrudd@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+
+<p align="center">
+<img src="./docs/images/Upscaled-Zenith.png" style="align: center; width: 150px; text-align: center; display: flex;">
+</p><br>
+
 # Zenith
 ![Python Version](https://img.shields.io/badge/Python-3.8-brightgreen.svg)
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
 ![PyPI Version](https://img.shields.io/pypi/v/ZenithLib)
 ![Downloads](https://img.shields.io/pypi/dm/ZenithLib)
 ![GitHub Issues](https://img.shields.io/github/issues/Ryan-Rudd/Zenith)
 ![GitHub Pull Requests](https://img.shields.io/github/issues-pr/Ryan-Rudd/Zenith)
 
-
-
 Zenith is a powerful Python framework that revolutionizes web development. It provides a declarative approach to designing efficient UI components, making it easier than ever to build interactive and scalable websites.
 
 ## Features
 
 - **Efficient UI components**: Zenith makes it easy to build and manage reusable UI components.
 - **Scalable**: Designed with large-scale applications in mind, Zenith helps you build websites that can grow with your needs.
 - **Declarative**: Zenith's declarative style makes your code easier to understand and maintain.
@@ -47,25 +50,41 @@
 ```python
 import Zenith
 
 app = Zenith.WApp()
 
 homePageContent = """
     <Container>
-        <Header idName="header">Hello world from Zenith</Header>
+        <Header>Welcome to Zenith</Header>
+        <Paragraph>A Python framework for web development</Paragraph>
     </Container>
 """
 
 builder = Zenith.Builder({"home": homePageContent})
 built = builder.Build()
 
-for route in builder.getRoutes():
-    app.register_route(f'{route}', built[route])
+style = Zenith.Stylesheet.new({
+    'body': {
+        'background-color': '#f8f9fa',
+        'font-family': 'Arial, sans-serif',
+    },
+    'h1': {
+        'color': '#007BFF',
+        'font-size': '32px',
+    },
+    'p': {
+        'color': '#6c757d',
+        'font-size': '16px',
+    },
+})
 
+style.apply(built, "home")
+app.register_route('/', built['home'])
 app.serve()
+
 ```
 
 # Documentation
 
 For more detailed information on using Zenith, please refer to our [documentation](/docs).
 
 # Contributing
```

