# Comparing `tmp/honeybee-idaice-0.3.0.tar.gz` & `tmp/honeybee-idaice-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.3.0.tar", last modified: Mon May 29 23:33:41 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.3.1.tar", last modified: Wed May 31 14:04:22 2023, max compression
```

## Comparing `honeybee-idaice-0.3.0.tar` & `honeybee-idaice-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/geometry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/bldgbody.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20497 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/setup.py
```

### Comparing `honeybee-idaice-0.3.0/LICENSE` & `honeybee-idaice-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.0/PKG-INFO` & `honeybee-idaice-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.0
+Version: 0.3.1
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.3.0/README.md` & `honeybee-idaice-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.3.1/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.3.1/honeybee_idaice/geometry_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,39 @@
+from typing import List
+
 from ladybug_geometry.geometry3d import Point3D, Face3D
 from ladybug_geometry.geometry2d import Polygon2D, Point2D
 from honeybee.facetype import Floor, Wall
 from honeybee.room import Room
 
 
-def get_floor_boundary(room: Room):
+def get_rooms_boundary(rooms: List[Room]) -> List[Polygon2D]:
+    """Get a list of boundaries vertices for a list of rooms."""
+    floor_geom = []
+    for room in rooms:
+        for face in room.faces:
+            if isinstance(face.type, Floor):
+                floor_geom.append(face.geometry)
+    boundaries = []
+    # floors are most likely horizontal - let's make them 2D polygons
+    for floor in floor_geom:
+        boundary = Polygon2D(
+            [
+                Point2D(v.x, v.y) for v in floor.lower_left_counter_clockwise_vertices
+            ]
+        )
+        boundaries.append(boundary)
+
+    # find the union of the boundary polygons - tolerance is set to 1 to count for
+    # wall thickness
+    boundaries = Polygon2D.boolean_union_all(boundaries, tolerance=1)
+    return boundaries
+
+
+def get_floor_boundary(room: Room, llc=True):
     """Get a list of vertices for floor boundary for a room.
 
     This function joins all the floor faces and returns a list of Point3D that define the
     border of the floor in counter clockwise order starting from the lower left corner.
     """
     floor_geom = []
 
@@ -68,15 +93,19 @@
     boundary = [
         Point3D(point.x, point.y, z) for point in boundary.vertices
     ]
 
     geometry = Face3D(boundary, plane=floor_geom[0].plane)
     geometry = geometry.flip()
 
-    vertices = geometry.lower_left_counter_clockwise_vertices
+    if llc:
+        vertices = geometry.lower_left_counter_clockwise_vertices
+    else:
+        vertices = geometry.upper_right_counter_clockwise_vertices
+
     center = geometry.center
     if geometry.is_point_on_face(center, 0.01):
         pole = center
     else:
         pole = geometry.pole_of_inaccessibility(0.01)
 
     return vertices, pole
```

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.3.1/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.3.1/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.3.1/honeybee_idaice/templates/building.idm`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
  (:IREF :N "Zone_sup_cold")
  (:IREF :N "Zone_rtn_cold")
  (:IREF :N "DHW_ctl" :T IN :F 208))
 ((SOURCE-FILE :DOCUMENT-PATH "clim:Kalmar.prn" :SF "clim:Kalmar.prn" :N CLIMATE-FILE)
  (:VAR :N TAIR :V 6.92))
 ((AGGREGATE :N PROJDATA)
  (:PAR :N RESP_ENG :V "Ladybug Tools")
- (:PAR :N DESCR :V "This model is auto generated from an HBJSON file. At this point, only the geometry is translated. All the other information are set to default IDA ICE values."))
+ (:PAR :N DESCR :V "This model is auto-generated from an HBJSON file. At this point, the translator only translates the geometry information.Use the Pollination discourse forum if you have any questions or comments: https://discourse.pollination.cloud/"))
 ((AGGREGATE :N THREE-D-MODEL :T THREE-D-PLAN)
  ((AGGREGATE :N VIEWPT :T VIEWPOINT)
   (:PAR :N POSITION :V #(43.464907646758 -51.2386356058975 58.302492260347))
   (:PAR :N FOCALPOINT :V #(25.0 9.99499988555908 2.5))))
 (CONNECTIONS
  ((PLANT "Zone_rtn_cold") ((:LIB WATPLUG) OUTLET) 2 0 NIL)
  ((PLANT "Zone_sup_cold") ((:LIB WATPLUG) INLET) 2 0 NIL)
```

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.3.1/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.3.1/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.3.1/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.3.1/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.3.1/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.0
+Version: 0.3.1
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.3.0/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.3.1/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 requirements.txt
 setup.cfg
 setup.py
 honeybee_idaice/__init__.py
 honeybee_idaice/__main__.py
 honeybee_idaice/_extend_honeybee.py
 honeybee_idaice/archive.py
+honeybee_idaice/bldgbody.py
+honeybee_idaice/face.py
 honeybee_idaice/geometry_utils.py
+honeybee_idaice/shade.py
 honeybee_idaice/writer.py
 honeybee_idaice/writer_obj.py
 honeybee_idaice.egg-info/PKG-INFO
 honeybee_idaice.egg-info/SOURCES.txt
 honeybee_idaice.egg-info/dependency_links.txt
 honeybee_idaice.egg-info/entry_points.txt
 honeybee_idaice.egg-info/requires.txt
```

### Comparing `honeybee-idaice-0.3.0/setup.py` & `honeybee-idaice-0.3.1/setup.py`

 * *Files identical despite different names*

