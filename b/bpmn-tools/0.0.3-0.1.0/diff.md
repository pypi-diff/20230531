# Comparing `tmp/bpmn-tools-0.0.3.tar.gz` & `tmp/bpmn-tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpmn-tools-0.0.3.tar", last modified: Mon May 29 16:19:35 2023, max compression
+gzip compressed data, was "bpmn-tools-0.1.0.tar", last modified: Wed May 31 09:45:30 2023, max compression
```

## Comparing `bpmn-tools-0.0.3.tar` & `bpmn-tools-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.984204 bpmn-tools-0.0.3/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.980168 bpmn-tools-0.0.3/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.0.3/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-05-29 16:19:35.984077 bpmn-tools-0.0.3/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.981713 bpmn-tools-0.0.3/bpmn_tools/
--rw-r--r--   0 xtof       (501) staff       (20)      670 2023-05-29 16:18:58.000000 bpmn-tools-0.0.3/bpmn_tools/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-05-29 15:02:23.000000 bpmn-tools-0.0.3/bpmn_tools/collaboration.py
--rw-r--r--   0 xtof       (501) staff       (20)     4422 2023-05-29 15:05:14.000000 bpmn-tools-0.0.3/bpmn_tools/diagrams.py
--rw-r--r--   0 xtof       (501) staff       (20)     3027 2023-05-29 15:06:20.000000 bpmn-tools-0.0.3/bpmn_tools/flow.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.982517 bpmn-tools-0.0.3/bpmn_tools/layout/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.0.3/bpmn_tools/layout/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     3446 2023-05-29 15:19:24.000000 bpmn-tools-0.0.3/bpmn_tools/layout/simple.py
--rw-r--r--   0 xtof       (501) staff       (20)      632 2023-05-27 14:21:17.000000 bpmn-tools-0.0.3/bpmn_tools/notation.py
--rw-r--r--   0 xtof       (501) staff       (20)      641 2023-05-26 11:11:01.000000 bpmn-tools-0.0.3/bpmn_tools/util.py
--rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.0.3/bpmn_tools/visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)     3789 2023-05-27 19:24:16.000000 bpmn-tools-0.0.3/bpmn_tools/xml.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.982333 bpmn-tools-0.0.3/bpmn_tools.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      597 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       48 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       24 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       22 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/top_level.txt
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.982893 bpmn-tools-0.0.3/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/docs/conf.py
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-05-29 16:19:35.984257 bpmn-tools-0.0.3/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.0.3/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.983760 bpmn-tools-0.0.3/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    10316 2023-05-29 15:17:23.000000 bpmn-tools-0.0.3/tests/test_hello.py
--rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.0.3/tests/test_visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.0.3/tests/test_xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.308263 bpmn-tools-0.1.0/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.305083 bpmn-tools-0.1.0/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.1.0/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-05-31 09:45:30.308155 bpmn-tools-0.1.0/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.306073 bpmn-tools-0.1.0/bpmn_tools/
+-rw-r--r--   0 xtof       (501) staff       (20)       91 2023-05-31 09:44:39.000000 bpmn-tools-0.1.0/bpmn_tools/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-05-30 17:10:54.000000 bpmn-tools-0.1.0/bpmn_tools/collaboration.py
+-rw-r--r--   0 xtof       (501) staff       (20)      957 2023-05-31 08:54:54.000000 bpmn-tools-0.1.0/bpmn_tools/colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)     6325 2023-05-31 09:17:36.000000 bpmn-tools-0.1.0/bpmn_tools/diagrams.py
+-rw-r--r--   0 xtof       (501) staff       (20)     6648 2023-05-31 08:29:20.000000 bpmn-tools-0.1.0/bpmn_tools/flow.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.306925 bpmn-tools-0.1.0/bpmn_tools/layout/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.1.0/bpmn_tools/layout/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4430 2023-05-31 09:03:53.000000 bpmn-tools-0.1.0/bpmn_tools/layout/simple.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3228 2023-05-31 08:57:15.000000 bpmn-tools-0.1.0/bpmn_tools/notation.py
+-rw-r--r--   0 xtof       (501) staff       (20)      744 2023-05-31 09:05:57.000000 bpmn-tools-0.1.0/bpmn_tools/util.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.1.0/bpmn_tools/visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4665 2023-05-31 07:52:16.000000 bpmn-tools-0.1.0/bpmn_tools/xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.306728 bpmn-tools-0.1.0/bpmn_tools.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      703 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       48 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       24 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       22 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/top_level.txt
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.307114 bpmn-tools-0.1.0/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/docs/conf.py
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-05-31 09:45:30.308301 bpmn-tools-0.1.0/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.1.0/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.307966 bpmn-tools-0.1.0/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1326 2023-05-30 20:03:04.000000 bpmn-tools-0.1.0/tests/test_colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2208 2023-05-31 08:38:49.000000 bpmn-tools-0.1.0/tests/test_flows.py
+-rw-r--r--   0 xtof       (501) staff       (20)    10458 2023-05-30 19:47:37.000000 bpmn-tools-0.1.0/tests/test_hello.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4076 2023-05-31 08:39:36.000000 bpmn-tools-0.1.0/tests/test_lanes.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1133 2023-05-31 08:58:08.000000 bpmn-tools-0.1.0/tests/test_roundtrip.py
+-rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.1.0/tests/test_visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.1.0/tests/test_xml.py
```

### Comparing `bpmn-tools-0.0.3/.github/README.md` & `bpmn-tools-0.1.0/.github/README.md`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.0.3/LICENSE.txt` & `bpmn-tools-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.0.3/PKG-INFO` & `bpmn-tools-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.0.3
+Version: 0.1.0
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.0.3/bpmn_tools/collaboration.py` & `bpmn-tools-0.1.0/bpmn_tools/collaboration.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.0.3/bpmn_tools/diagrams.py` & `bpmn-tools-0.1.0/bpmn_tools/diagrams.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 """
 
 from .util import prune
 
 from . import xml
 
 from .collaboration import Participant
-from .flow          import Process, Element, Flow
+from .flow          import Process, Element, Flow, MessageFlow
 
 class Bounds(xml.Element):
   __tag__ = "dc:Bounds"
   
   def __init__(self, x=0, y=0, height=0, width=0):
     super().__init__()
-    self["x"] = str(x)
-    self["y"] = str(y)
-    self["height"] = str(height)
-    self["width"] = str(width)
+    self["x"]      = str(int(x))
+    self["y"]      = str(int(y))
+    self["height"] = str(int(height))
+    self["width"]  = str(int(width))
 
 class Label(xml.Element):
   __tag__ = "bpmndi:BPMNLabel"
   
   def __init__(self, label=None):
     super().__init__()
     self.text = label
@@ -29,37 +29,48 @@
 class Shape(xml.Element):
   __tag__ = "bpmndi:BPMNShape"
 
   def __init__(self, element=None, id=None):
     super().__init__()
     self._element = element
     self.label    = None
+    self._bounds  = None
+
+  def append(self, child):
+    if isinstance(child, Bounds):
+      self._bounds = child
+      child._parent = self
+    else:
+      super().append(child)
+    return self
 
   @property
   def id(self):
     return f"shape_{self.element['id']}"
 
   @property
   def element(self):
     if self._element:
       return self._element
     if self["bpmnElement"]:
-      return self.root.find("id", self["bpmnElement"])
+      return self.root.find("id", self["bpmnElement"], skip=self)
     return None
 
   @property
   def attributes(self):
     attributes = {}
     if self.element:
       attributes.update({
         "id"          : self.id,
         "bpmnElement" : self.element["id"]
       })
       if self.element.__horizontal__:
         attributes["isHorizontal"] = "true"
+      if self.element.__color_scheme__:
+        attributes.update(self.element.__color_scheme__)
     return attributes
 
   @property
   def children(self):
     children = []
     if self.element:
       children = [
@@ -75,30 +86,30 @@
     return children
 
 class WayPoint(xml.Element):
   __tag__ = "di:waypoint"
   
   def __init__(self, x=0, y=0):
     super().__init__()
-    self["x"] = str(x)
-    self["y"] = str(y)
+    self["x"] = str(int(x))
+    self["y"] = str(int(y))
 
 class Edge(xml.Element):
   __tag__ = "bpmndi:BPMNEdge"
 
   def __init__(self, flow=None, id=None):
     super().__init__()
     self._flow = flow
 
   @property
   def flow(self):
     if self._flow:
       return self._flow
     if self["bpmnElement"]:
-      return self.root.find("id", self["bpmnElement"])
+      return self.root.find("id", self["bpmnElement"], skip=self)
     return None
 
   def __getitem__(self, name):
     if name == "id":
       return f"edge_{self.flow['id']}"
     return super().__getitem__(name)
 
@@ -112,64 +123,113 @@
       })
     return attributes
 
   @property
   def children(self):
     children = super().children.copy()
     if self.flow:
-      children = [
-        WayPoint(
-          x=self.flow.source.x + self.flow.source.width,
-          y=self.flow.source.y + int(self.flow.source.height/2)
-        ),
-        WayPoint(
-          x=self.flow.target.x,
-          y=self.flow.target.y + int(self.flow.target.height/2)
-        )
-      ]
+      if type(self.flow) == Flow:
+        children = [
+          WayPoint(
+            x=self.flow.source.x + self.flow.source.width,
+            y=self.flow.source.y + int(self.flow.source.height/2)
+          ),
+          WayPoint(
+            x=self.flow.target.x,
+            y=self.flow.target.y + int(self.flow.target.height/2)
+          )
+        ]
+      elif type(self.flow) == MessageFlow:
+        if self.flow.source.y < self.flow.target.y:
+          top     = self.flow.source
+          bottom  = self.flow.target
+          reverse = False
+        else:
+          top     = self.flow.target
+          bottom  = self.flow.source
+          reverse = True
+        half_way_dist = int((top.y + top.height - bottom.y) / 2)
+        children = [
+          WayPoint(
+            x=top.x + int(top.width/2),
+            y=top.y + top.height
+          ),
+          WayPoint(
+            x=top.x + int(top.width/2),
+            y=top.y + top.height - half_way_dist
+          ),
+          WayPoint(
+            x=bottom.x + int(bottom.width/2),
+            y=bottom.y + half_way_dist
+          ),
+          WayPoint(
+            x=bottom.x + int(bottom.width/2),
+            y=bottom.y
+          )
+        ]
+        if reverse:
+          children.reverse()
+      else:
+        raise ValueError("unsupported flow type: {type(self.flow)}")
     return children
 
 class Plane(xml.Element):
   __tag__ = "bpmndi:BPMNPlane"
 
   def __init__(self, id="plane", element=None):
     super().__init__()
     self._element = element
     self["id"] = id
+    self._shapes = []
+    self._edges  = []
 
   @property
   def element(self):
     if self._element:
       return self._element
     if self["bpmnElement"]:
-      return self.root.find("id", self["bpmnElement"])
+      return self.root.find("id", self["bpmnElement"], skip=self)
     return None
 
   @property
   def attributes(self):
     attributes = super().attributes.copy()
     if self.element:
       attributes.update({
         "bpmnElement" : self.element["id"],
         "id" : f"plane_{self.element['id']}"
       })
     return attributes
 
+  def append(self, child):
+    if isinstance(child, Shape):
+      self._shapes.append(child)
+      child._parent = self
+    elif isinstance(child, Edge):
+      self._edges.append(child)
+      child._parent = self
+    else:
+      super().append(child)
+    return self
+
   @property
   def children(self):
     children = super().children.copy()
-    children = []
     if self.element:
       for participant in self.element.children_oftype(Participant):
         children.append(Shape(participant))
         if participant.process:
+          for lane in participant.process.laneset.lanes:
+            children.append(Shape(lane))
           for element in participant.process.children_oftype(Element):
             children.append(Shape(element))
           for flow in participant.process.children_oftype(Flow):
             children.append(Edge(flow))
+      for flow in self.element.children_oftype(MessageFlow):
+        children.append(Edge(flow))
     return children
 
 class Diagram(xml.Element):
   __tag__ = "bpmndi:BPMNDiagram"
 
   def __init__(self, id="diagram", plane=None):
     super().__init__()
```

### Comparing `bpmn-tools-0.0.3/bpmn_tools/layout/simple.py` & `bpmn-tools-0.1.0/bpmn_tools/layout/simple.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 """
 
 import logging
 logger = logging.getLogger(__name__)
 
 import json
 
-from bpmn_tools.flow          import Process, Start, End, Task
+from bpmn_tools.flow          import Process, Start, End
+from bpmn_tools.flow          import Task, UserTask, ServiceTask, ScriptTask
 from bpmn_tools.collaboration import Participant
 from bpmn_tools.visitor       import Visitor, visiting
 
 class LayoutVisitor(Visitor):
   def __init__(self):
     super().__init__()
     self.processes = {}
@@ -40,38 +41,47 @@
     self._analyse_element(event)
 
   @visiting(End)
   def visit(self, event):
     self.current_process["end"] = event
     self._analyse_element (event)
 
-  @visiting(Task)
+  @visiting(Task, UserTask, ServiceTask, ScriptTask)
   def visit(self, task):
     self._analyse_element(task)
 
   @property
   def current_process(self):
     return self.processes[self._current_process.id]
 
   @current_process.setter
   def current_process(self, process):
     self._current_process = process
     if not self._current_process.id in self.processes:
       self.processes[self._current_process.id] = {
-        "start"       : None,
+        "process"     : self._current_process,
+        "height"      : 0,
         "elements"    : {},
+        "start"       : None,
+        "steps"       : {},
         "end"         : None
       }
 
   def _analyse_element(self, element):
-    logger.info(f"analysing element: {element}")
-    if element.outgoing:
-      self.current_process["elements"][element.id] = [
-        outgoing.target for outgoing in element.outgoing
-      ]
+    # keep index of all elements
+    self.current_process["elements"][element.id] = element
+    # record steps
+    self.current_process["steps"][element.id] = [
+      outgoing.target.id for outgoing in element.outgoing
+    ]
+    # track heighest element
+    self.current_process["height"] = max([
+      self.current_process["height"],
+      element.height
+    ])
 
   def layout(self):
     """
       start -> task (-> task)* -> end
 
       participant(x,y) = 160,80
       start(x,y) = (160+15+25,                     80+25+((80-36)/2)  (width,height=36)
@@ -85,38 +95,56 @@
     SPACING = 30
 
     top = 80
     for process, analysis in self.processes.items():
       left = START
       self.process_participant[process].x = left
       self.process_participant[process].y = top
+      for lane in analysis["process"].laneset.lanes:
+        lane.x = left + HEADER
+        lane.y = top
+        
       left += HEADER + PADDING
-      max_heigth = max([step[0].height for step in analysis["elements"].values()])
       top += PADDING
       for step in self._order(analysis):
         step.x = left
-        step.y = top + (max_heigth-step.height) / 2
+        step.y = top + (analysis["height"]-step.height) / 2
         left += step.width + SPACING
-      self.process_participant[process].width = left - START
+      width = left - START
+      self.process_participant[process].width = width
+      for lane in analysis["process"].laneset.lanes:
+        lane.width  = width - HEADER
+      top += self.process_participant[process].height
 
   def _order(self, analysis):
-    step = analysis["start"]
-    end  = analysis["end"]
-    yield step
-    while step != end:
-      step = analysis["elements"][step.id][0]
+    if analysis["start"] and analysis["end"]:
+      # follow from start to end
+      step = analysis["start"]
+      end  = analysis["end"]
       yield step
+      while step != end:
+        step = analysis["elements"][analysis["steps"][step.id][0]]
+        yield step
+    else:
+      # just return the elements
+      if analysis["start"]:
+        yield analysis["start"]
+      for element in analysis["elements"].values():
+        yield element
+      if analysis["end"]:
+        yield analysis["end"]
 
   @property
   def report(self):
     return self.processes
     return {
       process : list(self._order(analysis)) \
       for process, analysis in self.processes.items()
     }
 
 def layout(model):
   visitor = LayoutVisitor()
   
   visitor.analyze(model)
+  # print(json.dumps(visitor.report, indent=2, default=str))
   logger.debug(json.dumps(visitor.report, indent=2, default=str))
   visitor.layout()
```

### Comparing `bpmn-tools-0.0.3/bpmn_tools/util.py` & `bpmn-tools-0.1.0/bpmn_tools/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from difflib import unified_diff
 import json
+import xmltodict
 
 def prune(lst):
   if len(lst) == 1:
     return lst[0]
   return lst
 
 def show_diff(result, expected):
@@ -13,9 +14,11 @@
   expected = json.dumps(expected, indent=2, sort_keys=True, default=as_dict)
   diff = unified_diff(expected.splitlines(keepends=True),
                       result.splitlines(keepends=True),
                       fromfile="expected", tofile="result")
   print("".join(diff), end="")
 
 def compare(result, expected):
+  print(json.dumps(result, indent=2))
+  print(xmltodict.unparse(result, pretty=True))
   show_diff(result, expected)
   assert result == expected
```

### Comparing `bpmn-tools-0.0.3/bpmn_tools/visitor.py` & `bpmn-tools-0.1.0/bpmn_tools/visitor.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.0.3/bpmn_tools/xml.py` & `bpmn-tools-0.1.0/bpmn_tools/xml.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,34 @@
 
 The class can be overridden to create classes dealing with specialized Elements.
 
 A Visitor allows for accessing the entire Element-hierarchy.
 
 """
 
+import random
+import string
+
+
 class Element():
   __tag__     = "Element"
 
   def __init__(self, **kwargs):
     self._children   = []
     self._parent     = None
     self._attributes = {}
-    self.text        = None
+    self._text       = None
+
+  @property
+  def text(self):
+    return self._text
+  
+  @text.setter
+  def text(self, value):
+    self._text = value
 
   def __repr__(self):
     label = f"{self.__class__.__name__}"
     if self.attributes:
       label += f"({self.attributes})"
     if self.text:
       label += f" : {self.text}"
@@ -41,25 +53,35 @@
   @property
   def root(self):
     if self._parent:
       return self._parent.root
     else:
       return self
 
-  def find(self, key, value):
+  def find(self, key, value, skip=None, stack=None):
+    if stack is None:
+      stack = []
+
+    if self in stack:
+      logger.warn("avoided recursion")
+      return None
+
+    if self is skip:
+      return None
+
     # do I have the key=value attribute?
     try:
       if self._attributes[key] == value:
         return self
     except KeyError:
       pass
     
     # recurse down children
-    for child in self._children:
-      match = child.find(key, value)
+    for child in self.children:
+      match = child.find(key, value, skip=skip, stack=stack+[self])
       if match:
         return match
 
     return None
 
   def append(self, child):
     self._children.append(child)
@@ -76,15 +98,18 @@
     return self._attributes
 
   @property
   def children(self):
     return self._children
 
   def children_oftype(self, cls):
-    return [ child for child in self._children if isinstance(child, cls) ]
+    return [
+      child for child in self.children \
+      if isinstance(child, cls) or isinstance(child.wrapped, cls)
+    ]
 
   def as_dict(self, with_tag=False):
     # collect attributes
     definition = {
       f"@{key}" : value for key, value in self.attributes.items()
     }
 
@@ -115,25 +140,31 @@
     else:
       return definition
   
   @staticmethod
   def mapped_class(tag, classes):
     if classes:
       for clazz in classes:
-        if clazz.__tag__ == tag:
-          return clazz
+        try:
+          if clazz.__tag__ == tag:
+            return clazz
+        except AttributeError:
+          pass
     return Element
   
   @classmethod
   def from_dict(cls, d, classes=None, depth=0):
     element_type, element_definition = list(d.items())[0]
     element_class = cls.mapped_class(element_type, classes)
     element = element_class()
     element.__tag__ = element_type
     
+    if type(element_definition) == str:
+      element_definition = { "#text" : element_definition }
+    
     for key, defintions in element_definition.items():
       if key[0] == "@":
         element._attributes[key[1:]] = defintions
       elif key == "#text":
         element.text = defintions
       else:
         if type(defintions) != list:
@@ -150,7 +181,15 @@
     return element
 
   def accept(self, visitor):
     with visitor:
       visitor.visit(self)
       for child in self.children:
         child.accept(visitor)
+
+class IdentifiedElement(Element):
+  def __init__(self, id=None, **kwargs):
+    super().__init__(**kwargs)
+    if id is None:
+      random_str = ''.join(random.choices(string.ascii_uppercase + string.digits, k=8))
+      id = f"{self.__class__.__name__.lower()}_{random_str}"
+    self["id"] = id
```

### Comparing `bpmn-tools-0.0.3/bpmn_tools.egg-info/PKG-INFO` & `bpmn-tools-0.1.0/bpmn_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.0.3
+Version: 0.1.0
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.0.3/bpmn_tools.egg-info/SOURCES.txt` & `bpmn-tools-0.1.0/bpmn_tools.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 MANIFEST.in
 setup.py
 .github/README.md
 bpmn_tools/__init__.py
 bpmn_tools/collaboration.py
+bpmn_tools/colors.py
 bpmn_tools/diagrams.py
 bpmn_tools/flow.py
 bpmn_tools/notation.py
 bpmn_tools/util.py
 bpmn_tools/visitor.py
 bpmn_tools/xml.py
 bpmn_tools.egg-info/PKG-INFO
@@ -17,10 +18,14 @@
 bpmn_tools.egg-info/requires.txt
 bpmn_tools.egg-info/top_level.txt
 bpmn_tools/layout/__init__.py
 bpmn_tools/layout/simple.py
 docs/__init__.py
 docs/conf.py
 tests/__init__.py
+tests/test_colors.py
+tests/test_flows.py
 tests/test_hello.py
+tests/test_lanes.py
+tests/test_roundtrip.py
 tests/test_visitor.py
 tests/test_xml.py
```

### Comparing `bpmn-tools-0.0.3/docs/conf.py` & `bpmn-tools-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.0.3/setup.py` & `bpmn-tools-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.0.3/tests/test_hello.py` & `bpmn-tools-0.1.0/tests/test_hello.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,16 @@
   definitions = Definitions(id="definitions").extend([
     process,
     collaboration
   ])
 
   compare(definitions.as_dict(with_tag=True), {
     "bpmn:definitions": {
+      "@xmlns:bioc": "http://bpmn.io/schema/bpmn/biocolor/1.0",
+      "@xmlns:color": "http://www.omg.org/spec/BPMN/non-normative/color/1.0",
       "@xmlns:bpmn": "http://www.omg.org/spec/BPMN/20100524/MODEL",
       "@xmlns:bpmndi": "http://www.omg.org/spec/BPMN/20100524/DI",
       "@xmlns:dc": "http://www.omg.org/spec/DD/20100524/DC",
       "@xmlns:di": "http://www.omg.org/spec/DD/20100524/DI",
       "@id": "definitions",
       "bpmn:process": {
         "@id": "process",
```

### Comparing `bpmn-tools-0.0.3/tests/test_visitor.py` & `bpmn-tools-0.1.0/tests/test_visitor.py`

 * *Files identical despite different names*

