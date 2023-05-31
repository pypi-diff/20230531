# Comparing `tmp/RL_OM-0.0.4.tar.gz` & `tmp/RL_OM-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.0.4.tar", last modified: Thu May 25 09:41:48 2023, max compression
+gzip compressed data, was "RL_OM-0.0.5.tar", last modified: Wed May 31 09:18:48 2023, max compression
```

## Comparing `RL_OM-0.0.4.tar` & `RL_OM-0.0.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.569265 RL_OM-0.0.4/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.4/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.4/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-25 09:41:48.569116 RL_OM-0.0.4/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.4/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.562805 RL_OM-0.0.4/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   129546 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.564144 RL_OM-0.0.4/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.564442 RL_OM-0.0.4/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     5191 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/benchmark_agents/eoq.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.565072 RL_OM-0.0.4/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.565470 RL_OM-0.0.4/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)      929 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     4476 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.566328 RL_OM-0.0.4/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.567216 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.567965 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     4865 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5081 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16296 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     4824 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-23 14:52:52.000000 RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.568641 RL_OM-0.0.4/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    10669 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.568900 RL_OM-0.0.4/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     4863 2023-05-25 09:39:51.000000 RL_OM-0.0.4/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-25 09:41:48.563981 RL_OM-0.0.4/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.4/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-25 09:41:48.000000 RL_OM-0.0.4/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-25 09:39:45.000000 RL_OM-0.0.4/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-25 09:41:48.569308 RL_OM-0.0.4/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.4/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.023828 RL_OM-0.0.5/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.5/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.5/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 09:18:48.023692 RL_OM-0.0.5/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.5/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.016944 RL_OM-0.0.5/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   130892 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.018266 RL_OM-0.0.5/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.018538 RL_OM-0.0.5/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5364 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/benchmark_agents/eoq.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.019080 RL_OM-0.0.5/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.019466 RL_OM-0.0.5/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)      929 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.020353 RL_OM-0.0.5/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.021356 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.022407 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     4964 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5134 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16341 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4869 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.023189 RL_OM-0.0.5/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10928 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.023471 RL_OM-0.0.5/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6834 2023-05-31 09:17:29.000000 RL_OM-0.0.5/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-31 09:18:48.018119 RL_OM-0.0.5/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-05-31 09:18:48.000000 RL_OM-0.0.5/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.5/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-31 09:18:47.000000 RL_OM-0.0.5/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-31 09:17:23.000000 RL_OM-0.0.5/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-31 09:18:48.023882 RL_OM-0.0.5/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.5/setup.py
```

### Comparing `RL_OM-0.0.4/LICENSE` & `RL_OM-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/PKG-INFO` & `RL_OM-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.0.4
+Version: 0.0.5
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.4/RL_OM/_modidx.py` & `RL_OM-0.0.5/RL_OM/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,20 @@
                                                                                                                                 'RL_OM/agents/processors/eoq_preprocessors.py'),
                                                            'RL_OM.agents.processors.eoq_preprocessors.GetInventory.__init__': ( 'agents/processors/eoq_preprocessors.html#getinventory.__init__',
                                                                                                                                 'RL_OM/agents/processors/eoq_preprocessors.py')},
             'RL_OM.agents.processors.processors': { 'RL_OM.agents.processors.processors.ClipNegative': ( 'agents/processors/processors.html#clipnegative',
                                                                                                          'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.ClipNegative.__call__': ( 'agents/processors/processors.html#clipnegative.__call__',
                                                                                                                   'RL_OM/agents/processors/processors.py'),
+                                                    'RL_OM.agents.processors.processors.ContToBinary': ( 'agents/processors/processors.html#conttobinary',
+                                                                                                         'RL_OM/agents/processors/processors.py'),
+                                                    'RL_OM.agents.processors.processors.ContToBinary.__call__': ( 'agents/processors/processors.html#conttobinary.__call__',
+                                                                                                                  'RL_OM/agents/processors/processors.py'),
+                                                    'RL_OM.agents.processors.processors.ContToBinary.__init__': ( 'agents/processors/processors.html#conttobinary.__init__',
+                                                                                                                  'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.DiscreteToContinuous': ( 'agents/processors/processors.html#discretetocontinuous',
                                                                                                                  'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.DiscreteToContinuous.__call__': ( 'agents/processors/processors.html#discretetocontinuous.__call__',
                                                                                                                           'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.DiscreteToContinuous.__init__': ( 'agents/processors/processors.html#discretetocontinuous.__init__',
                                                                                                                           'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.HybridToContinuous': ( 'agents/processors/processors.html#hybridtocontinuous',
@@ -665,8 +671,10 @@
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.set_observation_space': ( 'environments/multi_period_inventory.html#multiperiodenv.set_observation_space',
                                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.set_observation_state': ( 'environments/multi_period_inventory.html#multiperiodenv.set_observation_state',
                                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.step': ( 'environments/multi_period_inventory.html#multiperiodenv.step',
                                                                                                                               'RL_OM/environments/multi_period_inventory.py')},
             'RL_OM.experiment_functions.run_experiment': { 'RL_OM.experiment_functions.run_experiment.experiment_stepwise': ( 'experiment_functions/run_experiment.html#experiment_stepwise',
-                                                                                                                              'RL_OM/experiment_functions/run_experiment.py')}}}
+                                                                                                                              'RL_OM/experiment_functions/run_experiment.py'),
+                                                           'RL_OM.experiment_functions.run_experiment.experiment_stepwise_no_log': ( 'experiment_functions/run_experiment.html#experiment_stepwise_no_log',
+                                                                                                                                     'RL_OM/experiment_functions/run_experiment.py')}}}
```

### Comparing `RL_OM-0.0.4/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.0.5/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,39 +21,43 @@
     Args:
         mdp_info (MDPInfo): Information about the Markov Decision Process (MDP).
         s (numpy.ndarray): The fixed ordering cost.
         h (numpy.ndarray): The holding cost per unit per period.
         preprocessors (list): List of preprocessors to be applied to the state.
         postprocessors (list): List of postprocessors to be applied to the policy.
         agent_name (str): Name of the agent. If set to None will use some default name.
+        precision (int): Number of decimal places to round the demand input to.
 
     Attributes:
         mdp_info (MDPInfo): Information about the Markov Decision Process (MDP).
         policy (EOQPolicy): The EOQ policy implemented by the agent.
 
     """
 
 
     def __init__(self,
                   mdp_info,
                   s, # fixed ordering cost
                   h, # holding cost per unit per period
                   preprocessors = None,
                   postprocessors = None,
-                  agent_name = None
+                  agent_name = None,
+                  precision = 5
         ):
 
         policy = EOQPolicy(
             d = None,
             s = s,
             h = h,
             preprocessors = preprocessors,
             postprocessors = postprocessors
         )
 
+        self.precision=precision
+
         if agent_name is None:
             self.name = 'EOQAgent'
         else:
             self.name = agent_name
 
         super().__init__(mdp_info, policy)
 
@@ -72,15 +76,15 @@
 
         """
 
 
         assert isinstance(demand, np.ndarray)
         assert demand.ndim == 2
 
-        self.policy.d = np.mean(demand, axis=0)
+        self.policy.d = np.round(np.mean(demand, axis=0), self.precision)
 
         self.policy.set_q_star()
 
 class EOQPolicy():
 
     """
     Policy implementing the Economic Order Quantity (EOQ) strategy.
```

### Comparing `RL_OM-0.0.4/RL_OM/agents/networks/actors.py` & `RL_OM-0.0.5/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/networks/base.py` & `RL_OM-0.0.5/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/networks/critics.py` & `RL_OM-0.0.5/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.0.5/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/processors/processors.py` & `RL_OM-0.0.5/RL_OM/agents/processors/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/agents/processors/01_processors.ipynb.
 
 # %% auto 0
 __all__ = ['RoundAction', 'ClipNegative', 'DiscreteToContinuous', 'OneHotToDiscrete', 'HybridToContinuous',
-           'OneHotHybridtoContinuous']
+           'OneHotHybridtoContinuous', 'ContToBinary']
 
 # %% ../../../nbs/agents/processors/01_processors.ipynb 4
 # General libraries:
 import numpy as np
 
 # %% ../../../nbs/agents/processors/01_processors.ipynb 6
 class RoundAction():
@@ -133,7 +133,25 @@
         order_quantity = action[:self.num_products]
         order_action = action[self.num_products:]
         for i in range(self.num_products):
             order_action_prod = order_action[i:i+2]
             order_action = np.argmax(order_action_prod)
         action = order_action * order_quantity
         return action
+
+# %% ../../../nbs/agents/processors/01_processors.ipynb 12
+class ContToBinary():
+
+    """
+    This class implements a processor that converts a continuous input 
+    into a binary input. The binary feature will be one if the continuous
+    input is greater than 0, and zero otherwise.
+
+    #! Currently only works for single product
+
+    """
+
+    def __init__(self):
+        pass
+
+    def __call__(self, state):
+        return np.array([1]) if state[0] > 0 else np.array([0])
```

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             batch_size = 64,
             n_features = 64,
             warmup_transitions = 100,
             lr_alpha = 3e-4,
             tau = 0.005,
             target_entropy = None,
             optimizer = optim.Adam,
+            squeeze_output = False,
             use_cuda = True,
             agent_name = None):
         
         use_cuda = use_cuda and torch.cuda.is_available()
 
         input_shape = mdp_info.observation_space.shape
         
@@ -96,14 +97,15 @@
         critic_params = dict(network=CriticNetworkState,
                                 optimizer={'class': optim.Adam,
                                         'params': {'lr': 3e-4}}, # default: 3e-4
                                 loss=F.mse_loss,
                                 n_features=n_features,
                                 input_shape=input_shape,
                                 output_shape=actor_output_shape,
+                                squeeze_output=squeeze_output,
                                 use_cuda=use_cuda)
     
         # Agent
         self.agent = SAC_discrete(mdp_info, actor_params,
                     actor_optimizer, critic_params, batch_size, initial_replay_size,
                     max_replay_size, warmup_transitions, tau, lr_alpha,
                     critic_fit_params=None, target_entropy=target_entropy)
```

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         critic_params = dict(network=CriticNetworkStateAction,
                                 optimizer={'class': optim.Adam,
                                         'params': {'lr': 3e-4}}, # default: 3e-4
                                 loss=F.mse_loss,
                                 n_features=n_features,
                                 input_shape=critic_input_shape,
                                 output_shape=(1,),
+                                squeeze_output=True,
                                 use_cuda=use_cuda)
     
         # Agent
         self.agent = SAC_gumbel(mdp_info, actor_params,
                     actor_optimizer, critic_params, batch_size, initial_replay_size,
                     max_replay_size, warmup_transitions, tau, lr_alpha, temperature = temperature,
                     critic_fit_params=None, target_entropy=target_entropy)
```

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         critic_params = dict(network=CriticNetworkStateAction,
                         optimizer={'class': optim.Adam,
                                 'params': {'lr': learning_rate_critic}}, 
                         loss=F.mse_loss,
                         n_features=n_features,
                         input_shape=critic_input_shape,
                         output_shape=(1,),
+                        squeeze_output=True,
                         use_cuda=use_cuda)
 
         self.agent = SAC_hybrid(mdp_info, actor_mu_params, actor_sigma_params,
                 actor_discrete_params, actor_optimizer, critic_params, batch_size, initial_replay_size,
                 max_replay_size, warmup_transitions, tau, lr_alpha,
                 critic_fit_params=None)
```

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         critic_params = dict(network=CriticNetworkStateAction,
                         optimizer={'class': optim.Adam,
                                 'params': {'lr': learning_rate_critic}}, 
                         loss=F.mse_loss,
                         n_features=n_features,
                         input_shape=critic_input_shape,
                         output_shape=(1,),
+                        squeeze_output=True,
                         use_cuda=use_cuda)
         
         self.agent = SAC(mdp_info, actor_mu_params, actor_sigma_params,
                     actor_optimizer, critic_params, batch_size, initial_replay_size,
                     max_replay_size, warmup_transitions, tau, lr_alpha,
                     critic_fit_params=None)
```

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.0.5/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/environments/calculation_functions.py` & `RL_OM-0.0.5/RL_OM/environments/calculation_functions.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/environments/data_generators.py` & `RL_OM-0.0.5/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/environments/feature_converters.py` & `RL_OM-0.0.5/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.0.5/RL_OM/environments/multi_period_inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,18 @@
 
                 ### other parameters
                 horizon = 365, # lenght of each episode in simulation
                 gamma = 1, # discount factor
                 observation_space_kwargs = None,
 
                 ### logic of step-method
-                calculations = None
+                calculations = None,
+
+                ### Precision of state
+                precision = 5
                 ):
         """
         Multi-period inventory environment covering all major single-echelon inventory models with decision on quantity.
 
         Note: Except True/False parameters and horizon/gamma, all parameters are arrays to set the parameter for each product individually.
 
         args:
@@ -79,14 +82,15 @@
             lead_time_variance: variance in lead time
             order_limit_low: maximum order allowed
             order_limit_high: minimum order allowed
             horizon: lenght of each episode in simulation
             gamma: discount factor
             observation_space_kwargs: kwargs for observation space
             calculations: function that calculates the next state and reward in the step function
+            precision: precision of state variables (decimal places)
         """
         
         self.demand = demand
         self.num_observations = demand.shape[0] # number of observations
         self.num_products = demand.shape[1] # number of products
         self.features = features
         if self.features is not None:
@@ -148,14 +152,16 @@
         mdp_info = MDPInfo(observation_space=self.observation_space,
                            action_space=self.action_space,
                            horizon=horizon,
                            gamma=gamma)
         
         super().__init__(mdp_info)
 
+        self.precision = precision
+
         # Set state variables
         self.reset()
 
 
     def set_observation_space(self,
                               features = False,
                               inventory = False,
@@ -234,14 +240,16 @@
             for product in range(self.num_products):
                 self.observation_state[self.num_features+self.num_products+slots_occupied:self.num_features+self.num_products+slots_occupied+self.max_lead_time[product]] = self.order_pipeline[product]
                 slots_occupied += self.max_lead_time[product]
 
         if self.max_demand_backlog > 0:
             self.observation_state[self.num_features+self.num_products+np.sum(self.num_products * self.lead_time):] = self.demand_backlog
 
+        self.observation_state = np.round(self.observation_state, self.precision)
+
 
     def step(self, action):
 
         absorbing = False
 
         reward, info = self.calculations(self, action)
```

### Comparing `RL_OM-0.0.4/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.0.5/RL_OM/experiment_functions/run_experiment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/experiment_functions/01_run_experiment.ipynb.
 
 # %% auto 0
-__all__ = ['experiment_stepwise']
+__all__ = ['experiment_stepwise', 'experiment_stepwise_no_log']
 
 # %% ../../nbs/experiment_functions/01_run_experiment.ipynb 4
 # MushroomRL:
 from mushroom_rl.core import Core, Logger
 from mushroom_rl.utils.dataset import compute_J,  parse_dataset
 
 # Pytorch
@@ -135,7 +135,60 @@
         E = None
 
     logger.epoch_info(epoch = "final", J=J, R=R, E=E)
     logger.log_numpy(J=J, R=R, E=E)
     logger.log_dataset(dataset, name_addition = "_final")
         
     return logger
+
+# %% ../../nbs/experiment_functions/01_run_experiment.ipynb 7
+def experiment_stepwise_no_log(mdp,
+                        agent,
+                        n_epochs,
+                        n_steps,
+                        n_episodes_test,
+                        rand_seed = None,
+                        dataset_log_freq = None):
+
+    """
+    TODO 1: Add function to (deep)save the entire agent to be able to reloead it later and potentially continue training.
+    TODO 2: Provide functionalita to turn of exploration during evaluation (e.g., epsilon=0 for DQN, sample_mean for SAC)
+
+    Function to run an experiment with a given agent and mdp.
+    Designed specifically for algorithms that learn on each step (e.g., SAC) to tune hyperparameters.
+    Does not use logger but simply returns the results.
+
+    The function assumes that that the mpd has a a demand attribute containing
+    a list of historical demands. This is used as input for the directly trained agents.
+
+    Args:
+        mdp (object): MDP to be solved.
+        agent (object): Agent to solve the MDP.
+        n_epochs (int): Number of epochs to train the agent.
+        n_steps (int): Number of steps per epoch.
+        n_episodes_test (int): Number of episodes to evaluate the agent.
+    """
+
+    if rand_seed is not None:
+        np.random.seed(rand_seed)
+        torch.manual_seed(rand_seed)
+
+    # ensure mdp starts from the same state
+    mdp.reset()
+
+    core = Core(agent, mdp)
+
+    ### Training
+    initial_replay_size = agent._replay_memory._initial_size
+    core.learn(n_steps=initial_replay_size, n_steps_per_fit=initial_replay_size, quiet=True)
+
+    R_hist = []
+
+    for n in trange(n_epochs, leave=False):
+        core.learn(n_steps=n_steps, n_steps_per_fit=1, quiet = True)
+        dataset = core.evaluate(n_episodes=n_episodes_test, render=False, quiet = True)
+
+        R = np.mean(compute_J(dataset))
+
+        R_hist.append(R)
+        
+    return R_hist
```

### Comparing `RL_OM-0.0.4/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.0.5/RL_OM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.0.4
+Version: 0.0.5
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.4/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.0.5/RL_OM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.4/settings.ini` & `RL_OM-0.0.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.0.4/setup.py` & `RL_OM-0.0.5/setup.py`

 * *Files identical despite different names*

