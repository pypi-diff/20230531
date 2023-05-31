# Comparing `tmp/nvidia-dali-nightly-cuda120-1.26.0.dev20230428.tar.gz` & `tmp/nvidia-dali-nightly-cuda120-1.27.0.dev20230530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda120-1.26.0.dev20230428.tar", last modified: Tue May  2 16:17:44 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda120-1.27.0.dev20230530.tar", last modified: Tue May 30 15:44:33 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda120-1.26.0.dev20230428.tar` & `nvidia-dali-nightly-cuda120-1.27.0.dev20230530.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-02 16:17:44.880686 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-05-02 16:17:44.000000 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-28 20:21:51.000000 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-05-02 16:17:44.000000 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-05-02 16:17:44.880686 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-05-02 16:17:44.000000 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-02 16:17:44.880686 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/nvidia_dali_nightly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-05-02 16:17:44.000000 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-05-02 16:17:44.000000 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-05-02 16:17:44.000000 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-05-02 16:17:44.000000 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-05-02 16:17:44.881686 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-28 20:21:51.000000 nvidia-dali-nightly-cuda120-1.26.0.dev20230428/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-30 15:44:33.132246 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-05-30 15:44:33.000000 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-05-24 10:07:51.000000 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-05-30 15:44:33.000000 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-05-30 15:44:33.132246 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-05-30 15:44:33.000000 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-30 15:44:33.128246 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/nvidia_dali_nightly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-05-30 15:44:33.000000 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-05-30 15:44:33.000000 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-05-30 15:44:33.000000 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-05-30 15:44:33.000000 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-05-30 15:44:33.132246 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-05-24 10:07:51.000000 nvidia-dali-nightly-cuda120-1.27.0.dev20230530/setup.py
```

### Comparing `nvidia-dali-nightly-cuda120-1.26.0.dev20230428/LICENSE.md` & `nvidia-dali-nightly-cuda120-1.27.0.dev20230530/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda120-1.26.0.dev20230428/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.27.0.dev20230530/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.26.0.dev20230428
+Version: 1.27.0.dev20230530
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.26.0.dev20230428/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.27.0.dev20230530/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.26.0.dev20230428
+Version: 1.27.0.dev20230530
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.26.0.dev20230428/setup.py` & `nvidia-dali-nightly-cuda120-1.27.0.dev20230530/setup.py`

 * *Files identical despite different names*

