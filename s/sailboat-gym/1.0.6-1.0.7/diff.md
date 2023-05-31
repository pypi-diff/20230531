# Comparing `tmp/sailboat-gym-1.0.6.tar.gz` & `tmp/sailboat-gym-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sailboat-gym-1.0.6.tar", last modified: Wed May 31 07:37:43 2023, max compression
+gzip compressed data, was "sailboat-gym-1.0.7.tar", last modified: Wed May 31 07:44:17 2023, max compression
```

## Comparing `sailboat-gym-1.0.6.tar` & `sailboat-gym-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:37:43.972480 sailboat-gym-1.0.6/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1074 2023-05-23 13:44:12.000000 sailboat-gym-1.0.6/LICENSE
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1480 2023-05-31 07:37:43.972102 sailboat-gym-1.0.6/PKG-INFO
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     5949 2023-05-31 06:34:03.000000 sailboat-gym-1.0.6/README.md
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:37:43.962147 sailboat-gym-1.0.6/sailboat_gym/
--rw-------   0 lucasmrdt   (501) staff       (20)      445 2023-05-31 07:35:45.000000 sailboat-gym-1.0.6/sailboat_gym/__init__.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:37:43.966914 sailboat-gym-1.0.6/sailboat_gym/envs/
--rw-------   0 lucasmrdt   (501) staff       (20)       41 2023-05-11 14:46:14.000000 sailboat-gym-1.0.6/sailboat_gym/envs/__init__.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      599 2023-05-11 15:47:26.000000 sailboat-gym-1.0.6/sailboat_gym/envs/env.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:37:43.970166 sailboat-gym-1.0.6/sailboat_gym/envs/sailboat_lsa/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       35 2023-05-11 14:43:54.000000 sailboat-gym-1.0.6/sailboat_gym/envs/sailboat_lsa/__init__.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     4054 2023-05-23 08:29:42.000000 sailboat-gym-1.0.6/sailboat_gym/envs/sailboat_lsa/lsa_env.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     7165 2023-05-23 08:33:00.000000 sailboat-gym-1.0.6/sailboat_gym/envs/sailboat_lsa/lsa_sim.py
--rw-------   0 lucasmrdt   (501) staff       (20)      699 2023-05-11 15:38:32.000000 sailboat-gym-1.0.6/sailboat_gym/interfaces.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:37:43.971660 sailboat-gym-1.0.6/sailboat_gym/renderers/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       41 2023-05-05 10:46:33.000000 sailboat-gym-1.0.6/sailboat_gym/renderers/__init__.py
--rw-------   0 lucasmrdt   (501) staff       (20)    12313 2023-05-23 08:55:36.000000 sailboat-gym-1.0.6/sailboat_gym/renderers/cv_2d_renderer.py
--rw-------   0 lucasmrdt   (501) staff       (20)     1475 2023-05-23 13:57:54.000000 sailboat-gym-1.0.6/sailboat_gym/types.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     2410 2023-05-23 13:57:59.000000 sailboat-gym-1.0.6/sailboat_gym/utils.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:37:43.966283 sailboat-gym-1.0.6/sailboat_gym.egg-info/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1480 2023-05-31 07:37:43.000000 sailboat-gym-1.0.6/sailboat_gym.egg-info/PKG-INFO
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      559 2023-05-31 07:37:43.000000 sailboat-gym-1.0.6/sailboat_gym.egg-info/SOURCES.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)        1 2023-05-31 07:37:43.000000 sailboat-gym-1.0.6/sailboat_gym.egg-info/dependency_links.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      113 2023-05-31 07:37:43.000000 sailboat-gym-1.0.6/sailboat_gym.egg-info/requires.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       13 2023-05-31 07:37:43.000000 sailboat-gym-1.0.6/sailboat_gym.egg-info/top_level.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       38 2023-05-31 07:37:43.972534 sailboat-gym-1.0.6/setup.cfg
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     2669 2023-05-31 07:37:14.000000 sailboat-gym-1.0.6/setup.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:44:17.620280 sailboat-gym-1.0.7/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1074 2023-05-23 13:44:12.000000 sailboat-gym-1.0.7/LICENSE
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1403 2023-05-31 07:44:17.620133 sailboat-gym-1.0.7/PKG-INFO
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     5949 2023-05-31 06:34:03.000000 sailboat-gym-1.0.7/README.md
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:44:17.617346 sailboat-gym-1.0.7/sailboat_gym/
+-rw-------   0 lucasmrdt   (501) staff       (20)      445 2023-05-31 07:44:10.000000 sailboat-gym-1.0.7/sailboat_gym/__init__.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:44:17.618535 sailboat-gym-1.0.7/sailboat_gym/envs/
+-rw-------   0 lucasmrdt   (501) staff       (20)       41 2023-05-11 14:46:14.000000 sailboat-gym-1.0.7/sailboat_gym/envs/__init__.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      599 2023-05-11 15:47:26.000000 sailboat-gym-1.0.7/sailboat_gym/envs/env.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:44:17.619277 sailboat-gym-1.0.7/sailboat_gym/envs/sailboat_lsa/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       35 2023-05-11 14:43:54.000000 sailboat-gym-1.0.7/sailboat_gym/envs/sailboat_lsa/__init__.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     4054 2023-05-23 08:29:42.000000 sailboat-gym-1.0.7/sailboat_gym/envs/sailboat_lsa/lsa_env.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     7165 2023-05-23 08:33:00.000000 sailboat-gym-1.0.7/sailboat_gym/envs/sailboat_lsa/lsa_sim.py
+-rw-------   0 lucasmrdt   (501) staff       (20)      699 2023-05-11 15:38:32.000000 sailboat-gym-1.0.7/sailboat_gym/interfaces.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:44:17.619774 sailboat-gym-1.0.7/sailboat_gym/renderers/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       41 2023-05-05 10:46:33.000000 sailboat-gym-1.0.7/sailboat_gym/renderers/__init__.py
+-rw-------   0 lucasmrdt   (501) staff       (20)    12313 2023-05-23 08:55:36.000000 sailboat-gym-1.0.7/sailboat_gym/renderers/cv_2d_renderer.py
+-rw-------   0 lucasmrdt   (501) staff       (20)     1475 2023-05-23 13:57:54.000000 sailboat-gym-1.0.7/sailboat_gym/types.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     2410 2023-05-23 13:57:59.000000 sailboat-gym-1.0.7/sailboat_gym/utils.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:44:17.618165 sailboat-gym-1.0.7/sailboat_gym.egg-info/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1403 2023-05-31 07:44:17.000000 sailboat-gym-1.0.7/sailboat_gym.egg-info/PKG-INFO
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      559 2023-05-31 07:44:17.000000 sailboat-gym-1.0.7/sailboat_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)        1 2023-05-31 07:44:17.000000 sailboat-gym-1.0.7/sailboat_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      173 2023-05-31 07:44:17.000000 sailboat-gym-1.0.7/sailboat_gym.egg-info/requires.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       13 2023-05-31 07:44:17.000000 sailboat-gym-1.0.7/sailboat_gym.egg-info/top_level.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       38 2023-05-31 07:44:17.620331 sailboat-gym-1.0.7/setup.cfg
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     2726 2023-05-31 07:43:54.000000 sailboat-gym-1.0.7/setup.py
```

### Comparing `sailboat-gym-1.0.6/LICENSE` & `sailboat-gym-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/PKG-INFO` & `sailboat-gym-1.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sailboat-gym
-Version: 1.0.6
+Version: 1.0.7
 Summary: A dynamic gym simulation environment specifically designed for sailboats.
 Home-page: https://github.com/lucasmrdt/sailboat-gym
 Author: Lucas Marandat
 Author-email: lucas.mrdt+sailboat@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/lucasmrdt/sailboat-gym
 Project-URL: Repository, https://github.com/lucasmrdt/sailboat-gym
@@ -17,16 +17,13 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
-Provides-Extra: cv2d-renderer
-Provides-Extra: docker
-Provides-Extra: moviepy
 License-File: LICENSE
 
 
 
 Welcome to Sailboat Gym! This repository provides a dynamic simulation environment specifically designed for sailboats. With Sailboat Gym, you can explore and experiment with different control algorithms and strategies in a realistic virtual sailing environment.
```

### Comparing `sailboat-gym-1.0.6/README.md` & `sailboat-gym-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/sailboat_gym/envs/env.py` & `sailboat-gym-1.0.7/sailboat_gym/envs/env.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/sailboat_gym/envs/sailboat_lsa/lsa_env.py` & `sailboat-gym-1.0.7/sailboat_gym/envs/sailboat_lsa/lsa_env.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/sailboat_gym/envs/sailboat_lsa/lsa_sim.py` & `sailboat-gym-1.0.7/sailboat_gym/envs/sailboat_lsa/lsa_sim.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/sailboat_gym/interfaces.py` & `sailboat-gym-1.0.7/sailboat_gym/interfaces.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/sailboat_gym/renderers/cv_2d_renderer.py` & `sailboat-gym-1.0.7/sailboat_gym/renderers/cv_2d_renderer.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/sailboat_gym/types.py` & `sailboat-gym-1.0.7/sailboat_gym/types.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/sailboat_gym/utils.py` & `sailboat-gym-1.0.7/sailboat_gym/utils.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/sailboat_gym.egg-info/PKG-INFO` & `sailboat-gym-1.0.7/sailboat_gym.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sailboat-gym
-Version: 1.0.6
+Version: 1.0.7
 Summary: A dynamic gym simulation environment specifically designed for sailboats.
 Home-page: https://github.com/lucasmrdt/sailboat-gym
 Author: Lucas Marandat
 Author-email: lucas.mrdt+sailboat@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/lucasmrdt/sailboat-gym
 Project-URL: Repository, https://github.com/lucasmrdt/sailboat-gym
@@ -17,16 +17,13 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
-Provides-Extra: cv2d-renderer
-Provides-Extra: docker
-Provides-Extra: moviepy
 License-File: LICENSE
 
 
 
 Welcome to Sailboat Gym! This repository provides a dynamic simulation environment specifically designed for sailboats. With Sailboat Gym, you can explore and experiment with different control algorithms and strategies in a realistic virtual sailing environment.
```

### Comparing `sailboat-gym-1.0.6/sailboat_gym.egg-info/SOURCES.txt` & `sailboat-gym-1.0.7/sailboat_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.6/setup.py` & `sailboat-gym-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -62,21 +62,25 @@
         "Repository": "https://github.com/lucasmrdt/sailboat-gym",
         "Documentation": "https://github.com/lucasmrdt/sailboat-gym/blob/main/DOCUMENTATION.md",
         "Bug Report": "https://github.com/lucasmrdt/sailboat-gym/issues",
     },
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
-        # list your dependencies here
+        'gymnasium==0.28.1',
+        'msgpack_python==0.5.6',
+        'numpy==1.24.3',
+        'pydantic==1.10.7',
+        'pyzmq==25.0.2',
+        'tqdm==4.65.0',
+        'opencv-python==4.7.0.72',
+        'imageio-ffmpeg==0.4.8',
+        'docker==6.1.2',
+        'moviepy==1.0.3'
     ],
-    extras_require={
-        "cv2d-renderer": ["opencv-python >=4.7.0.72", "imageio-ffmpeg >=0.4.8"],
-        "docker": ["docker >=6.1.2"],
-        "moviepy": ["moviepy >=1.0.3"],
-    },
     package_data={
         "sailboat_gym": [
             "docs/demo.gif",
             "docs/sailing_schema.png",
         ]
     },
 )
```

