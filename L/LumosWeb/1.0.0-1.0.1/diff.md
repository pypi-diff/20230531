# Comparing `tmp/LumosWeb-1.0.0.tar.gz` & `tmp/LumosWeb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-1.0.0.tar", last modified: Wed May 31 19:57:51 2023, max compression
+gzip compressed data, was "LumosWeb-1.0.1.tar", last modified: Wed May 31 20:54:58 2023, max compression
```

## Comparing `LumosWeb-1.0.0.tar` & `LumosWeb-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 19:57:51.768988 LumosWeb-1.0.0/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 19:57:51.410234 LumosWeb-1.0.0/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.0.0/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4872 2023-05-31 19:49:07.000000 LumosWeb-1.0.0/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      971 2023-05-31 15:15:46.000000 LumosWeb-1.0.0/LumosWeb/cli.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.0.0/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.0.0/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 19:57:51.712358 LumosWeb-1.0.0/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4269 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-31 19:57:50.000000 LumosWeb-1.0.0/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4269 2023-05-31 19:57:51.762984 LumosWeb-1.0.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4098 2023-05-31 19:57:30.000000 LumosWeb-1.0.0/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-31 19:57:51.771209 LumosWeb-1.0.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-05-31 19:55:55.000000 LumosWeb-1.0.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 20:54:58.257871 LumosWeb-1.0.1/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 20:54:57.908526 LumosWeb-1.0.1/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.0.1/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4872 2023-05-31 19:49:07.000000 LumosWeb-1.0.1/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-31 20:54:27.000000 LumosWeb-1.0.1/LumosWeb/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.0.1/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.0.1/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 20:54:58.198842 LumosWeb-1.0.1/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4269 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4269 2023-05-31 20:54:58.250866 LumosWeb-1.0.1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4098 2023-05-31 19:57:30.000000 LumosWeb-1.0.1/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-31 20:54:58.260935 LumosWeb-1.0.1/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-05-31 20:54:53.000000 LumosWeb-1.0.1/setup.py
```

### Comparing `LumosWeb-1.0.0/LumosWeb/api.py` & `LumosWeb-1.0.1/LumosWeb/api.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.0/LumosWeb/cli.py` & `LumosWeb-1.0.1/LumosWeb/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 from LumosWeb.api import API  # Import the API class
 
 
 def main():
     if len(sys.argv) < 4 or sys.argv[1] != "--app":
         print("Usage: Lumosweb --app <module_name> run")
         return
-    
+
     app_module = sys.argv[2]
     app_path = os.path.abspath(os.path.join(os.getcwd(), app_module + ".py"))
-
+    app_directory = os.path.dirname(app_path)
+    
     if os.path.exists(app_path):
+        sys.path.append(app_directory)  # Add app directory to the system path
+        
         with open(app_path, "r") as file:
             code = compile(file.read(), app_path, "exec")
             namespace = {}
             exec(code, namespace)
             app = None
             for obj in namespace.values():
                 if isinstance(obj, API):
```

### Comparing `LumosWeb-1.0.0/LumosWeb/middleware.py` & `LumosWeb-1.0.1/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.0/LumosWeb/response.py` & `LumosWeb-1.0.1/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.0/LumosWeb.egg-info/PKG-INFO` & `LumosWeb-1.0.1/LumosWeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 1.0.0
+Version: 1.0.1
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `LumosWeb-1.0.0/PKG-INFO` & `LumosWeb-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 1.0.0
+Version: 1.0.1
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `LumosWeb-1.0.0/README.md` & `LumosWeb-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.0/setup.py` & `LumosWeb-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

