# Comparing `tmp/csle_cluster-0.2.2.tar.gz` & `tmp/csle_cluster-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cluster-0.2.2.tar", last modified: Wed May 31 11:50:49 2023, max compression
+gzip compressed data, was "csle_cluster-0.2.3.tar", last modified: Wed May 31 12:16:32 2023, max compression
```

## Comparing `csle_cluster-0.2.2.tar` & `csle_cluster-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.871445 csle_cluster-0.2.2/
--rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 11:50:49.871576 csle_cluster-0.2.2/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     4256 2023-03-05 07:26:30.000000 csle_cluster-0.2.2/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      672 2023-02-12 09:12:26.000000 csle_cluster-0.2.2/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1406 2023-05-31 11:50:49.872172 csle_cluster-0.2.2/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cluster-0.2.2/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.851875 csle_cluster-0.2.2/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.854869 csle_cluster-0.2.2/src/csle_cluster/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2023-02-12 09:44:18.000000 csle_cluster-0.2.2/src/csle_cluster/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:45:39.000000 csle_cluster-0.2.2/src/csle_cluster/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.868822 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)   229454 2023-05-31 11:33:47.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)   269186 2023-05-01 07:57:15.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)   197343 2023-03-31 11:14:06.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)   349502 2023-03-31 11:14:06.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)   202990 2023-03-31 11:14:06.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)   188175 2023-04-19 06:25:48.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/query_cluster_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.870888 csle_cluster-0.2.2/src/csle_cluster/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-05 07:26:30.000000 csle_cluster-0.2.2/src/csle_cluster/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      375 2023-03-16 16:24:28.000000 csle_cluster-0.2.2/src/csle_cluster/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.856976 csle_cluster-0.2.2/src/csle_cluster.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      805 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-02-12 09:44:23.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      251 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       13 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:32.449602 csle_cluster-0.2.3/
+-rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 12:16:32.449742 csle_cluster-0.2.3/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     4256 2023-03-05 07:26:30.000000 csle_cluster-0.2.3/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      672 2023-02-12 09:12:26.000000 csle_cluster-0.2.3/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1406 2023-05-31 12:16:32.450381 csle_cluster-0.2.3/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cluster-0.2.3/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:32.430079 csle_cluster-0.2.3/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:32.432511 csle_cluster-0.2.3/src/csle_cluster/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2023-02-12 09:44:18.000000 csle_cluster-0.2.3/src/csle_cluster/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 12:12:15.000000 csle_cluster-0.2.3/src/csle_cluster/__version__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:32.447241 csle_cluster-0.2.3/src/csle_cluster/cluster_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_cluster-0.2.3/src/csle_cluster/cluster_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)   229454 2023-05-31 11:33:47.000000 csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)   269186 2023-05-01 07:57:15.000000 csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)   197343 2023-03-31 11:14:06.000000 csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)   349502 2023-03-31 11:14:06.000000 csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)   202990 2023-03-31 11:14:06.000000 csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_manager_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)   188175 2023-04-19 06:25:48.000000 csle_cluster-0.2.3/src/csle_cluster/cluster_manager/query_cluster_manager.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:32.449062 csle_cluster-0.2.3/src/csle_cluster/constants/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-05 07:26:30.000000 csle_cluster-0.2.3/src/csle_cluster/constants/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      375 2023-03-16 16:24:28.000000 csle_cluster-0.2.3/src/csle_cluster/constants/constants.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:16:32.434630 csle_cluster-0.2.3/src/csle_cluster.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 12:16:32.000000 csle_cluster-0.2.3/src/csle_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      805 2023-05-31 12:16:32.000000 csle_cluster-0.2.3/src/csle_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 12:16:32.000000 csle_cluster-0.2.3/src/csle_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-02-12 09:44:23.000000 csle_cluster-0.2.3/src/csle_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      251 2023-05-31 12:16:32.000000 csle_cluster-0.2.3/src/csle_cluster.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       13 2023-05-31 12:16:32.000000 csle_cluster-0.2.3/src/csle_cluster.egg-info/top_level.txt
```

### Comparing `csle_cluster-0.2.2/PKG-INFO` & `csle_cluster-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cluster
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.2.2/README.md` & `csle_cluster-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.2/pyproject.toml` & `csle_cluster-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.2/setup.cfg` & `csle_cluster-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	grpcio>=1.27.2
 	grpcio-tools>=1.27.2
-	csle-collector>=0.2.2
-	csle-common>=0.2.2
-	csle-ryu>=0.2.2
+	csle-collector>=0.2.3
+	csle-common>=0.2.3
+	csle-ryu>=0.2.3
 python_requires = >=3.5
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_controller.py` & `csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_controller.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager.py` & `csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_pb2.py` & `csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py` & `csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_util.py` & `csle_cluster-0.2.3/src/csle_cluster/cluster_manager/cluster_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/query_cluster_manager.py` & `csle_cluster-0.2.3/src/csle_cluster/cluster_manager/query_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.2/src/csle_cluster.egg-info/PKG-INFO` & `csle_cluster-0.2.3/src/csle_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cluster
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.2.2/src/csle_cluster.egg-info/SOURCES.txt` & `csle_cluster-0.2.3/src/csle_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

