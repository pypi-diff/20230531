# Comparing `tmp/histomics_stream-2.3.3.tar.gz` & `tmp/histomics_stream-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomics_stream-2.3.3.tar", last modified: Tue Mar 28 14:24:47 2023, max compression
+gzip compressed data, was "histomics_stream-2.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `histomics_stream-2.3.3.tar` & `histomics_stream-2.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11982 2023-03-28 14:24:39.848466 histomics_stream-2.3.3/README.md
--rw-r--r--   0        0        0     1009 2023-03-28 14:24:39.852467 histomics_stream-2.3.3/histomics_stream/__init__.py
--rw-r--r--   0        0        0     4411 2023-03-28 14:24:39.852467 histomics_stream-2.3.3/histomics_stream/codecs.py
--rw-r--r--   0        0        0    47414 2023-03-28 14:24:39.852467 histomics_stream-2.3.3/histomics_stream/configure.py
--rw-r--r--   0        0        0     9060 2023-03-28 14:24:39.852467 histomics_stream-2.3.3/histomics_stream/pytorch.py
--rw-r--r--   0        0        0    12352 2023-03-28 14:24:39.852467 histomics_stream-2.3.3/histomics_stream/tensorflow.py
--rw-r--r--   0        0        0      763 2023-03-28 14:24:39.852467 histomics_stream-2.3.3/pyproject.toml
--rw-r--r--   0        0        0    12681 1970-01-01 00:00:00.000000 histomics_stream-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11982 2023-05-31 17:23:00.240452 histomics_stream-2.4.0/README.md
+-rw-r--r--   0        0        0     1009 2023-05-31 17:23:00.240452 histomics_stream-2.4.0/histomics_stream/__init__.py
+-rw-r--r--   0        0        0     4411 2023-05-31 17:23:00.240452 histomics_stream-2.4.0/histomics_stream/codecs.py
+-rw-r--r--   0        0        0    47972 2023-05-31 17:23:00.244452 histomics_stream-2.4.0/histomics_stream/configure.py
+-rw-r--r--   0        0        0    10919 2023-05-31 17:23:00.244452 histomics_stream-2.4.0/histomics_stream/pytorch.py
+-rw-r--r--   0        0        0    12445 2023-05-31 17:23:00.244452 histomics_stream-2.4.0/histomics_stream/tensorflow.py
+-rw-r--r--   0        0        0      770 2023-05-31 17:23:00.244452 histomics_stream-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12688 1970-01-01 00:00:00.000000 histomics_stream-2.4.0/PKG-INFO
```

### Comparing `histomics_stream-2.3.3/README.md` & `histomics_stream-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `histomics_stream-2.3.3/histomics_stream/__init__.py` & `histomics_stream-2.4.0/histomics_stream/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # =========================================================================
 
 """Whole-slide image streamer for machine learning frameworks."""
 
-__version__ = "2.3.3"
+__version__ = "2.4.0"
 
 """
 
 This module supports efficient whole-slide reading and processing for a machine learning
 execution graph.
 
 """
```

### Comparing `histomics_stream-2.3.3/histomics_stream/codecs.py` & `histomics_stream-2.4.0/histomics_stream/codecs.py`

 * *Files identical despite different names*

### Comparing `histomics_stream-2.3.3/histomics_stream/configure.py` & `histomics_stream-2.4.0/histomics_stream/configure.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,15 +146,16 @@
         Sanity check the supplied parameters and store them for later use.
         """
         _TilesByCommon.__init__(self)
         # Check values.
         if not ("version" in study and study["version"] == "version-1"):
             raise ValueError('study["version"] must exist and be equal to "version-1".')
         if not (
-            isinstance(target_magnification, (int, float)) and 0 < target_magnification
+            isinstance(target_magnification, (int, np.integer, float, np.floating))
+            and 0 < target_magnification
         ):
             raise ValueError(
                 f"target_magnification ({target_magnification})"
                 " must be a positive number"
             )
         if not (
             isinstance(magnification_source, str)
@@ -317,15 +318,16 @@
                 and self.target_magnification != returned_magnification
             ):
                 raise ValueError(
                     f"Couldn't find magnification {self.target_magnification}X "
                     "in Zarr storage."
                 )
 
-        slide["level"] = level
+        int_level = int(round(level))
+        slide["level"] = int_level if abs(level - int_level) < 1e-4 else level
         # Note that slide size is defined by the requested magnification, which may not
         # be the same as the magnification for the selected level.  To get the slide
         # size for the magnification that we are using, these values must later be
         # multiplied by returned_magnification / target_magnification.
         slide["slide_height"] = slide_height
         slide["slide_width"] = slide_width
 
@@ -449,51 +451,57 @@
         )
 
         # Check values.
         if not ("version" in study and study["version"] == "version-1"):
             raise ValueError('study["version"] must exist and be equal to "version-1".')
         if not (
             "tile_height" in study
-            and isinstance(study["tile_height"], int)
+            and isinstance(study["tile_height"], (int, np.integer))
             and study["tile_height"] > 0
         ):
             raise ValueError(
                 'study["tile_height"]' " must exist and be a positive integer"
             )
         if not (
             "tile_width" in study
-            and isinstance(study["tile_width"], int)
+            and isinstance(study["tile_width"], (int, np.integer))
             and study["tile_width"] > 0
         ):
             raise ValueError(
                 'study["tile_width"]' " must exist and be a positive integer"
             )
-        if not (isinstance(randomly_select, int) and -1 <= randomly_select):
+        if not (
+            isinstance(randomly_select, (int, np.integer)) and -1 <= randomly_select
+        ):
             raise ValueError(
                 f"randomly_select ({randomly_select})"
                 " must be a non-negative integer or -1."
             )
         if not (
-            isinstance(overlap_height, int) and overlap_height < study["tile_height"]
+            isinstance(overlap_height, (int, np.integer))
+            and overlap_height < study["tile_height"]
         ):
             raise ValueError(
                 f"overlap_height ({overlap_height})"
                 " must be less than"
                 f' tile_height ({study["tile_height"]}).'
             )
-        if not (isinstance(overlap_width, int) and overlap_width < study["tile_width"]):
+        if not (
+            isinstance(overlap_width, (int, np.integer))
+            and overlap_width < study["tile_width"]
+        ):
             raise ValueError(
                 f"overlap_width ({overlap_width})"
                 " must be less than"
                 f' tile_width ({study["tile_width"]}).'
             )
         if mask_filename != "":
             mask_itk = self.check_mask_filename(mask_filename)
         if not (
-            isinstance(mask_threshold, float)
+            isinstance(mask_threshold, (float, np.floating))
             and mask_threshold >= 0.0
             and mask_threshold <= 1.0
         ):
             raise ValueError(
                 f"mask_threshold ({mask_threshold}) must be between 0 and 1 inclusive."
             )
 
@@ -713,29 +721,31 @@
         self._update_dict(study)
 
         # Check values
         if not ("version" in study and study["version"] == "version-1"):
             raise ValueError('study["version"] must exist and be equal to "version-1".')
         if not (
             "tile_height" in study
-            and isinstance(study["tile_height"], int)
+            and isinstance(study["tile_height"], (int, np.integer))
             and study["tile_height"] > 0
         ):
             raise ValueError(
                 'study["tile_height"]' " must exist and be a positive integer"
             )
         if not (
             "tile_width" in study
-            and isinstance(study["tile_width"], int)
+            and isinstance(study["tile_width"], (int, np.integer))
             and study["tile_width"] > 0
         ):
             raise ValueError(
                 'study["tile_width"]' " must exist and be a positive integer"
             )
-        if not (isinstance(randomly_select, int) and -1 <= randomly_select):
+        if not (
+            isinstance(randomly_select, (int, np.integer)) and -1 <= randomly_select
+        ):
             raise ValueError(
                 f"randomly_select ({randomly_select})"
                 " must be a non-negative integer or -1."
             )
         if not isinstance(tiles_dictionary, dict):
             raise ValueError("tiles_dictionary must be dictionary.")
         for tile_corner in tiles_dictionary.values():
@@ -753,15 +763,15 @@
                     key in tile_corner.keys()
                     for tile_corner in tiles_dictionary.values()
                     for key in ("tile_top", "tile_left")
                 ]
             )
             and all(
                 [
-                    isinstance(tile_corner[key], int)
+                    isinstance(tile_corner[key], (int, np.integer))
                     for tile_corner in tiles_dictionary.values()
                     for key in ("tile_top", "tile_left")
                 ]
             )
             and all(
                 [
                     tile_corner[key] >= 0
@@ -828,29 +838,31 @@
         self._update_dict(study)
 
         # Check values.
         if not ("version" in study and study["version"] == "version-1"):
             raise ValueError('study["version"] must exist and be equal to "version-1".')
         if not (
             "tile_height" in study
-            and isinstance(study["tile_height"], int)
+            and isinstance(study["tile_height"], (int, np.integer))
             and study["tile_height"] > 0
         ):
             raise ValueError(
                 'study["tile_height"]' " must exist and be a positive integer"
             )
         if not (
             "tile_width" in study
-            and isinstance(study["tile_width"], int)
+            and isinstance(study["tile_width"], (int, np.integer))
             and study["tile_width"] > 0
         ):
             raise ValueError(
                 'study["tile_width"]' " must exist and be a positive integer"
             )
-        if not (isinstance(randomly_select, int) and 0 <= randomly_select):
+        if not (
+            isinstance(randomly_select, (int, np.integer)) and 0 <= randomly_select
+        ):
             raise ValueError(
                 f"randomly_select ({randomly_select})"
                 " must be a non-negative integer."
             )
 
         # Save values.  To keep garbage collection efficient don't save all of `study`.
         self.tile_height = study["tile_height"]
@@ -900,37 +912,40 @@
             and study_description["version"] == "version-1"
         ):
             raise ValueError(
                 'study_description["version"] must exist and be equal to "version-1".'
             )
         if not (
             "tile_height" in study_description
-            and isinstance(study_description["tile_height"], int)
+            and isinstance(study_description["tile_height"], (int, np.integer))
             and study_description["tile_height"] > 0
         ):
             raise ValueError(
                 'study_description["tile_height"]'
                 " must exist and be a positive integer"
             )
         if not (
             "tile_width" in study_description
-            and isinstance(study_description["tile_width"], int)
+            and isinstance(study_description["tile_width"], (int, np.integer))
             and study_description["tile_width"] > 0
         ):
             raise ValueError(
                 'study_description["tile_width"]'
                 " must exist and be a positive integer"
             )
         for slide in study_description["slides"].values():
             # Update keys of the dictionary from deprecated names
             self._update_dict(slide)
 
             if not (
                 "returned_magnification" in slide
-                and isinstance(slide["returned_magnification"], (int, float))
+                and isinstance(
+                    slide["returned_magnification"],
+                    (int, np.integer, float, np.floating),
+                )
                 and slide["returned_magnification"] > 0
             ):
                 raise ValueError(
                     'slide["returned_magnification"]'
                     " must exist and be a positive number"
                 )
         # Check that other necessary keys are also present!!!
@@ -953,23 +968,23 @@
 
         for slide in study_description["slides"].values():
             # Update keys of the dictionary from deprecated names
             self._update_dict(slide)
 
             if not (
                 "chunk_height" in slide
-                and isinstance(slide["chunk_height"], int)
+                and isinstance(slide["chunk_height"], (int, np.integer))
                 and slide["chunk_height"] > 0
             ):
                 raise ValueError(
                     'slide["chunk_height"]' " must exist and be a positive integer"
                 )
             if not (
                 "chunk_width" in slide
-                and isinstance(slide["chunk_width"], int)
+                and isinstance(slide["chunk_width"], (int, np.integer))
                 and slide["chunk_width"] > 0
             ):
                 raise ValueError(
                     'slide["chunk_width"]' " must exist and be a positive integer"
                 )
             chunk_height = slide["chunk_height"]
             chunk_width = slide["chunk_width"]
```

### Comparing `histomics_stream-2.3.3/histomics_stream/tensorflow.py` & `histomics_stream-2.4.0/histomics_stream/tensorflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,16 @@
         del one_chunk_per_slice
         # print(
         #     f"Build study_dataset from_tensor_slices: end {datetime.datetime.now()}"
         # )
 
         # print(f"study_dataset.element_spec = {study_dataset.element_spec}")
 
-        # Shard the dataset
+        # Shard the dataset before we have broken chunks into tiles so that all a
+        # chunk's tiles stay together.
         if num_workers != 1 or worker_index != 0:
             study_dataset = study_dataset.shard(num_workers, worker_index)
 
         # We have accumulated the chunk datasets into a study_dataset where each element
         # is a chunk.  Read in the chunk pixel data and split it into tiles.
         # print(f"Build study_dataset map: begin {datetime.datetime.now()}")
         study_dataset = study_dataset.map(
```

### Comparing `histomics_stream-2.3.3/pyproject.toml` & `histomics_stream-2.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 maintainers = [{name = "Lee A. Newberg", email = "lee.newberg@kitware.com"}]
 keywords = ["tensorflow", "whole slide image", "stream", "machine learning"]
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 dependencies = [
     "imagecodecs",
     "itk",
     "numcodecs",
-    "numpy<1.24",
+    "numpy",
     "scipy",
-    "tensorflow",
-    "torch",
+    "tensorflow<3.0.0",
+    "torch<2.0.0",
     "zarr",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Source = "https://github.com/DigitalSlideArchive/HistomicsStream"
```

### Comparing `histomics_stream-2.3.3/PKG-INFO` & `histomics_stream-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: histomics_stream
-Version: 2.3.3
+Version: 2.4.0
 Summary: Whole-slide image streamer for machine learning frameworks.
 Keywords: tensorflow,whole slide image,stream,machine learning
 Author-email: "Lee A. Newberg" <lee.newberg@kitware.com>
 Maintainer-email: "Lee A. Newberg" <lee.newberg@kitware.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: imagecodecs
 Requires-Dist: itk
 Requires-Dist: numcodecs
-Requires-Dist: numpy<1.24
+Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: tensorflow
-Requires-Dist: torch
+Requires-Dist: tensorflow<3.0.0
+Requires-Dist: torch<2.0.0
 Requires-Dist: zarr
 Project-URL: Source, https://github.com/DigitalSlideArchive/HistomicsStream
 
 # HistomicsStream
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/InsightSoftwareConsortium/ITK/blob/master/LICENSE) [![PyPI Version](https://img.shields.io/pypi/v/histomics_stream.svg)](https://pypi.python.org/pypi/histomics_stream) [![GitHub repository](https://img.shields.io/badge/Powered%20by-HistomicsStream-blue.svg)](https://github.com/DigitalSlideArchive/HistomicsStream) [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DigitalSlideArchive/HistomicsStream/blob/master/example/tensorflow_stream.ipynb)
```

