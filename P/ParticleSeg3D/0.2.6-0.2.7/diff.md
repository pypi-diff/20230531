# Comparing `tmp/ParticleSeg3D-0.2.6.tar.gz` & `tmp/ParticleSeg3D-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParticleSeg3D-0.2.6.tar", last modified: Wed May 31 15:15:08 2023, max compression
+gzip compressed data, was "ParticleSeg3D-0.2.7.tar", last modified: Wed May 31 15:16:50 2023, max compression
```

## Comparing `ParticleSeg3D-0.2.6.tar` & `ParticleSeg3D-0.2.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:15:08.840838 ParticleSeg3D-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-05-31 15:15:08.840838 ParticleSeg3D-0.2.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:15:08.836838 ParticleSeg3D-0.2.6/ParticleSeg3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-05-31 15:15:08.000000 ParticleSeg3D-0.2.6/ParticleSeg3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-31 15:15:08.000000 ParticleSeg3D-0.2.6/ParticleSeg3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:15:08.000000 ParticleSeg3D-0.2.6/ParticleSeg3D.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-31 15:15:08.000000 ParticleSeg3D-0.2.6/ParticleSeg3D.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 15:15:08.000000 ParticleSeg3D-0.2.6/ParticleSeg3D.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 15:15:08.000000 ParticleSeg3D-0.2.6/ParticleSeg3D.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:15:08.836838 ParticleSeg3D-0.2.6/particleseg3d/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:15:08.836838 ParticleSeg3D-0.2.6/particleseg3d/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:15:08.836838 ParticleSeg3D-0.2.6/particleseg3d/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/conversion/nifti2tiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/conversion/nifti2zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/conversion/tiff2nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/conversion/tiff2zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/conversion/zarr2tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:15:08.840838 ParticleSeg3D-0.2.6/particleseg3d/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/inference/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/inference/border_core2instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    25363 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/inference/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/inference/model_nnunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23580 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/inference/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:15:08.840838 ParticleSeg3D-0.2.6/particleseg3d/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/train/instance2border_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/train/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:15:08.840838 ParticleSeg3D-0.2.6/particleseg3d/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28913 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/particleseg3d/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-31 15:15:08.840838 ParticleSeg3D-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:14:48.000000 ParticleSeg3D-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-05-31 15:16:50.344584 ParticleSeg3D-0.2.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 15:16:50.000000 ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/nifti2tiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/nifti2zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/tiff2nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/tiff2zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/conversion/zarr2tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/border_core2instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25363 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/model_nnunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23580 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/inference/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/train/instance2border_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/train/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:50.340584 ParticleSeg3D-0.2.7/particleseg3d/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28913 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/particleseg3d/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-31 15:16:50.344584 ParticleSeg3D-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:16:33.000000 ParticleSeg3D-0.2.7/setup.py
```

### Comparing `ParticleSeg3D-0.2.6/LICENSE` & `ParticleSeg3D-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/PKG-INFO` & `ParticleSeg3D-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticleSeg3D
-Version: 0.2.6
+Version: 0.2.7
 Summary: Scalable, out-of-the box segmentation of individual particles from mineral samples acquired with micro CT
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -40,15 +40,15 @@
 - Application of nnU-Net framework for reliable and scalable image processing
 - Border-core representation for instance segmentation
 - Particle size normalization to account for different mineral types
 - Trained on a diverse set of particles from various materials and minerals
 - Can be applied to a wide variety of particle types, without additional manual annotations or retraining
 
 ## Installation
-You can install `ParticleSeg3D` via [pip]:
+You can install `ParticleSeg3D` via [pip](https://pypi.org/project/ParticleSeg3D/):
 
     pip install ParticleSeg3D
 
 You should now have the ParticleSeg3D package installed in your Python environment, and you'll be able to use all ParticleSeg3D commands from anywhere on your system.
 
 If you intend to train ParticleSeg3D on new data, you will need to additionally install a modified version of the nnU-Net V1:
 ```cmd
```

### Comparing `ParticleSeg3D-0.2.6/ParticleSeg3D.egg-info/PKG-INFO` & `ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticleSeg3D
-Version: 0.2.6
+Version: 0.2.7
 Summary: Scalable, out-of-the box segmentation of individual particles from mineral samples acquired with micro CT
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -40,15 +40,15 @@
 - Application of nnU-Net framework for reliable and scalable image processing
 - Border-core representation for instance segmentation
 - Particle size normalization to account for different mineral types
 - Trained on a diverse set of particles from various materials and minerals
 - Can be applied to a wide variety of particle types, without additional manual annotations or retraining
 
 ## Installation
-You can install `ParticleSeg3D` via [pip]:
+You can install `ParticleSeg3D` via [pip](https://pypi.org/project/ParticleSeg3D/):
 
     pip install ParticleSeg3D
 
 You should now have the ParticleSeg3D package installed in your Python environment, and you'll be able to use all ParticleSeg3D commands from anywhere on your system.
 
 If you intend to train ParticleSeg3D on new data, you will need to additionally install a modified version of the nnU-Net V1:
 ```cmd
```

### Comparing `ParticleSeg3D-0.2.6/ParticleSeg3D.egg-info/SOURCES.txt` & `ParticleSeg3D-0.2.7/ParticleSeg3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/README.md` & `ParticleSeg3D-0.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - Application of nnU-Net framework for reliable and scalable image processing
 - Border-core representation for instance segmentation
 - Particle size normalization to account for different mineral types
 - Trained on a diverse set of particles from various materials and minerals
 - Can be applied to a wide variety of particle types, without additional manual annotations or retraining
 
 ## Installation
-You can install `ParticleSeg3D` via [pip]:
+You can install `ParticleSeg3D` via [pip](https://pypi.org/project/ParticleSeg3D/):
 
     pip install ParticleSeg3D
 
 You should now have the ParticleSeg3D package installed in your Python environment, and you'll be able to use all ParticleSeg3D commands from anywhere on your system.
 
 If you intend to train ParticleSeg3D on new data, you will need to additionally install a modified version of the nnU-Net V1:
 ```cmd
```

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/conversion/nifti2tiff.py` & `ParticleSeg3D-0.2.7/particleseg3d/conversion/nifti2tiff.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/conversion/nifti2zarr.py` & `ParticleSeg3D-0.2.7/particleseg3d/conversion/nifti2zarr.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/conversion/tiff2nifti.py` & `ParticleSeg3D-0.2.7/particleseg3d/conversion/tiff2nifti.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/conversion/tiff2zarr.py` & `ParticleSeg3D-0.2.7/particleseg3d/conversion/tiff2zarr.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/conversion/zarr2tiff.py` & `ParticleSeg3D-0.2.7/particleseg3d/conversion/zarr2tiff.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/inference/aggregator.py` & `ParticleSeg3D-0.2.7/particleseg3d/inference/aggregator.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/inference/border_core2instance.py` & `ParticleSeg3D-0.2.7/particleseg3d/inference/border_core2instance.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/inference/inference.py` & `ParticleSeg3D-0.2.7/particleseg3d/inference/inference.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/inference/model_nnunet.py` & `ParticleSeg3D-0.2.7/particleseg3d/inference/model_nnunet.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/inference/sampler.py` & `ParticleSeg3D-0.2.7/particleseg3d/inference/sampler.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/train/instance2border_core.py` & `ParticleSeg3D-0.2.7/particleseg3d/train/instance2border_core.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/train/preprocess.py` & `ParticleSeg3D-0.2.7/particleseg3d/train/preprocess.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/particleseg3d/utils/utils.py` & `ParticleSeg3D-0.2.7/particleseg3d/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/pyproject.toml` & `ParticleSeg3D-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ParticleSeg3D-0.2.6/setup.cfg` & `ParticleSeg3D-0.2.7/setup.cfg`

 * *Files identical despite different names*

