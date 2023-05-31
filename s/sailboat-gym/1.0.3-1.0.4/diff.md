# Comparing `tmp/sailboat-gym-1.0.3.tar.gz` & `tmp/sailboat-gym-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sailboat-gym-1.0.3.tar", last modified: Wed May 31 07:21:25 2023, max compression
+gzip compressed data, was "sailboat-gym-1.0.4.tar", last modified: Wed May 31 07:25:33 2023, max compression
```

## Comparing `sailboat-gym-1.0.3.tar` & `sailboat-gym-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:21:25.780703 sailboat-gym-1.0.3/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1074 2023-05-23 13:44:12.000000 sailboat-gym-1.0.3/LICENSE
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1480 2023-05-31 07:21:25.780562 sailboat-gym-1.0.3/PKG-INFO
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     5949 2023-05-31 06:34:03.000000 sailboat-gym-1.0.3/README.md
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:21:25.779254 sailboat-gym-1.0.3/sailboat_gym/
--rw-------   0 lucasmrdt   (501) staff       (20)      445 2023-05-31 07:19:51.000000 sailboat-gym-1.0.3/sailboat_gym/__init__.py
--rw-------   0 lucasmrdt   (501) staff       (20)      699 2023-05-11 15:38:32.000000 sailboat-gym-1.0.3/sailboat_gym/interfaces.py
--rw-------   0 lucasmrdt   (501) staff       (20)     1475 2023-05-23 13:57:54.000000 sailboat-gym-1.0.3/sailboat_gym/types.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     2410 2023-05-23 13:57:59.000000 sailboat-gym-1.0.3/sailboat_gym/utils.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:21:25.780314 sailboat-gym-1.0.3/sailboat_gym.egg-info/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1480 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/PKG-INFO
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      301 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/SOURCES.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)        1 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/dependency_links.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      113 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/requires.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       13 2023-05-31 07:21:25.000000 sailboat-gym-1.0.3/sailboat_gym.egg-info/top_level.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       38 2023-05-31 07:21:25.780758 sailboat-gym-1.0.3/setup.cfg
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     2655 2023-05-31 07:21:18.000000 sailboat-gym-1.0.3/setup.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:25:33.468308 sailboat-gym-1.0.4/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1074 2023-05-23 13:44:12.000000 sailboat-gym-1.0.4/LICENSE
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1480 2023-05-31 07:25:33.468149 sailboat-gym-1.0.4/PKG-INFO
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     5949 2023-05-31 06:34:03.000000 sailboat-gym-1.0.4/README.md
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:25:33.466490 sailboat-gym-1.0.4/sailboat_gym/
+-rw-------   0 lucasmrdt   (501) staff       (20)      445 2023-05-31 07:25:25.000000 sailboat-gym-1.0.4/sailboat_gym/__init__.py
+-rw-------   0 lucasmrdt   (501) staff       (20)      699 2023-05-11 15:38:32.000000 sailboat-gym-1.0.4/sailboat_gym/interfaces.py
+-rw-------   0 lucasmrdt   (501) staff       (20)     1475 2023-05-23 13:57:54.000000 sailboat-gym-1.0.4/sailboat_gym/types.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     2410 2023-05-23 13:57:59.000000 sailboat-gym-1.0.4/sailboat_gym/utils.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 07:25:33.467899 sailboat-gym-1.0.4/sailboat_gym.egg-info/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1480 2023-05-31 07:25:33.000000 sailboat-gym-1.0.4/sailboat_gym.egg-info/PKG-INFO
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      301 2023-05-31 07:25:33.000000 sailboat-gym-1.0.4/sailboat_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)        1 2023-05-31 07:25:33.000000 sailboat-gym-1.0.4/sailboat_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      113 2023-05-31 07:25:33.000000 sailboat-gym-1.0.4/sailboat_gym.egg-info/requires.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       13 2023-05-31 07:25:33.000000 sailboat-gym-1.0.4/sailboat_gym.egg-info/top_level.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       38 2023-05-31 07:25:33.468359 sailboat-gym-1.0.4/setup.cfg
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     2655 2023-05-31 07:21:18.000000 sailboat-gym-1.0.4/setup.py
```

### Comparing `sailboat-gym-1.0.3/LICENSE` & `sailboat-gym-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.3/PKG-INFO` & `sailboat-gym-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sailboat-gym
-Version: 1.0.3
+Version: 1.0.4
 Summary: A dynamic gym simulation environment specifically designed for sailboats.
 Home-page: https://github.com/lucasmrdt/sailboat-gym
 Author: Lucas Marandat
 Author-email: lucas.mrdt+sailboat@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/lucasmrdt/sailboat-gym
 Project-URL: Repository, https://github.com/lucasmrdt/sailboat-gym
```

### Comparing `sailboat-gym-1.0.3/README.md` & `sailboat-gym-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.3/sailboat_gym/interfaces.py` & `sailboat-gym-1.0.4/sailboat_gym/interfaces.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.3/sailboat_gym/types.py` & `sailboat-gym-1.0.4/sailboat_gym/types.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.3/sailboat_gym/utils.py` & `sailboat-gym-1.0.4/sailboat_gym/utils.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.3/sailboat_gym.egg-info/PKG-INFO` & `sailboat-gym-1.0.4/sailboat_gym.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sailboat-gym
-Version: 1.0.3
+Version: 1.0.4
 Summary: A dynamic gym simulation environment specifically designed for sailboats.
 Home-page: https://github.com/lucasmrdt/sailboat-gym
 Author: Lucas Marandat
 Author-email: lucas.mrdt+sailboat@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/lucasmrdt/sailboat-gym
 Project-URL: Repository, https://github.com/lucasmrdt/sailboat-gym
```

### Comparing `sailboat-gym-1.0.3/setup.py` & `sailboat-gym-1.0.4/setup.py`

 * *Files identical despite different names*

