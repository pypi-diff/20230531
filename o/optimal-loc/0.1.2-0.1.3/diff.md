# Comparing `tmp/optimal_loc-0.1.2.tar.gz` & `tmp/optimal_loc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.1.2.tar", max compression
+gzip compressed data, was "optimal_loc-0.1.3.tar", max compression
```

## Comparing `optimal_loc-0.1.2.tar` & `optimal_loc-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.2/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.1.2/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.2/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       87 2023-05-28 23:21:52.311668 optimal_loc-0.1.2/optimal_loc/__init__.py
--rw-r--r--   0        0        0    18115 2023-05-28 23:21:12.583110 optimal_loc-0.1.2/optimal_loc/app.py
--rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.2/optimal_loc/app_constants.py
--rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.2/optimal_loc/bash_command.py
--rw-r--r--   0        0        0     2691 2023-05-28 23:21:12.587249 optimal_loc-0.1.2/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-05-28 23:21:56.009013 optimal_loc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.3/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.1.3/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.3/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       87 2023-05-30 23:50:43.751464 optimal_loc-0.1.3/optimal_loc/__init__.py
+-rw-r--r--   0        0        0    19115 2023-05-30 23:50:23.788871 optimal_loc-0.1.3/optimal_loc/app.py
+-rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.3/optimal_loc/app_constants.py
+-rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.3/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     2691 2023-05-30 23:49:41.453579 optimal_loc-0.1.3/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-05-30 23:50:47.906822 optimal_loc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.1.3/PKG-INFO
```

### Comparing `optimal_loc-0.1.2/LICENSE` & `optimal_loc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.2/README.md` & `optimal_loc-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.2/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.1.3/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.2/optimal_loc/app.py` & `optimal_loc-0.1.3/optimal_loc/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from numpy import array, meshgrid, nan
+from numpy import array, meshgrid, nan, percentile
 from pandas import DataFrame, pivot_table
 from pymongo.mongo_client import MongoClient
 from h3 import geo_to_h3, h3_to_geo, edge_length
 import pickle
 from pulp import LpProblem, LpMinimize, LpVariable, lpSum, PULP_CBC_CMD
+from folium import plugins, Map, CircleMarker, Marker, Icon
+
 
 from optimal_loc.app_constants import (
     HEX_LAT, FROMHEX, TOHEX, HEX_LOCATION, SUPPLY_HEXAGON_ID, TOTAL_EVENT, HEX_ID, HEX_LON, HEXAGON_ID, LATITUDE,
     LONGITUDE, FROMHEX_LAT, FROMHEX_LON, HEXAGON, FILENAME, DISTANCE, SUPPLY_DATA_COLUMN, OPTIMAL_DATA_COLUMN, INDEX
 )
 
 
@@ -33,15 +35,34 @@
     def __init__(self):
         self.supply_data = None
         self.optimal_data = None
         self.hex_distance_data = None
         self.event_frequency_data = None
         self.resolution = None
 
-    def event_frequency(self, raw_data: DataFrame, hex_size: str = 'auto') -> None:
+    def plot_frequency_hexagons(self):
+        plot_data = self.event_frequency_data.copy()
+        perc_90 = percentile(plot_data["total_event"], 90)
+        perc_75 = percentile(plot_data["total_event"], 75)
+        plot_data["colors"] = plot_data["total_event"].apply(lambda x: "red" if x > perc_90 else (
+            "green" if x > perc_75 else "blue"), 1)
+        WHS_COORD = [plot_data['hex_lat'].median(), plot_data['hex_lon'].median()]
+        map_nyc = Map(location=WHS_COORD, zoom_start=10, width=740, height=500)
+
+        for j, i in plot_data.iterrows():
+            CircleMarker((i["hex_lat"], i["hex_lon"]),
+                         radius=5, color=i["colors"],
+                         popup={"Total Event": i["total_event"]}
+                         ).add_to(map_nyc)
+
+        plugins.Fullscreen(position='topleft').add_to(map_nyc)
+
+        return map_nyc
+
+    def event_frequency(self, raw_input_data: DataFrame, hex_size: str = 'auto') -> None:
         """
         Calculate the frequency of events in each hexagonal region.
 
         Parameters:
         raw_data (DataFrame): pandas DataFrame containing event data, with columns "latitude" and "longitude".
         hex_size (string): You can specify hexagon sizes by small, medium or big, otherwise it will be assigned as auto
 
@@ -60,14 +81,15 @@
         Example:
         raw_event_data = pd.DataFrame({'latitude': [42.123, 42.456, 42.789], 'longitude': [-71.123, -71.456, -71.789]})
         object_name = OptimalLoc()
         object_name.event_frequency(raw_event_data)
         event_freq_data = object_name.event_frequency_data
         print(event_freq_data)
         """
+        raw_data = raw_input_data.copy()
         self.resolution = set_resolution(raw_data, hex_size)
 
         raw_data[HEX_ID] = raw_data.apply(lambda x: geo_to_h3(x[LATITUDE], x[LONGITUDE], self.resolution), 1)
 
         raw_data = raw_data[HEX_ID].value_counts().reset_index().rename(columns={INDEX: HEXAGON_ID,
                                                                                  HEX_ID: TOTAL_EVENT})
         raw_data[HEX_LOCATION] = raw_data.apply(lambda x: h3_to_geo(h=x[HEXAGON_ID]), 1)
@@ -102,15 +124,15 @@
         Example:
         raw_event_data = pd.DataFrame({'latitude': [42.123, 42.456, 42.789], 'longitude': [-71.123, -71.456, -71.789]})
         object = OptimalLoc()
         object.create_hexagon_distance_data(raw_event_data)
         hex_distance_data = object.hex_distance_data
         """
         self.event_frequency(raw_data, hex_size)
-        event_data = self.event_frequency_data
+        event_data = self.event_frequency_data.copy()
 
         hexagon_ids = event_data[[HEXAGON_ID, HEX_LAT, HEX_LON]].rename(columns={HEXAGON_ID: HEXAGON})
         out_list = array(meshgrid(hexagon_ids.hexagon, hexagon_ids.hexagon)).T.reshape(-1, 2)
 
         hex_distance_data = DataFrame(data=out_list, columns=[FROMHEX, TOHEX])
 
         hex_distance_data = hex_distance_data.merge(
```

### Comparing `optimal_loc-0.1.2/optimal_loc/app_constants.py` & `optimal_loc-0.1.3/optimal_loc/app_constants.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.2/optimal_loc/st_app.py` & `optimal_loc-0.1.3/optimal_loc/st_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                       optimal_loc_data: DataFrame
                       ):
 
     plot_center = [optimization_data[HEX_LAT].median(), optimization_data[HEX_LON].median()]
     my_map = Map(location=plot_center, zoom_start=12)
 
     for j, i in optimal_data.iterrows():
-        CircleMarker([i[HEX_LAT], i[HEX_LON]],
+        CircleMarker((i[HEX_LAT], i[HEX_LON]),
                      radius=5,
                      color=i["my_colours"]).add_to(my_map)
 
     for j, i in optimal_loc_data.iterrows():
         Marker([i[HEX_LAT], i[HEX_LON]], radius=5,
                icon=Icon(color='red', icon='info-sign')).add_to(my_map)
```

### Comparing `optimal_loc-0.1.2/pyproject.toml` & `optimal_loc-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.1.2"
+version = "0.1.3"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.1.2/PKG-INFO` & `optimal_loc-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
```

