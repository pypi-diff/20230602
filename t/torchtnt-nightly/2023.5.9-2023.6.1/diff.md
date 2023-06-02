# Comparing `tmp/torchtnt-nightly-2023.5.9.tar.gz` & `tmp/torchtnt-nightly-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchtnt-nightly-2023.5.9.tar", last modified: Tue May  9 11:22:31 2023, max compression
+gzip compressed data, was "dist/torchtnt-nightly-2023.6.1.tar", last modified: Thu Jun  1 11:23:50 2023, max compression
```

## Comparing `torchtnt-nightly-2023.5.9.tar` & `torchtnt-nightly-2023.6.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28872 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-09 11:21:06.000000 torchtnt-nightly-2023.5.9/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:22:31.000000 torchtnt-nightly-2023.5.9/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30358 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-01 11:21:44.000000 torchtnt-nightly-2023.6.1/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:23:50.000000 torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt-nightly-2023.5.9/LICENSE` & `torchtnt-nightly-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/PKG-INFO` & `torchtnt-nightly-2023.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.5.9
+Version: 2023.6.1
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.5.9 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.6.1 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.5.9/README.md` & `torchtnt-nightly-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/setup.py` & `torchtnt-nightly-2023.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/__init__.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 # LICENSE file in the root directory of this source tree.
 
 from .auto_unit import AutoUnit
 from .callback import Callback
 from .evaluate import evaluate, init_eval_state
 from .fit import fit, init_fit_state
 from .predict import init_predict_state, predict
-from .progress import Progress
 from .state import PhaseState, State
 from .train import init_train_state, train
 from .unit import EvalUnit, PredictUnit, TEvalUnit, TPredictUnit, TrainUnit, TTrainUnit
 
 __all__ = [
     "AutoUnit",
     "Callback",
     "evaluate",
     "init_eval_state",
     "fit",
     "init_fit_state",
     "init_predict_state",
     "predict",
-    "Progress",
     "PhaseState",
     "State",
     "init_train_state",
     "train",
     "EvalUnit",
     "PredictUnit",
     "TEvalUnit",
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/_test_utils.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/auto_unit.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/auto_unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,22 @@
     BackwardPrefetch,
     CPUOffload,
     MixedPrecision,
     ShardingStrategy,
 )
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim.swa_utils import AveragedModel, SWALR
-from torch.profiler import record_function
 from torchtnt.framework.state import ActivePhase, State
 from torchtnt.framework.unit import EvalUnit, PredictUnit, TrainUnit
-from torchtnt.framework.utils import _is_fsdp_module, get_current_progress, StatefulInt
+from torchtnt.framework.utils import (
+    _get_timing_context,
+    _is_fsdp_module,
+    get_current_progress,
+    StatefulInt,
+)
 from torchtnt.utils import (
     init_from_env,
     is_torch_version_geq_1_12,
     TLRScheduler,
     transfer_batch_norm_stats,
     transfer_weights,
 )
@@ -87,14 +91,15 @@
     cpu_offload: Optional[CPUOffload] = None
     auto_wrap_policy: Optional[Callable[[torch.nn.Module, bool, int], bool]] = None
     backward_prefetch: Optional[BackwardPrefetch] = None
     ignored_modules: Optional[Iterable[torch.nn.Module]] = None
     sync_module_states: bool = False
     forward_prefetch: bool = False
     limit_all_gathers: bool = False
+    use_orig_params: bool = False
 
 
 @dataclass
 class SWAParams:
     """
     Dataclass to store parameters for stochastic weight averaging.
 
@@ -231,16 +236,14 @@
         clip_grad_value: Optional[float] = None,
         swa_params: Optional[SWAParams] = None,
         torchdynamo_params: Optional[TorchDynamoParams] = None,
         training: bool = True,
     ) -> None:
         super().__init__()
         self.device: torch.device = device or init_from_env()
-        module = module.to(self.device)  # move module to device
-
         self.precision: Optional[torch.dtype]
         if isinstance(precision, str):
             self.precision = _convert_precision_str_to_dtype(precision)
         else:
             self.precision = precision
 
         if strategy:
@@ -252,14 +255,15 @@
                 device_ids = None
                 if self.device.type == "cuda":
                     device_ids = [self.device.index]
                 params_dict = asdict(strategy)
                 # remove ddp comm hook variables from params dict
                 del params_dict["comm_state"]
                 del params_dict["comm_hook"]
+                module = module.to(self.device)
                 module = DDP(module, device_ids=device_ids, **params_dict)
                 if torchdynamo_params:
                     # TODO: Add support for dynamo and DDP
                     rank_zero_warn(
                         "Torchdynamo params has been set with DDP - Note that performance will likely be slower and we recommend using only one."
                     )
                 if strategy.comm_hook:
@@ -286,14 +290,16 @@
                 # wrap module in FSDP
                 module = FSDP(
                     module,
                     device_id=self.device,
                     mixed_precision=mixed_precision,
                     **asdict(strategy),
                 )
+        else:
+            module = module.to(self.device)
 
         self.module: torch.nn.Module = module
 
         self.step_lr_interval = step_lr_interval
 
         self.grad_scaler: Optional[GradScaler] = None
         if self.precision:
@@ -371,75 +377,85 @@
             data: a batch of data which is passed from the ``train_step``/``eval_step``
 
         Returns:
             Tuple containing the loss and the output of the model
         """
         ...
 
-    def move_data_to_device(self, state: State, data: TData) -> TData:
+    def move_data_to_device(
+        self, state: State, data: TData, non_blocking: bool
+    ) -> TData:
         """
         The user can override this method with custom code to copy data to device. This will be called at the start of every ``train_step``/``eval_step``/``predict_step``.
         By default this uses the utility function :py:func:`~torchtnt.utils.copy_data_to_device`.
 
         If on GPU, this method will be called on a separate CUDA stream.
 
         Args:
             state: a State object which is passed from the ``train_step``/``eval_step``/``predict_step``
             data: a batch of data which is passed from the ``train_step``/``eval_step``/``predict_step``
+            non_blocking: parameter to pass to ``torch.tensor.to``
 
         Returns:
             A batch of data which is on the device
         """
-        non_blocking = (
-            True
-            if state.active_phase == ActivePhase.TRAIN
-            and self.device.type == "cuda"
-            and self._prefetched
-            else False
-        )
         return copy_data_to_device(data, self.device, non_blocking=non_blocking)
 
     def prefetch_next_batch(self, state: State, data_iter: Iterator[TData]) -> None:
         """Prefetch the next batch on a separate CUDA stream."""
         try:
-            with record_function(__name__ + ".next(data_iter)"):
+            with _get_timing_context(
+                state, f"{self.__class__.__name__}.next(data_iter)"
+            ):
                 next_batch = next(data_iter)
         except StopIteration:
             self._next_batch = None
             self._is_last_train_batch = True
             return
 
+        non_blocking = (
+            True
+            if state.active_phase == ActivePhase.TRAIN
+            and self.device.type == "cuda"
+            and self._prefetched
+            else False
+        )
+
         # if on cpu, self._prefetch_stream is None so the torch.cuda.stream call is a no-op
-        with torch.cuda.stream(self._prefetch_stream), record_function(
-            __name__ + ".move_data_to_device"
+        with torch.cuda.stream(self._prefetch_stream), _get_timing_context(
+            state, f"{self.__class__.__name__}.move_data_to_device"
         ):
-            self._next_batch = self.move_data_to_device(state, next_batch)
+            self._next_batch = self.move_data_to_device(
+                state, next_batch, non_blocking=non_blocking
+            )
 
     def train_step(
         self, state: State, data: Iterator[TData]
     ) -> Tuple[torch.Tensor, Any]:
         train_state = none_throws(state.train_state)
         if not self._prefetched:
             self.prefetch_next_batch(state, data)
             self._prefetched = True
 
         if self._prefetch_stream:
-            with record_function(__name__ + ".wait_stream"):
+            with _get_timing_context(state, f"{self.__class__.__name__}.wait_stream"):
                 # wait on the CUDA stream to complete the host to device copy
                 torch.cuda.current_stream().wait_stream(self._prefetch_stream)
 
         # get the next batch which was stored by prefetch_next_batch
         batch = self._next_batch
         if not batch:
             self._prefetched = False
             self._is_last_train_batch = False
             raise StopIteration
 
         if self._prefetch_stream:
-            with record_function(__name__ + ".record_data_in_stream"):
+            with _get_timing_context(
+                state, f"{self.__class__.__name__}.record_data_in_stream"
+            ):
                 # record the batch in the current stream
                 record_data_in_stream(batch, torch.cuda.current_stream())
 
         # prefetch the next batch
         self.prefetch_next_batch(state, data)
 
         should_update_weights = (
@@ -450,15 +466,16 @@
 
         if should_update_weights:
             # TODO try to use dynamo here
             self._run_optimizer_lr_scheduler_step(state)
 
         step = get_current_progress(state).num_steps_completed
         # users can override this, by default this is a no-op
-        self.on_train_step_end(state, batch, step, loss, outputs)
+        with _get_timing_context(state, f"{self.__class__.__name__}.on_train_step_end"):
+            self.on_train_step_end(state, batch, step, loss, outputs)
         return loss, outputs
 
     def _forward_and_backward(
         self, state: State, data: TData, should_update_weights: bool
     ) -> Tuple[torch.Tensor, Any]:
         # if using gradient accumulation with either DDP or FSDP, when in a step where we will not update the weights,
         # run forward and backward in no_sync context
@@ -477,27 +494,31 @@
         maybe_detect_anomaly = (
             torch.autograd.set_detect_anomaly(detect_anomaly)
             if detect_anomaly is not None
             else contextlib.nullcontext()
         )
         with maybe_no_sync, maybe_detect_anomaly:
             with self.maybe_autocast_precision:
-                with record_function(__name__ + ".compute_loss"):
+                with _get_timing_context(
+                    state, f"{self.__class__.__name__}.compute_loss"
+                ):
                     # users must override this
                     loss, outputs = self.compute_loss(state, data)
 
             # normalize loss to account for gradient accumulation
             loss = loss / self.gradient_accumulation_steps
 
-            grad_scaler = self.grad_scaler
-            with record_function(__name__ + ".backward"):
-                if grad_scaler:
-                    grad_scaler.scale(loss).backward()
-                else:
+            if self.grad_scaler:
+                scaled_loss = self.grad_scaler.scale(loss)
+                with _get_timing_context(state, f"{self.__class__.__name__}.backward"):
+                    scaled_loss.backward()
+            else:
+                with _get_timing_context(state, f"{self.__class__.__name__}.backward"):
                     loss.backward()
+
         return loss, outputs
 
     def _run_optimizer_lr_scheduler_step(self, state: State) -> None:
         """Runs the optimizer step, sets gradients to zero, and runs lr scheduler step."""
         # optimizer step
         grad_scaler = self.grad_scaler
         clip_grad_norm = self.clip_grad_norm
@@ -523,15 +544,15 @@
         # gradient value clipping
         if clip_grad_value:
             torch.nn.utils.clip_grad_value_(
                 parameters=self.module.parameters(),
                 clip_value=clip_grad_value,
             )
 
-        with record_function(__name__ + ".optimizer_step"):
+        with _get_timing_context(state, f"{self.__class__.__name__}.optimizer_step"):
             if grad_scaler:
                 grad_scaler.step(self.optimizer)
                 # update the scale for next iteration
                 grad_scaler.update()
             else:
                 self.optimizer.step()
 
@@ -544,15 +565,17 @@
         train_state = none_throws(state.train_state)
         if (
             self.swa_params is None
             or train_state.progress.num_epochs_completed < self.swa_params.epoch_start
         ):
             lr_scheduler = self.lr_scheduler
             if lr_scheduler and self.step_lr_interval == "step":
-                with record_function(__name__ + ".lr_scheduler_step"):
+                with _get_timing_context(
+                    state, f"{self.__class__.__name__}.lr_scheduler_step"
+                ):
                     lr_scheduler.step()
 
     def on_train_step_end(
         self, state: State, data: TData, step: int, loss: torch.Tensor, outputs: Any
     ) -> None:
         """
         This will be called at the end of every ``train_step`` before returning. The user can implement this method with code to update and log their metrics,
@@ -578,36 +601,43 @@
             and self.swa_params
             and train_state.progress.num_epochs_completed >= self.swa_params.epoch_start
         ):
             self.swa_model.update_parameters(self.module)
             none_throws(self.swa_scheduler).step()
         elif self.lr_scheduler and self.step_lr_interval == "epoch":
             # optionally step lr scheduler
-            with record_function(__name__ + ".lr_scheduler_step"):
+            with _get_timing_context(
+                state, f"{self.__class__.__name__}.lr_scheduler_step"
+            ):
                 self.lr_scheduler.step()
 
     def on_train_end(self, state: State) -> None:
         """
         Note that if using SWA and implementing `on_train_end()`, must call `super().on_train_end()`.
         """
         swa_model = self.swa_model
         if swa_model:
             transfer_weights(swa_model, self.module)
             transfer_batch_norm_stats(swa_model, self.module)
 
     def eval_step(self, state: State, data: TData) -> Tuple[torch.Tensor, Any]:
-        data = self.move_data_to_device(state, data)
+        with _get_timing_context(
+            state, f"{self.__class__.__name__}.move_data_to_device"
+        ):
+            data = self.move_data_to_device(state, data, non_blocking=False)
 
         with self.maybe_autocast_precision:
             # users must override this
-            loss, outputs = self.compute_loss(state, data)
+            with _get_timing_context(state, f"{self.__class__.__name__}.compute_loss"):
+                loss, outputs = self.compute_loss(state, data)
 
         step = get_current_progress(state).num_steps_completed
         # users can override this, by default this is a no-op
-        self.on_eval_step_end(state, data, step, loss, outputs)
+        with _get_timing_context(state, f"{self.__class__.__name__}.on_eval_step_end"):
+            self.on_eval_step_end(state, data, step, loss, outputs)
         return loss, outputs
 
     def on_eval_step_end(
         self, state: State, data: TData, step: int, loss: torch.Tensor, outputs: Any
     ) -> None:
         """
         This will be called at the end of every ``eval_step`` before returning. The user can implement this method with code to update and log their metrics,
@@ -619,22 +649,29 @@
             step: how many steps have been completed (``train_step``s when running fit and ``eval_step``s when running evaluation)
             loss: the loss computed in the ``compute_loss`` function
             outputs: the outputs of the model forward pass
         """
         pass
 
     def predict_step(self, state: State, data: Any) -> Any:
-        data = self.move_data_to_device(state, data)
+        with _get_timing_context(
+            state, f"{self.__class__.__name__}.move_data_to_device"
+        ):
+            data = self.move_data_to_device(state, data, non_blocking=False)
 
         with self.maybe_autocast_precision:
-            outputs = self.module(data)
+            with _get_timing_context(state, f"{self.__class__.__name__}.module(data)"):
+                outputs = self.module(data)
 
         step = get_current_progress(state).num_steps_completed
         # users can override this, by default this is a no-op
-        self.on_predict_step_end(state, data, step, outputs)
+        with _get_timing_context(
+            state, f"{self.__class__.__name__}.on_predict_step_end"
+        ):
+            self.on_predict_step_end(state, data, step, outputs)
         return outputs
 
     def on_predict_step_end(
         self, state: State, data: TData, step: int, outputs: Any
     ) -> None:
         """
         This will be called at the end of every ``predict_step`` before returning. The user can implement this method with code to update and log their metrics,
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callback.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/__init__.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files 7% similar despite different names*

```diff
@@ -144,14 +144,25 @@
         # save snapshot to predetermined path
         # TODO: discuss whether this path should be customized
         global_step = train_progress.num_steps_completed
         snapshot_path = _get_snapshot_save_path(self._dirpath, epoch, global_step)
         self._async_snapshot(snapshot_path, app_state, wait=True)
 
     def on_train_end(self, state: State, unit: TTrainUnit) -> None:
+        train_state = none_throws(state.train_state)
+        global_step = train_state.progress.num_steps_completed
+
+        app_state = _get_app_state(state, unit, self._replicated, intra_epoch=False)
+
+        # save snapshot to predetermined path
+        # TODO: discuss whether this path should be customized
+        epoch = train_state.progress.num_epochs_completed
+        snapshot_path = _get_snapshot_save_path(self._dirpath, epoch, global_step)
+        self._async_snapshot(snapshot_path, app_state, wait=False)
+
         self._wait()
 
     def on_exception(
         self,
         state: State,
         unit: Union[TTrainUnit, TEvalUnit, TPredictUnit],
         exc: BaseException,
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,63 +34,63 @@
 
     def on_train_epoch_start(self, state: State, unit: TTrainUnit) -> None:
         train_state = none_throws(state.train_state)
         self._train_progress_bar = _create_progress_bar(
             train_state.dataloader,
             desc="Train Epoch",
             num_epochs_completed=train_state.progress.num_epochs_completed,
-            num_steps_completed=train_state.progress.num_steps_completed,
+            num_steps_completed=train_state.progress.num_steps_completed_in_epoch,
             max_steps=train_state.max_steps,
             max_steps_per_epoch=train_state.max_steps_per_epoch,
         )
 
     def on_train_step_end(self, state: State, unit: TTrainUnit) -> None:
         train_state = none_throws(state.train_state)
         if self._train_progress_bar is not None:
             _update_progress_bar(
                 self._train_progress_bar,
-                train_state.progress.num_steps_completed,
+                train_state.progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_train_epoch_end(self, state: State, unit: TTrainUnit) -> None:
         train_state = none_throws(state.train_state)
         if self._train_progress_bar is not None:
             _close_progress_bar(
                 self._train_progress_bar,
-                train_state.progress.num_steps_completed,
+                train_state.progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_eval_epoch_start(self, state: State, unit: TEvalUnit) -> None:
         eval_state = none_throws(state.eval_state)
         self._eval_progress_bar = _create_progress_bar(
             eval_state.dataloader,
             desc="Eval Epoch",
             num_epochs_completed=eval_state.progress.num_epochs_completed,
-            num_steps_completed=eval_state.progress.num_steps_completed,
+            num_steps_completed=eval_state.progress.num_steps_completed_in_epoch,
             max_steps=eval_state.max_steps,
             max_steps_per_epoch=eval_state.max_steps_per_epoch,
         )
 
     def on_eval_step_end(self, state: State, unit: TEvalUnit) -> None:
         eval_state = none_throws(state.eval_state)
         if self._eval_progress_bar is not None:
             _update_progress_bar(
                 self._eval_progress_bar,
-                eval_state.progress.num_steps_completed,
+                eval_state.progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_eval_epoch_end(self, state: State, unit: TEvalUnit) -> None:
         eval_state = none_throws(state.eval_state)
         if self._eval_progress_bar is not None and state.eval_state:
             _close_progress_bar(
                 self._eval_progress_bar,
-                eval_state.progress.num_steps_completed,
+                eval_state.progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_predict_epoch_start(self, state: State, unit: TPredictUnit) -> None:
         predict_state = none_throws(state.predict_state)
         self._predict_progress_bar = _create_progress_bar(
             predict_state.dataloader,
@@ -102,24 +102,24 @@
         )
 
     def on_predict_step_end(self, state: State, unit: TPredictUnit) -> None:
         predict_state = none_throws(state.predict_state)
         if self._predict_progress_bar is not None:
             _update_progress_bar(
                 self._predict_progress_bar,
-                predict_state.progress.num_steps_completed,
+                predict_state.progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_predict_epoch_end(self, state: State, unit: TPredictUnit) -> None:
         predict_state = none_throws(state.predict_state)
         if self._predict_progress_bar is not None:
             _close_progress_bar(
                 self._predict_progress_bar,
-                predict_state.progress.num_steps_completed,
+                predict_state.progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
 
 def _create_progress_bar(
     # pyre-ignore: Invalid type parameters [24]
     dataloader: Iterable,
@@ -136,15 +136,20 @@
     current_epoch = num_epochs_completed
     total = _estimated_steps_in_epoch(
         dataloader,
         num_steps_completed=num_steps_completed,
         max_steps=max_steps,
         max_steps_per_epoch=max_steps_per_epoch,
     )
-    return tqdm(desc=f"{desc} {current_epoch}", total=total)
+    return tqdm(
+        desc=f"{desc} {current_epoch}",
+        total=total,
+        initial=num_steps_completed,
+        bar_format="{l_bar}{bar}{r_bar}\n",
+    )
 
 
 def _update_progress_bar(
     progress_bar: tqdm, num_steps_completed: int, refresh_rate: int
 ) -> None:
     if not get_global_rank() == 0:
         return
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/evaluate.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/evaluate.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import logging
 from typing import Iterable, List, Optional
 
 import torch
 from pyre_extensions import none_throws
+from torchtnt.framework import AutoUnit
 from torchtnt.framework.callback import Callback
 
 from torchtnt.framework.state import ActivePhase, EntryPoint, PhaseState, State
 from torchtnt.framework.unit import TEvalData, TEvalUnit
 from torchtnt.framework.utils import (
     _get_timing_context,
     _is_epoch_done,
@@ -144,49 +145,52 @@
     )
 
     # Set all modules to eval mode
     # access modules made available through _AppStateMixin
     tracked_modules = eval_unit.tracked_modules()
     prior_module_train_states = _set_module_training_mode(tracked_modules, False)
 
-    with _get_timing_context(
-        state, f"eval.{eval_unit.__class__.__name__}.on_eval_start"
-    ):
+    with _get_timing_context(state, f"{eval_unit.__class__.__name__}.on_eval_start"):
         eval_unit.on_eval_start(state)
     _run_callback_fn(callbacks, "on_eval_start", state, eval_unit)
 
     # Conditionally run this to avoid running this multiple times
     # in the case of resuming from a checkpoint mid-epoch
     if eval_state.progress.num_steps_completed_in_epoch == 0:
         with _get_timing_context(
-            state, f"eval.{eval_unit.__class__.__name__}.on_eval_epoch_start"
+            state, f"{eval_unit.__class__.__name__}.on_eval_epoch_start"
         ):
             eval_unit.on_eval_epoch_start(state)
         _run_callback_fn(callbacks, "on_eval_epoch_start", state, eval_unit)
 
-    data_iter = iter(eval_state.dataloader)
+    with _get_timing_context(state, "evaluate.iter(dataloader)"):
+        data_iter = iter(eval_state.dataloader)
     step_input = data_iter
 
     pass_data_iter_to_step = _step_requires_iterator(eval_unit.eval_step)
+    is_auto_unit = isinstance(eval_unit, AutoUnit)
     prev_steps_in_epoch = eval_state.progress.num_steps_completed_in_epoch
 
     while not (
         state.should_stop
         or _is_epoch_done(
             eval_state.progress, eval_state.max_steps_per_epoch, eval_state.max_steps
         )
     ):
         try:
             if not pass_data_iter_to_step:
                 # get the next batch from the data iterator
-                with _get_timing_context(state, "eval.data_iter_next"):
+                with _get_timing_context(state, "evaluate.next(data_iter)"):
                     step_input = next(data_iter)
             _run_callback_fn(callbacks, "on_eval_step_start", state, eval_unit)
             with _get_timing_context(
-                state, f"eval.{eval_unit.__class__.__name__}.eval_step"
+                state,
+                f"{eval_unit.__class__.__name__}.eval_step",
+                skip_timer=is_auto_unit,
+                # skip timer if eval_unit is a subclass of AutoUnit because we have additional timing in the AutoUnit and all timing should be mutually exclusive
             ):
                 eval_state._step_output = eval_unit.eval_step(state, step_input)
 
             eval_state.progress.increment_step()
             _run_callback_fn(
                 callbacks,
                 "on_eval_step_end",
@@ -205,20 +209,20 @@
     if not any_steps_completed:
         logger.warning("No steps completed during evaluate epoch!")
 
     # set progress counters for the next epoch
     eval_state.progress.increment_epoch()
 
     with _get_timing_context(
-        state, f"eval.{eval_unit.__class__.__name__}.on_eval_epoch_end"
+        state, f"{eval_unit.__class__.__name__}.on_eval_epoch_end"
     ):
         eval_unit.on_eval_epoch_end(state)
     _run_callback_fn(callbacks, "on_eval_epoch_end", state, eval_unit)
 
-    with _get_timing_context(state, f"eval.{eval_unit.__class__.__name__}.on_eval_end"):
+    with _get_timing_context(state, f"{eval_unit.__class__.__name__}.on_eval_end"):
         eval_unit.on_eval_end(state)
     _run_callback_fn(callbacks, "on_eval_end", state, eval_unit)
 
     # Reset training mode for modules at the end of the epoch
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     _reset_module_training_mode(tracked_modules, prior_module_train_states)
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/fit.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,20 +177,20 @@
         f"max_steps={train_state.max_steps} "
         f"max_train_steps_per_epoch={train_state.max_steps_per_epoch} "
         f"max_eval_steps_per_epoch={eval_state.max_steps_per_epoch} "
         f"evaluate_every_n_steps={eval_state.evaluate_every_n_steps} "
         f"evaluate_every_n_epochs={eval_state.evaluate_every_n_epochs} "
     )
 
-    with _get_timing_context(state, f"train.{unit.__class__.__name__}.on_train_start"):
+    with _get_timing_context(state, f"{unit.__class__.__name__}.on_train_start"):
         unit.on_train_start(state)
     _run_callback_fn(callbacks, "on_train_start", state, unit)
 
     while not (
         state.should_stop
         or _is_done(train_state.progress, train_state.max_epochs, train_state.max_steps)
     ):
         _train_epoch_impl(state, unit, callbacks)
 
-    with _get_timing_context(state, f"train.{unit.__class__.__name__}.on_train_end"):
+    with _get_timing_context(state, f"{unit.__class__.__name__}.on_train_end"):
         unit.on_train_end(state)
     _run_callback_fn(callbacks, "on_train_end", state, unit)
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/predict.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import logging
 from typing import Iterable, List, Optional
 
 import torch
 from pyre_extensions import none_throws
+from torchtnt.framework import AutoUnit
 from torchtnt.framework.callback import Callback
 
 from torchtnt.framework.state import ActivePhase, EntryPoint, PhaseState, State
 from torchtnt.framework.unit import TPredictData, TPredictUnit
 from torchtnt.framework.utils import (
     _get_timing_context,
     _is_epoch_done,
@@ -146,51 +147,56 @@
 
     # Set all modules to eval mode
     # access modules made available through _AppStateMixin
     tracked_modules = predict_unit.tracked_modules()
     prior_module_train_states = _set_module_training_mode(tracked_modules, False)
 
     with _get_timing_context(
-        state, f"predict.{predict_unit.__class__.__name__}.on_predict_start"
+        state, f"{predict_unit.__class__.__name__}.on_predict_start"
     ):
         predict_unit.on_predict_start(state)
     _run_callback_fn(callbacks, "on_predict_start", state, predict_unit)
 
     # Conditionally run this to avoid running this multiple times
     # in the case of resuming from a checkpoint mid-epoch
     if predict_state.progress.num_steps_completed_in_epoch == 0:
         with _get_timing_context(
-            state, f"predict.{predict_unit.__class__.__name__}.on_predict_epoch_start"
+            state, f"{predict_unit.__class__.__name__}.on_predict_epoch_start"
         ):
             predict_unit.on_predict_epoch_start(state)
         _run_callback_fn(callbacks, "on_predict_epoch_start", state, predict_unit)
 
-    data_iter = iter(predict_state.dataloader)
+    with _get_timing_context(state, "predict.iter(dataloader)"):
+        data_iter = iter(predict_state.dataloader)
     step_input = data_iter
 
     pass_data_iter_to_step = _step_requires_iterator(predict_unit.predict_step)
+    is_auto_unit = isinstance(predict_unit, AutoUnit)
     prev_steps_in_epoch = predict_state.progress.num_steps_completed_in_epoch
 
     while not (
         state.should_stop
         or _is_epoch_done(
             predict_state.progress,
             predict_state.max_steps_per_epoch,
             predict_state.max_steps,
         )
     ):
         try:
             if not pass_data_iter_to_step:
                 # get the next batch from the data iterator
-                with _get_timing_context(state, "predict.data_iter_next"):
+                with _get_timing_context(state, "predict.next(data_iter)"):
                     step_input = next(data_iter)
 
             _run_callback_fn(callbacks, "on_predict_step_start", state, predict_unit)
             with _get_timing_context(
-                state, f"predict.{predict_unit.__class__.__name__}.predict_step"
+                state,
+                f"{predict_unit.__class__.__name__}.predict_step",
+                skip_timer=is_auto_unit,
+                # skip timer if predict_unit is a subclass of AutoUnit because we have additional timing in the AutoUnit and all timing should be mutually exclusive
             ):
                 predict_state._step_output = predict_unit.predict_step(
                     state, step_input
                 )
             predict_state.progress.increment_step()
             _run_callback_fn(callbacks, "on_predict_step_end", state, predict_unit)
 
@@ -207,21 +213,21 @@
     if not any_steps_completed:
         logger.warning("No steps completed during predict epoch!")
 
     # set progress counters for the next epoch
     predict_state.progress.increment_epoch()
 
     with _get_timing_context(
-        state, f"predict.{predict_unit.__class__.__name__}.on_predict_epoch_end"
+        state, f"{predict_unit.__class__.__name__}.on_predict_epoch_end"
     ):
         predict_unit.on_predict_epoch_end(state)
     _run_callback_fn(callbacks, "on_predict_epoch_end", state, predict_unit)
 
     with _get_timing_context(
-        state, f"predict.{predict_unit.__class__.__name__}.on_predict_end"
+        state, f"{predict_unit.__class__.__name__}.on_predict_end"
     ):
         predict_unit.on_predict_end(state)
     _run_callback_fn(callbacks, "on_predict_end", state, predict_unit)
 
     # Reset training mode for modules at the end of the epoch
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/progress.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/progress.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 
     @property
     def num_steps_completed_in_epoch(self) -> int:
         """Number of steps completed thus far in epoch."""
         return self._num_steps_completed_in_epoch
 
     def increment_step(self) -> None:
-        """Method called by framework to increment the step count. Not intended to be called by user."""
+        """Increment the step counts completed and completed within the epoch."""
         self._num_steps_completed += 1
         self._num_steps_completed_in_epoch += 1
 
     def increment_epoch(self) -> None:
-        """Method called by framework to increment the epoch count. Not intended to be called by user."""
+        """Increment the epochs completed and resets the steps completed within the epoch."""
         self._num_epochs_completed += 1
         self._num_steps_completed_in_epoch = 0
 
     def state_dict(self) -> Dict[str, Any]:
         """Returns a state_dict of a Progress instance in accordance with Stateful protocol."""
         return {
             "num_epochs_completed": self._num_epochs_completed,
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/state.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # pyre-ignore-all-errors[3]
 # pyre-ignore-all-errors[4]
 
 import logging
 from enum import auto, Enum
 from typing import Any, Iterable, Optional
 
-from torchtnt.framework.progress import Progress
+from torchtnt.utils.progress import Progress
 from torchtnt.utils.timer import Timer
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _check_loop_condition(name: str, val: Optional[int]) -> None:
     if val is not None and val < 0:
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/train.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import logging
 from typing import Iterable, List, Optional
 
 import torch
 from pyre_extensions import none_throws
-from torch.profiler import record_function
+from torchtnt.framework import AutoUnit
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.evaluate import _evaluate_impl
 from torchtnt.framework.state import ActivePhase, EntryPoint, PhaseState, State
 from torchtnt.framework.unit import TTrainData, TTrainUnit
 from torchtnt.framework.utils import (
     _get_timing_context,
     _is_done,
@@ -154,29 +154,25 @@
     state._active_phase = ActivePhase.TRAIN
 
     # Set all modules to train() mode
     # access modules made available through _AppStateMixin
     tracked_modules = train_unit.tracked_modules()
     prior_module_train_states = _set_module_training_mode(tracked_modules, True)
 
-    with _get_timing_context(
-        state, f"train.{train_unit.__class__.__name__}.on_train_start"
-    ):
+    with _get_timing_context(state, f"{train_unit.__class__.__name__}.on_train_start"):
         train_unit.on_train_start(state)
     _run_callback_fn(callbacks, "on_train_start", state, train_unit)
 
     while not (
         state.should_stop
         or _is_done(train_state.progress, train_state.max_epochs, train_state.max_steps)
     ):
         _train_epoch_impl(state, train_unit, callbacks)
 
-    with _get_timing_context(
-        state, f"train.{train_unit.__class__.__name__}.on_train_end"
-    ):
+    with _get_timing_context(state, f"{train_unit.__class__.__name__}.on_train_end"):
         train_unit.on_train_end(state)
     _run_callback_fn(callbacks, "on_train_end", state, train_unit)
 
     # Reset training mode for modules at the end of the epoch
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     _reset_module_training_mode(tracked_modules, prior_module_train_states)
@@ -250,47 +246,54 @@
             evaluate_every_n_epochs = state.eval_state.evaluate_every_n_epochs
 
     # Check the progress to conditionally run this
     # to avoid running this multiple times
     # in the case of resuming from a checkpoint mid-epoch
     if train_state.progress.num_steps_completed_in_epoch == 0:
         with _get_timing_context(
-            state, f"train.{train_unit.__class__.__name__}.on_train_epoch_start"
+            state, f"{train_unit.__class__.__name__}.on_train_epoch_start"
         ):
             train_unit.on_train_epoch_start(state)
         _run_callback_fn(callbacks, "on_train_epoch_start", state, train_unit)
 
     _maybe_set_distributed_sampler_epoch(
         train_state.dataloader, train_state.progress.num_epochs_completed
     )
 
-    with record_function(__name__ + ".iter(dataloader)"):
+    with _get_timing_context(state, "train.iter(dataloader)"):
         data_iter = iter(train_state.dataloader)
     step_input = data_iter
 
     pass_data_iter_to_step = _step_requires_iterator(train_unit.train_step)
+    is_auto_unit = isinstance(train_unit, AutoUnit)
+
     prev_steps_in_epoch = train_state.progress.num_steps_completed_in_epoch
 
     while not (
         state.should_stop
         or _is_epoch_done(
             train_state.progress, train_state.max_steps_per_epoch, train_state.max_steps
         )
     ):
         try:
             if not pass_data_iter_to_step:
                 # get the next batch from the data iterator
-                with record_function(__name__ + ".next(data_iter)"):
+                with _get_timing_context(state, "train.next(data_iter)"):
                     step_input = next(data_iter)
 
             _run_callback_fn(callbacks, "on_train_step_start", state, train_unit)
+
             with _get_timing_context(
-                state, f"train.{train_unit.__class__.__name__}.train_step"
-            ), record_function(__name__ + ".train_step"):
+                state,
+                f"{train_unit.__class__.__name__}.train_step",
+                skip_timer=is_auto_unit,
+                # skip timer if train_unit is a subclass of AutoUnit because there is additional timing in the AutoUnit, and all timing should be mutually exclusive
+            ):
                 train_state._step_output = train_unit.train_step(state, step_input)
+
             train_state.progress.increment_step()
             _run_callback_fn(callbacks, "on_train_step_end", state, train_unit)
 
             # clear step_output to avoid retaining extra memory
             train_state._step_output = None
 
             if (
@@ -317,15 +320,15 @@
     if not any_steps_completed:
         logger.warning("No steps completed during train epoch!")
 
     # set progress counters for the next epoch
     train_state.progress.increment_epoch()
 
     with _get_timing_context(
-        state, f"train.{train_unit.__class__.__name__}.on_train_epoch_end"
+        state, f"{train_unit.__class__.__name__}.on_train_epoch_end"
     ):
         train_unit.on_train_epoch_end(state)
     _run_callback_fn(callbacks, "on_train_epoch_end", state, train_unit)
 
     if (
         evaluate_every_n_epochs
         and train_state.progress.num_epochs_completed % evaluate_every_n_epochs == 0
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/unit.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         self,
         name: str,
         value: Any,
         tracked_objects: Dict[str, Any],
     ) -> None:
         if tracked_objects is None:
             raise AttributeError(
-                "cannot assign parameter before _AppStateMixin.__init__() call"
+                "Please call super().__init__() before setting attributes."
             )
         _remove_from_dicts(
             name,
             self.__dict__,
             self._modules,
             self._optimizers,
             self._lr_schedulers,
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/framework/utils.py` & `torchtnt-nightly-2023.6.1/torchtnt/framework/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import collections
+import contextlib
 import inspect
 import logging
-from typing import (
-    Any,
-    Callable,
-    ContextManager,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Union,
-)
+from contextlib import contextmanager
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import typing_extensions
 from torch.distributed.fsdp import (
     FullyShardedDataParallel,
     FullyShardedDataParallel as FSDP,
 )
-
+from torch.profiler import record_function
 from torchtnt.utils.version import is_torch_version_geq_2_0
 
 if is_torch_version_geq_2_0():
     from torch.distributed._composable_state import _get_module_state
     from torch.distributed.fsdp._common_utils import _FSDPState
 
-import contextlib
 
 from pyre_extensions import none_throws
 from torchtnt.framework.callback import Callback
-from torchtnt.framework.progress import Progress
 from torchtnt.framework.state import ActivePhase, EntryPoint, State
 from torchtnt.framework.unit import AppStateMixin
 from torchtnt.utils.lr_scheduler import TLRScheduler
+from torchtnt.utils.progress import Progress
 from typing_extensions import Self
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 # Helper functions common across the loops
 def _is_done(
@@ -98,30 +89,40 @@
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     for name, module in modules.items():
         if name in prior_modes:
             module.train(prior_modes[name])
 
 
-def _get_timing_context(state: State, event_name: str) -> ContextManager:
-    return state.timer.time(event_name) if state.timer else contextlib.nullcontext()
+@contextmanager
+# pyre-fixme[3]: Return type must be annotated.
+def _get_timing_context(state: State, event_name: str, skip_timer: bool = False):
+    """Returns a context manager that records an event to a :class:`~torchtnt.utils.timer.Timer` and to PyTorch Profiler."""
+    timer_context = (
+        state.timer.time(event_name)
+        if state.timer and not skip_timer
+        else contextlib.nullcontext()
+    )
+    profiler_context = record_function(event_name)
+    with timer_context, profiler_context:
+        yield (timer_context, profiler_context)
 
 
 def _run_callback_fn(
     callbacks: List[Callback],
     fn_name: str,
     state: State,
     *args: Any,
     **kwargs: Any,
 ) -> None:
     for cb in callbacks:
         fn = getattr(cb, fn_name)
         if not callable(fn):
             raise ValueError(f"Invalid callback method name provided: {fn_name}")
-        with _get_timing_context(state, f"callback.{cb.name}.{fn_name}"):
+        with _get_timing_context(state, f"{cb.name}.{fn_name}"):
             fn(state, *args, **kwargs)
 
 
 def log_api_usage(entry_point: str) -> None:
     torch._C._log_api_usage_once(f"torchtnt.framework.{entry_point}")
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/__init__.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from .early_stop_checker import EarlyStopChecker
 from .env import init_from_env
 from .fsspec import get_filesystem
 from .lr_scheduler import TLRScheduler
 from .memory import get_tensor_size_bytes_map, measure_rss_deltas, RSSProfiler
 from .misc import days_to_secs, transfer_batch_norm_stats, transfer_weights
 from .oom import is_out_of_cpu_memory, is_out_of_cuda_memory, is_out_of_memory_error
+from .progress import Progress
 from .rank_zero_log import (
     rank_zero_critical,
     rank_zero_debug,
     rank_zero_error,
     rank_zero_info,
     rank_zero_print,
     rank_zero_warn,
@@ -75,14 +76,15 @@
     "get_tensor_size_bytes_map",
     "measure_rss_deltas",
     "RSSProfiler",
     "days_to_secs",
     "is_out_of_cpu_memory",
     "is_out_of_cuda_memory",
     "is_out_of_memory_error",
+    "Progress",
     "rank_zero_critical",
     "rank_zero_debug",
     "rank_zero_error",
     "rank_zero_info",
     "rank_zero_print",
     "rank_zero_warn",
     "seed",
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/data/__init__.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/data/iterators.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/device.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/distributed.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/distributed.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,19 @@
         if self.pg is None:
             return 1
         return dist.get_world_size(group=self.pg)
 
     def barrier(self) -> None:
         if self.pg is None:
             return
-        dist.barrier(group=self.pg)
+        backend = dist.get_backend(group=self.pg)
+        if backend == dist.Backend.NCCL:
+            dist.barrier(group=self.pg, device_ids=[torch.cuda.current_device()])
+        else:
+            dist.barrier(group=self.pg)
 
     def broadcast_object_list(self, obj_list: List[Any], src: int = 0) -> None:
         if self.pg is None:
             return
         dist.broadcast_object_list(obj_list, src=src, group=self.pg)
 
     def all_gather_object(self, obj_list: List[Any], obj: Any) -> None:
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/early_stop_checker.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/env.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/fsspec.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/__init__.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/csv.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/file.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/in_memory.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/json.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/logger.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/tensorboard.py`

 * *Files 13% similar despite different names*

```diff
@@ -130,14 +130,37 @@
             hparams (dict): dictionary of hyperparameter names and corresponding values
             metrics (dict): dictionary of name of metric and corresponding values
         """
 
         if self._writer:
             self._writer.add_hparams(hparams, metrics)
 
+    def log_image(self, *args: Any, **kwargs: Any) -> None:
+        """Add image data to TensorBoard.
+
+
+        Args:
+            *args (Any): Positional arguments passed to SummaryWriter.add_image
+            **kwargs(Any): Keyword arguments passed to SummaryWriter.add_image
+        """
+        writer = self._writer
+        if writer:
+            writer.add_image(*args, **kwargs)
+
+    def log_images(self, *args: Any, **kwargs: Any) -> None:
+        """Add batched image data to summary.
+
+        Args:
+            *args (Any): Positional arguments passed to SummaryWriter.add_images
+            **kwargs(Any): Keyword arguments passed to SummaryWriter.add_images
+        """
+        writer = self._writer
+        if writer:
+            writer.add_images(*args, **kwargs)
+
     def flush(self) -> None:
         """Writes pending logs to disk."""
 
         if self._writer:
             self._writer.flush()
 
     def close(self) -> None:
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/loggers/utils.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/memory.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/misc.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/oom.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/rank_zero_log.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/seed.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/seed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/test_utils.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/timer.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt/utils/version.py` & `torchtnt-nightly-2023.6.1/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.9/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.5.9
+Version: 2023.6.1
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.5.9 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.6.1 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.5.9/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt-nightly-2023.6.1/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 torchtnt/framework/__init__.py
 torchtnt/framework/_test_utils.py
 torchtnt/framework/auto_unit.py
 torchtnt/framework/callback.py
 torchtnt/framework/evaluate.py
 torchtnt/framework/fit.py
 torchtnt/framework/predict.py
-torchtnt/framework/progress.py
 torchtnt/framework/state.py
 torchtnt/framework/train.py
 torchtnt/framework/unit.py
 torchtnt/framework/utils.py
 torchtnt/framework/callbacks/__init__.py
 torchtnt/framework/callbacks/base_csv_writer.py
 torchtnt/framework/callbacks/garbage_collector.py
@@ -34,14 +33,15 @@
 torchtnt/utils/early_stop_checker.py
 torchtnt/utils/env.py
 torchtnt/utils/fsspec.py
 torchtnt/utils/lr_scheduler.py
 torchtnt/utils/memory.py
 torchtnt/utils/misc.py
 torchtnt/utils/oom.py
+torchtnt/utils/progress.py
 torchtnt/utils/rank_zero_log.py
 torchtnt/utils/seed.py
 torchtnt/utils/test_utils.py
 torchtnt/utils/timer.py
 torchtnt/utils/version.py
 torchtnt/utils/data/__init__.py
 torchtnt/utils/data/data_prefetcher.py
```

