# Comparing `tmp/Signal8-2.2.tar.gz` & `tmp/Signal8-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-2.2.tar", last modified: Fri Jun  2 17:12:00 2023, max compression
+gzip compressed data, was "Signal8-2.3.tar", last modified: Fri Jun  2 17:26:37 2023, max compression
```

## Comparing `Signal8-2.2.tar` & `Signal8-2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:12:00.844531 Signal8-2.2/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.2/LICENSE
--rw-rw-rw-   0        0        0     4369 2023-06-02 17:12:00.840531 Signal8-2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 17:12:00.600561 Signal8-2.2/Signal8/
--rw-rw-rw-   0        0        0    11046 2023-06-02 17:11:02.000000 Signal8-2.2/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.2/Signal8/__init__.py
--rw-rw-rw-   0        0        0      238 2023-06-02 17:05:00.000000 Signal8-2.2/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:12:00.834532 Signal8-2.2/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.2/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5811 2023-05-31 18:22:02.000000 Signal8-2.2/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2783 2023-06-01 21:15:18.000000 Signal8-2.2/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     4402 2023-06-02 17:06:17.000000 Signal8-2.2/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.2/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12529 2023-06-02 16:26:33.000000 Signal8-2.2/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.2/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:12:00.765581 Signal8-2.2/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4369 2023-06-02 17:12:00.000000 Signal8-2.2/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-02 17:12:00.000000 Signal8-2.2/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:12:00.000000 Signal8-2.2/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 17:12:00.000000 Signal8-2.2/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 17:12:00.845546 Signal8-2.2/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-02 17:10:41.000000 Signal8-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:26:37.788918 Signal8-2.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.3/LICENSE
+-rw-rw-rw-   0        0        0     4369 2023-06-02 17:26:37.786918 Signal8-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 17:26:37.691919 Signal8-2.3/Signal8/
+-rw-rw-rw-   0        0        0    11040 2023-06-02 17:25:14.000000 Signal8-2.3/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.3/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      238 2023-06-02 17:05:00.000000 Signal8-2.3/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:26:37.781920 Signal8-2.3/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.3/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5811 2023-05-31 18:22:02.000000 Signal8-2.3/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2783 2023-06-01 21:15:18.000000 Signal8-2.3/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     4402 2023-06-02 17:06:17.000000 Signal8-2.3/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.3/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12529 2023-06-02 16:26:33.000000 Signal8-2.3/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.3/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:26:37.747919 Signal8-2.3/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4369 2023-06-02 17:26:37.000000 Signal8-2.3/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-02 17:26:37.000000 Signal8-2.3/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 17:26:37.000000 Signal8-2.3/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 17:26:37.000000 Signal8-2.3/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 17:26:37.788918 Signal8-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-02 17:25:17.000000 Signal8-2.3/setup.py
```

### Comparing `Signal8-2.2/LICENSE` & `Signal8-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-2.2/PKG-INFO` & `Signal8-2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.2
+Version: 2.3
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.2/README.md` & `Signal8-2.3/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-2.2/Signal8/Signal8.py` & `Signal8-2.3/Signal8/Signal8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 import copy
 import random
 import logging
 import threading
 import numpy as np
 
-
 from .utils.npc import NPC
 from .utils.scenario import BaseScenario
 from .utils.core import Agent, Goal, Obstacle, World
 from .utils.simple_env import SimpleEnv, make_env
 from .utils.problems import get_problem, get_problem_list
 
 from gymnasium.utils import EzPickle
@@ -219,15 +218,15 @@
         elif problem_name == 'disaster_response_1':
             obs.size += 0.0075
         elif problem_name == 'disaster_response_2':
             obs.size += 0.01
         elif problem_name == 'disaster_response_3':
             obs.size += 0.0125
         elif problem_name.startswith('precision_farming'):
-            obs_num = int(problem_name.split('_')[-1])
+            obs_num = int(obs.name.split('_')[-1])
             scenario_num = int(problem_name.split('_')[-1])
             action = self.npc[obs_num].get_scripted_action(obs, scenario_num)
 
         return action
 
     # Stop all threads for scripted obstacles
     def stop_scripted_obstacles(self):
```

### Comparing `Signal8-2.2/Signal8/utils/core.py` & `Signal8-2.3/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.2/Signal8/utils/npc.py` & `Signal8-2.3/Signal8/utils/npc.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.2/Signal8/utils/problems.py` & `Signal8-2.3/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.2/Signal8/utils/simple_env.py` & `Signal8-2.3/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.2/Signal8/utils/test_dynamic_obs.py` & `Signal8-2.3/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.2/Signal8.egg-info/PKG-INFO` & `Signal8-2.3/Signal8.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.2
+Version: 2.3
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.2/Signal8.egg-info/SOURCES.txt` & `Signal8-2.3/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-2.2/setup.py` & `Signal8-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="2.2",
+    version="2.3",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

