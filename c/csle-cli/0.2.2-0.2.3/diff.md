# Comparing `tmp/csle_cli-0.2.2.tar.gz` & `tmp/csle_cli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cli-0.2.2.tar", last modified: Wed May 31 11:50:29 2023, max compression
+gzip compressed data, was "csle_cli-0.2.3.tar", last modified: Wed May 31 12:16:15 2023, max compression
```

## Comparing `csle_cli-0.2.2.tar` & `csle_cli-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:29.318225 csle_cli-0.2.2/
--rw-r--r--   0 kimham     (501) staff       (20)      629 2023-05-31 11:50:29.318338 csle_cli-0.2.2/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)    22943 2023-02-12 17:03:02.000000 csle_cli-0.2.2/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      668 2023-02-12 08:59:32.000000 csle_cli-0.2.2/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1368 2023-05-31 11:50:29.318994 csle_cli-0.2.2/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cli-0.2.2/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:29.311524 csle_cli-0.2.2/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:29.314240 csle_cli-0.2.2/src/csle_cli/
--rw-r--r--   0 kimham     (501) staff       (20)       38 2022-11-28 13:00:49.000000 csle_cli-0.2.2/src/csle_cli/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:45:39.000000 csle_cli-0.2.2/src/csle_cli/__version__.py
--rwxr-xr-x   0 kimham     (501) staff       (20)   111257 2023-03-22 11:50:26.000000 csle_cli-0.2.2/src/csle_cli/cli.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:29.318025 csle_cli-0.2.2/src/csle_cli.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      629 2023-05-31 11:50:28.000000 csle_cli-0.2.2/src/csle_cli.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      369 2023-05-31 11:50:29.000000 csle_cli-0.2.2/src/csle_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:50:28.000000 csle_cli-0.2.2/src/csle_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)       47 2023-05-31 11:50:29.000000 csle_cli-0.2.2/src/csle_cli.egg-info/entry_points.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:54.000000 csle_cli-0.2.2/src/csle_cli.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      291 2023-05-31 11:50:29.000000 csle_cli-0.2.2/src/csle_cli.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)        9 2023-05-31 11:50:29.000000 csle_cli-0.2.2/src/csle_cli.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:15.347381 csle_cli-0.2.3/
+-rw-r--r--   0 kimham     (501) staff       (20)      629 2023-05-31 12:16:15.347494 csle_cli-0.2.3/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)    22943 2023-02-12 17:03:02.000000 csle_cli-0.2.3/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      668 2023-02-12 08:59:32.000000 csle_cli-0.2.3/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1368 2023-05-31 12:16:15.348039 csle_cli-0.2.3/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cli-0.2.3/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:15.338455 csle_cli-0.2.3/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:15.342864 csle_cli-0.2.3/src/csle_cli/
+-rw-r--r--   0 kimham     (501) staff       (20)       38 2022-11-28 13:00:49.000000 csle_cli-0.2.3/src/csle_cli/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 12:12:15.000000 csle_cli-0.2.3/src/csle_cli/__version__.py
+-rwxr-xr-x   0 kimham     (501) staff       (20)   111257 2023-03-22 11:50:26.000000 csle_cli-0.2.3/src/csle_cli/cli.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:15.347191 csle_cli-0.2.3/src/csle_cli.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      629 2023-05-31 12:16:14.000000 csle_cli-0.2.3/src/csle_cli.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      369 2023-05-31 12:16:15.000000 csle_cli-0.2.3/src/csle_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 12:16:14.000000 csle_cli-0.2.3/src/csle_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       47 2023-05-31 12:16:15.000000 csle_cli-0.2.3/src/csle_cli.egg-info/entry_points.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:54.000000 csle_cli-0.2.3/src/csle_cli.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      291 2023-05-31 12:16:15.000000 csle_cli-0.2.3/src/csle_cli.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        9 2023-05-31 12:16:15.000000 csle_cli-0.2.3/src/csle_cli.egg-info/top_level.txt
```

### Comparing `csle_cli-0.2.2/PKG-INFO` & `csle_cli-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.2.2/README.md` & `csle_cli-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.2/pyproject.toml` & `csle_cli-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.2/setup.cfg` & `csle_cli-0.2.3/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	click>=8.1.3
-	csle-common>=0.2.2
-	csle-cluster>=0.2.2
-	csle-collector>=0.2.2
-	csle-attacker>=0.2.2
-	csle-defender>=0.2.2
-	csle-system-identification>=0.2.2
-	gym-csle-stopping-game>=0.2.2
-	csle-agents>=0.2.2
+	csle-common>=0.2.3
+	csle-cluster>=0.2.3
+	csle-collector>=0.2.3
+	csle-attacker>=0.2.3
+	csle-defender>=0.2.3
+	csle-system-identification>=0.2.3
+	gym-csle-stopping-game>=0.2.3
+	csle-agents>=0.2.3
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cli-0.2.2/src/csle_cli/cli.py` & `csle_cli-0.2.3/src/csle_cli/cli.py`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.2/src/csle_cli.egg-info/PKG-INFO` & `csle_cli-0.2.3/src/csle_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

