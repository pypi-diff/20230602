# Comparing `tmp/ab-test-simulator-0.0.5.tar.gz` & `tmp/ab-test-simulator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-simulator-0.0.5.tar", last modified: Fri Jun  2 10:30:55 2023, max compression
+gzip compressed data, was "ab-test-simulator-0.0.6.tar", last modified: Fri Jun  2 12:56:48 2023, max compression
```

## Comparing `ab-test-simulator-0.0.5.tar` & `ab-test-simulator-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 10:30:55.972609 ab-test-simulator-0.0.5/
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.5/LICENSE
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.5/MANIFEST.in
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-02 10:30:55.972505 ab-test-simulator-0.0.5/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     5020 2023-06-01 14:37:46.000000 ab-test-simulator-0.0.5/README.md
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 10:30:55.971457 ab-test-simulator-0.0.5/ab_test_simulator/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-02 10:25:40.000000 ab-test-simulator-0.0.5/ab_test_simulator/__init__.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     3946 2023-06-02 10:25:40.000000 ab-test-simulator-0.0.5/ab_test_simulator/_modidx.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2198 2023-06-02 10:25:40.000000 ab-test-simulator-0.0.5/ab_test_simulator/generator.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     5848 2023-06-02 10:25:40.000000 ab-test-simulator-0.0.5/ab_test_simulator/plotting.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7904 2023-06-02 10:25:40.000000 ab-test-simulator-0.0.5/ab_test_simulator/power.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      525 2023-06-02 10:25:40.000000 ab-test-simulator-0.0.5/ab_test_simulator/wrappers.py
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 10:30:55.972326 ab-test-simulator-0.0.5/ab_test_simulator.egg-info/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-02 10:30:55.000000 ab-test-simulator-0.0.5/ab_test_simulator.egg-info/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      516 2023-06-02 10:30:55.000000 ab-test-simulator-0.0.5/ab_test_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-02 10:30:55.000000 ab-test-simulator-0.0.5/ab_test_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       77 2023-06-02 10:30:55.000000 ab-test-simulator-0.0.5/ab_test_simulator.egg-info/entry_points.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-05-31 12:40:20.000000 ab-test-simulator-0.0.5/ab_test_simulator.egg-info/not-zip-safe
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-02 10:30:55.000000 ab-test-simulator-0.0.5/ab_test_simulator.egg-info/requires.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       18 2023-06-02 10:30:55.000000 ab-test-simulator-0.0.5/ab_test_simulator.egg-info/top_level.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1054 2023-06-02 10:30:53.000000 ab-test-simulator-0.0.5/settings.ini
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-02 10:30:55.972646 ab-test-simulator-0.0.5/setup.cfg
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-01 06:53:26.000000 ab-test-simulator-0.0.5/setup.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 12:56:48.584619 ab-test-simulator-0.0.6/
+-rw-rw-r--   0 koljakleineberg   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.6/LICENSE
+-rw-rw-r--   0 koljakleineberg   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.6/MANIFEST.in
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-02 12:56:48.584507 ab-test-simulator-0.0.6/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     5020 2023-06-01 14:37:46.000000 ab-test-simulator-0.0.6/README.md
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 12:56:48.583135 ab-test-simulator-0.0.6/ab_test_simulator/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/__init__.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     4224 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/_modidx.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     3080 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/generator.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     5848 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/plotting.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7904 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/power.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      525 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/wrappers.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 12:56:48.584329 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      516 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       77 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/entry_points.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-05-31 12:40:20.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/not-zip-safe
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/requires.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       18 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/top_level.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1054 2023-06-02 12:56:21.000000 ab-test-simulator-0.0.6/settings.ini
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-02 12:56:48.584655 ab-test-simulator-0.0.6/setup.cfg
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-01 06:53:26.000000 ab-test-simulator-0.0.6/setup.py
```

### Comparing `ab-test-simulator-0.0.5/LICENSE` & `ab-test-simulator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.5/PKG-INFO` & `ab-test-simulator-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-simulator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple library to simulate AB tests.
 Home-page: https://github.com/k111git/ab-test-simulator
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-simulator
```

### Comparing `ab-test-simulator-0.0.5/README.md` & `ab-test-simulator-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.5/ab_test_simulator/_modidx.py` & `ab-test-simulator-0.0.6/ab_test_simulator/_modidx.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,16 @@
                 'doc_host': 'https://k111git.github.io',
                 'git_url': 'https://github.com/k111git/ab-test-simulator',
                 'lib_path': 'ab_test_simulator'},
   'syms': { 'ab_test_simulator.generator': { 'ab_test_simulator.generator.data_to_contingency': ( 'data_generation.html#data_to_contingency',
                                                                                                   'ab_test_simulator/generator.py'),
                                              'ab_test_simulator.generator.generate_binary_data': ( 'data_generation.html#generate_binary_data',
                                                                                                    'ab_test_simulator/generator.py'),
+                                             'ab_test_simulator.generator.generate_contingency': ( 'data_generation.html#generate_contingency',
+                                                                                                   'ab_test_simulator/generator.py'),
                                              'ab_test_simulator.generator.generate_continuous_data': ( 'data_generation.html#generate_continuous_data',
                                                                                                        'ab_test_simulator/generator.py')},
             'ab_test_simulator.plotting': { 'ab_test_simulator.plotting.plot_betas': ( 'plotting.html#plot_betas',
                                                                                        'ab_test_simulator/plotting.py'),
                                             'ab_test_simulator.plotting.plot_binary_power': ( 'plotting.html#plot_binary_power',
                                                                                               'ab_test_simulator/plotting.py'),
                                             'ab_test_simulator.plotting.plot_continuous_power': ( 'plotting.html#plot_continuous_power',
```

### Comparing `ab-test-simulator-0.0.5/ab_test_simulator/generator.py` & `ab-test-simulator-0.0.6/ab_test_simulator/generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_data_generation.ipynb.
 
 # %% auto 0
-__all__ = ['generate_binary_data', 'generate_continuous_data', 'data_to_contingency']
+__all__ = ['generate_binary_data', 'generate_continuous_data', 'data_to_contingency', 'generate_contingency']
 
 # %% ../nbs/00_data_generation.ipynb 4
 import numpy as np
 from scipy.stats import binom
 import pandas as pd
 
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 import plotly.figure_factory as ff
 
+from scipy.stats import binom
+
 # %% ../nbs/00_data_generation.ipynb 6
 def generate_binary_data(N=1000, cr0=0.010, cr1=0.011, split=0.5):
     """
     Generates synthethic data for a binary experiement with two groups (0: Control, 1: Variant).
     Inputs:
     N: Sample size (total number of users)
     Split: % of users assigned randomly to the variant (group 1)
@@ -56,7 +58,29 @@
     """
     df_result = df.groupby("group").agg(
         users=("target", "size"), converted=("target", "sum")
     )
     df_result["not_converted"] = df_result["users"] - df_result["converted"]
     df_result["cvr"] = df_result["converted"] / df_result["users"]
     return df_result
+
+# %% ../nbs/00_data_generation.ipynb 11
+def generate_contingency(N=1000, split=0.50, cr0=0.010, cr1=0.011):
+    """
+    Generate contingency table using binominal distribution
+    """
+    assert N > 5, "N need to be more than 5"
+    assert split >= 0.01, "Split needs to be >= 1%"
+    assert split <= 0.99, "Split needs to be <= 99%"
+    while True:
+        n1 = binom.rvs(N, split, loc=0, size=1)[0]
+        if n1 < N and n1 > 0:
+            break
+    n0 = N - n1
+    c0 = binom.rvs(n0, cr0, loc=0, size=1)[0]
+    c1 = binom.rvs(n1, cr1, loc=0, size=1)[0]
+    df_result = pd.DataFrame(
+        {"group": [0, 1], "users": [n0, n1], "converted": [c0, c1]}
+    )
+    df_result["not_converted"] = df_result["users"] - df_result["converted"]
+    df_result["cvr"] = df_result["converted"] / df_result["users"]
+    return df_result
```

### Comparing `ab-test-simulator-0.0.5/ab_test_simulator/plotting.py` & `ab-test-simulator-0.0.6/ab_test_simulator/plotting.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.5/ab_test_simulator/power.py` & `ab-test-simulator-0.0.6/ab_test_simulator/power.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.5/ab_test_simulator/wrappers.py` & `ab-test-simulator-0.0.6/ab_test_simulator/wrappers.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.5/ab_test_simulator.egg-info/PKG-INFO` & `ab-test-simulator-0.0.6/ab_test_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-simulator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple library to simulate AB tests.
 Home-page: https://github.com/k111git/ab-test-simulator
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-simulator
```

### Comparing `ab-test-simulator-0.0.5/ab_test_simulator.egg-info/SOURCES.txt` & `ab-test-simulator-0.0.6/ab_test_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.5/settings.ini` & `ab-test-simulator-0.0.6/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-simulator
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_simulator
```

### Comparing `ab-test-simulator-0.0.5/setup.py` & `ab-test-simulator-0.0.6/setup.py`

 * *Files identical despite different names*

