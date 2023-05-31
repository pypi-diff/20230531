# Comparing `tmp/csle_ryu-0.2.1.tar.gz` & `tmp/csle_ryu-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_ryu-0.2.1.tar", last modified: Wed May 31 11:22:48 2023, max compression
+gzip compressed data, was "csle_ryu-0.2.2.tar", last modified: Wed May 31 11:45:48 2023, max compression
```

## Comparing `csle_ryu-0.2.1.tar` & `csle_ryu-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:22:48.686681 csle_ryu-0.2.1/
--rw-r--r--   0 kimham     (501) staff       (20)      639 2023-05-31 11:22:48.686865 csle_ryu-0.2.1/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3913 2023-01-11 18:45:47.000000 csle_ryu-0.2.1/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      669 2023-02-12 08:59:32.000000 csle_ryu-0.2.1/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1244 2023-05-31 11:22:48.687808 csle_ryu-0.2.1/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_ryu-0.2.1/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:22:48.672407 csle_ryu-0.2.1/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:22:48.676263 csle_ryu-0.2.1/src/csle_ryu/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_ryu-0.2.1/src/csle_ryu/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:22:38.000000 csle_ryu-0.2.1/src/csle_ryu/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:22:48.679866 csle_ryu-0.2.1/src/csle_ryu/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.1/src/csle_ryu/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2484 2023-03-31 11:14:06.000000 csle_ryu-0.2.1/src/csle_ryu/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:22:48.681475 csle_ryu-0.2.1/src/csle_ryu/controllers/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.1/src/csle_ryu/controllers/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     8323 2022-11-28 13:00:49.000000 csle_ryu-0.2.1/src/csle_ryu/controllers/learning_switch_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    11773 2022-12-07 10:40:04.000000 csle_ryu-0.2.1/src/csle_ryu/controllers/learning_switch_stp_controller.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:22:48.685296 csle_ryu-0.2.1/src/csle_ryu/dao/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.1/src/csle_ryu/dao/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     4598 2023-03-22 11:50:26.000000 csle_ryu-0.2.1/src/csle_ryu/dao/agg_flow_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)     8629 2023-03-22 11:50:26.000000 csle_ryu-0.2.1/src/csle_ryu/dao/avg_flow_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)    15102 2023-03-22 11:50:26.000000 csle_ryu-0.2.1/src/csle_ryu/dao/avg_port_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)     7004 2023-03-22 11:50:26.000000 csle_ryu-0.2.1/src/csle_ryu/dao/flow_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)    10600 2023-03-22 11:50:26.000000 csle_ryu-0.2.1/src/csle_ryu/dao/port_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)      253 2022-11-28 13:00:49.000000 csle_ryu-0.2.1/src/csle_ryu/dao/ryu_controller_type.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:22:48.686093 csle_ryu-0.2.1/src/csle_ryu/monitor/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.1/src/csle_ryu/monitor/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    14663 2023-03-31 11:14:06.000000 csle_ryu-0.2.1/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:22:48.679245 csle_ryu-0.2.1/src/csle_ryu.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      639 2023-05-31 11:22:48.000000 csle_ryu-0.2.1/src/csle_ryu.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      873 2023-05-31 11:22:48.000000 csle_ryu-0.2.1/src/csle_ryu.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:22:48.000000 csle_ryu-0.2.1/src/csle_ryu.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:06.000000 csle_ryu-0.2.1/src/csle_ryu.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      230 2023-05-31 11:22:48.000000 csle_ryu-0.2.1/src/csle_ryu.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)        9 2023-05-31 11:22:48.000000 csle_ryu-0.2.1/src/csle_ryu.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:45:48.964332 csle_ryu-0.2.2/
+-rw-r--r--   0 kimham     (501) staff       (20)      639 2023-05-31 11:45:48.964456 csle_ryu-0.2.2/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     3913 2023-01-11 18:45:47.000000 csle_ryu-0.2.2/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      669 2023-02-12 08:59:32.000000 csle_ryu-0.2.2/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1244 2023-05-31 11:45:48.965077 csle_ryu-0.2.2/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_ryu-0.2.2/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:45:48.952087 csle_ryu-0.2.2/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:45:48.955423 csle_ryu-0.2.2/src/csle_ryu/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_ryu-0.2.2/src/csle_ryu/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:45:39.000000 csle_ryu-0.2.2/src/csle_ryu/__version__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:45:48.957965 csle_ryu-0.2.2/src/csle_ryu/constants/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.2/src/csle_ryu/constants/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2484 2023-03-31 11:14:06.000000 csle_ryu-0.2.2/src/csle_ryu/constants/constants.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:45:48.959420 csle_ryu-0.2.2/src/csle_ryu/controllers/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.2/src/csle_ryu/controllers/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8323 2022-11-28 13:00:49.000000 csle_ryu-0.2.2/src/csle_ryu/controllers/learning_switch_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11773 2022-12-07 10:40:04.000000 csle_ryu-0.2.2/src/csle_ryu/controllers/learning_switch_stp_controller.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:45:48.963116 csle_ryu-0.2.2/src/csle_ryu/dao/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.2/src/csle_ryu/dao/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4598 2023-03-22 11:50:26.000000 csle_ryu-0.2.2/src/csle_ryu/dao/agg_flow_statistic.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8629 2023-03-22 11:50:26.000000 csle_ryu-0.2.2/src/csle_ryu/dao/avg_flow_statistic.py
+-rw-r--r--   0 kimham     (501) staff       (20)    15102 2023-03-22 11:50:26.000000 csle_ryu-0.2.2/src/csle_ryu/dao/avg_port_statistic.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7004 2023-03-22 11:50:26.000000 csle_ryu-0.2.2/src/csle_ryu/dao/flow_statistic.py
+-rw-r--r--   0 kimham     (501) staff       (20)    10600 2023-03-22 11:50:26.000000 csle_ryu-0.2.2/src/csle_ryu/dao/port_statistic.py
+-rw-r--r--   0 kimham     (501) staff       (20)      253 2022-11-28 13:00:49.000000 csle_ryu-0.2.2/src/csle_ryu/dao/ryu_controller_type.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:45:48.963796 csle_ryu-0.2.2/src/csle_ryu/monitor/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.2/src/csle_ryu/monitor/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    14663 2023-03-31 11:14:06.000000 csle_ryu-0.2.2/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:45:48.957486 csle_ryu-0.2.2/src/csle_ryu.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      639 2023-05-31 11:45:48.000000 csle_ryu-0.2.2/src/csle_ryu.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      873 2023-05-31 11:45:48.000000 csle_ryu-0.2.2/src/csle_ryu.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:45:48.000000 csle_ryu-0.2.2/src/csle_ryu.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:06.000000 csle_ryu-0.2.2/src/csle_ryu.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      230 2023-05-31 11:45:48.000000 csle_ryu-0.2.2/src/csle_ryu.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        9 2023-05-31 11:45:48.000000 csle_ryu-0.2.2/src/csle_ryu.egg-info/top_level.txt
```

### Comparing `csle_ryu-0.2.1/PKG-INFO` & `csle_ryu-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_ryu
-Version: 0.2.1
+Version: 0.2.2
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.2.1/README.md` & `csle_ryu-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/pyproject.toml` & `csle_ryu-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/setup.cfg` & `csle_ryu-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-collector>=0.2.1
+	csle-collector>=0.2.2
 	ryu>=4.34
 	eventlet>=0.30.2
 	confluent-kafka>=1.9.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_ryu-0.2.1/src/csle_ryu/constants/constants.py` & `csle_ryu-0.2.2/src/csle_ryu/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/src/csle_ryu/controllers/learning_switch_controller.py` & `csle_ryu-0.2.2/src/csle_ryu/controllers/learning_switch_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/src/csle_ryu/controllers/learning_switch_stp_controller.py` & `csle_ryu-0.2.2/src/csle_ryu/controllers/learning_switch_stp_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/src/csle_ryu/dao/agg_flow_statistic.py` & `csle_ryu-0.2.2/src/csle_ryu/dao/agg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/src/csle_ryu/dao/avg_flow_statistic.py` & `csle_ryu-0.2.2/src/csle_ryu/dao/avg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/src/csle_ryu/dao/avg_port_statistic.py` & `csle_ryu-0.2.2/src/csle_ryu/dao/avg_port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/src/csle_ryu/dao/flow_statistic.py` & `csle_ryu-0.2.2/src/csle_ryu/dao/flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/src/csle_ryu/dao/port_statistic.py` & `csle_ryu-0.2.2/src/csle_ryu/dao/port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/src/csle_ryu/monitor/flow_and_port_stats_monitor.py` & `csle_ryu-0.2.2/src/csle_ryu/monitor/flow_and_port_stats_monitor.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.1/src/csle_ryu.egg-info/PKG-INFO` & `csle_ryu-0.2.2/src/csle_ryu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-ryu
-Version: 0.2.1
+Version: 0.2.2
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.2.1/src/csle_ryu.egg-info/SOURCES.txt` & `csle_ryu-0.2.2/src/csle_ryu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

