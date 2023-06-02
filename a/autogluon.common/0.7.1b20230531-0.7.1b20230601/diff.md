# Comparing `tmp/autogluon.common-0.7.1b20230531.tar.gz` & `tmp/autogluon.common-0.7.1b20230601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-0.7.1b20230531.tar", last modified: Wed May 31 09:03:58 2023, max compression
+gzip compressed data, was "autogluon.common-0.7.1b20230601.tar", last modified: Thu Jun  1 09:03:39 2023, max compression
```

## Comparing `autogluon.common-0.7.1b20230531.tar` & `autogluon.common-0.7.1b20230601.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:58.459393 autogluon.common-0.7.1b20230531/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-31 09:03:58.459393 autogluon.common-0.7.1b20230531/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:03:58.459393 autogluon.common-0.7.1b20230531/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:58.451393 autogluon.common-0.7.1b20230531/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:58.451393 autogluon.common-0.7.1b20230531/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:58.455393 autogluon.common-0.7.1b20230531/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:58.455393 autogluon.common-0.7.1b20230531/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:58.455393 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:58.455393 autogluon.common-0.7.1b20230531/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:58.459393 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/deprecated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-31 09:03:45.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 09:03:57.000000 autogluon.common-0.7.1b20230531/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:58.455393 autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-31 09:03:57.000000 autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-31 09:03:58.000000 autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:03:57.000000 autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:03:57.000000 autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-31 09:03:57.000000 autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:03:57.000000 autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:03:57.000000 autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.416630 autogluon.common-0.7.1b20230601/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-06-01 09:03:39.416630 autogluon.common-0.7.1b20230601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:03:39.416630 autogluon.common-0.7.1b20230601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.412630 autogluon.common-0.7.1b20230601/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.412630 autogluon.common-0.7.1b20230601/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.412630 autogluon.common-0.7.1b20230601/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.412630 autogluon.common-0.7.1b20230601/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.412630 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.412630 autogluon.common-0.7.1b20230601/src/autogluon/common/model_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/model_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/model_filter/_model_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.412630 autogluon.common-0.7.1b20230601/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.416630 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/deprecated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-01 09:03:27.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 09:03:38.000000 autogluon.common-0.7.1b20230601/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:39.412630 autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-06-01 09:03:39.000000 autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-01 09:03:39.000000 autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:03:39.000000 autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:03:39.000000 autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-01 09:03:39.000000 autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:03:39.000000 autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:03:39.000000 autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-0.7.1b20230531/LICENSE` & `autogluon.common-0.7.1b20230601/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/PKG-INFO` & `autogluon.common-0.7.1b20230601/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230531
+Version: 0.7.1b20230601
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230531/setup.py` & `autogluon.common-0.7.1b20230601/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/features/infer_types.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/features/types.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_str.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/loaders/load_zip.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/loaders/load_zip.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/savers/save_json.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/savers/save_pd.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/savers/save_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/savers/save_str.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/space.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/deprecated_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/deprecated_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/file_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/log_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/nvutil.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/try_import.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/try_import.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon/common/utils/utils.py` & `autogluon.common-0.7.1b20230601/src/autogluon/common/utils/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from hashlib import md5
 from pathlib import Path
 from datetime import datetime
 
 import logging
 import os
+import pandas as pd
 import platform
 import sys
 from typing import Dict, Any, Optional
 
 from ..version import __version__
 try:
     from ..version import __lite__
@@ -163,7 +165,20 @@
 
         if require_version_match:
             raise AssertionError(
                 f"Predictor was created on version {version_saved} but is being loaded with version {version_current}. "
                 f"Please ensure the versions match to avoid instability. While it is NOT recommended, "
                 f"this error can be bypassed by specifying `require_version_match=False`."
             )
+
+
+def hash_pandas_df(df: Optional[pd.DataFrame]) -> str:
+    """Compute a hash string for a pandas DataFrame."""
+    if df is not None:
+        # Convert in case TimeSeriesDataFrame object is passed
+        df = pd.DataFrame(df, copy=True)
+        df.reset_index(inplace=True)
+        df.sort_index(inplace=True, axis=1)
+        hashable_object = pd.util.hash_pandas_object(df).values
+    else:
+        hashable_object = "0".encode("utf-8")
+    return md5(hashable_object).hexdigest()
```

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230531
+Version: 0.7.1b20230601
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230531/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-0.7.1b20230601/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 src/autogluon/common/loaders/load_json.py
 src/autogluon/common/loaders/load_pd.py
 src/autogluon/common/loaders/load_pkl.py
 src/autogluon/common/loaders/load_pointer.py
 src/autogluon/common/loaders/load_s3.py
 src/autogluon/common/loaders/load_str.py
 src/autogluon/common/loaders/load_zip.py
+src/autogluon/common/model_filter/__init__.py
+src/autogluon/common/model_filter/_model_filter.py
 src/autogluon/common/savers/__init__.py
 src/autogluon/common/savers/save_json.py
 src/autogluon/common/savers/save_pd.py
 src/autogluon/common/savers/save_pkl.py
 src/autogluon/common/savers/save_pointer.py
 src/autogluon/common/savers/save_str.py
 src/autogluon/common/utils/__init__.py
```

