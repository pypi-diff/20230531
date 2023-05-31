# Comparing `tmp/abstract_gui-0.0.3.tar.gz` & `tmp/abstract_gui-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.3.tar", last modified: Wed May 31 05:25:29 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.4.tar", last modified: Wed May 31 14:30:40 2023, max compression
```

## Comparing `abstract_gui-0.0.3.tar` & `abstract_gui-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.706617 abstract_gui-0.0.3/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 05:25:29.706617 abstract_gui-0.0.3/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.3/README.md
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.3/pyproject.toml
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-31 05:25:29.706617 abstract_gui-0.0.3/setup.cfg
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1122 2023-05-31 05:25:13.000000 abstract_gui-0.0.3/setup.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.698617 abstract_gui-0.0.3/src/
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.698617 abstract_gui-0.0.3/src/abstract_gui/
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.702617 abstract_gui-0.0.3/src/abstract_gui/PyQt5/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.3/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.3/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.3/src/abstract_gui/__init__.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.3/src/abstract_gui/main.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.702617 abstract_gui-0.0.3/src/abstract_gui/simple_gui/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.3/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2872 2023-05-31 05:24:57.000000 abstract_gui-0.0.3/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)    11109 2023-05-31 05:24:56.000000 abstract_gui-0.0.3/src/abstract_gui/simple_gui/gui_template.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 05:25:29.702617 abstract_gui-0.0.3/src/abstract_gui.egg-info/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      495 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       31 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       13 2023-05-31 05:25:29.000000 abstract_gui-0.0.3/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:30:40.816909 abstract_gui-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-05-31 14:30:40.816909 abstract_gui-0.0.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.4/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 14:30:40.816909 abstract_gui-0.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1122 2023-05-31 14:30:21.000000 abstract_gui-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:30:40.808909 abstract_gui-0.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:30:40.812909 abstract_gui-0.0.4/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:30:40.812909 abstract_gui-0.0.4/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.4/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.4/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-31 05:17:43.000000 abstract_gui-0.0.4/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.4/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:30:40.816909 abstract_gui-0.0.4/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-05-31 04:26:08.000000 abstract_gui-0.0.4/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3140 2023-05-31 14:29:23.000000 abstract_gui-0.0.4/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    11109 2023-05-31 05:24:56.000000 abstract_gui-0.0.4/src/abstract_gui/simple_gui/gui_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:30:40.812909 abstract_gui-0.0.4/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3800 2023-05-31 14:30:40.000000 abstract_gui-0.0.4/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      495 2023-05-31 14:30:40.000000 abstract_gui-0.0.4/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-31 14:30:40.000000 abstract_gui-0.0.4/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-05-31 14:30:40.000000 abstract_gui-0.0.4/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-05-31 14:30:40.000000 abstract_gui-0.0.4/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.3/PKG-INFO` & `abstract_gui-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.3
+Version: 0.0.4
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.3/README.md` & `abstract_gui-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.3/setup.py` & `abstract_gui-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.3',
+    version='0.0.4',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/abstract_endeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.3/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.4/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.3/src/abstract_gui/main.py` & `abstract_gui-0.0.4/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.3/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.4/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from .gui_template import single_call, get_gui_fun
-from .__init__ import *
-def get_browser(title:str=None,type:str='Folder',args:dict={}):
-    if type.lower() not in ['folder','directory']:
-        type='File'
-    if title == None:
-        title = f'Please choose a {type.lower()}'
+
+def get_browser(title:str=None,type:str='Folder',args:dict={},initial_folder:str=os.getcwd()):
     """
     Function to get a browser GUI based on the type specified.
 
     Parameters:
     type (str): The type of GUI window to display. Defaults to 'Folder'.
     title (str): The title of the GUI window. Defaults to 'Directory'.
 
     Returns:
     dict: Returns the results of single_call function on the created GUI window.
     """
-    window = get_gui_fun(name=f'Window',args={"title":f'{type} Explorer', "layout":[[sg.Text(title)],[sg.Input(), get_gui_fun(name=f'{type}Browse',args=args)],[sg.OK(), sg.Cancel()]]})
+    if type.lower() not in 'folderdirectory':
+        type='File'
+    if title == None:
+        title = f'Please choose a {type.lower()}'
+    window = get_gui_fun('Window',{"title":f'{type} Explorer', "layout":[[get_gui_fun('Text',{"text":title})],
+                                                                         [get_gui_fun('Input'), get_gui_fun(f'{type}Browse',{**args,"initial_folder":initial_folder})],
+                                                                         [get_gui_fun('OK'), get_gui_fun('Cancel')]]
+                                   }
+                         )
     return single_call(window)['Browse']
 
 
 def update_progress(win:str='progress_window',st:str='bar',progress:(int or float)=0):
     """
     Function to update a progress bar in a GUI window.
 
@@ -60,11 +64,11 @@
     CIRCLE_LINE_WIDTH, LINE_COLOR = 20, 'yellow'
     TEXT_FONT = 'Courier'
     TEXT_HEIGHT = GRAPH_SIZE[0]//4
     TEXT_LOCATION = (GRAPH_SIZE[0]//2, GRAPH_SIZE[1]//2)
     TEXT_COLOR = LINE_COLOR
 
     for i in range(initial_value,max_value):
-        if not get_gui_fun(name="one_line_progress_meter",args={"title":title,"current_value":f"{i+1}","max_value":max_value,"text":'meter key',"text":'MY MESSAGE1',"text":'MY MESSAGE 2',"orientation":'v'}):
+        if not get_gui_fun("one_line_progress_meter",{"title":title,"current_value":f"{i+1}","max_value":max_value,"text":'meter key',"text":'MY MESSAGE1',"text":'MY MESSAGE 2',"orientation":'v'}):
             print('Hit the break')
             break
```

### Comparing `abstract_gui-0.0.3/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.4/src/abstract_gui/simple_gui/gui_template.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.3/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.4/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.3
+Version: 0.0.4
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

