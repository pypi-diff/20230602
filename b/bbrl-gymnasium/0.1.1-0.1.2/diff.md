# Comparing `tmp/bbrl_gymnasium-0.1.1.tar.gz` & `tmp/bbrl_gymnasium-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrl_gymnasium-0.1.1.tar", last modified: Fri May 26 14:15:00 2023, max compression
+gzip compressed data, was "bbrl_gymnasium-0.1.2.tar", last modified: Fri Jun  2 06:33:35 2023, max compression
```

## Comparing `bbrl_gymnasium-0.1.1.tar` & `bbrl_gymnasium-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:15:00.012598 bbrl_gymnasium-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:15:00.008598 bbrl_gymnasium-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:15:00.008598 bbrl_gymnasium-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 14:15:00.012598 bbrl_gymnasium-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:15:00.008598 bbrl_gymnasium-0.1.1/bbrl_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 14:14:59.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:15:00.012598 bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/continuous_2D_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5895 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/continuous_cartpole.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/continuous_line_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/debug_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/line_mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/maze_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/rocket_lander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:15:00.012598 bbrl_gymnasium-0.1.1/bbrl_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:15:00.008598 bbrl_gymnasium-0.1.1/bbrl_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 14:14:59.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-26 14:15:00.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:14:59.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 14:14:59.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 14:14:59.000000 bbrl_gymnasium-0.1.1/bbrl_gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-05-26 14:15:00.012598 bbrl_gymnasium-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:15:00.012598 bbrl_gymnasium-0.1.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/tests/test_bbrl_gym.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/tests/test_maze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-05-26 14:14:45.000000 bbrl_gymnasium-0.1.1/tests/test_rocket_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:33:35.615584 bbrl_gymnasium-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:33:35.611584 bbrl_gymnasium-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:33:35.615584 bbrl_gymnasium-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-02 06:33:35.615584 bbrl_gymnasium-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:33:35.615584 bbrl_gymnasium-0.1.2/bbrl_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 06:33:35.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:33:35.615584 bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/continuous_2D_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5895 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/continuous_cartpole.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/continuous_line_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/debug_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/line_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/maze_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/rocket_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:33:35.615584 bbrl_gymnasium-0.1.2/bbrl_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:33:35.615584 bbrl_gymnasium-0.1.2/bbrl_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-02 06:33:35.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-02 06:33:35.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:33:35.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 06:33:35.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 06:33:35.000000 bbrl_gymnasium-0.1.2/bbrl_gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-06-02 06:33:35.615584 bbrl_gymnasium-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:33:35.615584 bbrl_gymnasium-0.1.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/tests/test_bbrl_gym.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/tests/test_maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-06-02 06:32:55.000000 bbrl_gymnasium-0.1.2/tests/test_rocket_lander.py
```

### Comparing `bbrl_gymnasium-0.1.1/.github/workflows/python-publish.yml` & `bbrl_gymnasium-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/LICENSE` & `bbrl_gymnasium-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/Makefile` & `bbrl_gymnasium-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/PKG-INFO` & `bbrl_gymnasium-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl_gymnasium
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.1/README.md` & `bbrl_gymnasium-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/__init__.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/continuous_2D_mdp.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/continuous_2D_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/continuous_cartpole.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/continuous_cartpole.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/continuous_line_mdp.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/continuous_line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/debug_env.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/debug_env.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/line_mdp.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/maze_mdp.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/maze_mdp.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         self.set_render_func(partial(self.init_draw, self.title))
 
     def set_title(self, title):
         self.title = title
 
     def set_render_func(self, render_func: Callable, *args, **kwargs):
         """Sets the render mode"""
-        self.render_func = partial(render_func, *args, **kwargs, mode=self.render_mode)
+        kwargs = {**kwargs, "mode": self.render_mode}
+        self.render_func = partial(render_func, *args, **kwargs)
 
     def seed(self, seed=None):
         self.np_random, seed = seeding.np_random(seed)
         return [seed]
 
     def step(self, action):
         next_state, reward, done, info = self.mdp.step(action)
@@ -77,32 +78,41 @@
 
     def reset(self, **kwargs):
         r = self.mdp.reset(**kwargs)
         if isinstance(r, list):
             return r
         return self.mdp.reset(**kwargs), {}
 
+    def _draw(self, recorder, callable, *args, **kwargs):
+        """Draw and record 
+
+        :param recorder: A video recorder (or None)
+        """
+        if recorder is not None:
+            if recorder.enabled:
+                self.set_render_func(callable, *args, **kwargs)
+                recorder.capture_frame()
+        else:
+            return callable(*args, **kwargs)
+
     # Drawing functions
-    def draw_v_pi_a(self, v, policy, agent_pos, title="MDP studies", mode="legacy"):
-        return self.mdp.render(v, policy, agent_pos, title, mode=mode)
+    def draw_v_pi_a(self, v, policy, agent_pos, title="MDP studies", mode="legacy", recorder=None):
+        return self._draw(recorder, self.render, v, policy, agent_pos, title=title, mode=mode)
+
+    def draw_v_pi(self, v, policy, title="MDP studies", mode="legacy", recorder=None):
+        return self._draw(recorder, self.mdp.render, v, policy, None, title, mode=mode)
+
+    def draw_v(self, v, mode="legacy", title="MDP studies", recorder=None):
+        return self._draw(recorder, self.mdp.render, v, None, None, title, mode=mode)
 
-    def draw_v_pi(self, v, policy, title="MDP studies", mode="legacy"):
-        agent_pos = None
-        return self.mdp.render(v, policy, agent_pos, title, mode=mode)
-
-    def draw_v(self, v, mode="legacy", title="MDP studies"):
-        return self.mdp.render(v, None, None, title, mode=mode)
-
-    def draw_pi(self, policy, title="MDP studies", mode="legacy"):
-        v = None
-        agent_pos = None
-        return self.mdp.render(v, policy, agent_pos, title, mode=mode)
+    def draw_pi(self, policy, title="MDP studies", mode="legacy", recorder=None):
+        return self._draw(recorder, self.mdp.render, None, policy, None, title, mode=mode)
 
-    def init_draw(self, title, mode="legacy"):
-        return self.mdp.new_render(title, mode=mode)
+    def init_draw(self, title, mode="legacy", recorder=None):
+        return self._draw(recorder, self.mdp.new_render, title, mode=mode)
 
     def render(self):
         return self.render_func(mode=self.render_mode)
 
     def render_mdp(self, func, *args, **kwargs):
         self.set_render_func = partial(func, *args, **kwargs)
         self.render()
```

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/envs/rocket_lander.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/envs/rocket_lander.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium.egg-info/PKG-INFO` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl-gymnasium
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.1/bbrl_gymnasium.egg-info/SOURCES.txt` & `bbrl_gymnasium-0.1.2/bbrl_gymnasium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/setup.py` & `bbrl_gymnasium-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/tests/test_bbrl_gym.py` & `bbrl_gymnasium-0.1.2/tests/test_bbrl_gym.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.1/tests/test_maze.py` & `bbrl_gymnasium-0.1.2/tests/test_maze.py`

 * *Files identical despite different names*

