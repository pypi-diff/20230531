# Comparing `tmp/taisim-0.0.1.tar.gz` & `tmp/taisim-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taisim-0.0.1.tar", last modified: Sun May 28 14:52:10 2023, max compression
+gzip compressed data, was "taisim-0.0.2.tar", last modified: Tue May 30 21:57:48 2023, max compression
```

## Comparing `taisim-0.0.1.tar` & `taisim-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,32 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-28 14:52:10.845446 taisim-0.0.1/
--rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-27 07:23:21.000000 taisim-0.0.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       37 2023-05-27 07:23:21.000000 taisim-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      423 2023-05-27 07:23:21.000000 taisim-0.0.1/NEWS.txt
--rw-r--r--   0 root         (0) staff       (20)      659 2023-05-28 14:52:10.844776 taisim-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3613 2023-05-27 07:23:21.000000 taisim-0.0.1/README.rst
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-28 14:52:10.845585 taisim-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1619 2023-05-28 14:23:13.000000 taisim-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-28 14:52:10.809795 taisim-0.0.1/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-28 14:52:10.818147 taisim-0.0.1/src/taisim/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-28 14:52:10.827149 taisim-0.0.1/src/taisim/components/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/components/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/components/log.py
--rw-r--r--   0 root         (0) staff       (20)     1230 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/components/video.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-28 14:52:10.842171 taisim-0.0.1/src/taisim/data/
--rwxr-xr-x   0 root         (0) staff       (20)    28453 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/data/Cropps1.png
--rwxr-xr-x   0 root         (0) staff       (20)    28684 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/data/Cropps2.png
--rwxr-xr-x   0 root         (0) staff       (20)    26184 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/data/LaneKeeper1.png
--rwxr-xr-x   0 root         (0) staff       (20)    26228 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/data/LaneKeeper2.png
--rwxr-xr-x   0 root         (0) staff       (20)    25273 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/data/LaneKeeper3.png
--rwxr-xr-x   0 root         (0) staff       (20)    76717 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/data/LineFollower1.png
--rwxr-xr-x   0 root         (0) staff       (20)    17710 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/data/LineFollower2.png
--rw-r--r--   0 root         (0) staff       (20)      899 2023-05-27 07:41:50.000000 taisim-0.0.1/src/taisim/data/compass.png
--rw-r--r--   0 root         (0) staff       (20)    46864 2023-05-27 07:41:27.000000 taisim-0.0.1/src/taisim/data/logo.png
--rwxr-xr-x   0 root         (0) staff       (20)      152 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/data/player.png
--rw-r--r--   0 root         (0) staff       (20)     1037 2023-05-27 07:41:43.000000 taisim-0.0.1/src/taisim/data/position.png
--rw-r--r--   0 root         (0) staff       (20)     1432 2023-05-27 07:46:19.000000 taisim-0.0.1/src/taisim/external_data.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-28 14:52:10.844076 taisim-0.0.1/src/taisim/gui/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/gui/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8155 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/gui/help_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3895 2023-05-27 07:23:21.000000 taisim-0.0.1/src/taisim/gui/sensor_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3566 2023-05-27 07:24:41.000000 taisim-0.0.1/src/taisim/player.py
--rw-r--r--   0 root         (0) staff       (20)    17862 2023-05-28 14:52:09.000000 taisim-0.0.1/src/taisim/sensor.py
--rw-r--r--   0 root         (0) staff       (20)     2987 2023-05-27 07:24:38.000000 taisim-0.0.1/src/taisim/simulator.py
--rw-r--r--   0 root         (0) staff       (20)     9889 2023-05-28 14:46:40.000000 taisim-0.0.1/src/taisim/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-28 14:52:10.824784 taisim-0.0.1/src/taisim.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      659 2023-05-28 14:52:10.000000 taisim-0.0.1/src/taisim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      930 2023-05-28 14:52:10.000000 taisim-0.0.1/src/taisim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-28 14:52:10.000000 taisim-0.0.1/src/taisim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       39 2023-05-28 14:52:10.000000 taisim-0.0.1/src/taisim.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-27 07:26:03.000000 taisim-0.0.1/src/taisim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       21 2023-05-28 14:52:10.000000 taisim-0.0.1/src/taisim.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        7 2023-05-28 14:52:10.000000 taisim-0.0.1/src/taisim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.997840 taisim-0.0.2/
+-rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-30 21:36:27.000000 taisim-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)       37 2023-05-30 21:36:27.000000 taisim-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      423 2023-05-30 21:36:27.000000 taisim-0.0.2/NEWS.txt
+-rw-r--r--   0 root         (0) staff       (20)      678 2023-05-30 21:57:47.997187 taisim-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3613 2023-05-30 21:36:27.000000 taisim-0.0.2/README.rst
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-30 21:57:47.998077 taisim-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1619 2023-05-30 21:56:46.000000 taisim-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.979991 taisim-0.0.2/src/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.986223 taisim-0.0.2/src/taisim/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.994673 taisim-0.0.2/src/taisim/components/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/components/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/components/log.py
+-rw-r--r--   0 root         (0) staff       (20)     1230 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/components/video.py
+-rw-r--r--   0 root         (0) staff       (20)     1439 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/external_data.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.996348 taisim-0.0.2/src/taisim/gui/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/gui/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8155 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/gui/help_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3895 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/gui/sensor_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3566 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/player.py
+-rw-r--r--   0 root         (0) staff       (20)    17862 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/sensor.py
+-rw-r--r--   0 root         (0) staff       (20)     2987 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/simulator.py
+-rw-r--r--   0 root         (0) staff       (20)     9889 2023-05-30 21:36:27.000000 taisim-0.0.2/src/taisim/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 21:57:47.992796 taisim-0.0.2/src/taisim.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      678 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      601 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       40 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 21:36:48.000000 taisim-0.0.2/src/taisim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        7 2023-05-30 21:57:47.000000 taisim-0.0.2/src/taisim.egg-info/top_level.txt
```

### Comparing `taisim-0.0.1/LICENSE` & `taisim-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/PKG-INFO` & `taisim-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: taisim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple python3 simulator for advanced driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut@outlook.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
 
 simple python simulator for advanced driving systems
+
```

### Comparing `taisim-0.0.1/README.rst` & `taisim-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/setup.py` & `taisim-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # For more details, see:
     # http://packages.python.org/distribute/setuptools.html#declaring-dependencies
     'requests'	
 ]
 
 
 setup(name='taisim',
-    version='0.0.1',
+    version='0.0.2',
     description="Simple python3 simulator for advanced driving systems",
     long_description="simple python simulator for advanced driving systems",
     
     keywords='Simulator computer vision Advanced Driving',
     author='Tucudean Adrian-Ionut',
     author_email='Tucudean.Adrian.Ionut@outlook.com',
     url='https://github.com/Amporu/SparkVerse',
```

### Comparing `taisim-0.0.1/src/taisim/components/log.py` & `taisim-0.0.2/src/taisim/components/log.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/src/taisim/components/video.py` & `taisim-0.0.2/src/taisim/components/video.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/src/taisim/external_data.py` & `taisim-0.0.2/src/taisim/external_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 LEVEL1 = os.path.join(os.path.dirname(__file__), 'data/LineFollower1.png')
 LEVEL2 = os.path.join(os.path.dirname(__file__), 'data/LineFollower2.png')
 LEVEL3 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper1.png')
 LEVEL4 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper2.png')
 LEVEL5 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper3.png')
 LEVEL6 = os.path.join(os.path.dirname(__file__), 'data/Cropps1.png')
 LEVEL7 = os.path.join(os.path.dirname(__file__), 'data/Cropps2.png')
-LOGO   = os.path.join(os.path.dirname(__file__), 'data/logo.png')
+LOGO   = os.path.join(os.path.dirname(__file__), 'data/taisim_logo.png')
 COMPASS= os.path.join(os.path.dirname(__file__), 'data/compass.png')
 GPS    = os.path.join(os.path.dirname(__file__), 'data/position.png')
 if os.path.exists(CAR) and os.path.exists(LEVEL1) and os.path.exists(LOGO):
     logger.info("ASSETS : \033[92mOK\033[0m")
     logger.info("TRACK : \033[92mOK\033[0m")
 else:
     logger.error("ASSETS : \033[91mNOT FOUND\033[0m")
```

### Comparing `taisim-0.0.1/src/taisim/gui/help_bar.py` & `taisim-0.0.2/src/taisim/gui/help_bar.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/src/taisim/gui/sensor_bar.py` & `taisim-0.0.2/src/taisim/gui/sensor_bar.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/src/taisim/player.py` & `taisim-0.0.2/src/taisim/player.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/src/taisim/sensor.py` & `taisim-0.0.2/src/taisim/sensor.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/src/taisim/simulator.py` & `taisim-0.0.2/src/taisim/simulator.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/src/taisim/utils.py` & `taisim-0.0.2/src/taisim/utils.py`

 * *Files identical despite different names*

### Comparing `taisim-0.0.1/src/taisim.egg-info/PKG-INFO` & `taisim-0.0.2/src/taisim.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: taisim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple python3 simulator for advanced driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut@outlook.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
 
 simple python simulator for advanced driving systems
+
```

