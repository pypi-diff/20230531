# Comparing `tmp/balanna-1.2.tar.gz` & `tmp/balanna-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balanna-1.2.tar", last modified: Mon May 22 11:06:40 2023, max compression
+gzip compressed data, was "balanna-1.2.1.tar", last modified: Wed May 31 13:33:17 2023, max compression
```

## Comparing `balanna-1.2.tar` & `balanna-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-22 11:06:40.295783 balanna-1.2/
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1070 2023-05-22 07:50:24.000000 balanna-1.2/LICENSE
--rw-r--r--   0 sas      (23222) tumuser  (20909)      245 2023-05-22 11:06:40.295783 balanna-1.2/PKG-INFO
--rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-22 07:50:24.000000 balanna-1.2/README.md
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-22 11:06:40.279783 balanna-1.2/balanna/
--rw-r--r--   0 sas      (23222) tumuser  (20909)      613 2023-05-22 07:50:24.000000 balanna-1.2/balanna/__init__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1095 2023-05-22 07:50:24.000000 balanna-1.2/balanna/__main__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1581 2023-05-22 07:50:24.000000 balanna-1.2/balanna/camera_trajectories.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     2023 2023-05-22 07:54:36.000000 balanna-1.2/balanna/rendering_dataset.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)    10078 2023-05-22 07:50:24.000000 balanna-1.2/balanna/trimesh.py
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-22 11:06:40.291783 balanna-1.2/balanna/utils/
--rw-r--r--   0 sas      (23222) tumuser  (20909)       30 2023-05-22 07:50:24.000000 balanna-1.2/balanna/utils/__init__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)      559 2023-05-22 07:50:24.000000 balanna-1.2/balanna/utils/geometry.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)      122 2023-05-22 09:14:27.000000 balanna-1.2/balanna/utils/types.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     4463 2023-05-22 07:50:24.000000 balanna-1.2/balanna/utils/vedo_utils.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)    11208 2023-05-22 09:13:19.000000 balanna-1.2/balanna/window_base.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     4618 2023-05-22 08:19:05.000000 balanna-1.2/balanna/window_dataset.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     4566 2023-05-22 08:19:32.000000 balanna-1.2/balanna/window_generator.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     7265 2023-05-22 07:50:24.000000 balanna-1.2/balanna/window_real_time.py
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-22 11:06:40.287783 balanna-1.2/balanna.egg-info/
--rw-r--r--   0 sas      (23222) tumuser  (20909)      245 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/PKG-INFO
--rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/SOURCES.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)        1 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/dependency_links.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)       56 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/requires.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)        8 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/top_level.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)      103 2023-05-22 11:06:40.295783 balanna-1.2/setup.cfg
--rw-r--r--   0 sas      (23222) tumuser  (20909)      493 2023-05-22 11:06:34.000000 balanna-1.2/setup.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-31 13:33:17.896885 balanna-1.2.1/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1070 2023-05-31 12:50:49.000000 balanna-1.2.1/LICENSE
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      247 2023-05-31 13:33:17.896885 balanna-1.2.1/PKG-INFO
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-31 12:50:49.000000 balanna-1.2.1/README.md
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-31 13:33:17.880885 balanna-1.2.1/balanna/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      613 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/__init__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1095 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/__main__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1581 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/camera_trajectories.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     2023 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/rendering_dataset.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)    10078 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/trimesh.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-31 13:33:17.896885 balanna-1.2.1/balanna/utils/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)       30 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/utils/__init__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      559 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/utils/geometry.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      122 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/utils/types.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     4463 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/utils/vedo_utils.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)    10933 2023-05-31 13:17:57.000000 balanna-1.2.1/balanna/window_base.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     5138 2023-05-31 13:27:38.000000 balanna-1.2.1/balanna/window_dataset.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     4566 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/window_generator.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     7265 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/window_real_time.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-31 13:33:17.888885 balanna-1.2.1/balanna.egg-info/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      247 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/PKG-INFO
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/SOURCES.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)        1 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/dependency_links.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)       56 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/requires.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)        8 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/top_level.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      103 2023-05-31 13:33:17.900885 balanna-1.2.1/setup.cfg
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      495 2023-05-31 13:32:31.000000 balanna-1.2.1/setup.py
```

### Comparing `balanna-1.2/LICENSE` & `balanna-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `balanna-1.2/README.md` & `balanna-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna/__init__.py` & `balanna-1.2.1/balanna/__init__.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna/__main__.py` & `balanna-1.2.1/balanna/__main__.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna/camera_trajectories.py` & `balanna-1.2.1/balanna/camera_trajectories.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna/rendering_dataset.py` & `balanna-1.2.1/balanna/rendering_dataset.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna/trimesh.py` & `balanna-1.2.1/balanna/trimesh.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna/utils/geometry.py` & `balanna-1.2.1/balanna/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna/utils/vedo_utils.py` & `balanna-1.2.1/balanna/utils/vedo_utils.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna/window_base.py` & `balanna-1.2.1/balanna/window_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 import trimesh.viewer
 import time
 import vedo
 
 import matplotlib
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
-from matplotlib.backends.backend_qtagg import (
-    FigureCanvasQTAgg as FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
+from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg as FigureCanvas
 
 from functools import partial
 from PIL import Image
 from PyQt5 import Qt
 from typing import Any, Dict, List, Optional, Union
 from vtk.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
 
@@ -85,15 +84,14 @@
 
         vl3 = Qt.QVBoxLayout()
         self.figure_key_dict = {key: i for i, key in enumerate(figure_keys)}
         self.figureCanvas = []
         for _ in figure_keys:
             figure_canvas = FigureCanvas(Figure())
             self.figureCanvas.append(figure_canvas)
-            #vl3.addWidget(NavigationToolbar(figure_canvas, self))
             vl3.addWidget(figure_canvas)
         vl.addLayout(vl3)
 
         # Set up mouse timer for synchronizing mouse interactions across multiple (3D) widgets.
         # Therefore, the interaction is detected, tracked and transferred to all other 3D widgets.
         self._mouse_timer = Qt.QTimer(self)
         self._mouse_timer.timeout.connect(self.__align_event)  # noqa
@@ -142,18 +140,16 @@
                 self.image_widge_dict[key].setPixmap(Qt.QPixmap.fromImage(qt_img))
 
             elif isinstance(element, str):
                 print(f"{key}: {element}")
 
             elif isinstance(element, Axes) and key in self.figure_key_dict:
                 at = self.figure_key_dict[key]
-                # have to use this width/height to adjust the size of the axis somehow
-                width, height = self.figureCanvas[at].get_width_height()
                 # clear figure
-                self.figureCanvas[at].figure.clf()
+                self.figureCanvas[at].figure.clear()
                 # set new references of axes element
                 element.figure = self.figureCanvas[at].figure
                 self.figureCanvas[at].figure.add_axes(element)
                 # draw figure to update!
                 self.figureCanvas[at].draw()
 
             elif isinstance(element, vedo.Volume):
```

### Comparing `balanna-1.2/balanna/window_dataset.py` & `balanna-1.2.1/balanna/window_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import numpy as np
 import pathlib
 
 from matplotlib.axes import Axes
 from PyQt5 import Qt
 from typing import List, Optional, Union
 
@@ -59,15 +60,25 @@
     def render_loop(self):
         self.render_current_index()
         self.__frame_idx += 1  # TODO: run forward or backward
 
     def render_current_index(self, resetcam: bool = False) -> None:
         if 0 <= self.__frame_idx < len(self.scenes):
             scene_dict = self.scenes[self.__frame_idx]
-            self.render_(scene_dict, resetcam=resetcam)
+
+            # The same matplotlib.Axes cannot be used multiple times, as it is assigned to a figure during
+            # plotting. Therefore, we need to create a copy of the scene dictionary to be able to reuse it
+            # when plotting the scene again later.
+            scene_dict_safe = dict()
+            for key, value in scene_dict.items():
+                if key in self.figure_key_dict.keys():
+                    value = copy.deepcopy(value)
+                scene_dict_safe[key] = value
+
+            self.render_(scene_dict_safe, resetcam=resetcam)
         else:
             # Reset frame index to a valid index.
             self.__frame_idx = max(min(self.__frame_idx, len(self.scenes) - 1), 0)
             # Stop the timer, if it is running.
             if self.timer.isActive():
                 self.timer.stop()
```

### Comparing `balanna-1.2/balanna/window_generator.py` & `balanna-1.2.1/balanna/window_generator.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna/window_real_time.py` & `balanna-1.2.1/balanna/window_real_time.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2/balanna.egg-info/SOURCES.txt` & `balanna-1.2.1/balanna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

