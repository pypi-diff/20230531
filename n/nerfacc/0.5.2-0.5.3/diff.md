# Comparing `tmp/nerfacc-0.5.2.tar.gz` & `tmp/nerfacc-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nerfacc/nerfacc/dist/.tmp-0kkb42ub/nerfacc-0.5.2.tar", last modified: Mon Apr 24 08:00:56 2023, max compression
+gzip compressed data, was "/home/runner/work/nerfacc/nerfacc/dist/.tmp-w9c08qwb/nerfacc-0.5.3.tar", last modified: Wed May 31 18:47:56 2023, max compression
```

## Comparing `nerfacc-0.5.2.tar` & `nerfacc-0.5.3.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-24 08:00:36.000000 nerfacc-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 08:00:36.000000 nerfacc-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 08:00:56.000000 nerfacc-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-24 08:00:48.000000 nerfacc-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cameras2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/camera.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/grid.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/data_spec.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/data_spec_packed.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_camera.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_contraction.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_grid.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    38908 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_math.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_scan.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/nerfacc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/pdf.cu
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/scan.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/data_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/estimators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/estimators/occ_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/estimators/prop_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/volrend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 08:00:56.000000 nerfacc-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-24 08:00:37.000000 nerfacc-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:47:56.000000 nerfacc-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 18:47:37.000000 nerfacc-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 18:47:37.000000 nerfacc-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 18:47:56.000000 nerfacc-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-05-31 18:47:49.000000 nerfacc-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cameras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/camera.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/grid.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/include/data_spec.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/include/data_spec_packed.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_camera.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_contraction.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_grid.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    38908 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_math.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_scan.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/nerfacc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/pdf.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/cuda/csrc/scan.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/data_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/estimators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/estimators/occ_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/estimators/prop_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24054 2023-05-31 18:47:37.000000 nerfacc-0.5.3/nerfacc/volrend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 18:47:56.000000 nerfacc-0.5.3/nerfacc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 18:47:56.000000 nerfacc-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-31 18:47:37.000000 nerfacc-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:47:56.000000 nerfacc-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-31 18:47:37.000000 nerfacc-0.5.3/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-31 18:47:37.000000 nerfacc-0.5.3/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-31 18:47:37.000000 nerfacc-0.5.3/tests/test_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-31 18:47:37.000000 nerfacc-0.5.3/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-05-31 18:47:37.000000 nerfacc-0.5.3/tests/test_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-31 18:47:37.000000 nerfacc-0.5.3/tests/test_scan.py
```

### Comparing `nerfacc-0.5.2/LICENSE` & `nerfacc-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/README.md` & `nerfacc-0.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 We also provide pre-built wheels covering major combinations of Pytorch + CUDA supported by [official Pytorch](https://pytorch.org/get-started/previous-versions/).
 
 ```
 # e.g., torch 1.13.0 + cu117
 pip install nerfacc -f https://nerfacc-bucket.s3.us-west-2.amazonaws.com/whl/torch-1.13.0_cu117.html
 ```
 
-| Windows & Linux | `cu102` | `cu113` | `cu116` | `cu117` |
-|-----------------|---------|---------|---------|---------|
-| torch 1.10.0    | ✅      | ✅      |         |         |
-| torch 1.11.0    | ✅*     | ✅      |         |         |
-| torch 1.12.0    | ✅*     | ✅      | ✅      |         |
-| torch 1.13.0    |         |         | ✅      | ✅      |
+| Windows & Linux | `cu113` | `cu115` | `cu116` | `cu117` | `cu118` |
+|-----------------|---------|---------|---------|---------|---------|
+| torch 1.11.0    | ✅      | ✅      |         |         |         |
+| torch 1.12.0    | ✅      |         | ✅      |         |         |
+| torch 1.13.0    |         |         | ✅      | ✅      |         |
+| torch 2.0.0     |         |         |         | ✅      | ✅      |
 
-\* Pytorch does not support Windows pre-built wheels for those combinations thus we do not support as well.
+For previous version of nerfacc, please check [here](https://nerfacc-bucket.s3.us-west-2.amazonaws.com/whl/index.html) on the supported pre-built wheels.
 
 ## Usage
 
 The idea of NerfAcc is to perform efficient volumetric sampling with a computationally cheap estimator to discover surfaces.
 So NerfAcc can work with any user-defined radiance field. To plug the NerfAcc rendering pipeline into your code and enjoy 
 the acceleration, you only need to define two functions with your radience field.
 
@@ -191,31 +191,37 @@
 ```bash
 cd benchmarks/barf/
 # (set up the environment for that repo)
 bash script.sh nerfsyn-nerfacc-occgrid 0
 ```
 
 ### 3rd-Party Usages:
+
+#### Awesome Codebases.
 - [nerfstudio](https://github.com/nerfstudio-project/nerfstudio): A collaboration friendly studio for NeRFs.
-- [sdfstudio](https://autonomousvision.github.io/sdfstudio/): A unified framework for surface reconstruction..
+- [sdfstudio](https://autonomousvision.github.io/sdfstudio/): A unified framework for surface reconstruction.
+- [threestudio](https://github.com/threestudio-project/threestudio): A unified framework for 3D content creation.
 - [instant-nsr-pl](https://github.com/bennyguo/instant-nsr-pl): NeuS in 10 minutes.
 - [modelscope](https://github.com/modelscope/modelscope/blob/master/modelscope/models/cv/nerf_recon_acc/network/nerf.py): A collection of deep-learning algorithms.
-- [Representing Volumetric Videos as Dynamic MLP Maps, CVPR 2023](https://github.com/zju3dv/mlp_maps)
 
+#### Awesome Papers.
+- [Representing Volumetric Videos as Dynamic MLP Maps, CVPR 2023](https://github.com/zju3dv/mlp_maps)
+- [NeRSemble: Multi-view Radiance Field Reconstruction of Human Heads, ArXiv 2023](https://tobias-kirschstein.github.io/nersemble/)
+- [HumanRF: High-Fidelity Neural Radiance Fields for Humans in Motion, ArXiv 2023](https://synthesiaresearch.github.io/humanrf/)
 
 ## Common Installation Issues
 
 <details>
     <summary>ImportError: .../csrc.so: undefined symbol</summary>
     If you are installing a pre-built wheel, make sure the Pytorch and CUDA version matchs with the nerfacc version (nerfacc.__version__).
 </details>
 
 ## Citation
 
 ```bibtex
 @article{li2023nerfacc,
   title={NerfAcc: Efficient Sampling Accelerates NeRFs.},
   author={Li, Ruilong and Gao, Hang and Tancik, Matthew and Kanazawa, Angjoo},
-  journal={To Be Updated},
+  journal={arXiv preprint arXiv:2305.04966},
   year={2023}
 }
 ```
```

### Comparing `nerfacc-0.5.2/nerfacc/__init__.py` & `nerfacc-0.5.3/nerfacc/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/cameras.py` & `nerfacc-0.5.3/nerfacc/cameras.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/cuda/__init__.py` & `nerfacc-0.5.3/nerfacc/cuda/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,27 +11,22 @@
         from ._backend import _C
 
         return getattr(_C, name)(*args, **kwargs)
 
     return call_cuda
 
 
-is_cub_available = _make_lazy_cuda_func("is_cub_available")
-
 # data specs
-MultiScaleGridSpec = _make_lazy_cuda_func("MultiScaleGridSpec")
-RaysSpec = _make_lazy_cuda_func("RaysSpec")
 RaySegmentsSpec = _make_lazy_cuda_func("RaySegmentsSpec")
 
 # grid
 ray_aabb_intersect = _make_lazy_cuda_func("ray_aabb_intersect")
 traverse_grids = _make_lazy_cuda_func("traverse_grids")
 
 # scan
-exclusive_sum_by_key = _make_lazy_cuda_func("exclusive_sum_by_key")
 inclusive_sum = _make_lazy_cuda_func("inclusive_sum")
 exclusive_sum = _make_lazy_cuda_func("exclusive_sum")
 inclusive_prod_forward = _make_lazy_cuda_func("inclusive_prod_forward")
 inclusive_prod_backward = _make_lazy_cuda_func("inclusive_prod_backward")
 exclusive_prod_forward = _make_lazy_cuda_func("exclusive_prod_forward")
 exclusive_prod_backward = _make_lazy_cuda_func("exclusive_prod_backward")
```

### Comparing `nerfacc-0.5.2/nerfacc/cuda/_backend.py` & `nerfacc-0.5.3/nerfacc/cuda/_backend.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/camera.cu` & `nerfacc-0.5.3/nerfacc/cuda/csrc/camera.cu`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/grid.cu` & `nerfacc-0.5.3/nerfacc/cuda/csrc/grid.cu`

 * *Files 18% similar despite different names*

```diff
@@ -23,43 +23,86 @@
 inline __device__ float _calc_dt(
     const float t, const float cone_angle,
     const float dt_min, const float dt_max)
 {
     return clamp(t * cone_angle, dt_min, dt_max);
 }
 
+/* Ray traversal within multiple voxel grids. 
+
+About rays:
+    Each ray is defined by its origin (rays_o) and unit direction (rays_d). We also allows
+    a optional boolen ray mask (rays_mask) to indicate whether we want to skip some rays. 
+
+About voxel grids:
+    We support ray traversal through one or more voxel grids (n_grids). Each grid is defined
+    by an axis-aligned AABB (aabbs), and a binary occupancy grid (binaries) with resolution of
+    {resx, resy, resz}. Currently, we assume all grids have the same resolution. Note the ordering
+    of the grids is important when there are overlapping grids, because we assume the grid in front
+    has higher priority when examing occupancy status (e.g., the first grid's occupancy status
+    will overwrite the second grid's occupancy status if they overlap).
+
+About ray grid intersections:
+    We require the ray grid intersections to be precomputed and sorted. Specifically, if hit, each 
+    ray-grid pair has two intersections, one for entering the grid and one for leaving the grid. 
+    For multiple grids, there are in total 2 * n_grids intersections for each ray. The intersections
+    are sorted by the distance to the ray origin (t_sorted). We take a boolen array (hits) to indicate 
+    whether each ray-grid pair is hit. We also need a int64 array (t_indices) to indicate the grid id
+    (0-index) for each intersection.
+
+About ray traversal:
+    The ray is traversed through the grids in the order of the sorted intersections. We allows pre-ray
+    near and far planes (near_planes, far_planes) to be specified. Early termination can be controlled by
+    setting the maximum traverse steps via traverse_steps_limit. We also allow an optional step size
+    (step_size) to be specified. If step_size <= 0.0, we will record the steps of the ray pass through
+    each voxel cell. Otherwise, we will use the step_size to march through the grids. When step_size > 0.0,
+    we also allow a cone angle (cone_angle) to be provides, to linearly increase the step size as the ray
+    goes further away from the origin (see _calc_dt()). cone_angle should be always >= 0.0, and 0.0 
+    means uniform marching with step_size.
+
+About outputs:
+    The traversal intervals and samples are stored in `intervals` and `samples` respectively. Additionally,
+    we also return where the traversal actually terminates (terminate_planes). This is useful when 
+    traverse_steps_limit is set (traverse_steps_limit > 0) as the ray may not reach the far plane or the
+    boundary of the grids.
+*/
 __global__ void traverse_grids_kernel(
     // rays
     int32_t n_rays,
     float *rays_o,  // [n_rays, 3]
     float *rays_d,  // [n_rays, 3]
+    bool *rays_mask, // [n_rays]
     // grids
     int32_t n_grids,
     int3 resolution,
     bool *binaries, // [n_grids, resx, resy, resz]
     float *aabbs,   // [n_grids, 6]
     // sorted intersections
     bool *hits,         // [n_rays, n_grids]
     float *t_sorted,    // [n_rays, n_grids * 2]
     int64_t *t_indices, // [n_rays, n_grids * 2]
     // options
-    float *near_planes,
-    float *far_planes,
+    float *near_planes,  // [n_rays]
+    float *far_planes,   // [n_rays]
     float step_size,
     float cone_angle,
+    int32_t traverse_steps_limit,
     // outputs
     bool first_pass,
     PackedRaySegmentsSpec intervals,
-    PackedRaySegmentsSpec samples)
+    PackedRaySegmentsSpec samples,
+    float *terminate_planes)
 {
     float eps = 1e-6f;
 
     // parallelize over rays
     for (int32_t tid = blockIdx.x * blockDim.x + threadIdx.x; tid < n_rays; tid += blockDim.x * gridDim.x)
     {
+        if (rays_mask != nullptr && !rays_mask[tid]) continue;
+
         // skip rays that are empty.
         if (intervals.chunk_cnts != nullptr)
             if (!first_pass && intervals.chunk_cnts[tid] == 0) continue;
         if (samples.chunk_cnts != nullptr)
             if (!first_pass && samples.chunk_cnts[tid] == 0) continue;
 
         int64_t chunk_start, chunk_start_bin;
@@ -134,15 +177,15 @@
                 delta, tdist, step_index, current_index, final_index);
             // printf(
             //     "[traverse init], delta=(%f, %f, %f), step_index=(%d, %d, %d)\n",
             //     delta.x, delta.y, delta.z, step_index.x, step_index.y, step_index.z
             // );
 
             const int3 overflow_index = final_index + step_index;
-            while (true) {
+            while (traverse_steps_limit <= 0 || n_samples < traverse_steps_limit) {
                 float t_traverse = min(tdist.x, min(tdist.y, tdist.z));
                 t_traverse = fminf(t_traverse, this_tmax);
                 int64_t cell_id = (
                     current_index.x * resolution.y * resolution.z
                     + current_index.y * resolution.z
                     + current_index.z
                     + level * resolution.x * resolution.y * resolution.z
@@ -158,15 +201,15 @@
                             if (t_last + dt * 0.5f >= t_traverse) break;
                             t_last += dt;
                         }
                     }
                     continuous = false;
                 } else {
                     // this cell is not empty, so we need to traverse it.
-                    while (true) {
+                    while (traverse_steps_limit <= 0 || n_samples < traverse_steps_limit) {
                         float t_next;
                         if (step_size <= 0.0f) {
                             t_next = t_traverse;
                         } else {  // march until t_mid is right after t_traverse.
                             float dt = _calc_dt(t_last, cone_angle, step_size, 1e10f);
                             if (t_last + dt * 0.5f >= t_traverse) break;
                             t_next = t_last + dt;
@@ -203,18 +246,19 @@
 
                         // writeout the sample.
                         if (samples.chunk_cnts != nullptr) {
                             if (!first_pass) {
                                 int64_t idx = chunk_start_bin + n_samples;
                                 samples.vals[idx] = (t_next + t_last) * 0.5f;
                                 samples.ray_indices[idx] = tid;
+                                samples.is_valid[idx] = true;
                             }
-                            n_samples++;
                         }
 
+                        n_samples++;
                         continuous = true;
                         t_last = t_next;
                         if (t_next >= t_traverse) break;
                     }
                 }
 
                 // printf(
@@ -223,25 +267,24 @@
                 // );
 
                 if (!single_traversal(tdist, current_index, overflow_index, step_index, delta)) {
                     break;
                 }
             }
         }
-        
-        if (first_pass) {
-            if (intervals.chunk_cnts != nullptr)
-                intervals.chunk_cnts[tid] = n_intervals;
-            if (samples.chunk_cnts != nullptr)
-                samples.chunk_cnts[tid] = n_samples;
-        }
+        if (terminate_planes != nullptr)
+            terminate_planes[tid] = t_last;
+
+        if (intervals.chunk_cnts != nullptr)
+            intervals.chunk_cnts[tid] = n_intervals;
+        if (samples.chunk_cnts != nullptr)
+            samples.chunk_cnts[tid] = n_samples;
     }
 }
 
-
 __global__ void ray_aabb_intersect_kernel(
     const int32_t n_rays, float *rays_o, float *rays_d, float near, float far,
     const int32_t n_aabbs, float *aabbs,
     // outputs
     const float miss_value,
     float *t_mins, float *t_maxs, bool *hits)
 {
@@ -270,119 +313,168 @@
 }
 
 
 }  // namespace device
 }  // namespace
 
 
-std::vector<RaySegmentsSpec> traverse_grids(
+std::tuple<RaySegmentsSpec, RaySegmentsSpec, torch::Tensor> traverse_grids(
     // rays
     const torch::Tensor rays_o, // [n_rays, 3]
     const torch::Tensor rays_d, // [n_rays, 3]
+    const torch::Tensor rays_mask,   // [n_rays]
     // grids
     const torch::Tensor binaries,  // [n_grids, resx, resy, resz]
     const torch::Tensor aabbs,     // [n_grids, 6]
     // intersections
-    const torch::Tensor t_mins,  // [n_rays, n_grids]
-    const torch::Tensor t_maxs,  // [n_rays, n_grids]
+    const torch::Tensor t_sorted,  // [n_rays, n_grids]
+    const torch::Tensor t_indices,  // [n_rays, n_grids]
     const torch::Tensor hits,    // [n_rays, n_grids]
     // options
     const torch::Tensor near_planes,
     const torch::Tensor far_planes,
     const float step_size,
     const float cone_angle,
     const bool compute_intervals,
-    const bool compute_samples) 
+    const bool compute_samples,
+    const bool compute_terminate_planes,
+    const int32_t traverse_steps_limit, // <= 0 means no limit
+    const bool over_allocate) // over allocate the memory for intervals and samples
 {
     DEVICE_GUARD(rays_o);
+    if (over_allocate) {
+        TORCH_CHECK(traverse_steps_limit > 0, "traverse_steps_limit must be > 0 when over_allocate is true");
+    }
 
     int32_t n_rays = rays_o.size(0);
     int32_t n_grids = binaries.size(0);
     int3 resolution = make_int3(binaries.size(1), binaries.size(2), binaries.size(3));
 
     at::cuda::CUDAStream stream = at::cuda::getCurrentCUDAStream();
     int32_t max_threads = 512; 
     int32_t max_blocks = 65535;
     dim3 threads = dim3(min(max_threads, n_rays));
     dim3 blocks = dim3(min(max_blocks, ceil_div<int32_t>(n_rays, threads.x)));
 
-    // Sort the intersections. [n_rays, n_grids * 2]
-    torch::Tensor t_sorted, t_indices;
-    if (n_grids > 1) {
-        std::tie(t_sorted, t_indices) = torch::sort(torch::cat({t_mins, t_maxs}, -1), -1);
-    }
-    else {
-        t_sorted = torch::cat({t_mins, t_maxs}, -1);
-        t_indices = torch::arange(
-            0, n_grids * 2, t_mins.options().dtype(torch::kLong)
-        ).expand({n_rays, n_grids * 2}).contiguous();
-    }
-    
     // outputs
     RaySegmentsSpec intervals, samples;
+    torch::Tensor terminate_planes;
+    if (compute_terminate_planes) 
+        terminate_planes = torch::empty({n_rays}, rays_o.options());
+
+    if (over_allocate) {
+        // over allocate the memory so that we can traverse the grids in a single pass.
+        if (compute_intervals) {
+            intervals.chunk_cnts = torch::full({n_rays}, traverse_steps_limit * 2, rays_o.options().dtype(torch::kLong)) * rays_mask;
+            intervals.memalloc_data_from_chunk(true, true);
+        }
+        if (compute_samples) {
+            samples.chunk_cnts = torch::full({n_rays}, traverse_steps_limit, rays_o.options().dtype(torch::kLong)) * rays_mask;
+            samples.memalloc_data_from_chunk(false, true, true);
+        }
 
-    // first pass to count the number of segments along each ray.
-    if (compute_intervals)
-        intervals.memalloc_cnts(n_rays, rays_o.options(), false);
-    if (compute_samples)
-        samples.memalloc_cnts(n_rays, rays_o.options(), false);
-    device::traverse_grids_kernel<<<blocks, threads, 0, stream>>>(
-        // rays
-        n_rays,
-        rays_o.data_ptr<float>(),  // [n_rays, 3]
-        rays_d.data_ptr<float>(),  // [n_rays, 3]
-        // grids
-        n_grids,
-        resolution,
-        binaries.data_ptr<bool>(), // [n_grids, resx, resy, resz]
-        aabbs.data_ptr<float>(),   // [n_grids, 6]
-        // sorted intersections
-        hits.data_ptr<bool>(),         // [n_rays, n_grids]
-        t_sorted.data_ptr<float>(),    // [n_rays, n_grids * 2]
-        t_indices.data_ptr<int64_t>(), // [n_rays, n_grids * 2]
-        // options
-        near_planes.data_ptr<float>(), // [n_rays]
-        far_planes.data_ptr<float>(),  // [n_rays]
-        step_size,
-        cone_angle,
-        // outputs
-        true,
-        device::PackedRaySegmentsSpec(intervals),
-        device::PackedRaySegmentsSpec(samples));
+        device::traverse_grids_kernel<<<blocks, threads, 0, stream>>>(
+            // rays
+            n_rays,
+            rays_o.data_ptr<float>(),  // [n_rays, 3]
+            rays_d.data_ptr<float>(),  // [n_rays, 3]
+            rays_mask.data_ptr<bool>(),  // [n_rays]
+            // grids
+            n_grids,
+            resolution,
+            binaries.data_ptr<bool>(), // [n_grids, resx, resy, resz]
+            aabbs.data_ptr<float>(),   // [n_grids, 6]
+            // sorted intersections
+            hits.data_ptr<bool>(),         // [n_rays, n_grids]
+            t_sorted.data_ptr<float>(),    // [n_rays, n_grids * 2]
+            t_indices.data_ptr<int64_t>(), // [n_rays, n_grids * 2]
+            // options
+            near_planes.data_ptr<float>(), // [n_rays]
+            far_planes.data_ptr<float>(),  // [n_rays]
+            step_size,
+            cone_angle,
+            traverse_steps_limit,
+            // outputs
+            false,
+            device::PackedRaySegmentsSpec(intervals),
+            device::PackedRaySegmentsSpec(samples),
+            compute_terminate_planes ? terminate_planes.data_ptr<float>() : nullptr);
+        
+        // update the chunk starts with the actual chunk_cnts from traversal.
+        intervals.compute_chunk_start();
+        samples.compute_chunk_start();
+    } else {
+        // To allocate the accurate memory we need to traverse the grids twice.
+        // The first pass is to count the number of segments along each ray.
+        // The second pass is to fill the segments.
+        if (compute_intervals)
+            intervals.chunk_cnts = torch::empty({n_rays}, rays_o.options().dtype(torch::kLong));
+        if (compute_samples)
+            samples.chunk_cnts = torch::empty({n_rays}, rays_o.options().dtype(torch::kLong));
+        device::traverse_grids_kernel<<<blocks, threads, 0, stream>>>(
+            // rays
+            n_rays,
+            rays_o.data_ptr<float>(),  // [n_rays, 3]
+            rays_d.data_ptr<float>(),  // [n_rays, 3]
+            nullptr,  /* rays_mask */
+            // grids
+            n_grids,
+            resolution,
+            binaries.data_ptr<bool>(), // [n_grids, resx, resy, resz]
+            aabbs.data_ptr<float>(),   // [n_grids, 6]
+            // sorted intersections
+            hits.data_ptr<bool>(),         // [n_rays, n_grids]
+            t_sorted.data_ptr<float>(),    // [n_rays, n_grids * 2]
+            t_indices.data_ptr<int64_t>(), // [n_rays, n_grids * 2]
+            // options
+            near_planes.data_ptr<float>(), // [n_rays]
+            far_planes.data_ptr<float>(),  // [n_rays]
+            step_size,
+            cone_angle,
+            traverse_steps_limit,
+            // outputs
+            true,
+            device::PackedRaySegmentsSpec(intervals),
+            device::PackedRaySegmentsSpec(samples),
+            nullptr);  /* terminate_planes */
+        
+        // second pass to record the segments.
+        if (compute_intervals)
+            intervals.memalloc_data_from_chunk(true, true);
+        if (compute_samples)
+            samples.memalloc_data_from_chunk(false, false, true);
+        device::traverse_grids_kernel<<<blocks, threads, 0, stream>>>(
+            // rays
+            n_rays,
+            rays_o.data_ptr<float>(),  // [n_rays, 3]
+            rays_d.data_ptr<float>(),  // [n_rays, 3]
+            nullptr,  /* rays_mask */
+            // grids
+            n_grids,
+            resolution,
+            binaries.data_ptr<bool>(), // [n_grids, resx, resy, resz]
+            aabbs.data_ptr<float>(),   // [n_grids, 6]
+            // sorted intersections
+            hits.data_ptr<bool>(),         // [n_rays, n_grids]
+            t_sorted.data_ptr<float>(),    // [n_rays, n_grids * 2]
+            t_indices.data_ptr<int64_t>(), // [n_rays, n_grids * 2]
+            // options
+            near_planes.data_ptr<float>(), // [n_rays]
+            far_planes.data_ptr<float>(),  // [n_rays]
+            step_size,
+            cone_angle,
+            traverse_steps_limit,
+            // outputs
+            false,
+            device::PackedRaySegmentsSpec(intervals),
+            device::PackedRaySegmentsSpec(samples),
+            compute_terminate_planes ? terminate_planes.data_ptr<float>() : nullptr);
+    }
     
-    // second pass to record the segments.
-    if (compute_intervals)
-        intervals.memalloc_data(true, true);
-    if (compute_samples)
-        samples.memalloc_data(false, false);
-    device::traverse_grids_kernel<<<blocks, threads, 0, stream>>>(
-        // rays
-        n_rays,
-        rays_o.data_ptr<float>(),  // [n_rays, 3]
-        rays_d.data_ptr<float>(),  // [n_rays, 3]
-        // grids
-        n_grids,
-        resolution,
-        binaries.data_ptr<bool>(), // [n_grids, resx, resy, resz]
-        aabbs.data_ptr<float>(),   // [n_grids, 6]
-        // sorted intersections
-        hits.data_ptr<bool>(),         // [n_rays, n_grids]
-        t_sorted.data_ptr<float>(),    // [n_rays, n_grids * 2]
-        t_indices.data_ptr<int64_t>(), // [n_rays, n_grids * 2]
-        // options
-        near_planes.data_ptr<float>(), // [n_rays]
-        far_planes.data_ptr<float>(),  // [n_rays]
-        step_size,
-        cone_angle,
-        // outputs
-        false,
-        device::PackedRaySegmentsSpec(intervals),
-        device::PackedRaySegmentsSpec(samples));
-
-    return {intervals, samples};
+    return {intervals, samples, terminate_planes};
 }
 
 
 std::vector<torch::Tensor> ray_aabb_intersect(
     const torch::Tensor rays_o, // [n_rays, 3]
     const torch::Tensor rays_d, // [n_rays, 3]
     const torch::Tensor aabbs,  // [n_aabbs, 6]
```

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/include/data_spec.hpp` & `nerfacc-0.5.3/nerfacc/cuda/csrc/include/data_spec.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,21 @@
 #pragma once
 
 #include <torch/extension.h>
 #include "utils_cuda.cuh"
 
-struct MultiScaleGridSpec {
-  torch::Tensor data;      // [levels, resx, resy, resz]
-  torch::Tensor occupied;    // [levels, resx, resy, resz]
-  torch::Tensor base_aabb; // [6,]
-
-  inline void check() {
-    CHECK_INPUT(data);
-    CHECK_INPUT(occupied);
-    CHECK_INPUT(base_aabb);
-
-    TORCH_CHECK(data.ndimension() == 4);
-    TORCH_CHECK(occupied.ndimension() == 4);
-    TORCH_CHECK(base_aabb.ndimension() == 1);
-
-    TORCH_CHECK(data.numel() == occupied.numel());
-    TORCH_CHECK(base_aabb.numel() == 6);
-  }
-};
-
-struct RaysSpec {
-  torch::Tensor origins;  // [n_rays, 3]
-  torch::Tensor dirs;     // [n_rays, 3]
-
-  inline void check() {
-    CHECK_INPUT(origins);
-    CHECK_INPUT(dirs);
-
-    TORCH_CHECK(origins.ndimension() == 2);
-    TORCH_CHECK(dirs.ndimension() == 2);
-
-    TORCH_CHECK(origins.numel() == dirs.numel());
-
-    TORCH_CHECK(origins.size(1) == 3);
-    TORCH_CHECK(dirs.size(1) == 3);
-  }
-};
-
-
 struct RaySegmentsSpec {
   torch::Tensor vals;        // [n_edges] or [n_rays, n_edges_per_ray]
   // for flattened tensor
   torch::Tensor chunk_starts; // [n_rays]
   torch::Tensor chunk_cnts;   // [n_rays]
   torch::Tensor ray_indices;      // [n_edges]
   torch::Tensor is_left;      // [n_edges] have n_bins true values
   torch::Tensor is_right;     // [n_edges] have n_bins true values
+  torch::Tensor is_valid;     // [n_edges] have n_bins true values
 
   inline void check() {
     CHECK_INPUT(vals);
     TORCH_CHECK(vals.defined());
 
     // batched tensor [..., n_edges_per_ray]
     if (vals.ndimension() > 1) return;
@@ -76,45 +39,69 @@
       TORCH_CHECK(vals.numel() == is_left.numel());
     }
     if (is_right.defined()) {
       CHECK_INPUT(is_right);
       TORCH_CHECK(is_right.ndimension() == 1);
       TORCH_CHECK(vals.numel() == is_right.numel());
     }
+    if (is_valid.defined()) {
+      CHECK_INPUT(is_valid);
+      TORCH_CHECK(is_valid.ndimension() == 1);
+      TORCH_CHECK(vals.numel() == is_valid.numel());
+    }
   }
 
   inline void memalloc_cnts(int32_t n_rays, at::TensorOptions options, bool zero_init = true) {
     TORCH_CHECK(!chunk_cnts.defined());
     if (zero_init) {
       chunk_cnts = torch::zeros({n_rays}, options.dtype(torch::kLong));
     } else {
       chunk_cnts = torch::empty({n_rays}, options.dtype(torch::kLong));
     }
   }
 
-  inline int64_t memalloc_data(bool alloc_masks = true, bool zero_init = true) {
+  inline void memalloc_data(int32_t size, bool alloc_masks = true, bool zero_init = true, bool alloc_valid = false) {
     TORCH_CHECK(chunk_cnts.defined());
-    TORCH_CHECK(!chunk_starts.defined());
     TORCH_CHECK(!vals.defined());
-    
-    torch::Tensor cumsum = torch::cumsum(chunk_cnts, 0, chunk_cnts.scalar_type());
-    int64_t n_edges = cumsum[-1].item<int64_t>();
-    
-    chunk_starts = cumsum - chunk_cnts;
+
     if (zero_init) {
-      vals = torch::zeros({n_edges}, chunk_cnts.options().dtype(torch::kFloat32));
-      ray_indices = torch::zeros({n_edges}, chunk_cnts.options().dtype(torch::kLong));
+      vals = torch::zeros({size}, chunk_cnts.options().dtype(torch::kFloat32));
+      ray_indices = torch::zeros({size}, chunk_cnts.options().dtype(torch::kLong));
       if (alloc_masks) {
-        is_left = torch::zeros({n_edges}, chunk_cnts.options().dtype(torch::kBool));
-        is_right = torch::zeros({n_edges}, chunk_cnts.options().dtype(torch::kBool));
+        is_left = torch::zeros({size}, chunk_cnts.options().dtype(torch::kBool));
+        is_right = torch::zeros({size}, chunk_cnts.options().dtype(torch::kBool));
       }
     } else {
-      vals = torch::empty({n_edges}, chunk_cnts.options().dtype(torch::kFloat32));
-      ray_indices = torch::empty({n_edges}, chunk_cnts.options().dtype(torch::kLong));
+      vals = torch::empty({size}, chunk_cnts.options().dtype(torch::kFloat32));
+      ray_indices = torch::empty({size}, chunk_cnts.options().dtype(torch::kLong));
       if (alloc_masks) {
-        is_left = torch::empty({n_edges}, chunk_cnts.options().dtype(torch::kBool));
-        is_right = torch::empty({n_edges}, chunk_cnts.options().dtype(torch::kBool));
+        is_left = torch::empty({size}, chunk_cnts.options().dtype(torch::kBool));
+        is_right = torch::empty({size}, chunk_cnts.options().dtype(torch::kBool));
       }
     }
+    if (alloc_valid) {
+      is_valid = torch::zeros({size}, chunk_cnts.options().dtype(torch::kBool));
+    }
+  }
+
+  inline int64_t memalloc_data_from_chunk(bool alloc_masks = true, bool zero_init = true, bool alloc_valid = false) {
+    TORCH_CHECK(chunk_cnts.defined());
+    TORCH_CHECK(!chunk_starts.defined());
+    
+    torch::Tensor cumsum = torch::cumsum(chunk_cnts, 0, chunk_cnts.scalar_type());
+    int64_t n_edges = cumsum[-1].item<int64_t>();
+    
+    chunk_starts = cumsum - chunk_cnts;
+    memalloc_data(n_edges, alloc_masks, zero_init, alloc_valid);
+    return 1;
+  }
+
+  // compute the chunk_start from chunk_cnts
+  inline int64_t compute_chunk_start() {
+    TORCH_CHECK(chunk_cnts.defined());
+    // TORCH_CHECK(!chunk_starts.defined());
+    
+    torch::Tensor cumsum = torch::cumsum(chunk_cnts, 0, chunk_cnts.scalar_type());
+    chunk_starts = cumsum - chunk_cnts;
     return 1;
   }
 };
```

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_camera.cuh` & `nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_camera.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_contraction.cuh` & `nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_contraction.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_grid.cuh` & `nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_grid.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_math.cuh` & `nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_math.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_scan.cuh` & `nerfacc-0.5.3/nerfacc/cuda/csrc/include/utils_scan.cuh`

 * *Files 12% similar despite different names*

```diff
@@ -3,33 +3,14 @@
  * 
  * Modified from
  * https://github.com/pytorch/pytorch/blob/06a64f7eaa47ce430a3fa61016010075b59b18a7/aten/src/ATen/native/cuda/ScanUtils.cuh
  */
 
 #include "utils_cuda.cuh"
 
-// CUB support for scan by key is added to cub 1.15
-// in https://github.com/NVIDIA/cub/pull/376
-#if CUB_VERSION >= 101500
-#define CUB_SUPPORTS_SCAN_BY_KEY() 1
-#else
-#define CUB_SUPPORTS_SCAN_BY_KEY() 0
-#endif
-
-// https://github.com/pytorch/pytorch/blob/233305a852e1cd7f319b15b5137074c9eac455f6/aten/src/ATen/cuda/cub.cuh#L38-L46
-#define CUB_WRAPPER(func, ...) do {                                       \
-  size_t temp_storage_bytes = 0;                                          \
-  func(nullptr, temp_storage_bytes, __VA_ARGS__);                         \
-  auto& caching_allocator = *::c10::cuda::CUDACachingAllocator::get();    \
-  auto temp_storage = caching_allocator.allocate(temp_storage_bytes);     \
-  func(temp_storage.get(), temp_storage_bytes, __VA_ARGS__);              \
-  AT_CUDA_CHECK(cudaGetLastError());                                      \
-} while (false)
-
-
 namespace {
 namespace device {
 
 /* Perform an inclusive scan for a flattened tensor.
  *
  * - num_rows is the size of the outer dimensions;
  * - {chunk_starts, chunk_cnts} defines the regions of the flattened tensor to be scanned.
```

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/nerfacc.cpp` & `nerfacc-0.5.3/nerfacc/cuda/csrc/nerfacc.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 // This file contains only Python bindings
 #include "include/data_spec.hpp"
 
 #include <torch/extension.h>
 
-bool is_cub_available() {
-    // FIXME: why return false?
-    return (bool) CUB_SUPPORTS_SCAN_BY_KEY();
-}
 
 // scan
-torch::Tensor exclusive_sum_by_key(
-    torch::Tensor indices,
-    torch::Tensor inputs,
-    bool backward);
 torch::Tensor inclusive_sum(
     torch::Tensor chunk_starts,
     torch::Tensor chunk_cnts,
     torch::Tensor inputs,
     bool normalize,
     bool backward);
 torch::Tensor exclusive_sum(
@@ -50,32 +42,36 @@
 std::vector<torch::Tensor> ray_aabb_intersect(
     const torch::Tensor rays_o, // [n_rays, 3]
     const torch::Tensor rays_d, // [n_rays, 3]
     const torch::Tensor aabbs,  // [n_aabbs, 6]
     const float near_plane,
     const float far_plane, 
     const float miss_value);
-std::vector<RaySegmentsSpec> traverse_grids(
+std::tuple<RaySegmentsSpec, RaySegmentsSpec, torch::Tensor> traverse_grids(
     // rays
     const torch::Tensor rays_o, // [n_rays, 3]
     const torch::Tensor rays_d, // [n_rays, 3]
+    const torch::Tensor rays_mask,   // [n_rays]
     // grids
     const torch::Tensor binaries,  // [n_grids, resx, resy, resz]
     const torch::Tensor aabbs,     // [n_grids, 6]
     // intersections
-    const torch::Tensor t_mins,  // [n_rays, n_grids]
-    const torch::Tensor t_maxs,  // [n_rays, n_grids]
+    const torch::Tensor t_sorted,  // [n_rays, n_grids * 2]
+    const torch::Tensor t_indices,  // [n_rays, n_grids * 2]
     const torch::Tensor hits,    // [n_rays, n_grids]
     // options
     const torch::Tensor near_planes,
     const torch::Tensor far_planes,
     const float step_size,
     const float cone_angle,
     const bool compute_intervals,
-    const bool compute_samples);
+    const bool compute_samples,
+    const bool compute_terminate_planes,
+    const int32_t traverse_steps_limit, // <= 0 means no limit
+    const bool over_allocate); // over allocate the memory for intervals and samples
 
 // pdf
 std::vector<RaySegmentsSpec> importance_sampling(
     RaySegmentsSpec ray_segments,
     torch::Tensor cdfs,                 
     torch::Tensor n_intervels_per_ray,  
     bool stratified);
@@ -99,48 +95,35 @@
     const torch::Tensor& params,  // [..., 4]
     const float criteria_eps,
     const int criteria_iters);
 
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
 #define _REG_FUNC(funname) m.def(#funname, &funname)
-    _REG_FUNC(is_cub_available);  // TODO: check this function
-
-    _REG_FUNC(exclusive_sum_by_key);
     _REG_FUNC(inclusive_sum);
     _REG_FUNC(exclusive_sum);
     _REG_FUNC(inclusive_prod_forward);
     _REG_FUNC(inclusive_prod_backward);
     _REG_FUNC(exclusive_prod_forward);
     _REG_FUNC(exclusive_prod_backward);
 
     _REG_FUNC(ray_aabb_intersect);
     _REG_FUNC(traverse_grids);
     _REG_FUNC(searchsorted);
 
     _REG_FUNC(opencv_lens_undistortion);
-    _REG_FUNC(opencv_lens_undistortion_fisheye);
+    _REG_FUNC(opencv_lens_undistortion_fisheye);  // TODO: check this function.
 #undef _REG_FUNC
 
     m.def("importance_sampling", py::overload_cast<RaySegmentsSpec, torch::Tensor, torch::Tensor, bool>(&importance_sampling));
     m.def("importance_sampling", py::overload_cast<RaySegmentsSpec, torch::Tensor, int64_t, bool>(&importance_sampling));
 
-    py::class_<MultiScaleGridSpec>(m, "MultiScaleGridSpec")
-        .def(py::init<>())
-        .def_readwrite("data", &MultiScaleGridSpec::data)
-        .def_readwrite("occupied", &MultiScaleGridSpec::occupied)
-        .def_readwrite("base_aabb", &MultiScaleGridSpec::base_aabb);
-
-    py::class_<RaysSpec>(m, "RaysSpec")
-        .def(py::init<>())
-        .def_readwrite("origins", &RaysSpec::origins)
-        .def_readwrite("dirs", &RaysSpec::dirs);
-
     py::class_<RaySegmentsSpec>(m, "RaySegmentsSpec")
         .def(py::init<>())
         .def_readwrite("vals", &RaySegmentsSpec::vals)
         .def_readwrite("is_left", &RaySegmentsSpec::is_left)
         .def_readwrite("is_right", &RaySegmentsSpec::is_right)
+        .def_readwrite("is_valid", &RaySegmentsSpec::is_valid)
         .def_readwrite("chunk_starts", &RaySegmentsSpec::chunk_starts)
         .def_readwrite("chunk_cnts", &RaySegmentsSpec::chunk_cnts)
         .def_readwrite("ray_indices", &RaySegmentsSpec::ray_indices);
 }
```

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/pdf.cu` & `nerfacc-0.5.3/nerfacc/cuda/csrc/pdf.cu`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/cuda/csrc/scan.cu` & `nerfacc-0.5.3/nerfacc/cuda/csrc/scan.cu`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,13 @@
 /*
  * Copyright (c) 2022 Ruilong Li, UC Berkeley.
  */
 
 #include <thrust/iterator/reverse_iterator.h>
 #include "include/utils_scan.cuh"
-#if CUB_SUPPORTS_SCAN_BY_KEY()
-#include <cub/cub.cuh>
-#endif
-
-
-namespace {
-namespace device {
-    
-#if CUB_SUPPORTS_SCAN_BY_KEY()
-struct Product
-{
-    template <typename T>
-    __host__ __device__ __forceinline__ T operator()(const T &a, const T &b) const { return a * b; }
-};
-
-template <typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT>
-inline void exclusive_sum_by_key(
-    KeysInputIteratorT keys, ValuesInputIteratorT input, ValuesOutputIteratorT output, int64_t num_items)
-{
-    TORCH_CHECK(num_items <= std::numeric_limits<int64_t>::max(),
-                "cub ExclusiveSumByKey does not support more than LONG_MAX elements");
-    CUB_WRAPPER(cub::DeviceScan::ExclusiveSumByKey, keys, input, output,
-                num_items, cub::Equality(), at::cuda::getCurrentCUDAStream());
-}
-
-template <typename KeysInputIteratorT, typename ValuesInputIteratorT, typename ValuesOutputIteratorT>
-inline void exclusive_prod_by_key(
-    KeysInputIteratorT keys, ValuesInputIteratorT input, ValuesOutputIteratorT output, int64_t num_items)
-{
-    TORCH_CHECK(num_items <= std::numeric_limits<int64_t>::max(),
-                "cub ExclusiveScanByKey does not support more than LONG_MAX elements");
-    CUB_WRAPPER(cub::DeviceScan::ExclusiveScanByKey, keys, input, output, Product(), 1.0f,
-                num_items, cub::Equality(), at::cuda::getCurrentCUDAStream());
-}
-#endif
-
-
-} // namespace device
-} // namespace
-
-
-torch::Tensor exclusive_sum_by_key(
-    torch::Tensor indices,
-    torch::Tensor inputs,
-    bool backward) 
-{
-    DEVICE_GUARD(inputs);
-
-    torch::Tensor outputs = torch::empty_like(inputs);
-    int64_t n_items = inputs.size(0);
-#if CUB_SUPPORTS_SCAN_BY_KEY()
-    if (backward)
-        device::exclusive_sum_by_key(
-            thrust::make_reverse_iterator(indices.data_ptr<int64_t>() + n_items),
-            thrust::make_reverse_iterator(inputs.data_ptr<float>() + n_items),
-            thrust::make_reverse_iterator(outputs.data_ptr<float>() + n_items),
-            n_items);
-    else
-        device::exclusive_sum_by_key(
-            indices.data_ptr<int64_t>(),
-            inputs.data_ptr<float>(),
-            outputs.data_ptr<float>(),
-            n_items);
-#else
-    std::runtime_error("CUB functions are only supported in CUDA >= 11.6.");
-#endif
-    cudaGetLastError();
-    return outputs;
-}
 
 
 torch::Tensor inclusive_sum(
     torch::Tensor chunk_starts,
     torch::Tensor chunk_cnts,
     torch::Tensor inputs,
     bool normalize,
@@ -93,20 +24,23 @@
     TORCH_CHECK(chunk_starts.size(0) == chunk_cnts.size(0));
     if (backward)
         TORCH_CHECK(~normalize); // backward does not support normalize yet.
 
     uint32_t n_rays = chunk_cnts.size(0);
     int64_t n_edges = inputs.size(0);
 
+    torch::Tensor outputs = torch::empty_like(inputs);
+    if (n_edges == 0) {
+        return outputs;
+    }
+
     at::cuda::CUDAStream stream = at::cuda::getCurrentCUDAStream();
     int32_t max_blocks = 65535;
     dim3 threads = dim3(16, 32);
     dim3 blocks = dim3(min(max_blocks, ceil_div<int32_t>(n_rays, threads.y)));
-
-    torch::Tensor outputs = torch::empty_like(inputs);
     
     if (backward) {
         chunk_starts = n_edges - (chunk_starts + chunk_cnts);
         device::inclusive_scan_kernel<float, 16, 32><<<blocks, threads, 0, stream>>>(
             thrust::make_reverse_iterator(outputs.data_ptr<float>() + n_edges),
             thrust::make_reverse_iterator(inputs.data_ptr<float>() + n_edges),
             n_rays,
@@ -149,20 +83,23 @@
     TORCH_CHECK(chunk_starts.size(0) == chunk_cnts.size(0));
     if (backward)
         TORCH_CHECK(~normalize); // backward does not support normalize yet.
 
     uint32_t n_rays = chunk_cnts.size(0);
     int64_t n_edges = inputs.size(0);
 
+    torch::Tensor outputs = torch::empty_like(inputs);
+    if (n_edges == 0) {
+        return outputs;
+    }
+
     at::cuda::CUDAStream stream = at::cuda::getCurrentCUDAStream();
     int32_t max_blocks = 65535;
     dim3 threads = dim3(16, 32);
     dim3 blocks = dim3(min(max_blocks, ceil_div<int32_t>(n_rays, threads.y)));
-
-    torch::Tensor outputs = torch::empty_like(inputs);
     
     if (backward) {
         chunk_starts = n_edges - (chunk_starts + chunk_cnts);
         device::exclusive_scan_kernel<float, 16, 32><<<blocks, threads, 0, stream>>>(
             thrust::make_reverse_iterator(outputs.data_ptr<float>() + n_edges),
             thrust::make_reverse_iterator(inputs.data_ptr<float>() + n_edges),
             n_rays,
@@ -201,20 +138,23 @@
     TORCH_CHECK(chunk_cnts.ndimension() == 1);
     TORCH_CHECK(inputs.ndimension() == 1);
     TORCH_CHECK(chunk_starts.size(0) == chunk_cnts.size(0));
 
     uint32_t n_rays = chunk_cnts.size(0);
     int64_t n_edges = inputs.size(0);
 
+    torch::Tensor outputs = torch::empty_like(inputs);
+    if (n_edges == 0) {
+        return outputs;
+    }
+    
     at::cuda::CUDAStream stream = at::cuda::getCurrentCUDAStream();
     int32_t max_blocks = 65535;
     dim3 threads = dim3(16, 32);
     dim3 blocks = dim3(min(max_blocks, ceil_div<int32_t>(n_rays, threads.y)));
-
-    torch::Tensor outputs = torch::empty_like(inputs);
     
     device::inclusive_scan_kernel<float, 16, 32><<<blocks, threads, 0, stream>>>(
         outputs.data_ptr<float>(),
         inputs.data_ptr<float>(),
         n_rays,
         chunk_starts.data_ptr<int64_t>(), 
         chunk_cnts.data_ptr<int64_t>(), 
@@ -242,20 +182,23 @@
     TORCH_CHECK(chunk_cnts.ndimension() == 1);
     TORCH_CHECK(inputs.ndimension() == 1);
     TORCH_CHECK(chunk_starts.size(0) == chunk_cnts.size(0));
 
     uint32_t n_rays = chunk_cnts.size(0);
     int64_t n_edges = inputs.size(0);
 
+    torch::Tensor grad_inputs = torch::empty_like(grad_outputs);
+    if (n_edges == 0) {
+        return grad_inputs;
+    }
+
     at::cuda::CUDAStream stream = at::cuda::getCurrentCUDAStream();
     int32_t max_blocks = 65535;
     dim3 threads = dim3(16, 32);
     dim3 blocks = dim3(min(max_blocks, ceil_div<int32_t>(n_rays, threads.y)));
-
-    torch::Tensor grad_inputs = torch::empty_like(grad_outputs);
     
     chunk_starts = n_edges - (chunk_starts + chunk_cnts);
     device::inclusive_scan_kernel<float, 16, 32><<<blocks, threads, 0, stream>>>(
         thrust::make_reverse_iterator(grad_inputs.data_ptr<float>() + n_edges),
         thrust::make_reverse_iterator((grad_outputs * outputs).data_ptr<float>() + n_edges),
         n_rays,
         thrust::make_reverse_iterator(chunk_starts.data_ptr<int64_t>() + n_rays), 
@@ -285,20 +228,23 @@
     TORCH_CHECK(chunk_cnts.ndimension() == 1);
     TORCH_CHECK(inputs.ndimension() == 1);
     TORCH_CHECK(chunk_starts.size(0) == chunk_cnts.size(0));
 
     uint32_t n_rays = chunk_cnts.size(0);
     int64_t n_edges = inputs.size(0);
 
+    torch::Tensor outputs = torch::empty_like(inputs);
+    if (n_edges == 0) {
+        return outputs;
+    }
+
     at::cuda::CUDAStream stream = at::cuda::getCurrentCUDAStream();
     int32_t max_blocks = 65535;
     dim3 threads = dim3(16, 32);
     dim3 blocks = dim3(min(max_blocks, ceil_div<int32_t>(n_rays, threads.y)));
-
-    torch::Tensor outputs = torch::empty_like(inputs);
     
     device::exclusive_scan_kernel<float, 16, 32><<<blocks, threads, 0, stream>>>(
         outputs.data_ptr<float>(),
         inputs.data_ptr<float>(),
         n_rays,
         chunk_starts.data_ptr<int64_t>(), 
         chunk_cnts.data_ptr<int64_t>(), 
@@ -326,20 +272,23 @@
     TORCH_CHECK(chunk_cnts.ndimension() == 1);
     TORCH_CHECK(inputs.ndimension() == 1);
     TORCH_CHECK(chunk_starts.size(0) == chunk_cnts.size(0));
 
     uint32_t n_rays = chunk_cnts.size(0);
     int64_t n_edges = inputs.size(0);
 
+    torch::Tensor grad_inputs = torch::empty_like(grad_outputs);
+    if (n_edges == 0) {
+        return grad_inputs;
+    }
+
     at::cuda::CUDAStream stream = at::cuda::getCurrentCUDAStream();
     int32_t max_blocks = 65535;
     dim3 threads = dim3(16, 32);
     dim3 blocks = dim3(min(max_blocks, ceil_div<int32_t>(n_rays, threads.y)));
-
-    torch::Tensor grad_inputs = torch::empty_like(grad_outputs);
     
     chunk_starts = n_edges - (chunk_starts + chunk_cnts);
     device::exclusive_scan_kernel<float, 16, 32><<<blocks, threads, 0, stream>>>(
         thrust::make_reverse_iterator(grad_inputs.data_ptr<float>() + n_edges),
         thrust::make_reverse_iterator((grad_outputs * outputs).data_ptr<float>() + n_edges),
         n_rays,
         thrust::make_reverse_iterator(chunk_starts.data_ptr<int64_t>() + n_rays),
```

### Comparing `nerfacc-0.5.2/nerfacc/data_specs.py` & `nerfacc-0.5.3/nerfacc/data_specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         >>> )
 
     """
 
     vals: torch.Tensor
     packed_info: Optional[torch.Tensor] = None
     ray_indices: Optional[torch.Tensor] = None
+    is_valid: Optional[torch.Tensor] = None
 
     def _to_cpp(self):
         """
         Generate object to pass to C++
         """
 
         spec = _C.RaySegmentsSpec()
@@ -65,16 +66,24 @@
         Generate object from C++
         """
         if spec.chunk_starts is not None and spec.chunk_cnts is not None:
             packed_info = torch.stack([spec.chunk_starts, spec.chunk_cnts], -1)
         else:
             packed_info = None
         ray_indices = spec.ray_indices
+        if spec.is_valid is not None:
+            is_valid = spec.is_valid
+        else:
+            is_valid = None
+        vals = spec.vals
         return cls(
-            vals=spec.vals, packed_info=packed_info, ray_indices=ray_indices
+            vals=vals,
+            packed_info=packed_info,
+            ray_indices=ray_indices,
+            is_valid=is_valid,
         )
 
     @property
     def device(self) -> torch.device:
         return self.vals.device
```

### Comparing `nerfacc-0.5.2/nerfacc/estimators/base.py` & `nerfacc-0.5.3/nerfacc/estimators/base.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/estimators/occ_grid.py` & `nerfacc-0.5.3/nerfacc/estimators/occ_grid.py`

 * *Files 11% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         if t_min is not None:
             near_planes = torch.clamp(near_planes, min=t_min)
         if t_max is not None:
             far_planes = torch.clamp(far_planes, max=t_max)
 
         if stratified:
             near_planes += torch.rand_like(near_planes) * render_step_size
-        intervals, samples = traverse_grids(
+        intervals, samples, _ = traverse_grids(
             rays_o,
             rays_d,
             self.binaries,
             self.aabbs,
             near_planes=near_planes,
             far_planes=far_planes,
             step_size=render_step_size,
@@ -180,28 +180,34 @@
         if (alpha_thre > 0.0 or early_stop_eps > 0.0) and (
             sigma_fn is not None or alpha_fn is not None
         ):
             alpha_thre = min(alpha_thre, self.occs.mean().item())
 
             # Compute visibility of the samples, and filter out invisible samples
             if sigma_fn is not None:
-                sigmas = sigma_fn(t_starts, t_ends, ray_indices)
+                if t_starts.shape[0] != 0:
+                    sigmas = sigma_fn(t_starts, t_ends, ray_indices)
+                else:
+                    sigmas = torch.empty((0,), device=t_starts.device)
                 assert (
                     sigmas.shape == t_starts.shape
                 ), "sigmas must have shape of (N,)! Got {}".format(sigmas.shape)
                 masks = render_visibility_from_density(
                     t_starts=t_starts,
                     t_ends=t_ends,
                     sigmas=sigmas,
                     packed_info=packed_info,
                     early_stop_eps=early_stop_eps,
                     alpha_thre=alpha_thre,
                 )
             elif alpha_fn is not None:
-                alphas = alpha_fn(t_starts, t_ends, ray_indices)
+                if t_starts.shape[0] != 0:
+                    alphas = alpha_fn(t_starts, t_ends, ray_indices)
+                else:
+                    alphas = torch.empty((0,), device=t_starts.device)
                 assert (
                     alphas.shape == t_starts.shape
                 ), "alphas must have shape of (N,)! Got {}".format(alphas.shape)
                 masks = render_visibility_from_alpha(
                     alphas=alphas,
                     packed_info=packed_info,
                     early_stop_eps=early_stop_eps,
@@ -248,27 +254,109 @@
                 step=step,
                 occ_eval_fn=occ_eval_fn,
                 occ_thre=occ_thre,
                 ema_decay=ema_decay,
                 warmup_steps=warmup_steps,
             )
 
+    # adapted from https://github.com/kwea123/ngp_pl/blob/master/models/networks.py
+    @torch.no_grad()
+    def mark_invisible_cells(
+        self,
+        K: Tensor,
+        c2w: Tensor,
+        width: int,
+        height: int,
+        near_plane: float = 0.0,
+        chunk: int = 32**3,
+    ) -> None:
+        """Mark the cells that aren't covered by the cameras with density -1.
+        Should only be executed once before training starts.
+
+        Args:
+            K: Camera intrinsics of shape (N, 3, 3) or (1, 3, 3).
+            c2w: Camera to world poses of shape (N, 3, 4) or (N, 4, 4).
+            width: Image width in pixels
+            height: Image height in pixels
+            near_plane: Near plane distance
+            chunk: The chunk size to split the cells (to avoid OOM)
+        """
+        assert K.dim() == 3 and K.shape[1:] == (3, 3)
+        assert c2w.dim() == 3 and (
+            c2w.shape[1:] == (3, 4) or c2w.shape[1:] == (4, 4)
+        )
+        assert K.shape[0] == c2w.shape[0] or K.shape[0] == 1
+
+        N_cams = c2w.shape[0]
+        w2c_R = c2w[:, :3, :3].transpose(2, 1)  # (N_cams, 3, 3)
+        w2c_T = -w2c_R @ c2w[:, :3, 3:]  # (N_cams, 3, 1)
+
+        lvl_indices = self._get_all_cells()
+        for lvl, indices in enumerate(lvl_indices):
+            grid_coords = self.grid_coords[indices]
+
+            for i in range(0, len(indices), chunk):
+                x = grid_coords[i : i + chunk] / (self.resolution - 1)
+                indices_chunk = indices[i : i + chunk]
+                # voxel coordinates [0, 1]^3 -> world
+                xyzs_w = (
+                    self.aabbs[lvl, :3]
+                    + x * (self.aabbs[lvl, 3:] - self.aabbs[lvl, :3])
+                ).T
+                xyzs_c = w2c_R @ xyzs_w + w2c_T  # (N_cams, 3, chunk)
+                uvd = K @ xyzs_c  # (N_cams, 3, chunk)
+                uv = uvd[:, :2] / uvd[:, 2:]  # (N_cams, 2, chunk)
+                in_image = (
+                    (uvd[:, 2] >= 0)
+                    & (uv[:, 0] >= 0)
+                    & (uv[:, 0] < width)
+                    & (uv[:, 1] >= 0)
+                    & (uv[:, 1] < height)
+                )
+                covered_by_cam = (
+                    uvd[:, 2] >= near_plane
+                ) & in_image  # (N_cams, chunk)
+                # if the cell is visible by at least one camera
+                count = covered_by_cam.sum(0) / N_cams
+
+                too_near_to_cam = (
+                    uvd[:, 2] < near_plane
+                ) & in_image  # (N, chunk)
+                # if the cell is too close (in front) to any camera
+                too_near_to_any_cam = too_near_to_cam.any(0)
+                # a valid cell should be visible by at least one camera and not too close to any camera
+                valid_mask = (count > 0) & (~too_near_to_any_cam)
+
+                cell_ids_base = lvl * self.cells_per_lvl
+                self.occs[cell_ids_base + indices_chunk] = torch.where(
+                    valid_mask, 0.0, -1.0
+                )
+
     @torch.no_grad()
     def _get_all_cells(self) -> List[Tensor]:
         """Returns all cells of the grid."""
-        return [self.grid_indices] * self.levels
+        lvl_indices = []
+        for lvl in range(self.levels):
+            # filter out the cells with -1 density (non-visible to any camera)
+            cell_ids = lvl * self.cells_per_lvl + self.grid_indices
+            indices = self.grid_indices[self.occs[cell_ids] >= 0.0]
+            lvl_indices.append(indices)
+        return lvl_indices
 
     @torch.no_grad()
     def _sample_uniform_and_occupied_cells(self, n: int) -> List[Tensor]:
         """Samples both n uniform and occupied cells."""
         lvl_indices = []
         for lvl in range(self.levels):
             uniform_indices = torch.randint(
                 self.cells_per_lvl, (n,), device=self.device
             )
+            # filter out the cells with -1 density (non-visible to any camera)
+            cell_ids = lvl * self.cells_per_lvl + uniform_indices
+            uniform_indices = uniform_indices[self.occs[cell_ids] >= 0.0]
             occupied_indices = torch.nonzero(self.binaries[lvl].flatten())[:, 0]
             if n < len(occupied_indices):
                 selector = torch.randint(
                     len(occupied_indices), (n,), device=self.device
                 )
                 occupied_indices = occupied_indices[selector]
             indices = torch.cat([uniform_indices, occupied_indices], dim=0)
@@ -308,17 +396,16 @@
             self.occs[cell_ids] = torch.maximum(
                 self.occs[cell_ids] * ema_decay, occ
             )
             # suppose to use scatter max but emperically it is almost the same.
             # self.occs, _ = scatter_max(
             #     occ, indices, dim=0, out=self.occs * ema_decay
             # )
-        self.binaries = (
-            self.occs > torch.clamp(self.occs.mean(), max=occ_thre)
-        ).view(self.binaries.shape)
+        thre = torch.clamp(self.occs[self.occs >= 0].mean(), max=occ_thre)
+        self.binaries = (self.occs > thre).view(self.binaries.shape)
 
 
 def _meshgrid3d(
     res: Tensor, device: Union[torch.device, str] = "cpu"
 ) -> Tensor:
     """Create 3D grid coordinates."""
     assert len(res) == 3
```

### Comparing `nerfacc-0.5.2/nerfacc/estimators/prop_net.py` & `nerfacc-0.5.3/nerfacc/estimators/prop_net.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/grid.py` & `nerfacc-0.5.3/nerfacc/grid.py`

 * *Files 17% similar despite different names*

```diff
@@ -99,15 +99,22 @@
     binaries: Tensor,  # [m, resx, resy, resz]
     aabbs: Tensor,  # [m, 6]
     # options
     near_planes: Optional[Tensor] = None,  # [n_rays]
     far_planes: Optional[Tensor] = None,  # [n_rays]
     step_size: Optional[float] = 1e-3,
     cone_angle: Optional[float] = 0.0,
-) -> Tuple[RayIntervals, RaySamples]:
+    traverse_steps_limit: Optional[int] = None,
+    over_allocate: Optional[bool] = False,
+    rays_mask: Optional[Tensor] = None,  # [n_rays]
+    # pre-compute intersections
+    t_sorted: Optional[Tensor] = None,  # [n_rays, n_grids * 2]
+    t_indices: Optional[Tensor] = None,  # [n_rays, n_grids * 2]
+    hits: Optional[Tensor] = None,  # [n_rays, n_grids]
+) -> Tuple[RayIntervals, RaySamples, Tensor]:
     """Ray Traversal within Multiple Grids.
 
     Note:
         This function is not differentiable to any inputs.
 
     Args:
         rays_o: (n_rays, 3) Ray origins.
@@ -115,47 +122,78 @@
         binary_grids: (m, resx, resy, resz) Multiple binary grids with the same resolution.
         aabbs: (m, 6) Axis-aligned bounding boxes {xmin, ymin, zmin, xmax, ymax, zmax}.
         near_planes: Optional. (n_rays,) Near planes for the traversal to start. Default to 0.
         far_planes: Optional. (n_rays,) Far planes for the traversal to end. Default to infinity.
         step_size: Optional. Step size for ray traversal. Default to 1e-3.
         cone_angle: Optional. Cone angle for linearly-increased step size. 0. means
             constant step size. Default: 0.0.
+        traverse_steps_limit: Optional. Maximum number of samples per ray.
+        over_allocate: Optional. Whether to over-allocate the memory for the outputs.
+        rays_mask: Optional. (n_rays,) Skip some rays if given.
+        t_sorted: Optional. (n_rays, n_grids * 2) Pre-computed sorted t values for each ray-grid pair. Default to None.
+        t_indices: Optional. (n_rays, n_grids * 2) Pre-computed sorted t indices for each ray-grid pair. Default to None.
+        hits: Optional. (n_rays, n_grids) Pre-computed hit flags for each ray-grid pair. Default to None.
 
     Returns:
         A :class:`RayIntervals` object containing the intervals of the ray traversal, and
         a :class:`RaySamples` object containing the samples within each interval.
+        t :class:`Tensor` of shape (n_rays,) containing the terminated t values for each ray.
     """
-    # Compute ray aabb intersection for all levels of grid. [n_rays, m]
-    t_mins, t_maxs, hits = ray_aabb_intersect(rays_o, rays_d, aabbs)
 
     if near_planes is None:
         near_planes = torch.zeros_like(rays_o[:, 0])
     if far_planes is None:
         far_planes = torch.full_like(rays_o[:, 0], float("inf"))
 
-    intervals, samples = _C.traverse_grids(
+    if rays_mask is None:
+        rays_mask = torch.ones_like(rays_o[:, 0], dtype=torch.bool)
+    if traverse_steps_limit is None:
+        traverse_steps_limit = -1
+    if over_allocate:
+        assert (
+            traverse_steps_limit > 0
+        ), "traverse_steps_limit must be set if over_allocate is True."
+
+    if t_sorted is None or t_indices is None or hits is None:
+        # Compute ray aabb intersection for all levels of grid. [n_rays, m]
+        t_mins, t_maxs, hits = ray_aabb_intersect(rays_o, rays_d, aabbs)
+        # Sort the t values for each ray. [n_rays, m]
+        t_sorted, t_indices = torch.sort(
+            torch.cat([t_mins, t_maxs], dim=-1), dim=-1
+        )
+
+    # Traverse the grids.
+    intervals, samples, termination_planes = _C.traverse_grids(
         # rays
         rays_o.contiguous(),  # [n_rays, 3]
         rays_d.contiguous(),  # [n_rays, 3]
+        rays_mask.contiguous(),  # [n_rays]
         # grids
         binaries.contiguous(),  # [m, resx, resy, resz]
         aabbs.contiguous(),  # [m, 6]
         # intersections
-        t_mins.contiguous(),  # [n_rays, m]
-        t_maxs.contiguous(),  # [n_rays, m]
+        t_sorted.contiguous(),  # [n_rays, m * 2]
+        t_indices.contiguous(),  # [n_rays, m * 2]
         hits.contiguous(),  # [n_rays, m]
         # options
         near_planes.contiguous(),  # [n_rays]
         far_planes.contiguous(),  # [n_rays]
         step_size,
         cone_angle,
         True,
         True,
+        True,
+        traverse_steps_limit,
+        over_allocate,
+    )
+    return (
+        RayIntervals._from_cpp(intervals),
+        RaySamples._from_cpp(samples),
+        termination_planes,
     )
-    return RayIntervals._from_cpp(intervals), RaySamples._from_cpp(samples)
 
 
 def _enlarge_aabb(aabb, factor: float) -> Tensor:
     center = (aabb[:3] + aabb[3:]) / 2
     extent = (aabb[3:] - aabb[:3]) / 2
     return torch.cat([center - extent * factor, center + extent * factor])
```

### Comparing `nerfacc-0.5.2/nerfacc/pack.py` & `nerfacc-0.5.3/nerfacc/pack.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/pdf.py` & `nerfacc-0.5.3/nerfacc/pdf.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/scan.py` & `nerfacc-0.5.3/nerfacc/scan.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/nerfacc/volrend.py` & `nerfacc-0.5.3/nerfacc/volrend.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,19 @@
     if rgb_sigma_fn is None and rgb_alpha_fn is None:
         raise ValueError(
             "At least one of `rgb_sigma_fn` and `rgb_alpha_fn` should be specified."
         )
 
     # Query sigma/alpha and color with gradients
     if rgb_sigma_fn is not None:
-        rgbs, sigmas = rgb_sigma_fn(t_starts, t_ends, ray_indices)
+        if t_starts.shape[0] != 0:
+            rgbs, sigmas = rgb_sigma_fn(t_starts, t_ends, ray_indices)
+        else:
+            rgbs = torch.empty((0, 3), device=t_starts.device)
+            sigmas = torch.empty((0,), device=t_starts.device)
         assert rgbs.shape[-1] == 3, "rgbs must have 3 channels, got {}".format(
             rgbs.shape
         )
         assert (
             sigmas.shape == t_starts.shape
         ), "sigmas must have shape of (N,)! Got {}".format(sigmas.shape)
         # Rendering: compute weights.
@@ -104,15 +108,19 @@
             "weights": weights,
             "alphas": alphas,
             "trans": trans,
             "sigmas": sigmas,
             "rgbs": rgbs,
         }
     elif rgb_alpha_fn is not None:
-        rgbs, alphas = rgb_alpha_fn(t_starts, t_ends, ray_indices)
+        if t_starts.shape[0] != 0:
+            rgbs, alphas = rgb_alpha_fn(t_starts, t_ends, ray_indices)
+        else:
+            rgbs = torch.empty((0, 3), device=t_starts.device)
+            alphas = torch.empty((0,), device=t_starts.device)
         assert rgbs.shape[-1] == 3, "rgbs must have 3 channels, got {}".format(
             rgbs.shape
         )
         assert (
             alphas.shape == t_starts.shape
         ), "alphas must have shape of (N,)! Got {}".format(alphas.shape)
         # Rendering: compute weights.
@@ -533,7 +541,33 @@
         outputs = torch.zeros(
             (n_rays, src.shape[-1]), device=src.device, dtype=src.dtype
         )
         outputs.index_add_(0, ray_indices, src)
     else:
         outputs = torch.sum(src, dim=-2)
     return outputs
+
+
+def accumulate_along_rays_(
+    weights: Tensor,
+    values: Optional[Tensor] = None,
+    ray_indices: Optional[Tensor] = None,
+    outputs: Optional[Tensor] = None,
+) -> None:
+    """Accumulate volumetric values along the ray.
+
+    Inplace version of :func:`accumulate_along_rays`.
+    """
+    if values is None:
+        src = weights[..., None]
+    else:
+        assert values.dim() == weights.dim() + 1
+        assert weights.shape == values.shape[:-1]
+        src = weights[..., None] * values
+    if ray_indices is not None:
+        assert weights.dim() == 1, "weights must be flattened"
+        assert (
+            outputs.dim() == 2 and outputs.shape[-1] == src.shape[-1]
+        ), "outputs must be of shape (n_rays, D)"
+        outputs.index_add_(0, ray_indices, src)
+    else:
+        outputs.add_(src.sum(dim=-2))
```

### Comparing `nerfacc-0.5.2/nerfacc.egg-info/SOURCES.txt` & `nerfacc-0.5.3/nerfacc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 nerfacc/__init__.py
 nerfacc/cameras.py
-nerfacc/cameras2.py
 nerfacc/data_specs.py
 nerfacc/grid.py
 nerfacc/pack.py
 nerfacc/pdf.py
 nerfacc/scan.py
 nerfacc/version.py
 nerfacc/volrend.py
```

### Comparing `nerfacc-0.5.2/setup.py` & `nerfacc-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,27 +101,32 @@
     description="A General NeRF Acceleration Toolbox",
     author="Ruilong",
     author_email="ruilongli94@gmail.com",
     url=URL,
     download_url=f"{URL}/archive/{__version__}.tar.gz",
     keywords=[],
     python_requires=">=3.7",
-    install_requires=["rich>=12", "torch", "typing_extensions; python_version<'3.8'"],
+    install_requires=[
+        "rich>=12",
+        "torch",
+        "typing_extensions; python_version<'3.8'",
+    ],
     extras_require={
         # dev dependencies. Install them by `pip install nerfacc[dev]`
         "dev": [
             "black[jupyter]==22.3.0",
             "isort==5.10.1",
             "pylint==2.13.4",
             "pytest==7.1.2",
             "pytest-xdist==2.5.0",
             "typeguard>=2.13.3",
             "pyyaml==6.0",
             "build",
             "twine",
+            "ninja",
         ],
     },
     ext_modules=get_extensions() if not BUILD_NO_CUDA else [],
     cmdclass={"build_ext": get_ext()} if not BUILD_NO_CUDA else {},
     packages=find_packages(),
     include_package_data=include_package_data,
 )
```

### Comparing `nerfacc-0.5.2/tests/test_camera.py` & `nerfacc-0.5.3/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/tests/test_pack.py` & `nerfacc-0.5.3/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/tests/test_pdf.py` & `nerfacc-0.5.3/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/tests/test_rendering.py` & `nerfacc-0.5.3/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.2/tests/test_scan.py` & `nerfacc-0.5.3/tests/test_scan.py`

 * *Files identical despite different names*

