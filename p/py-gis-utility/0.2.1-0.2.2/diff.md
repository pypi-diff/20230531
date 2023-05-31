# Comparing `tmp/py-gis-utility-0.2.1.tar.gz` & `tmp/py-gis-utility-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-gis-utility-0.2.1.tar", last modified: Mon Oct 24 11:58:12 2022, max compression
+gzip compressed data, was "py-gis-utility-0.2.2.tar", last modified: Wed May 31 10:39:26 2023, max compression
```

## Comparing `py-gis-utility-0.2.1.tar` & `py-gis-utility-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:58:12.640807 py-gis-utility-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3833 2022-10-24 11:58:12.640807 py-gis-utility-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:58:12.636807 py-gis-utility-0.2.1/py_gis_utility/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/py_gis_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6502 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/py_gis_utility/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/py_gis_utility/image_func.py
--rw-r--r--   0 runner    (1001) docker     (121)     5670 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/py_gis_utility/math_func.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:58:12.640807 py-gis-utility-0.2.1/py_gis_utility/ops/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/py_gis_utility/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3417 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/py_gis_utility/ops/image_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)    20672 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/py_gis_utility/ops/math_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:58:12.636807 py-gis-utility-0.2.1/py_gis_utility.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3833 2022-10-24 11:58:12.000000 py-gis-utility-0.2.1/py_gis_utility.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-10-24 11:58:12.000000 py-gis-utility-0.2.1/py_gis_utility.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 11:58:12.000000 py-gis-utility-0.2.1/py_gis_utility.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-24 11:58:12.000000 py-gis-utility-0.2.1/py_gis_utility.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-24 11:58:12.000000 py-gis-utility-0.2.1/py_gis_utility.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 11:58:12.640807 py-gis-utility-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-10-24 11:58:04.000000 py-gis-utility-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:39:26.434829 py-gis-utility-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-31 10:39:26.430829 py-gis-utility-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:39:26.430829 py-gis-utility-0.2.2/py_gis_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/py_gis_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/py_gis_utility/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/py_gis_utility/image_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/py_gis_utility/math_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:39:26.430829 py-gis-utility-0.2.2/py_gis_utility/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/py_gis_utility/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/py_gis_utility/ops/image_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20672 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/py_gis_utility/ops/math_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:39:26.430829 py-gis-utility-0.2.2/py_gis_utility.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-31 10:39:26.000000 py-gis-utility-0.2.2/py_gis_utility.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-31 10:39:26.000000 py-gis-utility-0.2.2/py_gis_utility.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:39:26.000000 py-gis-utility-0.2.2/py_gis_utility.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-31 10:39:26.000000 py-gis-utility-0.2.2/py_gis_utility.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 10:39:26.000000 py-gis-utility-0.2.2/py_gis_utility.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 10:39:26.434829 py-gis-utility-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-31 10:39:15.000000 py-gis-utility-0.2.2/setup.py
```

### Comparing `py-gis-utility-0.2.1/LICENSE` & `py-gis-utility-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-gis-utility-0.2.1/PKG-INFO` & `py-gis-utility-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-gis-utility
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility for image and math related operation in GIS
 Home-page: https://github.com/fuzailpalnak/py-gis-utility
 Author: Fuzail Palnak
 Author-email: fuzailpalnak@gmail.com
 Keywords: GIS,Image
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-gis-utility Version: 0.2.1 Summary: Utility for
+Metadata-Version: 2.1 Name: py-gis-utility Version: 0.2.2 Summary: Utility for
 image and math related operation in GIS Home-page: https://github.com/
 fuzailpalnak/py-gis-utility Author: Fuzail Palnak Author-email:
 fuzailpalnak@gmail.com Keywords: GIS,Image Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Requires-Python:
```

### Comparing `py-gis-utility-0.2.1/README.md` & `py-gis-utility-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `py-gis-utility-0.2.1/py_gis_utility/helper.py` & `py-gis-utility-0.2.2/py_gis_utility/helper.py`

 * *Files identical despite different names*

### Comparing `py-gis-utility-0.2.1/py_gis_utility/image_func.py` & `py-gis-utility-0.2.2/py_gis_utility/image_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import affine
 import cv2
-import gdal
 import numpy as np
 from typing import Dict, Union
-
+from osgeo import gdal
 from geopandas import GeoDataFrame
 from rasterio.io import BufferedDatasetWriter, DatasetWriter
 
 from py_gis_utility.helper import (
     read_image_with_geo_transform,
     extract_geometry_from_data_frame_row,
     read_data_frame,
```

### Comparing `py-gis-utility-0.2.1/py_gis_utility/math_func.py` & `py-gis-utility-0.2.2/py_gis_utility/math_func.py`

 * *Files identical despite different names*

### Comparing `py-gis-utility-0.2.1/py_gis_utility/ops/image_ops.py` & `py-gis-utility-0.2.2/py_gis_utility/ops/image_ops.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from typing import Dict, Union
 
 import affine
-import gdal
-import osr
+from osgeo import gdal
+from osgeo import osr
 import rasterio
 import numpy as np
 
 from rasterio.features import shapes
 from rasterio.io import BufferedDatasetWriter, DatasetWriter
 from shapely.geometry import shape
 from stitch_n_split.geo_info import get_affine_transform, get_pixel_resolution
@@ -68,14 +68,38 @@
     ):
         yield {
             "geometry": shape(s) if is_shape else s,
             "properties": {"id": v, **kwargs},
         }
 
 
+def get_geo_referenced_image_obj(
+    copy_from: Union[BufferedDatasetWriter, DatasetWriter], copy_to: np.ndarray
+):
+    """
+
+    :param copy_from:
+    :param copy_to:
+    :return:
+    """
+    bands = copy_to.ndim if copy_to.ndim > 2 else 1
+    geo_referenced_image = rasterio.open(
+        "",
+        mode="w",
+        driver=copy_from.driver,
+        width=copy_from.width,
+        height=copy_from.height,
+        crs=copy_from.crs,
+        transform=copy_from.transform,
+        dtype=copy_to.dtype,
+        count=bands,
+    )
+    return geo_referenced_image
+
+
 def copy_geo_reference_to_image(
     copy_from: Union[BufferedDatasetWriter, DatasetWriter],
     copy_to: np.ndarray,
     save_to: str,
 ):
     """
```

### Comparing `py-gis-utility-0.2.1/py_gis_utility/ops/math_ops.py` & `py-gis-utility-0.2.2/py_gis_utility/ops/math_ops.py`

 * *Files identical despite different names*

### Comparing `py-gis-utility-0.2.1/py_gis_utility.egg-info/PKG-INFO` & `py-gis-utility-0.2.2/py_gis_utility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-gis-utility
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility for image and math related operation in GIS
 Home-page: https://github.com/fuzailpalnak/py-gis-utility
 Author: Fuzail Palnak
 Author-email: fuzailpalnak@gmail.com
 Keywords: GIS,Image
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-gis-utility Version: 0.2.1 Summary: Utility for
+Metadata-Version: 2.1 Name: py-gis-utility Version: 0.2.2 Summary: Utility for
 image and math related operation in GIS Home-page: https://github.com/
 fuzailpalnak/py-gis-utility Author: Fuzail Palnak Author-email:
 fuzailpalnak@gmail.com Keywords: GIS,Image Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Requires-Python:
```

### Comparing `py-gis-utility-0.2.1/setup.py` & `py-gis-utility-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         install_requires = f.read().split("\n")
 except FileNotFoundError:
     install_requires = []
 
 
 setup(
     name="py-gis-utility",
-    version="0.2.1",
+    version="0.2.2",
     author="Fuzail Palnak",
     author_email="fuzailpalnak@gmail.com",
     url="https://github.com/fuzailpalnak/py-gis-utility",
     description="Utility for image and math related operation in GIS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

