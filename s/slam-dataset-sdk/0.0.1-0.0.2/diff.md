# Comparing `tmp/slam_dataset_sdk-0.0.1.tar.gz` & `tmp/slam_dataset_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slam_dataset_sdk-0.0.1.tar", last modified: Wed Feb  8 19:21:22 2023, max compression
+gzip compressed data, was "slam_dataset_sdk-0.0.2.tar", last modified: Tue May 30 23:02:36 2023, max compression
```

## Comparing `slam_dataset_sdk-0.0.1.tar` & `slam_dataset_sdk-0.0.2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.468613 slam_dataset_sdk-0.0.1/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1623 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/CMakeLists.txt
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1071 2023-02-08 19:17:27.000000 slam_dataset_sdk-0.0.1/LICENSE
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      214 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/MANIFEST.in
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3645 2023-02-08 19:21:22.468613 slam_dataset_sdk-0.0.1/PKG-INFO
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2534 2023-01-31 17:05:11.000000 slam_dataset_sdk-0.0.1/README.md
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      376 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/pyproject.toml
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      994 2023-02-08 19:21:22.468613 slam_dataset_sdk-0.0.1/setup.cfg
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4406 2023-01-13 17:40:23.000000 slam_dataset_sdk-0.0.1/setup.py
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.460613 slam_dataset_sdk-0.0.1/src/
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.460613 slam_dataset_sdk-0.0.1/src/cpp/
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.460613 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.460613 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/eigen/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      779 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/eigen/LICENSE
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1874 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/eigen/eigen.cmake
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2130 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/find_dependencies.cmake
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.460613 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tbb/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)    11357 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tbb/LICENSE
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2285 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tbb/tbb.cmake
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.460613 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tsl_robin/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1102 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tsl_robin/LICENSE
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1888 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tsl_robin/tsl_robin.cmake
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1666 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/CMakeLists.txt
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.460613 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1759 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/CMakeLists.txt
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3013 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Deskew.cpp
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1918 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Deskew.hpp
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     6704 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Map.hpp
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2496 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Preprocessing.cpp
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1882 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Preprocessing.hpp
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4599 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Registration.cpp
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1950 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Registration.hpp
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4963 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/VoxelHashMap.cpp
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4128 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/VoxelHashMap.hpp
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/cpp/metrics/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1569 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/metrics/CMakeLists.txt
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3662 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/metrics/Metrics.cpp
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5455 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/cpp/metrics/Metrics.hpp
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/pybind/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2156 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/pybind/CMakeLists.txt
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3756 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/pybind/kiss_icp_pybind.cpp
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/pybind/pybind11/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1684 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/pybind/pybind11/LICENSE
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1358 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/pybind/pybind11/pybind11.cmake
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5753 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.1/src/pybind/stl_vector_eigen.h
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.460613 slam_dataset_sdk-0.0.1/src/python/
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1189 2023-01-13 17:35:35.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/__init__.py
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/config/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      604 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/config/advanced.yaml
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      283 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/config/default.yaml
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2431 2023-01-13 17:35:43.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/config.py
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2605 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/__init__.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2761 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/apollo.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3698 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/boreas.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4200 2023-01-13 19:30:24.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/generic.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4397 2023-01-13 19:25:19.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/kitti.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)    16202 2023-01-13 19:30:27.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/kitti_raw.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4379 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/mulran.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2126 2023-02-08 19:05:33.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/mydataset.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4276 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/ncd.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5254 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/nclt.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5667 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/nuscenes.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5180 2023-02-08 19:15:24.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/oxford.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2896 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/paris_luco.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3429 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/rosbag.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     7379 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/rosbag2.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3510 2023-02-08 18:13:31.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets_iterator.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2360 2023-01-13 17:47:08.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/deskew.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3170 2023-01-13 17:48:12.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/mapping.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1827 2023-01-13 17:48:25.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/metrics.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5552 2023-01-13 17:48:35.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/odometry.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     7413 2023-01-13 17:48:43.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/pipeline.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1794 2023-01-13 17:48:51.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/preprocess.py
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1166 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/__init__.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     6191 2023-01-13 19:30:53.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/cmd.py
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 17:55:34.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/__init__.py
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/extrinsics/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:13:28.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/extrinsics/__init__.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     8854 2023-02-08 18:14:14.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/interpolate_poses.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5322 2022-12-09 20:57:55.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/transform.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5556 2022-12-09 20:57:55.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/velodyne.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3082 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/pipeline_results.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1319 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/progress_bar.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     9045 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/visualizer.py
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1435 2023-01-13 17:48:56.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/voxelization.py
-drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:21:22.464613 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk.egg-info/
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3645 2023-02-08 19:21:22.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2976 2023-02-08 19:21:22.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)        1 2023-02-08 19:21:22.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)       68 2023-02-08 19:21:22.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      144 2023-02-08 19:21:22.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk.egg-info/requires.txt
--rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)       17 2023-02-08 19:21:22.000000 slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.421675 slam_dataset_sdk-0.0.2/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1623 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/CMakeLists.txt
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1071 2023-02-08 19:17:27.000000 slam_dataset_sdk-0.0.2/LICENSE
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      214 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/MANIFEST.in
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3645 2023-05-30 23:02:36.421675 slam_dataset_sdk-0.0.2/PKG-INFO
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2534 2023-01-31 17:05:11.000000 slam_dataset_sdk-0.0.2/README.md
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      376 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/pyproject.toml
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      994 2023-05-30 23:02:36.421675 slam_dataset_sdk-0.0.2/setup.cfg
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4435 2023-05-30 22:59:43.000000 slam_dataset_sdk-0.0.2/setup.py
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.413675 slam_dataset_sdk-0.0.2/src/
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/cpp/
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/eigen/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      779 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/eigen/LICENSE
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1874 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/eigen/eigen.cmake
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2130 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/find_dependencies.cmake
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tbb/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)    11357 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tbb/LICENSE
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2285 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tbb/tbb.cmake
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tsl_robin/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1102 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tsl_robin/LICENSE
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1888 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tsl_robin/tsl_robin.cmake
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1666 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/CMakeLists.txt
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1759 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/CMakeLists.txt
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3013 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Deskew.cpp
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1918 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Deskew.hpp
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     6704 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Map.hpp
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2496 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Preprocessing.cpp
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1882 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Preprocessing.hpp
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4599 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Registration.cpp
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1950 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Registration.hpp
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4963 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/VoxelHashMap.cpp
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4128 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/VoxelHashMap.hpp
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/cpp/metrics/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1569 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/metrics/CMakeLists.txt
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3662 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/metrics/Metrics.cpp
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5455 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/cpp/metrics/Metrics.hpp
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/pybind/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2156 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/pybind/CMakeLists.txt
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3756 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/pybind/kiss_icp_pybind.cpp
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/pybind/pybind11/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1684 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/pybind/pybind11/LICENSE
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1358 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/pybind/pybind11/pybind11.cmake
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5753 2023-01-13 17:22:42.000000 slam_dataset_sdk-0.0.2/src/pybind/stl_vector_eigen.h
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.413675 slam_dataset_sdk-0.0.2/src/python/
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.417675 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1189 2023-01-13 17:35:35.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/__init__.py
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.421675 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/config/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      604 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/config/advanced.yaml
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      283 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/config/default.yaml
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2431 2023-01-13 17:35:43.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/config.py
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.421675 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2605 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/__init__.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2761 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/apollo.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3698 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/boreas.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4200 2023-01-13 19:30:24.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/generic.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5109 2023-05-30 22:30:49.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/kitti.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)    16202 2023-01-13 19:30:27.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/kitti_raw.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4379 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/mulran.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2126 2023-02-08 19:05:33.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/mydataset.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4276 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/ncd.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5254 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/nclt.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5667 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/nuscenes.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5180 2023-02-08 19:15:24.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/oxford.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2896 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/paris_luco.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3881 2023-05-30 22:31:14.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/rosbag.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     7379 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/rosbag2.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     4031 2023-05-30 22:31:56.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets_iterator.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2360 2023-01-13 17:47:08.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/deskew.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3170 2023-01-13 17:48:12.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/mapping.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1827 2023-01-13 17:48:25.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/metrics.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5552 2023-01-13 17:48:35.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/odometry.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     7413 2023-01-13 17:48:43.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/pipeline.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1794 2023-01-13 17:48:51.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/preprocess.py
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.421675 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1166 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/__init__.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     6191 2023-01-13 19:30:53.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/cmd.py
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.421675 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 17:55:34.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/__init__.py
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.421675 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/extrinsics/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-02-08 19:13:28.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/extrinsics/__init__.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     8854 2023-02-08 18:14:14.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/interpolate_poses.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5322 2022-12-09 20:57:55.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/transform.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     5556 2022-12-09 20:57:55.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/velodyne.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3082 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/pipeline_results.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1319 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/progress_bar.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     9045 2023-01-13 17:35:29.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/visualizer.py
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     1435 2023-01-13 17:48:56.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/voxelization.py
+drwxrwxr-x   0 pranayspeed  (1000) pranayspeed  (1000)        0 2023-05-30 23:02:36.421675 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk.egg-info/
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     3645 2023-05-30 23:02:36.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)     2976 2023-05-30 23:02:36.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)        1 2023-05-30 23:02:36.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)       68 2023-05-30 23:02:36.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)      144 2023-05-30 23:02:36.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk.egg-info/requires.txt
+-rw-rw-r--   0 pranayspeed  (1000) pranayspeed  (1000)       17 2023-05-30 23:02:36.000000 slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk.egg-info/top_level.txt
```

### Comparing `slam_dataset_sdk-0.0.1/CMakeLists.txt` & `slam_dataset_sdk-0.0.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/LICENSE` & `slam_dataset_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/PKG-INFO` & `slam_dataset_sdk-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slam_dataset_sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple 3D LiDAR-Odometry dataset loading pipeline
 Home-page: https://github.com/pranayspeed/slam_dataset_iterator
 Author: Pranay Meshram
 Author-email: pranaywa@buffalo.edu
 License: MIT
 Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix
```

### Comparing `slam_dataset_sdk-0.0.1/README.md` & `slam_dataset_sdk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/setup.cfg` & `slam_dataset_sdk-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slam_dataset_sdk
-version = 0.0.1
+version = 0.0.2
 author = Pranay Meshram
 author_email = pranaywa@buffalo.edu
 description = Simple 3D LiDAR-Odometry dataset loading pipeline
 long_description = file:README.md,
 long_description_content_type = text/markdown
 url = https://github.com/pranayspeed/slam_dataset_iterator
 license = MIT
```

### Comparing `slam_dataset_sdk-0.0.1/setup.py` & `slam_dataset_sdk-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 # SOFTWARE.
 import contextlib
 import os
 import shutil
 import sys
 
 from setuptools import find_packages
-from skbuild import setup
-
+#from skbuild import setup
 
+from setuptools import setup
 @contextlib.contextmanager
 def skbuild_isolated_context():
     """This hack should be removed soon: https://github.com/scikit-build/scikit-build/issues/755.
 
     For whatever reason, when building the package in isolated mode (PEP 517) the cmake and ninja
     dependencies (that are indeed installed by the build system)do not expose the binary paths.
     Internally scikit-build uses $PATH/cmake and $PATH/ninja to analyze if those tools are installed
```

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/3rdparty/eigen/LICENSE` & `slam_dataset_sdk-0.0.2/src/cpp/3rdparty/eigen/LICENSE`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/3rdparty/eigen/eigen.cmake` & `slam_dataset_sdk-0.0.2/src/cpp/3rdparty/eigen/eigen.cmake`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/3rdparty/find_dependencies.cmake` & `slam_dataset_sdk-0.0.2/src/cpp/3rdparty/find_dependencies.cmake`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tbb/LICENSE` & `slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tbb/LICENSE`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tbb/tbb.cmake` & `slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tbb/tbb.cmake`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tsl_robin/LICENSE` & `slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tsl_robin/LICENSE`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/3rdparty/tsl_robin/tsl_robin.cmake` & `slam_dataset_sdk-0.0.2/src/cpp/3rdparty/tsl_robin/tsl_robin.cmake`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/CMakeLists.txt` & `slam_dataset_sdk-0.0.2/src/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/CMakeLists.txt` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Deskew.cpp` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Deskew.cpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Deskew.hpp` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Deskew.hpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Map.hpp` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Map.hpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Preprocessing.cpp` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Preprocessing.cpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Preprocessing.hpp` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Preprocessing.hpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Registration.cpp` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Registration.cpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/Registration.hpp` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/Registration.hpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/VoxelHashMap.cpp` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/VoxelHashMap.cpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/kiss_icp/VoxelHashMap.hpp` & `slam_dataset_sdk-0.0.2/src/cpp/kiss_icp/VoxelHashMap.hpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/metrics/CMakeLists.txt` & `slam_dataset_sdk-0.0.2/src/cpp/metrics/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/metrics/Metrics.cpp` & `slam_dataset_sdk-0.0.2/src/cpp/metrics/Metrics.cpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/cpp/metrics/Metrics.hpp` & `slam_dataset_sdk-0.0.2/src/cpp/metrics/Metrics.hpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/pybind/CMakeLists.txt` & `slam_dataset_sdk-0.0.2/src/pybind/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/pybind/kiss_icp_pybind.cpp` & `slam_dataset_sdk-0.0.2/src/pybind/kiss_icp_pybind.cpp`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/pybind/pybind11/LICENSE` & `slam_dataset_sdk-0.0.2/src/pybind/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/pybind/pybind11/pybind11.cmake` & `slam_dataset_sdk-0.0.2/src/pybind/pybind11/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/pybind/stl_vector_eigen.h` & `slam_dataset_sdk-0.0.2/src/pybind/stl_vector_eigen.h`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/__init__.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/config/advanced.yaml` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/config/advanced.yaml`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/config.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/config.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/__init__.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/apollo.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/apollo.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/boreas.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/boreas.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/generic.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/generic.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/kitti.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/kitti.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,34 +31,57 @@
         self.sequence_id = str(int(sequence)).zfill(2)
         self.kitti_sequence_dir = os.path.join(data_dir, "sequences", self.sequence_id)
         self.velodyne_dir = os.path.join(self.kitti_sequence_dir, "velodyne/")
 
         self.scan_files = sorted(glob.glob(self.velodyne_dir + "*.bin"))
         self.calibration = self.read_calib_file(os.path.join(self.kitti_sequence_dir, "calib.txt"))
 
+        self.label_dir = os.path.join(self.kitti_sequence_dir, "labels/")
+        self.label_files = sorted(glob.glob(self.label_dir + "*.label"))
+
+        print(f"Found {len(self.label_files)} scans in {self.kitti_sequence_dir}")
+
         # Load GT Poses (if available)
         if sequence < 11:
             self.poses_fn = os.path.join(data_dir, f"poses/{self.sequence_id}.txt")
             self.gt_poses = self.load_poses(self.poses_fn)
 
+
+
         # Add correction for KITTI datasets, can be easilty removed if unwanted
         from slam_dataset_sdk.pybind import kiss_icp_pybind
 
         self.correct_kitti_scan = lambda frame: np.asarray(
             kiss_icp_pybind._correct_kitti_scan(kiss_icp_pybind._Vector3dVector(frame))
         )
 
+        
+        
+
+
+    def open_label(self, label_file):
+        # if all goes well, open label
+        label = np.fromfile(label_file, dtype=np.uint32)
+        label = label.reshape((-1))
+        sem_label = label & 0xFFFF  # semantic label in lower half
+        inst_label = label >> 16    # instance id in upper half
+
+        return sem_label, inst_label#, label
+
     def __getitem__(self, idx):
-        return self.scans(idx)
+        return self.scans(idx), self.labels(idx)
 
     def __len__(self):
         return len(self.scan_files)
 
     def scans(self, idx):
         return self.read_point_cloud(self.scan_files[idx])
+    
+    def labels(self, idx):
+        return self.open_label(self.label_files[idx])
 
     def apply_calibration(self, poses: np.ndarray) -> np.ndarray:
         """Converts from Velodyne to Camera Frame"""
         Tr = np.eye(4, dtype=np.float64)
         Tr[:3, :4] = self.calibration["Tr"].reshape(3, 4)
         return Tr @ poses @ np.linalg.inv(Tr)
 
@@ -81,14 +104,16 @@
         n = poses.shape[0]
         poses = np.concatenate(
             (poses, np.zeros((n, 3), dtype=np.float32), np.ones((n, 1), dtype=np.float32)), axis=1
         )
         poses = poses.reshape((n, 4, 4))  # [N, 4, 4]
         return _lidar_pose_gt(poses)
 
+    
+
     @staticmethod
     def read_calib_file(file_path: str) -> dict:
         calib_dict = {}
         with open(file_path, "r") as calib_file:
             for line in calib_file.readlines():
                 tokens = line.split(" ")
                 if tokens[0] == "calib_time:":
```

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/kitti_raw.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/kitti_raw.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/mulran.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/mulran.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/mydataset.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/mydataset.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/ncd.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/ncd.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/nclt.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/nclt.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/nuscenes.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/nuscenes.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/oxford.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/oxford.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/paris_luco.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/paris_luco.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/rosbag.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/rosbag.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,36 +24,44 @@
 import os
 from pathlib import Path
 import sys
 
 import numpy as np
 import yaml
 
-
 class RosbagDataset:
-    def __init__(self, data_dir: Path, topic: str, *_, **__):
+    def __init__(self, data_dir: Path, *_, **kwargs):
         try:
             import rosbag
         except ModuleNotFoundError:
             print('python rosbag is not installed, run "sudo apt install python3-rosbag"')
             sys.exit(1)
 
         self.pc2 = importlib.import_module("sensor_msgs.point_cloud2")
         self.sequence_id = os.path.basename(data_dir).split(".")[0]
 
         # bagfile
+        if data_dir[-1]=='/':
+            data_dir = data_dir[:-1]
         self.bagfile = data_dir
+        print(f"Opening {self.bagfile}")
         self.bag = rosbag.Bag(data_dir, mode="r")
+        #topic = "sensor_msgs/PointCloud2"
+        #topic = "/ouster/points"
+        topic = kwargs.get("topic", "")
         self.topic = topic
         self.check_for_topics()
 
         # Get an iterable
         self.n_scans = self.bag.get_message_count(topic_filters=topic)
         self.msgs = self.bag.read_messages(topics=[topic])
 
+        self.gt_poses = np.zeros((self.n_scans, 4, 4))
+        print(self.n_scans, "scans in the bagfile")
+        
         # Visualization Options
         self.use_global_visualizer = True
 
     def __del__(self):
         self.bag.close()
 
     def __len__(self):
@@ -61,29 +69,32 @@
 
     def __getitem__(self, idx):
         return self.read_point_cloud(self.bagfile, self.topic, idx)
 
     def read_point_cloud(self, bagfile: Path, topic: str, idx: int):
         # TODO: implemnt [idx], expose field_names
         _, msg, _ = next(self.msgs)
+        print("read msg", msg.header.stamp)
         points = np.array(list(self.pc2.read_points(msg, field_names=["x", "y", "z"])))
 
         t_field = None
         for field in msg.fields:
             if field.name == "t" or field.name == "timestamp":
                 t_field = field.name
         timestamps = np.ones(points.shape[0])
         if t_field:
             timestamps = np.array(list(self.pc2.read_points(msg, field_names=t_field)))
             timestamps = timestamps / np.max(timestamps)
-        return points.astype(np.float64), timestamps
+        return points.astype(np.float64)#, timestamps
 
     def check_for_topics(self):
+        print("Checking for topics...")
         if self.topic:
             return
+        print("No topic provided")
         print("Please provide one of the following topics with the --topic flag")
         info_dict = yaml.safe_load(self.bag._get_yaml_info())
         info_dict.keys()
         print("PointCloud2 topics available:")
         for topic in info_dict["topics"]:
             if topic["type"] == "sensor_msgs/PointCloud2":
                 for k, v in topic.items():
```

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets/rosbag2.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets/rosbag2.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/datasets_iterator.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/datasets_iterator.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,35 +49,47 @@
 def get_dataset_subdir(dataset_name, sequence):
     sub_dir = dataset_name_to_subdir_map[dataset_name]
     if dataset_name == "paris_luco":
         sub_dir = os.path.join(sub_dir, f"{sequence:02d}")
     return sub_dir
 
 
-def dataset_itr(root_path, dataset_name, sequence):    
+def dataset_itr(root_path, dataset_name, sequence, topic="/ouster/points"):    
     dataset_root = os.path.join(root_path, get_dataset_subdir(dataset_name, sequence))
     cfg_file = os.path.join(os.path.dirname(slam_dataset_sdk.__file__), "config/default.yaml")
     def dataset_sequence_pipeline(sequence: int):
         return OdometryPipeline(
             dataset = dataset_factory(
                 dataloader=dataset_name,
                 data_dir=dataset_root,
                 config=cfg_file,
                 sequence=sequence,
+                topic=topic,
             ),
             config=cfg_file,
         )
 
     results = {}
     for raw_frame_timestamp, gt_pose in get_sequence(dataset_sequence_pipeline, sequence=sequence, results=results):
-        data = {
-            "raw_frame": raw_frame_timestamp[0],
-            "timestamp": raw_frame_timestamp[1],
-            "gt_pose": gt_pose
-        }
+
+        #print(raw_frame_timestamp[0].shape, len(raw_frame_timestamp[1]), gt_pose.shape)
+        if len(raw_frame_timestamp[1])==2:
+            data = {
+                "raw_frame": raw_frame_timestamp[0],
+                "sem_label": raw_frame_timestamp[1][0],
+                "inst_label": raw_frame_timestamp[1][1],
+                #"label": raw_frame_timestamp[1][2],
+                "gt_pose": gt_pose
+            }            
+        else:
+            data = {
+                "raw_frame": raw_frame_timestamp[0],
+                "timestamp": raw_frame_timestamp[1],
+                "gt_pose": gt_pose
+            }
         yield data
 
 
 def get_supported_datasets():
     return dataset_name_to_subdir_map.keys()
 
 # data_root = "/run/user/1000/gvfs/smb-share:server=10.84.164.159,share=datasets" #os.environ.get("DATASETS")
```

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/deskew.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/deskew.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/mapping.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/mapping.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/metrics.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/odometry.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/odometry.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/pipeline.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/pipeline.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/preprocess.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/preprocess.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/__init__.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/cmd.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/cmd.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/interpolate_poses.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/interpolate_poses.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/transform.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/transform.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/oxford_sdk/velodyne.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/oxford_sdk/velodyne.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/pipeline_results.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/pipeline_results.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/progress_bar.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/tools/visualizer.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/tools/visualizer.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk/voxelization.py` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk/voxelization.py`

 * *Files identical despite different names*

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk.egg-info/PKG-INFO` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slam-dataset-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple 3D LiDAR-Odometry dataset loading pipeline
 Home-page: https://github.com/pranayspeed/slam_dataset_iterator
 Author: Pranay Meshram
 Author-email: pranaywa@buffalo.edu
 License: MIT
 Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix
```

### Comparing `slam_dataset_sdk-0.0.1/src/python/slam_dataset_sdk.egg-info/SOURCES.txt` & `slam_dataset_sdk-0.0.2/src/python/slam_dataset_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

