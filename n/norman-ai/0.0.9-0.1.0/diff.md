# Comparing `tmp/norman_ai-0.0.9.tar.gz` & `tmp/norman_ai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "norman_ai-0.0.9.tar", last modified: Wed May 31 10:37:40 2023, max compression
+gzip compressed data, was "norman_ai-0.1.0.tar", last modified: Wed May 31 15:12:25 2023, max compression
```

## Comparing `norman_ai-0.0.9.tar` & `norman_ai-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 10:37:40.019447 norman_ai-0.0.9/
--rw-rw-rw-   0        0        0     7818 2023-05-16 12:28:05.000000 norman_ai-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0       43 2023-05-16 12:28:05.000000 norman_ai-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0    31935 2023-05-31 10:37:40.019951 norman_ai-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    31422 2023-05-31 10:26:05.000000 norman_ai-0.0.9/README.md
--rw-rw-rw-   0        0        0      108 2023-05-16 12:28:09.000000 norman_ai-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      688 2023-05-31 10:37:40.020998 norman_ai-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 10:37:39.998869 norman_ai-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 10:37:40.014629 norman_ai-0.0.9/src/norman_ai/
--rw-rw-rw-   0        0        0        0 2023-05-31 10:36:40.000000 norman_ai-0.0.9/src/norman_ai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:37:40.018113 norman_ai-0.0.9/src/norman_ai/data/
--rw-rw-rw-   0        0        0    31392 2023-05-16 12:28:09.000000 norman_ai-0.0.9/src/norman_ai/data/norman_model1.h5
--rw-rw-rw-   0        0        0    54035 2023-05-27 20:00:01.000000 norman_ai-0.0.9/src/norman_ai/norman_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:37:40.018113 norman_ai-0.0.9/src/norman_ai.egg-info/
--rw-rw-rw-   0        0        0    31935 2023-05-31 10:37:39.000000 norman_ai-0.0.9/src/norman_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-31 10:37:39.000000 norman_ai-0.0.9/src/norman_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 10:37:39.000000 norman_ai-0.0.9/src/norman_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-31 10:37:39.000000 norman_ai-0.0.9/src/norman_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 15:12:25.490819 norman_ai-0.1.0/
+-rw-rw-rw-   0        0        0     7818 2023-05-16 12:28:05.000000 norman_ai-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       43 2023-05-16 12:28:05.000000 norman_ai-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    31931 2023-05-31 15:12:25.492319 norman_ai-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    31418 2023-05-31 14:59:43.000000 norman_ai-0.1.0/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-16 12:28:09.000000 norman_ai-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      688 2023-05-31 15:12:25.493423 norman_ai-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 15:12:25.478232 norman_ai-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 15:12:25.485171 norman_ai-0.1.0/src/norman_ai/
+-rw-rw-rw-   0        0        0        0 2023-05-31 10:36:40.000000 norman_ai-0.1.0/src/norman_ai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:12:25.490819 norman_ai-0.1.0/src/norman_ai/data/
+-rw-rw-rw-   0        0        0    31392 2023-05-16 12:28:09.000000 norman_ai-0.1.0/src/norman_ai/data/norman_model1.h5
+-rw-rw-rw-   0        0        0    54035 2023-05-31 14:44:08.000000 norman_ai-0.1.0/src/norman_ai/norman_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:12:25.488803 norman_ai-0.1.0/src/norman_ai.egg-info/
+-rw-rw-rw-   0        0        0    31931 2023-05-31 15:12:25.000000 norman_ai-0.1.0/src/norman_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-31 15:12:25.000000 norman_ai-0.1.0/src/norman_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:12:25.000000 norman_ai-0.1.0/src/norman_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-31 15:12:25.000000 norman_ai-0.1.0/src/norman_ai.egg-info/top_level.txt
```

### Comparing `norman_ai-0.0.9/LICENSE.txt` & `norman_ai-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `norman_ai-0.0.9/PKG-INFO` & `norman_ai-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: norman_ai
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for automation of the novel object recognition test.
 Home-page: https://github.com/Seyij/norman
 Author: seyij_p
 Author-email: seyi.ooj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -198,15 +198,15 @@
 
 Hold the "r" key to reset the drawing and hold the escape key to exit once the drawing is complete.
 
 ```python
 #if you wish to mark object locations yourself use draw_objects as true
 #hold r to reset the drawing
 #press escape to exit the window once the drawing is complete
-x = nf.norkid(video, poses, "left", draw_objects=True)
+x = nf.norkid(video, poses, "left", draw_obj=True)
 
 #show the discrimination index, the time spent with left object, time spent with right object
 print("DI:"+str(x.di)+", Time left:"+str(x.tl)+ ", Time right:"+ str(x.tr))
 
 #make an video visualisation of norman labelling the mouse video
 #this is optional as not every video result will need visualisation
 x.draw_vid()
```

### Comparing `norman_ai-0.0.9/README.md` & `norman_ai-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
 Hold the "r" key to reset the drawing and hold the escape key to exit once the drawing is complete.
 
 ```python
 #if you wish to mark object locations yourself use draw_objects as true
 #hold r to reset the drawing
 #press escape to exit the window once the drawing is complete
-x = nf.norkid(video, poses, "left", draw_objects=True)
+x = nf.norkid(video, poses, "left", draw_obj=True)
 
 #show the discrimination index, the time spent with left object, time spent with right object
 print("DI:"+str(x.di)+", Time left:"+str(x.tl)+ ", Time right:"+ str(x.tr))
 
 #make an video visualisation of norman labelling the mouse video
 #this is optional as not every video result will need visualisation
 x.draw_vid()
```

### Comparing `norman_ai-0.0.9/setup.cfg` & `norman_ai-0.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6f72 6d61 6e5f 6169 0d0a 7665   = norman_ai..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 390d 0a61  rsion = 0.0.9..a
+00000020: 7273 696f 6e20 3d20 302e 312e 300d 0a61  rsion = 0.1.0..a
 00000030: 7574 686f 7220 3d20 7365 7969 6a5f 700d  uthor = seyij_p.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7365 7969 2e6f 6f6a 4067 6d61 696c 2e63  seyi.ooj@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 4120 7061 636b 6167 6520 666f 7220  = A package for 
 00000080: 6175 746f 6d61 7469 6f6e 206f 6620 7468  automation of th
 00000090: 6520 6e6f 7665 6c20 6f62 6a65 6374 2072  e novel object r
```

### Comparing `norman_ai-0.0.9/src/norman_ai/data/norman_model1.h5` & `norman_ai-0.1.0/src/norman_ai/data/norman_model1.h5`

 * *Files identical despite different names*

### Comparing `norman_ai-0.0.9/src/norman_ai/norman_functions.py` & `norman_ai-0.1.0/src/norman_ai/norman_functions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1016,17 +1016,17 @@
     #the class takes in a video and the associated deeplabcut pose file for it
     def __init__(self, video, pose_file, no_loc, draw_obj=False, model_path="normal"):
         #have the name of the video as a string
         self.video_name = video
         #the median image is a frame from the video without the mouse 
         self.median_img = median_filt_video(video)
         # object locations are the output of the find objects funtion
-        if draw_obj==True:
-            self.object_locs, self.fo_img = find_objects(self.median_img, img_out = True)
         if draw_obj==False:
+            self.object_locs, self.fo_img = find_objects(self.median_img, img_out = True)
+        if draw_obj==True:
             x = draw_objects(self.median_img)
             self.object_locs, self.fo_img = find_objects(x, img_out = True)
         # use relative position
         self.relative_pos = rel_pos(pose_file, self.object_locs)
         #get labels produced by the classification by norman
         self.labels = label_vid(self.relative_pos, model_path)  
         #get the discrimination index, seconds spent with left or right, and fps
```

### Comparing `norman_ai-0.0.9/src/norman_ai.egg-info/PKG-INFO` & `norman_ai-0.1.0/src/norman_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: norman-ai
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for automation of the novel object recognition test.
 Home-page: https://github.com/Seyij/norman
 Author: seyij_p
 Author-email: seyi.ooj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -198,15 +198,15 @@
 
 Hold the "r" key to reset the drawing and hold the escape key to exit once the drawing is complete.
 
 ```python
 #if you wish to mark object locations yourself use draw_objects as true
 #hold r to reset the drawing
 #press escape to exit the window once the drawing is complete
-x = nf.norkid(video, poses, "left", draw_objects=True)
+x = nf.norkid(video, poses, "left", draw_obj=True)
 
 #show the discrimination index, the time spent with left object, time spent with right object
 print("DI:"+str(x.di)+", Time left:"+str(x.tl)+ ", Time right:"+ str(x.tr))
 
 #make an video visualisation of norman labelling the mouse video
 #this is optional as not every video result will need visualisation
 x.draw_vid()
```

