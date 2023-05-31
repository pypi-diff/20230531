# Comparing `tmp/csle_defender-0.2.1.tar.gz` & `tmp/csle_defender-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_defender-0.2.1.tar", last modified: Wed May 31 11:24:19 2023, max compression
+gzip compressed data, was "csle_defender-0.2.2.tar", last modified: Wed May 31 11:47:16 2023, max compression
```

## Comparing `csle_defender-0.2.1.tar` & `csle_defender-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:24:19.239280 csle_defender-0.2.1/
--rw-r--r--   0 kimham     (501) staff       (20)      654 2023-05-31 11:24:19.239421 csle_defender-0.2.1/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3858 2023-01-11 18:45:47.000000 csle_defender-0.2.1/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      673 2023-02-12 08:59:32.000000 csle_defender-0.2.1/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1213 2023-05-31 11:24:19.240222 csle_defender-0.2.1/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_defender-0.2.1/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:24:19.230439 csle_defender-0.2.1/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:24:19.233066 csle_defender-0.2.1/src/csle_defender/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_defender-0.2.1/src/csle_defender/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:22:38.000000 csle_defender-0.2.1/src/csle_defender/__version__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1197 2022-11-28 13:00:49.000000 csle_defender-0.2.1/src/csle_defender/defender.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:24:19.238886 csle_defender-0.2.1/src/csle_defender/emulation/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_defender-0.2.1/src/csle_defender/emulation/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1879 2022-11-28 13:00:49.000000 csle_defender-0.2.1/src/csle_defender/emulation/defender_stopping_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)     1514 2022-11-28 13:00:49.000000 csle_defender-0.2.1/src/csle_defender/emulation/defender_update_state_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)     3034 2022-11-28 13:00:49.000000 csle_defender-0.2.1/src/csle_defender/emulation/emulated_defender.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:24:19.235626 csle_defender-0.2.1/src/csle_defender.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      654 2023-05-31 11:24:18.000000 csle_defender-0.2.1/src/csle_defender.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      593 2023-05-31 11:24:19.000000 csle_defender-0.2.1/src/csle_defender.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:24:18.000000 csle_defender-0.2.1/src/csle_defender.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:40.000000 csle_defender-0.2.1/src/csle_defender.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      177 2023-05-31 11:24:19.000000 csle_defender-0.2.1/src/csle_defender.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       14 2023-05-31 11:24:19.000000 csle_defender-0.2.1/src/csle_defender.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:47:16.978160 csle_defender-0.2.2/
+-rw-r--r--   0 kimham     (501) staff       (20)      654 2023-05-31 11:47:16.978285 csle_defender-0.2.2/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     3858 2023-01-11 18:45:47.000000 csle_defender-0.2.2/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      673 2023-02-12 08:59:32.000000 csle_defender-0.2.2/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1213 2023-05-31 11:47:16.978870 csle_defender-0.2.2/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_defender-0.2.2/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:47:16.970500 csle_defender-0.2.2/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:47:16.973315 csle_defender-0.2.2/src/csle_defender/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_defender-0.2.2/src/csle_defender/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:45:39.000000 csle_defender-0.2.2/src/csle_defender/__version__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1197 2022-11-28 13:00:49.000000 csle_defender-0.2.2/src/csle_defender/defender.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:47:16.977635 csle_defender-0.2.2/src/csle_defender/emulation/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_defender-0.2.2/src/csle_defender/emulation/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1879 2022-11-28 13:00:49.000000 csle_defender-0.2.2/src/csle_defender/emulation/defender_stopping_middleware.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1514 2022-11-28 13:00:49.000000 csle_defender-0.2.2/src/csle_defender/emulation/defender_update_state_middleware.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3034 2022-11-28 13:00:49.000000 csle_defender-0.2.2/src/csle_defender/emulation/emulated_defender.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:47:16.975992 csle_defender-0.2.2/src/csle_defender.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      654 2023-05-31 11:47:16.000000 csle_defender-0.2.2/src/csle_defender.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      593 2023-05-31 11:47:16.000000 csle_defender-0.2.2/src/csle_defender.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:47:16.000000 csle_defender-0.2.2/src/csle_defender.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:40.000000 csle_defender-0.2.2/src/csle_defender.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      177 2023-05-31 11:47:16.000000 csle_defender-0.2.2/src/csle_defender.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       14 2023-05-31 11:47:16.000000 csle_defender-0.2.2/src/csle_defender.egg-info/top_level.txt
```

### Comparing `csle_defender-0.2.1/PKG-INFO` & `csle_defender-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_defender
-Version: 0.2.1
+Version: 0.2.2
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.2.1/README.md` & `csle_defender-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.1/pyproject.toml` & `csle_defender-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.1/setup.cfg` & `csle_defender-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.2.1
+	csle-common>=0.2.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_defender-0.2.1/src/csle_defender/defender.py` & `csle_defender-0.2.2/src/csle_defender/defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.1/src/csle_defender/emulation/defender_stopping_middleware.py` & `csle_defender-0.2.2/src/csle_defender/emulation/defender_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.1/src/csle_defender/emulation/defender_update_state_middleware.py` & `csle_defender-0.2.2/src/csle_defender/emulation/defender_update_state_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.1/src/csle_defender/emulation/emulated_defender.py` & `csle_defender-0.2.2/src/csle_defender/emulation/emulated_defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.2.1/src/csle_defender.egg-info/PKG-INFO` & `csle_defender-0.2.2/src/csle_defender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-defender
-Version: 0.2.1
+Version: 0.2.2
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.2.1/src/csle_defender.egg-info/SOURCES.txt` & `csle_defender-0.2.2/src/csle_defender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

