# Comparing `tmp/mentpy-0.1.0a6.tar.gz` & `tmp/mentpy-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentpy-0.1.0a6.tar", last modified: Thu May 18 18:24:44 2023, max compression
+gzip compressed data, was "mentpy-0.1.0a7.tar", last modified: Wed May 31 21:45:30 2023, max compression
```

## Comparing `mentpy-0.1.0a6.tar` & `mentpy-0.1.0a7.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.405322 mentpy-0.1.0a6/
--rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a6/LICENSE
--rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-05-18 18:24:44.404624 mentpy-0.1.0a6/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     3056 2023-05-08 04:08:41.000000 mentpy-0.1.0a6/README.md
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.357618 mentpy-0.1.0a6/mentpy/
--rw-r--r--   0 luismantilla   (501) staff       (20)      308 2023-05-18 08:23:36.000000 mentpy-0.1.0a6/mentpy/__init__.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.361788 mentpy-0.1.0a6/mentpy/gradients/
--rw-r--r--   0 luismantilla   (501) staff       (20)       33 2023-03-17 21:21:26.000000 mentpy-0.1.0a6/mentpy/gradients/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2014 2023-04-25 08:57:09.000000 mentpy-0.1.0a6/mentpy/gradients/finite_difference.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.365113 mentpy-0.1.0a6/mentpy/mbqc/
--rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a6/mentpy/mbqc/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    17441 2023-05-16 19:16:57.000000 mentpy-0.1.0a6/mentpy/mbqc/flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    30925 2023-05-17 16:21:24.000000 mentpy-0.1.0a6/mentpy/mbqc/mbqcircuit.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.367974 mentpy-0.1.0a6/mentpy/mbqc/states/
--rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-05-06 07:23:30.000000 mentpy-0.1.0a6/mentpy/mbqc/states/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      197 2023-05-06 07:23:09.000000 mentpy-0.1.0a6/mentpy/mbqc/states/aklt.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      229 2023-05-06 07:23:14.000000 mentpy-0.1.0a6/mentpy/mbqc/states/cluster.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a6/mentpy/mbqc/states/graphstate.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     7594 2023-05-18 06:03:44.000000 mentpy-0.1.0a6/mentpy/mbqc/templates.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.368944 mentpy-0.1.0a6/mentpy/noise/
--rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a6/mentpy/noise/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a6/mentpy/noise/base_noise.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.385093 mentpy-0.1.0a6/mentpy/operators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      285 2023-05-10 00:16:14.000000 mentpy-0.1.0a6/mentpy/operators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3164 2023-05-10 00:16:14.000000 mentpy-0.1.0a6/mentpy/operators/controlled_ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1599 2023-05-07 19:04:31.000000 mentpy-0.1.0a6/mentpy/operators/gates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     8139 2023-05-16 20:00:06.000000 mentpy-0.1.0a6/mentpy/operators/ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5502 2023-05-18 06:12:52.000000 mentpy-0.1.0a6/mentpy/operators/pauliop.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.388170 mentpy-0.1.0a6/mentpy/optimizers/
--rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a6/mentpy/optimizers/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3054 2023-03-22 20:56:41.000000 mentpy-0.1.0a6/mentpy/optimizers/adam.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      632 2023-03-17 21:21:26.000000 mentpy-0.1.0a6/mentpy/optimizers/base_optimizer.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      379 2023-03-17 21:21:26.000000 mentpy-0.1.0a6/mentpy/optimizers/bp_tools.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3101 2023-04-25 09:08:43.000000 mentpy-0.1.0a6/mentpy/optimizers/rcd.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2637 2023-04-15 23:00:30.000000 mentpy-0.1.0a6/mentpy/optimizers/sgd.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.395011 mentpy-0.1.0a6/mentpy/simulators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a6/mentpy/simulators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2441 2023-05-07 19:04:31.000000 mentpy-0.1.0a6/mentpy/simulators/base_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a6/mentpy/simulators/cirq_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    15323 2023-05-18 16:31:06.000000 mentpy-0.1.0a6/mentpy/simulators/np_simulator_dm.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    15668 2023-05-10 00:49:41.000000 mentpy-0.1.0a6/mentpy/simulators/np_simulator_sv.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2678 2023-05-18 06:35:37.000000 mentpy-0.1.0a6/mentpy/simulators/pattern_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5677 2023-05-18 08:04:21.000000 mentpy-0.1.0a6/mentpy/simulators/pennylane_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1254 2023-04-25 08:57:09.000000 mentpy-0.1.0a6/mentpy/simulators/qiskit_simulators.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.398861 mentpy-0.1.0a6/mentpy/utils/
--rw-r--r--   0 luismantilla   (501) staff       (20)      160 2023-05-18 08:23:19.000000 mentpy-0.1.0a6/mentpy/utils/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     6673 2023-04-25 08:57:09.000000 mentpy-0.1.0a6/mentpy/utils/expressivity.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a6/mentpy/utils/flow_space.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a6/mentpy/utils/generate_data.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-05-06 07:13:49.000000 mentpy-0.1.0a6/mentpy/utils/lc_equivalence.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     6584 2023-05-18 06:20:35.000000 mentpy-0.1.0a6/mentpy/utils/lie_algebra.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      108 2023-05-18 08:28:37.000000 mentpy-0.1.0a6/mentpy/utils/math.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.360815 mentpy-0.1.0a6/mentpy.egg-info/
--rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-05-18 18:24:44.000000 mentpy-0.1.0a6/mentpy.egg-info/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     1430 2023-05-18 18:24:44.000000 mentpy-0.1.0a6/mentpy.egg-info/SOURCES.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-05-18 18:24:44.000000 mentpy-0.1.0a6/mentpy.egg-info/dependency_links.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-05-18 18:24:44.000000 mentpy-0.1.0a6/mentpy.egg-info/requires.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-05-18 18:24:44.000000 mentpy-0.1.0a6/mentpy.egg-info/top_level.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-05-18 18:24:44.405468 mentpy-0.1.0a6/setup.cfg
--rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-05-18 18:22:41.000000 mentpy-0.1.0a6/setup.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 18:24:44.403444 mentpy-0.1.0a6/tests/
--rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a6/tests/test_flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a6/tests/test_graph_state.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a6/tests/test_mbqc_templates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2110 2023-05-18 06:15:48.000000 mentpy-0.1.0a6/tests/test_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.806967 mentpy-0.1.0a7/
+-rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a7/LICENSE
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-05-31 21:45:30.806688 mentpy-0.1.0a7/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3056 2023-05-08 04:08:41.000000 mentpy-0.1.0a7/README.md
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.784252 mentpy-0.1.0a7/mentpy/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      278 2023-05-23 00:36:24.000000 mentpy-0.1.0a7/mentpy/__init__.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.786621 mentpy-0.1.0a7/mentpy/calculator/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       46 2023-05-23 00:44:55.000000 mentpy-0.1.0a7/mentpy/calculator/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      137 2023-05-23 00:43:44.000000 mentpy-0.1.0a7/mentpy/calculator/borrows.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1128 2023-05-23 00:43:45.000000 mentpy-0.1.0a7/mentpy/calculator/linalg2.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.787394 mentpy-0.1.0a7/mentpy/gradients/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       33 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/gradients/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2014 2023-04-25 08:57:09.000000 mentpy-0.1.0a7/mentpy/gradients/finite_difference.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.790183 mentpy-0.1.0a7/mentpy/mbqc/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a7/mentpy/mbqc/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    18653 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/mbqc/flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    29847 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/mbqc/mbqcircuit.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.791936 mentpy-0.1.0a7/mentpy/mbqc/states/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-05-06 07:23:30.000000 mentpy-0.1.0a7/mentpy/mbqc/states/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      197 2023-05-06 07:23:09.000000 mentpy-0.1.0a7/mentpy/mbqc/states/aklt.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      229 2023-05-06 07:23:14.000000 mentpy-0.1.0a7/mentpy/mbqc/states/cluster.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a7/mentpy/mbqc/states/graphstate.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     7594 2023-05-24 18:57:37.000000 mentpy-0.1.0a7/mentpy/mbqc/templates.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.792858 mentpy-0.1.0a7/mentpy/noise/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/noise/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/noise/base_noise.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.794157 mentpy-0.1.0a7/mentpy/operators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      285 2023-05-10 00:16:14.000000 mentpy-0.1.0a7/mentpy/operators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3364 2023-05-22 17:03:18.000000 mentpy-0.1.0a7/mentpy/operators/controlled_ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1599 2023-05-07 19:04:31.000000 mentpy-0.1.0a7/mentpy/operators/gates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     8139 2023-05-16 20:00:06.000000 mentpy-0.1.0a7/mentpy/operators/ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5675 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/operators/pauliop.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.797575 mentpy-0.1.0a7/mentpy/optimizers/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a7/mentpy/optimizers/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3054 2023-03-22 20:56:41.000000 mentpy-0.1.0a7/mentpy/optimizers/adam.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      632 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/optimizers/base_optimizer.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      379 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/optimizers/bp_tools.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3101 2023-04-25 09:08:43.000000 mentpy-0.1.0a7/mentpy/optimizers/rcd.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2637 2023-04-15 23:00:30.000000 mentpy-0.1.0a7/mentpy/optimizers/sgd.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.801268 mentpy-0.1.0a7/mentpy/simulators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a7/mentpy/simulators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2441 2023-05-07 19:04:31.000000 mentpy-0.1.0a7/mentpy/simulators/base_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a7/mentpy/simulators/cirq_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    15594 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/simulators/np_simulator_dm.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    19270 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/simulators/np_simulator_sv.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2678 2023-05-18 06:35:37.000000 mentpy-0.1.0a7/mentpy/simulators/pattern_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5677 2023-05-18 08:04:21.000000 mentpy-0.1.0a7/mentpy/simulators/pennylane_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1254 2023-04-25 08:57:09.000000 mentpy-0.1.0a7/mentpy/simulators/qiskit_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.802518 mentpy-0.1.0a7/mentpy/utils/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      140 2023-05-23 00:17:19.000000 mentpy-0.1.0a7/mentpy/utils/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     6673 2023-04-25 08:57:09.000000 mentpy-0.1.0a7/mentpy/utils/expressivity.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a7/mentpy/utils/flow_space.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a7/mentpy/utils/generate_data.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-05-06 07:13:49.000000 mentpy-0.1.0a7/mentpy/utils/lc_equivalence.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5383 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/utils/lie_algebra.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.785522 mentpy-0.1.0a7/mentpy.egg-info/
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1497 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/SOURCES.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/dependency_links.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/requires.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/top_level.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-05-31 21:45:30.807073 mentpy-0.1.0a7/setup.cfg
+-rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-05-31 21:45:19.000000 mentpy-0.1.0a7/setup.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.806024 mentpy-0.1.0a7/tests/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a7/tests/test_flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a7/tests/test_graph_state.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a7/tests/test_mbqc_templates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2110 2023-05-18 06:15:48.000000 mentpy-0.1.0a7/tests/test_simulators.py
```

### Comparing `mentpy-0.1.0a6/LICENSE` & `mentpy-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/PKG-INFO` & `mentpy-0.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a6 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a7 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
 Content-Type: text/markdown License-File: LICENSE
           [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
                  mentpy?label=mentpy&style=flat&logo=twitter]
```

### Comparing `mentpy-0.1.0a6/README.md` & `mentpy-0.1.0a7/README.md`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/gradients/finite_difference.py` & `mentpy-0.1.0a7/mentpy/gradients/finite_difference.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/mbqc/flow.py` & `mentpy-0.1.0a7/mentpy/mbqc/flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,41 +2,333 @@
 # Github: BestQuark
 """This is the Flow module. It deals with the flow of a given graph state"""
 import math
 import numpy as np
 import networkx as nx
 
 from mentpy.mbqc import GraphState
-from typing import List
+from typing import Any, List
 import warnings
 
 import galois
 
-## Not used in main MBQC module
 
-# This module should only export the flow class
+GF = galois.GF(2)
+
+
+def binary_gaussian_elimination(A, b):
+    rows, cols = A.shape
+    augmented_matrix = np.hstack((A, b.reshape(-1, 1)))
+
+    row = 0
+    for col in range(cols):
+        # Find pivot in current column
+        for pivot_row in range(row, rows):
+            if augmented_matrix[pivot_row, col]:
+                break
+        else:
+            continue
+
+        # Swap rows if needed
+        if pivot_row != row:
+            augmented_matrix[[row, pivot_row]] = augmented_matrix[[pivot_row, row]]
+
+        # Zero out below pivot
+        for i in range(row + 1, rows):
+            if augmented_matrix[i, col]:
+                augmented_matrix[i] ^= augmented_matrix[row]
+
+        row += 1
+
+        if row >= rows:
+            break
+
+    # Back-substitution
+    x = np.zeros(cols, dtype=int)
+    for row in range(min(rows, cols) - 1, -1, -1):
+        col = np.argmax(augmented_matrix[row, :cols])
+        x[col] = augmented_matrix[row, -1] ^ np.sum(
+            augmented_matrix[row, col + 1 : cols] * x[col + 1 : cols]
+        )
+
+    return x
 
 
 class Flow:
+    """This class deals with the flow of a given graph state"""
+
     def __init__(self, graph: GraphState, input_nodes, output_nodes):
         self.graph = graph
         self.input_nodes = input_nodes
         self.output_nodes = output_nodes
-        flow_function, partial_order = self.find_flow()
+        flow_function, partial_order, depth, layers = self.find_flow()
         self.func = flow_function
         self.partial_order = partial_order
-        self.depth = -1  # calculate depth
+        self.depth = depth
+        self.layers_dict = layers
+        if layers is not None:
+            ord_layers = [
+                [n for n, l in layers.items() if l == j]
+                for j in range(max(layers.values()) + 1)
+            ]
+            self.layers = ord_layers[::-1]
+
+            # This can be optimized!!
+            order = [item for sublist in self.layers for item in sublist]
+            for i in self.input_nodes[::-1]:
+                order.remove(i)
+                order.insert(0, i)
+            self.measurement_order = order
+        else:
+            self.layers = None
+            self.measurement_order = None
+
+    def __repr__(self):
+        return f"Flow(n={self.graph.number_of_nodes()})"
+
+    def __call__(self, node):
+        return self.func(node)
 
     def find_flow(self):
         # include gflow and pflow
-        return find_flow(self.graph, self.input_nodes, self.output_nodes)
+        flow_stuff = find_cflow(self.graph, self.input_nodes, self.output_nodes)
+        if flow_stuff[0] is None:
+            flow_stuff = find_gflow(self.graph, self.input_nodes, self.output_nodes)
+            if flow_stuff[0] is None:
+                # TODO: implement pflow
+                # flow_stuff = find_pflow(self.graph, self.input_nodes, self.output_nodes)
+                pass
+
+        return flow_stuff
 
     def adapt_angles(self, angles, outcomes):
         raise NotImplementedError
 
+    def adapt_angle(self, angle, node, previous_outcomes):
+        raise NotImplementedError
+
+
+### This section implements causal flow -- Runs in time O(min(m, kn))
+
+
+def find_cflow(graph: GraphState, input_nodes, output_nodes) -> object:
+    """Finds the causal flow of a ``MBQCGraph`` if it exists.
+    Retrieved from https://arxiv.org/pdf/0709.2670v1.pdf.
+    """
+    if len(input_nodes) != len(output_nodes):
+        raise ValueError(
+            f"Cannot find flow or gflow. Input ({len(input_nodes)}) and output ({len(output_nodes)}) nodes have different size."
+        )
+
+    l = {}
+    g = {}
+    past = {}
+    C_set = set()
+
+    for v in graph.nodes():
+        l[v] = 0
+        past[v] = 0
+
+    for v in set(output_nodes) - set(input_nodes):
+        past[v] = len(
+            set(graph.neighbors(v)) & (set(graph.nodes() - set(output_nodes)))
+        )
+        if past[v] == 1:
+            C_set = C_set.union({v})
+
+    flow, ln = causal_flow_aux(
+        graph, set(input_nodes), set(output_nodes), C_set, past, 1, g, l
+    )
+
+    if len(flow) != len(graph.nodes()) - len(output_nodes):
+        return None, None, None, None
+
+    return lambda x: flow[x], lambda u, v: ln[u] > ln[v], max(flow.values()), ln
+
+
+def causal_flow_aux(graph: GraphState, inputs, outputs, C, past, k, g, l) -> object:
+    """Aux function for causal_flow"""
+    V = set(graph.nodes())
+    C_prime = set()
+
+    for _, v in enumerate(C):
+        intersection = set(graph.neighbors(v)) & (V - outputs)
+        if len(intersection) == 1:
+            u = intersection.pop()
+            g[u] = v
+            l[u] = k
+            outputs.add(u)
+            if u not in inputs:
+                past[u] = len(set(graph.neighbors(u)) & (V - outputs))
+                if past[u] == 1:
+                    C_prime.add(u)
+            for w in set(graph.neighbors(u)):
+                if past[w] > 0:
+                    past[w] -= 1
+                    if past[w] == 1:
+                        C_prime.add(w)
+
+    if len(C_prime) == 0:
+        return g, l
+
+    else:
+        return causal_flow_aux(
+            graph,
+            inputs,
+            outputs,
+            C_prime,
+            past,
+            k + 1,
+            g,
+            l,
+        )
+
+
+### This section implements generalized flow -- Runs in time O(n^4)
+
+
+def find_gflow(graph: GraphState, input_nodes, output_nodes) -> object:
+    """Finds the generalized flow of a ``MBQCGraph`` if it exists.
+    Retrieved from https://arxiv.org/pdf/0709.2670v1.pdf.
+    """
+    gamma = nx.adjacency_matrix(graph).toarray()
+
+    l = {}
+    g = {}
+
+    for v in output_nodes:
+        l[v] = 0
+
+    result, gn, ln = gflowaux(
+        graph,
+        gamma,
+        set(input_nodes),
+        set(output_nodes),
+        1,
+        g,
+        l,
+    )
+
+    if result == False:
+        warnings.warn("No gflow exists for this graph.", UserWarning, stacklevel=2)
+        return None, None, None, None
+
+    return lambda x: gn[x], lambda u, v: ln[u] > ln[v], max(ln.values()), ln
+
+
+def gflowaux(graph: GraphState, gamma, inputs, outputs, k, g, l) -> object:
+    """Aux function for gflow"""
+
+    mapping = graph.index_mapping()
+    V = set(graph.nodes())
+    C = set()
+    vmol = list(V - outputs)
+    for u in vmol:
+        submatrix = np.zeros((len(vmol), len(outputs - inputs)), dtype=int)
+        for i, v in enumerate(vmol):
+            for j, w in enumerate(outputs - inputs):
+                submatrix[i, j] = gamma[mapping[v], mapping[w]]
+
+        b = np.zeros((len(vmol), 1), dtype=int)
+        b[vmol.index(u)] = 1
+        submatrix = GF(submatrix)
+        b = GF(b)
+        solution = GF(binary_gaussian_elimination(submatrix, b)).reshape(-1, 1)
+
+        if np.linalg.norm(submatrix @ solution - b) <= 1e-5:
+            l[u] = k
+            C.add(u)
+            g[u] = solution
+
+    if len(C) == 0:
+        if set(outputs) == V:
+            return True, g, l
+        else:
+            return False, g, l
+
+    else:
+        return gflowaux(graph, gamma, inputs, outputs | C, k + 1, g, l)
+
+
+## This section implements PauliFlow. Currently not working.
+
+
+def find_pflow(
+    graph: GraphState, input_nodes, output_nodes, basis="XY", testing=False
+) -> object:
+    """Implementation of pauli flow algorithm in https://arxiv.org/pdf/2109.05654v1.pdf"""
+
+    if not testing:
+        raise NotImplementedError("This algorithm is not yet implemented.")
+
+    if type(basis) == str:
+        basis = {v: basis for v in graph.nodes()}
+    elif type(basis) != dict:
+        raise TypeError("Basis must be a string or a dictionary.")
+
+    lx = set()
+    ly = set()
+    lz = set()
+    d = {}
+    p = {}
+
+    gamma = nx.adjacency_matrix(graph).toarray()
+
+    for v in graph.nodes():
+        if v in output_nodes:
+            d[v] = 0
+        if basis[v] == "X":
+            lx = lx.add(v)
+        elif basis[v] == "Y":
+            ly = ly.add(v)
+        elif basis[v] == "Z":
+            lz = lz.add(v)
+
+    return pflowaux(graph, gamma, input_nodes, basis, set(), output_nodes, 0, d, p)
+
+
+def pflowaux(graph: GraphState, gamma, inputs, plane, A, B, k, d, p) -> object:
+    """Aux function for pflow"""
+    C = set()
+    mapping = graph.index_mapping()
+    for u in set(graph.nodes()) - set(B):
+        submatrix1, submatrix2, submatrix3 = None, None, None
+        solution1, solution2, solution3 = None, None, None
+        if plane[u] in ["XY", "X", "Y"]:
+            submatrix1 = 0  # TODO
+            solution1 = 0  # TODO
+        if plane[u] in ["XZ", "X", "Z"]:
+            submatrix2 = 0  # TODO
+            solution2 = 0  # TODO
+        if plane[u] in ["YZ", "Y", "Z"]:
+            submatrix3 = 0  # TODO
+            solution3 = 0  # TODO
+
+        if (
+            (solution1 is not None)
+            or (solution2 is not None)
+            or (solution3 is not None)
+        ):
+            C.add(u)
+            sol = solution1 or solution2 or solution3
+            p[u] = sol
+            d[u] = k
+
+    if len(C) == 0 and k > 0:
+        if set(B) == set(graph.nodes()):
+            return True, p, d
+        else:
+            return False, set(), set()
+    else:
+        B = B.union(C)
+        return pflowaux(graph, gamma, inputs, plane, B, B, k + 1, d, p)
+
+
+## Finds flow of a graph state. This is deprecated and will be removed in the future.
+
 
 def find_flow(graph: GraphState, input_nodes, output_nodes, sanity_check=True):
     r"""Finds the generalized flow of graph state if allowed.
 
     Implementation of https://arxiv.org/pdf/quant-ph/0603072.pdf.
 
     Returns
@@ -44,19 +336,19 @@
     The flow function ``flow`` and the partial order function.
 
     Group
     -----
     states
     """
     # raise deprecated warning
-    # warnings.warn(
-    #     "The function find_flow is deprecated. Use find_cflow instead.",
-    #     DeprecationWarning,
-    #     stacklevel=2,
-    # )
+    warnings.warn(
+        "The function find_flow is deprecated. Use find_cflow instead.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
 
     n_input, n_output = len(input_nodes), len(output_nodes)
     inp = input_nodes
     outp = output_nodes
     if n_input != n_output:
         raise ValueError(
             f"Cannot find flow or gflow. Input ({n_input}) and output ({n_output}) nodes have different size."
@@ -323,259 +615,7 @@
             print(f"Condition 2 failed for node {i}. {i} ≮ {flow(i)}")
         if not c3:
             print(f"Condition 3 failed for node {i}.")
             for k in set(nfi) - {i}:
                 if not partial_order(i, k):
                     print(f"{i} ≮ {k}")
     return conds
-
-
-### This section implements causal flow
-
-
-def find_cflow(graph: GraphState, input_nodes, output_nodes) -> object:
-    """Finds the causal flow of a ``MBQCGraph`` if it exists.
-    Retrieved from https://arxiv.org/pdf/0709.2670v1.pdf.
-    """
-    if len(input_nodes) != len(output_nodes):
-        raise ValueError(
-            f"Cannot find flow or gflow. Input ({len(input_nodes)}) and output ({len(output_nodes)}) nodes have different size."
-        )
-
-    l = {}
-    g = {}
-    past = {}
-    C_set = set()
-
-    graph_extended = graph.copy()
-    max_node = max(graph.nodes()) + 1
-    input_nodes_extended = [max_node + i for i in range(len(input_nodes))]
-    graph_extended.add_edges_from(
-        [(input_nodes_extended[i], input_nodes[i]) for i in range(len(input_nodes))]
-    )
-
-    for v in graph_extended.nodes():
-        l[v] = 0
-        past[v] = 0
-
-    for v in set(output_nodes) - set(input_nodes_extended):
-        past[v] = len(
-            set(graph_extended.neighbors(v))
-            & (set(graph_extended.nodes() - set(output_nodes)))
-        )
-        if past[v] == 1:
-            C_set = C_set.union({v})
-
-    flow, l = causal_flow_aux(
-        graph_extended,
-        set(input_nodes_extended),
-        set(output_nodes),
-        C_set,
-        past,
-        1,
-        g,
-        l,
-    )
-
-    flow = {k: v for k, v in flow.items() if k not in input_nodes_extended}
-    ln = {k: v for k, v in l.items() if k not in input_nodes_extended}
-
-    if len(flow) != len(graph.nodes()) - len(output_nodes):
-        return None, None, None
-
-    return lambda x: flow[x], lambda u, v: ln[u] > ln[v], max(flow.values())
-
-
-def causal_flow_aux(graph: GraphState, inputs, outputs, C, past, k, g, l) -> object:
-    """Aux function for causal_flow"""
-    V = set(graph.nodes())
-    C_prime = set()
-
-    for _, v in enumerate(C):
-        # get intersection of neighbors of v and (V \ output nodes
-        intersection = set(graph.neighbors(v)) & (V - outputs)
-        if len(intersection) == 1:
-            u = intersection.pop()
-            g[u] = v
-            l[u] = k
-            outputs.add(u)
-            if u not in inputs:
-                past[u] = len(set(graph.neighbors(u)) & (V - outputs))
-                if past[u] == 1:
-                    C_prime.add(u)
-            for w in set(graph.neighbors(u)):
-                if past[w] > 0:
-                    past[w] -= 1
-                    if past[w] == 1:
-                        C_prime.add(w)
-
-    if len(C_prime) == 0:
-        return g, l
-
-    else:
-        return causal_flow_aux(
-            graph,
-            inputs,
-            outputs,
-            C_prime,
-            past,
-            k + 1,
-            g,
-            l,
-        )
-
-
-### This section implements generalized flow
-
-
-def find_gflow(graph: GraphState, input_nodes, output_nodes) -> object:
-    """Finds the generalized flow of a ``MBQCGraph`` if it exists.
-    Retrieved from https://arxiv.org/pdf/0709.2670v1.pdf.
-    """
-    graph_extended = graph.copy()
-    max_node = max(graph.nodes()) + 1
-    input_nodes_extended = [max_node + i for i in range(len(input_nodes))]
-    graph_extended.add_edges_from(
-        [(input_nodes_extended[i], input_nodes[i]) for i in range(len(input_nodes))]
-    )
-
-    gamma = nx.adjacency_matrix(graph_extended).toarray()
-
-    l = {}
-    g = {}
-
-    for v in output_nodes:
-        l[v] = 0
-
-    result, g, l = gflowaux(
-        graph_extended,
-        gamma,
-        set(input_nodes_extended),
-        set(output_nodes) - set(input_nodes_extended),
-        1,
-        g,
-        l,
-    )
-
-    if result == False:
-        warnings.warn("No gflow exists for this graph.", UserWarning, stacklevel=2)
-        return None, None, None
-
-    gn = {i: g[i] for i in set(graph.nodes()) - set(output_nodes)}
-    ln = {i: l[i] for i in graph.nodes()}
-
-    return lambda x: gn[x], lambda u, v: ln[u] > ln[v], max(ln.values())
-
-
-def gf2_matrix_solve(A, b):
-    A = A % 2
-    b = b % 2
-    sol, _, _, _ = np.linalg.lstsq(A, b, rcond=None)
-    return (sol.round() % 2).astype(int)
-
-
-def gflowaux(graph: GraphState, gamma, inputs, outputs, k, g, l) -> object:
-    """Aux function for gflow"""
-    out_prime = set()
-    mapping = graph.index_mapping()
-    GF = galois.GF(2)
-    V = set(graph.nodes())
-    C = set()
-    vmol = list(V - outputs)
-    for u in vmol:
-        submatrix = np.zeros((len(vmol), len(outputs - inputs)), dtype=int)
-        for i, v in enumerate(vmol):
-            for j, w in enumerate(outputs - inputs):
-                submatrix[i, j] = gamma[mapping[v], mapping[w]]
-
-        b = np.zeros((len(vmol), 1), dtype=int)
-        b[vmol.index(u)] = 1
-        solution = gf2_matrix_solve(submatrix, b)
-
-        # Check if solution is a valid solution
-        if np.linalg.norm(submatrix @ solution - b) <= 1e-5:
-            l[u] = k
-            C.add(u)
-            g[u] = solution
-
-    if len(C) == 0:
-        if set(outputs) == V:
-            return True, g, l
-        else:
-            return False, g, l
-
-    else:
-        return gflowaux(graph, gamma, inputs, outputs | C, k + 1, g, l)
-
-
-## This section implements PauliFlow
-
-
-def find_pflow(
-    graph: GraphState, input_nodes, output_nodes, basis="XY", testing=False
-) -> object:
-    """Implementation of pauli flow algorithm in https://arxiv.org/pdf/2109.05654v1.pdf"""
-
-    if not testing:
-        raise NotImplementedError("This algorithm is not yet implemented.")
-
-    if type(basis) == str:
-        basis = {v: basis for v in graph.nodes()}
-    elif type(basis) != dict:
-        raise TypeError("Basis must be a string or a dictionary.")
-
-    lx = set()
-    ly = set()
-    lz = set()
-    d = {}
-    p = {}
-
-    gamma = nx.adjacency_matrix(graph).toarray()
-
-    for v in graph.nodes():
-        if v in output_nodes:
-            d[v] = 0
-        if basis[v] == "X":
-            lx = lx.add(v)
-        elif basis[v] == "Y":
-            ly = ly.add(v)
-        elif basis[v] == "Z":
-            lz = lz.add(v)
-
-    return pflowaux(graph, gamma, input_nodes, basis, set(), output_nodes, 0, d, p)
-
-
-def pflowaux(graph: GraphState, gamma, inputs, plane, A, B, k, d, p) -> object:
-    """Aux function for pflow"""
-    C = set()
-    mapping = graph.index_mapping()
-    for u in set(graph.nodes()) - set(B):
-        submatrix1, submatrix2, submatrix3 = None, None, None
-        solution1, solution2, solution3 = None, None, None
-        if plane[u] in ["XY", "X", "Y"]:
-            submatrix1 = 0  # TODO
-            solution1 = 0  # TODO
-        if plane[u] in ["XZ", "X", "Z"]:
-            submatrix2 = 0  # TODO
-            solution2 = 0  # TODO
-        if plane[u] in ["YZ", "Y", "Z"]:
-            submatrix3 = 0  # TODO
-            solution3 = 0  # TODO
-
-        if (
-            (solution1 is not None)
-            or (solution2 is not None)
-            or (solution3 is not None)
-        ):
-            C.add(u)
-            sol = solution1 or solution2 or solution3
-            p[u] = sol
-            d[u] = k
-
-    if len(C) == 0 and k > 0:
-        if set(B) == set(graph.nodes()):
-            return True, p, d
-        else:
-            return False, set(), set()
-    else:
-        B = B.union(C)
-        return pflowaux(graph, gamma, inputs, plane, B, B, k + 1, d, p)
```

### Comparing `mentpy-0.1.0a6/mentpy/mbqc/mbqcircuit.py` & `mentpy-0.1.0a7/mentpy/mbqc/mbqcircuit.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import scipy as scp
 import networkx as nx
 import matplotlib.pyplot as plt
 
 from mentpy.operators import Ment, ControlMent, PauliOp
 from mentpy.mbqc.states.graphstate import GraphState
-from mentpy.mbqc.flow import find_cflow, find_flow, check_if_flow
+from mentpy.mbqc.flow import find_cflow, find_flow, check_if_flow, Flow
 
 __all__ = ["MBQCircuit", "draw", "merge", "hstack", "vstack"]
 
 
 class MBQCircuit:
     r"""The MBQCircuit class that deals with operations and manipulations of graph states
 
@@ -130,15 +130,21 @@
                     )
 
         self._measurements = measurements
         self._flow, self._partial_order = None, None
         self._update_attributes()
 
         if (flow is None) or (partial_order is None):
-            flow, partial_order, depth = find_cflow(graph, input_nodes, output_nodes)
+            flow, partial_order, depth, layers = find_cflow(
+                graph, input_nodes, output_nodes
+            )
+            self._layers = layers
+            self.gflow = Flow(
+                graph, input_nodes, output_nodes
+            )  # TODO: make this the standard flow in this class
             # try:
             #     flow, partial_order = find_flow(
             #         graph, input_nodes, output_nodes
             #     )  # TODO: FIX find_cflow!!!!
             # except:
             #     pass
             # if flow is None:
@@ -305,14 +311,26 @@
         return [v for v in self.graph.nodes() if v not in self.output_nodes]
 
     @cached_property
     def inputc(self) -> List:
         r"""Returns :math:`I^c`, the complement of input nodes."""
         return [v for v in self.graph.nodes() if v not in self.input_nodes]
 
+    def ordered_layers(self, train_indices=False) -> List[List[int]]:
+        r"""Returns the layers of the MBQC circuit."""
+        if self.gflow.func is None:
+            return None
+        if train_indices:
+            # return the nested layers in Flow.layers but with the trainable_nodes indices
+            return [
+                [self.trainable_nodes.index(node) for node in layer]
+                for layer in self.gflow.layers[:-1]
+            ]
+        return self.gflow.layers
+
     def _update_attributes(self) -> None:
         trainable_nodes = []
         controlled_nodes = []
         planes = {}
         quantum_outputs = []
         classical_outputs = []
         for nodei, menti in self._measurements.items():
@@ -375,86 +393,37 @@
                 self._trainable_nodes.remove(key)
 
     def calculate_order(self):
         r"""Returns the order of the measurements"""
         n = len(self.graph)
         mat = np.zeros((n, n), dtype=int)
 
-        # for c in self.controlled_nodes:
-        #     nodes_before = self.measurements[c].condition.cond_nodes
-        #     for node in nodes_before:
-
         for indi, i in enumerate(list(self.graph.nodes())):
             for indj, j in enumerate(list(self.graph.nodes())):
                 if self.partial_order(i, j):
                     mat[indi, indj] = 1
-        # print(mat)
+
         sum_mat = np.sum(mat, axis=1)
         order = np.argsort(sum_mat)[::-1]
-        # print("sum_mat", sum_mat)
-        # print("order", order)
 
         sum_dict = {}
         for i, s in enumerate(sum_mat):
             if s not in sum_dict:
                 sum_dict[s] = []
             sum_dict[s].append(i)
         sorted_indices = [
             sum_dict[key] for key in sorted(sum_dict.keys(), reverse=True)
         ]
         sorted_labels = [
             [list(self.graph.nodes())[i] for i in group] for group in sorted_indices
         ]
-        # print(sorted_labels)
-        # sort within groups can be optimized
+        self._sorted_labels = sorted_labels
 
-        # for group in sorted_labels:
-        #     if len(group) > 1:
-        #         for i in range(len(group)):
-        #             for j in range(i+1, len(group)):
-        #                 if not self.partial_order(group[i], group[j]):
-        #                     group[i], group[j] = group[j], group[i]
-
-        # order = []
-        # print("sorted_labels", sorted_labels)
-        # print(sorted_labels, "antes")
-        # for group in sorted_labels:
-        #     if len(group) > 1:
-        #         # arange controlled nodes
-        #         for c in self.controlled_nodes:
-        #             # check if c is in group
-        #             if c in group:
-        #                 nodes_before = self.measurements[c].condition.cond_nodes
-        #                 for node in nodes_before:
-        #                     # search if node is in group else, swap groups
-        #                     if node in group:
-        #                         indx_node = group.index(node)
-        #                         indx_c = group.index(c)
-        #                         if indx_node > indx_c:
-        #                             group.remove(c)
-        #                             group.insert(indx_node, c)
-
-        # print(sorted_labels)
         order = [item for sublist in sorted_labels for item in sublist]
-        # turn order into labels of graph
-        # order = [
-        #     list(self.graph.nodes())[i] for i in order
-        # ]  # remove once above is done
-
-        # for c in self.controlled_nodes:
-        #     nodes_before = self.measurements[c].condition.cond_nodes
-        #     for node in nodes_before:
-        #         indx_node = order.index(node)
-        #         indx_c = order.index(c)
-        #         if indx_node > indx_c:
-        #             print("swapping", node, c)
-        #             order.remove(c)
-        #             order.insert(indx_node, c)
 
-        # remove all input nodes and put them at the start
         for i in self.input_nodes[::-1]:
             order.remove(i)
             order.insert(0, i)
 
         return order
 
     def add_edge(self, u, v):
@@ -669,22 +638,29 @@
         "edge_color": "grey",
         "edge_color_control": "#CCCCCC",
         "with_labels": True,
         "label": "indices",
         "transparent": True,
         "figsize": (8, 3),
         "show_controls": True,
+        "show_flow": True,
         "pauliop": None,
+        "style": "default",
     }
 
     options.update(kwargs)
 
     show_controls = options.pop("show_controls")
+    show_flow = options.pop("show_flow")
     pauliop = options.pop("pauliop")
     edge_color_control = options.pop("edge_color_control")
+    style = options.pop("style")
+
+    possible_styles = ("default", "black_and_white")
+    assert style in possible_styles, f"Style must be one of {possible_styles}"
 
     if pauliop is not None:
         options["label"] = "pauliop"
 
     transp = options.pop("transparent")
     fig, ax = plt.subplots(figsize=options.pop("figsize"))
 
@@ -716,14 +692,17 @@
             elif i in state.controlled_nodes:
                 node_colors[i] = "#A88FE8"
             elif i in set(state.nodes()) - set(state.trainable_nodes):
                 node_colors[i] = "#CCCCCC"
             else:
                 node_colors[i] = "#FFBD59"
 
+        if style == "black_and_white":
+            node_colors = {i: "#FFFFFF" for i in state.graph.nodes()}
+
         options["node_color"] = [node_colors[node] for node in state.graph.nodes()]
 
         fixed_nodes = state.input_nodes + state.output_nodes
         position_xy = {}
         for indx, p in enumerate(state.input_nodes):
             position_xy[p] = (0, -1 * indx)
 
@@ -805,15 +784,15 @@
                     options["label"]
                 )
             )
 
         del options["label"]
 
         nx.draw(state.graph, ax=ax, pos=node_pos, **options)
-        if state.flow is not None:
+        if state.flow is not None and show_flow:
             nx.draw(_graph_with_flow(state), pos=node_pos, ax=ax, **options)
         if show_controls:
             dashed_edges = []
             for node in state.controlled_nodes:
                 for k in state.measurements[node].condition.cond_nodes:
                     dashed_edges.append((node, k))
             nx.draw_networkx_edges(
@@ -825,19 +804,19 @@
                 style="dashed",
             )
 
 
 def _graph_with_flow(state):
     """Return digraph with flow (but does not have all CZ edges!)"""
     g = state.graph
-    gflow = nx.DiGraph()
-    gflow.add_nodes_from(g.nodes())
+    dflow = nx.DiGraph()
+    dflow.add_nodes_from(g.nodes())
     for node in state.outputc:
-        gflow.add_edge(node, state.flow(node))
-    return gflow
+        dflow.add_edge(node, state.flow(node))
+    return dflow
 
 
 def _create_new_partial_order(controlled_nodes, measurements, old_partial_order):
     def new_partial_order(i, j):
         for c in controlled_nodes:
             cns = measurements[c].condition.cond_nodes
```

### Comparing `mentpy-0.1.0a6/mentpy/mbqc/states/graphstate.py` & `mentpy-0.1.0a7/mentpy/mbqc/states/graphstate.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/mbqc/templates.py` & `mentpy-0.1.0a7/mentpy/mbqc/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,23 +236,23 @@
     gr = many_wires([5, 2, 5]).graph
     gr.add_edge(2, 6)
     gr.add_edge(9, 6)
     sym_block1 = MBQCircuit(
         gr,
         input_nodes=[0, 7],
         output_nodes=[4, 11],
-        measurements={5: Ment(plane="XZ")},
+        measurements={5: Ment(plane="XY")},
         default_measurement=Ment(plane="X"),
     )
     sym_block2 = MBQCircuit(
         gr,
         input_nodes=[0, 7],
         output_nodes=[4, 11],
         measurements={
-            5: Ment(plane="XZ"),
+            5: Ment(plane="XY"),
             1: Ment(plane="Y"),
             3: Ment(plane="Y"),
             8: Ment(plane="Y"),
             10: Ment(plane="Y"),
         },
         default_measurement=Ment(plane="X"),
     )
```

### Comparing `mentpy-0.1.0a6/mentpy/operators/controlled_ment.py` & `mentpy-0.1.0a7/mentpy/operators/controlled_ment.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,20 @@
                 f"Invalid argument type. Expected bool or MentOutcome but got {type(condition)}"
             )
         self._condition = condition
 
     @property
     def angle(self, *args, **kwargs):
         if args == () and kwargs == {}:
-            if self._true_ment.angle is None or super().angle is None:
+            if isinstance(self._condition, bool):
+                if self._condition:
+                    return self._true_ment.angle
+                else:
+                    return super().angle
+            elif self._true_ment.angle is None or super().angle is None:
                 return None
             else:
                 return super().angle
         else:
             if self.condition(*args, **kwargs):
                 return self._true_ment.angle
             else:
```

### Comparing `mentpy-0.1.0a6/mentpy/operators/gates.py` & `mentpy-0.1.0a7/mentpy/operators/gates.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/operators/ment.py` & `mentpy-0.1.0a7/mentpy/operators/ment.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/operators/pauliop.py` & `mentpy-0.1.0a7/mentpy/operators/pauliop.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,20 @@
 
     def __contains__(self, item: "PauliOp"):
         for row in item.matrix:
             if not np.any((self.matrix == row).all(axis=1)):
                 return False
         return True
 
+    def __hash__(self):
+        return hash(str(self.matrix))
+
+    def __eq__(self, other: "PauliOp"):
+        return np.all(self.matrix == other.matrix)
+
     def _mat_to_txt(self, op):
         n_qubits = op.shape[1] // 2
         txt = ""
         for i in range(op.shape[0]):
             for j in range(op.shape[1] // 2):
                 if op[i, j] == 1 and op[i, j + n_qubits] == 0:
                     txt += "X"
@@ -176,12 +182,13 @@
         Examples
         --------
         .. ipython:: python
 
             op = mp.PauliOp('XIZ;ZII;IIZ;IZI')
             print(op.get_subset([0, 2]))
         """
-        if max(indices) >= self.matrix.shape[1] // 2:
+        inds = indices.copy()
+        if max(inds) >= self.matrix.shape[1] // 2:
             raise ValueError("Index out of range")
 
-        indices += [i + self.matrix.shape[1] // 2 for i in indices]
-        return PauliOp(self.matrix[:, indices])
+        inds += [i + self.matrix.shape[1] // 2 for i in inds]
+        return PauliOp(self.matrix[:, inds])
```

### Comparing `mentpy-0.1.0a6/mentpy/optimizers/adam.py` & `mentpy-0.1.0a7/mentpy/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/optimizers/base_optimizer.py` & `mentpy-0.1.0a7/mentpy/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/optimizers/rcd.py` & `mentpy-0.1.0a7/mentpy/optimizers/rcd.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/optimizers/sgd.py` & `mentpy-0.1.0a7/mentpy/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/simulators/base_simulator.py` & `mentpy-0.1.0a7/mentpy/simulators/base_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/simulators/cirq_simulator.py` & `mentpy-0.1.0a7/mentpy/simulators/cirq_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/simulators/np_simulator_dm.py` & `mentpy-0.1.0a7/mentpy/simulators/np_simulator_dm.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,23 +110,23 @@
         ]
 
     def current_number_simulated_nodes(self) -> int:
         """Returns the number of nodes that are currently simulated."""
         n = self.window_size
         return min(n, len(self.mbqcircuit) - self.current_measurement)
 
-    def measure(self, angle: float) -> Tuple:
+    def measure(self, angle: float, mode="sample") -> Tuple:
         if self.current_measurement >= len(self.schedule_measure):
             raise ValueError("No more measurements to be done.")
 
         current_ment = self.mbqcircuit[
             self.schedule_measure[self.current_measurement]
         ].copy()
         self.qstate, outcome = self.measure_ment(
-            current_ment, angle, 0, force0=self.force0
+            current_ment, angle, 0, force0=self.force0, mode=mode
         )
         # check if qstate has nan
         if np.isnan(self.qstate).any():
             raise ValueError(
                 "qstate has nan, you might want to increase the window size"
             )
         self.current_measurement += 1
@@ -148,29 +148,29 @@
                 if neighbour in self.current_simulated_nodes():
                     indxn = self.current_simulated_nodes().index(neighbour)
                     cz = self.controlled_z(indxn, indx_new, self.window_size)
                     self.qstate = cz @ self.qstate @ np.conj(cz.T)
 
         return self.qstate, outcome
 
-    def run(self, angles: List[float]) -> Tuple[List[int], np.ndarray]:
+    def run(self, angles: List[float], mode="sample") -> Tuple[List[int], np.ndarray]:
         """Measures the quantum state in the given pattern."""
 
         if len(angles) != len(self.mbqcircuit.trainable_nodes):
             raise ValueError(
                 f"Number of angles ({len(angles)}) does not match number of trainable nodes ({len(self.mbqcircuit.trainable_nodes)})."
             )
 
         for i in self.schedule_measure:
             if i in self.mbqcircuit.trainable_nodes:
                 angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
             else:
                 angle = self.mbqcircuit[i].angle
 
-            self.qstate, outcome = self.measure(angle)
+            self.qstate, outcome = self.measure(angle, mode)
             self.outcomes[i] = outcome
 
         current_output_order = [
             i for i in self.schedule if i not in self.schedule_measure
         ]
         if self.mbqcircuit.quantum_output_nodes != current_output_order:
             self.qstate = self.reorder_qubits(
@@ -275,15 +275,15 @@
                     elif qubits[idx] == "1":
                         ptrace = np.kron(ptrace, np.array([[0], [1]]))
                 else:
                     ptrace = np.kron(ptrace, np.eye(2))
             sigma = sigma + np.conjugate(ptrace.T) @ rho @ (ptrace)
         return sigma
 
-    def measure_ment(self, ment: Ment, angle, i, force0=False):
+    def measure_ment(self, ment: Ment, angle, i, force0=False, mode="sample"):
         """
         Measures a ment
         """
         op = ment.matrix(angle, self.outcomes)
         if op is None:
             raise ValueError(f"Ment has no matrix representation at qubit {i}")
 
@@ -294,26 +294,32 @@
         p1_extended = self.arbitrary_qubit_gate(
             p1, i, self.current_number_simulated_nodes()
         )
 
         prob0 = np.real(np.trace(self.qstate @ p0_extended))
         prob1 = np.real(np.trace(self.qstate @ p1_extended))
 
+        COND = (mode == "expectation" or mode == "exp") and ment.plane == "Z"
+
         if not force0 or ment.plane == "Z":
-            outcome = np.random.choice([0, 1], p=[prob0, prob1] / (prob0 + prob1))
+            if COND:
+                outcome = prob1 / (prob0 + prob1)
+            else:
+                outcome = np.random.choice([0, 1], p=[prob0, prob1] / (prob0 + prob1))
         else:
             if prob0 < 1e-4:
                 outcome = 1  # important when measuring Z's -- should make pretty
             else:
                 outcome = 0
 
-        if outcome == 0:
-            self.qstate = p0_extended @ self.qstate @ np.conj(p0_extended).T / prob0
-        else:
-            self.qstate = p1_extended @ self.qstate @ np.conj(p1_extended).T / prob1
+        if not COND:
+            if outcome == 0:
+                self.qstate = p0_extended @ self.qstate @ np.conj(p0_extended).T / prob0
+            else:
+                self.qstate = p1_extended @ self.qstate @ np.conj(p1_extended).T / prob1
 
         return self.qstate, outcome
 
     def controlled_z(self, i, j, n):
         """
         Controlled z gate between qubits i and j.
         n is the total number of qubits
```

### Comparing `mentpy-0.1.0a6/mentpy/simulators/np_simulator_sv.py` & `mentpy-0.1.0a7/mentpy/simulators/np_simulator_sv.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     ) -> None:
         super().__init__(mbqcircuit, input_state)
 
         self.window_size = kwargs.pop("window_size", 1)
         self.schedule = kwargs.pop("schedule", None)
         self.force0 = kwargs.pop("force0", True)
 
+        self.dev_mode = kwargs.pop("dev_mode", False)
+        self.wires = kwargs.pop("wires", None)
+
         if not self.force0:
             raise NotImplementedError("Numpy simulator does not support force0=False.")
 
         # Only support XY Measurements
         for node in mbqcircuit.graph.nodes:
             if mbqcircuit[node] is not None:
                 if mbqcircuit[node].plane not in ["X", "Y", "XY"]:
@@ -92,14 +95,17 @@
         # get subgraph of the first window_size nodes
         self.subgraph = self.mbqcircuit.graph.subgraph(
             self.schedule[: self.window_size]
         )
 
         self.initial_czs = np.eye(2**self.window_size)
 
+        if self.dev_mode:
+            self._current_simulated_nodes = self.schedule[0 : self.window_size]
+
         # apply cz gates to neighboring qubits
         for node in self.subgraph.nodes:
             for neighbour in self.subgraph.neighbors(node):
                 # avoid repeated application of cz gates
                 if node < neighbour:
                     indx = self.current_simulated_nodes().index(node)
                     indy = self.current_simulated_nodes().index(neighbour)
@@ -107,42 +113,94 @@
                     # self.qstate = cz @ self.qstate @ np.conj(cz).T
                     self.initial_czs = cz @ self.initial_czs
 
         self.qstate = self.initial_czs @ self.qstate
 
     def current_simulated_nodes(self) -> List[int]:
         """Returns the nodes that are currently simulated."""
-        return self.schedule[
-            self.current_measurement : self.current_measurement + self.window_size
-        ]
+        if not self.dev_mode:
+            return self.schedule[
+                self.current_measurement : self.current_measurement + self.window_size
+            ]
+        elif self.dev_mode:
+            return self._current_simulated_nodes
 
     def current_number_simulated_nodes(self) -> int:
         """Returns the number of nodes that are currently simulated."""
         n = self.window_size
         return min(n, len(self.mbqcircuit) - self.current_measurement)
 
+    def node_in_which_wire(self, node: int) -> int:
+        """Returns the wire in which the node is."""
+        for i, wire in enumerate(self.wires):
+            if node in wire:
+                return i
+
+    def neighbors_in_wire(self, node: int) -> List[int]:
+        """Returns the neighbors of a node in the same wire."""
+        wire = self.wires[self.node_in_which_wire(node)]
+        # return nodes that have edges with node
+        return [n for n in wire if self.mbqcircuit.graph.has_edge(node, n)]
+
+    def future_neighbors_in_wire(self, node: int) -> List[int]:
+        neighs = self.neighbors_in_wire(node)
+        future_neighs = []
+        for neigh in neighs:
+            if neigh > node:
+                future_neighs.append(neigh)
+        return future_neighs
+
     def measure(self, angle: float) -> Tuple:
         if self.current_measurement >= len(self.schedule_measure):
             raise ValueError("No more measurements to be done.")
 
-        current_ment = self.mbqcircuit[
-            self.schedule_measure[self.current_measurement]
-        ].copy()
+        if not self.dev_mode:
+            current_ment = self.mbqcircuit[
+                self.schedule_measure[self.current_measurement]
+            ].copy()
+            indx = 0
+        elif self.dev_mode:
+            # if in dev mode, we measure the first node in the current_simulated_nodes
+            # only if a neighbor in the same wire is also in the current_simulated_nodes
+            for node in self.current_simulated_nodes():
+                cond = False
+                futnods = self.future_neighbors_in_wire(node)
+                if len(futnods) == 0:
+                    cond = True
+                else:
+                    cond = futnods[0] in self.current_simulated_nodes()
+                if cond:
+                    current_ment = self.mbqcircuit[node].copy()
+                    indx = self.current_simulated_nodes().index(node)
+                    break
 
         self.qstate, outcome = self.measure_ment(
-            current_ment, angle, 0, force0=self.force0
+            current_ment, angle, indx, force0=self.force0
         )
 
         self.current_measurement += 1
-        self.qstate = self.partial_trace_pure_state(self.qstate, [0])
+        self.qstate = self.partial_trace_pure_state(self.qstate, [indx])
+
+        if self.dev_mode:
+            # remove qubit at indx from current_simulated_nodes
+            self._current_simulated_nodes = [
+                i for i in self._current_simulated_nodes if i != node
+            ]
+            if self.current_measurement + self.window_size <= len(
+                self.mbqcircuit.graph.nodes
+            ):
+                self._current_simulated_nodes.append(
+                    self.schedule[self.current_measurement + self.window_size - 1]
+                )
 
         if self.current_measurement + self.window_size <= len(
             self.mbqcircuit.graph.nodes
         ):
             self.qstate = np.kron(self.qstate, qubit_plus)
+
             new_qubit = self.current_simulated_nodes()[-1]
 
             # get neighbours of new qubit
             neighbours = nx.neighbors(self.mbqcircuit.graph, new_qubit)
 
             # do cz between new qubit and neighbours
             indx_new = self.current_simulated_nodes().index(new_qubit)
@@ -165,32 +223,57 @@
         """
 
         if len(angles) != len(self.mbqcircuit.trainable_nodes):
             raise ValueError(
                 f"Number of angles ({len(angles)}) does not match number of trainable nodes ({len(self.mbqcircuit.trainable_nodes)})."
             )
 
-        for i in self.schedule_measure:
-            if i in self.mbqcircuit.trainable_nodes:
-                angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
-            else:
-                angle = self.mbqcircuit[i].angle
+        if not self.dev_mode:
+            for i in self.schedule_measure:
+                if i in self.mbqcircuit.trainable_nodes:
+                    angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
+                else:
+                    angle = self.mbqcircuit[i].angle
+
+                self.qstate, outcome = self.measure(angle)
+                self.outcomes[i] = outcome
 
-            self.qstate, outcome = self.measure(angle)
-            self.outcomes[i] = outcome
+        elif self.dev_mode:
+            while self.current_measurement < len(self.schedule_measure):
+                for node in self.current_simulated_nodes():
+                    cond = False
+                    futnods = self.future_neighbors_in_wire(node)
+                    if len(futnods) == 0:
+                        cond = True
+                    else:
+                        cond = futnods[0] in self.current_simulated_nodes()
+                    if cond:
+                        current_ment = self.mbqcircuit[node].copy()
+                        indx = self.current_simulated_nodes().index(node)
+                        break
+
+                if cond == False:
+                    raise ValueError("WTF")
+                if node in self.mbqcircuit.trainable_nodes:
+                    angle = angles[self.mbqcircuit.trainable_nodes.index(node)]
+                else:
+                    angle = self.mbqcircuit[node].angle
+
+                self.qstate, outcome = self.measure(angle)
+                self.outcomes[node] = outcome
 
         # check if output nodes have a measurement, if so, measure them
         for i in self.mbqcircuit.output_nodes:
             if isinstance(self.mbqcircuit[i], Ment):
                 self.qstate, outcome = self.measure_ment(
                     self.mbqcircuit[i], self.mbqcircuit[i].angle, i, force0=self.force0
                 )
                 self.outcomes[i] = outcome
 
-        current_output_order = self.schedule[-len(self.mbqcircuit.output_nodes) :]
+        current_output_order = self.current_simulated_nodes()
         if self.mbqcircuit.quantum_output_nodes != current_output_order:
             self.qstate = self.reorder_qubits(
                 self.qstate, current_output_order, self.mbqcircuit.output_nodes
             )
 
         if output_form.lower() == "dm" or output_form.lower() == "densitymatrix":
             return np.outer(self.qstate, np.conj(self.qstate).T)
@@ -215,14 +298,17 @@
 
         self.qstate = self.input_state
 
         self.qstate = self.initial_czs @ self.qstate
 
         self.outcomes = {}
 
+        if self.dev_mode:
+            self._current_simulated_nodes = self.schedule[0 : self.window_size]
+
     def arbitrary_qubit_gate(self, u, i, n):
         """
         Single qubit gate u acting on qubit i
         n is the number of qubits
         """
         op = 1
         for k in range(0, n):
@@ -339,15 +425,15 @@
         return self.qstate, outcome
 
     def controlled_z(self, i, j, n):
         """
         Controlled z gate between qubits i and j.
         n is the total number of qubits
         """
-        assert i < n and j < n
+        assert i < n and j < n, f"{i} or {j} is larger than {n}"
         op1, op2 = 1, 2
         for k in range(0, n):
             op1 = np.kron(op1, np.eye(2))
             if k in [i, j]:
                 op2 = np.kron(
                     op2,
                     np.kron(np.conjugate(np.array([[0], [1]]).T), np.array([[0], [1]])),
```

### Comparing `mentpy-0.1.0a6/mentpy/simulators/pattern_simulator.py` & `mentpy-0.1.0a7/mentpy/simulators/pattern_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/simulators/pennylane_simulator.py` & `mentpy-0.1.0a7/mentpy/simulators/pennylane_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/simulators/qiskit_simulators.py` & `mentpy-0.1.0a7/mentpy/simulators/qiskit_simulators.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/utils/expressivity.py` & `mentpy-0.1.0a7/mentpy/utils/expressivity.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/utils/flow_space.py` & `mentpy-0.1.0a7/mentpy/utils/flow_space.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/utils/generate_data.py` & `mentpy-0.1.0a7/mentpy/utils/generate_data.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/utils/lc_equivalence.py` & `mentpy-0.1.0a7/mentpy/utils/lc_equivalence.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/mentpy/utils/lie_algebra.py` & `mentpy-0.1.0a7/mentpy/utils/lie_algebra.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,17 @@
 from itertools import combinations
 
 import numpy as np
 from mentpy import MBQCircuit, PauliOp
 import galois
-
 import copy
 
-GF = galois.GF(2)
-
-
-def binary_gaussian_elimination(A, b):
-    rows, cols = A.shape
-    augmented_matrix = np.hstack((A, b.reshape(-1, 1)))
-
-    row = 0
-    for col in range(cols):
-        # Find pivot in current column
-        for pivot_row in range(row, rows):
-            if augmented_matrix[pivot_row, col]:
-                break
-        else:
-            continue
-
-        # Swap rows if needed
-        if pivot_row != row:
-            augmented_matrix[[row, pivot_row]] = augmented_matrix[[pivot_row, row]]
-
-        # Zero out below pivot
-        for i in range(row + 1, rows):
-            if augmented_matrix[i, col]:
-                augmented_matrix[i] ^= augmented_matrix[row]
-
-        row += 1
-
-        if row >= rows:
-            break
-
-    # Back-substitution
-    x = np.zeros(cols, dtype=int)
-    for row in range(min(rows, cols) - 1, -1, -1):
-        col = np.argmax(augmented_matrix[row, :cols])
-        x[col] = augmented_matrix[row, -1] ^ np.sum(
-            augmented_matrix[row, col + 1 : cols] * x[col + 1 : cols]
-        )
+from mentpy.calculator import solve
 
-    return x
+GF = galois.GF(2)
 
 
 def _constrains(j: int, state: MBQCircuit, stabilizers: PauliOp):
     """Creates the A matrix for the constraints on the stabilizers"""
 
     if j not in state.outputc:
         raise ValueError("j should be in outputc")
@@ -79,15 +42,15 @@
     x = x.reshape(-1, 1)
     return np.linalg.norm(A @ x - b) == 0
 
 
 def _find_solution(j: int, state: MBQCircuit, stabilizers: PauliOp):
     """Finds the solution of the system of constraints"""
     A, b = _constrains(j, state, stabilizers)
-    sol = GF(binary_gaussian_elimination(A, b))
+    sol = GF(solve(A, b))
 
     if not _check_solution(A, b, sol):
         raise ValueError("Solution not found for j: " + str(j))
 
     op = PauliOp("I" * len(state.measurement_order))
     for i in range(len(sol)):
         if sol[i] == 1:
@@ -112,25 +75,18 @@
 
 def calculate_gens_lie_algebra(state: MBQCircuit):
     """Calculates the generators of the Lie algebra of a given state"""
     mapping = {
         i: j
         for i, j in zip(state.measurement_order, range(len(state.measurement_order)))
     }
-    graph_stabs = state.stabilizers()
 
-    lieAlgebra = None
-    for i in state.outputc:
-        op = _find_solution(i, state, graph_stabs)
-        if lieAlgebra is None:
-            lieAlgebra = op
-        else:
-            lieAlgebra.append(op)
+    lieAlgebra = calculate_complete_gens_lie_algebra(state)
 
-    output_ops = lieAlgebra.get_subset([mapping[i] for i in state.output_nodes])
+    output_ops = lieAlgebra.get_subset(state.output_nodes)
     return remove_repeated_ops(output_ops)
 
 
 # def lie_algebra_completion_old(generators: PauliOp, max_iter: int = 1000):
 #     """Completes a given set of Pauli operators to a basis of the Lie algebra"""
 #     lieAlg = copy.deepcopy(generators)
 #     already_commutated = []
@@ -163,34 +119,34 @@
 #     return lieAlg
 
 
 def lie_algebra_completion(generators: PauliOp, max_iter: int = 1000):
     """Completes a given set of Pauli operators to a basis of the Lie algebra"""
     lieAlg = copy.deepcopy(generators)
     already_commutated = set()
-    n = len(lieAlg)
-    queue = [(i, j) for i, j in combinations(range(n), 2)]
+    queue = [(i, j) for i, j in combinations(lieAlg, 2)]
     iter = 0
     while iter < max_iter and queue:
         iter += 1
-        i, j = queue.pop(0)
-        if (i, j) not in already_commutated:
-            already_commutated.add((i, j))
-            newOp = lieAlg[i].commutator(lieAlg[j])
+        x, y = queue.pop(0)
+        if (x, y) not in already_commutated and (y, x) not in already_commutated:
+            already_commutated.add((x, y))
+            already_commutated.add((y, x))
+            newOp = x.commutator(y)
             if newOp not in lieAlg:
                 lieAlg.append(newOp)
-                queue.extend((len(lieAlg) - 1, k) for k in range(len(lieAlg) - 1))
+                queue.extend((newOp, k) for k in lieAlg if k != newOp)
 
     if iter >= max_iter - 1 and queue:
         raise ValueError("Max iterations reached")
 
     # check IIII is in lieAlg
-    n_qubits = int(lieAlg.matrix.shape[1] // 2)
-    if PauliOp("I" * n_qubits) not in lieAlg:
-        lieAlg.append(PauliOp("I" * n_qubits))
+    identityPauli = PauliOp("I" * int(lieAlg[0].matrix.shape[1] // 2))
+    if identityPauli not in lieAlg:
+        lieAlg.append(identityPauli)
 
     return lieAlg
 
 
 def calculate_lie_algebra(state: MBQCircuit, max_iter: int = 10000):
     """Calculates the Lie algebra of a given state"""
     generators = calculate_gens_lie_algebra(state)
```

### Comparing `mentpy-0.1.0a6/mentpy.egg-info/PKG-INFO` & `mentpy-0.1.0a7/mentpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a6 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a7 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
 Content-Type: text/markdown License-File: LICENSE
           [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
                  mentpy?label=mentpy&style=flat&logo=twitter]
```

### Comparing `mentpy-0.1.0a6/mentpy.egg-info/SOURCES.txt` & `mentpy-0.1.0a7/mentpy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 setup.py
 mentpy/__init__.py
 mentpy.egg-info/PKG-INFO
 mentpy.egg-info/SOURCES.txt
 mentpy.egg-info/dependency_links.txt
 mentpy.egg-info/requires.txt
 mentpy.egg-info/top_level.txt
+mentpy/calculator/__init__.py
+mentpy/calculator/borrows.py
+mentpy/calculator/linalg2.py
 mentpy/gradients/__init__.py
 mentpy/gradients/finite_difference.py
 mentpy/mbqc/__init__.py
 mentpy/mbqc/flow.py
 mentpy/mbqc/mbqcircuit.py
 mentpy/mbqc/templates.py
 mentpy/mbqc/states/__init__.py
@@ -40,12 +43,11 @@
 mentpy/simulators/qiskit_simulators.py
 mentpy/utils/__init__.py
 mentpy/utils/expressivity.py
 mentpy/utils/flow_space.py
 mentpy/utils/generate_data.py
 mentpy/utils/lc_equivalence.py
 mentpy/utils/lie_algebra.py
-mentpy/utils/math.py
 tests/test_flow.py
 tests/test_graph_state.py
 tests/test_mbqc_templates.py
 tests/test_simulators.py
```

### Comparing `mentpy-0.1.0a6/setup.py` & `mentpy-0.1.0a7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.1.0a6"
+version = "0.1.0a7"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="mentpy",
     version=version,
```

### Comparing `mentpy-0.1.0a6/tests/test_mbqc_templates.py` & `mentpy-0.1.0a7/tests/test_mbqc_templates.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a6/tests/test_simulators.py` & `mentpy-0.1.0a7/tests/test_simulators.py`

 * *Files identical despite different names*

