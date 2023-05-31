# Comparing `tmp/my-favorite-things-0.1.tar.gz` & `tmp/my-favorite-things-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-favorite-things-0.1.tar", last modified: Wed May 31 01:22:08 2023, max compression
+gzip compressed data, was "my-favorite-things-0.2.0.tar", last modified: Wed May 31 17:37:40 2023, max compression
```

## Comparing `my-favorite-things-0.1.tar` & `my-favorite-things-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 01:22:08.690652 my-favorite-things-0.1/
--rw-r--r--   0 person    (1000) person    (1000)       66 2023-05-30 23:22:20.000000 my-favorite-things-0.1/.gitattributes
--rw-r--r--   0 person    (1000) person    (1000)       55 2023-05-31 01:19:47.000000 my-favorite-things-0.1/.gitignore
--rw-r--r--   0 person    (1000) person    (1000)    35149 2023-05-31 00:09:30.000000 my-favorite-things-0.1/LICENSE
--rw-r--r--   0 person    (1000) person    (1000)    41342 2023-05-31 01:22:08.690652 my-favorite-things-0.1/PKG-INFO
--rw-r--r--   0 person    (1000) person    (1000)      129 2023-05-30 23:23:23.000000 my-favorite-things-0.1/README.md
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 01:22:08.690652 my-favorite-things-0.1/my_favorite_things/
--rw-r--r--   0 person    (1000) person    (1000)      127 2023-05-31 01:18:21.000000 my-favorite-things-0.1/my_favorite_things/__init__.py
--rw-r--r--   0 person    (1000) person    (1000)     4509 2023-05-31 00:06:29.000000 my-favorite-things-0.1/my_favorite_things/save.py
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 01:22:08.690652 my-favorite-things-0.1/my_favorite_things.egg-info/
--rw-r--r--   0 person    (1000) person    (1000)    41342 2023-05-31 01:22:08.000000 my-favorite-things-0.1/my_favorite_things.egg-info/PKG-INFO
--rw-r--r--   0 person    (1000) person    (1000)      325 2023-05-31 01:22:08.000000 my-favorite-things-0.1/my_favorite_things.egg-info/SOURCES.txt
--rw-r--r--   0 person    (1000) person    (1000)        1 2023-05-31 01:22:08.000000 my-favorite-things-0.1/my_favorite_things.egg-info/dependency_links.txt
--rw-r--r--   0 person    (1000) person    (1000)       37 2023-05-31 01:22:08.000000 my-favorite-things-0.1/my_favorite_things.egg-info/requires.txt
--rw-r--r--   0 person    (1000) person    (1000)       19 2023-05-31 01:22:08.000000 my-favorite-things-0.1/my_favorite_things.egg-info/top_level.txt
--rw-r--r--   0 person    (1000) person    (1000)      917 2023-05-31 01:14:00.000000 my-favorite-things-0.1/pyproject.toml
--rw-r--r--   0 person    (1000) person    (1000)       38 2023-05-31 01:22:08.690652 my-favorite-things-0.1/setup.cfg
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 17:37:40.271560 my-favorite-things-0.2.0/
+-rw-r--r--   0 person    (1000) person    (1000)       66 2023-05-30 23:22:20.000000 my-favorite-things-0.2.0/.gitattributes
+-rw-r--r--   0 person    (1000) person    (1000)       55 2023-05-31 01:19:47.000000 my-favorite-things-0.2.0/.gitignore
+-rw-r--r--   0 person    (1000) person    (1000)    35149 2023-05-31 00:09:30.000000 my-favorite-things-0.2.0/LICENSE
+-rw-r--r--   0 person    (1000) person    (1000)    42724 2023-05-31 17:37:40.271560 my-favorite-things-0.2.0/PKG-INFO
+-rw-r--r--   0 person    (1000) person    (1000)     1509 2023-05-31 17:34:57.000000 my-favorite-things-0.2.0/README.md
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 17:37:40.268227 my-favorite-things-0.2.0/my_favorite_things/
+-rw-r--r--   0 person    (1000) person    (1000)      206 2023-05-31 17:26:01.000000 my-favorite-things-0.2.0/my_favorite_things/__init__.py
+-rw-r--r--   0 person    (1000) person    (1000)     1328 2023-05-31 17:22:59.000000 my-favorite-things-0.2.0/my_favorite_things/ddicts.py
+-rw-r--r--   0 person    (1000) person    (1000)     5189 2023-05-31 02:11:08.000000 my-favorite-things-0.2.0/my_favorite_things/save.py
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 17:37:40.271560 my-favorite-things-0.2.0/my_favorite_things.egg-info/
+-rw-r--r--   0 person    (1000) person    (1000)    42724 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/PKG-INFO
+-rw-r--r--   0 person    (1000) person    (1000)      354 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/SOURCES.txt
+-rw-r--r--   0 person    (1000) person    (1000)        1 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/dependency_links.txt
+-rw-r--r--   0 person    (1000) person    (1000)       37 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/requires.txt
+-rw-r--r--   0 person    (1000) person    (1000)       19 2023-05-31 17:37:40.000000 my-favorite-things-0.2.0/my_favorite_things.egg-info/top_level.txt
+-rw-r--r--   0 person    (1000) person    (1000)      919 2023-05-31 17:26:26.000000 my-favorite-things-0.2.0/pyproject.toml
+-rw-r--r--   0 person    (1000) person    (1000)       38 2023-05-31 17:37:40.271560 my-favorite-things-0.2.0/setup.cfg
```

### Comparing `my-favorite-things-0.1/LICENSE` & `my-favorite-things-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `my-favorite-things-0.1/PKG-INFO` & `my-favorite-things-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-favorite-things
-Version: 0.1
+Version: 0.2.0
 Summary: Convenient functions and classes I use too often.
 Author-email: Jacob Scott <jscott137@pm.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,7 +688,48 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # My Favorite Things
  Convenient functions and classes I use too often. If Coltrane was a programmer (_shudder_) and much worse.
+
+## Installation
+Install with
+```
+pip install my-favorite-things
+```
+
+## Current Methods
+### save
+#### `save()`
+Import by
+```
+from my_favorite_things import save
+```
+This method is used for saving data to a file. You can save as an `.npz` file for numpy array(s) or as a `.pkl` file for dictionaries and other odd python objects. By default, it will not overwrite existing files but instead append a number onto the end of file name (the keywords being, by default, `overwite=False` and `append=True`). You can save relative to your current directory (`absolute=False`) or as an absolute path (`absolute=True`). Addtionally, double check that you're saving to the correct directory with `dryrun=True`. Check the doc string for more info.
+
+---
+
+### ddict
+#### `nested_ddict()`
+Import by
+```
+from my_favorite_things import nested_ddict
+```
+This method allows for creating a nested defaultdictionary. This is useful if you have data that is dependent on multiple parameters that are heirarchical. For example, if we do
+```python
+d = nested_ddict(3, list)
+```
+then we can use it as
+```python
+d['zero']['one']['two']['three'].append(datum)
+```
+
+#### `format_ddict()`
+Import by
+```
+from my_favorite_things import format_ddict
+```
+This method will format your (nested) defaultdictionary into dictionaries. Additionally, it can turns lists in numpy arrays and/or sort the lists too.
+
+---
```

### Comparing `my-favorite-things-0.1/my_favorite_things/save.py` & `my-favorite-things-0.2.0/my_favorite_things/save.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pickle
 from pathlib import Path
 
-from numpy import savez
+import numpy as np
 
 
 def save(
     name: str,
     savedir: str = "",
     savepath: str = "",
     stype: str = "npz",
     absolute: bool = False,
     parents: int = 0,
     overwrite: bool = False,
     append: bool = True,
     dryrun: bool = False,
+    save_kwargs: dict = {},
     **files: ...,
 ) -> None:
     """
     Saves data to a file. If saving numpy arrays, use `stype="npz"`, to save as a .npz
     file. For other objects such as dicts, use `stype="pkl"` to pickle it.
 
     We start with: Path / `savepath` where Path is the CWD (either absolute or relative)
@@ -30,16 +31,16 @@
     Parameters:
     name - String representing name of file.
     savepath (default "") - Absolute or relative path to save file in depending on
         value of `absolute`.
     savedir (default "") - Directory to save in. Can be a path. This is added on top of
         `savepath` and after `parents` is applied.  So `parents` moves up the tree and
         `savedir` can move down a different branch.
-    stype (default "npz") - File type, can be either "npz" for saving numpy arrays or
-        "pkl" for saving anything as a pickle file.
+    stype (default "npz") - File type, can be either "npz" or "npy" for saving numpy
+        array(s) or "pkl" for saving anything as a pickle file.
     absolute (default False) - If True, we start in the directory `savepath`, move up it
         `parents` number of times, then append `savedir` to it. If False, we start in
         the directory $CWD/`savepath` and do the same thing.
     parents (default 0) - Which parent directory to save in. If 0, saves in same
         directory as this file. If 1, saves in parent directory. If 2, saves in
         grandparent directory. And so on.
     overwrite (default False) - If a file with the same path and file name exists,
@@ -47,14 +48,17 @@
         end of the file. If that is already taken, then append `_2` instead. And so on,
         until a unique number is found.
     append (default True) - If True and overwrite=False, append an int to the file name
         as described above in `overwrite` description. If False, abort. If
         overwrite=True, this keyword does nothing.
     dryrun (default False) - If True, will not save anything but only print out where
         the save will be to.
+    save_kwargs (default {}) - Keyword arguments to pass to the function that is doing
+        the savings, i.e. np.save, np.savez or pickle.dump. The method np.savez has no
+        extra kwargs, so this is NOT passed to savez.
     files - Kwargs for the python objects to save.
     """
     if not absolute:
         # Relative path
         path = Path.cwd() / savepath
     else:
         # Absolute path
@@ -102,11 +106,19 @@
     print(f"Saving to {path / (name + f'.{stype}')}.{dr_txt}")
     if dryrun:
         return
 
     # Save as the appropriate type
     match stype:
         case "npz":
-            savez(path / name, **files)
+            np.savez(path / name, **files)
+        case "npy":
+            if len(files.values()) != 1:
+                raise IndexError(
+                    f"Choosing stype={stype} allowing only a single array to be saved "
+                    + f"but there are {len(files.values())} arrays passed as the"
+                    + "`files` kwargs."
+                )
+            np.save(path / name, arr=list(files.values())[0], **save_kwargs)
         case "pkl":
             with open(f"{path / name}.pkl", "wb") as savefile:
-                pickle.dump(files, savefile)
+                pickle.dump(files, savefile, **save_kwargs)
```

### Comparing `my-favorite-things-0.1/my_favorite_things.egg-info/PKG-INFO` & `my-favorite-things-0.2.0/my_favorite_things.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-favorite-things
-Version: 0.1
+Version: 0.2.0
 Summary: Convenient functions and classes I use too often.
 Author-email: Jacob Scott <jscott137@pm.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,7 +688,48 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # My Favorite Things
  Convenient functions and classes I use too often. If Coltrane was a programmer (_shudder_) and much worse.
+
+## Installation
+Install with
+```
+pip install my-favorite-things
+```
+
+## Current Methods
+### save
+#### `save()`
+Import by
+```
+from my_favorite_things import save
+```
+This method is used for saving data to a file. You can save as an `.npz` file for numpy array(s) or as a `.pkl` file for dictionaries and other odd python objects. By default, it will not overwrite existing files but instead append a number onto the end of file name (the keywords being, by default, `overwite=False` and `append=True`). You can save relative to your current directory (`absolute=False`) or as an absolute path (`absolute=True`). Addtionally, double check that you're saving to the correct directory with `dryrun=True`. Check the doc string for more info.
+
+---
+
+### ddict
+#### `nested_ddict()`
+Import by
+```
+from my_favorite_things import nested_ddict
+```
+This method allows for creating a nested defaultdictionary. This is useful if you have data that is dependent on multiple parameters that are heirarchical. For example, if we do
+```python
+d = nested_ddict(3, list)
+```
+then we can use it as
+```python
+d['zero']['one']['two']['three'].append(datum)
+```
+
+#### `format_ddict()`
+Import by
+```
+from my_favorite_things import format_ddict
+```
+This method will format your (nested) defaultdictionary into dictionaries. Additionally, it can turns lists in numpy arrays and/or sort the lists too.
+
+---
```

### Comparing `my-favorite-things-0.1/pyproject.toml` & `my-favorite-things-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools.scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "my-favorite-things"
-version = "0.1"
+version = "0.2.0"
 description = "Convenient functions and classes I use too often."
 authors = [
     {name = "Jacob Scott", email = "jscott137@pm.me"}
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

