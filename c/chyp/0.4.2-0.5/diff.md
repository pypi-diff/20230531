# Comparing `tmp/chyp-0.4.2.tar.gz` & `tmp/chyp-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyp-0.4.2.tar", last modified: Wed May 24 18:38:39 2023, max compression
+gzip compressed data, was "chyp-0.5.tar", last modified: Wed May 31 16:11:52 2023, max compression
```

## Comparing `chyp-0.4.2.tar` & `chyp-0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-24 18:38:39.985602 chyp-0.4.2/
--rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.4.2/LICENSE
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16188 2023-05-24 18:38:39.985602 chyp-0.4.2/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    15651 2023-05-24 08:31:14.000000 chyp-0.4.2/README.md
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-24 18:38:39.985602 chyp-0.4.2/chyp/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      653 2023-05-22 22:21:15.000000 chyp-0.4.2/chyp/__init__.py
--rw-r--r--   0 aleger    (1000) aleger    (1000)      715 2023-05-22 22:21:24.000000 chyp-0.4.2/chyp/__main__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    17324 2023-05-24 18:35:06.000000 chyp-0.4.2/chyp/graph.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-24 18:38:39.985602 chyp-0.4.2/chyp/gui/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      651 2023-05-22 22:23:21.000000 chyp-0.4.2/chyp/gui/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2537 2023-05-22 22:22:46.000000 chyp-0.4.2/chyp/gui/app.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4911 2023-05-22 22:22:48.000000 chyp-0.4.2/chyp/gui/codeview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4824 2023-05-22 22:20:22.000000 chyp-0.4.2/chyp/gui/colors.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2060 2023-05-22 22:22:54.000000 chyp-0.4.2/chyp/gui/completion.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4774 2023-05-22 22:23:00.000000 chyp-0.4.2/chyp/gui/document.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11702 2023-05-24 18:31:04.000000 chyp-0.4.2/chyp/gui/editor.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3285 2023-05-22 22:23:06.000000 chyp-0.4.2/chyp/gui/errorlist.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     8136 2023-05-23 21:03:29.000000 chyp-0.4.2/chyp/gui/graphscene.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1258 2023-05-22 22:23:12.000000 chyp-0.4.2/chyp/gui/graphview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3307 2023-05-24 08:35:35.000000 chyp-0.4.2/chyp/gui/highlighter.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    13424 2023-05-22 22:23:18.000000 chyp-0.4.2/chyp/gui/mainwindow.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    10786 2023-05-23 21:40:13.000000 chyp-0.4.2/chyp/layout.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11350 2023-05-22 22:20:49.000000 chyp-0.4.2/chyp/matcher.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    15044 2023-05-24 18:36:44.000000 chyp-0.4.2/chyp/parser.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3804 2023-05-22 22:21:44.000000 chyp-0.4.2/chyp/rewrite.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1791 2023-05-22 22:21:48.000000 chyp-0.4.2/chyp/rule.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.4.2/chyp/scraps.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4650 2023-05-22 22:21:58.000000 chyp-0.4.2/chyp/state.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     6018 2023-05-23 23:17:32.000000 chyp-0.4.2/chyp/term.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-24 18:38:39.985602 chyp-0.4.2/chyp.egg-info/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16188 2023-05-24 18:38:39.000000 chyp-0.4.2/chyp.egg-info/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      630 2023-05-24 18:38:39.000000 chyp-0.4.2/chyp.egg-info/SOURCES.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-24 18:38:39.000000 chyp-0.4.2/chyp.egg-info/dependency_links.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-24 18:38:39.000000 chyp-0.4.2/chyp.egg-info/entry_points.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-24 18:38:39.000000 chyp-0.4.2/chyp.egg-info/requires.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-24 18:38:39.000000 chyp-0.4.2/chyp.egg-info/top_level.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.4.2/pyproject.toml
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-24 18:38:39.985602 chyp-0.4.2/setup.cfg
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1061 2023-05-24 18:37:29.000000 chyp-0.4.2/setup.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:11:52.552710 chyp-0.5/
+-rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.5/LICENSE
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16186 2023-05-31 16:11:52.552710 chyp-0.5/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    15651 2023-05-24 08:31:14.000000 chyp-0.5/README.md
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:11:52.552710 chyp-0.5/chyp/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      653 2023-05-22 22:21:15.000000 chyp-0.5/chyp/__init__.py
+-rw-r--r--   0 aleger    (1000) aleger    (1000)      715 2023-05-22 22:21:24.000000 chyp-0.5/chyp/__main__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    17564 2023-05-31 13:33:25.000000 chyp-0.5/chyp/graph.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:11:52.552710 chyp-0.5/chyp/gui/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      651 2023-05-22 22:23:21.000000 chyp-0.5/chyp/gui/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2537 2023-05-22 22:22:46.000000 chyp-0.5/chyp/gui/app.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4911 2023-05-22 22:22:48.000000 chyp-0.5/chyp/gui/codeview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4824 2023-05-22 22:20:22.000000 chyp-0.5/chyp/gui/colors.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2060 2023-05-22 22:22:54.000000 chyp-0.5/chyp/gui/completion.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4774 2023-05-22 22:23:00.000000 chyp-0.5/chyp/gui/document.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11344 2023-05-31 12:57:08.000000 chyp-0.5/chyp/gui/editor.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3285 2023-05-22 22:23:06.000000 chyp-0.5/chyp/gui/errorlist.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     8146 2023-05-31 13:34:32.000000 chyp-0.5/chyp/gui/graphscene.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1281 2023-05-29 12:07:27.000000 chyp-0.5/chyp/gui/graphview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3307 2023-05-24 08:35:35.000000 chyp-0.5/chyp/gui/highlighter.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    13424 2023-05-22 22:23:18.000000 chyp-0.5/chyp/gui/mainwindow.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10786 2023-05-23 21:40:13.000000 chyp-0.5/chyp/layout.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11350 2023-05-22 22:20:49.000000 chyp-0.5/chyp/matcher.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16896 2023-05-31 13:47:17.000000 chyp-0.5/chyp/parser.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3804 2023-05-22 22:21:44.000000 chyp-0.5/chyp/rewrite.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1806 2023-05-31 13:58:50.000000 chyp-0.5/chyp/rule.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.5/chyp/scraps.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     5504 2023-05-31 14:43:38.000000 chyp-0.5/chyp/state.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     6018 2023-05-23 23:17:32.000000 chyp-0.5/chyp/term.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:11:52.552710 chyp-0.5/chyp.egg-info/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16186 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      630 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/entry_points.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/requires.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/top_level.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.5/pyproject.toml
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-31 16:11:52.552710 chyp-0.5/setup.cfg
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1059 2023-05-31 16:10:54.000000 chyp-0.5/setup.py
```

### Comparing `chyp-0.4.2/LICENSE` & `chyp-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/PKG-INFO` & `chyp-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.4.2
+Version: 0.5
 Summary: An interactive theorem prover for string diagrams
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chyp-0.4.2/README.md` & `chyp-0.5/README.md`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/__init__.py` & `chyp-0.5/chyp/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/__main__.py` & `chyp-0.5/chyp/__main__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/graph.py` & `chyp-0.5/chyp/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,21 @@
                 quotient[p2] = p1
 
     def __rshift__(self, other: Graph) -> Graph:
         g = self.copy()
         g.compose(other)
         return g
 
-    def unhighlight(self):
+    def highlight(self, vertices: Set[int], edges: Set[int]) -> None:
+        for v, vd in self.vdata.items():
+            vd.highlight = v in vertices
+        for e, ed in self.edata.items():
+            ed.highlight = e in edges
+
+    def unhighlight(self) -> None:
         for vd in self.vdata.values():
             vd.highlight = False
         for ed in self.edata.values():
             ed.highlight = False
 
 def gen(value: str, arity: int, coarity: int, fg: str='', bg: str='') -> Graph:
     g = Graph()
```

### Comparing `chyp-0.4.2/chyp/gui/__init__.py` & `chyp-0.5/chyp/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/gui/app.py` & `chyp-0.5/chyp/gui/app.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/gui/codeview.py` & `chyp-0.5/chyp/gui/codeview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/gui/colors.py` & `chyp-0.5/chyp/gui/colors.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/gui/completion.py` & `chyp-0.5/chyp/gui/completion.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/gui/document.py` & `chyp-0.5/chyp/gui/document.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/gui/editor.py` & `chyp-0.5/chyp/gui/editor.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from PySide6.QtCore import QByteArray, QFileInfo, QObject, QThread, QTimer, Qt, QSettings
 from PySide6.QtGui import QTextCursor
 from PySide6.QtWidgets import QHBoxLayout, QSplitter, QTreeView, QVBoxLayout, QWidget
 
 from ..layout import convex_layout
 from ..graph import Graph
 from ..state import RewriteState, State
-from ..term import graph_to_term
-from ..matcher import match_rule
-from ..rewrite import rewrite
+# from ..term import graph_to_term
+# from ..matcher import match_rule
+# from ..rewrite import rewrite
 
 from .errorlist import ErrorListModel
 from .graphview import GraphView
 from .codeview import CodeView
 from .document import ChypDocument
 from .highlighter import STATUS_GOOD, STATUS_BAD
 
@@ -233,56 +233,47 @@
         self.update_state()
         if not self.parsed: return
 
         pos = self.code_view.textCursor().position()
         part = self.state.part_at(pos)
         if part and part[2] == 'rewrite' and part[3] in self.state.rewrites:
             rw = self.state.rewrites[part[3]]
-            if rw.rule and rw.lhs:
-                start, end = rw.term_pos
-                text = self.code_view.toPlainText()
-                term = text[start:end]
-                seen = set([term])
-
-                found_prev = (term == '?')
-                rw_term = None
-                for m in match_rule(rw.rule, rw.lhs):
-                    t = graph_to_term(rewrite(rw.rule, m))
-                    if found_prev and not t in seen:
-                        rw_term = t
-                        break
-                    elif not rw_term:
-                        rw_term = t
-
-                    seen.add(t)
-                    found_prev = (term == t)
-
-                if rw_term:
-                    cursor = self.code_view.textCursor()
-                    cursor.clearSelection()
-                    cursor.setPosition(start)
-                    cursor.setPosition(end, mode=QTextCursor.MoveMode.KeepAnchor)
-
-                    # self.blockSignals(True)
-                    cursor.insertText(rw_term)
-                    self.code_view.setTextCursor(cursor)
-                    # self.blockSignals(False)
-                    # self.update_state()
+            start, end = rw.term_pos
+            text = self.code_view.toPlainText()
+            term = text[start:end]
+            rw_term = rw.tactic.next_rhs(term)
+
+            if rw_term:
+                cursor = self.code_view.textCursor()
+                cursor.clearSelection()
+                cursor.setPosition(start)
+                cursor.setPosition(end, mode=QTextCursor.MoveMode.KeepAnchor)
+
+                # self.blockSignals(True)
+                cursor.insertText(rw_term)
+                self.code_view.setTextCursor(cursor)
+                # self.blockSignals(False)
+                # self.update_state()
 
     def repeat_step_at_cursor(self) -> None:
         self.update_state()
         pos = self.code_view.textCursor().position()
         part = self.state.part_at(pos)
         if part and part[2] == 'rewrite' and part[3] in self.state.rewrites:
-            rule = self.state.rewrites[part[3]].rule
+            rw = self.state.rewrites[part[3]]
+            tactic = rw.tactic.name()
+            args = ', '.join(rw.tactic.args)
+
+            if tactic == 'rule':
+                self.code_view.add_line_below('  = ? by ' + args)
+            else:
+                self.code_view.add_line_below(f'  = ? by {tactic}({args})')
 
-            if rule:
-                self.code_view.add_line_below('  = ? by ' + rule.name)
-                self.update_state()
-                self.next_rewrite_at_cursor()
+            self.update_state()
+            self.next_rewrite_at_cursor()
 
     def update_state(self) -> None:
         self.state = State()
         self.code_view.set_current_region(None)
         
         self.state.update(self.doc.toPlainText(), self.doc.file_name)
         model = self.error_view.model()
```

### Comparing `chyp-0.4.2/chyp/gui/errorlist.py` & `chyp-0.5/chyp/gui/errorlist.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/gui/graphscene.py` & `chyp-0.5/chyp/gui/graphscene.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,19 +79,19 @@
         self.v = v
         self.eitem = eitem
         self.i = i
         vd = g.vertex_data(v)
         self.setPos(vd.x * SCALE, vd.y * SCALE)
         self.setBrush(QBrush(QColor(0,0,0)))
 
-    def refresh(self):
+    def refresh(self) -> None:
         if self.eitem and self.i != -1:
             x_shift = 0.7 * SCALE
             if self.eitem.num_t == 1:
-                y_shift = 0
+                y_shift = 0.0
             else:
                 y_shift = ((self.i / (self.eitem.num_t - 1)) - 0.5) * SCALE
             p = self.eitem.pos()
             self.setPos(p.x() + x_shift, p.y() + y_shift)
 
 class TItem(QGraphicsPathItem):
     def __init__(self, vitem: VItem, eitem: EItem, i: int, src: bool) -> None:
```

### Comparing `chyp-0.4.2/chyp/gui/graphview.py` & `chyp-0.5/chyp/gui/graphview.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,8 +27,9 @@
         super().__init__(self.graph_scene)
         self.setMouseTracking(True)
         self.setRenderHint(QPainter.RenderHint.Antialiasing)
         self.setResizeAnchor(QGraphicsView.ViewportAnchor.AnchorViewCenter)
 
     def set_graph(self, g: Graph) -> None:
         self.graph_scene.set_graph(g)
+        self.repaint()
         self.centerOn(0,0)
```

### Comparing `chyp-0.4.2/chyp/gui/highlighter.py` & `chyp-0.5/chyp/gui/highlighter.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/gui/mainwindow.py` & `chyp-0.5/chyp/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/layout.py` & `chyp-0.5/chyp/layout.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/matcher.py` & `chyp-0.5/chyp/matcher.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/parser.py` & `chyp-0.5/chyp/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,19 @@
     ?statement : import_statement | gen | let | def_statement | rule | rewrite | show
     gen : "gen" var ":" num "->" num [ gen_color ]
     def_statement : "def" var "=" term [ gen_color ]
     gen_color : "\\\"" color "\\\"" | "\\\"" color "\\\"" "\\\"" color "\\\""
     let : "let" var "=" term
     rule : "rule" var ":" term (eq | le) term
     rewrite : "rewrite" [converse] var ":" term rewrite_part*
-    rewrite_part : (eq | le) term_hole [ "by" [ converse ] rule_ref ]
+    rewrite_part : (eq | le) term_hole [ "by" tactic ]
     converse : "-"
+
+    LPAREN: "("
+    tactic : [ converse ] IDENT | IDENT LPAREN [ TACTIC_ARG ("," TACTIC_ARG)* ] ")"
     ?term  : par_term | seq
     ?par_term : "(" term ")" | par | perm | id | id0 | term_ref
     par : par_term "*" par_term
     seq : term ";" term
     perm : "sw" [ "[" num ("," num)* "]" ]
     id : "id"
     id0 : "id0"
@@ -50,14 +53,15 @@
     module_name : IDENT
     var : IDENT
     term_ref : IDENT
     rule_ref : IDENT
     term_hole : term | "?"
     color : HEXDIGIT HEXDIGIT HEXDIGIT HEXDIGIT HEXDIGIT HEXDIGIT
     IDENT: ("_"|LETTER) ("_"|"."|LETTER|DIGIT)*
+    TACTIC_ARG: /[^(),]+/
 
     %import common.LETTER
     %import common.DIGIT
     %import common.HEXDIGIT
     %import common.INT
     %import common.WS
     %import common.SH_COMMENT
@@ -73,17 +77,19 @@
 
 class ChypParseData(Transformer):
     def __init__(self, namespace: str, file_name: str) -> None:
         self.namespace = namespace
         self.file_name = file_name
         self.import_depth = 0
 
+        self.sequence: int = 0
         self.graphs: Dict[str, Graph] = dict()
         self.rules: Dict[str, Rule] = {'refl': Rule(Graph(), Graph(), name="refl")}
-        self.rewrites: Dict[str, Tuple[int, int, bool, Optional[Rule],
+        self.rule_sequence: Dict[str, int] = {'refl': 0}
+        self.rewrites: Dict[str, Tuple[int, int, int, bool, str, List[str],
                                        Optional[Graph], Optional[Graph],
                                        Optional[Graph], Optional[Graph]]] = dict()
         self.errors: List[Tuple[str, int, str]] = list()
         self.parts: List[Tuple[int, int, str, str]] = list()
         self.parsed = False
     
     # def start(self, items: List[List[Tuple[int,int,str,str]]]):
@@ -199,14 +205,16 @@
     @v_args(meta=True)
     def rule(self, meta: Meta, items: List[Any]) -> None:
         name, lhs, invertible, rhs = items
         if not name in self.rules:
             if lhs and rhs:
                 try:
                     self.rules[name] = Rule(lhs, rhs, name, invertible)
+                    self.sequence += 1
+                    self.rule_sequence[name] = self.sequence
                 except RuleError as e:
                     self.errors.append((self.file_name, meta.line, str(e)))
         else:
             self.errors.append((self.file_name, meta.line, "Rule '{}' already defined.".format(name)))
         self.parts.append((meta.start_pos, meta.end_pos, 'rule', name))
 
     @v_args(meta=True)
@@ -221,25 +229,27 @@
                 arity = len(graph.inputs())
                 coarity = len(graph.outputs())
 
                 if not name in self.graphs:
                     lhs = gen(name, arity, coarity, fg, bg)
                     self.graphs[name] = lhs
                     self.rules[rule_name] = Rule(lhs, graph, rule_name, True)
+                    self.sequence += 1
+                    self.rule_sequence[rule_name] = self.sequence
                 else:
                     lhs = self.graphs[name]
                     inp = len(lhs.inputs())
                     outp = len(lhs.outputs())
-                    if inp == arity or outp == coarity:
+                    if inp == arity and outp == coarity:
                         self.rules[rule_name] = Rule(lhs, graph, rule_name, True)
                     else:
                         self.errors.append((self.file_name, meta.line, "Term '{}' already defined with incompatible type {} -> {}.".format(name, inp, outp)))
 
         else:
-            self.errors.append((self.file_name, meta.line, "Rule '{}' already defined.".format(name, rule_name)))
+            self.errors.append((self.file_name, meta.line, "Rule '{}' already defined.".format(rule_name)))
         self.parts.append((meta.start_pos, meta.end_pos, 'rule', rule_name))
 
     def gen_color(self, items: List[Any]) -> Tuple[str,str]:
         return (items[1], items[0]) if len(items) == 2 else ('', items[0])
 
     def color(self, items: List[Any]) -> str:
         return '#' + ''.join([str(it) for it in items])
@@ -278,15 +288,15 @@
         name = '-' + base_name if converse else base_name
 
         term = items[2]
         rw_parts = items[3:]
 
         if len(rw_parts) == 0:
             self.parts.append((meta.start_pos, meta.end_pos, "rewrite", name))
-            self.rewrites[name] = (0,0,False,None,term,None,None,None)
+            self.rewrites[name] = (self.sequence, 0,0,False,"",[],term,None,None,None)
         else:
             start = meta.start_pos
             lhs = term
             rhs = None
             all_equiv = True
 
             if converse and base_name in self.rules:
@@ -294,55 +304,79 @@
                 rhs_match = self.rules[base_name].lhs
             else:
                 lhs_match = None
                 rhs_match = None
 
             last_i = len(rw_parts)-1
             for i, rw_part in enumerate(rw_parts):
-                end, t_start, t_end, equiv, rule, rhs = rw_part
+                end, t_start, t_end, equiv, tactic, tactic_args, rhs = rw_part
                 all_equiv = all_equiv and equiv
-                self.rewrites[name + ":" + str(i)] = (t_start, t_end, equiv, rule, lhs, rhs,
+                self.rewrites[name + ":" + str(i)] = (self.sequence,
+                                                      t_start, t_end, equiv, tactic, tactic_args,
+                                                      lhs, rhs,
                                                       lhs_match if i == 0 else None,
                                                       rhs_match if i == last_i else None)
                 lhs = rhs.copy() if rhs else None
                 self.parts.append((start, end, "rewrite", name + ":" + str(i)))
                 start = end
             if term and rhs:
                 try:
                     if converse:
                         if base_name in self.rules:
                             self.rules[base_name].equiv = True
+
+                            # TODO: this will stop the <= version of the rule from being usable before the converse is
+                            # proven. While this is sound and workable, it might confuse people.
+                            self.sequence += 1
+                            self.rule_sequence[base_name] = self.sequence
                         else:
                             self.errors.append((self.file_name, meta.line, "Trying to prove converse for unknown rule: " + base_name))
                     else:
                         if not name in self.rules:
                             rule = Rule(term.copy(), rhs.copy(), name=name, equiv=all_equiv)
                             # remove any highlights placed there by the first/last proof step
                             rule.lhs.unhighlight()
                             rule.rhs.unhighlight()
                             self.rules[name] = rule
+                            self.sequence += 1
+                            self.rule_sequence[name] = self.sequence
                         else:
                             self.errors.append((self.file_name, meta.line, "Rule '{}' already defined.".format(name)))
                 except RuleError as e:
                     self.errors.append((self.file_name, meta.line, str(e)))
 
     @v_args(meta=True)
-    def rewrite_part(self, meta: Meta, items: List[Any]) -> Tuple[int, int, int, bool, Optional[Rule], Optional[Graph]]:
+    def rewrite_part(self, meta: Meta, items: List[Any]) -> Tuple[int, int, int, bool, str, List[str], Optional[Graph]]:
         equiv = items[0]
         t_start,t_end,rhs = items[1]
-        converse = True if items[2] else False
-
-        rule = items[3] if items[3] else self.rules['refl']
-        if rule and converse:
-            rule = rule.converse()
+        if items[2]:
+            tactic, tactic_args = items[2]
+        else:
+            tactic, tactic_args = ("rule", ["refl"])
 
-        if equiv and rule and not rule.equiv:
-            rule = None
+        # converse = True if items[2] else False
 
-        return (meta.end_pos, t_start, t_end, equiv, rule, rhs)
+        # rule = items[3] if items[3] else self.rules['refl']
+        # if rule and converse:
+        #     rule = rule.converse()
+        # if equiv and rule and not rule.equiv:
+        #     rule = None
+
+        return (meta.end_pos, t_start, t_end, equiv, tactic, tactic_args, rhs)
+
+    def tactic(self, items: List[Any]) -> Tuple[str, List[str]]:
+        if len(items) >= 2 and str(items[1]) == "(": #)
+            args = items[2:] if not items[2] is None else []
+            # arg_str = ', '.join(args)
+            # print(f"got tactic: {items[0]}({arg_str})")
+            return (items[0], args)
+        else:
+            rule_expr = ('-' if items[0] else '') + items[1]
+            # print(f"defaulting to rule tactic: rule({rule_expr})")
+            return ("rule", [rule_expr])
 
 
     @v_args(meta=True)
     def term_hole(self, meta: Meta, items: List[Any]) -> Tuple[int, int, Optional[Graph]]:
         t = items[0] if len(items) != 0 else None
         return (meta.start_pos, meta.end_pos, t)
 
@@ -364,14 +398,16 @@
 
     parse_data = ChypParseData(namespace, file_name)
 
     if parent:
         parse_data.graphs = parent.graphs
         parse_data.rules = parent.rules
         parse_data.errors = parent.errors
+        parse_data.rule_sequence = parent.rule_sequence
+        parse_data.sequence = parent.sequence
         parse_data.import_depth = parent.import_depth + 1
         if parse_data.import_depth > 255:
             parse_data.errors += [(parent.file_name, -1, "Maximum import depth (255) exceeded. Probably a cyclic import.")]
 
     try:
         if file_name and not code:
             mtime = os.path.getmtime(file_name)
@@ -389,9 +425,12 @@
         msg = 'Parse error: '
         e_lines = e.get_context(code).splitlines()
         if len(e_lines) >= 2:
             parse_data.errors += [(file_name, e.line, msg + e_lines[0] + '\n' + len(msg)*' ' + e_lines[1])]
         else:
             parse_data.errors += [(file_name, e.line, msg + e_lines[0])]
 
+    if parent:
+        parent.sequence = parse_data.sequence
+
     return parse_data
```

### Comparing `chyp-0.4.2/chyp/rewrite.py` & `chyp-0.5/chyp/rewrite.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/rule.py` & `chyp-0.5/chyp/rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,24 +30,24 @@
         if len(lhs.inputs()) != len(rhs.inputs()) or len(lhs.outputs()) != len(rhs.outputs()):
             raise RuleError("Inputs and outputs must match on LHS and RHS of rule")
         self.lhs = lhs
         self.rhs = rhs
         self.name = name
         self.equiv = equiv
 
-    def converse(self) -> Optional[Rule]:
-        if self.equiv:
-            if self.name.startswith('-'):
-                name = self.name[1:]
-            else:
-                name = '-' + self.name
+    def copy(self) -> Rule:
+        return Rule(self.lhs.copy(), self.rhs.copy(), self.name, self.equiv)
 
-            return Rule(self.rhs.copy(), self.lhs.copy(), name, True)
+    def converse(self) -> Rule:
+        if self.name.startswith('-'):
+            name = self.name[1:]
         else:
-            return None
+            name = '-' + self.name
+
+        return Rule(self.rhs.copy(), self.lhs.copy(), name, True)
 
     def is_left_linear(self) -> bool:
         """Returns True if boundary on lhs embeds injectively"""
         verts = set()
         for v in itertools.chain(self.lhs.inputs(), self.lhs.outputs()):
             if v in verts: return False
             verts.add(v)
```

### Comparing `chyp-0.4.2/chyp/scraps.py` & `chyp-0.5/chyp/scraps.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp/state.py` & `chyp-0.5/chyp/state.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,103 +9,119 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
 from typing import Dict, List, Optional, Tuple
 
-from .matcher import find_iso, match_rule
+from .tactic import Tactic
+from .tactic.simptac import SimpTac
+from .tactic.ruletac import RuleTac
+
 from .parser import parse
-from .rewrite import dpo
 from .graph import Graph
 from .rule import Rule
 
-# class SemanticError(Exception):
-#     def __init__(self, line: int, message: str):
-#         self.line = line
-#         self.message = message
-#         super().__init__(str(self.line) + ": " + self.message)
-
 
 class RewriteState:
     UNCHECKED = 0
     CHECKING = 1
     VALID = 2
     INVALID = 3
 
     def __init__(self,
+                 sequence: int,
+                 state: State,
                  term_pos: Tuple[int,int] = (0,0),
                  equiv: bool=True,
-                 rule: Optional[Rule]=None,
+                 tactic: str='',
+                 tactic_args: Optional[List[str]]=None,
                  lhs: Optional[Graph]=None,
                  rhs: Optional[Graph]=None,
                  lhs_match: Optional[Graph]=None,
                  rhs_match: Optional[Graph]=None,
                  stub: bool=False) -> None:
+        # store an integer representing my current location. This prevents cyclic dependencies of
+        # rules used inside of tactics. TODO: this doesn't work quite right for <= rules, since it
+        # doesn't store the location of the rule *and* its converse being proved.
+        self.sequence = sequence
+        self.state = state
         self.status = RewriteState.UNCHECKED
         self.term_pos = term_pos
         self.equiv = equiv
-        self.rule = rule
+        # self.rule = rule
         self.lhs = lhs
         self.rhs = rhs
         self.lhs_match = lhs_match
         self.rhs_match = rhs_match
+
+        tactic_args = [] if tactic_args is None else tactic_args
+        if tactic == 'rule':
+            self.tactic: Tactic = RuleTac(self, tactic_args)
+        elif tactic == 'simp':
+            self.tactic = SimpTac(self, tactic_args)
+        else:
+            self.tactic = Tactic(self, tactic_args)
         self.stub = stub
 
     def check(self) -> None:
-        if self.rule and self.lhs and self.rhs:
-            # check for any constraints on the LHS and RHS first
-            if self.lhs_match and not find_iso(self.lhs, self.lhs_match):
-                self.status = RewriteState.INVALID
-            if self.rhs_match and not find_iso(self.rhs, self.rhs_match):
-                self.status = RewriteState.INVALID
-
-            # if all LHS/RHS constraints are satisfied, try to prove the rule step by rewriting
-            if self.status == RewriteState.CHECKING:
-                for m_lhs in match_rule(self.rule, self.lhs):
-                    for m_rhs in dpo(self.rule, m_lhs):
-                        iso = find_iso(m_rhs.cod, self.rhs)
-                        if iso:
-                            self.status = RewriteState.VALID
-
-                            for v in m_lhs.dom.vertices():
-                                self.lhs.vertex_data(m_lhs.vmap[v]).highlight = True
-                            for e in m_lhs.dom.edges():
-                                self.lhs.edge_data(m_lhs.emap[e]).highlight = True
-
-                            for v in m_rhs.dom.vertices():
-                                self.rhs.vertex_data(iso.vmap[m_rhs.vmap[v]]).highlight = True
-                            for e in m_rhs.dom.edges():
-                                self.rhs.edge_data(iso.emap[m_rhs.emap[e]]).highlight = True
+        self.tactic.run_check()
+        # if self.rule and self.lhs and self.rhs:
+        #     # check for any constraints on the LHS and RHS first
+        #     if self.lhs_match and not find_iso(self.lhs, self.lhs_match):
+        #         self.status = RewriteState.INVALID
+        #     if self.rhs_match and not find_iso(self.rhs, self.rhs_match):
+        #         self.status = RewriteState.INVALID
+
+        #     # if all LHS/RHS constraints are satisfied, try to prove the rule step by rewriting
+        #     if self.status == RewriteState.CHECKING:
+        #         for m_lhs in match_rule(self.rule, self.lhs):
+        #             for m_rhs in dpo(self.rule, m_lhs):
+        #                 iso = find_iso(m_rhs.cod, self.rhs)
+        #                 if iso:
+        #                     self.status = RewriteState.VALID
+
+        #                     for v in m_lhs.dom.vertices():
+        #                         self.lhs.vertex_data(m_lhs.vmap[v]).highlight = True
+        #                     for e in m_lhs.dom.edges():
+        #                         self.lhs.edge_data(m_lhs.emap[e]).highlight = True
+
+        #                     for v in m_rhs.dom.vertices():
+        #                         self.rhs.vertex_data(iso.vmap[m_rhs.vmap[v]]).highlight = True
+        #                     for e in m_rhs.dom.edges():
+        #                         self.rhs.edge_data(iso.emap[m_rhs.emap[e]]).highlight = True
 
-                            break
+        #                     break
 
-        if self.status != RewriteState.VALID:
-            self.status = RewriteState.INVALID
+        # if self.status != RewriteState.VALID:
+        #     self.status = RewriteState.INVALID
 
 class State:
     def __init__(self) -> None:
         self.graphs: Dict[str, Graph] = dict()
         self.rules: Dict[str, Rule] = dict()
+        self.rule_sequence: Dict[str, int] = dict()
         self.rewrites: Dict[str, RewriteState] = dict()
         self.parts: List[Tuple[int, int, str, str]] = list()
         self.errors: List[Tuple[str, int, str]] = list()
 
     def update(self, code: str, file_name: str) -> None:
         parse_data = parse(code, file_name)
         self.graphs = parse_data.graphs
         self.rules = parse_data.rules
+        self.rule_sequence = parse_data.rule_sequence
         self.parts = parse_data.parts
         self.errors = parse_data.errors
 
-        for name, (t_start, t_end, equiv, rule, lhs, rhs, lhs_match, rhs_match) in parse_data.rewrites.items():
+        for name, (sequence, t_start, t_end, equiv, tactic, tactic_args, lhs, rhs, lhs_match, rhs_match) in parse_data.rewrites.items():
             stub = not (':' in name)
-            self.rewrites[name] = RewriteState((t_start, t_end), equiv, rule, lhs, rhs, lhs_match, rhs_match, stub)
+            self.rewrites[name] = RewriteState(sequence, self, (t_start, t_end), equiv, tactic, tactic_args, lhs, rhs, lhs_match, rhs_match, stub)
 
     def part_with_index_at(self, pos: int) -> Optional[Tuple[int, Tuple[int,int,str,str]]]:
         p0 = (0, self.parts[0]) if len(self.parts) >= 1 else None
         for (i,p) in enumerate(self.parts):
             if p[0] <= pos:
                 p0 = (i,p)
                 if p[1] >= pos:
```

### Comparing `chyp-0.4.2/chyp/term.py` & `chyp-0.5/chyp/term.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/chyp.egg-info/PKG-INFO` & `chyp-0.5/chyp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.4.2
+Version: 0.5
 Summary: An interactive theorem prover for string diagrams
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chyp-0.4.2/chyp.egg-info/SOURCES.txt` & `chyp-0.5/chyp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chyp-0.4.2/setup.py` & `chyp-0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 
 data_files = []
 
 setuptools.setup(
     name="chyp",
-    version="0.4.2",
+    version="0.5",
     author="Aleks Kissinger",
     author_email="aleks0@gmail.com",
     description="An interactive theorem prover for string diagrams",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akissinger/chyp",
     project_urls={
```

