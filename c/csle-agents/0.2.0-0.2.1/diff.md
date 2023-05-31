# Comparing `tmp/csle_agents-0.2.0.tar.gz` & `tmp/csle_agents-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_agents-0.2.0.tar", last modified: Sun Apr 30 12:37:40 2023, max compression
+gzip compressed data, was "csle_agents-0.2.1.tar", last modified: Wed May 31 11:26:26 2023, max compression
```

## Comparing `csle_agents-0.2.0.tar` & `csle_agents-0.2.1.tar`

### file list

```diff
@@ -1,97 +1,101 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.956838 csle_agents-0.2.0/
--rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-04-30 12:37:40.956838 csle_agents-0.2.0/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4154 2023-03-28 14:03:22.000000 csle_agents-0.2.0/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-28 14:03:22.000000 csle_agents-0.2.0/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1410 2023-04-30 12:37:40.956838 csle_agents-0.2.0/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_agents-0.2.0/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_agents-0.2.0/src/csle_agents/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents/agents/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents/agents/base/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/base/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1854 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/base/base_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents/agents/bayesian_optimization/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/bayesian_optimization/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    28162 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/cross_entropy/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/cross_entropy/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    26946 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/differential_evolution/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/differential_evolution/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    31459 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/dqn/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/dqn/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    19153 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/dqn/dqn_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/dynasec/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/dynasec/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    75392 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/dynasec/dynasec_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/fp/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/fp/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18259 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/fp/fictitious_play_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/hsvi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/hsvi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    49313 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/hsvi/hsvi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/hsvi_os_posg/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/hsvi_os_posg/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    75255 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/kiefer_wolfowitz/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    28849 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/lp_nf/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/lp_nf/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18360 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/pi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/pi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17642 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/pi/pi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/ppo/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/ppo/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    25515 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/ppo/ppo_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/q_learning/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/q_learning/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17360 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/q_learning/q_learning_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/random_search/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/random_search/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    26175 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/random_search/random_search_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/reinforce/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/reinforce/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    25109 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/reinforce/reinforce_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/sarsa/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/sarsa/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17456 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/sarsa/sarsa_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/shapley_iteration/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/shapley_iteration/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15788 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/sondik_vi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/sondik_vi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    22182 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/t_fp/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/t_fp/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    41896 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/t_fp/t_fp_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/t_spsa/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/t_spsa/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    32105 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/t_spsa/t_spsa_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/vi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/vi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    16358 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/vi/vi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/common/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5759 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/actor_critic_net.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4595 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/fnn_w_gaussian.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/fnn_w_linear.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3460 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/pruning.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.956838 csle_agents-0.2.0/src/csle_agents/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11221 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.956838 csle_agents-0.2.0/src/csle_agents/job_controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/job_controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2459 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/job_controllers/training_job_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     2876 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:05.000000 csle_agents-0.2.0/src/csle_agents.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      371 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.390761 csle_agents-0.2.1/
+-rw-r--r--   0 kimham     (501) staff       (20)      653 2023-05-31 11:26:26.390886 csle_agents-0.2.1/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     4154 2023-01-11 18:45:47.000000 csle_agents-0.2.1/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      671 2023-02-12 08:59:32.000000 csle_agents-0.2.1/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1410 2023-05-31 11:26:26.391455 csle_agents-0.2.1/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_agents-0.2.1/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.355027 csle_agents-0.2.1/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.361579 csle_agents-0.2.1/src/csle_agents/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:22:38.000000 csle_agents-0.2.1/src/csle_agents/__version__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.364009 csle_agents-0.2.1/src/csle_agents/agents/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/__init__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.364465 csle_agents-0.2.1/src/csle_agents/agents/base/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/base/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1854 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/base/base_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.365339 csle_agents-0.2.1/src/csle_agents/agents/bayesian_optimization/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-04-25 08:30:10.000000 csle_agents-0.2.1/src/csle_agents/agents/bayesian_optimization/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    28162 2023-04-25 11:33:39.000000 csle_agents-0.2.1/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.366478 csle_agents-0.2.1/src/csle_agents/agents/cross_entropy/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/cross_entropy/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    26958 2023-05-24 17:32:13.000000 csle_agents-0.2.1/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.368517 csle_agents-0.2.1/src/csle_agents/agents/dfsp_local/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/dfsp_local/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    37993 2023-05-24 17:19:50.000000 csle_agents-0.2.1/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
+-rw-r--r--   0 kimham     (501) staff       (20)    39891 2023-05-24 17:19:50.000000 csle_agents-0.2.1/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.369691 csle_agents-0.2.1/src/csle_agents/agents/differential_evolution/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/differential_evolution/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    31471 2023-05-24 17:30:57.000000 csle_agents-0.2.1/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.370750 csle_agents-0.2.1/src/csle_agents/agents/dqn/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/dqn/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    19153 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/dqn/dqn_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.372458 csle_agents-0.2.1/src/csle_agents/agents/dynasec/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/dynasec/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    75392 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/dynasec/dynasec_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.373526 csle_agents-0.2.1/src/csle_agents/agents/fp/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/fp/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    18259 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/fp/fictitious_play_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.374369 csle_agents-0.2.1/src/csle_agents/agents/hsvi/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/hsvi/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    49313 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/hsvi/hsvi_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.375214 csle_agents-0.2.1/src/csle_agents/agents/hsvi_os_posg/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/hsvi_os_posg/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    75255 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.376074 csle_agents-0.2.1/src/csle_agents/agents/kiefer_wolfowitz/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    28849 2023-04-25 09:34:50.000000 csle_agents-0.2.1/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.377111 csle_agents-0.2.1/src/csle_agents/agents/lp_nf/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/lp_nf/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    18360 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.378098 csle_agents-0.2.1/src/csle_agents/agents/pi/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/pi/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    17642 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/pi/pi_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.378713 csle_agents-0.2.1/src/csle_agents/agents/ppo/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/ppo/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    25589 2023-05-02 09:52:34.000000 csle_agents-0.2.1/src/csle_agents/agents/ppo/ppo_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.379797 csle_agents-0.2.1/src/csle_agents/agents/q_learning/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/q_learning/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    17360 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/q_learning/q_learning_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.380483 csle_agents-0.2.1/src/csle_agents/agents/random_search/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/random_search/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    26175 2023-04-25 09:38:36.000000 csle_agents-0.2.1/src/csle_agents/agents/random_search/random_search_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.381489 csle_agents-0.2.1/src/csle_agents/agents/reinforce/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/reinforce/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    25109 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/reinforce/reinforce_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.382626 csle_agents-0.2.1/src/csle_agents/agents/sarsa/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/sarsa/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    17456 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/sarsa/sarsa_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.383252 csle_agents-0.2.1/src/csle_agents/agents/shapley_iteration/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/shapley_iteration/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    15788 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.383821 csle_agents-0.2.1/src/csle_agents/agents/sondik_vi/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/sondik_vi/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    22182 2023-03-31 11:14:06.000000 csle_agents-0.2.1/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.384499 csle_agents-0.2.1/src/csle_agents/agents/t_fp/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/t_fp/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    41988 2023-05-01 11:12:26.000000 csle_agents-0.2.1/src/csle_agents/agents/t_fp/t_fp_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.385623 csle_agents-0.2.1/src/csle_agents/agents/t_spsa/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/t_spsa/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    32117 2023-05-24 17:29:31.000000 csle_agents-0.2.1/src/csle_agents/agents/t_spsa/t_spsa_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.386695 csle_agents-0.2.1/src/csle_agents/agents/vi/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/agents/vi/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    16358 2023-04-29 14:22:16.000000 csle_agents-0.2.1/src/csle_agents/agents/vi/vi_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.389015 csle_agents-0.2.1/src/csle_agents/common/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/common/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5759 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/common/actor_critic_net.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4595 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/common/fnn_w_gaussian.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3936 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/common/fnn_w_linear.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3460 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/common/pruning.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.389593 csle_agents-0.2.1/src/csle_agents/constants/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/constants/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11876 2023-05-01 11:24:17.000000 csle_agents-0.2.1/src/csle_agents/constants/constants.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.390337 csle_agents-0.2.1/src/csle_agents/job_controllers/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/job_controllers/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2459 2022-11-28 13:00:49.000000 csle_agents-0.2.1/src/csle_agents/job_controllers/training_job_manager.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:26:26.363721 csle_agents-0.2.1/src/csle_agents.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      653 2023-05-31 11:26:25.000000 csle_agents-0.2.1/src/csle_agents.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     3034 2023-05-31 11:26:26.000000 csle_agents-0.2.1/src/csle_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:26:25.000000 csle_agents-0.2.1/src/csle_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:28.000000 csle_agents-0.2.1/src/csle_agents.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      371 2023-05-31 11:26:26.000000 csle_agents-0.2.1/src/csle_agents.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       12 2023-05-31 11:26:26.000000 csle_agents-0.2.1/src/csle_agents.egg-info/top_level.txt
```

### Comparing `csle_agents-0.2.0/PKG-INFO` & `csle_agents-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_agents
-Version: 0.2.0
+Version: 0.2.1
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.2.0/README.md` & `csle_agents-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/pyproject.toml` & `csle_agents-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/setup.cfg` & `csle_agents-0.2.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.2.0
-	csle-collector>=0.2.0
-	csle-attacker>=0.2.0
-	csle-defender>=0.2.0
-	csle-system-identification>=0.2.0
-	gym-csle-stopping-game>=0.2.0
+	csle-common>=0.2.1
+	csle-collector>=0.2.1
+	csle-attacker>=0.2.1
+	csle-defender>=0.2.1
+	csle-system-identification>=0.2.1
+	gym-csle-stopping-game>=0.2.1
 	stable-baselines3>=1.8.0
 	pulp>=2.7.0
 	bayesian-optimization>=1.3.1
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/base/base_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/base/base_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,16 +471,16 @@
         """
         Utility method for getting the policy of a given parameter vector
 
         :param theta: the parameter vector
         :param L: the number of parameters
         :return: the policy
         """
-        if self.experiment_config.hparams[agents_constants.CROSS_ENTROPY.POLICY_TYPE] \
-                == PolicyType.MULTI_THRESHOLD:
+        if self.experiment_config.hparams[agents_constants.CROSS_ENTROPY.POLICY_TYPE].value \
+                == PolicyType.MULTI_THRESHOLD.value:
             policy = MultiThresholdStoppingPolicy(
                 theta=theta, simulation_name=self.simulation_env_config.name,
                 states=self.simulation_env_config.state_space_config.states,
                 player_type=self.experiment_config.player_type, L=L,
                 actions=self.simulation_env_config.joint_action_space_config.action_spaces[
                     self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
                 agent_type=AgentType.CROSS_ENTROPY)
```

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,16 +560,16 @@
         """
         Utility method for getting the policy from a parameter vector
 
         :param theta: the parameter vector
         :param L: the number of parameters
         :return: the policy
         """
-        if self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.POLICY_TYPE] \
-                == PolicyType.MULTI_THRESHOLD:
+        if self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.POLICY_TYPE].value \
+                == PolicyType.MULTI_THRESHOLD.value:
             policy = MultiThresholdStoppingPolicy(
                 theta=list(theta), simulation_name=self.simulation_env_config.name,
                 states=self.simulation_env_config.state_space_config.states,
                 player_type=self.experiment_config.player_type, L=L,
                 actions=self.simulation_env_config.joint_action_space_config.action_spaces[
                     self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
                 agent_type=AgentType.DIFFERENTIAL_EVOLUTION)
```

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/dqn/dqn_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/dqn/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/dynasec/dynasec_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/dynasec/dynasec_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/fp/fictitious_play_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/fp/fictitious_play_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/hsvi/hsvi_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/hsvi/hsvi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/pi/pi_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/pi/pi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/ppo/ppo_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/ppo/ppo_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,14 @@
         if self.save_to_metastore:
             exp_execution_id = MetastoreFacade.save_experiment_execution(self.exp_execution)
         self.exp_execution.id = exp_execution_id
 
         # Setup gym environment
         config = self.simulation_env_config.simulation_env_input_config
         orig_env = gymnasium.make(self.simulation_env_config.gym_env_name, config=config)
-        print(orig_env.observation_space)
         env = make_vec_env(env_id=self.simulation_env_config.gym_env_name,
                            n_envs=self.experiment_config.hparams[agents_constants.COMMON.NUM_PARALLEL_ENVS].value,
                            env_kwargs={"config": config}, vec_env_cls=DummyVecEnv)
         env = VecMonitor(env)
 
         # Training runs, one per seed
         for seed in self.experiment_config.random_seeds:
@@ -131,29 +130,32 @@
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_UPPER_BOUND_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RANDOM_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_HEURISTIC_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNTIME] = []
             ExperimentUtil.set_seed(seed)
 
             # Callback for logging training metrics
+            L = 1
+            if agents_constants.COMMON.L in self.experiment_config.hparams:
+                L = self.experiment_config.hparams[agents_constants.COMMON.L].value
             cb = PPOTrainingCallback(
                 eval_every=self.experiment_config.hparams[agents_constants.COMMON.EVAL_EVERY].value,
                 eval_batch_size=self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value,
                 random_seeds=self.experiment_config.random_seeds, training_job=self.training_job,
                 max_steps=self.experiment_config.hparams[agents_constants.COMMON.NUM_TRAINING_TIMESTEPS].value,
                 seed=seed, exp_result=exp_result, simulation_name=self.simulation_env_config.name,
                 player_type=self.experiment_config.player_type,
                 states=self.simulation_env_config.state_space_config.states,
                 actions=(
                     self.simulation_env_config.joint_action_space_config.action_spaces[
                         self.experiment_config.player_idx].actions),
                 save_every=self.experiment_config.hparams[agents_constants.COMMON.SAVE_EVERY].value,
                 save_dir=self.experiment_config.output_dir, exp_execution=self.exp_execution,
                 env=orig_env, experiment_config=self.experiment_config,
-                L=self.experiment_config.hparams[agents_constants.COMMON.L].value,
+                L=L,
                 gym_env_name=self.simulation_env_config.gym_env_name,
                 start=self.start, save_to_metastore=self.save_to_metastore
             )
 
             # Create PPO Agent
             policy_kwargs = dict(
                 net_arch=[self.experiment_config.hparams[constants.NEURAL_NETWORKS.NUM_NEURONS_PER_HIDDEN_LAYER].value
```

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/q_learning/q_learning_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/q_learning/q_learning_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/random_search/random_search_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/random_search/random_search_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/reinforce/reinforce_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/reinforce/reinforce_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/sarsa/sarsa_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/sarsa/sarsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/t_fp/t_fp_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/t_fp/t_fp_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 from csle_agents.agents.t_spsa.t_spsa_agent import TSPSAAgent
 import csle_agents.constants.constants as agents_constants
 import gym_csle_stopping_game.constants.constants as env_constants
 
 
 class TFPAgent(BaseAgent):
     """
-    RL Agent implementing the T-FP algorithm from TODO
+    RL Agent implementing the T-FP algorithm from (Hammar & Stadler '23 - Learning Near-Optimal Intrusion Responses
+    Against Dynamic Attackers)
     """
 
     def __init__(self, defender_simulation_env_config: SimulationEnvConfig,
                  attacker_simulation_env_config: SimulationEnvConfig,
                  emulation_env_config: Union[None, EmulationEnvConfig], experiment_config: ExperimentConfig,
                  training_job: Optional[TrainingJobConfig] = None):
         """
```

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/t_spsa/t_spsa_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/t_spsa/t_spsa_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,15 +577,15 @@
         """
         Gets the policy from a parameter vector
 
         :param theta: the parameter vector
         :param L: the number of parameters
         :return: the policy object
         """
-        if self.experiment_config.hparams[constants.T_SPSA.POLICY_TYPE] == PolicyType.MULTI_THRESHOLD:
+        if self.experiment_config.hparams[constants.T_SPSA.POLICY_TYPE].value == PolicyType.MULTI_THRESHOLD.value:
             policy = MultiThresholdStoppingPolicy(
                 theta=theta, simulation_name=self.simulation_env_config.name,
                 states=self.simulation_env_config.state_space_config.states,
                 player_type=self.experiment_config.player_type, L=L,
                 actions=self.simulation_env_config.joint_action_space_config.action_spaces[
                     self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
                 agent_type=AgentType.T_SPSA)
```

### Comparing `csle_agents-0.2.0/src/csle_agents/agents/vi/vi_agent.py` & `csle_agents-0.2.1/src/csle_agents/agents/vi/vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/common/actor_critic_net.py` & `csle_agents-0.2.1/src/csle_agents/common/actor_critic_net.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/common/fnn_w_gaussian.py` & `csle_agents-0.2.1/src/csle_agents/common/fnn_w_gaussian.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/common/fnn_w_linear.py` & `csle_agents-0.2.1/src/csle_agents/common/fnn_w_linear.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/common/pruning.py` & `csle_agents-0.2.1/src/csle_agents/common/pruning.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents/constants/constants.py` & `csle_agents-0.2.1/src/csle_agents/constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,7 +373,20 @@
     DEFENDER_ACTION = "a1"
     ATTACKER_ACTION = "a2"
     OBSERVATION = "o"
     TIME_STEP = "t"
     AVERAGE_UPPER_BOUND_RETURN = "average_upper_bound_return"
     AVERAGE_RANDOM_RETURN = "average_random_return"
     AVERAGE_HEURISTIC_RETURN = "average_heuristic_return"
+
+
+class LOCAL_DFSP:
+    """
+    String constants related to the local DFSP algorithm
+    """
+    BEST_RESPONSE_EVALUATION_ITERATIONS = "best_response_evaluation_iterations"
+    EQUILIBRIUM_STRATEGIES_EVALUATION_ITERATIONS = "equilibrium_strategies_evaluation_iterations"
+    AVERAGE_BEST_RESPONSE_DEFENDER_RETURN = "average_best_response_defender_return"
+    RUNNING_AVERAGE_BEST_RESPONSE_DEFENDER_RETURN = "running_average_best_response_defender_return"
+    AVERAGE_BEST_RESPONSE_ATTACKER_RETURN = "average_best_response_attacker_return"
+    RUNNING_AVERAGE_BEST_RESPONSE_ATTACKER_RETURN = "running_average_best_response_attacker_return"
+    N_2 = "N_2"
```

### Comparing `csle_agents-0.2.0/src/csle_agents/job_controllers/training_job_manager.py` & `csle_agents-0.2.1/src/csle_agents/job_controllers/training_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.0/src/csle_agents.egg-info/PKG-INFO` & `csle_agents-0.2.1/src/csle_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-agents
-Version: 0.2.0
+Version: 0.2.1
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.2.0/src/csle_agents.egg-info/SOURCES.txt` & `csle_agents-0.2.1/src/csle_agents.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 src/csle_agents/agents/__init__.py
 src/csle_agents/agents/base/__init__.py
 src/csle_agents/agents/base/base_agent.py
 src/csle_agents/agents/bayesian_optimization/__init__.py
 src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
 src/csle_agents/agents/cross_entropy/__init__.py
 src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
+src/csle_agents/agents/dfsp_local/__init__.py
+src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
+src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
 src/csle_agents/agents/differential_evolution/__init__.py
 src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
 src/csle_agents/agents/dqn/__init__.py
 src/csle_agents/agents/dqn/dqn_agent.py
 src/csle_agents/agents/dynasec/__init__.py
 src/csle_agents/agents/dynasec/dynasec_agent.py
 src/csle_agents/agents/fp/__init__.py
```

