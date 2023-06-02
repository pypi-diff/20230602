# Comparing `tmp/autogluon.timeseries-0.7.1b20230601.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230601.tar", last modified: Thu Jun  1 09:04:11 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230602.tar", last modified: Fri Jun  2 09:04:07 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230601.tar` & `autogluon.timeseries-0.7.1b20230602.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.489497 autogluon.timeseries-0.7.1b20230601/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-06-01 09:04:11.489497 autogluon.timeseries-0.7.1b20230601/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:04:11.489497 autogluon.timeseries-0.7.1b20230601/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.481497 autogluon.timeseries-0.7.1b20230601/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.481497 autogluon.timeseries-0.7.1b20230601/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.489497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.489497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49496 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.489497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48286 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.489497 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-01 09:03:27.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 09:04:11.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:11.485497 autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-06-01 09:04:11.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-01 09:04:11.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:04:11.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:04:11.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-01 09:04:11.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:04:11.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:04:11.000000 autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.649790 autogluon.timeseries-0.7.1b20230602/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-06-02 09:04:07.649790 autogluon.timeseries-0.7.1b20230602/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:04:07.649790 autogluon.timeseries-0.7.1b20230602/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.641790 autogluon.timeseries-0.7.1b20230602/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.649790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.649790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.649790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.649790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49496 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.649790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48286 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.649790 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-02 09:03:27.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-02 09:04:07.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:07.645790 autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-06-02 09:04:07.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-02 09:04:07.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:04:07.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:04:07.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-02 09:04:07.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:04:07.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:04:07.000000 autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230601/PKG-INFO` & `autogluon.timeseries-0.7.1b20230602/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230601
+Version: 0.7.1b20230602
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230601/setup.py` & `autogluon.timeseries-0.7.1b20230602/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,69 +24,70 @@
 
     Prediction is parallelized across CPU cores using joblib.Parallel.
 
     Attributes
     ----------
     allowed_local_model_args : List[str]
         Argument that can be passed to the underlying local model.
-    max_ts_length : int, optional
-        If not None, only the last ``max_ts_length`` time steps of each time series will be used to train the model.
     default_n_jobs : Union[int, float]
         Default number of CPU cores used to train models. If float, this fraction of CPU cores will be used.
     init_time_in_seconds : int
         Time that it takes to initialize the model in seconds (e.g., because of JIT compilation by Numba).
         If time_limit is below this number, model won't be trained.
     """
 
     allowed_local_model_args: List[str] = []
-    max_ts_length: Optional[int] = None
     default_n_jobs: Union[int, float] = 0.5
     init_time_in_seconds: int = 0
 
     def __init__(
         self,
         freq: Optional[str] = None,
         prediction_length: int = 1,
         path: Optional[str] = None,
         name: Optional[str] = None,
         eval_metric: str = None,
         hyperparameters: Dict[str, Any] = None,
         **kwargs,  # noqa
     ):
-        super().__init__(
-            path=path,
-            freq=freq,
-            prediction_length=prediction_length,
-            name=name,
-            eval_metric=eval_metric,
-            hyperparameters=hyperparameters,
-            **kwargs,
-        )
         if hyperparameters is None:
             hyperparameters = {}
         # TODO: Replace with 'num_cpus' argument passed to fit (after predictor API is changed)
-        n_jobs = hyperparameters.get("n_jobs", self.default_n_jobs)
+        n_jobs = hyperparameters.pop("n_jobs", self.default_n_jobs)
         if isinstance(n_jobs, float) and 0 < n_jobs <= 1:
             self.n_jobs = max(int(cpu_count() * n_jobs), 1)
         elif isinstance(n_jobs, int):
             self.n_jobs = n_jobs
         else:
             raise ValueError(f"n_jobs must be a float between 0 and 1 or an integer (received n_jobs = {n_jobs})")
+        # Default values, potentially overridden inside _fit()
+        self.use_fallback_model = hyperparameters.pop("use_fallback_model", True)
+        self.max_ts_length = hyperparameters.pop("max_ts_length", 2500)
+
+        super().__init__(
+            path=path,
+            freq=freq,
+            prediction_length=prediction_length,
+            name=name,
+            eval_metric=eval_metric,
+            hyperparameters=hyperparameters,
+            **kwargs,
+        )
+
         self._local_model_args: Dict[str, Any] = None
         self._seasonal_period: Optional[int] = None
         self.time_limit: Optional[float] = None
 
     def _fit(self, train_data: TimeSeriesDataFrame, time_limit: int = None, **kwargs):
         self._check_fit_params()
         if time_limit is not None and time_limit < self.init_time_in_seconds:
             raise TimeLimitExceeded
 
         # Initialize parameters passed to each local model
         raw_local_model_args = self._get_model_params().copy()
-        raw_local_model_args.pop("n_jobs", None)
 
         unused_local_model_args = []
         local_model_args = {}
         for key, value in raw_local_model_args.items():
             if key in self.allowed_local_model_args:
                 local_model_args[key] = value
             else:
@@ -132,16 +133,16 @@
         except TimeoutError:
             raise TimeLimitExceeded
 
         number_failed_models = sum(failed_flag for _, failed_flag in predictions_with_flags)
         if number_failed_models > 0:
             fraction_failed_models = number_failed_models / len(predictions_with_flags)
             logger.warning(
-                f"\t{self.name} failed for {number_failed_models} time series ({100 * fraction_failed_models:.1f}%). "
-                "Fallback model SeasonalNaive was used for these time series."
+                f"\tWarning: {self.name} failed for {number_failed_models} time series "
+                f"({fraction_failed_models:.1%}). Fallback model SeasonalNaive was used for these time series."
             )
         predictions_df = pd.concat([pred for pred, _ in predictions_with_flags])
         predictions_df.index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length)
         return TimeSeriesDataFrame(predictions_df)
 
     def score_and_cache_oof(
         self, val_data: TimeSeriesDataFrame, store_val_score: bool = False, store_predict_time: bool = False
@@ -155,22 +156,25 @@
             raise TimeLimitExceeded
         try:
             result = self._predict_with_local_model(
                 time_series=time_series,
                 local_model_args=self._local_model_args.copy(),
             )
             model_failed = False
-        except Exception as e:
-            result = seasonal_naive_forecast(
-                target=time_series.values.ravel(),
-                prediction_length=self.prediction_length,
-                quantile_levels=self.quantile_levels,
-                seasonal_period=self._seasonal_period,
-            )
-            model_failed = True
+        except:
+            if self.use_fallback_model:
+                result = seasonal_naive_forecast(
+                    target=time_series.values.ravel(),
+                    prediction_length=self.prediction_length,
+                    quantile_levels=self.quantile_levels,
+                    seasonal_period=self._seasonal_period,
+                )
+                model_failed = True
+            else:
+                raise
         return result, model_failed
 
     def _predict_with_local_model(
         self,
         time_series: pd.Series,
         local_model_args: dict,
     ) -> pd.DataFrame:
```

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,19 +91,22 @@
         If True, non-zero mean is allowed.
     seasonal_period : int or None, default = None
         Number of time steps in a complete seasonal cycle for seasonal models. For example, 7 for daily data with a
         weekly cycle or 12 for monthly data with an annual cycle.
         When set to None, seasonal_period will be inferred from the frequency of the training data. Can also be
         specified manually by providing an integer > 1.
         If seasonal_period (inferred or provided) is equal to 1, seasonality will be disabled.
-    n_jobs : int or float, default = -1
+    n_jobs : int or float, default = 0.5
         Number of CPU cores used to fit the models in parallel.
         When set to a float between 0.0 and 1.0, that fraction of available CPU cores is used.
         When set to a positive integer, that many cores are used.
         When set to -1, all CPU cores are used.
+    max_ts_length : int, default = 2500
+        If not None, only the last ``max_ts_length`` time steps of each time series will be used to train the model.
+        This significantly speeds up fitting and usually leads to no change in accuracy.
     """
 
     allowed_local_model_args = [
         "d",
         "D",
         "max_p",
         "max_q",
@@ -118,15 +121,14 @@
         "stationary",
         "seasonal",
         "approximation",
         "allowdrift",
         "allowmean",
         "seasonal_period",
     ]
-    MAX_TS_LENGTH = 3000
 
     def _update_local_model_args(self, local_model_args: dict) -> dict:
         local_model_args = super()._update_local_model_args(local_model_args)
         local_model_args.setdefault("approximation", True)
         local_model_args.setdefault("allowmean", True)
         return local_model_args
 
@@ -151,19 +153,22 @@
         (additive error, no trend, and no seasonality), ETS will explore only a simple exponential smoothing.
     seasonal_period : int or None, default = None
         Number of time steps in a complete seasonal cycle for seasonal models. For example, 7 for daily data with a
         weekly cycle or 12 for monthly data with an annual cycle.
         When set to None, seasonal_period will be inferred from the frequency of the training data. Can also be
         specified manually by providing an integer > 1.
         If seasonal_period (inferred or provided) is equal to 1, seasonality will be disabled.
-    n_jobs : int or float, default = -1
+    n_jobs : int or float, default = 0.5
         Number of CPU cores used to fit the models in parallel.
         When set to a float between 0.0 and 1.0, that fraction of available CPU cores is used.
         When set to a positive integer, that many cores are used.
         When set to -1, all CPU cores are used.
+    max_ts_length : int, default = 2500
+        If not None, only the last ``max_ts_length`` time steps of each time series will be used to train the model.
+        This significantly speeds up fitting and usually leads to no change in accuracy.
     """
 
     allowed_local_model_args = [
         "model",
         "seasonal_period",
     ]
 
@@ -192,19 +197,22 @@
         Seasonal decomposition type.
     seasonal_period : int or None, default = None
         Number of time steps in a complete seasonal cycle for seasonal models. For example, 7 for daily data with a
         weekly cycle or 12 for monthly data with an annual cycle.
         When set to None, seasonal_period will be inferred from the frequency of the training data. Can also be
         specified manually by providing an integer > 1.
         If seasonal_period (inferred or provided) is equal to 1, seasonality will be disabled.
-    n_jobs : int or float, default = -1
+    n_jobs : int or float, default = 0.5
         Number of CPU cores used to fit the models in parallel.
         When set to a float between 0.0 and 1.0, that fraction of available CPU cores is used.
         When set to a positive integer, that many cores are used.
         When set to -1, all CPU cores are used.
+    max_ts_length : int, default = 2500
+        If not None, only the last ``max_ts_length`` time steps of each time series will be used to train the model.
+        This significantly speeds up fitting and usually leads to no change in accuracy.
     """
 
     allowed_local_model_args = [
         "decomposition_type",
         "seasonal_period",
     ]
 
@@ -233,19 +241,22 @@
         Seasonal decomposition type.
     seasonal_period : int or None, default = None
         Number of time steps in a complete seasonal cycle for seasonal models. For example, 7 for daily data with a
         weekly cycle or 12 for monthly data with an annual cycle.
         When set to None, seasonal_period will be inferred from the frequency of the training data. Can also be
         specified manually by providing an integer > 1.
         If seasonal_period (inferred or provided) is equal to 1, seasonality will be disabled.
-    n_jobs : int or float, default = -1
+    n_jobs : int or float, default = 0.5
         Number of CPU cores used to fit the models in parallel.
         When set to a float between 0.0 and 1.0, that fraction of available CPU cores is used.
         When set to a positive integer, that many cores are used.
         When set to -1, all CPU cores are used.
+    max_ts_length : int, default = 2500
+        If not None, only the last ``max_ts_length`` time steps of each time series will be used to train the model.
+        This significantly speeds up fitting and usually leads to no change in accuracy.
     """
 
     max_ts_length = 3000
 
     allowed_local_model_args = [
         "decomposition_type",
         "seasonal_period",
```

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,17 @@
     maxiter : int, default = 1000
         Number of iterations during optimization.
     n_jobs : int or float, default = 0.5
         Number of CPU cores used to fit the models in parallel.
         When set to a float between 0.0 and 1.0, that fraction of available CPU cores is used.
         When set to a positive integer, that many cores are used.
         When set to -1, all CPU cores are used.
+    max_ts_length : int, default = 2500
+        If not None, only the last ``max_ts_length`` time steps of each time series will be used to train the model.
+        This significantly speeds up fitting and usually leads to no change in accuracy.
     """
 
     allowed_local_model_args = [
         "error",
         "trend",
         "damped_trend",
         "seasonal",
@@ -180,26 +183,28 @@
     maxiter : int, default = 50
         Number of iterations during optimization.
     n_jobs : int or float, default = 0.5
         Number of CPU cores used to fit the models in parallel.
         When set to a float between 0.0 and 1.0, that fraction of available CPU cores is used.
         When set to a positive integer, that many cores are used.
         When set to -1, all CPU cores are used.
+    max_ts_length : int, default = 2500
+        If not None, only the last ``max_ts_length`` time steps of each time series will be used to train the model.
+        This significantly speeds up fitting and usually leads to no change in accuracy.
     """
 
     allowed_local_model_args = [
         "order",
         "seasonal_order",
         "seasonal_period",
         "trend",
         "enforce_stationarity",
         "enforce_invertibility",
         "maxiter",
     ]
-    MAX_TS_LENGTH = 3000
 
     def _update_local_model_args(self, local_model_args: Dict[str, Any]) -> Dict[str, Any]:
         local_model_args.setdefault("trend", "c")
         local_model_args.setdefault("order", (1, 1, 1))
         local_model_args.setdefault("maxiter", 50)
 
         seasonal_period = local_model_args.pop("seasonal_period")
@@ -284,14 +289,17 @@
     difference : bool, default = False
         Whether to difference the data before testing for seasonality.
     n_jobs : int or float, default = 0.5
         Number of CPU cores used to fit the models in parallel.
         When set to a float between 0.0 and 1.0, that fraction of available CPU cores is used.
         When set to a positive integer, that many cores are used.
         When set to -1, all CPU cores are used.
+    max_ts_length : int, default = 2500
+        If not None, only the last ``max_ts_length`` time steps of each time series will be used to train the model.
+        This significantly speeds up fitting and usually leads to no change in accuracy.
     """
 
     allowed_local_model_args = [
         "deseasonalize",
         "seasonal_period",
         "use_test",
         "method",
```

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230602/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230601
+Version: 0.7.1b20230602
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230601/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230602/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

