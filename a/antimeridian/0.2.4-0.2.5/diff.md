# Comparing `tmp/antimeridian-0.2.4.tar.gz` & `tmp/antimeridian-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.2.4.tar", last modified: Fri May 12 16:01:39 2023, max compression
+gzip compressed data, was "antimeridian-0.2.5.tar", last modified: Wed May 31 14:26:59 2023, max compression
```

## Comparing `antimeridian-0.2.4.tar` & `antimeridian-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.228834 antimeridian-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-12 16:01:28.000000 antimeridian-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-12 16:01:39.228834 antimeridian-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-12 16:01:28.000000 antimeridian-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-12 16:01:28.000000 antimeridian-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:01:39.228834 antimeridian-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.224834 antimeridian-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.224834 antimeridian-0.2.4/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-12 16:01:28.000000 antimeridian-0.2.4/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-12 16:01:28.000000 antimeridian-0.2.4/src/antimeridian/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-12 16:01:28.000000 antimeridian-0.2.4/src/antimeridian/_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.228834 antimeridian-0.2.4/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.228834 antimeridian-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.697650 antimeridian-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-31 14:26:49.000000 antimeridian-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 14:26:59.697650 antimeridian-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-31 14:26:49.000000 antimeridian-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-31 14:26:49.000000 antimeridian-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:26:59.697650 antimeridian-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.693650 antimeridian-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.693650 antimeridian-0.2.5/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-31 14:26:49.000000 antimeridian-0.2.5/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-31 14:26:49.000000 antimeridian-0.2.5/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-05-31 14:26:49.000000 antimeridian-0.2.5/src/antimeridian/_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.693650 antimeridian-0.2.5/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 14:26:59.000000 antimeridian-0.2.5/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:26:59.697650 antimeridian-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 14:26:49.000000 antimeridian-0.2.5/tests/test_segment.py
```

### Comparing `antimeridian-0.2.4/LICENSE` & `antimeridian-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.4/PKG-INFO` & `antimeridian-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.2.4
+Version: 0.2.5
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
```

### Comparing `antimeridian-0.2.4/README.md` & `antimeridian-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.4/pyproject.toml` & `antimeridian-0.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-[build-system]
-requires = ["setuptools >= 64"]
-
 [project]
 name = "antimeridian"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
     {name = "Pete Gadomski", email = "pete.gadomski@gmail.com"}
 ]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
@@ -33,15 +30,15 @@
     "black~=23.3",
     "blacken-docs~=1.13",
     "mypy~=1.2",
     "packaging~=23.1",
     "pre-commit~=3.2",
     "pytest~=7.3",
     "pytest-console-scripts~=1.3",
-    "ruff==0.0.265",
+    "ruff==0.0.270",
     "tomli~=2.0; python_version<'3.11'"
 ]
 docs = [
     "cartopy~=0.21",
     "ipykernel~=6.22",
     "jupytext~=1.14",
     "nbsphinx~=0.9",
@@ -59,7 +56,10 @@
 
 [tool.mypy]
 strict = true
 
 [[tool.mypy.overrides]]
 module = ["shapely", "shapely.geometry"]
 ignore_missing_imports = true
+
+[build-system]
+requires = ["setuptools >= 64"]
```

### Comparing `antimeridian-0.2.4/src/antimeridian/_cli.py` & `antimeridian-0.2.5/src/antimeridian/_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.4/src/antimeridian/_implementation.py` & `antimeridian-0.2.5/src/antimeridian/_implementation.py`

 * *Files 8% similar despite different names*

```diff
@@ -430,7 +430,58 @@
 
 def is_self_closing(segment: List[Point]) -> bool:
     is_right = segment[-1][0] == 180
     return segment[0][0] == segment[-1][0] and (
         (is_right and segment[0][1] > segment[-1][1])
         or (not is_right and segment[0][1] < segment[-1][1])
     )
+
+
+def bbox(shape: Dict[str, Any] | GeoInterface) -> List[float]:
+    """Calculates a GeoJSON-spec conforming bounding box for a shape.
+
+    Per `the GeoJSON spec
+    <https://datatracker.ietf.org/doc/html/rfc7946#section-5.2>`_, an
+    antimeridian-spanning bounding box should have its larger longitude as its
+    first bounding box coordinate.
+
+    Args:
+        shape: The polygon or multipolygon for which to calculate the bounding box.
+
+    Returns:
+        List[float]: The bounding box.
+    """
+    geom = shapely.geometry.shape(shape)
+    if geom.geom_type == "Polygon":
+        return list(geom.bounds)
+    elif geom.geom_type == "MultiPolygon":
+        crosses_antimeridian = False
+        xmins = list()
+        ymin = 90
+        xmaxs = list()
+        ymax = -90
+        for polygon in geom.geoms:
+            bounds = polygon.bounds
+            xmins.append(bounds[0])
+            if bounds[1] < ymin:
+                ymin = bounds[1]
+            xmaxs.append(bounds[2])
+            if bounds[3] > ymax:
+                ymax = bounds[3]
+            if is_coincident_to_antimeridian(polygon):
+                crosses_antimeridian = True
+
+        if crosses_antimeridian:
+            return [max(xmins), ymin, min(xmaxs), ymax]
+        else:
+            return [min(xmins), ymin, max(xmaxs), ymax]
+    else:
+        raise ValueError(
+            f"unsupported geom_type for bbox calculation: {geom.geom_type}"
+        )
+
+
+def is_coincident_to_antimeridian(polygon: Polygon) -> bool:
+    for start, end in zip(polygon.exterior.coords, polygon.exterior.coords[1:]):
+        if abs(start[0]) == 180 and start[0] == end[0]:
+            return True
+    return False
```

### Comparing `antimeridian-0.2.4/src/antimeridian.egg-info/PKG-INFO` & `antimeridian-0.2.5/src/antimeridian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.2.4
+Version: 0.2.5
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
```

### Comparing `antimeridian-0.2.4/tests/test_cli.py` & `antimeridian-0.2.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.4/tests/test_geojson.py` & `antimeridian-0.2.5/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.4/tests/test_multi_polygon.py` & `antimeridian-0.2.5/tests/test_multi_polygon.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import antimeridian
+import pytest
 import shapely.geometry
 from shapely.geometry import MultiPolygon
 
 from .conftest import Reader
 
 
+@pytest.mark.parametrize(
+    ("name"),
+    [
+        "multi-split",
+        "multi-no-antimeridian",
+    ],
+)
 def test_multi_polygon(
     read_input: Reader,
     read_output: Reader,
+    name: str,
 ) -> None:
-    input = read_input("multi-split")
+    input = read_input(name)
     assert isinstance(input, MultiPolygon)
-    output = read_output("multi-split")
+    output = read_output(name)
     assert isinstance(output, MultiPolygon)
     fixed = antimeridian.fix_multi_polygon(input)
     assert fixed.is_valid
     assert fixed.normalize() == output.normalize()
 
 
 def test_fix_shape(read_input: Reader) -> None:
```

### Comparing `antimeridian-0.2.4/tests/test_polygon.py` & `antimeridian-0.2.5/tests/test_polygon.py`

 * *Files identical despite different names*

