# Comparing `tmp/highway-env-1.8.1.tar.gz` & `tmp/highway-env-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highway-env-1.8.1.tar", last modified: Wed Mar 22 19:56:40 2023, max compression
+gzip compressed data, was "highway-env-1.8.2.tar", last modified: Tue May 30 22:08:47 2023, max compression
```

## Comparing `highway-env-1.8.1.tar` & `highway-env-1.8.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.428681 highway-env-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-22 19:56:36.000000 highway-env-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-03-22 19:56:40.428681 highway-env-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-03-22 19:56:36.000000 highway-env-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.412680 highway-env-1.8.1/highway_env/
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.420681 highway-env-1.8.1/highway_env/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.420681 highway-env-1.8.1/highway_env/envs/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/common/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/common/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/common/finite_mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/common/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28642 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/common/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/exit_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/highway_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/intersection_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/lane_keeping_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/merge_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/parking_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/racetrack_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/roundabout_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/two_way_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/envs/u_turn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.424681 highway-env-1.8.1/highway_env/road/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/road/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/road/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/road/lane.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/road/regulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/road/road.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/road/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.424681 highway-env-1.8.1/highway_env/vehicle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.428681 highway-env-1.8.1/highway_env/vehicle/uncertainty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/uncertainty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/uncertainty/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-03-22 19:56:36.000000 highway-env-1.8.1/highway_env/vehicle/uncertainty/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.412680 highway-env-1.8.1/highway_env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-03-22 19:56:40.000000 highway-env-1.8.1/highway_env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-22 19:56:40.000000 highway-env-1.8.1/highway_env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:56:40.000000 highway-env-1.8.1/highway_env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-22 19:56:40.000000 highway-env-1.8.1/highway_env.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-22 19:56:40.000000 highway-env-1.8.1/highway_env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-22 19:56:40.000000 highway-env-1.8.1/highway_env.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-22 19:56:36.000000 highway-env-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-22 19:56:40.428681 highway-env-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-22 19:56:36.000000 highway-env-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.408681 highway-env-1.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:40.428681 highway-env-1.8.1/tests/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:56:36.000000 highway-env-1.8.1/tests/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-22 19:56:36.000000 highway-env-1.8.1/tests/envs/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-22 19:56:36.000000 highway-env-1.8.1/tests/envs/test_env_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-22 19:56:36.000000 highway-env-1.8.1/tests/envs/test_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-22 19:56:36.000000 highway-env-1.8.1/tests/envs/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.114263 highway-env-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 22:08:43.000000 highway-env-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-05-30 22:08:47.114263 highway-env-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-30 22:08:43.000000 highway-env-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.110263 highway-env-1.8.2/highway_env/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.110263 highway-env-1.8.2/highway_env/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.110263 highway-env-1.8.2/highway_env/envs/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/common/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/common/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/common/finite_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/common/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28724 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/common/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/exit_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/highway_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/intersection_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/lane_keeping_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/merge_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/parking_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/racetrack_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/roundabout_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/two_way_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/envs/u_turn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.110263 highway-env-1.8.2/highway_env/road/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/road/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/road/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/road/lane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/road/regulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/road/road.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/road/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.114263 highway-env-1.8.2/highway_env/vehicle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.114263 highway-env-1.8.2/highway_env/vehicle/uncertainty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/uncertainty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/uncertainty/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-05-30 22:08:43.000000 highway-env-1.8.2/highway_env/vehicle/uncertainty/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.110263 highway-env-1.8.2/highway_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-05-30 22:08:46.000000 highway-env-1.8.2/highway_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-30 22:08:47.000000 highway-env-1.8.2/highway_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:08:46.000000 highway-env-1.8.2/highway_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 22:08:46.000000 highway-env-1.8.2/highway_env.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 22:08:46.000000 highway-env-1.8.2/highway_env.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 22:08:46.000000 highway-env-1.8.2/highway_env.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 22:08:43.000000 highway-env-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-30 22:08:47.114263 highway-env-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-30 22:08:43.000000 highway-env-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.110263 highway-env-1.8.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:47.114263 highway-env-1.8.2/tests/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:43.000000 highway-env-1.8.2/tests/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 22:08:43.000000 highway-env-1.8.2/tests/envs/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-30 22:08:43.000000 highway-env-1.8.2/tests/envs/test_env_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-30 22:08:43.000000 highway-env-1.8.2/tests/envs/test_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-30 22:08:43.000000 highway-env-1.8.2/tests/envs/test_time.py
```

### Comparing `highway-env-1.8.1/LICENSE` & `highway-env-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/PKG-INFO` & `highway-env-1.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: highway-env
-Version: 1.8.1
+Version: 1.8.2
 Summary: An environment for simulated highway driving tasks.
 Home-page: https://github.com/eleurent/highway-env
 Author: Edouard Leurent
 Author-email: eleurent@gmail.com
 License: MIT
 Description: # highway-env
         
         [![build](https://github.com/eleurent/highway-env/workflows/build/badge.svg)](https://github.com/eleurent/highway-env/actions?query=workflow%3Abuild)
-        [![Documentation Status](https://readthedocs.org/projects/highway-env/badge/?version=latest)](https://highway-env.readthedocs.io/en/latest/?badge=latest)
+        [![Documentation Status](https://github.com/Farama-Foundation/HighwayEnv/actions/workflows/build-docs-dev.yml/badge.svg)](https://farama-foundation.github.io/HighwayEnv/)
         [![Downloads](https://img.shields.io/pypi/dm/highway-env)](https://pypi.org/project/highway-env/)
         [![Codacy Badge](https://api.codacy.com/project/badge/Grade/63847d9328f64fce9c137b03fcafcc27)](https://app.codacy.com/manual/eleurent/highway-env?utm_source=github.com&utm_medium=referral&utm_content=eleurent/highway-env&utm_campaign=Badge_Grade_Dashboard)
-        [![Coverage](https://codecov.io/gh/eleurent/highway-env/branch/master/graph/badge.svg)](https://codecov.io/gh/eleurent/highway-env)
         [![GitHub contributors](https://img.shields.io/github/contributors/eleurent/highway-env)](https://github.com/eleurent/highway-env/graphs/contributors)
-        [![Environments](https://img.shields.io/github/search/eleurent/highway-env/import%20filename:*_env%20path:highway_env/envs?label=environments)](#the-environments)
+        
         
         A collection of environments for *autonomous driving* and tactical decision-making tasks
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/eleurent/highway-env/master/../gh-media/docs/media/highway-env.gif?raw=true"><br/>
             <em>An episode of one of the environments available in highway-env.</em>
         </p>
@@ -109,15 +108,15 @@
         </p>
         
         
         ## Examples of agents
         
         Agents solving the `highway-env` environments are available in the [eleurent/rl-agents](https://github.com/eleurent/rl-agents) and [DLR-RM/stable-baselines3](https://github.com/DLR-RM/stable-baselines3) repositories.
         
-        See the [documentation](https://highway-env.readthedocs.io/en/latest/quickstart.html#training-an-agent) for some examples and notebooks.
+        See the [documentation](https://farama-foundation.github.io/HighwayEnv/quickstart/#training-an-agent) for some examples and notebooks.
         
         ### [Deep Q-Network](https://github.com/eleurent/rl-agents/tree/master/rl_agents/agents/deep_q_network)
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/eleurent/highway-env/master/../gh-media/docs/media/dqn.gif?raw=true"><br/>
             <em>The DQN agent solving highway-v0.</em>
         </p>
@@ -158,26 +157,26 @@
         `pip install highway-env`
         
         ## Usage
         
         ```python
         import gymnasium as gym
         
-        env = gym.make("highway-v0")
+        env = gym.make('highway-v0', render_mode='human')
         
+        obs, info = env.reset()
         done = truncated = False
         while not (done or truncated):
             action = ... # Your agent code here
             obs, reward, done, truncated, info = env.step(action)
-            env.render()
         ```
         
         ## Documentation
         
-        Read the [documentation online](https://highway-env.readthedocs.io/).
+        Read the [documentation online](https://farama-foundation.github.io/HighwayEnv/).
         
         ## Citing
         
         If you use the project in your work, please consider citing it with:
         ```bibtex
         @misc{highway-env,
           author = {Leurent, Edouard},
@@ -215,16 +214,18 @@
         *   [Corner Case Generation and Analysis for Safety Assessment of Autonomous Vehicles](https://arxiv.org/abs/2102.03483) (Feb 2021)
         *   [Intelligent driving intelligence test for autonomous vehicles with naturalistic and adversarial environment](https://www.nature.com/articles/s41467-021-21007-8) (Feb 2021)
         *   [Building Safer Autonomous Agents by Leveraging Risky Driving Behavior Knowledge](https://arxiv.org/abs/2103.10245)
         *   [Quick Learner Automated Vehicle Adapting its Roadmanship to Varying Traffic Cultures with Meta Reinforcement Learning](https://arxiv.org/abs/2104.08876) (Apr 2021)
         *   [Deep Multi-agent Reinforcement Learning for Highway On-Ramp Merging in Mixed Traffic](https://arxiv.org/abs/2105.05701) (May 2021)
         *   [Accelerated Policy Evaluation: Learning Adversarial Environments with Adaptive Importance Sampling](https://arxiv.org/abs/2106.10566) (Jun 2021)
         *   [Learning Interaction-aware Guidance Policies for Motion Planning in Dense Traffic Scenarios](https://arxiv.org/abs/2107.04538) (Jul 2021)
+        *   [Automatic Overtaking on Two-way Roads with Vehicle Interactions Based on Proximal Policy Optimization](https://ieeexplore.ieee.org/abstract/document/9575954) (Jul 2021)
         *   [Robust Predictable Control](https://arxiv.org/abs/2109.03214) (Sep 2021)
         *   [Improving Robustness of Deep Reinforcement Learning Agents: Environment Attack based on the Critic Network](https://ieeexplore.ieee.org/document/9892901) (Jul 2022)
+        *   [Autonomous Highway Merging in Mixed Traffic Using Reinforcement Learning and Motion Predictive Safety Controller](https://ieeexplore.ieee.org/document/9921741) (Oct 2022)
         
         PhD theses
         *   [Reinforcement learning for Dialogue Systems optimization with user adaptation](https://hal.inria.fr/tel-02422691/) (2019)
         *   [Safe and Efficient Reinforcement Learning for Behavioural Planning in Autonomous Driving](https://hal.inria.fr/tel-03035705/) (2020)
         *   [Many-agent Reinforcement Learning](https://discovery.ucl.ac.uk/id/eprint/10124273/) (2021)
         
         Master theses
```

### Comparing `highway-env-1.8.1/README.md` & `highway-env-1.8.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # highway-env
 
 [![build](https://github.com/eleurent/highway-env/workflows/build/badge.svg)](https://github.com/eleurent/highway-env/actions?query=workflow%3Abuild)
-[![Documentation Status](https://readthedocs.org/projects/highway-env/badge/?version=latest)](https://highway-env.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://github.com/Farama-Foundation/HighwayEnv/actions/workflows/build-docs-dev.yml/badge.svg)](https://farama-foundation.github.io/HighwayEnv/)
 [![Downloads](https://img.shields.io/pypi/dm/highway-env)](https://pypi.org/project/highway-env/)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/63847d9328f64fce9c137b03fcafcc27)](https://app.codacy.com/manual/eleurent/highway-env?utm_source=github.com&utm_medium=referral&utm_content=eleurent/highway-env&utm_campaign=Badge_Grade_Dashboard)
-[![Coverage](https://codecov.io/gh/eleurent/highway-env/branch/master/graph/badge.svg)](https://codecov.io/gh/eleurent/highway-env)
 [![GitHub contributors](https://img.shields.io/github/contributors/eleurent/highway-env)](https://github.com/eleurent/highway-env/graphs/contributors)
-[![Environments](https://img.shields.io/github/search/eleurent/highway-env/import%20filename:*_env%20path:highway_env/envs?label=environments)](#the-environments)
+
 
 A collection of environments for *autonomous driving* and tactical decision-making tasks
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/eleurent/highway-env/master/../gh-media/docs/media/highway-env.gif?raw=true"><br/>
     <em>An episode of one of the environments available in highway-env.</em>
 </p>
@@ -101,15 +100,15 @@
 </p>
 
 
 ## Examples of agents
 
 Agents solving the `highway-env` environments are available in the [eleurent/rl-agents](https://github.com/eleurent/rl-agents) and [DLR-RM/stable-baselines3](https://github.com/DLR-RM/stable-baselines3) repositories.
 
-See the [documentation](https://highway-env.readthedocs.io/en/latest/quickstart.html#training-an-agent) for some examples and notebooks.
+See the [documentation](https://farama-foundation.github.io/HighwayEnv/quickstart/#training-an-agent) for some examples and notebooks.
 
 ### [Deep Q-Network](https://github.com/eleurent/rl-agents/tree/master/rl_agents/agents/deep_q_network)
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/eleurent/highway-env/master/../gh-media/docs/media/dqn.gif?raw=true"><br/>
     <em>The DQN agent solving highway-v0.</em>
 </p>
@@ -150,26 +149,26 @@
 `pip install highway-env`
 
 ## Usage
 
 ```python
 import gymnasium as gym
 
-env = gym.make("highway-v0")
+env = gym.make('highway-v0', render_mode='human')
 
+obs, info = env.reset()
 done = truncated = False
 while not (done or truncated):
     action = ... # Your agent code here
     obs, reward, done, truncated, info = env.step(action)
-    env.render()
 ```
 
 ## Documentation
 
-Read the [documentation online](https://highway-env.readthedocs.io/).
+Read the [documentation online](https://farama-foundation.github.io/HighwayEnv/).
 
 ## Citing
 
 If you use the project in your work, please consider citing it with:
 ```bibtex
 @misc{highway-env,
   author = {Leurent, Edouard},
@@ -207,16 +206,18 @@
 *   [Corner Case Generation and Analysis for Safety Assessment of Autonomous Vehicles](https://arxiv.org/abs/2102.03483) (Feb 2021)
 *   [Intelligent driving intelligence test for autonomous vehicles with naturalistic and adversarial environment](https://www.nature.com/articles/s41467-021-21007-8) (Feb 2021)
 *   [Building Safer Autonomous Agents by Leveraging Risky Driving Behavior Knowledge](https://arxiv.org/abs/2103.10245)
 *   [Quick Learner Automated Vehicle Adapting its Roadmanship to Varying Traffic Cultures with Meta Reinforcement Learning](https://arxiv.org/abs/2104.08876) (Apr 2021)
 *   [Deep Multi-agent Reinforcement Learning for Highway On-Ramp Merging in Mixed Traffic](https://arxiv.org/abs/2105.05701) (May 2021)
 *   [Accelerated Policy Evaluation: Learning Adversarial Environments with Adaptive Importance Sampling](https://arxiv.org/abs/2106.10566) (Jun 2021)
 *   [Learning Interaction-aware Guidance Policies for Motion Planning in Dense Traffic Scenarios](https://arxiv.org/abs/2107.04538) (Jul 2021)
+*   [Automatic Overtaking on Two-way Roads with Vehicle Interactions Based on Proximal Policy Optimization](https://ieeexplore.ieee.org/abstract/document/9575954) (Jul 2021)
 *   [Robust Predictable Control](https://arxiv.org/abs/2109.03214) (Sep 2021)
 *   [Improving Robustness of Deep Reinforcement Learning Agents: Environment Attack based on the Critic Network](https://ieeexplore.ieee.org/document/9892901) (Jul 2022)
+*   [Autonomous Highway Merging in Mixed Traffic Using Reinforcement Learning and Motion Predictive Safety Controller](https://ieeexplore.ieee.org/document/9921741) (Oct 2022)
 
 PhD theses
 *   [Reinforcement learning for Dialogue Systems optimization with user adaptation](https://hal.inria.fr/tel-02422691/) (2019)
 *   [Safe and Efficient Reinforcement Learning for Behavioural Planning in Autonomous Driving](https://hal.inria.fr/tel-03035705/) (2020)
 *   [Many-agent Reinforcement Learning](https://discovery.ucl.ac.uk/id/eprint/10124273/) (2021)
 
 Master theses
```

### Comparing `highway-env-1.8.1/highway_env/__init__.py` & `highway-env-1.8.2/highway_env/__init__.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/common/abstract.py` & `highway-env-1.8.2/highway_env/envs/common/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         self.time = 0  # Simulation time
         self.steps = 0  # Actions performed
         self.done = False
 
         # Rendering
         self.viewer = None
         self._record_video_wrapper = None
+        assert render_mode is None or render_mode in self.metadata["render_modes"]
         self.render_mode = render_mode
         self.enable_auto_render = False
 
         self.reset()
 
     @property
     def vehicle(self) -> Vehicle:
@@ -201,14 +202,16 @@
         self.define_spaces()  # First, to set the controlled vehicle class depending on action space
         self.time = self.steps = 0
         self.done = False
         self._reset()
         self.define_spaces()  # Second, to link the obs and actions to the vehicles once the scene is created
         obs = self.observation_type.observe()
         info = self._info(obs, action=self.action_space.sample())
+        if self.render_mode == 'human':
+            self.render()
         return obs, info
 
     def _reset(self) -> None:
         """
         Reset the scene: roads and vehicles.
 
         This method must be overloaded by the environments.
@@ -232,14 +235,16 @@
         self._simulate(action)
 
         obs = self.observation_type.observe()
         reward = self._reward(action)
         terminated = self._is_terminated()
         truncated = self._is_truncated()
         info = self._info(obs, action)
+        if self.render_mode == 'human':
+            self.render()
 
         return obs, reward, terminated, truncated, info
 
     def _simulate(self, action: Optional[Action] = None) -> None:
         """Perform several steps of simulation with constant action."""
         frames = int(self.config["simulation_frequency"] // self.config["policy_frequency"])
         for frame in range(frames):
@@ -256,31 +261,38 @@
             # Automatically render intermediate simulation steps if a viewer has been launched
             # Ignored if the rendering is done offscreen
             if frame < frames - 1:  # Last frame will be rendered through env.render() as usual
                 self._automatic_rendering()
 
         self.enable_auto_render = False
 
-    def render(self, mode: str = 'rgb_array') -> Optional[np.ndarray]:
+    def render(self) -> Optional[np.ndarray]:
         """
         Render the environment.
 
         Create a viewer if none exists, and use it to render an image.
-        :param mode: the rendering mode
         """
+        if self.render_mode is None:
+            assert self.spec is not None
+            gym.logger.warn(
+                "You are calling render method without specifying any render mode. "
+                "You can specify the render_mode at initialization, "
+                f'e.g. gym.make("{self.spec.id}", render_mode="rgb_array")'
+            )
+            return
         if self.viewer is None:
             self.viewer = EnvViewer(self)
 
         self.enable_auto_render = True
 
         self.viewer.display()
 
         if not self.viewer.offscreen:
             self.viewer.handle_events()
-        if mode == 'rgb_array':
+        if self.render_mode == 'rgb_array':
             image = self.viewer.get_image()
             return image
 
     def close(self) -> None:
         """
         Close the environment.
 
@@ -306,15 +318,15 @@
         If a RecordVideo wrapper has been set, use it to capture intermediate frames.
         """
         if self.viewer is not None and self.enable_auto_render:
 
             if self._record_video_wrapper and self._record_video_wrapper.video_recorder:
                 self._record_video_wrapper.video_recorder.capture_frame()
             else:
-                self.render(self.render_mode)
+                self.render()
 
     def simplify(self) -> 'AbstractEnv':
         """
         Return a simplified copy of the environment where distant vehicles have been removed from the road.
 
         This is meant to lower the policy computational load while preserving the optimal actions set.
```

### Comparing `highway-env-1.8.1/highway_env/envs/common/action.py` & `highway-env-1.8.2/highway_env/envs/common/action.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/common/finite_mdp.py` & `highway-env-1.8.2/highway_env/envs/common/finite_mdp.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/common/graphics.py` & `highway-env-1.8.2/highway_env/envs/common/graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,63 +13,67 @@
 
 
 class EnvViewer(object):
 
     """A viewer to render a highway driving environment."""
 
     SAVE_IMAGES = False
+    agent_display = None
 
     def __init__(self, env: 'AbstractEnv', config: Optional[dict] = None) -> None:
         self.env = env
         self.config = config or env.config
         self.offscreen = self.config["offscreen_rendering"]
+        self.observer_vehicle = None
+        self.agent_surface = None
+        self.vehicle_trajectory = None
+        self.frame = 0
+        self.directory = None
 
         pygame.init()
         pygame.display.set_caption("Highway-env")
         panel_size = (self.config["screen_width"], self.config["screen_height"])
 
         # A display is not mandatory to draw things. Ignoring the display.set_mode()
         # instruction allows the drawing to be done on surfaces without
         # handling a screen display, useful for e.g. cloud computing
         if not self.offscreen:
             self.screen = pygame.display.set_mode([self.config["screen_width"], self.config["screen_height"]])
+        if self.agent_display:
+            self.extend_display()
         self.sim_surface = WorldSurface(panel_size, 0, pygame.Surface(panel_size))
         self.sim_surface.scaling = self.config.get("scaling", self.sim_surface.INITIAL_SCALING)
         self.sim_surface.centering_position = self.config.get("centering_position", self.sim_surface.INITIAL_CENTERING)
         self.clock = pygame.time.Clock()
 
         self.enabled = True
         if os.environ.get("SDL_VIDEODRIVER", None) == "dummy":
             self.enabled = False
 
-        self.observer_vehicle = None
-        self.agent_display = None
-        self.agent_surface = None
-        self.vehicle_trajectory = None
-        self.frame = 0
-        self.directory = None
-
     def set_agent_display(self, agent_display: Callable) -> None:
         """
         Set a display callback provided by an agent
 
         So that they can render their behaviour on a dedicated agent surface, or even on the simulation surface.
 
         :param agent_display: a callback provided by the agent to display on surfaces
         """
-        if self.agent_display is None:
-            if not self.offscreen:
-                if self.config["screen_width"] > self.config["screen_height"]:
-                    self.screen = pygame.display.set_mode((self.config["screen_width"],
-                                                           2 * self.config["screen_height"]))
-                else:
-                    self.screen = pygame.display.set_mode((2 * self.config["screen_width"],
-                                                           self.config["screen_height"]))
-            self.agent_surface = pygame.Surface((self.config["screen_width"], self.config["screen_height"]))
-        self.agent_display = agent_display
+        if EnvViewer.agent_display is None:
+            self.extend_display()
+        EnvViewer.agent_display = agent_display
+
+    def extend_display(self) -> None:
+        if not self.offscreen:
+            if self.config["screen_width"] > self.config["screen_height"]:
+                self.screen = pygame.display.set_mode((self.config["screen_width"],
+                                                       2 * self.config["screen_height"]))
+            else:
+                self.screen = pygame.display.set_mode((2 * self.config["screen_width"],
+                                                       self.config["screen_height"]))
+        self.agent_surface = pygame.Surface((self.config["screen_width"], self.config["screen_height"]))
 
     def set_agent_action_sequence(self, actions: List['Action']) -> None:
         """
         Set the sequence of actions chosen by the agent, so that it can be displayed
 
         :param actions: list of action, following the env's action space specification
         """
@@ -106,16 +110,16 @@
 
         RoadGraphics.display_road_objects(
             self.env.road,
             self.sim_surface,
             offscreen=self.offscreen
         )
 
-        if self.agent_display:
-            self.agent_display(self.agent_surface, self.sim_surface)
+        if EnvViewer.agent_display:
+            EnvViewer.agent_display(self.agent_surface, self.sim_surface)
             if not self.offscreen:
                 if self.config["screen_width"] > self.config["screen_height"]:
                     self.screen.blit(self.agent_surface, (0, self.config["screen_height"]))
                 else:
                     self.screen.blit(self.agent_surface, (self.config["screen_width"], 0))
 
         RoadGraphics.display_traffic(
```

### Comparing `highway-env-1.8.1/highway_env/envs/common/observation.py` & `highway-env-1.8.2/highway_env/envs/common/observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,14 +152,15 @@
                  see_behind: bool = False,
                  observe_intentions: bool = False,
                  **kwargs: dict) -> None:
         """
         :param env: The environment to observe
         :param features: Names of features used in the observation
         :param vehicles_count: Number of observed vehicles
+        :param features_range: a dict mapping a feature name to [min, max] values
         :param absolute: Use absolute coordinates
         :param order: Order of observed vehicles. Values: sorted, shuffled
         :param normalize: Should the observation be normalized
         :param clip: Should the value be clipped in the desired range
         :param see_behind: Should the observation contains the vehicles behind
         :param observe_intentions: Observe the destinations of other vehicles
         """
```

### Comparing `highway-env-1.8.1/highway_env/envs/exit_env.py` & `highway-env-1.8.2/highway_env/envs/exit_env.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/highway_env.py` & `highway-env-1.8.2/highway_env/envs/highway_env.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/intersection_env.py` & `highway-env-1.8.2/highway_env/envs/intersection_env.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/lane_keeping_env.py` & `highway-env-1.8.2/highway_env/envs/lane_keeping_env.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/merge_env.py` & `highway-env-1.8.2/highway_env/envs/merge_env.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/parking_env.py` & `highway-env-1.8.2/highway_env/envs/parking_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 "normalize": False
             },
             "action": {
                 "type": "ContinuousAction"
             },
             "reward_weights": [1, 0.3, 0, 0, 0.02, 0.02],
             "success_goal_reward": 0.12,
-            "collision_reward": -500,
+            "collision_reward": -5,
             "steering_range": np.deg2rad(45),
             "simulation_frequency": 15,
             "policy_frequency": 5,
             "duration": 100,
             "screen_width": 600,
             "screen_height": 300,
             "centering_position": [0.5, 0.5],
@@ -169,24 +169,26 @@
         for v in self.road.vehicles:  # Prevent early collisions
             if v is not self.vehicle and (
                     np.linalg.norm(v.position - self.goal.position) < 20 or
                     np.linalg.norm(v.position - self.vehicle.position) < 20):
                 self.road.vehicles.remove(v)
 
         # Walls
-        for y in [-21, 21]:
-            obstacle = Obstacle(self.road, [0, y])
-            obstacle.LENGTH, obstacle.WIDTH = (70, 1)
-            obstacle.diagonal = np.sqrt(obstacle.LENGTH**2 + obstacle.WIDTH**2)
-            self.road.objects.append(obstacle)
-        for x in [-35, 35]:
-            obstacle = Obstacle(self.road, [x, 0], heading=np.pi / 2)
-            obstacle.LENGTH, obstacle.WIDTH = (42, 1)
-            obstacle.diagonal = np.sqrt(obstacle.LENGTH**2 + obstacle.WIDTH**2)
-            self.road.objects.append(obstacle)
+        if self.config['add_walls']:
+            width, height = 70, 42
+            for y in [-height / 2, height / 2]:
+                obstacle = Obstacle(self.road, [0, y])
+                obstacle.LENGTH, obstacle.WIDTH = (width, 1)
+                obstacle.diagonal = np.sqrt(obstacle.LENGTH**2 + obstacle.WIDTH**2)
+                self.road.objects.append(obstacle)
+            for x in [-width / 2, width / 2]:
+                obstacle = Obstacle(self.road, [x, 0], heading=np.pi / 2)
+                obstacle.LENGTH, obstacle.WIDTH = (height, 1)
+                obstacle.diagonal = np.sqrt(obstacle.LENGTH**2 + obstacle.WIDTH**2)
+                self.road.objects.append(obstacle)
 
     def compute_reward(self, achieved_goal: np.ndarray, desired_goal: np.ndarray, info: dict, p: float = 0.5) -> float:
         """
         Proximity to the goal is rewarded
 
         We use a weighted p-norm
```

### Comparing `highway-env-1.8.1/highway_env/envs/racetrack_env.py` & `highway-env-1.8.2/highway_env/envs/racetrack_env.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/roundabout_env.py` & `highway-env-1.8.2/highway_env/envs/roundabout_env.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/two_way_env.py` & `highway-env-1.8.2/highway_env/envs/two_way_env.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/envs/u_turn_env.py` & `highway-env-1.8.2/highway_env/envs/u_turn_env.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/interval.py` & `highway-env-1.8.2/highway_env/interval.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/road/graphics.py` & `highway-env-1.8.2/highway_env/road/graphics.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/road/lane.py` & `highway-env-1.8.2/highway_env/road/lane.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/road/regulation.py` & `highway-env-1.8.2/highway_env/road/regulation.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/road/road.py` & `highway-env-1.8.2/highway_env/road/road.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/road/spline.py` & `highway-env-1.8.2/highway_env/road/spline.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/utils.py` & `highway-env-1.8.2/highway_env/utils.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/vehicle/behavior.py` & `highway-env-1.8.2/highway_env/vehicle/behavior.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,19 @@
                             reason about other vehicles behaviors even though they may not IDMs.
         :param front_vehicle: the vehicle preceding the ego-vehicle
         :param rear_vehicle: the vehicle following the ego-vehicle
         :return: the acceleration command for the ego-vehicle [m/s2]
         """
         if not ego_vehicle or not isinstance(ego_vehicle, Vehicle):
             return 0
-        ego_target_speed = abs(utils.not_zero(getattr(ego_vehicle, "target_speed", 0)))
-        acceleration = self.COMFORT_ACC_MAX * (
-                1 - np.power(max(ego_vehicle.speed, 0) / ego_target_speed, self.DELTA))
+        ego_target_speed = getattr(ego_vehicle, "target_speed", 0)
+        if ego_vehicle.lane and ego_vehicle.lane.speed_limit is not None:
+            ego_target_speed = np.clip(ego_target_speed, 0, ego_vehicle.lane.speed_limit)
+        acceleration = self.COMFORT_ACC_MAX * (1 - np.power(
+            max(ego_vehicle.speed, 0) / abs(utils.not_zero(ego_target_speed)), self.DELTA))
 
         if front_vehicle:
             d = ego_vehicle.lane_distance_to(front_vehicle)
             acceleration -= self.COMFORT_ACC_MAX * \
                 np.power(self.desired_gap(ego_vehicle, front_vehicle) / utils.not_zero(d), 2)
         return acceleration
```

### Comparing `highway-env-1.8.1/highway_env/vehicle/controller.py` & `highway-env-1.8.2/highway_env/vehicle/controller.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/vehicle/dynamics.py` & `highway-env-1.8.2/highway_env/vehicle/dynamics.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/vehicle/graphics.py` & `highway-env-1.8.2/highway_env/vehicle/graphics.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/vehicle/kinematics.py` & `highway-env-1.8.2/highway_env/vehicle/kinematics.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/vehicle/objects.py` & `highway-env-1.8.2/highway_env/vehicle/objects.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/vehicle/uncertainty/estimation.py` & `highway-env-1.8.2/highway_env/vehicle/uncertainty/estimation.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env/vehicle/uncertainty/prediction.py` & `highway-env-1.8.2/highway_env/vehicle/uncertainty/prediction.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/highway_env.egg-info/PKG-INFO` & `highway-env-1.8.2/highway_env.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: highway-env
-Version: 1.8.1
+Version: 1.8.2
 Summary: An environment for simulated highway driving tasks.
 Home-page: https://github.com/eleurent/highway-env
 Author: Edouard Leurent
 Author-email: eleurent@gmail.com
 License: MIT
 Description: # highway-env
         
         [![build](https://github.com/eleurent/highway-env/workflows/build/badge.svg)](https://github.com/eleurent/highway-env/actions?query=workflow%3Abuild)
-        [![Documentation Status](https://readthedocs.org/projects/highway-env/badge/?version=latest)](https://highway-env.readthedocs.io/en/latest/?badge=latest)
+        [![Documentation Status](https://github.com/Farama-Foundation/HighwayEnv/actions/workflows/build-docs-dev.yml/badge.svg)](https://farama-foundation.github.io/HighwayEnv/)
         [![Downloads](https://img.shields.io/pypi/dm/highway-env)](https://pypi.org/project/highway-env/)
         [![Codacy Badge](https://api.codacy.com/project/badge/Grade/63847d9328f64fce9c137b03fcafcc27)](https://app.codacy.com/manual/eleurent/highway-env?utm_source=github.com&utm_medium=referral&utm_content=eleurent/highway-env&utm_campaign=Badge_Grade_Dashboard)
-        [![Coverage](https://codecov.io/gh/eleurent/highway-env/branch/master/graph/badge.svg)](https://codecov.io/gh/eleurent/highway-env)
         [![GitHub contributors](https://img.shields.io/github/contributors/eleurent/highway-env)](https://github.com/eleurent/highway-env/graphs/contributors)
-        [![Environments](https://img.shields.io/github/search/eleurent/highway-env/import%20filename:*_env%20path:highway_env/envs?label=environments)](#the-environments)
+        
         
         A collection of environments for *autonomous driving* and tactical decision-making tasks
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/eleurent/highway-env/master/../gh-media/docs/media/highway-env.gif?raw=true"><br/>
             <em>An episode of one of the environments available in highway-env.</em>
         </p>
@@ -109,15 +108,15 @@
         </p>
         
         
         ## Examples of agents
         
         Agents solving the `highway-env` environments are available in the [eleurent/rl-agents](https://github.com/eleurent/rl-agents) and [DLR-RM/stable-baselines3](https://github.com/DLR-RM/stable-baselines3) repositories.
         
-        See the [documentation](https://highway-env.readthedocs.io/en/latest/quickstart.html#training-an-agent) for some examples and notebooks.
+        See the [documentation](https://farama-foundation.github.io/HighwayEnv/quickstart/#training-an-agent) for some examples and notebooks.
         
         ### [Deep Q-Network](https://github.com/eleurent/rl-agents/tree/master/rl_agents/agents/deep_q_network)
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/eleurent/highway-env/master/../gh-media/docs/media/dqn.gif?raw=true"><br/>
             <em>The DQN agent solving highway-v0.</em>
         </p>
@@ -158,26 +157,26 @@
         `pip install highway-env`
         
         ## Usage
         
         ```python
         import gymnasium as gym
         
-        env = gym.make("highway-v0")
+        env = gym.make('highway-v0', render_mode='human')
         
+        obs, info = env.reset()
         done = truncated = False
         while not (done or truncated):
             action = ... # Your agent code here
             obs, reward, done, truncated, info = env.step(action)
-            env.render()
         ```
         
         ## Documentation
         
-        Read the [documentation online](https://highway-env.readthedocs.io/).
+        Read the [documentation online](https://farama-foundation.github.io/HighwayEnv/).
         
         ## Citing
         
         If you use the project in your work, please consider citing it with:
         ```bibtex
         @misc{highway-env,
           author = {Leurent, Edouard},
@@ -215,16 +214,18 @@
         *   [Corner Case Generation and Analysis for Safety Assessment of Autonomous Vehicles](https://arxiv.org/abs/2102.03483) (Feb 2021)
         *   [Intelligent driving intelligence test for autonomous vehicles with naturalistic and adversarial environment](https://www.nature.com/articles/s41467-021-21007-8) (Feb 2021)
         *   [Building Safer Autonomous Agents by Leveraging Risky Driving Behavior Knowledge](https://arxiv.org/abs/2103.10245)
         *   [Quick Learner Automated Vehicle Adapting its Roadmanship to Varying Traffic Cultures with Meta Reinforcement Learning](https://arxiv.org/abs/2104.08876) (Apr 2021)
         *   [Deep Multi-agent Reinforcement Learning for Highway On-Ramp Merging in Mixed Traffic](https://arxiv.org/abs/2105.05701) (May 2021)
         *   [Accelerated Policy Evaluation: Learning Adversarial Environments with Adaptive Importance Sampling](https://arxiv.org/abs/2106.10566) (Jun 2021)
         *   [Learning Interaction-aware Guidance Policies for Motion Planning in Dense Traffic Scenarios](https://arxiv.org/abs/2107.04538) (Jul 2021)
+        *   [Automatic Overtaking on Two-way Roads with Vehicle Interactions Based on Proximal Policy Optimization](https://ieeexplore.ieee.org/abstract/document/9575954) (Jul 2021)
         *   [Robust Predictable Control](https://arxiv.org/abs/2109.03214) (Sep 2021)
         *   [Improving Robustness of Deep Reinforcement Learning Agents: Environment Attack based on the Critic Network](https://ieeexplore.ieee.org/document/9892901) (Jul 2022)
+        *   [Autonomous Highway Merging in Mixed Traffic Using Reinforcement Learning and Motion Predictive Safety Controller](https://ieeexplore.ieee.org/document/9921741) (Oct 2022)
         
         PhD theses
         *   [Reinforcement learning for Dialogue Systems optimization with user adaptation](https://hal.inria.fr/tel-02422691/) (2019)
         *   [Safe and Efficient Reinforcement Learning for Behavioural Planning in Autonomous Driving](https://hal.inria.fr/tel-03035705/) (2020)
         *   [Many-agent Reinforcement Learning](https://discovery.ucl.ac.uk/id/eprint/10124273/) (2021)
         
         Master theses
```

### Comparing `highway-env-1.8.1/highway_env.egg-info/SOURCES.txt` & `highway-env-1.8.2/highway_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/setup.cfg` & `highway-env-1.8.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = highway-env
-version = 1.8.1
+version = 1.8.2
 author = Edouard Leurent
 author_email = eleurent@gmail.com
 description = An environment for simulated highway driving tasks.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/eleurent/highway-env
 license = MIT
```

### Comparing `highway-env-1.8.1/tests/envs/test_actions.py` & `highway-env-1.8.2/tests/envs/test_actions.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/tests/envs/test_env_preprocessors.py` & `highway-env-1.8.2/tests/envs/test_env_preprocessors.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/tests/envs/test_gym.py` & `highway-env-1.8.2/tests/envs/test_gym.py`

 * *Files identical despite different names*

### Comparing `highway-env-1.8.1/tests/envs/test_time.py` & `highway-env-1.8.2/tests/envs/test_time.py`

 * *Files identical despite different names*

