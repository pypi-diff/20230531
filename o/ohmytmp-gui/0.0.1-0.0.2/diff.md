# Comparing `tmp/ohmytmp-gui-0.0.1.tar.gz` & `tmp/ohmytmp-gui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmytmp-gui-0.0.1.tar", last modified: Wed May 31 09:10:18 2023, max compression
+gzip compressed data, was "ohmytmp-gui-0.0.2.tar", last modified: Wed May 31 09:18:44 2023, max compression
```

## Comparing `ohmytmp-gui-0.0.1.tar` & `ohmytmp-gui-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 09:10:18.107161 ohmytmp-gui-0.0.1/
--rw-rw-rw-   0        0        0     1064 2023-05-31 08:46:46.000000 ohmytmp-gui-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1863 2023-05-31 09:10:18.106160 ohmytmp-gui-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-05-31 08:46:46.000000 ohmytmp-gui-0.0.1/README.md
--rw-rw-rw-   0        0        0      996 2023-05-31 09:00:22.000000 ohmytmp-gui-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 09:10:18.107161 ohmytmp-gui-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 09:10:18.084160 ohmytmp-gui-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 09:10:18.102160 ohmytmp-gui-0.0.1/src/ohmytmp_gui.egg-info/
--rw-rw-rw-   0        0        0     1863 2023-05-31 09:10:18.000000 ohmytmp-gui-0.0.1/src/ohmytmp_gui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-05-31 09:10:18.000000 ohmytmp-gui-0.0.1/src/ohmytmp_gui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 09:10:18.000000 ohmytmp-gui-0.0.1/src/ohmytmp_gui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-31 09:10:18.000000 ohmytmp-gui-0.0.1/src/ohmytmp_gui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-31 09:10:18.000000 ohmytmp-gui-0.0.1/src/ohmytmp_gui.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 09:10:18.084160 ohmytmp-gui-0.0.1/src/ohmytmp_plugins/
-drwxrwxrwx   0        0        0        0 2023-05-31 09:10:18.105160 ohmytmp-gui-0.0.1/src/ohmytmp_plugins/gui/
--rw-rw-rw-   0        0        0       65 2023-05-31 09:00:30.000000 ohmytmp-gui-0.0.1/src/ohmytmp_plugins/gui/__init__.py
--rw-rw-rw-   0        0        0     1342 2023-05-31 09:06:25.000000 ohmytmp-gui-0.0.1/src/ohmytmp_plugins/gui/gui.py
--rw-rw-rw-   0        0        0     1792 2023-05-27 09:30:48.000000 ohmytmp-gui-0.0.1/src/ohmytmp_plugins/gui/img.html
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:44.607775 ohmytmp-gui-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-05-31 08:46:46.000000 ohmytmp-gui-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1949 2023-05-31 09:18:44.607775 ohmytmp-gui-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2023-05-31 09:15:26.000000 ohmytmp-gui-0.0.2/README.md
+-rw-rw-rw-   0        0        0      996 2023-05-31 09:15:03.000000 ohmytmp-gui-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 09:18:44.608775 ohmytmp-gui-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:44.590776 ohmytmp-gui-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:44.604778 ohmytmp-gui-0.0.2/src/ohmytmp_gui.egg-info/
+-rw-rw-rw-   0        0        0     1949 2023-05-31 09:18:44.000000 ohmytmp-gui-0.0.2/src/ohmytmp_gui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-05-31 09:18:44.000000 ohmytmp-gui-0.0.2/src/ohmytmp_gui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 09:18:44.000000 ohmytmp-gui-0.0.2/src/ohmytmp_gui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-31 09:18:44.000000 ohmytmp-gui-0.0.2/src/ohmytmp_gui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-31 09:18:44.000000 ohmytmp-gui-0.0.2/src/ohmytmp_gui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:44.591776 ohmytmp-gui-0.0.2/src/ohmytmp_plugins/
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:44.606776 ohmytmp-gui-0.0.2/src/ohmytmp_plugins/gui/
+-rw-rw-rw-   0        0        0       65 2023-05-31 09:15:08.000000 ohmytmp-gui-0.0.2/src/ohmytmp_plugins/gui/__init__.py
+-rw-rw-rw-   0        0        0     1407 2023-05-31 09:14:38.000000 ohmytmp-gui-0.0.2/src/ohmytmp_plugins/gui/gui.py
+-rw-rw-rw-   0        0        0     1792 2023-05-27 09:30:48.000000 ohmytmp-gui-0.0.2/src/ohmytmp_plugins/gui/img.html
```

### Comparing `ohmytmp-gui-0.0.1/LICENSE` & `ohmytmp-gui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmytmp-gui-0.0.1/PKG-INFO` & `ohmytmp-gui-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp-gui
-Version: 0.0.1
+Version: 0.0.2
 Summary: ohmytmp plugin gui
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
         
@@ -33,7 +33,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # plugin-gui
+
+```sh
+pip install ohmytmp-gui
+```
+
+```py
+from ohmytmp_plugins import gui
+```
```

### Comparing `ohmytmp-gui-0.0.1/pyproject.toml` & `ohmytmp-gui-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ohmytmp-gui"
-version = "0.0.1"
+version = "0.0.2"
 description = "ohmytmp plugin gui"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["ohmytmp"]
 
 authors = [
```

### Comparing `ohmytmp-gui-0.0.1/src/ohmytmp_gui.egg-info/PKG-INFO` & `ohmytmp-gui-0.0.2/src/ohmytmp_gui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp-gui
-Version: 0.0.1
+Version: 0.0.2
 Summary: ohmytmp plugin gui
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
         
@@ -33,7 +33,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # plugin-gui
+
+```sh
+pip install ohmytmp-gui
+```
+
+```py
+from ohmytmp_plugins import gui
+```
```

### Comparing `ohmytmp-gui-0.0.1/src/ohmytmp_plugins/gui/gui.py` & `ohmytmp-gui-0.0.2/src/ohmytmp_plugins/gui/gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import os
 import json
 import flask
 import hashlib
 
 from ohmytmp import Ohmytmp
 from ohmytmp_plugins.taggy import TagInterpreter
 from ohmytmp_plugins.simimg import SimImg
 
+HTML = open(os.path.join(os.path.dirname(__file__), 'img.html'), 'r').read()
 
 class SSR:
     def __init__(self) -> None:
         self.sha_p = dict()
         self.p_sha = dict()
 
         self.ai = Ohmytmp()
@@ -23,15 +25,15 @@
         jsrc = list()
         for p in files:
             if p not in self.p_sha:
                 psha = hashlib.new('sha256', p.encode('utf8')).hexdigest()
                 self.p_sha[p] = psha
                 self.sha_p[psha] = p
             jsrc.append('/file/%s' % self.p_sha[p])
-        return open('img.html', 'r').read().replace(
+        return HTML.replace(
             '["Untitled.png"]',
             json.dumps(jsrc)
         )
 
     def walk(self, d: str) -> None:
         self.ai.walk(d)
```

### Comparing `ohmytmp-gui-0.0.1/src/ohmytmp_plugins/gui/img.html` & `ohmytmp-gui-0.0.2/src/ohmytmp_plugins/gui/img.html`

 * *Files identical despite different names*

