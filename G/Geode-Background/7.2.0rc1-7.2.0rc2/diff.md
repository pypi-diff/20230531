# Comparing `tmp/Geode_Background-7.2.0rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Background-7.2.0rc2-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 3436779 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      195 b- defN 23-May-30 15:30 geode_background/__init__.py
--rw-rw-rw-  2.0 fat      199 b- defN 23-May-30 15:30 geode_background/solid.py
--rw-rw-rw-  2.0 fat      203 b- defN 23-May-30 15:30 geode_background/surface.py
--rw-rw-rw-  2.0 fat  2136576 b- defN 23-May-30 15:31 geode_background/bin/Geode-Background_brep.dll
--rw-rw-rw-  2.0 fat    67072 b- defN 23-May-30 15:31 geode_background/bin/Geode-Background_common.dll
--rw-rw-rw-  2.0 fat  2380800 b- defN 23-May-30 15:31 geode_background/bin/Geode-Background_solid.dll
--rw-rw-rw-  2.0 fat  2175488 b- defN 23-May-30 15:31 geode_background/bin/Geode-Background_surface.dll
--rw-rw-rw-  2.0 fat   125440 b- defN 23-May-30 15:31 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   124928 b- defN 23-May-30 15:31 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 23-May-30 15:31 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1112 b- defN 23-May-30 15:31 Geode_Background-7.2.0rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-30 15:31 Geode_Background-7.2.0rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-30 15:31 Geode_Background-7.2.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1398 b- defN 23-May-30 15:31 Geode_Background-7.2.0rc1.dist-info/RECORD
-14 files, 7138968 bytes uncompressed, 3434405 bytes compressed:  51.9%
+Zip file size: 4584266 bytes, number of entries: 14
+-rw-r--r--  2.0 unx       90 b- defN 23-May-31 08:17 geode_background/__init__.py
+-rw-r--r--  2.0 unx      192 b- defN 23-May-31 08:17 geode_background/solid.py
+-rw-r--r--  2.0 unx      196 b- defN 23-May-31 08:17 geode_background/surface.py
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-May-31 08:18 geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-May-31 08:18 geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-May-31 08:18 geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  3235248 b- defN 23-May-31 08:18 geode_background/lib64/libGeode-Background_brep.so
+-rwxr-xr-x  2.0 unx   170672 b- defN 23-May-31 08:18 geode_background/lib64/libGeode-Background_common.so
+-rwxr-xr-x  2.0 unx  3540560 b- defN 23-May-31 08:18 geode_background/lib64/libGeode-Background_solid.so
+-rwxr-xr-x  2.0 unx  3260464 b- defN 23-May-31 08:18 geode_background/lib64/libGeode-Background_surface.so
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-31 08:18 Geode_Background-7.2.0rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-May-31 08:18 Geode_Background-7.2.0rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-31 08:18 Geode_Background-7.2.0rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1456 b- defN 23-May-31 08:18 Geode_Background-7.2.0rc2.dist-info/RECORD
+14 files, 10576762 bytes uncompressed, 4581776 bytes compressed:  56.7%
```

## zipnote {}

```diff
@@ -3,41 +3,41 @@
 
 Filename: geode_background/solid.py
 Comment: 
 
 Filename: geode_background/surface.py
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_brep.dll
+Filename: geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_common.dll
+Filename: geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_solid.dll
+Filename: geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_surface.dll
+Filename: geode_background/lib64/libGeode-Background_brep.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_common.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_solid.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_surface.so
 Comment: 
 
-Filename: Geode_Background-7.2.0rc1.dist-info/METADATA
+Filename: Geode_Background-7.2.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Background-7.2.0rc1.dist-info/WHEEL
+Filename: Geode_Background-7.2.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Background-7.2.0rc1.dist-info/top_level.txt
+Filename: Geode_Background-7.2.0rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Background-7.2.0rc1.dist-info/RECORD
+Filename: Geode_Background-7.2.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_background/__init__.py

```diff
@@ -1,7 +1,4 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .surface import *
-from .solid import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .surface import *
+from .solid import *
```

## geode_background/solid.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_solid import *
-BackgroundSolidLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_solid import *
+BackgroundSolidLibrary.initialize()
```

## geode_background/surface.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_surface import *
-BackgroundSurfaceLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_surface import *
+BackgroundSurfaceLibrary.initialize()
```

## Comparing `Geode_Background-7.2.0rc1.dist-info/METADATA` & `Geode_Background-7.2.0rc2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1
-Name: Geode-Background
-Version: 7.2.0rc1
-Summary: Geode-solutions OpenGeode module for building background meshes
-Home-page: https://github.com/Geode-solutions/Geode-Background
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-common (==26.*,>=26.0.0rc1)
-Requires-Dist: opengeode-core (==14.*,>=14.1.10rc5)
-
-<h1 align="center">BackgroundMesh<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Module to generate a background mesh for OpenGeode</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/BackgroundMesh_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/BackgroundMesh_private.svg" alt="Version">
-</p>
-
-
+Metadata-Version: 2.1
+Name: Geode-Background
+Version: 7.2.0rc2
+Summary: Geode-solutions OpenGeode module for building background meshes
+Home-page: https://github.com/Geode-solutions/Geode-Background
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-common (==26.*,>=26.0.0rc1)
+Requires-Dist: opengeode-core (==14.*,>=14.1.10rc5)
+
+<h1 align="center">BackgroundMesh<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Module to generate a background mesh for OpenGeode</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/BackgroundMesh_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/BackgroundMesh_private.svg" alt="Version">
+</p>
```

