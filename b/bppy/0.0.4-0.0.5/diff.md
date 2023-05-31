# Comparing `tmp/bppy-0.0.4.tar.gz` & `tmp/bppy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bppy-0.0.4.tar", last modified: Sun Feb  5 14:04:47 2023, max compression
+gzip compressed data, was "bppy-0.0.5.tar", last modified: Wed May 31 14:48:36 2023, max compression
```

## Comparing `bppy-0.0.4.tar` & `bppy-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:47.897365 bppy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-05 14:04:35.000000 bppy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-05 14:04:35.000000 bppy-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-02-05 14:04:47.897365 bppy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-02-05 14:04:35.000000 bppy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:47.893365 bppy-0.0.4/bppy/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:47.893365 bppy-0.0.4/bppy/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/examples/exponential_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/examples/external_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/examples/hot_cold_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/examples/hot_cold_bath.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/examples/hot_cold_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/examples/hot_cold_smt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/examples/robots_smt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:47.893365 bppy-0.0.4/bppy/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:47.897365 bppy-0.0.4/bppy/execution/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/execution/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/execution/listeners/b_program_runner_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/execution/listeners/print_b_program_runner_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:47.897365 bppy-0.0.4/bppy/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/b_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/b_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/bprogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:47.897365 bppy-0.0.4/bppy/model/event_selection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/event_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/event_selection/event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/event_selection/experimental_smt_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/event_selection/simple_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/event_selection/smt_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/event_selection/solver_based_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/event_set.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/model/sync_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:47.897365 bppy-0.0.4/bppy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-05 14:04:35.000000 bppy-0.0.4/bppy/utils/z3helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:04:47.893365 bppy-0.0.4/bppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-02-05 14:04:47.000000 bppy-0.0.4/bppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-02-05 14:04:47.000000 bppy-0.0.4/bppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 14:04:47.000000 bppy-0.0.4/bppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-05 14:04:47.000000 bppy-0.0.4/bppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-05 14:04:47.000000 bppy-0.0.4/bppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-05 14:04:47.897365 bppy-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-05 14:04:35.000000 bppy-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.863540 bppy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 14:48:25.000000 bppy-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 14:48:25.000000 bppy-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-31 14:48:36.863540 bppy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-31 14:48:25.000000 bppy-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/exponential_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/external_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hot_cold_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hot_cold_bath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hot_cold_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hot_cold_smt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/robots_smt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/tic_tac_toe_priorities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/execution/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/execution/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/execution/listeners/b_program_runner_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/execution/listeners/print_b_program_runner_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/b_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/b_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/bprogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/model/event_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/experimental_smt_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/priority_based_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/simple_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/smt_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/solver_based_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/sync_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.863540 bppy-0.0.5/bppy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/utils/z3helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:48:36.863540 bppy-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-31 14:48:25.000000 bppy-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.863540 bppy-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-31 14:48:25.000000 bppy-0.0.5/tests/test_bprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-05-31 14:48:25.000000 bppy-0.0.5/tests/test_examples.py
```

### Comparing `bppy-0.0.4/LICENSE` & `bppy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/__init__.py` & `bppy-0.0.5/bppy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from bppy.execution.listeners.b_program_runner_listener import *
 from bppy.execution.listeners.print_b_program_runner_listener import *
 from bppy.model.event_selection.event_selection_strategy import *
 from bppy.model.event_selection.simple_event_selection_strategy import *
 from bppy.model.event_selection.solver_based_event_selection_strategy import *
 from bppy.model.event_selection.smt_event_selection_strategy import *
 from bppy.model.event_selection.experimental_smt_event_selection_strategy import *
+from bppy.model.event_selection.priority_based_event_selection_strategy import *
 from bppy.model.b_event import *
 from bppy.model.bprogram import *
 from bppy.model.event_set import *
 from bppy.model.sync_statement import *
 from bppy.model.b_thread import *
 from bppy.utils.z3helper import *
```

### Comparing `bppy-0.0.4/bppy/examples/external_events.py` & `bppy-0.0.5/bppy/examples/external_events.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/examples/hot_cold_all.py` & `bppy-0.0.5/bppy/examples/hot_cold_all.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/examples/hot_cold_bath.py` & `bppy-0.0.5/bppy/examples/hot_cold_bath.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/examples/hot_cold_dynamic.py` & `bppy-0.0.5/bppy/examples/hot_cold_dynamic.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/examples/hot_cold_smt.py` & `bppy-0.0.5/bppy/examples/hot_cold_smt.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/examples/robots_smt.py` & `bppy-0.0.5/bppy/examples/robots_smt.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/execution/listeners/b_program_runner_listener.py` & `bppy-0.0.5/bppy/execution/listeners/b_program_runner_listener.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/execution/listeners/print_b_program_runner_listener.py` & `bppy-0.0.5/bppy/execution/listeners/print_b_program_runner_listener.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/model/b_event.py` & `bppy-0.0.5/bppy/model/b_event.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/model/event_selection/simple_event_selection_strategy.py` & `bppy-0.0.5/bppy/model/event_selection/simple_event_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/model/event_selection/smt_event_selection_strategy.py` & `bppy-0.0.5/bppy/model/event_selection/smt_event_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/model/event_set.py` & `bppy-0.0.5/bppy/model/event_set.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy/utils/z3helper.py` & `bppy-0.0.5/bppy/utils/z3helper.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.4/bppy.egg-info/SOURCES.txt` & `bppy-0.0.5/bppy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,25 +12,29 @@
 bppy/examples/external_events.py
 bppy/examples/hello_world.py
 bppy/examples/hot_cold_all.py
 bppy/examples/hot_cold_bath.py
 bppy/examples/hot_cold_dynamic.py
 bppy/examples/hot_cold_smt.py
 bppy/examples/robots_smt.py
+bppy/examples/tic_tac_toe_priorities.py
 bppy/execution/__init__.py
 bppy/execution/listeners/__init__.py
 bppy/execution/listeners/b_program_runner_listener.py
 bppy/execution/listeners/print_b_program_runner_listener.py
 bppy/model/__init__.py
 bppy/model/b_event.py
 bppy/model/b_thread.py
 bppy/model/bprogram.py
 bppy/model/event_set.py
 bppy/model/sync_statement.py
 bppy/model/event_selection/__init__.py
 bppy/model/event_selection/event_selection_strategy.py
 bppy/model/event_selection/experimental_smt_event_selection_strategy.py
+bppy/model/event_selection/priority_based_event_selection_strategy.py
 bppy/model/event_selection/simple_event_selection_strategy.py
 bppy/model/event_selection/smt_event_selection_strategy.py
 bppy/model/event_selection/solver_based_event_selection_strategy.py
 bppy/utils/__init__.py
-bppy/utils/z3helper.py
+bppy/utils/z3helper.py
+tests/test_bprogram.py
+tests/test_examples.py
```

