# Comparing `tmp/BatchParse-0.0.2.tar.gz` & `tmp/BatchParse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BatchParse-0.0.2.tar", last modified: Tue May 30 00:32:39 2023, max compression
+gzip compressed data, was "BatchParse-0.0.3.tar", last modified: Wed May 31 00:06:23 2023, max compression
```

## Comparing `BatchParse-0.0.2.tar` & `BatchParse-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/BatchParse/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/BatchParse/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/util/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/util/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/util/splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/BatchParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 00:32:21.000000 BatchParse-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 00:32:39.471039 BatchParse-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 00:32:21.000000 BatchParse-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:32:39.471039 BatchParse-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 00:32:21.000000 BatchParse-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-30 00:32:21.000000 BatchParse-0.0.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.729117 BatchParse-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.725117 BatchParse-0.0.3/BatchParse/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.725117 BatchParse-0.0.3/BatchParse/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/util/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/util/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-31 00:06:09.000000 BatchParse-0.0.3/BatchParse/util/splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.725117 BatchParse-0.0.3/BatchParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 00:06:23.000000 BatchParse-0.0.3/BatchParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 00:06:09.000000 BatchParse-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 00:06:23.729117 BatchParse-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 00:06:09.000000 BatchParse-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:06:23.729117 BatchParse-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-31 00:06:09.000000 BatchParse-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:23.725117 BatchParse-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-31 00:06:09.000000 BatchParse-0.0.3/test/test.py
```

### Comparing `BatchParse-0.0.2/BatchParse/main.py` & `BatchParse-0.0.3/BatchParse/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,36 +21,45 @@
 else:
     logging.basicConfig(
         level=logging.INFO, format="%(message)s", datefmt="[%X]", handlers=[handler]
     )
 logger = logging.getLogger("rich")
 
 
-def parse(code: str, bsplit_and: bool = True, bsplit_carrot: bool = True) -> list:
+def parse(
+    code: str,
+    bsplit_and: bool = True,
+    bsplit_carrot: bool = True,
+    bsplit_script_block: bool = True,
+) -> list:
     """Parse initial Batch Code
 
     Args:
         code (str): Inital Batch Code to Parse
 
     Returns:
         list: Returns Parsed Batch Code as an Array
     """
     code_to_array = code.split("\n")
 
-    initial_split_methods = {
-        bsplit_and: parse_and,
-        bsplit_carrot: parse_carrot,
-    }
-
-    # if split_and:
-    #    code_to_array = parse_and(code_to_array)
-
-    for method in initial_split_methods:
-        if method:
-            code_to_array = initial_split_methods[method](code_to_array)
+    functions = [
+        parse_and,
+        parse_carrot,
+        parse_script_block,
+    ]
+
+    bool_parse = [
+        bsplit_and,
+        bsplit_carrot,
+        bsplit_script_block,
+    ]
+
+    for function in track(functions, description="Splitting Batch Code..."):
+        if bool_parse[functions.index(function)]:
+            code_to_array = function(code_to_array)
 
     parsed_code = []
 
     allowed_methods = Settings.allowed_methods
 
     ignorable_lines = Settings.ignorable_lines
```

### Comparing `BatchParse-0.0.2/BatchParse/util/info.py` & `BatchParse-0.0.3/BatchParse/util/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
     Args:
         line (str): Line of Batch Code
 
     Returns:
         str: Returns the Method of the Batch Code
     """
-    return line.split(" ")[0]
+    out = line.split(" ")[0]
+    if not out.startswith(":"):
+        return out
+    else:
+        return "label: " + out[1:]
 
 
 def get_args(line: str) -> str:
     """Get's the Arguments from a line of Batch Code
 
     Args:
         line (str): Line of Batch Code
```

### Comparing `BatchParse-0.0.2/LICENSE` & `BatchParse-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.2/setup.py` & `BatchParse-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "A Batch Parser"
 LONG_DESCRIPTION = "Easy Way to Parse Batch Code in Python"
 
 setup(
     name="BatchParse",
     version=VERSION,
     description=DESCRIPTION,
```

