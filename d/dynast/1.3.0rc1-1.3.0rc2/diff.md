# Comparing `tmp/dynast-1.3.0rc1.tar.gz` & `tmp/dynast-1.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynast-1.3.0rc1.tar", last modified: Wed May 31 22:10:22 2023, max compression
+gzip compressed data, was "dynast-1.3.0rc2.tar", last modified: Fri Jun  2 03:43:01 2023, max compression
```

## Comparing `dynast-1.3.0rc1.tar` & `dynast-1.3.0rc2.tar`

### file list

```diff
@@ -1,121 +1,116 @@
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1676 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/LICENSE.md
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13175 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/README.md
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.546404 dynast-1.3.0rc1/dynast/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/analytics/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/analytics/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3111 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/analytics/results.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10039 2023-05-31 17:20:13.000000 dynast-1.3.0rc1/dynast/analytics/visualize.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4860 2023-05-30 21:43:00.000000 dynast-1.3.0rc1/dynast/cli.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/common.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/dynast_manager.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/measure/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/measure/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/measure/latency.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/predictors/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/predictors/__init__.py
--rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6751 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/predictors/dynamic_predictor.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/predictors/predictor_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/python.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/search/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/search/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/search/encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2609 2023-05-30 21:50:38.000000 dynast-1.3.0rc1/dynast/search/evaluation_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16397 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/search/evolutionary.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41296 2023-05-30 21:43:00.000000 dynast-1.3.0rc1/dynast/search/search_tactic.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      815 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2294 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    11238 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      847 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    29037 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13827 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      912 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14923 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14561 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12721 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3638 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1178 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10456 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8793 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8312 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      887 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8399 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16147 2023-05-05 17:45:18.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4500 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      966 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4597 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24387 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      660 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1925 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3552 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9184 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4792 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6955 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2235 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    15297 2023-05-31 22:09:25.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7752 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22141 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43472 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/recommendation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/recommendation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-05-30 21:43:00.000000 dynast-1.3.0rc1/dynast/supernetwork/supernetwork_registry.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/text_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12046 2023-05-30 21:50:38.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7282 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3595 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/sst2_dataloader.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/dynast/utils/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7599 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/utils/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/utils/cache.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10458 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/utils/datasets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/utils/distributed.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6423 2023-05-18 21:41:10.000000 dynast-1.3.0rc1/dynast/utils/nn.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6734 2023-05-05 17:45:18.000000 dynast-1.3.0rc1/dynast/utils/reference.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.546404 dynast-1.3.0rc1/dynast.egg-info/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4906 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/SOURCES.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/dependency_links.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/entry_points.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      295 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/requires.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/top_level.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      361 2023-05-05 17:45:18.000000 dynast-1.3.0rc1/pyproject.toml
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/setup.cfg
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-05-31 22:10:04.000000 dynast-1.3.0rc1/setup.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/tests/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/tests/checks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/checks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2104 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/checks/check_license.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1168 2023-05-05 17:45:18.000000 dynast-1.3.0rc1/tests/checks/helpers.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/functional_reference.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1451 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_cache.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1873 2023-05-30 20:09:23.000000 dynast-1.3.0rc1/tests/test_datasets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_dynast_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      905 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_nn.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6136 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_utils.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3149 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_utils_distributed.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.427156 dynast-1.3.0rc2/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1676 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/LICENSE.md
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-06-02 03:43:01.427156 dynast-1.3.0rc2/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13175 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/README.md
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.411157 dynast-1.3.0rc2/dynast/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.411157 dynast-1.3.0rc2/dynast/analytics/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/analytics/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3111 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/analytics/results.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4596 2023-06-02 03:42:21.000000 dynast-1.3.0rc2/dynast/analytics/visualize.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4860 2023-06-02 03:42:13.000000 dynast-1.3.0rc2/dynast/cli.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/common.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/dynast_manager.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.411157 dynast-1.3.0rc2/dynast/measure/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/measure/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/measure/latency.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.411157 dynast-1.3.0rc2/dynast/predictors/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/predictors/__init__.py
+-rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6751 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/predictors/dynamic_predictor.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/predictors/predictor_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/python.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.415156 dynast-1.3.0rc2/dynast/search/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/search/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/search/encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1849 2023-06-02 03:42:21.000000 dynast-1.3.0rc2/dynast/search/evaluation_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16397 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/search/evolutionary.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41296 2023-06-02 03:42:13.000000 dynast-1.3.0rc2/dynast/search/search_tactic.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.415156 dynast-1.3.0rc2/dynast/supernetwork/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.415156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.415156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.415156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.415156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.415156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      815 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2294 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    11238 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.415156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.419156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      847 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    29037 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13827 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.419156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      912 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14923 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14561 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12721 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3638 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.419156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1178 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10456 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8793 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8312 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.419156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      887 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8399 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16147 2023-05-05 17:45:18.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4500 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.419156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      966 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4597 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24387 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.423156 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      660 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1925 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3552 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9184 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4792 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6955 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2235 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    15297 2023-06-01 18:29:08.000000 dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa_interface.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.423156 dynast-1.3.0rc2/dynast/supernetwork/machine_translation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/machine_translation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/machine_translation/modules_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7752 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/machine_translation/transformer_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22141 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/machine_translation/transformer_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43472 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/machine_translation/transformer_supernetwork.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.423156 dynast-1.3.0rc2/dynast/supernetwork/recommendation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/recommendation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-06-02 03:42:13.000000 dynast-1.3.0rc2/dynast/supernetwork/supernetwork_registry.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.423156 dynast-1.3.0rc2/dynast/supernetwork/text_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/text_classification/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/supernetwork/text_classification/bert_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12528 2023-06-01 18:51:42.000000 dynast-1.3.0rc2/dynast/supernetwork/text_classification/bert_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7282 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/text_classification/bert_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3595 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/supernetwork/text_classification/sst2_dataloader.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.427156 dynast-1.3.0rc2/dynast/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8884 2023-06-01 18:29:08.000000 dynast-1.3.0rc2/dynast/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/utils/cache.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10458 2023-05-30 18:27:20.000000 dynast-1.3.0rc2/dynast/utils/datasets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/dynast/utils/distributed.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6423 2023-05-18 21:41:10.000000 dynast-1.3.0rc2/dynast/utils/nn.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6734 2023-05-05 17:45:18.000000 dynast-1.3.0rc2/dynast/utils/reference.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.411157 dynast-1.3.0rc2/dynast.egg-info/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-06-02 03:43:01.000000 dynast-1.3.0rc2/dynast.egg-info/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4794 2023-06-02 03:43:01.000000 dynast-1.3.0rc2/dynast.egg-info/SOURCES.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-06-02 03:43:01.000000 dynast-1.3.0rc2/dynast.egg-info/dependency_links.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-06-02 03:43:01.000000 dynast-1.3.0rc2/dynast.egg-info/entry_points.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      295 2023-06-02 03:43:01.000000 dynast-1.3.0rc2/dynast.egg-info/requires.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-06-02 03:43:01.000000 dynast-1.3.0rc2/dynast.egg-info/top_level.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      361 2023-06-01 18:50:40.000000 dynast-1.3.0rc2/pyproject.toml
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-06-02 03:43:01.427156 dynast-1.3.0rc2/setup.cfg
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-06-02 03:42:29.000000 dynast-1.3.0rc2/setup.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.427156 dynast-1.3.0rc2/tests/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/tests/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-06-02 03:43:01.427156 dynast-1.3.0rc2/tests/checks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/tests/checks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2104 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/tests/checks/check_license.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1168 2023-05-05 17:45:18.000000 dynast-1.3.0rc2/tests/checks/helpers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/tests/functional_reference.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-05-01 19:25:12.000000 dynast-1.3.0rc2/tests/test_dynast_manager.py
```

### Comparing `dynast-1.3.0rc1/LICENSE.md` & `dynast-1.3.0rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/PKG-INFO` & `dynast-1.3.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.3.0rc1
+Version: 1.3.0rc2
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `dynast-1.3.0rc1/README.md` & `dynast-1.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/__init__.py` & `dynast-1.3.0rc2/dynast/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/analytics/__init__.py` & `dynast-1.3.0rc2/dynast/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/analytics/results.py` & `dynast-1.3.0rc2/dynast/analytics/results.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/cli.py` & `dynast-1.3.0rc2/dynast/cli.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/common.py` & `dynast-1.3.0rc2/dynast/common.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/dynast_manager.py` & `dynast-1.3.0rc2/dynast/dynast_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/measure/__init__.py` & `dynast-1.3.0rc2/dynast/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/measure/latency.py` & `dynast-1.3.0rc2/dynast/measure/latency.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/predictors/__init__.py` & `dynast-1.3.0rc2/dynast/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/predictors/dynamic_predictor.py` & `dynast-1.3.0rc2/dynast/predictors/dynamic_predictor.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/predictors/predictor_manager.py` & `dynast-1.3.0rc2/dynast/predictors/predictor_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/python.py` & `dynast-1.3.0rc2/dynast/python.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/search/__init__.py` & `dynast-1.3.0rc2/dynast/search/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/search/encoding.py` & `dynast-1.3.0rc2/dynast/search/encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/search/evolutionary.py` & `dynast-1.3.0rc2/dynast/search/evolutionary.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/search/search_tactic.py` & `dynast-1.3.0rc2/dynast/search/search_tactic.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py` & `dynast-1.3.0rc2/dynast/supernetwork/image_classification/ofa/ofa_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/machine_translation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py` & `dynast-1.3.0rc2/dynast/supernetwork/machine_translation/modules_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_encoding.py` & `dynast-1.3.0rc2/dynast/supernetwork/machine_translation/transformer_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_interface.py` & `dynast-1.3.0rc2/dynast/supernetwork/machine_translation/transformer_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py` & `dynast-1.3.0rc2/dynast/supernetwork/machine_translation/transformer_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/recommendation/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/supernetwork_registry.py` & `dynast-1.3.0rc2/dynast/supernetwork/supernetwork_registry.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/text_classification/__init__.py` & `dynast-1.3.0rc2/dynast/supernetwork/text_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_encoding.py` & `dynast-1.3.0rc2/dynast/supernetwork/text_classification/bert_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_interface.py` & `dynast-1.3.0rc2/dynast/supernetwork/text_classification/bert_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import copy
+import csv
 import logging
 import time
 import warnings
+from datetime import datetime
 
 import numpy as np
 import torch
 import torchprofile
 from transformers import BertConfig
 
 from dynast.search.evaluation_interface import EvaluationInterface
@@ -326,19 +328,28 @@
             if 'latency' in self.measurements:
                 individual_results['latency'], _ = self.evaluator.measure_latency(subnet_sample)
             if 'accuracy_sst2' in self.measurements:
                 individual_results['accuracy_sst2'] = self.evaluator.validate_accuracy_sst2(subnet_sample)
 
         subnet_sample = param_dict
         sample = param_dict
-
-        # self.write_results(
-        #     subnet_sample=subnet_sample,
-        # )
-        # exit()
+        # Write result for csv_path
+        if self.csv_path:
+            with open(self.csv_path, 'a') as f:
+                writer = csv.writer(f)
+                date = str(datetime.now())
+                result = [
+                    subnet_sample,
+                    date,
+                    individual_results['params'],
+                    individual_results['latency'],
+                    individual_results['macs'],
+                    individual_results['accuracy_sst2'],
+                ]
+                writer.writerow(result)
 
         # PyMoo only minimizes objectives, thus accuracy needs to be negative
         individual_results['accuracy_sst2'] = -individual_results['accuracy_sst2']
         # Return results to pymoo
         if len(self.optimization_metrics) == 1:
             return sample, individual_results[self.optimization_metrics[0]]
         elif len(self.optimization_metrics) == 2:
```

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_supernetwork.py` & `dynast-1.3.0rc2/dynast/supernetwork/text_classification/bert_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/supernetwork/text_classification/sst2_dataloader.py` & `dynast-1.3.0rc2/dynast/supernetwork/text_classification/sst2_dataloader.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/utils/__init__.py` & `dynast-1.3.0rc2/dynast/utils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools as _functools
+import importlib
 import json
 import logging
 import os
 import subprocess
 import time as _time
 from typing import List
 
@@ -244,7 +245,42 @@
 
         return metrics
 
     for key, value in kwargs.items():
         if key in ['optimization_metrics', 'measurements']:
             key = _deprecated_metric_names(value, kwargs['supernet'])
     return kwargs
+
+
+class LazyImport(object):
+    """Lazy import python module till use.
+
+    Original implementation: https://github.com/intel/neural-compressor/blob/ee049c749f0926c563683a74463354770a75afca/neural_compressor/utils/utility.py#L88
+    """
+
+    def __init__(self, module_name):
+        """Init LazyImport object.
+
+        Args:
+           module_name (string): The name of module imported later
+        """
+        self.module_name = module_name
+        self.module = None
+
+    def __getattr__(self, name):
+        """Get the attributes of the module by name."""
+        try:
+            self.module = importlib.import_module(self.module_name)
+            mod = getattr(self.module, name)
+        except:
+            spec = importlib.util.find_spec(str(self.module_name + '.' + name))
+            mod = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(mod)
+        return mod
+
+    def __call__(self, *args, **kwargs):
+        """Call the function in that module."""
+        function_name = self.module_name.split('.')[-1]
+        module_name = self.module_name.split(f'.{function_name}')[0]
+        self.module = importlib.import_module(module_name)
+        function = getattr(self.module, function_name)
+        return function(*args, **kwargs)
```

### Comparing `dynast-1.3.0rc1/dynast/utils/cache.py` & `dynast-1.3.0rc2/dynast/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/utils/datasets.py` & `dynast-1.3.0rc2/dynast/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/utils/distributed.py` & `dynast-1.3.0rc2/dynast/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/utils/nn.py` & `dynast-1.3.0rc2/dynast/utils/nn.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast/utils/reference.py` & `dynast-1.3.0rc2/dynast/utils/reference.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/dynast.egg-info/PKG-INFO` & `dynast-1.3.0rc2/dynast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.3.0rc1
+Version: 1.3.0rc2
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `dynast-1.3.0rc1/dynast.egg-info/SOURCES.txt` & `dynast-1.3.0rc2/dynast.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,11 @@
 dynast/utils/cache.py
 dynast/utils/datasets.py
 dynast/utils/distributed.py
 dynast/utils/nn.py
 dynast/utils/reference.py
 tests/__init__.py
 tests/functional_reference.py
-tests/test_cache.py
-tests/test_datasets.py
 tests/test_dynast_manager.py
-tests/test_nn.py
-tests/test_utils.py
-tests/test_utils_distributed.py
 tests/checks/__init__.py
 tests/checks/check_license.py
 tests/checks/helpers.py
```

### Comparing `dynast-1.3.0rc1/setup.py` & `dynast-1.3.0rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # import datetime
 
 from setuptools import find_packages, setup
 
 
 def get_version():
     # TODO(macsz) Replace with __version__
-    return '1.3.0rc1'
+    return '1.3.0rc2'
 
 
 def get_dependencies():
     deps = []
     with open('requirements.txt') as f:
         lines = f.readlines()
         for line in lines:
```

### Comparing `dynast-1.3.0rc1/tests/__init__.py` & `dynast-1.3.0rc2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/tests/checks/__init__.py` & `dynast-1.3.0rc2/tests/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/tests/checks/check_license.py` & `dynast-1.3.0rc2/tests/checks/check_license.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/tests/checks/helpers.py` & `dynast-1.3.0rc2/tests/checks/helpers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/tests/functional_reference.py` & `dynast-1.3.0rc2/tests/functional_reference.py`

 * *Files identical despite different names*

### Comparing `dynast-1.3.0rc1/tests/test_dynast_manager.py` & `dynast-1.3.0rc2/tests/test_dynast_manager.py`

 * *Files identical despite different names*

