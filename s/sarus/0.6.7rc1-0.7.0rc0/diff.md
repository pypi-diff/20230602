# Comparing `tmp/sarus-0.6.7rc1.tar.gz` & `tmp/sarus-0.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.6.7rc1.tar", last modified: Tue May 30 19:12:41 2023, max compression
+gzip compressed data, was "sarus-0.7.0rc0.tar", last modified: Fri Jun  2 15:37:40 2023, max compression
```

## Comparing `sarus-0.6.7rc1.tar` & `sarus-0.7.0rc0.tar`

### file list

```diff
@@ -1,104 +1,98 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.295837 sarus-0.6.7rc1/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-05-30 19:12:41.295837 sarus-0.6.7rc1/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.7rc1/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.7rc1/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.283836 sarus-0.6.7rc1/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      547 2023-05-30 14:13:21.000000 sarus-0.6.7rc1/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13201 2023-05-26 07:33:58.000000 sarus-0.6.7rc1/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.283836 sarus-0.6.7rc1/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-25 13:23:23.000000 sarus-0.6.7rc1/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13842 2023-05-25 13:23:26.000000 sarus-0.6.7rc1/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.283836 sarus-0.6.7rc1/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.283836 sarus-0.6.7rc1/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.287836 sarus-0.6.7rc1/sarus/legacy/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-05-25 13:23:23.000000 sarus-0.6.7rc1/sarus/legacy/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-05-25 13:23:23.000000 sarus-0.6.7rc1/sarus/legacy/pandas/dataframe.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.287836 sarus-0.6.7rc1/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.287836 sarus-0.6.7rc1/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7609 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.287836 sarus-0.6.7rc1/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-05-25 13:23:26.000000 sarus-0.6.7rc1/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    20847 2023-05-25 13:23:26.000000 sarus-0.6.7rc1/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.287836 sarus-0.6.7rc1/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.287836 sarus-0.6.7rc1/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-05-26 07:33:58.000000 sarus-0.6.7rc1/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-05-25 13:23:26.000000 sarus-0.6.7rc1/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.291836 sarus-0.6.7rc1/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.291836 sarus-0.6.7rc1/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    55850 2023-05-25 13:23:23.000000 sarus-0.6.7rc1/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.291836 sarus-0.6.7rc1/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.291836 sarus-0.6.7rc1/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.291836 sarus-0.6.7rc1/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.291836 sarus-0.6.7rc1/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.291836 sarus-0.6.7rc1/sarus/storage/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-25 13:23:23.000000 sarus-0.6.7rc1/sarus/storage/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-05-25 13:23:23.000000 sarus-0.6.7rc1/sarus/storage/legacy_local.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.291836 sarus-0.6.7rc1/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.291836 sarus-0.6.7rc1/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.6.7rc1/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.283836 sarus-0.6.7rc1/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-05-30 19:12:41.000000 sarus-0.6.7rc1/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-30 19:12:41.000000 sarus-0.6.7rc1/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-30 19:12:41.000000 sarus-0.6.7rc1/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.7rc1/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      358 2023-05-30 19:12:41.000000 sarus-0.6.7rc1/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-30 19:12:41.000000 sarus-0.6.7rc1/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1318 2023-05-30 19:12:41.295837 sarus-0.6.7rc1/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      109 2023-05-30 19:12:00.000000 sarus-0.6.7rc1/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-30 19:12:41.295837 sarus-0.6.7rc1/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.7rc1/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.7.0rc0/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.7.0rc0/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.501549 sarus-0.7.0rc0/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      547 2023-06-02 15:33:14.000000 sarus-0.7.0rc0/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13201 2023-06-02 08:49:56.000000 sarus-0.7.0rc0/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.501549 sarus-0.7.0rc0/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2023-06-02 15:33:20.000000 sarus-0.7.0rc0/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13990 2023-06-02 08:52:35.000000 sarus-0.7.0rc0/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.505549 sarus-0.7.0rc0/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.505549 sarus-0.7.0rc0/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.505549 sarus-0.7.0rc0/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7609 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-05-25 13:23:26.000000 sarus-0.7.0rc0/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    20847 2023-05-25 13:23:26.000000 sarus-0.7.0rc0/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-06-02 08:49:56.000000 sarus-0.7.0rc0/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-06-02 08:49:56.000000 sarus-0.7.0rc0/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42677 2023-06-02 15:33:20.000000 sarus-0.7.0rc0/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/scripts/generate_op_list.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.529549 sarus-0.7.0rc0/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.529549 sarus-0.7.0rc0/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.501549 sarus-0.7.0rc0/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1965 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.7.0rc0/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      342 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1301 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      109 2023-06-02 15:34:08.000000 sarus-0.7.0rc0/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.7.0rc0/tests/test_sanity.py
```

### Comparing `sarus-0.6.7rc1/PKG-INFO` & `sarus-0.7.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.7rc1
+Version: 0.7.0rc0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.7rc1/README.rst` & `sarus-0.7.0rc0/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/__init__.py` & `sarus-0.7.0rc0/sarus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.6.7rc0"
+VERSION = "0.6.7rc1"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.6.7rc1/sarus/config.yaml` & `sarus-0.7.0rc0/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/context/local_sdk.py` & `sarus-0.7.0rc0/sarus/context/local_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from sarus_data_spec.attribute import Attribute
 from sarus_data_spec.context.public import Public as PublicContext
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.factory import Factory
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.schema import Schema
 
-# from sarus.storage.local import Storage
 from sarus_data_spec.storage.local import Storage
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 from sarus.dataspec_wrapper import MetaWrapper
 from sarus.manager.sdk_manager import SDKManager, manager
 from sarus.typing import Client
```

### Comparing `sarus-0.6.7rc1/sarus/dataspec_wrapper.py` & `sarus-0.7.0rc0/sarus/dataspec_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import inspect
 import logging
 from typing import (
     Any,
     Dict,
     Generic,
     List,
+    Literal,
     Optional,
     Tuple,
     TypeVar,
     Union,
     cast,
     get_args,
 )
@@ -161,15 +162,18 @@
         symbols = dict()
         for uuid, _id in DataSpecWrapper.instances.items():
             symbols[uuid] = mapping.get(_id, None)
         return symbols
 
     def dot(
         self,
-        kind: Union[DataSpecVariant, str] = DataSpecVariant.ALTERNATIVE,
+        kind: Union[
+            DataSpecVariant,
+            Literal["alternative", "mock", "user_defined", "synthetic"],
+        ] = "alternative",
         remote: bool = True,
     ) -> str:
         """Graphviz's dot representation of the DataSpecWrapper graph.
 
         Uses color codes to show statuses.
 
         Args:
@@ -177,14 +181,15 @@
             remote (true): Which Manager to inspect.
                 If true shows the DataSpec's status on the server,
                 else show the DataSpec's status locally.
         """
         if isinstance(kind, str):
             kind = DataSpecVariant(kind)
         ds = self.dataspec(kind)
+        self.alternative_dataspec()  # send to the server
         caller_frame = inspect.currentframe().f_back
         symbols = self.dataspec_wrapper_symbols(
             caller_frame.f_locals, caller_frame.f_globals
         )
         return self.manager().dot(ds, symbols=symbols, remote=remote)
 
     def alternative_dataspec(
```

### Comparing `sarus-0.6.7rc1/sarus/debug.py` & `sarus-0.7.0rc0/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/imblearn/over_sampling.py` & `sarus-0.7.0rc0/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/imblearn/pipeline.py` & `sarus-0.7.0rc0/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/imblearn/under_sampling.py` & `sarus-0.7.0rc0/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/legacy/tensorflow/dataset.py` & `sarus-0.7.0rc0/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/legacy/tensorflow/model.py` & `sarus-0.7.0rc0/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/arrow_local.py` & `sarus-0.7.0rc0/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/arrow_remote.py` & `sarus-0.7.0rc0/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/base_remote.py` & `sarus-0.7.0rc0/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/cache_scalar_local.py` & `sarus-0.7.0rc0/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/dataspec_api.py` & `sarus-0.7.0rc0/sarus/manager/dataspec_api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/ops/api.py` & `sarus-0.7.0rc0/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/parquet_local.py` & `sarus-0.7.0rc0/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/sdk_manager.py` & `sarus-0.7.0rc0/sarus/manager/sdk_manager.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/typing.py` & `sarus-0.7.0rc0/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/value_local.py` & `sarus-0.7.0rc0/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/manager/value_remote.py` & `sarus-0.7.0rc0/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/numpy/scalars.py` & `sarus-0.7.0rc0/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/pandas/core.py` & `sarus-0.7.0rc0/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/pandas/dataframe.py` & `sarus-0.7.0rc0/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sarus.py` & `sarus-0.7.0rc0/sarus/sarus.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,21 +40,19 @@
 import typing as t
 import warnings
 import webbrowser
 from dataclasses import dataclass
 from io import BytesIO
 from typing import Any, Dict, List, Optional
 
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 import sarus_data_spec
-from PIL import Image
 from requests import Session
 from sarus_data_spec.attribute import attach_properties
 
 import sarus.typing as srt
 from sarus.dataspec_wrapper import DataSpecWrapper
 from sarus.manager.dataspec_api import (
     compile_dataspec,
@@ -65,15 +63,15 @@
 from sarus.manager.typing import SDKManager
 from sarus.pandas.dataframe import DataFrame
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import sarus_data_spec.protobuf as sp
     import sarus_data_spec.typing as st
-    from sarus_data_spec.constants import BIG_DATA_TASK, SCHEMA_TASK
+    from sarus_data_spec.constants import SCHEMA_TASK
     from sarus_data_spec.context import push_global_context
     from sarus_data_spec.dataspec_rewriter.simple_rules import attach_variant
     from sarus_data_spec.dataspec_validator.privacy_limit import (
         DeltaEpsilonLimit,
     )
     from sarus_data_spec.protobuf.utilities import dict_deserialize
     from sarus_data_spec.transform import extract, select_sql
@@ -154,30 +152,27 @@
     Args:
         id: The dataset id.
         client: The Sarus client where the dataset is defined.
         type_metadata: A serialized json holding the dataset metadata.
         marginals: A serialized json holding the dataset marginals.
         human_description: A short human readable description.
         policy:
-        transforms:
-            A list of transformations to be applied to the original dataset.
     """
 
     def __init__(
         self,
         id: int,
         client: "Client",
         dataspec: st.DataSpec,
         is_bigdata: Optional[bool] = None,
         type_metadata: Optional[str] = None,
         human_description: Optional[str] = None,
         marginals: Optional[str] = None,
         policy: Optional[dict] = None,
         synthetic: Dict[str, Synthetic] = None,
-        transforms: List = [],
     ):
         self.client: "Client" = client
         self._set_dataspec(dataspec)
         name = dataspec.properties().get("slugname")
         attach_properties(
             dataspec,
             name=srt.ATTRIBUTES_DS,
@@ -197,21 +192,14 @@
             self._synthetic = synthetic
         self.marginals: Optional[Dict[str, Any]] = None
         if marginals is not None:
             self.marginals = json.loads(marginals)
 
         self.policy: Optional[dict] = policy
 
-        # We set `unbatch` as the default first transform
-        # for a better user experience.
-        # TODO remove the default batching on the API side
-        if len(transforms) == 0:
-            transforms.append(("unbatch", {}))
-        self.transforms = transforms
-
     @classmethod
     def _from_dict(cls, admin_ds: dict, client: Client) -> Dataset:
         """Get a dataset from the json data sent by the server.
 
         Deserializes the protobufs contained in the response and registers them
         in the storage.
 
@@ -291,107 +279,14 @@
             dataspec=dataspec,
             client=client,
             type_metadata=admin_ds.get("type_metadata"),
             marginals=admin_ds.get("marginals"),
             human_description=admin_ds.get("human_description"),
         )
 
-    def _split(
-        self, split: t.Union[str, List[str]]
-    ) -> t.Union[Dataset, List[Dataset]]:
-        """Get subsets of the Sarus dataset.
-
-        The `split` parameter is a string that specifies a slice of the dataset
-        to select. The format is inspired by the format used by Tensorflow
-        datasets slices.
-
-        A slice consist of a `start` and an `end` separated by a semi-colon
-        wrapped in square brackets. The `start` and `end` are integers,
-        optionally followed by a percent sign. If the percent sign is omitted,
-        the number indicates a row number. If the percent sign is present, the
-        number indicates a proportion of a the dataset to select, the number of
-        rows is rounded to the closest lower integer.
-
-        Similar to python slices, an empty `start` value is considered to be the
-        first row and an empty `end` value is considered to be the last row.
-
-
-        >>> sarus_ds.split("[10:40]")  # select rows 10 to 39
-        >>> sarus_ds.split("[10:70%]")  # select the first 70% rows but skip the first 10 rows
-        >>> sarus_ds.split("[:-100]")  # select all but the last 100 rows
-
-        Args:
-            split (str): specifies the portion of the dataset to select.
-
-        Returns:
-            Dataset: The selected split as a `Sarus Dataset`.
-
-        """
-        split_list = [split] if isinstance(split, str) else split
-        split_pattern = r"^\[(?P<start>|-?\d+%?):(?P<end>|-?\d+%?)\]$"
-        split_re = re.compile(split_pattern)
-
-        out_datasets = []
-        for spl in split_list:
-            match = split_re.match(spl)
-            if match is None:
-                raise ValueError(
-                    f"Could not match the split pattern {spl}. "
-                    "Expected pattern is `[start(%):end(%)]`."
-                )
-
-            # Get start and end rows
-            start_str, end_str = match.group("start"), match.group("end")
-            if self.marginals is None:
-                raise ValueError("Cannot split dataset as marginals is None.")
-            ds_size = int(self.marginals["rows"])
-            if start_str == "":
-                start = 0
-            else:
-                num = (
-                    int(start_str[:-1]) * ds_size // 100
-                    if start_str.endswith("%")
-                    else int(start_str)
-                )
-                start = ds_size + num if num < 0 else num
-
-            if end_str == "":
-                end = ds_size
-            else:
-                num = (
-                    int(end_str[:-1]) * ds_size // 100
-                    if end_str.endswith("%")
-                    else int(end_str)
-                )
-                end = ds_size + num if num < 0 else num
-
-            # Check consistency
-            if start >= end:
-                raise ValueError(
-                    f"Start ({start}) is greater that end ({end}) "
-                    f"in split {spl}"
-                )
-            if start < 0:
-                raise ValueError(
-                    f"Start ({start}) is lower that 0 " f"in split {spl}"
-                )
-            if end > ds_size:
-                raise ValueError(
-                    f"End ({end}) is greater that the dataset size ({ds_size}) "
-                    f"in split {spl}"
-                )
-
-            split_transform = ("split", {"start": start, "end": end})
-            out_datasets.append(self._add_transform(split_transform))
-
-        if isinstance(split, str):
-            return out_datasets[0]
-        else:
-            return out_datasets
-
     @property
     def features(self) -> Optional[Dict[str, Dict]]:
         """Features of the Sarus dataset and associated metadata.
 
         Returns:
             Dict[str, Dict]: A dictionary holding metadata where each key
             is a table name and each value is a dict with features.
@@ -683,68 +578,14 @@
 
             synthetic_table = pq.ParquetFile(io.BytesIO(resp.content)).read()
             self._synthetic[synthetic_type].data = synthetic_table
             self._synthetic[synthetic_type].rows = rows_number
 
         return self._synthetic[synthetic_type].data.slice(length=rows_number)
 
-    def _synthetic_as_pd_dataframe(
-        self,
-        rows_number: Optional[int] = None,
-        force_refresh: bool = False,
-        original: bool = True,
-        table_name: Optional[str] = None,
-    ):
-        """Return synthetic data as a pandas.DataFrame.
-
-         Args:
-            rows_number (int, optional): number of rows to return
-            force_refresh (bool): if True, always fetch from server
-            original (bool): if False, get categorical values as integers
-
-        Returns:
-            pandas.DataFrame: synthetic data
-        """
-        if table_name is None and len(self.type_metadata) > 1:
-            raise ValueError("Table name needs to be specified in this case.")
-
-        synthetic_data = self._fetch_synthetic(
-            rows_number=rows_number,
-            force_refresh=force_refresh,
-            original=original,
-        )
-
-        synthetic_df = synthetic_data.to_pandas()
-
-        # Convert images encoded as bytes to 3d arrays
-        if table_name is None:
-            features = self.features
-        else:
-            features = self.features[table_name]
-
-        for feature in features:
-            dtype = list(feature["type"].keys())[0]
-            if dtype == "image":
-                synthetic_df[feature["name"]] = synthetic_df[
-                    feature["name"]
-                ].map(Dataset.decode_image)
-        # replace min values = -9e+18 by pd.NA and change the data types
-        for column in synthetic_df.columns:
-            if synthetic_df[column].dtype in [
-                np.dtype("int64"),
-                np.dtype("int32"),
-                np.dtype("int16"),
-            ]:
-                synthetic_df[column] = synthetic_df[column].astype("Int64")
-                synthetic_df.loc[
-                    synthetic_df[column] <= np.iinfo(np.int64).min, column
-                ] = pd.NA
-
-        return synthetic_df
-
     @staticmethod
     def _sarus_features_to_tf_spec(
         features: Dict[str, Any],
         original: bool,
     ) -> Dict[str, tf.TensorSpec]:
         """Convert Sarus features to Tensorflow spec."""
         mapping = {
@@ -771,20 +612,14 @@
             return tf.TensorSpec(dtype=dtype, shape=shape)
 
         return {
             feature["name"]: get_tensorspec(feature) for feature in features
         }
 
     @staticmethod
-    def decode_image(serialized_image: bytes) -> np.ndarray:
-        # Need to be careful when decoding images with PIL while encoding with
-        # OpenCV. See https://stackoverflow.com/questions/58861577/differences-between-pil-image-open-and-cv2-imdecode
-        return np.load(BytesIO(serialized_image))
-
-    @staticmethod
     def _adapt_for_tf(
         batch: Dict[str, Any],
         features: Dict[str, Any],
         original: bool,
     ) -> Dict[str, Any]:
         """Convert python data to tensorflow compatible data.
 
@@ -897,206 +732,14 @@
 
         tf_signature = Dataset._sarus_features_to_tf_spec(features, original)
 
         return tf.data.Dataset.from_generator(
             generator, output_signature=tf_signature
         )
 
-    def _plot_marginal_feature(
-        self,
-        marginal_feature: Dict[str, Any],
-        width: float = 1.5,
-        heigth: float = 1.5,
-    ) -> Optional[str]:
-        if "statistics" not in marginal_feature:
-            return None
-
-        # text-based representations
-        # count for categories
-        distrib = marginal_feature["statistics"].get("distribution")
-        if distrib:
-            html_response = ""
-            distrib_s = sorted(distrib, key=lambda x: -x["probability"])
-            if len(distrib_s) > 5:
-                others_count = len(distrib_s) - 5
-                others_sum = sum([x["probability"] for x in distrib_s[5:]])
-                distrib_s = distrib_s[0:5]
-                distrib_s.append(
-                    {
-                        "name": f"Other ({others_count})",
-                        "probability": others_sum,
-                        "class_other": "True",
-                    }
-                )
-            for item in distrib_s:
-                html_response += "<div><div class='category "
-                if "class_other" in item:
-                    html_response += "other"
-                html_response += f"''>\
-                    {item['name']}\
-                  </div>\
-                  <div class='number'> {round(100*item['probability'],2)}%\
-                  </div>\
-                 </div>"
-            return html_response
-
-        # Graph-based representation
-        _ = plt.figure(figsize=(width, heigth))
-        # cumulDistribution for real
-        cumul = marginal_feature["statistics"].get("cumulativeDistribution")
-        if cumul:
-            try:
-                plt.fill_between(
-                    [vp["value"] for vp in cumul],
-                    [vp["probability"] for vp in cumul],
-                )
-            except Exception:
-                pass
-        fi = io.BytesIO()
-        plt.tight_layout()
-        plt.savefig(fi, format="svg")
-        plt.clf()
-        svg_dta = fi.getvalue()  # this is svg data
-        return svg_dta.decode()
-
-    def _marginals_to_html(self, display_type: bool = False) -> str:
-        """Return a HTML representation of this dataset.
-
-        To be displayedin a Notebook for example.
-        We'd like to render something like: https://www.kaggle.com/fmejia21/
-        demographics-of-academy-awards-oscars-winners
-
-        Args:
-            display_type (bool): if True, display each column type in the html
-
-        Returns:
-            str: HTML representation of the dataset
-        """
-        css = """<style>
-        @import url('https://rsms.me/inter/inter.css');
-        @supports (font-variation-settings: normal) {
-            html {font-family: 'Inter var', sans-serif; }
-            table {font-size: 12px; border-collapse: collapse;}
-            td, th {
-                border: 1px solid rgb(222, 223, 224);
-                font-weight: 500;
-                color: rgba(0,0,0,0.7);
-                padding: 8px;
-                vertical-align:top;
-                }
-            tr.desc>td>div {
-                display: flex; width: 140px;
-                flex-wrap: wrap;
-                justify-content: space-between;
-            }
-            tr.desc>td {
-                border-bottom-width: 4px;
-                }
-            div.category {
-                width: 70px;
-                padding: 4px;
-                margin-bottom: 4px;
-                color: black;
-                }
-            div.number {
-                padding: 4px;
-                margin-bottom: 4px;
-                color: rgb(0, 138, 188);
-                text-align: right;
-            }
-            td>div:hover {
-                background-color: rgba(0,0,0,0.03);
-              }
-            tr.synthetic {
-                font-family: 'Roboto Mono', Monaco, Consolas, monospace;
-              }
-            tr.synthetic>td {
-                padding: 8px 4px;
-                color: rgba(0, 0, 0, 0.7);
-              }
-            div.other {color: rgba(0, 0, 0, 0.4);!important}
-         </style>"""
-
-        table = "<table>\
-                <thead><tr>\n"
-        if self.type_metadata is None:
-            raise ValueError(
-                "The dataset has no type_metadata, may be pending..."
-            )
-        try:
-            columns = self.type_metadata["features"]
-        except Exception:
-            raise Exception(
-                "Dataset does not have proper typing yet. Maybe pending..."
-            )
-        for c in columns:
-            table += f"<th>{c['name']}</th>\n"
-
-        table += """</thead></tr>
-                <tbody>
-                <tr class='desc'>"""
-        if self.marginals is None:
-            raise ValueError(
-                "The dataset has no marginals yet, may be pending..."
-            )
-        try:
-            for c in self.marginals["features"]:
-                table += f"<td>{self._plot_marginal_feature(c)}</td>\n"
-        except Exception:
-            raise Exception(
-                "Dataset does not have proper marginals yet. Maybe pending..."
-            )
-        table += "</tr><tr>"
-        if display_type:
-            for c in columns:
-                table += f"<td>{c['type']}</td>\n"
-
-        table += "</tr></tbody></table>"
-
-        return f"<html>{css}<body>\n \
-                   {table}\
-                 </body></html>"
-
-    def to_html(
-        self, rows_number: int = None, force_refresh: bool = False
-    ) -> str:
-        """Return synthetic data as html.
-
-        Args:
-            rows_number (int): number of rows to display
-
-            force_refresh (bool): if True, does not use cached synthetic data
-
-        Returns:
-            str: HTML representation of the synthetic data
-        """
-        synthetic: pd.DataFrame = self._synthetic_as_pd_dataframe(
-            rows_number=rows_number, force_refresh=force_refresh
-        )
-        image_cols = [
-            f["name"]
-            for f in self.type_metadata["features"]
-            if "image" in f["type"]
-        ]
-
-        def _image_formatter(img_array):
-            img_array = np.squeeze(img_array)
-            image_from_array = Image.fromarray(img_array)
-            buffered = BytesIO()
-            image_from_array.save(buffered, format="png")
-            return (
-                f'<img src="data:image/png;base64,'
-                f'{base64.b64encode(buffered.getvalue()).decode()}">'
-            )
-
-        return synthetic.to_html(
-            formatters={c: _image_formatter for c in image_cols},
-            escape=False,
-        )
-
 
 class Client:
     """Entry point for the Sarus API client."""
 
     def _url_validator(self, url):
         """URL validator.
 
@@ -1243,15 +886,15 @@
             f"redirected automatically, you can visit {oidc_login_url}\n"
         )
         self.session().cookies.set(
             "session", base64.b64decode(token).decode("ascii")
         )
         # just to check that the login is successful
         try:
-            self._available_datasets()
+            self.list_datasets()
         except Exception:
             raise Exception("Error during login: incorrect token")
 
     def _credentials_login(self, email=None, password=None):
         if email is None:
             raise ValueError("Please enter your email")
 
@@ -1273,24 +916,14 @@
 
         if response.status_code == 401:
             raise ValueError("Error during login: incorrect credentials")
 
         # Let `requests` handle unexpected HTTP status codes.
         response.raise_for_status()
 
-    def _available_datasets(self) -> List[str]:
-        """List available datasets.
-
-        Returns:
-            List[str]: list of available dataset names.
-        """
-        request = self.session().get(f"{self.base_url}/datasets")
-        raise_response(request)
-        return [ds["name"] for ds in request.json()]
-
     def list_datasets(self) -> DatasetList:
         """List available Sarus datasets.
 
         Returns:
             DatasetList: List of available Sarus datasets.
         """
         request = self.session().get(f"{self.base_url}/datasets")
@@ -1332,16 +965,15 @@
             id (int): id of the dataset to be fetched
 
         Returns:
             an instance of Dataset
         """
         request = self.session().get(f"{self.base_url}/datasets/{id}")
         raise_response(request)
-        dataset = Dataset._from_dict(request.json(), self)
-        return dataset
+        return Dataset._from_dict(request.json(), self)
 
     def _fetch_dataset_by_name(self, name: str) -> Dataset:
         """Fetch a dataset from the Sarus Gateway.
 
         Args:
             name (string): name of the dataset to be fetched
```

### Comparing `sarus-0.6.7rc1/sarus/scripts/generate_op_list.py` & `sarus-0.7.0rc0/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/__init__.py` & `sarus-0.7.0rc0/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/cluster.py` & `sarus-0.7.0rc0/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/compose.py` & `sarus-0.7.0rc0/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/decomposition.py` & `sarus-0.7.0rc0/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/ensemble.py` & `sarus-0.7.0rc0/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/impute.py` & `sarus-0.7.0rc0/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/linear_model.py` & `sarus-0.7.0rc0/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/model_selection.py` & `sarus-0.7.0rc0/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/pipeline.py` & `sarus-0.7.0rc0/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/preprocessing.py` & `sarus-0.7.0rc0/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/sklearn/svm.py` & `sarus-0.7.0rc0/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/skopt/searchcv.py` & `sarus-0.7.0rc0/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/std/types.py` & `sarus-0.7.0rc0/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/typing.py` & `sarus-0.7.0rc0/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/utils.py` & `sarus-0.7.0rc0/sarus/utils.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/wrapper_factory.py` & `sarus-0.7.0rc0/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus/xgboost/xgboost.py` & `sarus-0.7.0rc0/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.7rc1/sarus.egg-info/PKG-INFO` & `sarus-0.7.0rc0/sarus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.7rc1
+Version: 0.7.0rc0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.7rc1/sarus.egg-info/SOURCES.txt` & `sarus-0.7.0rc0/sarus.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 sarus/context/local_sdk.py
 sarus/context/typing.py
 sarus/imblearn/__init__.py
 sarus/imblearn/over_sampling.py
 sarus/imblearn/pipeline.py
 sarus/imblearn/under_sampling.py
 sarus/legacy/__init__.py
-sarus/legacy/pandas/__init__.py
-sarus/legacy/pandas/dataframe.py
 sarus/legacy/tensorflow/__init__.py
 sarus/legacy/tensorflow/dataset.py
 sarus/legacy/tensorflow/model.py
 sarus/manager/__init__.py
 sarus/manager/arrow_local.py
 sarus/manager/arrow_remote.py
 sarus/manager/base_remote.py
@@ -69,13 +67,11 @@
 sarus/sklearn/pipeline.py
 sarus/sklearn/preprocessing.py
 sarus/sklearn/svm.py
 sarus/skopt/__init__.py
 sarus/skopt/searchcv.py
 sarus/std/__init__.py
 sarus/std/types.py
-sarus/storage/__init__.py
-sarus/storage/legacy_local.py
 sarus/tensorflow/__init__.py
 sarus/xgboost/__init__.py
 sarus/xgboost/xgboost.py
 tests/test_sanity.py
```

### Comparing `sarus-0.6.7rc1/setup.cfg` & `sarus-0.7.0rc0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
 	sarus-data-spec-public==3.3.0
-	matplotlib>=3.1
 	cloudpickle>=1.2, <2.1
 	pyarrow >= 11.0
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.2.2
 	scipy==1.9.0
```

