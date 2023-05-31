# Comparing `tmp/ugot-0.1.3.tar.gz` & `tmp/ugot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugot-0.1.3.tar", last modified: Tue May 30 02:55:46 2023, max compression
+gzip compressed data, was "ugot-0.1.4.tar", last modified: Wed May 31 07:12:08 2023, max compression
```

## Comparing `ugot-0.1.3.tar` & `ugot-0.1.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.218756 ugot-0.1.3/
--rw-r--r--   0 jesse      (501) staff       (20)     1103 2023-05-15 09:14:27.000000 ugot-0.1.3/LICENSE
--rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-30 02:55:46.218298 ugot-0.1.3/PKG-INFO
--rwxrwxrwx   0 jesse      (501) staff       (20)      246 2023-05-11 07:07:58.000000 ugot-0.1.3/README.md
--rwxrwxrwx   0 jesse      (501) staff       (20)      425 2023-05-30 02:54:52.000000 ugot-0.1.3/pyproject.toml
--rw-r--r--   0 jesse      (501) staff       (20)       38 2023-05-30 02:55:46.218888 ugot-0.1.3/setup.cfg
--rwxrwxrwx   0 jesse      (501) staff       (20)      558 2023-05-30 02:54:52.000000 ugot-0.1.3/setup.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.055563 ugot-0.1.3/ugot/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:37:21.000000 ugot-0.1.3/ugot/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.182883 ugot-0.1.3/ugot/grpc_pb/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/grpc_pb/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     6021 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/audio_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    23990 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/audio_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6234 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/bluetooth_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    18284 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/bluetooth_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     9603 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/device_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    30498 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/device_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6103 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/gpio_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    18277 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/gpio_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     8843 2023-05-29 08:59:43.000000 ugot-0.1.3/ugot/grpc_pb/model_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    23309 2023-05-29 08:59:43.000000 ugot-0.1.3/ugot/grpc_pb/model_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6803 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/network_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    24828 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/network_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     2135 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/power_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)     5561 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/power_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     5080 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/sensor_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    13911 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/sensor_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)    10875 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/servo_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    24766 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/servo_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     5891 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/vision_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    16618 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/vision_pb2_grpc.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.183664 ugot-0.1.3/ugot/protos/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/protos/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.207967 ugot-0.1.3/ugot/src/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     2674 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/audio_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      517 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/base_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      615 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/bluetooth_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     4159 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/device_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     5085 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/enum.py
--rw-r--r--   0 jesse      (501) staff       (20)     3089 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/gpio_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     8210 2023-05-29 08:59:43.000000 ugot-0.1.3/ugot/src/model_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     5566 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/network_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      592 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/power_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     2031 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/scan_device.py
--rw-r--r--   0 jesse      (501) staff       (20)     1108 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/sensor_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     2291 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/servo_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     4110 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/util.py
--rw-r--r--   0 jesse      (501) staff       (20)    12490 2023-05-19 07:22:40.000000 ugot-0.1.3/ugot/src/vision_client.py
--rw-r--r--   0 jesse      (501) staff       (20)    87110 2023-05-30 02:38:47.000000 ugot-0.1.3/ugot/ugot.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.057609 ugot-0.1.3/ugot.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     1206 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)       67 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)        5 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/top_level.txt
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:08.049381 ugot-0.1.4/
+-rw-r--r--   0 jesse      (501) staff       (20)     1103 2023-05-15 09:14:27.000000 ugot-0.1.4/LICENSE
+-rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-31 07:12:08.049002 ugot-0.1.4/PKG-INFO
+-rwxrwxrwx   0 jesse      (501) staff       (20)      246 2023-05-11 07:07:58.000000 ugot-0.1.4/README.md
+-rwxrwxrwx   0 jesse      (501) staff       (20)      425 2023-05-31 07:09:42.000000 ugot-0.1.4/pyproject.toml
+-rw-r--r--   0 jesse      (501) staff       (20)       38 2023-05-31 07:12:08.049494 ugot-0.1.4/setup.cfg
+-rwxrwxrwx   0 jesse      (501) staff       (20)      558 2023-05-31 07:09:47.000000 ugot-0.1.4/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:07.953365 ugot-0.1.4/ugot/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:37:21.000000 ugot-0.1.4/ugot/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:08.011757 ugot-0.1.4/ugot/grpc_pb/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/grpc_pb/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6021 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/audio_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    23990 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/audio_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6234 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/bluetooth_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    18284 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/bluetooth_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     9603 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/device_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    30498 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/device_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6103 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/gpio_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    18277 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/gpio_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     8843 2023-05-29 08:59:43.000000 ugot-0.1.4/ugot/grpc_pb/model_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    23309 2023-05-29 08:59:43.000000 ugot-0.1.4/ugot/grpc_pb/model_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6803 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/network_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    24828 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/network_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2135 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/power_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5561 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/power_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5080 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/sensor_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    13911 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/sensor_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)    10875 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/servo_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    24766 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/servo_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5891 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/vision_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    16618 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/vision_pb2_grpc.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:08.012426 ugot-0.1.4/ugot/protos/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/protos/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:08.039053 ugot-0.1.4/ugot/src/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2674 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/audio_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      517 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/base_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      615 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/bluetooth_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4159 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/device_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5085 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/enum.py
+-rw-r--r--   0 jesse      (501) staff       (20)     3089 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/gpio_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     8210 2023-05-29 08:59:43.000000 ugot-0.1.4/ugot/src/model_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5566 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/network_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      592 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/power_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2245 2023-05-31 07:06:58.000000 ugot-0.1.4/ugot/src/scan_device.py
+-rw-r--r--   0 jesse      (501) staff       (20)     1108 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/sensor_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2291 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/servo_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4110 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/util.py
+-rw-r--r--   0 jesse      (501) staff       (20)    12490 2023-05-19 07:22:40.000000 ugot-0.1.4/ugot/src/vision_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)    87205 2023-05-31 07:06:58.000000 ugot-0.1.4/ugot/ugot.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:07.956184 ugot-0.1.4/ugot.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)     1206 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)       67 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/requires.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        5 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/top_level.txt
```

### Comparing `ugot-0.1.3/LICENSE` & `ugot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/PKG-INFO` & `ugot-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugot
-Version: 0.1.3
+Version: 0.1.4
 Summary: ugot-Python SDK
 Author-email: Jesse <jesse.huang@ubtrobot.com>
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ugot-0.1.3/setup.py` & `ugot-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name = "ugot",
-    version = "0.1.3",
+    version = "0.1.4",
     description = "ugot-Python SDK",
     long_description = "",
 
     packages = find_packages(include=["ugot","ugot.*"]),
     # package_data = {"ugot": ["*"],
     #                 },
     # packages=find_packages(),
```

### Comparing `ugot-0.1.3/ugot/grpc_pb/audio_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/audio_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/audio_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/audio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/bluetooth_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/bluetooth_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/bluetooth_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/bluetooth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/device_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/device_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/device_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/gpio_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/gpio_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/gpio_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/gpio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/model_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/model_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/model_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/network_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/network_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/network_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/network_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/power_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/power_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/power_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/power_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/sensor_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/sensor_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/sensor_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/sensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/servo_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/servo_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/servo_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/servo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/vision_pb2.py` & `ugot-0.1.4/ugot/grpc_pb/vision_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/grpc_pb/vision_pb2_grpc.py` & `ugot-0.1.4/ugot/grpc_pb/vision_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/audio_client.py` & `ugot-0.1.4/ugot/src/audio_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/base_client.py` & `ugot-0.1.4/ugot/src/base_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/bluetooth_client.py` & `ugot-0.1.4/ugot/src/bluetooth_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/device_client.py` & `ugot-0.1.4/ugot/src/device_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/enum.py` & `ugot-0.1.4/ugot/src/enum.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/gpio_client.py` & `ugot-0.1.4/ugot/src/gpio_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/model_client.py` & `ugot-0.1.4/ugot/src/model_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/network_client.py` & `ugot-0.1.4/ugot/src/network_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/power_client.py` & `ugot-0.1.4/ugot/src/power_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/scan_device.py` & `ugot-0.1.4/ugot/src/scan_device.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 from zeroconf import ServiceBrowser, ServiceListener, Zeroconf
 import socket
 import time
 
+DEV_LIST = {}
 
 class DeviceListener(ServiceListener):
-    #设备名称+IP列表
-    device_info = {}
-    #原始方法
+    def __init__(self):
+        #设备名称+IP列表
+        self.device_info = {}
     def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:
         #print(f"Service {name} updated")
         pass
     def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:
         #print(f"Service {name} removed")
         pass
     def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:
+        global DEV_LIST
         info = zc.get_service_info(type_, name)
         #print(f"Service {name} added, service info: {info}")
-        #print("name: ",info.name)
-        device_name = info.name.split(".")[0].split(":")
-        result_name = "UGOT_" + device_name[-2] + device_name[-1]
-        #print("device_name : ",result_name)
-        #print("ip: ",  socket.inet_ntoa(info.addresses[0]))
-        device_ip = socket.inet_ntoa(info.addresses[0])
-        self.device_info[result_name] = device_ip
+        if info:
+            device_name = info.name.split(".")[0].split(":")
+            result_name = "UGOT_" + device_name[-2] + device_name[-1]
+            #print("device_name : ",result_name)
+            if len(info.addresses)>0:
+                #print("ip: ",  socket.inet_ntoa(info.addresses[0]))
+                device_ip = socket.inet_ntoa(info.addresses[0])
+                self.device_info[result_name] = device_ip
+                DEV_LIST[result_name] = device_ip
 
 class DeviceScan:
-    listener = DeviceListener()
-    device_name_list=[]
-    device_info_list={}
+    def __init__(self):
+        self.listener = DeviceListener()
+        self.device_name_list=[]
+        self.device_info_list={}
     def device_discovery(self):
         zeroconf = Zeroconf()
         #当连接wifi的时候服务名不带usb
         browser = ServiceBrowser(zeroconf, "_uExplore_channel_server._tcp.local.", self.listener)
         #当连接usb调试线时候服务名带usb
         browser = ServiceBrowser(zeroconf, "_uExplore_channel_server_usb._tcp.local.", self.listener)
-        time.sleep(2)
+        time.sleep(3)
         zeroconf.close()
     def get_device_info_list(self):
         self.device_info_list = self.listener.device_info
         return self.device_info_list
     def get_device_name_list(self):
         for key in self.listener.device_info:
             self.device_name_list.append(key)
```

### Comparing `ugot-0.1.3/ugot/src/sensor_client.py` & `ugot-0.1.4/ugot/src/sensor_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/servo_client.py` & `ugot-0.1.4/ugot/src/servo_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/util.py` & `ugot-0.1.4/ugot/src/util.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/src/vision_client.py` & `ugot-0.1.4/ugot/src/vision_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.3/ugot/ugot.py` & `ugot-0.1.4/ugot/ugot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ugot.src.model_client import ModelClient
 from ugot.src.vision_client import VisionClient
 from ugot.src.util import num_normal, Color
 from ugot.src.enum import E_Model, E_Device, E_Vision, E_Audio
 from ugot.src.scan_device import DeviceScan
+from ugot.src.scan_device import DEV_LIST
 from ugot.src.device_client import DeviceClient
 from ugot.src.audio_client import AudioClient
 from ugot.src.sensor_client import SensorClient
 from ugot.src.network_client import NetworkClient
 from ugot.src.power_client import PowerClient
 from ugot.src.bluetooth_client import BlueToothClient
 from ugot.src.servo_client import ServoClient
@@ -18,31 +19,35 @@
 import time
 import sys
 
 class UGOT:
     def __init__(self):
         pass
 
+    def __scan(self):
+        self.SCAN = DeviceScan()
+        self.SCAN.device_discovery()
+
     def scan_device(self):
         """搜索扫描设备
 
         搜索获取同一局域网内的UGOT设备并打印.
 
         Args:
             无
 
         Returns:
             name_list (dict): 格式：{"设备名称1":"IP地址1","设备名称2":"IP地址2",...}
 
         """
-        self.SCAN = DeviceScan()
-        self.SCAN.device_discovery()
-        name_list = self.SCAN.get_device_info_list()
-        print(name_list)
-        return name_list
+        t = threading.Thread(target= self.__scan)
+        t.start()
+        t.join()
+        print(DEV_LIST)
+        return DEV_LIST
 
     def initialize(self, device_ip):
         """初始化设备
 
         通过IP地址初始化相关设备.
 
         Args:
```

### Comparing `ugot-0.1.3/ugot.egg-info/PKG-INFO` & `ugot-0.1.4/ugot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugot
-Version: 0.1.3
+Version: 0.1.4
 Summary: ugot-Python SDK
 Author-email: Jesse <jesse.huang@ubtrobot.com>
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ugot-0.1.3/ugot.egg-info/SOURCES.txt` & `ugot-0.1.4/ugot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

