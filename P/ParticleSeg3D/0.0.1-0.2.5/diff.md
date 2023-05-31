# Comparing `tmp/ParticleSeg3D-0.0.1.tar.gz` & `tmp/ParticleSeg3D-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParticleSeg3D-0.0.1.tar", last modified: Wed May 31 12:24:45 2023, max compression
+gzip compressed data, was "ParticleSeg3D-0.2.5.tar", last modified: Wed May 31 13:03:46 2023, max compression
```

## Comparing `ParticleSeg3D-0.0.1.tar` & `ParticleSeg3D-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/ParticleSeg3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-05-31 12:24:45.000000 ParticleSeg3D-0.0.1/ParticleSeg3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-31 12:24:45.000000 ParticleSeg3D-0.0.1/ParticleSeg3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:24:45.000000 ParticleSeg3D-0.0.1/ParticleSeg3D.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-31 12:24:45.000000 ParticleSeg3D-0.0.1/ParticleSeg3D.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 12:24:45.000000 ParticleSeg3D-0.0.1/ParticleSeg3D.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 12:24:45.000000 ParticleSeg3D-0.0.1/ParticleSeg3D.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/particleseg3d/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/particleseg3d/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/particleseg3d/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/conversion/nifti2tiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/conversion/nifti2zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/conversion/tiff2nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/conversion/tiff2zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/conversion/zarr2tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/particleseg3d/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/inference/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/inference/border_core2instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    25363 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/inference/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/inference/model_nnunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23580 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/inference/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/particleseg3d/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/train/instance2border_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/train/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/particleseg3d/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28913 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/particleseg3d/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-31 12:24:45.978242 ParticleSeg3D-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:24:27.000000 ParticleSeg3D-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:46.778621 ParticleSeg3D-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-05-31 13:03:46.778621 ParticleSeg3D-0.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:46.774621 ParticleSeg3D-0.2.5/ParticleSeg3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-05-31 13:03:46.000000 ParticleSeg3D-0.2.5/ParticleSeg3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-31 13:03:46.000000 ParticleSeg3D-0.2.5/ParticleSeg3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:03:46.000000 ParticleSeg3D-0.2.5/ParticleSeg3D.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-31 13:03:46.000000 ParticleSeg3D-0.2.5/ParticleSeg3D.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 13:03:46.000000 ParticleSeg3D-0.2.5/ParticleSeg3D.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 13:03:46.000000 ParticleSeg3D-0.2.5/ParticleSeg3D.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:46.774621 ParticleSeg3D-0.2.5/particleseg3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:46.774621 ParticleSeg3D-0.2.5/particleseg3d/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:46.774621 ParticleSeg3D-0.2.5/particleseg3d/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/conversion/nifti2tiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/conversion/nifti2zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/conversion/tiff2nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/conversion/tiff2zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/conversion/zarr2tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:46.778621 ParticleSeg3D-0.2.5/particleseg3d/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/inference/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/inference/border_core2instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25363 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/inference/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/inference/model_nnunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23580 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/inference/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:46.778621 ParticleSeg3D-0.2.5/particleseg3d/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/train/instance2border_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/train/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:46.778621 ParticleSeg3D-0.2.5/particleseg3d/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28913 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/particleseg3d/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-31 13:03:46.778621 ParticleSeg3D-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:03:18.000000 ParticleSeg3D-0.2.5/setup.py
```

### Comparing `ParticleSeg3D-0.0.1/LICENSE` & `ParticleSeg3D-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/PKG-INFO` & `ParticleSeg3D-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticleSeg3D
-Version: 0.0.1
+Version: 0.2.5
 Summary: Scalable, out-of-the box segmentation of individual particles from mineral samples acquired with micro CT
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ParticleSeg3D-0.0.1/ParticleSeg3D.egg-info/PKG-INFO` & `ParticleSeg3D-0.2.5/ParticleSeg3D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticleSeg3D
-Version: 0.0.1
+Version: 0.2.5
 Summary: Scalable, out-of-the box segmentation of individual particles from mineral samples acquired with micro CT
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ParticleSeg3D-0.0.1/ParticleSeg3D.egg-info/SOURCES.txt` & `ParticleSeg3D-0.2.5/ParticleSeg3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/README.md` & `ParticleSeg3D-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/conversion/nifti2tiff.py` & `ParticleSeg3D-0.2.5/particleseg3d/conversion/nifti2tiff.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/conversion/nifti2zarr.py` & `ParticleSeg3D-0.2.5/particleseg3d/conversion/nifti2zarr.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/conversion/tiff2nifti.py` & `ParticleSeg3D-0.2.5/particleseg3d/conversion/tiff2nifti.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/conversion/tiff2zarr.py` & `ParticleSeg3D-0.2.5/particleseg3d/conversion/tiff2zarr.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/conversion/zarr2tiff.py` & `ParticleSeg3D-0.2.5/particleseg3d/conversion/zarr2tiff.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/inference/aggregator.py` & `ParticleSeg3D-0.2.5/particleseg3d/inference/aggregator.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/inference/border_core2instance.py` & `ParticleSeg3D-0.2.5/particleseg3d/inference/border_core2instance.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/inference/inference.py` & `ParticleSeg3D-0.2.5/particleseg3d/inference/inference.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/inference/model_nnunet.py` & `ParticleSeg3D-0.2.5/particleseg3d/inference/model_nnunet.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/inference/sampler.py` & `ParticleSeg3D-0.2.5/particleseg3d/inference/sampler.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/train/instance2border_core.py` & `ParticleSeg3D-0.2.5/particleseg3d/train/instance2border_core.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/train/preprocess.py` & `ParticleSeg3D-0.2.5/particleseg3d/train/preprocess.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/particleseg3d/utils/utils.py` & `ParticleSeg3D-0.2.5/particleseg3d/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/pyproject.toml` & `ParticleSeg3D-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.0.1/setup.cfg` & `ParticleSeg3D-0.2.5/setup.cfg`

 * *Files identical despite different names*

