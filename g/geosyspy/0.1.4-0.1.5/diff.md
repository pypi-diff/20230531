# Comparing `tmp/geosyspy-0.1.4.tar.gz` & `tmp/geosyspy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosyspy-0.1.4.tar", last modified: Tue May 30 14:04:21 2023, max compression
+gzip compressed data, was "geosyspy-0.1.5.tar", last modified: Wed May 31 08:19:48 2023, max compression
```

## Comparing `geosyspy-0.1.4.tar` & `geosyspy-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-30 14:04:21.371617 geosyspy-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-30 14:02:30.000000 geosyspy-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 14:02:30.000000 geosyspy-0.1.4/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/geosyspy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35285 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/geosys.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/image_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/geosyspy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/geosys_platform_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/oauth2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/geosyspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 14:04:21.371617 geosyspy-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-30 14:02:30.000000 geosyspy-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_int_geosys.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_unit_geosys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_unit_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_unit_oauth2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.964245 geosyspy-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-31 08:19:48.964245 geosyspy-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-31 08:18:02.000000 geosyspy-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 08:18:02.000000 geosyspy-0.1.5/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.960245 geosyspy-0.1.5/geosyspy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/image_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.964245 geosyspy-0.1.5/geosyspy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/geosys_platform_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-31 08:18:02.000000 geosyspy-0.1.5/geosyspy/utils/oauth2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.964245 geosyspy-0.1.5/geosyspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 08:19:48.000000 geosyspy-0.1.5/geosyspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 08:19:48.964245 geosyspy-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-31 08:18:02.000000 geosyspy-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:19:48.964245 geosyspy-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_int_geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_unit_geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_unit_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-31 08:18:02.000000 geosyspy-0.1.5/tests/test_unit_oauth2_client.py
```

### Comparing `geosyspy-0.1.4/PKG-INFO` & `geosyspy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geosyspy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easy-to-use python wrapper for Geosys APIs (time series, imagery products)
 Author: Geosys
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 <!--
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_vj53xp33_/tmpowg60jkt_TarContainer/0/1", line 25, column 4: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_vj53xp33_/tmpowg60jkt_TarContainer/0/1", line 25, column 4: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geosyspy Version: 0.1.4 Summary: Easy-to-use python
+Metadata-Version: 2.1 Name: geosyspy Version: 0.1.5 Summary: Easy-to-use python
 wrapper for Geosys APIs (time series, imagery products) Author: Geosys
 Description-Content-Type: text/markdown
 
                                     [Logo]
                             ****** GeosysPy ******
   To be able to discover, request and use imagery products based on  virtual
                    constellation using the &ltgeosys/> API.
```

### Comparing `geosyspy-0.1.4/README.md` & `geosyspy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/geosyspy/geosys.py` & `geosyspy-0.1.5/geosyspy/geosys.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
             end_date : The end date of the time series
             collections : The Satellite Imagery Collection targeted
             indicators : The indicators to retrieve on the collections
 
         Returns:
             ('dataframe or xarray'): Either a pandas dataframe or a xarray for the time series
         """
+
         if not collections:
             raise ValueError(
                 "The argument collections is empty. It must be a list of SatelliteImageryCollection objects"
             )
         elif all([isinstance(elem, SatelliteImageryCollection) for elem in collections]):
             if set(collections).issubset(set(LR_SATELLITE_COLLECTION)):
                 return self.__get_time_series_by_pixel(
@@ -671,15 +672,15 @@
                                          "landsat_8", "landsat_9", "cbers4", "kazstsat",
                                          "alsat_1b", "huanjing_2", "deimos", "gaofen_1", "gaofen_6",
                                         "resourcesat2","dmc_2","landsat_5","landsat_7",
                                         "spot","rapideye_3a", "rapideye_1b"],
                             denoiser: bool =True,
                             smoother: str ="ww",
                             eoc: bool =True,
-                            func: str ="mean",
+                            aggregation: str ="mean",
                             index: str ="ndvi",
                             raw_data: bool =False
                             ):
 
         """Retrieve mr time series on the collection targeted.
 
         Args:
@@ -707,15 +708,15 @@
             "parameters": {
                 "start_date": start_date,
                 "end_date": end_date,
                 "sensors": list_sensors,
                 "denoiser": denoiser,
                 "smoother": smoother,
                 "eoc": eoc,
-                "aggregation": func,
+                "aggregation": aggregation,
                 "index": index,
                 "raw_data": raw_data
             },
             "data": [
                 {"wkt": polygon}
             ]
         }
```

### Comparing `geosyspy-0.1.4/geosyspy/utils/constants.py` & `geosyspy-0.1.5/geosyspy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/geosyspy/utils/geosys_platform_urls.py` & `geosyspy-0.1.5/geosyspy/utils/geosys_platform_urls.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/geosyspy/utils/helper.py` & `geosyspy-0.1.5/geosyspy/utils/helper.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/geosyspy/utils/http_client.py` & `geosyspy-0.1.5/geosyspy/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/geosyspy/utils/oauth2_client.py` & `geosyspy-0.1.5/geosyspy/utils/oauth2_client.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/geosyspy.egg-info/PKG-INFO` & `geosyspy-0.1.5/geosyspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geosyspy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easy-to-use python wrapper for Geosys APIs (time series, imagery products)
 Author: Geosys
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 <!--
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_vj53xp33_/tmpowg60jkt_TarContainer/0/16", line 25, column 4: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_vj53xp33_/tmpowg60jkt_TarContainer/0/16", line 25, column 4: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geosyspy Version: 0.1.4 Summary: Easy-to-use python
+Metadata-Version: 2.1 Name: geosyspy Version: 0.1.5 Summary: Easy-to-use python
 wrapper for Geosys APIs (time series, imagery products) Author: Geosys
 Description-Content-Type: text/markdown
 
                                     [Logo]
                             ****** GeosysPy ******
   To be able to discover, request and use imagery products based on  virtual
                    constellation using the &ltgeosys/> API.
```

### Comparing `geosyspy-0.1.4/geosyspy.egg-info/SOURCES.txt` & `geosyspy-0.1.5/geosyspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/setup.py` & `geosyspy-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     description="Easy-to-use python wrapper for Geosys APIs (time series, imagery products)",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Geosys",
     packages=find_packages(),
     include_package_data=True,
     data_files=[('', ['VERSION.txt'])],
-    install_requires=["requests", "requests-oauthlib", "oauthlib", "scipy", "pandas==1.3.5", "shapely", "rasterio", "xarray", "boto3"]
-)
+    install_requires=["requests", "requests-oauthlib", "oauthlib", "scipy", "pandas==1.3.5", "shapely", "rasterio", "xarray"]
+)
```

### Comparing `geosyspy-0.1.4/tests/test_helper.py` & `geosyspy-0.1.5/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/tests/test_int_geosys.py` & `geosyspy-0.1.5/tests/test_int_geosys.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/tests/test_unit_geosys.py` & `geosyspy-0.1.5/tests/test_unit_geosys.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/tests/test_unit_http_client.py` & `geosyspy-0.1.5/tests/test_unit_http_client.py`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.4/tests/test_unit_oauth2_client.py` & `geosyspy-0.1.5/tests/test_unit_oauth2_client.py`

 * *Files identical despite different names*

