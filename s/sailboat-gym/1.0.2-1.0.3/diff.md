# Comparing `tmp/sailboat-gym-1.0.2.tar.gz` & `tmp/sailboat-gym-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sailboat-gym-1.0.2.tar", last modified: Wed May 31 06:58:44 2023, max compression
+gzip compressed data, was "sailboat-gym-1.0.3.tar", last modified: Wed May 31 07:21:25 2023, max compression
```

## Comparing `sailboat-gym-1.0.2.tar` & `sailboat-gym-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,17 @@
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 06:58:44.876680 sailboat-gym-1.0.2/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1074 2023-05-23 13:44:12.000000 sailboat-gym-1.0.2/LICENSE
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     6724 2023-05-31 06:58:44.876512 sailboat-gym-1.0.2/PKG-INFO
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     5949 2023-05-31 06:34:03.000000 sailboat-gym-1.0.2/README.md
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 06:58:44.872961 sailboat-gym-1.0.2/sailboat_gym/
--rw-------   0 lucasmrdt   (501) staff       (20)      294 2023-05-31 06:34:02.000000 sailboat-gym-1.0.2/sailboat_gym/__init__.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 06:58:44.874486 sailboat-gym-1.0.2/sailboat_gym/envs/
--rw-------   0 lucasmrdt   (501) staff       (20)       41 2023-05-11 14:46:14.000000 sailboat-gym-1.0.2/sailboat_gym/envs/__init__.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      599 2023-05-11 15:47:26.000000 sailboat-gym-1.0.2/sailboat_gym/envs/env.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 06:58:44.875611 sailboat-gym-1.0.2/sailboat_gym/envs/sailboat_lsa/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       35 2023-05-11 14:43:54.000000 sailboat-gym-1.0.2/sailboat_gym/envs/sailboat_lsa/__init__.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     4054 2023-05-23 08:29:42.000000 sailboat-gym-1.0.2/sailboat_gym/envs/sailboat_lsa/lsa_env.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     7165 2023-05-23 08:33:00.000000 sailboat-gym-1.0.2/sailboat_gym/envs/sailboat_lsa/lsa_sim.py
--rw-------   0 lucasmrdt   (501) staff       (20)      699 2023-05-11 15:38:32.000000 sailboat-gym-1.0.2/sailboat_gym/interfaces.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 06:58:44.876216 sailboat-gym-1.0.2/sailboat_gym/renderers/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       41 2023-05-05 10:46:33.000000 sailboat-gym-1.0.2/sailboat_gym/renderers/__init__.py
--rw-------   0 lucasmrdt   (501) staff       (20)    12313 2023-05-23 08:55:36.000000 sailboat-gym-1.0.2/sailboat_gym/renderers/cv_2d_renderer.py
--rw-------   0 lucasmrdt   (501) staff       (20)     1475 2023-05-23 13:57:54.000000 sailboat-gym-1.0.2/sailboat_gym/types.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     2410 2023-05-23 13:57:59.000000 sailboat-gym-1.0.2/sailboat_gym/utils.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 06:58:44.873852 sailboat-gym-1.0.2/sailboat_gym.egg-info/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     6724 2023-05-31 06:58:44.000000 sailboat-gym-1.0.2/sailboat_gym.egg-info/PKG-INFO
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      559 2023-05-31 06:58:44.000000 sailboat-gym-1.0.2/sailboat_gym.egg-info/SOURCES.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)        1 2023-05-31 06:58:44.000000 sailboat-gym-1.0.2/sailboat_gym.egg-info/dependency_links.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      173 2023-05-31 06:58:44.000000 sailboat-gym-1.0.2/sailboat_gym.egg-info/requires.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       13 2023-05-31 06:58:44.000000 sailboat-gym-1.0.2/sailboat_gym.egg-info/top_level.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       38 2023-05-31 06:58:44.876727 sailboat-gym-1.0.2/setup.cfg
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1235 2023-05-31 06:58:29.000000 sailboat-gym-1.0.2/setup.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:21:25.780703 sailboat-gym-1.0.3/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1074 2023-05-23 13:44:12.000000 sailboat-gym-1.0.3/LICENSE
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1480 2023-05-31 07:21:25.780562 sailboat-gym-1.0.3/PKG-INFO
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     5949 2023-05-31 06:34:03.000000 sailboat-gym-1.0.3/README.md
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:21:25.779254 sailboat-gym-1.0.3/sailboat_gym/
+-rw-------   0 lucasmrdt   (501) staff       (20)      445 2023-05-31 07:19:51.000000 sailboat-gym-1.0.3/sailboat_gym/__init__.py
+-rw-------   0 lucasmrdt   (501) staff       (20)      699 2023-05-11 15:38:32.000000 sailboat-gym-1.0.3/sailboat_gym/interfaces.py
+-rw-------   0 lucasmrdt   (501) staff       (20)     1475 2023-05-23 13:57:54.000000 sailboat-gym-1.0.3/sailboat_gym/types.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     2410 2023-05-23 13:57:59.000000 sailboat-gym-1.0.3/sailboat_gym/utils.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:21:25.780314 sailboat-gym-1.0.3/sailboat_gym.egg-info/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1480 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/PKG-INFO
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      301 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)        1 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      113 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/requires.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       13 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/top_level.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       38 2023-05-31 07:21:25.780758 sailboat-gym-1.0.3/setup.cfg
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     2655 2023-05-31 07:21:18.000000 sailboat-gym-1.0.3/setup.py
```

### Comparing `sailboat-gym-1.0.2/LICENSE` & `sailboat-gym-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.2/PKG-INFO` & `sailboat-gym-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: sailboat-gym
-Version: 1.0.2
-Summary: Dynamic simulation environment for sailboats. With Sailboat Gym, you can explore and experiment with different control algorithms and strategies in a realistic virtual sailing environment.
-Home-page: https://github.com/lucasmrdt/sailboat-gym
-Author: Lucas Marandat
-Author-email: lucas.mrdt+sailboat@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Sailboat Gym ⛵
 
 ![demo](./docs/demo.gif)
 
 Welcome to Sailboat Gym! This repository provides a dynamic simulation environment specifically designed for sailboats. With Sailboat Gym, you can explore and experiment with different control algorithms and strategies in a realistic virtual sailing environment.
 
 ## Table of Contents
@@ -143,8 +126,8 @@
 
 ## Contributing
 
 We welcome contributions to Sailboat Gym. Please refer to our [contributing guidelines](./CONTRIBUTING.md) for more information.
 
 ## License
 
-Sailboat Gym is released under the [MIT License](./LICENSE). You are free to use, modify, and distribute this software for both commercial and non-commercial purposes.
+Sailboat Gym is released under the [MIT License](./LICENSE). You are free to use, modify, and distribute this software for both commercial and non-commercial purposes.
```

### Comparing `sailboat-gym-1.0.2/sailboat_gym/interfaces.py` & `sailboat-gym-1.0.3/sailboat_gym/interfaces.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.2/sailboat_gym/types.py` & `sailboat-gym-1.0.3/sailboat_gym/types.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.2/sailboat_gym/utils.py` & `sailboat-gym-1.0.3/sailboat_gym/utils.py`

 * *Files identical despite different names*

