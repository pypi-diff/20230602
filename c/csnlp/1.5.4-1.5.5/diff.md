# Comparing `tmp/csnlp-1.5.4.tar.gz` & `tmp/csnlp-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csnlp-1.5.4.tar", last modified: Wed Apr  5 14:08:16 2023, max compression
+gzip compressed data, was "csnlp-1.5.5.tar", last modified: Fri Jun  2 17:17:48 2023, max compression
```

## Comparing `csnlp-1.5.4.tar` & `csnlp-1.5.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.916386 csnlp-1.5.4/
--rw-rw-rw-   0        0        0     1093 2022-11-02 20:11:46.000000 csnlp-1.5.4/LICENSE
--rw-rw-rw-   0        0        0     7007 2023-04-05 14:08:16.914395 csnlp-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     6267 2023-02-24 10:22:25.000000 csnlp-1.5.4/README.md
--rw-rw-rw-   0        0        0     1082 2023-04-05 14:05:07.000000 csnlp-1.5.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 14:08:16.916386 csnlp-1.5.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.823700 csnlp-1.5.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.834662 csnlp-1.5.4/src/csnlp/
--rw-rw-rw-   0        0        0      210 2023-04-04 11:47:09.000000 csnlp-1.5.4/src/csnlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.852604 csnlp-1.5.4/src/csnlp/core/
--rw-rw-rw-   0        0        0     3267 2023-01-02 20:43:22.000000 csnlp-1.5.4/src/csnlp/core/cache.py
--rw-rw-rw-   0        0        0     3186 2023-04-04 11:47:09.000000 csnlp-1.5.4/src/csnlp/core/data.py
--rw-rw-rw-   0        0        0     6057 2023-03-24 10:24:25.000000 csnlp-1.5.4/src/csnlp/core/debug.py
--rw-rw-rw-   0        0        0     2085 2023-02-16 10:35:36.000000 csnlp-1.5.4/src/csnlp/core/derivatives.py
--rw-rw-rw-   0        0        0     5241 2023-02-16 10:40:42.000000 csnlp-1.5.4/src/csnlp/core/scaling.py
--rw-rw-rw-   0        0        0     6426 2023-03-23 22:24:06.000000 csnlp-1.5.4/src/csnlp/core/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.860588 csnlp-1.5.4/src/csnlp/multistart/
--rw-rw-rw-   0        0        0      425 2023-03-20 12:01:22.000000 csnlp-1.5.4/src/csnlp/multistart/__init__.py
--rw-rw-rw-   0        0        0    15804 2023-04-05 14:05:07.000000 csnlp-1.5.4/src/csnlp/multistart/multistart_nlp.py
--rw-rw-rw-   0        0        0     3831 2023-03-20 12:48:12.000000 csnlp-1.5.4/src/csnlp/multistart/startpoints.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.873531 csnlp-1.5.4/src/csnlp/nlps/
--rw-rw-rw-   0        0        0    12295 2023-04-05 14:05:07.000000 csnlp-1.5.4/src/csnlp/nlps/constraints.py
--rw-rw-rw-   0        0        0     9068 2023-04-05 14:05:07.000000 csnlp-1.5.4/src/csnlp/nlps/nlp.py
--rw-rw-rw-   0        0        0     9390 2023-04-05 13:48:36.000000 csnlp-1.5.4/src/csnlp/nlps/objective.py
--rw-rw-rw-   0        0        0     2039 2023-03-25 14:04:48.000000 csnlp-1.5.4/src/csnlp/nlps/parameters.py
--rw-rw-rw-   0        0        0     2030 2023-03-25 14:01:54.000000 csnlp-1.5.4/src/csnlp/nlps/variables.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.885511 csnlp-1.5.4/src/csnlp/util/
--rw-rw-rw-   0        0        0     5231 2023-03-26 20:40:12.000000 csnlp-1.5.4/src/csnlp/util/docs.py
--rw-rw-rw-   0        0        0    11398 2023-03-25 13:36:29.000000 csnlp-1.5.4/src/csnlp/util/io.py
--rw-rw-rw-   0        0        0     5187 2023-04-05 14:05:07.000000 csnlp-1.5.4/src/csnlp/util/math.py
--rw-rw-rw-   0        0        0     3455 2023-03-24 17:58:30.000000 csnlp-1.5.4/src/csnlp/util/plot.py
--rw-rw-rw-   0        0        0      920 2023-03-17 16:33:38.000000 csnlp-1.5.4/src/csnlp/util/random.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.897450 csnlp-1.5.4/src/csnlp/wrappers/
--rw-rw-rw-   0        0        0      294 2023-03-29 19:05:51.000000 csnlp-1.5.4/src/csnlp/wrappers/__init__.py
--rw-rw-rw-   0        0        0    16506 2023-03-25 14:29:46.000000 csnlp-1.5.4/src/csnlp/wrappers/mpc.py
--rw-rw-rw-   0        0        0     7474 2023-02-16 10:51:07.000000 csnlp-1.5.4/src/csnlp/wrappers/scaling.py
--rw-rw-rw-   0        0        0    16282 2023-04-04 11:47:09.000000 csnlp-1.5.4/src/csnlp/wrappers/sensitivity.py
--rw-rw-rw-   0        0        0     3644 2023-01-07 17:14:55.000000 csnlp-1.5.4/src/csnlp/wrappers/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.842635 csnlp-1.5.4/src/csnlp.egg-info/
--rw-rw-rw-   0        0        0     7007 2023-04-05 14:08:16.000000 csnlp-1.5.4/src/csnlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1040 2023-04-05 14:08:16.000000 csnlp-1.5.4/src/csnlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 14:08:16.000000 csnlp-1.5.4/src/csnlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-05 14:08:16.000000 csnlp-1.5.4/src/csnlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-05 14:08:16.000000 csnlp-1.5.4/src/csnlp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 14:08:16.912400 csnlp-1.5.4/tests/
--rw-rw-rw-   0        0        0    13201 2023-03-29 19:49:44.000000 csnlp-1.5.4/tests/test_core.py
--rw-rw-rw-   0        0        0    10172 2023-04-05 14:05:07.000000 csnlp-1.5.4/tests/test_examples.py
--rw-rw-rw-   0        0        0     7610 2023-03-22 17:16:32.000000 csnlp-1.5.4/tests/test_multistart.py
--rw-rw-rw-   0        0        0    25071 2023-04-05 14:05:07.000000 csnlp-1.5.4/tests/test_nlps.py
--rw-rw-rw-   0        0        0    27469 2023-03-17 16:39:02.000000 csnlp-1.5.4/tests/test_quadrotor_mpc.py
--rw-rw-rw-   0        0        0     8655 2023-04-05 13:15:57.000000 csnlp-1.5.4/tests/test_util.py
--rw-rw-rw-   0        0        0    28699 2023-04-05 14:05:07.000000 csnlp-1.5.4/tests/test_wrappers.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.983255 csnlp-1.5.5/
+-rw-rw-rw-   0        0        0     1093 2022-11-02 20:11:46.000000 csnlp-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0     7069 2023-06-02 17:17:48.982580 csnlp-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6267 2023-02-24 10:22:25.000000 csnlp-1.5.5/README.md
+-rw-rw-rw-   0        0        0     1155 2023-06-02 17:13:58.000000 csnlp-1.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 17:17:48.984358 csnlp-1.5.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.822631 csnlp-1.5.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.847830 csnlp-1.5.5/src/csnlp/
+-rw-rw-rw-   0        0        0      210 2023-04-04 11:47:09.000000 csnlp-1.5.5/src/csnlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.885464 csnlp-1.5.5/src/csnlp/core/
+-rw-rw-rw-   0        0        0     3267 2023-01-02 20:43:22.000000 csnlp-1.5.5/src/csnlp/core/cache.py
+-rw-rw-rw-   0        0        0     3186 2023-04-04 11:47:09.000000 csnlp-1.5.5/src/csnlp/core/data.py
+-rw-rw-rw-   0        0        0     6057 2023-03-24 10:24:25.000000 csnlp-1.5.5/src/csnlp/core/debug.py
+-rw-rw-rw-   0        0        0     2085 2023-02-16 10:35:36.000000 csnlp-1.5.5/src/csnlp/core/derivatives.py
+-rw-rw-rw-   0        0        0     5241 2023-02-16 10:40:42.000000 csnlp-1.5.5/src/csnlp/core/scaling.py
+-rw-rw-rw-   0        0        0     6426 2023-03-23 22:24:06.000000 csnlp-1.5.5/src/csnlp/core/solutions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.896386 csnlp-1.5.5/src/csnlp/multistart/
+-rw-rw-rw-   0        0        0      425 2023-03-20 12:01:22.000000 csnlp-1.5.5/src/csnlp/multistart/__init__.py
+-rw-rw-rw-   0        0        0    15829 2023-06-02 17:10:40.000000 csnlp-1.5.5/src/csnlp/multistart/multistart_nlp.py
+-rw-rw-rw-   0        0        0     3831 2023-03-20 12:48:12.000000 csnlp-1.5.5/src/csnlp/multistart/startpoints.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.911677 csnlp-1.5.5/src/csnlp/nlps/
+-rw-rw-rw-   0        0        0    12295 2023-04-05 14:05:07.000000 csnlp-1.5.5/src/csnlp/nlps/constraints.py
+-rw-rw-rw-   0        0        0     9068 2023-04-05 14:05:07.000000 csnlp-1.5.5/src/csnlp/nlps/nlp.py
+-rw-rw-rw-   0        0        0     9584 2023-06-02 17:10:40.000000 csnlp-1.5.5/src/csnlp/nlps/objective.py
+-rw-rw-rw-   0        0        0     2039 2023-03-25 14:04:48.000000 csnlp-1.5.5/src/csnlp/nlps/parameters.py
+-rw-rw-rw-   0        0        0     2030 2023-03-25 14:01:54.000000 csnlp-1.5.5/src/csnlp/nlps/variables.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.929036 csnlp-1.5.5/src/csnlp/util/
+-rw-rw-rw-   0        0        0     5231 2023-03-26 20:40:12.000000 csnlp-1.5.5/src/csnlp/util/docs.py
+-rw-rw-rw-   0        0        0    11398 2023-03-25 13:36:29.000000 csnlp-1.5.5/src/csnlp/util/io.py
+-rw-rw-rw-   0        0        0     5187 2023-04-05 14:05:07.000000 csnlp-1.5.5/src/csnlp/util/math.py
+-rw-rw-rw-   0        0        0     3455 2023-03-24 17:58:30.000000 csnlp-1.5.5/src/csnlp/util/plot.py
+-rw-rw-rw-   0        0        0      920 2023-03-17 16:33:38.000000 csnlp-1.5.5/src/csnlp/util/random.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.946460 csnlp-1.5.5/src/csnlp/wrappers/
+-rw-rw-rw-   0        0        0      294 2023-03-29 19:05:51.000000 csnlp-1.5.5/src/csnlp/wrappers/__init__.py
+-rw-rw-rw-   0        0        0    16506 2023-03-25 14:29:46.000000 csnlp-1.5.5/src/csnlp/wrappers/mpc.py
+-rw-rw-rw-   0        0        0     7474 2023-02-16 10:51:07.000000 csnlp-1.5.5/src/csnlp/wrappers/scaling.py
+-rw-rw-rw-   0        0        0    16282 2023-04-04 11:47:09.000000 csnlp-1.5.5/src/csnlp/wrappers/sensitivity.py
+-rw-rw-rw-   0        0        0     3644 2023-01-07 17:14:55.000000 csnlp-1.5.5/src/csnlp/wrappers/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.865631 csnlp-1.5.5/src/csnlp.egg-info/
+-rw-rw-rw-   0        0        0     7069 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1040 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.978647 csnlp-1.5.5/tests/
+-rw-rw-rw-   0        0        0    13201 2023-03-29 19:49:44.000000 csnlp-1.5.5/tests/test_core.py
+-rw-rw-rw-   0        0        0    10172 2023-04-05 14:05:07.000000 csnlp-1.5.5/tests/test_examples.py
+-rw-rw-rw-   0        0        0     7610 2023-03-22 17:16:32.000000 csnlp-1.5.5/tests/test_multistart.py
+-rw-rw-rw-   0        0        0    25071 2023-04-05 14:05:07.000000 csnlp-1.5.5/tests/test_nlps.py
+-rw-rw-rw-   0        0        0    27469 2023-03-17 16:39:02.000000 csnlp-1.5.5/tests/test_quadrotor_mpc.py
+-rw-rw-rw-   0        0        0     8655 2023-04-05 13:15:57.000000 csnlp-1.5.5/tests/test_util.py
+-rw-rw-rw-   0        0        0    28699 2023-04-05 14:05:07.000000 csnlp-1.5.5/tests/test_wrappers.py
```

### Comparing `csnlp-1.5.4/LICENSE` & `csnlp-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/PKG-INFO` & `csnlp-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: csnlp
-Version: 1.5.4
+Version: 1.5.5
 Summary: Nonlinear Progamming with CasADi
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/casadi-nlp
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/casadi-nlp/issues
+Keywords: nonlinear-optimization,casadi,sensitivity-analysis
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
```

### Comparing `csnlp-1.5.4/README.md` & `csnlp-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/pyproject.toml` & `csnlp-1.5.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "csnlp"
-version = "1.5.4"
+version = "1.5.5"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Nonlinear Progamming with CasADi"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
@@ -21,14 +21,15 @@
     "Topic :: Scientific/Engineering :: Mathematics"
 ]
 dependencies = [
     "numpy >= 1.21.6",
     "casadi >= 3.6.0",
     "joblib >= 1.2.0",
 ]
+keywords = ["nonlinear-optimization", "casadi", "sensitivity-analysis"]
 
 [project.optional-dependencies]
 all = [
     "matplotlib >= 3.6.2",
     "tikzplotlib >= 0.10.1",
 ]
```

### Comparing `csnlp-1.5.4/src/csnlp/core/cache.py` & `csnlp-1.5.5/src/csnlp/core/cache.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/core/data.py` & `csnlp-1.5.5/src/csnlp/core/data.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/core/debug.py` & `csnlp-1.5.5/src/csnlp/core/debug.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/core/derivatives.py` & `csnlp-1.5.5/src/csnlp/core/derivatives.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/core/scaling.py` & `csnlp-1.5.5/src/csnlp/core/scaling.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/core/solutions.py` & `csnlp-1.5.5/src/csnlp/core/solutions.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/multistart/multistart_nlp.py` & `csnlp-1.5.5/src/csnlp/multistart/multistart_nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         ]
         self._stacked_nlp.minimize(sum(self._fs))
         return out
 
     def init_solver(
         self,
         opts: Optional[Dict[str, Any]] = None,
-        solver: Literal["opti", "qp"] = "opti",
+        solver: Literal["ipopt", "sqpmethod", "qrqp", "osqp"] = "ipopt",
     ) -> None:
         out = super().init_solver(opts, solver)
         self._stacked_nlp.init_solver(opts, solver)
         return out
 
     def solve_multi(
         self,
```

### Comparing `csnlp-1.5.4/src/csnlp/multistart/startpoints.py` & `csnlp-1.5.5/src/csnlp/multistart/startpoints.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/nlps/constraints.py` & `csnlp-1.5.5/src/csnlp/nlps/constraints.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/nlps/nlp.py` & `csnlp-1.5.5/src/csnlp/nlps/nlp.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/nlps/objective.py` & `csnlp-1.5.5/src/csnlp/nlps/objective.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from functools import partial
-from typing import Any, Dict, Literal, Optional, TypeVar
+from typing import Any, Callable, Dict, Literal, Optional, TypeVar
 
 import casadi as cs
 import numpy as np
 import numpy.typing as npt
 from joblib import Memory
 from joblib.memory import MemorizedFunc
 
 from csnlp.core.solutions import Solution, subsevalf
 from csnlp.nlps.constraints import HasConstraints
 
 SymType = TypeVar("SymType", cs.SX, cs.MX)
 
+_XXSOL: Dict[str, Callable] = {
+    "ipopt": cs.nlpsol,
+    "sqpmethod": cs.nlpsol,
+    "qrqp": cs.qpsol,
+    "osqp": cs.qpsol,
+}
+
 
 def _solve_and_get_stats(
     solver: MemorizedFunc, kwargs: Dict[str, npt.ArrayLike]
 ) -> Dict[str, Any]:
     """Internal utility to simultaneously run the solver and get its stats."""
     sol = solver(**kwargs)
     sol["p"] = kwargs["p"]  # add to solution the parameters for which it was computed
@@ -90,39 +97,41 @@
     def failures(self) -> int:
         """Gets the cumulative number of failures of the NLP solver."""
         return self._failures
 
     def init_solver(
         self,
         opts: Optional[Dict[str, Any]] = None,
-        solver: Literal["opti", "qp"] = "opti",
+        solver: Literal["ipopt", "sqpmethod", "qrqp", "osqp"] = "ipopt",
     ) -> None:
         """Initializes the solver for this NLP with the given options.
 
         Parameters
         ----------
         opts : Dict[str, Any], optional
             Options to be passed to the CasADi interface to the solver.
-        solver : 'ipopt' or 'qp', optional
-            Type of solver to instantiate. By default, IPOPT is chosen to deal with
-            NLPs. However, if the optimization problem is linear, `qp` can be specified.
+        solver : {'ipopt', 'sqpmethod', 'qrqp', 'osqp'}, optional
+            Type of solver to instantiate. "ipopt" and "sqpmethod" trigger the
+            instantiation of an NLP problem, while "qrqp" and "osqp" a conic one. By
+            default, 'ipopt' is selected.
 
         Raises
         ------
         RuntimeError
             Raises if the objective has not yet been specified with `minimize`.
         """
         if self._f is None:
             raise RuntimeError("NLP objective not set.")
 
         opts = {} if opts is None else opts.copy()
         con = cs.vertcat(self._g, self._h)
         problem = {"x": self._x, "p": self._p, "g": con, "f": self._f}
-        func, stype = (cs.qpsol, "qrqp") if solver == "qp" else (cs.nlpsol, "ipopt")
-        solver_func = func(f"solver_{stype}_{self.name}", stype, problem, opts)
+
+        func = _XXSOL.get(solver, cs.nlpsol)
+        solver_func = func(f"solver_{solver}_{self.name}", solver, problem, opts)
 
         self._solver = self._cache.cache(solver_func)
         self._solver_type = solver
         self._solver_opts = opts
 
     def refresh_solver(self) -> None:
         """Refresh and resets the internal solver function (with the same options, if
```

### Comparing `csnlp-1.5.4/src/csnlp/nlps/parameters.py` & `csnlp-1.5.5/src/csnlp/nlps/parameters.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/nlps/variables.py` & `csnlp-1.5.5/src/csnlp/nlps/variables.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/util/docs.py` & `csnlp-1.5.5/src/csnlp/util/docs.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/util/io.py` & `csnlp-1.5.5/src/csnlp/util/io.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/util/math.py` & `csnlp-1.5.5/src/csnlp/util/math.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/util/plot.py` & `csnlp-1.5.5/src/csnlp/util/plot.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/util/random.py` & `csnlp-1.5.5/src/csnlp/util/random.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/wrappers/mpc.py` & `csnlp-1.5.5/src/csnlp/wrappers/mpc.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/wrappers/scaling.py` & `csnlp-1.5.5/src/csnlp/wrappers/scaling.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/wrappers/sensitivity.py` & `csnlp-1.5.5/src/csnlp/wrappers/sensitivity.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp/wrappers/wrapper.py` & `csnlp-1.5.5/src/csnlp/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/src/csnlp.egg-info/PKG-INFO` & `csnlp-1.5.5/src/csnlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: csnlp
-Version: 1.5.4
+Version: 1.5.5
 Summary: Nonlinear Progamming with CasADi
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/casadi-nlp
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/casadi-nlp/issues
+Keywords: nonlinear-optimization,casadi,sensitivity-analysis
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
```

### Comparing `csnlp-1.5.4/src/csnlp.egg-info/SOURCES.txt` & `csnlp-1.5.5/src/csnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/tests/test_core.py` & `csnlp-1.5.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/tests/test_examples.py` & `csnlp-1.5.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/tests/test_multistart.py` & `csnlp-1.5.5/tests/test_multistart.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/tests/test_nlps.py` & `csnlp-1.5.5/tests/test_nlps.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/tests/test_quadrotor_mpc.py` & `csnlp-1.5.5/tests/test_quadrotor_mpc.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/tests/test_util.py` & `csnlp-1.5.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.4/tests/test_wrappers.py` & `csnlp-1.5.5/tests/test_wrappers.py`

 * *Files identical despite different names*

