# Comparing `tmp/gym_csle_intrusion_response_game-0.2.0.tar.gz` & `tmp/gym_csle_intrusion_response_game-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_intrusion_response_game-0.2.0.tar", last modified: Sun Apr 30 12:37:26 2023, max compression
+gzip compressed data, was "gym_csle_intrusion_response_game-0.2.1.tar", last modified: Wed May 31 11:25:55 2023, max compression
```

## Comparing `gym_csle_intrusion_response_game-0.2.0.tar` & `gym_csle_intrusion_response_game-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/
--rw-rw-r--   0 kim       (1000) kim       (1000)      719 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      713 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1402 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.780772 gym_csle_intrusion_response_game-0.2.0/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.780772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/
--rw-rw-r--   0 kim       (1000) kim       (1000)     1479 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.780772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1841 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.784772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3189 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3258 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2468 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6078 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4599 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2890 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2890 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)      749 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13921 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17161 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12925 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12783 2023-04-18 14:55:10.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    16406 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    52898 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.780772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      719 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1936 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 11:24:24.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      259 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       33 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:25:55.575115 gym_csle_intrusion_response_game-0.2.1/
+-rw-r--r--   0 kimham     (501) staff       (20)      719 2023-05-31 11:25:55.575254 gym_csle_intrusion_response_game-0.2.1/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      713 2023-03-22 11:50:26.000000 gym_csle_intrusion_response_game-0.2.1/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1402 2023-05-31 11:25:55.575898 gym_csle_intrusion_response_game-0.2.1/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2023-03-01 07:00:43.000000 gym_csle_intrusion_response_game-0.2.1/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:25:55.557181 gym_csle_intrusion_response_game-0.2.1/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:25:55.559670 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/
+-rw-r--r--   0 kimham     (501) staff       (20)     1479 2023-04-19 10:43:59.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:22:38.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/__version__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:25:55.562527 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/constants/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-01 07:00:43.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/constants/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1841 2023-04-29 14:20:57.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/constants/constants.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:25:55.568322 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-01 07:00:43.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4096 2023-05-02 14:34:02.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3835 2023-05-02 14:38:37.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2468 2023-03-08 07:57:44.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6078 2023-04-25 09:16:02.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4599 2023-04-25 11:10:22.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2890 2023-03-16 16:16:16.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2890 2023-03-16 16:16:16.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:25:55.572800 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/
+-rw-r--r--   0 kimham     (501) staff       (20)      749 2023-04-19 10:42:34.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    14772 2023-05-24 17:19:50.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
+-rw-r--r--   0 kimham     (501) staff       (20)    18009 2023-05-24 17:19:50.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
+-rw-r--r--   0 kimham     (501) staff       (20)    13736 2023-05-02 15:57:40.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py
+-rw-r--r--   0 kimham     (501) staff       (20)    12783 2023-04-19 06:25:48.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
+-rw-r--r--   0 kimham     (501) staff       (20)    16406 2023-04-29 14:20:16.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:25:55.573934 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/util/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-01 07:00:43.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/util/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    52914 2023-05-02 07:40:07.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:25:55.561944 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      719 2023-05-31 11:25:55.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     1936 2023-05-31 11:25:55.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:25:55.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-05 11:23:52.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      259 2023-05-31 11:25:55.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       33 2023-05-31 11:25:55.000000 gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/PKG-INFO` & `gym_csle_intrusion_response_game-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_intrusion_response_game
-Version: 0.2.0
+Version: 0.2.1
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/pyproject.toml` & `gym_csle_intrusion_response_game-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.2.0/setup.cfg` & `gym_csle_intrusion_response_game-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
-	csle-common>=0.2.0
-	csle-attacker>=0.2.0
-	csle-defender>=0.2.0
-	csle-collector>=0.2.0
+	csle-common>=0.2.1
+	csle-attacker>=0.2.1
+	csle-defender>=0.2.1
+	csle-collector>=0.2.1
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/__init__.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/constants/constants.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,67 @@
-from typing import Dict, Any
-from csle_common.dao.simulation_config.simulation_env_input_config import SimulationEnvInputConfig
+from typing import Dict, Any, List
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.training.random_policy import RandomPolicy
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
 from csle_common.dao.training.ppo_policy import PPOPolicy
 from csle_common.dao.training.tabular_policy import TabularPolicy
-from gym_csle_intrusion_response_game.dao.local_intrusion_response_game_config import LocalIntrusionResponseGameConfig
+from gym_csle_intrusion_response_game.dao.workflow_intrusion_response_game_config \
+    import WorkflowIntrusionResponseGameConfig
+from csle_common.dao.simulation_config.simulation_env_input_config import SimulationEnvInputConfig
 
 
-class IntrusionResponseGameLocalPOMDPAttackerConfig(SimulationEnvInputConfig):
+class WorkflowIntrusionResponsePOMDPAttackerConfig(SimulationEnvInputConfig):
     """
-    DTO class representing the configuration of the local POMDP environment of the attacker for a specific node
-    when facing a static defender strategy
+    DTO representing the configuration of a workflow intrusion response POMDP when the attacker faces a static
+    defender opponent
     """
 
-    def __init__(self, env_name: str, local_intrusion_response_game_config: LocalIntrusionResponseGameConfig,
-                 defender_strategy: Policy):
+    def __init__(self, env_name: str, game_config: WorkflowIntrusionResponseGameConfig,
+                 defender_strategies: List[Policy]):
         """
-        Initializes the DTO
+        Initializes teh DTO
 
-        :param env_name: the environment name
-        :param local_intrusion_response_game_config: The underlying game config
-        :param defender_strategy: the defender's strategy
+        :param env_name: the name of the environment
+        :param game_config: the workflow game configuration
+        :param defender_strategies: the list of defender strategies for the local nodes in the workflow game
         """
         super().__init__()
         self.env_name = env_name
-        self.local_intrusion_response_game_config = local_intrusion_response_game_config
-        self.defender_strategy = defender_strategy
-
-    @staticmethod
-    def from_dict(d: Dict[str, Any]) -> "IntrusionResponseGameLocalPOMDPAttackerConfig":
-        """
-        Converts a dict representation to an instance
-
-        :param d: the dict to convert
-        :return: the created instance
-        """
-        defender_strategy = None
-        parse_functions = [MultiThresholdStoppingPolicy.from_dict, RandomPolicy.from_dict, PPOPolicy.from_dict,
-                           TabularPolicy.from_dict]
-        for parse_fun in parse_functions:
-            try:
-                defender_strategy = parse_fun(d["defender_strategy"])
-                break
-            except Exception:
-                pass
-        if defender_strategy is None:
-            raise ValueError("Could not parse the defender strategy")
-
-        obj = IntrusionResponseGameLocalPOMDPAttackerConfig(
-            local_intrusion_response_game_config=LocalIntrusionResponseGameConfig.from_dict(
-                d["local_intrusion_response_game_config"]),
-            defender_strategy=defender_strategy, env_name=d["env_name"])
-        return obj
+        self.game_config = game_config
+        self.defender_strategies = defender_strategies
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
-        d["local_intrusion_response_game_config"] = self.local_intrusion_response_game_config.to_dict()
-        d["defender_strategy"] = self.defender_strategy.to_dict()
         d["env_name"] = self.env_name
+        d["game_config"] = self.game_config.to_dict()
+        d["defender_strategies"] = list(map(lambda x: x.to_dict(), self.defender_strategies))
         return d
 
-    def __str__(self) -> str:
+    @staticmethod
+    def from_dict(d: Dict[str, Any]) -> "WorkflowIntrusionResponsePOMDPAttackerConfig":
         """
-        :return:  a string representation of the object
+        Converts a dict representation to an instance
+
+        :param d: the dict to convert
+        :return: the created instance
         """
-        return f"local_intrusion_response_game_config: {self.local_intrusion_response_game_config}, " \
-               f"defender_strategy: {self.defender_strategy}," \
-               f"env_name: {self.env_name}"
+        defender_strategies = []
+        parse_functions = [MultiThresholdStoppingPolicy.from_dict, RandomPolicy.from_dict, PPOPolicy.from_dict,
+                           TabularPolicy.from_dict]
+        for strategy in d["defender_strategies"]:
+            for parse_fun in parse_functions:
+                try:
+                    defender_strategy = parse_fun(strategy)
+                    defender_strategies.append(defender_strategy)
+                    break
+                except Exception:
+                    pass
+            if defender_strategies is None:
+                raise ValueError("Could not parse the defender strategy")
+
+        obj = WorkflowIntrusionResponsePOMDPAttackerConfig(
+            env_name=d["env_name"], game_config=WorkflowIntrusionResponseGameConfig.from_dict(d["game_config"]),
+            defender_strategies=defender_strategies)
+        return obj
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,67 @@
-from typing import Dict, Any
-from csle_common.dao.simulation_config.simulation_env_input_config import SimulationEnvInputConfig
+from typing import Dict, Any, List
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.training.random_policy import RandomPolicy
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
 from csle_common.dao.training.ppo_policy import PPOPolicy
 from csle_common.dao.training.tabular_policy import TabularPolicy
-from gym_csle_intrusion_response_game.dao.local_intrusion_response_game_config import LocalIntrusionResponseGameConfig
+from gym_csle_intrusion_response_game.dao.workflow_intrusion_response_game_config \
+    import WorkflowIntrusionResponseGameConfig
+from csle_common.dao.simulation_config.simulation_env_input_config import SimulationEnvInputConfig
 
 
-class IntrusionResponseGameLocalPOMDPDefenderConfig(SimulationEnvInputConfig):
+class WorkflowIntrusionResponsePOMDPDefenderConfig(SimulationEnvInputConfig):
     """
-    DTO class representing the configuration of the local POMDP environment of the defender for a specific node
-    when facing a static attacker strategy
+    DTO representing the configuration of a workflow intrusion response POMDP when the defender faces a static
+    defender opponent
     """
 
-    def __init__(self, env_name: str, local_intrusion_response_game_config: LocalIntrusionResponseGameConfig,
-                 attacker_strategy: Policy):
+    def __init__(self, env_name: str, game_config: WorkflowIntrusionResponseGameConfig,
+                 attacker_strategies: List[Policy]):
         """
-        Initializes the DTO
+        Initializes teh DTO
 
-        :param env_name: the environment name
-        :param local_intrusion_response_game_config: The underlying game config
-        :param attacker_strategy: the attacker's strategy name
+        :param env_name: the name of the environment
+        :param game_config: the workflow game configuration
+        :param attacker_strategies: the list of attacker strategies for the local nodes in the workflow game
         """
         super().__init__()
         self.env_name = env_name
-        self.local_intrusion_response_game_config = local_intrusion_response_game_config
-        self.attacker_strategy = attacker_strategy
-        self.stopping_action = 3
-        self.stopping_zone = 3
-
-    @staticmethod
-    def from_dict(d: Dict[str, Any]) -> "IntrusionResponseGameLocalPOMDPDefenderConfig":
-        """
-        Converts a dict representation to an instance
-
-        :param d: the dict to convert
-        :return: the created instance
-        """
-        attacker_strategy = None
-        parse_functions = [MultiThresholdStoppingPolicy.from_dict, RandomPolicy.from_dict, PPOPolicy.from_dict,
-                           TabularPolicy.from_dict]
-        for parse_fun in parse_functions:
-            try:
-                attacker_strategy = parse_fun(d["attacker_strategy"])
-                break
-            except Exception:
-                pass
-        if attacker_strategy is None:
-            raise ValueError("Could not parse the attacker strategy")
-
-        obj = IntrusionResponseGameLocalPOMDPDefenderConfig(
-            local_intrusion_response_game_config=LocalIntrusionResponseGameConfig.from_dict(
-                d["local_intrusion_response_game_config"]),
-            attacker_strategy=attacker_strategy, env_name=d["env_name"])
-        return obj
+        self.game_config = game_config
+        self.attacker_strategies = attacker_strategies
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
-        d["local_intrusion_response_game_config"] = self.local_intrusion_response_game_config.to_dict()
-        d["attacker_strategy"] = self.attacker_strategy.to_dict()
         d["env_name"] = self.env_name
+        d["game_config"] = self.game_config.to_dict()
+        d["attacker_strategies"] = list(map(lambda x: x.to_dict(), self.attacker_strategies))
         return d
 
-    def __str__(self) -> str:
+    @staticmethod
+    def from_dict(d: Dict[str, Any]) -> "WorkflowIntrusionResponsePOMDPDefenderConfig":
         """
-        :return:  a string representation of the object
+        Converts a dict representation to an instance
+
+        :param d: the dict to convert
+        :return: the created instance
         """
-        return f"local_intrusion_response_game_config: {self.local_intrusion_response_game_config}, " \
-               f"attacker_strategy: {self.attacker_strategy}," \
-               f"env_name: {self.env_name}"
+        attacker_strategies = []
+        parse_functions = [MultiThresholdStoppingPolicy.from_dict, RandomPolicy.from_dict, PPOPolicy.from_dict,
+                           TabularPolicy.from_dict]
+        for strategy in d["attacker_strategies"]:
+            for parse_fun in parse_functions:
+                try:
+                    attacker_strategy = parse_fun(strategy)
+                    attacker_strategies.append(attacker_strategy)
+                    break
+                except Exception:
+                    pass
+            if attacker_strategies is None:
+                raise ValueError("Could not parse the attacker strategy")
+
+        obj = WorkflowIntrusionResponsePOMDPDefenderConfig(
+            env_name=d["env_name"], game_config=WorkflowIntrusionResponseGameConfig.from_dict(d["game_config"]),
+            attacker_strategies=attacker_strategies)
+        return obj
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/__init__.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,37 +39,39 @@
 
         # Setup spaces
         self.observation_space = self.config.local_intrusion_response_game_config.attacker_observation_space()
         self.action_space = self.config.local_intrusion_response_game_config.attacker_action_space()
 
         # Setup static attacker strategy
         self.static_defender_strategy = self.config.defender_strategy
+        self.static_attacker_strategy = self.config.attacker_strategy
 
         # Setup Config
         self.viewer = None
         self.metadata = {
             'render.modes': ['human', 'rgb_array'],
             'video.frames_per_second': 50  # Video rendering speed
         }
 
         # Setup traces
         self.traces = []
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         self.latest_defender_obs = None
+        self.latest_attacker_obs = None
 
         # Reset
         self.reset()
 
         # Get upper bound and random return estimate
         self.upper_bound_return = 0
         self.random_return = 0
         self.attack_return = 0
-        self.upper_bound_return = self.get_upper_bound_return(samples=100)
-        self.random_return = self.get_random_baseline_return(samples=100)
-        self.attack_return = self.get_attack_baseline_return(samples=100)
+        # self.upper_bound_return = self.get_upper_bound_return(samples=100)
+        # self.random_return = self.get_random_baseline_return(samples=100)
+        # self.attack_return = self.get_attack_baseline_return(samples=100)
 
         # Reset
         self.reset()
         super().__init__()
 
     def get_random_baseline_return(self, samples: int = 100) -> float:
         """
@@ -185,31 +187,41 @@
 
         # Check if game is done
         if IntrusionResponseGameUtil.is_local_state_terminal(self.state.state_vector()):
             done = True
 
         if not done:
             # Update the beliefs
-            self.state.a_b = IntrusionResponseGameUtil.next_local_attacker_belief(
-                o=o, a1=a1, a_b=self.state.a_b, pi1=pi1, config=self.config.local_intrusion_response_game_config,
-                a2=a2, s_d=self.state.defender_state(), s_a_prime=self.state.attacker_state(), s_a=s_a)
+            try:
+                self.state.a_b = IntrusionResponseGameUtil.next_local_attacker_belief(
+                    o=o, a1=a1, a_b=self.state.a_b, pi1=pi1, config=self.config.local_intrusion_response_game_config,
+                    a2=a2, s_d=self.state.defender_state(), s_a_prime=self.state.attacker_state(), s_a=s_a)
+                pi2 = np.array(self.static_attacker_strategy.stage_policy(self.latest_attacker_obs))
+                self.state.d_b = IntrusionResponseGameUtil.next_local_defender_belief(
+                    o=o, a1=a1, d_b=self.state.d_b, pi2=pi2, config=self.config.local_intrusion_response_game_config,
+                    a2=a2, s_a=self.state.attacker_state(),
+                    s_d_prime=self.state.defender_state(), s_d=self.state.defender_state())
+            except Exception:
+                pass
 
         # Update time-step
         self.state.t += 1
 
         # Populate info dict
         info[env_constants.ENV_METRICS.STATE] = self.state.state_vector()
         info[env_constants.ENV_METRICS.DEFENDER_ACTION] = a1
         info[env_constants.ENV_METRICS.ATTACKER_ACTION] = a2
         info[env_constants.ENV_METRICS.OBSERVATION] = o
         info[env_constants.ENV_METRICS.TIME_STEP] = self.state.t
 
         # Get observations
         attacker_obs = self.state.attacker_observation()
         defender_obs = self.state.defender_observation()
+        self.latest_defender_obs=defender_obs
+        self.latest_attacker_obs=attacker_obs
 
         # Log trace
         self.trace.defender_rewards.append(r)
         self.trace.attacker_rewards.append(-r)
         self.trace.attacker_actions.append(a2)
         self.trace.defender_actions.append(a1)
         self.trace.infos.append(info)
@@ -236,27 +248,29 @@
         info[env_constants.ENV_METRICS.RETURN] = R
         info[env_constants.ENV_METRICS.TIME_HORIZON] = self.state.t
         info[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = self.upper_bound_return
         info[env_constants.ENV_METRICS.AVERAGE_RANDOM_RETURN] = self.random_return
         info[env_constants.ENV_METRICS.AVERAGE_HEURISTIC_RETURN] = self.attack_return
         return info
 
-    def reset(self, seed: int = 0, soft: bool = False) -> np.ndarray:
+    def reset(self, seed: int = 0, soft: bool = False) -> Tuple[np.ndarray, Dict]:
         """
         Resets the environment state, this should be called whenever step() returns <done>
 
         :return: initial observation
         """
         super().reset(seed=seed)
         self.state.reset()
         if len(self.trace.attacker_rewards) > 0:
             self.traces.append(self.trace)
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         attacker_obs = self.state.attacker_observation()
         defender_obs = self.state.defender_observation()
+        self.latest_defender_obs=defender_obs
+        self.latest_attacker_obs=attacker_obs
         self.trace.attacker_observations.append(attacker_obs)
         self.trace.defender_observations.append(defender_obs)
         info = {}
         return attacker_obs, info
 
     def render(self, mode: str = 'human'):
         """
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,26 +41,28 @@
 
         # Setup spaces
         self.observation_space = self.config.local_intrusion_response_game_config.defender_observation_space()
         self.action_space = self.config.local_intrusion_response_game_config.defender_action_space()
 
         # Setup static attacker strategy
         self.static_attacker_strategy = self.config.attacker_strategy
+        self.static_defender_strategy = self.config.defender_strategy
 
         # Setup Config
         self.viewer = None
         self.metadata = {
             'render.modes': ['human', 'rgb_array'],
             'video.frames_per_second': 50  # Video rendering speed
         }
 
         # Setup traces
         self.traces = []
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         self.latest_attacker_obs = None
+        self.latest_defender_obs = None
         self.latest_attacker_action = None
 
         # Reset
         self.reset()
 
         # Get upper bound and random return estimate
         self.upper_bound_return = 0
@@ -160,33 +162,43 @@
         self.state.s_idx = s_idx_prime
 
         # Check if game is done
         if IntrusionResponseGameUtil.is_local_state_terminal(self.state.state_vector()):
             done = True
 
         if not done:
-            # Update the beliefs
-            self.state.d_b = IntrusionResponseGameUtil.next_local_defender_belief(
-                o=o, a1=a1, d_b=self.state.d_b, pi2=pi2, config=self.config.local_intrusion_response_game_config,
-                a2=a2, s_a=self.state.attacker_state(),
-                s_d_prime=self.state.defender_state(), s_d=s_d)
+            try:
+                # Update the beliefs
+                self.state.d_b = IntrusionResponseGameUtil.next_local_defender_belief(
+                    o=o, a1=a1, d_b=self.state.d_b, pi2=pi2, config=self.config.local_intrusion_response_game_config,
+                    a2=a2, s_a=self.state.attacker_state(),
+                    s_d_prime=self.state.defender_state(), s_d=s_d)
+                pi1 = np.array(self.static_defender_strategy.stage_policy(self.latest_defender_obs))
+                self.state.a_b = IntrusionResponseGameUtil.next_local_attacker_belief(
+                    o=o, a1=a1, a_b=self.state.a_b, pi1=pi1, config=self.config.local_intrusion_response_game_config,
+                    a2=a2, s_d=self.state.defender_state(), s_a_prime=self.state.attacker_state(),
+                    s_a=self.state.attacker_state())
+            except Exception:
+                pass
 
         # Update time-step
         self.state.t += 1
 
         # Populate info dict
         info[env_constants.ENV_METRICS.STATE] = self.state.state_vector()
         info[env_constants.ENV_METRICS.DEFENDER_ACTION] = a1
         info[env_constants.ENV_METRICS.ATTACKER_ACTION] = a2
         info[env_constants.ENV_METRICS.OBSERVATION] = o
         info[env_constants.ENV_METRICS.TIME_STEP] = self.state.t
 
         # Get observations
         attacker_obs = self.state.attacker_observation()
         defender_obs = self.state.defender_observation()
+        self.latest_attacker_obs = attacker_obs
+        self.latest_defender_obs = defender_obs
 
         # Log trace
         self.trace.defender_rewards.append(r)
         self.trace.attacker_rewards.append(-r)
         self.trace.attacker_actions.append(a2)
         self.trace.defender_actions.append(a1)
         self.trace.infos.append(info)
@@ -225,14 +237,16 @@
         super().reset(seed=seed)
         self.state.reset()
         if len(self.trace.attacker_rewards) > 0:
             self.traces.append(self.trace)
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         attacker_obs = self.state.attacker_observation()
         defender_obs = self.state.defender_observation()
+        self.latest_attacker_obs = attacker_obs
+        self.latest_defender_obs = defender_obs
         self.trace.attacker_observations.append(attacker_obs)
         self.trace.defender_observations.append(defender_obs)
         info = {}
         return defender_obs, info
 
     def render(self, mode: str = 'human'):
         """
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,21 +52,23 @@
             S_A=self.config.local_intrusion_response_game_config.S_A,
             a1=a1
         )
 
         # Initialize environment state
         self.s = 0
         self.b = self.config.local_intrusion_response_game_config.d_b1
+        self.a_b = self.config.local_intrusion_response_game_config.a_b1
 
         # Setup spaces
         self.observation_space = self.config.local_intrusion_response_game_config.defender_observation_space_stopping()
         self.action_space = self.config.local_intrusion_response_game_config.defender_action_space_stopping()
 
         # Setup static attacker strategy
         self.static_attacker_strategy = self.config.attacker_strategy
+        self.static_defender_strategy = self.config.defender_strategy
 
         # Setup Config
         self.viewer = None
         self.metadata = {
             'render.modes': ['human', 'rgb_array'],
             'video.frames_per_second': 50  # Video rendering speed
         }
@@ -82,15 +84,16 @@
         self.reset()
 
         # Get upper bound and random return estimate
         self.upper_bound_return = 0
         self.random_return = 0
         self.t = 0
         self.intrusion_length = 0
-        self.upper_bound_return = self.get_upper_bound_return(samples=100)
+        self.upper_bound_return = 0
+        # self.upper_bound_return = self.get_upper_bound_return(samples=100)
 
         # Reset
         self.reset()
         super().__init__()
 
     def step(self, a1: int) -> Tuple[np.ndarray, float, bool, bool, Dict[str, Union[float, int]]]:
         """
@@ -112,14 +115,15 @@
         self.latest_a2 = a2
 
         # Compute the reward
         r = self.R[a1][a2][self.s + 1]
 
         # Sample the next state
         S = np.append([-1], self.config.local_intrusion_response_game_config.S_A)
+        s_a = self.s
         s_idx_prime = IntrusionResponseGameUtil.sample_next_state(
             a1=a1, a2=a2, T=self.T, S=S,
             s_idx=self.s + 1)
 
         # Sample the next observation
         o = IntrusionResponseGameUtil.sample_next_observation(
             Z=self.Z, O=self.config.local_intrusion_response_game_config.O,
@@ -140,14 +144,19 @@
             S = self.config.local_intrusion_response_game_config.S_A
             # Update the beliefs
             self.b = IntrusionResponseGameUtil.next_stopping_belief(
                 o=o, a1=a1, b=self.b, pi2=pi2, S=S, Z=self.Z,
                 O=self.config.local_intrusion_response_game_config.O,
                 T=self.T,
                 A2=self.config.local_intrusion_response_game_config.A2, a2=a2, s=self.s)
+            pi1 = np.array(self.static_defender_strategy.stage_policy(self.latest_defender_obs))
+            self.a_b = IntrusionResponseGameUtil.next_local_attacker_belief(
+                o=o, a1=a1, a_b=self.a_b, pi1=pi1, config=self.config.local_intrusion_response_game_config,
+                a2=a2, s_d=self.zone, s_a_prime=self.s,
+                s_a=s_a)
 
         # Update metrics
         self.t += 1
         if self.s == env_constants.ATTACK_STATES.COMPROMISED:
             self.intrusion_length += 1
 
         # Populate info dict
@@ -160,14 +169,16 @@
         info[env_constants.ENV_METRICS.WEIGHTED_INTRUSION_PREDICTION_DISTANCE] = 0
         info[env_constants.ENV_METRICS.START_POINT_CORRECT] = 0
         info[env_constants.ENV_METRICS.INTRUSION_START] = 0
         info[env_constants.ENV_METRICS.INTRUSION_END] = 0
 
         # Get observations
         defender_obs = self.b
+        self.latest_attacker_obs = [self.s] + list(self.a_b)
+        self.latest_defender_obs = [self.zone] + list(self.b)
 
         # Log trace
         self.trace.defender_rewards.append(r)
         self.trace.attacker_rewards.append(-r)
         self.trace.attacker_actions.append(a2)
         self.trace.defender_actions.append(a1)
         self.trace.infos.append(info)
@@ -232,14 +243,16 @@
         self.intrusion_length = 0
         self.b = self.config.local_intrusion_response_game_config.d_b1
         if len(self.trace.attacker_rewards) > 0:
             self.traces.append(self.trace)
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         attacker_obs = self.b
         defender_obs = self.b
+        self.latest_attacker_obs = [self.s] + list(self.a_b)
+        self.latest_defender_obs = [self.zone] + list(self.b)
         self.trace.attacker_observations.append(attacker_obs)
         self.trace.defender_observations.append(defender_obs)
         info = {}
         return defender_obs, info
 
     def render(self, mode: str = 'human'):
         """
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import iteround
 from scipy.stats import betabinom
 from gym_csle_intrusion_response_game.dao.local_intrusion_response_game_config import LocalIntrusionResponseGameConfig
 import gym_csle_intrusion_response_game.constants.constants as env_constants
 from csle_common.dao.training.policy import Policy
 
 
 class IntrusionResponseGameUtil:
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-intrusion-response-game
-Version: 0.2.0
+Version: 0.2.1
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt` & `gym_csle_intrusion_response_game-0.2.1/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

