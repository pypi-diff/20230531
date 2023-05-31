# Comparing `tmp/mespaint-0.0.3.tar.gz` & `tmp/mespaint-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mespaint-0.0.3.tar", last modified: Sat Apr 15 08:20:54 2023, max compression
+gzip compressed data, was "mespaint-0.0.4.tar", last modified: Wed May 31 18:16:53 2023, max compression
```

## Comparing `mespaint-0.0.3.tar` & `mespaint-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-04-15 08:20:54.495756 mespaint-0.0.3/
--rw-r--r--   0 vandi     (1000) vandi     (1000)     1067 2023-04-15 02:13:50.000000 mespaint-0.0.3/LICENSE
--rw-r--r--   0 vandi     (1000) vandi     (1000)      647 2023-04-15 08:20:54.495756 mespaint-0.0.3/PKG-INFO
--rw-r--r--   0 vandi     (1000) vandi     (1000)      369 2023-04-15 08:13:02.000000 mespaint-0.0.3/README.md
-drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-04-15 08:20:54.492423 mespaint-0.0.3/mespaint.egg-info/
--rw-r--r--   0 vandi     (1000) vandi     (1000)      647 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/PKG-INFO
--rw-r--r--   0 vandi     (1000) vandi     (1000)      378 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/SOURCES.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)        1 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/dependency_links.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)       43 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/entry_points.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)       26 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/requires.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)        4 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/top_level.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)       38 2023-04-15 08:20:54.495756 mespaint-0.0.3/setup.cfg
--rw-r--r--   0 vandi     (1000) vandi     (1000)      788 2023-04-15 07:51:14.000000 mespaint-0.0.3/setup.py
-drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-04-15 08:20:54.495756 mespaint-0.0.3/src/
--rw-r--r--   0 vandi     (1000) vandi     (1000)      237 2023-04-15 08:20:17.000000 mespaint-0.0.3/src/__init__.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     3047 2023-04-15 02:07:19.000000 mespaint-0.0.3/src/aboutdialog.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     5999 2023-04-15 02:02:01.000000 mespaint-0.0.3/src/canvas.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     1366 2023-04-15 02:02:49.000000 mespaint-0.0.3/src/inittab.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)      374 2023-04-15 07:44:51.000000 mespaint-0.0.3/src/main.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     5608 2023-04-15 08:20:17.000000 mespaint-0.0.3/src/mainwindow.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     3467 2023-04-15 07:44:51.000000 mespaint-0.0.3/src/menubar.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     2385 2023-04-15 00:35:35.000000 mespaint-0.0.3/src/palette.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     6576 2023-04-15 07:44:51.000000 mespaint-0.0.3/src/palettebutton.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     1093 2023-03-31 10:38:17.000000 mespaint-0.0.3/src/utils.py
+drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-05-31 18:16:53.336800 mespaint-0.0.4/
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     1067 2023-04-15 02:13:50.000000 mespaint-0.0.4/LICENSE
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     1605 2023-05-31 18:16:53.336800 mespaint-0.0.4/PKG-INFO
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     1328 2023-05-24 19:40:39.000000 mespaint-0.0.4/README.md
+drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-05-31 18:16:53.333467 mespaint-0.0.4/mespaint.egg-info/
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     1605 2023-05-31 18:16:53.000000 mespaint-0.0.4/mespaint.egg-info/PKG-INFO
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      378 2023-05-31 18:16:53.000000 mespaint-0.0.4/mespaint.egg-info/SOURCES.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)        1 2023-05-31 18:16:53.000000 mespaint-0.0.4/mespaint.egg-info/dependency_links.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)       43 2023-05-31 18:16:53.000000 mespaint-0.0.4/mespaint.egg-info/entry_points.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)       26 2023-05-31 18:16:53.000000 mespaint-0.0.4/mespaint.egg-info/requires.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)        4 2023-05-31 18:16:53.000000 mespaint-0.0.4/mespaint.egg-info/top_level.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)       38 2023-05-31 18:16:53.336800 mespaint-0.0.4/setup.cfg
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      777 2023-04-17 09:58:10.000000 mespaint-0.0.4/setup.py
+drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-05-31 18:16:53.336800 mespaint-0.0.4/src/
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      237 2023-05-31 18:16:31.000000 mespaint-0.0.4/src/__init__.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     2974 2023-04-17 09:58:10.000000 mespaint-0.0.4/src/aboutdialog.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     6814 2023-05-31 18:05:16.000000 mespaint-0.0.4/src/canvas.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     1320 2023-04-17 09:58:10.000000 mespaint-0.0.4/src/inittab.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      262 2023-05-24 19:26:59.000000 mespaint-0.0.4/src/main.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     5623 2023-05-31 18:07:52.000000 mespaint-0.0.4/src/mainwindow.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     3420 2023-04-17 09:58:09.000000 mespaint-0.0.4/src/menubar.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     2323 2023-04-17 09:58:10.000000 mespaint-0.0.4/src/palette.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     6576 2023-04-15 07:44:51.000000 mespaint-0.0.4/src/palettebutton.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     1093 2023-03-31 10:38:17.000000 mespaint-0.0.4/src/utils.py
```

### Comparing `mespaint-0.0.3/LICENSE` & `mespaint-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.3/setup.py` & `mespaint-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pathlib
 from os.path import join
-import sys
 
 from src import *
 
 from setuptools import setup, find_packages
 here = pathlib.Path(__file__).parent.resolve()
 readme = open(join(here,'README.md')).read()
```

### Comparing `mespaint-0.0.3/src/aboutdialog.py` & `mespaint-0.0.4/src/aboutdialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from PyQt5 import *
-from PyQt5.QtCore import *
 from PyQt5.QtWidgets import *
-from PyQt5.QtGui import *
 
 import src.__init__ as init
 
 class aboutDialog(QDialog):
     """main class for the "about" dialooooooog that displays some information on the author etc.
 
     Args:
```

### Comparing `mespaint-0.0.3/src/canvas.py` & `mespaint-0.0.4/src/canvas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from PyQt5 import *
 from PyQt5.QtCore import *
 from PyQt5.QtWidgets import *
 from PyQt5.QtGui import *
 
 import os
 
 from src import utils
@@ -19,14 +18,17 @@
         self.selected = False
         self.resize(self.width() - 10, self.height() - 10)
         # self.scroll_widget.wheelEvent = self.wheelEvent
         self.dragging = False
         self.last_mouse_pos = QPoint(0, 0)
         self.zoom = 1
         self.window = window
+        self.setSizePolicy(
+            QSizePolicy.Expanding, QSizePolicy.Expanding
+        )
         # self.scroll_widget.resize(self, 1000)
         # self.setPixmap(QPixmap(self.image).scaledToWidth(int(self.width())))
 
 
     # def wheelEvent(self, event: QWheelEvent):
     #     self.scroll_widget.resize(self.width() - 10, self.height() - 5)
     #     if event.modifiers() == Qt.ControlModifier and event.angleDelta().x() == 0:
@@ -111,26 +113,47 @@
         # self.width() * 0.9), int(self.height() * 0.9), Qt.KeepAspectRatio)
         # self.scroll_widget.setPixmap(QPixmap(self.image).scaledToWidth(int(self.width())))
         # self.pixmap.fill(Qt.black)
         # self.setPixmap(self.pixmap)
         # self.scroll_widget.pixmap().
         # self.repaint()
         # self = Canvas(self.path)
+        if not self.isCanvas:
+            return
         pixmap = QPixmap()
         pixmap.convertFromImage(self.image)
-        self.setPixmap(pixmap.scaledToWidth(int(self.height()*0.9)))
-        pass
+
+        try:
+            rectangle_aspect_ratio = pixmap.width() / pixmap.height()
+            target_aspect_ratio = self.width() / self.height()
+        except ZeroDivisionError:
+            return
+
+        # Determine the scaling factor for width and height
+        if rectangle_aspect_ratio > target_aspect_ratio:
+            scale_factor = self.width() / pixmap.width()
+        else:
+            scale_factor = self.height() / pixmap.height()
+
+        # Calculate the new dimensions of the resized rectangle
+        new_width = int(pixmap.width() * scale_factor * 0.9)
+        new_height = int(pixmap.height() * scale_factor * 0.9)
+
+        self.setPixmap(pixmap.scaled(new_width, new_height))
+
+    def resizeEvent(self, *__args):
+        super().resizeEvent(*__args)
+        self.reload_preview()
 
     def set_palette(self, palette):
         # self.image.load(self.path)
         # self.image.setColorCount(8)
         # for i in range(8):
         #     self.image.setColor(i, palette.colors[i].rgb())
         # self.image.setColorTable([4278190080, 4278190080, 4278190080, 4278190080])
         if self.image.format() == QImage.Format_Indexed8:
             self.image.setColorTable([i.rgb() for i in palette.colors])
         else:
             self.image = self.image.convertToFormat(QImage.Format_Indexed8, [i.rgb() for i in palette.colors])
         # self.scroll_widget.
         # self.image = self.image.convertToFormat(QImage.Format_Indexed8)
         # self.image.fill(QColor(4278190080))
-        self.reload_preview()
```

### Comparing `mespaint-0.0.3/src/inittab.py` & `mespaint-0.0.4/src/inittab.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from PyQt5 import *
 from PyQt5.QtCore import *
 from PyQt5.QtWidgets import *
-from PyQt5.QtGui import *
 
 import src.__init__ as init
 
 class initTab(QWidget):
     def __init__(self, window):
         super().__init__()
         self.Title = QLabel(f"""
```

### Comparing `mespaint-0.0.3/src/mainwindow.py` & `mespaint-0.0.4/src/mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import os
 
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import *
 
 from src.palette import Palette
-from src import canvas, palette, inittab, menubar, palettebutton
+from src import canvas, inittab
+from src import palette, menubar, palettebutton
 
 
 class Mainwindow(QMainWindow):
     def __init__(self, app):
         """Its the main window and parent of all Widgets and Dialog in the application.
 
         Args:
```

### Comparing `mespaint-0.0.3/src/menubar.py` & `mespaint-0.0.4/src/menubar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from PyQt5 import *
-from PyQt5.QtCore import *
 from PyQt5.QtWidgets import *
 from PyQt5.QtGui import *
 
 import webbrowser
 
 from src import aboutdialog
 from src import canvas
```

### Comparing `mespaint-0.0.3/src/palette.py` & `mespaint-0.0.4/src/palette.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import json
 
-from PyQt5 import *
-from PyQt5.QtCore import *
 from PyQt5.QtWidgets import *
 from PyQt5.QtGui import *
 import os
 
-from src import palettebutton
-from src import utils
+from src import utils, palettebutton
 
 
 class Palette:
     main = None
 
     def __init__(self, name, colors):
         self.colors = colors
```

### Comparing `mespaint-0.0.3/src/palettebutton.py` & `mespaint-0.0.4/src/palettebutton.py`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.3/src/utils.py` & `mespaint-0.0.4/src/utils.py`

 * *Files identical despite different names*

