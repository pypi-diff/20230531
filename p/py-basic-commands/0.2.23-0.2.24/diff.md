# Comparing `tmp/py_basic_commands-0.2.23.tar.gz` & `tmp/py_basic_commands-0.2.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_basic_commands-0.2.23.tar", last modified: Tue May 30 23:35:12 2023, max compression
+gzip compressed data, was "py_basic_commands-0.2.24.tar", last modified: Wed May 31 00:38:54 2023, max compression
```

## Comparing `py_basic_commands-0.2.23.tar` & `py_basic_commands-0.2.24.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.362952 py_basic_commands-0.2.23/py_basic_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/example_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.362952 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/create_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/create_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/get_src_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/join_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/remove_file_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/write_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/py_basic_commands/fscripts/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/fscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/fscripts/finput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/fscripts/fprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/fscripts/fprint_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/py_basic_commands/json_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/json_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/json_scripts/create_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/json_scripts/read_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/json_scripts/write_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/py_basic_commands/other/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/basic_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/choose_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/function_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.362952 py_basic_commands-0.2.23/py_basic_commands.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-30 23:35:12.000000 py_basic_commands-0.2.23/py_basic_commands.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-30 23:35:12.000000 py_basic_commands-0.2.23/py_basic_commands.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 23:35:12.000000 py_basic_commands-0.2.23/py_basic_commands.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 23:35:12.000000 py_basic_commands-0.2.23/py_basic_commands.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.684094 py_basic_commands-0.2.24/py_basic_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/example_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.688094 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/create_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/create_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/get_src_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/join_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/remove_file_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/write_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.688094 py_basic_commands-0.2.24/py_basic_commands/fscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/fscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/fscripts/finput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/fscripts/fprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/fscripts/fprint_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/py_basic_commands/json_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/json_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/json_scripts/create_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/json_scripts/read_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/json_scripts/write_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/py_basic_commands/other/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/basic_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/choose_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/function_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.688094 py_basic_commands-0.2.24/py_basic_commands.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-31 00:38:54.000000 py_basic_commands-0.2.24/py_basic_commands.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-31 00:38:54.000000 py_basic_commands-0.2.24/py_basic_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:38:54.000000 py_basic_commands-0.2.24/py_basic_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 00:38:54.000000 py_basic_commands-0.2.24/py_basic_commands.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/setup.cfg
```

### Comparing `py_basic_commands-0.2.23/LICENSE.md` & `py_basic_commands-0.2.24/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/PKG-INFO` & `py_basic_commands-0.2.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_basic_commands
-Version: 0.2.23
+Version: 0.2.24
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.23/README.md` & `py_basic_commands-0.2.24/README.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/__init__.py` & `py_basic_commands-0.2.24/py_basic_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/base.py` & `py_basic_commands-0.2.24/py_basic_commands/base.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/__init__.py` & `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/create_dirs.py` & `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/create_dirs.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/create_file.py` & `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/create_file.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/get_src_path.py` & `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/get_src_path.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/join_path.py` & `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/join_path.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/read_file.py` & `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/read_file.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/remove_file_dir.py` & `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/remove_file_dir.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     force:bool = True
 
     def __post_init__(self):
         super().__init__()
 
 
     @try_traceback(print_traceback=True)
-    def __call__(self, do:str, do_path:str, force:bool=False, do_print:bool=True) -> bool:
+    def __call__(self, do:str, do_path:str, force:bool=None, do_print:bool=None) -> bool:
         """Remove a file or directory at the specified path.
         
         Parameters:
         - `do` (str): Whether to remove a `'d'`irectory or a `'f'`ile.
         - `do_path` (str): The path to the file or directory to remove.
         - `force` (bool): Whether to force the removal of the file or directory.
         - `do_print` (bool): Whether to print information about the file or directory removal process.
@@ -29,14 +29,16 @@
         - `bool`: Whether the file or directory was removed.
         """
 
         # Check input values
         force    = self._check_input_val(force, self.force)
         do_print = self._check_input_val(do_print, self.do_print)
 
+        fprint.config(do_print=do_print)
+
         if do == 'd': # Directory
             try:
                 dir_content = listdir(do_path)
             except FileNotFoundError:
                 fprint(f'Directory path not found: {do_path}')
                 return False
             except NotADirectoryError:
```

### Comparing `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/write_file.py` & `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/write_file.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/fscripts/finput.py` & `py_basic_commands-0.2.24/py_basic_commands/fscripts/finput.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/fscripts/fprint.py` & `py_basic_commands-0.2.24/py_basic_commands/fscripts/fprint.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/fscripts/fprint_array.py` & `py_basic_commands-0.2.24/py_basic_commands/fscripts/fprint_array.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/json_scripts/create_json.py` & `py_basic_commands-0.2.24/py_basic_commands/json_scripts/create_json.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/json_scripts/read_json.py` & `py_basic_commands-0.2.24/py_basic_commands/json_scripts/read_json.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/json_scripts/write_json.py` & `py_basic_commands-0.2.24/py_basic_commands/json_scripts/write_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         - `do_print` (bool): Whether to print information about the data writing process. Default is `True`.
 
         Return:
         - `bool`: Whether the file was created.
         """
 
         # Check input values
-        indent = self._check_input_val(indent, self._indent)
-        force = self._check_input_val(force, self._force)
+        indent = self._check_input_val(indent, self.indent)
+        force = self._check_input_val(force, self.force)
         do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         try:
             if data.__class__.__name__ == ('str'):
                 data = json.loads(data)
```

### Comparing `py_basic_commands-0.2.23/py_basic_commands/other/basic_commands.py` & `py_basic_commands-0.2.24/py_basic_commands/other/basic_commands.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/other/choose_from_list.py` & `py_basic_commands-0.2.24/py_basic_commands/other/choose_from_list.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/other/function_timer.py` & `py_basic_commands-0.2.24/py_basic_commands/other/function_timer.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands/other/timer.py` & `py_basic_commands-0.2.24/py_basic_commands/other/timer.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/py_basic_commands.egg-info/PKG-INFO` & `py_basic_commands-0.2.24/py_basic_commands.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-basic-commands
-Version: 0.2.23
+Version: 0.2.24
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.23/py_basic_commands.egg-info/SOURCES.txt` & `py_basic_commands-0.2.24/py_basic_commands.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.23/pyproject.toml` & `py_basic_commands-0.2.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_basic_commands"
-version = "0.2.23"
+version = "0.2.24"
 authors = [
   { name="Rasmus Ohert", email="rassemichael@gmail.com" },
 ]
 description = "Basic tools for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py_basic_commands-0.2.23/setup.cfg` & `py_basic_commands-0.2.24/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py_basic_commands
-version = 0.2.23
+version = 0.2.24
 author = Rasmus Ohert
 author_email = rassemichael@gmail.com
 description = Basic tools for Python
 long_description = A package that has some basic tools for your basic Python needs
 url = https://github.com/RasseTheBoy/Py_Basic_Commands
 keywords = python, tool, help
 classifiers =
```

