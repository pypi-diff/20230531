# Comparing `tmp/taisim-0.0.2.tar.gz` & `tmp/taisim-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taisim-0.0.2.tar", last modified: Tue May 30 21:57:48 2023, max compression
+gzip compressed data, was "taisim-0.0.3.tar", last modified: Wed May 31 17:36:16 2023, max compression
```

## Comparing `taisim-0.0.2.tar` & `taisim-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.997840 taisim-0.0.2/
--rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-30 21:36:27.000000 taisim-0.0.2/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       37 2023-05-30 21:36:27.000000 taisim-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      423 2023-05-30 21:36:27.000000 taisim-0.0.2/NEWS.txt
--rw-r--r--   0 root         (0) staff       (20)      678 2023-05-30 21:57:47.997187 taisim-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3613 2023-05-30 21:36:27.000000 taisim-0.0.2/README.rst
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-30 21:57:47.998077 taisim-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1619 2023-05-30 21:56:46.000000 taisim-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.979991 taisim-0.0.2/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.986223 taisim-0.0.2/src/taisim/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.994673 taisim-0.0.2/src/taisim/components/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/components/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/components/log.py
--rw-r--r--   0 root         (0) staff       (20)     1230 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/components/video.py
--rw-r--r--   0 root         (0) staff       (20)     1439 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/external_data.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.996348 taisim-0.0.2/src/taisim/gui/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/gui/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8155 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/gui/help_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3895 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/gui/sensor_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3566 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/player.py
--rw-r--r--   0 root         (0) staff       (20)    17862 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/sensor.py
--rw-r--r--   0 root         (0) staff       (20)     2987 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/simulator.py
--rw-r--r--   0 root         (0) staff       (20)     9889 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.992796 taisim-0.0.2/src/taisim.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      678 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      601 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       40 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 21:36:48.000000 taisim-0.0.2/src/taisim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       21 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        7 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 17:36:16.276256 taisim-0.0.3/
+-rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-30 21:36:27.000000 taisim-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)       37 2023-05-30 21:36:27.000000 taisim-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      423 2023-05-30 21:36:27.000000 taisim-0.0.3/NEWS.txt
+-rw-r--r--   0 root         (0) staff       (20)      678 2023-05-31 17:36:16.275403 taisim-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3613 2023-05-30 21:36:27.000000 taisim-0.0.3/README.rst
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-31 17:36:16.276490 taisim-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1619 2023-05-31 17:34:40.000000 taisim-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 17:36:16.254871 taisim-0.0.3/src/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 17:36:16.262166 taisim-0.0.3/src/taisim/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 17:36:16.269683 taisim-0.0.3/src/taisim/components/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/components/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/components/log.py
+-rw-r--r--   0 root         (0) staff       (20)     1230 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/components/video.py
+-rw-r--r--   0 root         (0) staff       (20)     1439 2023-05-31 17:34:40.000000 taisim-0.0.3/src/taisim/external_data.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 17:36:16.273944 taisim-0.0.3/src/taisim/gui/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/gui/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8155 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/gui/help_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3895 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/gui/sensor_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3831 2023-05-31 17:32:31.000000 taisim-0.0.3/src/taisim/player.py
+-rw-r--r--   0 root         (0) staff       (20)    17862 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/sensor.py
+-rw-r--r--   0 root         (0) staff       (20)     2987 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/simulator.py
+-rw-r--r--   0 root         (0) staff       (20)     9889 2023-05-30 21:36:27.000000 taisim-0.0.3/src/taisim/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 17:36:16.267833 taisim-0.0.3/src/taisim.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      678 2023-05-31 17:36:16.000000 taisim-0.0.3/src/taisim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      601 2023-05-31 17:36:16.000000 taisim-0.0.3/src/taisim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-31 17:36:16.000000 taisim-0.0.3/src/taisim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       40 2023-05-31 17:36:16.000000 taisim-0.0.3/src/taisim.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 21:36:48.000000 taisim-0.0.3/src/taisim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-05-31 17:36:16.000000 taisim-0.0.3/src/taisim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        7 2023-05-31 17:36:16.000000 taisim-0.0.3/src/taisim.egg-info/top_level.txt
```

### Comparing `taisim-0.0.2/LICENSE` & `taisim-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taisim-0.0.2/PKG-INFO` & `taisim-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taisim
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple python3 simulator for advanced driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut@outlook.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Platform: UNKNOWN
```

### Comparing `taisim-0.0.2/README.rst` & `taisim-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `taisim-0.0.2/setup.py` & `taisim-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # For more details, see:
     # http://packages.python.org/distribute/setuptools.html#declaring-dependencies
     'requests'	
 ]
 
 
 setup(name='taisim',
-    version='0.0.2',
+    version='0.0.3',
     description="Simple python3 simulator for advanced driving systems",
     long_description="simple python simulator for advanced driving systems",
     
     keywords='Simulator computer vision Advanced Driving',
     author='Tucudean Adrian-Ionut',
     author_email='Tucudean.Adrian.Ionut@outlook.com',
     url='https://github.com/Amporu/SparkVerse',
```

### Comparing `taisim-0.0.2/src/taisim/components/log.py` & `taisim-0.0.3/src/taisim/components/log.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.2/src/taisim/components/video.py` & `taisim-0.0.3/src/taisim/components/video.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.2/src/taisim/external_data.py` & `taisim-0.0.3/src/taisim/external_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 autor: Tucudean Adrian-Ionut
 date: 22.05.2023
 email: Tucudean.Adrian.Ionut@outlook.com
 license: MIT
 """
 import os
 from taisim.components.log import logger
-VERSION='0.0.1'
+VERSION='0.0.3'
 logger.info("VERSION : \033[92m%s\033[0m",VERSION)
 CAR    = os.path.join(os.path.dirname(__file__), 'data/player.png')
 LEVEL1 = os.path.join(os.path.dirname(__file__), 'data/LineFollower1.png')
 LEVEL2 = os.path.join(os.path.dirname(__file__), 'data/LineFollower2.png')
 LEVEL3 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper1.png')
 LEVEL4 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper2.png')
 LEVEL5 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper3.png')
```

### Comparing `taisim-0.0.2/src/taisim/gui/help_bar.py` & `taisim-0.0.3/src/taisim/gui/help_bar.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.2/src/taisim/gui/sensor_bar.py` & `taisim-0.0.3/src/taisim/gui/sensor_bar.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.2/src/taisim/player.py` & `taisim-0.0.3/src/taisim/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 # pylint: disable=too-many-instance-attributes
 import math
 import pygame
 import taisim.external_data as ex
 from taisim.utils import Utils
 from taisim.components.log import logger
-PLAYER=pygame.image.load(ex.CAR)
+PLAYER=Utils.scale_image(pygame.image.load(ex.CAR),0.5)
 START_POS = (180, 200)
 class CarProperties:
     """class for car properties"""
     def __init__(self, max_vel, rotation_vel):
         """class constructor
 
         Parameters:
@@ -38,15 +38,15 @@
         right (boolean): turn right if true 
         """
         if left:
             self.angle += self.rotation_vel
         elif right:
             self.angle -= self.rotation_vel
         Utils.rotation=self.angle % 360
-
+    
     def draw(self, win):
         """function to draw images
         Parameters:
         win (pygameobj): imput window
         """
         Utils.blit_rotate_center(win, self.img, (self.x_value-4, self.y_value-2), self.angle)
 
@@ -100,13 +100,19 @@
     """Player car class"""
     IMG = PLAYER
     #@classmethod
     def reduce_speed(self):
         """function to reduce speed"""
         self.vel = max(self.vel - self.acceleration / 2, 0)
         self.move()
-
+    def control(self,speed,rotation_vel):
+        """simpler"""
+        self.angle+=rotation_vel
+        self.vel = min(self.vel + speed, self.max_vel)
+        Utils.speed=self.vel
+        Utils.rotation=self.angle%360
+        self.move()
 def draw(win, player_car,background):
     """function to draw character and background"""
     win.blit(background,(0,0))
     player_car.draw(win)
     pygame.display.update()
```

### Comparing `taisim-0.0.2/src/taisim/sensor.py` & `taisim-0.0.3/src/taisim/sensor.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.2/src/taisim/simulator.py` & `taisim-0.0.3/src/taisim/simulator.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.2/src/taisim/utils.py` & `taisim-0.0.3/src/taisim/utils.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.2/src/taisim.egg-info/PKG-INFO` & `taisim-0.0.3/src/taisim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taisim
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple python3 simulator for advanced driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut@outlook.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Platform: UNKNOWN
```

### Comparing `taisim-0.0.2/src/taisim.egg-info/SOURCES.txt` & `taisim-0.0.3/src/taisim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

