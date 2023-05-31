# Comparing `tmp/zen3geo-0.6.0.tar.gz` & `tmp/zen3geo-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen3geo-0.6.0.tar", max compression
+gzip compressed data, was "zen3geo-0.6.1.tar", max compression
```

## Comparing `zen3geo-0.6.0.tar` & `zen3geo-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     7652 2023-04-18 01:40:28.438814 zen3geo-0.6.0/LICENSE.md
--rw-r--r--   0        0        0      826 2023-04-18 01:40:28.438814 zen3geo-0.6.0/README.md
--rw-r--r--   0        0        0     2912 2023-04-18 01:40:51.284191 zen3geo-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      207 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/__init__.py
--rw-r--r--   0        0        0     1050 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/__init__.py
--rw-r--r--   0        0        0    15153 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/datashader.py
--rw-r--r--   0        0        0     7162 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/geopandas.py
--rw-r--r--   0        0        0     3350 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/pyogrio.py
--rw-r--r--   0        0        0     3395 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/pystac.py
--rw-r--r--   0        0        0     5232 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/pystac_client.py
--rw-r--r--   0        0        0     2723 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/rioxarray.py
--rw-r--r--   0        0        0     7123 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/stackstac.py
--rw-r--r--   0        0        0     3899 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/xbatcher.py
--rw-r--r--   0        0        0     5302 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/xpystac.py
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 zen3geo-0.6.0/setup.py
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 zen3geo-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-31 05:14:08.491117 zen3geo-0.6.1/LICENSE.md
+-rw-r--r--   0        0        0      826 2023-05-31 05:14:08.491117 zen3geo-0.6.1/README.md
+-rw-r--r--   0        0        0     2912 2023-05-31 05:14:29.288022 zen3geo-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/__init__.py
+-rw-r--r--   0        0        0     1050 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/__init__.py
+-rw-r--r--   0        0        0    15274 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/datashader.py
+-rw-r--r--   0        0        0     7162 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/geopandas.py
+-rw-r--r--   0        0        0     3350 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/pyogrio.py
+-rw-r--r--   0        0        0     3395 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/pystac.py
+-rw-r--r--   0        0        0     5153 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/pystac_client.py
+-rw-r--r--   0        0        0     2723 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/rioxarray.py
+-rw-r--r--   0        0        0     7123 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/stackstac.py
+-rw-r--r--   0        0        0     3899 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/xbatcher.py
+-rw-r--r--   0        0        0     5323 2023-05-31 05:14:08.495117 zen3geo-0.6.1/zen3geo/datapipes/xpystac.py
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 zen3geo-0.6.1/PKG-INFO
```

### Comparing `zen3geo-0.6.0/LICENSE.md` & `zen3geo-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.0/README.md` & `zen3geo-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.0/pyproject.toml` & `zen3geo-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zen3geo"
-version = "0.6.0"
+version = "0.6.1"
 description = "The 🌏 data science library you've been waiting for~"
 authors = ["Wei Ji <23487320+weiji14@users.noreply.github.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
@@ -65,16 +65,16 @@
     "graphviz",
     "jupyter-book",
     "matplotlib",
     "planetary-computer",
     "pyogrio",
     "pystac",
     "pystac_client",
-    "stackstac",
     "spatialpandas",
+    "stackstac",
     "xarray-datatree",
     "xbatcher",
     "xpystac",
     "zarr"
 ]
 raster = [
     "xbatcher",
@@ -95,9 +95,9 @@
 [tool.poetry-dynamic-versioning]
 bump = true
 enable = true
 metadata = false
 style = "pep440"
 
 [build-system]
-requires = ["poetry-core>=1.4.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.5.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/__init__.py` & `zen3geo-0.6.1/zen3geo/datapipes/__init__.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/datashader.py` & `zen3geo-0.6.1/zen3geo/datapipes/datashader.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         self.source_datapipe: IterDataPipe = source_datapipe  # datashader.Canvas
         self.vector_datapipe: IterDataPipe = vector_datapipe  # geopandas.GeoDataFrame
         self.agg: Optional = agg  # Datashader Aggregation/Reduction function
         self.kwargs = kwargs
 
         len_vector_datapipe: int = len(self.vector_datapipe)
         len_canvas_datapipe: int = len(self.source_datapipe)
-        if len_vector_datapipe != 1 or len_vector_datapipe != len_canvas_datapipe:
+        if len_vector_datapipe != 1 and len_vector_datapipe != len_canvas_datapipe:
             raise ValueError(
                 f"Unmatched lengths for the canvas datapipe ({self.source_datapipe}) "
                 f"and vector datapipe ({self.vector_datapipe}). \n"
                 f"The vector datapipe's length ({len_vector_datapipe}) should either "
                 f"be (1) to allow for broadcasting, or match the canvas datapipe's "
                 f"length of ({len_canvas_datapipe})."
             )
@@ -210,21 +210,24 @@
                     f"with the following bounds: \n {vector.bounds} \n"
                     f"Please set crs using e.g. `vector = vector.set_crs(crs='OGC:CRS84')`."
                 ) from e
 
             # Convert vector to spatialpandas format to allow datashader's
             # rasterization methods to work
             try:
-                columns = ["geometry"] if not hasattr(vector, "columns") else None
-                _vector = spatialpandas.GeoDataFrame(data=vector, columns=columns)
+                _vector = spatialpandas.GeoDataFrame(data=vector.geometry)
             except ValueError as e:
-                raise NotImplementedError(
-                    f"Unsupported geometry type(s) {set(vector.geom_type)} detected, "
-                    "only point, line or polygon vector geometry types are supported."
-                ) from e
+                if str(e) == "Unable to convert data argument to a GeometryList array":
+                    raise NotImplementedError(
+                        f"Unsupported geometry type(s) {set(vector.geom_type)} detected, "
+                        "only point, line or polygon vector geometry types "
+                        "(or their multi- equivalents) are supported."
+                    ) from e
+                else:
+                    raise e
 
             # Determine geometry type to know which rasterization method to use
             vector_dtype: spatialpandas.geometry.GeometryDtype = _vector.geometry.dtype
 
             if isinstance(vector_dtype, (PointDtype, MultiPointDtype)):
                 raster: xr.DataArray = canvas.points(
                     source=_vector, agg=self.agg, geometry="geometry", **self.kwargs
```

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/geopandas.py` & `zen3geo-0.6.1/zen3geo/datapipes/geopandas.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/pyogrio.py` & `zen3geo-0.6.1/zen3geo/datapipes/pyogrio.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/pystac.py` & `zen3geo-0.6.1/zen3geo/datapipes/pystac.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/pystac_client.py` & `zen3geo-0.6.1/zen3geo/datapipes/pystac_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,15 @@
           `RFC 3339-compliant <https://tools.ietf.org/html/rfc3339>`_
           timestamp, or a simple date string.
         - **collections** - List of one or more Collection IDs or
           :py:class:`pystac.Collection` instances. Only Items in one of the
           provided Collections will be searched.
 
     catalog_url : str
-        The URL of a STAC Catalog. If not specified, this will use the
-        ``STAC_URL`` environment variable.
+        The URL of a STAC Catalog.
 
     kwargs : Optional
         Extra keyword arguments to pass to
         :py:meth:`pystac_client.Client.open`. For example:
 
         - **headers** - A dictionary of additional headers to use in all
           requests made to any part of this Catalog/API.
```

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/rioxarray.py` & `zen3geo-0.6.1/zen3geo/datapipes/rioxarray.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/stackstac.py` & `zen3geo-0.6.1/zen3geo/datapipes/stackstac.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/xbatcher.py` & `zen3geo-0.6.1/zen3geo/datapipes/xbatcher.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.6.0/zen3geo/datapipes/xpystac.py` & `zen3geo-0.6.1/zen3geo/datapipes/xpystac.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     def __init__(
         self,
         source_datapipe: IterDataPipe,
         engine: str = "stac",
         **kwargs: Optional[Dict[str, Any]]
     ) -> None:
-        if xpystac is None:
+        if xpystac is None and engine == "stac":
             raise ModuleNotFoundError(
                 "Package `xpystac` is required to be installed to use this datapipe. "
                 "Please use `pip install xpystac` "
                 "to install the package"
             )
         self.source_datapipe: IterDataPipe = source_datapipe
         self.engine: str = engine
```

### Comparing `zen3geo-0.6.0/PKG-INFO` & `zen3geo-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen3geo
-Version: 0.6.0
+Version: 0.6.1
 Summary: The 🌏 data science library you've been waiting for~
 License: LGPL-3.0-or-later
 Author: Wei Ji
 Author-email: 23487320+weiji14@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

