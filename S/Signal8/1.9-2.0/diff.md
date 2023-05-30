# Comparing `tmp/Signal8-1.9.tar.gz` & `tmp/Signal8-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-1.9.tar", last modified: Tue May 30 21:07:16 2023, max compression
+gzip compressed data, was "Signal8-2.0.tar", last modified: Tue May 30 22:42:50 2023, max compression
```

## Comparing `Signal8-1.9.tar` & `Signal8-2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 21:07:16.093798 Signal8-1.9/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.9/LICENSE
--rw-rw-rw-   0        0        0     4356 2023-05-30 21:07:16.084627 Signal8-1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3868 2023-05-22 23:14:08.000000 Signal8-1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 21:07:15.965630 Signal8-1.9/Signal8/
--rw-rw-rw-   0        0        0     9650 2023-05-30 20:36:11.000000 Signal8-1.9/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.9/Signal8/__init__.py
--rw-rw-rw-   0        0        0      225 2023-05-30 20:54:02.000000 Signal8-1.9/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:07:16.079629 Signal8-1.9/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.9/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5746 2023-05-30 18:28:08.000000 Signal8-1.9/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     4265 2023-05-30 17:26:10.000000 Signal8-1.9/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.9/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12606 2023-05-30 19:27:51.000000 Signal8-1.9/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:07:16.044627 Signal8-1.9/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4356 2023-05-30 21:07:15.000000 Signal8-1.9/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-30 21:07:15.000000 Signal8-1.9/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 21:07:15.000000 Signal8-1.9/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 21:07:15.000000 Signal8-1.9/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 21:07:16.093798 Signal8-1.9/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-05-30 21:07:07.000000 Signal8-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:42:50.324783 Signal8-2.0/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.0/LICENSE
+-rw-rw-rw-   0        0        0     4356 2023-05-30 22:42:50.322956 Signal8-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3868 2023-05-22 23:14:08.000000 Signal8-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 22:42:50.242956 Signal8-2.0/Signal8/
+-rw-rw-rw-   0        0        0     9975 2023-05-30 22:42:04.000000 Signal8-2.0/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.0/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-05-30 22:27:03.000000 Signal8-2.0/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:42:50.314957 Signal8-2.0/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.0/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5746 2023-05-30 18:28:08.000000 Signal8-2.0/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     4265 2023-05-30 17:26:10.000000 Signal8-2.0/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.0/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12606 2023-05-30 19:27:51.000000 Signal8-2.0/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:42:50.291960 Signal8-2.0/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4356 2023-05-30 22:42:49.000000 Signal8-2.0/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-30 22:42:50.000000 Signal8-2.0/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 22:42:49.000000 Signal8-2.0/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 22:42:49.000000 Signal8-2.0/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 22:42:50.324783 Signal8-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-05-30 22:42:22.000000 Signal8-2.0/setup.py
```

### Comparing `Signal8-1.9/LICENSE` & `Signal8-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-1.9/PKG-INFO` & `Signal8-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.9
+Version: 2.0
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.9/README.md` & `Signal8-2.0/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-1.9/Signal8/Signal8.py` & `Signal8-2.0/Signal8/Signal8.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import copy
 import random
 import logging
 import threading
 import numpy as np
 
 from gymnasium.utils import EzPickle
-from utils.scenario import BaseScenario
-from utils.core import Agent, Goal, Obstacle, World
-from utils.simple_env import SimpleEnv, make_env
-from utils.problems import get_problem, get_problem_list
+from .utils.scenario import BaseScenario
+from .utils.core import Agent, Goal, Obstacle, World
+from .utils.simple_env import SimpleEnv, make_env
+from .utils.problems import get_problem, get_problem_list
+
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(
         self, 
         num_agents=1,
         render_mode="human"):
         
@@ -97,15 +98,15 @@
         obstacle.size = 0.025
         obstacle.movable = True
         self.obstacle_locks += [threading.Lock()]
         obstacle.color = np.array([0.5, 0, 0])
         obstacle.state.p_vel = np.zeros(world.dim_p)
         dynamic_obs_constr = random.choice(temp_dynamic_obs_constr)
         obstacle.state.p_pos = np_random.uniform(*zip(*dynamic_obs_constr))
-        obstacle.action_callback = self.get_scripted_action
+        obstacle.action_callback = self.action_callback
         temp_dynamic_obs_constr.remove(dynamic_obs_constr)
 
     # Reset position of static obstacles, taking leftover entities from goal constraints
     def _reset_static_obstacle(self, world, obstacle, np_random, temp_static_obs_constr):
         obstacle.color = np.array([0.2, 0.2, 0.2])
         obstacle.state.p_vel = np.zeros(world.dim_p)
         static_obs_constr = random.choice(temp_static_obs_constr)
@@ -125,14 +126,16 @@
     # Reset position of obstacles
     def _reset_obstacles(self, world, np_random, leftover_entities):
         temp_static_obs_constr = list(copy.copy(world.static_obstacle_constr))
         temp_static_obs_constr += leftover_entities
         temp_dynamic_obs_constr = list(copy.copy(world.dynamic_obstacle_constr))
         
         num_dynamic_obs = len(temp_dynamic_obs_constr)
+        self.prev_action = {i: np.zeros(world.dim_p) for i in range(num_dynamic_obs)}
+        
         self._match_obstacles_to_problem(world, len(temp_static_obs_constr))
 
         for i, obstacle in enumerate(world.obstacles):
             if i < num_dynamic_obs:
                 self._reset_dynamic_obstacle(world, obstacle, np_random, temp_dynamic_obs_constr)
             else:
                 self._reset_static_obstacle(world, obstacle, np_random, temp_static_obs_constr)
@@ -158,54 +161,65 @@
     
     # Do not need to implement this function
     def reward(self, agent, world):
         return 0
 
     def observation(self, agent, world):
         return np.concatenate((agent.state.p_pos, agent.state.p_vel))
+    
+    # Run a thread for each scripted obstacle
+    def run_scripted_obstacle(self, world, obstacle, obstacle_idx):
+        sensitivity = 5.0
+        while self.scripted_obstacle_running:
+            with self.obstacle_locks[obstacle_idx]:
+                self.logger.debug(f'{obstacle.name} started at size: {obstacle.size}, position: {obstacle.state.p_pos}')
+                action = self.action_callback(obstacle, world)
+                obstacle.action = action * sensitivity
+                obstacle.move()
+                self.logger.debug(f'{obstacle.name} is now: {obstacle.size}, position: {obstacle.state.p_pos}')
+                time.sleep(0.1)
         
-    # TODO: Implement behavior for scripted obstacles
     """
     Disaster Response: Increase size of obstacle to resemble increasing size of fire/flood
     Precision Farming: Move obstacle in a zamboni pattern to resemble the tractor
     """
-    def get_scripted_action(self, obs, world):
+    def action_callback(self, obs, world):
         action = np.zeros(world.dim_p)
         
         problem_name = world.problem_name
+        problem_name = 'precision_farming_0'
         if problem_name == 'disaster_response_0':
             obs.size *= 1.125
         elif problem_name == 'disaster_response_1':
             obs.size *= 1.100
         elif problem_name == 'disaster_response_2':
             obs.size *= 1.150
         elif problem_name == 'disaster_response_3':
             obs.size *= 1.050
-        elif problem_name == 'precision_farming_0':
-            action[0] = +1.0
-        elif problem_name == 'precision_farming_1':
-            action[0] = -1.0
-        elif problem_name == 'precision_farming_2':
-            action[0] = +1.0
-        elif problem_name == 'precision_farming_3':
-            action[0] = -1.0
+        elif problem_name.startswith('precision_farming'):
+            scenario_num = int(problem_name.split('_')[-1])
+            action = self._get_scripted_action(obs, scenario_num)
 
         return action
     
-    # Run a thread for each scripted obstacle
-    def run_scripted_obstacle(self, world, obstacle, obstacle_idx):
-        sensitivity = 5.0
-        while self.scripted_obstacle_running:
-            with self.obstacle_locks[obstacle_idx]:
-                self.logger.debug(f'{obstacle.name} started at size: {obstacle.size}, position: {obstacle.state.p_pos}')
-                action = self.get_scripted_action(obstacle, world)
-                obstacle.action = action * sensitivity
-                obstacle.move()
-                self.logger.debug(f'{obstacle.name} is now: {obstacle.size}, position: {obstacle.state.p_pos}')
-                time.sleep(0.1)
+    def _get_scripted_action(self, obs, scenario):
+        obs_num = int(obs.name.split('_')[-1])
+        action = [+1, 0]
+        
+        if scenario == 0:
+            a=3
+        elif scenario == 1:
+            a=3
+        elif scenario == 2:
+            a=3
+        else:
+            a=3
+        
+        self.prev_action[obs_num] = action
+        return action
 
     # Stop all threads for scripted obstacles
     def _stop_scripted_obstacles(self):
         self.scripted_obstacle_running = False
         for t in self.scripted_obstacle_threads:
             t.join()
         self.scripted_obstacle_threads.clear()
```

### Comparing `Signal8-1.9/Signal8/utils/core.py` & `Signal8-2.0/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.9/Signal8/utils/problems.py` & `Signal8-2.0/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.9/Signal8/utils/simple_env.py` & `Signal8-2.0/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.9/Signal8.egg-info/PKG-INFO` & `Signal8-2.0/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.9
+Version: 2.0
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.9/setup.py` & `Signal8-2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="1.9",
+    version="2.0",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

