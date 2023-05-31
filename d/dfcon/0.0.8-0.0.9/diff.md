# Comparing `tmp/dfcon-0.0.8.tar.gz` & `tmp/dfcon-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfcon-0.0.8.tar", last modified: Tue May 30 15:12:22 2023, max compression
+gzip compressed data, was "dfcon-0.0.9.tar", last modified: Tue May 30 16:40:59 2023, max compression
```

## Comparing `dfcon-0.0.8.tar` & `dfcon-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 15:12:22.281090 dfcon-0.0.8/
--rw-rw-rw-   0        0        0     1159 2023-05-30 15:11:14.000000 dfcon-0.0.8/CHANGELOG.md
--rw-rw-rw-   0        0        0     1082 2023-01-30 05:00:07.000000 dfcon-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       53 2023-01-30 14:43:14.000000 dfcon-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2884 2023-05-30 15:12:22.281589 dfcon-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2097 2023-01-30 15:37:22.000000 dfcon-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 15:12:22.244593 dfcon-0.0.8/dfcon/
--rw-rw-rw-   0        0        0      420 2023-05-30 15:09:40.000000 dfcon-0.0.8/dfcon/__init__.py
--rw-rw-rw-   0        0        0    17070 2023-05-30 15:09:20.000000 dfcon-0.0.8/dfcon/directory.py
--rw-rw-rw-   0        0        0     3150 2023-01-30 14:12:01.000000 dfcon-0.0.8/dfcon/filters.py
--rw-rw-rw-   0        0        0    13314 2023-01-30 07:06:17.000000 dfcon-0.0.8/dfcon/path_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:12:22.275633 dfcon-0.0.8/dfcon.egg-info/
--rw-rw-rw-   0        0        0     2884 2023-05-30 15:12:22.000000 dfcon-0.0.8/dfcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-30 15:12:22.000000 dfcon-0.0.8/dfcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 15:12:22.000000 dfcon-0.0.8/dfcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 15:12:22.000000 dfcon-0.0.8/dfcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 15:12:22.283093 dfcon-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2032 2023-01-30 15:39:25.000000 dfcon-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:12:22.278103 dfcon-0.0.8/test/
--rw-rw-rw-   0        0        0     2300 2023-05-30 09:22:33.000000 dfcon-0.0.8/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:40:59.828121 dfcon-0.0.9/
+-rw-rw-rw-   0        0        0     1246 2023-05-30 16:39:59.000000 dfcon-0.0.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1082 2023-01-30 05:00:07.000000 dfcon-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-01-30 14:43:14.000000 dfcon-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2884 2023-05-30 16:40:59.828618 dfcon-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2097 2023-01-30 15:37:22.000000 dfcon-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 16:40:59.784619 dfcon-0.0.9/dfcon/
+-rw-rw-rw-   0        0        0      420 2023-05-30 16:38:59.000000 dfcon-0.0.9/dfcon/__init__.py
+-rw-rw-rw-   0        0        0    17070 2023-05-30 15:09:20.000000 dfcon-0.0.9/dfcon/directory.py
+-rw-rw-rw-   0        0        0     3122 2023-05-30 16:38:26.000000 dfcon-0.0.9/dfcon/filters.py
+-rw-rw-rw-   0        0        0    13314 2023-01-30 07:06:17.000000 dfcon-0.0.9/dfcon/path_filter.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:40:59.823620 dfcon-0.0.9/dfcon.egg-info/
+-rw-rw-rw-   0        0        0     2884 2023-05-30 16:40:59.000000 dfcon-0.0.9/dfcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-30 16:40:59.000000 dfcon-0.0.9/dfcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 16:40:59.000000 dfcon-0.0.9/dfcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 16:40:59.000000 dfcon-0.0.9/dfcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 16:40:59.831632 dfcon-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2032 2023-01-30 15:39:25.000000 dfcon-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:40:59.826119 dfcon-0.0.9/test/
+-rw-rw-rw-   0        0        0     2300 2023-05-30 09:22:33.000000 dfcon-0.0.9/test/test1.py
```

### Comparing `dfcon-0.0.8/CHANGELOG.md` & `dfcon-0.0.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,8 +32,12 @@
 
 ## [0.0.7] - 2023-05-30
 ### Fixed
 - Change update_dir_name() return value: None -> self
 
 ## [0.0.8] - 2023-05-31
 ### Added
-- Supported fuction for copying files in hierarchy.
+- Supported fuction for copying files in hierarchy.
+
+## [0.0.7] - 2023-05-31
+### Fixed
+- Fixed sum bugs. (in Filter.overlap & Filter.tile)
```

### Comparing `dfcon-0.0.8/LICENSE` & `dfcon-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.8/PKG-INFO` & `dfcon-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcon
-Version: 0.0.8
+Version: 0.0.9
 Summary: To make access to the database easier.
 Home-page: https://github.com/MTamon/dataFileController.git
 Author: Tamon Mikawa
 Author-email: mtamon.engineering@gmail.com
 License: MIT License
 Keywords: DataSet,File-Search,File-Controle
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dfcon-0.0.8/README.md` & `dfcon-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.8/dfcon/directory.py` & `dfcon-0.0.9/dfcon/directory.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.8/dfcon/filters.py` & `dfcon-0.0.9/dfcon/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             filters (List[Filter] | Filter)
 
         Returns:
             TiledFilter: Compound filter consisting of a fFilter joined by the OR operator.
         """
 
         if isinstance(filters, Filter):
-            filters = [Filter]
+            pass
         elif not isinstance(filters, list):
             raise TypeError(
                 "The argument 'filters' type must be 'Filter' or 'List[Filter]', "
                 + f"but detect '{filters.__class__.__name__}'",
             )
         elif filters == []:
             return TiledFilter(None)
@@ -47,15 +47,15 @@
             filters (List[Filter] | Filter)
 
         Returns:
             OverlapedFilter: Compound filter consisting of a fFilter joined by the AND operator.
         """
 
         if isinstance(filters, Filter):
-            filters = [Filter]
+            pass
         elif not isinstance(filters, list):
             raise TypeError(
                 "The argument 'filters' type must be 'Filter' or 'List[Filter]', "
                 + f"but detect '{filters.__class__.__name__}'",
             )
         elif filters == []:
             return OverlapedFilter(None)
```

### Comparing `dfcon-0.0.8/dfcon/path_filter.py` & `dfcon-0.0.9/dfcon/path_filter.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.8/dfcon.egg-info/PKG-INFO` & `dfcon-0.0.9/dfcon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcon
-Version: 0.0.8
+Version: 0.0.9
 Summary: To make access to the database easier.
 Home-page: https://github.com/MTamon/dataFileController.git
 Author: Tamon Mikawa
 Author-email: mtamon.engineering@gmail.com
 License: MIT License
 Keywords: DataSet,File-Search,File-Controle
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dfcon-0.0.8/setup.py` & `dfcon-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.8/test/test1.py` & `dfcon-0.0.9/test/test1.py`

 * *Files identical despite different names*

