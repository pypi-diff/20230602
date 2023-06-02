# Comparing `tmp/ml-research-0.4a1.tar.gz` & `tmp/ml-research-0.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-research-0.4a1.tar", last modified: Thu Apr 14 00:39:58 2022, max compression
+gzip compressed data, was "ml-research-0.4a2.tar", last modified: Mon Oct 10 09:38:02 2022, max compression
```

## Comparing `ml-research-0.4a1.tar` & `ml-research-0.4a2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.496310 ml-research-0.4a1/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-04-14 00:39:44.000000 ml-research-0.4a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5371 2022-04-14 00:39:58.496310 ml-research-0.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4270 2022-04-14 00:39:44.000000 ml-research-0.4a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/ml_research.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5371 2022-04-14 00:39:57.000000 ml-research-0.4a1/ml_research.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-04-14 00:39:58.000000 ml-research-0.4a1/ml_research.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-14 00:39:57.000000 ml-research-0.4a1/ml_research.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-04-14 00:39:58.000000 ml-research-0.4a1/ml_research.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-14 00:39:58.000000 ml-research-0.4a1/ml_research.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/mlresearch/
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/_min_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/mlresearch/active_learning/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/active_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/active_learning/_acquisition_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14935 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/active_learning/_active_learning.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/active_learning/_deep_al.py
--rw-r--r--   0 runner    (1001) docker     (121)    12402 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/active_learning/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/mlresearch/active_learning/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/active_learning/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/active_learning/tests/test_acquisition_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6740 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/active_learning/tests/test_active_learning_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/mlresearch/data_augmentation/
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/data_augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25784 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/data_augmentation/_gsmote.py
--rw-r--r--   0 runner    (1001) docker     (121)     5375 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/data_augmentation/_image_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     9301 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/data_augmentation/_oversampling_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/mlresearch/data_augmentation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/data_augmentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15847 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/data_augmentation/tests/test_gsmote.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/data_augmentation/tests/test_image_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     6205 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/data_augmentation/tests/test_oversampling_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/mlresearch/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16678 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/datasets/_binary.py
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/datasets/_image.py
--rw-r--r--   0 runner    (1001) docker     (121)    20657 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/datasets/_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     5522 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/datasets/_remote_sensing.py
--rw-r--r--   0 runner    (1001) docker     (121)    13789 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/datasets/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/mlresearch/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/datasets/tests/test_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/mlresearch/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/metrics/_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.492309 ml-research-0.4a1/mlresearch/metrics/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/metrics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/metrics/tests/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.496310 ml-research-0.4a1/mlresearch/self_supervised/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/self_supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6549 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/self_supervised/_byol.py
--rw-r--r--   0 runner    (1001) docker     (121)     6321 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/self_supervised/_components.py
--rw-r--r--   0 runner    (1001) docker     (121)     5889 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/self_supervised/_lars.py
--rw-r--r--   0 runner    (1001) docker     (121)     5142 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/self_supervised/_simsiam.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.496310 ml-research-0.4a1/mlresearch/self_supervised/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/self_supervised/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/self_supervised/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/self_supervised/tests/test_ssl_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.496310 ml-research-0.4a1/mlresearch/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8661 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/tests/test_docstring_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.496310 ml-research-0.4a1/mlresearch/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/_check_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3678 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3225 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:58.496310 ml-research-0.4a1/mlresearch/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9066 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/tests/test_check_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-04-14 00:39:44.000000 ml-research-0.4a1/mlresearch/utils/tests/test_load_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-14 00:39:58.496310 ml-research-0.4a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-04-14 00:39:44.000000 ml-research-0.4a1/setup.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.093639 ml-research-0.4a2/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1081 2022-02-14 04:38:40.000000 ml-research-0.4a2/LICENSE
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6059 2022-10-10 09:38:02.093639 ml-research-0.4a2/PKG-INFO
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     4978 2022-04-22 15:10:17.000000 ml-research-0.4a2/README.md
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.089638 ml-research-0.4a2/ml_research.egg-info/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6059 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/PKG-INFO
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     2247 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/SOURCES.txt
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        1 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/dependency_links.txt
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      936 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/requires.txt
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)       11 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/top_level.txt
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.089638 ml-research-0.4a2/mlresearch/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1888 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     2258 2022-04-13 14:07:23.000000 ml-research-0.4a2/mlresearch/_min_dependencies.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      585 2022-10-10 09:26:21.000000 ml-research-0.4a2/mlresearch/_version.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.089638 ml-research-0.4a2/mlresearch/active_learning/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      247 2022-02-22 22:57:29.000000 ml-research-0.4a2/mlresearch/active_learning/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1025 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/active_learning/_acquisition_functions.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    14935 2022-03-09 17:13:27.000000 ml-research-0.4a2/mlresearch/active_learning/_active_learning.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1266 2022-03-14 16:14:24.000000 ml-research-0.4a2/mlresearch/active_learning/_deep_al.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    12402 2022-03-10 09:50:23.000000 ml-research-0.4a2/mlresearch/active_learning/base.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.090638 ml-research-0.4a2/mlresearch/active_learning/tests/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/active_learning/tests/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      441 2022-02-22 22:48:12.000000 ml-research-0.4a2/mlresearch/active_learning/tests/test_acquisition_functions.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6740 2022-03-10 09:58:24.000000 ml-research-0.4a2/mlresearch/active_learning/tests/test_active_learning_models.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.090638 ml-research-0.4a2/mlresearch/data_augmentation/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      423 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    25784 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/_gsmote.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     5375 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/_image_transforms.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     9301 2022-03-08 19:04:51.000000 ml-research-0.4a2/mlresearch/data_augmentation/_oversampling_augmentation.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.090638 ml-research-0.4a2/mlresearch/data_augmentation/tests/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/tests/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    15847 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/tests/test_gsmote.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      589 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/tests/test_image_transforms.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6205 2022-03-08 19:07:38.000000 ml-research-0.4a2/mlresearch/data_augmentation/tests/test_oversampling_augmentation.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/datasets/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      493 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/datasets/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    16678 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/datasets/_binary.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3215 2022-04-13 10:45:51.000000 ml-research-0.4a2/mlresearch/datasets/_image.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    21236 2022-04-14 15:07:12.000000 ml-research-0.4a2/mlresearch/datasets/_multiclass.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     5522 2022-04-13 10:45:51.000000 ml-research-0.4a2/mlresearch/datasets/_remote_sensing.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    13894 2022-04-16 12:13:40.000000 ml-research-0.4a2/mlresearch/datasets/base.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/datasets/tests/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/datasets/tests/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1833 2022-04-16 12:39:03.000000 ml-research-0.4a2/mlresearch/datasets/tests/test_datasets.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/metrics/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      511 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/metrics/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3683 2022-04-13 13:49:22.000000 ml-research-0.4a2/mlresearch/metrics/_metrics.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/metrics/tests/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/metrics/tests/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1953 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/metrics/tests/test_metrics.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/self_supervised/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)       85 2022-03-19 15:51:17.000000 ml-research-0.4a2/mlresearch/self_supervised/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6549 2022-03-19 13:55:53.000000 ml-research-0.4a2/mlresearch/self_supervised/_byol.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6321 2022-03-18 17:26:17.000000 ml-research-0.4a2/mlresearch/self_supervised/_components.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     5889 2022-03-18 13:26:59.000000 ml-research-0.4a2/mlresearch/self_supervised/_lars.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     5142 2022-03-19 15:45:30.000000 ml-research-0.4a2/mlresearch/self_supervised/_simsiam.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.092638 ml-research-0.4a2/mlresearch/self_supervised/tests/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/self_supervised/tests/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      852 2022-03-18 17:26:17.000000 ml-research-0.4a2/mlresearch/self_supervised/tests/test_scheduler.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3029 2022-03-19 15:33:15.000000 ml-research-0.4a2/mlresearch/self_supervised/tests/test_ssl_models.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.092638 ml-research-0.4a2/mlresearch/tests/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/tests/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     8661 2022-02-23 00:15:38.000000 ml-research-0.4a2/mlresearch/tests/test_docstring_parameters.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.092638 ml-research-0.4a2/mlresearch/utils/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      820 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3368 2022-04-13 14:04:47.000000 ml-research-0.4a2/mlresearch/utils/_check_pipelines.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     2288 2022-02-23 18:59:45.000000 ml-research-0.4a2/mlresearch/utils/_data.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      484 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/_image.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3678 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/_testing.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3225 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/_utils.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1830 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/_visualization.py
+drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.093639 ml-research-0.4a2/mlresearch/utils/tests/
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/tests/__init__.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     9066 2022-04-13 14:04:47.000000 ml-research-0.4a2/mlresearch/utils/tests/test_check_pipelines.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1719 2022-02-23 18:59:45.000000 ml-research-0.4a2/mlresearch/utils/tests/test_load_datasets.py
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)       38 2022-10-10 09:38:02.093639 ml-research-0.4a2/setup.cfg
+-rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     2363 2022-04-14 00:35:14.000000 ml-research-0.4a2/setup.py
```

### Comparing `ml-research-0.4a1/LICENSE` & `ml-research-0.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/PKG-INFO` & `ml-research-0.4a2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,41 @@
-Metadata-Version: 2.1
-Name: ml-research
-Version: 0.4a1
-Summary: Implementation of Machine Learning algorithms, experiments and utilities.
-Home-page: https://github.com/joaopfonseca/ml-research
-Download-URL: https://github.com/joaopfonseca/ml-research
-Maintainer: J. Fonseca
-Maintainer-email: jpfonseca@novaims.unl.pt
-License: MIT
-Platform: UNKNOWN
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: optional
-Provides-Extra: docs
-Provides-Extra: examples
-Provides-Extra: tests
-Provides-Extra: all
-License-File: LICENSE
-
 <div align="center">
 <img src="docs/_static/logo.png" width="400px">
 </div>
 
 ______________________________________________________________________
 
 <p align="center">
 <a href="https://github.com/joaopfonseca/ml-research/actions/workflows/ci.yml"><img alt="Github Actions" src="https://github.com/joaopfonseca/ml-research/actions/workflows/ci.yml/badge.svg"></a>
 <a href="https://codecov.io/gh/joaopfonseca/ml-research"><img alt="Codecov" src="https://codecov.io/gh/joaopfonseca/ml-research/branch/master/graph/badge.svg?token=J2EBA4YTMN"></a>
 <a href="https://mlresearch.readthedocs.io/en/latest/?badge=latest"><img alt="Documentation Status" src="https://readthedocs.org/projects/mlresearch/badge/?version=latest"></a>
-<a href="https://badge.fury.io/py/ml-research"><img alt="Pypi Version" src="https://badge.fury.io/py/ml-research.svg"></a>
-<a href="https://pepy.tech/project/ml-research"><img alt="Downloads" src="https://pepy.tech/badge/ml-research"></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://img.shields.io/badge/python-3.8%20|%203.9-blue"><img alt="Python Versions" src="https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue"></a>
 <a href="https://doi.org/10.3390/RS13132619"><img alt="DOI" src="https://zenodo.org/badge/DOI/10.3390/RS13132619.svg"></a>
 </p>
+<table align="center">
+  <tr>
+    <td>
+      <b>PyPI</b>
+    </td>
+    <td>
+      <a href="https://badge.fury.io/py/ml-research"><img alt="Pypi Version" src="https://badge.fury.io/py/ml-research.svg"></a>
+      <a href="https://pepy.tech/project/ml-research"><img alt="Downloads" src="https://static.pepy.tech/personalized-badge/ml-research?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads"></a>
+    </td>
+  </tr>
+  <tr>
+    <td>
+      <b>Anaconda</b>
+    </td>
+    <td>
+      <a href="https://anaconda.org/conda-forge/ml-research"><img alt="Conda Version" src="https://img.shields.io/conda/vn/conda-forge/ml-research.svg"></a>
+      <a href="https://anaconda.org/conda-forge/ml-research"><img alt="Conda Downloads" src="https://img.shields.io/conda/dn/conda-forge/ml-research.svg"></a>
+    </td>
+  </tr>
+</table>
 
 ``ML-Research`` is an open source library for machine learning research.  It
 contains the software implementation of most algorithms used or developed in
 my research. Specifically, it contains ``scikit-learn`` compatible
 implementations for Active Learning, Oversampling, Datasets and various
 utilities to assist in experiment design and results reporting. Other
 techniques, such as self-supervised learning and semi-supervised learning are
@@ -78,19 +65,22 @@
 - seaborn (>= 0.9.0)
 - pytorch (>= 1.10.1)
 - torchvision (>= 0.11.2)
 - pytorch_lightning (>= 1.5.8)
 
 ### User Installation
 
-If you already have a working installation of numpy and scipy, the easiest way
-to install scikit-learn is using ``pip`` :
+The easiest way to install ml-research is using ``pip`` :
 
     pip install -U ml-research
 
+Or ``conda`` :
+
+    conda install -c conda-forge ml-research
+
 The documentation includes more detailed [installation
 instructions](https://mlresearch.readthedocs.io/en/latest/getting-started.html).
 
 ### Installing from source
 
 The following commands should allow you to setup the development version of the
 project with minimal effort:
@@ -99,16 +89,17 @@
     git clone https://github.com/joaopfonseca/ml-research.git
     cd ml-research
 
     # Create and activate an environment 
     make environment 
     conda activate mlresearch # Adapt this line accordingly if you're not running conda
 
-    # Install project requirements and the research package
-    pip install .[tests,docs]
+    # Install project requirements and the research package. Dependecy group
+    # "all" will also install both dependency groups shown below.
+    pip install .[tests,docs] 
 
 ## Citing ML-Research
 
 If you use ML-Research in a scientific publication, we would appreciate
 citations to the following paper:
 
     @article{Fonseca2021,
@@ -120,9 +111,7 @@
       publisher = {Multidisciplinary Digital Publishing Institute},
       volume = {13},
       pages = {2619},
       author = {Fonseca, Joao and Douzas, Georgios and Bacao, Fernando},
       title = {{Increasing the Effectiveness of Active Learning: Introducing Artificial Data Generation in Active Learning for Land Use/Land Cover Classification}},
       journal = {Remote Sensing}
     }
-
-
```

#### html2text {}

```diff
@@ -1,26 +1,13 @@
-Metadata-Version: 2.1 Name: ml-research Version: 0.4a1 Summary: Implementation
-of Machine Learning algorithms, experiments and utilities. Home-page: https://
-github.com/joaopfonseca/ml-research Download-URL: https://github.com/
-joaopfonseca/ml-research Maintainer: J. Fonseca Maintainer-email:
-jpfonseca@novaims.unl.pt License: MIT Platform: UNKNOWN Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
-Engineering Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: POSIX Classifier: Operating System :: Unix Classifier:
-Operating System :: MacOS Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Description-Content-Type: text/markdown Provides-
-Extra: optional Provides-Extra: docs Provides-Extra: examples Provides-Extra:
-tests Provides-Extra: all License-File: LICENSE
                             [docs/_static/logo.png]
 ______________________________________________________________________
- [Github_Actions] [Codecov] [Documentation_Status] [Pypi_Version] [Downloads]
-                        [Black] [Python_Versions] [DOI]
+ [Github_Actions] [Codecov] [Documentation_Status] [Black] [Python_Versions]
+                                     [DOI]
+                  PyPI     [Pypi_Version] [Downloads]
+                  Anaconda [Conda_Version] [Conda_Downloads]
 ``ML-Research`` is an open source library for machine learning research. It
 contains the software implementation of most algorithms used or developed in my
 research. Specifically, it contains ``scikit-learn`` compatible implementations
 for Active Learning, Oversampling, Datasets and various utilities to assist in
 experiment design and results reporting. Other techniques, such as self-
 supervised learning and semi-supervised learning are currently under
 development and are being implemented in ``pytorch`` and intended to be
@@ -30,27 +17,28 @@
 joaopfonseca/publications). Contributions at the algorithm level are available
 in the package ``mlresearch``. ## Installation A Python distribution of version
 3.8, 3.9 or 3.10 is required to run this project. Earlier Python versions might
 work in most cases, but they are not tested. ``ML-Research`` requires: - numpy
 (>= 1.14.6) - pandas (>= 1.3.5) - sklearn (>= 1.0.0) - imblearn (>= 0.8.0) -
 rich (>= 10.16.1) - matplotlib (>= 2.2.3) - seaborn (>= 0.9.0) - pytorch (>=
 1.10.1) - torchvision (>= 0.11.2) - pytorch_lightning (>= 1.5.8) ### User
-Installation If you already have a working installation of numpy and scipy, the
-easiest way to install scikit-learn is using ``pip`` : pip install -U ml-
-research The documentation includes more detailed [installation instructions]
-(https://mlresearch.readthedocs.io/en/latest/getting-started.html). ###
-Installing from source The following commands should allow you to setup the
-development version of the project with minimal effort: # Clone the project.
-git clone https://github.com/joaopfonseca/ml-research.git cd ml-research #
-Create and activate an environment make environment conda activate mlresearch #
-Adapt this line accordingly if you're not running conda # Install project
-requirements and the research package pip install .[tests,docs] ## Citing ML-
-Research If you use ML-Research in a scientific publication, we would
-appreciate citations to the following paper: @article{Fonseca2021, doi =
-{10.3390/RS13132619}, url = {https://doi.org/10.3390/RS13132619}, keywords =
-{SMOTE,active learning,artificial data generation,land use/land cover
+Installation The easiest way to install ml-research is using ``pip`` : pip
+install -U ml-research Or ``conda`` : conda install -c conda-forge ml-research
+The documentation includes more detailed [installation instructions](https://
+mlresearch.readthedocs.io/en/latest/getting-started.html). ### Installing from
+source The following commands should allow you to setup the development version
+of the project with minimal effort: # Clone the project. git clone https://
+github.com/joaopfonseca/ml-research.git cd ml-research # Create and activate an
+environment make environment conda activate mlresearch # Adapt this line
+accordingly if you're not running conda # Install project requirements and the
+research package. Dependecy group # "all" will also install both dependency
+groups shown below. pip install .[tests,docs] ## Citing ML-Research If you use
+ML-Research in a scientific publication, we would appreciate citations to the
+following paper: @article{Fonseca2021, doi = {10.3390/RS13132619}, url =
+{https://doi.org/10.3390/RS13132619}, keywords = {SMOTE,active
+learning,artificial data generation,land use/land cover
 classification,oversampling}, year = {2021}, month = {jul}, publisher =
 {Multidisciplinary Digital Publishing Institute}, volume = {13}, pages =
 {2619}, author = {Fonseca, Joao and Douzas, Georgios and Bacao, Fernando},
 title = {{Increasing the Effectiveness of Active Learning: Introducing
 Artificial Data Generation in Active Learning for Land Use/Land Cover
 Classification}}, journal = {Remote Sensing} }
```

### Comparing `ml-research-0.4a1/ml_research.egg-info/PKG-INFO` & `ml-research-0.4a2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ml-research
-Version: 0.4a1
+Version: 0.4a2
 Summary: Implementation of Machine Learning algorithms, experiments and utilities.
 Home-page: https://github.com/joaopfonseca/ml-research
 Download-URL: https://github.com/joaopfonseca/ml-research
 Maintainer: J. Fonseca
 Maintainer-email: jpfonseca@novaims.unl.pt
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
@@ -35,20 +34,38 @@
 
 ______________________________________________________________________
 
 <p align="center">
 <a href="https://github.com/joaopfonseca/ml-research/actions/workflows/ci.yml"><img alt="Github Actions" src="https://github.com/joaopfonseca/ml-research/actions/workflows/ci.yml/badge.svg"></a>
 <a href="https://codecov.io/gh/joaopfonseca/ml-research"><img alt="Codecov" src="https://codecov.io/gh/joaopfonseca/ml-research/branch/master/graph/badge.svg?token=J2EBA4YTMN"></a>
 <a href="https://mlresearch.readthedocs.io/en/latest/?badge=latest"><img alt="Documentation Status" src="https://readthedocs.org/projects/mlresearch/badge/?version=latest"></a>
-<a href="https://badge.fury.io/py/ml-research"><img alt="Pypi Version" src="https://badge.fury.io/py/ml-research.svg"></a>
-<a href="https://pepy.tech/project/ml-research"><img alt="Downloads" src="https://pepy.tech/badge/ml-research"></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://img.shields.io/badge/python-3.8%20|%203.9-blue"><img alt="Python Versions" src="https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue"></a>
 <a href="https://doi.org/10.3390/RS13132619"><img alt="DOI" src="https://zenodo.org/badge/DOI/10.3390/RS13132619.svg"></a>
 </p>
+<table align="center">
+  <tr>
+    <td>
+      <b>PyPI</b>
+    </td>
+    <td>
+      <a href="https://badge.fury.io/py/ml-research"><img alt="Pypi Version" src="https://badge.fury.io/py/ml-research.svg"></a>
+      <a href="https://pepy.tech/project/ml-research"><img alt="Downloads" src="https://static.pepy.tech/personalized-badge/ml-research?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads"></a>
+    </td>
+  </tr>
+  <tr>
+    <td>
+      <b>Anaconda</b>
+    </td>
+    <td>
+      <a href="https://anaconda.org/conda-forge/ml-research"><img alt="Conda Version" src="https://img.shields.io/conda/vn/conda-forge/ml-research.svg"></a>
+      <a href="https://anaconda.org/conda-forge/ml-research"><img alt="Conda Downloads" src="https://img.shields.io/conda/dn/conda-forge/ml-research.svg"></a>
+    </td>
+  </tr>
+</table>
 
 ``ML-Research`` is an open source library for machine learning research.  It
 contains the software implementation of most algorithms used or developed in
 my research. Specifically, it contains ``scikit-learn`` compatible
 implementations for Active Learning, Oversampling, Datasets and various
 utilities to assist in experiment design and results reporting. Other
 techniques, such as self-supervised learning and semi-supervised learning are
@@ -78,19 +95,22 @@
 - seaborn (>= 0.9.0)
 - pytorch (>= 1.10.1)
 - torchvision (>= 0.11.2)
 - pytorch_lightning (>= 1.5.8)
 
 ### User Installation
 
-If you already have a working installation of numpy and scipy, the easiest way
-to install scikit-learn is using ``pip`` :
+The easiest way to install ml-research is using ``pip`` :
 
     pip install -U ml-research
 
+Or ``conda`` :
+
+    conda install -c conda-forge ml-research
+
 The documentation includes more detailed [installation
 instructions](https://mlresearch.readthedocs.io/en/latest/getting-started.html).
 
 ### Installing from source
 
 The following commands should allow you to setup the development version of the
 project with minimal effort:
@@ -99,16 +119,17 @@
     git clone https://github.com/joaopfonseca/ml-research.git
     cd ml-research
 
     # Create and activate an environment 
     make environment 
     conda activate mlresearch # Adapt this line accordingly if you're not running conda
 
-    # Install project requirements and the research package
-    pip install .[tests,docs]
+    # Install project requirements and the research package. Dependecy group
+    # "all" will also install both dependency groups shown below.
+    pip install .[tests,docs] 
 
 ## Citing ML-Research
 
 If you use ML-Research in a scientific publication, we would appreciate
 citations to the following paper:
 
     @article{Fonseca2021,
@@ -120,9 +141,7 @@
       publisher = {Multidisciplinary Digital Publishing Institute},
       volume = {13},
       pages = {2619},
       author = {Fonseca, Joao and Douzas, Georgios and Bacao, Fernando},
       title = {{Increasing the Effectiveness of Active Learning: Introducing Artificial Data Generation in Active Learning for Land Use/Land Cover Classification}},
       journal = {Remote Sensing}
     }
-
-
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
-Metadata-Version: 2.1 Name: ml-research Version: 0.4a1 Summary: Implementation
+Metadata-Version: 2.1 Name: ml-research Version: 0.4a2 Summary: Implementation
 of Machine Learning algorithms, experiments and utilities. Home-page: https://
 github.com/joaopfonseca/ml-research Download-URL: https://github.com/
 joaopfonseca/ml-research Maintainer: J. Fonseca Maintainer-email:
-jpfonseca@novaims.unl.pt License: MIT Platform: UNKNOWN Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
-Engineering Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: POSIX Classifier: Operating System :: Unix Classifier:
-Operating System :: MacOS Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Description-Content-Type: text/markdown Provides-
-Extra: optional Provides-Extra: docs Provides-Extra: examples Provides-Extra:
-tests Provides-Extra: all License-File: LICENSE
+jpfonseca@novaims.unl.pt License: MIT Classifier: Intended Audience :: Science/
+Research Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved Classifier: Programming Language :: Python Classifier: Topic ::
+Software Development Classifier: Topic :: Scientific/Engineering Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown Provides-Extra: optional Provides-
+Extra: docs Provides-Extra: examples Provides-Extra: tests Provides-Extra: all
+License-File: LICENSE
                             [docs/_static/logo.png]
 ______________________________________________________________________
- [Github_Actions] [Codecov] [Documentation_Status] [Pypi_Version] [Downloads]
-                        [Black] [Python_Versions] [DOI]
+ [Github_Actions] [Codecov] [Documentation_Status] [Black] [Python_Versions]
+                                     [DOI]
+                  PyPI     [Pypi_Version] [Downloads]
+                  Anaconda [Conda_Version] [Conda_Downloads]
 ``ML-Research`` is an open source library for machine learning research. It
 contains the software implementation of most algorithms used or developed in my
 research. Specifically, it contains ``scikit-learn`` compatible implementations
 for Active Learning, Oversampling, Datasets and various utilities to assist in
 experiment design and results reporting. Other techniques, such as self-
 supervised learning and semi-supervised learning are currently under
 development and are being implemented in ``pytorch`` and intended to be
@@ -30,27 +32,28 @@
 joaopfonseca/publications). Contributions at the algorithm level are available
 in the package ``mlresearch``. ## Installation A Python distribution of version
 3.8, 3.9 or 3.10 is required to run this project. Earlier Python versions might
 work in most cases, but they are not tested. ``ML-Research`` requires: - numpy
 (>= 1.14.6) - pandas (>= 1.3.5) - sklearn (>= 1.0.0) - imblearn (>= 0.8.0) -
 rich (>= 10.16.1) - matplotlib (>= 2.2.3) - seaborn (>= 0.9.0) - pytorch (>=
 1.10.1) - torchvision (>= 0.11.2) - pytorch_lightning (>= 1.5.8) ### User
-Installation If you already have a working installation of numpy and scipy, the
-easiest way to install scikit-learn is using ``pip`` : pip install -U ml-
-research The documentation includes more detailed [installation instructions]
-(https://mlresearch.readthedocs.io/en/latest/getting-started.html). ###
-Installing from source The following commands should allow you to setup the
-development version of the project with minimal effort: # Clone the project.
-git clone https://github.com/joaopfonseca/ml-research.git cd ml-research #
-Create and activate an environment make environment conda activate mlresearch #
-Adapt this line accordingly if you're not running conda # Install project
-requirements and the research package pip install .[tests,docs] ## Citing ML-
-Research If you use ML-Research in a scientific publication, we would
-appreciate citations to the following paper: @article{Fonseca2021, doi =
-{10.3390/RS13132619}, url = {https://doi.org/10.3390/RS13132619}, keywords =
-{SMOTE,active learning,artificial data generation,land use/land cover
+Installation The easiest way to install ml-research is using ``pip`` : pip
+install -U ml-research Or ``conda`` : conda install -c conda-forge ml-research
+The documentation includes more detailed [installation instructions](https://
+mlresearch.readthedocs.io/en/latest/getting-started.html). ### Installing from
+source The following commands should allow you to setup the development version
+of the project with minimal effort: # Clone the project. git clone https://
+github.com/joaopfonseca/ml-research.git cd ml-research # Create and activate an
+environment make environment conda activate mlresearch # Adapt this line
+accordingly if you're not running conda # Install project requirements and the
+research package. Dependecy group # "all" will also install both dependency
+groups shown below. pip install .[tests,docs] ## Citing ML-Research If you use
+ML-Research in a scientific publication, we would appreciate citations to the
+following paper: @article{Fonseca2021, doi = {10.3390/RS13132619}, url =
+{https://doi.org/10.3390/RS13132619}, keywords = {SMOTE,active
+learning,artificial data generation,land use/land cover
 classification,oversampling}, year = {2021}, month = {jul}, publisher =
 {Multidisciplinary Digital Publishing Institute}, volume = {13}, pages =
 {2619}, author = {Fonseca, Joao and Douzas, Georgios and Bacao, Fernando},
 title = {{Increasing the Effectiveness of Active Learning: Introducing
 Artificial Data Generation in Active Learning for Land Use/Land Cover
 Classification}}, journal = {Remote Sensing} }
```

### Comparing `ml-research-0.4a1/ml_research.egg-info/SOURCES.txt` & `ml-research-0.4a2/ml_research.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/ml_research.egg-info/requires.txt` & `ml-research-0.4a2/ml_research.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/__init__.py` & `ml-research-0.4a2/mlresearch/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/_min_dependencies.py` & `ml-research-0.4a2/mlresearch/_min_dependencies.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/_version.py` & `ml-research-0.4a2/mlresearch/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #   X.YrcN  # Release Candidate
 #   X.Y     # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
 
-__version__ = "0.4a1"
+__version__ = "0.4a2"
```

### Comparing `ml-research-0.4a1/mlresearch/active_learning/_acquisition_functions.py` & `ml-research-0.4a2/mlresearch/active_learning/_acquisition_functions.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/active_learning/_active_learning.py` & `ml-research-0.4a2/mlresearch/active_learning/_active_learning.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/active_learning/_deep_al.py` & `ml-research-0.4a2/mlresearch/active_learning/_deep_al.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/active_learning/base.py` & `ml-research-0.4a2/mlresearch/active_learning/base.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/active_learning/tests/test_active_learning_models.py` & `ml-research-0.4a2/mlresearch/active_learning/tests/test_active_learning_models.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/data_augmentation/_gsmote.py` & `ml-research-0.4a2/mlresearch/data_augmentation/_gsmote.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/data_augmentation/_image_transforms.py` & `ml-research-0.4a2/mlresearch/data_augmentation/_image_transforms.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/data_augmentation/_oversampling_augmentation.py` & `ml-research-0.4a2/mlresearch/data_augmentation/_oversampling_augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/data_augmentation/tests/test_gsmote.py` & `ml-research-0.4a2/mlresearch/data_augmentation/tests/test_gsmote.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/data_augmentation/tests/test_image_transforms.py` & `ml-research-0.4a2/mlresearch/data_augmentation/tests/test_image_transforms.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/data_augmentation/tests/test_oversampling_augmentation.py` & `ml-research-0.4a2/mlresearch/data_augmentation/tests/test_oversampling_augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/datasets/_binary.py` & `ml-research-0.4a2/mlresearch/datasets/_binary.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/datasets/_image.py` & `ml-research-0.4a2/mlresearch/datasets/_image.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/datasets/_multiclass.py` & `ml-research-0.4a2/mlresearch/datasets/_multiclass.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,18 @@
     def fetch_adult(self):
         """Download and transform the Adult Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Adult
         """
         data = pd.read_csv(FETCH_URLS["adult"], header=None, na_values=" ?").dropna()
         data.rename(columns={data.columns[-1]: "target"}, inplace=True)
+
+        mapper = {v: k for k, v in enumerate(data.target.unique())}
+        data.target = data.target.map(mapper)
+
         categorical_features = [1, 3, 5, 6, 7, 8, 9, 13]
         return data, categorical_features
 
     def fetch_abalone(self):
         """Download and transform the Abalone Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Abalone
@@ -89,14 +93,18 @@
         https://archive.ics.uci.edu/ml/datasets/Acute+Inflammations
         """
         data = pd.read_csv(
             FETCH_URLS["acute"], header=None, sep="\t", decimal=",", encoding="UTF-16"
         )
         data["target"] = data[6].str[0] + data[7].str[0]
         data.drop(columns=[6, 7], inplace=True)
+
+        mapper = {v: k for k, v in enumerate(data.target.unique())}
+        data.target = data.target.map(mapper)
+
         categorical_features = list(range(1, 6))
         return data, categorical_features
 
     def fetch_annealing(self):
         """Download and transform the Annealing Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Annealing
@@ -107,14 +115,17 @@
         missing_feats = (data.isnull().sum(0) / data.shape[0]) < 0.1
         data = data.iloc[:, missing_feats.values]
         data[2].fillna(data[2].mode().squeeze(), inplace=True)
 
         data = data.T.reset_index(drop=True).T
         data.rename(columns={data.columns[-1]: "target"}, inplace=True)
 
+        mapper = {v: k for k, v in enumerate(data.target.unique())}
+        data.target = data.target.map(mapper)
+
         categorical_features = [0, 1, 5, 9]
         return data, categorical_features
 
     def fetch_census(self):
         """Download and transform the Census-Income (KDD) Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Census-Income+%28KDD%29
@@ -142,14 +153,18 @@
         data = data.drop(columns=cols_ids).T.reset_index(drop=True).T
         # some rows are dropped; they have rare missing values
         data = data.iloc[
             data.applymap(lambda x: x != " Not in universe").all(1).values, :
         ]
 
         data.rename(columns={data.columns[-1]: "target"}, inplace=True)
+
+        mapper = {v: k for k, v in enumerate(data.target.unique())}
+        data.target = data.target.map(mapper)
+
         return data, categorical_features
 
     def fetch_contraceptive(self):
         """Download and transform the Contraceptive Method Choice Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Contraceptive+Method+Choice
         """
@@ -182,14 +197,18 @@
 
         https://archive.ics.uci.edu/ml/datasets/Credit+Approval
         """
         data = pd.read_csv(
             FETCH_URLS["credit_approval"], header=None, na_values="?"
         ).dropna()
         data.rename(columns={data.columns[-1]: "target"}, inplace=True)
+
+        mapper = {v: k for k, v in enumerate(data.target.unique())}
+        data.target = data.target.map(mapper)
+
         categorical_features = [0, 3, 4, 5, 6, 8, 9, 11, 12]
         return data, categorical_features
 
     def fetch_dermatology(self):
         """Download and transform the Dermatology Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Dermatology
```

### Comparing `ml-research-0.4a1/mlresearch/datasets/_remote_sensing.py` & `ml-research-0.4a2/mlresearch/datasets/_remote_sensing.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/datasets/base.py` & `ml-research-0.4a2/mlresearch/datasets/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,21 +202,20 @@
             sampling_strategy[c] = f_new
 
         return sampling_strategy
 
     def _make_imbalance(self, data, sampling_strategy, random_state=None):
         """Undersample the minority class."""
         X_columns = [col for col in data.columns if col != "target"]
-        X, y = check_X_y(data.loc[:, X_columns], data.target)
+        X, y = check_X_y(data.loc[:, X_columns], data.target, dtype=None)
         X, y = make_imbalance(
             X, y, sampling_strategy=sampling_strategy, random_state=random_state
         )
         data = pd.DataFrame(np.column_stack((X, y)))
         data.iloc[:, -1] = data.iloc[:, -1].astype(int)
-        data.rename(columns={data.columns[-1]: "target"}, inplace=True)
         return data
 
     def download(self):
         """Download the datasets."""
         self.data_home_ = get_data_home(data_home=self.data_home)
         dataset_prefix = self.__class__.__name__.lower().replace("datasets", "")
 
@@ -272,23 +271,26 @@
 
         """
         imbalanced_content = []
         base_content = [
             dataset for dataset in self.content_ if not dataset[0].endswith(")")
         ]
         for name, data in base_content:
-            base_freqs = list(Counter(data.target).values())
+            base_freqs = Counter(data.target).values()
             base_ir = int(max(base_freqs) / min(base_freqs))
             sampling_strategy = self._calculate_sampling_strategy(
                 ir=imbalance_ratio, y=data.target
             )
             data_imb = self._make_imbalance(
                 data, sampling_strategy=sampling_strategy, random_state=random_state
             )
-            freqs = list(Counter(data_imb.target).values())
+
+            data_imb.columns = data.columns
+
+            freqs = Counter(data_imb.target).values()
             new_ir = int(max(freqs) / min(freqs))
             name_imb = f"{name} ({new_ir})"
             if name_imb not in dict(self.content_).keys() and base_ir < new_ir:
                 imbalanced_content.append((name_imb, data_imb))
 
         self.content_.extend(imbalanced_content)
         return self
@@ -308,14 +310,15 @@
         summary_columns = [
             "Dataset name",
             "Features",
             "Instances",
             "Minority instances",
             "Majority instances",
             "Imbalance Ratio",
+            "Classes",
         ]
 
         # Define empty summary table
         datasets_summary = []
 
         # Populate summary table
         for dataset_name, (X, y) in datasets:
@@ -325,22 +328,24 @@
             values = [
                 dataset_name,
                 X.shape[1],
                 len(X),
                 n_minority_instances,
                 n_majority_instances,
                 round(n_majority_instances / n_minority_instances, 2),
+                len(n_instances),
             ]
             datasets_summary.append(values)
         datasets_summary = pd.DataFrame(datasets_summary, columns=summary_columns)
 
         # Cast to integer columns
-        datasets_summary[summary_columns[1:-1]] = datasets_summary[
-            summary_columns[1:-1]
-        ].astype(int)
+        int_cols = datasets_summary.columns.drop(["Dataset name", "Imbalance Ratio"])
+        datasets_summary.loc[:, int_cols] = datasets_summary.loc[:, int_cols].astype(
+            int
+        )
 
         # Sort datasets summary
         datasets_summary = datasets_summary.sort_values("Imbalance Ratio").reset_index(
             drop=True
         )
 
         return datasets_summary
```

### Comparing `ml-research-0.4a1/mlresearch/datasets/tests/test_datasets.py` & `ml-research-0.4a2/mlresearch/datasets/tests/test_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,13 +55,13 @@
     content = datasets.content_
 
     # imbalance_datasets
     assert len(content) == len(exp_irs) + 1
     assert list(dict(content).keys()) == [name] + [f"{name} ({ir})" for ir in exp_irs]
 
     # summarize_datasets
-    assert descr.shape == (len(exp_irs) + 1, 6)
+    assert descr.shape == (len(exp_irs) + 1, 7)
     assert (descr["Features"] == N_FEATURES).all()
     assert descr["Dataset name"].tolist() == list(dict(content).keys())
     assert descr["Imbalance Ratio"].astype(int).tolist() == [
         i for i in irs if i >= base_ir
     ]
```

### Comparing `ml-research-0.4a1/mlresearch/metrics/_metrics.py` & `ml-research-0.4a2/mlresearch/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/metrics/tests/test_metrics.py` & `ml-research-0.4a2/mlresearch/metrics/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/self_supervised/_byol.py` & `ml-research-0.4a2/mlresearch/self_supervised/_byol.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/self_supervised/_components.py` & `ml-research-0.4a2/mlresearch/self_supervised/_components.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/self_supervised/_lars.py` & `ml-research-0.4a2/mlresearch/self_supervised/_lars.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/self_supervised/_simsiam.py` & `ml-research-0.4a2/mlresearch/self_supervised/_simsiam.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/self_supervised/tests/test_scheduler.py` & `ml-research-0.4a2/mlresearch/self_supervised/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/self_supervised/tests/test_ssl_models.py` & `ml-research-0.4a2/mlresearch/self_supervised/tests/test_ssl_models.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/tests/test_docstring_parameters.py` & `ml-research-0.4a2/mlresearch/tests/test_docstring_parameters.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/utils/__init__.py` & `ml-research-0.4a2/mlresearch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/utils/_check_pipelines.py` & `ml-research-0.4a2/mlresearch/utils/_check_pipelines.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/utils/_data.py` & `ml-research-0.4a2/mlresearch/utils/_data.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/utils/_testing.py` & `ml-research-0.4a2/mlresearch/utils/_testing.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/utils/_utils.py` & `ml-research-0.4a2/mlresearch/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/utils/_visualization.py` & `ml-research-0.4a2/mlresearch/utils/_visualization.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/utils/tests/test_check_pipelines.py` & `ml-research-0.4a2/mlresearch/utils/tests/test_check_pipelines.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/mlresearch/utils/tests/test_load_datasets.py` & `ml-research-0.4a2/mlresearch/utils/tests/test_load_datasets.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a1/setup.py` & `ml-research-0.4a2/setup.py`

 * *Files identical despite different names*

