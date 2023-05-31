# Comparing `tmp/chartart-0.0.3.dev14.tar.gz` & `tmp/chartart-0.0.3.dev15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartart-0.0.3.dev14.tar", last modified: Mon Apr 17 20:00:12 2023, max compression
+gzip compressed data, was "chartart-0.0.3.dev15.tar", last modified: Wed May 31 13:20:42 2023, max compression
```

## Comparing `chartart-0.0.3.dev14.tar` & `chartart-0.0.3.dev15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 20:00:12.384849 chartart-0.0.3.dev14/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/LICENSE
--rw-r--r--   0 dhananjay   (504) staff       (20)     2028 2023-04-17 20:00:12.385225 chartart-0.0.3.dev14/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)     1506 2023-04-17 16:25:20.000000 chartart-0.0.3.dev14/README.md
--rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/pyproject.toml
--rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-04-17 20:00:12.386633 chartart-0.0.3.dev14/setup.cfg
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 20:00:12.354573 chartart-0.0.3.dev14/src/
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 20:00:12.369788 chartart-0.0.3.dev14/src/chartart/
--rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/src/chartart/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/src/chartart/conftest.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/src/chartart/helpers.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    79257 2023-04-17 19:59:11.000000 chartart-0.0.3.dev14/src/chartart/plot.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/src/chartart/simple_eda_template.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/src/chartart/test_plot.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 20:00:12.381557 chartart-0.0.3.dev14/src/chartart/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/src/chartart/tests/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/src/chartart/tests/test_simple.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 20:00:12.378885 chartart-0.0.3.dev14/src/chartart.egg-info/
--rw-r--r--   0 dhananjay   (504) staff       (20)     2028 2023-04-17 20:00:12.000000 chartart-0.0.3.dev14/src/chartart.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-04-17 20:00:12.000000 chartart-0.0.3.dev14/src/chartart.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-04-17 20:00:12.000000 chartart-0.0.3.dev14/src/chartart.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-04-17 20:00:12.000000 chartart-0.0.3.dev14/src/chartart.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-04-17 20:00:12.000000 chartart-0.0.3.dev14/src/chartart.egg-info/top_level.txt
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-04-17 20:00:12.383798 chartart-0.0.3.dev14/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev14/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.888101 chartart-0.0.3.dev15/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/LICENSE
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-05-31 13:20:42.888423 chartart-0.0.3.dev15/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1814 2023-05-31 13:18:32.000000 chartart-0.0.3.dev15/README.md
+-rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/pyproject.toml
+-rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-05-31 13:20:42.890194 chartart-0.0.3.dev15/setup.cfg
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.863726 chartart-0.0.3.dev15/src/
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.878116 chartart-0.0.3.dev15/src/chartart/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/conftest.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/helpers.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    80235 2023-05-31 13:16:14.000000 chartart-0.0.3.dev15/src/chartart/plot.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/simple_eda_template.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/test_plot.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.885937 chartart-0.0.3.dev15/src/chartart/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/tests/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.883654 chartart-0.0.3.dev15/src/chartart.egg-info/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/top_level.txt
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.887132 chartart-0.0.3.dev15/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/tests/test_simple.py
```

### Comparing `chartart-0.0.3.dev14/LICENSE` & `chartart-0.0.3.dev15/LICENSE`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev14/PKG-INFO` & `chartart-0.0.3.dev15/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: chartart
-Version: 0.0.3.dev14
-Summary: ChartArt python package
-Home-page: https://github.com/pypa/sampleproject
-Author: BR-Advisers
-Author-email: info@br-advisers.com
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Keywords: chartart,NLP
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ChartArt Package is under development
 
 Use 
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
 
 Change Log 
@@ -64,7 +48,12 @@
 -Resolved unauthorized error and changed sleep time
 
 0.0.3.dev12 => 0.0.3.dev13
 - Added line/bar/scatter chart subtypes
 - line type : line, area, spline, stepLine, splineArea, stepArea, stackedLine, stackedArea, stackedArea100, stackedLine100
 - bar type : bar,column,stackedBar,stackedColumn,stackedBar,stackedBar100,stackedColumn100  
 - scatter : bubble , if size is specified as list of float scatter chart will get ploted as bubble chart
+
+0.0.3.dev14 => 0.0.3.dev15
+- Tree Map : c (color) param is optional
+- Map : shapeDataField is new optional param (defaults to key 'Name'). primaryValueMapper and data is optional parameters now. This will be usefull for markers/bubbles where we dont need these inputs.
+- Map : added support fo sub layers.
```

### Comparing `chartart-0.0.3.dev14/setup.cfg` & `chartart-0.0.3.dev15/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chartart
-version = 0.0.3.dev14
+version = 0.0.3.dev15
 author = BR-Advisers
 author_email = info@br-advisers.com
 description = ChartArt python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `chartart-0.0.3.dev14/src/chartart/__init__.py` & `chartart-0.0.3.dev15/src/chartart/__init__.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev14/src/chartart/conftest.py` & `chartart-0.0.3.dev15/src/chartart/conftest.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev14/src/chartart/helpers.py` & `chartart-0.0.3.dev15/src/chartart/helpers.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev14/src/chartart/plot.py` & `chartart-0.0.3.dev15/src/chartart/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1246,70 +1246,81 @@
         heatmap_info['vmin'] = vmin
         heatmap_info['vmax'] = vmax
         heatmap_info['showCellValues'] = annotate
         heatmap_info['invertedColors'] = invertedColors
 
         self.data.insert(heatmap_info)
 
-    def treemap(self,levels: list, data : pd.DataFrame,values,c:list,layout: str = "squarified"):
+    def treemap(self,levels: list, data : pd.DataFrame, values,  c: Optional[list] = None, layout: str = "squarified"):
 
         current_fig_type: str = 'treemap'
         if self.check_multi_axes_consistency(current_fig_type):
             self.fig_type = current_fig_type
         self.set_datagrid_figure_details()
         treemap_info: dict = {
             'type': 'treemap',
         }
 
         levelList=[]
-        for level,color in zip(levels,c):
-            levelList.append({"groupMapper": level,
-                              "color": color})
+        if(c == None):
+            for level in levels:
+                levelList.append({"groupMapper": level})
+        else:
+            for level,color in zip(levels,c):
+                levelList.append({"groupMapper": level,
+                                "color": color})
 
         treemap_info["levels"]=levelList
         treemap_info["weightValueMapper"] = values
         treemap_info["layout"] =  layout
         treemap_info["legend"] = {
                            "mode": "bar",
                            "position": "top"
                         }
         treemap_info["enableDrilldown"] =  True
         levels.append(values)
         treemap_info['data'] = data[levels].to_dict(orient='records')
         self.data.insert(treemap_info)
 
-    def map(self, mapOf: str, data: Union[str, list, np.ndarray, pd.Series], primaryValueMapper : str, zoomLevel: Optional[float] = None, focalLatitude: Optional[float] = None, 
+    def map(self, mapOf: str, shapeDataField:  Optional[str] = None, data: Optional[Union[str, list, np.ndarray, pd.Series]] = None, primaryValueMapper : Optional[str] = None, zoomLevel: Optional[float] = None, focalLatitude: Optional[float] = None, 
             focalLongitude: Optional[float] = None, shapeColorValueMapper: Optional[str] = None, shapeColorMapper: Optional[list] = None, 
-            bubbleSizeMapper: Optional[str] = None, bubbleColorValueMapper: Optional[str] = None, bubbleColorMappers: Optional[list] = None, legend: Optional[dict] = None, marker: Optional[list] = None):
+            bubbleSizeMapper: Optional[str] = None, bubbleColorValueMapper: Optional[str] = None, bubbleColorMappers: Optional[list] = None, legend: Optional[dict] = None, marker: Optional[list] = None, layers: Optional[list] = None):
         """Generate Map.
 
         :param mapOf: world or india 
+        :shapeDataField: this is key from geojson. The shapeDataField property is used to refer the unique field name in the .json source to identify each shapes. 
+         This shapeDataField will be used to map with respective value returned in primaryValueMapper from the data source.
         :param data: list of input data values , see example below
         :param primaryValueMapper: key to bind given data to jeo json data.
         :param zoomLevel: Used to set the current zoom level of the map. Default value is 1 which will show the whole map in the viewport.
         :param focalLatitude: Latitude value of focal point of the map layer based on which zooming happens.
         :param focalLongitude: Longitude value of focal point of the map layer based on which zooming happens.
         :param shapeColorValueMapper: A Field from data which decides color of shapes.
         :param shapeColorMapper: A value or range of values and its corresponding color mapping for shapes. 
         :param bubbleSizeMapper: A field from data which decides size of bubble.
         :param bubbleColorValueMapper: A field from data which decides color of shape.
         :param bubbleColorMappers: A value or range of values and its corresponding color mapping for bubbles.
         :param legend: legends for a map.
+        :param marker: place icon markers and tooltip on it.
+        :param layers: add sublayers on top of main chart. (line / arc / polyline/ circle / polygon / shape(geojson))
         :return:
         """
         current_fig_type: str = 'map'
         if self.check_multi_axes_consistency(current_fig_type):
             self.fig_type = current_fig_type
         self.set_datagrid_figure_details()
         map_info: dict = {
             'type': 'map',
         }
 
         map_info["mapOf"] = mapOf
-        map_info["primaryValueMapper"] = primaryValueMapper
+        if shapeDataField is not None:
+            map_info['shapeDataField'] = shapeDataField
+        if primaryValueMapper is not None:
+            map_info["primaryValueMapper"] = primaryValueMapper
         if zoomLevel is not None:
             map_info['zoomLevel'] = zoomLevel
         if focalLatitude is not None:
             map_info['focalLatitude'] = focalLatitude
         if focalLongitude is not None:
             map_info['focalLongitude'] = focalLongitude
         if shapeColorValueMapper is not None:
@@ -1322,16 +1333,20 @@
             map_info['bubbleColorValueMapper'] = bubbleColorValueMapper
         if bubbleColorMappers is not None:
             map_info['bubbleColorMappers'] = bubbleColorMappers
         if legend is not None:
             map_info['legend'] = legend
         if marker is not None:
             map_info['marker'] = marker
+        if layers is not None:
+            map_info['layers'] = layers
+
+        if data is not None:
+            map_info['data'] = data 
 
-        map_info['data'] = data
         self.data.insert(map_info)
 
     def candlestick(self, df: pd.DataFrame, label: Optional[str] = None, indicators: Optional[list] = None, animationDelay: Optional[float] = None, animationDuration: Optional[float] = None):
         """Generate candlestick chart.
 
         :param df: Dataframe with time index and four columns representing
         open, close, high, and low values.
```

### Comparing `chartart-0.0.3.dev14/src/chartart/simple_eda_template.py` & `chartart-0.0.3.dev15/src/chartart/simple_eda_template.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev14/src/chartart/test_plot.py` & `chartart-0.0.3.dev15/src/chartart/test_plot.py`

 * *Files identical despite different names*

