# Comparing `tmp/csle_agents-0.2.2.tar.gz` & `tmp/csle_agents-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_agents-0.2.2.tar", last modified: Wed May 31 11:49:40 2023, max compression
+gzip compressed data, was "csle_agents-0.2.3.tar", last modified: Wed May 31 12:15:35 2023, max compression
```

## Comparing `csle_agents-0.2.2.tar` & `csle_agents-0.2.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:40.001761 csle_agents-0.2.2/
--rw-r--r--   0 kimham     (501) staff       (20)      653 2023-05-31 11:49:40.001944 csle_agents-0.2.2/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     4154 2023-01-11 18:45:47.000000 csle_agents-0.2.2/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      671 2023-02-12 08:59:32.000000 csle_agents-0.2.2/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1410 2023-05-31 11:49:40.003020 csle_agents-0.2.2/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_agents-0.2.2/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.919070 csle_agents-0.2.2/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.928131 csle_agents-0.2.2/src/csle_agents/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:45:39.000000 csle_agents-0.2.2/src/csle_agents/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.931761 csle_agents-0.2.2/src/csle_agents/agents/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/__init__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.932387 csle_agents-0.2.2/src/csle_agents/agents/base/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/base/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1854 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/base/base_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.933651 csle_agents-0.2.2/src/csle_agents/agents/bayesian_optimization/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-04-25 08:30:10.000000 csle_agents-0.2.2/src/csle_agents/agents/bayesian_optimization/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    28162 2023-04-25 11:33:39.000000 csle_agents-0.2.2/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.935699 csle_agents-0.2.2/src/csle_agents/agents/cross_entropy/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/cross_entropy/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    26958 2023-05-24 17:32:13.000000 csle_agents-0.2.2/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.938984 csle_agents-0.2.2/src/csle_agents/agents/dfsp_local/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/dfsp_local/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    37993 2023-05-24 17:19:50.000000 csle_agents-0.2.2/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
--rw-r--r--   0 kimham     (501) staff       (20)    39891 2023-05-24 17:19:50.000000 csle_agents-0.2.2/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.940757 csle_agents-0.2.2/src/csle_agents/agents/differential_evolution/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/differential_evolution/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    31471 2023-05-24 17:30:57.000000 csle_agents-0.2.2/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.942846 csle_agents-0.2.2/src/csle_agents/agents/dqn/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/dqn/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    19153 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/dqn/dqn_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.945176 csle_agents-0.2.2/src/csle_agents/agents/dynasec/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/dynasec/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    75392 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/dynasec/dynasec_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.947392 csle_agents-0.2.2/src/csle_agents/agents/fp/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/fp/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    18259 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/fp/fictitious_play_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.949105 csle_agents-0.2.2/src/csle_agents/agents/hsvi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/hsvi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    49313 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/hsvi/hsvi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.951222 csle_agents-0.2.2/src/csle_agents/agents/hsvi_os_posg/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/hsvi_os_posg/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    75255 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.953597 csle_agents-0.2.2/src/csle_agents/agents/kiefer_wolfowitz/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    28849 2023-04-25 09:34:50.000000 csle_agents-0.2.2/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.955244 csle_agents-0.2.2/src/csle_agents/agents/lp_nf/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/lp_nf/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    18360 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.956776 csle_agents-0.2.2/src/csle_agents/agents/pi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/pi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    17642 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/pi/pi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.958887 csle_agents-0.2.2/src/csle_agents/agents/ppo/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/ppo/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    25589 2023-05-02 09:52:34.000000 csle_agents-0.2.2/src/csle_agents/agents/ppo/ppo_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.961746 csle_agents-0.2.2/src/csle_agents/agents/q_learning/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/q_learning/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    17360 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/q_learning/q_learning_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.965207 csle_agents-0.2.2/src/csle_agents/agents/random_search/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/random_search/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    26175 2023-04-25 09:38:36.000000 csle_agents-0.2.2/src/csle_agents/agents/random_search/random_search_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.967242 csle_agents-0.2.2/src/csle_agents/agents/reinforce/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/reinforce/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    25109 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/reinforce/reinforce_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.973451 csle_agents-0.2.2/src/csle_agents/agents/sarsa/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/sarsa/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    17456 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/sarsa/sarsa_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.975008 csle_agents-0.2.2/src/csle_agents/agents/shapley_iteration/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/shapley_iteration/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    15788 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.979216 csle_agents-0.2.2/src/csle_agents/agents/sondik_vi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/sondik_vi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    22182 2023-03-31 11:14:06.000000 csle_agents-0.2.2/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.986214 csle_agents-0.2.2/src/csle_agents/agents/t_fp/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/t_fp/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    41988 2023-05-01 11:12:26.000000 csle_agents-0.2.2/src/csle_agents/agents/t_fp/t_fp_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.988222 csle_agents-0.2.2/src/csle_agents/agents/t_spsa/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/t_spsa/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    32117 2023-05-24 17:29:31.000000 csle_agents-0.2.2/src/csle_agents/agents/t_spsa/t_spsa_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.993030 csle_agents-0.2.2/src/csle_agents/agents/vi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/agents/vi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    16358 2023-04-29 14:22:16.000000 csle_agents-0.2.2/src/csle_agents/agents/vi/vi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.998178 csle_agents-0.2.2/src/csle_agents/common/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/common/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     5759 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/common/actor_critic_net.py
--rw-r--r--   0 kimham     (501) staff       (20)     4595 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/common/fnn_w_gaussian.py
--rw-r--r--   0 kimham     (501) staff       (20)     3936 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/common/fnn_w_linear.py
--rw-r--r--   0 kimham     (501) staff       (20)     3460 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/common/pruning.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:40.000011 csle_agents-0.2.2/src/csle_agents/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    11876 2023-05-01 11:24:17.000000 csle_agents-0.2.2/src/csle_agents/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:40.001154 csle_agents-0.2.2/src/csle_agents/job_controllers/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/job_controllers/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2459 2022-11-28 13:00:49.000000 csle_agents-0.2.2/src/csle_agents/job_controllers/training_job_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:49:39.931345 csle_agents-0.2.2/src/csle_agents.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      653 2023-05-31 11:49:39.000000 csle_agents-0.2.2/src/csle_agents.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3034 2023-05-31 11:49:39.000000 csle_agents-0.2.2/src/csle_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:49:39.000000 csle_agents-0.2.2/src/csle_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:28.000000 csle_agents-0.2.2/src/csle_agents.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      371 2023-05-31 11:49:39.000000 csle_agents-0.2.2/src/csle_agents.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       12 2023-05-31 11:49:39.000000 csle_agents-0.2.2/src/csle_agents.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.085434 csle_agents-0.2.3/
+-rw-r--r--   0 kimham     (501) staff       (20)      653 2023-05-31 12:15:35.085621 csle_agents-0.2.3/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     4154 2023-01-11 18:45:47.000000 csle_agents-0.2.3/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      671 2023-02-12 08:59:32.000000 csle_agents-0.2.3/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1410 2023-05-31 12:15:35.086381 csle_agents-0.2.3/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_agents-0.2.3/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.028389 csle_agents-0.2.3/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.040346 csle_agents-0.2.3/src/csle_agents/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 12:12:15.000000 csle_agents-0.2.3/src/csle_agents/__version__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.042904 csle_agents-0.2.3/src/csle_agents/agents/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/__init__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.043473 csle_agents-0.2.3/src/csle_agents/agents/base/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/base/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1854 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/base/base_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.044462 csle_agents-0.2.3/src/csle_agents/agents/bayesian_optimization/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-04-25 08:30:10.000000 csle_agents-0.2.3/src/csle_agents/agents/bayesian_optimization/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    28162 2023-04-25 11:33:39.000000 csle_agents-0.2.3/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.045765 csle_agents-0.2.3/src/csle_agents/agents/cross_entropy/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/cross_entropy/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    26958 2023-05-24 17:32:13.000000 csle_agents-0.2.3/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.048506 csle_agents-0.2.3/src/csle_agents/agents/dfsp_local/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/dfsp_local/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    37993 2023-05-24 17:19:50.000000 csle_agents-0.2.3/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
+-rw-r--r--   0 kimham     (501) staff       (20)    39891 2023-05-24 17:19:50.000000 csle_agents-0.2.3/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.049903 csle_agents-0.2.3/src/csle_agents/agents/differential_evolution/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/differential_evolution/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    31471 2023-05-24 17:30:57.000000 csle_agents-0.2.3/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.051117 csle_agents-0.2.3/src/csle_agents/agents/dqn/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/dqn/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    19153 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/dqn/dqn_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.052642 csle_agents-0.2.3/src/csle_agents/agents/dynasec/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/dynasec/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    75392 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/dynasec/dynasec_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.053918 csle_agents-0.2.3/src/csle_agents/agents/fp/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/fp/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    18259 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/fp/fictitious_play_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.054914 csle_agents-0.2.3/src/csle_agents/agents/hsvi/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/hsvi/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    49313 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/hsvi/hsvi_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.056175 csle_agents-0.2.3/src/csle_agents/agents/hsvi_os_posg/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/hsvi_os_posg/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    75255 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.057439 csle_agents-0.2.3/src/csle_agents/agents/kiefer_wolfowitz/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    28849 2023-04-25 09:34:50.000000 csle_agents-0.2.3/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.058565 csle_agents-0.2.3/src/csle_agents/agents/lp_nf/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/lp_nf/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    18360 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.061255 csle_agents-0.2.3/src/csle_agents/agents/pi/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/pi/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    17642 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/pi/pi_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.065125 csle_agents-0.2.3/src/csle_agents/agents/ppo/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/ppo/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    25589 2023-05-02 09:52:34.000000 csle_agents-0.2.3/src/csle_agents/agents/ppo/ppo_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.067008 csle_agents-0.2.3/src/csle_agents/agents/q_learning/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/q_learning/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    17360 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/q_learning/q_learning_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.068516 csle_agents-0.2.3/src/csle_agents/agents/random_search/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/random_search/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    26175 2023-04-25 09:38:36.000000 csle_agents-0.2.3/src/csle_agents/agents/random_search/random_search_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.070215 csle_agents-0.2.3/src/csle_agents/agents/reinforce/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/reinforce/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    25109 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/reinforce/reinforce_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.072225 csle_agents-0.2.3/src/csle_agents/agents/sarsa/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/sarsa/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    17456 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/sarsa/sarsa_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.073714 csle_agents-0.2.3/src/csle_agents/agents/shapley_iteration/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/shapley_iteration/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    15788 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.074696 csle_agents-0.2.3/src/csle_agents/agents/sondik_vi/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/sondik_vi/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    22182 2023-03-31 11:14:06.000000 csle_agents-0.2.3/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.076862 csle_agents-0.2.3/src/csle_agents/agents/t_fp/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/t_fp/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    41988 2023-05-01 11:12:26.000000 csle_agents-0.2.3/src/csle_agents/agents/t_fp/t_fp_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.078256 csle_agents-0.2.3/src/csle_agents/agents/t_spsa/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/t_spsa/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    32117 2023-05-24 17:29:31.000000 csle_agents-0.2.3/src/csle_agents/agents/t_spsa/t_spsa_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.079736 csle_agents-0.2.3/src/csle_agents/agents/vi/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/agents/vi/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    16358 2023-04-29 14:22:16.000000 csle_agents-0.2.3/src/csle_agents/agents/vi/vi_agent.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.082902 csle_agents-0.2.3/src/csle_agents/common/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/common/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5759 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/common/actor_critic_net.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4595 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/common/fnn_w_gaussian.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3936 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/common/fnn_w_linear.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3460 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/common/pruning.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.083833 csle_agents-0.2.3/src/csle_agents/constants/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/constants/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11876 2023-05-01 11:24:17.000000 csle_agents-0.2.3/src/csle_agents/constants/constants.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.084756 csle_agents-0.2.3/src/csle_agents/job_controllers/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/job_controllers/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2459 2022-11-28 13:00:49.000000 csle_agents-0.2.3/src/csle_agents/job_controllers/training_job_manager.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:15:35.042558 csle_agents-0.2.3/src/csle_agents.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      653 2023-05-31 12:15:34.000000 csle_agents-0.2.3/src/csle_agents.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     3034 2023-05-31 12:15:35.000000 csle_agents-0.2.3/src/csle_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 12:15:34.000000 csle_agents-0.2.3/src/csle_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:28.000000 csle_agents-0.2.3/src/csle_agents.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      371 2023-05-31 12:15:34.000000 csle_agents-0.2.3/src/csle_agents.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       12 2023-05-31 12:15:34.000000 csle_agents-0.2.3/src/csle_agents.egg-info/top_level.txt
```

### Comparing `csle_agents-0.2.2/PKG-INFO` & `csle_agents-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_agents
-Version: 0.2.2
+Version: 0.2.3
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.2.2/README.md` & `csle_agents-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/pyproject.toml` & `csle_agents-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/setup.cfg` & `csle_agents-0.2.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.2.2
-	csle-collector>=0.2.2
-	csle-attacker>=0.2.2
-	csle-defender>=0.2.2
-	csle-system-identification>=0.2.2
-	gym-csle-stopping-game>=0.2.2
+	csle-common>=0.2.3
+	csle-collector>=0.2.3
+	csle-attacker>=0.2.3
+	csle-defender>=0.2.3
+	csle-system-identification>=0.2.3
+	gym-csle-stopping-game>=0.2.3
 	stable-baselines3>=1.8.0
 	pulp>=2.7.0
 	bayesian-optimization>=1.3.1
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/base/base_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/base/base_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/dqn/dqn_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/dqn/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/dynasec/dynasec_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/dynasec/dynasec_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/fp/fictitious_play_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/fp/fictitious_play_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/hsvi/hsvi_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/hsvi/hsvi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/pi/pi_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/pi/pi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/ppo/ppo_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/ppo/ppo_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/q_learning/q_learning_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/q_learning/q_learning_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/random_search/random_search_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/random_search/random_search_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/reinforce/reinforce_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/reinforce/reinforce_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/sarsa/sarsa_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/sarsa/sarsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/t_fp/t_fp_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/t_fp/t_fp_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/t_spsa/t_spsa_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/t_spsa/t_spsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/agents/vi/vi_agent.py` & `csle_agents-0.2.3/src/csle_agents/agents/vi/vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/common/actor_critic_net.py` & `csle_agents-0.2.3/src/csle_agents/common/actor_critic_net.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/common/fnn_w_gaussian.py` & `csle_agents-0.2.3/src/csle_agents/common/fnn_w_gaussian.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/common/fnn_w_linear.py` & `csle_agents-0.2.3/src/csle_agents/common/fnn_w_linear.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/common/pruning.py` & `csle_agents-0.2.3/src/csle_agents/common/pruning.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/constants/constants.py` & `csle_agents-0.2.3/src/csle_agents/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents/job_controllers/training_job_manager.py` & `csle_agents-0.2.3/src/csle_agents/job_controllers/training_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.2/src/csle_agents.egg-info/PKG-INFO` & `csle_agents-0.2.3/src/csle_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-agents
-Version: 0.2.2
+Version: 0.2.3
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.2.2/src/csle_agents.egg-info/SOURCES.txt` & `csle_agents-0.2.3/src/csle_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

