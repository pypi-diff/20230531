# Comparing `tmp/RL_OM-0.0.5.tar.gz` & `tmp/RL_OM-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.0.5.tar", last modified: Wed May 31 09:18:48 2023, max compression
+gzip compressed data, was "RL_OM-0.0.6.tar", last modified: Wed May 31 15:42:49 2023, max compression
```

## Comparing `RL_OM-0.0.5.tar` & `RL_OM-0.0.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.023828 RL_OM-0.0.5/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.5/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.5/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 09:18:48.023692 RL_OM-0.0.5/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.5/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.016944 RL_OM-0.0.5/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   130892 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.018266 RL_OM-0.0.5/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.018538 RL_OM-0.0.5/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     5364 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/benchmark_agents/eoq.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.019080 RL_OM-0.0.5/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.019466 RL_OM-0.0.5/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)      929 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.020353 RL_OM-0.0.5/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.021356 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.022407 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     4964 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5134 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16341 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     4869 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.023189 RL_OM-0.0.5/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    10928 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.023471 RL_OM-0.0.5/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6834 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.018119 RL_OM-0.0.5/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-05-31 09:18:48.000000 RL_OM-0.0.5/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.5/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-31 09:17:23.000000 RL_OM-0.0.5/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-31 09:18:48.023882 RL_OM-0.0.5/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.5/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.657440 RL_OM-0.0.6/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.6/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.6/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 15:42:49.657304 RL_OM-0.0.6/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.6/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.650989 RL_OM-0.0.6/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   130892 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.652362 RL_OM-0.0.6/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.652638 RL_OM-0.0.6/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5364 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/benchmark_agents/eoq.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.653254 RL_OM-0.0.6/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.653648 RL_OM-0.0.6/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)      929 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.654543 RL_OM-0.0.6/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.655468 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.656201 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16476 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5004 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.656832 RL_OM-0.0.6/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10928 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.657079 RL_OM-0.0.6/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6834 2023-05-31 15:42:16.000000 RL_OM-0.0.6/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 15:42:49.652208 RL_OM-0.0.6/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.6/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-31 15:42:49.000000 RL_OM-0.0.6/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-31 15:42:01.000000 RL_OM-0.0.6/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-31 15:42:49.657492 RL_OM-0.0.6/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.6/setup.py
```

### Comparing `RL_OM-0.0.5/LICENSE` & `RL_OM-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/PKG-INFO` & `RL_OM-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.0.5
+Version: 0.0.6
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.5/RL_OM/_modidx.py` & `RL_OM-0.0.6/RL_OM/_modidx.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.0.6/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/networks/actors.py` & `RL_OM-0.0.6/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/networks/base.py` & `RL_OM-0.0.6/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/networks/critics.py` & `RL_OM-0.0.6/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.0.6/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/processors/processors.py` & `RL_OM-0.0.6/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         batch_size (int): Number of transitions to sample each time experience is replayed.
         n_features (int): Number of features for the hidden layers of the networks.
         warmup_transitions (int): Number of transitions to replay before starting to update the networks.
         lr_alpha (float): Learning rate for the temperature parameter.
         tau (float): Parameter for the soft update of the target networks.
         target_entropy (float): Target entropy - follows rule of thumb of 0.98 * -log(1/|A|) if None, otherwise it uses the provided value.
         optimizer (torch.optim): Optimizer to use for the networks.
+        squeeze_output (bool): Whether to squeeze the output of the actor network or not.
         use_cuda (bool): Whether to use CUDA or not. If True and not available, it will use CPU.
         agent_name (str): Name of the agent. If set to None will use some default name.
 
     """
 
     def __init__(
             self,
@@ -62,15 +63,15 @@
             batch_size = 64,
             n_features = 64,
             warmup_transitions = 100,
             lr_alpha = 3e-4,
             tau = 0.005,
             target_entropy = None,
             optimizer = optim.Adam,
-            squeeze_output = False,
+            squeeze_output = True,
             use_cuda = True,
             agent_name = None):
         
         use_cuda = use_cuda and torch.cuda.is_available()
 
         input_shape = mdp_info.observation_space.shape
```

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         n_features (int): Number of features for the hidden layers of the networks.
         warmup_transitions (int): Number of transitions to replay before starting to update the networks.
         lr_alpha (float): Learning rate for the temperature parameter.
         tau (float): Parameter for the soft update of the target networks.
         target_entropy (float): Target entropy - follows rule of thumb of 0.98 * -log(1/|A|) if None, otherwise it uses the provided value.
         temperature (float): Temperature of the Gumbel Softmax distribution for backpropagation.
         optimizer (torch.optim): Optimizer to use for the networks.
+        squeeze_output (bool): Whether to squeeze the output of the actor network or not.
         use_cuda (bool): Whether to use CUDA or not. If True and not available, it will use CPU.
         agent_name (str): Name of the agent. If set to None will use some default name.
 
     """
 
     def __init__(
             self,
@@ -64,14 +65,15 @@
             n_features = 64,
             warmup_transitions = 100,
             lr_alpha = 3e-4,
             tau = 0.005,
             target_entropy = None,
             temperature = 1.0,
             optimizer = optim.Adam,
+            squeeze_output = True,
             use_cuda = True,
             agent_name = None):
         
         use_cuda = use_cuda and torch.cuda.is_available()
 
         actor_input_shape = mdp_info.observation_space.shape
         
@@ -100,15 +102,15 @@
         critic_params = dict(network=CriticNetworkStateAction,
                                 optimizer={'class': optim.Adam,
                                         'params': {'lr': 3e-4}}, # default: 3e-4
                                 loss=F.mse_loss,
                                 n_features=n_features,
                                 input_shape=critic_input_shape,
                                 output_shape=(1,),
-                                squeeze_output=True,
+                                squeeze_output=squeeze_output,
                                 use_cuda=use_cuda)
     
         # Agent
         self.agent = SAC_gumbel(mdp_info, actor_params,
                     actor_optimizer, critic_params, batch_size, initial_replay_size,
                     max_replay_size, warmup_transitions, tau, lr_alpha, temperature = temperature,
                     critic_fit_params=None, target_entropy=target_entropy)
```

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         batch_size (int): Number of transitions to sample each time experience is replayed.
         n_features (int): Number of features for the hidden layers of the networks.
         n_features_discrete (int): Number of features for the hidden layers of the discrete network. If set to None will use the same as n_features.
         warmup_transitions (int): Number of transitions to replay before starting to update the networks.
         lr_alpha (float): Learning rate for the temperature parameter.
         tau (float): Parameter for the soft update of the target networks.
         optimizer (torch.optim): Optimizer to use for the networks.
+        squeeze_output (bool): Whether to squeeze the output of the actor network or not.
         use_cuda (bool): Whether to use CUDA or not. If True and not available, it will use CPU.
         agent_name (str): Name of the agent. If set to None will use some default name.
 
     """
 
     def __init__(
             self,
@@ -66,14 +67,15 @@
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
@@ -109,15 +111,15 @@
         critic_params = dict(network=CriticNetworkStateAction,
                         optimizer={'class': optim.Adam,
                                 'params': {'lr': learning_rate_critic}}, 
                         loss=F.mse_loss,
                         n_features=n_features,
                         input_shape=critic_input_shape,
                         output_shape=(1,),
-                        squeeze_output=True,
+                        squeeze_output=squeeze_output,
                         use_cuda=use_cuda)
 
         self.agent = SAC_hybrid(mdp_info, actor_mu_params, actor_sigma_params,
                 actor_discrete_params, actor_optimizer, critic_params, batch_size, initial_replay_size,
                 max_replay_size, warmup_transitions, tau, lr_alpha,
                 critic_fit_params=None)
```

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         max_replay_size (int): Maximum number of transitions to save in the replay buffer.
         batch_size (int): Number of transitions to sample each time experience is replayed.
         n_features (int): Number of features for the hidden layers of the networks.
         warmup_transitions (int): Number of transitions to replay before starting to update the networks.
         lr_alpha (float): Learning rate for the temperature parameter.
         tau (float): Parameter for the soft update of the target networks.
         optimizer (torch.optim): Optimizer to use for the networks.
+        squeeze_output (bool): Whether to squeeze the output of the actor network or not.
         use_cuda (bool): Whether to use CUDA or not. If True and not available, it will use CPU.
         agent_name (str): Name of the agent. If set to None will use some default name.
 
     """
 
     def __init__(
             self,
@@ -60,14 +61,15 @@
             batch_size = 64,
             n_features = 64,
             warmup_transitions = 100,
             lr_alpha = 3e-4,
             tau = 0.005,
             target_entropy = None,
             optimizer = optim.Adam,
+            squeeze_output = True,
             use_cuda = True,
             agent_name = None):
         
         use_cuda = use_cuda and torch.cuda.is_available()
 
         input_shape = mdp_info.observation_space.shape
         actor_output_shape = (mdp_info.action_space.shape[0]*2,) # Currently hardcoded for binary discrete actions
@@ -95,15 +97,15 @@
         critic_params = dict(network=CriticNetworkStateAction,
                         optimizer={'class': optim.Adam,
                                 'params': {'lr': learning_rate_critic}}, 
                         loss=F.mse_loss,
                         n_features=n_features,
                         input_shape=critic_input_shape,
                         output_shape=(1,),
-                        squeeze_output=True,
+                        squeeze_output=squeeze_output,
                         use_cuda=use_cuda)
         
         self.agent = SAC(mdp_info, actor_mu_params, actor_sigma_params,
                     actor_optimizer, critic_params, batch_size, initial_replay_size,
                     max_replay_size, warmup_transitions, tau, lr_alpha,
                     critic_fit_params=None)
```

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.0.6/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/environments/calculation_functions.py` & `RL_OM-0.0.6/RL_OM/environments/calculation_functions.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/environments/data_generators.py` & `RL_OM-0.0.6/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/environments/feature_converters.py` & `RL_OM-0.0.6/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.0.6/RL_OM/environments/multi_period_inventory.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.0.6/RL_OM/experiment_functions/run_experiment.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.0.6/RL_OM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.0.5
+Version: 0.0.6
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.5/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.0.6/RL_OM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.5/settings.ini` & `RL_OM-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.0.5/setup.py` & `RL_OM-0.0.6/setup.py`

 * *Files identical despite different names*

