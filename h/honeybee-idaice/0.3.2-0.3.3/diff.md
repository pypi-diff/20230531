# Comparing `tmp/honeybee-idaice-0.3.2.tar.gz` & `tmp/honeybee-idaice-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.3.2.tar", last modified: Wed May 31 18:51:55 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.3.3.tar", last modified: Wed May 31 19:14:10 2023, max compression
```

## Comparing `honeybee-idaice-0.3.2.tar` & `honeybee-idaice-0.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/bldgbody.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20497 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 18:51:55.000000 honeybee-idaice-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 18:50:37.000000 honeybee-idaice-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/bldgbody.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/setup.py
```

### Comparing `honeybee-idaice-0.3.2/LICENSE` & `honeybee-idaice-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/PKG-INFO` & `honeybee-idaice-0.3.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.2
+Version: 0.3.3
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -13,15 +13,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Honeybee -> IDA-ICE
 
 A honeybee extension to convert HBJSON files to [IDA ICE](https://www.equa.se/en/ida-ice) `idm` files.
 
-![image](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/12840ca3-a94f-4c68-9251-e8eb393bc048)
+![Revit Sample Model](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/97ce39b6-8f45-4dfc-b2f6-152d457a9c82)
 
 Two comments on how the model should be prepared.
 
-1. IDA ICE expects the model to be exported at the finish line of the one - and not the center of the wall.
+1. IDA ICE expects the model to be exported at the finish line of the one instead of the center of the wall.
 1. IDA ICE intersects the faces automatically. Do not intersect the faces in HBJSON files.
+If the model is already intersected, use Pollination Rhino's `PO_RebuildRooms` command to merge the faces together.
 
 The exporter only exports the geometry. None of the energy or Radiance properties are exported.
```

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/archive.py` & `honeybee-idaice-0.3.3/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/bldgbody.py` & `honeybee-idaice-0.3.3/honeybee_idaice/bldgbody.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.3.3/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/face.py` & `honeybee-idaice-0.3.3/honeybee_idaice/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.3.3/honeybee_idaice/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/shade.py` & `honeybee-idaice-0.3.3/honeybee_idaice/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.3.3/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.3.3/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.3.3/honeybee_idaice/templates/building.idm`

 * *Files 0% similar despite different names*

```diff
@@ -495,18 +495,15 @@
  (:IREF :N "Zone_rtn_cold")
  (:IREF :N "DHW_ctl" :T IN :F 208))
 ((SOURCE-FILE :DOCUMENT-PATH "clim:Kalmar.prn" :SF "clim:Kalmar.prn" :N CLIMATE-FILE)
  (:VAR :N TAIR :V 6.92))
 ((AGGREGATE :N PROJDATA)
  (:PAR :N RESP_ENG :V "Ladybug Tools")
  (:PAR :N DESCR :V "This model is auto-generated from an HBJSON file. At this point, the translator only translates the geometry information.Use the Pollination discourse forum if you have any questions or comments: https://discourse.pollination.cloud/"))
-((AGGREGATE :N THREE-D-MODEL :T THREE-D-PLAN)
- ((AGGREGATE :N VIEWPT :T VIEWPOINT)
-  (:PAR :N POSITION :V #(43.464907646758 -51.2386356058975 58.302492260347))
-  (:PAR :N FOCALPOINT :V #(25.0 9.99499988555908 2.5))))
+((AGGREGATE :N THREE-D-MODEL :T THREE-D-PLAN))
 (CONNECTIONS
  ((PLANT "Zone_rtn_cold") ((:LIB WATPLUG) OUTLET) 2 0 NIL)
  ((PLANT "Zone_sup_cold") ((:LIB WATPLUG) INLET) 2 0 NIL)
  ((PLANT "Zone_rtn_hot") ((:LIB WATPLUG) OUTLET) 2 0 NIL)
  ((PLANT "Zone_sup_hot") ((:LIB WATPLUG) INLET) 2 0 NIL)
  ((PLANT "AHU_rtn_hot") ((:LIB WATPLUG) OUTLET) 2 0 NIL)
  ((PLANT "AHU_sup_hot") ((:LIB WATPLUG) INLET) 2 0 NIL)
```

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.3.3/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.3.3/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.3.3/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/writer.py` & `honeybee-idaice-0.3.3/honeybee_idaice/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.3.3/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.3.3/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.2
+Version: 0.3.3
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -13,15 +13,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Honeybee -> IDA-ICE
 
 A honeybee extension to convert HBJSON files to [IDA ICE](https://www.equa.se/en/ida-ice) `idm` files.
 
-![image](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/12840ca3-a94f-4c68-9251-e8eb393bc048)
+![Revit Sample Model](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/97ce39b6-8f45-4dfc-b2f6-152d457a9c82)
 
 Two comments on how the model should be prepared.
 
-1. IDA ICE expects the model to be exported at the finish line of the one - and not the center of the wall.
+1. IDA ICE expects the model to be exported at the finish line of the one instead of the center of the wall.
 1. IDA ICE intersects the faces automatically. Do not intersect the faces in HBJSON files.
+If the model is already intersected, use Pollination Rhino's `PO_RebuildRooms` command to merge the faces together.
 
 The exporter only exports the geometry. None of the energy or Radiance properties are exported.
```

### Comparing `honeybee-idaice-0.3.2/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.3.3/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.2/setup.py` & `honeybee-idaice-0.3.3/setup.py`

 * *Files identical despite different names*

