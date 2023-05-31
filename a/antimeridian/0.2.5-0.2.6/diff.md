# Comparing `tmp/antimeridian-0.2.5.tar.gz` & `tmp/antimeridian-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.2.5.tar", last modified: Wed May 31 14:26:59 2023, max compression
+gzip compressed data, was "antimeridian-0.2.6.tar", last modified: Wed May 31 18:12:09 2023, max compression
```

## Comparing `antimeridian-0.2.5.tar` & `antimeridian-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.697650 antimeridian-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-31 14:26:49.000000 antimeridian-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 14:26:59.697650 antimeridian-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-31 14:26:49.000000 antimeridian-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-31 14:26:49.000000 antimeridian-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:26:59.697650 antimeridian-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.693650 antimeridian-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.693650 antimeridian-0.2.5/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-31 14:26:49.000000 antimeridian-0.2.5/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-31 14:26:49.000000 antimeridian-0.2.5/src/antimeridian/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-05-31 14:26:49.000000 antimeridian-0.2.5/src/antimeridian/_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.693650 antimeridian-0.2.5/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.697650 antimeridian-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-31 18:12:01.000000 antimeridian-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 18:12:09.593973 antimeridian-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-31 18:12:01.000000 antimeridian-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-31 18:12:01.000000 antimeridian-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:12:09.593973 antimeridian-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-31 18:12:01.000000 antimeridian-0.2.6/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-31 18:12:01.000000 antimeridian-0.2.6/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-05-31 18:12:01.000000 antimeridian-0.2.6/src/antimeridian/_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_segment.py
```

### Comparing `antimeridian-0.2.5/LICENSE` & `antimeridian-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.5/PKG-INFO` & `antimeridian-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.2.5
+Version: 0.2.6
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
```

### Comparing `antimeridian-0.2.5/README.md` & `antimeridian-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.5/pyproject.toml` & `antimeridian-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "antimeridian"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
     {name = "Pete Gadomski", email = "pete.gadomski@gmail.com"}
 ]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
```

### Comparing `antimeridian-0.2.5/src/antimeridian/_cli.py` & `antimeridian-0.2.6/src/antimeridian/_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.5/src/antimeridian/_implementation.py` & `antimeridian-0.2.6/src/antimeridian/_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,16 @@
 
 
 def segment(coords: List[Point]) -> List[List[Point]]:
     segment = []
     segments = []
     for i, point in enumerate(coords):
         # Ensure all longitudes are between -180 and 180
-        coords[i] = (((point[0] + 180) % 360) - 180, point[1])
+        if point[0] != 180:
+            coords[i] = (((point[0] + 180) % 360) - 180, point[1])
     for start, end in zip(coords, coords[1:]):
         segment.append(start)
         if (end[0] - start[0] > 180) and (end[0] - start[0] != 360):  # left
             latitude = crossing_latitude(start, end)
             segment.append((-180, latitude))
             segments.append(segment)
             segment = [(180, latitude)]
```

### Comparing `antimeridian-0.2.5/src/antimeridian.egg-info/PKG-INFO` & `antimeridian-0.2.6/src/antimeridian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.2.5
+Version: 0.2.6
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
```

### Comparing `antimeridian-0.2.5/tests/test_cli.py` & `antimeridian-0.2.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.5/tests/test_geojson.py` & `antimeridian-0.2.6/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.5/tests/test_multi_polygon.py` & `antimeridian-0.2.6/tests/test_multi_polygon.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.5/tests/test_polygon.py` & `antimeridian-0.2.6/tests/test_polygon.py`

 * *Files 19% similar despite different names*

```diff
@@ -56,7 +56,14 @@
 
 
 def test_force_north_pole(read_input: Reader, read_output: Reader) -> None:
     input = read_input("force-north-pole")
     output = read_output("force-north-pole")
     fixed = antimeridian.fix_polygon(input, force_north_pole=True)
     assert fixed.normalize() == output.normalize()
+
+
+@pytest.mark.parametrize("minx,maxx", [(-180, -170), (170, 180)])
+def test_dont_segment_antimeridian_overlap(minx: float, maxx: float) -> None:
+    shape = shapely.geometry.box(minx=minx, miny=-10, maxx=maxx, maxy=10)
+    fixed = antimeridian.fix_polygon(shape)
+    assert fixed.geom_type == "Polygon"
```

