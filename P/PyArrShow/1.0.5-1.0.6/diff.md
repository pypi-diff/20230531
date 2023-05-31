# Comparing `tmp/PyArrShow-1.0.5.tar.gz` & `tmp/PyArrShow-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyArrShow-1.0.5.tar", last modified: Tue May 30 04:46:19 2023, max compression
+gzip compressed data, was "PyArrShow-1.0.6.tar", last modified: Wed May 31 09:13:22 2023, max compression
```

## Comparing `PyArrShow-1.0.5.tar` & `PyArrShow-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 04:46:19.537634 PyArrShow-1.0.5/
--rw-rw-rw-   0        0        0     1088 2023-05-29 10:29:19.000000 PyArrShow-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      961 2023-05-30 04:46:19.538629 PyArrShow-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 04:46:19.515689 PyArrShow-1.0.5/PyArrShow.egg-info/
--rw-rw-rw-   0        0        0      961 2023-05-30 04:46:18.000000 PyArrShow-1.0.5/PyArrShow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-30 04:46:19.000000 PyArrShow-1.0.5/PyArrShow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 04:46:18.000000 PyArrShow-1.0.5/PyArrShow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-30 04:46:19.000000 PyArrShow-1.0.5/PyArrShow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-30 04:46:19.000000 PyArrShow-1.0.5/PyArrShow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      174 2023-05-29 10:29:41.000000 PyArrShow-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 04:46:19.535639 PyArrShow-1.0.5/pyas/
--rw-rw-rw-   0        0        0     5088 2023-05-30 01:48:38.000000 PyArrShow-1.0.5/pyas/DataCursorFrame.py
--rw-rw-rw-   0        0        0     3605 2023-05-05 11:35:48.000000 PyArrShow-1.0.5/pyas/ImgDisplayFrame.py
--rw-rw-rw-   0        0        0    13988 2023-05-06 08:42:19.000000 PyArrShow-1.0.5/pyas/PilotFrame.py
--rw-rw-rw-   0        0        0    47464 2023-05-30 04:37:12.000000 PyArrShow-1.0.5/pyas/main.py
--rw-rw-rw-   0        0        0    67984 2023-05-29 12:06:03.000000 PyArrShow-1.0.5/pyas/qrc_resources.py
--rw-rw-rw-   0        0        0      604 2023-05-30 04:44:30.000000 PyArrShow-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-05-30 04:46:19.539626 PyArrShow-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      938 2023-05-30 04:44:26.000000 PyArrShow-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:13:22.878993 PyArrShow-1.0.6/
+-rw-rw-rw-   0        0        0     1088 2023-05-29 10:29:19.000000 PyArrShow-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      961 2023-05-31 09:13:22.878993 PyArrShow-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 09:13:22.849453 PyArrShow-1.0.6/PyArrShow.egg-info/
+-rw-rw-rw-   0        0        0      961 2023-05-31 09:13:22.000000 PyArrShow-1.0.6/PyArrShow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-31 09:13:22.000000 PyArrShow-1.0.6/PyArrShow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 09:13:22.000000 PyArrShow-1.0.6/PyArrShow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-31 09:13:22.000000 PyArrShow-1.0.6/PyArrShow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-31 09:13:22.000000 PyArrShow-1.0.6/PyArrShow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      174 2023-05-29 10:29:41.000000 PyArrShow-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 09:13:22.876001 PyArrShow-1.0.6/pyas/
+-rw-rw-rw-   0        0        0     5088 2023-05-30 01:48:38.000000 PyArrShow-1.0.6/pyas/DataCursorFrame.py
+-rw-rw-rw-   0        0        0     3605 2023-05-05 11:35:48.000000 PyArrShow-1.0.6/pyas/ImgDisplayFrame.py
+-rw-rw-rw-   0        0        0    13988 2023-05-06 08:42:19.000000 PyArrShow-1.0.6/pyas/PilotFrame.py
+-rw-rw-rw-   0        0        0    47826 2023-05-31 09:10:52.000000 PyArrShow-1.0.6/pyas/main.py
+-rw-rw-rw-   0        0        0    67984 2023-05-29 12:06:03.000000 PyArrShow-1.0.6/pyas/qrc_resources.py
+-rw-rw-rw-   0        0        0      604 2023-05-31 09:12:35.000000 PyArrShow-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-05-31 09:13:22.880985 PyArrShow-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      938 2023-05-31 09:12:30.000000 PyArrShow-1.0.6/setup.py
```

### Comparing `PyArrShow-1.0.5/LICENSE` & `PyArrShow-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.5/PKG-INFO` & `PyArrShow-1.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PyArrShow
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python ArrayShow for MRI data visualization.
 Home-page: https://github.com/15625148866/PyArrShow
-Download-URL: https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.5.tar.gz
+Download-URL: https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.6.tar.gz
 Author: kaixuan,zhao
 Author-email: "Kaixuan,Zhao" <kaixuan_zhao@163.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/15625148866/PyArrShow
 Project-URL: Bug Tracker, https://github.com/15625148866/PyArrShow/issues
 Keywords: MRI,visualization
 Platform: UNKNOWN
```

### Comparing `PyArrShow-1.0.5/PyArrShow.egg-info/PKG-INFO` & `PyArrShow-1.0.6/PyArrShow.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PyArrShow
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python ArrayShow for MRI data visualization.
 Home-page: https://github.com/15625148866/PyArrShow
-Download-URL: https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.5.tar.gz
+Download-URL: https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.6.tar.gz
 Author: kaixuan,zhao
 Author-email: "Kaixuan,Zhao" <kaixuan_zhao@163.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/15625148866/PyArrShow
 Project-URL: Bug Tracker, https://github.com/15625148866/PyArrShow/issues
 Keywords: MRI,visualization
 Platform: UNKNOWN
```

### Comparing `PyArrShow-1.0.5/pyas/DataCursorFrame.py` & `PyArrShow-1.0.6/pyas/DataCursorFrame.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.5/pyas/ImgDisplayFrame.py` & `PyArrShow-1.0.6/pyas/ImgDisplayFrame.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.5/pyas/PilotFrame.py` & `PyArrShow-1.0.6/pyas/PilotFrame.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.5/pyas/main.py` & `PyArrShow-1.0.6/pyas/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import time
 
 
 from PySide6.QtWidgets import (QApplication,QMainWindow,QWidget,QVBoxLayout,QMenuBar,QMenu,QDialog,QLabel,QFileDialog,QInputDialog,
                                QPushButton,QLineEdit,QFrame,QLayout,QSlider,QComboBox,QGraphicsView,QMessageBox,QErrorMessage)
 from PySide6.QtGui import QAction, QImage, QIcon,qRgb, QPixmap,QMouseEvent,QResizeEvent
 from PySide6.QtCore import Slot,Qt,QSize,QRect,QDir,QTimer
-from .DataCursorFrame import DataCursorFrame
-from .ImgDisplayFrame import ImgDisplayFrame
-from .PilotFrame import PilotFrame
+from pyas.DataCursorFrame import DataCursorFrame
+from pyas.ImgDisplayFrame import ImgDisplayFrame
+from pyas.PilotFrame import PilotFrame
 from typing import overload
 import sigpy
-from .qrc_resources import *
+from pyas.qrc_resources import *
 
 class pyArrShowWindow(QMainWindow):
     #pyArrShowView class
     def __init__(self):
         QMainWindow.__init__(self)
         self.appTitle = 'PyArrShow'
         self.setWindowTitle(self.appTitle)
@@ -980,26 +980,40 @@
             dlg.setText('Error: Roll dim not choosen!')
             dlg.setStandardButtons(QMessageBox.StandardButton.Ok)
             dlg.setIcon(QMessageBox.Icon().Warning)
             dlg.exec()
     
     def cfgPlayVideoAction(self):
         self.timer = QTimer()
-        self.timer.setInterval(200)
+        self.timer.setInterval(200) #in ms
         self.playVideoFlag = False
 
     # #Figure slot
     # def posTitleInImgDisplay(self):
     #     self.title_label = QLabel()
 
 class PyArrShow:
     def __init__(self,np_array = np.random.randn(256,256)):
-        app = QApplication([])
+        self.app = QApplication([])
+        self.show(np_array)
+        # view = pyArrShowWindow()
+        # view.resize(500,900)
+        # view.show()
+        # pyArrShowController(model = pyArrShowModel(np_array), view = view)
+        # self.app.exec()
+        # sys.exit()
+    
+    def show(self,np_array):
         view = pyArrShowWindow()
         view.resize(500,900)
         view.show()
         pyArrShowController(model = pyArrShowModel(np_array), view = view)
-        sys.exit(app.exec())
+        self.app.exec()
+
+
+        
 
 if __name__ == '__main__':
     im_c = np.random.rand(256,256,3,3).astype(float) + np.random.rand(256,256,3,3).astype(float) * 1j
-    PyArrShow(im_c)
+    pas = PyArrShow()
+    pas.show(im_c)
+    pas.show(im_c)
```

### Comparing `PyArrShow-1.0.5/pyas/qrc_resources.py` & `PyArrShow-1.0.6/pyas/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.5/pyproject.toml` & `PyArrShow-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["hatchling"]
 build-backend="hatchling.build"
 
 [project]
 name = "PyArrShow"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Kaixuan,Zhao", email="kaixuan_zhao@163.com" },
 ]
 description = "Python ArrayShow for MRI data visualization."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `PyArrShow-1.0.5/setup.py` & `PyArrShow-1.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #! /usr/bin/env python
 from io import open
 from setuptools import setup, find_packages
 setup(
     name='PyArrShow',
-    version='1.0.5',
+    version='1.0.6',
     description='Python ArrayShow for MRI data visualization.',
     long_description='Python ArrayShow for MRI data visualization.',
     author="kaixuan,zhao",
     author_email='kaixuan_zhao@163.com',
     license='Apache License 2.0',
     url="https://github.com/15625148866/PyArrShow",
-    download_url="https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.5.tar.gz",
+    download_url="https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.6.tar.gz",
     keywords = ["MRI",'visualization'],
     install_requires=[
         'numpy',
         'PySide6',
         'matplotlib'
     ],
     classifiers=[
```

