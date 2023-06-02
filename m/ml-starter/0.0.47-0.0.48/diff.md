# Comparing `tmp/ml-starter-0.0.47.tar.gz` & `tmp/ml-starter-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.47.tar", last modified: Sat May 27 23:20:37 2023, max compression
+gzip compressed data, was "ml-starter-0.0.48.tar", last modified: Fri Jun  2 04:33:36 2023, max compression
```

## Comparing `ml-starter-0.0.47.tar` & `ml-starter-0.0.48.tar`

### file list

```diff
@@ -1,168 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.608633 ml-starter-0.0.47/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 23:20:26.000000 ml-starter-0.0.47/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 23:20:26.000000 ml-starter-0.0.47/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-27 23:20:37.608633 ml-starter-0.0.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-27 23:20:26.000000 ml-starter-0.0.47/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.592633 ml-starter-0.0.47/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.592633 ml-starter-0.0.47/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.592633 ml-starter-0.0.47/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.596633 ml-starter-0.0.47/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.596633 ml-starter-0.0.47/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.596633 ml-starter-0.0.47/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.596633 ml-starter-0.0.47/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.596633 ml-starter-0.0.47/ml/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    40856 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26329 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60524 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/models/pretrained/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.600633 ml-starter-0.0.47/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.600633 ml-starter-0.0.47/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.600633 ml-starter-0.0.47/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.600633 ml-starter-0.0.47/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.600633 ml-starter-0.0.47/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.600633 ml-starter-0.0.47/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.604633 ml-starter-0.0.47/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.604633 ml-starter-0.0.47/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.604633 ml-starter-0.0.47/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.604633 ml-starter-0.0.47/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.608633 ml-starter-0.0.47/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.608633 ml-starter-0.0.47/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-27 23:20:26.000000 ml-starter-0.0.47/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:20:37.608633 ml-starter-0.0.47/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-27 23:20:37.000000 ml-starter-0.0.47/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-27 23:20:37.000000 ml-starter-0.0.47/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 23:20:37.000000 ml-starter-0.0.47/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-27 23:20:37.000000 ml-starter-0.0.47/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-27 23:20:37.000000 ml-starter-0.0.47/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-27 23:20:26.000000 ml-starter-0.0.47/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-27 23:20:26.000000 ml-starter-0.0.47/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-27 23:20:26.000000 ml-starter-0.0.47/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-27 23:20:26.000000 ml-starter-0.0.47/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-27 23:20:37.608633 ml-starter-0.0.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-27 23:20:26.000000 ml-starter-0.0.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.023205 ml-starter-0.0.48/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 04:33:23.000000 ml-starter-0.0.48/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-02 04:33:23.000000 ml-starter-0.0.48/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-02 04:33:36.023205 ml-starter-0.0.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-02 04:33:23.000000 ml-starter-0.0.48/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.003205 ml-starter-0.0.48/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.003205 ml-starter-0.0.48/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.003205 ml-starter-0.0.48/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.003205 ml-starter-0.0.48/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.007205 ml-starter-0.0.48/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.007205 ml-starter-0.0.48/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.007205 ml-starter-0.0.48/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34785 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.007205 ml-starter-0.0.48/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.011205 ml-starter-0.0.48/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.011205 ml-starter-0.0.48/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.011205 ml-starter-0.0.48/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.011205 ml-starter-0.0.48/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.011205 ml-starter-0.0.48/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.015205 ml-starter-0.0.48/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.015205 ml-starter-0.0.48/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.015205 ml-starter-0.0.48/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.015205 ml-starter-0.0.48/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.019205 ml-starter-0.0.48/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.019205 ml-starter-0.0.48/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-06-02 04:33:23.000000 ml-starter-0.0.48/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:36.023205 ml-starter-0.0.48/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-02 04:33:35.000000 ml-starter-0.0.48/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-02 04:33:35.000000 ml-starter-0.0.48/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:33:35.000000 ml-starter-0.0.48/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-02 04:33:35.000000 ml-starter-0.0.48/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-02 04:33:35.000000 ml-starter-0.0.48/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-02 04:33:23.000000 ml-starter-0.0.48/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-02 04:33:23.000000 ml-starter-0.0.48/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-02 04:33:23.000000 ml-starter-0.0.48/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 04:33:23.000000 ml-starter-0.0.48/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 04:33:36.023205 ml-starter-0.0.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-02 04:33:23.000000 ml-starter-0.0.48/setup.py
```

### Comparing `ml-starter-0.0.47/LICENSE` & `ml-starter-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/PKG-INFO` & `ml-starter-0.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.47
+Version: 0.0.48
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.47/README.md` & `ml-starter-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/api.py` & `ml-starter-0.0.48/ml/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "DictIndex",
     "ensure_downloaded",
     "Environment",
     "format_timedelta",
     "from_args",
     "get_activation",
     "get_args",
+    "get_audio_props",
     "get_cache_dir",
     "get_data_dir",
     "get_dataset_split_for_phase",
     "get_dataset_splits",
     "get_distributed_backend",
     "get_eval_run_dir",
     "get_exp_name",
@@ -100,17 +101,22 @@
     "is_master",
     "launch_subprocesses",
     "LearnedPositionalEmbeddings",
     "load_model_and_task",
     "lora",
     "LoraConv1d",
     "LoraConv2d",
+    "LoraConvTranspose1d",
+    "LoraConvTranspose2d",
     "LoraEmbedding",
+    "LoraGRU",
     "LoraLinear",
+    "LoraLSTM",
     "Loss",
+    "maybe_lora",
     "meta_to_empty_func",
     "MultiIterDataset",
     "MultiprocessConfig",
     "MultiProcessLauncher",
     "MultiProcessLauncherConfig",
     "NormType",
     "open_atomic",
@@ -123,21 +129,25 @@
     "Phase",
     "pretrained_blip",
     "pretrained_clip",
     "pretrained_hubert",
     "pretrained_llama",
     "pretrained_rwkv",
     "pretrained_sam",
+    "pretrained_tacotron2_tts",
+    "pretrained_tacotron2",
+    "pretrained_vocoder",
     "PretrainedBlipKey",
     "PretrainedClipSize",
     "PretrainedHubertSize",
     "PretrainedLlamaKey",
     "PretrainedRwkvKey",
     "PretrainedSamSize",
     "project_dir_paths",
+    "read_audio",
     "read_gif",
     "read_video",
     "reduce",
     "register_logger",
     "register_lr_scheduler",
     "register_model",
     "register_optimizer",
@@ -170,14 +180,15 @@
     "test_dataset",
     "test_environment",
     "timeout",
     "Timer",
     "transforms",
     "VideoFileDataset",
     "WorkerPool",
+    "write_audio",
     "write_gif",
     "write_video",
 ]
 
 from ml.core.common_types import Batch, Loss, Output
 from ml.core.config import conf_field
 from ml.core.env import (
@@ -209,23 +220,35 @@
     LearnedPositionalEmbeddings,
     RotaryEmbeddings,
     SinusoidalEmbeddings,
     cast_embedding_kind,
     get_positional_embeddings,
 )
 from ml.models.init import InitializationType, cast_init_type, init_
-from ml.models.lora import LoraConv1d, LoraConv2d, LoraEmbedding, LoraLinear, lora
+from ml.models.lora import (
+    LoraConv1d,
+    LoraConv2d,
+    LoraConvTranspose1d,
+    LoraConvTranspose2d,
+    LoraEmbedding,
+    LoraGRU,
+    LoraLinear,
+    LoraLSTM,
+    lora,
+    maybe_lora,
+)
 from ml.models.norms import NormType, cast_norm_type, get_norm_1d, get_norm_2d, get_norm_3d, get_norm_linear
 from ml.models.parallel import ColumnParallelLinear, ParallelEmbedding, RowParallelLinear
 from ml.models.pretrained.blip import PretrainedBlipKey, pretrained_blip
 from ml.models.pretrained.clip import PretrainedClipSize, pretrained_clip
 from ml.models.pretrained.hubert import PretrainedHubertSize, pretrained_hubert
 from ml.models.pretrained.llama import PretrainedLlamaKey, pretrained_llama
 from ml.models.pretrained.rwkv import PretrainedRwkvKey, pretrained_rwkv
 from ml.models.pretrained.sam import PretrainedSamSize, pretrained_sam
+from ml.models.pretrained.tacotron2 import pretrained_tacotron2, pretrained_tacotron2_tts, pretrained_vocoder
 from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
 from ml.tasks.base import BaseTask, BaseTaskConfig
 from ml.tasks.datasets import transforms
 from ml.tasks.datasets.async_iterable import AsyncIterableDataset
 from ml.tasks.datasets.clippify import ClippifyDataset
 from ml.tasks.datasets.collate import CollateMode, collate, collate_non_null, pad_all, pad_sequence
 from ml.tasks.datasets.multi_iter import MultiIterDataset
@@ -248,14 +271,15 @@
 from ml.tasks.sl.base import SupervisedLearningTask, SupervisedLearningTaskConfig
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig
 from ml.trainers.learning import BaseLearningTrainer, BaseLearningTrainerConfig
 from ml.trainers.rl import ReinforcementLearningTrainer, ReinforcementLearningTrainerConfig
 from ml.trainers.sl import SupervisedLearningTrainer, SupervisedLearningTrainerConfig
 from ml.utils.argparse import from_args, get_args, get_type_from_string
 from ml.utils.atomic import atomic_save, open_atomic
+from ml.utils.audio import get_audio_props, read_audio, write_audio
 from ml.utils.augmentation import get_image_mask
 from ml.utils.caching import DictIndex, cached_object
 from ml.utils.checkpoint import ensure_downloaded, get_state_dict_prefix, instantiate_config, load_model_and_task
 from ml.utils.checks import assert_no_nans
 from ml.utils.colors import colorize
 from ml.utils.data import check_md5, check_sha256, get_dataset_split_for_phase, get_dataset_splits, get_worker_info
 from ml.utils.datetime import format_timedelta
```

### Comparing `ml-starter-0.0.47/ml/core/common_types.py` & `ml-starter-0.0.48/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/core/config.py` & `ml-starter-0.0.48/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/core/env.py` & `ml-starter-0.0.48/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/core/registry.py` & `ml-starter-0.0.48/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/core/state.py` & `ml-starter-0.0.48/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/launchers/base.py` & `ml-starter-0.0.48/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/launchers/mp.py` & `ml-starter-0.0.48/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/launchers/slurm.py` & `ml-starter-0.0.48/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/launchers/torchrun.py` & `ml-starter-0.0.48/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/loggers/base.py` & `ml-starter-0.0.48/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/loggers/meter.py` & `ml-starter-0.0.48/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/loggers/multi.py` & `ml-starter-0.0.48/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/loggers/stdout.py` & `ml-starter-0.0.48/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/loggers/tensorboard.py` & `ml-starter-0.0.48/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/lr_schedulers/base.py` & `ml-starter-0.0.48/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/lr_schedulers/constant.py` & `ml-starter-0.0.48/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.48/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.48/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/lr_schedulers/linear.py` & `ml-starter-0.0.48/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.48/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.48/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/models/activations.py` & `ml-starter-0.0.48/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/models/base.py` & `ml-starter-0.0.48/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/models/embeddings.py` & `ml-starter-0.0.48/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/models/init.py` & `ml-starter-0.0.48/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/models/kmeans.py` & `ml-starter-0.0.48/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/models/lora.py` & `ml-starter-0.0.48/ml/models/lora.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,23 +32,32 @@
 ``r`` parameter. The ``lora_alpha`` parameter is typically set to 1.0, but
 can be tuned to improve performance.
 """
 
 import math
 import warnings
 import weakref
-from typing import Any, TypeVar, cast, overload
+from typing import Any, TypeVar, Union, cast, overload
 
 import torch.nn.functional as F
 from torch import Tensor, nn
 from torch.nn.modules.module import _IncompatibleKeys
 
 T = TypeVar("T")
 
-SupportedModule = nn.Embedding | nn.Linear | nn.Conv1d | nn.Conv2d | nn.LSTM | nn.GRU
+SupportedModule = Union[
+    nn.Embedding,
+    nn.Linear,
+    nn.Conv1d,
+    nn.ConvTranspose1d,
+    nn.Conv2d,
+    nn.ConvTranspose2d,
+    nn.LSTM,
+    nn.GRU,
+]
 
 
 def _lora_post_hook(module: "_Lora", incompatible_keys: _IncompatibleKeys) -> None:
     lora_keys = [k for k in incompatible_keys.missing_keys if k.split(".")[-1].startswith("lora_")]
     for lora_key in lora_keys:
         incompatible_keys.missing_keys.remove(lora_key)
 
@@ -303,14 +312,117 @@
             mm = F.conv1d(mm_a, self.lora_b)
             result += mm * self.scaling
             return result
 
         return F.conv1d(x, self.weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 
+class LoraConvTranspose1d(nn.ConvTranspose1d, _Lora):
+    __constants__ = nn.ConvTranspose1d.__constants__ + ["r", "lora_alpha", "scaling", "merge", "merged"]
+
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        kernel_size: int | tuple[int],
+        r: int,
+        lora_alpha: float = 1.0,
+        lora_dropout: float = 0.0,
+        merge: bool = False,
+        stride: int | tuple[int] = 1,
+        padding: int | tuple[int] = 0,
+        output_padding: int | tuple[int] = 0,
+        dilation: int | tuple[int] = 1,
+        groups: int = 1,
+        bias: bool = True,
+    ) -> None:
+        super().__init__(
+            in_channels,
+            out_channels,
+            kernel_size,
+            stride=stride,
+            padding=padding,
+            output_padding=output_padding,
+            dilation=dilation,
+            groups=groups,
+            bias=bias,
+        )
+
+        assert r > 0
+
+        self.r = r
+        self.lora_alpha = lora_alpha
+        self.scaling = self.lora_alpha / self.r
+        self.merge = merge
+
+        self.dropout = nn.Identity() if lora_dropout == 0.0 else nn.Dropout(p=lora_dropout)
+        self.merged = False
+
+        self.lora_a = nn.Parameter(self.weight.new_empty((in_channels, r, *self.kernel_size)))
+        self.lora_b = nn.Parameter(self.weight.new_empty((r, out_channels, 1)))
+        self.weight.requires_grad = False
+
+        self.reset_parameters()
+
+    def reset_parameters(self) -> None:
+        super().reset_parameters()
+
+        if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
+            nn.init.kaiming_uniform_(self.lora_a, a=math.sqrt(5))
+            nn.init.zeros_(self.lora_b)
+
+    def train(self, mode: bool = True) -> "LoraConvTranspose1d":
+        super().train()
+
+        if mode:
+            if self.merge and self.merged:
+                # Make sure that the weights are not merged
+                if self.lora_a is not None and self.lora_b is not None:
+                    self.weight.data -= self.lora_b @ self.lora_a * self.scaling
+                self.merged = False
+
+        elif self.merge and not self.merged:
+            # Merge the weights and mark it
+            if self.lora_a is not None and self.lora_b is not None:
+                self.weight.data += self.lora_b @ self.lora_a * self.scaling
+            self.merged = True
+
+        return self
+
+    def forward(self, x: Tensor, output_size: list[int] | None = None) -> Tensor:
+        assert isinstance(self.padding, tuple)
+
+        if self.lora_a is not None and self.lora_b is not None and not self.merged:
+            result = F.conv_transpose1d(
+                x,
+                self.weight,
+                self.bias,
+                self.stride,
+                self.padding,
+                self.output_padding,
+                self.groups,
+                self.dilation,
+            )
+            mm_a = F.conv_transpose1d(
+                self.dropout(x),
+                self.lora_a,
+                None,
+                self.stride,
+                self.padding,
+                self.output_padding,
+                self.groups,
+                self.dilation,
+            )
+            mm = F.conv_transpose1d(mm_a, self.lora_b)
+            result += mm * self.scaling
+            return result
+
+        return F.conv_transpose1d(x, self.weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
+
+
 class LoraConv2d(nn.Conv2d, _Lora):
     __constants__ = nn.Conv2d.__constants__ + ["r", "lora_alpha", "scaling", "merge", "merged"]
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
@@ -384,14 +496,126 @@
             mm = F.conv2d(mm_a, self.lora_b)
             result += mm * self.scaling
             return result
 
         return F.conv2d(x, self.weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 
+class LoraConvTranspose2d(nn.ConvTranspose2d, _Lora):
+    __constants__ = nn.ConvTranspose2d.__constants__ + ["r", "lora_alpha", "scaling", "merge", "merged"]
+
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        kernel_size: int | tuple[int, int],
+        r: int,
+        lora_alpha: float = 1.0,
+        lora_dropout: float = 0.0,
+        merge: bool = False,
+        stride: int | tuple[int, int] = (1, 1),
+        padding: int | tuple[int, int] = (0, 0),
+        output_padding: int | tuple[int, int] = (0, 0),
+        dilation: int | tuple[int, int] = (1, 1),
+        groups: int = 1,
+        bias: bool = True,
+    ) -> None:
+        super().__init__(
+            in_channels,
+            out_channels,
+            kernel_size,
+            stride=stride,
+            padding=padding,
+            output_padding=output_padding,
+            dilation=dilation,
+            groups=groups,
+            bias=bias,
+        )
+
+        assert r > 0
+
+        self.r = r
+        self.lora_alpha = lora_alpha
+        self.scaling = self.lora_alpha / self.r
+        self.merge = merge
+
+        self.dropout = nn.Identity() if lora_dropout == 0.0 else nn.Dropout(p=lora_dropout)
+        self.merged = False
+
+        self.lora_a = nn.Parameter(self.weight.new_empty((in_channels, r, *self.kernel_size)))
+        self.lora_b = nn.Parameter(self.weight.new_empty((r, out_channels, 1, 1)))
+        self.weight.requires_grad = False
+
+        self.reset_parameters()
+
+    def reset_parameters(self) -> None:
+        super().reset_parameters()
+
+        if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
+            nn.init.kaiming_uniform_(self.lora_a, a=math.sqrt(5))
+            nn.init.zeros_(self.lora_b)
+
+    def train(self, mode: bool = True) -> "LoraConvTranspose2d":
+        super().train()
+
+        if mode:
+            if self.merge and self.merged:
+                # Make sure that the weights are not merged
+                if self.lora_a is not None and self.lora_b is not None:
+                    self.weight.data -= self.lora_b @ self.lora_a * self.scaling
+                self.merged = False
+
+        elif self.merge and not self.merged:
+            # Merge the weights and mark it
+            if self.lora_a is not None and self.lora_b is not None:
+                self.weight.data += self.lora_b @ self.lora_a * self.scaling
+            self.merged = True
+
+        return self
+
+    def forward(self, x: Tensor, output_size: list[int] | None = None) -> Tensor:
+        assert isinstance(self.padding, tuple)
+
+        if self.lora_a is not None and self.lora_b is not None and not self.merged:
+            result = F.conv_transpose2d(
+                x,
+                self.weight,
+                self.bias,
+                self.stride,
+                self.padding,
+                self.output_padding,
+                self.groups,
+                self.dilation,
+            )
+            mm_a = F.conv_transpose2d(
+                self.dropout(x),
+                self.lora_a,
+                None,
+                self.stride,
+                self.padding,
+                self.output_padding,
+                self.groups,
+                self.dilation,
+            )
+            mm = F.conv_transpose2d(mm_a, self.lora_b)
+            result += mm * self.scaling
+            return result
+
+        return F.conv_transpose2d(
+            x,
+            self.weight,
+            self.bias,
+            self.stride,
+            self.padding,
+            self.output_padding,
+            self.groups,
+            self.dilation,
+        )
+
+
 class _LoraRNN(nn.RNNBase, _Lora):
     __constants__ = nn.RNNBase.__constants__ + ["r", "lora_alpha", "scaling"]
 
     def __init__(
         self,
         mode: str,
         input_size: int,
@@ -563,28 +787,47 @@
 
 @overload
 def lora(module: nn.Conv1d, r: int, alpha: float = 1.0, dropout: float = 0.0, merge: bool = False) -> LoraConv1d:
     ...
 
 
 @overload
+def lora(
+    module: nn.ConvTranspose1d, r: int, alpha: float = 1.0, dropout: float = 0.0, merge: bool = False
+) -> LoraConv1d:
+    ...
+
+
+@overload
 def lora(module: nn.Conv2d, r: int, alpha: float = 1.0, dropout: float = 0.0, merge: bool = False) -> LoraConv2d:
     ...
 
 
 @overload
+def lora(
+    module: nn.ConvTranspose2d, r: int, alpha: float = 1.0, dropout: float = 0.0, merge: bool = False
+) -> LoraConv2d:
+    ...
+
+
+@overload
 def lora(module: nn.LSTM, r: int, alpha: float = 1.0, dropout: float = 0.0, merge: bool = False) -> LoraLSTM:
     ...
 
 
 @overload
 def lora(module: nn.GRU, r: int, alpha: float = 1.0, dropout: float = 0.0, merge: bool = False) -> LoraGRU:
     ...
 
 
+@overload
+def lora(module: SupportedModule, r: int, alpha: float = 1.0, dropout: float = 0.0, merge: bool = False) -> nn.Module:
+    ...
+
+
 def lora(module: SupportedModule, r: int, alpha: float = 1.0, dropout: float = 0.0, merge: bool = False) -> nn.Module:
     """Wraps a module with LoRA.
 
     This function takes a base module and returns the LoRA version of that
     module. The new module is effectively a drop-in replacement for the
     original module; for example, it can load the same state dict, and it has
     the same input and output shapes.
@@ -645,44 +888,86 @@
             module.out_channels,
             cast(tuple[int], module.kernel_size),
             r=r,
             lora_alpha=alpha,
             lora_dropout=dropout,
             merge=merge,
             stride=cast(tuple[int], module.stride),
-            padding=cast(tuple[int], module.padding),
+            padding=cast(str | tuple[int], module.padding),
             dilation=cast(tuple[int], module.dilation),
             groups=module.groups,
             bias=module.bias is not None,
         )
         conv_1d.weight.data.copy_(module.weight.data)
         if module.bias is not None and conv_1d.bias is not None:
             conv_1d.bias.data.copy_(module.bias.data)
         return conv_1d
 
+    if isinstance(module, nn.ConvTranspose1d):
+        conv_transpose_1d = LoraConvTranspose1d(
+            module.in_channels,
+            module.out_channels,
+            cast(tuple[int], module.kernel_size),
+            r=r,
+            lora_alpha=alpha,
+            lora_dropout=dropout,
+            merge=merge,
+            stride=cast(tuple[int], module.stride),
+            padding=cast(tuple[int], module.padding),
+            output_padding=cast(tuple[int], module.output_padding),
+            dilation=cast(tuple[int], module.dilation),
+            groups=module.groups,
+            bias=module.bias is not None,
+        )
+        conv_transpose_1d.weight.data.copy_(module.weight.data)
+        if module.bias is not None and conv_transpose_1d.bias is not None:
+            conv_transpose_1d.bias.data.copy_(module.bias.data)
+        return conv_transpose_1d
+
     if isinstance(module, nn.Conv2d):
         conv_2d = LoraConv2d(
             module.in_channels,
             module.out_channels,
             cast(tuple[int, int], module.kernel_size),
             r=r,
             lora_alpha=alpha,
             lora_dropout=dropout,
             merge=merge,
             stride=cast(tuple[int, int], module.stride),
-            padding=cast(tuple[int, int], module.padding),
+            padding=cast(str | tuple[int, int], module.padding),
             dilation=cast(tuple[int, int], module.dilation),
             groups=module.groups,
             bias=module.bias is not None,
         )
         conv_2d.weight.data.copy_(module.weight.data)
         if module.bias is not None and conv_2d.bias is not None:
             conv_2d.bias.data.copy_(module.bias.data)
         return conv_2d
 
+    if isinstance(module, nn.ConvTranspose2d):
+        conv_transpose_2d = LoraConvTranspose2d(
+            module.in_channels,
+            module.out_channels,
+            cast(tuple[int, int], module.kernel_size),
+            r=r,
+            lora_alpha=alpha,
+            lora_dropout=dropout,
+            merge=merge,
+            stride=cast(tuple[int, int], module.stride),
+            padding=cast(tuple[int, int], module.padding),
+            output_padding=cast(tuple[int, int], module.output_padding),
+            dilation=cast(tuple[int, int], module.dilation),
+            groups=module.groups,
+            bias=module.bias is not None,
+        )
+        conv_transpose_2d.weight.data.copy_(module.weight.data)
+        if module.bias is not None and conv_transpose_2d.bias is not None:
+            conv_transpose_2d.bias.data.copy_(module.bias.data)
+        return conv_transpose_2d
+
     if isinstance(module, nn.LSTM):
         if dropout > 0.0:
             warnings.warn("LoRA dropout is not supported for LSTMs")
 
         lstm = LoraLSTM(
             module.input_size,
             module.hidden_size,
@@ -716,7 +1001,20 @@
             proj_size=module.proj_size,
         )
         for param_name, param_value in module.named_parameters():
             getattr(gru, param_name).data.copy_(param_value.data)
         return gru
 
     raise ValueError(f"Unsupported module type {type(module)}")
+
+
+T_module = TypeVar("T_module", bound=SupportedModule)
+
+
+def maybe_lora(
+    module: T_module,
+    r: int | None,
+    alpha: float = 1.0,
+    dropout: float = 0.0,
+    merge: bool = False,
+) -> T_module:
+    return module if r is None else lora(module, r, alpha, dropout, merge)
```

### Comparing `ml-starter-0.0.47/ml/models/norms.py` & `ml-starter-0.0.48/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/models/parallel.py` & `ml-starter-0.0.48/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/optimizers/adam.py` & `ml-starter-0.0.48/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/optimizers/adamw.py` & `ml-starter-0.0.48/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/optimizers/adan.py` & `ml-starter-0.0.48/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/optimizers/base.py` & `ml-starter-0.0.48/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/optimizers/common.py` & `ml-starter-0.0.48/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/optimizers/sgd.py` & `ml-starter-0.0.48/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/optimizers/shampoo.py` & `ml-starter-0.0.48/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/scripts/cli.py` & `ml-starter-0.0.48/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/scripts/stage.py` & `ml-starter-0.0.48/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/scripts/train.py` & `ml-starter-0.0.48/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/base.py` & `ml-starter-0.0.48/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.48/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.48/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/collate.py` & `ml-starter-0.0.48/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.48/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.48/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.48/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.48/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.48/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/utils.py` & `ml-starter-0.0.48/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.48/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/environments/base.py` & `ml-starter-0.0.48/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/environments/utils.py` & `ml-starter-0.0.48/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/environments/worker.py` & `ml-starter-0.0.48/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/losses/reduce.py` & `ml-starter-0.0.48/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/rl/base.py` & `ml-starter-0.0.48/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/rl/replay.py` & `ml-starter-0.0.48/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/tasks/sl/base.py` & `ml-starter-0.0.48/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/base.py` & `ml-starter-0.0.48/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/learning.py` & `ml-starter-0.0.48/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/compile.py` & `ml-starter-0.0.48/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.48/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.48/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.48/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.48/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.48/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.48/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.48/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.48/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.48/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/rl.py` & `ml-starter-0.0.48/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/trainers/sl.py` & `ml-starter-0.0.48/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/argparse.py` & `ml-starter-0.0.48/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/atomic.py` & `ml-starter-0.0.48/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/augmentation.py` & `ml-starter-0.0.48/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/caching.py` & `ml-starter-0.0.48/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/checkpoint.py` & `ml-starter-0.0.48/ml/utils/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 These functions can be used to load a model from an arbitrary config file
 and checkpoint. Note that there might be some issues if you move the checkpoint
 around places.
 """
 
 import logging
+import tempfile
 from pathlib import Path
 from typing import Mapping, TypeVar, cast
 
 import torch
 from omegaconf import DictConfig, OmegaConf
 from torchvision.datasets.utils import download_url
 
@@ -167,15 +168,15 @@
         sha256: The SHA256 hash of the file, if known.
         is_tmp: If set, use ``tmp/`` instead of ``get_model_dir()``
 
     Returns:
         The path to the downloaded file.
     """
     assert len(dnames) >= 1, "Must provide at least 1 directory name"
-    filepath = Path("tmp") if is_tmp else get_model_dir()
+    filepath = Path(tempfile.mkdtemp("models")) if is_tmp else get_model_dir()
     for dname in dnames:
         filepath = filepath / dname
     (root := filepath.parent).mkdir(parents=True, exist_ok=True)
     if not filepath.exists() or not check_sha256(filepath, sha256) or not check_md5(filepath, md5):
         download_url(url, root=root, filename=filepath.name, md5=md5)
         assert filepath.is_file(), f"Failed to download {url} to {filepath}"
     return filepath
```

### Comparing `ml-starter-0.0.47/ml/utils/cli.py` & `ml-starter-0.0.48/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/colors.py` & `ml-starter-0.0.48/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/config.py` & `ml-starter-0.0.48/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/data.py` & `ml-starter-0.0.48/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/datetime.py` & `ml-starter-0.0.48/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/device/auto.py` & `ml-starter-0.0.48/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/device/base.py` & `ml-starter-0.0.48/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/device/cpu.py` & `ml-starter-0.0.48/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/device/gpu.py` & `ml-starter-0.0.48/ml/utils/device/gpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,21 +39,18 @@
 
     @classmethod
     def get_floating_point_type(cls) -> torch.dtype:
         use_bf16 = get_env_bool("USE_BF16")
         use_fp32 = get_env_bool("USE_FP32")
         use_fp64 = get_env_bool("USE_FP64")
         if use_fp64:
-            logger.info("Using FP64")
             return torch.float64
         elif use_fp32:
-            logger.info("Using FP32")
             return torch.float32
         elif use_bf16:
-            logger.info("Using BF16")
             return torch.bfloat16
         else:
             return torch.float16
 
     @classmethod
     def get_torch_compile_backend(cls) -> str | Callable:
         capability = torch.cuda.get_device_capability()
```

### Comparing `ml-starter-0.0.47/ml/utils/device/metal.py` & `ml-starter-0.0.48/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/distributed.py` & `ml-starter-0.0.48/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/image.py` & `ml-starter-0.0.48/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/large_models.py` & `ml-starter-0.0.48/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/logging.py` & `ml-starter-0.0.48/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/meter.py` & `ml-starter-0.0.48/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/parallel.py` & `ml-starter-0.0.48/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/staging.py` & `ml-starter-0.0.48/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/timer.py` & `ml-starter-0.0.48/ml/utils/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,23 +72,24 @@
 
     def _spinner(self) -> None:
         chars = [colorize(c, "light-yellow") for c in ("|", "/", "-", "\\")]
         while not self._spinner_close:
             self._flag.wait()
             start_time = time.time()
             while not self._spinner_stop:
+                time.sleep(0.1)
                 max_line_len = 0
-                for char in chars:
-                    elapsed_secs = time.time() - start_time
-                    line = f"[ {char} {elapsed_secs:.1f} ] {self._text}\r"
-                    max_line_len = max(max_line_len, len(line))
-                    sys.stderr.write(line)
-                    sys.stderr.flush()
-                    time.sleep(0.05)
-                sys.stderr.write(" " * (max_line_len + 1) + "\r")
+                char = chars[int((time.time() * 10) % len(chars))]
+                elapsed_secs = time.time() - start_time
+                line = f"[ {char} {elapsed_secs:.1f} ] {self._text}\r"
+                max_line_len = max(max_line_len, len(line))
+                sys.stderr.write(line)
+                sys.stderr.flush()
+            sys.stderr.write(" " * (max_line_len + 1) + "\r")
+            sys.stderr.flush()
             self._flag.clear()
 
 
 @functools.lru_cache
 def spinner() -> Spinner:
     return Spinner()
```

### Comparing `ml-starter-0.0.47/ml/utils/torch_distributed.py` & `ml-starter-0.0.48/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.47/ml/utils/video.py` & `ml-starter-0.0.48/ml/utils/video.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import shutil
 import warnings
 from dataclasses import dataclass
 from fractions import Fraction
 from pathlib import Path
 from typing import AsyncGenerator, Iterator, Literal
 
+import av
 import cv2
 import ffmpeg
 import matplotlib.animation as ani
 import matplotlib.pyplot as plt
 import numpy as np
 from torch import Tensor
 
@@ -66,21 +67,44 @@
                     frame_count=count,
                     fps=Fraction(int(fps_num), int(fps_denom)),
                 )
 
         raise ValueError(f"Could not parse video properties from video in {fpath}")
 
 
+def read_video_av(
+    in_file: str | Path,
+    *,
+    target_dims: tuple[int | None, int | None] | None = None,
+) -> Iterator[np.ndarray]:
+    """Function that reads a video file to a stream of numpy arrays using PyAV.
+
+    Args:
+        in_file: The input video to read
+        target_dims: If not None, resize each frame to this size
+
+    Yields:
+        Frames from the video as numpy arrays with shape (H, W, C)
+    """
+    container = av.open(str(in_file))
+
+    for frame in container.decode(video=0):
+        frame = frame.to_rgb().to_ndarray()
+        if target_dims is not None:
+            frame = cv2.resize(frame, target_dims[::-1])
+        yield as_uint8(frame)
+
+
 def read_video_ffmpeg(
     in_file: str | Path,
     *,
     output_fmt: str = "rgb24",
     channels: int = 3,
 ) -> Iterator[np.ndarray]:
-    """Function that reads a video to a stream of numpy arrays using FFMPEG.
+    """Function that reads a video file to a stream of numpy arrays using FFMPEG.
 
     Args:
         in_file: The input video to read
         output_fmt: The output image format
         channels: Number of output channels for each video frame
 
     Yields:
@@ -233,14 +257,61 @@
     for img in itr:
         write_frame(standardize_image(img, keep_resolution=keep_resolution))
 
     stream.release()
     cv2.destroyAllWindows()
 
 
+def write_video_av(
+    itr: Iterator[np.ndarray | Tensor],
+    out_file: str | Path,
+    *,
+    keep_resolution: bool = False,
+    fps: int | Fraction = 30,
+    codec: str = "libx264",
+    input_fmt: str = "rgb24",
+    output_fmt: str = "yuv420p",
+) -> None:
+    """Function that writes an video from a stream of numpy arrays using PyAV.
+
+    Args:
+        itr: The image iterator, yielding images with shape (H, W, C).
+        out_file: The path to the output file.
+        keep_resolution: If set, don't change the image resolution, otherwise
+            resize to a human-friendly resolution.
+        fps: Frames per second for the video.
+        codec: The video codec to use for the output video
+        input_fmt: The input pixel format
+        output_fmt: The output pixel format
+    """
+    Path(out_file).parent.mkdir(exist_ok=True, parents=True)
+
+    first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
+
+    output = av.open(out_file, "w", format="mp4")
+    stream = output.add_stream(codec, rate=fps)
+    stream.pix_fmt = output_fmt
+
+    def write_frame(img: np.ndarray) -> None:
+        frame = av.VideoFrame.from_ndarray(as_uint8(img), format=input_fmt)
+        packet = stream.encode(frame)
+        if packet is not None:
+            output.mux(packet)
+
+    write_frame(first_img)
+    for img in itr:
+        write_frame(standardize_image(img, keep_resolution=keep_resolution))
+
+    packet = stream.encode()
+    if packet is not None:
+        output.mux(packet)
+
+    output.close()
+
+
 def write_video_ffmpeg(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     *,
     keep_resolution: bool = False,
     fps: int | Fraction = 30,
     out_fps: int | Fraction = 30,
@@ -342,26 +413,38 @@
         mpl_writer.grab_frame()
 
         for img in itr:
             im.set_data(as_uint8(standardize_image(img, keep_resolution=keep_resolution)))
             mpl_writer.grab_frame()
 
 
-Reader = Literal["ffmpeg", "opencv"]
-Writer = Literal["ffmpeg", "matplotlib", "opencv"]
+Reader = Literal["ffmpeg", "av", "opencv"]
+Writer = Literal["ffmpeg", "matplotlib", "av", "opencv"]
 
 
 def read_video(in_file: str | Path, *, reader: Reader = "ffmpeg") -> Iterator[np.ndarray]:
+    """Function that reads a video from a file to a stream of Numpy arrays.
+
+    Args:
+        in_file: The path to the input file.
+        reader: The video reader to use.
+
+    Yields:
+        The video frames as Numpy arrays.
+    """
     if reader == "ffmpeg":
         if not shutil.which("ffmpeg"):
-            warnings.warn("FFMPEG is not available in the system. Falling back to OpenCV.")
-            reader = "opencv"
+            warnings.warn("FFMPEG is not available in the system.")
+            reader = "av"
         else:
             return read_video_ffmpeg(in_file)
 
+    if reader == "av":
+        return read_video_av(in_file)
+
     if reader == "opencv":
         return read_video_opencv(in_file)
 
     raise ValueError(f"Invalid reader: {reader}")
 
 
 def write_video(
@@ -383,26 +466,30 @@
         writer: The video writer to use.
 
     Raises:
         ValueError: If the writer is invalid.
     """
     if writer == "ffmpeg":
         if not shutil.which("ffmpeg"):
-            warnings.warn("FFMPEG is not available in the system. Falling back to OpenCV.")
-            writer = "opencv"
+            warnings.warn("FFMPEG is not available in the system.")
+            writer = "av"
         else:
             write_video_ffmpeg(itr, out_file, fps=fps, keep_resolution=keep_resolution)
             return
 
     if writer == "matplotlib":
         if not shutil.which("ffmpeg"):
-            warnings.warn("FFMPEG is not available in the system. Falling back to OpenCV.")
-            writer = "opencv"
+            warnings.warn("FFMPEG is not available in the system.")
+            writer = "av"
         else:
             write_video_matplotlib(itr, out_file, fps=fps, keep_resolution=keep_resolution)
             return
 
+    if writer == "av":
+        write_video_av(itr, out_file, fps=fps, keep_resolution=keep_resolution)
+        return
+
     if writer == "opencv":
         write_video_opencv(itr, out_file, fps=fps, keep_resolution=keep_resolution)
         return
 
     raise ValueError(f"Invalid writer: {writer}")
```

### Comparing `ml-starter-0.0.47/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.48/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.47
+Version: 0.0.48
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.47/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.48/ml_starter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,21 +41,14 @@
 ml/models/base.py
 ml/models/embeddings.py
 ml/models/init.py
 ml/models/kmeans.py
 ml/models/lora.py
 ml/models/norms.py
 ml/models/parallel.py
-ml/models/pretrained/__init__.py
-ml/models/pretrained/blip.py
-ml/models/pretrained/clip.py
-ml/models/pretrained/hubert.py
-ml/models/pretrained/llama.py
-ml/models/pretrained/rwkv.py
-ml/models/pretrained/sam.py
 ml/optimizers/__init__.py
 ml/optimizers/adam.py
 ml/optimizers/adamw.py
 ml/optimizers/adan.py
 ml/optimizers/base.py
 ml/optimizers/common.py
 ml/optimizers/sgd.py
@@ -106,14 +99,15 @@
 ml/trainers/mixins/mixed_precision.py
 ml/trainers/mixins/monitor_process.py
 ml/trainers/mixins/profiler.py
 ml/trainers/mixins/step_wrapper.py
 ml/utils/__init__.py
 ml/utils/argparse.py
 ml/utils/atomic.py
+ml/utils/audio.py
 ml/utils/augmentation.py
 ml/utils/caching.py
 ml/utils/checkpoint.py
 ml/utils/checks.py
 ml/utils/cli.py
 ml/utils/colors.py
 ml/utils/config.py
```

### Comparing `ml-starter-0.0.47/pyproject.toml` & `ml-starter-0.0.48/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 # For TorchScript stuff.
 disable_error_code = ["attr-defined"]
 
 [[tool.mypy.overrides]]
 
 module = [
+    "av.*",
     "cv2.*",
     "ffmpeg.*",
     "matplotlib.*",
     "torchvision.*",
 ]
 
 ignore_missing_imports = true
```

### Comparing `ml-starter-0.0.47/setup.py` & `ml-starter-0.0.48/setup.py`

 * *Files identical despite different names*

