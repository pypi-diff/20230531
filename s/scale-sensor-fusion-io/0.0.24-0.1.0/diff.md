# Comparing `tmp/scale_sensor_fusion_io-0.0.24.tar.gz` & `tmp/scale_sensor_fusion_io-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_sensor_fusion_io-0.0.24.tar", max compression
+gzip compressed data, was "scale_sensor_fusion_io-0.1.0.tar", max compression
```

## Comparing `scale_sensor_fusion_io-0.0.24.tar` & `scale_sensor_fusion_io-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,58 @@
--rw-r--r--   0        0        0      867 2023-05-17 00:36:10.812070 scale_sensor_fusion_io-0.0.24/pyproject.toml
--rw-r--r--   0        0        0       95 2023-05-04 15:36:43.270532 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/__init__.py
--rw-r--r--   0        0        0       52 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/loaders/__init__.py
--rw-r--r--   0        0        0     2716 2023-05-04 15:36:43.270532 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/loaders/bs5_loader.py
--rw-r--r--   0        0        0     2837 2023-05-04 15:36:43.270532 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/loaders/sfs_loader.py
--rw-r--r--   0        0        0       96 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/__init__.py
--rw-r--r--   0        0        0      456 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/__init__.py
--rw-r--r--   0        0        0      512 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/attributes.py
--rw-r--r--   0        0        0      626 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/box_2d.py
--rw-r--r--   0        0        0     1129 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/cuboid.py
--rw-r--r--   0        0        0      520 2023-05-05 02:52:04.396890 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/event.py
--rw-r--r--   0        0        0      690 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/labeled_points.py
--rw-r--r--   0        0        0      924 2023-05-12 21:39:19.819533 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
--rw-r--r--   0        0        0      425 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/object.py
--rw-r--r--   0        0        0      638 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/polygon.py
--rw-r--r--   0        0        0      509 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/common.py
--rw-r--r--   0        0        0      109 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/paths/__init__.py
--rw-r--r--   0        0        0      291 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/paths/attribute_path.py
--rw-r--r--   0        0        0     5350 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/paths/cuboid_path.py
--rw-r--r--   0        0        0    16186 2023-05-05 02:52:04.400889 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/paths/pose_path.py
--rw-r--r--   0        0        0      593 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/scene.py
--rw-r--r--   0        0        0      253 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/__init__.py
--rw-r--r--   0        0        0       94 2023-04-19 20:43:33.126613 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/camera/__init__.py
--rw-r--r--   0        0        0     6318 2023-05-12 21:39:19.819533 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
--rw-r--r--   0        0        0      310 2023-05-12 21:39:19.819533 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
--rw-r--r--   0        0        0      896 2023-05-12 21:39:19.819533 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
--rw-r--r--   0        0        0       27 2023-04-19 20:43:33.126613 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
--rw-r--r--   0        0        0      931 2023-05-05 02:52:04.400889 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
--rw-r--r--   0        0        0       28 2023-04-19 20:43:33.126613 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/radar/__init__.py
--rw-r--r--   0        0        0      825 2023-05-12 21:39:19.819533 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
--rw-r--r--   0        0        0       22 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/LICENSE
--rw-r--r--   0        0        0      297 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/README.md
--rw-r--r--   0        0        0      135 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/__init__.py
--rw-r--r--   0        0        0      502 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/config.py
--rw-r--r--   0        0        0     7388 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/core.py
--rw-r--r--   0        0        0       90 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/data.py
--rw-r--r--   0        0        0     1121 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/dataclasses.py
--rw-r--r--   0        0        0     2949 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/exceptions.py
--rw-r--r--   0        0        0     8189 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/types.py
--rw-r--r--   0        0        0     7554 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/helpers.py
--rw-r--r--   0        0        0    10500 2023-05-12 21:39:19.823533 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/parser.py
--rw-r--r--   0        0        0        0 2023-03-29 20:56:32.935581 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/py.typed
--rw-r--r--   0        0        0       91 2023-05-04 15:36:43.270532 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/spec/__init__.py
--rw-r--r--   0        0        0       21 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/spec/sfs/__init__.py
--rw-r--r--   0        0        0     7837 2023-05-17 00:36:10.812070 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/spec/sfs/types.py
--rw-r--r--   0        0        0       21 2023-05-01 17:27:01.060541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/spec/v5/__init__.py
--rw-r--r--   0        0        0     3001 2023-05-17 00:36:10.812070 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/spec/v5/types.py
--rw-r--r--   0        0        0        0 2023-05-01 17:27:01.064541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/utils/__init__.py
--rw-r--r--   0        0        0     2005 2023-05-01 17:27:01.064541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/utils/downsample.py
--rw-r--r--   0        0        0     1857 2023-05-01 17:27:01.064541 scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/utils/generate_video.py
--rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.0.24/PKG-INFO
+-rw-r--r--   0        0        0     2945 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/docs/README.md
+-rw-r--r--   0        0        0      883 2023-05-31 21:21:03.307775 scale_sensor_fusion_io-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-25 07:12:37.457890 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/loaders/__init__.py
+-rw-r--r--   0        0        0     2716 2023-05-22 20:30:40.190095 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/loaders/bs5_loader.py
+-rw-r--r--   0        0        0     3088 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/loaders/sfs_loader.py
+-rw-r--r--   0        0        0       19 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/model_converters/__init__.py
+-rw-r--r--   0        0        0     8175 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/model_converters/sfs.py
+-rw-r--r--   0        0        0       96 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/__init__.py
+-rw-r--r--   0        0        0      456 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/attributes.py
+-rw-r--r--   0        0        0      626 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/box_2d.py
+-rw-r--r--   0        0        0     1129 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/cuboid.py
+-rw-r--r--   0        0        0      520 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/event.py
+-rw-r--r--   0        0        0      690 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/labeled_points.py
+-rw-r--r--   0        0        0      924 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
+-rw-r--r--   0        0        0      425 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/object.py
+-rw-r--r--   0        0        0      638 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/polygon.py
+-rw-r--r--   0        0        0      509 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/common.py
+-rw-r--r--   0        0        0      109 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/paths/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/paths/attribute_path.py
+-rw-r--r--   0        0        0     5350 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/paths/cuboid_path.py
+-rw-r--r--   0        0        0    16186 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/paths/pose_path.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/scene.py
+-rw-r--r--   0        0        0      253 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/__init__.py
+-rw-r--r--   0        0        0       94 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/camera/__init__.py
+-rw-r--r--   0        0        0     6340 2023-05-23 23:02:19.283596 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
+-rw-r--r--   0        0        0      310 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
+-rw-r--r--   0        0        0      896 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
+-rw-r--r--   0        0        0       27 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
+-rw-r--r--   0        0        0      931 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
+-rw-r--r--   0        0        0       28 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/radar/__init__.py
+-rw-r--r--   0        0        0      825 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
+-rw-r--r--   0        0        0        0 2023-03-29 20:56:32.935581 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/py.typed
+-rw-r--r--   0        0        0       91 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/spec/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/spec/sfs/__init__.py
+-rw-r--r--   0        0        0     7837 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/spec/sfs/types.py
+-rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/spec/v5/__init__.py
+-rw-r--r--   0        0        0     3001 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/spec/v5/types.py
+-rw-r--r--   0        0        0        0 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/utils/__init__.py
+-rw-r--r--   0        0        0     2005 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/utils/downsample.py
+-rw-r--r--   0        0        0     2730 2023-05-31 15:52:17.723567 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/utils/generate_video.py
+-rw-r--r--   0        0        0      899 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/LICENSE
+-rw-r--r--   0        0        0      297 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/README.md
+-rw-r--r--   0        0        0      135 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-25 17:06:14.174721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/config.py
+-rw-r--r--   0        0        0     7388 2023-05-25 17:06:14.178721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/core.py
+-rw-r--r--   0        0        0       90 2023-05-25 17:06:14.178721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/data.py
+-rw-r--r--   0        0        0     1121 2023-05-25 17:06:14.178721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py
+-rw-r--r--   0        0        0     2949 2023-05-25 17:06:14.178721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py
+-rw-r--r--   0        0        0     8189 2023-05-25 17:06:14.178721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/types.py
+-rw-r--r--   0        0        0     2802 2023-05-31 21:08:46.057329 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/error.py
+-rw-r--r--   0        0        0      965 2023-05-25 17:06:14.178721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/helpers.py
+-rw-r--r--   0        0        0       19 2023-05-25 17:06:14.178721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/parser/__init__.py
+-rw-r--r--   0        0        0     7530 2023-05-25 17:06:14.178721 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/parser/sfs.py
+-rw-r--r--   0        0        0     6932 2023-05-29 18:51:19.676454 scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/validate.py
+-rw-r--r--   0        0        0     3756 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.1.0/PKG-INFO
```

### Comparing `scale_sensor_fusion_io-0.0.24/pyproject.toml` & `scale_sensor_fusion_io-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "scale_sensor_fusion_io"
-version = "0.0.24"
+version = "0.1.0"
 description = "Library for working with timestamp-based sensor fusion scenes"
 authors = [
     "Michael Choi <michael.choi@scale.com>", 
     "Rodrigo Belfiore <rodrigo.belfiore@scale.com>"
 ]
+readme = ["docs/README.md"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numpy = "^1.22.4"
 ujson = "^5.7.0"
 pandas = "^2.0.0"
 scipy = "^1.10.1"
@@ -21,16 +22,15 @@
 mypy = "^0.991"
 types-ujson = "^5.7.0"
 pytest = "^7.2.2"
 
 [[tool.poetry.source]]
 name = "scale-pypi"
 url = "https://scale-307185671274.d.codeartifact.us-west-2.amazonaws.com/pypi/scale-pypi/simple/"
-default = false
-secondary = true
+priority = "explicit"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/loaders/bs5_loader.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/loaders/bs5_loader.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/loaders/sfs_loader.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/loaders/sfs_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from enum import Enum
-from typing import Optional, cast
+from typing import cast
 
 import dacite
 from scale_json_binary import JSONBinaryEncoder
+import scale_sensor_fusion_io.models
+from scale_sensor_fusion_io.model_converters import from_scene_spec_sfs
 
 from ..spec import SFS
 
 encoder = JSONBinaryEncoder()
 
 
 def _fix_data_shape(scene: SFS.Scene) -> SFS.Scene:
@@ -40,15 +42,19 @@
 class SFSLoader:
     def __init__(
         self,
         scene_url: str,
     ):
         self.scene_url = scene_url
 
-    def load(self) -> SFS.Scene:
+    def load(self) -> scale_sensor_fusion_io.models.Scene:
+        scene_sfs = self.load_as_sfs()
+        return from_scene_spec_sfs(scene_sfs)
+
+    def load_as_sfs(self) -> SFS.Scene:
         raw_data: bytes
         with open(self.scene_url, "rb") as fd:
             raw_data = cast(bytes, fd.read())
 
         obj = encoder.loads(raw_data)
         if "version" not in obj or not obj["version"].startswith("1.0"):
             raise Exception(f"Cannot load scene with version {obj['version']}")
```

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/attributes.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/attributes.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/box_2d.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/box_2d.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/cuboid.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/cuboid.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/event.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/event.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/labeled_points.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/labeled_points.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/localization_adjustment.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/localization_adjustment.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/annotations/polygon.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/annotations/polygon.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/paths/cuboid_path.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/paths/cuboid_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/paths/pose_path.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/paths/pose_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/scene.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/scene.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 @dataclass
 class Scene:
     sensors: Optional[List[Sensor]] = None
     annotations: Optional[List[Annotation]] = None
     attributes: Optional[List[AttributePath]] = None
     time_offset: Optional[int] = None
     time_unit: Optional[
-        Literal["milliseconds", "microseconds", "nanoseconds"]
+        Literal["microseconds", "nanoseconds"]
     ] = "microseconds"
 
     def add_sensor(self) -> None:
         pass
```

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,16 +159,18 @@
     elif isinstance(distortion, Mapping):
         distortion_fields = {k: v for k, v in distortion.items()}
     elif is_dataclass(distortion):
         distortion_fields = asdict(distortion)
     else:
         distortion_fields = distortion.__dict__
 
-    model: DistortionModel = distortion_fields.get(
-        "model", distortion_fields.get("camera_model", DistortionModel.BROWN_CONRADY)
+    model: DistortionModel = (
+        distortion_fields.get("model")
+        or distortion_fields.get("camera_model")
+        or DistortionModel.BROWN_CONRADY
     )
 
     dataclass = get_params_from_model(model)
     # construct param dict for dataclass
     d = {}
     for key in dataclass.__dataclass_fields__:
         if (
```

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/LICENSE` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/LICENSE`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/core.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/core.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/dataclasses.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/exceptions.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/dacite_internal/types.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/dacite_internal/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/parsers/helpers.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/validation/validate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,240 +1,228 @@
-# from enum import Enum
-# from typing_extensions import TypeAlias
-# from typing import Any, List, Type, Literal, Optional, Union, Tuple, TypeVar, Generic
-# from scale_json_binary import read_file
-# from scale_sensor_fusion_io.models import (
-#     PosePath,
-#     Scene,
-#     SensorID,
-#     AnnotationID,
-#     CameraSensor,
-#     CameraIntrinsics,
-#     Sensor,
-#     LidarSensor,
-#     LidarSensorFrame,
-#     LidarSensorPoints,
-#     RadarSensor,
-# )
-# 
-# from dataclasses import dataclass, field, asdict
-# from scale_sensor_fusion_io.spec import BS5
-# 
-# import dacite
-# import ujson
-# 
-# from scale_sensor_fusion_io.parsers.dacite_internal.types import is_instance
-# from scale_sensor_fusion_io.parsers import dacite_internal
-# 
-# from scale_sensor_fusion_io.models.sensors.camera.camera_sensor import CameraDistortion
-# 
-# def parse_parent_id(sensor: dict) -> ParseResult[Optional[SensorID]]:
-#     """Parse parent id from sensor object"""
-#     parent_id = sensor.get("parent_id")
-#     if parent_id and not (type(parent_id) == int or type(parent_id) == str):
-#         return ParseError.from_msg(
-#             f"Invalid sensor id provided: {parent_id}. Only int or string supported",
-#             path="parent_id",
-#         )
-# 
-#     return ParseSuccess(parent_id)
-# 
-# 
-# def parse_sensor_id(sensor: dict) -> ParseResult[SensorID]:
-#     """Parse sensor id from sensor object"""
-#     # sensor id
-#     sensor_id = sensor.get("id")
-#     if not sensor_id:
-#         return ParseError.from_msg(f"Missing field: id", path="id")
-# 
-#     if not (type(sensor_id) == int or type(sensor_id) == str):
-#         return ParseError.from_msg(
-#             f"Invalid sensor id provided: {sensor_id}. Only int or string supported",
-#             path="id",
-#         )
-# 
-#     return ParseSuccess(sensor_id)
-# 
-# 
-# def parse_pose_path(sensor: dict) -> ParseResult[PosePath]:
-#     """
-#     Parse pose_path from sensor object
-#     """
-#     error_details = []
-#     poses = sensor.get("poses")
-#     if not poses:
-#         return ParseError.missing_field("poses")
-# 
-#     values = poses.get("values")
-#     if values is None:
-#         error_details.append(
-#             ErrorDetails.missing_field("values", path=["poses", "values"])
-#         )
-# 
-#     timestamps = poses.get("timestamps")
-#     if timestamps is None:
-#         error_details.append(
-#             ErrorDetails.missing_field("timestamps", path=["poses", "timestamps"])
-#         )
-# 
-#     try:
-#         pose_path = PosePath(values, timestamps)
-#     except Exception as e:
-#         error_details.append(
-#             ErrorDetails.from_msg(
-#                 f"Unable to instantiate PosePath. Error: {e}", path="poses"
-#             )
-#         )
-# 
-#     if len(error_details) > 0:
-#         return ParseError(details=error_details)
-#     return ParseSuccess(pose_path)
-# 
-# 
-# 
-# def parse_camera_intrinsics(intrinsics: dict) -> ParseResult[CameraIntrinsics]:
-#     error_details = []
-# 
-#     CUSTOM_CHECK = ["distortion"]
-# 
-#     # for field_key, field_data in BS5.CameraIntrinsics.__dataclass_fields__.items():
-#     #     if field_key in CUSTOM_CHECK:
-#     #         continue
-# 
-#     #     if not is_instance(intrinsics.get(field_key), field_data.type):
-#     #         error_details.append(ErrorDetails.wrong_type(field_key))
-# 
-#     # print(BS5.CameraIntrinsics(**intrinsics))
-# 
-#     init_values = intrinsics
-#     # fx = intrinsics.get("fx")
-#     # if fx is None:
-#     #     error_details.append(ErrorDetails.missing_field("fx"))
-# 
-#     # fy = intrinsics.get("fy")
-#     # if fy is None:
-#     #     error_details.append(ErrorDetails.missing_field("fy"))
-# 
-#     # cx = intrinsics.get("cx")
-#     # if cx is None:
-#     #     error_details.append(ErrorDetails.missing_field("cx"))
-# 
-#     # cy = intrinsics.get("cy")
-#     # if cy is None:
-#     #     error_details.append(ErrorDetails.missing_field("cy"))
-# 
-#     # width = intrinsics.get("width")
-#     # if width is None:
-#     #     error_details.append(ErrorDetails.missing_field("width"))
-# 
-#     # height = intrinsics.get("height")
-#     # if height is None:
-#     #     error_details.append(ErrorDetails.missing_field("height"))
-# 
-#     _distortion = intrinsics.get("distortion")
-#     distortion = None
-#     if _distortion:
-#         model = _distortion.get("model")
-#         if model is None:
-#             error_details.append(
-#                 ErrorDetails.missing_field("model", path=["distortion"])
-#             )
-# 
-#         params = _distortion.get("params")
-#         if params is None:
-#             error_details.append(
-#                 ErrorDetails.missing_field("params", path=["distortion"])
-#             )
-# 
-#         if model and params:
-#             distortion = CameraDistortion.from_values(model, params)
-#             init_values["distortion"] = distortion
-# 
-#     if len(error_details) > 0:
-#         return ParseError(details=error_details)
-#     return ParseSuccess(data=CameraIntrinsics(**init_values))
-
-# def parse_lidar_frame(frame: dict) -> ParseResult[LidarSensorFrame]:
-#     error_details: List[ErrorDetails] = []
-# 
-#     timestamp = frame.get("timestamp")
-#     if timestamp is None:
-#         error_details.append(ErrorDetails.missing_field("timestamp"))
-# 
-#     points = frame.get("points")
-#     if points is None:
-#         error_details.append(ErrorDetails.missing_field("points"))
-# 
-#     return ParseSuccess(
-#         LidarSensorFrame(
-#             timestamp=timestamp,
-#             points=points,
-#         )
-#     )
-# 
-# 
-# def parse_lidar(sensor: dict) -> ParseResult[LidarSensor]:
-#     error_details: List[ErrorDetails] = []
-# 
-#     # frames
-#     _frames = sensor.get("frames")
-#     if _frames is None:
-#         error_details.append(ErrorDetails.missing_field("frames"))
-#     if type(_frames) != list:
-#         error_details.append(
-#             ErrorDetails.from_msg("frames must be a list", path="frames")
-#         )
-#     else:
-#         for idx, frame in enumerate(_frames):
-#             result = parse_lidar_frame(frame)
-#             if result.success:
-#                 frames = result.data
-#             else:
-#                 error_details.extend(result.prepend_path(["frames", idx]).details)
-# 
-#     # coordinates
-#     coordinates = sensor.get("coordinates")
-#     if coordinates is None:
-#         error_details.append(ErrorDetails.missing_field("coordinates"))
-#     if coordinates != "ego" and coordinates != "world":
-#         error_details.append(
-#             ErrorDetails.from_msg(
-#                 f"Coordinates must be either 'ego' or 'world'. Provided '{coordinates}'",
-#                 path="coordinates",
-#             )
-#         )
-# 
-#     # parent id
-#     result = parse_parent_id(sensor)
-#     if result.success:
-#         parent_id = result.data
-#     else:
-#         error_details.extend(result.details)
-# 
-#     # sensor id
-#     result = parse_sensor_id(sensor)
-#     if result.success:
-#         sensor_id = result.data
-#     else:
-#         error_details.extend(result.details)
-# 
-#     # pose path
-#     result = parse_pose_path(sensor)
-#     if result.success:
-#         pose_path = result.data
-#     else:
-#         error_details.extend(result.details)
-# 
-#     if len(error_details) > 0:
-#         return ParseError(details=error_details)
-# 
-#     return ParseSuccess(
-#         LidarSensor(
-#             id=sensor_id,
-#             poses=pose_path,
-#             frames=frames,
-#             parent_id=parent_id,
-#             coordinates=coordinates,
-#         )
-#     )
-# 
-# 
+from dataclasses import asdict, dataclass
+from typing import List
+
+import numpy as np
+from scale_sensor_fusion_io.models import (
+    CameraDistortion,
+    CameraIntrinsics,
+    CameraSensor,
+    LidarSensor,
+    LidarSensorFrame,
+    LidarSensorPoints,
+    PosePath,
+    RadarSensor,
+    RadarSensorFrame,
+    RadarSensorPoints,
+    Scene,
+    Sensor,
+    SensorKind,
+)
+
+from .error import (
+    DataValidationError,
+    ErrorDetails,
+    PathField,
+    ValidationResult,
+)
+from .helpers import is_monotonically_increasing
+
+MICRO_IN_SEC = 1e6
+
+
+def _handle_result(
+    res: ValidationResult, error_details: List[ErrorDetails], path: List[PathField] = []
+) -> None:
+    if res:
+        error_details.extend(
+            res.details if not path else res.prepend_path(path).details
+        )
+
+    return None
+
+
+def validate_radar(sensor: RadarSensor) -> ValidationResult:
+    """Validate lidar sensor"""
+    error_details: List[ErrorDetails] = []
+    content_timestamps = [frame.timestamp for frame in sensor.frames]
+
+    _handle_result(
+        validate_timestamps(content_timestamps), error_details, path=["frames"]
+    )
+    _handle_result(validate_fps(content_timestamps), error_details)
+
+    if len(error_details) > 0:
+        return DataValidationError(details=error_details)
+
+    return None
+
+
+def validate_timestamps(timestamps: List[int]) -> ValidationResult:
+    error_details: List[ErrorDetails] = []
+    if any(ts < 0 for ts in timestamps):
+        error_details.append(
+            ErrorDetails.from_msg(
+                "timestamps must not be negative",
+            )
+        )
+    if not is_monotonically_increasing(timestamps):
+        error_details.append(
+            ErrorDetails.from_msg(
+                "timestamps be monotonically increasing",
+            )
+        )
+    if len(error_details) > 0:
+        return DataValidationError(details=error_details)
+    return None
+
+
+def validate_fps(timestamps: List[int], max_fps: int = 100) -> ValidationResult:
+    error_details: List[ErrorDetails] = []
+
+    # compute approximate fps from timestamps
+    avg_ts_diffs = np.mean([t2 - t1 for t1, t2 in zip(timestamps, timestamps[1:])])
+    fps = MICRO_IN_SEC / avg_ts_diffs
+
+    if fps > max_fps:
+        error_details.append(
+            ErrorDetails.from_msg(
+                f"approximate fps is too high: {fps} > {max_fps}",
+            )
+        )
+
+    if len(error_details) > 0:
+        return DataValidationError(details=error_details)
+
+    return None
+
+
+def validate_lidar(sensor: LidarSensor) -> ValidationResult:
+    """Validate lidar sensor"""
+    error_details: List[ErrorDetails] = []
+    content_timestamps = [frame.timestamp for frame in sensor.frames]
+
+    _handle_result(
+        validate_timestamps(content_timestamps), error_details, path=["frames"]
+    )
+    _handle_result(validate_fps(content_timestamps), error_details)
+
+    for frame in sensor.frames:
+        ### validate all fields of points have same length
+        pos_length = len(frame.points.positions)
+        if (
+            frame.points.intensities is not None
+            and len(frame.points.intensities) != pos_length
+        ):
+            error_details.append(
+                ErrorDetails.from_msg(
+                    f"length of positions ({len(frame.points.positions)}) and intensities ({len(frame.points.intensities)}) must be the same"
+                )
+            )
+
+        if frame.points.colors is not None and len(frame.points.colors) != pos_length:
+            error_details.append(
+                ErrorDetails.from_msg(
+                    f"length of positions ({len(frame.points.positions)}) and colors ({len(frame.points.colors)}) must be the same"
+                )
+            )
+
+        if (
+            frame.points.timestamps is not None
+            and len(frame.points.timestamps) != pos_length
+        ):
+            error_details.append(
+                ErrorDetails.from_msg(
+                    f"length of positions ({len(frame.points.positions)}) and timestamps ({len(frame.points.timestamps)}) must be the same"
+                )
+            )
+
+    if len(error_details) > 0:
+        return DataValidationError(details=error_details)
+
+    return None
+
+
+def validate_camera(sensor: CameraSensor) -> ValidationResult:
+    """Validate camera sensor"""
+    error_details: List[ErrorDetails] = []
+
+    # camera content
+    content_timestamps: List[int] = []
+    content_timestamps_path: List[PathField] = []
+    if sensor.video:
+        content_timestamps = sensor.video.timestamps
+        content_timestamps_path = ["video"]
+    elif sensor.images:
+        content_timestamps = [img.timestamp for img in sensor.images]
+        content_timestamps_path = ["images"]
+    else:
+        error_details.append(
+            ErrorDetails.from_msg('Exactly one of "images" or "video" expected')
+        )
+
+    _handle_result(
+        validate_timestamps(content_timestamps),
+        error_details,
+        path=content_timestamps_path,
+    )
+    _handle_result(
+        validate_fps(content_timestamps),
+        error_details,
+    )
+
+    if len(error_details) > 0:
+        return DataValidationError(details=error_details)
+
+    return None
+
+
+def validate_sensor(sensor: Sensor) -> ValidationResult:
+    error_details: List[ErrorDetails] = []
+    if sensor.type is SensorKind.Camera:
+        _handle_result(validate_camera(sensor), error_details)
+    elif sensor.type is SensorKind.Lidar:
+        _handle_result(validate_lidar(sensor), error_details)
+    elif sensor.type is SensorKind.Radar:
+        _handle_result(validate_radar(sensor), error_details)
+    else:
+        error_details.append(
+            ErrorDetails(
+                path=["type"], errors=[f"Invalid sensor type provided: {sensor.type}"]
+            )
+        )
+    if len(error_details) > 0:
+        return DataValidationError(details=error_details)
+
+    return None
+
+
+def validate_scene(scene: Scene) -> ValidationResult:
+    """Validate scene"""
+    error_details: List[ErrorDetails] = []
+    if scene.sensors:
+        for sensor in scene.sensors:
+            _handle_result(
+                validate_sensor(sensor),
+                error_details,
+                path=["sensors", str(sensor.id)],
+            )
+
+        if len(scene.sensors) != len(set([sensor.id for sensor in scene.sensors])):
+            error_details.append(
+                ErrorDetails.from_msg("Sensor ids must be unique", path=["sensors"])
+            )
+
+    if scene.time_unit != "microseconds":
+        error_details.append(
+            ErrorDetails.from_msg(
+                f"Invalid time unit provided: {scene.time_unit}. Expected: microseconds"
+            )
+        )
+
+    if scene.time_offset is not None and scene.time_offset < 0:
+        error_details.append(
+            ErrorDetails.from_msg("Scene timestamp must not be negative")
+        )
+
+    if len(error_details) > 0:
+        return DataValidationError(details=error_details)
+    return None
```

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/spec/sfs/types.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/spec/sfs/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/spec/v5/types.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/spec/v5/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/utils/downsample.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/utils/downsample.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.0.24/scale_sensor_fusion_io/utils/generate_video.py` & `scale_sensor_fusion_io-0.1.0/scale_sensor_fusion_io/utils/generate_video.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import subprocess
+import tempfile
 from typing import Any, List
 
 import cv2
 import ffmpeg
 import numpy as np
 import numpy.typing as npt
 import skvideo.io
@@ -40,20 +42,50 @@
 
     def __exit__(self, exc_type: Any, exc_value: Any, exc_traceback: Any) -> None:
         if self.count > 0:
             self.writer.close()
 
 
 def generate_video(
-    image_files: List[str], target_file: str = "tmp.mp4"
+    image_files: List[str], target_file: str = "out.mp4", fps=10, threads=4
 ) -> npt.NDArray[np.uint8]:
-    with VideoWriter(target_file) as writer:
-        for image_file in image_files:
-            writer.writeFrame(cv2.imread(image_file))
-    return np.fromfile(target_file, dtype=np.uint8)
+    """Generate a video from a list of image files using ffmpeg as a subprocess"""
+    duration = 1 / fps
+    with tempfile.NamedTemporaryFile(mode="w", dir=".") as tmp_fp:
+        tmp_fp.write(
+            "\n".join(f"file {name}\nduration {duration:04f}" for name in image_files)
+        )
+
+        # Call ffmpeg as a subprocess to generate the video
+        subprocess.call(
+            [
+                "ffmpeg",
+                "-hide_banner",
+                "-loglevel",
+                "error",
+                "-y",
+                "-f",
+                "concat",
+                "-i",
+                tmp_fp.name,
+                "-vcodec",
+                "libx264",
+                "-x264-params",
+                "keyint=2:scenecut=0",
+                "-pix_fmt",
+                "yuv420p",
+                "-crf",
+                "24",
+                "-r",
+                str(fps),
+                "-threads",
+                str(threads),
+                target_file,
+            ]
+        )
 
 
 def write_audio_and_video(audio_file: str, video_file: str, output_file: str) -> None:
     if not os.path.isfile(audio_file) or not os.path.isfile(video_file):
         raise ValueError("Audio or video file does not exist")
 
     input_video = ffmpeg.input(video_file)
```

