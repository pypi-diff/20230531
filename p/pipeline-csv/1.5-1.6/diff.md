# Comparing `tmp/pipeline_csv-1.5.tar.gz` & `tmp/pipeline_csv-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_csv-1.5.tar", last modified: Mon May  8 07:01:45 2023, max compression
+gzip compressed data, was "pipeline_csv-1.6.tar", last modified: Wed May 31 08:07:44 2023, max compression
```

## Comparing `pipeline_csv-1.5.tar` & `pipeline_csv-1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 07:01:45.342965 pipeline_csv-1.5/
--rw-rw-rw-   0        0        0     1094 2023-03-13 10:59:03.000000 pipeline_csv-1.5/LICENSE
--rw-rw-rw-   0        0        0       60 2023-03-14 17:31:18.000000 pipeline_csv-1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7171 2023-05-08 07:01:45.342965 pipeline_csv-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6634 2023-05-04 09:42:35.000000 pipeline_csv-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 07:01:45.311714 pipeline_csv-1.5/pipeline_csv/
--rw-rw-rw-   0        0        0      701 2023-03-15 17:59:16.000000 pipeline_csv-1.5/pipeline_csv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:01:45.342965 pipeline_csv-1.5/pipeline_csv/csvfile/
--rw-rw-rw-   0        0        0    13072 2023-05-05 10:15:19.000000 pipeline_csv-1.5/pipeline_csv/csvfile/README.md
--rw-rw-rw-   0        0        0    10238 2023-05-06 10:11:21.000000 pipeline_csv-1.5/pipeline_csv/csvfile/__init__.py
--rw-rw-rw-   0        0        0    16783 2023-05-04 09:42:35.000000 pipeline_csv-1.5/pipeline_csv/csvfile/row.py
--rw-rw-rw-   0        0        0     4943 2023-05-06 10:11:21.000000 pipeline_csv-1.5/pipeline_csv/csvfile/tubes.py
--rw-rw-rw-   0        0        0     5965 2023-03-29 13:25:05.000000 pipeline_csv-1.5/pipeline_csv/oegiv.py
--rw-rw-rw-   0        0        0     2267 2023-04-14 04:49:03.000000 pipeline_csv-1.5/pipeline_csv/orientation.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:01:45.327340 pipeline_csv-1.5/pipeline_csv.egg-info/
--rw-rw-rw-   0        0        0     7171 2023-05-08 07:01:45.000000 pipeline_csv-1.5/pipeline_csv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-05-08 07:01:45.000000 pipeline_csv-1.5/pipeline_csv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 07:01:45.000000 pipeline_csv-1.5/pipeline_csv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 07:01:45.000000 pipeline_csv-1.5/pipeline_csv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-03-14 17:31:18.000000 pipeline_csv-1.5/pyproject.toml
--rw-rw-rw-   0        0        0      664 2023-05-08 07:01:45.342965 pipeline_csv-1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 08:07:44.382492 pipeline_csv-1.6/
+-rw-rw-rw-   0        0        0     1094 2023-03-13 10:59:03.000000 pipeline_csv-1.6/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-03-14 17:31:18.000000 pipeline_csv-1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7171 2023-05-31 08:07:44.382492 pipeline_csv-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6634 2023-05-04 09:42:35.000000 pipeline_csv-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 08:07:44.351240 pipeline_csv-1.6/pipeline_csv/
+-rw-rw-rw-   0        0        0      701 2023-03-15 17:59:16.000000 pipeline_csv-1.6/pipeline_csv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 08:07:44.382492 pipeline_csv-1.6/pipeline_csv/csvfile/
+-rw-rw-rw-   0        0        0    13072 2023-05-05 10:15:19.000000 pipeline_csv-1.6/pipeline_csv/csvfile/README.md
+-rw-rw-rw-   0        0        0    10238 2023-05-06 10:11:21.000000 pipeline_csv-1.6/pipeline_csv/csvfile/__init__.py
+-rw-rw-rw-   0        0        0    16783 2023-05-04 09:42:35.000000 pipeline_csv-1.6/pipeline_csv/csvfile/row.py
+-rw-rw-rw-   0        0        0     5701 2023-05-31 08:04:00.000000 pipeline_csv-1.6/pipeline_csv/csvfile/tubes.py
+-rw-rw-rw-   0        0        0     5965 2023-03-29 13:25:05.000000 pipeline_csv-1.6/pipeline_csv/oegiv.py
+-rw-rw-rw-   0        0        0     2267 2023-04-14 04:49:03.000000 pipeline_csv-1.6/pipeline_csv/orientation.py
+drwxrwxrwx   0        0        0        0 2023-05-31 08:07:44.366868 pipeline_csv-1.6/pipeline_csv.egg-info/
+-rw-rw-rw-   0        0        0     7171 2023-05-31 08:07:44.000000 pipeline_csv-1.6/pipeline_csv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-31 08:07:44.000000 pipeline_csv-1.6/pipeline_csv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 08:07:44.000000 pipeline_csv-1.6/pipeline_csv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 08:07:44.000000 pipeline_csv-1.6/pipeline_csv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-03-14 17:31:18.000000 pipeline_csv-1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      664 2023-05-31 08:07:44.382492 pipeline_csv-1.6/setup.cfg
```

### Comparing `pipeline_csv-1.5/LICENSE` & `pipeline_csv-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.5/PKG-INFO` & `pipeline_csv-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline_csv
-Version: 1.5
+Version: 1.6
 Summary: Pipeline inline inspection data as CSV file.
 Home-page: https://github.com/vb64/pipeline.csv
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/pipeline.csv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pipeline_csv-1.5/README.md` & `pipeline_csv-1.6/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.5/pipeline_csv/__init__.py` & `pipeline_csv-1.6/pipeline_csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.5/pipeline_csv/csvfile/README.md` & `pipeline_csv-1.6/pipeline_csv/csvfile/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.5/pipeline_csv/csvfile/__init__.py` & `pipeline_csv-1.6/pipeline_csv/csvfile/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.5/pipeline_csv/csvfile/row.py` & `pipeline_csv-1.6/pipeline_csv/csvfile/row.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.5/pipeline_csv/csvfile/tubes.py` & `pipeline_csv-1.6/pipeline_csv/csvfile/tubes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tubes iterator interface for csv file."""
 from .. import Error, TypeHorWeld
+from ..orientation import Orientation
 
 
 def summary_text(objects, names):
     """Return summary text for given items."""
     items = {}
     for item in objects:
         code = int(item.object_code)
@@ -25,15 +26,15 @@
         self.auto_number = auto_number
         self.stream = stream
 
         self.length = None
         self.thick = None
         self.category = None
 
-        self.is_thick_change = False
+        self.is_thick_change = None
         self.is_category_change = False
 
         self.seams = []
         self.lineobjects = []
         self.defects = []
         self.categories = []
         self.thicks = []
@@ -68,16 +69,16 @@
                 self.stream.category = category
                 self.is_category_change = True
             self.categories.append(row)
 
         elif row.is_thick:
             thick = int(row.depth_max)
             if self.stream.thick != thick:
+                self.is_thick_change = self.stream.thick
                 self.stream.thick = thick
-                self.is_thick_change = True
             self.thicks.append(row)
 
         else:
             raise Error("Tube at dist {} has wrong row: {}".format(self.dist, str(row)))
 
     def set_geo(self, latitude, longtitude, altitude):
         """Set geo coords for tube."""
@@ -139,29 +140,44 @@
         return ', '.join([i for i in [
           summary_text(self.defects, defect_names),
           summary_text(self.lineobjects, line_names)
         ] if i])
 
     @property
     def typ(self):
-        """Pipe type according pipe seams data."""
+        """Return pipe type according pipe seams data."""
         if not self.seams:
             return TypeHorWeld.UNKNOWN
 
         return int(self.seams[0].object_code)
 
     @property
-    def seam_info(self):
-        """Return text string with seams orientation."""
-        text = ''
-        if self.typ == TypeHorWeld.HORIZONTAL:
+    def seam1(self):
+        """Return orientation in minutes for longditual and spiral first pipe seam."""
+        ornt = None
+        if (len(self.seams) > 0) and (self.typ in [TypeHorWeld.HORIZONTAL, TypeHorWeld.SECOND, TypeHorWeld.SPIRAL]):
             text = self.seams[0].orient_td
-        elif self.typ == TypeHorWeld.SECOND:
-            text = self.seams[0].orient_td + ' / ' + self.seams[0].orient_bd
-        elif self.typ == TypeHorWeld.SPIRAL:
-            text = ' / '.join([i.orient_td for i in self.seams])
+            ornt = Orientation.from_csv(text).as_minutes if text else None
+
+        return ornt
+
+    @property
+    def seam2(self):
+        """Return orientation in minutes for longditual and spiral second pipe seam."""
+        ornt = None
+        if (len(self.seams) > 0) and (self.typ == TypeHorWeld.SECOND):
+            text = self.seams[0].orient_bd
+            ornt = Orientation.from_csv(text).as_minutes if text else None
+        elif (len(self.seams) > 1) and (self.typ == TypeHorWeld.SPIRAL):
+            text = self.seams[-1].orient_td
+            ornt = Orientation.from_csv(text).as_minutes if text else None
 
-        return text
+        return ornt
+
+    @property
+    def seam_info(self):
+        """Return text string with seams orientation."""
+        return ' / '.join([str(Orientation.from_minutes(i)) for i in [self.seam1, self.seam2] if i])
 
     def features(self):
         """Return defects and lineobjects of the pipe, arranged by distance."""
         return sorted(self.lineobjects + self.defects, key=lambda i: i.dist)
```

### Comparing `pipeline_csv-1.5/pipeline_csv/oegiv.py` & `pipeline_csv-1.6/pipeline_csv/oegiv.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.5/pipeline_csv/orientation.py` & `pipeline_csv-1.6/pipeline_csv/orientation.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.5/pipeline_csv.egg-info/PKG-INFO` & `pipeline_csv-1.6/pipeline_csv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-csv
-Version: 1.5
+Version: 1.6
 Summary: Pipeline inline inspection data as CSV file.
 Home-page: https://github.com/vb64/pipeline.csv
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/pipeline.csv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pipeline_csv-1.5/setup.cfg` & `pipeline_csv-1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6970 656c 696e 655f 6373 760d   = pipeline_csv.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e35 0d0a  .version = 1.5..
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e36 0d0a  .version = 1.6..
 00000030: 6175 7468 6f72 203d 2056 6974 616c 7920  author = Vitaly 
 00000040: 426f 676f 6d6f 6c6f 760d 0a61 7574 686f  Bogomolov..autho
 00000050: 725f 656d 6169 6c20 3d20 6d61 696c 4076  r_email = mail@v
 00000060: 6974 616c 792d 626f 676f 6d6f 6c6f 762e  italy-bogomolov.
 00000070: 7275 0d0a 6465 7363 7269 7074 696f 6e20  ru..description 
 00000080: 3d20 5069 7065 6c69 6e65 2069 6e6c 696e  = Pipeline inlin
 00000090: 6520 696e 7370 6563 7469 6f6e 2064 6174  e inspection dat
```

