# Comparing `tmp/honeybee-idaice-0.3.1.tar.gz` & `tmp/honeybee-idaice-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.3.1.tar", last modified: Wed May 31 14:04:22 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.3.2.tar", last modified: Wed May 31 18:51:55 2023, max compression
```

## Comparing `honeybee-idaice-0.3.1.tar` & `honeybee-idaice-0.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/bldgbody.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20497 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 14:04:22.000000 honeybee-idaice-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 14:03:14.000000 honeybee-idaice-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/bldgbody.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20497 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/setup.py
```

### Comparing `honeybee-idaice-0.3.1/LICENSE` & `honeybee-idaice-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/PKG-INFO` & `honeybee-idaice-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.1
+Version: 0.3.2
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.3.1/README.md` & `honeybee-idaice-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/archive.py` & `honeybee-idaice-0.3.2/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/bldgbody.py` & `honeybee-idaice-0.3.2/honeybee_idaice/bldgbody.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """A module for functions related to IDM building-bodies."""
 from typing import List
 from ladybug_geometry.bounding import bounding_box
 from ladybug_geometry.geometry2d import Polygon2D, Point2D
+from ladybug_geometry.geometry3d import Plane, LineSegment3D, Face3D
 
 from honeybee.room import Room
 from honeybee.facetype import RoofCeiling, Floor
 
 from .geometry_utils import get_floor_boundary, get_rooms_boundary
 
 
 def _section_to_idm_protected(rooms: List[Room]):
     if not rooms:
         return ''
-
+    XY_PLANE = Plane()
     sections = []
     for room in rooms:
         room_section = []
         vertices, _ = get_floor_boundary(room)
         min_pt, max_pt = bounding_box(room.geometry)
         ver_count = len(vertices)
         idm_vertices = ' '.join(f'({v.x} {v.y})' for v in vertices)
@@ -26,40 +27,100 @@
             f' (:PAR :N CORNERS :DIM ({ver_count} 2) :V #2A({idm_vertices}))\n' \
             f' (:PAR :N CONTOURS :V ({ver_count}))\n' \
             f' (:PAR :N HEIGHT :V {max_pt.z - min_pt.z})\n' \
             f' (:PAR :N BOTTOM :V {min_pt.z})'
         room_section.append(header)
         wall_count = 0
         floor_count = 0
-        roof_count = 0
         for face in room.faces:
-            if isinstance(face, RoofCeiling):
-                type_ = 'ROOF-FACE'
-                index = -1000 - roof_count
-                roof_count += 1
-            elif isinstance(face, Floor):
+            if isinstance(face.type, Floor):
                 type_ = 'CRAWL-FACE'
                 index = -2000 - floor_count
                 floor_count += 1
             else:
                 type_ = 'WALL-FACE'
                 index = wall_count + 1
                 wall_count += 1
+
             vertices = face.geometry.upper_right_counter_clockwise_vertices
             count = len(vertices)
             vertices_idm = ' '.join((
                 f'({v.x} {v.y} {v.z})' for v in vertices
             ))
-            body = f' ((FACE :N "{face.identifier}" :T {type_} :INDEX {index})\n' \
-                f'  (:PAR :N NCORN :V {count})\n' \
-                f'  (:PAR :N CORNERS :DIM ({count} 3) :V #2A({vertices_idm}))\n' \
-                f'  (:PAR :N SLOPE :V {face.altitude + 90})\n' \
-                f'  ((FACE :N GROUND-FACE)\n' \
-                f'  (:PAR :N NCORN :V 0)\n' \
-                f'  (:PAR :N CORNERS :DIM (0 3))))'
+
+            if type_ == 'CRAWL-FACE':
+                body = f' ((FACE :N "{face.identifier}" :T {type_} :INDEX {index})\n' \
+                    '  (:PAR :N NCORN :V 0)\n' \
+                    '  (:PAR :N CORNERS :DIM (0 3) :V #2A())\n' \
+                    '  ((FACE :N GROUND-FACE)\n' \
+                    f'  (:PAR :N NCORN :V {count})\n' \
+                    f'  (:PAR :N CORNERS :DIM ({count} 3) :V #2A({vertices_idm}))))'
+            else:
+                body = f' ((FACE :N "{face.identifier}" :T {type_} :INDEX {index})\n' \
+                    f'  (:PAR :N NCORN :V {count})\n' \
+                    f'  (:PAR :N CORNERS :DIM ({count} 3) :V #2A({vertices_idm}))\n' \
+                    f'  (:PAR :N SLOPE :V {face.altitude + 90})\n' \
+                    '  ((FACE :N GROUND-FACE)\n' \
+                    '  (:PAR :N NCORN :V 0)\n' \
+                    '  (:PAR :N CORNERS :DIM (0 3))))'
+
+            if type_ == 'WALL-FACE' and min_pt.z < -0.1:
+                # intersect the edges with the XY plane to create two separate segments
+                geometry = face.geometry
+                lines = geometry.intersect_plane(XY_PLANE)
+                if not lines:
+                    room_section.append(body)
+                    continue
+                # calculate the top and the bottom segments
+                line = lines[0]
+                pt_1 = line.p1
+                pt_2 = line.p2
+                vertices = list(geometry.upper_right_counter_clockwise_vertices)
+                top_part = [vertices[0]]
+                for vc, v in enumerate(vertices[1:]):
+                    line = LineSegment3D.from_end_points(top_part[-1], v)
+                    if line.distance_to_point(pt_1) < 0.001:
+                        top_part.extend([pt_1, pt_2])
+                        bottom_part = [pt_2, pt_1]
+                        other_point = pt_2
+                        break
+                    elif line.distance_to_point(pt_2) < 0.001:
+                        top_part.extend([pt_2, pt_1])
+                        bottom_part = [pt_1, pt_2]
+                        other_point = pt_1
+                        break
+                    top_part.append(v)
+
+                vertices_rev = list(reversed(vertices))[:-1]
+                top_part_2 = [vertices[0]]
+                for c, v in enumerate(vertices_rev):
+                    line = LineSegment3D.from_end_points(top_part_2[-1], v)
+                    if line.distance_to_point(other_point) < 0.001:
+                        indx = -(c + 1)
+                        if indx == -1:
+                            top_part = top_part + vertices[indx:-1]
+                            bottom_part = bottom_part + vertices[vc + 1:]
+                        else:
+                            top_part = top_part + vertices[indx + 1:]
+                            bottom_part = bottom_part + vertices[vc + 1:indx + 1]
+                    top_part_2.append(v)
+
+                up_count = len(top_part)
+                btm_count = len(bottom_part)
+                up_vertices = ' '.join(f'({v[0]} {v[1]} {v[2]})' for v in top_part)
+                btm_vertices = ' '.join(f'({v[0]} {v[1]} {v[2]})' for v in bottom_part)
+
+                body = \
+                    f' ((FACE :N "f{index}" :T WALL-FACE :INDEX {index})\n' \
+                    f'  (:PAR :N NCORN :V {up_count})\n' \
+                    f'  (:PAR :N CORNERS :V #2A({up_vertices}))\n' \
+                    f'  ((FACE :N GROUND-FACE)\n' \
+                    f'  (:PAR :N NCORN :V {btm_count})\n' \
+                    f'  (:PAR :N CORNERS :V #2A({btm_vertices}))))'
+
             room_section.append(body)
 
         sections.append('\n'.join(room_section) + ')')
 
     return '\n'.join(sections)
```

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.3.2/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/face.py` & `honeybee-idaice-0.3.2/honeybee_idaice/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.3.2/honeybee_idaice/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/shade.py` & `honeybee-idaice-0.3.2/honeybee_idaice/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.3.2/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.3.2/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.3.2/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.3.2/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.3.2/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.3.2/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/writer.py` & `honeybee-idaice-0.3.2/honeybee_idaice/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.3.2/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.3.2/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.1
+Version: 0.3.2
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.3.1/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.3.2/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.1/setup.py` & `honeybee-idaice-0.3.2/setup.py`

 * *Files identical despite different names*

