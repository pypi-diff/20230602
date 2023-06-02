# Comparing `tmp/cvxcovariance-0.1.0.tar.gz` & `tmp/cvxcovariance-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxcovariance-0.1.0.tar", max compression
+gzip compressed data, was "cvxcovariance-0.1.1.tar", max compression
```

## Comparing `cvxcovariance-0.1.0.tar` & `cvxcovariance-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11375 2023-06-02 04:45:29.964957 cvxcovariance-0.1.0/LICENSE
--rw-r--r--   0        0        0     6749 2023-06-02 04:45:29.964957 cvxcovariance-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 04:45:29.988957 cvxcovariance-0.1.0/cvx/covariance/__init__.py
--rw-r--r--   0        0        0     9179 2023-06-02 04:45:29.992956 cvxcovariance-0.1.0/cvx/covariance/combination.py
--rw-r--r--   0        0        0     6706 2023-06-02 04:45:29.992956 cvxcovariance-0.1.0/cvx/covariance/ewma.py
--rw-r--r--   0        0        0     1863 2023-06-02 04:45:29.992956 cvxcovariance-0.1.0/cvx/covariance/regularization.py
--rw-r--r--   0        0        0      645 2023-06-02 04:46:03.184546 cvxcovariance-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7347 1970-01-01 00:00:00.000000 cvxcovariance-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-02 19:03:52.533689 cvxcovariance-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6742 2023-06-02 19:03:52.533689 cvxcovariance-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 19:03:52.557689 cvxcovariance-0.1.1/cvx/covariance/__init__.py
+-rw-r--r--   0        0        0     9207 2023-06-02 19:03:52.557689 cvxcovariance-0.1.1/cvx/covariance/combination.py
+-rw-r--r--   0        0        0     6766 2023-06-02 19:03:52.557689 cvxcovariance-0.1.1/cvx/covariance/ewma.py
+-rw-r--r--   0        0        0     1923 2023-06-02 19:03:52.557689 cvxcovariance-0.1.1/cvx/covariance/regularization.py
+-rw-r--r--   0        0        0      645 2023-06-02 19:04:28.501631 cvxcovariance-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7340 1970-01-01 00:00:00.000000 cvxcovariance-0.1.1/PKG-INFO
```

### Comparing `cvxcovariance-0.1.0/LICENSE` & `cvxcovariance-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.1.0/README.md` & `cvxcovariance-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,21 +42,21 @@
 # Load return data
 returns = pd.read_csv("data/ff5.csv", index_col=0, header=0, parse_dates=True).iloc[:1000]
 n = returns.shape[1]
 
 # Define half-life pairs for K=3 experts, (halflife_vola, halflife_cov)
 halflife_pairs = [(10, 21), (21, 63), (63, 125)]
 
-# Define the covariance combinator 
+# Define the covariance combinator
 combinator = from_ewmas(returns,
                         halflife_pairs,
                         min_periods_vola=n,  # min periods for volatility estimation
                         min_periods_cov=3 * n)  # min periods for correlation estimation (must be at least n)
 
-# Solve combination problem and loop through combination results to get predictors   
+# Solve combination problem and loop through combination results to get predictors
 covariance_predictors = {}
 for predictor in combinator.solve(window=10):  # lookback window in convex optimization problem
     # From predictor we can access predictor.time, predictor.mean (=0 here), predictor.covariance, and predictor.weights
     covariance_predictors[predictor.time] = predictor.covariance
 ```
 Here `covariance_predictors[t]` is the covariance prediction for time $t+1$, $\textit{i.e.}$, it is uses knowledge of $r_1,\ldots,r_t$.
 
@@ -79,15 +79,15 @@
 expert1 = {time: ewma21.loc[time] for time in ewma21.index.get_level_values(0).unique()}
 ewma63 = returns.ewm(halflife=63, min_periods=5 * n).cov().dropna()
 expert2 = {time: ewma63.loc[time] for time in ewma63.index.get_level_values(0).unique()}
 
 # Create expert dictionary
 experts = {1: expert1, 2: expert2}
 
-# Define the covariance combinator 
+# Define the covariance combinator
 combinator = from_sigmas(sigmas=experts, returns=returns)
 
 # Solve combination problem and loop through combination results to get predictors
 covariance_predictors = {}
 for predictor in combinator.solve(window=10):
     # From predictor we can access predictor.time, predictor.mean (=0 here), predictor.covariance, and predictor.weights
     covariance_predictors[predictor.time] = predictor.covariance
@@ -113,9 +113,7 @@
 ```bash
 ./create_kernel.sh
 ```
 
 constructs a dedicated
 [Kernel](https://docs.jupyter.org/en/latest/projects/kernels.html) for the
 project.
-
-
```

### Comparing `cvxcovariance-0.1.0/cvx/covariance/combination.py` & `cvxcovariance-0.1.1/cvx/covariance/combination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import warnings
 from collections import namedtuple
+
 import cvxpy as cvx
 import numpy as np
 import pandas as pd
-import warnings
 
 from cvx.covariance.ewma import iterated_ewma
 
 # Mute specific warning
 warnings.filterwarnings("ignore", message="Solution may be inaccurate.*")
 
+
 def _map_nested_dicts(ob, func):
     """
     Recursively applies a function to a nested dictionary
     """
     if isinstance(ob, dict):
         return {k: _map_nested_dicts(v, func) for k, v in ob.items()}
-    else:
-        return func(ob)
+
+    return func(ob)
 
 
 def _cholesky_precision(cov):
     """
     Computes Cholesky factor of the inverse of each covariance matrix in cov
 
     param cov: dictionary of covariance matrices {time: Sigma}
@@ -96,20 +101,15 @@
 
     @property
     def weights(self):
         return pd.Series(index=self.keys, data=self._weight.value)
 
 
 def from_ewmas(
-    returns,
-    pairs,
-    min_periods_vola=20,
-    min_periods_cov=20,
-    clip_at=None,
-    mean=False
+    returns, pairs, min_periods_vola=20, min_periods_cov=20, clip_at=None, mean=False
 ):
     """
     Estimate a series of covariance matrices using the iterated EWMA method
 
     param returns: Frame of returns
     param pairs: list of pairs of EWMA half lives, e.g. [(20, 20), (10, 50), (20, 60)],
                 pair[0] is the half life for volatility estimation
@@ -140,14 +140,15 @@
 
     sigmas = _map_nested_dicts(results, lambda result: result.covariance)
     means = _map_nested_dicts(results, lambda result: result.mean)
 
     # combination of covariance matrix valued time series
     return _CovarianceCombination(sigmas=sigmas, returns=returns, means=means)
 
+
 def from_sigmas(sigmas, returns, means=None):
     return _CovarianceCombination(sigmas=sigmas, returns=returns, means=means)
 
 
 class _CovarianceCombination:
     def __init__(self, sigmas, returns, means=None):
         """
@@ -194,15 +195,14 @@
     def means(self):
         return self.__means
 
     @property
     def returns(self):
         return self.__returns
 
-
     @property
     def K(self):
         """
         Returns the number of expert predictors
         """
         return len(self.sigmas)
 
@@ -278,8 +278,7 @@
         nu = sum(self.__nus.loc[time] * weights.values)  # prediction for time+1
 
         mean = pd.Series(index=self.assets, data=np.linalg.inv(L.T) @ nu)
         sigma = pd.DataFrame(
             index=self.assets, columns=self.assets, data=np.linalg.inv(L @ L.T)
         )
         return Result(time=time, mean=mean, covariance=sigma, weights=weights)
-
```

### Comparing `cvxcovariance-0.1.0/cvx/covariance/ewma.py` & `cvxcovariance-0.1.1/cvx/covariance/ewma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
 from collections import namedtuple
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from pandas._typing import TimedeltaConvertibleTypes
-from typing import Union
 
 IEWMA = namedtuple("IEWMA", ["time", "mean", "covariance", "volatility"])
 
 
 def _generator2frame(generator):
     return pd.DataFrame(dict(generator)).transpose()
```

### Comparing `cvxcovariance-0.1.0/cvx/covariance/regularization.py` & `cvxcovariance-0.1.1/cvx/covariance/regularization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
 from collections import namedtuple
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 import scipy as sc
 
 LowRank = namedtuple("LowRank", ["Loading", "Cov", "D", "Approximation"])
 
 
 def _regularize_correlation(R, r):
     """
```

### Comparing `cvxcovariance-0.1.0/pyproject.toml` & `cvxcovariance-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxcovariance"
-version = "v0.1.0"             # Don't touch, leave at 0.0.0
+version = "v0.1.1"             # Don't touch, leave at 0.0.0
 description = "..."
 authors = ["Kasper Johansson", "Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cov_pred_finance"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxcovariance-0.1.0/PKG-INFO` & `cvxcovariance-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxcovariance
-Version: 0.1.0
+Version: 0.1.1
 Summary: ...
 Home-page: https://github.com/cvxgrp/cov_pred_finance
 Author: Kasper Johansson
 Requires-Python: >=3.8.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -60,21 +60,21 @@
 # Load return data
 returns = pd.read_csv("data/ff5.csv", index_col=0, header=0, parse_dates=True).iloc[:1000]
 n = returns.shape[1]
 
 # Define half-life pairs for K=3 experts, (halflife_vola, halflife_cov)
 halflife_pairs = [(10, 21), (21, 63), (63, 125)]
 
-# Define the covariance combinator 
+# Define the covariance combinator
 combinator = from_ewmas(returns,
                         halflife_pairs,
                         min_periods_vola=n,  # min periods for volatility estimation
                         min_periods_cov=3 * n)  # min periods for correlation estimation (must be at least n)
 
-# Solve combination problem and loop through combination results to get predictors   
+# Solve combination problem and loop through combination results to get predictors
 covariance_predictors = {}
 for predictor in combinator.solve(window=10):  # lookback window in convex optimization problem
     # From predictor we can access predictor.time, predictor.mean (=0 here), predictor.covariance, and predictor.weights
     covariance_predictors[predictor.time] = predictor.covariance
 ```
 Here `covariance_predictors[t]` is the covariance prediction for time $t+1$, $\textit{i.e.}$, it is uses knowledge of $r_1,\ldots,r_t$.
 
@@ -97,15 +97,15 @@
 expert1 = {time: ewma21.loc[time] for time in ewma21.index.get_level_values(0).unique()}
 ewma63 = returns.ewm(halflife=63, min_periods=5 * n).cov().dropna()
 expert2 = {time: ewma63.loc[time] for time in ewma63.index.get_level_values(0).unique()}
 
 # Create expert dictionary
 experts = {1: expert1, 2: expert2}
 
-# Define the covariance combinator 
+# Define the covariance combinator
 combinator = from_sigmas(sigmas=experts, returns=returns)
 
 # Solve combination problem and loop through combination results to get predictors
 covariance_predictors = {}
 for predictor in combinator.solve(window=10):
     # From predictor we can access predictor.time, predictor.mean (=0 here), predictor.covariance, and predictor.weights
     covariance_predictors[predictor.time] = predictor.covariance
@@ -132,9 +132,7 @@
 ./create_kernel.sh
 ```
 
 constructs a dedicated
 [Kernel](https://docs.jupyter.org/en/latest/projects/kernels.html) for the
 project.
 
-
-
```

