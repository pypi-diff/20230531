# Comparing `tmp/mpscenes-0.4.1.tar.gz` & `tmp/mpscenes-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpscenes-0.4.1.tar", max compression
+gzip compressed data, was "mpscenes-0.4.2.tar", max compression
```

## Comparing `mpscenes-0.4.1.tar` & `mpscenes-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       71 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/.__init__.py
--rw-r--r--   0        0        0       71 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/__init__.py
--rw-r--r--   0        0        0     1161 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/analytic_trajectory.py
--rw-r--r--   0        0        0     1684 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/component.py
--rw-r--r--   0        0        0      500 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/errors.py
--rw-r--r--   0        0        0      755 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/reference_trajectory.py
--rw-r--r--   0        0        0     3271 2023-05-31 08:15:45.356129 mpscenes-0.4.1/mpscenes/common/spline_trajectory.py
--rw-r--r--   0        0        0     3314 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/dynamic_sub_goal.py
--rw-r--r--   0        0        0     2513 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/goal_composition.py
--rw-r--r--   0        0        0     1961 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/static_joint_space_sub_goal.py
--rw-r--r--   0        0        0     2642 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/static_sub_goal.py
--rw-r--r--   0        0        0     1958 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/sub_goal.py
--rw-r--r--   0        0        0      905 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/goals/sub_goal_creator.py
--rw-r--r--   0        0        0     3985 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/box_obstacle.py
--rw-r--r--   0        0        0       14 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/box_smooth.mtl
--rw-r--r--   0        0        0      836 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/box_smooth.obj
--rw-r--r--   0        0        0     3646 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/collision_obstacle.py
--rw-r--r--   0        0        0     3759 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/cylinder_obstacle.py
--rw-r--r--   0        0        0     1227 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_box_obstacle.py
--rw-r--r--   0        0        0     1312 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_cylinder_obstacle.py
--rw-r--r--   0        0        0     2901 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_obstacle.py
--rw-r--r--   0        0        0     1278 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_sphere_obstacle.py
--rw-r--r--   0        0        0     1244 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/dynamic_urdf_obstacle.py
--rw-r--r--   0        0        0      817 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/obstacleCreator.py
--rw-r--r--   0        0        0     3098 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/sphere_obstacle.py
--rw-r--r--   0        0        0      136 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/sphere_smooth.mtl
--rw-r--r--   0        0        0   111602 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/sphere_smooth.obj
--rw-r--r--   0        0        0     1833 2023-05-31 08:15:45.360129 mpscenes-0.4.1/mpscenes/obstacles/urdf_obstacle.py
--rw-r--r--   0        0        0      551 2023-05-31 08:15:45.360129 mpscenes-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 mpscenes-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/.__init__.py
+-rw-r--r--   0        0        0       71 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/__init__.py
+-rw-r--r--   0        0        0     1161 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/common/analytic_trajectory.py
+-rw-r--r--   0        0        0     1684 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/common/component.py
+-rw-r--r--   0        0        0      500 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/common/errors.py
+-rw-r--r--   0        0        0      755 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/common/reference_trajectory.py
+-rw-r--r--   0        0        0     3271 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/common/spline_trajectory.py
+-rw-r--r--   0        0        0     3314 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/goals/dynamic_sub_goal.py
+-rw-r--r--   0        0        0     2513 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/goals/goal_composition.py
+-rw-r--r--   0        0        0     1961 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/goals/static_joint_space_sub_goal.py
+-rw-r--r--   0        0        0     2642 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/goals/static_sub_goal.py
+-rw-r--r--   0        0        0     1958 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/goals/sub_goal.py
+-rw-r--r--   0        0        0      905 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/goals/sub_goal_creator.py
+-rw-r--r--   0        0        0     3985 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/box_obstacle.py
+-rw-r--r--   0        0        0       14 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/box_smooth.mtl
+-rw-r--r--   0        0        0      836 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/box_smooth.obj
+-rw-r--r--   0        0        0     3873 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/collision_obstacle.py
+-rw-r--r--   0        0        0     3759 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/cylinder_obstacle.py
+-rw-r--r--   0        0        0     1227 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/dynamic_box_obstacle.py
+-rw-r--r--   0        0        0     1312 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/dynamic_cylinder_obstacle.py
+-rw-r--r--   0        0        0     2901 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/dynamic_obstacle.py
+-rw-r--r--   0        0        0     1278 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/dynamic_sphere_obstacle.py
+-rw-r--r--   0        0        0     1244 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/dynamic_urdf_obstacle.py
+-rw-r--r--   0        0        0      817 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/obstacleCreator.py
+-rw-r--r--   0        0        0     3098 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/sphere_obstacle.py
+-rw-r--r--   0        0        0      136 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/sphere_smooth.mtl
+-rw-r--r--   0        0        0   111602 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/sphere_smooth.obj
+-rw-r--r--   0        0        0     1833 2023-05-31 08:57:28.245750 mpscenes-0.4.2/mpscenes/obstacles/urdf_obstacle.py
+-rw-r--r--   0        0        0      551 2023-05-31 08:57:28.245750 mpscenes-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 mpscenes-0.4.2/PKG-INFO
```

### Comparing `mpscenes-0.4.1/mpscenes/common/analytic_trajectory.py` & `mpscenes-0.4.2/mpscenes/common/analytic_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/common/component.py` & `mpscenes-0.4.2/mpscenes/common/component.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/common/reference_trajectory.py` & `mpscenes-0.4.2/mpscenes/common/reference_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/common/spline_trajectory.py` & `mpscenes-0.4.2/mpscenes/common/spline_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/goals/dynamic_sub_goal.py` & `mpscenes-0.4.2/mpscenes/goals/dynamic_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/goals/goal_composition.py` & `mpscenes-0.4.2/mpscenes/goals/goal_composition.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/goals/static_joint_space_sub_goal.py` & `mpscenes-0.4.2/mpscenes/goals/static_joint_space_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/goals/static_sub_goal.py` & `mpscenes-0.4.2/mpscenes/goals/static_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/goals/sub_goal.py` & `mpscenes-0.4.2/mpscenes/goals/sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/goals/sub_goal_creator.py` & `mpscenes-0.4.2/mpscenes/goals/sub_goal_creator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/box_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/box_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/box_smooth.obj` & `mpscenes-0.4.2/mpscenes/obstacles/box_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/collision_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/collision_obstacle.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     of an obstacle. This class is further specified for the other obstacles.
 
     Parameters:
     ------------
 
     position: list: Position of the obstacle
     orientation: list: Orientation of the obstacle
+    color: list: RGB-A color code
     """
 
     position: List[float] = field(default_factory=lambda: [0.0, 0.0, 0.0])
     orientation: List[float] = field(default_factory=lambda: [1.0, 0.0, 0.0, 0.0])
 
 
 @dataclass
@@ -71,21 +72,23 @@
     ------------
 
     type : str : Type of the obstacle
     geometry : GeometryConfig : Geometry of the obstacle
     movable : bool : Flag indicating whether an obstacle can be pushed around
     low : GeometryConfig : Lower limit for randomization
     high : GeometryConfig : Upper limit for randomization
+    rgba: list: Color in rgba encoding
     """
 
     type: str
     geometry: GeometryConfig
     movable: bool = False
     low: Optional[GeometryConfig] = None
     high: Optional[GeometryConfig] = None
+    rgba: List[float] = field(default_factory=lambda: [0.0, 0.0, 0.0, 1.0])
 
 
 class CollisionObstacle(MPComponent):
     def type(self) -> str:
         return self._config.type
 
     def geometry(self) -> GeometryConfig:
@@ -103,14 +106,17 @@
 
     def orientation(self, **kwarg) -> np.ndarray:
         return np.array(self.geometry().orientation)
 
     def position(self, **kwargs) -> np.ndarray:
         return np.array(self.geometry().position)
 
+    def rgba(self) -> np.ndarray:
+        return np.array(self._config.rgba)
+
     def velocity(self, **kwargs) -> np.ndarray:
         return np.zeros(self.dimension())
 
     def acceleration(self, **kwargs) -> np.ndarray:
         return np.zeros(self.dimension())
 
     def movable(self) -> bool:
```

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/cylinder_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/cylinder_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/dynamic_box_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/dynamic_box_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/dynamic_cylinder_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/dynamic_cylinder_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/dynamic_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/dynamic_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/dynamic_sphere_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/dynamic_sphere_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/dynamic_urdf_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/dynamic_urdf_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/obstacleCreator.py` & `mpscenes-0.4.2/mpscenes/obstacles/obstacleCreator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/sphere_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/sphere_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/sphere_smooth.obj` & `mpscenes-0.4.2/mpscenes/obstacles/sphere_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/mpscenes/obstacles/urdf_obstacle.py` & `mpscenes-0.4.2/mpscenes/obstacles/urdf_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.1/pyproject.toml` & `mpscenes-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpscenes"
-version = "0.4.1"
+version = "0.4.2"
 description = "Generic motion planning scenes, including goals and obstacles."
 authors = ["Max <m.spahn@tudelft.nl>"]
   
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.22.0"
```

### Comparing `mpscenes-0.4.1/PKG-INFO` & `mpscenes-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpscenes
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generic motion planning scenes, including goals and obstacles.
 Author: Max
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

