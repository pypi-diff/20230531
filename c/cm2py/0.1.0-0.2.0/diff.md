# Comparing `tmp/cm2py-0.1.0.tar.gz` & `tmp/cm2py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.1.0.tar", last modified: Sun May 21 06:02:21 2023, max compression
+gzip compressed data, was "cm2py-0.2.0.tar", last modified: Wed May 31 02:13:37 2023, max compression
```

## Comparing `cm2py-0.1.0.tar` & `cm2py-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.295195 cm2py-0.1.0/
--rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3012 2023-05-21 06:02:21.294191 cm2py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1189 2023-05-09 09:48:28.000000 cm2py-0.1.0/README.md
--rw-rw-rw-   0        0        0      687 2023-05-21 06:01:41.000000 cm2py-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 06:02:21.296192 cm2py-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.233193 cm2py-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.253189 cm2py-0.1.0/src/cm2py/
--rw-rw-rw-   0        0        0      213 2023-05-21 06:01:41.000000 cm2py-0.1.0/src/cm2py/__init__.py
--rw-rw-rw-   0        0        0     5804 2023-05-21 06:01:41.000000 cm2py-0.1.0/src/cm2py/cm2py.py
-drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.288198 cm2py-0.1.0/src/cm2py.egg-info/
--rw-rw-rw-   0        0        0     3012 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.290189 cm2py-0.1.0/tests/
--rw-rw-rw-   0        0        0     1525 2023-05-21 06:01:41.000000 cm2py-0.1.0/tests/test_app.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.737789 cm2py-0.2.0/
+-rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3012 2023-05-31 02:13:37.736789 cm2py-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1189 2023-05-31 02:10:18.000000 cm2py-0.2.0/README.md
+-rw-rw-rw-   0        0        0      687 2023-05-31 02:13:17.000000 cm2py-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 02:13:37.737789 cm2py-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.687788 cm2py-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.705789 cm2py-0.2.0/src/cm2py/
+-rw-rw-rw-   0        0        0      213 2023-05-21 06:01:41.000000 cm2py-0.2.0/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     6215 2023-05-31 02:13:21.000000 cm2py-0.2.0/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.729792 cm2py-0.2.0/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0     3012 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.732794 cm2py-0.2.0/tests/
+-rw-rw-rw-   0        0        0     1671 2023-05-31 02:08:47.000000 cm2py-0.2.0/tests/test_app.py
```

### Comparing `cm2py-0.1.0/LICENSE` & `cm2py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cm2py-0.1.0/PKG-INFO` & `cm2py-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.1.0
+Version: 0.2.0
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.1.0/README.md` & `cm2py-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cm2py-0.1.0/pyproject.toml` & `cm2py-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="SKM GEEK", email="qestudios17@gmail.com" },
 ]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `cm2py-0.1.0/src/cm2py/cm2py.py` & `cm2py-0.2.0/src/cm2py/cm2py.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 __copyright__ = "Copyright 2023, SKM GEEK"
 __date__ = "2023/05/21"
 __deprecated__ = False
 __email__ = "qestudios17@example.com"
 __license__ = "MIT"
 __maintainer__ = "SKM GEEK"
 __status__ = "Production"
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 import re
 from uuid import UUID, uuid4
 import numpy as np
 
 
 class Save:
     """A class to represent a save, which can be modified."""
 
     def __init__(self):
         self.blocks = []
         self.connections = {}
 
-    def addBlock(self, blockId, pos, state=False, snapToGrid=True):
+    def addBlock(self, blockId, pos, state=False, properties=None, snapToGrid=True):
         """Add a block to the save."""
         if snapToGrid:
-            newBlock = Block(blockId, tuple(np.floor(pos)), state)
+            newBlock = Block(blockId, tuple(np.floor(pos)), state=state, properties=properties)
         else:
-            newBlock = Block(blockId, pos, state)
+            newBlock = Block(blockId, pos, state=state, properties=properties)
         self.blocks.append(newBlock)
         return newBlock
 
     def addConnection(self, source, target):
         """Add a connection to the save."""
         newConnection = Connection(source, target)
         if str(newConnection.target.uuid) in self.connections:
@@ -46,15 +46,16 @@
             self.connections[str(newConnection.target.uuid)] = [newConnection]
         return newConnection
 
     def exportSave(self):
         """Export the save to a Circuit Maker 2 save string."""
         blockStrings = []
         for b in self.blocks:
-            blockStrings.append(f"{b.blockId},{int(b.state)},{b.x},{b.y},{b.z},")
+            p = "+".join(str(v) for v in b.properties) if b.properties else ""
+            blockStrings.append(f"{b.blockId},{int(b.state)},{b.x},{b.y},{b.z}," + p)
         saveString = ";".join(blockStrings) + "?"
         connectionStrings = []
         for c in self.connections.values():
             for n in c:
                 connectionStrings.append(
                     (
                         f"{[str(b.uuid) for b in self.blocks].index(str(n.source.uuid))+1},"
@@ -83,30 +84,32 @@
         for c in self.connections.values():
             for n in c:
                 if connectionRef == n:
                     del self.connections[str(n.target.uuid)][self.connections[str(n.target.uuid)].index(n)]
 
 
 class Block:
-    def __init__(self, blockId, pos, state=False):
+    def __init__(self, blockId, pos, state=False, properties=None):
         assert isinstance(blockId, int) and 0 <= blockId <= 11, "blockId must be an integer between 0 and 11"
         assert (
             isinstance(pos, tuple)
             and len(pos) == 3
             and (isinstance(pos[0], float) or isinstance(pos[0], int))
             and (isinstance(pos[1], float) or isinstance(pos[1], int))
             and (isinstance(pos[2], float) or isinstance(pos[2], int))
         ), "pos must be a 3d tuple of integers"
         assert isinstance(state, bool), "state must be a boolean"
+        assert isinstance(properties, list) or properties == None, "properties must be a list of numbers, or None"
         self.blockId = blockId
         self.pos = tuple(np.round(pos))
         self.x = self.pos[0]
         self.y = self.pos[1]
         self.z = self.pos[2]
         self.state = state
+        self.properties = properties
         self.uuid = uuid4()
 
 
 class Connection:
     def __init__(self, source, target):
         assert isinstance(source, Block), "source must be a Block object"
         assert isinstance(target, Block), "target must be a Block object"
@@ -127,24 +130,27 @@
         r"((\w+(,(-?\d+(\+-?\d+)*)*)+)(;(\w+(,(-?\d+(\+-?\d+)*)*)+))*)*$"
     )
 
     assert re.match(regex, string), "invalid save string"
 
     newSave = Save()
 
-    blocks = [[int(v) if v else None for v in i.split(",")] for i in "".join(string.split("?")[0]).split(";")]
+    blocks = [
+        [[int(a) for a in v] if "+" in v else int(v) if v else None for v in i.split(",")]
+        for i in "".join(string.split("?")[0]).split(";")
+    ]
     connections = [
         [int(v) for v in i.split(",")]
         for i in "".join(string.split("?")[1]).split(";")
         if len("".join(string.split("?")[1]).split(";")) > 1
         and isinstance("".join(string.split("?")[1]).split(";")[0], int)
         and isinstance("".join(string.split("?")[1]).split(";")[0], int)
     ]
-    # Need to refactor this line
+    # Need to refactor these lines
 
     for b in blocks:
-        newSave.addBlock(b[0], (b[2], b[3], b[4]), state=bool(b[1]), snapToGrid=snapToGrid)
+        newSave.addBlock(b[0], (b[2], b[3], b[4]), state=bool(b[1]), properties=b[5], snapToGrid=snapToGrid)
 
     for c in connections:
         newSave.addConnection(blocks[c[0] - 1], blocks[c[1] - 1])
 
     return newSave
```

### Comparing `cm2py-0.1.0/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.2.0/src/cm2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.1.0
+Version: 0.2.0
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.1.0/tests/test_app.py` & `cm2py-0.2.0/tests/test_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,7 +66,15 @@
     b2 = save.addBlock(cm2.OR, (2, 0, 0))
 
     c1 = save.addConnection(b1, b2)
 
     save.deleteConnection(c1)
 
     save.exportSave()
+
+
+def test_properties():
+    save = cm2.Save()
+
+    b1 = save.addBlock(cm2.LED, (0, 0, 0), properties=[255, 0, 0])
+
+    save.exportSave()
```

