# Comparing `tmp/ab-test-simulator-0.0.3.tar.gz` & `tmp/ab-test-simulator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-simulator-0.0.3.tar", last modified: Thu Jun  1 14:41:44 2023, max compression
+gzip compressed data, was "ab-test-simulator-0.0.4.tar", last modified: Fri Jun  2 06:34:32 2023, max compression
```

## Comparing `ab-test-simulator-0.0.3.tar` & `ab-test-simulator-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 14:41:44.814565 ab-test-simulator-0.0.3/
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.3/LICENSE
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.3/MANIFEST.in
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-01 14:41:44.814458 ab-test-simulator-0.0.3/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     5020 2023-06-01 14:37:46.000000 ab-test-simulator-0.0.3/README.md
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 14:41:44.813158 ab-test-simulator-0.0.3/ab_test_simulator/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/__init__.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     3218 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/_modidx.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2198 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/generator.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     3539 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/plotting.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7904 2023-06-01 14:39:35.000000 ab-test-simulator-0.0.3/ab_test_simulator/power.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      475 2023-06-01 14:32:32.000000 ab-test-simulator-0.0.3/ab_test_simulator/wrappers.py
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-01 14:41:44.814254 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      516 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       77 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/entry_points.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-05-31 12:40:20.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/not-zip-safe
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/requires.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       18 2023-06-01 14:41:44.000000 ab-test-simulator-0.0.3/ab_test_simulator.egg-info/top_level.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1054 2023-06-01 14:38:46.000000 ab-test-simulator-0.0.3/settings.ini
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-01 14:41:44.814600 ab-test-simulator-0.0.3/setup.cfg
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-01 06:53:26.000000 ab-test-simulator-0.0.3/setup.py
+drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-02 06:34:32.405079 ab-test-simulator-0.0.4/
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)    11337 2023-05-31 19:02:27.000000 ab-test-simulator-0.0.4/LICENSE
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)      111 2023-05-31 19:02:27.000000 ab-test-simulator-0.0.4/MANIFEST.in
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     7419 2023-06-02 06:34:32.405079 ab-test-simulator-0.0.4/PKG-INFO
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     5020 2023-06-01 21:33:08.000000 ab-test-simulator-0.0.4/README.md
+drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-02 06:34:32.401079 ab-test-simulator-0.0.4/ab_test_simulator/
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       22 2023-06-02 06:30:23.000000 ab-test-simulator-0.0.4/ab_test_simulator/__init__.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     3475 2023-06-02 06:30:23.000000 ab-test-simulator-0.0.4/ab_test_simulator/_modidx.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     2198 2023-06-02 06:30:23.000000 ab-test-simulator-0.0.4/ab_test_simulator/generator.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     4566 2023-06-02 06:30:23.000000 ab-test-simulator-0.0.4/ab_test_simulator/plotting.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     7904 2023-06-02 06:30:23.000000 ab-test-simulator-0.0.4/ab_test_simulator/power.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)      475 2023-06-01 21:33:08.000000 ab-test-simulator-0.0.4/ab_test_simulator/wrappers.py
+drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-02 06:34:32.405079 ab-test-simulator-0.0.4/ab_test_simulator.egg-info/
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     7419 2023-06-02 06:34:32.000000 ab-test-simulator-0.0.4/ab_test_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)      516 2023-06-02 06:34:32.000000 ab-test-simulator-0.0.4/ab_test_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-06-02 06:34:32.000000 ab-test-simulator-0.0.4/ab_test_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       77 2023-06-02 06:34:32.000000 ab-test-simulator-0.0.4/ab_test_simulator.egg-info/entry_points.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-05-31 19:03:37.000000 ab-test-simulator-0.0.4/ab_test_simulator.egg-info/not-zip-safe
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       98 2023-06-02 06:34:32.000000 ab-test-simulator-0.0.4/ab_test_simulator.egg-info/requires.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       18 2023-06-02 06:34:32.000000 ab-test-simulator-0.0.4/ab_test_simulator.egg-info/top_level.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     1054 2023-06-02 06:33:52.000000 ab-test-simulator-0.0.4/settings.ini
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       38 2023-06-02 06:34:32.405079 ab-test-simulator-0.0.4/setup.cfg
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     2711 2023-05-31 19:36:26.000000 ab-test-simulator-0.0.4/setup.py
```

### Comparing `ab-test-simulator-0.0.3/LICENSE` & `ab-test-simulator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.3/PKG-INFO` & `ab-test-simulator-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-simulator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple library to simulate AB tests.
 Home-page: https://github.com/k111git/ab-test-simulator
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-simulator
```

### Comparing `ab-test-simulator-0.0.3/README.md` & `ab-test-simulator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.3/ab_test_simulator/_modidx.py` & `ab-test-simulator-0.0.4/ab_test_simulator/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
                                                                                                   'ab_test_simulator/generator.py'),
                                              'ab_test_simulator.generator.generate_binary_data': ( 'data_generation.html#generate_binary_data',
                                                                                                    'ab_test_simulator/generator.py'),
                                              'ab_test_simulator.generator.generate_continuous_data': ( 'data_generation.html#generate_continuous_data',
                                                                                                        'ab_test_simulator/generator.py')},
             'ab_test_simulator.plotting': { 'ab_test_simulator.plotting.plot_betas': ( 'plotting.html#plot_betas',
                                                                                        'ab_test_simulator/plotting.py'),
+                                            'ab_test_simulator.plotting.plot_binary_power': ( 'plotting.html#plot_binary_power',
+                                                                                              'ab_test_simulator/plotting.py'),
                                             'ab_test_simulator.plotting.plot_distribution': ( 'plotting.html#plot_distribution',
                                                                                               'ab_test_simulator/plotting.py'),
                                             'ab_test_simulator.plotting.plot_power': ( 'plotting.html#plot_power',
                                                                                        'ab_test_simulator/plotting.py')},
             'ab_test_simulator.power': { 'ab_test_simulator.power._compute_sample_size_from_powerline': ( 'power.html#_compute_sample_size_from_powerline',
                                                                                                           'ab_test_simulator/power.py'),
                                          'ab_test_simulator.power.continuous_sample_size': ( 'power.html#continuous_sample_size',
```

### Comparing `ab-test-simulator-0.0.3/ab_test_simulator/generator.py` & `ab-test-simulator-0.0.4/ab_test_simulator/generator.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.3/ab_test_simulator/plotting.py` & `ab-test-simulator-0.0.4/ab_test_simulator/plotting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_plotting.ipynb.
 
 # %% auto 0
-__all__ = ['plot_distribution', 'plot_power', 'plot_betas']
+__all__ = ['plot_distribution', 'plot_power', 'plot_betas', 'plot_binary_power']
 
 # %% ../nbs/03_plotting.ipynb 5
 import numpy as np
 from scipy.stats import binom
 import pandas as pd
 
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 import plotly.figure_factory as ff
 
 from scipy.stats import beta
 
+from .power import sample_size_chi2
+
 # %% ../nbs/03_plotting.ipynb 7
 def plot_distribution(df):
     """
     Plots the distribution for both groups of generate_continuous_data
     """
     fig = ff.create_distplot(
         [
@@ -83,15 +85,15 @@
         yaxis_range=[0, 1],
         legend=dict(yanchor="top", y=1, xanchor="left", x=0.0),
     )
     # fig.update_layout(showlegend=True)
     return fig
 
 # %% ../nbs/03_plotting.ipynb 10
-def plot_betas(df_contingency, xmin=0.0,xmax=0.2, names=["A", "B"]):
+def plot_betas(df_contingency, xmin=0.0, xmax=0.2, names=["A", "B"]):
     """
     Plots two beta distributions, one for control and for variant.
     Takes as input a contigency table as dataframe
     """
     betas = dict()
     for group in [0, 1]:
         betas[group] = beta(
@@ -120,7 +122,44 @@
         template="simple_white",
         xaxis_title="CVR",
         yaxis_title="PDF",
         legend=dict(yanchor="top", y=1, xanchor="left", x=0.0),
     )
 
     return fig
+
+# %% ../nbs/03_plotting.ipynb 11
+def plot_binary_power(cr0=0.01, cr1=0.012, alpha=0.05, one_sided=True):
+    powers = np.arange(0.1, 0.91, 0.1)
+    sizes = []
+    for power in powers:
+        size = sample_size_chi2(
+            cr0=cr0, cr1=cr1, alpha=alpha, power=power, one_sided=one_sided
+        )
+        sizes.append(size)
+        fig = make_subplots()
+
+    fig.add_trace(
+        go.Scatter(
+            x=sizes,
+            y=powers,
+            mode="lines",
+        )
+    )
+
+    fig.add_vline(
+        x=sample_size_chi2(
+            cr0=cr0, cr1=cr1, alpha=alpha, power=0.8, one_sided=one_sided
+        ),
+        line_width=2,
+        line_dash="dash",
+        line_color="gray",
+    )
+
+    fig.update_layout(
+        title="Statistical power vs sample size",
+        template="simple_white",
+        xaxis_title="Sample size per variant",
+        yaxis_title="Power",
+        legend=dict(yanchor="top", y=1, xanchor="left", x=0.0),
+    )
+    return fig
```

### Comparing `ab-test-simulator-0.0.3/ab_test_simulator/power.py` & `ab-test-simulator-0.0.4/ab_test_simulator/power.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.3/ab_test_simulator.egg-info/PKG-INFO` & `ab-test-simulator-0.0.4/ab_test_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-simulator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple library to simulate AB tests.
 Home-page: https://github.com/k111git/ab-test-simulator
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-simulator
```

### Comparing `ab-test-simulator-0.0.3/ab_test_simulator.egg-info/SOURCES.txt` & `ab-test-simulator-0.0.4/ab_test_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.3/settings.ini` & `ab-test-simulator-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-simulator
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_simulator
```

### Comparing `ab-test-simulator-0.0.3/setup.py` & `ab-test-simulator-0.0.4/setup.py`

 * *Files identical despite different names*

