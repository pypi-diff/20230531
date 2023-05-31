# Comparing `tmp/merlin-systems-23.4.0.tar.gz` & `tmp/merlin-systems-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-systems-23.4.0.tar", last modified: Tue May  2 21:26:48 2023, max compression
+gzip compressed data, was "merlin-systems-23.5.0.tar", last modified: Wed May 31 14:39:38 2023, max compression
```

## Comparing `merlin-systems-23.4.0.tar` & `merlin-systems-23.5.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.744853 merlin-systems-23.4.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/merlin/systems/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/merlin/systems/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.748853 merlin-systems-23.4.0/merlin/systems/dag/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/dag/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/feast.py
--rw-r--r--   0 runner    (1001) docker     (123)    18177 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/fil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/implicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/session_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/softmax_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/unroll_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/dag/runtimes/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/base_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17418 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/fil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/model_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/triton/
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/triton/models/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/models/executor_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/models/pytorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/models/workflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/workflow/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/merlin_systems.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/test-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/test-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81388 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.385280 merlin-systems-23.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-31 14:39:38.385280 merlin-systems-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.377279 merlin-systems-23.5.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.385280 merlin-systems-23.5.0/merlin/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:38.385280 merlin-systems-23.5.0/merlin/systems/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.377279 merlin-systems-23.5.0/merlin/systems/dag/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.381279 merlin-systems-23.5.0/merlin/systems/dag/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/feast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18177 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/fil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/session_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/softmax_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/unroll_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/ops/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.381279 merlin-systems-23.5.0/merlin/systems/dag/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/base_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.381279 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.381279 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/fil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/model_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.381279 merlin-systems-23.5.0/merlin/systems/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13908 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/triton/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/triton/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.381279 merlin-systems-23.5.0/merlin/systems/triton/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/triton/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/triton/models/executor_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/triton/models/pytorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/triton/models/workflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/triton/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.381279 merlin-systems-23.5.0/merlin/systems/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/merlin/systems/workflow/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.381279 merlin-systems-23.5.0/merlin_systems.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-31 14:39:38.000000 merlin-systems-23.5.0/merlin_systems.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-31 14:39:38.000000 merlin-systems-23.5.0/merlin_systems.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:38.000000 merlin-systems-23.5.0/merlin_systems.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:38.000000 merlin-systems-23.5.0/merlin_systems.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-31 14:39:38.000000 merlin-systems-23.5.0/merlin_systems.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 14:39:38.000000 merlin-systems-23.5.0/merlin_systems.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:38.385280 merlin-systems-23.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/requirements/gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/requirements/test-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/requirements/test-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-31 14:39:38.385280 merlin-systems-23.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81339 2023-05-31 14:39:31.000000 merlin-systems-23.5.0/versioneer.py
```

### Comparing `merlin-systems-23.4.0/LICENSE` & `merlin-systems-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/PKG-INFO` & `merlin-systems-23.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-systems
-Version: 23.4.0
+Version: 23.5.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/systems
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-systems-23.4.0/README.md` & `merlin-systems-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/__init__.py` & `merlin-systems-23.5.0/merlin/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/__init__.py` & `merlin-systems-23.5.0/merlin/systems/dag/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ensemble.py` & `merlin-systems-23.5.0/merlin/systems/dag/ensemble.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/node.py` & `merlin-systems-23.5.0/merlin/systems/dag/node.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/__init__.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/compat.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/compat.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/faiss.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/faiss.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/feast.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/feast.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from typing import List
 
 import numpy as np
 from feast import FeatureStore, ValueType
 
 from merlin.core.protocols import Transformable
 from merlin.dag import ColumnSelector
@@ -78,15 +79,15 @@
 
         input_schema = Schema(
             [ColumnSchema(column, dtype=entity_dtype, is_list=ent_is_list, is_ragged=ent_is_ragged)]
         )
 
         output_schema = Schema([])
         for feature in feature_view.features:
-            feature_dtype, is_list, is_ragged = feast_2_numpy[feature.dtype]
+            feature_dtype, is_list, is_ragged = feast_2_numpy[feature.dtype.to_value_type()]
 
             if is_list:
                 mh_features.append(feature.name)
             else:
                 features.append(feature.name)
 
             name = cls._prefixed_name(output_prefix, feature.name)
@@ -161,14 +162,17 @@
         self.mh_features = mh_features
         self.input_schema = input_schema
         self.output_schema = output_schema
         self.include_id = include_id
         self.output_prefix = output_prefix
 
         self.store = FeatureStore(repo_path=repo_path)
+        # add feature view to the online store
+        self.store.materialize_incremental(datetime.now(), feature_views=[self.entity_view])
+
         super().__init__()
 
     def __getstate__(self):
         # feature store objects aren't picklable - exclude from saved representation
         return {k: v for k, v in self.__dict__.items() if k != "store"}
 
     def load_artifacts(self, artifact_path):
```

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/fil.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/fil.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/implicit.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/implicit.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/operator.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/operator.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/pytorch.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/pytorch.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/session_filter.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/session_filter.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/softmax_sampling.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/softmax_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/tensorflow.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/tensorflow.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/unroll_features.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/unroll_features.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/ops/workflow.py` & `merlin-systems-23.5.0/merlin/systems/dag/ops/workflow.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/__init__.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/base_runtime.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/base_runtime.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/__init__.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/__init__.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/fil.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/fil.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,20 +141,26 @@
         input0 = (
             np.array([column.values.ravel() for column in transformable.values()])
             .astype(np.float32)
             .T
         )
 
         inputs = TensorTable({"input__0": input0})
+        input_schema = Schema(["input__0"])
+        output_schema = Schema(["output__0"])
 
         inference_request = tensor_table_to_triton_request(
-            self.fil_model_name, inputs, ["input__0"], ["output__0"]
+            self.fil_model_name, inputs, input_schema, output_schema
         )
         inference_response = inference_request.exec()
-        return triton_response_to_tensor_table(inference_response, type(inputs), ["output__0"])
+
+        if inference_response.has_error():
+            raise RuntimeError(str(inference_response.error().message()))
+
+        return triton_response_to_tensor_table(inference_response, type(inputs), output_schema)
 
 
 class FILTriton(TritonOperator):
     """Operator for Forest Inference Library (FIL) models.
 
     Packages up XGBoost models to run on Triton inference server using the fil backend.
     """
```

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/operator.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/operator.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/pytorch.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,22 +73,25 @@
         """
         self._torch_model_name = torch_model_name
 
     def transform(self, col_selector: ColumnSelector, transformable: Transformable):
         inference_request = tensor_table_to_triton_request(
             self.torch_model_name,
             transformable,
-            self.input_schema.column_names,
-            self.output_schema.column_names,
+            self.input_schema,
+            self.output_schema,
         )
 
         inference_response = inference_request.exec()
 
+        if inference_response.has_error():
+            raise RuntimeError(str(inference_response.error().message()))
+
         return triton_response_to_tensor_table(
-            inference_response, type(transformable), self.output_schema.column_names
+            inference_response, type(transformable), self.output_schema
         )
 
     def compute_input_schema(
         self,
         root_schema: Schema,
         parents_schema: Schema,
         deps_schema: Schema,
```

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/tensorflow.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/tensorflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,22 +67,25 @@
             TensorFlow Model Outputs
         """
         # TODO: Validate that the inputs match the schema
         # TODO: Should we coerce the dtypes to match the schema here?
         inference_request = tensor_table_to_triton_request(
             self.tf_model_name,
             transformable,
-            self.input_schema.column_names,
-            self.output_schema.column_names,
+            self.input_schema,
+            self.output_schema,
         )
         inference_response = inference_request.exec()
 
+        if inference_response.has_error():
+            raise RuntimeError(inference_response.error().message())
+
         # TODO: Validate that the outputs match the schema
         return triton_response_to_tensor_table(
-            inference_response, type(transformable), self.output_schema.column_names
+            inference_response, type(transformable), self.output_schema
         )
 
     def export(
         self,
         path: str,
         input_schema: Schema,
         output_schema: Schema,
```

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/workflow.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/ops/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import importlib.resources
 import json
 import os
 import pathlib
 from shutil import copyfile
 
 import tritonclient.grpc.model_config_pb2 as model_config
-import tritonclient.utils
 from google.protobuf import text_format
 
 from merlin.core.protocols import Transformable
 from merlin.dag import ColumnSelector
 from merlin.schema import ColumnSchema, Schema
 from merlin.systems.dag.runtimes.triton.ops.operator import TritonOperator
 from merlin.systems.triton.conversions import (
@@ -76,40 +75,28 @@
             A pandas or cudf dataframe that this operator will work on
 
         Returns
         -------
         TensorTable
             Returns a transformed dataframe for this operator"""
 
-        output_names = []
-        for col in self.output_schema:
-            if col.is_ragged:
-                output_names.append(f"{col.name}__values")
-                output_names.append(f"{col.name}__offsets")
-            else:
-                output_names.append(col.name)
-
         inference_request = tensor_table_to_triton_request(
             self._nvt_model_name,
             transformable,
-            self.input_schema.column_names,
-            output_names,
+            self.input_schema,
+            self.output_schema,
         )
 
         inference_response = inference_request.exec()
 
-        # check inference response for errors:
         if inference_response.has_error():
-            # Cannot raise inference response error because it is not derived from BaseException
-            raise tritonclient.utils.InferenceServerException(
-                str(inference_response.error().message())
-            )
+            raise RuntimeError(inference_response.error().message())
 
         response_table = triton_response_to_tensor_table(
-            inference_response, type(transformable), output_names
+            inference_response, type(transformable), self.output_schema
         )
 
         return response_table
 
     @classmethod
     def from_config(cls, config: dict, **kwargs) -> "TransformWorkflowTriton":
         """Instantiate the class from a dictionary representation.
```

### Comparing `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/runtime.py` & `merlin-systems-23.5.0/merlin/systems/dag/runtimes/triton/runtime.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/model_registry.py` & `merlin-systems-23.5.0/merlin/systems/model_registry.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/triton/__init__.py` & `merlin-systems-23.5.0/merlin/systems/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/triton/conversions.py` & `merlin-systems-23.5.0/merlin/systems/triton/conversions.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,27 +21,116 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 # OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import itertools
+from typing import Any, Dict, List
 
 import numpy as np
 import pandas as pd
 
 from merlin.core.compat import cudf
 from merlin.core.compat import cupy as cp
 from merlin.core.dispatch import build_cudf_list_column, is_list_dtype
 from merlin.dag import Supports
+from merlin.schema import Schema
 from merlin.systems.dag.ops.compat import pb_utils
 from merlin.table import TensorTable
 
 
-def triton_request_to_tensor_table(request, column_names):
+def tensor_names(schema: Schema) -> List[str]:
+    """
+    Compute the expected tensor names from a Merlin schema
+
+    This takes the columns from a schema, checks whether the columns are ragged or not,
+    and translates ragged columns to two separate tensor names for the values/offsets
+    representation.
+
+    Parameters
+    ----------
+    schema : Schema
+        Schema to compute tensor names for
+
+    Returns
+    -------
+    List[str]
+        A list of the tensors implied by the schema
+    """
+    tensor_names = []
+    for col_name, col_schema in schema.column_schemas.items():
+        if col_schema.is_ragged:
+            tensor_names.append(f"{col_name}__values")
+            tensor_names.append(f"{col_name}__offsets")
+        else:
+            tensor_names.append(col_name)
+    return tensor_names
+
+
+def match_representations(schema: Schema, dict_array: Dict[str, Any]) -> Dict[str, Any]:
+    """
+    Convert values-only tensors to values/offsets when indicated by the schema
+
+    Parameters
+    ----------
+    schema : Schema
+        Downstream input schema to match
+    dict_array : Dict[str, Any]
+        A dictionary of NumPy or CuPy ndarrays
+
+    Returns
+    -------
+    Dict[str, Any]
+        A dictionary of NumPy or CuPy ndarrays with representations adjusted
+    """
+    aligned = {}
+    for col_name, col_schema in schema.column_schemas.items():
+        if col_schema.is_ragged:
+            vals_name = f"{col_name}__values"
+            offs_name = f"{col_name}__offsets"
+
+            try:
+                # Look for values and offsets that already exist
+                aligned[vals_name] = dict_array[vals_name]
+                aligned[offs_name] = dict_array[offs_name]
+            except KeyError:
+                # If you don't find them, create the offsets
+                values, offsets = _to_values_offsets(dict_array[col_name])
+                aligned[vals_name] = values
+                aligned[offs_name] = offsets
+        else:
+            aligned[col_name] = dict_array[col_name]
+
+    return aligned
+
+
+def _to_values_offsets(array):
+    """Convert array to values/offsets representation
+
+    Parameters
+    ----------
+    array : numpy.ndarray or cupy.ndarray
+        Array to convert
+
+    Returns
+    -------
+    values, offsets
+        Tuple of values and offsets
+    """
+    num_rows = array.shape[0]
+    row_lengths = [array.shape[1]] * num_rows
+    offsets = [0] + list(itertools.accumulate(row_lengths))
+    array_lib = cp if cp and isinstance(array, cp.ndarray) else np
+    offsets = array_lib.array(offsets, dtype="int32")
+    values = array.reshape(-1, *array.shape[2:])
+    return values, offsets
+
+
+def triton_request_to_tensor_table(request, schema):
     """
     Turns a Triton request into a TensorTable by extracting individual tensors
     from the request using pb_utils.
 
     Parameters
     ----------
     request : TritonInferenceRequest
@@ -50,55 +139,41 @@
         List of the input columns to extract from the request
 
     Returns
     -------
     TensorTable
         Dictionary-like representation of the input columns
     """
-    dict_inputs = {}
-    for name in column_names:
-        try:
-            values = _array_from_triton_tensor(request, f"{name}__values")
-            lengths = _array_from_triton_tensor(request, f"{name}__offsets")
-            dict_inputs[name] = (values, lengths)
-        except (AttributeError, ValueError):
-            dict_inputs[name] = _array_from_triton_tensor(request, name)
-
-    return TensorTable(dict_inputs)
+    return TensorTable(
+        {name: _array_from_triton_tensor(request, name) for name in tensor_names(schema)}
+    )
 
 
-def tensor_table_to_triton_response(tensor_table):
+def tensor_table_to_triton_response(tensor_table, schema):
     """
     Turns a TensorTable into a Triton response that can be returned
     to resolve an incoming request.
 
     Parameters
     ----------
     tensor_table : TensorTable
         Dictionary-like representation of the output columns
 
     Returns
     -------
     response : TritonInferenceResponse
         The output response for predictions
     """
-    output_tensors = []
-    for name, column in tensor_table.items():
-        if column.offsets is not None:
-            values = _triton_tensor_from_array(f"{name}__values", column.values)
-            offsets = _triton_tensor_from_array(f"{name}__offsets", column.offsets)
-            output_tensors.extend([values, offsets])
-        else:
-            col_tensor = _triton_tensor_from_array(name, column.values)
-            output_tensors.append(col_tensor)
-
-    return pb_utils.InferenceResponse(output_tensors)
+    aligned = match_representations(schema, tensor_table.to_dict())
+    return pb_utils.InferenceResponse(
+        [_triton_tensor_from_array(name, array) for name, array in aligned.items()]
+    )
 
 
-def tensor_table_to_triton_request(model_name, tensor_table, input_col_names, output_col_names):
+def tensor_table_to_triton_request(model_name, tensor_table, input_schema, output_schema):
     """
     Turns a TensorTable into a Triton request that can, for example, be used to make a
     Business Logic Scripting call to a Triton model on the same Triton instance.
 
     Parameters
     ----------
     model_name : String
@@ -111,34 +186,25 @@
         List of the output columns to extract from the response
 
     Returns
     -------
     TritonInferenceRequest
         The TensorTable reformatted as a Triton request
     """
-    input_tensors = []
-
-    for name, column in tensor_table.items():
-        if name in input_col_names:
-            if column.offsets is not None:
-                values = _triton_tensor_from_array(f"{name}__values", column.values)
-                offsets = _triton_tensor_from_array(f"{name}__offsets", column.offsets)
-                input_tensors.extend([values, offsets])
-            else:
-                col_tensor = _triton_tensor_from_array(name, column.values)
-                input_tensors.append(col_tensor)
+    aligned = match_representations(input_schema, tensor_table.to_dict())
+    input_tensors = [_triton_tensor_from_array(name, tensor) for name, tensor in aligned.items()]
 
     return pb_utils.InferenceRequest(
         model_name=model_name,
-        requested_output_names=output_col_names,
+        requested_output_names=tensor_names(output_schema),
         inputs=input_tensors,
     )
 
 
-def triton_response_to_tensor_table(response, transformable_type, output_column_names):
+def triton_response_to_tensor_table(response, transformable_type, schema):
     """
     Turns a Triton response into a TensorTable by extracting individual tensors
     from the request using pb_utils.
 
     Parameters
     ----------
     response : pb_utils.InferenceResponse
@@ -149,28 +215,17 @@
         List of the output columns to extract from the response
 
     Returns
     -------
     Transformable
         A TensorTable or DataFrame representing the response columns from a Triton request
     """
-    outputs_dict = {}
-
-    for out_col_name in output_column_names:
-        try:
-            values = _array_from_triton_tensor(response, f"{out_col_name}__values")
-            lengths = _array_from_triton_tensor(response, f"{out_col_name}__offsets")
-            outputs_dict[out_col_name] = (values, lengths)
-        except (AttributeError, ValueError):
-            outputs_dict[out_col_name] = _array_from_triton_tensor(response, out_col_name)
-
-        output_val = _array_from_triton_tensor(response, out_col_name)
-        outputs_dict[out_col_name] = output_val
-
-    return transformable_type(outputs_dict)
+    return transformable_type(
+        {name: _array_from_triton_tensor(response, name) for name in tensor_names(schema)}
+    )
 
 
 def _triton_tensor_from_array(name, array):
     # The .get() here handles variations across Numpy versions, some of which
     # require .get() to be used here and some of which don't.
     array = array.get() if hasattr(array, "get") else array
     if not isinstance(array, np.ndarray):
```

### Comparing `merlin-systems-23.4.0/merlin/systems/triton/export.py` & `merlin-systems-23.5.0/merlin/systems/triton/export.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/triton/models/__init__.py` & `merlin-systems-23.5.0/merlin/systems/triton/models/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/triton/models/executor_model.py` & `merlin-systems-23.5.0/merlin/systems/triton/models/executor_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 # OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import pathlib
 from pathlib import Path
 
+import triton_python_backend_utils as pb_utils
+
 from merlin.dag import postorder_iter_nodes
 from merlin.systems.dag import Ensemble
 from merlin.systems.dag.runtimes.triton import TritonExecutorRuntime
 from merlin.systems.triton.conversions import (
     tensor_table_to_triton_response,
     triton_request_to_tensor_table,
 )
@@ -88,17 +90,27 @@
 
         Returns
         -------
         list
           A list of pb_utils.InferenceResponse. The length of this list must
           be the same as `requests`
         """
-        inputs = triton_request_to_tensor_table(request, self.ensemble.input_schema.column_names)
-        outputs = self.ensemble.transform(inputs, runtime=TritonExecutorRuntime())
-        return tensor_table_to_triton_response(outputs)
+        inputs = triton_request_to_tensor_table(request, self.ensemble.input_schema)
+
+        try:
+            outputs = self.ensemble.transform(inputs, runtime=TritonExecutorRuntime())
+        except Exception as exc:
+            import traceback
+
+            raise pb_utils.TritonModelException(
+                f"Error: {type(exc)} - {str(exc)}, "
+                f"Traceback: {traceback.format_tb(exc.__traceback__)}"
+            ) from exc
+
+        return tensor_table_to_triton_response(outputs, self.ensemble.output_schema)
 
 
 def _parse_model_repository(model_repository: str) -> str:
     """
     Extract the model repository path from the model_repository value
     passed to the TritonPythonModel initialize method.
     """
```

### Comparing `merlin-systems-23.4.0/merlin/systems/triton/models/pytorch_model.py` & `merlin-systems-23.5.0/merlin/systems/triton/models/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/triton/models/workflow_model.py` & `merlin-systems-23.5.0/merlin/systems/triton/models/workflow_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,32 +93,43 @@
 
     @triton_multi_request
     @triton_error_handling
     def execute(self, request):
         """Transforms the input batches by running through a NVTabular workflow.transform
         function.
         """
-        # transform the triton tensors to a dict of name:numpy tensor
-        input_tensors = {
-            name: _convert_tensor(pb_utils.get_input_tensor_by_name(request, name))
-            for name in self.input_dtypes
-        }
-
-        # multihots are represented as a tuple of (values, offsets)
-        for name, dtype in self.input_multihots.items():
-            values = _convert_tensor(pb_utils.get_input_tensor_by_name(request, name + "__values"))
-            offsets = _convert_tensor(
-                pb_utils.get_input_tensor_by_name(request, name + "__offsets")
-            )
-            input_tensors[name] = (values, offsets)
+        try:
+            # transform the triton tensors to a dict of name:numpy tensor
+            input_tensors = {
+                name: _convert_tensor(pb_utils.get_input_tensor_by_name(request, name))
+                for name in self.input_dtypes
+            }
 
-        transformed = self.runner.run_workflow(input_tensors)
-        result = [pb_utils.Tensor(name, data) for name, data in transformed.items()]
+            # multihots are represented as a tuple of (values, offsets)
+            for name, dtype in self.input_multihots.items():
+                values = _convert_tensor(
+                    pb_utils.get_input_tensor_by_name(request, name + "__values")
+                )
+                offsets = _convert_tensor(
+                    pb_utils.get_input_tensor_by_name(request, name + "__offsets")
+                )
+                input_tensors[name] = (values, offsets)
 
-        return pb_utils.InferenceResponse(result)
+            transformed = self.runner.run_workflow(input_tensors)
+            result = [pb_utils.Tensor(name, data) for name, data in transformed.items()]
+
+            return pb_utils.InferenceResponse(result)
+
+        except Exception as exc:
+            import traceback
+
+            raise pb_utils.TritonModelException(
+                f"Error: {type(exc)} - {str(exc)}, "
+                f"Traceback: {traceback.format_tb(exc.__traceback__)}"
+            ) from exc
 
     def _is_list_dtype(self, column: str) -> bool:
         """Check if a column of a Workflow contains list elements"""
         col_schema = self.workflow.input_schema.get(column)
         if col_schema is None:
             return False
         return col_schema.is_list and col_schema.is_ragged
```

### Comparing `merlin-systems-23.4.0/merlin/systems/triton/utils.py` & `merlin-systems-23.5.0/merlin/systems/triton/utils.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin/systems/workflow/__init__.py` & `merlin-systems-23.5.0/merlin/systems/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin_systems.egg-info/PKG-INFO` & `merlin-systems-23.5.0/merlin_systems.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-systems
-Version: 23.4.0
+Version: 23.5.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/systems
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-systems-23.4.0/merlin_systems.egg-info/SOURCES.txt` & `merlin-systems-23.5.0/merlin_systems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/merlin_systems.egg-info/requires.txt` & `merlin-systems-23.5.0/merlin_systems.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-merlin-core>=23.4.0
-nvtabular>=23.4.0
+merlin-core>=0.2.0
+nvtabular>=1.0.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
-tritonclient[all]
 
 [cpu]
-merlin-core>=23.4.0
-nvtabular>=23.4.0
+merlin-core>=0.2.0
+nvtabular>=1.0.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
-tritonclient[all]
 
 [dev]
 tritonclient[all]
 
 [docs]
-merlin-core>=23.4.0
-nvtabular>=23.4.0
+merlin-core>=0.2.0
+nvtabular>=1.0.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
 tritonclient[all]
 tritonclient[all]
 tensorflow<=2.9.0
 Sphinx==3.5.4
@@ -42,66 +40,66 @@
 faiss-gpu
 pytest
 pytest-cov
 dask>=2022.3.0
 distributed>=2022.3.0
 
 [test]
-merlin-core>=23.4.0
-nvtabular>=23.4.0
+merlin-core>=0.2.0
+nvtabular>=1.0.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
 tritonclient[all]
-tritonclient[all]
 pytest>=5
 pytest-cov>=2
 scikit-learn<1.2
 asvdb@ git+https://github.com/rapidsai/asvdb.git
 testbook==0.4.2
-feast==0.18.1
+tritonclient
+feast==0.31
 xgboost==1.6.2
 implicit==0.6.0
 
 [test-cpu]
-merlin-core>=23.4.0
-nvtabular>=23.4.0
+merlin-core>=0.2.0
+nvtabular>=1.0.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
 tritonclient[all]
-tritonclient[all]
 pytest>=5
 pytest-cov>=2
 scikit-learn<1.2
 asvdb@ git+https://github.com/rapidsai/asvdb.git
 testbook==0.4.2
-feast==0.18.1
+tritonclient
+feast==0.31
 xgboost==1.6.2
 implicit==0.6.0
-merlin-models>=23.4.0
+merlin-models>=0.6.0
 faiss-cpu==1.7.2
 tensorflow<=2.9.0
 treelite==2.4.0
 treelite_runtime==2.4.0
 torch~=1.12
 lightgbm==3.3.2
 ipykernel
 
 [test-gpu]
-merlin-core>=23.4.0
-nvtabular>=23.4.0
+merlin-core>=0.2.0
+nvtabular>=1.0.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
 tritonclient[all]
-tritonclient[all]
 pytest>=5
 pytest-cov>=2
 scikit-learn<1.2
 asvdb@ git+https://github.com/rapidsai/asvdb.git
 testbook==0.4.2
-feast==0.18.1
+tritonclient
+feast==0.31
 xgboost==1.6.2
 implicit==0.6.0
-tensorflow-gpu<=2.9.0
+tensorflow
 faiss-gpu==1.7.2
```

### Comparing `merlin-systems-23.4.0/pyproject.toml` & `merlin-systems-23.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/requirements/test.txt` & `merlin-systems-23.5.0/requirements/test.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 pytest>=5
 pytest-cov>=2
 scikit-learn<1.2
 asvdb@git+https://github.com/rapidsai/asvdb.git
 testbook==0.4.2
 
 # packages necessary to run tests and push PRs
-feast==0.18.1
+tritonclient
+feast==0.31
 xgboost==1.6.2
 implicit==0.6.0
 
 # TODO: do we need more of these?
 # https://github.com/NVIDIA-Merlin/Merlin/blob/a1cc48fe23c4dfc627423168436f26ef7e028204/ci/dockerfile.ci#L13-L18
```

### Comparing `merlin-systems-23.4.0/setup.cfg` & `merlin-systems-23.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.4.0/setup.py` & `merlin-systems-23.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 }
 
 with open("README.md", encoding="utf8") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="merlin-systems",
-    version="23.04.00",
+    version=versioneer.get_version(),
     packages=find_namespace_packages(include=["merlin*"]),
     url="https://github.com/NVIDIA-Merlin/systems",
     author="NVIDIA Corporation",
     license="Apache 2.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `merlin-systems-23.4.0/versioneer.py` & `merlin-systems-23.5.0/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1700,17 +1700,14 @@
 
 
 def get_versions(verbose=False):
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
-    return {
-        "version": "23.04.00"
-    }
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
```

