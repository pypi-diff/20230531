# Comparing `tmp/csle_attacker-0.2.3.tar.gz` & `tmp/csle_attacker-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_attacker-0.2.3.tar", last modified: Wed May 31 12:13:21 2023, max compression
+gzip compressed data, was "csle_attacker-0.2.4.tar", last modified: Wed May 31 13:43:05 2023, max compression
```

## Comparing `csle_attacker-0.2.3.tar` & `csle_attacker-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:21.696872 csle_attacker-0.2.3/
--rw-r--r--   0 kimham     (501) staff       (20)      659 2023-05-31 12:13:21.697005 csle_attacker-0.2.3/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3922 2023-01-11 18:45:47.000000 csle_attacker-0.2.3/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      673 2023-02-12 08:59:32.000000 csle_attacker-0.2.3/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1218 2023-05-31 12:13:21.697599 csle_attacker-0.2.3/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:21.682200 csle_attacker-0.2.3/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:21.685269 csle_attacker-0.2.3/src/csle_attacker/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 12:12:15.000000 csle_attacker-0.2.3/src/csle_attacker/__version__.py
--rw-r--r--   0 kimham     (501) staff       (20)      941 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/attacker.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:21.691519 csle_attacker-0.2.3/src/csle_attacker/emulation/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      994 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/attacker_stopping_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)    11411 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/emulated_attacker.py
--rw-r--r--   0 kimham     (501) staff       (20)    11560 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/exploit_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)     4676 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/post_exploit_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)     5951 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/recon_middleware.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:21.696060 csle_attacker-0.2.3/src/csle_attacker/emulation/util/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/util/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    45611 2023-04-19 06:25:48.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/util/exploit_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     7585 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/util/nikto_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    34189 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/util/nmap_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    29810 2022-11-28 13:00:49.000000 csle_attacker-0.2.3/src/csle_attacker/emulation/util/shell_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:21.688183 csle_attacker-0.2.3/src/csle_attacker.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      659 2023-05-31 12:13:21.000000 csle_attacker-0.2.3/src/csle_attacker.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      916 2023-05-31 12:13:21.000000 csle_attacker-0.2.3/src/csle_attacker.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 12:13:21.000000 csle_attacker-0.2.3/src/csle_attacker.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:33.000000 csle_attacker-0.2.3/src/csle_attacker.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      177 2023-05-31 12:13:21.000000 csle_attacker-0.2.3/src/csle_attacker.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       14 2023-05-31 12:13:21.000000 csle_attacker-0.2.3/src/csle_attacker.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.944818 csle_attacker-0.2.4/
+-rw-r--r--   0 kimham     (501) staff       (20)      659 2023-05-31 13:43:05.944937 csle_attacker-0.2.4/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     3922 2023-01-11 18:45:47.000000 csle_attacker-0.2.4/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      673 2023-02-12 08:59:32.000000 csle_attacker-0.2.4/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1218 2023-05-31 13:43:05.945491 csle_attacker-0.2.4/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.933069 csle_attacker-0.2.4/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.936040 csle_attacker-0.2.4/src/csle_attacker/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 csle_attacker-0.2.4/src/csle_attacker/__version__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      941 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/attacker.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.940961 csle_attacker-0.2.4/src/csle_attacker/emulation/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      994 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/attacker_stopping_middleware.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11411 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/emulated_attacker.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11560 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/exploit_middleware.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4676 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/post_exploit_middleware.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5951 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/recon_middleware.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.943987 csle_attacker-0.2.4/src/csle_attacker/emulation/util/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    45611 2023-04-19 06:25:48.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/exploit_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7585 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/nikto_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)    34189 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/nmap_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)    29810 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/shell_util.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.938195 csle_attacker-0.2.4/src/csle_attacker.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      659 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      916 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:33.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      177 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       14 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/top_level.txt
```

### Comparing `csle_attacker-0.2.3/PKG-INFO` & `csle_attacker-0.2.4/src/csle_attacker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle_attacker
-Version: 0.2.3
+Name: csle-attacker
+Version: 0.2.4
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.2.3/README.md` & `csle_attacker-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/pyproject.toml` & `csle_attacker-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/setup.cfg` & `csle_attacker-0.2.4/setup.cfg`

 * *Files 7% similar despite different names*

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

### Comparing `csle_attacker-0.2.3/src/csle_attacker/attacker.py` & `csle_attacker-0.2.4/src/csle_attacker/attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker/emulation/attacker_stopping_middleware.py` & `csle_attacker-0.2.4/src/csle_attacker/emulation/attacker_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker/emulation/emulated_attacker.py` & `csle_attacker-0.2.4/src/csle_attacker/emulation/emulated_attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker/emulation/exploit_middleware.py` & `csle_attacker-0.2.4/src/csle_attacker/emulation/exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker/emulation/post_exploit_middleware.py` & `csle_attacker-0.2.4/src/csle_attacker/emulation/post_exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker/emulation/recon_middleware.py` & `csle_attacker-0.2.4/src/csle_attacker/emulation/recon_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker/emulation/util/exploit_util.py` & `csle_attacker-0.2.4/src/csle_attacker/emulation/util/exploit_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker/emulation/util/nikto_util.py` & `csle_attacker-0.2.4/src/csle_attacker/emulation/util/nikto_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker/emulation/util/nmap_util.py` & `csle_attacker-0.2.4/src/csle_attacker/emulation/util/nmap_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker/emulation/util/shell_util.py` & `csle_attacker-0.2.4/src/csle_attacker/emulation/util/shell_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.3/src/csle_attacker.egg-info/PKG-INFO` & `csle_attacker-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle-attacker
-Version: 0.2.3
+Name: csle_attacker
+Version: 0.2.4
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.2.3/src/csle_attacker.egg-info/SOURCES.txt` & `csle_attacker-0.2.4/src/csle_attacker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

