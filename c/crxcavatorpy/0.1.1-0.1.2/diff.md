# Comparing `tmp/crxcavatorpy-0.1.1.tar.gz` & `tmp/crxcavatorpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crxcavatorpy-0.1.1.tar", max compression
+gzip compressed data, was "crxcavatorpy-0.1.2.tar", max compression
```

## Comparing `crxcavatorpy-0.1.1.tar` & `crxcavatorpy-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      120 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/README.md
--rw-r--r--   0        0        0       51 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/crxcavator/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/crxcavator/__main__.py
--rw-r--r--   0        0        0      911 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/crxcavator/api.py
--rw-r--r--   0        0        0      729 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 crxcavatorpy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      120 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/README.md
+-rw-r--r--   0        0        0       51 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/crxcavator/__init__.py
+-rw-r--r--   0        0        0     1643 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/crxcavator/__main__.py
+-rw-r--r--   0        0        0      911 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/crxcavator/api.py
+-rw-r--r--   0        0        0      729 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 crxcavatorpy-0.1.2/PKG-INFO
```

### Comparing `crxcavatorpy-0.1.1/crxcavator/__main__.py` & `crxcavatorpy-0.1.2/crxcavator/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,14 @@
         )
         parser.add_argument(
             "extension_version",
             help="The extension version of the extension",
             type=str
         )
         args = parser.parse_args()
-        reports = api.get_all_reports(
+        reports = api.get_report(
             args.extension_id, args.extension_version)
         print(reports)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `crxcavatorpy-0.1.1/crxcavator/api.py` & `crxcavatorpy-0.1.2/crxcavator/api.py`

 * *Files identical despite different names*

### Comparing `crxcavatorpy-0.1.1/pyproject.toml` & `crxcavatorpy-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crxcavatorpy"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python module for interacting with the Crxcavator api"
 authors = ["Garrett Primm <garrett@alabamacloudsecurity.com>"]
 readme = "README.md"
 packages = [
     { include = "crxcavator" }
 ]
```

### Comparing `crxcavatorpy-0.1.1/PKG-INFO` & `crxcavatorpy-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crxcavatorpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python module for interacting with the Crxcavator api
 Author: Garrett Primm
 Author-email: garrett@alabamacloudsecurity.com
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

