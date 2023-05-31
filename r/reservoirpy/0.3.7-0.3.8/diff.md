# Comparing `tmp/reservoirpy-0.3.7.tar.gz` & `tmp/reservoirpy-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reservoirpy-0.3.7.tar", last modified: Mon Mar 20 10:59:40 2023, max compression
+gzip compressed data, was "reservoirpy-0.3.8.tar", last modified: Wed May 31 15:20:58 2023, max compression
```

## Comparing `reservoirpy-0.3.7.tar` & `reservoirpy-0.3.8.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.742548 reservoirpy-0.3.7/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1066 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/LICENSE
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    12580 2023-03-20 10:59:40.742548 reservoirpy-0.3.7/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    10961 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/README.md
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      217 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/pyproject.toml
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.730548 reservoirpy-0.3.7/reservoirpy/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      888 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    24076 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/reservoirpy/_base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       22 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/reservoirpy/_version.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3923 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/activationsfunc.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.730548 reservoirpy-0.3.7/reservoirpy/compat/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5647 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/compat/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    25130 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/_base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    10288 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/_esn.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    17763 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/_esn_online.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     7950 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/compat/regression_models.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.730548 reservoirpy-0.3.7/reservoirpy/compat/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       40 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     7040 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/tests/test_esn.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2288 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/tests/test_esnonline.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2301 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/tests/test_load_from_previous_versions.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2434 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/tests/test_regression_models.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3573 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/tests/test_validation.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.734548 reservoirpy-0.3.7/reservoirpy/compat/utils/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/utils/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4650 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/compat/utils/parallel.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5534 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/utils/save.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6591 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/compat/utils/validation.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.734548 reservoirpy-0.3.7/reservoirpy/datasets/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     9167 2023-03-17 08:49:20.000000 reservoirpy-0.3.7/reservoirpy/datasets/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    26022 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/reservoirpy/datasets/_chaos.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5451 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/datasets/_japanese_vowels.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      832 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/datasets/_seed.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      515 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/datasets/_utils.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.734548 reservoirpy-0.3.7/reservoirpy/datasets/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/datasets/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3958 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/datasets/tests/test_datasets.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.734548 reservoirpy-0.3.7/reservoirpy/experimental/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1078 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/experimental/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1658 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/experimental/add.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3381 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/experimental/batchforce.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.734548 reservoirpy-0.3.7/reservoirpy/experimental/gpu/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/experimental/gpu/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1149 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/experimental/norm.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      937 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/experimental/randomchoice.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1106 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/experimental/sklearn.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.734548 reservoirpy-0.3.7/reservoirpy/experimental/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       48 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/experimental/tests/__init__.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.734548 reservoirpy-0.3.7/reservoirpy/hyper/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      746 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/hyper/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    11789 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/hyper/_hyperplot.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6067 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/hyper/_hypersearch.py
--rwxrwxr-x   0 nathan    (1000) nathan    (1000)    32665 2023-03-17 08:47:36.000000 reservoirpy-0.3.7/reservoirpy/mat_gen.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    38076 2023-03-17 18:09:50.000000 reservoirpy-0.3.7/reservoirpy/model.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    40127 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/node.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.734548 reservoirpy-0.3.7/reservoirpy/nodes/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2553 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6113 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/activations.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1963 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/concat.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    12376 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/esn.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2794 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/io.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.738548 reservoirpy-0.3.7/reservoirpy/nodes/readouts/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      136 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/readouts/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3349 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/readouts/base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5785 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/readouts/force.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4797 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/readouts/lms.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6012 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/readouts/ridge.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4437 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/readouts/rls.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.738548 reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      299 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     8471 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    18699 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/intrinsic_plasticity.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6370 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/nvar.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    14000 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/reservoir.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.738548 reservoirpy-0.3.7/reservoirpy/nodes/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       48 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      493 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_activations.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1013 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_concat.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3706 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_esn.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5804 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_force.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2000 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_intrinsic_plasticity.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      720 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_io.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3945 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_lms.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1053 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_nvar.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6462 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_reservoir.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3220 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_ridge.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4419 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/nodes/tests/test_rls.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6038 2023-03-17 08:49:20.000000 reservoirpy-0.3.7/reservoirpy/observables.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    13703 2023-03-17 18:02:32.000000 reservoirpy-0.3.7/reservoirpy/ops.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.742548 reservoirpy-0.3.7/reservoirpy/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       44 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     8546 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/tests/dummy_nodes.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2070 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/tests/test_activationsfunc.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    10705 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/tests/test_base.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    15591 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/tests/test_mat_gen.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    14441 2023-03-17 18:09:50.000000 reservoirpy-0.3.7/reservoirpy/tests/test_model.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    11827 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/tests/test_node.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1819 2023-03-17 08:49:20.000000 reservoirpy-0.3.7/reservoirpy/tests/test_observables.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2690 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/tests/test_ops.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2398 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/type.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.742548 reservoirpy-0.3.7/reservoirpy/utils/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1005 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/utils/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     8919 2023-03-17 18:09:50.000000 reservoirpy-0.3.7/reservoirpy/utils/graphflow.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5618 2023-03-17 18:09:50.000000 reservoirpy-0.3.7/reservoirpy/utils/model_utils.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2412 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/reservoirpy/utils/parallel.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2104 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/reservoirpy/utils/random.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.742548 reservoirpy-0.3.7/reservoirpy/utils/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/utils/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1202 2023-03-20 10:54:59.000000 reservoirpy-0.3.7/reservoirpy/utils/tests/test_random.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1417 2023-02-05 11:29:19.000000 reservoirpy-0.3.7/reservoirpy/utils/tests/test_utils.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4891 2023-03-17 08:48:30.000000 reservoirpy-0.3.7/reservoirpy/utils/validation.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-03-20 10:59:40.730548 reservoirpy-0.3.7/reservoirpy.egg-info/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    12580 2023-03-20 10:59:40.000000 reservoirpy-0.3.7/reservoirpy.egg-info/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3313 2023-03-20 10:59:40.000000 reservoirpy-0.3.7/reservoirpy.egg-info/SOURCES.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2023-03-20 10:59:40.000000 reservoirpy-0.3.7/reservoirpy.egg-info/dependency_links.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      130 2023-03-20 10:59:40.000000 reservoirpy-0.3.7/reservoirpy.egg-info/requires.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       12 2023-03-20 10:59:40.000000 reservoirpy-0.3.7/reservoirpy.egg-info/top_level.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      522 2023-03-20 10:59:40.742548 reservoirpy-0.3.7/setup.cfg
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2633 2023-03-17 08:49:21.000000 reservoirpy-0.3.7/setup.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1066 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/LICENSE
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    12580 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    10961 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/README.md
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      217 2023-03-20 16:00:23.000000 reservoirpy-0.3.8/pyproject.toml
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.209360 reservoirpy-0.3.8/reservoirpy/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      888 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    24076 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/_base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       22 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/_version.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3923 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/activationsfunc.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.209360 reservoirpy-0.3.8/reservoirpy/compat/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5647 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/compat/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    25130 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/_base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    10288 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/_esn.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    17763 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/_esn_online.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     7950 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/compat/regression_models.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.209360 reservoirpy-0.3.8/reservoirpy/compat/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       40 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     7040 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_esn.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2288 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_esnonline.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2301 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_load_from_previous_versions.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2434 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_regression_models.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3573 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/tests/test_validation.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/compat/utils/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/utils/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4650 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/utils/parallel.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5534 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/compat/utils/save.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6591 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/compat/utils/validation.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/datasets/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     9167 2023-03-17 08:49:20.000000 reservoirpy-0.3.8/reservoirpy/datasets/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    26022 2023-03-20 16:00:23.000000 reservoirpy-0.3.8/reservoirpy/datasets/_chaos.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5451 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/datasets/_japanese_vowels.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      832 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/datasets/_seed.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      515 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/datasets/_utils.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/datasets/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/datasets/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3958 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/datasets/tests/test_datasets.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/experimental/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1078 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1658 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/add.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3381 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/experimental/batchforce.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/experimental/gpu/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/gpu/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1149 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/norm.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      937 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/randomchoice.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1106 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/sklearn.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/experimental/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       48 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/experimental/tests/__init__.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/hyper/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      746 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/hyper/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    11789 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/hyper/_hyperplot.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6067 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/hyper/_hypersearch.py
+-rwxrwxr-x   0 nathan    (1000) nathan    (1000)    32665 2023-05-31 15:17:24.000000 reservoirpy-0.3.8/reservoirpy/mat_gen.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    38076 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/model.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    40127 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/node.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/nodes/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2553 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/nodes/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6113 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/activations.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1963 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/nodes/concat.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    12376 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/esn.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2794 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/io.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.213360 reservoirpy-0.3.8/reservoirpy/nodes/readouts/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      136 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3349 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5785 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/force.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4797 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/lms.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6012 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/ridge.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4437 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/readouts/rls.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      299 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     8535 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    18731 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/intrinsic_plasticity.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6370 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/nvar.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    14032 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/reservoir.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/nodes/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       48 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      493 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_activations.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1013 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_concat.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3706 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_esn.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5804 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_force.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2000 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_intrinsic_plasticity.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      720 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_io.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3945 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_lms.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1053 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_nvar.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6889 2023-05-31 15:17:28.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_reservoir.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3220 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_ridge.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4419 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/nodes/tests/test_rls.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6038 2023-03-17 08:49:20.000000 reservoirpy-0.3.8/reservoirpy/observables.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    13703 2023-04-15 10:20:03.000000 reservoirpy-0.3.8/reservoirpy/ops.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       44 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     8546 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/tests/dummy_nodes.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2070 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/tests/test_activationsfunc.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    10705 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_base.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    15591 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_mat_gen.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    14441 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_model.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    11827 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_node.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1819 2023-03-17 08:49:20.000000 reservoirpy-0.3.8/reservoirpy/tests/test_observables.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2690 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/tests/test_ops.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2398 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/type.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/utils/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1005 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/utils/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     8919 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/utils/graphflow.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5618 2023-03-17 18:09:50.000000 reservoirpy-0.3.8/reservoirpy/utils/model_utils.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2412 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/utils/parallel.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2104 2023-03-20 16:00:23.000000 reservoirpy-0.3.8/reservoirpy/utils/random.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/reservoirpy/utils/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-02-05 11:29:19.000000 reservoirpy-0.3.8/reservoirpy/utils/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1202 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/utils/tests/test_random.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1417 2023-05-31 13:58:10.000000 reservoirpy-0.3.8/reservoirpy/utils/tests/test_utils.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4891 2023-03-17 08:48:30.000000 reservoirpy-0.3.8/reservoirpy/utils/validation.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-31 15:20:58.209360 reservoirpy-0.3.8/reservoirpy.egg-info/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    12580 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3313 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      130 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/requires.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       12 2023-05-31 15:20:58.000000 reservoirpy-0.3.8/reservoirpy.egg-info/top_level.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      522 2023-05-31 15:20:58.217360 reservoirpy-0.3.8/setup.cfg
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2633 2023-03-17 08:49:21.000000 reservoirpy-0.3.8/setup.py
```

### Comparing `reservoirpy-0.3.7/LICENSE` & `reservoirpy-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/PKG-INFO` & `reservoirpy-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reservoirpy
-Version: 0.3.7
+Version: 0.3.8
 Summary: A simple and flexible code for Reservoir Computing architectures like Echo State Networks.
 Home-page: https://github.com/reservoirpy/reservoirpy
-Download-URL: https://github.com/reservoirpy/reservoirpy/v0.3.7.tar.gz
+Download-URL: https://github.com/reservoirpy/reservoirpy/v0.3.8.tar.gz
 Author: Xavier Hinaut
 Author-email: xavier.hinaut@inria.fr
 Maintainer: Xavier Hinaut, Nathan Trouvain
 Maintainer-email: xavier.hinaut@inria.fr, nathan.trouvain@inria.fr
 Project-URL: Bug Tracker, https://github.com/reservoirpy/reservoirpy/issues
 Project-URL: Documentation, https://reservoirpy.readthedocs.io/en/latest/index.html
 Project-URL: Source Code, https://github.com/reservoirpy/reservoirpy
@@ -40,15 +40,15 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reservoirpy)
 [![PyPI version](https://badge.fury.io/py/reservoirpy.svg)](https://badge.fury.io/py/reservoirpy)
 [![Documentation Status](https://readthedocs.org/projects/reservoirpy/badge/?version=latest)](https://reservoirpy.readthedocs.io/en/latest/?badge=latest)
 [![Testing](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/reservoirpy/reservoirpy/branch/master/graph/badge.svg?token=JC8R1PB5EO)](https://codecov.io/gh/reservoirpy/reservoirpy)
 
-# ReservoirPy (v0.3.7) 🌀🧠
+# ReservoirPy (v0.3.8) 🌀🧠
 **Simple and flexible code for Reservoir Computing architectures like Echo State Networks (ESN).**
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/reservoirpy/reservoirpy/HEAD)
 
 ```python
 from reservoirpy.nodes import Reservoir, Ridge, Input
```

### Comparing `reservoirpy-0.3.7/README.md` & `reservoirpy-0.3.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reservoirpy)
 [![PyPI version](https://badge.fury.io/py/reservoirpy.svg)](https://badge.fury.io/py/reservoirpy)
 [![Documentation Status](https://readthedocs.org/projects/reservoirpy/badge/?version=latest)](https://reservoirpy.readthedocs.io/en/latest/?badge=latest)
 [![Testing](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/reservoirpy/reservoirpy/branch/master/graph/badge.svg?token=JC8R1PB5EO)](https://codecov.io/gh/reservoirpy/reservoirpy)
 
-# ReservoirPy (v0.3.7) 🌀🧠
+# ReservoirPy (v0.3.8) 🌀🧠
 **Simple and flexible code for Reservoir Computing architectures like Echo State Networks (ESN).**
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/reservoirpy/reservoirpy/HEAD)
 
 ```python
 from reservoirpy.nodes import Reservoir, Ridge, Input
```

### Comparing `reservoirpy-0.3.7/reservoirpy/__init__.py` & `reservoirpy-0.3.8/reservoirpy/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/_base.py` & `reservoirpy-0.3.8/reservoirpy/_base.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/activationsfunc.py` & `reservoirpy-0.3.8/reservoirpy/activationsfunc.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/__init__.py` & `reservoirpy-0.3.8/reservoirpy/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/_base.py` & `reservoirpy-0.3.8/reservoirpy/compat/_base.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/_esn.py` & `reservoirpy-0.3.8/reservoirpy/compat/_esn.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/_esn_online.py` & `reservoirpy-0.3.8/reservoirpy/compat/_esn_online.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/regression_models.py` & `reservoirpy-0.3.8/reservoirpy/compat/regression_models.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/tests/test_esn.py` & `reservoirpy-0.3.8/reservoirpy/compat/tests/test_esn.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/tests/test_esnonline.py` & `reservoirpy-0.3.8/reservoirpy/compat/tests/test_esnonline.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/tests/test_load_from_previous_versions.py` & `reservoirpy-0.3.8/reservoirpy/compat/tests/test_load_from_previous_versions.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/tests/test_regression_models.py` & `reservoirpy-0.3.8/reservoirpy/compat/tests/test_regression_models.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/tests/test_validation.py` & `reservoirpy-0.3.8/reservoirpy/compat/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/utils/parallel.py` & `reservoirpy-0.3.8/reservoirpy/compat/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/utils/save.py` & `reservoirpy-0.3.8/reservoirpy/compat/utils/save.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/compat/utils/validation.py` & `reservoirpy-0.3.8/reservoirpy/compat/utils/validation.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/datasets/__init__.py` & `reservoirpy-0.3.8/reservoirpy/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/datasets/_chaos.py` & `reservoirpy-0.3.8/reservoirpy/datasets/_chaos.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/datasets/_japanese_vowels.py` & `reservoirpy-0.3.8/reservoirpy/datasets/_japanese_vowels.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/datasets/_seed.py` & `reservoirpy-0.3.8/reservoirpy/datasets/_seed.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/datasets/_utils.py` & `reservoirpy-0.3.8/reservoirpy/datasets/_utils.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/datasets/tests/test_datasets.py` & `reservoirpy-0.3.8/reservoirpy/datasets/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/experimental/__init__.py` & `reservoirpy-0.3.8/reservoirpy/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/experimental/add.py` & `reservoirpy-0.3.8/reservoirpy/experimental/add.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/experimental/batchforce.py` & `reservoirpy-0.3.8/reservoirpy/experimental/batchforce.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/experimental/norm.py` & `reservoirpy-0.3.8/reservoirpy/experimental/norm.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/experimental/randomchoice.py` & `reservoirpy-0.3.8/reservoirpy/experimental/randomchoice.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/experimental/sklearn.py` & `reservoirpy-0.3.8/reservoirpy/experimental/sklearn.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/hyper/__init__.py` & `reservoirpy-0.3.8/reservoirpy/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/hyper/_hyperplot.py` & `reservoirpy-0.3.8/reservoirpy/hyper/_hyperplot.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/hyper/_hypersearch.py` & `reservoirpy-0.3.8/reservoirpy/hyper/_hypersearch.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/mat_gen.py` & `reservoirpy-0.3.8/reservoirpy/mat_gen.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/model.py` & `reservoirpy-0.3.8/reservoirpy/model.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/node.py` & `reservoirpy-0.3.8/reservoirpy/node.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/__init__.py` & `reservoirpy-0.3.8/reservoirpy/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/activations.py` & `reservoirpy-0.3.8/reservoirpy/nodes/activations.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/concat.py` & `reservoirpy-0.3.8/reservoirpy/nodes/concat.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/esn.py` & `reservoirpy-0.3.8/reservoirpy/nodes/esn.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/io.py` & `reservoirpy-0.3.8/reservoirpy/nodes/io.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/readouts/base.py` & `reservoirpy-0.3.8/reservoirpy/nodes/readouts/base.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/readouts/force.py` & `reservoirpy-0.3.8/reservoirpy/nodes/readouts/force.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/readouts/lms.py` & `reservoirpy-0.3.8/reservoirpy/nodes/readouts/lms.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/readouts/ridge.py` & `reservoirpy-0.3.8/reservoirpy/nodes/readouts/ridge.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/readouts/rls.py` & `reservoirpy-0.3.8/reservoirpy/nodes/readouts/rls.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/base.py` & `reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     g_rc = reservoir.noise_rc
     noise_gen = reservoir.noise_generator
 
     u = x.reshape(-1, 1)
     r = reservoir.state().T
 
     s_next = (
-        (1 - lr) * r
-        + lr * f(reservoir_kernel(reservoir, u, r))
+        np.multiply((1 - lr), r.T).T
+        + np.multiply(lr, f(reservoir_kernel(reservoir, u, r)).T).T
         + noise_gen(dist=dist, shape=r.shape, gain=g_rc)
     )
 
     return s_next.T
 
 
 def forward_external(reservoir, x: np.ndarray) -> np.ndarray:
@@ -83,16 +83,16 @@
     noise_gen = reservoir.noise_generator
 
     u = x.reshape(-1, 1)
     r = reservoir.state().T
     s = reservoir.internal_state.T
 
     s_next = (
-        (1 - lr) * s
-        + lr * reservoir_kernel(reservoir, u, r)
+        np.multiply((1 - lr), s.T).T
+        + np.multiply(lr, reservoir_kernel(reservoir, u, r).T).T
         + noise_gen(dist=dist, shape=r.shape, gain=g_rc)
     )
 
     reservoir.set_param("internal_state", s_next.T)
 
     return f(s_next).T
```

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/intrinsic_plasticity.py` & `reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/intrinsic_plasticity.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     ======================= ========================================================
 
     Parameters
     ----------
     units : int, optional
         Number of reservoir units. If None, the number of units will be infered from
         the ``W`` matrix shape.
-    lr : float, default to 1.0
+    lr : float or array-like of shape (units,), default to 1.0
         Neurons leak rate. Must be in :math:`[0, 1]`.
     sr : float, optional
         Spectral radius of recurrent weight matrix.
     mu : float, default to 0.0
         Mean of the target distribution.
     sigma : float, default to 1.0
         Variance of the target distribution.
```

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/nvar.py` & `reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/nvar.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/reservoirs/reservoir.py` & `reservoirpy-0.3.8/reservoirpy/nodes/reservoirs/reservoir.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     ======================= ========================================================
 
     Parameters
     ----------
     units : int, optional
         Number of reservoir units. If None, the number of units will be infered from
         the ``W`` matrix shape.
-    lr : float, default to 1.0
+    lr : float or array-like of shape (units,), default to 1.0
         Neurons leak rate. Must be in :math:`[0, 1]`.
     sr : float, optional
         Spectral radius of recurrent weight matrix.
     input_bias : bool, default to True
         If False, no bias is added to inputs.
     noise_rc : float, default to 0.0
         Gain of noise applied to reservoir activations.
```

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_concat.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_concat.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_esn.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_esn.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_force.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_force.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_intrinsic_plasticity.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_intrinsic_plasticity.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_io.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_lms.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_lms.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_nvar.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_nvar.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_reservoir.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_reservoir.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,28 @@
         Reservoir(100, equation="foo")
 
     res = Reservoir(100, activation="relu", fb_activation="relu")
     assert id(res.activation) == id(relu)
     assert id(res.fb_activation) == id(relu)
 
 
+def test_reservoir_init_from_lr_is_arrays():
+    lr = np.ones((100,)) * 0.5
+    input_scaling = np.ones((10,)) * 0.8
+    node = Reservoir(100, lr=lr, input_scaling=input_scaling)
+
+    data = np.ones((2, 10))
+    res = node.run(data)
+
+    assert node.W.shape == (100, 100)
+    assert node.Win.shape == (100, 10)
+    assert_array_equal(node.lr, np.ones(100) * 0.5)
+    assert_array_equal(node.input_scaling, np.ones(10) * 0.8)
+
+
 def test_reservoir_init_from_matrices():
     Win = np.ones((100, 10))
 
     node = Reservoir(100, lr=0.8, Win=Win, input_bias=False)
 
     data = np.ones((1, 10))
     res = node(data)
```

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_ridge.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_ridge.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/nodes/tests/test_rls.py` & `reservoirpy-0.3.8/reservoirpy/nodes/tests/test_rls.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/observables.py` & `reservoirpy-0.3.8/reservoirpy/observables.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/ops.py` & `reservoirpy-0.3.8/reservoirpy/ops.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/tests/dummy_nodes.py` & `reservoirpy-0.3.8/reservoirpy/tests/dummy_nodes.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/tests/test_activationsfunc.py` & `reservoirpy-0.3.8/reservoirpy/tests/test_activationsfunc.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/tests/test_base.py` & `reservoirpy-0.3.8/reservoirpy/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/tests/test_mat_gen.py` & `reservoirpy-0.3.8/reservoirpy/tests/test_mat_gen.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/tests/test_model.py` & `reservoirpy-0.3.8/reservoirpy/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/tests/test_node.py` & `reservoirpy-0.3.8/reservoirpy/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/tests/test_observables.py` & `reservoirpy-0.3.8/reservoirpy/tests/test_observables.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/tests/test_ops.py` & `reservoirpy-0.3.8/reservoirpy/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/type.py` & `reservoirpy-0.3.8/reservoirpy/type.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/utils/__init__.py` & `reservoirpy-0.3.8/reservoirpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/utils/graphflow.py` & `reservoirpy-0.3.8/reservoirpy/utils/graphflow.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/utils/model_utils.py` & `reservoirpy-0.3.8/reservoirpy/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/utils/parallel.py` & `reservoirpy-0.3.8/reservoirpy/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/utils/random.py` & `reservoirpy-0.3.8/reservoirpy/utils/random.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/utils/tests/test_random.py` & `reservoirpy-0.3.8/reservoirpy/utils/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/utils/tests/test_utils.py` & `reservoirpy-0.3.8/reservoirpy/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy/utils/validation.py` & `reservoirpy-0.3.8/reservoirpy/utils/validation.py`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/reservoirpy.egg-info/PKG-INFO` & `reservoirpy-0.3.8/reservoirpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reservoirpy
-Version: 0.3.7
+Version: 0.3.8
 Summary: A simple and flexible code for Reservoir Computing architectures like Echo State Networks.
 Home-page: https://github.com/reservoirpy/reservoirpy
-Download-URL: https://github.com/reservoirpy/reservoirpy/v0.3.7.tar.gz
+Download-URL: https://github.com/reservoirpy/reservoirpy/v0.3.8.tar.gz
 Author: Xavier Hinaut
 Author-email: xavier.hinaut@inria.fr
 Maintainer: Xavier Hinaut, Nathan Trouvain
 Maintainer-email: xavier.hinaut@inria.fr, nathan.trouvain@inria.fr
 Project-URL: Bug Tracker, https://github.com/reservoirpy/reservoirpy/issues
 Project-URL: Documentation, https://reservoirpy.readthedocs.io/en/latest/index.html
 Project-URL: Source Code, https://github.com/reservoirpy/reservoirpy
@@ -40,15 +40,15 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reservoirpy)
 [![PyPI version](https://badge.fury.io/py/reservoirpy.svg)](https://badge.fury.io/py/reservoirpy)
 [![Documentation Status](https://readthedocs.org/projects/reservoirpy/badge/?version=latest)](https://reservoirpy.readthedocs.io/en/latest/?badge=latest)
 [![Testing](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/reservoirpy/reservoirpy/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/reservoirpy/reservoirpy/branch/master/graph/badge.svg?token=JC8R1PB5EO)](https://codecov.io/gh/reservoirpy/reservoirpy)
 
-# ReservoirPy (v0.3.7) 🌀🧠
+# ReservoirPy (v0.3.8) 🌀🧠
 **Simple and flexible code for Reservoir Computing architectures like Echo State Networks (ESN).**
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/reservoirpy/reservoirpy/HEAD)
 
 ```python
 from reservoirpy.nodes import Reservoir, Ridge, Input
```

### Comparing `reservoirpy-0.3.7/reservoirpy.egg-info/SOURCES.txt` & `reservoirpy-0.3.8/reservoirpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/setup.cfg` & `reservoirpy-0.3.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `reservoirpy-0.3.7/setup.py` & `reservoirpy-0.3.8/setup.py`

 * *Files identical despite different names*

