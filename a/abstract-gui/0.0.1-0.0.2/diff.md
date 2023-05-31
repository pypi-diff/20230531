# Comparing `tmp/abstract_gui-0.0.1.tar.gz` & `tmp/abstract_gui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.1.tar", last modified: Wed May 31 03:38:17 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.2.tar", last modified: Wed May 31 03:55:23 2023, max compression
```

## Comparing `abstract_gui-0.0.1.tar` & `abstract_gui-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:38:17.069375 abstract_gui-0.0.1/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 03:38:17.069375 abstract_gui-0.0.1/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.1/README.md
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.1/pyproject.toml
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-31 03:38:17.069375 abstract_gui-0.0.1/setup.cfg
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1101 2023-05-31 02:40:57.000000 abstract_gui-0.0.1/setup.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:38:17.061375 abstract_gui-0.0.1/src/
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:38:17.065375 abstract_gui-0.0.1/src/abstract_gui/
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:38:17.065375 abstract_gui-0.0.1/src/abstract_gui/PyQt5/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.1/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.1/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1356 2023-05-26 09:29:37.000000 abstract_gui-0.0.1/src/abstract_gui/__init__.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.1/src/abstract_gui/main.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:38:17.069375 abstract_gui-0.0.1/src/abstract_gui/simple_gui/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      131 2023-05-31 02:47:00.000000 abstract_gui-0.0.1/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2690 2023-05-31 02:45:27.000000 abstract_gui-0.0.1/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)    10590 2023-05-31 03:36:46.000000 abstract_gui-0.0.1/src/abstract_gui/simple_gui/gui_template.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:38:17.065375 abstract_gui-0.0.1/src/abstract_gui.egg-info/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 03:38:17.000000 abstract_gui-0.0.1/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      495 2023-05-31 03:38:17.000000 abstract_gui-0.0.1/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 03:38:17.000000 abstract_gui-0.0.1/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       12 2023-05-31 03:38:17.000000 abstract_gui-0.0.1/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       13 2023-05-31 03:38:17.000000 abstract_gui-0.0.1/src/abstract_gui.egg-info/top_level.txt
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/PKG-INFO
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3065 2023-05-30 02:10:16.000000 abstract_gui-0.0.2/README.md
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-31 01:51:39.000000 abstract_gui-0.0.2/pyproject.toml
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/setup.cfg
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1122 2023-05-31 03:55:04.000000 abstract_gui-0.0.2/setup.py
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.059490 abstract_gui-0.0.2/src/
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.063490 abstract_gui-0.0.2/src/abstract_gui/
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2500 2023-05-26 21:54:16.000000 abstract_gui-0.0.2/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        0 2023-05-26 02:06:40.000000 abstract_gui-0.0.2/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1356 2023-05-26 09:29:37.000000 abstract_gui-0.0.2/src/abstract_gui/__init__.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1294 2023-05-29 11:40:08.000000 abstract_gui-0.0.2/src/abstract_gui/main.py
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      131 2023-05-31 02:47:00.000000 abstract_gui-0.0.2/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2856 2023-05-31 03:54:12.000000 abstract_gui-0.0.2/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)    10590 2023-05-31 03:54:49.000000 abstract_gui-0.0.2/src/abstract_gui/simple_gui/gui_template.py
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 03:55:23.067490 abstract_gui-0.0.2/src/abstract_gui.egg-info/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     3800 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      495 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       31 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       13 2023-05-31 03:55:23.000000 abstract_gui-0.0.2/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.1/PKG-INFO` & `abstract_gui-0.0.2/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract_gui
-Version: 0.0.1
+Name: abstract-gui
+Version: 0.0.2
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.1/README.md` & `abstract_gui-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.1/setup.py` & `abstract_gui-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.1',
+    version='0.0.2',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/abstract_endeavors/abstract_essentials/abstract_gui',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.11',
     ],
     install_requires=[
-        'PySimpleGui'
+        'PySimpleGui','abstract_utilities'
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
```

### Comparing `abstract_gui-0.0.1/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.2/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.1/src/abstract_gui/__init__.py` & `abstract_gui-0.0.2/src/abstract_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.1/src/abstract_gui/main.py` & `abstract_gui-0.0.2/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.1/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.2/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-from gui_template import *
-def get_browser(type:str='Folder',title:str='Directory'):
+from .gui_template import single_call, get_gui_fun
+def get_browser(type:str='Folder',title:str=None,args:dict={}):
+    if type.lower() not in ['Folder'.lower(),'directory']:
+        type='File'
+    if title == None:
+        title = f'Please choose a {type.lower()}'
     """
     Function to get a browser GUI based on the type specified.
 
     Parameters:
     type (str): The type of GUI window to display. Defaults to 'Folder'.
     title (str): The title of the GUI window. Defaults to 'Directory'.
 
     Returns:
     dict: Returns the results of single_call function on the created GUI window.
     """
-    window = get_gui_fun(name=f'Window',args={"title":"Get filename example", "layout":[[sg.Text()],[sg.Input(), get_gui_fun(name=f'{type}Browse',args={})],[sg.OK(), sg.Cancel()]]})
+    window = get_gui_fun(name=f'Window',args={"title":f'{type} Explorer', "layout":[[sg.Text(title)],[sg.Input(), get_gui_fun(name=f'{type}Browse',args=args)],[sg.OK(), sg.Cancel()]]})
     return single_call(window)['Browse']
 
 
 def update_progress(win:str='progress_window',st:str='bar',progress:(int or float)=0):
     """
     Function to update a progress bar in a GUI window.
 
@@ -59,9 +63,7 @@
     TEXT_COLOR = LINE_COLOR
 
     for i in range(initial_value,max_value):
         if not get_gui_fun(name="one_line_progress_meter",args={"title":title,"current_value":f"{i+1}","max_value":max_value,"text":'meter key',"text":'MY MESSAGE1',"text":'MY MESSAGE 2',"orientation":'v'}):
             print('Hit the break')
             break
 
-
-fancy_progress()
```

### Comparing `abstract_gui-0.0.1/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.2/src/abstract_gui/simple_gui/gui_template.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.1/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract-gui
-Version: 0.0.1
+Name: abstract_gui
+Version: 0.0.2
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

