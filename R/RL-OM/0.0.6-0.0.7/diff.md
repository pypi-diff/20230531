# Comparing `tmp/RL_OM-0.0.6.tar.gz` & `tmp/RL_OM-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.0.6.tar", last modified: Wed May 31 15:42:49 2023, max compression
+gzip compressed data, was "RL_OM-0.0.7.tar", last modified: Wed May 31 16:04:35 2023, max compression
```

## Comparing `RL_OM-0.0.6.tar` & `RL_OM-0.0.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.657440 RL_OM-0.0.6/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.6/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.6/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 15:42:49.657304 RL_OM-0.0.6/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.6/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.650989 RL_OM-0.0.6/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   130892 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.652362 RL_OM-0.0.6/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.652638 RL_OM-0.0.6/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     5364 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/benchmark_agents/eoq.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.653254 RL_OM-0.0.6/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.653648 RL_OM-0.0.6/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)      929 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.654543 RL_OM-0.0.6/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.655468 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.656201 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     5053 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5269 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16476 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     5004 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.656832 RL_OM-0.0.6/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    10928 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.657079 RL_OM-0.0.6/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6834 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.652208 RL_OM-0.0.6/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.6/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-31 15:42:01.000000 RL_OM-0.0.6/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-31 15:42:49.657492 RL_OM-0.0.6/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.6/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.926334 RL_OM-0.0.7/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.7/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.7/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 16:04:35.926190 RL_OM-0.0.7/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.7/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.919334 RL_OM-0.0.7/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   130892 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.920549 RL_OM-0.0.7/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.920781 RL_OM-0.0.7/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5364 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/benchmark_agents/eoq.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.921702 RL_OM-0.0.7/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.922236 RL_OM-0.0.7/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)      929 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.923224 RL_OM-0.0.7/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.924174 RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.925023 RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16656 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5004 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.925711 RL_OM-0.0.7/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10928 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.925995 RL_OM-0.0.7/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6834 2023-05-31 16:04:14.000000 RL_OM-0.0.7/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 16:04:35.920413 RL_OM-0.0.7/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 16:04:35.000000 RL_OM-0.0.7/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-05-31 16:04:35.000000 RL_OM-0.0.7/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-31 16:04:35.000000 RL_OM-0.0.7/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-31 16:04:35.000000 RL_OM-0.0.7/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.7/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-31 16:04:35.000000 RL_OM-0.0.7/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-31 16:04:35.000000 RL_OM-0.0.7/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-31 16:03:29.000000 RL_OM-0.0.7/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-31 16:04:35.926386 RL_OM-0.0.7/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.7/setup.py
```

### Comparing `RL_OM-0.0.6/LICENSE` & `RL_OM-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/PKG-INFO` & `RL_OM-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.0.6
+Version: 0.0.7
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.6/RL_OM/_modidx.py` & `RL_OM-0.0.7/RL_OM/_modidx.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.0.7/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/networks/actors.py` & `RL_OM-0.0.7/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/networks/base.py` & `RL_OM-0.0.7/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/networks/critics.py` & `RL_OM-0.0.7/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.0.7/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/processors/processors.py` & `RL_OM-0.0.7/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,15 @@
             n_features = 64,
             n_features_discrete = None,
             warmup_transitions = 100,
             lr_alpha = 3e-4,
             tau = 0.005,
             target_entropy = None,
             optimizer = optim.Adam,
+            squeeze_output = True,
             use_cuda = True,
             agent_name = None):
         
         use_cuda = use_cuda and torch.cuda.is_available()
 
         actor_input_shape = mdp_info.observation_space.shape
         actor_output_shape = (mdp_info.action_space.shape[0],)
@@ -219,14 +220,15 @@
         critic_params = dict(network=CriticNetworkStateAction,
                         optimizer={'class': optim.Adam,
                                 'params': {'lr': learning_rate_critic}}, 
                         loss=F.mse_loss,
                         n_features=n_features,
                         input_shape=critic_input_shape,
                         output_shape=(1,),
+                        squeeze_output=squeeze_output,
                         use_cuda=use_cuda)
 
         # Change here: Use reversed SAC algorithm
         self.agent = SAC_hybrid_reversed(mdp_info, actor_mu_params, actor_sigma_params,
                 actor_discrete_params, actor_optimizer, critic_params, batch_size, initial_replay_size,
                 max_replay_size, warmup_transitions, tau, lr_alpha,
                 critic_fit_params=None)
@@ -281,14 +283,15 @@
             n_features = 64,
             n_features_discrete = None,
             warmup_transitions = 100,
             lr_alpha = 3e-4,
             tau = 0.005,
             target_entropy = None,
             optimizer = optim.Adam,
+            squeeze_output = True,
             use_cuda = True,
             agent_name = None):
         
         use_cuda = use_cuda and torch.cuda.is_available()
 
         actor_input_shape = mdp_info.observation_space.shape
         actor_output_shape = (mdp_info.action_space.shape[0],)
@@ -323,14 +326,15 @@
         critic_params = dict(network=CriticNetworkStateAction,
                         optimizer={'class': optim.Adam,
                                 'params': {'lr': learning_rate_critic}}, 
                         loss=F.mse_loss,
                         n_features=n_features,
                         input_shape=critic_input_shape,
                         output_shape=(1,),
+                        squeeze_output=squeeze_output,
                         use_cuda=use_cuda)
 
         # Change here: Use separate SAC algorithm
         self.agent = SAC_hybrid_separate(mdp_info, actor_mu_params, actor_sigma_params,
                 actor_discrete_params, actor_optimizer, critic_params, batch_size, initial_replay_size,
                 max_replay_size, warmup_transitions, tau, lr_alpha,
                 critic_fit_params=None)
```

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.0.7/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/environments/calculation_functions.py` & `RL_OM-0.0.7/RL_OM/environments/calculation_functions.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/environments/data_generators.py` & `RL_OM-0.0.7/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/environments/feature_converters.py` & `RL_OM-0.0.7/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.0.7/RL_OM/environments/multi_period_inventory.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.0.7/RL_OM/experiment_functions/run_experiment.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.0.7/RL_OM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.0.6
+Version: 0.0.7
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.6/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.0.7/RL_OM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.6/settings.ini` & `RL_OM-0.0.7/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.0.6/setup.py` & `RL_OM-0.0.7/setup.py`

 * *Files identical despite different names*

