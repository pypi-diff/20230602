# Comparing `tmp/auto-surprise-0.1.8.tar.gz` & `tmp/auto-surprise-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-surprise-0.1.8.tar", last modified: Tue May  3 07:46:36 2022, max compression
+gzip compressed data, was "auto-surprise-0.1.9.tar", last modified: Fri Jun  2 20:00:35 2023, max compression
```

## Comparing `auto-surprise-0.1.8.tar` & `auto-surprise-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 07:46:36.604495 auto-surprise-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5900 2022-05-03 07:46:36.604495 auto-surprise-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 07:46:36.600494 auto-surprise-0.1.8/auto_surprise/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 07:46:36.600494 auto-surprise-0.1.8/auto_surprise/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/algorithms/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3943 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/algorithms/spaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 07:46:36.604495 auto-surprise-0.1.8/auto_surprise/context/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/context/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/context/limits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/context/result_logging_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 07:46:36.604495 auto-surprise-0.1.8/auto_surprise/strategies/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/strategies/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/strategies/basic_reduction.py
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/strategies/smbo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4551 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/auto_surprise/validation_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 07:46:36.600494 auto-surprise-0.1.8/auto_surprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5900 2022-05-03 07:46:36.000000 auto-surprise-0.1.8/auto_surprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-05-03 07:46:36.000000 auto-surprise-0.1.8/auto_surprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 07:46:36.000000 auto-surprise-0.1.8/auto_surprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-03 07:46:36.000000 auto-surprise-0.1.8/auto_surprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-05-03 07:46:36.000000 auto-surprise-0.1.8/auto_surprise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-03 07:46:36.604495 auto-surprise-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 07:46:36.604495 auto-surprise-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 07:46:36.604495 auto-surprise-0.1.8/tests/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/tests/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/tests/algorithms/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/tests/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/tests/test_validation_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-05-03 07:45:10.000000 auto-surprise-0.1.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:35.385398 auto-surprise-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-02 20:00:35.385398 auto-surprise-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:35.381398 auto-surprise-0.1.9/auto_surprise/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:35.381398 auto-surprise-0.1.9/auto_surprise/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/algorithms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/algorithms/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:35.385398 auto-surprise-0.1.9/auto_surprise/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/context/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/context/limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/context/result_logging_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:35.385398 auto-surprise-0.1.9/auto_surprise/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/strategies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/strategies/basic_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/strategies/smbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/auto_surprise/validation_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:35.381398 auto-surprise-0.1.9/auto_surprise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-02 20:00:35.000000 auto-surprise-0.1.9/auto_surprise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-02 20:00:35.000000 auto-surprise-0.1.9/auto_surprise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:00:35.000000 auto-surprise-0.1.9/auto_surprise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-02 20:00:35.000000 auto-surprise-0.1.9/auto_surprise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 20:00:35.000000 auto-surprise-0.1.9/auto_surprise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 20:00:35.385398 auto-surprise-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:35.385398 auto-surprise-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:35.385398 auto-surprise-0.1.9/tests/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/tests/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/tests/algorithms/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/tests/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/tests/test_validation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-02 19:57:54.000000 auto-surprise-0.1.9/tests/utils.py
```

### Comparing `auto-surprise-0.1.8/LICENSE` & `auto-surprise-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/PKG-INFO` & `auto-surprise-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,113 @@
 Metadata-Version: 2.1
 Name: auto-surprise
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package that automates algorithm selection and hyperparameter tuning for the recommender system library Surprise
-Home-page: https://github.com/BeelGroup/Auto-Surprise
+Home-page: https://github.com/ISG-Siegen/Auto-Surprise
 Author: Rohan Anand
 Author-email: anandr@tcd.ie
-License: UNKNOWN
-Description: # Auto-Surprise
-        
-        ![GitHub release (latest by date)](https://img.shields.io/github/v/release/BeelGroup/Auto-Surprise) ![PyPI](https://img.shields.io/pypi/v/Auto-Surprise.svg) [![Downloads](https://pepy.tech/badge/auto-surprise)](https://pepy.tech/project/auto-surprise) ![Codecov](https://img.shields.io/codecov/c/github/BeelGroup/Auto-Surprise.svg) ![Travis (.org)](https://img.shields.io/travis/BeelGroup/Auto-Surprise.svg)
-        
-        Auto-Surprise is built as a wrapper around the Python [Surprise](https://surprise.readthedocs.io/en/stable/index.html) recommender-system library. It automates algorithm selection and hyper parameter optimization in a highly parallelized manner. 
-        
-        - Documentation is available at [Auto-Surprise ReadTheDocs](https://auto-surprise.readthedocs.io/en/stable/)
-        - AutoSurprise is currently in development.
-        
-        # Setup
-        
-        Auto-Surprise is easy to install with Pip, and required Python>=3.6 installed on a linux system. Currently not supported in windows, but can be used using [WSL](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
-        
-        ```bash
-        $ pip install auto-surprise
-        ```
-        
-        # Usage
-        
-        Basic usage of AutoSurprise is given below.
-        
-        ```python
-        from surprise import Dataset
-        from auto_surprise.engine import Engine
-        
-        # Load the dataset
-        data = Dataset.load_builtin('ml-100k')
-        
-        # Intitialize auto surprise engine
-        engine = Engine(verbose=True)
-        
-        # Start the trainer
-        best_algo, best_params, best_score, tasks = engine.train(
-            data=data, 
-            target_metric='test_rmse', 
-            cpu_time_limit=60 * 60, 
-            max_evals=100
-        )
-        ```
-        
-        In the above example, we first initialize the `Engine`. We then run `engine.train()` to begin training our model. To train the model we need to pass the following
-        
-        - `data` : The data as an instance of `surprise.dataset.DatasetAutoFolds`. Please read [Surprise Dataset docs](https://surprise.readthedocs.io/en/stable/dataset.html)
-        - `target_metric` : The metric we seek to minimize. Available options are `test_rmse` and `test_mae`.
-        - `cpu_time_limit` : The time limit we want to train. This is in seconds. For datasets like Movielens 100k, 1 hour is sufficient. But you may want to increase this based on the size of your dataset
-        - `max_evals`: The maximum number of evaluations each algorithm gets for hyper parameter optimization.
-        - `hpo_algo`: Auto-Surprise uses Hyperopt for hyperparameter tuning. By default, it's set to use TPE, but you can change this to any algorithm supported by hyperopt, such as Adaptive TPE or Random search.
-        
-        ## Setting the Hyperparameter Optimization Algorithm
-        
-        Auto-Surprise uses Hyperopt. You can change the HPO algo as shown below.
-        
-        ```python
-        # Example for setting the HPO algorithm to adaptive TPE
-        import hyperopt
-        
-        ...
-        
-        engine = Engine(verbose=True)
-        engine.train(
-            data=data,
-            target_metric='test_rmse',
-            cpu_time_limit=60 * 60,
-            max_evals=100,
-            hpo_algo=hyperopt.atpe.suggest
-        )
-        ```
-        
-        ## Building back the best model
-        
-        You can build a pickelable model as shown.
-        
-        ```python
-        model = engine.build_model(best_algo, best_params)
-        ```
-        
-        # Benchmarks
-        
-        In my testing, Auto-Surprise performed anywhere from 0.8 to 4% improvement in RMSE compared to the best performing default algorithm configuration. In the table below are the results for the Jester 2 dataset. Benchmark results for Movielens and Book-Crossing dataset are also available [here](https://auto-surprise.readthedocs.io/en/stable/benchmarks/results.html)
-        
-        |       Algorithm      |  RMSE  |   MAE  |   Time   |
-        |:--------------------:|:------:|:------:|:--------:|
-        | Normal Predictor     |  7.277 |  5.886 | 00:00:01 |
-        | SVD                  |  4.905 |  3.97  | 00:00:13 |
-        | SVD++                |  5.102 |  4.055 | 00:00:29 |
-        | NMF                  |   --   |   --   |    --    |
-        | Slope One            |  5.189 |  3.945 | 00:00:02 |
-        | KNN Basic            |  5.078 |  4.034 | 00:02:14 |
-        | KNN with Means       |  5.124 |  3.955 | 00:02:16 |
-        | KNN with   Z-score   |  5.219 |  3.955 | 00:02:20 |
-        | KNN Baseline         |  4.898 |  3.896 | 00:02:14 |
-        | Co-clustering        |  5.153 |  3.917 | 00:00:12 |
-        | Baseline Only        |  4.849 |  3.934 | 00:00:01 |
-        | GridSearch           | 4.7409 | 3.8147 | 80:52:35 |
-        | Auto-Surprise (TPE)  | 4.6489 | 3.6837 | 02:00:10 |
-        | Auto-Surprise (ATPE) | 4.6555 | 3.6906 | 02:00:01 |
-        
-        # Papers
-        
-        [Auto-Surprise: An Automated Recommender-System (AutoRecSys) Library with Tree of Parzens Estimator (TPE) Optimization](https://dl.acm.org/doi/abs/10.1145/3383313.3411467?casa_token=ADmaOhK2tHgAAAAA:4UXHmuLXM_gJYQdUZp7ab5hwn-eNv2Daot5FtfYLG3m1KYLc99Y1_rhwzY2qcCJySUhoFBAfGnt5Qg)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Auto-Surprise
+
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/BeelGroup/Auto-Surprise) ![PyPI](https://img.shields.io/pypi/v/Auto-Surprise.svg) [![Downloads](https://pepy.tech/badge/auto-surprise)](https://pepy.tech/project/auto-surprise)
+Auto-Surprise is built as a wrapper around the Python [Surprise](https://surprise.readthedocs.io/en/stable/index.html) recommender-system library. It automates algorithm selection and hyper parameter optimization in a highly parallelized manner. 
+
+- Documentation is available at [Auto-Surprise ReadTheDocs](https://auto-surprise.readthedocs.io/en/stable/)
+- AutoSurprise is currently in development.
+
+# Setup
+
+Auto-Surprise is easy to install with Pip, and required Python>=3.6 installed on a linux system. Currently not supported in windows, but can be used using [WSL](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
+
+```bash
+$ pip install auto-surprise
+```
+
+# Usage
+
+Basic usage of AutoSurprise is given below.
+
+```python
+from surprise import Dataset
+from auto_surprise.engine import Engine
+
+# Load the dataset
+data = Dataset.load_builtin('ml-100k')
+
+# Intitialize auto surprise engine
+engine = Engine(verbose=True)
+
+# Start the trainer
+best_algo, best_params, best_score, tasks = engine.train(
+    data=data, 
+    target_metric='test_rmse', 
+    cpu_time_limit=60 * 60, 
+    max_evals=100
+)
+```
+
+In the above example, we first initialize the `Engine`. We then run `engine.train()` to begin training our model. To train the model we need to pass the following
+
+- `data` : The data as an instance of `surprise.dataset.DatasetAutoFolds`. Please read [Surprise Dataset docs](https://surprise.readthedocs.io/en/stable/dataset.html)
+- `target_metric` : The metric we seek to minimize. Available options are `test_rmse` and `test_mae`.
+- `cpu_time_limit` : The time limit we want to train. This is in seconds. For datasets like Movielens 100k, 1 hour is sufficient. But you may want to increase this based on the size of your dataset
+- `max_evals`: The maximum number of evaluations each algorithm gets for hyper parameter optimization.
+- `hpo_algo`: Auto-Surprise uses Hyperopt for hyperparameter tuning. By default, it's set to use TPE, but you can change this to any algorithm supported by hyperopt, such as Adaptive TPE or Random search.
+
+## Setting the Hyperparameter Optimization Algorithm
+
+Auto-Surprise uses Hyperopt. You can change the HPO algo as shown below.
+
+```python
+# Example for setting the HPO algorithm to adaptive TPE
+import hyperopt
+
+...
+
+engine = Engine(verbose=True)
+engine.train(
+    data=data,
+    target_metric='test_rmse',
+    cpu_time_limit=60 * 60,
+    max_evals=100,
+    hpo_algo=hyperopt.atpe.suggest
+)
+```
+
+## Building back the best model
+
+You can build a pickelable model as shown.
+
+```python
+model = engine.build_model(best_algo, best_params)
+```
+
+# Benchmarks
+
+In my testing, Auto-Surprise performed anywhere from 0.8 to 4% improvement in RMSE compared to the best performing default algorithm configuration. In the table below are the results for the Jester 2 dataset. Benchmark results for Movielens and Book-Crossing dataset are also available [here](https://auto-surprise.readthedocs.io/en/stable/benchmarks/results.html)
+
+|       Algorithm      |  RMSE  |   MAE  |   Time   |
+|:--------------------:|:------:|:------:|:--------:|
+| Normal Predictor     |  7.277 |  5.886 | 00:00:01 |
+| SVD                  |  4.905 |  3.97  | 00:00:13 |
+| SVD++                |  5.102 |  4.055 | 00:00:29 |
+| NMF                  |   --   |   --   |    --    |
+| Slope One            |  5.189 |  3.945 | 00:00:02 |
+| KNN Basic            |  5.078 |  4.034 | 00:02:14 |
+| KNN with Means       |  5.124 |  3.955 | 00:02:16 |
+| KNN with   Z-score   |  5.219 |  3.955 | 00:02:20 |
+| KNN Baseline         |  4.898 |  3.896 | 00:02:14 |
+| Co-clustering        |  5.153 |  3.917 | 00:00:12 |
+| Baseline Only        |  4.849 |  3.934 | 00:00:01 |
+| GridSearch           | 4.7409 | 3.8147 | 80:52:35 |
+| Auto-Surprise (TPE)  | 4.6489 | 3.6837 | 02:00:10 |
+| Auto-Surprise (ATPE) | 4.6555 | 3.6906 | 02:00:01 |
+
+# Papers
+
+[Auto-Surprise: An Automated Recommender-System (AutoRecSys) Library with Tree of Parzens Estimator (TPE) Optimization](https://dl.acm.org/doi/abs/10.1145/3383313.3411467?casa_token=ADmaOhK2tHgAAAAA:4UXHmuLXM_gJYQdUZp7ab5hwn-eNv2Daot5FtfYLG3m1KYLc99Y1_rhwzY2qcCJySUhoFBAfGnt5Qg)
```

### Comparing `auto-surprise-0.1.8/README.md` & `auto-surprise-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Auto-Surprise
 
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/BeelGroup/Auto-Surprise) ![PyPI](https://img.shields.io/pypi/v/Auto-Surprise.svg) [![Downloads](https://pepy.tech/badge/auto-surprise)](https://pepy.tech/project/auto-surprise) ![Codecov](https://img.shields.io/codecov/c/github/BeelGroup/Auto-Surprise.svg) ![Travis (.org)](https://img.shields.io/travis/BeelGroup/Auto-Surprise.svg)
-
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/BeelGroup/Auto-Surprise) ![PyPI](https://img.shields.io/pypi/v/Auto-Surprise.svg) [![Downloads](https://pepy.tech/badge/auto-surprise)](https://pepy.tech/project/auto-surprise)
 Auto-Surprise is built as a wrapper around the Python [Surprise](https://surprise.readthedocs.io/en/stable/index.html) recommender-system library. It automates algorithm selection and hyper parameter optimization in a highly parallelized manner. 
 
 - Documentation is available at [Auto-Surprise ReadTheDocs](https://auto-surprise.readthedocs.io/en/stable/)
 - AutoSurprise is currently in development.
 
 # Setup
```

### Comparing `auto-surprise-0.1.8/auto_surprise/algorithms/base.py` & `auto-surprise-0.1.9/auto_surprise/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise/algorithms/spaces.py` & `auto-surprise-0.1.9/auto_surprise/algorithms/spaces.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise/constants.py` & `auto-surprise-0.1.9/auto_surprise/constants.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise/context/backend.py` & `auto-surprise-0.1.9/auto_surprise/context/backend.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise/context/limits.py` & `auto-surprise-0.1.9/auto_surprise/context/limits.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise/context/result_logging_manager.py` & `auto-surprise-0.1.9/auto_surprise/context/result_logging_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import time
 import datetime
-import pathlib
 import logging
 
 class ResultLoggingManager:
     """
     Log results of each algorithm
     """
```

### Comparing `auto-surprise-0.1.8/auto_surprise/engine.py` & `auto-surprise-0.1.9/auto_surprise/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from auto_surprise.strategies.smbo import SMBO
 from auto_surprise.__version__ import __version__
 import auto_surprise.validation_util as validation_util
 
 
 class Engine(object):
     def __init__(
-        self, verbose=True, algorithms=FULL_ALGO_LIST, random_state=numpy.random
+        self, verbose=True, algorithms=FULL_ALGO_LIST, random_state=numpy.random.default_rng()
     ):
         """
         Initialize new engine
         """
         self.__logger = logging.getLogger(__name__)
         self.verbose = verbose
         self.algorithms = algorithms
```

### Comparing `auto-surprise-0.1.8/auto_surprise/strategies/base.py` & `auto-surprise-0.1.9/auto_surprise/strategies/base.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise/strategies/basic_reduction.py` & `auto-surprise-0.1.9/auto_surprise/strategies/basic_reduction.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise/strategies/smbo.py` & `auto-surprise-0.1.9/auto_surprise/strategies/smbo.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise/trainer.py` & `auto-surprise-0.1.9/auto_surprise/trainer.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise/validation_util.py` & `auto-surprise-0.1.9/auto_surprise/validation_util.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/auto_surprise.egg-info/PKG-INFO` & `auto-surprise-0.1.9/auto_surprise.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,113 @@
 Metadata-Version: 2.1
 Name: auto-surprise
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package that automates algorithm selection and hyperparameter tuning for the recommender system library Surprise
-Home-page: https://github.com/BeelGroup/Auto-Surprise
+Home-page: https://github.com/ISG-Siegen/Auto-Surprise
 Author: Rohan Anand
 Author-email: anandr@tcd.ie
-License: UNKNOWN
-Description: # Auto-Surprise
-        
-        ![GitHub release (latest by date)](https://img.shields.io/github/v/release/BeelGroup/Auto-Surprise) ![PyPI](https://img.shields.io/pypi/v/Auto-Surprise.svg) [![Downloads](https://pepy.tech/badge/auto-surprise)](https://pepy.tech/project/auto-surprise) ![Codecov](https://img.shields.io/codecov/c/github/BeelGroup/Auto-Surprise.svg) ![Travis (.org)](https://img.shields.io/travis/BeelGroup/Auto-Surprise.svg)
-        
-        Auto-Surprise is built as a wrapper around the Python [Surprise](https://surprise.readthedocs.io/en/stable/index.html) recommender-system library. It automates algorithm selection and hyper parameter optimization in a highly parallelized manner. 
-        
-        - Documentation is available at [Auto-Surprise ReadTheDocs](https://auto-surprise.readthedocs.io/en/stable/)
-        - AutoSurprise is currently in development.
-        
-        # Setup
-        
-        Auto-Surprise is easy to install with Pip, and required Python>=3.6 installed on a linux system. Currently not supported in windows, but can be used using [WSL](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
-        
-        ```bash
-        $ pip install auto-surprise
-        ```
-        
-        # Usage
-        
-        Basic usage of AutoSurprise is given below.
-        
-        ```python
-        from surprise import Dataset
-        from auto_surprise.engine import Engine
-        
-        # Load the dataset
-        data = Dataset.load_builtin('ml-100k')
-        
-        # Intitialize auto surprise engine
-        engine = Engine(verbose=True)
-        
-        # Start the trainer
-        best_algo, best_params, best_score, tasks = engine.train(
-            data=data, 
-            target_metric='test_rmse', 
-            cpu_time_limit=60 * 60, 
-            max_evals=100
-        )
-        ```
-        
-        In the above example, we first initialize the `Engine`. We then run `engine.train()` to begin training our model. To train the model we need to pass the following
-        
-        - `data` : The data as an instance of `surprise.dataset.DatasetAutoFolds`. Please read [Surprise Dataset docs](https://surprise.readthedocs.io/en/stable/dataset.html)
-        - `target_metric` : The metric we seek to minimize. Available options are `test_rmse` and `test_mae`.
-        - `cpu_time_limit` : The time limit we want to train. This is in seconds. For datasets like Movielens 100k, 1 hour is sufficient. But you may want to increase this based on the size of your dataset
-        - `max_evals`: The maximum number of evaluations each algorithm gets for hyper parameter optimization.
-        - `hpo_algo`: Auto-Surprise uses Hyperopt for hyperparameter tuning. By default, it's set to use TPE, but you can change this to any algorithm supported by hyperopt, such as Adaptive TPE or Random search.
-        
-        ## Setting the Hyperparameter Optimization Algorithm
-        
-        Auto-Surprise uses Hyperopt. You can change the HPO algo as shown below.
-        
-        ```python
-        # Example for setting the HPO algorithm to adaptive TPE
-        import hyperopt
-        
-        ...
-        
-        engine = Engine(verbose=True)
-        engine.train(
-            data=data,
-            target_metric='test_rmse',
-            cpu_time_limit=60 * 60,
-            max_evals=100,
-            hpo_algo=hyperopt.atpe.suggest
-        )
-        ```
-        
-        ## Building back the best model
-        
-        You can build a pickelable model as shown.
-        
-        ```python
-        model = engine.build_model(best_algo, best_params)
-        ```
-        
-        # Benchmarks
-        
-        In my testing, Auto-Surprise performed anywhere from 0.8 to 4% improvement in RMSE compared to the best performing default algorithm configuration. In the table below are the results for the Jester 2 dataset. Benchmark results for Movielens and Book-Crossing dataset are also available [here](https://auto-surprise.readthedocs.io/en/stable/benchmarks/results.html)
-        
-        |       Algorithm      |  RMSE  |   MAE  |   Time   |
-        |:--------------------:|:------:|:------:|:--------:|
-        | Normal Predictor     |  7.277 |  5.886 | 00:00:01 |
-        | SVD                  |  4.905 |  3.97  | 00:00:13 |
-        | SVD++                |  5.102 |  4.055 | 00:00:29 |
-        | NMF                  |   --   |   --   |    --    |
-        | Slope One            |  5.189 |  3.945 | 00:00:02 |
-        | KNN Basic            |  5.078 |  4.034 | 00:02:14 |
-        | KNN with Means       |  5.124 |  3.955 | 00:02:16 |
-        | KNN with   Z-score   |  5.219 |  3.955 | 00:02:20 |
-        | KNN Baseline         |  4.898 |  3.896 | 00:02:14 |
-        | Co-clustering        |  5.153 |  3.917 | 00:00:12 |
-        | Baseline Only        |  4.849 |  3.934 | 00:00:01 |
-        | GridSearch           | 4.7409 | 3.8147 | 80:52:35 |
-        | Auto-Surprise (TPE)  | 4.6489 | 3.6837 | 02:00:10 |
-        | Auto-Surprise (ATPE) | 4.6555 | 3.6906 | 02:00:01 |
-        
-        # Papers
-        
-        [Auto-Surprise: An Automated Recommender-System (AutoRecSys) Library with Tree of Parzens Estimator (TPE) Optimization](https://dl.acm.org/doi/abs/10.1145/3383313.3411467?casa_token=ADmaOhK2tHgAAAAA:4UXHmuLXM_gJYQdUZp7ab5hwn-eNv2Daot5FtfYLG3m1KYLc99Y1_rhwzY2qcCJySUhoFBAfGnt5Qg)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Auto-Surprise
+
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/BeelGroup/Auto-Surprise) ![PyPI](https://img.shields.io/pypi/v/Auto-Surprise.svg) [![Downloads](https://pepy.tech/badge/auto-surprise)](https://pepy.tech/project/auto-surprise)
+Auto-Surprise is built as a wrapper around the Python [Surprise](https://surprise.readthedocs.io/en/stable/index.html) recommender-system library. It automates algorithm selection and hyper parameter optimization in a highly parallelized manner. 
+
+- Documentation is available at [Auto-Surprise ReadTheDocs](https://auto-surprise.readthedocs.io/en/stable/)
+- AutoSurprise is currently in development.
+
+# Setup
+
+Auto-Surprise is easy to install with Pip, and required Python>=3.6 installed on a linux system. Currently not supported in windows, but can be used using [WSL](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
+
+```bash
+$ pip install auto-surprise
+```
+
+# Usage
+
+Basic usage of AutoSurprise is given below.
+
+```python
+from surprise import Dataset
+from auto_surprise.engine import Engine
+
+# Load the dataset
+data = Dataset.load_builtin('ml-100k')
+
+# Intitialize auto surprise engine
+engine = Engine(verbose=True)
+
+# Start the trainer
+best_algo, best_params, best_score, tasks = engine.train(
+    data=data, 
+    target_metric='test_rmse', 
+    cpu_time_limit=60 * 60, 
+    max_evals=100
+)
+```
+
+In the above example, we first initialize the `Engine`. We then run `engine.train()` to begin training our model. To train the model we need to pass the following
+
+- `data` : The data as an instance of `surprise.dataset.DatasetAutoFolds`. Please read [Surprise Dataset docs](https://surprise.readthedocs.io/en/stable/dataset.html)
+- `target_metric` : The metric we seek to minimize. Available options are `test_rmse` and `test_mae`.
+- `cpu_time_limit` : The time limit we want to train. This is in seconds. For datasets like Movielens 100k, 1 hour is sufficient. But you may want to increase this based on the size of your dataset
+- `max_evals`: The maximum number of evaluations each algorithm gets for hyper parameter optimization.
+- `hpo_algo`: Auto-Surprise uses Hyperopt for hyperparameter tuning. By default, it's set to use TPE, but you can change this to any algorithm supported by hyperopt, such as Adaptive TPE or Random search.
+
+## Setting the Hyperparameter Optimization Algorithm
+
+Auto-Surprise uses Hyperopt. You can change the HPO algo as shown below.
+
+```python
+# Example for setting the HPO algorithm to adaptive TPE
+import hyperopt
+
+...
+
+engine = Engine(verbose=True)
+engine.train(
+    data=data,
+    target_metric='test_rmse',
+    cpu_time_limit=60 * 60,
+    max_evals=100,
+    hpo_algo=hyperopt.atpe.suggest
+)
+```
+
+## Building back the best model
+
+You can build a pickelable model as shown.
+
+```python
+model = engine.build_model(best_algo, best_params)
+```
+
+# Benchmarks
+
+In my testing, Auto-Surprise performed anywhere from 0.8 to 4% improvement in RMSE compared to the best performing default algorithm configuration. In the table below are the results for the Jester 2 dataset. Benchmark results for Movielens and Book-Crossing dataset are also available [here](https://auto-surprise.readthedocs.io/en/stable/benchmarks/results.html)
+
+|       Algorithm      |  RMSE  |   MAE  |   Time   |
+|:--------------------:|:------:|:------:|:--------:|
+| Normal Predictor     |  7.277 |  5.886 | 00:00:01 |
+| SVD                  |  4.905 |  3.97  | 00:00:13 |
+| SVD++                |  5.102 |  4.055 | 00:00:29 |
+| NMF                  |   --   |   --   |    --    |
+| Slope One            |  5.189 |  3.945 | 00:00:02 |
+| KNN Basic            |  5.078 |  4.034 | 00:02:14 |
+| KNN with Means       |  5.124 |  3.955 | 00:02:16 |
+| KNN with   Z-score   |  5.219 |  3.955 | 00:02:20 |
+| KNN Baseline         |  4.898 |  3.896 | 00:02:14 |
+| Co-clustering        |  5.153 |  3.917 | 00:00:12 |
+| Baseline Only        |  4.849 |  3.934 | 00:00:01 |
+| GridSearch           | 4.7409 | 3.8147 | 80:52:35 |
+| Auto-Surprise (TPE)  | 4.6489 | 3.6837 | 02:00:10 |
+| Auto-Surprise (ATPE) | 4.6555 | 3.6906 | 02:00:01 |
+
+# Papers
+
+[Auto-Surprise: An Automated Recommender-System (AutoRecSys) Library with Tree of Parzens Estimator (TPE) Optimization](https://dl.acm.org/doi/abs/10.1145/3383313.3411467?casa_token=ADmaOhK2tHgAAAAA:4UXHmuLXM_gJYQdUZp7ab5hwn-eNv2Daot5FtfYLG3m1KYLc99Y1_rhwzY2qcCJySUhoFBAfGnt5Qg)
```

### Comparing `auto-surprise-0.1.8/auto_surprise.egg-info/SOURCES.txt` & `auto-surprise-0.1.9/auto_surprise.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 auto_surprise/__init__.py
 auto_surprise/__version__.py
 auto_surprise/constants.py
 auto_surprise/engine.py
 auto_surprise/exceptions.py
```

### Comparing `auto-surprise-0.1.8/setup.py` & `auto-surprise-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-"""
-When updating version
-
-- Update version and download URL here
-- Update release version in Docs configuration
-"""
-
 import setuptools
 
-install_requires = [
-    "hyperopt>=0.2.5",
-    "numpy",
-    "scikit-learn>=0.23.0",
-    "scikit-surprise",
-    "rich"
-]
+with open("requirements.txt", "r") as fh:
+    install_requires =[line.strip() for line in fh.read().split("\n")]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("auto_surprise/__version__.py") as fh:
     version = fh.readlines()[-1].split()[-1].strip("\"'")
 
@@ -25,15 +13,15 @@
     name="auto-surprise",
     version=version,
     author="Rohan Anand",
     author_email="anandr@tcd.ie",
     description="A python package that automates algorithm selection and hyperparameter tuning for the recommender system library Surprise",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/BeelGroup/Auto-Surprise",
+    url="https://github.com/ISG-Siegen/Auto-Surprise",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
```

### Comparing `auto-surprise-0.1.8/tests/algorithms/test_base.py` & `auto-surprise-0.1.9/tests/algorithms/test_base.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/tests/test_engine.py` & `auto-surprise-0.1.9/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/tests/test_trainer.py` & `auto-surprise-0.1.9/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/tests/test_validation_util.py` & `auto-surprise-0.1.9/tests/test_validation_util.py`

 * *Files identical despite different names*

### Comparing `auto-surprise-0.1.8/tests/utils.py` & `auto-surprise-0.1.9/tests/utils.py`

 * *Files identical despite different names*

