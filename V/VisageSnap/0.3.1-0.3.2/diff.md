# Comparing `tmp/VisageSnap-0.3.1.tar.gz` & `tmp/VisageSnap-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisageSnap-0.3.1.tar", last modified: Tue May 30 06:14:08 2023, max compression
+gzip compressed data, was "VisageSnap-0.3.2.tar", last modified: Wed May 31 03:02:48 2023, max compression
```

## Comparing `VisageSnap-0.3.1.tar` & `VisageSnap-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.971130 VisageSnap-0.3.1/VisageSnap/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.971130 VisageSnap-0.3.1/VisageSnap/image/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/image/imageloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.971130 VisageSnap-0.3.1/VisageSnap/model/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/model/modelhandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/VisageSnap/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/processor/faceprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/processor/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/processor/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.971130 VisageSnap-0.3.1/VisageSnap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:02:48.759060 VisageSnap-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-31 03:02:48.759060 VisageSnap-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:02:48.759060 VisageSnap-0.3.2/VisageSnap/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:02:48.759060 VisageSnap-0.3.2/VisageSnap/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/image/imageloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:02:48.759060 VisageSnap-0.3.2/VisageSnap/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/model/modelhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:02:48.759060 VisageSnap-0.3.2/VisageSnap/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/processor/faceprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/processor/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/processor/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/VisageSnap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:02:48.759060 VisageSnap-0.3.2/VisageSnap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-31 03:02:48.000000 VisageSnap-0.3.2/VisageSnap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-31 03:02:48.000000 VisageSnap-0.3.2/VisageSnap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 03:02:48.000000 VisageSnap-0.3.2/VisageSnap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 03:02:48.000000 VisageSnap-0.3.2/VisageSnap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 03:02:48.000000 VisageSnap-0.3.2/VisageSnap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 03:02:48.759060 VisageSnap-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:02:48.759060 VisageSnap-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-31 03:02:37.000000 VisageSnap-0.3.2/tests/test.py
```

### Comparing `VisageSnap-0.3.1/LICENSE` & `VisageSnap-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/PKG-INFO` & `VisageSnap-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisageSnap
-Version: 0.3.1
+Version: 0.3.2
 Summary: Face Classification package
 Home-page: https://github.com/asheswook/VisageSnap
 Author: Jaewook Lee
 Author-email: me@jwlee.xyz
 Project-URL: Bug Tracker, https://github.com/asheswook/VisageSnap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VisageSnap-0.3.1/README.md` & `VisageSnap-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/VisageSnap/classes.py` & `VisageSnap-0.3.2/VisageSnap/classes.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/VisageSnap/image/imageloader.py` & `VisageSnap-0.3.2/VisageSnap/image/imageloader.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/VisageSnap/main.py` & `VisageSnap-0.3.2/VisageSnap/main.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/VisageSnap/model/modelhandler.py` & `VisageSnap-0.3.2/VisageSnap/model/modelhandler.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/VisageSnap/processor/faceprocessor.py` & `VisageSnap-0.3.2/VisageSnap/processor/faceprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ..classes import Face, GlobalState, From, To, As
 from typing import Generator, Union
 import logging
 
 logger = logging.getLogger(__name__)
 
+
 class FaceProcessor:
     def __init__(self, globalState: GlobalState):
         self.__state = globalState
 
     def gen_faces(self) -> Generator[Face, None, None]:
         for face in self.__state.faces:
             yield face
@@ -74,18 +75,22 @@
         ----------
         target:
             - "From.LABEL" : label of the face object. (name of the person)
             - "From.FILENAME" : filename of the face object.
 
         value (str) : value of the target.
         """
-        assert isinstance(target, str), "target must be 'From.LABEL' or 'From.FILENAME'."
+        assert isinstance(
+            target, str), "target must be 'From.LABEL' or 'From.FILENAME'."
         assert isinstance(value, str), "value must be a string."
 
         for face in self.gen_faces():
             if target == "Label":
                 if face.label == value:
                     return face
             elif target == "Filename":
                 if value in face.filenames:
                     return face
-        return None
+        return None
+    
+    def get_faces(self) -> list[Face]:
+        return self.__state.faces
```

### Comparing `VisageSnap-0.3.1/VisageSnap/processor/predictor.py` & `VisageSnap-0.3.2/VisageSnap/processor/predictor.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/VisageSnap/processor/trainer.py` & `VisageSnap-0.3.2/VisageSnap/processor/trainer.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/VisageSnap/utils.py` & `VisageSnap-0.3.2/VisageSnap/utils.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/VisageSnap.egg-info/PKG-INFO` & `VisageSnap-0.3.2/VisageSnap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisageSnap
-Version: 0.3.1
+Version: 0.3.2
 Summary: Face Classification package
 Home-page: https://github.com/asheswook/VisageSnap
 Author: Jaewook Lee
 Author-email: me@jwlee.xyz
 Project-URL: Bug Tracker, https://github.com/asheswook/VisageSnap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VisageSnap-0.3.1/VisageSnap.egg-info/SOURCES.txt` & `VisageSnap-0.3.2/VisageSnap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.1/setup.py` & `VisageSnap-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'scikit-learn',
     'dlib',
     'face_recognition',
 ]
 
 setuptools.setup(
     name='VisageSnap',
-    version='0.3.1',
+    version='0.3.2',
     author='Jaewook Lee',
     author_email='me@jwlee.xyz',
     description='Face Classification package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/asheswook/VisageSnap',
     project_urls={
```

