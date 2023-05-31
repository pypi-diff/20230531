# Comparing `tmp/nvidia-dali-nightly-cuda110-1.26.0.dev20230427.tar.gz` & `tmp/nvidia-dali-nightly-cuda110-1.27.0.dev20230530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda110-1.26.0.dev20230427.tar", last modified: Tue May  2 16:22:35 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda110-1.27.0.dev20230530.tar", last modified: Tue May 30 16:44:58 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda110-1.26.0.dev20230427.tar` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230530.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-02 16:22:35.065720 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-05-02 16:22:34.000000 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-28 20:21:51.000000 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-05-02 16:22:34.000000 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-05-02 16:22:35.065720 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-05-02 16:22:34.000000 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-02 16:22:35.064720 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/nvidia_dali_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-05-02 16:22:35.000000 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-05-02 16:22:35.000000 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-05-02 16:22:35.000000 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-05-02 16:22:35.000000 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-05-02 16:22:35.065720 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-28 20:21:51.000000 nvidia-dali-nightly-cuda110-1.26.0.dev20230427/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-30 16:44:58.106748 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-05-30 16:44:58.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-05-24 10:07:51.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-05-30 16:44:58.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-05-30 16:44:58.106748 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-05-30 16:44:58.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-30 16:44:58.106748 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/nvidia_dali_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-05-30 16:44:58.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-05-30 16:44:58.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-05-30 16:44:58.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-05-30 16:44:58.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-05-30 16:44:58.106748 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-05-24 10:07:51.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230530/setup.py
```

### Comparing `nvidia-dali-nightly-cuda110-1.26.0.dev20230427/LICENSE.md` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230530/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda110-1.26.0.dev20230427/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230530/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.26.0.dev20230427
+Version: 1.27.0.dev20230530
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.26.0.dev20230427/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230530/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.26.0.dev20230427
+Version: 1.27.0.dev20230530
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.26.0.dev20230427/setup.py` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230530/setup.py`

 * *Files identical despite different names*

