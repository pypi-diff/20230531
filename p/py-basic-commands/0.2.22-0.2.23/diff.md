# Comparing `tmp/py_basic_commands-0.2.22.tar.gz` & `tmp/py_basic_commands-0.2.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_basic_commands-0.2.22.tar", last modified: Sat May  6 01:15:31 2023, max compression
+gzip compressed data, was "py_basic_commands-0.2.23.tar", last modified: Tue May 30 23:35:12 2023, max compression
```

## Comparing `py_basic_commands-0.2.22.tar` & `py_basic_commands-0.2.23.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.703888 py_basic_commands-0.2.22/py_basic_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/example_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/create_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/create_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/get_src_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/join_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/remove_file_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/write_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/py_basic_commands/fscripts/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/fscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/fscripts/finput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/fscripts/fprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/fscripts/fprint_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/py_basic_commands/json_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/json_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/json_scripts/create_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/json_scripts/read_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/json_scripts/write_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/py_basic_commands/other/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/basic_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/choose_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/function_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.703888 py_basic_commands-0.2.22/py_basic_commands.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 01:15:31.000000 py_basic_commands-0.2.22/py_basic_commands.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-06 01:15:31.000000 py_basic_commands-0.2.22/py_basic_commands.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:15:31.000000 py_basic_commands-0.2.22/py_basic_commands.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 01:15:31.000000 py_basic_commands-0.2.22/py_basic_commands.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.362952 py_basic_commands-0.2.23/py_basic_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/example_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.362952 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/create_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/create_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/get_src_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/join_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/remove_file_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/write_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/py_basic_commands/fscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/fscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/fscripts/finput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/fscripts/fprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/fscripts/fprint_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/py_basic_commands/json_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/json_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/json_scripts/create_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/json_scripts/read_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/json_scripts/write_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/py_basic_commands/other/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/basic_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/choose_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/function_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/py_basic_commands/other/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:35:12.362952 py_basic_commands-0.2.23/py_basic_commands.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-30 23:35:12.000000 py_basic_commands-0.2.23/py_basic_commands.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-30 23:35:12.000000 py_basic_commands-0.2.23/py_basic_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 23:35:12.000000 py_basic_commands-0.2.23/py_basic_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 23:35:12.000000 py_basic_commands-0.2.23/py_basic_commands.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-30 23:35:01.000000 py_basic_commands-0.2.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-30 23:35:12.366952 py_basic_commands-0.2.23/setup.cfg
```

### Comparing `py_basic_commands-0.2.22/LICENSE.md` & `py_basic_commands-0.2.23/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/PKG-INFO` & `py_basic_commands-0.2.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_basic_commands
-Version: 0.2.22
+Version: 0.2.23
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.22/README.md` & `py_basic_commands-0.2.23/README.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/py_basic_commands/__init__.py` & `py_basic_commands-0.2.23/py_basic_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/py_basic_commands/base.py` & `py_basic_commands-0.2.23/py_basic_commands/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
     
     def config(self, **kwargs):
         """Configure variables"""
         for key, value in kwargs.items():
             if hasattr(self, key):
                 setattr(self, key, value)
-                print(f'Changed {key} to {value}')
             else:
                 raise AttributeError(f'{self.__class__.__name__} has no attribute {key}')
         
 
     def _check_input_val(self, inpt_val, saved_val):
         """Check if input value is None, if so return saved value"""
         return saved_val if inpt_val == None else inpt_val
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/__init__.py` & `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/create_dirs.py` & `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/create_dirs.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/create_file.py` & `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/create_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from py_basic_commands.fscripts   import fprint
 from os.path   import exists
 from py_basic_commands.base   import Base
 
 
 @dataclass
 class CreateFile(Base):
-    _force:bool = False
+    force:bool = False
 
     def __post_init__(self):
         super().__init__()
 
 
     def _create_empty_file(self, dst_path:str) -> bool:
         """Create an empty file at the specified path.
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/get_src_path.py` & `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/get_src_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from py_basic_commands.fscripts   import fprint
 from os.path    import dirname, basename, splitext
 from typing     import Any
 from py_basic_commands.base   import Base
 
 @dataclass
 class GetSourcePath(Base):
-    _ret_val:bool = 'a'
+    ret_val:bool = 'a'
 
     def __post_init__(self):
         super().__init__()
 
 
     def __call__(self, src_path:str, ret_val=None, do_print:bool=None) -> Any:
         """Get the path for the given source.
@@ -27,15 +27,15 @@
         """
 
         if not src_path:
             fprint('No source path given')
             return None
 
         # Check input values
-        ret_val = self._check_input_val(ret_val, self._ret_val)
+        ret_val = self._check_input_val(ret_val, self.ret_val)
         do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         root, ext = splitext(src_path)
         if not ext:
             dir_path = root
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/join_path.py` & `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/join_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from py_basic_commands.fscripts   import fprint
 from os.path    import dirname, basename, splitext
 from py_basic_commands.base   import Base
 
 
 @dataclass
 class JoinPath(Base):
-    _join_with:str = '/'
-    _remove_empty:bool=True
-    _dir_end:bool=False
+    join_with:str = '/'
+    remove_empty:bool=True
+    dir_end:bool=False
 
     def __post_init__(self):
         super().__init__(False)
 
 
     def __call__(self, *args:str, join_with:str=None, remove_empty:bool=None, dir_end:bool=None, do_print:bool=None) -> str:
         r"""Join path segments together, removing certain characters (`<>:"/\|?*`) and adjust for correct slash direction.
@@ -29,17 +29,17 @@
         """
 
         def split_join(var:str, split_with:str=' '):
             """Split a string and then join it back together"""
             return join_with.join(var.split(split_with))
         
         # Check input values
-        join_with = self._check_input_val(join_with, self._join_with)
-        remove_empty = self._check_input_val(remove_empty, self._remove_empty)
-        dir_end = self._check_input_val(dir_end, self._dir_end)
+        join_with = self._check_input_val(join_with, self.join_with)
+        remove_empty = self._check_input_val(remove_empty, self.remove_empty)
+        dir_end = self._check_input_val(dir_end, self.dir_end)
         do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         # Iterate through args and join them together
         new_args = []
         for arg_indx, arg in enumerate(args):
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/read_file.py` & `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/read_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from py_basic_commands.fscripts.fprint   import fprint
 from typing     import Any
 from py_basic_commands.base   import Base
 
 
 @dataclass
 class ReadFile(Base):
-    _create:bool = False
-    _ret_did_create:bool = False
-    _splitlines:bool = True
-    _remove_empty:bool = True
-    _do_strip:bool = True
-    _do_lower:bool = False
-    _encoding:str = 'utf-8'
+    create:bool = False
+    ret_did_create:bool = False
+    splitlines:bool = True
+    remove_empty:bool = True
+    do_strip:bool = True
+    do_lower:bool = False
+    encoding:str = 'utf-8'
 
 
     def __post_init__(self):
         super().__init__()
 
     
     def __call__(self, file_path:str, create:bool=None, ret_did_create:bool=None, splitlines:bool=None, remove_empty:bool=None, do_strip:bool=None, do_lower:bool=None, encoding:str=None, do_print:bool=None) -> Any:
@@ -63,21 +63,21 @@
                 fprint(f'File not found: {file_path}', do_print=do_print)
                 if create:
                     create_file(file_path, force=True, do_print=do_print)
                     return try_reading(True)
             return lines, did_create
 
         # Check input values
-        create      = self._check_input_val(create, self._create)
-        ret_did_create = self._check_input_val(ret_did_create, self._ret_did_create)
-        splitlines  = self._check_input_val(splitlines, self._splitlines)
-        remove_empty = self._check_input_val(remove_empty, self._remove_empty)
-        do_strip    = self._check_input_val(do_strip, self._do_strip)
-        do_lower    = self._check_input_val(do_lower, self._do_lower)
-        encoding    = self._check_input_val(encoding, self._encoding)
+        create      = self._check_input_val(create, self.create)
+        ret_did_create = self._check_input_val(ret_did_create, self.ret_did_create)
+        splitlines  = self._check_input_val(splitlines, self.splitlines)
+        remove_empty = self._check_input_val(remove_empty, self.remove_empty)
+        do_strip    = self._check_input_val(do_strip, self.do_strip)
+        do_lower    = self._check_input_val(do_lower, self.do_lower)
+        encoding    = self._check_input_val(encoding, self.encoding)
         do_print    = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         lines, did_create = try_reading()
 
         # Return the file contents
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/remove_file_dir.py` & `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/remove_file_dir.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dataclasses    import dataclass
 from shutil     import rmtree
 from os     import listdir, remove
 
 
 @dataclass
 class RemoveFileDir(Base):
-    _force:bool = True
+    force:bool = True
 
     def __post_init__(self):
         super().__init__()
 
 
     @try_traceback(print_traceback=True)
     def __call__(self, do:str, do_path:str, force:bool=False, do_print:bool=True) -> bool:
@@ -26,15 +26,15 @@
         - `do_print` (bool): Whether to print information about the file or directory removal process.
         
         Returns:
         - `bool`: Whether the file or directory was removed.
         """
 
         # Check input values
-        force    = self._check_input_val(force, self._force)
+        force    = self._check_input_val(force, self.force)
         do_print = self._check_input_val(do_print, self.do_print)
 
         if do == 'd': # Directory
             try:
                 dir_content = listdir(do_path)
             except FileNotFoundError:
                 fprint(f'Directory path not found: {do_path}')
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/write_file.py` & `py_basic_commands-0.2.23/py_basic_commands/file_dir_scripts/write_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from py_basic_commands.fscripts   import fprint
 from typing     import Any
 from py_basic_commands.base   import Base
 
 
 @dataclass
 class WriteFile(Base):
-    _append:bool    = False
-    _force_create:bool  = True
-    _remove_duplicates:bool = False
-    _encoding:str   = 'utf-8'
+    append:bool    = False
+    force_create:bool  = True
+    remove_duplicates:bool = False
+    encoding:str   = 'utf-8'
 
     def __post_init__(self):
         super().__init__()
 
 
     def __call__(self, text:Any, file_path:str, append:bool=None, force_create:bool=None, remove_duplicates:bool=None, encoding:str=None, do_print:bool=None) -> bool:
         """Write text to a file.
@@ -30,18 +30,18 @@
         - `do_print` (bool): Whether to print information about the file writing process. Default is `True`.
         
         Returns:
         - `bool`: Whether the file was created.
         """
 
         # Check input values
-        append = self._check_input_val(append, self._append)
-        force_create = self._check_input_val(force_create, self._force_create)
-        remove_duplicates = self._check_input_val(remove_duplicates, self._remove_duplicates)
-        encoding = self._check_input_val(encoding, self._encoding)
+        append = self._check_input_val(append, self.append)
+        force_create = self._check_input_val(force_create, self.force_create)
+        remove_duplicates = self._check_input_val(remove_duplicates, self.remove_duplicates)
+        encoding = self._check_input_val(encoding, self.encoding)
         do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         if text.__class__.__name__ == 'ndarray':
             text = text.tolist()
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/fscripts/finput.py` & `py_basic_commands-0.2.23/py_basic_commands/fscripts/finput.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses    import dataclass
 from py_basic_commands.fscripts.fprint   import fprint
 from py_basic_commands.base   import Base
 
 
 @dataclass
 class Finput(Base):
-    _text:str = 'Input: '
-    _nl:bool = True
-    _use_suffix:bool = True
-    _ret_type:type = str
+    text:str = 'Input: '
+    nl:bool = True
+    use_suffix:bool = True
+    ret_type:type = str
 
     def __post_init__(self):
         super().__init__()
 
 
     def __call__(self, text:str=None, ret_type:type=None, nl:bool=None, use_suffix:bool=None):
         """Get input from the user and return it as a specified type.
@@ -23,18 +23,18 @@
         - `nl` (bool): Whether to append a newline character after the input. Default is `True`.
         - `use_suffix` (bool): Whether to append a colon character to the end of the prompt text. Default is `True`.
         
         Returns:
         - The input value, converted to the specified type. If the conversion fails, the value is returned as a string.
         """
 
-        text = self._check_input_val(text, self._text)
-        nl = self._check_input_val(nl, self._nl)
-        use_suffix = self._check_input_val(use_suffix, self._use_suffix)
-        ret_type = self._check_input_val(ret_type, self._ret_type)
+        text = self._check_input_val(text, self.text)
+        nl = self._check_input_val(nl, self.nl)
+        use_suffix = self._check_input_val(use_suffix, self.use_suffix)
+        ret_type = self._check_input_val(ret_type, self.ret_type)
 
         if use_suffix and text.rstrip()[-1] != ':':
             text = f'{text}: '
 
         inpt = input(text)
 
         if nl:
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/fscripts/fprint.py` & `py_basic_commands-0.2.23/py_basic_commands/fscripts/fprint.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/py_basic_commands/fscripts/fprint_array.py` & `py_basic_commands-0.2.23/py_basic_commands/fscripts/fprint_array.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from dataclasses    import dataclass
 from textwrap   import dedent
 from py_basic_commands.base   import Base
 
 
 @dataclass
 class FprintArray(Base):
-    _header:str=''
-    _indx_brackets:str='[]'
-    _print_num=False
-    _start_num:int=0
-    _nl:bool=True
+    header:str=''
+    indx_brackets:str='[]'
+    print_num=False
+    start_num:int=0
+    nl:bool=True
 
     def __post_init__(self):
         super().__init__()
 
 
     def __call__(self, arr, header:str=None, indx_brackets:str=None, print_num=None, start_num:int=None, nl:bool=None) -> None:
         """This function prints the elements of an array along with their index numbers.
@@ -59,19 +59,19 @@
             if print_num:
                 print(f'{config_indx_num(indx)} {text}')
             else:
                 print(text)
 
 
         # Check input values
-        header      = self._check_input_val(header, self._header)
-        indx_brackets = self._check_input_val(indx_brackets, self._indx_brackets)
-        print_num   = self._check_input_val(print_num, self._print_num)
-        start_num   = self._check_input_val(start_num, self._start_num)
-        nl          = self._check_input_val(nl, self._nl)
+        header      = self._check_input_val(header, self.header)
+        indx_brackets = self._check_input_val(indx_brackets, self.indx_brackets)
+        print_num   = self._check_input_val(print_num, self.print_num)
+        start_num   = self._check_input_val(start_num, self.start_num)
+        nl          = self._check_input_val(nl, self.nl)
 
         config_indx_num = lambda indx : f'{indx_brackets[0]}{indx}{indx_brackets[1]}'
 
         arr_type = arr.__class__.__name__
 
         # Check if the input is a valid array
         if arr_type in ['list', 'set', 'tuple', 'dict']:
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/json_scripts/create_json.py` & `py_basic_commands-0.2.23/py_basic_commands/json_scripts/create_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from py_basic_commands.json_scripts.read_json  import read_json
 from py_basic_commands.fscripts   import fprint
 from py_basic_commands.base   import Base
 
 
 @dataclass
 class CreateJson(Base):
-    _force:bool = True
+    force:bool = True
 
     def __post_init__(self):
         super().__init__()
 
 
     def __call__(self, file_path:str, force:bool=None, do_print:bool=None) -> bool:
         """Create a new empty JSON file.
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/json_scripts/read_json.py` & `py_basic_commands-0.2.23/py_basic_commands/json_scripts/read_json.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/py_basic_commands/json_scripts/write_json.py` & `py_basic_commands-0.2.23/py_basic_commands/json_scripts/write_json.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from py_basic_commands.fscripts   import fprint
 from typing     import Any
 from py_basic_commands.base   import Base
 
 
 @dataclass
 class WriteJson(Base):
-    _indent:bool = True
-    _force:bool = False
+    indent:bool = True
+    force:bool = False
 
     def __post_init__(self):
         super().__init__()
                 
 
     def __call__(self, data:Any, file_path:str, force:bool=None, indent:int=None, do_print:bool=None) -> bool:
         """Write data to a JSON file.
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/other/basic_commands.py` & `py_basic_commands-0.2.23/py_basic_commands/other/basic_commands.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/py_basic_commands/other/choose_from_list.py` & `py_basic_commands-0.2.23/py_basic_commands/other/choose_from_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from py_basic_commands.fscripts import fprint, finput
 from typing     import Any
 from py_basic_commands.base   import Base
 
 
 @dataclass
 class ChooseFromList(Base):
-    _header_text:str    = ''
-    _header_nl:bool     = False
-    _input_text:str     = 'Input index: '
-    _choose_total:int   = 1
-    _start_num:int      = 0
-    _choose_until_correct:bool = True
+    header_text:str    = ''
+    header_nl:bool     = False
+    input_text:str     = 'Input index: '
+    choose_total:int   = 1
+    start_num:int      = 0
+    choose_until_correct:bool = True
 
 
     def __post_init__(self):
         super().__init__()
 
 
     def __call__(self, _array:Any, header_text:str=None, header_nl:bool=None, input_text:str=None, choose_total:int=None, start_num:int=None, choose_until_correct:bool=None) -> list:
@@ -31,20 +31,20 @@
         - `choose_until_correct` (bool): Whether to keep prompting the user until a correct input is given. Default is `True`
         
         Returns:
         - `list`: A list of the chosen values.
         """
 
         # Check input values
-        header_text = self._check_input_val(header_text, self._header_text)
-        header_nl = self._check_input_val(header_nl, self._header_nl)
-        input_text = self._check_input_val(input_text, self._input_text)
-        choose_total = self._check_input_val(choose_total, self._choose_total)
-        start_num = self._check_input_val(start_num, self._start_num)
-        choose_until_correct = self._check_input_val(choose_until_correct, self._choose_until_correct)
+        header_text = self._check_input_val(header_text, self.header_text)
+        header_nl = self._check_input_val(header_nl, self.header_nl)
+        input_text = self._check_input_val(input_text, self.input_text)
+        choose_total = self._check_input_val(choose_total, self.choose_total)
+        start_num = self._check_input_val(start_num, self.start_num)
+        choose_until_correct = self._check_input_val(choose_until_correct, self.choose_until_correct)
         
 
         if not header_text:
             if choose_total == 1:
                 header_text = '---Choose 1 value---'
             else:
                 header_text = f'---Choose {choose_total} values---'
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/other/function_timer.py` & `py_basic_commands-0.2.23/py_basic_commands/other/function_timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from py_basic_commands.fscripts   import fprint
 from py_basic_commands.base   import Base
 from time   import perf_counter
 
 
 @dataclass
 class FunctionTimer(Base):
-    _ret_time:bool = False
-    _skip_intro:bool = True
-    _skip_inputs:bool = True    
+    ret_time:bool = False
+    skip_intro:bool = True
+    skip_inputs:bool = True    
     
     def __post_init__(self) -> None:
         super().__init__()
 
 
     # TODO: Add self.do_print to function
     def _func_timer(self, do_print:bool=True, ret_time:bool=False, skip_intro:bool=True, skip_inputs:bool=True):
@@ -31,23 +31,23 @@
                 if ret_time:
                     return ret_val, time_delta
                 return ret_val
             return wrapper
         
         # Check input values
         do_print = self._check_input_val(do_print, self.do_print)
-        ret_time = self._check_input_val(ret_time, self._ret_time)
-        skip_intro = self._check_input_val(skip_intro, self._skip_intro)
-        skip_inputs = self._check_input_val(skip_inputs, self._skip_inputs)
+        ret_time = self._check_input_val(ret_time, self.ret_time)
+        skip_intro = self._check_input_val(skip_intro, self.skip_intro)
+        skip_inputs = self._check_input_val(skip_inputs, self.skip_inputs)
 
         return timer
     
 
     def __call__(self, func, *args, **kwargs):
-        fprint(f'Function timer started: {self._get_func_name(func)}', do_print=not self._skip_intro and self.do_print)
+        fprint(f'Function timer started: {self._get_func_name(func)}', do_print=not self.skip_intro and self.do_print)
         
         time_start = perf_counter()
         ret_val = func(*args, **kwargs)
         time_delta = perf_counter() - time_start
         
         self._print_time(func, time_delta, self.skip_inputs, self.do_print, *args, **kwargs)
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands/other/timer.py` & `py_basic_commands-0.2.23/py_basic_commands/other/timer.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/py_basic_commands.egg-info/PKG-INFO` & `py_basic_commands-0.2.23/py_basic_commands.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-basic-commands
-Version: 0.2.22
+Version: 0.2.23
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.22/py_basic_commands.egg-info/SOURCES.txt` & `py_basic_commands-0.2.23/py_basic_commands.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.22/pyproject.toml` & `py_basic_commands-0.2.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_basic_commands"
-version = "0.2.22"
+version = "0.2.23"
 authors = [
   { name="Rasmus Ohert", email="rassemichael@gmail.com" },
 ]
 description = "Basic tools for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py_basic_commands-0.2.22/setup.cfg` & `py_basic_commands-0.2.23/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py_basic_commands
-version = 0.2.22
+version = 0.2.23
 author = Rasmus Ohert
 author_email = rassemichael@gmail.com
 description = Basic tools for Python
 long_description = A package that has some basic tools for your basic Python needs
 url = https://github.com/RasseTheBoy/Py_Basic_Commands
 keywords = python, tool, help
 classifiers =
```

