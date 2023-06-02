# Comparing `tmp/fides-0.7.7.tar.gz` & `tmp/fides-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fides-0.7.7.tar", last modified: Mon May  1 13:09:13 2023, max compression
+gzip compressed data, was "fides-0.7.8.tar", last modified: Fri Jun  2 18:32:17 2023, max compression
```

## Comparing `fides-0.7.7.tar` & `fides-0.7.8.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:09:13.799842 fides-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-05-01 13:09:13.799842 fides-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-05-01 13:09:12.000000 fides-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:09:13.799842 fides-0.7.7/fides/
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-05-01 13:09:12.000000 fides-0.7.7/fides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5270 2023-05-01 13:09:12.000000 fides-0.7.7/fides/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20130 2023-05-01 13:09:12.000000 fides-0.7.7/fides/hessian_approximation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-05-01 13:09:12.000000 fides-0.7.7/fides/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    32013 2023-05-01 13:09:12.000000 fides-0.7.7/fides/minimize.py
--rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-05-01 13:09:12.000000 fides-0.7.7/fides/stepback.py
--rw-r--r--   0 runner    (1001) docker     (122)    17254 2023-05-01 13:09:12.000000 fides-0.7.7/fides/steps.py
--rw-r--r--   0 runner    (1001) docker     (122)    10253 2023-05-01 13:09:12.000000 fides-0.7.7/fides/subproblem.py
--rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-05-01 13:09:12.000000 fides-0.7.7/fides/trust_region.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-01 13:09:12.000000 fides-0.7.7/fides/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:09:13.799842 fides-0.7.7/fides.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      367 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-01 13:09:13.799842 fides-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-05-01 13:09:12.000000 fides-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:32:17.248677 fides-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-02 18:32:17.248677 fides-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-06-02 18:32:09.000000 fides-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:32:17.244677 fides-0.7.8/fides/
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-06-02 18:32:09.000000 fides-0.7.8/fides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-06-02 18:32:09.000000 fides-0.7.8/fides/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20443 2023-06-02 18:32:09.000000 fides-0.7.8/fides/hessian_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-02 18:32:09.000000 fides-0.7.8/fides/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32354 2023-06-02 18:32:09.000000 fides-0.7.8/fides/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-06-02 18:32:09.000000 fides-0.7.8/fides/stepback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17433 2023-06-02 18:32:09.000000 fides-0.7.8/fides/steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10223 2023-06-02 18:32:09.000000 fides-0.7.8/fides/subproblem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5172 2023-06-02 18:32:09.000000 fides-0.7.8/fides/trust_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-02 18:32:09.000000 fides-0.7.8/fides/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:32:17.244677 fides-0.7.8/fides.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-02 18:32:17.000000 fides-0.7.8/fides.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-02 18:32:17.000000 fides-0.7.8/fides.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 18:32:17.000000 fides-0.7.8/fides.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-02 18:32:17.000000 fides-0.7.8/fides.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-02 18:32:17.000000 fides-0.7.8/fides.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-06-02 18:32:09.000000 fides-0.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-06-02 18:32:17.248677 fides-0.7.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:32:17.248677 fides-0.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-06-02 18:32:09.000000 fides-0.7.8/tests/test_hessian_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11534 2023-06-02 18:32:09.000000 fides-0.7.8/tests/test_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4886 2023-06-02 18:32:09.000000 fides-0.7.8/tests/test_subproblem.py
```

### Comparing `fides-0.7.7/PKG-INFO` & `fides-0.7.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 Metadata-Version: 2.1
 Name: fides
-Version: 0.7.7
-Summary: python Trust Region Optimization
-Home-page: https://github.com/Fides-dev/fides
-Author: Fabian Froehlich
-Author-email: froehlichfab@gmail.com
+Version: 0.7.8
+Summary: python-based Trust Region Optimization toolbox
+Home-page: https://github.com/fides-dev/fides
+Download-URL: https://github.com/fides-dev/fides/releases
+Author: The fides developers
+Author-email: frohlichfab@gmail.com
+Maintainer: Fabian Fröhlich
+Maintainer-email: frohlichfab@gmail.com
 License: BSD-3-Clause
-Description: # Fides - A python package for Trust Region Optimization
-        
-        <a href="https://badge.fury.io/py/fides">
-          <img src="https://badge.fury.io/py/fides.svg" alt="PyPI version"></a>
-        <a href="https://codecov.io/gh/fides-dev/fides">
-          <img src="https://codecov.io/gh/fides-dev/fides/branch/master/graph/badge.svg" alt="Code coverage"></a>
-        <a href="https://fides-optimizer.readthedocs.io/en/latest/?badge=latest">
-         <img src="https://readthedocs.org/projects/fides-optimizer/badge/?version=latest" alt="ReadTheDocs status"></a>
-        <a href="https://zenodo.org/badge/latestdoi/312057973">
-         <img src="https://zenodo.org/badge/312057973.svg" alt="DOI"></a>
-        
-        ## About Fides
-        
-        Fides implements an Interior Trust Region Reflective for boundary constrained
-        optimization problems based on the papers
-        [ColemanLi1994](https://doi.org/10.1007/BF01582221) and
-        [ColemanLi1996](http://dx.doi.org/10.1137/0806023). Accordingly, Fides is named
-        after the Roman goddess of trust and
-        reliability.
-        
-        Fides can be installed via `pip install fides`. Further documentation is
-         available at [Read the Docs](https://fides-optimizer.readthedocs.io/).
-         
-         
-        ## Features
-        
-        
-        * Boundary constrained and unconstrained interior trust-region optimization
-        * Reflective, truncated and optimization based boundary heuristics
-        * Exact, 2D and CG subproblem solvers
-        * BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative
-         Hessian Approximation schemes
-        * SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian Approximations schemes
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
+Project-URL: Bug Tracker, https://github.com/fides-dev/fides/issues
+Project-URL: Documentation, https://fides-optimizer.readthedocs.io/
+Project-URL: Changelog, https://github.com/fides-dev/fides/releases
+Keywords: optimization,trust-region,systems biology
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: test
+
+# Fides - A python package for Trust Region Optimization
+
+<a href="https://badge.fury.io/py/fides">
+  <img src="https://badge.fury.io/py/fides.svg" alt="PyPI version"></a>
+<a href="https://codecov.io/gh/fides-dev/fides">
+  <img src="https://codecov.io/gh/fides-dev/fides/branch/master/graph/badge.svg" alt="Code coverage"></a>
+<a href="https://fides-optimizer.readthedocs.io/en/latest/?badge=latest">
+ <img src="https://readthedocs.org/projects/fides-optimizer/badge/?version=latest" alt="ReadTheDocs status"></a>
+<a href="https://zenodo.org/badge/latestdoi/312057973">
+ <img src="https://zenodo.org/badge/312057973.svg" alt="DOI"></a>
+
+## About Fides
+
+Fides implements an Interior Trust Region Reflective for boundary constrained
+optimization problems based on the papers
+[ColemanLi1994](https://doi.org/10.1007/BF01582221) and
+[ColemanLi1996](http://dx.doi.org/10.1137/0806023). Accordingly, Fides is named
+after the Roman goddess of trust and
+reliability.
+
+Fides can be installed via `pip install fides`. Further documentation is
+ available at [Read the Docs](https://fides-optimizer.readthedocs.io/).
+ 
+ 
+## Features
+
+
+* Boundary constrained and unconstrained interior trust-region optimization
+* Reflective, truncated and optimization based boundary heuristics
+* Exact, 2D and CG subproblem solvers
+* BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative
+ Hessian Approximation schemes
+* SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian Approximations schemes
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,24 +1,29 @@
-Metadata-Version: 2.1 Name: fides Version: 0.7.7 Summary: python Trust Region
-Optimization Home-page: https://github.com/Fides-dev/fides Author: Fabian
-Froehlich Author-email: froehlichfab@gmail.com License: BSD-3-Clause
-Description: # Fides - A python package for Trust Region Optimization [PyPI
-version] [Code_coverage] [ReadTheDocs_status] [DOI] ## About Fides Fides
-implements an Interior Trust Region Reflective for boundary constrained
-optimization problems based on the papers [ColemanLi1994](https://doi.org/
-10.1007/BF01582221) and [ColemanLi1996](http://dx.doi.org/10.1137/0806023).
-Accordingly, Fides is named after the Roman goddess of trust and reliability.
-Fides can be installed via `pip install fides`. Further documentation is
-available at [Read the Docs](https://fides-optimizer.readthedocs.io/). ##
-Features * Boundary constrained and unconstrained interior trust-region
-optimization * Reflective, truncated and optimization based boundary heuristics
-* Exact, 2D and CG subproblem solvers * BFGS, DFP, SR1, Broyden (good and bad)
-and Broyden class iterative Hessian Approximation schemes * SSM, TSSM, FX,
-GNSBFGS and custom hybrid Hessian Approximations schemes Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Software Development ::
-Libraries Classifier: License :: OSI Approved :: BSD License Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: fides Version: 0.7.8 Summary: python-based Trust
+Region Optimization toolbox Home-page: https://github.com/fides-dev/fides
+Download-URL: https://github.com/fides-dev/fides/releases Author: The fides
+developers Author-email: frohlichfab@gmail.com Maintainer: Fabian FrÃ¶hlich
+Maintainer-email: frohlichfab@gmail.com License: BSD-3-Clause Project-URL: Bug
+Tracker, https://github.com/fides-dev/fides/issues Project-URL: Documentation,
+https://fides-optimizer.readthedocs.io/ Project-URL: Changelog, https://
+github.com/fides-dev/fides/releases Keywords: optimization,trust-region,systems
+biology Classifier: Development Status :: 4 - Beta Classifier: Topic ::
+Software Development :: Libraries Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: BSD License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.9
+Description-Content-Type: text/markdown Provides-Extra: test # Fides - A python
+package for Trust Region Optimization [PyPI_version] [Code_coverage]
+[ReadTheDocs_status] [DOI] ## About Fides Fides implements an Interior Trust
+Region Reflective for boundary constrained optimization problems based on the
+papers [ColemanLi1994](https://doi.org/10.1007/BF01582221) and [ColemanLi1996]
+(http://dx.doi.org/10.1137/0806023). Accordingly, Fides is named after the
+Roman goddess of trust and reliability. Fides can be installed via `pip install
+fides`. Further documentation is available at [Read the Docs](https://fides-
+optimizer.readthedocs.io/). ## Features * Boundary constrained and
+unconstrained interior trust-region optimization * Reflective, truncated and
+optimization based boundary heuristics * Exact, 2D and CG subproblem solvers *
+BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative Hessian
+Approximation schemes * SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian
+Approximations schemes
```

### Comparing `fides-0.7.7/README.md` & `fides-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `fides-0.7.7/fides/constants.py` & `fides-0.7.8/fides/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 Constants
 -----------
 This module provides a central place to define native python enums and
 constants that are used in multiple other modules
 """
 
 import enum
-import numpy as np
-
-from numbers import Real, Integral
+from numbers import Integral, Real
 from pathlib import PosixPath, WindowsPath
-
 from typing import Dict
 
+import numpy as np
+
 
 class Options(str, enum.Enum):
     """
     Defines all the fields that can be specified in Options to
     :py:class:`Optimizer`
     """
+
     MAXITER = 'maxiter'  #: maximum number of allowed iterations
     MAXTIME = 'maxtime'  #: maximum amount of walltime in seconds
     FATOL = 'fatol'  #: absolute tolerance for convergence based on fval
     FRTOL = 'frtol'  #: relative tolerance for convergence based on fval
     XTOL = 'xtol'  #: tolerance for convergence based on x
     GATOL = 'gatol'  #: absolute tolerance for convergence based on grad
     GRTOL = 'grtol'  #: relative tolerance for convergence based on grad
@@ -49,14 +49,15 @@
 
 
 class StepBackStrategy(str, enum.Enum):
     """
     Defines the possible choices of search refinement if proposed step
     reaches optimization boundary
     """
+
     SINGLE_REFLECT = 'reflect_single'  #: single reflection at boundary
     REFLECT = 'reflect'  #: recursive reflections at boundary
     TRUNCATE = 'truncate'  #: truncate step at boundary and re-solve
     # restricted subproblem
     MIXED = 'mixed'  #: mix reflections and truncations
     REFINE = 'refine'  #: perform optimization to refine step
 
@@ -71,26 +72,27 @@
     Options.GRTOL: 0,
     Options.SUBSPACE_DIM: SubSpaceDim.TWO,
     Options.STEPBACK_STRAT: StepBackStrategy.REFLECT,
     Options.THETA_MAX: 0.95,
     Options.DELTA_INIT: 1.0,
     Options.MU: 0.25,  # [NodedalWright2006]
     Options.ETA: 0.75,  # [NodedalWright2006]
-    Options.GAMMA1: 1/4,  # [NodedalWright2006]
+    Options.GAMMA1: 1 / 4,  # [NodedalWright2006]
     Options.GAMMA2: 2,  # [NodedalWright2006]
     Options.HISTORY_FILE: None,
 }
 
 
 class ExitFlag(int, enum.Enum):
     """
     Defines possible exitflag values for the optimizer to indicate why
     optimization exited. Negative value indicate errors while positive
     values indicate convergence.
     """
+
     DID_NOT_RUN = 0  #: Optimizer did not run
     MAXITER = -1  #: Reached maximum number of allowed iterations
     MAXTIME = -2  #: Expected to reach maximum allowed time in next iteration
     NOT_FINITE = -3  #: Encountered non-finite fval/grad/hess
     EXCEEDED_BOUNDARY = -4  #: Exceeded specified boundaries
     DELTA_TOO_SMALL = -5  #: Trust Region Radius too small to proceed
     FTOL = 1  #: Converged according to fval difference
@@ -130,10 +132,12 @@
         if option_key is Options.STEPBACK_STRAT:
             option_value = StepBackStrategy(option_value)
 
         expected_type = expected_types[option]
         if not isinstance(option_value, expected_type):
             if expected_type == Integral and int(option_value) == option_value:
                 continue
-            raise TypeError(f'Type mismatch for option {option_key}. '
-                            f'Expected {expected_type} but got '
-                            f'{type(option_value)}')
+            raise TypeError(
+                f'Type mismatch for option {option_key}. '
+                f'Expected {expected_type} but got '
+                f'{type(option_value)}'
+            )
```

### Comparing `fides-0.7.7/fides/hessian_approximation.py` & `fides-0.7.8/fides/hessian_approximation.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 -------------------------
 This module provides various generic Hessian approximation strategies that
 can be employed when the calculating the exact Hessian or an approximation
 is computationally too demanding.
 """
 
 
+import warnings
 from typing import Optional
+
 import numpy as np
-import warnings
 from numpy.linalg import norm
 
 
 class HessianApproximation:
     """
     Abstract class from which Hessian update strategies should subclass
     """
+
     def __init__(self, init_with_hess: Optional[bool] = False):
         """
         Create a Hessian update strategy instance
 
         :param init_with_hess:
             Whether the hybrid update strategy should be initialized
             according to the user-provided objective function
@@ -39,17 +41,19 @@
         :param hess:
             user provided initialization
         """
         if hess is None or not self.init_with_hess:
             self._hess = np.eye(dim)
         else:
             if hess.shape[0] != dim:
-                raise ValueError('Initial approximation had inconsistent '
-                                 f'dimension, was {hess.shape[0]}, '
-                                 f'but should be {dim}.')
+                raise ValueError(
+                    'Initial approximation had inconsistent '
+                    f'dimension, was {hess.shape[0]}, '
+                    f'but should be {dim}.'
+                )
             self._hess = hess.copy()
         self._diff = np.zeros_like(self._hess)
 
     def get_mat(self) -> np.ndarray:
         """
         Getter for the Hessian approximation
 
@@ -71,17 +75,19 @@
         """
         Setter for the Hessian approximation
 
         :param mat:
             Hessian approximation
         """
         if mat.shape != self._hess.shape:
-            raise ValueError('Passed matrix had inconsistent '
-                             f'shape, was {mat.shape}, '
-                             f'but should be {self._hess.shape}.')
+            raise ValueError(
+                'Passed matrix had inconsistent '
+                f'shape, was {mat.shape}, '
+                f'but should be {self._hess.shape}.'
+            )
         self._hess = mat.copy()
 
     @property
     def requires_resfun(self):
         return False  # pragma: no cover
 
     @property
@@ -93,14 +99,15 @@
         self._hess = hess.copy()
 
 
 class IterativeHessianApproximation(HessianApproximation):
     """
     Iterative update schemes that only use s and y values for update.
     """
+
     def update(self, s: np.ndarray, y: np.ndarray) -> None:
         """
         Update the Hessian approximation
 
         :param s:
             step in optimization variables
 
@@ -133,64 +140,87 @@
         DFP (phi==1).
     :parameter enforce_curv_cond:
         boolean that controls whether the employed broyden class update
         should attempt to preserve positive definiteness. If set to True,
         updates from steps that violate the curvature condition will be
         discarded.
     """
-    def __init__(self, phi: float, init_with_hess: Optional[bool] = False,
-                 enforce_curv_cond: Optional[bool] = True):
+
+    def __init__(
+        self,
+        phi: float,
+        init_with_hess: Optional[bool] = False,
+        enforce_curv_cond: Optional[bool] = True,
+    ):
         self.phi = phi
         self.enforce_curv_cond = enforce_curv_cond
         if phi < 0 or phi > 1:
-            warnings.warn('Setting phi to values outside the interval [0, 1]'
-                          'will not guarantee that positive definiteness is '
-                          'preserved during updating.')
+            warnings.warn(
+                'Setting phi to values outside the interval [0, 1]'
+                'will not guarantee that positive definiteness is '
+                'preserved during updating.'
+            )
         super(Broyden, self).__init__(init_with_hess)
 
     def _compute_update(self, s: np.ndarray, y: np.ndarray):
-        self._diff = broyden_class_update(y, s, self._hess, self.phi,
-                                          self.enforce_curv_cond)
+        self._diff = broyden_class_update(
+            y, s, self._hess, self.phi, self.enforce_curv_cond
+        )
 
 
 class BFGS(Broyden):
     """
     Broyden-Fletcher-Goldfarb-Shanno update strategy. This is a rank 2
     update strategy that preserves symmetry and positive-semidefiniteness.
 
     This scheme only works with a function that returns (fval, grad)
     """
-    def __init__(self, init_with_hess: Optional[bool] = False,
-                 enforce_curv_cond: Optional[bool] = True):
-        super(BFGS, self).__init__(phi=0.0, init_with_hess=init_with_hess,
-                                   enforce_curv_cond=enforce_curv_cond)
+
+    def __init__(
+        self,
+        init_with_hess: Optional[bool] = False,
+        enforce_curv_cond: Optional[bool] = True,
+    ):
+        super(BFGS, self).__init__(
+            phi=0.0,
+            init_with_hess=init_with_hess,
+            enforce_curv_cond=enforce_curv_cond,
+        )
 
 
 class DFP(Broyden):
     """
     Davidon-Fletcher-Powell update strategy. This is a rank 2
     update strategy that preserves symmetry and positive-semidefiniteness.
 
     This scheme only works with a function that returns (fval, grad)
     """
-    def __init__(self, init_with_hess: Optional[bool] = False,
-                 enforce_curv_cond: Optional[bool] = True):
-        super(DFP, self).__init__(phi=1.0, init_with_hess=init_with_hess,
-                                  enforce_curv_cond=enforce_curv_cond)
+
+    def __init__(
+        self,
+        init_with_hess: Optional[bool] = False,
+        enforce_curv_cond: Optional[bool] = True,
+    ):
+        super(DFP, self).__init__(
+            phi=1.0,
+            init_with_hess=init_with_hess,
+            enforce_curv_cond=enforce_curv_cond,
+        )
 
 
 class SR1(IterativeHessianApproximation):
     """
     Symmetric Rank 1 update strategy as described in
     [Nocedal & Wright](http://dx.doi.org/10.1007/b98874) Chapter 6.2.
     This is a rank 1 update  strategy that preserves symmetry but does not
     preserve positive-semidefiniteness.
 
     This scheme only works with a function that returns (fval, grad)
     """
+
     def _compute_update(self, s: np.ndarray, y: np.ndarray):
         z = y - self._hess.dot(s)
         d = z.T.dot(s)
 
         # [NocedalWright2006] (6.26) reject if update degenerate
         if np.abs(d) >= np.sqrt(np.spacing(1)) * norm(s) * norm(z):
             self._diff = np.outer(z, z.T) / d
@@ -203,28 +233,30 @@
     Broydens "good" method as introduced in
     [Broyden 1965](https://doi.org/10.1090%2FS0025-5718-1965-0198670-6).
     This is a rank 1 update strategy that does not preserve symmetry or
     positive definiteness.
 
     This scheme only works with a function that returns (fval, grad)
     """
+
     def _compute_update(self, s: np.ndarray, y: np.ndarray):
         z = y - self._hess.dot(s)
         self._diff = np.outer(z, s.T) / s.T.dot(s)
 
 
 class BB(IterativeHessianApproximation):
     """
     Broydens "bad" method as introduced in
     [Broyden 1965](https://doi.org/10.1090%2FS0025-5718-1965-0198670-6).
     This is a rank 1 update strategy that does not preserve symmetry or
     positive definiteness.
 
     This scheme only works with a function that returns (fval, grad)
     """
+
     def update(self, s: np.ndarray, y: np.ndarray) -> None:
         b = y.T.dot(s)
         z = y - self._hess.dot(s)
         if b <= 0:
             self._diff = np.zeros_like(self._hess)
         else:
             self._diff = np.outer(z, s.T) / b
@@ -247,28 +279,29 @@
         super(HybridApproximation, self).init_mat(dim, hess)
 
     def requires_hess(self):
         return True  # pragma: no cover
 
 
 class HybridSwitchApproximation(HybridApproximation):
-    def _switched_update(self, s: np.ndarray, y: np.ndarray,
-                         hess: np.ndarray):
+    def _switched_update(self, s: np.ndarray, y: np.ndarray, hess: np.ndarray):
         self.hessian_update.update(s, y)
         if self._switched:
             new_hess = self.hessian_update.get_mat()
         else:
             new_hess = hess
         self._update_hess_and_store_diff(new_hess)
 
 
 class HybridFixed(HybridSwitchApproximation):
-    def __init__(self,
-                 happ: IterativeHessianApproximation = BFGS(),
-                 switch_iteration: Optional[int] = 20):
+    def __init__(
+        self,
+        happ: IterativeHessianApproximation = BFGS(),
+        switch_iteration: Optional[int] = 20,
+    ):
         """
         Switch from a dynamic approximation to the user provided iterative
         scheme after a fixed number of successive iterations without
         trust-region update. The switching is non-reversible. The iterative
         scheme is initialized and updated rom the beginning, but only
         employed after the specified number of iterations.
 
@@ -278,25 +311,32 @@
             Number of iterations without trust region update after which
             switch occurs.
         """
         self.switch_iteration: int = switch_iteration
         super(HybridFixed, self).__init__(happ)
         self._switched = False
 
-    def update(self, s: np.ndarray, y: np.ndarray, hess: np.ndarray,
-               iter_since_tr_update: int):
+    def update(
+        self,
+        s: np.ndarray,
+        y: np.ndarray,
+        hess: np.ndarray,
+        iter_since_tr_update: int,
+    ):
         self._switched_update(s, y, hess)
         if not self._switched:
             self._switched = iter_since_tr_update >= self.switch_iteration
 
 
 class HybridFraction(HybridSwitchApproximation):
-    def __init__(self,
-                 happ: IterativeHessianApproximation = BFGS(),
-                 switch_threshold: Optional[float] = 0.8):
+    def __init__(
+        self,
+        happ: IterativeHessianApproximation = BFGS(),
+        switch_threshold: Optional[float] = 0.8,
+    ):
         """
         Switch from a dynamic approximation to the user provided iterative
         scheme as soon as the fraction of iterations where the step is
         accepted but the trust region is not update exceeds the user provided
         threshold.Threshold check is only performed after 25 iterations.
         The switching is  non-reversible. The iterative scheme is
         initialized and updated rom the beginning, but only employed after
@@ -309,25 +349,33 @@
             trust region is not updated, which when exceeded triggers switch
             of approximation.
         """
         self.switch_threshold: float = switch_threshold
         super(HybridFraction, self).__init__(happ)
         self._switched = False
 
-    def update(self, s: np.ndarray, y: np.ndarray, hess: np.ndarray,
-               tr_nonupdates: int, iterations: int):
+    def update(
+        self,
+        s: np.ndarray,
+        y: np.ndarray,
+        hess: np.ndarray,
+        tr_nonupdates: int,
+        iterations: int,
+    ):
         self._switched_update(s, y, hess)
         if not self._switched and iterations > 25:
-            self._switched = tr_nonupdates/iterations > self.switch_threshold
+            self._switched = tr_nonupdates / iterations > self.switch_threshold
 
 
 class FX(HybridApproximation):
-    def __init__(self,
-                 happ: IterativeHessianApproximation = BFGS(),
-                 hybrid_tol: Optional[float] = 0.2):
+    def __init__(
+        self,
+        happ: IterativeHessianApproximation = BFGS(),
+        hybrid_tol: Optional[float] = 0.2,
+    ):
         r"""
         Hybrid method HY2 as introduced by
         [Fletcher & Xu 1986](https://doi.org/10.1093/imanum/7.3.371). This
         approximation scheme employs a dynamic approximation as long as
         function values satisfy :math:`\frac{f_k - f_{k+1}}{f_k} < \epsilon`
         and employs the iterative scheme applied to the last dynamic
         approximation if not.
@@ -336,16 +384,22 @@
 
         :param hybrid_tol:
             switch tolerance :math:`\epsilon`
         """
         self.hybrid_tol = hybrid_tol
         super(FX, self).__init__(happ)
 
-    def update(self, delta: np.ndarray, gamma: np.ndarray,
-               r: np.ndarray, rprev: np.ndarray, hess: np.ndarray) -> None:
+    def update(
+        self,
+        delta: np.ndarray,
+        gamma: np.ndarray,
+        r: np.ndarray,
+        rprev: np.ndarray,
+        hess: np.ndarray,
+    ) -> None:
         """
         Update the Hessian approximation
 
         :param delta:
             step in optimization variables
 
         :param gamma:
@@ -357,15 +411,15 @@
         :param rprev:
             residuals befor current step
 
         :param hess:
             user-provided (Gauss-Newton) Hessian approximation
         """
         # Equation (3.5)
-        ratio = (rprev.dot(rprev) - r.dot(r))/rprev.dot(rprev)
+        ratio = (rprev.dot(rprev) - r.dot(r)) / rprev.dot(rprev)
         if ratio >= self.hybrid_tol:
             self._diff = hess - self.hessian_update.get_mat()
             self.hessian_update.set_mat(hess)
         else:
             self.hessian_update.update(delta, gamma)
             self._diff = self.hessian_update.get_diff()
 
@@ -374,16 +428,19 @@
 
     @property
     def requires_resfun(self) -> bool:
         return True  # pragma: no cover
 
 
 class StructuredApproximation(HessianApproximation):
-    def __init__(self, phi: Optional[float] = 0.0,
-                 enforce_curv_cond: Optional[bool] = True):
+    def __init__(
+        self,
+        phi: Optional[float] = 0.0,
+        enforce_curv_cond: Optional[bool] = True,
+    ):
         """
         This is the base class for structured secant methods (SSM). SSMs
         approximate the hessian by combining the Gauss-Newton component C(x)
         and an iteratively updated component that approximates the
         difference S to the true Hessian.
 
         :parameter phi:
@@ -397,26 +454,34 @@
             discarded.
         """
         self.A: np.ndarray = np.empty(0)
         self.phi = phi
         self.enforce_curv_cond = enforce_curv_cond
         self._structured_diff = np.empty(0)
         if phi < 0 or phi > 1:
-            warnings.warn('Setting phi to values outside the interval [0, 1]'
-                          'will not guarantee that positive definiteness is '
-                          'preserved during updating.')
+            warnings.warn(
+                'Setting phi to values outside the interval [0, 1]'
+                'will not guarantee that positive definiteness is '
+                'preserved during updating.'
+            )
         super(StructuredApproximation, self).__init__(init_with_hess=True)
 
     def init_mat(self, dim: int, hess: Optional[np.ndarray] = None):
         self.A = np.eye(dim) * np.spacing(1)
         self._structured_diff = np.zeros_like(self.A)
         super(StructuredApproximation, self).init_mat(dim, hess)
 
-    def update(self, s: np.ndarray, y: np.ndarray, r: np.ndarray,
-               hess: np.ndarray, yb: np.ndarray) -> None:
+    def update(
+        self,
+        s: np.ndarray,
+        y: np.ndarray,
+        r: np.ndarray,
+        hess: np.ndarray,
+        yb: np.ndarray,
+    ) -> None:
         """
         Update the structured approximation
 
         :param s:
             step in optimization parameters
         :param y:
             step in gradient parameters
@@ -446,16 +511,22 @@
     Structured Secant Method as introduced by
     [Dennis et al 1989](https://doi.org/10.1007/BF00962795), which is
     compatible with BFGS, DFP update schemes.
 
     This scheme only works with a function that returns (res, sres)
     """
 
-    def update(self, s: np.ndarray, y: np.ndarray, r: np.ndarray,
-               hess: np.ndarray, yb: np.ndarray) -> None:
+    def update(
+        self,
+        s: np.ndarray,
+        y: np.ndarray,
+        r: np.ndarray,
+        hess: np.ndarray,
+        yb: np.ndarray,
+    ) -> None:
         # B^S = A + C(x_+)
         Bs = hess + self.A
         # y^S = y^# + C(x_+)*s
         ys = yb + hess.dot(s)
         # Equation (13)
         self._structured_diff = broyden_class_update(
             ys, s, Bs, phi=self.phi, enforce_curv_cond=self.enforce_curv_cond
@@ -470,71 +541,90 @@
     Totally Structured Secant Method as introduced by
     [Huschens 1994](https://doi.org/10.1137/0804005), which uses a
     self-adjusting update method for the second order term.
 
     This scheme only works with a function that returns (res, sres)
     """
 
-    def update(self, s: np.ndarray, y: np.ndarray, r: np.ndarray,
-               hess: np.ndarray, yb: np.ndarray) -> None:
+    def update(
+        self,
+        s: np.ndarray,
+        y: np.ndarray,
+        r: np.ndarray,
+        hess: np.ndarray,
+        yb: np.ndarray,
+    ) -> None:
         # Equation (2.7)
         Bs = hess + norm(r) * self.A
         # Equation (2.6)
         ys = hess.dot(s) + yb
         # Equation (2.10)
         self._structured_diff = broyden_class_update(
             ys, s, Bs, phi=self.phi, enforce_curv_cond=self.enforce_curv_cond
-        )/norm(r)
+        ) / norm(r)
         self.A += self._structured_diff
         # Equation (2.9)
         self._update_hess_and_store_diff(hess + norm(r) * self.A)
 
 
 class GNSBFGS(StructuredApproximation):
-    def __init__(self, hybrid_tol: float = 1e-6,
-                 enforce_curv_cond: bool = True):
+    def __init__(
+        self, hybrid_tol: float = 1e-6, enforce_curv_cond: bool = True
+    ):
         """
         Hybrid Gauss-Newton Structured BFGS method as introduced by
         [Zhou & Chen 2010](https://doi.org/10.1137/090748470),
         which combines ideas of hybrid switching methods and structured
         secant methods.
 
         This scheme only works with a function that returns (res, sres)
 
         :parameter hybrid_tol:
             switching tolerance that controls switching between update methods
         """
         self.hybrid_tol: float = hybrid_tol
-        super(GNSBFGS, self).__init__(phi=0.0,
-                                      enforce_curv_cond=enforce_curv_cond)
+        super(GNSBFGS, self).__init__(
+            phi=0.0, enforce_curv_cond=enforce_curv_cond
+        )
 
-    def update(self, s: np.ndarray, y: np.ndarray, r: np.ndarray,
-               hess: np.ndarray, yb: np.ndarray) -> None:
+    def update(
+        self,
+        s: np.ndarray,
+        y: np.ndarray,
+        r: np.ndarray,
+        hess: np.ndarray,
+        yb: np.ndarray,
+    ) -> None:
         # Equation (2.1)
-        ratio = yb.T.dot(s)/s.dot(s)
+        ratio = yb.T.dot(s) / s.dot(s)
         if ratio > self.hybrid_tol:
             # Equation (2.3)
             self._structured_diff = broyden_class_update(
-                yb, s, self.A, phi=self.phi,
-                enforce_curv_cond=self.enforce_curv_cond
+                yb,
+                s,
+                self.A,
+                phi=self.phi,
+                enforce_curv_cond=self.enforce_curv_cond,
             )
             self.A += self._structured_diff
             # Equation (2.2)
             self._update_hess_and_store_diff(hess + self.A)
         else:
             # Equation (2.2)
             self._structured_diff = np.zeros_like(self.A)
             self._update_hess_and_store_diff(hess + norm(r) * np.eye(len(y)))
 
 
-def broyden_class_update(y: np.ndarray,
-                         s: np.ndarray,
-                         mat: np.ndarray,
-                         phi: float = 0.0,
-                         enforce_curv_cond: bool = True) -> np.ndarray:
+def broyden_class_update(
+    y: np.ndarray,
+    s: np.ndarray,
+    mat: np.ndarray,
+    phi: float = 0.0,
+    enforce_curv_cond: bool = True,
+) -> np.ndarray:
     """
     Scale free implementation of the broyden class update scheme.
 
     :param y:
         difference in gradient
     :param s:
         search direction in previous step
```

### Comparing `fides-0.7.7/fides/logging.py` & `fides-0.7.8/fides/logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,13 +28,13 @@
     logger_count += 1
     # add logger count to differentiate between different fides
     # optimization instances and avoid deadlocks
     logger = logging.getLogger(f'fides_{logger_count}')
     ch = logging.StreamHandler()
     formatter = logging.Formatter(
         fmt='%(asctime)s fides(%(levelname)s) %(message)s',
-        datefmt='%Y-%m-%d %H:%M:%S'
+        datefmt='%Y-%m-%d %H:%M:%S',
     )
     ch.setFormatter(formatter)
     logger.addHandler(ch)
     logger.setLevel(level)
     return logger
```

### Comparing `fides-0.7.7/fides/minimize.py` & `fides-0.7.8/fides/minimize.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,123 +1,161 @@
 """
 Minimization
 ------------
 This module performs the optimization given a step proposal.
 """
 
-import time
-
-import numpy as np
 import logging
+import time
 import uuid
+from collections import defaultdict
+from typing import Callable, Dict, List, Optional, Tuple, Union
+
 import h5py
+import numpy as np
 from numpy.linalg import norm
 from scipy.sparse import csc_matrix
-from .trust_region import trust_region, Step
-from .hessian_approximation import (
-    HessianApproximation, StructuredApproximation, HybridFixed,
-    HybridFraction, FX, IterativeHessianApproximation, TSSM, GNSBFGS
-)
+
 from .constants import (
-    Options, ExitFlag, DEFAULT_OPTIONS, StepBackStrategy, SubSpaceDim,
-    validate_options
+    DEFAULT_OPTIONS,
+    ExitFlag,
+    Options,
+    StepBackStrategy,
+    SubSpaceDim,
+    validate_options,
+)
+from .hessian_approximation import (
+    FX,
+    GNSBFGS,
+    TSSM,
+    HessianApproximation,
+    HybridFixed,
+    HybridFraction,
+    IterativeHessianApproximation,
+    StructuredApproximation,
 )
 from .logging import create_logger
-from collections import defaultdict
-from typing import Callable, Dict, Optional, Tuple, Union, List
+from .trust_region import Step, trust_region
 
 
 class FunEvaluator:
-    def __init__(self, fun: Callable, nargout: int, resfun: bool,
-                 funargs: dict):
+    def __init__(
+        self, fun: Callable, nargout: int, resfun: bool, funargs: dict
+    ):
         self.fun = fun
         self.nargout = nargout
         self.resfun = resfun
         if funargs is None:
             funargs = {}
         self.funargs = funargs
 
     def __call__(self, x: np.ndarray):
         ret = self.fun(x, **self.funargs)
 
         if not isinstance(ret, tuple) or len(ret) != self.nargout:
             nargout = len(ret) if isinstance(ret, tuple) else 1
-            raise ValueError(f'Provided function returned {nargout} values, '
-                             f'but was expected to return {self.nargout}.'
-                             f'Please make sure the provided function is '
-                             f'compatible with the employed Hessian '
-                             f'Approximation Scheme. If no Hessian '
-                             f'Approximation Scheme is employed, the function '
-                             f'needs to return 3 values (fval, grad, hess).')
+            raise ValueError(
+                f'Provided function returned {nargout} values, '
+                f'but was expected to return {self.nargout}.'
+                f'Please make sure the provided function is '
+                f'compatible with the employed Hessian '
+                f'Approximation Scheme. If no Hessian '
+                f'Approximation Scheme is employed, the function '
+                f'needs to return 3 values (fval, grad, hess).'
+            )
 
         if self.resfun:
             res, sres = ret
-            return Funout(fval=0.5 * res.T.dot(res), grad=res.T.dot(sres),
-                          hess=sres.T.dot(sres), res=res, sres=sres, x=x)
+            return Funout(
+                fval=0.5 * res.T.dot(res),
+                grad=res.T.dot(sres),
+                hess=sres.T.dot(sres),
+                res=res,
+                sres=sres,
+                x=x,
+            )
         else:
             if self.nargout == 3:
                 fval, grad, hess = ret
                 return Funout(fval=fval, grad=grad, hess=hess, x=x)
             else:
                 fval, grad = ret
                 return Funout(fval=fval, grad=grad, x=x)
 
 
 class Funout:
-    def __init__(self, fval: float, grad: np.ndarray, x: np.ndarray,
-                 hess: Optional[np.ndarray] = None,
-                 res: Optional[np.ndarray] = None,
-                 sres: Optional[np.ndarray] = None,):
+    def __init__(
+        self,
+        fval: float,
+        grad: np.ndarray,
+        x: np.ndarray,
+        hess: Optional[np.ndarray] = None,
+        res: Optional[np.ndarray] = None,
+        sres: Optional[np.ndarray] = None,
+    ):
         self.fval = fval
         self.grad = grad
         self.hess = hess
         self.x = x
         self.res = res
         self.sres = sres
 
     def checkdims(self):
         if not np.isscalar(self.fval):
-            raise ValueError('Provided objective function must return a '
-                             'scalar!')
+            raise ValueError(
+                'Provided objective function must return a ' 'scalar!'
+            )
 
         if np.isscalar(self.grad):
-            raise ValueError('Provided objective function gradient must '
-                             'return a vector!')
+            raise ValueError(
+                'Provided objective function gradient must ' 'return a vector!'
+            )
 
         if not self.grad.ndim == 1:
-            raise ValueError('Provided objective function must return a '
-                             'gradient vector with x.ndim == 1, was '
-                             f'{self.grad.ndim}!')
+            raise ValueError(
+                'Provided objective function must return a '
+                'gradient vector with x.ndim == 1, was '
+                f'{self.grad.ndim}!'
+            )
         if not len(self.grad) == len(self.x):
-            raise ValueError('Provided objective function must return a '
-                             'gradient vector of the same shape as x, '
-                             f'x has {len(self.x)} entries but gradient has '
-                             f'{len(self.grad)}!')
+            raise ValueError(
+                'Provided objective function must return a '
+                'gradient vector of the same shape as x, '
+                f'x has {len(self.x)} entries but gradient has '
+                f'{len(self.grad)}!'
+            )
 
         if self.hess is None:
             return
 
         if np.isscalar(self.hess):
-            raise ValueError('Provided objective function Hessian must '
-                             'return a matrix!')
+            raise ValueError(
+                'Provided objective function Hessian must ' 'return a matrix!'
+            )
 
         if not self.hess.ndim == 2:
-            raise ValueError('Provided objective function must return a '
-                             'Hessian matrix with x.ndim == 2, was '
-                             f'{self.hess.ndim}!')
+            raise ValueError(
+                'Provided objective function must return a '
+                'Hessian matrix with x.ndim == 2, was '
+                f'{self.hess.ndim}!'
+            )
 
         if not self.hess.shape[0] == self.hess.shape[1]:
-            raise ValueError('Provided objective function must return a '
-                             'square Hessian matrix!')
+            raise ValueError(
+                'Provided objective function must return a '
+                'square Hessian matrix!'
+            )
 
         if not self.hess.shape[0] == len(self.x):
-            raise ValueError('Provided objective function must return a '
-                             'square Hessian matrix with same dimension as x. '
-                             f'x has {len(self.x)} entries but Hessian has '
-                             f'{self.hess.shape[0]}!')
+            raise ValueError(
+                'Provided objective function must return a '
+                'square Hessian matrix with same dimension as x. '
+                f'x has {len(self.x)} entries but Hessian has '
+                f'{self.hess.shape[0]}!'
+            )
 
     def __repr__(self):
         return f'Funout(fval={self.fval}, grad={self.grad}, hess={self.hess})'
 
 
 class Optimizer:
     """
@@ -140,23 +178,26 @@
     :ivar starttime: Time at which optimization was started
     :ivar iteration: Current iteration
     :ivar converged: Flag indicating whether optimization has converged
     :ivar exitflag: ExitFlag to indicate reason for termination
     :ivar verbose: Verbosity level for logging
     :ivar logger: logger instance
     """
-    def __init__(self,
-                 fun: Callable,
-                 ub: np.ndarray,
-                 lb: np.ndarray,
-                 verbose: Optional[int] = logging.INFO,
-                 options: Optional[Dict] = None,
-                 funargs: Optional[Dict] = None,
-                 hessian_update: Optional[HessianApproximation] = None,
-                 resfun: bool = False):
+
+    def __init__(
+        self,
+        fun: Callable,
+        ub: np.ndarray,
+        lb: np.ndarray,
+        verbose: Optional[int] = logging.INFO,
+        options: Optional[Dict] = None,
+        funargs: Optional[Dict] = None,
+        hessian_update: Optional[HessianApproximation] = None,
+        resfun: bool = False,
+    ):
         """
         Create an optimizer object
 
         :param fun:
             This is the objective function, if no `hessian_update` is
             provided, this function must return a tuple (fval, grad),
             otherwise this function must return a tuple (fval, grad, Hessian).
@@ -179,44 +220,58 @@
         :param hessian_update:
             Subclass of :py:class:`fides.hessian_update.HessianApproximation`
             that performs the hessian updates in every iteration.
         :param resfun:
             Boolean flag indicating whether fun returns function values
             (False, default) or residuals (True).
         """
-        nargout = 3 if hessian_update is None or (
-            hessian_update.requires_hess and not hessian_update.requires_resfun
-        ) else 2
-
-        self.fevaler = FunEvaluator(fun=fun, nargout=nargout, resfun=resfun,
-                                    funargs=funargs)
-
-        if hessian_update is not None and \
-                resfun != hessian_update.requires_resfun:
-            raise ValueError(f'Hessian update scheme {type(hessian_update)} '
-                             f'requires an objective function that returns '
-                             f'(residual, residual derivative). Please make'
-                             f'sure that is the case and then call this '
-                             f'function with argument resfun set to `True`.')
+        nargout = (
+            3
+            if hessian_update is None
+            or (
+                hessian_update.requires_hess
+                and not hessian_update.requires_resfun
+            )
+            else 2
+        )
+
+        self.fevaler = FunEvaluator(
+            fun=fun, nargout=nargout, resfun=resfun, funargs=funargs
+        )
+
+        if (
+            hessian_update is not None
+            and resfun != hessian_update.requires_resfun
+        ):
+            raise ValueError(
+                f'Hessian update scheme {type(hessian_update)} '
+                f'requires an objective function that returns '
+                f'(residual, residual derivative). Please make'
+                f'sure that is the case and then call this '
+                f'function with argument resfun set to `True`.'
+            )
 
         self.lb: np.ndarray = np.array(lb)
         self.ub: np.ndarray = np.array(ub)
 
         if options is None:
             options = {}
 
         validate_options(options)
 
         self.options: Dict = options
 
-        if (self.get_option(Options.SUBSPACE_DIM) == SubSpaceDim.STEIHAUG and
-                self.get_option(Options.STEPBACK_STRAT) ==
-                StepBackStrategy.REFINE):
-            raise ValueError('Selected base step is not compatible with '
-                             'refinement.')
+        if (
+            self.get_option(Options.SUBSPACE_DIM) == SubSpaceDim.STEIHAUG
+            and self.get_option(Options.STEPBACK_STRAT)
+            == StepBackStrategy.REFINE
+        ):
+            raise ValueError(
+                'Selected base step is not compatible with ' 'refinement.'
+            )
 
         self.delta: float = self.get_option(Options.DELTA_INIT)
         self.delta_iter: float = self.delta
 
         self.tr_ratio: float = 1
 
         self.x: np.ndarray = np.empty(ub.shape)
@@ -233,16 +288,17 @@
 
         self.starttime: float = np.nan
         self.iteration: int = 0
         self.converged: bool = False
         self.exitflag: ExitFlag = ExitFlag.DID_NOT_RUN
         self.verbose: int = verbose
         self.logger: Union[logging.Logger, None] = None
-        self.history: Dict[str, List[Union[float, int, bool]]] = \
-            defaultdict(list)
+        self.history: Dict[str, List[Union[float, int, bool]]] = defaultdict(
+            list
+        )
         self.start_id: str = ''
 
     def _reset(self, start_id: Optional[str] = None):
         self.starttime = time.time()
         self.iteration = 0
         self.iterations_since_tr_update = 0
         self.n_intermediate_tr_radius = 0
@@ -311,27 +367,35 @@
         while self.check_continue():
             self.iteration += 1
             self.delta_iter = self.delta
 
             v, dv = self.get_affine_scaling()
 
             scaling = csc_matrix(np.diag(np.sqrt(np.abs(v))))
-            theta = max(self.get_option(Options.THETA_MAX),
-                        1 - norm(v * self.grad, np.inf))
+            theta = max(
+                self.get_option(Options.THETA_MAX),
+                1 - norm(v * self.grad, np.inf),
+            )
 
             self.check_finite()
 
-            step = \
-                trust_region(
-                    self.x, self.grad, self.hess, scaling,
-                    self.delta_iter, dv, theta, self.lb, self.ub,
-                    subspace_dim=self.get_option(Options.SUBSPACE_DIM),
-                    stepback_strategy=self.get_option(Options.STEPBACK_STRAT),
-                    logger=self.logger
-                )
+            step = trust_region(
+                self.x,
+                self.grad,
+                self.hess,
+                scaling,
+                self.delta_iter,
+                dv,
+                theta,
+                self.lb,
+                self.ub,
+                subspace_dim=self.get_option(Options.SUBSPACE_DIM),
+                stepback_strategy=self.get_option(Options.STEPBACK_STRAT),
+                logger=self.logger,
+            )
 
             x_new = self.x + step.s + step.s0
             funout_new = self.fevaler(x_new)
 
             if np.isfinite(funout_new.fval):
                 self.check_finite(funout_new)
 
@@ -371,18 +435,15 @@
 
         """
         if np.isfinite(funout.fval) and funout.fval < self.fval_min:
             self.x_min = funout.x
             self.fval_min = funout.fval
             self.grad_min = funout.grad
 
-    def update(self,
-               step: Step,
-               funout_new: Funout,
-               funout: Funout) -> None:
+    def update(self, step: Step, funout_new: Funout, funout: Funout) -> None:
         """
         Update self according to employed step
 
         :param step:
             Employed step
 
         :param funout:
@@ -397,59 +458,68 @@
             s = step.s + step.s0
             y = funout_new.grad - self.grad
 
             if isinstance(self.hessian_update, IterativeHessianApproximation):
                 self.hessian_update.update(s=s, y=y)
             elif isinstance(self.hessian_update, HybridFixed):
                 self.hessian_update.update(
-                    s=s, y=y, hess=funout_new.hess,
-                    iter_since_tr_update=self.iterations_since_tr_update
+                    s=s,
+                    y=y,
+                    hess=funout_new.hess,
+                    iter_since_tr_update=self.iterations_since_tr_update,
                 )
             elif isinstance(self.hessian_update, HybridFraction):
                 self.hessian_update.update(
-                    s=s, y=y, hess=funout_new.hess,
+                    s=s,
+                    y=y,
+                    hess=funout_new.hess,
                     tr_nonupdates=self.n_intermediate_tr_radius,
-                    iterations=self.iteration
+                    iterations=self.iteration,
                 )
             elif isinstance(self.hessian_update, FX):
                 # Equation (1.16)
                 # A = sres
                 # M = hess
                 # \delta = s
                 # r = res
-                gamma = funout_new.hess.dot(s) + \
-                        (funout_new.sres - funout.sres).T.dot(funout_new.res)
-                self.hessian_update.update(delta=s, gamma=gamma,
-                                           r=funout_new.res, rprev=funout.res,
-                                           hess=funout_new.hess)
+                gamma = funout_new.hess.dot(s) + (
+                    funout_new.sres - funout.sres
+                ).T.dot(funout_new.res)
+                self.hessian_update.update(
+                    delta=s,
+                    gamma=gamma,
+                    r=funout_new.res,
+                    rprev=funout.res,
+                    hess=funout_new.hess,
+                )
             elif isinstance(self.hessian_update, StructuredApproximation):
                 # SSM: Equation (43) in [Dennis et al 1989]
                 yb = (funout_new.sres - funout.sres).T.dot(funout_new.res)
                 if isinstance(self.hessian_update, (TSSM, GNSBFGS)):
                     # TSSM: Equation (2.5)/(2.6) in [Huschens 1994]
                     # GNSBFGS: Equation (2.1) in [Zhou & Chen 2010]
-                    yb *= norm(funout_new.res)/norm(funout.res)
-                self.hessian_update.update(s=s, y=y, yb=yb, r=funout_new.res,
-                                           hess=funout_new.hess)
+                    yb *= norm(funout_new.res) / norm(funout.res)
+                self.hessian_update.update(
+                    s=s, y=y, yb=yb, r=funout_new.res, hess=funout_new.hess
+                )
             else:
                 raise NotImplementedError
 
             self.hess = self.hessian_update.get_mat()
         else:
             self.hess = funout_new.hess.copy()
         self.check_in_bounds(funout_new.x)
         self.fval = funout_new.fval
         self.x = funout_new.x
         self.grad = funout_new.grad
         self.make_non_degenerate()
 
-    def update_tr_radius(self,
-                         funout: Funout,
-                         step: Step,
-                         dv: np.ndarray) -> bool:
+    def update_tr_radius(
+        self, funout: Funout, step: Step, dv: np.ndarray
+    ) -> bool:
         """
         Update the trust region radius
 
         :param funout:
             Function output generated by a :py:class:`FunEvaluator` for new
             variables after step is taken
 
@@ -464,45 +534,48 @@
         """
         fval, grad = funout.fval, funout.grad
         stepsx = step.ss + step.ss0
         nsx = norm(stepsx)
         self.iterations_since_tr_update += 1
         if not np.isfinite(fval):
             self.tr_ratio = 0
-            self.delta = np.nanmin([
-                self.delta * self.get_option(Options.GAMMA1),
-                nsx / 4
-            ])
+            self.delta = np.nanmin(
+                [self.delta * self.get_option(Options.GAMMA1), nsx / 4]
+            )
             self.iterations_since_tr_update = 0
             return False
         else:
             aug = 0.5 * stepsx.dot(dv * np.abs(grad) * stepsx)
             actual_decrease = self.fval - fval - aug
             predicted_decrease = -step.qpval
             if predicted_decrease <= 0.0:
                 self.tr_ratio = 0.0
             else:
                 self.tr_ratio = actual_decrease / predicted_decrease
 
             interior_solution = nsx < self.delta_iter * 0.9
 
-            if self.tr_ratio >= self.get_option(Options.ETA) \
-                    and not interior_solution:
+            if (
+                self.tr_ratio >= self.get_option(Options.ETA)
+                and not interior_solution
+            ):
                 # increase radius
                 self.delta = self.get_option(Options.GAMMA2) * self.delta
                 self.iterations_since_tr_update = 0
             elif self.tr_ratio <= self.get_option(Options.MU):
                 # decrease radius
-                self.delta = np.nanmin([
-                    self.delta * self.get_option(Options.GAMMA1),
-                    nsx / 4
-                ])
+                self.delta = np.nanmin(
+                    [self.delta * self.get_option(Options.GAMMA1), nsx / 4]
+                )
                 self.iterations_since_tr_update = 0
-            elif self.get_option(Options.MU) < self.tr_ratio < \
-                    self.get_option(Options.ETA):
+            elif (
+                self.get_option(Options.MU)
+                < self.tr_ratio
+                < self.get_option(Options.ETA)
+            ):
                 self.n_intermediate_tr_radius += 1
             return self.tr_ratio > 0.0
 
     def check_convergence(self, step: Step, funout: Funout) -> None:
         """
         Check whether optimization has converged.
 
@@ -520,16 +593,17 @@
         xtol = self.get_option(Options.XTOL)
         gatol = self.get_option(Options.GATOL)
         grtol = self.get_option(Options.GRTOL)
         gnorm = norm(grad)
         stepsx = step.ss + step.ss0
         nsx = norm(stepsx)
 
-        if self.tr_ratio > self.get_option(Options.MU) and \
-                np.abs(fval - self.fval) < fatol + frtol*np.abs(self.fval):
+        if self.tr_ratio > self.get_option(Options.MU) and np.abs(
+            fval - self.fval
+        ) < fatol + frtol * np.abs(self.fval):
             self.exitflag = ExitFlag.FTOL
             self.logger.info(
                 'Stopping as function difference '
                 f'{np.abs(self.fval - fval):.2E} was smaller than specified '
                 f'tolerances (atol={fatol:.2E}, rtol={frtol:.2E})'
             )
             converged = True
@@ -582,15 +656,15 @@
                 f'exceeded.'
             )
             return False
 
         time_elapsed = time.time() - self.starttime
         maxtime = self.get_option(Options.MAXTIME)
         time_remaining = maxtime - time_elapsed
-        avg_iter_time = time_elapsed/(self.iteration + (self.iteration == 0))
+        avg_iter_time = time_elapsed / (self.iteration + (self.iteration == 0))
         if time_remaining < avg_iter_time:
             self.exitflag = ExitFlag.MAXTIME
             self.logger.warning(
                 f'Stopping as maximum runtime {maxtime} is expected to be '
                 f'exceeded in the next iteration.'
             )
             return False
@@ -608,16 +682,18 @@
     def make_non_degenerate(self, eps=1e2 * np.spacing(1)) -> None:
         """
         Ensures that x is non-degenerate, this should only be necessary for
         initial points.
 
         :param eps: degeneracy threshold
         """
-        if np.min(np.abs(self.ub - self.x)) < eps or \
-                np.min(np.abs(self.x - self.lb)) < eps:
+        if (
+            np.min(np.abs(self.ub - self.x)) < eps
+            or np.min(np.abs(self.x - self.lb)) < eps
+        ):
             upperi = (self.ub - self.x) < eps
             loweri = (self.x - self.lb) < eps
             self.x[upperi] = self.x[upperi] - eps
             self.x[loweri] = self.x[loweri] + eps
 
     def get_affine_scaling(self) -> Tuple[np.ndarray, np.ndarray]:
         """
@@ -655,16 +731,19 @@
 
         :param funout:
             Function output generated by a :py:class:`FunEvaluator`
         """
         normdx = norm(step.s + step.s0)
         normg = norm(self.grad)
 
-        iterspaces = max(len(str(self.get_option(Options.MAXITER))), 5) - \
-            len(str(self.iteration)) - 1
+        iterspaces = (
+            max(len(str(self.get_option(Options.MAXITER))), 5)
+            - len(str(self.iteration))
+            - 1
+        )
         steptypespaces = 4 - len(step.type)
 
         fval = funout.fval
         if not np.isfinite(fval):
             fval = self.fval
         self.logger.info(
             f'{" " * iterspaces}{self.iteration}'
@@ -683,25 +762,25 @@
         normg = norm(self.grad)
 
         min_ev_hess, max_ev_hess = _min_max_evs(self.hess)
         min_ev_hess_update, max_ev_hess_update = np.NaN, np.NaN
         min_ev_hess_supdate, max_ev_hess_supdate = np.NaN, np.NaN
         if self.hessian_update:
             if accepted:
-                min_ev_hess_update, max_ev_hess_update = \
-                    _min_max_evs(self.hessian_update.get_diff())
+                min_ev_hess_update, max_ev_hess_update = _min_max_evs(
+                    self.hessian_update.get_diff()
+                )
             else:
                 min_ev_hess_update, max_ev_hess_update = 0.0, 0.0
 
             if isinstance(self.hessian_update, StructuredApproximation):
                 if accepted:
-                    min_ev_hess_supdate, max_ev_hess_supdate = \
-                        _min_max_evs(
-                            self.hessian_update.get_structured_diff()
-                        )
+                    min_ev_hess_supdate, max_ev_hess_supdate = _min_max_evs(
+                        self.hessian_update.get_structured_diff()
+                    )
                 else:
                     min_ev_hess_supdate, max_ev_hess_supdate = 0.0, 0.0
 
         update = {
             'fval': funout.fval,
             'tr_ratio': self.tr_ratio,
             'tr_radius': self.delta_iter,
@@ -730,16 +809,19 @@
             self.history[key].append(val)
 
     def log_step_initial(self):
         """
         Prints diagnostic information about the initial step to the log
         """
 
-        iterspaces = max(len(str(self.get_option(Options.MAXITER))), 5) - \
-            len(str(self.iteration)) - 1
+        iterspaces = (
+            max(len(str(self.get_option(Options.MAXITER))), 5)
+            - len(str(self.iteration))
+            - 1
+        )
         self.logger.info(
             f'{" " * iterspaces}{self.iteration}'
             f'| {self.fval:+.2E} '
             f'|    NaN   '
             f'|    NaN   '
             f'| {self.delta:.1E} '
             f'| {norm(self.grad):.1E} '
@@ -781,33 +863,39 @@
         if funout is not None:
             fval, grad, hess = funout.fval, funout.grad, funout.hess
         else:
             fval, grad, hess = self.fval, self.grad, self.hess
 
         if not np.isfinite(fval):
             self.exitflag = ExitFlag.NOT_FINITE
-            raise RuntimeError(f'Encountered non-finite function {self.fval} '
-                               f'value {pointstr}')
+            raise RuntimeError(
+                f'Encountered non-finite function {self.fval} '
+                f'value {pointstr}'
+            )
 
         if not np.isfinite(grad).all():
             self.exitflag = ExitFlag.NOT_FINITE
             ix = np.where(np.logical_not(np.isfinite(grad)))
-            raise RuntimeError('Encountered non-finite gradient entries'
-                               f' {grad[ix]} for indices {ix} '
-                               f'{pointstr}')
+            raise RuntimeError(
+                'Encountered non-finite gradient entries'
+                f' {grad[ix]} for indices {ix} '
+                f'{pointstr}'
+            )
 
         if hess is None:
             return
 
         if not np.isfinite(hess).all():
             self.exitflag = ExitFlag.NOT_FINITE
             ix = np.where(np.logical_not(np.isfinite(hess)))
-            raise RuntimeError('Encountered non-finite gradient hessian'
-                               f' {hess[ix]} for indices {ix} '
-                               f'{pointstr}')
+            raise RuntimeError(
+                'Encountered non-finite gradient hessian'
+                f' {hess[ix]} for indices {ix} '
+                f'{pointstr}'
+            )
 
     def check_in_bounds(self, x: Optional[np.ndarray] = None):
         """
         Checks whether the current optimization variables are all within the
         specified boundaries
 
         :raises:
@@ -817,23 +905,25 @@
             x = self.x
 
         if self.iteration == 0:
             pointstr = 'at initial point.'
         else:
             pointstr = f'at iteration {self.iteration}.'
 
-        for ref, sign, name in zip([self.ub, self.lb],
-                                   [-1.0, 1.0],
-                                   ['upper bounds', 'lower bounds']):
+        for ref, sign, name in zip(
+            [self.ub, self.lb], [-1.0, 1.0], ['upper bounds', 'lower bounds']
+        ):
             diff = sign * (ref - x)
             if not np.all(diff <= 0):
                 ix = np.where(diff > 0)[0]
                 self.exitflag = ExitFlag.EXCEEDED_BOUNDARY
-                raise RuntimeError(f'Exceeded {name} for indices {ix} by '
-                                   f'{diff[ix]} {pointstr}')
+                raise RuntimeError(
+                    f'Exceeded {name} for indices {ix} by '
+                    f'{diff[ix]} {pointstr}'
+                )
 
     def get_option(self, option):
         return self.options.get(option, DEFAULT_OPTIONS.get(option))
 
 
 def _min_max_evs(mat: np.ndarray):
     evs = np.linalg.eigvals(mat)
```

### Comparing `fides-0.7.7/fides/stepback.py` & `fides-0.7.8/fides/stepback.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 Trust Region StepBack
 -----------------------------
 This module provides the machinery to combine various step-back strategies
 that can be used to compute longer steps in case the initially proposed step
 had to be truncated due to non-compliance with boundary constraints.
 """
 
+from typing import List
+
 import numpy as np
 from scipy.sparse import csc_matrix
-from typing import List
 
 from .steps import Step, TRStepReflected, TRStepTruncated
 
 
-def stepback_reflect(tr_step: Step,
-                     x: np.ndarray,
-                     sg: np.ndarray,
-                     hess: np.ndarray,
-                     scaling: csc_matrix,
-                     g_dscaling: csc_matrix,
-                     delta: float,
-                     theta: float,
-                     ub: np.ndarray,
-                     lb: np.ndarray) -> List[Step]:
+def stepback_reflect(
+    tr_step: Step,
+    x: np.ndarray,
+    sg: np.ndarray,
+    hess: np.ndarray,
+    scaling: csc_matrix,
+    g_dscaling: csc_matrix,
+    delta: float,
+    theta: float,
+    ub: np.ndarray,
+    lb: np.ndarray,
+) -> List[Step]:
     """
     Compute new proposal steps according to a reflection strategy.
 
     :param tr_step:
         Reference trust region step that will be reflected
     :param x:
         Current values of the optimization variables
@@ -48,41 +51,45 @@
         lower optimization variable boundaries
     :param ub:
         upper optimization variable boundaries
 
     :return:
         New proposal steps
     """
-    rtr_step = TRStepReflected(x, sg, hess, scaling, g_dscaling, delta,
-                               theta, ub, lb, tr_step)
+    rtr_step = TRStepReflected(
+        x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, tr_step
+    )
     rtr_step.calculate()
     steps = [rtr_step]
     for ireflection in range(len(x) - 1):
         if rtr_step.alpha == 1.0:
             break
         # recursively add more reflections
         rtr_old = rtr_step
-        rtr_step = TRStepReflected(x, sg, hess, scaling, g_dscaling, delta,
-                                   theta, ub, lb, rtr_old)
+        rtr_step = TRStepReflected(
+            x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, rtr_old
+        )
         rtr_step.calculate()
         steps.append(rtr_step)
 
     return steps
 
 
-def stepback_truncate(tr_step: Step,
-                      x: np.ndarray,
-                      sg: np.ndarray,
-                      hess: np.ndarray,
-                      scaling: csc_matrix,
-                      g_dscaling: csc_matrix,
-                      delta: float,
-                      theta: float,
-                      ub: np.ndarray,
-                      lb: np.ndarray) -> List[Step]:
+def stepback_truncate(
+    tr_step: Step,
+    x: np.ndarray,
+    sg: np.ndarray,
+    hess: np.ndarray,
+    scaling: csc_matrix,
+    g_dscaling: csc_matrix,
+    delta: float,
+    theta: float,
+    ub: np.ndarray,
+    lb: np.ndarray,
+) -> List[Step]:
     """
     Compute new proposal steps according to a truncation strategy.
 
     :param tr_step:
         Reference trust region step that will be reflect
     :param x:
         Current values of the optimization variables
@@ -104,20 +111,22 @@
         lower optimization variable boundaries
     :param ub:
         upper optimization variable boundaries
 
     :return:
         New proposal steps
     """
-    rtt_step = TRStepTruncated(x, sg, hess, scaling, g_dscaling, delta,
-                               theta, ub, lb, tr_step)
+    rtt_step = TRStepTruncated(
+        x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, tr_step
+    )
     rtt_step.calculate()
     steps = [rtt_step]
     while rtt_step.subspace.shape[1] > 0:
         if rtt_step.alpha == 1.0:
             break
-        rtt_step = TRStepTruncated(x, sg, hess, scaling, g_dscaling, delta,
-                                   theta, ub, lb, rtt_step)
+        rtt_step = TRStepTruncated(
+            x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, rtt_step
+        )
         rtt_step.calculate()
         steps.append(rtt_step)
 
     return steps
```

### Comparing `fides-0.7.7/fides/steps.py` & `fides-0.7.8/fides/steps.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,40 +2,41 @@
 Trust Region Step Calculation
 -----------------------------
 This module provides the machinery to calculate different trust-region(
 -reflective) step proposals
 """
 
 
+from logging import Logger
+from typing import Union
+
 import numpy as np
 import scipy.linalg as linalg
-
 from numpy.linalg import norm
+from scipy.optimize import LinearConstraint, NonlinearConstraint, minimize
 from scipy.sparse import csc_matrix
-from scipy.optimize import NonlinearConstraint, LinearConstraint, minimize
 
-from logging import Logger
 from .subproblem import (
-    solve_1d_trust_region_subproblem, solve_nd_trust_region_subproblem,
-    get_1d_trust_region_boundary_solution, quadratic_form
+    get_1d_trust_region_boundary_solution,
+    quadratic_form,
+    solve_1d_trust_region_subproblem,
+    solve_nd_trust_region_subproblem,
 )
 
-from typing import Union
-
 
 def normalize(v: np.ndarray) -> None:
     """
     Inplace normalization of a vector
 
     :param v:
         vector to be normalized
     """
     nv = norm(v)
     if nv > 0:
-        v[:] = v/nv  # change inplace
+        v[:] = v / nv  # change inplace
 
 
 class Step:
     """
     Base class for the computation of a proposal step
 
     :ivar x: Current state of optimization variables
@@ -66,27 +67,30 @@
     :ivar reflection_indices: Indices of variables for which reflection was
         applied
     :ivar truncation_indices: Indices of variables for which truncation was
         applied
 
     :cvar type: Identifier that allows identification of subclasses
     """
+
     type = 'step'
 
-    def __init__(self,
-                 x: np.ndarray,
-                 sg: np.ndarray,
-                 hess: np.ndarray,
-                 scaling: csc_matrix,
-                 g_dscaling: csc_matrix,
-                 delta: float,
-                 theta: float,
-                 ub: np.ndarray,
-                 lb: np.ndarray,
-                 logger: Logger):
+    def __init__(
+        self,
+        x: np.ndarray,
+        sg: np.ndarray,
+        hess: np.ndarray,
+        scaling: csc_matrix,
+        g_dscaling: csc_matrix,
+        delta: float,
+        theta: float,
+        ub: np.ndarray,
+        lb: np.ndarray,
+        logger: Logger,
+    ):
         """
 
         :param x:
             Reference point
         :param sg:
             Gradient in rescaled coordinates
         :param hess:
@@ -130,16 +134,17 @@
         self.minbr: float = 1.0
         self.alpha: float = 1.0
         self.iminbr: np.ndarray = np.array([])
 
         self.qpval: float = 0.0
 
         # B_hat (Eq 2.5) [ColemanLi1996]
-        self.shess: np.ndarray = np.asarray(scaling * hess * scaling
-                                            + g_dscaling)
+        self.shess: np.ndarray = np.asarray(
+            scaling * hess * scaling + g_dscaling
+        )
 
         self.cg: Union[np.ndarray, None] = None
         self.chess: Union[np.ndarray, None] = None
         self.subspace: Union[np.ndarray, None] = None
 
         self.s0: np.ndarray = np.zeros(sg.shape)
         self.ss0: np.ndarray = np.zeros(sg.shape)
@@ -179,18 +184,23 @@
         nonzero = np.abs(self.s) > 0
         self.br = np.inf * np.ones(self.s.shape)
         if np.any(nonzero):
             # br quantifies the distance to the boundary normalized
             # by the proposed step, this indicates the fraction of the step
             # that would put the respective variable at the boundary
             # This is defined in [Coleman-Li1994] (3.1)
-            self.br[nonzero] = np.max(np.vstack([
-                (self.ub[nonzero] - self.x[nonzero])/self.s[nonzero],
-                (self.lb[nonzero] - self.x[nonzero])/self.s[nonzero]
-            ]), axis=0)
+            self.br[nonzero] = np.max(
+                np.vstack(
+                    [
+                        (self.ub[nonzero] - self.x[nonzero]) / self.s[nonzero],
+                        (self.lb[nonzero] - self.x[nonzero]) / self.s[nonzero],
+                    ]
+                ),
+                axis=0,
+            )
         self.minbr = np.min(self.br)
         self.iminbr = np.where(self.br == self.minbr)[0]
         # compute the minimum of the step
         self.alpha = np.min([1, self.theta * self.minbr])
 
         self.s *= self.alpha
         self.sc *= self.alpha
@@ -212,17 +222,18 @@
         if self.subspace.shape[1] == 0:
             self.sc = np.empty((0, 0))
             self.ss = np.zeros(self.ss0.shape)
             self.s = np.zeros(self.s0.shape)
             return
         if self.subspace.shape[1] > 1:
             self.sc, _ = solve_nd_trust_region_subproblem(
-                self.chess, self.cg,
-                np.sqrt(max(self.delta ** 2 - norm(self.ss0) ** 2, 0.0)),
-                self.logger
+                self.chess,
+                self.cg,
+                np.sqrt(max(self.delta**2 - norm(self.ss0) ** 2, 0.0)),
+                self.logger,
             )
         else:
             self.sc = solve_1d_trust_region_subproblem(
                 self.shess, self.sg, self.subspace[:, 0], self.delta, self.ss0
             )
         self.ss = self.subspace.dot(np.real(self.sc))
         self.s = self.scaling.dot(self.ss)
@@ -242,47 +253,51 @@
     """
     This class provides the machinery to compute an exact solution of
     the trust region subproblem.
     """
 
     type = 'nd'
 
-    def __init__(self, x, sg, hess, scaling, g_dscaling, delta, theta,
-                 ub, lb, logger):
-        super().__init__(x, sg, hess, scaling, g_dscaling, delta, theta,
-                         ub, lb, logger)
+    def __init__(
+        self, x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, logger
+    ):
+        super().__init__(
+            x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, logger
+        )
         self.subspace = np.eye(hess.shape[0])
 
 
 class TRStep2D(Step):
     """
     This class provides the machinery to compute an approximate solution of
     the trust region subproblem according to a 2D subproblem
     """
 
     type = '2d'
 
-    def __init__(self, x, sg, hess, scaling, g_dscaling, delta, theta,
-                 ub, lb, logger):
-        super().__init__(x, sg, hess, scaling, g_dscaling, delta, theta,
-                         ub, lb, logger)
-        s_newt = - linalg.lstsq(self.shess, sg)[0]
+    def __init__(
+        self, x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, logger
+    ):
+        super().__init__(
+            x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, logger
+        )
+        s_newt = -linalg.lstsq(self.shess, sg)[0]
         # lstsq only returns absolute ev values
         e, v = np.linalg.eig(self.shess)
-        self.posdef = np.min(np.real(e)) > - np.spacing(1) * np.max(np.abs(e))
+        self.posdef = np.min(np.real(e)) > -np.spacing(1) * np.max(np.abs(e))
 
         if len(sg) == 1:
-            s_newt = - sg[0]/self.shess[0]
+            s_newt = -sg[0] / self.shess[0]
             self.subspace = np.expand_dims(s_newt, 1)
             return
 
         self.newton = False
 
         if self.posdef:
-            s_newt = - linalg.lstsq(self.shess, sg)[0]
+            s_newt = -linalg.lstsq(self.shess, sg)[0]
 
             if norm(s_newt) < delta:
                 # Case 0 of Fig 12 in [ColemanLi1994]
                 normalize(s_newt)
                 self.newton = True
                 self.subspace = np.expand_dims(s_newt, 1)
                 return
@@ -357,20 +372,23 @@
             r2 = np.dot(r, r)
             alpha = r2 / c
             zp = z + alpha * d
             if c <= 0 or norm(zp) >= self.delta:
                 self.subspace = np.expand_dims(d, 1)
                 self.ss0 = z
                 self.sc = get_1d_trust_region_boundary_solution(
-                    self.shess, self.sg, self.subspace[:, 0], self.ss0,
-                    self.delta
+                    self.shess,
+                    self.sg,
+                    self.subspace[:, 0],
+                    self.ss0,
+                    self.delta,
                 ) * np.ones((1,))
                 self.ss = self.subspace.dot(self.sc)
                 return
-            rp = r + alpha*bd
+            rp = r + alpha * bd
             rp2 = np.dot(rp, rp)
             if np.sqrt(rp2) < eps:
                 normalize(d)
                 self.subspace = np.expand_dims(d, 1)
                 self.sc = zp.dot(d) * np.ones((1,))
                 self.ss = self.subspace.dot(self.sc)
                 self.ss0 = zp - self.ss
@@ -386,22 +404,34 @@
     """
     This class provides the machinery to compute a reflected step based on
     trust region subproblem solution that hit the boundaries.
     """
 
     type = 'trr'
 
-    def __init__(self, x, sg, hess, scaling, g_dscaling, delta, theta,
-                 ub, lb, step: Step):
+    def __init__(
+        self,
+        x,
+        sg,
+        hess,
+        scaling,
+        g_dscaling,
+        delta,
+        theta,
+        ub,
+        lb,
+        step: Step,
+    ):
         """
         :param step:
             Trust-region step that is reflected
         """
-        super().__init__(x, sg, hess, scaling, g_dscaling, delta, theta,
-                         ub, lb, step.logger)
+        super().__init__(
+            x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, step.logger
+        )
 
         alpha = min(step.minbr, 1)
         self.s0 = alpha * step.og_s + step.s0
         self.ss0 = alpha * step.og_ss + step.ss0
         # update x and at breakpoint
         self.x = x + self.s0
 
@@ -419,22 +449,34 @@
     """
     This class provides the machinery to compute a reduced step based on
     trust region subproblem solution that hit the boundaries.
     """
 
     type = 'trt'
 
-    def __init__(self, x, sg, hess, scaling, g_dscaling, delta, theta,
-                 ub, lb, step: Step):
+    def __init__(
+        self,
+        x,
+        sg,
+        hess,
+        scaling,
+        g_dscaling,
+        delta,
+        theta,
+        ub,
+        lb,
+        step: Step,
+    ):
         """
         :param step:
             Trust-region step that is reduced
         """
-        super().__init__(x, sg, hess, scaling, g_dscaling, delta, theta,
-                         ub, lb, step.logger)
+        super().__init__(
+            x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, step.logger
+        )
 
         self.s0 = step.s0.copy()
         self.ss0 = step.ss0.copy()
         iminbr = step.iminbr
         self.s0[iminbr] += step.theta * step.br[iminbr] * step.og_s[iminbr]
         self.ss0[iminbr] += step.theta * step.br[iminbr] * step.og_ss[iminbr]
         # update x and at breakpoint
@@ -456,66 +498,72 @@
 class GradientStep(Step):
     """
     This class provides the machinery to compute a gradient step.
     """
 
     type = 'g'
 
-    def __init__(self, x, sg, hess, scaling, g_dscaling, delta, theta,
-                 ub, lb, logger):
-        super().__init__(x, sg, hess, scaling, g_dscaling, delta, theta,
-                         ub, lb, logger)
+    def __init__(
+        self, x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, logger
+    ):
+        super().__init__(
+            x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, logger
+        )
         s_grad = sg.copy()
         normalize(s_grad)
         self.subspace = np.expand_dims(s_grad, 1)
 
 
 class RefinedStep(Step):
     """
     This class provides the machinery to refine a step based on interior
     point optimization
     """
 
     type = 'ref'
 
-    def __init__(self, x, sg, hess, scaling, g_dscaling, delta, theta,
-                 ub, lb, step):
-        super().__init__(x, sg, hess, scaling, g_dscaling, delta, theta,
-                         ub, lb, step.logger)
+    def __init__(
+        self, x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, step
+    ):
+        super().__init__(
+            x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, step.logger
+        )
         self.subspace: np.ndarray = step.subspace.copy()
         self.chess: np.ndarray = step.chess.copy()
         self.cg: np.ndarray = step.cg.copy()
         self.constraints = [
             NonlinearConstraint(
-                fun=lambda xc: (norm(self.subspace.dot(xc)) - delta) *
-                np.ones((1,)),
-                jac=lambda xc:
-                np.expand_dims(self.subspace.dot(xc), 1).T.dot(self.subspace) /
-                norm(self.subspace.dot(xc)),
+                fun=lambda xc: (norm(self.subspace.dot(xc)) - delta)
+                * np.ones((1,)),
+                jac=lambda xc: np.expand_dims(self.subspace.dot(xc), 1).T.dot(
+                    self.subspace
+                )
+                / norm(self.subspace.dot(xc)),
                 lb=-np.ones((1,)) * np.inf,
                 ub=np.zeros((1,)),
             ),
             LinearConstraint(
                 A=self.subspace,
                 lb=self.theta * (lb - x) / scaling.diagonal(),
-                ub=self.theta * (ub - x) / scaling.diagonal()
-            )
+                ub=self.theta * (ub - x) / scaling.diagonal(),
+            ),
         ]
         self.guess: np.ndarray = step.sc.copy()
         self.qpval0: float = step.qpval
         self.reflection_indices: int = step.reflection_indices
         self.truncation_indices: int = step.truncation_indices
 
     def calculate(self):
-        res = minimize(fun=lambda c: quadratic_form(self.chess, self.cg, c),
-                       jac=lambda c: self.chess.dot(c) + self.cg,
-                       hess=lambda c: self.chess,
-                       x0=self.guess,
-                       method='trust-constr',
-                       constraints=self.constraints,
-                       options={'verbose': 0, 'maxiter': 100,
-                                'gtol': 0, 'xtol': 0})
+        res = minimize(
+            fun=lambda c: quadratic_form(self.chess, self.cg, c),
+            jac=lambda c: self.chess.dot(c) + self.cg,
+            hess=lambda c: self.chess,
+            x0=self.guess,
+            method='trust-constr',
+            constraints=self.constraints,
+            options={'verbose': 0, 'maxiter': 100, 'gtol': 0, 'xtol': 0},
+        )
         self.sc = res.x
         self.ss = self.subspace.dot(self.sc)
         self.s = self.scaling.dot(self.ss)
         self.step_back()
         self.qpval = quadratic_form(self.shess, self.sg, self.ss)
```

### Comparing `fides-0.7.7/fides/subproblem.py` & `fides-0.7.8/fides/subproblem.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 Subproblem Solvers
 ------------------
 This module provides the machinery to solve 1- and N-dimensional
 trust-region subproblems.
 """
 
 import logging
+import math
+from typing import Tuple, Union
 
 import numpy as np
-import math
 from numpy.linalg import norm
-
 from scipy import linalg
-from scipy.optimize import newton, brentq
-
-from typing import Tuple, Union
+from scipy.optimize import brentq, newton
 
 
 def quadratic_form(Q: np.ndarray, p: np.ndarray, x: np.ndarray) -> float:
     """
     Computes the quadratic form :math:`x^TQx + x^Tp`
 
     :param Q: Matrix
@@ -27,19 +25,17 @@
 
     :return:
         Value of form
     """
     return 0.5 * x.T.dot(Q).dot(x) + p.T.dot(x)
 
 
-def solve_1d_trust_region_subproblem(B: np.ndarray,
-                                     g: np.ndarray,
-                                     s: np.ndarray,
-                                     delta: float,
-                                     s0: np.ndarray) -> np.ndarray:
+def solve_1d_trust_region_subproblem(
+    B: np.ndarray, g: np.ndarray, s: np.ndarray, delta: float, s0: np.ndarray
+) -> np.ndarray:
     """
     Solves the special case of a one-dimensional subproblem
 
     :param B:
         Hessian of the quadratic subproblem
     :param g:
         Gradient of the quadratic subproblem
@@ -61,38 +57,40 @@
         return np.zeros((1,))
 
     a = 0.5 * B.dot(s).dot(s)
     if not isinstance(a, float):
         a = a[0, 0]
     b = s.T.dot(B.dot(s0) + g)
 
-    minq = - b / (2 * a)
+    minq = -b / (2 * a)
     if a > 0 and norm(minq * s + s0) <= delta:
         # interior solution
         tau = minq
     else:
         tau = get_1d_trust_region_boundary_solution(B, g, s, s0, delta)
 
     return tau * np.ones((1,))
 
 
 def get_1d_trust_region_boundary_solution(B, g, s, s0, delta):
     a = np.dot(s, s)
     b = 2 * np.dot(s0, s)
     c = np.dot(s0, s0) - delta**2
 
-    aux = b + math.copysign(np.sqrt(b**2 - 4*a*c), b)
+    aux = b + math.copysign(np.sqrt(b**2 - 4 * a * c), b)
     ts = [-aux / (2 * a), -2 * c / aux]
-    qs = [quadratic_form(B, g, s0 + t*s) for t in ts]
+    qs = [quadratic_form(B, g, s0 + t * s) for t in ts]
     return ts[np.argmin(qs)]
 
 
 def solve_nd_trust_region_subproblem(
-        B: np.ndarray, g: np.ndarray, delta: float,
-        logger: Union[logging.Logger, None] = None
+    B: np.ndarray,
+    g: np.ndarray,
+    delta: float,
+    logger: Union[logging.Logger, None] = None,
 ) -> Tuple[np.ndarray, str]:
     r"""
     This function exactly solves the n-dimensional subproblem.
 
     :math:`argmin_s\{s^T B s + s^T g = 0: ||s|| <= \Delta, s \in \mathbb{
     R}^n\}`
 
@@ -137,15 +135,15 @@
     # INITIALIZATION
 
     # instead of a cholesky factorization, we go with an eigenvalue
     # decomposition, which works pretty well for n=2
     eigvals, eigvecs = linalg.eig(B)
     eigvals = np.real(eigvals)
     eigvecs = np.real(eigvecs)
-    w = - eigvecs.T.dot(g)
+    w = -eigvecs.T.dot(g)
     jmin = eigvals.argmin()
     mineig = eigvals[jmin]
 
     # since B symmetric eigenvecs V are orthonormal
     # B + lambda I = V * (E + lambda I) * V.T
     # inv(B + lambda I) = V * inv(E + lambda I) * V.T
     # w = V.T * g
@@ -168,60 +166,70 @@
     # INDEFINITE CASE
     # note that this includes what Nocedal calls the "hard case" but with
     # ||s|| > delta, so the provided formula is not applicable,
     # the respective w should be close to 0 anyways
     if secular(laminit, w, eigvals, eigvecs, delta) < 0:
         maxiter = 100
         try:
-            r = newton(secular, laminit, dsecular, tol=1e-12, maxiter=maxiter,
-                       args=(w, eigvals, eigvecs, delta),)
+            r = newton(
+                secular,
+                laminit,
+                dsecular,
+                tol=1e-12,
+                maxiter=maxiter,
+                args=(w, eigvals, eigvecs, delta),
+            )
             s = slam(r, w, eigvals, eigvecs)
             if norm(s) <= delta + 1e-12:
                 logger.debug('Found boundary subproblem solution via newton')
                 return s, 'indef'
         except RuntimeError:
             pass
         try:
             xa = laminit
             xb = (laminit + np.sqrt(np.spacing(1))) * 10
             # search to the right for a change of sign
-            while secular(xb, w, eigvals, eigvecs, delta) < 0 and \
-                    maxiter > 0:
+            while secular(xb, w, eigvals, eigvecs, delta) < 0 and maxiter > 0:
                 xa = xb
                 xb = xb * 10
                 maxiter -= 1
             if maxiter > 0:
-                r = brentq(secular, xa, xb, xtol=1e-12, maxiter=maxiter,
-                           args=(w, eigvals, eigvecs, delta))
+                r = brentq(
+                    secular,
+                    xa,
+                    xb,
+                    xtol=1e-12,
+                    maxiter=maxiter,
+                    args=(w, eigvals, eigvecs, delta),
+                )
                 s = slam(r, w, eigvals, eigvecs)
                 if norm(s) <= delta + np.sqrt(np.spacing(1)):
                     logger.debug(
                         'Found boundary subproblem solution via brentq'
                     )
                     return s, 'indef'
         except RuntimeError:
             pass  # may end up here due to ill-conditioning, treat as hard case
 
     # HARD CASE (gradient is orthogonal to eigenvector to smallest eigenvalue)
-    w[(eigvals-mineig) == 0] = 0
+    w[(eigvals - mineig) == 0] = 0
     s = slam(-mineig, w, eigvals, eigvecs)
     # we know that ||s(lam) + sigma*v_jmin|| = delta, since v_jmin is
     # orthonormal, we can just substract the difference in norm to get
     # the right length.
 
-    sigma = np.sqrt(max(delta ** 2 - norm(s) ** 2, 0))
+    sigma = np.sqrt(max(delta**2 - norm(s) ** 2, 0))
     s = s + sigma * eigvecs[:, jmin]
     logger.debug('Found boundary 2D subproblem solution via hard case')
     return s, 'hard'
 
 
-def slam(lam: float,
-         w: np.ndarray,
-         eigvals: np.ndarray,
-         eigvecs: np.ndarray) -> np.ndarray:
+def slam(
+    lam: float, w: np.ndarray, eigvals: np.ndarray, eigvecs: np.ndarray
+) -> np.ndarray:
     r"""
     Computes the solution :math:`s(\lambda)` as subproblem solution according
     to
 
     :math:`-(B + \lambda I)s = g`
 
     :param lam:
@@ -238,18 +246,15 @@
     """
     c = w.copy()
     el = eigvals + lam
     c[el != 0] /= el[el != 0]
     return eigvecs.dot(c)
 
 
-def dslam(lam: float,
-          w: np.ndarray,
-          eigvals: np.ndarray,
-          eigvecs: np.ndarray):
+def dslam(lam: float, w: np.ndarray, eigvals: np.ndarray, eigvecs: np.ndarray):
     r"""
     Computes the derivative of the solution :math:`s(\lambda)` with respect to
     lambda, where :math:`s` is the subproblem solution according to
 
     :math:`-(B + \lambda I)s = g`
 
     :param lam:
@@ -262,24 +267,26 @@
         precomputed eigenvectors of B
 
     :return:
         :math:`\frac{\partial s(\lambda)}{\partial \lambda}`
     """
     c = w.copy()
     el = eigvals + lam
-    c[el != 0] /= - np.power(el[el != 0], 2)
+    c[el != 0] /= -np.power(el[el != 0], 2)
     c[(el == 0) & (c != 0)] = np.inf
     return eigvecs.dot(c)
 
 
-def secular(lam: float,
-            w: np.ndarray,
-            eigvals: np.ndarray,
-            eigvecs: np.ndarray,
-            delta: float):
+def secular(
+    lam: float,
+    w: np.ndarray,
+    eigvals: np.ndarray,
+    eigvecs: np.ndarray,
+    delta: float,
+):
     r"""
     Secular equation
 
     :math:`\phi(\lambda) = \frac{1}{||s||} - \frac{1}{\Delta}`
 
     Subproblem solutions are given by the roots of this equation
 
@@ -303,16 +310,21 @@
     sn = norm(s)
     if sn > 0:
         return 1 / sn - 1 / delta
     else:
         return np.inf
 
 
-def dsecular(lam: float, w: np.ndarray, eigvals: np.ndarray,
-             eigvecs: np.ndarray, delta: float):
+def dsecular(
+    lam: float,
+    w: np.ndarray,
+    eigvals: np.ndarray,
+    eigvecs: np.ndarray,
+    delta: float,
+):
     r"""
     Derivative of the secular equation
 
     :math:`\phi(\lambda) = \frac{1}{||s||} - \frac{1}{\Delta}`
 
     with respect to :math:`\lambda`
 
@@ -330,10 +342,10 @@
     :return:
         :math:`\frac{\partial \phi(\lambda)}{\partial \lambda}`
     """
     s = slam(lam, w, eigvals, eigvecs)
     ds = dslam(lam, w, eigvals, eigvecs)
     sn = norm(s)
     if sn > 0:
-        return - s.T.dot(ds) / (norm(s) ** 3)
+        return -s.T.dot(ds) / (norm(s) ** 3)
     else:
         return np.inf
```

### Comparing `fides-0.7.7/fides/trust_region.py` & `fides-0.7.8/fides/trust_region.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,46 @@
 Trust Region Step Evaluation
 ----------------------------
 This module provides the machinery to evaluate different trust-region(
 -reflective) step proposals and select among them based on to their
 performance according to the quadratic approximation of the objective function
 """
 
-import numpy as np
 import logging
 
+import numpy as np
 from scipy.sparse import csc_matrix
 
-from .constants import SubSpaceDim, StepBackStrategy
+from .constants import StepBackStrategy, SubSpaceDim
+from .stepback import stepback_reflect, stepback_truncate
 from .steps import (
-    Step, GradientStep, TRStep2D, TRStepFull, RefinedStep,
-    TRStepReflected, TRStepSteihaug
+    GradientStep,
+    RefinedStep,
+    Step,
+    TRStep2D,
+    TRStepFull,
+    TRStepReflected,
+    TRStepSteihaug,
 )
-from .stepback import stepback_reflect, stepback_truncate
 
 
-def trust_region(x: np.ndarray,
-                 g: np.ndarray,
-                 hess: np.ndarray,
-                 scaling: csc_matrix,
-                 delta: float,
-                 dv: np.ndarray,
-                 theta: float,
-                 lb: np.ndarray,
-                 ub: np.ndarray,
-                 subspace_dim: SubSpaceDim,
-                 stepback_strategy: StepBackStrategy,
-                 logger: logging.Logger) -> Step:
+def trust_region(
+    x: np.ndarray,
+    g: np.ndarray,
+    hess: np.ndarray,
+    scaling: csc_matrix,
+    delta: float,
+    dv: np.ndarray,
+    theta: float,
+    lb: np.ndarray,
+    ub: np.ndarray,
+    subspace_dim: SubSpaceDim,
+    stepback_strategy: StepBackStrategy,
+    logger: logging.Logger,
+) -> Step:
     """
     Compute a step according to the solution of the trust-region subproblem.
     If step-back is necessary, gradient and reflected trust region step are
     also evaluated in terms of their performance according to the local
     quadratic approximation
 
     :param x:
@@ -74,63 +81,96 @@
     g_dscaling = csc_matrix(np.diag(np.abs(g) * dv))
 
     step_options = {
         SubSpaceDim.TWO: TRStep2D,
         SubSpaceDim.FULL: TRStepFull,
         SubSpaceDim.STEIHAUG: TRStepSteihaug,
     }
-    tr_step = step_options[subspace_dim](x, sg, hess, scaling, g_dscaling,
-                                         delta, theta, ub, lb, logger)
+    tr_step = step_options[subspace_dim](
+        x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, logger
+    )
     tr_step.calculate()
 
     # in case of truncation, we hit the boundary and we check both the
     # gradient and the reflected step, either of which could be better than the
     # TR step
 
     steps = [tr_step]
     if tr_step.alpha < 1.0 and len(g) > 1:
-        g_step = GradientStep(x, sg, hess, scaling, g_dscaling, delta,
-                              theta, ub, lb, logger)
+        g_step = GradientStep(
+            x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, logger
+        )
         g_step.calculate()
         steps.append(g_step)
         if stepback_strategy == StepBackStrategy.SINGLE_REFLECT:
-            rtr_step = TRStepReflected(x, sg, hess, scaling, g_dscaling, delta,
-                                       theta, ub, lb, tr_step)
+            rtr_step = TRStepReflected(
+                x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, tr_step
+            )
             rtr_step.calculate()
             steps.append(rtr_step)
 
-        if stepback_strategy in [StepBackStrategy.REFLECT,
-                                 StepBackStrategy.MIXED]:
-            steps.extend(stepback_reflect(
-                tr_step, x, sg, hess, scaling, g_dscaling, delta, theta, ub,
-                lb
-            ))
-
-        if stepback_strategy in [StepBackStrategy.TRUNCATE,
-                                 StepBackStrategy.MIXED]:
-            steps.extend(stepback_truncate(
-                tr_step, x, sg, hess, scaling, g_dscaling, delta, theta, ub,
-                lb
-            ))
+        if stepback_strategy in [
+            StepBackStrategy.REFLECT,
+            StepBackStrategy.MIXED,
+        ]:
+            steps.extend(
+                stepback_reflect(
+                    tr_step,
+                    x,
+                    sg,
+                    hess,
+                    scaling,
+                    g_dscaling,
+                    delta,
+                    theta,
+                    ub,
+                    lb,
+                )
+            )
+
+        if stepback_strategy in [
+            StepBackStrategy.TRUNCATE,
+            StepBackStrategy.MIXED,
+        ]:
+            steps.extend(
+                stepback_truncate(
+                    tr_step,
+                    x,
+                    sg,
+                    hess,
+                    scaling,
+                    g_dscaling,
+                    delta,
+                    theta,
+                    ub,
+                    lb,
+                )
+            )
 
-        if stepback_strategy == StepBackStrategy.REFINE and \
-                tr_step.subspace.shape[1] > 1:
+        if (
+            stepback_strategy == StepBackStrategy.REFINE
+            and tr_step.subspace.shape[1] > 1
+        ):
             ref_step = RefinedStep(
-                x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb,
-                tr_step
+                x, sg, hess, scaling, g_dscaling, delta, theta, ub, lb, tr_step
             )
             ref_step.calculate()
             steps.append(ref_step)
 
     if len(steps) > 1:
-        rcountstrs = [str(step.reflection_count)
-                      * int(step.reflection_count > 0)
-                      for step in steps]
-        logger.debug(' | '.join([
-            f'{step.type + rcountstr}: [qp:'
-            f' {step.qpval:.2E}, '
-            f'a: {step.alpha:.2E}]'
-            for rcountstr, step in zip(rcountstrs, steps)
-        ]))
+        rcountstrs = [
+            str(step.reflection_count) * int(step.reflection_count > 0)
+            for step in steps
+        ]
+        logger.debug(
+            ' | '.join(
+                [
+                    f'{step.type + rcountstr}: [qp:'
+                    f' {step.qpval:.2E}, '
+                    f'a: {step.alpha:.2E}]'
+                    for rcountstr, step in zip(rcountstrs, steps)
+                ]
+            )
+        )
 
     qpvals = [step.qpval for step in steps]
     return steps[np.argmin(qpvals)]
```

### Comparing `fides-0.7.7/fides.egg-info/PKG-INFO` & `fides-0.7.8/fides.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 Metadata-Version: 2.1
 Name: fides
-Version: 0.7.7
-Summary: python Trust Region Optimization
-Home-page: https://github.com/Fides-dev/fides
-Author: Fabian Froehlich
-Author-email: froehlichfab@gmail.com
+Version: 0.7.8
+Summary: python-based Trust Region Optimization toolbox
+Home-page: https://github.com/fides-dev/fides
+Download-URL: https://github.com/fides-dev/fides/releases
+Author: The fides developers
+Author-email: frohlichfab@gmail.com
+Maintainer: Fabian Fröhlich
+Maintainer-email: frohlichfab@gmail.com
 License: BSD-3-Clause
-Description: # Fides - A python package for Trust Region Optimization
-        
-        <a href="https://badge.fury.io/py/fides">
-          <img src="https://badge.fury.io/py/fides.svg" alt="PyPI version"></a>
-        <a href="https://codecov.io/gh/fides-dev/fides">
-          <img src="https://codecov.io/gh/fides-dev/fides/branch/master/graph/badge.svg" alt="Code coverage"></a>
-        <a href="https://fides-optimizer.readthedocs.io/en/latest/?badge=latest">
-         <img src="https://readthedocs.org/projects/fides-optimizer/badge/?version=latest" alt="ReadTheDocs status"></a>
-        <a href="https://zenodo.org/badge/latestdoi/312057973">
-         <img src="https://zenodo.org/badge/312057973.svg" alt="DOI"></a>
-        
-        ## About Fides
-        
-        Fides implements an Interior Trust Region Reflective for boundary constrained
-        optimization problems based on the papers
-        [ColemanLi1994](https://doi.org/10.1007/BF01582221) and
-        [ColemanLi1996](http://dx.doi.org/10.1137/0806023). Accordingly, Fides is named
-        after the Roman goddess of trust and
-        reliability.
-        
-        Fides can be installed via `pip install fides`. Further documentation is
-         available at [Read the Docs](https://fides-optimizer.readthedocs.io/).
-         
-         
-        ## Features
-        
-        
-        * Boundary constrained and unconstrained interior trust-region optimization
-        * Reflective, truncated and optimization based boundary heuristics
-        * Exact, 2D and CG subproblem solvers
-        * BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative
-         Hessian Approximation schemes
-        * SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian Approximations schemes
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
+Project-URL: Bug Tracker, https://github.com/fides-dev/fides/issues
+Project-URL: Documentation, https://fides-optimizer.readthedocs.io/
+Project-URL: Changelog, https://github.com/fides-dev/fides/releases
+Keywords: optimization,trust-region,systems biology
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: test
+
+# Fides - A python package for Trust Region Optimization
+
+<a href="https://badge.fury.io/py/fides">
+  <img src="https://badge.fury.io/py/fides.svg" alt="PyPI version"></a>
+<a href="https://codecov.io/gh/fides-dev/fides">
+  <img src="https://codecov.io/gh/fides-dev/fides/branch/master/graph/badge.svg" alt="Code coverage"></a>
+<a href="https://fides-optimizer.readthedocs.io/en/latest/?badge=latest">
+ <img src="https://readthedocs.org/projects/fides-optimizer/badge/?version=latest" alt="ReadTheDocs status"></a>
+<a href="https://zenodo.org/badge/latestdoi/312057973">
+ <img src="https://zenodo.org/badge/312057973.svg" alt="DOI"></a>
+
+## About Fides
+
+Fides implements an Interior Trust Region Reflective for boundary constrained
+optimization problems based on the papers
+[ColemanLi1994](https://doi.org/10.1007/BF01582221) and
+[ColemanLi1996](http://dx.doi.org/10.1137/0806023). Accordingly, Fides is named
+after the Roman goddess of trust and
+reliability.
+
+Fides can be installed via `pip install fides`. Further documentation is
+ available at [Read the Docs](https://fides-optimizer.readthedocs.io/).
+ 
+ 
+## Features
+
+
+* Boundary constrained and unconstrained interior trust-region optimization
+* Reflective, truncated and optimization based boundary heuristics
+* Exact, 2D and CG subproblem solvers
+* BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative
+ Hessian Approximation schemes
+* SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian Approximations schemes
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,24 +1,29 @@
-Metadata-Version: 2.1 Name: fides Version: 0.7.7 Summary: python Trust Region
-Optimization Home-page: https://github.com/Fides-dev/fides Author: Fabian
-Froehlich Author-email: froehlichfab@gmail.com License: BSD-3-Clause
-Description: # Fides - A python package for Trust Region Optimization [PyPI
-version] [Code_coverage] [ReadTheDocs_status] [DOI] ## About Fides Fides
-implements an Interior Trust Region Reflective for boundary constrained
-optimization problems based on the papers [ColemanLi1994](https://doi.org/
-10.1007/BF01582221) and [ColemanLi1996](http://dx.doi.org/10.1137/0806023).
-Accordingly, Fides is named after the Roman goddess of trust and reliability.
-Fides can be installed via `pip install fides`. Further documentation is
-available at [Read the Docs](https://fides-optimizer.readthedocs.io/). ##
-Features * Boundary constrained and unconstrained interior trust-region
-optimization * Reflective, truncated and optimization based boundary heuristics
-* Exact, 2D and CG subproblem solvers * BFGS, DFP, SR1, Broyden (good and bad)
-and Broyden class iterative Hessian Approximation schemes * SSM, TSSM, FX,
-GNSBFGS and custom hybrid Hessian Approximations schemes Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Software Development ::
-Libraries Classifier: License :: OSI Approved :: BSD License Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: fides Version: 0.7.8 Summary: python-based Trust
+Region Optimization toolbox Home-page: https://github.com/fides-dev/fides
+Download-URL: https://github.com/fides-dev/fides/releases Author: The fides
+developers Author-email: frohlichfab@gmail.com Maintainer: Fabian FrÃ¶hlich
+Maintainer-email: frohlichfab@gmail.com License: BSD-3-Clause Project-URL: Bug
+Tracker, https://github.com/fides-dev/fides/issues Project-URL: Documentation,
+https://fides-optimizer.readthedocs.io/ Project-URL: Changelog, https://
+github.com/fides-dev/fides/releases Keywords: optimization,trust-region,systems
+biology Classifier: Development Status :: 4 - Beta Classifier: Topic ::
+Software Development :: Libraries Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: BSD License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.9
+Description-Content-Type: text/markdown Provides-Extra: test # Fides - A python
+package for Trust Region Optimization [PyPI_version] [Code_coverage]
+[ReadTheDocs_status] [DOI] ## About Fides Fides implements an Interior Trust
+Region Reflective for boundary constrained optimization problems based on the
+papers [ColemanLi1994](https://doi.org/10.1007/BF01582221) and [ColemanLi1996]
+(http://dx.doi.org/10.1137/0806023). Accordingly, Fides is named after the
+Roman goddess of trust and reliability. Fides can be installed via `pip install
+fides`. Further documentation is available at [Read the Docs](https://fides-
+optimizer.readthedocs.io/). ## Features * Boundary constrained and
+unconstrained interior trust-region optimization * Reflective, truncated and
+optimization based boundary heuristics * Exact, 2D and CG subproblem solvers *
+BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative Hessian
+Approximation schemes * SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian
+Approximations schemes
```

