# Comparing `tmp/imaxt-multiscale-plugin-0.3.0.tar.gz` & `tmp/imaxt-multiscale-plugin-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaxt-multiscale-plugin-0.3.0.tar", last modified: Thu May 11 10:24:24 2023, max compression
+gzip compressed data, was "imaxt-multiscale-plugin-0.3.1.tar", last modified: Wed May 31 04:01:19 2023, max compression
```

## Comparing `imaxt-multiscale-plugin-0.3.0.tar` & `imaxt-multiscale-plugin-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.868656 imaxt-multiscale-plugin-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     7653 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3880 2023-05-11 10:24:24.868656 imaxt-multiscale-plugin-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1748 2023-05-11 10:24:24.868656 imaxt-multiscale-plugin-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.865656 imaxt-multiscale-plugin-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.867656 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_reader.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_sample_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.868656 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_reader.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_sample_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     1990 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     2449 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/napari.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1203 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/s3.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.867656 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3880 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      926 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:01:19.595253 imaxt-multiscale-plugin-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2023-05-31 04:01:04.000000 imaxt-multiscale-plugin-0.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-31 04:01:04.000000 imaxt-multiscale-plugin-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-31 04:01:19.595253 imaxt-multiscale-plugin-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-31 04:01:04.000000 imaxt-multiscale-plugin-0.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1763 2023-05-31 04:01:19.595253 imaxt-multiscale-plugin-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:01:19.592253 imaxt-multiscale-plugin-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:01:19.593253 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_sample_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:01:19.594253 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_tests/test_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_tests/test_sample_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_tests/test_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_tests/test_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1990 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/napari.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-31 04:01:05.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:01:19.594253 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-31 04:01:19.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      926 2023-05-31 04:01:19.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 04:01:19.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-31 04:01:19.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-31 04:01:19.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-31 04:01:19.000000 imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin.egg-info/top_level.txt
```

### Comparing `imaxt-multiscale-plugin-0.3.0/LICENSE` & `imaxt-multiscale-plugin-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.3.0/PKG-INFO` & `imaxt-multiscale-plugin-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaxt-multiscale-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple plugin to use with napari
 Home-page: https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/imaxt-multiscale-plugin
 Author: Eduardo Gonzalez Solares
 Author-email: E.GonzalezSolares@ast.cam.ac.uk
 License: LGPL-3.0-only
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `imaxt-multiscale-plugin-0.3.0/README.md` & `imaxt-multiscale-plugin-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.3.0/setup.cfg` & `imaxt-multiscale-plugin-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.0
+current_version = 0.3.1
 commit = True
 tag = True
 
 [metadata]
 name = imaxt-multiscale-plugin
 version = attr:imaxt_multiscale_plugin.__version__
 description = A simple plugin to use with napari
@@ -32,14 +32,16 @@
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	qtpy
 	xarray
 	dask
+	astropy
+	zarr
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_reader.py` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         (data, metadata, layer_type), where data is a numpy array, metadata is
         a dict of keyword arguments for the corresponding viewer.add_* method
         in napari, and layer_type is a lower-case string naming the type of
         layer. Both "meta", and "layer_type" are optional. napari will
         default to layer_type=="image" if not provided
     """
     def _get_data(ds, group):
-        if group in ["l.32", "l.16"]:
+        if group in ["l.32"]:
             res = ds.values
         else:
             res = ds.data
         return res.astype('float32')
 
     store = get_store_from_path(path)
     ds = xr.open_zarr(store, group="l.16")
@@ -100,15 +100,15 @@
 
     cube = []
     bscale = 1
     bzero = 0
     if "type" in ds.coords:
         ds = ds.sel(type="mosaic").astype("float32")
     p1, p2 = get_display_range(ds["S001"].sel(z=0) * bscale + bzero)
-    for group in ["", "l.2", "l.4", "l.8", "l.16"]:
+    for group in ["", "l.2", "l.4", "l.8", "l.16", "l.32"]:
         ds = xr.open_zarr(store, group=group)
         if "type" in ds.coords:  # v0.9 of pipeline
             ds = ds.sel(type="mosaic").astype("float32")
         datalist = [
             [
                 (_get_data(ds[s].sel(z=z), group) * bscale + bzero - p1)
                 / (p2 - p1)
```

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_reader.py` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_widget.py` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_widget.py` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_widget.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_writer.py` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/_writer.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/napari.yaml` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/napari.yaml`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/s3.py` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/s3.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/utils.py` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/PKG-INFO` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaxt-multiscale-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple plugin to use with napari
 Home-page: https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/imaxt-multiscale-plugin
 Author: Eduardo Gonzalez Solares
 Author-email: E.GonzalezSolares@ast.cam.ac.uk
 License: LGPL-3.0-only
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt` & `imaxt-multiscale-plugin-0.3.1/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

