# Comparing `tmp/cv2box-0.5.0.tar.gz` & `tmp/cv2box-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cv2box-0.5.0.tar", last modified: Sat Mar 18 08:54:43 2023, max compression
+gzip compressed data, was "cv2box-0.5.2.tar", last modified: Wed May 31 08:22:03 2023, max compression
```

## Comparing `cv2box-0.5.0.tar` & `cv2box-0.5.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2480 2023-03-18 08:54:43.000000 cv2box-0.5.0/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1961 2023-02-22 05:57:33.000000 cv2box-0.5.0/README.md
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      527 2023-03-18 08:53:47.000000 cv2box-0.5.0/cv2box/__init__.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box/cv_gears/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      616 2023-02-01 05:51:54.000000 cv2box-0.5.0/cv2box/cv_gears/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      946 2022-11-10 06:54:32.000000 cv2box-0.5.0/cv2box/cv_gears/concurrent_wrapper.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     7736 2022-08-18 08:30:30.000000 cv2box-0.5.0/cv2box/cv_gears/cv_multi_video_thread.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     7186 2023-02-21 05:56:55.000000 cv2box-0.5.0/cv2box/cv_gears/cv_threads_base.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5914 2023-02-22 06:10:39.000000 cv2box-0.5.0/cv2box/cv_gears/cv_video_thread.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1454 2022-08-23 08:57:26.000000 cv2box-0.5.0/cv2box/cv_gears/keyboard_listener_thread.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box/cv_gears/vidgear/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       29 2022-08-16 03:29:17.000000 cv2box-0.5.0/cv2box/cv_gears/vidgear/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    12378 2022-08-18 03:23:12.000000 cv2box-0.5.0/cv2box/cv_gears/vidgear/camgear.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    40175 2022-08-18 03:23:12.000000 cv2box-0.5.0/cv2box/cv_gears/vidgear/helper.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box/cv_ops/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      376 2022-08-15 06:07:56.000000 cv2box-0.5.0/cv2box/cv_ops/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4314 2022-08-15 09:06:48.000000 cv2box-0.5.0/cv2box/cv_ops/cv_bbox.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     9555 2022-09-08 06:00:09.000000 cv2box-0.5.0/cv2box/cv_ops/cv_camera.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1226 2022-07-15 07:11:53.000000 cv2box-0.5.0/cv2box/cv_ops/cv_excel.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4491 2023-01-31 01:41:48.000000 cv2box-0.5.0/cv2box/cv_ops/cv_file.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3750 2022-10-11 06:02:36.000000 cv2box-0.5.0/cv2box/cv_ops/cv_folder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    15154 2023-02-21 05:59:43.000000 cv2box-0.5.0/cv2box/cv_ops/cv_image.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6410 2022-10-14 10:13:09.000000 cv2box-0.5.0/cv2box/cv_ops/cv_queue.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6655 2022-08-23 08:55:19.000000 cv2box-0.5.0/cv2box/cv_ops/cv_rotate.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    15409 2023-03-18 08:52:28.000000 cv2box-0.5.0/cv2box/cv_ops/cv_video.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box/utils/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      395 2023-01-28 09:31:57.000000 cv2box-0.5.0/cv2box/utils/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      418 2023-01-30 10:21:42.000000 cv2box-0.5.0/cv2box/utils/apscheduler.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box/utils/compress/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1082 2022-11-15 02:53:44.000000 cv2box-0.5.0/cv2box/utils/compress/cv_compress.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box/utils/encrypt/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      142 2022-11-15 03:03:24.000000 cv2box-0.5.0/cv2box/utils/encrypt/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3605 2022-11-15 03:02:08.000000 cv2box-0.5.0/cv2box/utils/encrypt/cv_encrypt.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box/utils/logging/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      189 2022-09-06 03:12:06.000000 cv2box-0.5.0/cv2box/utils/logging/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1571 2022-09-08 06:00:09.000000 cv2box-0.5.0/cv2box/utils/logging/cv_logging.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2925 2022-10-09 07:01:42.000000 cv2box-0.5.0/cv2box/utils/math.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3995 2023-01-29 08:41:58.000000 cv2box-0.5.0/cv2box/utils/util.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2480 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1041 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       72 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box.egg-info/requires.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-03-18 08:54:43.000000 cv2box-0.5.0/cv2box.egg-info/top_level.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       38 2023-03-18 08:54:43.000000 cv2box-0.5.0/setup.cfg
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1052 2023-03-18 08:54:33.000000 cv2box-0.5.0/setup.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.827289 cv2box-0.5.2/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2443 2023-05-31 08:22:03.827289 cv2box-0.5.2/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1961 2023-02-22 05:57:33.000000 cv2box-0.5.2/README.md
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.823289 cv2box-0.5.2/cv2box/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      527 2023-05-31 08:21:20.000000 cv2box-0.5.2/cv2box/__init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.823289 cv2box-0.5.2/cv2box/cv_gears/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      616 2023-02-01 05:51:54.000000 cv2box-0.5.2/cv2box/cv_gears/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      946 2022-11-10 06:54:32.000000 cv2box-0.5.2/cv2box/cv_gears/concurrent_wrapper.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7736 2022-08-18 08:30:30.000000 cv2box-0.5.2/cv2box/cv_gears/cv_multi_video_thread.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7186 2023-02-21 05:56:55.000000 cv2box-0.5.2/cv2box/cv_gears/cv_threads_base.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5914 2023-02-22 06:10:39.000000 cv2box-0.5.2/cv2box/cv_gears/cv_video_thread.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1454 2022-08-23 08:57:26.000000 cv2box-0.5.2/cv2box/cv_gears/keyboard_listener_thread.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.823289 cv2box-0.5.2/cv2box/cv_gears/vidgear/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       29 2022-08-16 03:29:17.000000 cv2box-0.5.2/cv2box/cv_gears/vidgear/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    12378 2022-08-18 03:23:12.000000 cv2box-0.5.2/cv2box/cv_gears/vidgear/camgear.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    40175 2022-08-18 03:23:12.000000 cv2box-0.5.2/cv2box/cv_gears/vidgear/helper.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.823289 cv2box-0.5.2/cv2box/cv_ops/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      376 2022-08-15 06:07:56.000000 cv2box-0.5.2/cv2box/cv_ops/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4421 2023-05-31 06:02:30.000000 cv2box-0.5.2/cv2box/cv_ops/cv_bbox.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     9555 2022-09-08 06:00:09.000000 cv2box-0.5.2/cv2box/cv_ops/cv_camera.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1226 2022-07-15 07:11:53.000000 cv2box-0.5.2/cv2box/cv_ops/cv_excel.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4535 2023-04-19 07:03:38.000000 cv2box-0.5.2/cv2box/cv_ops/cv_file.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3750 2022-10-11 06:02:36.000000 cv2box-0.5.2/cv2box/cv_ops/cv_folder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    15302 2023-05-31 03:21:34.000000 cv2box-0.5.2/cv2box/cv_ops/cv_image.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6410 2022-10-14 10:13:09.000000 cv2box-0.5.2/cv2box/cv_ops/cv_queue.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6655 2022-08-23 08:55:19.000000 cv2box-0.5.2/cv2box/cv_ops/cv_rotate.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    17639 2023-05-30 06:38:48.000000 cv2box-0.5.2/cv2box/cv_ops/cv_video.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.823289 cv2box-0.5.2/cv2box/utils/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      395 2023-03-31 06:22:53.000000 cv2box-0.5.2/cv2box/utils/__init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.827289 cv2box-0.5.2/cv2box/utils/compress/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1082 2022-11-15 02:53:44.000000 cv2box-0.5.2/cv2box/utils/compress/cv_compress.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.827289 cv2box-0.5.2/cv2box/utils/encrypt/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      142 2022-11-15 03:03:24.000000 cv2box-0.5.2/cv2box/utils/encrypt/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3609 2023-05-24 08:47:31.000000 cv2box-0.5.2/cv2box/utils/encrypt/cv_encrypt.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.827289 cv2box-0.5.2/cv2box/utils/logging/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      189 2022-09-06 03:12:06.000000 cv2box-0.5.2/cv2box/utils/logging/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1571 2022-09-08 06:00:09.000000 cv2box-0.5.2/cv2box/utils/logging/cv_logging.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3117 2023-05-31 08:20:59.000000 cv2box-0.5.2/cv2box/utils/math.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1426 2023-03-31 06:19:37.000000 cv2box-0.5.2/cv2box/utils/scheduler.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    27336 2023-05-19 09:23:21.000000 cv2box-0.5.2/cv2box/utils/send_notify.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4394 2023-03-29 07:46:27.000000 cv2box-0.5.2/cv2box/utils/util.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:22:03.823289 cv2box-0.5.2/cv2box.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2443 2023-05-31 08:22:03.000000 cv2box-0.5.2/cv2box.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1067 2023-05-31 08:22:03.000000 cv2box-0.5.2/cv2box.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-31 08:22:03.000000 cv2box-0.5.2/cv2box.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       72 2023-05-31 08:22:03.000000 cv2box-0.5.2/cv2box.egg-info/requires.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-05-31 08:22:03.000000 cv2box-0.5.2/cv2box.egg-info/top_level.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       38 2023-05-31 08:22:03.827289 cv2box-0.5.2/setup.cfg
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1052 2023-05-31 08:22:01.000000 cv2box-0.5.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cv2box-0.5.0/PKG-INFO` & `cv2box-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: cv2box
-Version: 0.5.0
+Version: 0.5.2
 Summary: cv toolbox
 Home-page: https://github.com/ykk648/cv2box
 Author: ykk648
 Author-email: ykk648@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ykk648/cv2box/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: light
 Provides-Extra: full
 
@@ -71,9 +69,7 @@
 ### utils
 
 - fps counter
 - apscheduler
 - math (cal distances
 
 ### AI power (moved to [AI_power](https://github.com/ykk648/AI_power))
-
-
```

### Comparing `cv2box-0.5.0/README.md` & `cv2box-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/__init__.py` & `cv2box-0.5.2/cv2box/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# VERSION 0.5.0
+# VERSION 0.5.2
 import os
 
 try:
     _ = os.environ['CV_LOG_LEVEL']
 except KeyError:
     os.environ['CV_LOG_LEVEL'] = 'info'
     from .utils import cv_print
```

### Comparing `cv2box-0.5.0/cv2box/cv_gears/__init__.py` & `cv2box-0.5.2/cv2box/cv_gears/__init__.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_gears/concurrent_wrapper.py` & `cv2box-0.5.2/cv2box/cv_gears/concurrent_wrapper.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_gears/cv_multi_video_thread.py` & `cv2box-0.5.2/cv2box/cv_gears/cv_multi_video_thread.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_gears/cv_threads_base.py` & `cv2box-0.5.2/cv2box/cv_gears/cv_threads_base.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_gears/cv_video_thread.py` & `cv2box-0.5.2/cv2box/cv_gears/cv_video_thread.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_gears/keyboard_listener_thread.py` & `cv2box-0.5.2/cv2box/cv_gears/keyboard_listener_thread.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_gears/vidgear/camgear.py` & `cv2box-0.5.2/cv2box/cv_gears/vidgear/camgear.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_gears/vidgear/helper.py` & `cv2box-0.5.2/cv2box/cv_gears/vidgear/helper.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_ops/cv_bbox.py` & `cv2box-0.5.2/cv2box/cv_ops/cv_bbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,40 +61,37 @@
             box_results.append(box_list_temp[aim_ind])
             box_list_temp.pop(aim_ind)
             box_dis_from_center.pop(aim_ind)
         return box_results
 
     def area_center_filter(self, image_shape, max_num=1):
         """
-
         Args:
-            image_shape: HWC
-            max_num:
-
-        Returns:
-
+            image_shape: HWC from origin full image
+            max_num: max number of bbox
+        Returns: new bbox list [[bbox, index], ...]
         """
         if len(self.bbox_array) == 0:
             return [[]]
         box_results = []
-        dummy1 = []
-        dummy2 = []
+        dummy1 = []  # center dis
+        dummy2 = []  # area
         if not isinstance(self.bbox_array, list):
             self.bbox_array = self.bbox_array.tolist()
         box_list_temp = self.bbox_array.copy()
         for box in box_list_temp:
             dummy1.append(CalDistance([box[0] + (box[2] - box[0]) / 2, box[1] + (box[3] - box[1]) / 2],
                                       [image_shape[1] / 2, image_shape[0] / 2]).euc())
             dummy2.append((box[2] - box[0]) * (box[3] - box[1]))
 
         box_area_dis = Normalize(dummy2).np_norm() - Normalize(dummy1).np_norm()
         for i in range(max_num):
             aim_ind = np.argmax(np.array(box_area_dis))
 
-            box_results.append(box_list_temp[aim_ind])
+            box_results.append([box_list_temp[aim_ind], aim_ind])
             box_list_temp.pop(aim_ind)
             box_area_dis.tolist().pop(aim_ind)
         return box_results
 
     @staticmethod
     def get_bbox_from_points(points_in_, image_shape, margin_ratio=0.8):
         """
```

### Comparing `cv2box-0.5.0/cv2box/cv_ops/cv_camera.py` & `cv2box-0.5.2/cv2box/cv_ops/cv_camera.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_ops/cv_excel.py` & `cv2box-0.5.2/cv2box/cv_ops/cv_excel.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_ops/cv_file.py` & `cv2box-0.5.2/cv2box/cv_ops/cv_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         if Path(self.file_path).exists():
             self.suffix = Path(self.file_path).suffix
             if self.suffix == '.pkl':
                 with open(file_path, 'rb') as f:
                     self.file_data = pickle.load(f)
             elif self.suffix == '.txt':
-                with open(file_path, 'rb') as f:
+                with open(file_path, encoding='utf-8', mode='r') as f:
                     self.file_data = f.readlines()
             elif self.suffix == '.json':
                 with open(file_path, 'rb') as f:
                     self.file_data = json.load(f)
             elif self.suffix == '.npz':
                 # h = arrays['key'][()]
                 self.file_data = np.load(file_path, allow_pickle=True)
@@ -89,16 +89,16 @@
             pickle.dump(data_in, f)
 
     def json_write(self, data_in):
         if isinstance(data_in, dict):
             for k, v in data_in.items():
                 if isinstance(v, np.bool_):
                     data_in[k] = bool(v)
-        with open(self.file_path, 'w', encoding='utf-8') as f:
-            json.dump(data_in, f)
+        with open(self.file_path, 'w', encoding='utf-8', ) as f:
+            json.dump(data_in, f, ensure_ascii=False)
 
     def json_update(self, data_in):
         with open(self.file_path, 'rb') as f:
             file_data = json.load(f)
         if isinstance(data_in, dict):
             for k, v in data_in.items():
                 if isinstance(v, np.bool_):
```

### Comparing `cv2box-0.5.0/cv2box/cv_ops/cv_folder.py` & `cv2box-0.5.2/cv2box/cv_ops/cv_folder.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_ops/cv_image.py` & `cv2box-0.5.2/cv2box/cv_ops/cv_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 
     def rgb(self):
         return cv2.cvtColor(self.cv_image, cv2.COLOR_BGR2RGB)
 
     def rgba(self):
         return cv2.cvtColor(self.cv_image, cv2.COLOR_BGR2RGBA)
 
+    def gray(self):
+        return cv2.cvtColor(self.cv_image, cv2.COLOR_BGR2GRAY)
+
     @property
     def bgr(self):
         return self.cv_image
 
     def pillow(self):
         Image = try_import('PIL.Image', 'cv_math: need pillow here.')
         return Image.fromarray(cv2.cvtColor(self.cv_image, cv2.COLOR_BGR2RGB))
@@ -353,14 +356,18 @@
             from ..utils.util import mat2mask
             from cv2box import MyFpsCounter
             # with MyFpsCounter() as mfs:
             img_fg_mask = mat2mask(img_bg, mat_rev)
         else:
             img_fg_mask = cv2.warpAffine(img_fg_mask, mat_rev, img_bg.shape[:2][::-1], borderMode=cv2.BORDER_REPLICATE)[
                 ..., np.newaxis]
+
+        # # clip
+        # img_fg_mask[img_fg_mask > 0.2] = 1
+
         local_dict = {
             'img_fg_mask': img_fg_mask,
             'img_fg_trans': img_fg_trans,
             'img_bg': img_bg,
         }
         img = ne.evaluate('img_fg_mask * (img_fg_trans * 255)+(1 - img_fg_mask) * img_bg', local_dict=local_dict,
                           global_dict=None)
```

### Comparing `cv2box-0.5.0/cv2box/cv_ops/cv_queue.py` & `cv2box-0.5.2/cv2box/cv_ops/cv_queue.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_ops/cv_rotate.py` & `cv2box-0.5.2/cv2box/cv_ops/cv_rotate.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/cv_ops/cv_video.py` & `cv2box-0.5.2/cv2box/cv_ops/cv_video.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,16 +36,17 @@
         frame_number = cap.get(cv2.CAP_PROP_FRAME_COUNT)  # 视频文件的帧数
         duration = frame_number / fps  # 帧速率/视频总帧数 是s
 
         size = (int(cap.get(cv2.CAP_PROP_FRAME_WIDTH)),
                 int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT)))
         cap.release()
         print(
-            'video info:\nname: {}\nfourcc: {}\nfps: {}\nsize: {}'.format(self.video_name, decode_fourcc(fourcc), fps,
-                                                                          size))
+            'video info:\nname: {}\nfourcc: {}\nframe_number: {}\nfps: {}\nsize: {}'.format(self.video_name,
+                                                                                            decode_fourcc(fourcc),
+                                                                                            frame_number, fps, size))
 
     def show_video_cv(self, delay=100):
         cap = cv2.VideoCapture(self.video_path)
         success = True
         while success:
             success, frame = cap.read()
             cv2.namedWindow("First Frame", 0)
@@ -96,25 +97,32 @@
         size_str = '{}:{}:{}:{}'.format(str(out_w), str(out_h), str(x), str(y))
         command = 'ffmpeg -y -i {} -filter:v "crop={}" -c:v {} -crf 17 -c:a copy {}.mp4'.format(self.video_path,
                                                                                                 size_str, format,
                                                                                                 self.video_dir + '/' + self.prefix + '_out')
         os_call(command)
 
     def cut_video(self, start, last_time, accurate=False):
+        """
+        :param start: start time(s)
+        :param last_time: video clip length(s)
+        :param accurate: using keyframe or not
+        :return:
+        """
         assert re.match(r"(\d{1,2}:\d{1,2}:\d{1,2})",
                         start) is not None, 'The time format: start:00:00:15 last_time:00:00:15 etc.'
         assert re.match(r"(\d{1,2}:\d{1,2}:\d{1,2})",
                         last_time) is not None, 'The time format: start:00:00:15 last_time:00:00:15 etc.'
+        cut_out_video_path = self.video_dir + '/' + self.prefix + '_cut_out.mp4'
         if not accurate:
-            command = 'ffmpeg -y -ss {} -t {} -i {} -codec copy {}.mp4'.format(start, last_time, self.video_path,
-                                                                               self.video_dir + '/' + self.prefix + '_cut_out')
+            command = 'ffmpeg -y -ss {} -t {} -i {} -codec copy {}'.format(start, last_time, self.video_path,
+                                                                           cut_out_video_path)
         else:
-            command = 'ffmpeg -y -ss {} -t {} -i {} {}.mp4'.format(start, last_time, self.video_path,
-                                                                   self.video_dir + '/' + self.prefix + '_cut_out')
+            command = 'ffmpeg -y -ss {} -t {} -i {} {}'.format(start, last_time, self.video_path, cut_out_video_path)
         os_call(command)
+        return cut_out_video_path
 
     def add_text(self, text, left_top_coord: tuple, fontsize=20):
 
         command = 'ffmpeg -i {} -vf drawtext="text={}:x={}:y={}:fontsize={}:fontcolor=white:box=1:boxcolor=blue" -y {}.mp4'.format(
             self.video_path, text, left_top_coord[0], left_top_coord[1], fontsize,
             self.video_dir + '/' + self.prefix + '_add_text_out')
         os_call(command)
@@ -203,14 +211,25 @@
         video_capture.release()
 
     def resize_video(self, out_size=(768, 1024), inplace=False):
         out_p = self.video_path.replace('.mp4', '_{}x{}.mp4'.format(out_size[0], out_size[1]))
         if inplace:
             shutil.move(self.video_path, out_p)
             self.video_path, out_p = out_p, self.video_path
+            # os.remove(self.video_path)
+        os_call(
+            f'ffmpeg -y -loglevel error -i {self.video_path} -s {out_size[0]}x{out_size[1]} -c:a copy {out_p}')
+        if inplace:
+            os.remove(self.video_path)
+
+    def resize_video_cv(self, out_size=(768, 1024), inplace=False):
+        out_p = self.video_path.replace('.mp4', '_{}x{}.mp4'.format(out_size[0], out_size[1]))
+        if inplace:
+            shutil.move(self.video_path, out_p)
+            self.video_path, out_p = out_p, self.video_path
 
         cap = cv2.VideoCapture(self.video_path)
         fps = cap.get(cv2.CAP_PROP_FPS)
 
         video_writer = cv2.VideoWriter(out_p, cv2.VideoWriter_fourcc(*'mp4v'), fps, out_size)
 
         while True:
@@ -285,17 +304,43 @@
 
         if copy_audio:
             os_call('ffmpeg -i {} -vn -codec copy {}'.format(self.video_path, './temp.m4a'))
             os_call("ffmpeg -i {} -i {} -vcodec copy -acodec copy {}".format(video_out_p, './temp.m4a',
                                                                              video_out_p.replace('_concat_out.mp4',
                                                                                                  '_concat_out_audio.mp4')))
             os_call('rm ./temp.m4a')
+            os_call(f'rm {video_out_p}')
 
         return video_out_p
 
+    def extract_audio(self, output_path=None):
+        if not output_path:
+            output_path = self.video_path.replace('.mp4', '_audio.wav')
+        os_call(f'ffmpeg -i {self.video_path} -vn -acodec pcm_s16le -ar 44100 -ac 2 {output_path}')
+
+    def copy_audio(self, audio_src):
+        """
+        support mp4 or wav
+        ffmpeg -hide_banner -i "input.mp4" -i "input1.wav" -i "input2.wav" -filter_complex "[1:a]volume=1.5[a1];[2:a]volume=1[a2];[a1][a2]amix=inputs=2:duration=first:dropout_transition=0" -c:v "libx264" -c:a 'aac' -y "mix.mp4"
+        :param audio_src:
+        :return:
+        """
+        # mod to mkv when met "Could not find tag for codec pcm_s24le in stream #1"
+        # output_path = self.video_path.replace('.mp4', '_audio_replaced.mkv')
+        output_path = self.video_path.replace('.mp4', '_audio_replaced.mp4')
+        if Path(audio_src).suffix == '.mp4':
+            audio_temp_path = audio_src.replace('.mp4', '_temp.mp4')
+            os_call(f'ffmpeg -i {audio_src} -vn -codec copy {audio_temp_path}')
+            os_call(
+                f'ffmpeg -i {self.video_path} -i {audio_temp_path} -vcodec copy -acodec copy -map 0:v:0 -map 1:a:0 {output_path}')
+            os.remove(audio_temp_path)
+        else:
+            os_call(
+                f'ffmpeg -i {self.video_path} -i {audio_src} -c copy -map 0:v -map 1:a -shortest {output_path}')
+
 
 class CVVideoLoader(object, ):
     """
     based on OpenCV
     """
 
     def __init__(self, video_p):
@@ -305,15 +350,15 @@
         self.cap = cv2.VideoCapture(self.video_p)
         self.fps = self.cap.get(cv2.CAP_PROP_FPS)
         self.size = (int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH)),
                      int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT)))
         self.frames_num = self.cap.get(7)
         codec = int(self.cap.get(cv2.CAP_PROP_FOURCC))
         self.codec = chr(codec & 0xFF) + chr((codec >> 8) & 0xFF) + chr((codec >> 16) & 0xFF) + chr(
-                (codec >> 24) & 0xFF)
+            (codec >> 24) & 0xFF)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.cap.release()
 
     def __len__(self):
         return int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT))
```

### Comparing `cv2box-0.5.0/cv2box/utils/compress/cv_compress.py` & `cv2box-0.5.2/cv2box/utils/compress/cv_compress.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/utils/encrypt/cv_encrypt.py` & `cv2box-0.5.2/cv2box/utils/encrypt/cv_encrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -- coding: utf-8 --
 # @Time : 2021/11/26
 # @Author : ykk648
 # @Project : https://github.com/ykk648/cv2box
 from ... import try_import
 
-AES = try_import('Crypto.Cipher', 'cv_encrypt need crypto: pip install pycryptodome')
+AES = try_import('Crypto.Cipher.AES', 'cv_encrypt need crypto: pip install pycryptodome')
 import operator
 import time
 from pathlib import Path
 
 AES_BLOCK_SIZE = AES.block_size  # AES 加密数据块大小, 只能是16
 AES_KEY_SIZE = 16  # AES 密钥长度（单位字节），可选 16、24、32，对应 128、192、256 位密钥
```

### Comparing `cv2box-0.5.0/cv2box/utils/logging/cv_logging.py` & `cv2box-0.5.2/cv2box/utils/logging/cv_logging.py`

 * *Files identical despite different names*

### Comparing `cv2box-0.5.0/cv2box/utils/math.py` & `cv2box-0.5.2/cv2box/utils/math.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,14 +72,19 @@
         :return:
         """
         norm = np.linalg.norm(self.aim_in)
         if norm == 0:
             return self.aim_in
         return self.aim_in / norm
 
+    def batch_norm(self, axis=-1, order=2):
+        l2 = np.atleast_1d(np.linalg.norm(self.aim_in, order, axis))
+        l2[l2 == 0] = 1
+        return self.aim_in / np.expand_dims(l2, axis)
+
     def torch_l2_norm(self, axis=1):
         torch = try_import('torch', 'cv_math: need torch here.')
         if not isinstance(self.aim_in, torch.tensor):
             self.aim_in = torch.tensor(self.aim_in)
         norm = torch.norm(self.aim_in, 2, axis, True)
         output = torch.div(self.aim_in, norm)
         return output
```

### Comparing `cv2box-0.5.0/cv2box/utils/util.py` & `cv2box-0.5.2/cv2box/utils/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from importlib import import_module
 import warnings
 import sys
 import numpy as np
 from .logging import cv_print
 import platform
 import cv2
+from io import StringIO
 
 
 def mat2mask(frame, mat):
     kernel_size = int(0.05 * min((frame.shape[1], frame.shape[0])))
 
     img_mask = np.full((frame.shape[0], frame.shape[1]), 255, dtype=float)
 
@@ -141,7 +142,22 @@
 
 
 def try_import(module_name, warn_message=None):
     try:
         return import_module(module_name)
     except Exception as e:
         cv_print('got exception: {}, {}'.format(e, warn_message), level='error')
+
+
+class OutCapture(list):
+    """
+    capture output to string
+    """
+    def __enter__(self):
+        self._stdout = sys.stdout
+        sys.stdout = self._stringio = StringIO()
+        return self
+
+    def __exit__(self, *args):
+        self.extend(self._stringio.getvalue().splitlines())
+        del self._stringio  # free up some memory
+        sys.stdout = self._stdout
```

### Comparing `cv2box-0.5.0/cv2box.egg-info/PKG-INFO` & `cv2box-0.5.2/cv2box.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: cv2box
-Version: 0.5.0
+Version: 0.5.2
 Summary: cv toolbox
 Home-page: https://github.com/ykk648/cv2box
 Author: ykk648
 Author-email: ykk648@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ykk648/cv2box/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: light
 Provides-Extra: full
 
@@ -71,9 +69,7 @@
 ### utils
 
 - fps counter
 - apscheduler
 - math (cal distances
 
 ### AI power (moved to [AI_power](https://github.com/ykk648/AI_power))
-
-
```

### Comparing `cv2box-0.5.0/cv2box.egg-info/SOURCES.txt` & `cv2box-0.5.2/cv2box.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 cv2box/cv_ops/cv_file.py
 cv2box/cv_ops/cv_folder.py
 cv2box/cv_ops/cv_image.py
 cv2box/cv_ops/cv_queue.py
 cv2box/cv_ops/cv_rotate.py
 cv2box/cv_ops/cv_video.py
 cv2box/utils/__init__.py
-cv2box/utils/apscheduler.py
 cv2box/utils/math.py
+cv2box/utils/scheduler.py
+cv2box/utils/send_notify.py
 cv2box/utils/util.py
 cv2box/utils/compress/cv_compress.py
 cv2box/utils/encrypt/__init__.py
 cv2box/utils/encrypt/cv_encrypt.py
 cv2box/utils/logging/__init__.py
 cv2box/utils/logging/cv_logging.py
```

### Comparing `cv2box-0.5.0/setup.py` & `cv2box-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='cv2box',  # 项目的名称
-    version='0.5.0',  # 项目版本
+    version='0.5.2',  # 项目版本
     author='ykk648',  # 项目作者
     author_email='ykk648@gmail.com',  # 作者email
     url='https://github.com/ykk648/cv2box',  # 项目代码仓库
     project_urls={
         "Bug Tracker": "https://github.com/ykk648/cv2box/issues",
     },
     description='cv toolbox',  # 项目描述
```

