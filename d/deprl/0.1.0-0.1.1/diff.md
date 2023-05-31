# Comparing `tmp/deprl-0.1.0.tar.gz` & `tmp/deprl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprl-0.1.0.tar", max compression
+gzip compressed data, was "deprl-0.1.1.tar", max compression
```

## Comparing `deprl-0.1.0.tar` & `deprl-0.1.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0     1083 2023-04-19 09:11:34.327760 deprl-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     6881 2023-04-28 12:48:24.334114 deprl-0.1.0/README.md
--rw-r--r--   0        0        0      529 2023-05-14 15:44:14.190590 deprl-0.1.0/deprl/__init__.py
--rw-r--r--   0        0        0     5819 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/custom_agents.py
--rw-r--r--   0        0        0     8859 2023-04-08 11:41:40.942841 deprl-0.1.0/deprl/custom_distributed.py
--rw-r--r--   0        0        0     3639 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/custom_mpo_torch.py
--rw-r--r--   0        0        0     3476 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/custom_test_environment.py
--rw-r--r--   0        0        0     1244 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/custom_torso.py
--rw-r--r--   0        0        0     5818 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/custom_trainer.py
--rw-r--r--   0        0        0     7373 2023-04-08 11:41:40.942841 deprl-0.1.0/deprl/dep_controller.py
--rw-r--r--   0        0        0      132 2023-04-08 11:41:40.942841 deprl-0.1.0/deprl/env_wrappers/__init__.py
--rw-r--r--   0        0        0     5534 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/env_wrappers/wrappers.py
--rw-r--r--   0        0        0     2121 2023-05-15 12:13:39.110351 deprl-0.1.0/deprl/log.py
--rw-r--r--   0        0        0     7722 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/main.py
--rw-r--r--   0        0        0      704 2023-04-08 11:41:40.942841 deprl-0.1.0/deprl/param_files/default_agents.json
--rw-r--r--   0        0        0     9038 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/play.py
--rw-r--r--   0        0        0    10596 2023-05-12 16:32:07.067142 deprl-0.1.0/deprl/play_plot.py
--rw-r--r--   0        0        0       80 2023-05-14 15:44:14.190590 deprl-0.1.0/deprl/plot.py
--rw-r--r--   0        0        0      115 2023-05-14 15:44:14.190590 deprl-0.1.0/deprl/utils/__init__.py
--rw-r--r--   0        0        0     3741 2023-05-15 11:57:15.335445 deprl-0.1.0/deprl/utils/utils.py
--rw-r--r--   0        0        0       39 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/__init__.py
--rwxr-xr-x   0        0        0       80 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/.gitignore
--rw-r--r--   0        0        0     1110 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/LICENSE
--rw-r--r--   0        0        0      207 2023-05-11 10:40:42.082155 deprl-0.1.0/deprl/vendor/tonic/__init__.py
--rw-r--r--   0        0        0      178 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/agents/__init__.py
--rw-r--r--   0        0        0     1038 2023-05-14 15:44:14.190590 deprl-0.1.0/deprl/vendor/tonic/agents/agent.py
--rw-r--r--   0        0        0     3954 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/agents/basic.py
--rw-r--r--   0        0        0      293 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/environments/__init__.py
--rw-r--r--   0        0        0     5641 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/environments/builders.py
--rw-r--r--   0        0        0     6612 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/environments/distributed.py
--rw-r--r--   0        0        0     1914 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/environments/wrappers.py
--rw-r--r--   0        0        0      175 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/explorations/__init__.py
--rw-r--r--   0        0        0     2939 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/explorations/noisy.py
--rw-r--r--   0        0        0     8754 2023-04-21 17:51:40.339710 deprl-0.1.0/deprl/vendor/tonic/play.py
--rw-r--r--   0        0        0    18151 2023-05-14 15:44:14.190590 deprl-0.1.0/deprl/vendor/tonic/plot.py
--rw-r--r--   0        0        0      167 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/replays/__init__.py
--rw-r--r--   0        0        0     3636 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/replays/buffers.py
--rw-r--r--   0        0        0     2815 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/replays/segments.py
--rw-r--r--   0        0        0      821 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/replays/utils.py
--rw-r--r--   0        0        0      103 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/__init__.py
--rw-r--r--   0        0        0      303 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/__init__.py
--rw-r--r--   0        0        0     4630 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/a2c.py
--rw-r--r--   0        0        0      519 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/agent.py
--rw-r--r--   0        0        0     1456 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/d4pg.py
--rw-r--r--   0        0        0     4327 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/ddpg.py
--rw-r--r--   0        0        0     4089 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/mpo.py
--rw-r--r--   0        0        0     2452 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/ppo.py
--rw-r--r--   0        0        0     1868 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/sac.py
--rw-r--r--   0        0        0     2181 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/td3.py
--rw-r--r--   0        0        0     1448 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/td4.py
--rw-r--r--   0        0        0     3754 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/trpo.py
--rw-r--r--   0        0        0      819 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/__init__.py
--rw-r--r--   0        0        0     6247 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/actor_critics.py
--rw-r--r--   0        0        0     4849 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/actors.py
--rw-r--r--   0        0        0     3046 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/critics.py
--rw-r--r--   0        0        0      734 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/encoders.py
--rw-r--r--   0        0        0      627 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/utils.py
--rw-r--r--   0        0        0       88 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
--rw-r--r--   0        0        0     2442 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1339 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/normalizers/returns.py
--rw-r--r--   0        0        0     1260 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/updaters/__init__.py
--rw-r--r--   0        0        0    19301 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/updaters/actors.py
--rw-r--r--   0        0        0    13820 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/updaters/critics.py
--rw-r--r--   0        0        0     4232 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
--rw-r--r--   0        0        0      193 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/tensorflow/updaters/utils.py
--rw-r--r--   0        0        0      103 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/__init__.py
--rw-r--r--   0        0        0      277 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/agents/__init__.py
--rw-r--r--   0        0        0     5287 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/agents/a2c.py
--rw-r--r--   0        0        0     1441 2023-05-14 15:44:14.190590 deprl-0.1.0/deprl/vendor/tonic/torch/agents/agent.py
--rw-r--r--   0        0        0     1522 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/agents/d4pg.py
--rw-r--r--   0        0        0     4551 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/agents/ddpg.py
--rw-r--r--   0        0        0     4446 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/agents/mpo.py
--rw-r--r--   0        0        0     2608 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/agents/ppo.py
--rw-r--r--   0        0        0     2102 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/agents/sac.py
--rw-r--r--   0        0        0     2315 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/agents/td3.py
--rw-r--r--   0        0        0     4077 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/agents/trpo.py
--rw-r--r--   0        0        0      817 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/models/__init__.py
--rw-r--r--   0        0        0     5824 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/models/actor_critics.py
--rw-r--r--   0        0        0     4874 2023-05-12 09:59:41.471381 deprl-0.1.0/deprl/vendor/tonic/torch/models/actors.py
--rw-r--r--   0        0        0     3177 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/models/critics.py
--rw-r--r--   0        0        0     1084 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/models/encoders.py
--rw-r--r--   0        0        0      791 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/models/utils.py
--rw-r--r--   0        0        0       88 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/normalizers/__init__.py
--rw-r--r--   0        0        0     2615 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1429 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/normalizers/returns.py
--rw-r--r--   0        0        0     1156 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/updaters/__init__.py
--rw-r--r--   0        0        0    20504 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/updaters/actors.py
--rw-r--r--   0        0        0    11054 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/updaters/critics.py
--rw-r--r--   0        0        0     4317 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/updaters/optimizers.py
--rw-r--r--   0        0        0      156 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/torch/updaters/utils.py
--rw-r--r--   0        0        0     5722 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/train.py
--rw-r--r--   0        0        0      213 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/utils/__init__.py
--rw-r--r--   0        0        0      822 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/utils/csv_utils.py
--rw-r--r--   0        0        0     8867 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/utils/logger.py
--rw-r--r--   0        0        0     5477 2023-04-21 17:51:40.343710 deprl-0.1.0/deprl/vendor/tonic/utils/trainer.py
--rw-r--r--   0        0        0     1276 2023-05-15 11:58:17.698616 deprl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8671 1970-01-01 00:00:00.000000 deprl-0.1.0/setup.py
--rw-r--r--   0        0        0     7742 1970-01-01 00:00:00.000000 deprl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-19 09:11:34.327760 deprl-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     7411 2023-05-25 12:51:55.706811 deprl-0.1.1/README.md
+-rw-r--r--   0        0        0      529 2023-05-25 12:51:55.722810 deprl-0.1.1/deprl/__init__.py
+-rw-r--r--   0        0        0     5819 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/custom_agents.py
+-rw-r--r--   0        0        0     8956 2023-05-31 08:20:41.661687 deprl-0.1.1/deprl/custom_distributed.py
+-rw-r--r--   0        0        0     3639 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/custom_mpo_torch.py
+-rw-r--r--   0        0        0     3476 2023-05-31 08:19:31.158603 deprl-0.1.1/deprl/custom_test_environment.py
+-rw-r--r--   0        0        0     1244 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/custom_torso.py
+-rw-r--r--   0        0        0     5818 2023-05-31 08:19:31.186602 deprl-0.1.1/deprl/custom_trainer.py
+-rw-r--r--   0        0        0     7373 2023-04-08 11:41:40.942841 deprl-0.1.1/deprl/dep_controller.py
+-rw-r--r--   0        0        0      132 2023-05-31 08:19:31.186602 deprl-0.1.1/deprl/env_wrappers/__init__.py
+-rw-r--r--   0        0        0     5534 2023-05-31 08:19:31.210602 deprl-0.1.1/deprl/env_wrappers/wrappers.py
+-rw-r--r--   0        0        0     2120 2023-05-25 12:51:55.722810 deprl-0.1.1/deprl/log.py
+-rw-r--r--   0        0        0     7722 2023-05-19 19:35:23.071772 deprl-0.1.1/deprl/main.py
+-rw-r--r--   0        0        0      704 2023-04-08 11:41:40.942841 deprl-0.1.1/deprl/param_files/default_agents.json
+-rw-r--r--   0        0        0     9038 2023-05-31 08:19:31.234602 deprl-0.1.1/deprl/play.py
+-rw-r--r--   0        0        0    10596 2023-05-12 16:32:07.067142 deprl-0.1.1/deprl/play_plot.py
+-rw-r--r--   0        0        0       80 2023-05-25 12:51:55.726810 deprl-0.1.1/deprl/plot.py
+-rw-r--r--   0        0        0      115 2023-05-25 12:51:55.726810 deprl-0.1.1/deprl/utils/__init__.py
+-rw-r--r--   0        0        0     3741 2023-05-25 12:51:55.738810 deprl-0.1.1/deprl/utils/utils.py
+-rw-r--r--   0        0        0       39 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/__init__.py
+-rwxr-xr-x   0        0        0       80 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/.gitignore
+-rw-r--r--   0        0        0     1110 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/LICENSE
+-rw-r--r--   0        0        0      207 2023-05-11 10:40:42.082155 deprl-0.1.1/deprl/vendor/tonic/__init__.py
+-rw-r--r--   0        0        0      178 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/agents/__init__.py
+-rw-r--r--   0        0        0     1038 2023-05-25 12:51:55.738810 deprl-0.1.1/deprl/vendor/tonic/agents/agent.py
+-rw-r--r--   0        0        0     3954 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/agents/basic.py
+-rw-r--r--   0        0        0      293 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/environments/__init__.py
+-rw-r--r--   0        0        0     5641 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/environments/builders.py
+-rw-r--r--   0        0        0     6612 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/environments/distributed.py
+-rw-r--r--   0        0        0     1914 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/environments/wrappers.py
+-rw-r--r--   0        0        0      175 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/explorations/__init__.py
+-rw-r--r--   0        0        0     2939 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/explorations/noisy.py
+-rw-r--r--   0        0        0     8754 2023-04-21 17:51:40.339710 deprl-0.1.1/deprl/vendor/tonic/play.py
+-rw-r--r--   0        0        0    18151 2023-05-25 12:51:55.738810 deprl-0.1.1/deprl/vendor/tonic/plot.py
+-rw-r--r--   0        0        0      167 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/replays/__init__.py
+-rw-r--r--   0        0        0     3636 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/replays/buffers.py
+-rw-r--r--   0        0        0     2815 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/replays/segments.py
+-rw-r--r--   0        0        0      821 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/replays/utils.py
+-rw-r--r--   0        0        0      103 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/__init__.py
+-rw-r--r--   0        0        0      303 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/__init__.py
+-rw-r--r--   0        0        0     4630 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/a2c.py
+-rw-r--r--   0        0        0      519 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/agent.py
+-rw-r--r--   0        0        0     1456 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/d4pg.py
+-rw-r--r--   0        0        0     4327 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/ddpg.py
+-rw-r--r--   0        0        0     4089 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/mpo.py
+-rw-r--r--   0        0        0     2452 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/ppo.py
+-rw-r--r--   0        0        0     1868 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/sac.py
+-rw-r--r--   0        0        0     2181 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/td3.py
+-rw-r--r--   0        0        0     1448 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/td4.py
+-rw-r--r--   0        0        0     3754 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/trpo.py
+-rw-r--r--   0        0        0      819 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/__init__.py
+-rw-r--r--   0        0        0     6247 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/actor_critics.py
+-rw-r--r--   0        0        0     4849 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/actors.py
+-rw-r--r--   0        0        0     3046 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/critics.py
+-rw-r--r--   0        0        0      734 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/encoders.py
+-rw-r--r--   0        0        0      627 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/utils.py
+-rw-r--r--   0        0        0       88 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
+-rw-r--r--   0        0        0     2442 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1339 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/normalizers/returns.py
+-rw-r--r--   0        0        0     1260 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/updaters/__init__.py
+-rw-r--r--   0        0        0    19301 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/updaters/actors.py
+-rw-r--r--   0        0        0    13820 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/updaters/critics.py
+-rw-r--r--   0        0        0     4232 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
+-rw-r--r--   0        0        0      193 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/tensorflow/updaters/utils.py
+-rw-r--r--   0        0        0      103 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/agents/__init__.py
+-rw-r--r--   0        0        0     5287 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/agents/a2c.py
+-rw-r--r--   0        0        0     1441 2023-05-25 12:51:55.738810 deprl-0.1.1/deprl/vendor/tonic/torch/agents/agent.py
+-rw-r--r--   0        0        0     1522 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/agents/d4pg.py
+-rw-r--r--   0        0        0     4551 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/agents/ddpg.py
+-rw-r--r--   0        0        0     4446 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/agents/mpo.py
+-rw-r--r--   0        0        0     2608 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/agents/ppo.py
+-rw-r--r--   0        0        0     2102 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/agents/sac.py
+-rw-r--r--   0        0        0     2315 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/agents/td3.py
+-rw-r--r--   0        0        0     4077 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/agents/trpo.py
+-rw-r--r--   0        0        0      817 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/models/__init__.py
+-rw-r--r--   0        0        0     5824 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/models/actor_critics.py
+-rw-r--r--   0        0        0     4874 2023-05-12 09:59:41.471381 deprl-0.1.1/deprl/vendor/tonic/torch/models/actors.py
+-rw-r--r--   0        0        0     3177 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/models/critics.py
+-rw-r--r--   0        0        0     1084 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/models/encoders.py
+-rw-r--r--   0        0        0      791 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/models/utils.py
+-rw-r--r--   0        0        0       88 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/normalizers/__init__.py
+-rw-r--r--   0        0        0     2615 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1429 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/normalizers/returns.py
+-rw-r--r--   0        0        0     1156 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/updaters/__init__.py
+-rw-r--r--   0        0        0    20504 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/updaters/actors.py
+-rw-r--r--   0        0        0    11054 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/updaters/critics.py
+-rw-r--r--   0        0        0     4317 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/updaters/optimizers.py
+-rw-r--r--   0        0        0      156 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/torch/updaters/utils.py
+-rw-r--r--   0        0        0     5722 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/train.py
+-rw-r--r--   0        0        0      213 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/utils/__init__.py
+-rw-r--r--   0        0        0      822 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/utils/csv_utils.py
+-rw-r--r--   0        0        0     8867 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/utils/logger.py
+-rw-r--r--   0        0        0     5477 2023-04-21 17:51:40.343710 deprl-0.1.1/deprl/vendor/tonic/utils/trainer.py
+-rw-r--r--   0        0        0     1276 2023-05-31 08:21:35.484989 deprl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9207 1970-01-01 00:00:00.000000 deprl-0.1.1/setup.py
+-rw-r--r--   0        0        0     8272 1970-01-01 00:00:00.000000 deprl-0.1.1/PKG-INFO
```

### Comparing `deprl-0.1.0/LICENSE.txt` & `deprl-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/README.md` & `deprl-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 <img src=https://user-images.githubusercontent.com/24903880/229783811-44c422e9-3cc3-42e4-b657-d21be9af6458.gif width=250>
 <img src=https://user-images.githubusercontent.com/24903880/229783729-d068e87c-cb0b-43c7-91d5-ff2ba836f05b.gif width=214>
 
  <img src=https://user-images.githubusercontent.com/24903880/229783370-ee95b9c3-06a0-4ef3-9b60-78e88c4eae38.gif width=214>
 </p>
 
 
+### MyoLeg
+If you are coming here for the MyoLeg, take a look at this [tutorial](https://github.com/facebookresearch/myosuite/blob/main/docs/source/tutorials.rst#load-dep-rl-baseline). It will show you how to run the pre-trained baseline. We also explain how to train the walking agent in the MyoSuite  [documentation](https://myosuite.readthedocs.io/en/latest/baselines.html#dep-rl-baseline).  
+<p align="center">
+<img src=https://github.com/martius-lab/depRL/assets/24903880/d06200ae-ad35-484c-9d55-83b5235269bc width=350
+</p>
+
 ## Abstract
 Muscle-actuated organisms are capable of learning an unparalleled diversity of
 dexterous movements despite their vast amount of muscles. Reinforcement learning (RL) on large musculoskeletal models, however, has not been able to show
 similar performance. We conjecture that ineffective exploration in large overactuated action spaces is a key problem. This is supported by our finding that common
 exploration noise strategies are inadequate in synthetic examples of overactuated
 systems. We identify differential extrinsic plasticity (DEP), a method from the
 domain of self-organization, as being able to induce state-space covering exploration within seconds of interaction. By integrating DEP into RL, we achieve fast
```

### Comparing `deprl-0.1.0/deprl/__init__.py` & `deprl-0.1.1/deprl/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/custom_agents.py` & `deprl-0.1.1/deprl/custom_agents.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/custom_distributed.py` & `deprl-0.1.1/deprl/custom_distributed.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,16 @@
         dummy_environment.apply_args()
 
         self.observation_space = dummy_environment.observation_space
         self.action_space = dummy_environment.action_space
         del dummy_environment
         self.started = False
 
+        # fork is default on linux, but not mac
+        multiprocessing.set_start_method('fork')
         self.output_queue = multiprocessing.Queue()
         self.action_pipes = []
 
         for i in range(self.worker_groups):
             pipe, worker_end = multiprocessing.Pipe()
             self.action_pipes.append(pipe)
             group_seed = (
```

### Comparing `deprl-0.1.0/deprl/custom_mpo_torch.py` & `deprl-0.1.1/deprl/custom_mpo_torch.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/custom_test_environment.py` & `deprl-0.1.1/deprl/custom_test_environment.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/custom_torso.py` & `deprl-0.1.1/deprl/custom_torso.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/custom_trainer.py` & `deprl-0.1.1/deprl/custom_trainer.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/dep_controller.py` & `deprl-0.1.1/deprl/dep_controller.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/env_wrappers/wrappers.py` & `deprl-0.1.1/deprl/env_wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/log.py` & `deprl-0.1.1/deprl/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import os
 import time
 
+import wandb
 import yaml
 
-import wandb
 from deprl.vendor.tonic import utils
 
 
 class WandbProcessor:
     def __init__(self, path):
         self._path = path
         self._current_line_number = 0
@@ -61,10 +61,9 @@
     )
     wandb.init(project=args.project, entity="rlpractitioner", config=config)
     processor = WandbProcessor(args.path)
     while True:
         processor.update()
         time.sleep(100)
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `deprl-0.1.0/deprl/main.py` & `deprl-0.1.1/deprl/main.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/param_files/default_agents.json` & `deprl-0.1.1/deprl/param_files/default_agents.json`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/play.py` & `deprl-0.1.1/deprl/play.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/play_plot.py` & `deprl-0.1.1/deprl/play_plot.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/utils/utils.py` & `deprl-0.1.1/deprl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/LICENSE` & `deprl-0.1.1/deprl/vendor/tonic/LICENSE`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/agents/agent.py` & `deprl-0.1.1/deprl/vendor/tonic/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/agents/basic.py` & `deprl-0.1.1/deprl/vendor/tonic/agents/basic.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/environments/builders.py` & `deprl-0.1.1/deprl/vendor/tonic/environments/builders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/environments/distributed.py` & `deprl-0.1.1/deprl/vendor/tonic/environments/distributed.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/environments/wrappers.py` & `deprl-0.1.1/deprl/vendor/tonic/environments/wrappers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/explorations/noisy.py` & `deprl-0.1.1/deprl/vendor/tonic/explorations/noisy.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/play.py` & `deprl-0.1.1/deprl/vendor/tonic/play.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/plot.py` & `deprl-0.1.1/deprl/vendor/tonic/plot.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/replays/buffers.py` & `deprl-0.1.1/deprl/vendor/tonic/replays/buffers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/replays/segments.py` & `deprl-0.1.1/deprl/vendor/tonic/replays/segments.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/replays/utils.py` & `deprl-0.1.1/deprl/vendor/tonic/replays/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/a2c.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/agent.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/d4pg.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/ddpg.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/mpo.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/ppo.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/sac.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/td3.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/td4.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/td4.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/agents/trpo.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/__init__.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/actor_critics.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/actors.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/critics.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/encoders.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/models/utils.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/normalizers/returns.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/updaters/__init__.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/updaters/actors.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/updaters/critics.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/tensorflow/updaters/optimizers.py` & `deprl-0.1.1/deprl/vendor/tonic/tensorflow/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/agents/a2c.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/agents/agent.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/agents/d4pg.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/agents/ddpg.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/agents/mpo.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/agents/ppo.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/agents/sac.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/agents/td3.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/agents/trpo.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/models/__init__.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/models/actor_critics.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/models/actors.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/models/critics.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/models/encoders.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/models/utils.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/normalizers/mean_stds.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/normalizers/returns.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/updaters/__init__.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/updaters/actors.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/updaters/critics.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/torch/updaters/optimizers.py` & `deprl-0.1.1/deprl/vendor/tonic/torch/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/train.py` & `deprl-0.1.1/deprl/vendor/tonic/train.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/utils/csv_utils.py` & `deprl-0.1.1/deprl/vendor/tonic/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/utils/logger.py` & `deprl-0.1.1/deprl/vendor/tonic/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/deprl/vendor/tonic/utils/trainer.py` & `deprl-0.1.1/deprl/vendor/tonic/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.0/pyproject.toml` & `deprl-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deprl"
-version = "0.1.0"
+version = "0.1.1"
 description = "DEP-RL, a method for robust control of musculoskeletal systems."
 authors = ["Pierre Schumacher <pierre.schumacher@tuebingen.mpg.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
```

### Comparing `deprl-0.1.0/setup.py` & `deprl-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,17 @@
  'torch>=1.13.1']
 
 entry_points = \
 {'console_scripts': ['log = deprl.log:main', 'plot = deprl.plot:main']}
 
 setup_kwargs = {
     'name': 'deprl',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'DEP-RL, a method for robust control of musculoskeletal systems.',
-    'long_description': '# DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems\n\n This repo contains the code for the paper [DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems](https://openreview.net/forum?id=C-xa_D3oTj6) paper, published at ICLR 2023 with perfect review scores (8, 8, 8, 10) and a notable-top-25% rating. See [here](https://sites.google.com/view/dep-rl) for videos.\n\nThe work was performed by Pierre Schumacher, Daniel F.B. Haeufle, Dieter Büchler, Syn Schmitt and Georg Martius.\n\nIf you just want to see the code for DEP, take a look at `deprl/dep_controller.py`, `deprl/custom_agents.py` and `deprl/env_wrapper/wrappers.py`\n\n<p align="center">\n<img src=https://user-images.githubusercontent.com/24903880/229783811-44c422e9-3cc3-42e4-b657-d21be9af6458.gif width=250>\n<img src=https://user-images.githubusercontent.com/24903880/229783729-d068e87c-cb0b-43c7-91d5-ff2ba836f05b.gif width=214>\n\n <img src=https://user-images.githubusercontent.com/24903880/229783370-ee95b9c3-06a0-4ef3-9b60-78e88c4eae38.gif width=214>\n</p>\n\n\n## Abstract\nMuscle-actuated organisms are capable of learning an unparalleled diversity of\ndexterous movements despite their vast amount of muscles. Reinforcement learning (RL) on large musculoskeletal models, however, has not been able to show\nsimilar performance. We conjecture that ineffective exploration in large overactuated action spaces is a key problem. This is supported by our finding that common\nexploration noise strategies are inadequate in synthetic examples of overactuated\nsystems. We identify differential extrinsic plasticity (DEP), a method from the\ndomain of self-organization, as being able to induce state-space covering exploration within seconds of interaction. By integrating DEP into RL, we achieve fast\nlearning of reaching and locomotion in musculoskeletal systems, outperforming\ncurrent approaches in all considered tasks in sample efficiency and robustness.\n\n\n## Installation\n\nWe provide a python package for easy installation:\n```\npip install deprl\n```\nIf you would like to use `jax` with CUDA support, which significantly speeds up learning, we recommend running:\n```\npip install --upgrade "jax[cuda12_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html\n```\nor similar afterwards.\n\nThe humanreacher environment can be installed with\n```\npip install git+https://github.com/P-Schumacher/warmup.git\n```\n\nOstrichRL can be installed from [here](https://github.com/vittorione94/ostrichrl).\n\n\n## Experiments\n\nThe major experiments (humanreacher reaching and ostrich running) can be repeated with the config files.\nSimply run from the root folder:\n```\npython -m deprl.main experiments/ostrich_running_dep.json\npython -m deprl.main experiments/humanreacher.json\n```\nto train an agent. Model checkpoints will be saved in the `output` directory.\nThe progress can be monitored with:\n```\npython -m tonic.plot --path output/folder/\n```\n\nTo execute a trained policy, use:\n\n```\npython -m deprl.play --path output/folder/\n```\n\nSee the [TonicRL](https://github.com/fabiopardo/tonic) documentation for details.\n\nBe aware that ostrich training can be seed-dependant, as seen in the plots of the original publication.\n\n## Pure DEP\nIf you want to see pure DEP in action, just run the following bash files after installing the ostrichrl and warmup environments.\n```\nbash play_files/play_dep_humanreacher.sh\nbash play_files/play_dep_ostrich.sh\nbash play_files/play_dep_dmcontrol_quadruped.sh\n```\n\nYou might see a more interesting ostrich behavior by disabling episode resets in the ostrich environment first.\n## Environments\n\nThe ostrich environment can be found [here](https://github.com/vittorione94/ostrichrl) and is installed automatically via poetry.\n\nThe arm-environment [warmup](https://github.com/P-Schumacher/warmup) is also automatically installed by poetry and can be used like any other gym environment:\n\n```\nimport gym\nimport warmup\n\nenv = gym.make("humanreacher-v0")\n\nfor ep in range(5):\n     ep_steps = 0\n     state = env.reset()\n     while True:\n         next_state, reward, done, info = env.step(env.action_space.sample())\n         env.render()\n         if done or (ep_steps >= env.max_episode_steps):\n             break\n         ep_steps += 1\n\n```\n\nThe humanoid environments were simulated with [SCONE](https://scone.software/doku.php?id=start). A ready-to-use RL package will be released in cooperation with GOATSTREAM at a later date.\n\n## Source Code Installation\n\nWe recommend an installation with [poetry](https://python-poetry.org/) to ensure reproducibility.\nWhile [TonicRL](https://github.com/fabiopardo/tonic) with PyTorch is used for the RL algorithms, DEP itself is implemented in JAX. We *strongly* recommend GPU-usage to speed up the computation of DEP. On systems without GPUs, give the tensorflow version of TonicRL a try! We alternatively provide a pip_requirements file.\n1. Make sure to install poetry and deactivate all virtual environments.\n2. Clone the environment\n```\ngit clone https://github.com/martius-lab/depRL\n```\n\n3. Go to the root folder and run\n```\npoetry install\npoetry shell\n```\n\nThat\'s it!\n\nThe build has been tested with:\n```\nUbuntu 20.04 and Ubuntu 22.04\nCUDA 12.0\npoetry 1.4.0\n```\n### Troubleshooting\n* A common error with poetry is a faulty interaction with the python keyring, resulting in a `Failed to unlock the collection!`-error. It could also happen that the dependency solving takes very long (more than 60s), this is caused by the same error.\n  If it happens, try to append\n```\nexport PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring\n```\nto your bashrc. You can also try to prepend it to the poetry command: `PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring poetry install`.\n* If you have an error related to your `ptxas` version, this means that your cuda environment is not setup correctly and you should install the cuda-toolkit. The easiest way is to do this via conda if you don\'t have admin rights on your workstation.\n  I recommend running\n```\nconda install -c conda-forge cudatoolkit-dev\n```\n* In any other case, first try to delete the `poetry.lock` file and the virtual env `.venv`, then run `poetry install` again.\n\n\nFeel free to open an issue if you encounter any problems.\n\n## Citation\n\nPlease use the following citation if you make use of our work:\n\n```\n@inproceedings{schumacher2023:deprl,\n  title = {DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems},\n  author = {Schumacher, Pierre and Haeufle, Daniel F.B. and B{\\"u}chler, Dieter and Schmitt, Syn and Martius, Georg},\n  booktitle = {Proceedings of the Eleventh International Conference on Learning Representations (ICLR)},\n  month = may,\n  year = {2023},\n  doi = {},\n  url = {https://openreview.net/forum?id=C-xa_D3oTj6},\n  month_numeric = {5}\n}\n```\n',
+    'long_description': '# DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems\n\n This repo contains the code for the paper [DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems](https://openreview.net/forum?id=C-xa_D3oTj6) paper, published at ICLR 2023 with perfect review scores (8, 8, 8, 10) and a notable-top-25% rating. See [here](https://sites.google.com/view/dep-rl) for videos.\n\nThe work was performed by Pierre Schumacher, Daniel F.B. Haeufle, Dieter Büchler, Syn Schmitt and Georg Martius.\n\nIf you just want to see the code for DEP, take a look at `deprl/dep_controller.py`, `deprl/custom_agents.py` and `deprl/env_wrapper/wrappers.py`\n\n<p align="center">\n<img src=https://user-images.githubusercontent.com/24903880/229783811-44c422e9-3cc3-42e4-b657-d21be9af6458.gif width=250>\n<img src=https://user-images.githubusercontent.com/24903880/229783729-d068e87c-cb0b-43c7-91d5-ff2ba836f05b.gif width=214>\n\n <img src=https://user-images.githubusercontent.com/24903880/229783370-ee95b9c3-06a0-4ef3-9b60-78e88c4eae38.gif width=214>\n</p>\n\n\n### MyoLeg\nIf you are coming here for the MyoLeg, take a look at this [tutorial](https://github.com/facebookresearch/myosuite/blob/main/docs/source/tutorials.rst#load-dep-rl-baseline). It will show you how to run the pre-trained baseline. We also explain how to train the walking agent in the MyoSuite  [documentation](https://myosuite.readthedocs.io/en/latest/baselines.html#dep-rl-baseline).  \n<p align="center">\n<img src=https://github.com/martius-lab/depRL/assets/24903880/d06200ae-ad35-484c-9d55-83b5235269bc width=350\n</p>\n\n## Abstract\nMuscle-actuated organisms are capable of learning an unparalleled diversity of\ndexterous movements despite their vast amount of muscles. Reinforcement learning (RL) on large musculoskeletal models, however, has not been able to show\nsimilar performance. We conjecture that ineffective exploration in large overactuated action spaces is a key problem. This is supported by our finding that common\nexploration noise strategies are inadequate in synthetic examples of overactuated\nsystems. We identify differential extrinsic plasticity (DEP), a method from the\ndomain of self-organization, as being able to induce state-space covering exploration within seconds of interaction. By integrating DEP into RL, we achieve fast\nlearning of reaching and locomotion in musculoskeletal systems, outperforming\ncurrent approaches in all considered tasks in sample efficiency and robustness.\n\n\n## Installation\n\nWe provide a python package for easy installation:\n```\npip install deprl\n```\nIf you would like to use `jax` with CUDA support, which significantly speeds up learning, we recommend running:\n```\npip install --upgrade "jax[cuda12_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html\n```\nor similar afterwards.\n\nThe humanreacher environment can be installed with\n```\npip install git+https://github.com/P-Schumacher/warmup.git\n```\n\nOstrichRL can be installed from [here](https://github.com/vittorione94/ostrichrl).\n\n\n## Experiments\n\nThe major experiments (humanreacher reaching and ostrich running) can be repeated with the config files.\nSimply run from the root folder:\n```\npython -m deprl.main experiments/ostrich_running_dep.json\npython -m deprl.main experiments/humanreacher.json\n```\nto train an agent. Model checkpoints will be saved in the `output` directory.\nThe progress can be monitored with:\n```\npython -m tonic.plot --path output/folder/\n```\n\nTo execute a trained policy, use:\n\n```\npython -m deprl.play --path output/folder/\n```\n\nSee the [TonicRL](https://github.com/fabiopardo/tonic) documentation for details.\n\nBe aware that ostrich training can be seed-dependant, as seen in the plots of the original publication.\n\n## Pure DEP\nIf you want to see pure DEP in action, just run the following bash files after installing the ostrichrl and warmup environments.\n```\nbash play_files/play_dep_humanreacher.sh\nbash play_files/play_dep_ostrich.sh\nbash play_files/play_dep_dmcontrol_quadruped.sh\n```\n\nYou might see a more interesting ostrich behavior by disabling episode resets in the ostrich environment first.\n## Environments\n\nThe ostrich environment can be found [here](https://github.com/vittorione94/ostrichrl) and is installed automatically via poetry.\n\nThe arm-environment [warmup](https://github.com/P-Schumacher/warmup) is also automatically installed by poetry and can be used like any other gym environment:\n\n```\nimport gym\nimport warmup\n\nenv = gym.make("humanreacher-v0")\n\nfor ep in range(5):\n     ep_steps = 0\n     state = env.reset()\n     while True:\n         next_state, reward, done, info = env.step(env.action_space.sample())\n         env.render()\n         if done or (ep_steps >= env.max_episode_steps):\n             break\n         ep_steps += 1\n\n```\n\nThe humanoid environments were simulated with [SCONE](https://scone.software/doku.php?id=start). A ready-to-use RL package will be released in cooperation with GOATSTREAM at a later date.\n\n## Source Code Installation\n\nWe recommend an installation with [poetry](https://python-poetry.org/) to ensure reproducibility.\nWhile [TonicRL](https://github.com/fabiopardo/tonic) with PyTorch is used for the RL algorithms, DEP itself is implemented in JAX. We *strongly* recommend GPU-usage to speed up the computation of DEP. On systems without GPUs, give the tensorflow version of TonicRL a try! We alternatively provide a pip_requirements file.\n1. Make sure to install poetry and deactivate all virtual environments.\n2. Clone the environment\n```\ngit clone https://github.com/martius-lab/depRL\n```\n\n3. Go to the root folder and run\n```\npoetry install\npoetry shell\n```\n\nThat\'s it!\n\nThe build has been tested with:\n```\nUbuntu 20.04 and Ubuntu 22.04\nCUDA 12.0\npoetry 1.4.0\n```\n### Troubleshooting\n* A common error with poetry is a faulty interaction with the python keyring, resulting in a `Failed to unlock the collection!`-error. It could also happen that the dependency solving takes very long (more than 60s), this is caused by the same error.\n  If it happens, try to append\n```\nexport PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring\n```\nto your bashrc. You can also try to prepend it to the poetry command: `PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring poetry install`.\n* If you have an error related to your `ptxas` version, this means that your cuda environment is not setup correctly and you should install the cuda-toolkit. The easiest way is to do this via conda if you don\'t have admin rights on your workstation.\n  I recommend running\n```\nconda install -c conda-forge cudatoolkit-dev\n```\n* In any other case, first try to delete the `poetry.lock` file and the virtual env `.venv`, then run `poetry install` again.\n\n\nFeel free to open an issue if you encounter any problems.\n\n## Citation\n\nPlease use the following citation if you make use of our work:\n\n```\n@inproceedings{schumacher2023:deprl,\n  title = {DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems},\n  author = {Schumacher, Pierre and Haeufle, Daniel F.B. and B{\\"u}chler, Dieter and Schmitt, Syn and Martius, Georg},\n  booktitle = {Proceedings of the Eleventh International Conference on Learning Representations (ICLR)},\n  month = may,\n  year = {2023},\n  doi = {},\n  url = {https://openreview.net/forum?id=C-xa_D3oTj6},\n  month_numeric = {5}\n}\n```\n',
     'author': 'Pierre Schumacher',
     'author_email': 'pierre.schumacher@tuebingen.mpg.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `deprl-0.1.0/PKG-INFO` & `deprl-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprl
-Version: 0.1.0
+Version: 0.1.1
 Summary: DEP-RL, a method for robust control of musculoskeletal systems.
 License: MIT
 Author: Pierre Schumacher
 Author-email: pierre.schumacher@tuebingen.mpg.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,14 +34,20 @@
 <img src=https://user-images.githubusercontent.com/24903880/229783811-44c422e9-3cc3-42e4-b657-d21be9af6458.gif width=250>
 <img src=https://user-images.githubusercontent.com/24903880/229783729-d068e87c-cb0b-43c7-91d5-ff2ba836f05b.gif width=214>
 
  <img src=https://user-images.githubusercontent.com/24903880/229783370-ee95b9c3-06a0-4ef3-9b60-78e88c4eae38.gif width=214>
 </p>
 
 
+### MyoLeg
+If you are coming here for the MyoLeg, take a look at this [tutorial](https://github.com/facebookresearch/myosuite/blob/main/docs/source/tutorials.rst#load-dep-rl-baseline). It will show you how to run the pre-trained baseline. We also explain how to train the walking agent in the MyoSuite  [documentation](https://myosuite.readthedocs.io/en/latest/baselines.html#dep-rl-baseline).  
+<p align="center">
+<img src=https://github.com/martius-lab/depRL/assets/24903880/d06200ae-ad35-484c-9d55-83b5235269bc width=350
+</p>
+
 ## Abstract
 Muscle-actuated organisms are capable of learning an unparalleled diversity of
 dexterous movements despite their vast amount of muscles. Reinforcement learning (RL) on large musculoskeletal models, however, has not been able to show
 similar performance. We conjecture that ineffective exploration in large overactuated action spaces is a key problem. This is supported by our finding that common
 exploration noise strategies are inadequate in synthetic examples of overactuated
 systems. We identify differential extrinsic plasticity (DEP), a method from the
 domain of self-organization, as being able to induce state-space covering exploration within seconds of interaction. By integrating DEP into RL, we achieve fast
```

