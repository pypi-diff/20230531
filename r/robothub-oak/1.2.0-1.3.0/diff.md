# Comparing `tmp/robothub_oak-1.2.0.tar.gz` & `tmp/robothub_oak-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub_oak-1.2.0.tar", last modified: Wed May 17 17:54:08 2023, max compression
+gzip compressed data, was "robothub_oak-1.3.0.tar", last modified: Wed May 31 11:10:23 2023, max compression
```

## Comparing `robothub_oak-1.2.0.tar` & `robothub_oak-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.436290 robothub_oak-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.436290 robothub_oak-1.2.0/src/robothub_oak/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/src/robothub_oak/components/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/imu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/stereo.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/device.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13297 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8584 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/src/robothub_oak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-17 17:54:08.000000 robothub_oak-1.2.0/src/robothub_oak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-17 17:54:08.000000 robothub_oak-1.2.0/src/robothub_oak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:54:08.000000 robothub_oak-1.2.0/src/robothub_oak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 17:54:08.000000 robothub_oak-1.2.0/src/robothub_oak.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/tests/test_hub_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:10:23.953551 robothub_oak-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-31 11:10:23.949551 robothub_oak-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:10:23.953551 robothub_oak-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:10:23.949551 robothub_oak-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:10:23.949551 robothub_oak-1.3.0/src/robothub_oak/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:10:23.949551 robothub_oak-1.3.0/src/robothub_oak/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/components/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/components/imu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/components/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/components/stereo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/components/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/device.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13522 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8584 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/src/robothub_oak/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:10:23.949551 robothub_oak-1.3.0/src/robothub_oak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-31 11:10:23.000000 robothub_oak-1.3.0/src/robothub_oak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 11:10:23.000000 robothub_oak-1.3.0/src/robothub_oak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:10:23.000000 robothub_oak-1.3.0/src/robothub_oak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 11:10:23.000000 robothub_oak-1.3.0/src/robothub_oak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:10:23.949551 robothub_oak-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/tests/test_hub_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:52.000000 robothub_oak-1.3.0/tests/test_manager.py
```

### Comparing `robothub_oak-1.2.0/LICENSE` & `robothub_oak-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/PKG-INFO` & `robothub_oak-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub_oak
-Version: 1.2.0
+Version: 1.3.0
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.2.0/README.md` & `robothub_oak-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/setup.py` & `robothub_oak-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = io.open('README.md', encoding='utf-8').read()
 
 setup(
     name='robothub_oak',
-    version='1.2.0',
+    version='1.3.0',
     description='RobotHub-OAK integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
     keywords='robothub robot hub connect agent depthai oak sdk',
     author='Luxonis',
```

### Comparing `robothub_oak-1.2.0/src/robothub_oak/callbacks.py` & `robothub_oak-1.3.0/src/robothub_oak/callbacks.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/src/robothub_oak/commands.py` & `robothub_oak-1.3.0/src/robothub_oak/commands.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/src/robothub_oak/components/camera.py` & `robothub_oak-1.3.0/src/robothub_oak/components/camera.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/src/robothub_oak/components/neural_network.py` & `robothub_oak-1.3.0/src/robothub_oak/components/neural_network.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/src/robothub_oak/components/stereo.py` & `robothub_oak-1.3.0/src/robothub_oak/components/stereo.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/src/robothub_oak/device.py` & `robothub_oak-1.3.0/src/robothub_oak/device.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/src/robothub_oak/hub_camera.py` & `robothub_oak-1.3.0/src/robothub_oak/hub_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import depthai
 import depthai as dai
 import depthai_sdk
 import robothub
 from depthai_sdk import OakCamera
 from depthai_sdk.components import CameraComponent, StereoComponent, NNComponent
 
+import robothub_oak
 from robothub_oak.callbacks import get_default_color_callback, get_default_nn_callback, get_default_depth_callback
 from robothub_oak.utils import try_or_default
 
 __all__ = ['HubCamera']
 
 
 class HubCamera:
@@ -47,15 +48,19 @@
         Initializes the OakCamera instance. Will try to initialize for 5 seconds before returning None.
 
         :return: OakCamera instance if successful, None otherwise.
         """
         start_time = time.time()
         while not self.stop_event.is_set():
             try:
-                camera = OakCamera(self.device_name, usb_speed=self.usb_speed, rotation=self.rotation)
+                camera = OakCamera(self.device_name, usb_speed=self.usb_speed,
+                                   rotation=self.rotation, replay=robothub_oak.REPLAY_PATH)
+                if camera.replay:
+                    camera.replay.set_loop(True)
+
                 self.available_sensors = camera.sensors
                 return camera
             except Exception:
                 if time.time() - start_time > 10:
                     break
 
                 self.stop_event.wait(1)
@@ -119,14 +124,15 @@
         :param right: Right camera component, optional.
         :return: Stereo component.
         """
         if not self.has_stereo:
             raise RuntimeError('Device does not have stereo cameras.')
 
         comp = self.oak_camera.create_stereo(resolution=resolution, fps=fps, left=left, right=right, encode='h264')
+        comp.set_colormap(dai.Colormap.STEREO_TURBO)
         return comp
 
     def create_stream(self,
                       component: Union[CameraComponent, NNComponent, StereoComponent],
                       unique_key: str,
                       name: str,
                       callback: Callable = None
```

### Comparing `robothub_oak-1.2.0/src/robothub_oak/manager.py` & `robothub_oak-1.3.0/src/robothub_oak/manager.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/src/robothub_oak/packets.py` & `robothub_oak-1.3.0/src/robothub_oak/packets.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/src/robothub_oak/utils.py` & `robothub_oak-1.3.0/src/robothub_oak/utils.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.2.0/src/robothub_oak.egg-info/PKG-INFO` & `robothub_oak-1.3.0/src/robothub_oak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub-oak
-Version: 1.2.0
+Version: 1.3.0
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.2.0/src/robothub_oak.egg-info/SOURCES.txt` & `robothub_oak-1.3.0/src/robothub_oak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

