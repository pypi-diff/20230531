# Comparing `tmp/csle_cli-0.2.0.tar.gz` & `tmp/csle_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cli-0.2.0.tar", last modified: Sun Apr 30 12:38:03 2023, max compression
+gzip compressed data, was "csle_cli-0.2.1.tar", last modified: Wed May 31 11:27:07 2023, max compression
```

## Comparing `csle_cli-0.2.0.tar` & `csle_cli-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:03.764944 csle_cli-0.2.0/
--rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-04-30 12:38:03.764944 csle_cli-0.2.0/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)    22943 2023-03-28 14:03:22.000000 csle_cli-0.2.0/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      668 2023-03-28 14:03:22.000000 csle_cli-0.2.0/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1368 2023-04-30 12:38:03.764944 csle_cli-0.2.0/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cli-0.2.0/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:03.760944 csle_cli-0.2.0/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:03.760944 csle_cli-0.2.0/src/csle_cli/
--rw-rw-r--   0 kim       (1000) kim       (1000)       38 2023-03-28 14:03:22.000000 csle_cli-0.2.0/src/csle_cli/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_cli-0.2.0/src/csle_cli/__version__.py
--rwxrwxr-x   0 kim       (1000) kim       (1000)   111257 2023-03-28 14:03:22.000000 csle_cli-0.2.0/src/csle_cli/cli.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:03.764944 csle_cli-0.2.0/src/csle_cli.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-04-30 12:38:03.000000 csle_cli-0.2.0/src/csle_cli.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      369 2023-04-30 12:38:03.000000 csle_cli-0.2.0/src/csle_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:38:03.000000 csle_cli-0.2.0/src/csle_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       47 2023-04-30 12:38:03.000000 csle_cli-0.2.0/src/csle_cli.egg-info/entry_points.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:27.000000 csle_cli-0.2.0/src/csle_cli.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      291 2023-04-30 12:38:03.000000 csle_cli-0.2.0/src/csle_cli.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-04-30 12:38:03.000000 csle_cli-0.2.0/src/csle_cli.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:07.651961 csle_cli-0.2.1/
+-rw-r--r--   0 kimham     (501) staff       (20)      629 2023-05-31 11:27:07.652076 csle_cli-0.2.1/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)    22943 2023-02-12 17:03:02.000000 csle_cli-0.2.1/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      668 2023-02-12 08:59:32.000000 csle_cli-0.2.1/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1368 2023-05-31 11:27:07.652680 csle_cli-0.2.1/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cli-0.2.1/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:07.643265 csle_cli-0.2.1/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:07.646708 csle_cli-0.2.1/src/csle_cli/
+-rw-r--r--   0 kimham     (501) staff       (20)       38 2022-11-28 13:00:49.000000 csle_cli-0.2.1/src/csle_cli/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:22:38.000000 csle_cli-0.2.1/src/csle_cli/__version__.py
+-rwxr-xr-x   0 kimham     (501) staff       (20)   111257 2023-03-22 11:50:26.000000 csle_cli-0.2.1/src/csle_cli/cli.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:07.651733 csle_cli-0.2.1/src/csle_cli.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      629 2023-05-31 11:27:07.000000 csle_cli-0.2.1/src/csle_cli.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      369 2023-05-31 11:27:07.000000 csle_cli-0.2.1/src/csle_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:27:07.000000 csle_cli-0.2.1/src/csle_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       47 2023-05-31 11:27:07.000000 csle_cli-0.2.1/src/csle_cli.egg-info/entry_points.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:54.000000 csle_cli-0.2.1/src/csle_cli.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      291 2023-05-31 11:27:07.000000 csle_cli-0.2.1/src/csle_cli.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        9 2023-05-31 11:27:07.000000 csle_cli-0.2.1/src/csle_cli.egg-info/top_level.txt
```

### Comparing `csle_cli-0.2.0/PKG-INFO` & `csle_cli-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.2.0/README.md` & `csle_cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.0/pyproject.toml` & `csle_cli-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.0/setup.cfg` & `csle_cli-0.2.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	click>=8.1.3
-	csle-common>=0.2.0
-	csle-cluster>=0.2.0
-	csle-collector>=0.2.0
-	csle-attacker>=0.2.0
-	csle-defender>=0.2.0
-	csle-system-identification>=0.2.0
-	gym-csle-stopping-game>=0.2.0
-	csle-agents>=0.2.0
+	csle-common>=0.2.1
+	csle-cluster>=0.2.1
+	csle-collector>=0.2.1
+	csle-attacker>=0.2.1
+	csle-defender>=0.2.1
+	csle-system-identification>=0.2.1
+	gym-csle-stopping-game>=0.2.1
+	csle-agents>=0.2.1
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cli-0.2.0/src/csle_cli/cli.py` & `csle_cli-0.2.1/src/csle_cli/cli.py`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.0/src/csle_cli.egg-info/PKG-INFO` & `csle_cli-0.2.1/src/csle_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

