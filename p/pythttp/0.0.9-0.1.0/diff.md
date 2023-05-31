# Comparing `tmp/pythttp-0.0.9.tar.gz` & `tmp/pythttp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.0.9.tar", last modified: Tue May 30 16:15:22 2023, max compression
+gzip compressed data, was "pythttp-0.1.0.tar", last modified: Wed May 31 11:00:27 2023, max compression
```

## Comparing `pythttp-0.0.9.tar` & `pythttp-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 16:15:22.041201 pythttp-0.0.9/
--rw-rw-rw-   0        0        0     1093 2023-05-30 16:15:22.041201 pythttp-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.9/README.md
--rw-rw-rw-   0        0        0      419 2023-05-30 16:15:20.000000 pythttp-0.0.9/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-30 16:15:22.030090 pythttp-0.0.9/pythttp/
--rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.9/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     6654 2023-05-30 16:14:59.000000 pythttp-0.0.9/pythttp/Protocol.py
--rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.9/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3037 2023-05-30 15:45:28.000000 pythttp-0.0.9/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.9/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:15:22.040201 pythttp-0.0.9/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-05-30 16:15:21.000000 pythttp-0.0.9/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-30 16:15:21.000000 pythttp-0.0.9/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 16:15:21.000000 pythttp-0.0.9/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 16:15:21.000000 pythttp-0.0.9/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 16:15:22.041201 pythttp-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-05-30 16:15:17.000000 pythttp-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:00:27.348911 pythttp-0.1.0/
+-rw-rw-rw-   0        0        0     1093 2023-05-31 11:00:27.348911 pythttp-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.0/README.md
+-rw-rw-rw-   0        0        0      419 2023-05-31 11:00:25.000000 pythttp-0.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-31 11:00:27.327837 pythttp-0.1.0/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.1.0/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     3282 2023-05-31 10:51:06.000000 pythttp-0.1.0/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0     3885 2023-05-31 11:00:03.000000 pythttp-0.1.0/pythttp/RequestHandler.py
+-rw-rw-rw-   0        0        0     2732 2023-05-31 10:59:28.000000 pythttp-0.1.0/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3037 2023-05-30 15:45:28.000000 pythttp-0.1.0/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      139 2023-05-31 09:28:19.000000 pythttp-0.1.0/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:00:27.346906 pythttp-0.1.0/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-05-31 11:00:27.000000 pythttp-0.1.0/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-31 11:00:27.000000 pythttp-0.1.0/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 11:00:27.000000 pythttp-0.1.0/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 11:00:27.000000 pythttp-0.1.0/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 11:00:27.349911 pythttp-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-05-31 11:00:18.000000 pythttp-0.1.0/setup.py
```

### Comparing `pythttp-0.0.9/PKG-INFO` & `pythttp-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.9/README.md` & `pythttp-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.9/pythttp/Log_Manager.py` & `pythttp-0.1.0/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.9/pythttp/Structure.py` & `pythttp-0.1.0/pythttp/Structure.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.9/pythttp/Thread_Manager.py` & `pythttp-0.1.0/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.9/pythttp.egg-info/PKG-INFO` & `pythttp-0.1.0/pythttp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.9/setup.py` & `pythttp-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.0.9",
+    version="0.1.0",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

