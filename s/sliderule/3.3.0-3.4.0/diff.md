# Comparing `tmp/sliderule-3.3.0.tar.gz` & `tmp/sliderule-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.3.0.tar", last modified: Thu May 11 23:51:59 2023, max compression
+gzip compressed data, was "sliderule-3.4.0.tar", last modified: Wed May 31 19:43:48 2023, max compression
```

## Comparing `sliderule-3.3.0.tar` & `sliderule-3.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 23:51:59.088946 sliderule-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-11 23:51:48.000000 sliderule-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-11 23:51:48.000000 sliderule-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-11 23:51:59.088946 sliderule-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-11 23:51:48.000000 sliderule-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-11 23:51:48.000000 sliderule-3.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 23:51:59.088946 sliderule-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-05-11 23:51:48.000000 sliderule-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 23:51:59.084946 sliderule-3.3.0/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/arcticdem.py
--rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    17509 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    34861 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/raster.py
--rw-r--r--   0 runner    (1001) docker     (122)    45777 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 23:51:59.084946 sliderule-3.3.0/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 23:51:59.088946 sliderule-3.3.0/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/lpdaac_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-11 23:51:48.000000 sliderule-3.3.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 19:43:48.075043 sliderule-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-31 19:43:36.000000 sliderule-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-31 19:43:36.000000 sliderule-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-31 19:43:48.075043 sliderule-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-31 19:43:36.000000 sliderule-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-31 19:43:36.000000 sliderule-3.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 19:43:48.075043 sliderule-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-31 19:43:36.000000 sliderule-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 19:43:48.071043 sliderule-3.4.0/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29288 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17509 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34861 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45777 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-31 19:43:36.000000 sliderule-3.4.0/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 19:43:48.071043 sliderule-3.4.0/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-31 19:43:47.000000 sliderule-3.4.0/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-31 19:43:48.000000 sliderule-3.4.0/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 19:43:47.000000 sliderule-3.4.0/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-31 19:43:47.000000 sliderule-3.4.0/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-31 19:43:47.000000 sliderule-3.4.0/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 19:43:48.075043 sliderule-3.4.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/build_3dep_DEM_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-05-31 19:43:36.000000 sliderule-3.4.0/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-31 19:43:36.000000 sliderule-3.4.0/version.txt
```

### Comparing `sliderule-3.3.0/LICENSE` & `sliderule-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/PKG-INFO` & `sliderule-3.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.3.0
+Version: 3.4.0
 Summary: Python client for interacting with sliderule server
-Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
+Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sliderule-3.3.0/README.md` & `sliderule-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/setup.py` & `sliderule-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 scripts=[os.path.join('utils',f) for f in os.listdir('utils') if f.endswith('.py')]
 
 setup(
     name='sliderule',
     author='SlideRule Developers',
     description='Python client for interacting with sliderule server',
     long_description_content_type="text/markdown",
-    url='https://github.com/ICESat2-SlideRule/sliderule-python/',
+    url='https://github.com/ICESat2-SlideRule/sliderule/',
     license='BSD 3-Clause',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Physics',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
```

### Comparing `sliderule-3.3.0/sliderule/earthdata.py` & `sliderule-3.4.0/sliderule/earthdata.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,19 +29,18 @@
 
 import itertools
 import copy
 import json
 import ssl
 import urllib.request
 import requests
-import datetime
 import logging
-import warnings
 import numpy
 import geopandas
+from datetime import datetime
 from shapely.geometry.multipolygon import MultiPolygon
 from shapely.geometry import Polygon
 import sliderule
 
 
 ###############################################################################
 # GLOBALS
@@ -52,31 +51,35 @@
 
 # default maximum number of resources to process in one request
 DEFAULT_MAX_REQUESTED_RESOURCES = 300
 max_requested_resources = DEFAULT_MAX_REQUESTED_RESOURCES
 
 # best effort match of datasets to providers and versions for earthdata
 DATASETS = {
-    "ATL03":                                {"provider": "NSIDC_ECS",   "version": "005",   "stac": False,  "collections": [] },
-    "ATL06":                                {"provider": "NSIDC_ECS",   "version": "005",   "stac": False,  "collections": []},
-    "ATL08":                                {"provider": "NSIDC_ECS",   "version": "005",   "stac": False,  "collections": []},
-    "GEDI01_B":                             {"provider": "LPDAAC_ECS",  "version": "002",   "stac": False,  "collections": []},
-    "GEDI02_A":                             {"provider": "LPDAAC_ECS",  "version": "002",   "stac": False,  "collections": []},
-    "GEDI02_B":                             {"provider": "LPDAAC_ECS",  "version": "002",   "stac": False,  "collections": []},
-    "GEDI_L3_LandSurface_Metrics_V2_1952":  {"provider": "ORNL_CLOUD",  "version": None,    "stac": False,  "collections": []},
-    "GEDI_L4A_AGB_Density_V2_1_2056":       {"provider": "ORNL_CLOUD",  "version": None,    "stac": False,  "collections": []},
-    "GEDI_L4B_Gridded_Biomass_2017":        {"provider": "ORNL_CLOUD",  "version": None,    "stac": False,  "collections": []},
-    "HLS":                                  {"provider": "LPCLOUD",     "version": None,    "stac": True,   "collections": ["HLSS30.v2.0", "HLSL30.v2.0"]}
+    "ATL03":                                    {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "collections": [] },
+    "ATL06":                                    {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "collections": []},
+    "ATL08":                                    {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "collections": []},
+    "GEDI01_B":                                 {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "collections": []},
+    "GEDI02_A":                                 {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "collections": []},
+    "GEDI02_B":                                 {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "collections": []},
+    "GEDI_L3_LandSurface_Metrics_V2_1952":      {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "collections": []},
+    "GEDI_L4A_AGB_Density_V2_1_2056":           {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "collections": []},
+    "GEDI_L4B_Gridded_Biomass_2017":            {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "collections": []},
+    "HLS":                                      {"provider": "LPCLOUD",     "version": None,   "api": "stac",  "collections": ["HLSS30.v2.0", "HLSL30.v2.0"]},
+    "Digital Elevation Model (DEM) 1 meter":    {"provider": "USGS",        "version": None,   "api": "tnm",   "collections": []}
 }
 
-# page size for requests
+# upper limit on resources returned from CMR query per request
 CMR_PAGE_SIZE = 2000
 
-# upper limit on stac resources returned from stac query per request
-MAX_STAC_RESOURCES_PER_PAGE = 100
+# upper limit on resources returned from STAC query per request
+STAC_PAGE_SIZE = 100
+
+# upper limit on resources returned from TNM query per request
+TNM_PAGE_SIZE = 100
 
 ###############################################################################
 # NSIDC UTILITIES
 ###############################################################################
 # The functions below have been adapted from the NSIDC download script and
 # carry the following notice:
 #
@@ -341,15 +344,15 @@
     context = requests.Session()
     context.trust_env = False # prevent requests from attaching credentials from environment
 
     # build stac request
     url = 'https://cmr.earthdata.nasa.gov/stac/{}/search'.format(provider)
     headers = {'Content-Type': 'application/json'}
     rqst = {
-        "limit": MAX_STAC_RESOURCES_PER_PAGE,
+        "limit": STAC_PAGE_SIZE,
         "datetime": '{}/{}'.format(time_start, time_end),
         "collections": collections,
     }
 
     # add polygon if provided
     if polygons:
         rqst["intersects"] = {
@@ -440,15 +443,15 @@
     '''
     global max_requested_resources
     max_requested_resources = max_resources
 
 #
 #  Common Metadata Repository
 #
-def cmr(short_name=None, version=None, polygon=None, time_start='2018-01-01T00:00:00Z', time_end=datetime.datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ"), return_metadata=False, name_filter=None):
+def cmr(short_name=None, version=None, polygon=None, time_start='2018-01-01T00:00:00Z', time_end=datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ"), return_metadata=False, name_filter=None):
     '''
     Query the `NASA Common Metadata Repository (CMR) <https://cmr.earthdata.nasa.gov>`_ for a list of data within temporal and spatial parameters
 
     Parameters
     ----------
         short_name:         str
                             dataset short name as defined in the `NASA CMR Directory <https://cmr.earthdata.nasa.gov/search/site/collections/directory/eosdis>`_
@@ -495,15 +498,15 @@
 
     # perform query
     return __cmr_search(provider, short_name, version, polygons, time_start, time_end, return_metadata, name_filter)
 
 #
 #  SpatioTemporal Asset Catalog
 #
-def stac(short_name=None, collections=None, polygon=None, time_start='2018-01-01T00:00:00Z', time_end=datetime.datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ"), as_str=False):
+def stac(short_name=None, collections=None, polygon=None, time_start='2018-01-01T00:00:00Z', time_end=datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ"), as_str=True):
     '''
     Perform a STAC query of the `NASA Common Metadata Repository (CMR) <https://cmr.earthdata.nasa.gov>`_ catalog for a list of data within temporal and spatial parameters
 
     Parameters
     ----------
         short_name:     str
                         dataset short name as defined in the `NASA CMR Directory <https://cmr.earthdata.nasa.gov/search/site/collections/directory/eosdis>`_
@@ -574,7 +577,116 @@
     geojson = __stac_search(provider, short_name, collections, polygons, time_start, time_end)
 
     # return
     if as_str:
         return json.dumps(geojson)
     else:
         return geojson
+
+#
+#  The National Map
+#
+def tnm(short_name, polygon, time_start=None, time_end=datetime.utcnow().strftime("%Y-%m-%d"), as_str=True):
+    '''
+    Query `USGS National Map API <https://tnmaccess.nationalmap.gov/api/v1/products>`_ for a list of data within temporal and spatial parameters.  See https://apps.nationalmap.gov/help/documents/TNMAccessAPIDocumentation/TNMAccessAPIDocumentation.pdf for more details on the API.
+
+    Parameters
+    ----------
+        short_name:         str
+                            dataset name
+        polygon:            list
+                            a single list of longitude,latitude in counter-clockwise order with first and last point matching, defining region of interest (see `polygons </web/rtd/user_guide/SlideRule.html#polygons>`_)
+        time_start:         str
+                            starting time for query in format ``<year>-<month>-<day>``
+        time_end:           str
+                            ending time for query in format ``<year>-<month>-<day>``
+
+    Returns
+    -------
+    dict
+        geojson of resources intersecting area of interest
+
+    Examples
+    --------
+        >>> from sliderule import earthdata
+        >>> region = [ {"lon": -108.3435200747503, "lat": 38.89102961045247},
+        ...            {"lon": -107.7677425431139, "lat": 38.90611184543033},
+        ...            {"lon": -107.7818591266989, "lat": 39.26613714985466},
+        ...            {"lon": -108.3605610678553, "lat": 39.25086131372244},
+        ...            {"lon": -108.3435200747503, "lat": 38.89102961045247} ]
+        >>> geojson = earthdata.tnm(short_name='Digital Elevation Model (DEM) 1 meter', polygon=region)
+        >>> geojson
+        {'type': 'FeatureCollection', 'features': [{'type': 'Feature', 'id': '5eaa4a0582cefae35a21ee8c', 'geometry': {'type': 'Polygon'...
+    '''
+    # Flatten polygon (the list must be formated as 'x y, x y, x y, x y, x y', the documentation is incorrect)
+    coord_list = []
+    for coord in polygon:
+        coord_list.append('{} {}'.format(coord["lon"], coord["lat"]))
+    poly_str = ', '.join(coord_list)
+
+    # Create requests context
+    context = requests.Session()
+    context.trust_env = False # prevent requests from attaching credentials from environment
+
+    # Make paged requests to collect all resources that intersect area of interest
+    items = []
+    while True:
+
+        # Build request
+        url='https://tnmaccess.nationalmap.gov/api/v1/products'
+        rqst = {
+            "datasets":     short_name,
+            "polygon":      poly_str,
+            "prodFormats":  'GeoTIFF',
+            "outputFormat": 'JSON',
+            "max":          TNM_PAGE_SIZE,
+            "offset":       len(items)
+        }
+
+        # Optional request parameters
+        if time_start != None:
+            rqst["start"] = time_start
+            rqst["stop"] = time_end
+
+        # Make request
+        rsps = context.get(url, params=rqst)
+        rsps.raise_for_status()
+        data = json.loads(rsps.content)
+        items += data['items']
+        if len(items) == data['total']:
+            break
+
+    # Create GeoJSON
+    geojson = {
+        "type": "FeatureCollection",
+        "features": []
+    }
+    for i in range(len(items)):
+        geojson['features'].append({"type": "Feature"})
+        id = items[i]['sourceId']
+        geojson['features'][i].update({"id": id})
+
+        # Create polygon from bounding box
+        minX = items[i]['boundingBox']['minX']
+        maxX = items[i]['boundingBox']['maxX']
+        minY = items[i]['boundingBox']['minY']
+        maxY = items[i]['boundingBox']['maxY']
+
+        # Counter-clockwise for interior of bounding box
+        coordList = [[[minX, minY], [maxX, minY], [maxX, maxY], [minX, maxY], [minX, minY]]]
+
+        geometryDic = {"type": "Polygon", "coordinates": coordList}
+        geojson['features'][i].update({"geometry": geometryDic})
+
+        date = items[i]['lastUpdated']
+        pydate = datetime.fromisoformat(date)
+        date = pydate.astimezone(None).isoformat()
+        url  = items[i]['urls']['TIFF']
+        propertiesDict = {"datetime": date, "url": url }
+        geojson['features'][i].update({"properties": propertiesDict})
+
+    # Return GeoJSON
+    if as_str:
+        return json.dumps(geojson)
+    else:
+        return geojson
+
```

### Comparing `sliderule-3.3.0/sliderule/gedi.py` & `sliderule-3.4.0/sliderule/gedi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/sliderule/h5.py` & `sliderule-3.4.0/sliderule/h5.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,18 +89,18 @@
     Returns
     -------
     numpy array
         dataset values
 
     Examples
     --------
-        >>> segments    = icesat2.h5("/gt1r/land_ice_segments/segment_id",  resource, asset)
-        >>> heights     = icesat2.h5("/gt1r/land_ice_segments/h_li",        resource, asset)
-        >>> latitudes   = icesat2.h5("/gt1r/land_ice_segments/latitude",    resource, asset)
-        >>> longitudes  = icesat2.h5("/gt1r/land_ice_segments/longitude",   resource, asset)
+        >>> segments    = h5.h5("/gt1r/land_ice_segments/segment_id",  resource, asset)
+        >>> heights     = h5.h5("/gt1r/land_ice_segments/h_li",        resource, asset)
+        >>> latitudes   = h5.h5("/gt1r/land_ice_segments/latitude",    resource, asset)
+        >>> longitudes  = h5.h5("/gt1r/land_ice_segments/longitude",   resource, asset)
         >>> df = pd.DataFrame(data=list(zip(heights, latitudes, longitudes)), index=segments, columns=["h_mean", "latitude", "longitude"])
     '''
     tstart = time.perf_counter()
     datasets = [ { "dataset": dataset, "datatype": datatype, "col": col, "startrow": startrow, "numrows": numrows } ]
     values = h5p(datasets, resource, asset=asset)
     if len(values) > 0:
         profiles[h5.__name__] = time.perf_counter() - tstart
@@ -150,15 +150,15 @@
         ...         {"dataset": "/gt1l/land_ice_segments/h_li", "numrows": 5},
         ...         {"dataset": "/gt1r/land_ice_segments/h_li", "numrows": 5},
         ...         {"dataset": "/gt2l/land_ice_segments/h_li", "numrows": 5},
         ...         {"dataset": "/gt2r/land_ice_segments/h_li", "numrows": 5},
         ...         {"dataset": "/gt3l/land_ice_segments/h_li", "numrows": 5},
         ...         {"dataset": "/gt3r/land_ice_segments/h_li", "numrows": 5}
         ...     ]
-        >>> rsps = icesat2.h5p(datasets, "ATL06_20181019065445_03150111_003_01.h5", "atlas-local")
+        >>> rsps = h5.h5p(datasets, "ATL06_20181019065445_03150111_003_01.h5", "atlas-local")
         >>> print(rsps)
         {'/gt2r/land_ice_segments/h_li': array([45.3146427 , 45.27640582, 45.23608027, 45.21131015, 45.15692304]),
          '/gt2l/land_ice_segments/h_li': array([45.35118977, 45.33535027, 45.27195617, 45.21816889, 45.18534204]),
          '/gt1l/land_ice_segments/h_li': array([45.68811156, 45.71368944, 45.74234326, 45.74614113, 45.79866465]),
          '/gt3l/land_ice_segments/h_li': array([45.29602321, 45.34764226, 45.31430979, 45.31471701, 45.30034622]),
          '/gt1r/land_ice_segments/h_li': array([45.72632446, 45.76512574, 45.76337375, 45.77102473, 45.81307948]),
          '/gt3r/land_ice_segments/h_li': array([45.14954134, 45.18970635, 45.16637644, 45.15235916, 45.17135806])}
```

### Comparing `sliderule-3.3.0/sliderule/icesat2.py` & `sliderule-3.4.0/sliderule/icesat2.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/sliderule/io.py` & `sliderule-3.4.0/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/sliderule/ipxapi.py` & `sliderule-3.4.0/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/sliderule/ipysliderule.py` & `sliderule-3.4.0/sliderule/ipysliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/sliderule/raster.py` & `sliderule-3.4.0/sliderule/raster.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/sliderule/sliderule.py` & `sliderule-3.4.0/sliderule/sliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/sliderule.egg-info/PKG-INFO` & `sliderule-3.4.0/sliderule.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.3.0
+Version: 3.4.0
 Summary: Python client for interacting with sliderule server
-Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
+Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sliderule-3.3.0/sliderule.egg-info/SOURCES.txt` & `sliderule-3.4.0/sliderule.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 version.txt
 sliderule/__init__.py
-sliderule/arcticdem.py
 sliderule/earthdata.py
 sliderule/gedi.py
 sliderule/h5.py
 sliderule/icesat2.py
 sliderule/io.py
 sliderule/ipxapi.py
 sliderule/ipysliderule.py
@@ -18,14 +17,15 @@
 sliderule/version.py
 sliderule.egg-info/PKG-INFO
 sliderule.egg-info/SOURCES.txt
 sliderule.egg-info/dependency_links.txt
 sliderule.egg-info/requires.txt
 sliderule.egg-info/top_level.txt
 utils/big_query.py
+utils/build_3dep_DEM_geojson.py
 utils/build_arctic_dem_mosaics_index.py
 utils/build_arctic_dem_mosaics_vrt_list.py
 utils/build_arctic_dem_strips_vrt.py
 utils/extract_h5_dataset.py
 utils/icepyx_region.py
 utils/lpdaac_download.py
 utils/monitor.py
```

### Comparing `sliderule-3.3.0/utils/big_query.py` & `sliderule-3.4.0/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.4.0/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.4.0/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.4.0/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/extract_h5_dataset.py` & `sliderule-3.4.0/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/icepyx_region.py` & `sliderule-3.4.0/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/lpdaac_download.py` & `sliderule-3.4.0/utils/lpdaac_download.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/monitor.py` & `sliderule-3.4.0/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/query_cmr.py` & `sliderule-3.4.0/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/query_elevations.py` & `sliderule-3.4.0/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/query_metrics.py` & `sliderule-3.4.0/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/query_photons.py` & `sliderule-3.4.0/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/query_stac.py` & `sliderule-3.4.0/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/query_version.py` & `sliderule-3.4.0/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/region_of_interest.py` & `sliderule-3.4.0/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/results_to_s3.py` & `sliderule-3.4.0/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/stac.py` & `sliderule-3.4.0/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/stream_events.py` & `sliderule-3.4.0/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/tail_events.py` & `sliderule-3.4.0/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.3.0/utils/utils.py` & `sliderule-3.4.0/utils/utils.py`

 * *Files identical despite different names*

