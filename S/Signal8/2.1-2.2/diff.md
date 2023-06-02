# Comparing `tmp/Signal8-2.1.tar.gz` & `tmp/Signal8-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-2.1.tar", last modified: Thu Jun  1 21:27:53 2023, max compression
+gzip compressed data, was "Signal8-2.2.tar", last modified: Fri Jun  2 17:12:00 2023, max compression
```

## Comparing `Signal8-2.1.tar` & `Signal8-2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 21:27:53.739916 Signal8-2.1/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.1/LICENSE
--rw-rw-rw-   0        0        0     4369 2023-06-01 21:27:53.737916 Signal8-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 21:27:53.602917 Signal8-2.1/Signal8/
--rw-rw-rw-   0        0        0    10986 2023-06-01 21:26:04.000000 Signal8-2.1/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.1/Signal8/__init__.py
--rw-rw-rw-   0        0        0      226 2023-06-01 21:25:31.000000 Signal8-2.1/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:27:53.732920 Signal8-2.1/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.1/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5811 2023-05-31 18:22:02.000000 Signal8-2.1/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2783 2023-06-01 21:15:18.000000 Signal8-2.1/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     4265 2023-05-31 22:48:11.000000 Signal8-2.1/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.1/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12529 2023-06-01 21:21:33.000000 Signal8-2.1/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.1/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:27:53.707917 Signal8-2.1/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4369 2023-06-01 21:27:53.000000 Signal8-2.1/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-01 21:27:53.000000 Signal8-2.1/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 21:27:53.000000 Signal8-2.1/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 21:27:53.000000 Signal8-2.1/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 21:27:53.740918 Signal8-2.1/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-01 21:27:15.000000 Signal8-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:12:00.844531 Signal8-2.2/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.2/LICENSE
+-rw-rw-rw-   0        0        0     4369 2023-06-02 17:12:00.840531 Signal8-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 17:12:00.600561 Signal8-2.2/Signal8/
+-rw-rw-rw-   0        0        0    11046 2023-06-02 17:11:02.000000 Signal8-2.2/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.2/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      238 2023-06-02 17:05:00.000000 Signal8-2.2/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:12:00.834532 Signal8-2.2/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.2/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5811 2023-05-31 18:22:02.000000 Signal8-2.2/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2783 2023-06-01 21:15:18.000000 Signal8-2.2/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     4402 2023-06-02 17:06:17.000000 Signal8-2.2/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.2/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12529 2023-06-02 16:26:33.000000 Signal8-2.2/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.2/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:12:00.765581 Signal8-2.2/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4369 2023-06-02 17:12:00.000000 Signal8-2.2/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-02 17:12:00.000000 Signal8-2.2/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 17:12:00.000000 Signal8-2.2/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 17:12:00.000000 Signal8-2.2/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 17:12:00.845546 Signal8-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-02 17:10:41.000000 Signal8-2.2/setup.py
```

### Comparing `Signal8-2.1/LICENSE` & `Signal8-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-2.1/PKG-INFO` & `Signal8-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.1
+Version: 2.2
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.1/README.md` & `Signal8-2.2/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-2.1/Signal8/Signal8.py` & `Signal8-2.2/Signal8/Signal8.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import time
 import copy
 import random
 import logging
 import threading
 import numpy as np
 
+
 from .utils.npc import NPC
 from .utils.scenario import BaseScenario
 from .utils.core import Agent, Goal, Obstacle, World
 from .utils.simple_env import SimpleEnv, make_env
 from .utils.problems import get_problem, get_problem_list
 
 from gymnasium.utils import EzPickle
 
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(self, num_agents=1, render_mode=None):
         
+        if num_agents > 2:
+            raise ValueError("Signal8 currently can only support up to 2 agents.")
+        
         scenario = Scenario()
         world = scenario.make_world(num_agents)
         
         super().__init__(
             scenario=scenario, 
             world=world, 
             render_mode=render_mode,
@@ -71,28 +75,27 @@
         world.dynamic_obstacle_constr = problem['dynamic_obs']
     
     """
     Returns goal constraints that haven't been selected to be used as an obstacle
     for the precision farming case (i.e., crop that wasn't selected as goal becomes an obstacle)
     """
     def _reset_agents_and_goals(self, world, np_random):
-        temp_goal_constr = list(copy.copy(world.goal_constr))
+        temp_goal_constr = copy.copy(world.goal_constr)
         for i, agent in enumerate(world.agents):
             agent.color = np.array([1, 0.95, 0.8])
             agent.state.p_vel = np.zeros(world.dim_p)
             agent_constr = random.choice(world.start_constr)
             agent.state.p_pos = np_random.uniform(*zip(*agent_constr))
 
             agent.goal_a = world.goals[i]
             agent.goal_a.color = np.array([0.835, 0.90, 0.831])
             agent.goal_a.state.p_vel = np.zeros(world.dim_p)
             goal_constr = random.choice(temp_goal_constr)
             agent.goal_a.state.p_pos = np_random.uniform(*zip(*goal_constr))
-            if world.problem_name.startswith('precision_farming'):
-                temp_goal_constr.remove(goal_constr)
+            temp_goal_constr.remove(goal_constr)
             
             agent.goal_b = world.goals[len(world.goals) - 1 - i]
             agent.goal_b.color = np.array([0.85, 0.90, 0.99])
             agent.goal_b.state.p_vel = np.zeros(world.dim_p)
             agent.goal_b.state.p_pos = copy.copy(agent.state.p_pos)
 
         return temp_goal_constr
@@ -124,17 +127,18 @@
         elif len(world.obstacles) < num_total_obstacles:
             additional_obstacles = [Obstacle() for _ in range(len(world.obstacles), num_total_obstacles)]
             [setattr(obstacle, 'name', f"obs_{i+len(world.obstacles)}") for i, obstacle in enumerate(additional_obstacles)]
             world.obstacles.extend(additional_obstacles)
     
     # Reset position of obstacles
     def _reset_obstacles(self, world, np_random, leftover_entities):
-        temp_static_obs_constr = list(copy.copy(world.static_obstacle_constr))
-        temp_static_obs_constr += leftover_entities
-        temp_dynamic_obs_constr = list(copy.copy(world.dynamic_obstacle_constr))
+        temp_static_obs_constr = copy.copy(world.static_obstacle_constr)
+        if world.problem_name.startswith('precision_farming'):
+            temp_static_obs_constr += leftover_entities
+        temp_dynamic_obs_constr = copy.copy(world.dynamic_obstacle_constr)
         
         num_dynamic_obs = len(temp_dynamic_obs_constr)        
         self._match_obstacles_to_problem(world, len(temp_static_obs_constr))
 
         for i, obstacle in enumerate(world.obstacles):
             if i < num_dynamic_obs:
                 self._reset_dynamic_obstacle(world, obstacle, np_random, temp_dynamic_obs_constr)
@@ -155,16 +159,15 @@
                 
     def reset_world(self, world, np_random, problem_name=None):
         self.npc.clear()
         self.stop_scripted_obstacles()
         self._set_problem_scenario(world, np_random, problem_name)
         leftover_entities = self._reset_agents_and_goals(world, np_random)
         self._reset_obstacles(world, np_random, leftover_entities)
-        if problem_name is not None:
-            self._start_scripted_obstacles(world)
+        self._start_scripted_obstacles(world)
     
     # Reward given by agents to agents for reaching their respective goals
     def reward(self, agent, world):
         return 0
     
     def observation(self, agent, world):
         agent_pos = agent.state.p_pos
```

### Comparing `Signal8-2.1/Signal8/utils/core.py` & `Signal8-2.2/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.1/Signal8/utils/npc.py` & `Signal8-2.2/Signal8/utils/npc.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.1/Signal8/utils/simple_env.py` & `Signal8-2.2/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.1/Signal8/utils/test_dynamic_obs.py` & `Signal8-2.2/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.1/Signal8.egg-info/PKG-INFO` & `Signal8-2.2/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.1
+Version: 2.2
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.1/Signal8.egg-info/SOURCES.txt` & `Signal8-2.2/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-2.1/setup.py` & `Signal8-2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="2.1",
+    version="2.2",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

