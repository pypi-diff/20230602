# Comparing `tmp/mindcv-0.2.0.tar.gz` & `tmp/mindcv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindcv-0.2.0.tar", last modified: Fri Mar 31 10:58:43 2023, max compression
+gzip compressed data, was "mindcv-0.2.1.tar", last modified: Fri Jun  2 10:13:16 2023, max compression
```

## Comparing `mindcv-0.2.0.tar` & `mindcv-0.2.1.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.986560 mindcv-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-31 10:58:07.000000 mindcv-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-31 10:58:43.986560 mindcv-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-03-31 10:58:07.000000 mindcv-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.970560 mindcv-0.2.0/mindcv/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.974560 mindcv-0.2.0/mindcv/data/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/data/auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/data/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/data/dataset_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/data/dataset_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/data/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/data/transforms_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.974560 mindcv-0.2.0/mindcv/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/loss/binary_cross_entropy_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/loss/cross_entropy_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/loss/loss_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.982560 mindcv-0.2.0/mindcv/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/bit.py
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/cait.py
--rw-r--r--   0 runner    (1001) docker     (123)    30450 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/coat.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/convit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/convnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    19524 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/crossvit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/dpn.py
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/edgenext.py
--rw-r--r--   0 runner    (1001) docker     (123)    26756 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/ghostnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/googlenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    25516 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/inception_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.982560 mindcv-0.2.0/mindcv/models/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/conv_norm_act.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/selective_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/layers/squeeze_excite.py
--rw-r--r--   0 runner    (1001) docker     (123)    15007 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/mixnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/mlpmixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/mnasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/mobilenet_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    32934 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/pit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/pnasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/poolformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/pvt.py
--rw-r--r--   0 runner    (1001) docker     (123)    17938 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/pvtv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    26718 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/regnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    20406 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/repmlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/repvgg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/res2net.py
--rw-r--r--   0 runner    (1001) docker     (123)    19138 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/resnetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/rexnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/shufflenetv1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/shufflenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/sknet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/squeezenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/visformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29730 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/xception.py
--rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/models/xcit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.986560 mindcv-0.2.0/mindcv/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/optim/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/optim/nadam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/optim/optim_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.986560 mindcv-0.2.0/mindcv/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/scheduler/dynamic_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/scheduler/multi_step_decay_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/scheduler/warmup_cosine_decay_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.986560 mindcv-0.2.0/mindcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/checkpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/reduce_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/train_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/trainer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-31 10:58:07.000000 mindcv-0.2.0/mindcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:58:43.970560 mindcv-0.2.0/mindcv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-31 10:58:43.000000 mindcv-0.2.0/mindcv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-03-31 10:58:43.000000 mindcv-0.2.0/mindcv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 10:58:43.000000 mindcv-0.2.0/mindcv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 10:58:43.000000 mindcv-0.2.0/mindcv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-31 10:58:43.000000 mindcv-0.2.0/mindcv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 10:58:43.000000 mindcv-0.2.0/mindcv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-31 10:58:07.000000 mindcv-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 10:58:43.986560 mindcv-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-31 10:58:07.000000 mindcv-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.274639 mindcv-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 10:12:30.000000 mindcv-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15496 2023-06-02 10:13:16.274639 mindcv-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-06-02 10:12:30.000000 mindcv-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.254639 mindcv-0.2.1/mindcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.254639 mindcv-0.2.1/mindcv/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26775 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/dataset_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/dataset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/data/transforms_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.254639 mindcv-0.2.1/mindcv/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/loss/binary_cross_entropy_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/loss/cross_entropy_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/loss/loss_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.266639 mindcv-0.2.1/mindcv/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/bit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/cait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30524 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/coat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/convit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/crossvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/dpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/edgenext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26853 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/ghostnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/googlenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25516 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/inception_v4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.270639 mindcv-0.2.1/mindcv/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/conv_norm_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/selective_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/layers/squeeze_excite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mixnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mlpmixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mnasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mobilenet_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/mobilevit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32934 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16250 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/pit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/pnasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/poolformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/pvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/pvtv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27263 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/regnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20406 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/repmlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/repvgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/res2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19265 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/resnetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/rexnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/shufflenetv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/shufflenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/sknet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/squeezenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/visformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28992 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18630 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/models/xcit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.270639 mindcv-0.2.1/mindcv/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/optim/optim_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.270639 mindcv-0.2.1/mindcv/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/dynamic_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/multi_step_decay_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/scheduler/warmup_cosine_decay_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.274639 mindcv-0.2.1/mindcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/checkpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/reduce_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/train_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/trainer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 10:12:30.000000 mindcv-0.2.1/mindcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:13:16.254639 mindcv-0.2.1/mindcv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15496 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 10:13:16.000000 mindcv-0.2.1/mindcv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-02 10:12:30.000000 mindcv-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 10:13:16.274639 mindcv-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-02 10:12:30.000000 mindcv-0.2.1/setup.py
```

### Comparing `mindcv-0.2.0/LICENSE.md` & `mindcv-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/README.md` & `mindcv-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,238 +1,212 @@
-<div align="center">
+<div align="center" markdown>
 
 # MindCV
 
 [![CI](https://github.com/mindspore-lab/mindcv/actions/workflows/ci.yml/badge.svg)](https://github.com/mindspore-lab/mindcv/actions/workflows/ci.yml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mindcv)](https://pypi.org/project/mindcv)
 [![PyPI](https://img.shields.io/pypi/v/mindcv)](https://pypi.org/project/mindcv)
-[![docs](https://img.shields.io/badge/docs-latest-blue)](https://mindcv.readthedocs.io/en/latest)
+[![docs](https://github.com/mindspore-lab/mindcv/actions/workflows/docs.yml/badge.svg)](https://mindspore-lab.github.io/mindcv)
 [![license](https://img.shields.io/github/license/mindspore-lab/mindcv.svg)](https://github.com/mindspore-lab/mindcv/blob/main/LICENSE.md)
 [![open issues](https://img.shields.io/github/issues/mindspore-lab/mindcv)](https://github.com/mindspore-lab/mindcv/issues)
 [![PRs](https://img.shields.io/badge/PRs-welcome-pink.svg)](https://github.com/mindspore-lab/mindcv/pulls)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 English | [中文](README_CN.md)
 
 [Introduction](#introduction) |
 [Installation](#installation) |
 [Get Started](#get-started) |
 [Tutorials](#tutorials) |
 [Model List](#model-list) |
-[Supported Algorithms](#supported-algorithms) |
-[Notes](#notes)
+[Supported Algorithms](#supported-algorithms)
 
 </div>
 
 ## Introduction
+
 MindCV is an open-source toolbox for computer vision research and development based on [MindSpore](https://www.mindspore.cn/en). It collects a series of classic and SoTA vision models, such as ResNet and SwinTransformer, along with their pre-trained weights and training strategies. SoTA methods such as auto augmentation are also provided for performance improvement. With the decoupled module design, it is easy to apply or adapt MindCV to your own CV tasks.
 
-<details open>
-<summary> Major Features </summary>
+### Major Features
 
 - **Easy-to-Use.** MindCV decomposes the vision framework into various configurable components. It is easy to customize your data pipeline, models, and learning pipeline with MindCV:
 
-```python
->>> import mindcv
-# create a dataset
->>> dataset = mindcv.create_dataset('cifar10', download=True)
-# create a model
->>> network = mindcv.create_model('resnet50', pretrained=True)
-```
-
-Users can customize and launch their transfer learning or training task in one command line.
-
-``` python
-# transfer learning in one command line
->>> !python train.py --model=swin_tiny --pretrained --opt=adamw --lr=0.001 --data_dir={data_dir}
-```
+    ```pycon
+    >>> import mindcv
+    # create a dataset
+    >>> dataset = mindcv.create_dataset('cifar10', download=True)
+    # create a model
+    >>> network = mindcv.create_model('resnet50', pretrained=True)
+    ```
+
+    Users can customize and launch their transfer learning or training task in one command line.
+
+    ```shell
+    # transfer learning in one command line
+    python train.py --model=swin_tiny --pretrained --opt=adamw --lr=0.001 --data_dir=/path/to/data
+    ```
 
 - **State-of-The-Art.** MindCV provides various CNN-based and Transformer-based vision models including SwinTransformer. Their pretrained weights and performance reports are provided to help users select and reuse the right model:
 
-- **Flexibility and efficiency.** MindCV is built on MindSpore which is an efficent DL framework that can be run on different hardware platforms (GPU/CPU/Ascend). It supports both graph mode for high efficiency and pynative mode for flexibility.
-
+- **Flexibility and efficiency.** MindCV is built on MindSpore which is an efficient DL framework that can be run on different hardware platforms (GPU/CPU/Ascend). It supports both graph mode for high efficiency and pynative mode for flexibility.
 
-</details>
-
-### Benchmark Results
+## Model Zoo
 
-The performance of the models trained with MindCV is summarized in [benchmark_results.md](./benchmark_results.md), where the training recipes and weights are both available.
+The performance of the models trained with MindCV is summarized in [here](https://mindspore-lab.github.io/mindcv/modelzoo/), where the training recipes and weights are both available.
 
-Model introduction and training details can be viewed in each subfolder under [configs](configs).
+Model introduction and training details can be viewed in each sub-folder under [configs](configs).
 
 ## Installation
 
-### Dependency
-
-- mindspore >= 1.8.1
-- numpy >= 1.17.0
-- pyyaml >= 5.3
-- tqdm
-- openmpi 4.0.3 (for distributed mode)
-
-To install the dependency, please run
-```shell
-pip install -r requirements.txt
-```
-
-MindSpore can be easily installed by following the official [instructions](https://www.mindspore.cn/install) where you can select your hardware platform for the best fit. To run in distributed mode, [openmpi](https://www.open-mpi.org/software/ompi/v4.0/) is required to install.
+See [Installation](https://mindspore-lab.github.io/mindcv/installation/) for details.
 
-The following instructions assume the desired dependency is fulfilled.
-
-### Install with PyPI
-
-The released version of MindCV can be installed via `PyPI` as follows:
-```shell
-pip install mindcv
-```
-
-### Install from Source
-
-The latest version of MindCV can be installed as follows:
-```shell
-pip install git+https://github.com/mindspore-lab/mindcv.git
-```
-
-> Notes: MindCV can be installed on Linux and Mac but not on Windows currently.
-
-## Get Started
+## Getting Started
 
 ### Hands-on Tutorial
 
-To get started with MindCV, please see the [transfer learning tutorial](tutorials/finetune.md), which will give you a quick tour on each key component and the train/validate/predict pipelines.
+To get started with MindCV, please see the [Quick Start](docs/en/tutorials/quick_start.md), which will give you a quick tour on each key component and the train/validate/predict pipelines.
 
 Below are a few code snippets for your taste.
 
-```python
+```pycon
 >>> import mindcv
 # List and find a pretrained vision model
 >>> mindcv.list_models("swin*", pretrained=True)
 ['swin_tiny']
 # Create the model object
 >>> network = mindcv.create_model('swin_tiny', pretrained=True)
 # Validate its accuracy
 >>> !python validate.py --model=swin_tiny --pretrained --dataset=imagenet --val_split=validation
 {'Top_1_Accuracy': 0.808343989769821, 'Top_5_Accuracy': 0.9527253836317136, 'loss': 0.8474242982580839}
 ```
 
 **Image classification demo**
 
+Right click on the image below and save as `dog.jpg`.
+
 <p align="left">
   <img src="https://user-images.githubusercontent.com/8156835/210049681-89f68b9f-eb44-44e2-b689-4d30c93c6191.jpg" width=360 />
 </p>
 
-Infer the input image with a pretrained SoTA model,
+Classify the downloaded image with a pretrained SoTA model:
 
-```python
->>> !python infer.py --model=swin_tiny --image_path='./tutorials/data/test/dog/dog.jpg'
+```pycon
+>>> !python infer.py --model=swin_tiny --image_path='./dog.jpg'
 {'Labrador retriever': 0.5700152, 'golden retriever': 0.034551315, 'kelpie': 0.010108651, 'Chesapeake Bay retriever': 0.008229004, 'Walker hound, Walker foxhound': 0.007791956}
 ```
-The top-1 prediction result is labrador retriever (拉布拉多犬), which is the breed of this cut dog.
+The top-1 prediction result is labrador retriever, which is the breed of this cut dog.
 
 ### Training
 
 It is easy to train your model on a standard or customized dataset using `train.py`, where the training strategy (e.g., augmentation, LR scheduling) can be configured with external arguments or a yaml config file.
 
 - Standalone Training
 
-``` shell
-# standalone training
-python train.py --model=resnet50 --dataset=cifar10 --dataset_download
-```
+    ```shell
+    # standalone training
+    python train.py --model=resnet50 --dataset=cifar10 --dataset_download
+    ```
 
-Above is an example for training ResNet50 on CIFAR10 dataset on a CPU/GPU/Ascend device
+    Above is an example for training ResNet50 on CIFAR10 dataset on a CPU/GPU/Ascend device
 
 - Distributed Training
 
-For large datasets like ImageNet, it is necessary to do training in distributed mode on multiple devices. This can be achieved with `mpirun` and parallel features supported by MindSpore.
+    For large datasets like ImageNet, it is necessary to do training in distributed mode on multiple devices. This can be achieved with `mpirun` and parallel features supported by MindSpore.
 
-```shell
-# distributed training
-# assume you have 4 GPUs/NPUs
-mpirun -n 4 python train.py --distribute \
-	--model=densenet121 --dataset=imagenet --data_dir=/path/to/imagenet
-```
-> Notes: If the script is executed by the root user, the `--allow-run-as-root` parameter must be added to `mpirun`.
+    ```shell
+    # distributed training
+    # assume you have 4 GPUs/NPUs
+    mpirun -n 4 python train.py --distribute \
+        --model=densenet121 --dataset=imagenet --data_dir=/path/to/imagenet
+    ```
+    > Notes: If the script is executed by the root user, the `--allow-run-as-root` parameter must be added to `mpirun`.
 
-Detailed parameter definitions  can be seen in `config.py` and checked by running `python train.py --help'.
+    Detailed parameter definitions can be seen in `config.py` and checked by running `python train.py --help'.
 
-To resume training, please set the `--ckpt_path` and `--ckpt_save_dir` arguments. The optimizer state including the learning rate of the last stopped epoch will also be recovered.
+    To resume training, please set the `--ckpt_path` and `--ckpt_save_dir` arguments. The optimizer state including the learning rate of the last stopped epoch will also be recovered.
 
 - Config and Training Strategy
 
-You can configure your model and other components either by specifying external parameters or by writing a yaml config file. Here is an example of training using a preset yaml file.
-
-```shell
-mpirun --allow-run-as-root -n 4 python train.py -c configs/squeezenet/squeezenet_1.0_gpu.yaml
-```
+    You can configure your model and other components either by specifying external parameters or by writing a yaml config file. Here is an example of training using a preset yaml file.
 
-**Pre-defined Training Strategies:** We provide more than 20 training recipes that achieve SoTA results on ImageNet currently. Please look into the [`configs`](configs) folder for details. Please feel free to adapt these training strategies to your own model for performance improvement， which can be easily done by modifying the yaml file.
+    ```shell
+    mpirun --allow-run-as-root -n 4 python train.py -c configs/squeezenet/squeezenet_1.0_gpu.yaml
+    ```
+
+    **Pre-defined Training Strategies:**
+    We provide more than 20 training recipes that achieve SoTA results on ImageNet currently.
+    Please look into the [`configs`](configs) folder for details.
+    Please feel free to adapt these training strategies to your own model for performance improvement, which can be easily done by modifying the yaml file.
 
 - Train on ModelArts/OpenI Platform
 
-To run training on the [ModelArts](https://www.huaweicloud.com/intl/en-us/product/modelarts.html) or [OpenI](https://openi.pcl.ac.cn/) cloud platform:
+    To run training on the [ModelArts](https://www.huaweicloud.com/intl/en-us/product/modelarts.html) or [OpenI](https://openi.pcl.ac.cn/) cloud platform:
+
+    ```text
+    1. Create a new training task on the cloud platform.
+    2. Add run parameter `config` and specify the path to the yaml config file on the website UI interface.
+    3. Add run parameter `enable_modelarts` and set True on the website UI interface.
+    4. Fill in other blanks on the website and launch the training task.
+    ```
+
+**Graph Mode and PyNative Mode**:
+
+By default, the training pipeline `train.py` is run in [graph mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E9%9D%99%E6%80%81%E5%9B%BE) on MindSpore, which is optimized for efficiency and parallel computing with a compiled static graph.
+In contrast, [pynative mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E5%8A%A8%E6%80%81%E5%9B%BE) is optimized for flexibility and easy debugging. You may alter the parameter `--mode` to switch to pure pynative mode for debugging purpose.
 
-```text
-1. Create a new training task on the cloud platform.
-2. Add run parameter `config` and specify the path to the yaml config file on the website UI interface.
-3. Add run parameter `enable_modelarts` and set True on the website UI interface.
-4. Fill in other blanks on the website and launch the training task.
+**Mixed Mode**:
+
+[Pynative mode with ms_function ](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/combine.html) is a mixed mode for comprising flexibility and efficiency in MindSpore. To apply pynative mode with ms_function for training, please run `train_with_func.py`, e.g.,
+
+```shell
+python train_with_func.py --model=resnet50 --dataset=cifar10 --dataset_download  --epoch_size=10
 ```
 
+> Note: this is an **experimental** function under improvement. It is not stable on MindSpore 1.8.1 or earlier versions.
+
 ### Validation
 
-To evalute the model performance, please run `validate.py`
+To evaluate the model performance, please run `validate.py`
 
 ```shell
 # validate a trained checkpoint
 python validate.py --model=resnet50 --dataset=imagenet --data_dir=/path/to/data --ckpt_path=/path/to/model.ckpt
 ```
 
-- Validation while Training
+**Validation while Training**
 
 You can also track the validation accuracy during training by enabling the `--val_while_train` option.
 
 ```shell
 python train.py --model=resnet50 --dataset=cifar10 \
-		--val_while_train --val_split=test --val_interval=1
+    --val_while_train --val_split=test --val_interval=1
 ```
 
 The training loss and validation accuracy for each epoch  will be saved in `{ckpt_save_dir}/results.log`.
 
-More examples about training and validation can be seen in [examples/scripts](examples/scripts).
-
-- Graph Mode and Pynative Mode
-
-By default, the training pipeline `train.py` is run in [graph mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E9%9D%99%E6%80%81%E5%9B%BE) on MindSpore, which is optimized for efficiency and parallel computing with a compiled static graph. In contrast, [pynative mode](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/mode.html#%E5%8A%A8%E6%80%81%E5%9B%BE) is optimized for flexibility and easy debugging. You may alter the parameter `--mode` to switch to pure pynative mode for debugging purpose.
-
-[Pynative mode with ms_function ](https://www.mindspore.cn/tutorials/zh-CN/r1.8/advanced/pynative_graph/combine.html) is a mixed mode for comprising flexibility and efficiency in MindSpore. To apply pynative mode with ms_function for training, please run `train_with_func.py`, e.g.,
-
-``` shell
-python train_with_func.py --model=resnet50 --dataset=cifar10 --dataset_download  --epoch_size=10
-```
->Note: this is an **experimental** function under improvement. It is not stable on MindSpore 1.8.1 or earlier versions.
-
+More examples about training and validation can be seen in [examples](examples/scripts).
 
 ## Tutorials
+
 We provide the following jupyter notebook tutorials to help users learn to use MindCV.
 
-- [Learn about configs](tutorials/learn_about_config.md)
-- [Inference with a pretrained model](tutorials/inference.md)
-- [Finetune a pretrained model on custom datasets](tutorials/finetune.md)
+- [Learn about configs](docs/en/tutorials/configuration.md)
+- [Inference with a pretrained model](docs/en/tutorials/inference.md)
+- [Finetune a pretrained model on custom datasets](docs/en/tutorials/finetune.md)
 - [Customize your model]() //coming soon
 - [Optimizing performance for vision transformer]() //coming soon
-- [Deployment demo](tutorials/deployment.md)
+- [Deployment demo](docs/en/tutorials/deployment.md)
 
 ## Model List
 
 Currently, MindCV supports the model families listed below. More models with pre-trained weights are under development and will be released soon.
 
-<details open>
+<details open markdown>
 <summary> Supported models </summary>
 
 * Big Transfer ResNetV2 (BiT) - https://arxiv.org/abs/1912.11370
 * ConvNeXt - https://arxiv.org/abs/2201.03545
 * ConViT (Soft Convolutional Inductive Biases Vision Transformers)- https://arxiv.org/abs/2103.10697
 * DenseNet - https://arxiv.org/abs/1608.06993
 * DPN (Dual-Path Network) - https://arxiv.org/abs/1707.01629
@@ -268,120 +242,84 @@
 * Xception - https://arxiv.org/abs/1610.02357
 
 Please see [configs](./configs) for the details about model performance and pretrained weights.
 
 </details>
 
 ## Supported Algorithms
-<details open>
+
+<details open markdown>
 <summary> Supported algorithms </summary>
 
 * Augmentation
-	* [AutoAugment](https://arxiv.org/abs/1805.09501)
-	* [RandAugment](https://arxiv.org/abs/1909.13719)
-	* [Repeated Augmentation](https://openaccess.thecvf.com/content_CVPR_2020/papers/Hoffer_Augment_Your_Batch_Improving_Generalization_Through_Instance_Repetition_CVPR_2020_paper.pdf)
-	* RandErasing (Cutout)
-	* CutMix
-	* Mixup
-	* RandomResizeCrop
-	* Color Jitter, Flip, etc
+    * [AutoAugment](https://arxiv.org/abs/1805.09501)
+    * [RandAugment](https://arxiv.org/abs/1909.13719)
+    * [Repeated Augmentation](https://openaccess.thecvf.com/content_CVPR_2020/papers/Hoffer_Augment_Your_Batch_Improving_Generalization_Through_Instance_Repetition_CVPR_2020_paper.pdf)
+    * RandErasing (Cutout)
+    * CutMix
+    * MixUp
+    * RandomResizeCrop
+    * Color Jitter, Flip, etc
 * Optimizer
-	* Adam
-	* Adamw
-	* [Lion](https://arxiv.org/abs/2302.06675)
-	* Adan (experimental)
-	* AdaGrad
-	* LAMB
-	* Momentum
-	* RMSProp
-	* SGD
-	* NAdam
+    * Adam
+    * AdamW
+    * [Lion](https://arxiv.org/abs/2302.06675)
+    * Adan (experimental)
+    * AdaGrad
+    * LAMB
+    * Momentum
+    * RMSProp
+    * SGD
+    * NAdam
 * LR Scheduler
-	* Warmup Cosine Decay
-	* Step LR
-	* Polynomial Decay
-	* Exponential Decay
+    * Warmup Cosine Decay
+    * Step LR
+    * Polynomial Decay
+    * Exponential Decay
 * Regularization
-	* Weight Decay
-	* Label Smoothing
-	* Stochastic Depth (depends on networks)
-	* Dropout (depends on networks)
+    * Weight Decay
+    * Label Smoothing
+    * Stochastic Depth (depends on networks)
+    * Dropout (depends on networks)
 * Loss
-	* Cross Entropy (w/ class weight and auxiliary logit support)
-	* Binary Cross Entropy  (w/ class weight and auxiliary logit support)
-	* Soft Cross Entropy Loss (automatically enabled if mixup or label smoothing is used)
-	* Soft Binary Cross Entropy Loss (automatically enabled if mixup or label smoothing is used)
+    * Cross Entropy (w/ class weight and auxiliary logit support)
+    * Binary Cross Entropy  (w/ class weight and auxiliary logit support)
+    * Soft Cross Entropy Loss (automatically enabled if mixup or label smoothing is used)
+    * Soft Binary Cross Entropy Loss (automatically enabled if mixup or label smoothing is used)
 * Ensemble
-	* Warmup EMA (Exponential Moving Average)
+    * Warmup EMA (Exponential Moving Average)
+
 </details>
 
-## Notes
-### What is New
-- 2023/03/25
-1. Update checkpoints for pretrained ResNet for better accuracy
-    - ResNet18 (from 70.09 to 70.31 @Top1 accuracy)
-    - ResNet34 (from 73.69 to 74.15 @Top1 accuracy)
-    - ResNet50 (from 76.64 to 76.69 @Top1 accuracy)
-    - ResNet101 (from 77.63 to 78.24 @Top1 accuracy)
-    - ResNet152 (from 78.63 to 78.72 @Top1 accuracy)
-2. Rename checkpoint file name to follow naming rule ({model_scale-sha256sum.ckpt}) and update download URLs.
-
-- 2023/03/05
-1. Add Lion (EvoLved Sign Momentum) optimizer from paper https://arxiv.org/abs/2302.06675
-	- To replace adamw with lion, LR is usually 3-10x smaller, and weight decay is usually 3-10x larger than adamw.
-2. Add 6 new models with training recipes and pretrained weights for
-	- [HRNet](configs/hrnet)
-	- [SENet](configs/senet)
-	- [GoogLeNet](configs/googlenet)
-	- [Inception V3](configs/inception_v3)
-	- [Inception V4](configs/inception_v4)
-	- [Xception](configs/xception)
-3. Support gradient clip
-4. Arg name `use_ema` changed to **`ema`**, add `ema: True` in yaml to enable EMA.
-
-- 2023/01/10
-1. MindCV v0.1 released! It can be installed via PyPI `pip install mindcv` now.
-2. Add training recipe and trained weights of googlenet, inception_v3, inception_v4, xception
-
-- 2022/12/09
-1. Support lr warmup for all lr scheduling algorithms besides cosine decay.
-2. Add repeated augmentation, which can be enabled by setting `--aug_repeats` to be a value larger than 1 (typically, 3 or 4 is a common choice).
-3. Add EMA.
-4. Improve BCE loss to support mixup/cutmix.
-
-- 2022/11/21
-1. Add visualization for loss and acc curves
-2. Support epochwise lr warmup cosine decay (previous is stepwise)
-- 2022/11/09
-1. Add 7 pretrained ViT models.
-2. Add RandAugment augmentation.
-3. Fix CutMix efficiency issue and CutMix and Mixup can be used together.
-4. Fix lr plot and scheduling bug.
-- 2022/10/12
-1. Both BCE and CE loss now support class-weight config, label smoothing, and auxiliary logit input (for networks like inception).
-- 2022/09/13
-1. Add Adan optimizer (experimental)
+## What is New
+
+- 2023/6/2
+1. New version: `0.2.1` is released!
+2. New [documents](https://mindspore-lab.github.io/mindcv/) is online!
+
+See [RELEASE](RELEASE.md) for detailed history.
 
-### How to Contribute
+## How to Contribute
 
 We appreciate all kind of contributions including issues and PRs to make MindCV better.
 
-Please refer to [CONTRIBUTING.md](CONTRIBUTING.md) for the contributing guideline. Please follow the [Model Template and Guideline](mindcv/models/model_template.md) for contributing a model that fits the overall interface :)
+Please refer to [CONTRIBUTING.md](CONTRIBUTING.md) for the contributing guideline.
+Please follow the [Model Template and Guideline](docs/en/how_to_guides/write_a_new_model.md) for contributing a model that fits the overall interface :)
 
-### License
+## License
 
 This project follows the [Apache License 2.0](LICENSE.md) open-source license.
 
-### Acknowledgement
+## Acknowledgement
 
 MindCV is an open-source project jointly developed by the MindSpore team, Xidian University, and Xi'an Jiaotong University.
 Sincere thanks to all participating researchers and developers for their hard work on this project.
 We also acknowledge the computing resources provided by [OpenI](https://openi.pcl.ac.cn/).
 
-### Citation
+## Citation
 
 If you find this project useful in your research, please consider citing:
 
 ```latex
 @misc{MindSpore Computer Vision 2022,
     title={{MindSpore Computer  Vision}:MindSpore Computer Vision Toolbox and Benchmark},
     author={MindSpore Vision Contributors},
```

### Comparing `mindcv-0.2.0/mindcv/data/dataset_download.py` & `mindcv-0.2.1/mindcv/data/dataset_download.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/data/dataset_factory.py` & `mindcv-0.2.1/mindcv/data/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/data/distributed_sampler.py` & `mindcv-0.2.1/mindcv/data/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/data/loader.py` & `mindcv-0.2.1/mindcv/data/loader.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/data/mixup.py` & `mindcv-0.2.1/mindcv/data/mixup.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/data/transforms_factory.py` & `mindcv-0.2.1/mindcv/data/transforms_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 """
 
 import math
 
 from mindspore.dataset import vision
 from mindspore.dataset.vision import Inter
 
-from .auto_augment import auto_augment_transform, rand_augment_transform
+from .auto_augment import (
+    augment_and_mix_transform,
+    auto_augment_transform,
+    rand_augment_transform,
+    trivial_augment_wide_transform,
+)
 from .constants import DEFAULT_CROP_PCT, IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 
 __all__ = [
     "create_transforms",
 ]
 
 
@@ -61,16 +66,21 @@
         augement_params = dict(
             translate_const=int(image_resize_min * 0.45),
             img_mean=tuple([min(255, round(x)) for x in mean]),
         )
         augement_params["interpolation"] = interpolation
         if auto_augment.startswith("randaug"):
             trans_list += [rand_augment_transform(auto_augment, augement_params)]
-        elif auto_augment.startswith("autoaug") or auto_augment.startswith("autoaugr"):
+        elif auto_augment.startswith("autoaug") or auto_augment.startswith("3a"):
             trans_list += [auto_augment_transform(auto_augment, augement_params)]
+        elif auto_augment.startswith("trivialaugwide"):
+            trans_list += [trivial_augment_wide_transform(auto_augment, augement_params)]
+        elif auto_augment.startswith("augmix"):
+            augement_params["translate_pct"] = 0.3
+            trans_list += [augment_and_mix_transform(auto_augment, augement_params)]
         else:
             assert False, "Unknown auto augment policy (%s)" % auto_augment
     elif color_jitter is not None:
         if isinstance(color_jitter, (list, tuple)):
             # color jitter shoulf be a 3-tuple/list for brightness/contrast/saturation
             # or 4 if also augmenting hue
             assert len(color_jitter) in (3, 4)
@@ -164,14 +174,15 @@
     return trans
 
 
 def create_transforms(
     dataset_name="",
     image_resize=224,
     is_training=False,
+    auto_augment=None,
     **kwargs,
 ):
     r"""Creates a list of transform operation on image data.
 
     Args:
         dataset_name (str): if '', customized dataset. Currently, apply the same transform pipeline as ImageNet.
             if standard dataset name is given including imagenet, cifar10, mnist, preset transforms will be returned.
@@ -185,15 +196,15 @@
     """
 
     dataset_name = dataset_name.lower()
 
     if dataset_name in ("imagenet", ""):
         trans_args = dict(image_resize=image_resize, **kwargs)
         if is_training:
-            return transforms_imagenet_train(**trans_args)
+            return transforms_imagenet_train(auto_augment=auto_augment, **trans_args)
 
         return transforms_imagenet_eval(**trans_args)
     elif dataset_name in ("cifar10", "cifar100"):
         trans_list = transforms_cifar(resize=image_resize, is_training=is_training)
         return trans_list
     elif dataset_name == "mnist":
         trans_list = transforms_mnist(resize=image_resize)
```

### Comparing `mindcv-0.2.0/mindcv/loss/binary_cross_entropy_smooth.py` & `mindcv-0.2.1/mindcv/loss/binary_cross_entropy_smooth.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/loss/cross_entropy_smooth.py` & `mindcv-0.2.1/mindcv/loss/cross_entropy_smooth.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/loss/loss_factory.py` & `mindcv-0.2.1/mindcv/loss/loss_factory.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/__init__.py` & `mindcv-0.2.1/mindcv/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     layers,
     mixnet,
     mlpmixer,
     mnasnet,
     mobilenet_v1,
     mobilenet_v2,
     mobilenet_v3,
+    mobilevit,
     model_factory,
     nasnet,
     pit,
     pnasnet,
     poolformer,
     pvt,
     pvtv2,
@@ -68,14 +69,15 @@
 from .layers import *
 from .mixnet import *
 from .mlpmixer import *
 from .mnasnet import *
 from .mobilenet_v1 import *
 from .mobilenet_v2 import *
 from .mobilenet_v3 import *
+from .mobilevit import *
 from .model_factory import *
 from .nasnet import *
 from .pit import *
 from .pnasnet import *
 from .poolformer import *
 from .pvt import *
 from .pvtv2 import *
@@ -122,14 +124,15 @@
 __all__.extend(layers.__all__)
 __all__.extend(mixnet.__all__)
 __all__.extend(mlpmixer.__all__)
 __all__.extend(mnasnet.__all__)
 __all__.extend(mobilenet_v1.__all__)
 __all__.extend(mobilenet_v2.__all__)
 __all__.extend(mobilenet_v3.__all__)
+__all__.extend(mobilevit.__all__)
 __all__.extend(model_factory.__all__)
 __all__.extend(nasnet.__all__)
 __all__.extend(pit.__all__)
 __all__.extend(["Pnasnet", "pnasnet"])
 __all__.extend(poolformer.__all__)
 __all__.extend(pvt.__all__)
 __all__.extend(pvtv2.__all__)
```

### Comparing `mindcv-0.2.0/mindcv/models/bit.py` & `mindcv-0.2.1/mindcv/models/bit.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/cait.py` & `mindcv-0.2.1/mindcv/models/cait.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/coat.py` & `mindcv-0.2.1/mindcv/models/coat.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         'mean': (0.485, 0.456, 0.406), 'std': (0.229, 0.224, 0.225),
         'first_conv': 'patch_embed.proj', 'classifier': 'head',
         **kwargs
     }
 
 
 default_cfgs = {
-    'coat_tiny': _cfg(url=''),
+    'coat_tiny': _cfg(url='https://download.mindspore.cn/toolkits/mindcv/coat/coat_tiny-071cb792.ckpt'),
     'coat_mini': _cfg(url=''),
     'coat_small': _cfg(url=''),
     'coat_lite_tiny': _cfg(url='https://download.mindspore.cn/toolkits/mindcv/coat/coat_lite_tiny-fa7bf894.ckpt'),
     'coat_lite_mini': _cfg(url='https://download.mindspore.cn/toolkits/mindcv/coat/coat_lite_mini-55a52f05.ckpt'),
     'coat_lite_small': _cfg(url=''),
     'coat_lite_medium': _cfg(url='')
 }
```

### Comparing `mindcv-0.2.0/mindcv/models/convit.py` & `mindcv-0.2.1/mindcv/models/convit.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/convnext.py` & `mindcv-0.2.1/mindcv/models/convnext.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/crossvit.py` & `mindcv-0.2.1/mindcv/models/crossvit.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,35 @@
 from .layers.helpers import to_2tuple
 from .layers.identity import Identity
 from .layers.mlp import Mlp
 from .registry import register_model
 from .utils import load_pretrained
 
 __all__ = [
+    "crossvit9",
     "crossvit15",
     "crossvit18",
 ]
 
 
 def _cfg(url='', **kwargs):
     return {
         'url': url,
         'num_classes': 1000,
+        "input_size": (3, 224, 224),
         'first_conv': 'patch_embed.proj',
         'classifier': 'head',
         **kwargs
     }
 
 
 default_cfgs = {
+    "crossvit_9": _cfg(
+        url="https://download.mindspore.cn/toolkits/mindcv/crossvit/crossvit_9-e74c8e18.ckpt",
+        input_size=(3, 240, 240)),
     "crossvit_15": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/crossvit/crossvit_15-eaa43c02.ckpt"),
     "crossvit_18": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/crossvit/crossvit_18-ca0a2e43.ckpt"),
 }
 
 
 class Attention(nn.Cell):
     def __init__(self, dim, num_heads=8, qkv_bias=False, attn_drop=0., proj_drop=0.):
@@ -442,14 +447,26 @@
     def construct(self, x: Tensor) -> Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
 @register_model
+def crossvit9(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
+    model = VisionTransformer(img_size=[240, 224],
+                              patch_size=[12, 16], embed_dim=[128, 256], depth=[[1, 3, 0], [1, 3, 0], [1, 3, 0]],
+                              num_heads=[4, 4], mlp_ratio=[3, 3, 1], qkv_bias=True,
+                              norm_layer=nn.LayerNorm, in_channels=in_channels, num_classes=num_classes, **kwargs)
+    default_cfg = default_cfgs["crossvit_9"]
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+    return model
+
+
+@register_model
 def crossvit15(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> VisionTransformer:
     model = VisionTransformer(img_size=[240, 224],
                               patch_size=[12, 16], embed_dim=[192, 384], depth=[[1, 5, 0], [1, 5, 0], [1, 5, 0]],
                               num_heads=[6, 6], mlp_ratio=[3, 3, 1], qkv_bias=True,
                               norm_layer=nn.LayerNorm, in_channels=in_channels, num_classes=num_classes, **kwargs)
     default_cfg = default_cfgs["crossvit_15"]
     if pretrained:
```

### Comparing `mindcv-0.2.0/mindcv/models/densenet.py` & `mindcv-0.2.1/mindcv/models/densenet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/dpn.py` & `mindcv-0.2.1/mindcv/models/dpn.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/edgenext.py` & `mindcv-0.2.1/mindcv/models/edgenext.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/efficientnet.py` & `mindcv-0.2.1/mindcv/models/efficientnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
         **kwargs,
     }
 
 
 default_cfgs = {
     "efficientnet_b0": _cfg(
         url="https://download.mindspore.cn/toolkits/mindcv/efficientnet/efficientnet_b0-103ec70c.ckpt"),
-    "efficientnet_b1": _cfg(url=""),
+    "efficientnet_b1": _cfg(
+        url="https://download.mindspore.cn/toolkits/mindcv/efficientnet/efficientnet_b1-f8c6b13f.ckpt"),
     "efficientnet_b2": _cfg(url=""),
     "efficientnet_b3": _cfg(url=""),
     "efficientnet_b4": _cfg(url=""),
     "efficientnet_b5": _cfg(url=""),
     "efficientnet_b6": _cfg(url=""),
     "efficientnet_b7": _cfg(url=""),
     "efficientnet_v2_s": _cfg(url=""),
```

### Comparing `mindcv-0.2.0/mindcv/models/ghostnet.py` & `mindcv-0.2.1/mindcv/models/ghostnet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,75 @@
-"""MindSpore implementation of `GhostNet`."""
+"""MindSpore implementation of `GhostNet`.
+Refer to GhostNet: More Features from Cheap Operations.
+"""
 
 import math
 
-import numpy as np
-
+import mindspore.common.initializer as init
 from mindspore import Tensor, nn, ops
 
 from .layers.pooling import GlobalAvgPooling
 from .layers.squeeze_excite import SqueezeExcite
 from .registry import register_model
 from .utils import load_pretrained, make_divisible
 
 __all__ = [
     "GhostNet",
-    "ghostnet_1x",
-    "ghostnet_nose_1x",
+    "ghostnet_050",
+    "ghostnet_100",
+    "ghostnet_130",
 ]
 
 
 def _cfg(url="", **kwargs):
     return {
         "url": url,
         "num_classes": 1000,
         "first_conv": "conv_stem",
         "classifier": "classifier",
         **kwargs,
     }
 
 
 default_cfgs = {
-    "ghostnet_1x": _cfg(url=""),
-    "ghostnet_nose_1x": _cfg(url=""),
+    "ghostnet_050": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/ghostnet/ghostnet_050-85b91860.ckpt"),
+    "ghostnet_100": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/ghostnet/ghostnet_100-bef8025a.ckpt"),
+    "ghostnet_130": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/ghostnet/ghostnet_130-cf4c235c.ckpt"),
 }
 
 
-class GhostGate(nn.Cell):
+class HardSigmoid(nn.Cell):
     """Implementation for (relu6 + 3) / 6"""
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.relu6 = nn.ReLU6()
 
-    def construct(self, x):
-        return self.relu6(x + 3.0) * 0.16666667
+    def construct(self, x: Tensor) -> Tensor:
+        return self.relu6(x + 3.0) / 6.0
 
 
 class ConvBnAct(nn.Cell):
-    """A block for conv bn and relu"""
-
-    def __init__(self, in_chs, out_chs, kernel_size,
-                 stride=1, act_layer=nn.ReLU):
+    def __init__(
+        self,
+        in_chs: int,
+        out_chs: int,
+        kernel_size: int,
+        stride: int = 1,
+        act_layer: nn.Cell = nn.ReLU,
+    ) -> None:
         super().__init__()
-        self.conv = nn.Conv2d(in_chs, out_chs, kernel_size=kernel_size, stride=stride,
-                              padding=kernel_size // 2, pad_mode="pad", has_bias=False)
-        self.bn1 = nn.BatchNorm2d(out_chs)
-        self.act1 = act_layer()
+        self.features = nn.SequentialCell([
+            nn.Conv2d(in_chs, out_chs, kernel_size, stride, pad_mode="same"),
+            nn.BatchNorm2d(out_chs),
+            act_layer(),
+        ])
 
-    def construct(self, x):
-        x = self.conv(x)
-        x = self.bn1(x)
-        x = self.act1(x)
+    def construct(self, x: Tensor) -> Tensor:
+        x = self.features(x)
         return x
 
 
 class GhostModule(nn.Cell):
     def __init__(
         self,
         inp: int,
@@ -76,33 +82,32 @@
     ) -> None:
         super().__init__()
         self.oup = oup
         init_channels = math.ceil(oup / ratio)
         new_channels = init_channels * (ratio - 1)
 
         self.primary_conv = nn.SequentialCell(
-            nn.Conv2d(inp, init_channels, kernel_size, stride=stride,
-                      padding=kernel_size // 2, pad_mode="pad", has_bias=False),
+            nn.Conv2d(inp, init_channels, kernel_size, stride, pad_mode="pad",
+                      padding=kernel_size // 2, has_bias=False),
             nn.BatchNorm2d(init_channels),
             nn.ReLU() if relu else nn.SequentialCell(),
         )
 
         self.cheap_operation = nn.SequentialCell(
-            nn.Conv2d(init_channels, new_channels, dw_size, stride=1,
-                      padding=dw_size // 2, pad_mode="pad", group=init_channels, has_bias=False),
+            nn.Conv2d(init_channels, new_channels, dw_size, 1, pad_mode="pad",
+                      padding=dw_size // 2, group=init_channels, has_bias=False),
             nn.BatchNorm2d(new_channels),
             nn.ReLU() if relu else nn.SequentialCell(),
         )
 
     def construct(self, x: Tensor) -> Tensor:
         x1 = self.primary_conv(x)
         x2 = self.cheap_operation(x1)
         out = ops.concat((x1, x2), axis=1)
-
-        return out[:, : self.oup, :, :]
+        return out[:, :self.oup, :, :]
 
 
 class GhostBottleneck(nn.Cell):
     def __init__(
         self,
         in_chs: int,
         mid_chs: int,
@@ -117,36 +122,36 @@
 
         # Point-wise expansion
         self.ghost1 = GhostModule(in_chs, mid_chs, relu=True)
 
         # Depth-wise convolution
         if self.stride > 1:
             self.conv_dw = nn.Conv2d(mid_chs, mid_chs, dw_kernel_size, stride=stride,
-                                     padding=(dw_kernel_size - 1) // 2, pad_mode="pad",
+                                     pad_mode="pad", padding=(dw_kernel_size - 1) // 2,
                                      group=mid_chs, has_bias=False)
             self.bn_dw = nn.BatchNorm2d(mid_chs)
 
         # Squeeze-and-excitation
         if has_se:
-            self.se = SqueezeExcite(mid_chs, rd_ratio=1.0 / 4, rd_divisor=4, act_layer=nn.ReLU, gate_layer=GhostGate)
+            self.se = SqueezeExcite(mid_chs, rd_ratio=se_ratio, rd_divisor=4, gate_layer=HardSigmoid)
         else:
             self.se = None
 
         # Point-wise linear projection
         self.ghost2 = GhostModule(mid_chs, out_chs, relu=False)
 
         # shortcut
-        if in_chs == out_chs and self.stride == 1:
+        if (in_chs == out_chs and self.stride == 1):
             self.shortcut = nn.SequentialCell()
         else:
             self.shortcut = nn.SequentialCell(
-                nn.Conv2d(in_chs, in_chs, dw_kernel_size, stride=stride,
-                          pad_mode="pad", padding=(dw_kernel_size - 1) // 2, group=in_chs, has_bias=False),
+                nn.Conv2d(in_chs, in_chs, dw_kernel_size, stride=stride, pad_mode="pad",
+                          padding=(dw_kernel_size - 1) // 2, group=in_chs, has_bias=False),
                 nn.BatchNorm2d(in_chs),
-                nn.Conv2d(in_chs, out_chs, 1, stride=1, padding=0, has_bias=False),
+                nn.Conv2d(in_chs, out_chs, 1, stride=1, pad_mode="pad", padding=0, has_bias=False),
                 nn.BatchNorm2d(out_chs),
             )
 
     def construct(self, x: Tensor) -> Tensor:
         residual = x
 
         # 1st ghost bottleneck
@@ -166,194 +171,160 @@
 
         x += self.shortcut(residual)
         return x
 
 
 class GhostNet(nn.Cell):
     r"""GhostNet model class, based on
-    `"GhostNet: More Features from Cheap Operations " <https://arxiv.org/abs/1911.11907>`_
-
+    `"GhostNet: More Features from Cheap Operations " <https://arxiv.org/abs/1911.11907>`_.
     Args:
-        cfgs: the config of the GhostNet.
         num_classes: number of classification classes. Default: 1000.
+        width: base width of hidden channel in blocks. Default: 1.0.
         in_channels: number of input channels. Default: 3.
-        width: base width of hidden channel in blocks. Default: 1.0
-        droupout: the probability of the features before classification. Default: 0.2
+        drop_rate: the probability of the features before classification. Default: 0.2.
     """
 
     def __init__(
         self,
-        cfgs,
         num_classes: int = 1000,
-        in_channels: int = 3,
         width: float = 1.0,
-        dropout: float = 0.2,
+        in_channels: int = 3,
+        drop_rate: float = 0.2,
     ) -> None:
         super().__init__()
         # setting of inverted residual blocks
-        self.cfgs = cfgs
-        self.dropout_rate = dropout
+        self.num_classes = num_classes
+        self.drop_rate = drop_rate
+        self.cfgs = [
+            # k, t, c, SE, s
+            # stage1
+            [[3, 16, 16, 0, 1]],
+            # stage2
+            [[3, 48, 24, 0, 2]],
+            [[3, 72, 24, 0, 1]],
+            # stage3
+            [[5, 72, 40, 0.25, 2]],
+            [[5, 120, 40, 0.25, 1]],
+            # stage4
+            [[3, 240, 80, 0, 2]],
+            [[3, 200, 80, 0, 1],
+             [3, 184, 80, 0, 1],
+             [3, 184, 80, 0, 1],
+             [3, 480, 112, 0.25, 1],
+             [3, 672, 112, 0.25, 1]
+             ],
+            # stage5
+            [[5, 672, 160, 0.25, 2]],
+            [[5, 960, 160, 0, 1],
+             [5, 960, 160, 0.25, 1],
+             [5, 960, 160, 0, 1],
+             [5, 960, 160, 0.25, 1]
+             ]
+        ]
 
         # building first layer
-        output_channel = make_divisible(16 * width, 4)
-        self.conv_stem = nn.Conv2d(in_channels, output_channel, kernel_size=3,
-                                   padding=1, stride=2, has_bias=False, pad_mode="pad")
-        self.bn1 = nn.BatchNorm2d(output_channel)
+        stem_chs = make_divisible(16 * width, 4)
+        self.conv_stem = nn.Conv2d(in_channels, stem_chs, 3, 2, pad_mode="pad", padding=1, has_bias=False)
+        self.bn1 = nn.BatchNorm2d(stem_chs)
         self.act1 = nn.ReLU()
-        input_channel = output_channel
+        prev_chs = stem_chs
 
         # building inverted residual blocks
         stages = []
-        block = GhostBottleneck
-        exp_size = 128
         for cfg in self.cfgs:
             layers = []
             for k, exp_size, c, se_ratio, s in cfg:
-                output_channel = make_divisible(c * width, 4)
-                hidden_channel = make_divisible(exp_size * width, 4)
-                layers.append(block(input_channel, hidden_channel, output_channel, k, s, se_ratio=se_ratio))
-                input_channel = output_channel
-            stages.append(nn.SequentialCell([*layers]))
-
-        output_channel = make_divisible(exp_size * width, 4)
-        stages.append(nn.SequentialCell([ConvBnAct(input_channel, output_channel, 1)]))
-        input_channel = output_channel
+                out_chs = make_divisible(c * width, 4)
+                mid_chs = make_divisible(exp_size * width, 4)
+                layers.append(GhostBottleneck(prev_chs, mid_chs, out_chs, k, s, se_ratio=se_ratio))
+                prev_chs = out_chs
+            stages.append(nn.SequentialCell(layers))
+
+        out_chs = make_divisible(exp_size * width, 4)
+        stages.append(ConvBnAct(prev_chs, out_chs, 1))
+        prev_chs = out_chs
 
-        self.blocks = nn.SequentialCell([*stages])
+        self.blocks = nn.SequentialCell(stages)
 
         # building last several layers
-        output_channel = 1280
+        self.num_features = out_chs = 1280
         self.global_pool = GlobalAvgPooling(keep_dims=True)
-        self.conv_head = nn.Conv2d(input_channel, output_channel, kernel_size=1,
-                                   padding=0, stride=1, has_bias=True, pad_mode="pad")
+        self.conv_head = nn.Conv2d(prev_chs, out_chs, 1, 1, pad_mode="pad", padding=0, has_bias=True)
         self.act2 = nn.ReLU()
-        if self.dropout_rate > 0:
-            self.dropout = nn.Dropout(self.dropout_rate)
-        self.classifier = nn.Dense(output_channel, num_classes)
+        self.flatten = nn.Flatten()
+        if self.drop_rate > 0.0:
+            self.dropout = nn.Dropout(keep_prob=1 - drop_rate)
+        self.classifier = nn.Dense(out_chs, num_classes)
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
-        self.init_parameters_data()
-        for _, m in self.cells_and_names():
-            if isinstance(m, nn.Conv2d):
-                n = m.kernel_size[0] * m.kernel_size[1] * m.out_channels
-                m.weight.set_data(Tensor(np.random.normal(0, np.sqrt(2.0 / n), m.weight.data.shape).astype("float32")))
-                if m.bias is not None:
-                    m.bias.set_data(Tensor(np.zeros(m.bias.data.shape, dtype="float32")))
-            elif isinstance(m, nn.BatchNorm2d):
-                m.gamma.set_data(Tensor(np.ones(m.gamma.data.shape, dtype="float32")))
-                m.beta.set_data(Tensor(np.zeros(m.beta.data.shape, dtype="float32")))
-            elif isinstance(m, nn.Dense):
-                m.weight.set_data(Tensor(np.random.normal(0, 0.01, m.weight.data.shape).astype("float32")))
-                if m.bias is not None:
-                    m.bias.set_data(Tensor(np.zeros(m.bias.data.shape, dtype="float32")))
+        for _, cell in self.cells_and_names():
+            if isinstance(cell, nn.Conv2d):
+                cell.weight.set_data(init.initializer(init.HeUniform(), cell.weight.shape, cell.weight.dtype))
+                if cell.bias is not None:
+                    cell.bias.set_data(init.initializer("zeros", cell.bias.shape, cell.bias.dtype))
+            elif isinstance(cell, nn.BatchNorm2d):
+                cell.gamma.set_data(init.initializer("ones", cell.gamma.shape, cell.gamma.dtype))
+                cell.beta.set_data(init.initializer("zeros", cell.beta.shape, cell.beta.dtype))
+            elif isinstance(cell, nn.Dense):
+                cell.weight.set_data(init.initializer(init.HeUniform(), cell.weight.shape, cell.weight.dtype))
+                if cell.bias is not None:
+                    cell.bias.set_data(init.initializer("zeros", cell.bias.shape, cell.bias.dtype))
 
     def forward_features(self, x: Tensor) -> Tensor:
         x = self.conv_stem(x)
         x = self.bn1(x)
         x = self.act1(x)
         x = self.blocks(x)
-        x = self.global_pool(x)
         return x
 
     def forward_head(self, x: Tensor) -> Tensor:
+        x = self.global_pool(x)
         x = self.conv_head(x)
         x = self.act2(x)
-        x = ops.flatten(x)
-        if self.dropout_rate > 0.0:
+        x = self.flatten(x)
+        if self.drop_rate > 0.0:
             x = self.dropout(x)
         x = self.classifier(x)
         return x
 
     def construct(self, x: Tensor) -> Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
-model_cfgs = {
-    "1x": {
-        "cfg": [
-            # k, t, c, SE, s
-            # stage1
-            [[3, 16, 16, 0, 1]],
-            # stage2
-            [[3, 48, 24, 0, 2]],
-            [[3, 72, 24, 0, 1]],
-            # stage3
-            [[5, 72, 40, 0.25, 2]],
-            [[5, 120, 40, 0.25, 1]],
-            # stage4
-            [[3, 240, 80, 0, 2]],
-            [[3, 200, 80, 0, 1],
-             [3, 184, 80, 0, 1],
-             [3, 184, 80, 0, 1],
-             [3, 480, 112, 0.25, 1],
-             [3, 672, 112, 0.25, 1]],
-            # stage5
-            [[5, 672, 160, 0.25, 2]],
-            [[5, 960, 160, 0, 1],
-             [5, 960, 160, 0.25, 1],
-             [5, 960, 160, 0, 1],
-             [5, 960, 160, 0.25, 1]]
-        ],
-        "cls_ch_squeeze": 960,
-        "cls_ch_expand": 1280,
-    },
-    "nose_1x": {
-        "cfg": [
-            # k, exp, c,  se,     nl,  s,
-            # stage1
-            [[3, 16, 16, 0, 1]],
-            # stage2
-            [[3, 48, 24, 0, 2]],
-            [[3, 72, 24, 0, 1]],
-            # stage3
-            [[5, 72, 40, 0, 2]],
-            [[5, 120, 40, 0, 1]],
-            # stage4
-            [[3, 240, 80, 0, 2]],
-            [[3, 200, 80, 0, 1],
-             [3, 184, 80, 0, 1],
-             [3, 184, 80, 0, 1],
-             [3, 480, 112, 0, 1],
-             [3, 672, 112, 0, 1]],
-            # stage5
-            [[5, 672, 160, 0, 2]],
-            [[5, 960, 160, 0, 1],
-             [5, 960, 160, 0, 1],
-             [5, 960, 160, 0, 1],
-             [5, 960, 160, 0, 1]]
-        ],
-        "cls_ch_squeeze": 960,
-        "cls_ch_expand": 1280,
-    },
-}
+@register_model
+def ghostnet_050(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs):
+    """ GhostNet-0.5x """
+    default_cfg = default_cfgs["ghostnet_050"]
+    model = GhostNet(width=0.5, in_channels=in_channels, num_classes=num_classes, **kwargs)
+
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+
+    return model
 
 
 @register_model
-def ghostnet_1x(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs) -> GhostNet:
-    """Get GhostNet model.
-    Refer to the base class 'models.GhostNet' for more details.
-    """
-    model_args = model_cfgs["1x"]["cfg"]
-    model = GhostNet(cfgs=model_args, num_classes=num_classes, in_channels=in_channels, **kwargs)
+def ghostnet_100(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs):
+    """ GhostNet-1.0x """
+    default_cfg = default_cfgs["ghostnet_100"]
+    model = GhostNet(width=1.0, in_channels=in_channels, num_classes=num_classes, **kwargs)
 
     if pretrained:
-        load_pretrained(model, model_args, num_classes=num_classes, in_channels=in_channels)
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
     return model
 
 
 @register_model
-def ghostnet_nose_1x(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs) -> GhostNet:
-    """Get GhostNet model without SEModule.
-    Refer to the base class 'models.GhostNet' for more details.
-    """
-    model_args = model_cfgs["nose_1x"]["cfg"]
-    model = GhostNet(cfgs=model_args, num_classes=num_classes, in_channels=in_channels, **kwargs)
+def ghostnet_130(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs):
+    """ GhostNet-1.3x """
+    default_cfg = default_cfgs["ghostnet_130"]
+    model = GhostNet(width=1.3, in_channels=in_channels, num_classes=num_classes, **kwargs)
 
     if pretrained:
-        load_pretrained(model, model_args, num_classes=num_classes, in_channels=in_channels)
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
     return model
```

### Comparing `mindcv-0.2.0/mindcv/models/googlenet.py` & `mindcv-0.2.1/mindcv/models/googlenet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/hrnet.py` & `mindcv-0.2.1/mindcv/models/hrnet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/inception_v3.py` & `mindcv-0.2.1/mindcv/models/inception_v3.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/inception_v4.py` & `mindcv-0.2.1/mindcv/models/inception_v4.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/layers/activation.py` & `mindcv-0.2.1/mindcv/models/layers/activation.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/layers/conv_norm_act.py` & `mindcv-0.2.1/mindcv/models/layers/conv_norm_act.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/layers/drop_path.py` & `mindcv-0.2.1/mindcv/models/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/layers/mlp.py` & `mindcv-0.2.1/mindcv/models/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/layers/patch_embed.py` & `mindcv-0.2.1/mindcv/models/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/layers/selective_kernel.py` & `mindcv-0.2.1/mindcv/models/layers/selective_kernel.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/layers/squeeze_excite.py` & `mindcv-0.2.1/mindcv/models/layers/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/mixnet.py` & `mindcv-0.2.1/mindcv/models/mixnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         **kwargs,
     }
 
 
 default_cfgs = {
     "mixnet_s": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mixnet/mixnet_s-2a5ef3a3.ckpt"),
     "mixnet_m": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mixnet/mixnet_m-74cc4cb1.ckpt"),
-    "mixnet_l": _cfg(url=""),
+    "mixnet_l": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mixnet/mixnet_l-978edf2b.ckpt"),
 }
 
 
 def _roundchannels(filters: float, divisor: int = 8, min_depth: Optional[int] = None) -> int:
     if min_depth is None:
         min_depth = divisor
     new_filters = max(min_depth, int(filters + divisor / 2) // divisor * divisor)
```

### Comparing `mindcv-0.2.0/mindcv/models/mlpmixer.py` & `mindcv-0.2.1/mindcv/models/mlpmixer.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,26 +2,50 @@
 MindSpore implementation of `MLP-Mixer`.
 Refer to MLP-Mixer: An all-MLP Architecture for Vision.
 """
 
 import mindspore.nn as nn
 import mindspore.ops as ops
 
+from .registry import register_model
+from .utils import load_pretrained
+
 __all__ = [
     "MLPMixer",
     "mlp_mixer_s_p32",
     "mlp_mixer_s_p16",
     "mlp_mixer_b_p16",
     "mlp_mixer_b_p32",
     "mlp_mixer_l_p16",
     "mlp_mixer_l_p32",
     "mlp_mixer_h_p14"
 ]
 
 
+def _cfg(url="", **kwargs):
+    return {
+        "url": url,
+        "num_classes": 1000,
+        "first_conv": "to_patch_embedding.0",
+        "classifier": "mlp_head",
+        **kwargs,
+    }
+
+
+default_cfgs = {
+    "mlp_mixer_s_p16": _cfg(url=""),
+    "mlp_mixer_s_p32": _cfg(url=""),
+    "mlp_mixer_b_p16": _cfg(url=""),
+    "mlp_mixer_b_p32": _cfg(url=""),
+    "mlp_mixer_l_p16": _cfg(url=""),
+    "mlp_mixer_l_p32": _cfg(url=""),
+    "mlp_mixer_h_p14": _cfg(url=""),
+}
+
+
 class FeedForward(nn.Cell):
     """Feed Forward Block. MLP Layer. FC -> GELU -> FC"""
 
     def __init__(self, dim, hidden_dim, dropout=0.):
         super(FeedForward, self).__init__()
         self.net = nn.SequentialCell(
             nn.Dense(dim, hidden_dim),
@@ -83,31 +107,33 @@
     Args:
         depth (int) : number of MixerBlocks.
         patch_size (int or tuple) : size of a single image patch.
         n_patches (int) : number of patches.
         n_channels (int) : channels(dimension) of a single embedded patch.
         token_dim (int) : hidden dim of token-mixing MLP.
         channel_dim (int) : hidden dim of channel-mixing MLP.
-        n_classes (int) : number of classification classes.
+        num_classes (int) : number of classification classes.
+        in_channels: number the channels of the input. Default: 3.
     """
 
-    def __init__(self, depth, patch_size, n_patches, n_channels, token_dim, channel_dim, n_classes=1000):
+    def __init__(self, depth, patch_size, n_patches, n_channels, token_dim, channel_dim, num_classes=1000,
+                 in_channels=3):
         super().__init__()
         self.n_patches = n_patches
         self.n_channels = n_channels
         # patch with shape of (3, patch_size, patch_size) is embedded to n_channels dim feature.
         self.to_patch_embedding = nn.SequentialCell(
-            nn.Conv2d(3, n_channels, patch_size, patch_size, pad_mode="pad", padding=0),
+            nn.Conv2d(in_channels, n_channels, patch_size, patch_size, pad_mode="pad", padding=0),
             TransPose(permutation=(0, 2, 1), embedding=True),
         )
         self.mixer_blocks = nn.SequentialCell()
         for _ in range(depth):
             self.mixer_blocks.append(MixerBlock(n_patches, n_channels, token_dim, channel_dim))
         self.layer_norm = nn.LayerNorm((n_channels,))
-        self.mlp_head = nn.Dense(n_channels, n_classes)
+        self.mlp_head = nn.Dense(n_channels, num_classes)
         self.mean = ops.ReduceMean()
         self._initialize_weights()
 
     def construct(self, x):
         x = self.to_patch_embedding(x)
         x = self.mixer_blocks(x)
         x = self.layer_norm(x)
@@ -126,71 +152,104 @@
         assert sl == (ir // pr) ** 2, "Sequence length must be equal to ir/pr."
     elif isinstance(pr, tuple) and list(map(type, pr)) == [int, int]:
         ir = (224, 224)
         assert ir[0] % pr[0] == 0 and ir[1] % pr[1] == 0, 'Image resolution must be divisible by the patch resolution.'
         assert sl == (ir[0] // pr[0]) * (ir[1] // pr[1]), "Sequence length must be equal to ir/pr."
 
 
-def mlp_mixer_s_p32(**kwargs):
+@register_model
+def mlp_mixer_s_p32(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     # number_of_layers, patch_resolution, length_of_sequence, hidden_size, mpl_dim_sequence, mpl_dim_channel
     nl, pr, ls, hs, ds, dc = 8, 32, 49, 512, 256, 2048
     _check_resolution_and_length_of_patch(pr, ls)
-    return MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs,
-                    token_dim=ds, channel_dim=dc, **kwargs)
+    model = MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs,
+                     token_dim=ds, channel_dim=dc, num_classes=num_classes, in_channels=in_channels, **kwargs)
+
+    default_cfg = default_cfgs["mlp_mixer_s_p32"]
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
+    return model
 
-def mlp_mixer_s_p16(**kwargs):
+
+@register_model
+def mlp_mixer_s_p16(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     nl, pr, ls, hs, ds, dc = 8, 16, 196, 512, 256, 2048
     _check_resolution_and_length_of_patch(pr, ls)
-    return MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs,
-                    token_dim=ds, channel_dim=dc, **kwargs)
+    model = MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs, token_dim=ds, channel_dim=dc,
+                     num_classes=num_classes, in_channels=in_channels, **kwargs)
+
+    default_cfg = default_cfgs["mlp_mixer_s_p16"]
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
+    return model
 
-def mlp_mixer_b_p32(**kwargs):
+
+@register_model
+def mlp_mixer_b_p32(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     nl, pr, ls, hs, ds, dc = 12, 32, 49, 768, 384, 3072
     _check_resolution_and_length_of_patch(pr, ls)
-    return MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs,
-                    token_dim=ds, channel_dim=dc, **kwargs)
+    model = MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs, token_dim=ds, channel_dim=dc,
+                     num_classes=num_classes, in_channels=in_channels, **kwargs)
+
+    default_cfg = default_cfgs["mlp_mixer_b_p32"]
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
+    return model
 
-def mlp_mixer_b_p16(**kwargs):
+
+@register_model
+def mlp_mixer_b_p16(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     nl, pr, ls, hs, ds, dc = 12, 16, 196, 768, 384, 3072
     _check_resolution_and_length_of_patch(pr, ls)
-    return MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs,
-                    token_dim=ds, channel_dim=dc, **kwargs)
+    model = MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs, token_dim=ds, channel_dim=dc,
+                     num_classes=num_classes, in_channels=in_channels, **kwargs)
+
+    default_cfg = default_cfgs["mlp_mixer_b_p16"]
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
+    return model
 
-def mlp_mixer_l_p32(**kwargs):
+
+@register_model
+def mlp_mixer_l_p32(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     nl, pr, ls, hs, ds, dc = 24, 32, 49, 1024, 512, 4096
     _check_resolution_and_length_of_patch(pr, ls)
-    return MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs,
-                    token_dim=ds, channel_dim=dc, **kwargs)
+    model = MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs, token_dim=ds, channel_dim=dc,
+                     num_classes=num_classes, in_channels=in_channels, **kwargs)
+
+    default_cfg = default_cfgs["mlp_mixer_l_p32"]
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
+    return model
 
-def mlp_mixer_l_p16(**kwargs):
+
+@register_model
+def mlp_mixer_l_p16(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     nl, pr, ls, hs, ds, dc = 24, 16, 196, 1024, 512, 4096
     _check_resolution_and_length_of_patch(pr, ls)
-    return MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs,
-                    token_dim=ds, channel_dim=dc, **kwargs)
+    model = MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs, token_dim=ds, channel_dim=dc,
+                     num_classes=num_classes, in_channels=in_channels, **kwargs)
+
+    default_cfg = default_cfgs["mlp_mixer_l_p16"]
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
+    return model
 
-def mlp_mixer_h_p14(**kwargs):
+
+@register_model
+def mlp_mixer_h_p14(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
     nl, pr, ls, hs, ds, dc = 32, 14, 256, 1280, 640, 5120
     _check_resolution_and_length_of_patch(pr, ls)
-    return MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs,
-                    token_dim=ds, channel_dim=dc, **kwargs)
-
+    model = MLPMixer(depth=nl, patch_size=pr, n_patches=ls, n_channels=hs, token_dim=ds, channel_dim=dc,
+                     num_classes=num_classes, in_channels=in_channels, **kwargs)
 
-if __name__ == "__main__":
-    import numpy as np
+    default_cfg = default_cfgs["mlp_mixer_h_p14"]
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
-    import mindspore
-    from mindspore import Tensor
-
-    model = mlp_mixer_s_p16()
-    print(model)
-    parameters = model.trainable_params()
-    parameters = sum([np.prod(p.shape) for p in parameters]) / 1_000_000
-    print('Trainable Parameters: %.3fM' % parameters)
-    dummy_input = Tensor(np.random.rand(8, 3, 224, 224), dtype=mindspore.float32)
-    y = model(dummy_input)
-    print("Shape of out :", y.shape)
+    return model
```

### Comparing `mindcv-0.2.0/mindcv/models/mnasnet.py` & `mindcv-0.2.1/mindcv/models/mnasnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "first_conv": "features.0",
         "classifier": "classifier",
         **kwargs,
     }
 
 
 default_cfgs = {
-    "mnasnet0.5": _cfg(url=""),
+    "mnasnet0.5": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mnasnet/mnasnet_050-7d8bf4db.ckpt"),
     "mnasnet0.75": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mnasnet/mnasnet_075-465d366d.ckpt"),
     "mnasnet1.0": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mnasnet/mnasnet_100-1bcf43f8.ckpt"),
     "mnasnet1.3": _cfg(url=""),
     "mnasnet1.4": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/mnasnet/mnasnet_140-7e20bb30.ckpt"),
 }
```

### Comparing `mindcv-0.2.0/mindcv/models/mobilenet_v1.py` & `mindcv-0.2.1/mindcv/models/mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/mobilenet_v2.py` & `mindcv-0.2.1/mindcv/models/mobilenet_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,36 +47,36 @@
         "classifier": "classifier.1",
         **kwargs,
     }
 
 
 default_cfgs = {
     "mobilenet_v2_1.4_224": _cfg(
-        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv2/mobilenet_v2_140-015cfb04.ckpt"
+        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv2/mobilenet_v2_140-98776171.ckpt"
     ),
     "mobilenet_v2_1.3_224": _cfg(
         url=""
     ),
     "mobilenet_v2_1.0_224": _cfg(
-        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv2/mobilenet_v2_100-52122156.ckpt"
+        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv2/mobilenet_v2_100-d5532038.ckpt"
     ),
     "mobilenet_v2_1.0_192": _cfg(
         url=""
     ),
     "mobilenet_v2_1.0_160": _cfg(
         url=""
     ),
     "mobilenet_v2_1.0_128": _cfg(
         url=""
     ),
     "mobilenet_v2_1.0_96": _cfg(
         url=""
     ),
     "mobilenet_v2_0.75_224": _cfg(
-        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv2/mobilenet_v2_075-243f9404.ckpt"
+        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv2/mobilenet_v2_075-bd7bd4c4.ckpt"
     ),
     "mobilenet_v2_0.75_192": _cfg(
         url=""
     ),
     "mobilenet_v2_0.75_160": _cfg(
         url=""
     ),
```

### Comparing `mindcv-0.2.0/mindcv/models/mobilenet_v3.py` & `mindcv-0.2.1/mindcv/models/mobilenet_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,18 @@
         "classifier": "classifier.3",
         **kwargs,
     }
 
 
 default_cfgs = {
     "mobilenet_v3_small_1.0": _cfg(
-        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv3/mobilenetv3_small_100-c884b105.ckpt"
+        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv3/mobilenet_v3_small_100-509c6047.ckpt"
     ),
     "mobilenet_v3_large_1.0": _cfg(
-        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv3/mobilenet_v3_large_100-6f5bf961.ckpt"
+        url="https://download.mindspore.cn/toolkits/mindcv/mobilenet/mobilenetv3/mobilenet_v3_large_100-1279ad5f.ckpt"
     ),
     "mobilenet_v3_small_0.75": _cfg(url=""),
     "mobilenet_v3_large_0.75": _cfg(url=""),
 }
 
 
 class Bottleneck(nn.Cell):
```

### Comparing `mindcv-0.2.0/mindcv/models/model_factory.py` & `mindcv-0.2.1/mindcv/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/nasnet.py` & `mindcv-0.2.1/mindcv/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/pit.py` & `mindcv-0.2.1/mindcv/models/pit.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,18 @@
         "first_conv": "patch_embed.proj",
         "classifier": "head",
         **kwargs,
     }
 
 
 default_cfgs = {
-    "pit_ti_224": _cfg(url=""),
-    "pit_xs_224": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pit/pit_xs-fea0d37e.ckpt"),
-    "pit_s_224": _cfg(url=""),
-    "pit_b_224": _cfg(url=""),
+    "pit_ti": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pit/pit_ti-e647a593.ckpt"),
+    "pit_xs": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pit/pit_xs-fea0d37e.ckpt"),
+    "pit_s": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pit/pit_s-3c1ba36f.ckpt"),
+    "pit_b": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pit/pit_b-2411c9b6.ckpt"),
 }
 
 
 class conv_embedding(nn.Cell):
     """define embedding layer using conv2d"""
 
     def __init__(
@@ -399,15 +399,15 @@
         return cls_token
 
 
 @register_model
 def pit_ti(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs) -> PoolingTransformer:
     """Get PiT-Ti model.
     Refer to the base class `models.PoolingTransformer` for more details."""
-    default_cfg = default_cfgs["pit_ti_224"]
+    default_cfg = default_cfgs["pit_ti"]
     model = PoolingTransformer(
         image_size=224,
         patch_size=16,
         stride=8,
         base_dims=[32, 32, 32],
         depth=[2, 6, 4],
         heads=[2, 4, 8],
@@ -420,25 +420,25 @@
     if pretrained:
         load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
     return model
 
 
 @register_model
-def pit_b(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs) -> PoolingTransformer:
-    """Get PiT-B model.
+def pit_xs(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs) -> PoolingTransformer:
+    """Get PiT-XS model.
     Refer to the base class `models.PoolingTransformer` for more details."""
-    default_cfg = default_cfgs["pit_b_224"]
+    default_cfg = default_cfgs["pit_xs"]
     model = PoolingTransformer(
         image_size=224,
-        patch_size=14,
-        stride=7,
-        base_dims=[64, 64, 64],
-        depth=[3, 6, 4],
-        heads=[4, 8, 16],
+        patch_size=16,
+        stride=8,
+        base_dims=[48, 48, 48],
+        depth=[2, 6, 4],
+        heads=[2, 4, 8],
         mlp_ratio=4.0,
         num_classes=num_classes,
         in_chans=in_channels,
         **kwargs
     )
 
     if pretrained:
@@ -447,15 +447,15 @@
     return model
 
 
 @register_model
 def pit_s(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs) -> PoolingTransformer:
     """Get PiT-S model.
     Refer to the base class `models.PoolingTransformer` for more details."""
-    default_cfg = default_cfgs["pit_s_224"]
+    default_cfg = default_cfgs["pit_s"]
     model = PoolingTransformer(
         image_size=224,
         patch_size=16,
         stride=8,
         base_dims=[48, 48, 48],
         depth=[2, 6, 4],
         heads=[3, 6, 12],
@@ -468,25 +468,25 @@
     if pretrained:
         load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
 
     return model
 
 
 @register_model
-def pit_xs(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs) -> PoolingTransformer:
-    """Get PiT-XS model.
+def pit_b(pretrained: bool = False, num_classes: int = 1000, in_channels: int = 3, **kwargs) -> PoolingTransformer:
+    """Get PiT-B model.
     Refer to the base class `models.PoolingTransformer` for more details."""
-    default_cfg = default_cfgs["pit_xs_224"]
+    default_cfg = default_cfgs["pit_b"]
     model = PoolingTransformer(
         image_size=224,
-        patch_size=16,
-        stride=8,
-        base_dims=[48, 48, 48],
-        depth=[2, 6, 4],
-        heads=[2, 4, 8],
+        patch_size=14,
+        stride=7,
+        base_dims=[64, 64, 64],
+        depth=[3, 6, 4],
+        heads=[4, 8, 16],
         mlp_ratio=4.0,
         num_classes=num_classes,
         in_chans=in_channels,
         **kwargs
     )
 
     if pretrained:
```

### Comparing `mindcv-0.2.0/mindcv/models/pnasnet.py` & `mindcv-0.2.1/mindcv/models/pnasnet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/poolformer.py` & `mindcv-0.2.1/mindcv/models/poolformer.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/pvt.py` & `mindcv-0.2.1/mindcv/models/pvt.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/pvtv2.py` & `mindcv-0.2.1/mindcv/models/pvtv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     }
 
 
 default_cfgs = {
     "pvt_v2_b0": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pvt_v2/pvt_v2_b0-1c4f6683.ckpt"),
     "pvt_v2_b1": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pvt_v2/pvt_v2_b1-3ceb171a.ckpt"),
     "pvt_v2_b2": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pvt_v2/pvt_v2_b2-0565d18e.ckpt"),
-    "pvt_v2_b3": _cfg(url=""),
-    "pvt_v2_b4": _cfg(url=""),
+    "pvt_v2_b3": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pvt_v2/pvt_v2_b3-feaae3fc.ckpt"),
+    "pvt_v2_b4": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/pvt_v2/pvt_v2_b4-1cf4bc03.ckpt"),
     "pvt_v2_b5": _cfg(url=""),
 }
 
 
 class DWConv(nn.Cell):
     """Depthwise separable convolution"""
```

### Comparing `mindcv-0.2.0/mindcv/models/registry.py` & `mindcv-0.2.1/mindcv/models/registry.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/regnet.py` & `mindcv-0.2.1/mindcv/models/regnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,30 +50,30 @@
         "first_conv": "",
         "classifier": "classifier",
         **kwargs,
     }
 
 
 default_cfgs = {
-    "regnet_x_200mf": _cfg(url=""),
-    "regnet_x_400mf": _cfg(url=""),
-    "regnet_x_600mf": _cfg(url=""),
+    "regnet_x_200mf": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/regnet/regnet_x_200mf-0c2b1eb5.ckpt"),
+    "regnet_x_400mf": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/regnet/regnet_x_400mf-4848837d.ckpt"),
+    "regnet_x_600mf": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/regnet/regnet_x_600mf-ccd76c94.ckpt"),
     "regnet_x_800mf": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/regnet/regnet_x_800mf-617227f4.ckpt"),
     "regnet_x_1_6gf": _cfg(url=""),
     "regnet_x_3_2gf": _cfg(url=""),
     "regnet_x_4_0gf": _cfg(url=""),
     "regnet_x_6_4gf": _cfg(url=""),
     "regnet_x_8_0gf": _cfg(url=""),
     "regnet_x_12gf": _cfg(url=""),
     "regnet_x_16gf": _cfg(url=""),
     "regnet_x_32gf": _cfg(url=""),
-    "regnet_y_200mf": _cfg(url=""),
-    "regnet_y_400mf": _cfg(url=""),
-    "regnet_y_600mf": _cfg(url=""),
-    "regnet_y_800mf": _cfg(url=""),
+    "regnet_y_200mf": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/regnet/regnet_y_200mf-76a2f720.ckpt"),
+    "regnet_y_400mf": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/regnet/regnet_y_400mf-d496799d.ckpt"),
+    "regnet_y_600mf": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/regnet/regnet_y_600mf-a84e19b2.ckpt"),
+    "regnet_y_800mf": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/regnet/regnet_y_800mf-9b5211bd.ckpt"),
     "regnet_y_1_6gf": _cfg(url=""),
     "regnet_y_3_2gf": _cfg(url=""),
     "regnet_y_4_0gf": _cfg(url=""),
     "regnet_y_6_4gf": _cfg(url=""),
     "regnet_y_8_0gf": _cfg(url=""),
     "regnet_y_12gf": _cfg(url=""),
     "regnet_y_16gf": _cfg(url=""),
@@ -490,15 +490,14 @@
             "num_classes": num_classes,
         }
 
     def __init__(self, w_a, w_0, w_m, d, group_w, stride=2, bot_mul=1.0, stem_type="simple_stem_in", stem_w=32,
                  block_type="res_bottleneck_block", head_w=0, num_classes=1000, se_r=0.0, in_channels=3):
         params = RegNet.regnet_get_params(w_a, w_0, w_m, d, stride, bot_mul, group_w, stem_type, stem_w, block_type,
                                           head_w, num_classes, se_r)
-        print(params)
         super(RegNet, self).__init__(params["depths"], params["stem_type"], params["stem_w"], params["block_type"],
                                      params["widths"], params["strides"], params["bot_muls"], params["group_ws"],
                                      params["head_w"], params["num_classes"], params["se_r"], in_channels)
 
 
 @register_model
 def regnet_x_200mf(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs):
```

### Comparing `mindcv-0.2.0/mindcv/models/repmlp.py` & `mindcv-0.2.1/mindcv/models/repmlp.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/repvgg.py` & `mindcv-0.2.1/mindcv/models/repvgg.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     "repvgg_a0",
     "repvgg_a1",
     "repvgg_a2",
     "repvgg_b0",
     "repvgg_b1",
     "repvgg_b2",
     "repvgg_b3",
+    "repvgg_b1g2",
+    "repvgg_b1g4",
+    "repvgg_b2g4"
 ]
 
 
 def _cfg(url="", **kwargs):
     return {
         "url": url,
         "num_classes": 1000,
@@ -40,14 +43,17 @@
     "repvgg_a0": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_a0-6e71139d.ckpt"),
     "repvgg_a1": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_a1-539513ac.ckpt"),
     "repvgg_a2": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_a2-cdc90b11.ckpt"),
     "repvgg_b0": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_b0-54d5862c.ckpt"),
     "repvgg_b1": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_b1-4673797.ckpt"),
     "repvgg_b2": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_b2-7c91ccd4.ckpt"),
     "repvgg_b3": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_b3-30b35f52.ckpt"),
+    "repvgg_b1g2": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_b1g2-f0dc714f.ckpt"),
+    "repvgg_b1g4": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_b1g4-bd93230e.ckpt"),
+    "repvgg_b2g4": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/repvgg/repvgg_b2g4-e79eeadd.ckpt"),
 }
 
 
 def conv_bn(in_channels: int, out_channels: int, kernel_size: int,
             stride: int, padding: int, group: int = 1) -> nn.SequentialCell:
     cell = nn.SequentialCell([
         nn.Conv2d(in_channels=in_channels, out_channels=out_channels,
@@ -56,14 +62,15 @@
         nn.BatchNorm2d(num_features=out_channels)
     ])
     return cell
 
 
 class RepVGGBlock(nn.Cell):
     """Basic Block of RepVGG"""
+
     def __init__(self, in_channels: int, out_channels: int, kernel_size: int,
                  stride: int = 1, padding: int = 0, dilation: int = 1,
                  group: int = 1, padding_mode: str = "zeros",
                  deploy: bool = False, use_se: bool = False) -> None:
         super().__init__()
         self.deploy = deploy
         self.group = group
@@ -116,17 +123,17 @@
             ops.sqrt((self.rbr_dense.bn.moving_variance + self.rbr_dense.bn.eps)))
         t3 = ops.reshape(t3, (-1, 1, 1, 1))
 
         t1 = (self.rbr_1x1.bn.weight /
               ((self.rbr_1x1.bn.moving_variance + self.rbr_1x1.bn.eps).sqrt()))
         t1 = ops.reshape(t1, (-1, 1, 1, 1))
 
-        l2_loss_circle = ops.reduce_sum(k3**2) - ops.reduce_sum(k3[:, :, 1:2, 1:2] ** 2)
+        l2_loss_circle = ops.reduce_sum(k3 ** 2) - ops.reduce_sum(k3[:, :, 1:2, 1:2] ** 2)
         eq_kernel = k3[:, :, 1:2, 1:2] * t3 + k1 * t1
-        l2_loss_eq_kernel = ops.reduce_sum(eq_kernel**2 / (t3**2 + t1**2))
+        l2_loss_eq_kernel = ops.reduce_sum(eq_kernel ** 2 / (t3 ** 2 + t1 ** 2))
         return l2_loss_eq_kernel + l2_loss_circle
 
     #   This func derives the equivalent kernel and bias in a DIFFERENTIABLE way.
     #   You can get the equivalent kernel and bias at any time and do whatever you want,
     #   for example, apply some penalties or constraints during training, just like you do to the other models.
     #   May be useful for quantization or pruning.
     def get_equivalent_kernel_bias(self):
@@ -378,14 +385,61 @@
     if pretrained:
         load_pretrained(model, default_cfg,
                         num_classes=num_classes, in_channels=in_channels)
 
     return model
 
 
+optional_groupwise_layers = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26]
+g2_map = {g_layer: 2 for g_layer in optional_groupwise_layers}
+g4_map = {g_layer: 4 for g_layer in optional_groupwise_layers}
+
+
+@register_model
+def repvgg_b1g2(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
+    """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[2.0, 2.0, 2.0, 4.0].
+    Refer to the base class `models.RepVGG` for more details.
+    """
+    default_cfg = default_cfgs["repvgg_b1g2"]
+    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                   width_multiplier=[2.0, 2.0, 2.0, 4.0], override_group_map=g2_map, deploy=False, **kwargs)
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+
+    return model
+
+
+@register_model
+def repvgg_b1g4(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
+    """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[2.0, 2.0, 2.0, 4.0].
+    Refer to the base class `models.RepVGG` for more details.
+    """
+    default_cfg = default_cfgs["repvgg_b1g4"]
+    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                   width_multiplier=[2.0, 2.0, 2.0, 4.0], override_group_map=g4_map, deploy=False, **kwargs)
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+
+    return model
+
+
+@register_model
+def repvgg_b2g4(pretrained: bool = False, num_classes: int = 1000, in_channels=3, **kwargs) -> RepVGG:
+    """Get RepVGG model with num_blocks=[4, 6, 16, 1], width_multiplier=[2.5, 2.5, 2.5, 5.0].
+    Refer to the base class `models.RepVGG` for more details.
+    """
+    default_cfg = default_cfgs["repvgg_b2g4"]
+    model = RepVGG(num_blocks=[4, 6, 16, 1], num_classes=num_classes, in_channels=in_channels,
+                   width_multiplier=[2.5, 2.5, 2.5, 5.0], override_group_map=g4_map, deploy=False, **kwargs)
+    if pretrained:
+        load_pretrained(model, default_cfg, num_classes=num_classes, in_channels=in_channels)
+
+    return model
+
+
 def repvgg_model_convert(model: nn.Cell, save_path=None, do_copy=True):
     """repvgg_model_convert"""
     if do_copy:
         model = copy.deepcopy(model)
     for module in model.modules():
         if hasattr(module, "switch_to_deploy"):
             module.switch_to_deploy()
```

### Comparing `mindcv-0.2.0/mindcv/models/res2net.py` & `mindcv-0.2.1/mindcv/models/res2net.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/resnest.py` & `mindcv-0.2.1/mindcv/models/resnest.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     }
 
 
 default_cfgs = {
     "resnest14": _cfg(url=""),
     "resnest26": _cfg(url=""),
     "resnest50": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/resnest/resnest50-f2e7fc9c.ckpt"),
-    "resnest101": _cfg(url=""),
+    "resnest101": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/resnest/resnest101-7cc5c258.ckpt"),
     "resnest200": _cfg(url=""),
     "resnest269": _cfg(url=""),
 }
 
 
 class RadixSoftmax(nn.Cell):
     def __init__(
@@ -270,14 +270,15 @@
         # ResNet-D params
         self.inplanes = stem_width * 2 if deep_stem else 64
         self.avg_down = avg_down
         # ResNeSt params
         self.radix = radix
         self.avd = avd
         self.avd_first = avd_first
+        self.drop_rate = drop_rate
 
         if deep_stem:
             self.conv1 = nn.SequentialCell([
                 nn.Conv2d(3, stem_width, kernel_size=3, stride=2, pad_mode="pad",
                           padding=1, has_bias=False),
                 norm_layer(stem_width),
                 nn.ReLU(),
@@ -304,15 +305,15 @@
         elif dilation == 2:
             self.layer3 = self._make_layer(block, 256, layers[2], stride=2, dilation=1, norm_layer=norm_layer)
             self.layer4 = self._make_layer(block, 512, layers[3], stride=1, dilation=2, norm_layer=norm_layer)
         else:
             self.layer3 = self._make_layer(block, 256, layers[2], stride=2, norm_layer=norm_layer)
             self.layer4 = self._make_layer(block, 512, layers[3], stride=2, norm_layer=norm_layer)
         self.avgpool = GlobalAvgPooling()
-        self.drop = nn.Dropout(keep_prob=1.0 - drop_rate) if drop_rate > 0.0 else None
+        self.drop = nn.Dropout(keep_prob=1.0 - drop_rate) if self.drop_rate > 0.0 else None
         self.fc = nn.Dense(512 * block.expansion, num_classes)
 
         self._initialize_weights()
 
     def _initialize_weights(self) -> None:
         """Initialize weights for cells."""
         for _, cell in self.cells_and_names():
@@ -429,15 +430,15 @@
         x = self.layer2(x)
         x = self.layer3(x)
         x = self.layer4(x)
         return x
 
     def forward_head(self, x: Tensor) -> Tensor:
         x = self.avgpool(x)
-        if self.drop:
+        if self.drop_rate > 0:
             x = self.drop(x)
         x = self.fc(x)
         return x
 
     def construct(self, x: Tensor) -> Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
```

### Comparing `mindcv-0.2.0/mindcv/models/resnet.py` & `mindcv-0.2.1/mindcv/models/resnet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/resnetv2.py` & `mindcv-0.2.1/mindcv/models/resnetv2.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/rexnet.py` & `mindcv-0.2.1/mindcv/models/rexnet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/senet.py` & `mindcv-0.2.1/mindcv/models/senet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/shufflenetv1.py` & `mindcv-0.2.1/mindcv/models/shufflenetv1.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/shufflenetv2.py` & `mindcv-0.2.1/mindcv/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/sknet.py` & `mindcv-0.2.1/mindcv/models/sknet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/squeezenet.py` & `mindcv-0.2.1/mindcv/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/swin_transformer.py` & `mindcv-0.2.1/mindcv/models/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/utils.py` & `mindcv-0.2.1/mindcv/models/utils.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/vgg.py` & `mindcv-0.2.1/mindcv/models/vgg.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         "first_conv": "features.0",
         "classifier": "classifier.6",
         **kwargs,
     }
 
 
 default_cfgs = {
-    "vgg11": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/vgg/vgg11-59a09738.ckpt"),
-    "vgg13": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/vgg/vgg13-d30c46b7.ckpt"),
-    "vgg16": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/vgg/vgg16-22d7d708.ckpt"),
-    "vgg19": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/vgg/vgg19-0c442461.ckpt"),
+    "vgg11": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/vgg/vgg11-ef31d161.ckpt"),
+    "vgg13": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/vgg/vgg13-da805e6e.ckpt"),
+    "vgg16": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/vgg/vgg16-95697531.ckpt"),
+    "vgg19": _cfg(url="https://download.mindspore.cn/toolkits/mindcv/vgg/vgg19-bedee7b6.ckpt"),
 }
 
 
 cfgs: Dict[str, List[Union[str, int]]] = {
     "vgg11": [64, "M", 128, "M", 256, 256, "M", 512, 512, "M", 512, 512, "M"],
     "vgg13": [64, 64, "M", 128, 128, "M", 256, 256, "M", 512, 512, "M", 512, 512, "M"],
     "vgg16": [64, 64, "M", 128, 128, "M", 256, 256, 256, "M", 512, 512, 512, "M", 512, 512, 512, "M"],
```

### Comparing `mindcv-0.2.0/mindcv/models/visformer.py` & `mindcv-0.2.1/mindcv/models/visformer.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/vit.py` & `mindcv-0.2.1/mindcv/models/vit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2022 Huawei Technologies Co., Ltd
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
 """ViT"""
 from typing import List, Optional, Union
 
 import numpy as np
 
 import mindspore as ms
 from mindspore import Tensor, nn
@@ -551,16 +537,14 @@
         drop_path_keep_prob: float = 1.0,
         activation: nn.Cell = nn.GELU,
         norm: Optional[nn.Cell] = nn.LayerNorm,
         pool: str = "cls",
     ) -> None:
         super().__init__()
 
-        # Validator.check_string(pool, ["cls", "mean"], "pool type")
-
         self.patch_embedding = PatchEmbedding(image_size=image_size,
                                               patch_size=patch_size,
                                               embed_dim=embed_dim,
                                               input_channels=input_channels)
         num_patches = self.patch_embedding.num_patches
 
         if pool == "cls":
@@ -612,15 +596,15 @@
         x = self.pos_dropout(x)
         x = self.transformer(x)
         x = self.norm(x)
 
         if self.pool == "cls":
             x = x[:, 0]
         else:
-            x = self.mean(x, (1, 2))  # (1,) or (1,2)
+            x = self.mean(x, (1, ))  # (1,) or (1,2)
         return x
 
 
 def vit(
     image_size: int,
     input_channels: int,
     patch_size: int,
```

### Comparing `mindcv-0.2.0/mindcv/models/xception.py` & `mindcv-0.2.1/mindcv/models/xception.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/models/xcit.py` & `mindcv-0.2.1/mindcv/models/xcit.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 def conv3x3(in_planes, out_planes, stride=1):
     """3x3 convolution with padding"""
     return nn.SequentialCell([
         nn.Conv2d(
             in_planes, out_planes, kernel_size=3, stride=stride, padding=1, pad_mode='pad', has_bias=False
         ),
-        nn.BatchNorm2d(out_planes, use_batch_statistics=True)
+        nn.BatchNorm2d(out_planes)
     ])
 
 
 class ConvPatchEmbed(nn.Cell):
     """ Image to Patch Embedding using multiple convolutional layers
     """
 
@@ -161,15 +161,15 @@
         out_features = out_features or in_features
 
         padding = kernel_size // 2
 
         self.conv1 = nn.Conv2d(in_features, out_features, kernel_size=kernel_size,
                                padding=padding, pad_mode='pad', group=out_features, has_bias=True)
         self.act = act_layer()
-        self.bn = nn.BatchNorm2d(in_features, use_batch_statistics=True)
+        self.bn = nn.BatchNorm2d(in_features)
         self.conv2 = nn.Conv2d(in_features, out_features, kernel_size=kernel_size,
                                padding=padding, pad_mode='pad', group=out_features, has_bias=True)
 
     def construct(self, x, H, W) -> Tensor:
         B, N, C = x.shape
         x = ops.reshape(ops.transpose(x, (0, 2, 1)), (B, C, H, W))
         x = self.conv1(x)
```

### Comparing `mindcv-0.2.0/mindcv/optim/adamw.py` & `mindcv-0.2.1/mindcv/optim/adamw.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 """Gradient clipping wrapper for optimizers."""
-
 import numpy as np
 
 import mindspore as ms
 from mindspore import ops
-from mindspore._checkparam import Rel
-from mindspore._checkparam import Validator as validator
 from mindspore.common.initializer import initializer
 from mindspore.common.parameter import Parameter
 from mindspore.common.tensor import Tensor
 from mindspore.nn.optim import Optimizer
 from mindspore.nn.optim.optimizer import opt_init_args_register
 
 
 def _check_param_value(beta1, beta2, eps, prim_name):
     """Check the type of inputs."""
-    validator.check_value_type("beta1", beta1, [float], prim_name)
-    validator.check_value_type("beta2", beta2, [float], prim_name)
-    validator.check_value_type("eps", eps, [float], prim_name)
-    validator.check_float_range(beta1, 0.0, 1.0, Rel.INC_NEITHER, "beta1", prim_name)
-    validator.check_float_range(beta2, 0.0, 1.0, Rel.INC_NEITHER, "beta2", prim_name)
-    validator.check_positive_float(eps, "eps", prim_name)
+    assert isinstance(beta1, float) and 0 <= beta1 <= 1.0, f"For {prim_name}, beta1 should between 0 and 1"
+    assert isinstance(beta2, float) and 0 <= beta2 <= 1.0, f"For {prim_name}, beta2 should between 0 and 1"
+    assert isinstance(eps, float) and eps > 0, f"For {prim_name}, eps should be bigger than 0"
 
 
 _grad_scale = ops.MultitypeFuncGraph("grad_scale")
 map_ = ops.Map()
 
 
 @_grad_scale.register("Number", "Tensor")
```

### Comparing `mindcv-0.2.0/mindcv/optim/lion.py` & `mindcv-0.2.1/mindcv/optim/lion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import numpy as np
 
 import mindspore as ms
 from mindspore import ops
-from mindspore._checkparam import Rel
-from mindspore._checkparam import Validator as validator
 from mindspore.common.initializer import initializer
 from mindspore.common.parameter import Parameter
 from mindspore.common.tensor import Tensor
 from mindspore.nn.optim import Optimizer
 from mindspore.nn.optim.optimizer import opt_init_args_register
 
 
 def _check_param_value(beta1, beta2, prim_name):
     """Check the type of inputs."""
-    validator.check_value_type("beta1", beta1, [float], prim_name)
-    validator.check_value_type("beta2", beta2, [float], prim_name)
-    validator.check_float_range(beta1, 0.0, 1.0, Rel.INC_NEITHER, "beta1", prim_name)
-    validator.check_float_range(beta2, 0.0, 1.0, Rel.INC_NEITHER, "beta2", prim_name)
+    assert isinstance(beta1, float) and 0 <= beta1 <= 1.0, f"For {prim_name}, beta1 should between 0 and 1"
+    assert isinstance(beta2, float) and 0 <= beta2 <= 1.0, f"For {prim_name}, beta2 should between 0 and 1"
 
 
 _grad_scale = ops.MultitypeFuncGraph("grad_scale")
 map_ = ops.Map()
 
 
 @_grad_scale.register("Number", "Tensor")
```

### Comparing `mindcv-0.2.0/mindcv/optim/optim_factory.py` & `mindcv-0.2.1/mindcv/optim/optim_factory.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/scheduler/dynamic_lr.py` & `mindcv-0.2.1/mindcv/scheduler/dynamic_lr.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/scheduler/multi_step_decay_lr.py` & `mindcv-0.2.1/mindcv/scheduler/multi_step_decay_lr.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/scheduler/scheduler_factory.py` & `mindcv-0.2.1/mindcv/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/scheduler/warmup_cosine_decay_lr.py` & `mindcv-0.2.1/mindcv/scheduler/warmup_cosine_decay_lr.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/utils/amp.py` & `mindcv-0.2.1/mindcv/utils/amp.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/utils/callbacks.py` & `mindcv-0.2.1/mindcv/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/utils/checkpoint_manager.py` & `mindcv-0.2.1/mindcv/utils/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/utils/download.py` & `mindcv-0.2.1/mindcv/utils/download.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/utils/path.py` & `mindcv-0.2.1/mindcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/utils/train_step.py` & `mindcv-0.2.1/mindcv/utils/train_step.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/utils/trainer_factory.py` & `mindcv-0.2.1/mindcv/utils/trainer_factory.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv/utils/utils.py` & `mindcv-0.2.1/mindcv/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mindcv-0.2.0/mindcv.egg-info/SOURCES.txt` & `mindcv-0.2.1/mindcv.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 mindcv/models/inception_v4.py
 mindcv/models/mixnet.py
 mindcv/models/mlpmixer.py
 mindcv/models/mnasnet.py
 mindcv/models/mobilenet_v1.py
 mindcv/models/mobilenet_v2.py
 mindcv/models/mobilenet_v3.py
+mindcv/models/mobilevit.py
 mindcv/models/model_factory.py
 mindcv/models/nasnet.py
 mindcv/models/pit.py
 mindcv/models/pnasnet.py
 mindcv/models/poolformer.py
 mindcv/models/pvt.py
 mindcv/models/pvtv2.py
```

