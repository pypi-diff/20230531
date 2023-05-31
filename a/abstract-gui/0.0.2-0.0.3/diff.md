# Comparing `tmp/abstract_gui-0.0.2.tar.gz` & `tmp/abstract_gui-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.2.tar", last modified: Wed May 31 03:55:23 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.3.tar", last modified: Wed May 31 05:25:29 2023, max compression
```

## Comparing `abstract_gui-0.0.2.tar` & `abstract_gui-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.2/README.md
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.2/pyproject.toml
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/setup.cfg
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1122 2023-05-31 03:55:04.000000 abstract_gui-0.0.2/setup.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.059490 abstract_gui-0.0.2/src/
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.063490 abstract_gui-0.0.2/src/abstract_gui/
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/src/abstract_gui/PyQt5/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.2/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.2/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1356 2023-05-26 09:29:37.000000 abstract_gui-0.0.2/src/abstract_gui/__init__.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.2/src/abstract_gui/main.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/src/abstract_gui/simple_gui/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      131 2023-05-31 02:47:00.000000 abstract_gui-0.0.2/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2856 2023-05-31 03:54:12.000000 abstract_gui-0.0.2/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)    10590 2023-05-31 03:54:49.000000 abstract_gui-0.0.2/src/abstract_gui/simple_gui/gui_template.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/src/abstract_gui.egg-info/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      495 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       31 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       13 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/top_level.txt
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.706617 abstract_gui-0.0.3/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 05:25:29.706617 abstract_gui-0.0.3/PKG-INFO
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.3/README.md
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.3/pyproject.toml
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-31 05:25:29.706617 abstract_gui-0.0.3/setup.cfg
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1122 2023-05-31 05:25:13.000000 abstract_gui-0.0.3/setup.py
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.698617 abstract_gui-0.0.3/src/
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.698617 abstract_gui-0.0.3/src/abstract_gui/
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.702617 abstract_gui-0.0.3/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.3/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.3/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.3/src/abstract_gui/__init__.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.3/src/abstract_gui/main.py
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.702617 abstract_gui-0.0.3/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.3/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2872 2023-05-31 05:24:57.000000 abstract_gui-0.0.3/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)    11109 2023-05-31 05:24:56.000000 abstract_gui-0.0.3/src/abstract_gui/simple_gui/gui_template.py
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.702617 abstract_gui-0.0.3/src/abstract_gui.egg-info/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      495 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       31 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       13 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.2/PKG-INFO` & `abstract_gui-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.2
+Version: 0.0.3
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.2/README.md` & `abstract_gui-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.2/setup.py` & `abstract_gui-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.2',
+    version='0.0.3',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/abstract_endeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.2/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.3/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.2/src/abstract_gui/main.py` & `abstract_gui-0.0.3/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.2/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.3/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .gui_template import single_call, get_gui_fun
-def get_browser(type:str='Folder',title:str=None,args:dict={}):
-    if type.lower() not in ['Folder'.lower(),'directory']:
+from .__init__ import *
+def get_browser(title:str=None,type:str='Folder',args:dict={}):
+    if type.lower() not in ['folder','directory']:
         type='File'
     if title == None:
         title = f'Please choose a {type.lower()}'
     """
     Function to get a browser GUI based on the type specified.
 
     Parameters:
```

### Comparing `abstract_gui-0.0.2/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.3/src/abstract_gui/simple_gui/gui_template.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from abstract_utilities.json_utils import get_keys
 from abstract_utilities.thread_utils import thread_alive
-from __init__ import *
+from abstract_utilities.class_utils import call_functions, process_args, get_fun
+from .__init__ import *
+globals()['registry_name'] = 'simple_gui_windows_manager'
+global_registry(name=registry_name,glob=globals())
 def expandable(size: tuple = (None, None)):
     """Returns a dictionary with window parameters for creating an expandable PySimpleGUI window."""
     return {"size": size, "resizable": True, "scrollable": True, "auto_size_text": True, "expand_x": True, "expand_y": True}
-
-change_glob(var='all_windows', val={'last_window': {'name': '', 'values': {}, 'event': ''}}, glob=globals())
+update_registry(var='all_windows', val={'last_window': {'name': '', 'values': {}, 'event': ''}},name=registry_name)
+def get_all_windows():
+    glob = get_global_from_registry(registry_name)
+    return glob['all_windows']
+def get_window_from_global(obj:str):
+    glob = get_global_from_registry(registry_name)
+    if obj in glob:
+        return glob[obj]
 def get_window(title: str = 'basic window', layout: list = [[]]):
     """
     Returns a callable object for creating a PySimpleGUI window with the specified title and layout.
 
     Args:
         title (str): The title of the window.
         layout (list): The layout of the window.
@@ -26,15 +35,15 @@
     Args:
         win (any): The object to verify.
 
     Returns:
         bool: True if the object is a valid window, False otherwise.
     """
     if type(win) == str:
-        win = ret_globals(obj=win)
+        win = get_window_from_global(obj=win)
     if type(win) == type(get_window()):
         return True
     return False
 
 def close_window(win: any = None):
     """
     Closes the given PySimpleGUI window.
@@ -128,15 +137,15 @@
 def create_win_name():
     """
     Generates a unique window name based on the existing window names.
 
     Returns:
         str: The generated unique window name.
     """
-    all_windows = ret_globals('all_windows')
+    all_windows = get_all_windows()
     keys = get_keys(all_windows)
     i, curr_try = 'default_window', 0
     while curr_try in keys:
         curr_try = f'default_window_{i}'
         i += 1
     return curr_try
 
@@ -144,25 +153,26 @@
     """
     Updates the current window's event and values based on the latest user input.
 
     Args:
         curr_win (type(get_window())): The current window to update.
         win_name (str): The name of the current window.
     """
-    all_windows = ret_globals('all_windows')
+    all_windows = get_all_windows()
     event, values = curr_win.read()
     if win_name not in all_windows:
         all_windows[win_name] = {'event': '', 'values': {}}
-        change_glob(win_name, curr_win)
+        change_glob(var=win_name, val=curr_win)
+        update_registry(var=win_name, val=curr_win,name=registry_name)
     all_windows[win_name]['event'] = event
     all_windows[win_name]['values'] = values
     all_windows['last_window']['name'] = win_name
     all_windows['last_window']['event'] = event
     all_windows['last_window']['values'] = values
-    change_glob('all_windows', all_windows)
+    update_registry(var='all_windows', val=all_windows,name=registry_name)
 
 def get_js_st(js: dict, st: str):
     """
     Retrieves a value from a dictionary based on the specified key.
 
     Args:
         js (dict): The dictionary to retrieve the value from.
@@ -264,33 +274,32 @@
     Updates the value of a specific element in the current window.
 
     Args:
         curr_win (str or type(get_window())): The current window to update. If not provided, it uses the last opened window.
         st (str): The element to update.
         obj (any): The value to assign to the element.
     """
-    all_windows = ret_globals('all_windows')
-    input(all_windows)
+    all_windows = get_all_windows()
     all_windows['last_window'][st].update(values=obj)
     if type(obj) is list:
         all_windows['last_window'][st].update(value=obj[0])
-    change_glob('all_windows', all_windows)
+    update_registry(var='all_windows', val=all_windows,name=registry_name)
 
 def get_value(curr_win: (str or type(get_window())) = 'last_window', st: str = ''):
     """
     Retrieves the value of a specific element in the current window.
 
     Args:
         curr_win (str or type(get_window())): The current window to retrieve the value from. If not provided, it uses the last opened window.
         st (str): The element to retrieve the value for.
 
     Returns:
         any: The retrieved value of the element.
     """
-    all_windows = ret_globals('all_windows')
+    all_windows = get_all_windows()
     win_name = curr_win
     if type(curr_win) == type(get_window()):
         update_read(curr_win)
         win_name = 'last_window'
     curr_js = all_windows[curr_win]
     if st in curr_js['values']:
         return curr_js['values'][st]
@@ -302,15 +311,15 @@
     Args:
         curr_win (str or type(get_window())): The current window to retrieve the event from. If not provided, it uses the last opened window.
         st (str): Unused parameter for consistency with other functions.
 
     Returns:
         any: The retrieved event of the window.
     """
-    all_windows = ret_globals('all_windows')
+    all_windows = get_all_windows()
     win_name = curr_win
     if type(curr_win) == type(get_window()):
         update_read(curr_win)
         win_name = 'last_window'
     curr_js = all_windows[win_name]
     return curr_js['event']
```

### Comparing `abstract_gui-0.0.2/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.3/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.2
+Version: 0.0.3
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

