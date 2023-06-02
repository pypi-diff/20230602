# Comparing `tmp/cvxcovariance-0.0.5.tar.gz` & `tmp/cvxcovariance-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxcovariance-0.0.5.tar", max compression
+gzip compressed data, was "cvxcovariance-0.0.7.tar", max compression
```

## Comparing `cvxcovariance-0.0.5.tar` & `cvxcovariance-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11375 2023-05-23 18:05:21.231819 cvxcovariance-0.0.5/LICENSE
--rw-r--r--   0        0        0      542 2023-05-23 18:05:21.231819 cvxcovariance-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-23 18:05:21.255820 cvxcovariance-0.0.5/cvx/covariance/__init__.py
--rw-r--r--   0        0        0     6737 2023-05-23 18:05:21.255820 cvxcovariance-0.0.5/cvx/covariance/covariance_combination.py
--rw-r--r--   0        0        0     6542 2023-05-23 18:05:21.255820 cvxcovariance-0.0.5/cvx/covariance/ewma.py
--rw-r--r--   0        0        0     8440 2023-05-23 18:05:21.255820 cvxcovariance-0.0.5/cvx/covariance/iterated_ewma_vec.py
--rw-r--r--   0        0        0      600 2023-05-23 18:05:51.312697 cvxcovariance-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 cvxcovariance-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-02 01:05:02.456010 cvxcovariance-0.0.7/LICENSE
+-rw-r--r--   0        0        0     6749 2023-06-02 01:05:02.456010 cvxcovariance-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 01:05:02.484010 cvxcovariance-0.0.7/cvx/covariance/__init__.py
+-rw-r--r--   0        0        0     9179 2023-06-02 01:05:02.484010 cvxcovariance-0.0.7/cvx/covariance/combination.py
+-rw-r--r--   0        0        0     6706 2023-06-02 01:05:02.484010 cvxcovariance-0.0.7/cvx/covariance/ewma.py
+-rw-r--r--   0        0        0     1863 2023-06-02 01:05:02.484010 cvxcovariance-0.0.7/cvx/covariance/regularization.py
+-rw-r--r--   0        0        0      645 2023-06-02 01:05:31.691910 cvxcovariance-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     7347 1970-01-01 00:00:00.000000 cvxcovariance-0.0.7/PKG-INFO
```

### Comparing `cvxcovariance-0.0.5/LICENSE` & `cvxcovariance-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.5/cvx/covariance/covariance_combination.py` & `cvxcovariance-0.0.7/cvx/covariance/combination.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,177 +1,285 @@
 from collections import namedtuple
 import cvxpy as cvx
 import numpy as np
 import pandas as pd
-from tqdm import tqdm
 import warnings
 
+from cvx.covariance.ewma import iterated_ewma
+
 # Mute specific warning
 warnings.filterwarnings("ignore", message="Solution may be inaccurate.*")
 
+def _map_nested_dicts(ob, func):
+    """
+    Recursively applies a function to a nested dictionary
+    """
+    if isinstance(ob, dict):
+        return {k: _map_nested_dicts(v, func) for k, v in ob.items()}
+    else:
+        return func(ob)
+
 
 def _cholesky_precision(cov):
     """
     Computes Cholesky factor of the inverse of each covariance matrix in cov
 
     param cov: dictionary of covariance matrices {time: Sigma}
     """
-    return {time: np.linalg.cholesky(np.linalg.inv(item.values)) for time, item in cov.items()}
+    return {
+        time: np.linalg.cholesky(np.linalg.inv(item.values))
+        for time, item in cov.items()
+    }
+
 
 def _B_t_col(Ls, nus, returns):
     """
     Computes L.T @ return for each L factor in Ls and corresponding
     return in returns
     """
-    return {time:  L.T @ returns.loc[time].values - nus[time] for time, L in Ls.items()}
+    return {time: L.T @ returns.loc[time].values - nus[time] for time, L in Ls.items()}
+
 
 def _diag_part(cholesky):
     return {key: np.diag(L) for key, L in cholesky.items()}
 
+
 def _A(diags_interval, K):
-        """
-        param diags_interval: NxK pandas DataFrame where each entry is diagonal
-        of an expert Cholesky factor matrix
-        param K: number of expert predictors
+    """
+    param diags_interval: NxK pandas DataFrame where each entry is diagonal
+    of an expert Cholesky factor matrix
+    param K: number of expert predictors
 
-        returns: nNxK matrix where each column is a vector of stacked diagonals
-        """
-        return np.column_stack([np.vstack(diags_interval.iloc[:,i]).flatten() for i in range(K)])
+    returns: nNxK matrix where each column is a vector of stacked diagonals
+    """
+    return np.column_stack(
+        [np.vstack(diags_interval.iloc[:, i]).flatten() for i in range(K)]
+    )
 
-def _zero_means(times, n):
-    return  {time: np.zeros(n) for time in times}
 
 def _nu(Ls, means):
     """
     Computes L.T @ mu for each L factor in Ls and corresponding
     mu in means
     """
-    return {time:  L.T @ means[time] for time, L in Ls.items()}  
+    return {time: L.T @ means[time] for time, L in Ls.items()}
+
 
 # Declaring namedtuple()
-Result = namedtuple('Result', ['time', 'window', 'mean', 'covariance', 'weights'])
+Result = namedtuple("Result", ["time", "mean", "covariance", "weights"])
 
 
-class CovarianceCombination:
-    def __init__(self, Sigmas, returns, means=None):
+class _CombinationProblem:
+    def __init__(self, keys, n, window):
+        self.keys = keys
+        K = len(keys)
+        self._weight = cvx.Variable(len(keys), name="weights")
+        self.A_param = cvx.Parameter((n * window, K))
+        self.P_chol_param = cvx.Parameter((K, K))
+
+    @property
+    def _constraints(self):
+        return [cvx.sum(self._weight) == 1, self._weight >= 0]
+
+    @property
+    def _objective(self):
+        return cvx.sum(cvx.log(self.A_param @ self._weight)) - 0.5 * cvx.sum_squares(
+            self.P_chol_param.T @ self._weight
+        )
+
+    @property
+    def _problem(self):
+        return cvx.Problem(cvx.Maximize(self._objective), self._constraints)
+
+    def solve(self, **kwargs):
+        return self._problem.solve(**kwargs)
+        # return self.weights
+
+    @property
+    def weights(self):
+        return pd.Series(index=self.keys, data=self._weight.value)
+
+
+def from_ewmas(
+    returns,
+    pairs,
+    min_periods_vola=20,
+    min_periods_cov=20,
+    clip_at=None,
+    mean=False
+):
+    """
+    Estimate a series of covariance matrices using the iterated EWMA method
+
+    param returns: Frame of returns
+    param pairs: list of pairs of EWMA half lives, e.g. [(20, 20), (10, 50), (20, 60)],
+                pair[0] is the half life for volatility estimation
+                pair[1] is the half life for covariance estimation
+    param min_periods_vola: minimum number of observations to start EWMA for volatility estimation (optional)
+    param min_periods_cov: minimum number of observations to start EWMA for covariance estimation (optional)
+    param clip_at: clip volatility adjusted returns at +- clip_at (optional)
+    param mean: subtract EWMA mean from returns and volatility adjusted returns (optional)
+
+    return: Yields tuples with time, mean, covariance matrix, weights
+    """
+    # compute the covariance matrices, one time series for each pair
+    results = {
+        f"{pair[0]}-{pair[1]}": {
+            result.time: result
+            for result in iterated_ewma(
+                returns=returns,
+                vola_halflife=pair[0],
+                cov_halflife=pair[1],
+                min_periods_vola=min_periods_vola,
+                min_periods_cov=min_periods_cov,
+                clip_at=clip_at,
+                mean=mean,
+            )
+        }
+        for pair in pairs
+    }
+
+    sigmas = _map_nested_dicts(results, lambda result: result.covariance)
+    means = _map_nested_dicts(results, lambda result: result.mean)
+
+    # combination of covariance matrix valued time series
+    return _CovarianceCombination(sigmas=sigmas, returns=returns, means=means)
+
+def from_sigmas(sigmas, returns, means=None):
+    return _CovarianceCombination(sigmas=sigmas, returns=returns, means=means)
+
+
+class _CovarianceCombination:
+    def __init__(self, sigmas, returns, means=None):
+        """
+        Computes the covariance combination of a set of covariance matrices
 
-        ### Assert Sigmas and means have same keys if means not None
+        param sigmas: dictionary of covariance matrices {key: {time: sigma}}
+        param returns: pandas DataFrame of returns
+        param means: dictionary of means {key: {time: mu}}, optional
+        """
+        # Assert Sigmas and means have same keys if means not None
         n = returns.shape[1]
         if means is not None:
-            for key, Sigma in Sigmas.items():
-                assert Sigma.keys() == means[key].keys(), "Sigmas and means must have same keys"
+            for key, sigma in sigmas.items():
+                # Assert sigmas and means have same keys
+                assert (
+                    sigma.keys() == means[key].keys()
+                ), "sigmas and means must have same keys"
         else:
-            means = {k: _zero_means(Sigma.keys(), n) for k, Sigma in Sigmas.items()}
-    
-        # ### Fix conditioning
-        # # Multiply entries in means and returns by 100
-        # means = {k: {time: 100*item for time, item in means[k].items()} for k in means.keys()}
-        # returns = 100*returns
-
-        # # Multiply entries in Sigmas by 10000
-        # Sigmas = {k: {time: 10000*item for time, item in Sigma.items()} for k, Sigma in Sigmas.items()}
-                
+            # Set means to zero if not provided
+            means = {
+                k: {time: np.zeros(n) for time in sigma.keys()}
+                for k, sigma in sigmas.items()
+            }
+
         self.__means = means
-        self.__Sigmas = Sigmas
+        self.__sigmas = sigmas
         self.__returns = returns
-        self.__K = len(self.__Sigmas)
-        self.__weight = cvx.Variable(self.__K, name="weights")
-        self.__n = n
-        self._initilized = False
+
+        # all those quantities don't depend on the window size
+        self.__Ls = pd.DataFrame(
+            {k: _cholesky_precision(sigma) for k, sigma in self.sigmas.items()}
+        )
+        self.__Ls_shifted = self.__Ls.shift(1).dropna()
+        self.__nus = pd.DataFrame(
+            {key: _nu(Ls, self.means[key]) for key, Ls in self.__Ls.items()}
+        )
+        self.__nus_shifted = self.__nus.shift(1).dropna()
 
     @property
-    def K(self):
-        return self.__K
+    def sigmas(self):
+        return self.__sigmas
 
     @property
-    def index(self):
-        return self.__A.index
+    def means(self):
+        return self.__means
 
     @property
-    def assets(self):
-        return self.__returns.columns
+    def returns(self):
+        return self.__returns
+
 
-    def _combine_experts(self, experts):
-        return np.sum([expert * w_k for expert, w_k in zip(experts, self.__weight)])
+    @property
+    def K(self):
+        """
+        Returns the number of expert predictors
+        """
+        return len(self.sigmas)
 
-    def _precompute(self, window=10):
+    @property
+    def assets(self):
         """
-        Precomputes parameter values for CVXPY problem
+        Returns the assets in the covariance combination problem
         """
-        returns = self.__returns
-        Sigmas = self.__Sigmas
-        means = self.__means
+        return self.returns.columns
 
-        self.Ls = pd.DataFrame({k: _cholesky_precision(Sigma) for k, Sigma in Sigmas.items()})
-        self.Ls_shifted = self.Ls.shift(1).dropna()
-        self.nus = pd.DataFrame({key: _nu(Ls, means[key]) for key, Ls in self.Ls.items()})
-        nus_shifted = self.nus.shift(1).dropna()
-        
+    def solve(self, window=None, **kwargs):
+        """
+        The size of the window is crucial to specify the size of the parameters
+        for the cvxpy problem. Hence those computations are not in the __init__ method
+
+        Solves the covariance combination problem at a given time, i.e.,
+        finds the prediction for the covariance matrix at 'time+1'
+
+        param window: number of previous time steps to use in the covariance combination
+        """
         # If window is None, use all available data; cap window at length of data
-        window = window or len(self.Ls_shifted)
-        window = min(window, len(self.Ls_shifted))
+        window = window or len(self.__Ls_shifted)
+        window = min(window, len(self.__Ls_shifted))
 
-        ### Compute the parameter values for CVXPY problem
         # Compute P matrix and its Cholesky factor
-        Lts_at_r = pd.DataFrame({key: _B_t_col(Ls, nus_shifted[key], returns) for key, Ls in self.Ls_shifted.items()}) 
+        Lts_at_r = pd.DataFrame(
+            {
+                key: _B_t_col(Ls, self.__nus_shifted[key], self.returns)
+                for key, Ls in self.__Ls_shifted.items()
+            }
+        )
+
         Bs = {time: np.column_stack(Lts_at_r.loc[time]) for time in Lts_at_r.index}
-        prod_Bs = pd.Series({time: B.T@B for time, B in Bs.items()})
+        prod_Bs = pd.Series({time: B.T @ B for time, B in Bs.items()})
         times = prod_Bs.index
-        P = pd.Series({times[i]: sum(prod_Bs.loc[times[i-window+1]:times[i]]) for i in range(window-1, len(times))})
-        self.__P_chol = pd.Series({time: np.linalg.cholesky(P.loc[time]) for time in P.index})
-
-        # Compute A matrix
-        Ls_diag = pd.DataFrame({k: _diag_part(L) for k, L in self.Ls_shifted.items()})
-        self.__A = pd.Series({times[i]: _A(Ls_diag.truncate(before=times[i-window+1], after=times[i]), self.K) for i in range(window-1, len(times))})
+        P = {
+            times[i]: sum(prod_Bs.loc[times[i - window + 1] : times[i]])
+            for i in range(window - 1, len(times))
+        }
 
-        ### Generate CVPXY problem
-        self.__A_param = cvx.Parameter((self.__n*window, self.__K))
-        self.__P_chol_param = cvx.Parameter((self.__K, self.__K))
-        self.__obj = cvx.sum(cvx.log(self.__A_param@self.__weight)) - 0.5*cvx.sum_squares(self.__P_chol_param.T@self.__weight)
-        self.__constraints = [self.__weight >= 0, cvx.sum(self.__weight) == 1]
-        self.__prob = cvx.Problem(cvx.Maximize(self.__obj), self.__constraints)
+        P_chol = {time: np.linalg.cholesky(matrix) for time, matrix in P.items()}
 
-    def solve(self, time, window=10, **kwargs):
-        """
-        Solves the covariance combination problem at a given time, i.e.,
-        finds the prediction for the covariance matrix at 'time+1'
-        """
-        
-
-        # Precompute parameter values for CVXPY problem (only do once)
-        if not self._initilized:
-            self._precompute(window)
-            self._initilized = True
-
-        # Update parameters and solve problem
-        self.__A_param.value = self.__A.loc[time]
-        self.__P_chol_param.value = self.__P_chol.loc[time]
-        self.__prob.solve(**kwargs)
+        # Compute A matrix
+        Ls_diag = pd.DataFrame({k: _diag_part(L) for k, L in self.__Ls_shifted.items()})
 
-        # Get non-shifted L
-        L = sum(self.Ls.loc[time]*self.__weight.value) # prediction for time+1
-        nu = sum(self.nus.loc[time]*self.__weight.value) # prediction for time+1
+        A = {
+            times[i]: _A(
+                Ls_diag.truncate(before=times[i - window + 1], after=times[i]), self.K
+            )
+            for i in range(window - 1, len(times))
+        }
+
+        problem = _CombinationProblem(
+            keys=self.sigmas.keys(), n=len(self.assets), window=window
+        )
+
+        for time in A.keys():
+            problem.A_param.value = A[time]
+            problem.P_chol_param.value = P_chol[time]
 
-        ### Conditioning
-        mean = np.linalg.inv(L.T)@nu # / 100
-        mean = pd.Series(index=self.assets, data=mean)
-        Sigma = np.linalg.inv(L @ L.T) # / 10000
-        Sigma = pd.DataFrame(index=self.assets, columns=self.assets, data=Sigma)
-        weights = pd.Series(index=self.__Sigmas.keys(), data=self.__weight.value)
-        return Result(time=time, window=window, mean=mean, covariance=Sigma, weights=weights)
+            yield self._solve(time=time, problem=problem, **kwargs)
 
-    def solve_window(self, window=10, verbose=True, **kwargs):
+    def _solve(self, time, problem, **kwargs):
         """
-        Solves the covariance combination problem for all timesteps
+        Solves the covariance combination problem at a given time t
         """
+        # solve problem
+        problem.solve(**kwargs)
+        weights = problem.weights
 
-        self._precompute(window)
-        self._initilized = True
-
-        if verbose:
-            for time in tqdm(self.index):
-                yield self.solve(time, window=window, **kwargs)
-        else:
-            for time in self.index:
-                yield self.solve(time, window=window, **kwargs)
+        # Get non-shifted L
+        L = sum(self.__Ls.loc[time] * weights.values)  # prediction for time+1
+        nu = sum(self.__nus.loc[time] * weights.values)  # prediction for time+1
 
+        mean = pd.Series(index=self.assets, data=np.linalg.inv(L.T) @ nu)
+        sigma = pd.DataFrame(
+            index=self.assets, columns=self.assets, data=np.linalg.inv(L @ L.T)
+        )
+        return Result(time=time, mean=mean, covariance=sigma, weights=weights)
```

### Comparing `cvxcovariance-0.0.5/pyproject.toml` & `cvxcovariance-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "cvxcovariance"
-version = "v0.0.5"             # Don't touch, leave at 0.0.0
+version = "v0.0.7"             # Don't touch, leave at 0.0.0
 description = "..."
-authors = ["Kasper", "Thomas"]
+authors = ["Kasper Johansson", "Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cov_pred_finance"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0"
-pandas = "<2.0.0"
+pandas = "*"
 cvxpy = "*"
+scipy = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.1.3"
 pytest-cov = "*"
 seaborn = "*"
 arch = "*"
 tqdm = "*"
 scikit-learn = "*"
 matplotlib = "*"
 loguru = "*"
 plotly = "*"
 jupyterlab = "*"
-
+cvxsimulator = "*"
 
 [build-system]
 requires = ["poetry>=1.0.2"]
 build-backend = "poetry.masonry.api"
```

