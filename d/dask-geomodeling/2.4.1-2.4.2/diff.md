# Comparing `tmp/dask-geomodeling-2.4.1.tar.gz` & `tmp/dask-geomodeling-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-geomodeling-2.4.1.tar", last modified: Tue Apr 18 13:13:33 2023, max compression
+gzip compressed data, was "dask-geomodeling-2.4.2.tar", last modified: Wed May 31 11:50:01 2023, max compression
```

## Comparing `dask-geomodeling-2.4.1.tar` & `dask-geomodeling-2.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.729328 dask-geomodeling-2.4.1/
--rw-rw-r--   0 casper    (1000) casper    (1000)    19112 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/CHANGES.rst
--rw-rw-r--   0 casper    (1000) casper    (1000)     1503 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/LICENSE
--rw-rw-r--   0 casper    (1000) casper    (1000)       59 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/MANIFEST.in
--rw-rw-r--   0 casper    (1000) casper    (1000)    20982 2023-04-18 13:13:33.729328 dask-geomodeling-2.4.1/PKG-INFO
--rw-rw-r--   0 casper    (1000) casper    (1000)     1240 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/README.rst
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.721328 dask-geomodeling-2.4.1/dask_geomodeling/
--rw-rw-r--   0 casper    (1000) casper    (1000)      228 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)      318 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/config.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.725328 dask-geomodeling-2.4.1/dask_geomodeling/core/
--rw-rw-r--   0 casper    (1000) casper    (1000)       30 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/core/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    11147 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/core/graphs.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.725328 dask-geomodeling-2.4.1/dask_geomodeling/geometry/
--rw-rw-r--   0 casper    (1000) casper    (1000)      337 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    23038 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/aggregate.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    10953 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/base.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/constructive.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    24495 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/field_operations.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     1492 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/geom_operations.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     5351 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/merge.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     3458 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/parallelize.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4978 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/set_operations.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    10587 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/sinks.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     9096 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/sources.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4138 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/text.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4987 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/ipyleaflet_plugin.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4796 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/measurements.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.729328 dask-geomodeling-2.4.1/dask_geomodeling/raster/
--rw-rw-r--   0 casper    (1000) casper    (1000)      291 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/base.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    16996 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/combine.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    25032 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/elemwise.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    26079 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/misc.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4450 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/parallelize.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     8124 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/reduction.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    17971 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/sources.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    26435 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/spatial.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    32375 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/temporal.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    31545 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/utils.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.725328 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/
--rw-rw-r--   0 casper    (1000) casper    (1000)    20982 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/PKG-INFO
--rw-rw-r--   0 casper    (1000) casper    (1000)     1341 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/SOURCES.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/dependency_links.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/not-zip-safe
--rw-rw-r--   0 casper    (1000) casper    (1000)      112 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/requires.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)       17 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/top_level.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)      324 2023-04-18 13:13:33.729328 dask-geomodeling-2.4.1/setup.cfg
--rw-rw-r--   0 casper    (1000) casper    (1000)     1670 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/setup.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.532863 dask-geomodeling-2.4.2/
+-rw-rw-r--   0 casper    (1000) casper    (1000)    19228 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/CHANGES.rst
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1503 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/LICENSE
+-rw-rw-r--   0 casper    (1000) casper    (1000)       59 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/MANIFEST.in
+-rw-rw-r--   0 casper    (1000) casper    (1000)    21098 2023-05-31 11:50:01.532863 dask-geomodeling-2.4.2/PKG-INFO
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1240 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/README.rst
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.528863 dask-geomodeling-2.4.2/dask_geomodeling/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      228 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)      318 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/config.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.528863 dask-geomodeling-2.4.2/dask_geomodeling/core/
+-rw-rw-r--   0 casper    (1000) casper    (1000)       30 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/core/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    11147 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/core/graphs.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.528863 dask-geomodeling-2.4.2/dask_geomodeling/geometry/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      337 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    23024 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/aggregate.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    10953 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/base.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/constructive.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    24495 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/field_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1492 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/geom_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     5351 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/merge.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     3458 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/parallelize.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4978 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/set_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    10587 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/sinks.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     9096 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/sources.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4138 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/geometry/text.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4987 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/ipyleaflet_plugin.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4796 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/measurements.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.532863 dask-geomodeling-2.4.2/dask_geomodeling/raster/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      291 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/base.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    16996 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/combine.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    25032 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/elemwise.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    26079 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/misc.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4450 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/parallelize.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     8124 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/reduction.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    17971 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/sources.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    26435 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/spatial.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    33321 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/raster/temporal.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    31545 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/dask_geomodeling/utils.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-05-31 11:50:01.528863 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/
+-rw-rw-r--   0 casper    (1000) casper    (1000)    21098 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/PKG-INFO
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1341 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/SOURCES.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/dependency_links.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/not-zip-safe
+-rw-rw-r--   0 casper    (1000) casper    (1000)      112 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/requires.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)       17 2023-05-31 11:50:01.000000 dask-geomodeling-2.4.2/dask_geomodeling.egg-info/top_level.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)      324 2023-05-31 11:50:01.532863 dask-geomodeling-2.4.2/setup.cfg
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1670 2023-05-31 11:50:00.000000 dask-geomodeling-2.4.2/setup.py
```

### Comparing `dask-geomodeling-2.4.1/CHANGES.rst` & `dask-geomodeling-2.4.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.2 (2023-05-31)
+------------------
+
+- Fixed TemporalAggregate and Cumulative for month start ("MS") frequency.
+
+
 2.4.1 (2023-04-18)
 ------------------
 
 - AggregateRaster will do a point request to the raster if only 1 cell is required
   (instead of a box request that encompasses the cell).
```

### Comparing `dask-geomodeling-2.4.1/LICENSE` & `dask-geomodeling-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/PKG-INFO` & `dask-geomodeling-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-geomodeling
-Version: 2.4.1
+Version: 2.4.2
 Summary: On-the-fly operations on geographical maps.
 Home-page: https://github.com/nens/dask-geomodeling
 Author: Casper van der Wel
 Author-email: casper.vanderwel@nelen-schuurmans.nl
 License: BSD 3-Clause License
 Keywords: dask
 Classifier: Development Status :: 4 - Beta
@@ -43,14 +43,20 @@
 
 `Read the docs <https://dask-geomodeling.readthedocs.org/>`_ for further information.
 
 
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.2 (2023-05-31)
+------------------
+
+- Fixed TemporalAggregate and Cumulative for month start ("MS") frequency.
+
+
 2.4.1 (2023-04-18)
 ------------------
 
 - AggregateRaster will do a point request to the raster if only 1 cell is required
   (instead of a box request that encompasses the cell).
```

### Comparing `dask-geomodeling-2.4.1/README.rst` & `dask-geomodeling-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/core/graphs.py` & `dask-geomodeling-2.4.2/dask_geomodeling/core/graphs.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/aggregate.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/aggregate.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     threshold_values,
     statistic,
     percentile,
 ):
     """Compute aggregates for given geometries.
 
     Geometries are rasterized using gdal_rasterize (without the ALL_TOUCHED option).
-    
+
     Args:
       geometries (GeoSeries): The geometries to aggregate the raster in.
       values (ndarray): A three-dimensional raster ``(t, y, x)`` to aggregate.
       no_data_value (number): The value in ``values`` that denotes missing data.
       agg_bbox (tuple of 4 numbers): The bbox of ``values``.
       agg_srs (str): The projection of ``values``.
       threshold_values (ndarray, optional): A threshold value per geometry.
@@ -210,15 +210,15 @@
     agg_bbox,
     threshold_values,
     statistic,
 ):
     """Compute aggregates for given point geometries.
 
     The values of the raster is taken at the point coordinates.
-    
+
     Args:
       points (GeoSeries): The geometries (points) to aggregate the raster in.
       values (ndarray): A three-dimensional raster ``(t, y, x)`` to aggregate.
       no_data_value (number): The value in ``values`` that denotes missing data.
       agg_bbox (tuple of 4 numbers): The bbox of ``values``.
       threshold_values (ndarray): A threshold value per geometry.
       statistic (str): A key in ``AggregateRaster.STATISTICS``.
@@ -252,26 +252,26 @@
     return agg
 
 
 class AggregateRaster(GeometryBlock):
     """
     Compute statistics of a raster for each geometry in a geometry source.
 
-    A statistic is computed in a specific projection and with a specified raster 
+    A statistic is computed in a specific projection and with a specified raster
     cell size. If ``projection`` or ``pixel_size`` are not given, these default to
     the native projection of the provided raster source. The following cells are
     selected to perform the statistic (e.g. mean) on:
 
     - Polygons: all raster cells whose center is inside the polygon
     - Points: the raster cell (singular) that contains the point
     - Linestrings: Bresenham's line algorithm is used
 
     If this assignment leads to the situation that a geometry covers no raster
     cells (for instance with a polygon much smaller than the raster cell size),
-    the geometry is reduced to a point by taking its centroid.    
+    the geometry is reduced to a point by taking its centroid.
 
     Should the combination of the requested pixel_size and the extent of the
     source geometry cause the required raster size to exceed ``max_pixels``,
     the ``pixel_size`` can be adjusted automatically if ``auto_pixel_size`` is
     set to ``True``, else (the default) a RuntimeError is raised.
 
     Please note that for any field operation on the result of this block
@@ -460,15 +460,15 @@
         # compute the width and height
         width = max(int((x2 - x1) / pixel_size), 1)
         height = max(int((y2 - y1) / pixel_size), 1)
 
         # change point-like requests in real point requests
         # (reducing possible edge effects)
         if width == 1 and height == 1:
-            raster_req_bbox = ((x1 + x2) / 2, (y1 + y2) / 2 ) * 2
+            raster_req_bbox = ((x1 + x2) / 2, (y1 + y2) / 2) * 2
         else:
             raster_req_bbox = (x1, y1, x2, y2)
 
         raster_request = {
             "mode": "vals",
             "projection": agg_srs,
             "start": request.get("start"),
```

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/base.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/base.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/constructive.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/constructive.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/field_operations.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/field_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/geom_operations.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/geom_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/merge.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/merge.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/parallelize.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/parallelize.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/set_operations.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/set_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/sinks.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/sinks.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/sources.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/sources.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/geometry/text.py` & `dask-geomodeling-2.4.2/dask_geomodeling/geometry/text.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/ipyleaflet_plugin.py` & `dask-geomodeling-2.4.2/dask_geomodeling/ipyleaflet_plugin.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/measurements.py` & `dask-geomodeling-2.4.2/dask_geomodeling/measurements.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/raster/base.py` & `dask-geomodeling-2.4.2/dask_geomodeling/raster/base.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/raster/combine.py` & `dask-geomodeling-2.4.2/dask_geomodeling/raster/combine.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/raster/elemwise.py` & `dask-geomodeling-2.4.2/dask_geomodeling/raster/elemwise.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/raster/misc.py` & `dask-geomodeling-2.4.2/dask_geomodeling/raster/misc.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/raster/parallelize.py` & `dask-geomodeling-2.4.2/dask_geomodeling/raster/parallelize.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/raster/reduction.py` & `dask-geomodeling-2.4.2/dask_geomodeling/raster/reduction.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/raster/sources.py` & `dask-geomodeling-2.4.2/dask_geomodeling/raster/sources.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/raster/spatial.py` & `dask-geomodeling-2.4.2/dask_geomodeling/raster/spatial.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/raster/temporal.py` & `dask-geomodeling-2.4.2/dask_geomodeling/raster/temporal.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
 from .base import RasterBlock, BaseSingle
 
 
 __all__ = ["Snap", "Shift", "TemporalSum", "TemporalAggregate", "Cumulative"]
 
 
+MICROSECOND = Timedelta(microseconds=1)
+
+
 class Snap(RasterBlock):
     """
     Snap the time structure of a raster to that of another raster.
 
     This operations allows to take the cell values from one raster ('store')
     and the temporal properties of another raster ('index').
 
@@ -299,37 +302,122 @@
         differences = differences[differences >= pd.Timedelta(0)]
     elif side == "left":
         differences = differences[differences <= pd.Timedelta(0)]
     result = differences.abs().idxmin()
     return _ts_to_dt(result, timezone)
 
 
-def _label_to_period(dt, frequency, closed, label, timezone):
-    """Converts a datetime to a period whose label equals that datetime"""
-    label_ts = _dt_to_ts(dt, timezone)
-    # translate that back to the period
-    series = pd.Series([0], index=[label_ts])
-    label_candidate = (
-        series.resample(frequency, closed=closed, label=label, kind="timestamp")
-        .first()
-        .index[0]
-    )
-    # in most cases the label_candidate == label, but sometimes it doesnt work
-    # because the label actually falls outside of the bin
-    if label_candidate < label_ts:
-        series.index += to_offset(frequency)
-    elif label_candidate > label_ts:
-        series.index -= to_offset(frequency)
-    # now retrieve the period
-    period = (
-        series.resample(frequency, closed=closed, label=label, kind="period")
-        .first()
-        .index[0]
+def _default_closed_label(frequency, closed, label):
+    """To make closed & label not-None"""
+    if frequency is None:
+        return ("right", "right")
+    # Copied from pandas 'TimeGrouper.__init__':
+    end_types = {"M", "A", "Q", "BM", "BA", "BQ", "W"}
+    rule = to_offset(frequency).rule_code
+    if rule in end_types or ("-" in rule and rule[: rule.find("-")] in end_types):
+        if closed is None:
+            closed = "right"
+        if label is None:
+            label = "right"
+    else:
+        if closed is None:
+            closed = "left"
+        if label is None:
+            label = "left"
+    return closed, label
+
+
+def _label_to_bin_start(dt, frequency, closed, label, timezone):
+    """Returns the first datetime in bin with label 'dt'"""
+    ts = _dt_to_ts(dt, timezone)
+    if label == "right":
+        ts -= to_offset(frequency)
+    if closed == "right":
+        ts += MICROSECOND
+    return _ts_to_dt(ts, timezone)
+
+
+def _label_to_bin_end(dt, frequency, closed, label, timezone):
+    """Returns the last datetime in bin with label 'dt'"""
+    ts = _dt_to_ts(dt, timezone)
+    if label == "left":
+        ts += to_offset(frequency)
+    if closed == "left":
+        ts -= MICROSECOND
+    return _ts_to_dt(ts, timezone)
+
+
+def _resampled_period(period, frequency, closed, label, timezone):
+    """Given a source (start, stop) and frequency, compute the (start, stop) interval
+    that contains data after resampling. The returned start and stop are bin labels.
+    """
+    if period is None:
+        return
+    if frequency is None:
+        return period[-1], period[-1]
+    return tuple(_get_bin_label(x, frequency, closed, label, timezone) for x in period)
+
+
+def _snap_to_resampled_labels(period, start, stop, frequency, closed, label, timezone):
+    """Snap start and stop to the bin labels (so timeframes of a resampled raster).
+
+    The result are 2 labels: a start and a stop label, as python datetimes.
+    If the stop label is None, start == stop. If both are None, there is no label in range.
+    """
+    period = _resampled_period(period, frequency, closed, label, timezone)
+    if period is None:  # return early for an empty source
+        return None, None
+
+    if start is None:  # start is None means: return the latest
+        start = period[1]
+
+    if stop is None:
+        # snap start to a label closest to it
+        if start <= period[0]:
+            start = period[0]
+        elif start >= period[1]:
+            start = period[1]
+        else:
+            start = _get_closest_label(
+                start, frequency, closed, label, timezone, side="both"
+            )
+    else:
+        # snap start to a label right from it
+        if start <= period[0]:
+            start = period[0]
+        elif start > period[1]:
+            return None, None
+        else:
+            start = _get_closest_label(
+                start, frequency, closed, label, timezone, side="right"
+            )
+        # snap stop to a label left from it
+        if stop >= period[1]:
+            stop = period[1]
+        elif stop < period[0]:
+            return None, None
+        else:
+            stop = _get_closest_label(
+                stop, frequency, closed, label, timezone, side="left"
+            )
+
+        if start > stop:
+            return None, None
+
+    return start, stop
+
+
+def _labels_to_start_stop(start_label, stop_label, frequency, closed, label, timezone):
+    """Given a start and stop label, get the start/stop to request from source"""
+    assert frequency is not None
+    start = _label_to_bin_start(start_label, frequency, closed, label, timezone)
+    stop = _label_to_bin_end(
+        stop_label or start_label, frequency, closed, label, timezone
     )
-    return period
+    return start, stop
 
 
 def count_not_nan(x, *args, **kwargs):
     return np.sum(~np.isnan(x), *args, **kwargs)
 
 
 class TemporalAggregate(BaseSingle):
@@ -438,29 +526,26 @@
 
     @property
     def timezone(self):
         return self.args[5]
 
     @property
     def _snap_kwargs(self):
+        # make closed & label not-None
+        closed, label = _default_closed_label(self.frequency, self.closed, self.label)
         return {
             "frequency": self.frequency,
-            "closed": self.closed,
-            "label": self.label,
+            "closed": closed,
+            "label": label,
             "timezone": self.timezone,
         }
 
     @property
     def period(self):
-        period = self.source.period
-        if period is None:
-            return
-        if self.frequency is None:
-            return period[-1], period[-1]
-        return tuple(_get_bin_label(x, **self._snap_kwargs) for x in period)
+        return _resampled_period(self.source.period, **self._snap_kwargs)
 
     @property
     def timedelta(self):
         try:
             return to_offset(self.frequency).delta
         except AttributeError:
             return  # e.g. Month is non-equidistant
@@ -469,90 +554,45 @@
     def dtype(self):
         return dtype_for_statistic(self.source.dtype, self.statistic)
 
     @property
     def fillvalue(self):
         return get_dtype_max(self.dtype)
 
-    def _snap_to_resampled_labels(self, start, stop):
-        """Snaps start and stop to resampled frames"""
-        kwargs = self._snap_kwargs
-        period = self.period
-        if period is None:  # return early for an empty source
-            return None, None
-
-        if start is None:  # start is None means: return the latest
-            start = period[1]
-
-        if stop is None:
-            # snap start to a label closest to it
-            if start <= period[0]:
-                start = period[0]
-            elif start >= period[1]:
-                start = period[1]
-            else:
-                start = _get_closest_label(start, side="both", **kwargs)
-        else:
-            # snap start to a label right from it
-            if start <= period[0]:
-                start = period[0]
-            elif start > period[1]:
-                return None, None
-            else:
-                start = _get_closest_label(start, side="right", **kwargs)
-            # snap stop to a label left from it
-            if stop >= period[1]:
-                stop = period[1]
-            elif stop < period[0]:
-                return None, None
-            else:
-                stop = _get_closest_label(stop, side="left", **kwargs)
-        return start, stop
-
     def get_sources_and_requests(self, **request):
         kwargs = self._snap_kwargs
         start = request.get("start")
         stop = request.get("stop")
         mode = request["mode"]
 
-        start, stop = self._snap_to_resampled_labels(start, stop)
-        if start is None:
+        start_label, stop_label = _snap_to_resampled_labels(
+            self.source.period, start, stop, **kwargs
+        )
+        if start_label is None:
             return [({"empty": True, "mode": mode}, None)]
 
         # a time request does not involve a request to self.source
         if mode == "time":
             kwargs["mode"] = "time"
-            kwargs["start"] = start
-            kwargs["stop"] = stop
+            kwargs["start"] = start_label
+            kwargs["stop"] = stop_label
             return [(kwargs, None)]
 
         # vals or source requests do need a request to self.source
         if self.frequency is None:
             request["start"], request["stop"] = self.source.period
         else:
-            if stop is None or start == stop:
-                # recover the period that is closest to start
-                start_period = stop_period = _label_to_period(start, **kwargs)
-            else:
-                # recover the period that has label >= start
-                start_period = _label_to_period(start, **kwargs)
-                # recover the period that has label <= stop
-                stop_period = _label_to_period(stop, **kwargs)
-
-            # snap request 'start' to the start of the first period
-            request["start"] = _ts_to_dt(start_period.start_time, self.timezone)
-            # snap request 'stop' to the end of the last period
-            request["stop"] = _ts_to_dt(stop_period.end_time, self.timezone)
-            if kwargs["closed"] != "left":
-                request["stop"] += Timedelta(microseconds=1)
+            request["start"], request["stop"] = _labels_to_start_stop(
+                start_label, stop_label, **kwargs
+            )
 
         # return sources and requests depending on the mode
         kwargs["mode"] = request["mode"]
-        kwargs["start"] = start
-        kwargs["stop"] = stop
+        kwargs["start"] = start_label
+        kwargs["stop"] = stop_label
         if mode == "vals":
             kwargs["dtype"] = np.dtype(self.dtype).str
             kwargs["statistic"] = self.statistic
 
         time_request = {
             "mode": "time",
             "start": request["start"],
```

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling/utils.py` & `dask-geomodeling-2.4.2/dask_geomodeling/utils.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling.egg-info/PKG-INFO` & `dask-geomodeling-2.4.2/dask_geomodeling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-geomodeling
-Version: 2.4.1
+Version: 2.4.2
 Summary: On-the-fly operations on geographical maps.
 Home-page: https://github.com/nens/dask-geomodeling
 Author: Casper van der Wel
 Author-email: casper.vanderwel@nelen-schuurmans.nl
 License: BSD 3-Clause License
 Keywords: dask
 Classifier: Development Status :: 4 - Beta
@@ -43,14 +43,20 @@
 
 `Read the docs <https://dask-geomodeling.readthedocs.org/>`_ for further information.
 
 
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.2 (2023-05-31)
+------------------
+
+- Fixed TemporalAggregate and Cumulative for month start ("MS") frequency.
+
+
 2.4.1 (2023-04-18)
 ------------------
 
 - AggregateRaster will do a point request to the raster if only 1 cell is required
   (instead of a box request that encompasses the cell).
```

### Comparing `dask-geomodeling-2.4.1/dask_geomodeling.egg-info/SOURCES.txt` & `dask-geomodeling-2.4.2/dask_geomodeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.1/setup.py` & `dask-geomodeling-2.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = '2.4.1'
+version = '2.4.2'
 
 long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read()])
 
 install_requires = (
     [
         "dask[delayed]>=0.20",
         "pandas>=0.23",
```

