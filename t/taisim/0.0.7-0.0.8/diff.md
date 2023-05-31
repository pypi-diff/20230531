# Comparing `tmp/taisim-0.0.7.tar.gz` & `tmp/taisim-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taisim-0.0.7.tar", last modified: Wed May 31 19:27:26 2023, max compression
+gzip compressed data, was "taisim-0.0.8.tar", last modified: Wed May 31 19:28:56 2023, max compression
```

## Comparing `taisim-0.0.7.tar` & `taisim-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:27:26.657560 taisim-0.0.7/
--rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-30 21:36:27.000000 taisim-0.0.7/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       37 2023-05-30 21:36:27.000000 taisim-0.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      423 2023-05-30 21:36:27.000000 taisim-0.0.7/NEWS.txt
--rw-r--r--   0 root         (0) staff       (20)      678 2023-05-31 19:27:26.656933 taisim-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3613 2023-05-30 21:36:27.000000 taisim-0.0.7/README.rst
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-31 19:27:26.657809 taisim-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1619 2023-05-31 19:27:02.000000 taisim-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:27:26.637570 taisim-0.0.7/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:27:26.646597 taisim-0.0.7/src/taisim/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.7/src/taisim/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:27:26.653426 taisim-0.0.7/src/taisim/components/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.7/src/taisim/components/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-30 21:36:27.000000 taisim-0.0.7/src/taisim/components/log.py
--rw-r--r--   0 root         (0) staff       (20)     1230 2023-05-30 21:36:27.000000 taisim-0.0.7/src/taisim/components/video.py
--rw-r--r--   0 root         (0) staff       (20)     1439 2023-05-31 19:27:24.000000 taisim-0.0.7/src/taisim/external_data.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:27:26.656108 taisim-0.0.7/src/taisim/gui/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.7/src/taisim/gui/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8155 2023-05-30 21:36:27.000000 taisim-0.0.7/src/taisim/gui/help_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3895 2023-05-30 21:36:27.000000 taisim-0.0.7/src/taisim/gui/sensor_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-05-31 17:40:43.000000 taisim-0.0.7/src/taisim/player.py
--rw-r--r--   0 root         (0) staff       (20)    17862 2023-05-30 21:36:27.000000 taisim-0.0.7/src/taisim/sensor.py
--rw-r--r--   0 root         (0) staff       (20)     3417 2023-05-31 19:26:52.000000 taisim-0.0.7/src/taisim/simulator.py
--rw-r--r--   0 root         (0) staff       (20)     9889 2023-05-30 21:36:27.000000 taisim-0.0.7/src/taisim/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:27:26.651551 taisim-0.0.7/src/taisim.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      678 2023-05-31 19:27:26.000000 taisim-0.0.7/src/taisim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      601 2023-05-31 19:27:26.000000 taisim-0.0.7/src/taisim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-31 19:27:26.000000 taisim-0.0.7/src/taisim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       40 2023-05-31 19:27:26.000000 taisim-0.0.7/src/taisim.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 21:36:48.000000 taisim-0.0.7/src/taisim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       21 2023-05-31 19:27:26.000000 taisim-0.0.7/src/taisim.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        7 2023-05-31 19:27:26.000000 taisim-0.0.7/src/taisim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:28:56.111539 taisim-0.0.8/
+-rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-30 21:36:27.000000 taisim-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)       37 2023-05-30 21:36:27.000000 taisim-0.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      423 2023-05-30 21:36:27.000000 taisim-0.0.8/NEWS.txt
+-rw-r--r--   0 root         (0) staff       (20)      678 2023-05-31 19:28:56.110640 taisim-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3613 2023-05-30 21:36:27.000000 taisim-0.0.8/README.rst
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-31 19:28:56.111879 taisim-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1619 2023-05-31 19:28:41.000000 taisim-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:28:56.089287 taisim-0.0.8/src/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:28:56.098661 taisim-0.0.8/src/taisim/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.8/src/taisim/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:28:56.106207 taisim-0.0.8/src/taisim/components/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.8/src/taisim/components/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-30 21:36:27.000000 taisim-0.0.8/src/taisim/components/log.py
+-rw-r--r--   0 root         (0) staff       (20)     1230 2023-05-30 21:36:27.000000 taisim-0.0.8/src/taisim/components/video.py
+-rw-r--r--   0 root         (0) staff       (20)     1439 2023-05-31 19:28:54.000000 taisim-0.0.8/src/taisim/external_data.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:28:56.109294 taisim-0.0.8/src/taisim/gui/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.8/src/taisim/gui/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8155 2023-05-30 21:36:27.000000 taisim-0.0.8/src/taisim/gui/help_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3895 2023-05-30 21:36:27.000000 taisim-0.0.8/src/taisim/gui/sensor_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3875 2023-05-31 17:40:43.000000 taisim-0.0.8/src/taisim/player.py
+-rw-r--r--   0 root         (0) staff       (20)    17862 2023-05-30 21:36:27.000000 taisim-0.0.8/src/taisim/sensor.py
+-rw-r--r--   0 root         (0) staff       (20)     3406 2023-05-31 19:28:31.000000 taisim-0.0.8/src/taisim/simulator.py
+-rw-r--r--   0 root         (0) staff       (20)     9889 2023-05-30 21:36:27.000000 taisim-0.0.8/src/taisim/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:28:56.103851 taisim-0.0.8/src/taisim.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      678 2023-05-31 19:28:56.000000 taisim-0.0.8/src/taisim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      601 2023-05-31 19:28:56.000000 taisim-0.0.8/src/taisim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-31 19:28:56.000000 taisim-0.0.8/src/taisim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       40 2023-05-31 19:28:56.000000 taisim-0.0.8/src/taisim.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 21:36:48.000000 taisim-0.0.8/src/taisim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-05-31 19:28:56.000000 taisim-0.0.8/src/taisim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        7 2023-05-31 19:28:56.000000 taisim-0.0.8/src/taisim.egg-info/top_level.txt
```

### Comparing `taisim-0.0.7/LICENSE` & `taisim-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `taisim-0.0.7/PKG-INFO` & `taisim-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taisim
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple python3 simulator for advanced driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut@outlook.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Platform: UNKNOWN
```

### Comparing `taisim-0.0.7/README.rst` & `taisim-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `taisim-0.0.7/setup.py` & `taisim-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # For more details, see:
     # http://packages.python.org/distribute/setuptools.html#declaring-dependencies
     'requests'	
 ]
 
 
 setup(name='taisim',
-    version='0.0.7',
+    version='0.0.8',
     description="Simple python3 simulator for advanced driving systems",
     long_description="simple python simulator for advanced driving systems",
     
     keywords='Simulator computer vision Advanced Driving',
     author='Tucudean Adrian-Ionut',
     author_email='Tucudean.Adrian.Ionut@outlook.com',
     url='https://github.com/Amporu/SparkVerse',
```

### Comparing `taisim-0.0.7/src/taisim/components/log.py` & `taisim-0.0.8/src/taisim/components/log.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.7/src/taisim/components/video.py` & `taisim-0.0.8/src/taisim/components/video.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.7/src/taisim/external_data.py` & `taisim-0.0.8/src/taisim/external_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 autor: Tucudean Adrian-Ionut
 date: 22.05.2023
 email: Tucudean.Adrian.Ionut@outlook.com
 license: MIT
 """
 import os
 from taisim.components.log import logger
-VERSION='0.0.7'
+VERSION='0.0.8'
 logger.info("VERSION : \033[92m%s\033[0m",VERSION)
 CAR    = os.path.join(os.path.dirname(__file__), 'data/player.png')
 LEVEL1 = os.path.join(os.path.dirname(__file__), 'data/LineFollower1.png')
 LEVEL2 = os.path.join(os.path.dirname(__file__), 'data/LineFollower2.png')
 LEVEL3 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper1.png')
 LEVEL4 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper2.png')
 LEVEL5 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper3.png')
```

### Comparing `taisim-0.0.7/src/taisim/gui/help_bar.py` & `taisim-0.0.8/src/taisim/gui/help_bar.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.7/src/taisim/gui/sensor_bar.py` & `taisim-0.0.8/src/taisim/gui/sensor_bar.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.7/src/taisim/player.py` & `taisim-0.0.8/src/taisim/player.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.7/src/taisim/sensor.py` & `taisim-0.0.8/src/taisim/sensor.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.7/src/taisim/simulator.py` & `taisim-0.0.8/src/taisim/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
     @staticmethod
     def control(linear_vel,angular_vel):
         """simpler"""
         Simulator.player_car.angle+=angular_vel
         if linear_vel==0:
             Simulator.player_car.vel=0
-        if
         Simulator.player_car.vel = min(Simulator.player_car.vel + linear_vel, Simulator.player_car.max_vel)
         Utils.speed=Simulator.player_car.vel
         Utils.rotation=Simulator.player_car.angle%360
         Simulator.player_car.move()
     def data():
         """function that returns simulator variables"""
         return (Simulator.WIN,
```

### Comparing `taisim-0.0.7/src/taisim/utils.py` & `taisim-0.0.8/src/taisim/utils.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.7/src/taisim.egg-info/PKG-INFO` & `taisim-0.0.8/src/taisim.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taisim
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple python3 simulator for advanced driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut@outlook.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Platform: UNKNOWN
```

### Comparing `taisim-0.0.7/src/taisim.egg-info/SOURCES.txt` & `taisim-0.0.8/src/taisim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

