# Comparing `tmp/csle_defender-0.2.3.tar.gz` & `tmp/csle_defender-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_defender-0.2.3.tar", last modified: Wed May 31 12:13:38 2023, max compression
+gzip compressed data, was "csle_defender-0.2.4.tar", last modified: Wed May 31 13:43:23 2023, max compression
```

## Comparing `csle_defender-0.2.3.tar` & `csle_defender-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:38.350790 csle_defender-0.2.3/
--rw-r--r--   0 kimham     (501) staff       (20)      654 2023-05-31 12:13:38.350918 csle_defender-0.2.3/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3858 2023-01-11 18:45:47.000000 csle_defender-0.2.3/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      673 2023-02-12 08:59:32.000000 csle_defender-0.2.3/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1213 2023-05-31 12:13:38.351525 csle_defender-0.2.3/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_defender-0.2.3/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:38.343893 csle_defender-0.2.3/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:38.346365 csle_defender-0.2.3/src/csle_defender/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_defender-0.2.3/src/csle_defender/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 12:12:15.000000 csle_defender-0.2.3/src/csle_defender/__version__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1197 2022-11-28 13:00:49.000000 csle_defender-0.2.3/src/csle_defender/defender.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:38.350462 csle_defender-0.2.3/src/csle_defender/emulation/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_defender-0.2.3/src/csle_defender/emulation/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1879 2022-11-28 13:00:49.000000 csle_defender-0.2.3/src/csle_defender/emulation/defender_stopping_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)     1514 2022-11-28 13:00:49.000000 csle_defender-0.2.3/src/csle_defender/emulation/defender_update_state_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)     3034 2022-11-28 13:00:49.000000 csle_defender-0.2.3/src/csle_defender/emulation/emulated_defender.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:38.348788 csle_defender-0.2.3/src/csle_defender.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      654 2023-05-31 12:13:37.000000 csle_defender-0.2.3/src/csle_defender.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      593 2023-05-31 12:13:38.000000 csle_defender-0.2.3/src/csle_defender.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 12:13:37.000000 csle_defender-0.2.3/src/csle_defender.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:40.000000 csle_defender-0.2.3/src/csle_defender.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      177 2023-05-31 12:13:38.000000 csle_defender-0.2.3/src/csle_defender.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       14 2023-05-31 12:13:38.000000 csle_defender-0.2.3/src/csle_defender.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:23.398544 csle_defender-0.2.4/
+-rw-r--r--   0 kimham     (501) staff       (20)      654 2023-05-31 13:43:23.398727 csle_defender-0.2.4/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     3858 2023-01-11 18:45:47.000000 csle_defender-0.2.4/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      673 2023-02-12 08:59:32.000000 csle_defender-0.2.4/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1213 2023-05-31 13:43:23.399609 csle_defender-0.2.4/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_defender-0.2.4/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:23.389638 csle_defender-0.2.4/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:23.392742 csle_defender-0.2.4/src/csle_defender/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_defender-0.2.4/src/csle_defender/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 csle_defender-0.2.4/src/csle_defender/__version__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1197 2022-11-28 13:00:49.000000 csle_defender-0.2.4/src/csle_defender/defender.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:23.397972 csle_defender-0.2.4/src/csle_defender/emulation/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_defender-0.2.4/src/csle_defender/emulation/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1879 2022-11-28 13:00:49.000000 csle_defender-0.2.4/src/csle_defender/emulation/defender_stopping_middleware.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1514 2022-11-28 13:00:49.000000 csle_defender-0.2.4/src/csle_defender/emulation/defender_update_state_middleware.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3034 2022-11-28 13:00:49.000000 csle_defender-0.2.4/src/csle_defender/emulation/emulated_defender.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:23.396022 csle_defender-0.2.4/src/csle_defender.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      654 2023-05-31 13:43:22.000000 csle_defender-0.2.4/src/csle_defender.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      593 2023-05-31 13:43:23.000000 csle_defender-0.2.4/src/csle_defender.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:43:22.000000 csle_defender-0.2.4/src/csle_defender.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:40.000000 csle_defender-0.2.4/src/csle_defender.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      177 2023-05-31 13:43:23.000000 csle_defender-0.2.4/src/csle_defender.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       14 2023-05-31 13:43:23.000000 csle_defender-0.2.4/src/csle_defender.egg-info/top_level.txt
```

### Comparing `csle_defender-0.2.3/PKG-INFO` & `csle_defender-0.2.4/src/csle_defender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle_defender
-Version: 0.2.3
+Name: csle-defender
+Version: 0.2.4
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.2.3/README.md` & `csle_defender-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.3/pyproject.toml` & `csle_defender-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.3/setup.cfg` & `csle_defender-0.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.2.3
+	csle-common>=0.2.4
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_defender-0.2.3/src/csle_defender/defender.py` & `csle_defender-0.2.4/src/csle_defender/defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.3/src/csle_defender/emulation/defender_stopping_middleware.py` & `csle_defender-0.2.4/src/csle_defender/emulation/defender_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.3/src/csle_defender/emulation/defender_update_state_middleware.py` & `csle_defender-0.2.4/src/csle_defender/emulation/defender_update_state_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.3/src/csle_defender/emulation/emulated_defender.py` & `csle_defender-0.2.4/src/csle_defender/emulation/emulated_defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.3/src/csle_defender.egg-info/PKG-INFO` & `csle_defender-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle-defender
-Version: 0.2.3
+Name: csle_defender
+Version: 0.2.4
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.2.3/src/csle_defender.egg-info/SOURCES.txt` & `csle_defender-0.2.4/src/csle_defender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

