# Comparing `tmp/mpscenes-0.4.0.tar.gz` & `tmp/mpscenes-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpscenes-0.4.0.tar", max compression
+gzip compressed data, was "mpscenes-0.4.1.tar", max compression
```

## Comparing `mpscenes-0.4.0.tar` & `mpscenes-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       71 2023-05-10 09:47:35.022060 mpscenes-0.4.0/mpscenes/.__init__.py
--rw-r--r--   0        0        0       71 2023-05-10 09:47:35.022060 mpscenes-0.4.0/mpscenes/__init__.py
--rw-r--r--   0        0        0     1161 2023-05-10 09:47:35.022060 mpscenes-0.4.0/mpscenes/common/analytic_trajectory.py
--rw-r--r--   0        0        0     1684 2023-05-10 09:47:35.022060 mpscenes-0.4.0/mpscenes/common/component.py
--rw-r--r--   0        0        0      500 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/common/errors.py
--rw-r--r--   0        0        0      755 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/common/reference_trajectory.py
--rw-r--r--   0        0        0     3271 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/common/spline_trajectory.py
--rw-r--r--   0        0        0     3314 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/dynamic_sub_goal.py
--rw-r--r--   0        0        0     2513 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/goal_composition.py
--rw-r--r--   0        0        0     1961 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/static_joint_space_sub_goal.py
--rw-r--r--   0        0        0     2642 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/static_sub_goal.py
--rw-r--r--   0        0        0     1958 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/sub_goal.py
--rw-r--r--   0        0        0      905 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/sub_goal_creator.py
--rw-r--r--   0        0        0     4045 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/box_obstacle.py
--rw-r--r--   0        0        0       14 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/box_smooth.mtl
--rw-r--r--   0        0        0      836 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/box_smooth.obj
--rw-r--r--   0        0        0     2217 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/collision_obstacle.py
--rw-r--r--   0        0        0     3747 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/cylinder_obstacle.py
--rw-r--r--   0        0        0     1227 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_box_obstacle.py
--rw-r--r--   0        0        0     1312 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_cylinder_obstacle.py
--rw-r--r--   0        0        0     2901 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_obstacle.py
--rw-r--r--   0        0        0     1278 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_sphere_obstacle.py
--rw-r--r--   0        0        0     1244 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_urdf_obstacle.py
--rw-r--r--   0        0        0      817 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/obstacleCreator.py
--rw-r--r--   0        0        0     3092 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/sphere_obstacle.py
--rw-r--r--   0        0        0      136 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/sphere_smooth.mtl
--rw-r--r--   0        0        0   111602 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/sphere_smooth.obj
--rw-r--r--   0        0        0     1833 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/urdf_obstacle.py
--rw-r--r--   0        0        0      551 2023-05-10 09:47:35.026060 mpscenes-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 mpscenes-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/.__init__.py
+-rw-r--r--   0        0        0       71 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/__init__.py
+-rw-r--r--   0        0        0     1161 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/analytic_trajectory.py
+-rw-r--r--   0        0        0     1684 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/component.py
+-rw-r--r--   0        0        0      500 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/errors.py
+-rw-r--r--   0        0        0      755 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/reference_trajectory.py
+-rw-r--r--   0        0        0     3271 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/spline_trajectory.py
+-rw-r--r--   0        0        0     3314 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/dynamic_sub_goal.py
+-rw-r--r--   0        0        0     2513 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/goal_composition.py
+-rw-r--r--   0        0        0     1961 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/static_joint_space_sub_goal.py
+-rw-r--r--   0        0        0     2642 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/static_sub_goal.py
+-rw-r--r--   0        0        0     1958 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/sub_goal.py
+-rw-r--r--   0        0        0      905 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/sub_goal_creator.py
+-rw-r--r--   0        0        0     3985 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/box_obstacle.py
+-rw-r--r--   0        0        0       14 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/box_smooth.mtl
+-rw-r--r--   0        0        0      836 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/box_smooth.obj
+-rw-r--r--   0        0        0     3646 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/collision_obstacle.py
+-rw-r--r--   0        0        0     3759 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/cylinder_obstacle.py
+-rw-r--r--   0        0        0     1227 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_box_obstacle.py
+-rw-r--r--   0        0        0     1312 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_cylinder_obstacle.py
+-rw-r--r--   0        0        0     2901 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_obstacle.py
+-rw-r--r--   0        0        0     1278 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_sphere_obstacle.py
+-rw-r--r--   0        0        0     1244 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_urdf_obstacle.py
+-rw-r--r--   0        0        0      817 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/obstacleCreator.py
+-rw-r--r--   0        0        0     3098 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/sphere_obstacle.py
+-rw-r--r--   0        0        0      136 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/sphere_smooth.mtl
+-rw-r--r--   0        0        0   111602 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/sphere_smooth.obj
+-rw-r--r--   0        0        0     1833 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/urdf_obstacle.py
+-rw-r--r--   0        0        0      551 2023-05-31 08:15:45.360129 mpscenes-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 mpscenes-0.4.1/PKG-INFO
```

### Comparing `mpscenes-0.4.0/mpscenes/common/analytic_trajectory.py` & `mpscenes-0.4.1/mpscenes/common/analytic_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/common/component.py` & `mpscenes-0.4.1/mpscenes/common/component.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/common/reference_trajectory.py` & `mpscenes-0.4.1/mpscenes/common/reference_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/common/spline_trajectory.py` & `mpscenes-0.4.1/mpscenes/common/spline_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/goals/dynamic_sub_goal.py` & `mpscenes-0.4.1/mpscenes/goals/dynamic_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/goals/goal_composition.py` & `mpscenes-0.4.1/mpscenes/goals/goal_composition.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/goals/static_joint_space_sub_goal.py` & `mpscenes-0.4.1/mpscenes/goals/static_joint_space_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/goals/static_sub_goal.py` & `mpscenes-0.4.1/mpscenes/goals/static_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/goals/sub_goal.py` & `mpscenes-0.4.1/mpscenes/goals/sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/goals/sub_goal_creator.py` & `mpscenes-0.4.1/mpscenes/goals/sub_goal_creator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/box_obstacle.py` & `mpscenes-0.4.1/mpscenes/obstacles/box_obstacle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from dataclasses import dataclass
 from typing import Optional
-import os
 import numpy as np
 from omegaconf import OmegaConf
 
 from mpscenes.obstacles.collision_obstacle import CollisionObstacle, CollisionObstacleConfig, GeometryConfig
-from mpscenes.common.errors import DimensionNotSuitableForEnv
 
 
 @dataclass
 class BoxGeometryConfig(GeometryConfig):
     """Configuration dataclass for geometry.
 
     This configuration class holds information about position
@@ -19,16 +17,16 @@
     ------------
 
     length: float: Length of the box
     width: float: Width of the box
     height: float: Height of the box
     """
 
-    length: float
-    width: float
+    length: float = 1.0
+    width: float = 1.0
     height: float = 1.0
 
 
 @dataclass
 class BoxObstacleConfig(CollisionObstacleConfig):
     """Configuration dataclass for box obstacle.
```

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/box_smooth.obj` & `mpscenes-0.4.1/mpscenes/obstacles/box_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/cylinder_obstacle.py` & `mpscenes-0.4.1/mpscenes/obstacles/cylinder_obstacle.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     Parameters:
     ------------
 
     radius: float: Radius of the cylinder
     height: float: Height of the cylinder
     """
 
-    radius: float
-    height: float
+    radius: float = 1.0
+    height: float = 1.0
 
 
 @dataclass
 class CylinderObstacleConfig(CollisionObstacleConfig):
     """Configuration dataclass for box obstacle.
 
     This configuration class holds information about the position, size
```

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/dynamic_box_obstacle.py` & `mpscenes-0.4.1/mpscenes/obstacles/dynamic_box_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/dynamic_cylinder_obstacle.py` & `mpscenes-0.4.1/mpscenes/obstacles/dynamic_cylinder_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/dynamic_obstacle.py` & `mpscenes-0.4.1/mpscenes/obstacles/dynamic_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/dynamic_sphere_obstacle.py` & `mpscenes-0.4.1/mpscenes/obstacles/dynamic_sphere_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/dynamic_urdf_obstacle.py` & `mpscenes-0.4.1/mpscenes/obstacles/dynamic_urdf_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/obstacleCreator.py` & `mpscenes-0.4.1/mpscenes/obstacles/obstacleCreator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/sphere_obstacle.py` & `mpscenes-0.4.1/mpscenes/obstacles/sphere_obstacle.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Parameters:
     ------------
 
     radius: float: Radius of the obstacle
     """
 
-    radius: float
+    radius: float = 1.0
 
 
 @dataclass
 class SphereObstacleConfig(CollisionObstacleConfig):
     """Configuration dataclass for sphere obstacle.
 
     This configuration class holds information about the position, size
```

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/sphere_smooth.obj` & `mpscenes-0.4.1/mpscenes/obstacles/sphere_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/mpscenes/obstacles/urdf_obstacle.py` & `mpscenes-0.4.1/mpscenes/obstacles/urdf_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.0/pyproject.toml` & `mpscenes-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpscenes"
-version = "0.4.0"
+version = "0.4.1"
 description = "Generic motion planning scenes, including goals and obstacles."
 authors = ["Max <m.spahn@tudelft.nl>"]
   
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.22.0"
```

### Comparing `mpscenes-0.4.0/PKG-INFO` & `mpscenes-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpscenes
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generic motion planning scenes, including goals and obstacles.
 Author: Max
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

