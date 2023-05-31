# Comparing `tmp/lingfo-0.2.2.tar.gz` & `tmp/lingfo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingfo-0.2.2.tar", last modified: Sat May 20 12:55:56 2023, max compression
+gzip compressed data, was "lingfo-0.2.3.tar", last modified: Wed May 31 13:33:59 2023, max compression
```

## Comparing `lingfo-0.2.2.tar` & `lingfo-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:56.635362 lingfo-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 12:55:33.000000 lingfo-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 12:55:56.635362 lingfo-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-20 12:55:33.000000 lingfo-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-20 12:55:56.635362 lingfo-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:56.623361 lingfo-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:56.627362 lingfo-0.2.2/src/lingfo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:56.631362 lingfo-0.2.2/src/lingfo/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/cache/cache_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/cache/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:56.631362 lingfo-0.2.2/src/lingfo/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/config/auto_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/config/extends.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/one_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:56.631362 lingfo-0.2.2/src/lingfo/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/scripts/git_init.ps1
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/scripts/git_init.sh
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:56.635362 lingfo-0.2.2/src/lingfo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/utils/find_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/utils/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-20 12:55:33.000000 lingfo-0.2.2/src/lingfo/utils/verbose_print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:56.631362 lingfo-0.2.2/src/lingfo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 12:55:56.000000 lingfo-0.2.2/src/lingfo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-20 12:55:56.000000 lingfo-0.2.2/src/lingfo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:55:56.000000 lingfo-0.2.2/src/lingfo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-20 12:55:56.000000 lingfo-0.2.2/src/lingfo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:55:56.635362 lingfo-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-20 12:55:33.000000 lingfo-0.2.2/tests/test_execute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:59.079447 lingfo-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-31 13:33:41.000000 lingfo-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-31 13:33:59.079447 lingfo-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-31 13:33:41.000000 lingfo-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-31 13:33:59.079447 lingfo-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:59.071447 lingfo-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:59.075447 lingfo-0.2.3/src/lingfo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:59.075447 lingfo-0.2.3/src/lingfo/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/cache/cache_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/cache/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:59.075447 lingfo-0.2.3/src/lingfo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/config/auto_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/config/extends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/one_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:59.079447 lingfo-0.2.3/src/lingfo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/utils/find_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/utils/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-31 13:33:41.000000 lingfo-0.2.3/src/lingfo/utils/verbose_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:59.075447 lingfo-0.2.3/src/lingfo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-31 13:33:59.000000 lingfo-0.2.3/src/lingfo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 13:33:59.000000 lingfo-0.2.3/src/lingfo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:33:59.000000 lingfo-0.2.3/src/lingfo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 13:33:59.000000 lingfo-0.2.3/src/lingfo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:33:59.079447 lingfo-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-31 13:33:41.000000 lingfo-0.2.3/tests/test_execute.py
```

### Comparing `lingfo-0.2.2/LICENSE` & `lingfo-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lingfo-0.2.2/src/lingfo/cache/main.py` & `lingfo-0.2.3/src/lingfo/cache/main.py`

 * *Files identical despite different names*

### Comparing `lingfo-0.2.2/src/lingfo/config/extends.py` & `lingfo-0.2.3/src/lingfo/config/extends.py`

 * *Files identical despite different names*

### Comparing `lingfo-0.2.2/src/lingfo/execute.py` & `lingfo-0.2.3/src/lingfo/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import configparser
 import inspect
 import re
 import shlex
 import subprocess
 import sys
 
+from random import choices
+from string import ascii_lowercase
+
 from dataclasses import dataclass
 from os import remove
 from os.path import isfile
 from rich import print as rich_print
 
 from .cache.main import Cache
 from .stores import ONE_COMPILE
@@ -38,14 +41,15 @@
 
 @dataclass
 class TranslateData:
     import_syntax: str
     file_name: str
     call_function: str
     args: str
+    is_class: bool
 
 
 class MultipleExecute:
     def __init__(self, name: str = "default") -> None:
         if config.getboolean("launch", "multiple_functions") is False:
             rich_print(
                 "[bold red]lingfo[/bold red]   running multiple_functions mode when \
@@ -87,15 +91,15 @@
 
     def launch(self):
         """launch functions"""
 
         file = self._open_file()
         lines = file.readlines()
 
-        execute = Execute(None, None, None, use_multiple_execute=True)
+        execute = Execute(None, None, None, use_multiple_execute=True, class_name="")
 
         # get import syntax from config (TODO: its already defined somewhere else)
         if config.getboolean("main", "use_templates") is True:
             import_syntax = lingfocache.TEMPLATE_IMPORT_SYNTAX
             temp_file = lingfocache.TEMPLATE_TEMP_FILE
         else:
             import_syntax = launch_config["import_syntax"]
@@ -116,29 +120,30 @@
 
             # TODO: add support for languages without semicolon
 
             functions += str(function)
         file.close()
 
         # translate it
-        data = TranslateData(import_syntax, file_split, functions, args)
+        data = TranslateData(import_syntax, file_split, functions, args, is_class=False)
         output = execute.translate(
             data,
             temp_file,
         )
 
         # execute it
         execute.function("", output=output)
 
         # remove temp file
         remove(f".lingfo/multiple-execute-{self.state_name}.txt")
 
     def __exit__(self, *args_function):
         self.launch()
 
+
 class Execute:
     """executes function"""
 
     def translate(self, data: TranslateData, temp_file=""):
         """translates string (multiple replace)"""
 
         if temp_file != "":
@@ -150,36 +155,67 @@
             if len(args_list) >= 1:
                 args = args_list[0]
             else:
                 args = ""
         else:
             args = ""
 
-
         translate_data_temp = {
             "$LINGFO_ARGS": args,
         }
 
+        translate_utils = {
+            "$LINGFO_SEMICOLON": ";",
+            "$LINGFO_FUNCTION": data.call_function,
+        }
+
+        class_call_translate = {}
+
+        if data.is_class:
+            # prepare translate data
+            class_call_translate = {
+                "$LINGFO_RANDOM": "".join(choices(ascii_lowercase, k=3)),
+                "$LINGFO_CLASS": self.class_name,
+            }
+
+            class_call_translate = {**class_call_translate, **translate_utils}
+
         translate_data = {
             "$LINGFO_IMPORT": data.import_syntax.replace("[file-name]", data.file_name),
-            "$LINGFO_FUNCTION": data.call_function,
-            "$LINGFO_SEMICOLON": ";",
             "$LINGFO_NEWLINE": "\n",
             "$LINGFO_ARGS": "",
         }
 
+        translate_data = {**translate_data, **translate_utils}
+
+        if data.is_class:
+            # translate it
+            translate_data = {**class_call_translate, **translate_data}
+            function_class = config["launch"]["class_call_syntax"]
+
+            for i, j in {**translate_data, **translate_data_temp}.items():
+                function_class = function_class.replace(i, j)
+
+            # and then combine translate data and output of this translate process
+            new_translate_data = {"$LINGFO_FUNCTION": function_class}
+            translate_data = {**translate_data, **new_translate_data}
+
         for i, j in {**translate_data, **translate_data_temp}.items():
             self.temp_file = self.temp_file.replace(i, j)
 
         return self.temp_file
 
-    def __init__(self, file, uuid, *args, use_multiple_execute=False) -> None:
+    def __init__(
+        self, file, uuid, is_class, class_name, *args, use_multiple_execute=False
+    ) -> None:
         self.temp_file = ""
         self.init_args = INIT_ARGS
         self.temp_file = TEMP_FILE
+        self.is_class = is_class
+        self.class_name = class_name
 
         if use_multiple_execute is True:
             return
 
         # get from what function was this called
         if lingfocache.CUSTOM_TEMP_FILE is None:
             call_function = inspect.stack()[1].function
@@ -192,19 +228,14 @@
         )
 
         self.init_args = re.sub("[()]", "", rf"{args}".replace(",", ""))
         if config.getboolean("main", "use_templates") is True:
             import_syntax = lingfocache.TEMPLATE_IMPORT_SYNTAX
         else:
             import_syntax = launch_config["import_syntax"]
-        file_name = main_config["lib_path"].split("/")[-1]
-        if main_config["lib_path"][-1] == "*":
-            # user selected multiple files
-            file_name = main_config["lib_path"].replace("*", file)
-            file_name = file_name.split("/")[-1]
 
         if config.getboolean("main", "use_templates") is True:
             self.temp_file = lingfocache.TEMPLATE_TEMP_FILE
         else:
             self.temp_file = config["temp_file"]["temp_file"]
 
         if ONE_COMPILE:
@@ -220,15 +251,19 @@
                 .replace("$LINGFO_SEMICOLON", "")
                 .replace("}", "")
             )
 
             if after == "()":
                 self.temp_file = self.temp_file.replace("($LINGFO_ARGS)", "")
 
-        data = TranslateData(import_syntax, file_name, call_function, self.init_args)
+        lib_path_first = config["main"]["lib_path"].split("/")[0]
+        new_file = file.replace(f"{lib_path_first}/", "")
+        data = TranslateData(
+            import_syntax, new_file, call_function, self.init_args, self.is_class
+        )
         self.translate(data)
 
         if config.getboolean("launch", "multiple_functions") is True:
             multiple_execute = MultipleExecute()
             multiple_execute.save("function", call_function, file, self.init_args)
         else:
             self.function(uuid)
```

### Comparing `lingfo-0.2.2/src/lingfo/main.py` & `lingfo-0.2.3/src/lingfo/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from os.path import isfile
 
 from git import Repo
 from rich import print as rich_print
 
 from .cache.main import Cache
 from .config import extends
-from .git import GitTracking
 from .index import find
 from .utils.verbose_print import verbose_print
 
 config = configparser.ConfigParser()
 config.read("lingfo.conf")
 
 
@@ -113,13 +112,12 @@
         verbose_print("[bold green]lingfo[/bold green]   checking lingfo config ")
 
         # cleaner way to run multiple functions
         functions = [
             Cache,
             self._check_config,
             self._extend_check,
-            GitTracking,
         ]
         for f in functions:
             f()
 
         find()
```

### Comparing `lingfo-0.2.2/src/lingfo/one_compile.py` & `lingfo-0.2.3/src/lingfo/one_compile.py`

 * *Files identical despite different names*

### Comparing `lingfo-0.2.2/src/lingfo/utils/variables.py` & `lingfo-0.2.3/src/lingfo/utils/variables.py`

 * *Files identical despite different names*

### Comparing `lingfo-0.2.2/src/lingfo/utils/verbose_print.py` & `lingfo-0.2.3/src/lingfo/utils/verbose_print.py`

 * *Files identical despite different names*

### Comparing `lingfo-0.2.2/src/lingfo.egg-info/SOURCES.txt` & `lingfo-0.2.3/src/lingfo.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 LICENSE
 pyproject.toml
 setup.cfg
 src/lingfo/__init__.py
 src/lingfo/execute.py
-src/lingfo/git.py
 src/lingfo/index.py
 src/lingfo/main.py
 src/lingfo/one_compile.py
 src/lingfo/stores.py
 src/lingfo.egg-info/PKG-INFO
 src/lingfo.egg-info/SOURCES.txt
 src/lingfo.egg-info/dependency_links.txt
 src/lingfo.egg-info/top_level.txt
 src/lingfo/cache/__init__.py
 src/lingfo/cache/cache_template.py
 src/lingfo/cache/main.py
 src/lingfo/config/__init__.py
 src/lingfo/config/auto_detect.py
 src/lingfo/config/extends.py
-src/lingfo/scripts/git_init.ps1
-src/lingfo/scripts/git_init.sh
 src/lingfo/utils/__init__.py
 src/lingfo/utils/find_dict.py
 src/lingfo/utils/variables.py
 src/lingfo/utils/verbose_print.py
 tests/test_execute.py
```

### Comparing `lingfo-0.2.2/tests/test_execute.py` & `lingfo-0.2.3/tests/test_execute.py`

 * *Files identical despite different names*

