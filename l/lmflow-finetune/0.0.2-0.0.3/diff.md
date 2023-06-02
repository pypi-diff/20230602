# Comparing `tmp/lmflow-finetune-0.0.2.tar.gz` & `tmp/lmflow-finetune-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmflow-finetune-0.0.2.tar", last modified: Tue May 30 08:39:38 2023, max compression
+gzip compressed data, was "lmflow-finetune-0.0.3.tar", last modified: Fri Jun  2 08:06:51 2023, max compression
```

## Comparing `lmflow-finetune-0.0.2.tar` & `lmflow-finetune-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.005690 lmflow-finetune-0.0.2/
--rw-r--r--   0 kashun     (501) staff       (20)    11356 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/LICENSE
--rw-r--r--   0 kashun     (501) staff       (20)    23006 2023-05-30 08:39:38.005424 lmflow-finetune-0.0.2/PKG-INFO
--rw-r--r--   0 kashun     (501) staff       (20)    22653 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/README.md
--rw-r--r--   0 kashun     (501) staff       (20)       38 2023-05-30 08:39:38.005756 lmflow-finetune-0.0.2/setup.cfg
--rw-r--r--   0 kashun     (501) staff       (20)     1545 2023-05-30 08:38:19.000000 lmflow-finetune-0.0.2/setup.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.993582 lmflow-finetune-0.0.2/src/
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.995258 lmflow-finetune-0.0.2/src/lmflow/
--rw-r--r--   0 kashun     (501) staff       (20)      494 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)    19977 2023-05-30 08:37:31.000000 lmflow-finetune-0.0.2/src/lmflow/args.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.995688 lmflow-finetune-0.0.2/src/lmflow/datasets/
--rw-r--r--   0 kashun     (501) staff       (20)      387 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/datasets/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)    11619 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/datasets/dataset.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.998644 lmflow-finetune-0.0.2/src/lmflow/models/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)      887 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/models/auto_model.py
--rw-r--r--   0 kashun     (501) staff       (20)      162 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/base_model.py
--rw-r--r--   0 kashun     (501) staff       (20)      544 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/decoder_model.py
--rw-r--r--   0 kashun     (501) staff       (20)      550 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/models/encoder_decoder_model.py
--rw-r--r--   0 kashun     (501) staff       (20)    24039 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/models/hf_decoder_model.py
--rw-r--r--   0 kashun     (501) staff       (20)    11568 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/models/hf_encoder_decoder_model.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.999131 lmflow-finetune-0.0.2/src/lmflow/models/interfaces/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/interfaces/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)      110 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/interfaces/tunable.py
--rw-r--r--   0 kashun     (501) staff       (20)      208 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.2/src/lmflow/models/regression_model.py
--rw-r--r--   0 kashun     (501) staff       (20)     1304 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/models/text_regression_model.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.001248 lmflow-finetune-0.0.2/src/lmflow/pipeline/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)     1042 2023-05-30 06:30:04.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/auto_pipeline.py
--rw-r--r--   0 kashun     (501) staff       (20)      593 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/base_aligner.py
--rw-r--r--   0 kashun     (501) staff       (20)      140 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/base_pipeline.py
--rw-r--r--   0 kashun     (501) staff       (20)      522 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/base_tuner.py
--rw-r--r--   0 kashun     (501) staff       (20)    12694 2023-05-30 06:25:08.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/finetuner.py
--rw-r--r--   0 kashun     (501) staff       (20)     6683 2023-05-02 23:11:41.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/inferencer.py
--rw-r--r--   0 kashun     (501) staff       (20)    17246 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/raft_aligner.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.001833 lmflow-finetune-0.0.2/src/lmflow/pipeline/utils/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/utils/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)   185721 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/utils/raft_trainer.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.003301 lmflow-finetune-0.0.2/src/lmflow/utils/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/utils/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)     3884 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/utils/constants.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.003983 lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)     3649 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/gpt_neo_flash_attention.py
--rw-r--r--   0 kashun     (501) staff       (20)     4052 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/llama_flash_attention.py
--rw-r--r--   0 kashun     (501) staff       (20)       21 2023-05-30 08:38:29.000000 lmflow-finetune-0.0.2/src/lmflow/version.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.005082 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/
--rw-r--r--   0 kashun     (501) staff       (20)    23006 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/PKG-INFO
--rw-r--r--   0 kashun     (501) staff       (20)     1366 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/SOURCES.txt
--rw-r--r--   0 kashun     (501) staff       (20)        1 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/dependency_links.txt
--rw-r--r--   0 kashun     (501) staff       (20)      200 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/requires.txt
--rw-r--r--   0 kashun     (501) staff       (20)        7 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/top_level.txt
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.773785 lmflow-finetune-0.0.3/
+-rw-r--r--   0 kashun     (501) staff       (20)    11356 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/LICENSE
+-rw-r--r--   0 kashun     (501) staff       (20)    23006 2023-06-02 08:06:51.773558 lmflow-finetune-0.0.3/PKG-INFO
+-rw-r--r--   0 kashun     (501) staff       (20)    22653 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/README.md
+-rw-r--r--   0 kashun     (501) staff       (20)       38 2023-06-02 08:06:51.773845 lmflow-finetune-0.0.3/setup.cfg
+-rw-r--r--   0 kashun     (501) staff       (20)     1545 2023-06-02 08:06:48.000000 lmflow-finetune-0.0.3/setup.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.765196 lmflow-finetune-0.0.3/src/
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.767461 lmflow-finetune-0.0.3/src/lmflow/
+-rw-r--r--   0 kashun     (501) staff       (20)      494 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)    25209 2023-06-02 08:03:57.000000 lmflow-finetune-0.0.3/src/lmflow/args.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.767860 lmflow-finetune-0.0.3/src/lmflow/datasets/
+-rw-r--r--   0 kashun     (501) staff       (20)      387 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/datasets/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)    11619 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/datasets/dataset.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.769338 lmflow-finetune-0.0.3/src/lmflow/models/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)      887 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/auto_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)      162 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/base_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)      544 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/decoder_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)      550 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/encoder_decoder_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)    24039 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/hf_decoder_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)    11568 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/hf_encoder_decoder_model.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.769609 lmflow-finetune-0.0.3/src/lmflow/models/interfaces/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/interfaces/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)      110 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/interfaces/tunable.py
+-rw-r--r--   0 kashun     (501) staff       (20)      208 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/regression_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)     1304 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/models/text_regression_model.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.771010 lmflow-finetune-0.0.3/src/lmflow/pipeline/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)     1090 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/auto_pipeline.py
+-rw-r--r--   0 kashun     (501) staff       (20)      593 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/base_aligner.py
+-rw-r--r--   0 kashun     (501) staff       (20)      140 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/base_pipeline.py
+-rw-r--r--   0 kashun     (501) staff       (20)      522 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/base_tuner.py
+-rw-r--r--   0 kashun     (501) staff       (20)    23789 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/evaluator.py
+-rw-r--r--   0 kashun     (501) staff       (20)    13043 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/finetuner.py
+-rw-r--r--   0 kashun     (501) staff       (20)     6803 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/inferencer.py
+-rw-r--r--   0 kashun     (501) staff       (20)    17246 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/raft_aligner.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.771444 lmflow-finetune-0.0.3/src/lmflow/pipeline/utils/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/utils/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)     2997 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/utils/peft_trainer.py
+-rw-r--r--   0 kashun     (501) staff       (20)   185721 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/pipeline/utils/raft_trainer.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.772018 lmflow-finetune-0.0.3/src/lmflow/utils/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/utils/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)     3884 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/utils/constants.py
+-rw-r--r--   0 kashun     (501) staff       (20)     6590 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/utils/data_utils.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.772473 lmflow-finetune-0.0.3/src/lmflow/utils/flash_attention/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/utils/flash_attention/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)     3649 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/utils/flash_attention/gpt_neo_flash_attention.py
+-rw-r--r--   0 kashun     (501) staff       (20)     4052 2023-06-02 08:00:14.000000 lmflow-finetune-0.0.3/src/lmflow/utils/flash_attention/llama_flash_attention.py
+-rw-r--r--   0 kashun     (501) staff       (20)       21 2023-06-02 08:02:41.000000 lmflow-finetune-0.0.3/src/lmflow/version.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-06-02 08:06:51.773282 lmflow-finetune-0.0.3/src/lmflow_finetune.egg-info/
+-rw-r--r--   0 kashun     (501) staff       (20)    23006 2023-06-02 08:06:51.000000 lmflow-finetune-0.0.3/src/lmflow_finetune.egg-info/PKG-INFO
+-rw-r--r--   0 kashun     (501) staff       (20)     1472 2023-06-02 08:06:51.000000 lmflow-finetune-0.0.3/src/lmflow_finetune.egg-info/SOURCES.txt
+-rw-r--r--   0 kashun     (501) staff       (20)        1 2023-06-02 08:06:51.000000 lmflow-finetune-0.0.3/src/lmflow_finetune.egg-info/dependency_links.txt
+-rw-r--r--   0 kashun     (501) staff       (20)      200 2023-06-02 08:06:51.000000 lmflow-finetune-0.0.3/src/lmflow_finetune.egg-info/requires.txt
+-rw-r--r--   0 kashun     (501) staff       (20)        7 2023-06-02 08:06:51.000000 lmflow-finetune-0.0.3/src/lmflow_finetune.egg-info/top_level.txt
```

### Comparing `lmflow-finetune-0.0.2/LICENSE` & `lmflow-finetune-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/PKG-INFO` & `lmflow-finetune-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: lmflow-finetune
-Version: 0.0.2
-Summary: LMFlow: Large Model Flow.
-Author: The LMFlow Team
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center" width="100%">
 <img src="assets/logo.png" alt="LMFlow" style="width: 100%; min-width: 300px; display: block; margin: auto; background-color: transparent;">
 </p>
 
 # LMFlow
 
 <h4 align="center">
@@ -28,15 +17,15 @@
 
 [![Website](https://img.shields.io/badge/Website-Demo-20B2AA.svg)](https://lmflow.com)
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/OptimalScale/LMFlow/blob/main/LICENSE)
 [![Python 3.9+](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![Doc](https://img.shields.io/badge/Website-Doc-ff69b4.svg)](https://optimalscale.github.io/LMFlow/)
 [![Embark](https://img.shields.io/badge/Discord-LMFlow-%237289da.svg?logo=discord)](https://discord.gg/u9VJNpzhvA)
 [![slack badge](https://img.shields.io/badge/Slack-Join-blueviolet?logo=slack&amp)](https://join.slack.com/t/lmflow/shared_invite/zt-1s6egx12s-THlwHuCjF6~JGKmx7JoJPA)
-[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/05/23/V4aEoL.jpeg)
+[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/06/01/Vki1CZ.jpeg)
 
 An extensible, convenient, and efficient toolbox for finetuning large machine learning models, designed to be user-friendly, speedy and reliable, and accessible to the entire community.
 
 Large Model for All. See our [vision](https://github.com/OptimalScale/LMFlow#vision).
 
 <p align="center" width="100%">
 <img src="assets/features.png" alt="LMFlow-features" style="width: 100%; min-width: 300px; display: block; margin: auto;">
@@ -391,15 +380,15 @@
 
 Moreover, we aim to create an open and democratic LLM sharing platform where people can share their checkpoints and experiences to collectively improve the skills of the community. We welcome anyone who is interested in LLM to participate and join us in building an open and friendly community!
 
 Whether you are a beginner or an expert, we believe that you can benefit from this platform. Let's work together to build a vibrant and innovative LLM community!
 
 [![Embark](https://img.shields.io/badge/discord-LMFlow-%237289da.svg?logo=discord)](https://discord.gg/u9VJNpzhvA)
 [![slack badge](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/lmflow/shared_invite/zt-1s6egx12s-THlwHuCjF6~JGKmx7JoJPA)
-[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/05/23/V4aEoL.jpeg)
+[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/06/01/Vki1CZ.jpeg)
 
 
 
 ## Acknowledgement
 LMFlow draws inspiration from various studies, including but not limited to:
 - Alpaca: https://github.com/tatsu-lab/stanford_alpaca
 - Vicuna: https://github.com/lm-sys/FastChat
```

#### html2text {}

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1 Name: lmflow-finetune Version: 0.0.2 Summary: LMFlow:
-Large Model Flow. Author: The LMFlow Team Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
-Content-Type: text/markdown License-File: LICENSE
                                    [LMFlow]
 # LMFlow
 *** English | ç®ä½ä¸­æ | EspaÃ±ol | æ¥æ¬èª | íêµ­ì´ | à¤¹à¤¿à¤à¤¦à¥
                                       ***
 [![Website](https://img.shields.io/badge/Website-Demo-20B2AA.svg)](https://
 lmflow.com) [![Code License](https://img.shields.io/badge/Code%20License-
 Apache_2.0-green.svg)](https://github.com/OptimalScale/LMFlow/blob/main/
@@ -14,15 +9,15 @@
 (https://www.python.org/downloads/release/python-390/) [![Doc](https://
 img.shields.io/badge/Website-Doc-ff69b4.svg)](https://optimalscale.github.io/
 LMFlow/) [![Embark](https://img.shields.io/badge/Discord-LMFlow-
 %237289da.svg?logo=discord)](https://discord.gg/u9VJNpzhvA) [![slack badge]
 (https://img.shields.io/badge/Slack-Join-blueviolet?logo=slack&)](https://
 join.slack.com/t/lmflow/shared_invite/zt-1s6egx12s-THlwHuCjF6~JGKmx7JoJPA) [!
 [WeChat badge](https://img.shields.io/badge/WeChat-Join-
-brightgreen?logo=wechat&)](https://i.imgloc.com/2023/05/23/V4aEoL.jpeg) An
+brightgreen?logo=wechat&)](https://i.imgloc.com/2023/06/01/Vki1CZ.jpeg) An
 extensible, convenient, and efficient toolbox for finetuning large machine
 learning models, designed to be user-friendly, speedy and reliable, and
 accessible to the entire community. Large Model for All. See our [vision]
 (https://github.com/OptimalScale/LMFlow#vision).
                                [LMFlow-features]
 ## Latest News * [2023-05-15] :rocket: Release [LMFlow-data](http://lmflow.org:
 5000/lmflow_data.tar.gz), the training dataset of Robin-7B-v2. A new [test
@@ -243,16 +238,16 @@
 join us in building an open and friendly community! Whether you are a beginner
 or an expert, we believe that you can benefit from this platform. Let's work
 together to build a vibrant and innovative LLM community! [![Embark](https://
 img.shields.io/badge/discord-LMFlow-%237289da.svg?logo=discord)](https://
 discord.gg/u9VJNpzhvA) [![slack badge](https://img.shields.io/badge/Slack-join-
 blueviolet?logo=slack&)](https://join.slack.com/t/lmflow/shared_invite/zt-
 1s6egx12s-THlwHuCjF6~JGKmx7JoJPA) [![WeChat badge](https://img.shields.io/
-badge/WeChat-Join-brightgreen?logo=wechat&)](https://i.imgloc.com/2023/05/23/
-V4aEoL.jpeg) ## Acknowledgement LMFlow draws inspiration from various studies,
+badge/WeChat-Join-brightgreen?logo=wechat&)](https://i.imgloc.com/2023/06/01/
+Vki1CZ.jpeg) ## Acknowledgement LMFlow draws inspiration from various studies,
 including but not limited to: - Alpaca: https://github.com/tatsu-lab/
 stanford_alpaca - Vicuna: https://github.com/lm-sys/FastChat ## Support If you
 need any help, please submit a [Github](https://github.com/OptimalScale/LMFlow)
 issue. ## Contributors [https://contrib.rocks/image?repo=OptimalScale/LMFlow]
 ## Citation If you find this repository useful, please consider giving â­ and
 citing: ``` @misc{lmflow, author = {Shizhe Diao and Rui Pan and Hanze Dong and
 KaShun Shum and Jipeng Zhang and Wei Xiong and Tong Zhang}, title = {LMFlow: An
```

### Comparing `lmflow-finetune-0.0.2/README.md` & `lmflow-finetune-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: lmflow-finetune
+Version: 0.0.3
+Summary: LMFlow: Large Model Flow.
+Author: The LMFlow Team
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center" width="100%">
 <img src="assets/logo.png" alt="LMFlow" style="width: 100%; min-width: 300px; display: block; margin: auto; background-color: transparent;">
 </p>
 
 # LMFlow
 
 <h4 align="center">
@@ -17,15 +28,15 @@
 
 [![Website](https://img.shields.io/badge/Website-Demo-20B2AA.svg)](https://lmflow.com)
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/OptimalScale/LMFlow/blob/main/LICENSE)
 [![Python 3.9+](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![Doc](https://img.shields.io/badge/Website-Doc-ff69b4.svg)](https://optimalscale.github.io/LMFlow/)
 [![Embark](https://img.shields.io/badge/Discord-LMFlow-%237289da.svg?logo=discord)](https://discord.gg/u9VJNpzhvA)
 [![slack badge](https://img.shields.io/badge/Slack-Join-blueviolet?logo=slack&amp)](https://join.slack.com/t/lmflow/shared_invite/zt-1s6egx12s-THlwHuCjF6~JGKmx7JoJPA)
-[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/05/23/V4aEoL.jpeg)
+[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/06/01/Vki1CZ.jpeg)
 
 An extensible, convenient, and efficient toolbox for finetuning large machine learning models, designed to be user-friendly, speedy and reliable, and accessible to the entire community.
 
 Large Model for All. See our [vision](https://github.com/OptimalScale/LMFlow#vision).
 
 <p align="center" width="100%">
 <img src="assets/features.png" alt="LMFlow-features" style="width: 100%; min-width: 300px; display: block; margin: auto;">
@@ -380,15 +391,15 @@
 
 Moreover, we aim to create an open and democratic LLM sharing platform where people can share their checkpoints and experiences to collectively improve the skills of the community. We welcome anyone who is interested in LLM to participate and join us in building an open and friendly community!
 
 Whether you are a beginner or an expert, we believe that you can benefit from this platform. Let's work together to build a vibrant and innovative LLM community!
 
 [![Embark](https://img.shields.io/badge/discord-LMFlow-%237289da.svg?logo=discord)](https://discord.gg/u9VJNpzhvA)
 [![slack badge](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/lmflow/shared_invite/zt-1s6egx12s-THlwHuCjF6~JGKmx7JoJPA)
-[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/05/23/V4aEoL.jpeg)
+[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/06/01/Vki1CZ.jpeg)
 
 
 
 ## Acknowledgement
 LMFlow draws inspiration from various studies, including but not limited to:
 - Alpaca: https://github.com/tatsu-lab/stanford_alpaca
 - Vicuna: https://github.com/lm-sys/FastChat
```

#### html2text {}

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1 Name: lmflow-finetune Version: 0.0.3 Summary: LMFlow:
+Large Model Flow. Author: The LMFlow Team Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
+Content-Type: text/markdown License-File: LICENSE
                                    [LMFlow]
 # LMFlow
 *** English | ç®ä½ä¸­æ | EspaÃ±ol | æ¥æ¬èª | íêµ­ì´ | à¤¹à¤¿à¤à¤¦à¥
                                       ***
 [![Website](https://img.shields.io/badge/Website-Demo-20B2AA.svg)](https://
 lmflow.com) [![Code License](https://img.shields.io/badge/Code%20License-
 Apache_2.0-green.svg)](https://github.com/OptimalScale/LMFlow/blob/main/
@@ -9,15 +14,15 @@
 (https://www.python.org/downloads/release/python-390/) [![Doc](https://
 img.shields.io/badge/Website-Doc-ff69b4.svg)](https://optimalscale.github.io/
 LMFlow/) [![Embark](https://img.shields.io/badge/Discord-LMFlow-
 %237289da.svg?logo=discord)](https://discord.gg/u9VJNpzhvA) [![slack badge]
 (https://img.shields.io/badge/Slack-Join-blueviolet?logo=slack&)](https://
 join.slack.com/t/lmflow/shared_invite/zt-1s6egx12s-THlwHuCjF6~JGKmx7JoJPA) [!
 [WeChat badge](https://img.shields.io/badge/WeChat-Join-
-brightgreen?logo=wechat&)](https://i.imgloc.com/2023/05/23/V4aEoL.jpeg) An
+brightgreen?logo=wechat&)](https://i.imgloc.com/2023/06/01/Vki1CZ.jpeg) An
 extensible, convenient, and efficient toolbox for finetuning large machine
 learning models, designed to be user-friendly, speedy and reliable, and
 accessible to the entire community. Large Model for All. See our [vision]
 (https://github.com/OptimalScale/LMFlow#vision).
                                [LMFlow-features]
 ## Latest News * [2023-05-15] :rocket: Release [LMFlow-data](http://lmflow.org:
 5000/lmflow_data.tar.gz), the training dataset of Robin-7B-v2. A new [test
@@ -238,16 +243,16 @@
 join us in building an open and friendly community! Whether you are a beginner
 or an expert, we believe that you can benefit from this platform. Let's work
 together to build a vibrant and innovative LLM community! [![Embark](https://
 img.shields.io/badge/discord-LMFlow-%237289da.svg?logo=discord)](https://
 discord.gg/u9VJNpzhvA) [![slack badge](https://img.shields.io/badge/Slack-join-
 blueviolet?logo=slack&)](https://join.slack.com/t/lmflow/shared_invite/zt-
 1s6egx12s-THlwHuCjF6~JGKmx7JoJPA) [![WeChat badge](https://img.shields.io/
-badge/WeChat-Join-brightgreen?logo=wechat&)](https://i.imgloc.com/2023/05/23/
-V4aEoL.jpeg) ## Acknowledgement LMFlow draws inspiration from various studies,
+badge/WeChat-Join-brightgreen?logo=wechat&)](https://i.imgloc.com/2023/06/01/
+Vki1CZ.jpeg) ## Acknowledgement LMFlow draws inspiration from various studies,
 including but not limited to: - Alpaca: https://github.com/tatsu-lab/
 stanford_alpaca - Vicuna: https://github.com/lm-sys/FastChat ## Support If you
 need any help, please submit a [Github](https://github.com/OptimalScale/LMFlow)
 issue. ## Contributors [https://contrib.rocks/image?repo=OptimalScale/LMFlow]
 ## Citation If you find this repository useful, please consider giving â­ and
 citing: ``` @misc{lmflow, author = {Shizhe Diao and Rui Pan and Hanze Dong and
 KaShun Shum and Jipeng Zhang and Wei Xiong and Tong Zhang}, title = {LMFlow: An
```

### Comparing `lmflow-finetune-0.0.2/setup.py` & `lmflow-finetune-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/args.py` & `lmflow-finetune-0.0.3/src/lmflow/args.py`

 * *Files 12% similar despite different names*

```diff
@@ -377,14 +377,175 @@
     """
     Adapt transformers.TrainingArguments
     """
     eval_dataset_path: Optional[str] = field(
         default=None, metadata={"help": "The path of the eval dataset to use."}
     )
 
+
+@dataclass
+class EvaluatorArguments:
+    """
+    Define a class EvaluatorArguments using the dataclass decorator. The class contains several optional
+    parameters that can be used to configure a evaluator.
+
+    local_rank : str
+        For distributed training: local_rank
+
+    random_shuffle : bool
+
+    use_wandb : bool
+
+    random_seed : int, default = 1
+
+    output_dir : str, default = './output_dir',
+
+    mixed_precision : str, choice from ["bf16","fp16"].
+        mixed precision mode, whether to use bf16 or fp16
+
+    deepspeed : 
+        Enable deepspeed and pass the path to deepspeed json config file (e.g. ds_config.json) or an already
+        loaded json file as a dict
+        
+    temperature : float
+        An argument of model.generate in huggingface to control the diversity of generation.
+        
+    repetition_penalty : float
+        An argument of model.generate in huggingface to penalize repetitions.
+    """
+    local_rank: int = field(
+        default=-1,
+        metadata={"help": "For distributed training: local_rank"
+        }
+    )
+
+    random_shuffle: Optional[bool] = field(
+        default=False, 
+        metadata={"help": ""
+        }
+    )
+    
+    use_wandb: Optional[bool] = field(
+        default=False,
+        metadata={
+            "help": (
+                "When this flag is True, wandb will be enabled"
+            )
+        },
+    )
+    random_seed: Optional[int] = field(
+        default=1,
+        metadata={
+            "help": (
+                "used to set random seed"
+            )
+        },
+    )
+    output_dir: Optional[str] = field(
+        default="./output_dir",
+        metadata={"help": "Output path for the inferenced results"},
+    )
+    mixed_precision: Optional[str] = field(
+        default="bf16",
+        metadata={
+            "help": (
+                "mixed precision mode, whether to use bf16 or fp16"
+            ),
+            "choices": ["bf16","fp16"],
+        },
+    )
+    deepspeed: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": (
+                "Enable deepspeed and pass the path to deepspeed json config file (e.g. ds_config.json) or an already"
+                " loaded json file as a dict"
+            )
+        },
+    )
+    answer_type: Optional[str] = field(
+        default="text",
+        metadata={
+            "help": (
+                'Question type for answer extraction from the decoder output.'
+                ' Supported types: \n'
+                '   1) "multiple_choice", e.g. A, B, C, D, ...\n'
+                '   2) "binary_choice", e.g. yes, no, maybe\n'
+                '   3) "math", e.g. 1.0, -3.52\n'
+                '   4) "text", e.g. "I think that it is okay"\n'
+                '   5) Special treatment for several datasets\n'
+                '     - "gsm8k"\n'
+                '     - "svamp"\n'
+                '     - "asdiv"\n'
+                '     - "addsub"\n'
+                '     - "singleeq"\n'
+                '     - "multiarith"\n'
+                '     - "aqua"\n'
+                '     - "csqa"\n'
+                '     - "strategyqa"\n'
+                '     - "pubmedqa"\n'
+                '     - "medmcqa"\n'
+                '     - "usmle"\n'
+            )
+        },
+    )
+    prompt_structure: Optional[str] = field(
+        default="{input}",
+        metadata={
+            "help": (
+                'Prompt structure to facilitate prompt engineering during'
+                ' inference. The model will receive'
+                ' `prompt_structure.format(input=input)` as its input.'
+            )
+        },
+    )
+    evaluate_block_size: Optional[int] = field(
+        default=512,
+        metadata={
+            "help": (
+                "the model will have at least block_size tokens for context when calculating the conditional likelihood of any one token"
+                " (provided there are block_size preceding tokens available to condition on)"
+            )
+        },
+    )
+    metric: Optional[str] = field(
+        default="accuracy",
+        metadata={
+            "help": "the metric the model will be evaluated on",
+            "choices": ["ppl", "perplexity", "acc", "accuracy", "nll", "neg_log_likelihood"],
+        },
+    )
+    inference_batch_size_per_device: Optional[int] = field(
+        default=1,
+        metadata={
+            "help": (
+                "every device will infer {inference_batch_size_per_device}"
+                " samples in parallel. The inferred results will be concatenaed"
+                " with inputs and attach a reward."
+            ),
+        },
+    )
+    use_accelerator_for_evaluator: bool = field(
+        default=False, metadata={"help": "Whether to use Huggingface Accelerator instead of Deepspeed"},
+    )
+        
+    temperature: float = field(
+        default=0,
+        metadata={"help": "Temperature during inference."},
+    )
+    
+    repetition_penalty: float = field(
+        default=1,
+        metadata={"help": "Repetition_penalty during inference."},
+    )
+        
+    max_new_tokens: int = field(
+        default=100,
+        metadata={"help": "Maximum length during inference."},
+    )
     
 @dataclass
 class InferencerArguments:
     """
     Define a class InferencerArguments using the dataclass decorator. The class contains several optional
     parameters that can be used to configure a inferencer.
 
@@ -394,28 +555,49 @@
     random_seed : int, default = 1
 
     deepspeed :
         Enable deepspeed and pass the path to deepspeed json config file (e.g. ds_config.json) or an already
         loaded json file as a dict
     mixed_precision : str, choice from ["bf16","fp16"].
         mixed precision mode, whether to use bf16 or fp16
-
+    
+    temperature : float
+        An argument of model.generate in huggingface to control the diversity of generation.
+        
+    repetition_penalty : float
+        An argument of model.generate in huggingface to penalize repetitions.
     """
     device: str = field(
         default="gpu",
         metadata={
             "help": "device of chatbot",
             "choices": ["gpu", "cpu"],
         },
     )
     local_rank: int = field(
         default=-1,
         metadata={"help": "For distributed training: local_rank"
-        }
+        },
+    )
+        
+    temperature: float = field(
+        default=0,
+        metadata={"help": "Temperature during inference."},
     )
+    
+    repetition_penalty: float = field(
+        default=1,
+        metadata={"help": "Repetition_penalty during inference."},
+    )
+        
+    max_new_tokens: int = field(
+        default=100,
+        metadata={"help": "Maximum length during inference."},
+    )
+        
     random_seed: Optional[int] = field(
         default=1,
         metadata={
             "help": (
                 "used to set random seed"
             )
         },
@@ -440,14 +622,15 @@
     )
     do_sample: Optional[bool] = field(
         default=False,
         metadata={
             "help": "whether turn on true random sampling during inference."
         },
     )
+        
 
 
 @dataclass
 class RaftAlignerArguments(TrainingArguments):
     """
     Define a class RaftAlignerArguments to configure raft aligner.
     """
@@ -506,34 +689,17 @@
                 "every device will infer {inference_batch_size_per_device}"
                 " samples in parallel. The inferred results will be concatenaed"
                 " with inputs and attach a reward."
             ),
         },
     )
 
-@dataclass
-class BenchmarkingArguments:
-    dataset_name: Optional[str] = field(
-        default=None,
-        metadata={
-            "help": "benchmark dataset name provided by lmflow"
-        },
-    )
-    lm_evaluation_metric: Optional[str] = field(
-        default="accuracy",
-        metadata={
-            "help": "the metric the model will be evaluated on",
-            "choices": ["acc", "acc_norm", "bleu", "chrf", "em", "f1", "ppl", \
-                "ter", "r@1", "r@2", "mrr", "mc1", "mc2", "word_perplexity", \
-                    "byte_perplexity", "bits_per_byte"],
-        },
-    )
-
 PIPELINE_ARGUMENT_MAPPING = {
     "finetuner": FinetunerArguments,
+    "evaluator": EvaluatorArguments,
     "inferencer": InferencerArguments,
     "raft_aligner": RaftAlignerArguments,
 }
 
 
 class AutoArguments:
     """
```

### Comparing `lmflow-finetune-0.0.2/src/lmflow/datasets/dataset.py` & `lmflow-finetune-0.0.3/src/lmflow/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/models/auto_model.py` & `lmflow-finetune-0.0.3/src/lmflow/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/models/decoder_model.py` & `lmflow-finetune-0.0.3/src/lmflow/models/decoder_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/models/encoder_decoder_model.py` & `lmflow-finetune-0.0.3/src/lmflow/models/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/models/hf_decoder_model.py` & `lmflow-finetune-0.0.3/src/lmflow/models/hf_decoder_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/models/hf_encoder_decoder_model.py` & `lmflow-finetune-0.0.3/src/lmflow/models/hf_encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/models/text_regression_model.py` & `lmflow-finetune-0.0.3/src/lmflow/models/text_regression_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/pipeline/auto_pipeline.py` & `lmflow-finetune-0.0.3/src/lmflow/pipeline/auto_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # coding=utf-8
 """Return a pipeline automatically based on its name.
 """
 
+from lmflow.pipeline.evaluator import Evaluator
 from lmflow.pipeline.finetuner import Finetuner
 from lmflow.pipeline.inferencer import Inferencer
 from lmflow.pipeline.raft_aligner import RaftAligner
 
 
 PIPELINE_MAPPING = {
     "evaluator": Evaluator,
```

### Comparing `lmflow-finetune-0.0.2/src/lmflow/pipeline/base_aligner.py` & `lmflow-finetune-0.0.3/src/lmflow/pipeline/base_aligner.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/pipeline/base_tuner.py` & `lmflow-finetune-0.0.3/src/lmflow/pipeline/base_tuner.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/pipeline/finetuner.py` & `lmflow-finetune-0.0.3/src/lmflow/pipeline/finetuner.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 )
 from copy import deepcopy
 from transformers.utils import send_example_telemetry
 from transformers.trainer_utils import get_last_checkpoint
 
 from lmflow.datasets.dataset import Dataset
 from lmflow.pipeline.base_tuner import BaseTuner
+from lmflow.pipeline.utils.peft_trainer import PeftTrainer, PeftSavingCallback
 
 
 logger = logging.getLogger(__name__)
 
 
 class Finetuner(BaseTuner):
     """
@@ -248,24 +249,33 @@
         if finetuner_args.do_train:
             if data_args.max_train_samples is not None:
                 max_train_samples = min(len(train_dataset), data_args.max_train_samples)
                 train_dataset = train_dataset.select(range(max_train_samples))
 
         # Initialize our Trainer
         training_args = finetuner_args
-        trainer = Trainer(
+
+        if model_args.use_lora:
+            FinetuningTrainer = PeftTrainer
+            trainer_callbacks = [PeftSavingCallback]
+        else:
+            FinetuningTrainer = Trainer
+            trainer_callbacks = []
+
+        trainer = FinetuningTrainer(
             model=model.get_backend_model(),
             args=training_args,
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
             tokenizer=model.get_tokenizer(),
             # Data collator will default to DataCollatorWithPadding, so we change it.
             data_collator=default_data_collator,
             compute_metrics=compute_metrics if training_args.do_eval else None,
             preprocess_logits_for_metrics=preprocess_logits_for_metrics if training_args.do_eval else None,
+            callbacks=trainer_callbacks
         )
 
         # Training
         if training_args.do_train:
             checkpoint = None
             last_checkpoint = self.last_checkpoint
             if training_args.resume_from_checkpoint is not None:
```

### Comparing `lmflow-finetune-0.0.2/src/lmflow/pipeline/inferencer.py` & `lmflow-finetune-0.0.3/src/lmflow/pipeline/inferencer.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,17 +136,17 @@
             else:
                 raise NotImplementedError(
                     f"device \"{self.inferencer_args.device}\" is not supported"
                 )
 
             outputs = model.inference(
                 inputs,
-                max_new_tokens=max_new_tokens,
-                temperature=temperature,
-                repetition_penalty=1.0,
+                max_new_tokens=self.inferencer_args.max_new_tokens,
+                temperature=self.inferencer_args.temperature,
+                repetition_penalty=self.inferencer_args.repetition_penalty,
                 do_sample=self.inferencer_args.do_sample,
             )
             text_out = model.decode(outputs[0], skip_special_tokens=True)
 
             # only return the generation, trucating the input
             prompt_length = len(model.decode(inputs[0], skip_special_tokens=True,))
             text_out = text_out[prompt_length:]
@@ -161,20 +161,20 @@
         response = ""
         history = []
         if "ChatGLMModel" in self.config.architectures:
             for response, history in model.get_backend_model().stream_chat(model.get_tokenizer(), context, history=history):
                 response = rstrip_partial_utf8(response)
                 yield response, False
         else:
-            for _ in range(0, max_new_tokens // token_per_step):
+            for _ in range(0, self.inferencer_args.max_new_tokens // token_per_step):
                 output_dataset = self.inference(
                     model=model,
                     dataset=input_dataset,
                     max_new_tokens=token_per_step,
-                    temperature=temperature,
+                    temperature=self.inferencer_args.temperature,
                 )
 
                 new_append_text = output_dataset.to_dict()["instances"][0]["text"]
                 new_append_text = rstrip_partial_utf8(new_append_text)
                 response += new_append_text
 
                 input_dict = input_dataset.to_dict()
```

### Comparing `lmflow-finetune-0.0.2/src/lmflow/pipeline/raft_aligner.py` & `lmflow-finetune-0.0.3/src/lmflow/pipeline/raft_aligner.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/pipeline/utils/raft_trainer.py` & `lmflow-finetune-0.0.3/src/lmflow/pipeline/utils/raft_trainer.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/utils/constants.py` & `lmflow-finetune-0.0.3/src/lmflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/gpt_neo_flash_attention.py` & `lmflow-finetune-0.0.3/src/lmflow/utils/flash_attention/gpt_neo_flash_attention.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/llama_flash_attention.py` & `lmflow-finetune-0.0.3/src/lmflow/utils/flash_attention/llama_flash_attention.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/PKG-INFO` & `lmflow-finetune-0.0.3/src/lmflow_finetune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmflow-finetune
-Version: 0.0.2
+Version: 0.0.3
 Summary: LMFlow: Large Model Flow.
 Author: The LMFlow Team
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,15 +28,15 @@
 
 [![Website](https://img.shields.io/badge/Website-Demo-20B2AA.svg)](https://lmflow.com)
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/OptimalScale/LMFlow/blob/main/LICENSE)
 [![Python 3.9+](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![Doc](https://img.shields.io/badge/Website-Doc-ff69b4.svg)](https://optimalscale.github.io/LMFlow/)
 [![Embark](https://img.shields.io/badge/Discord-LMFlow-%237289da.svg?logo=discord)](https://discord.gg/u9VJNpzhvA)
 [![slack badge](https://img.shields.io/badge/Slack-Join-blueviolet?logo=slack&amp)](https://join.slack.com/t/lmflow/shared_invite/zt-1s6egx12s-THlwHuCjF6~JGKmx7JoJPA)
-[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/05/23/V4aEoL.jpeg)
+[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/06/01/Vki1CZ.jpeg)
 
 An extensible, convenient, and efficient toolbox for finetuning large machine learning models, designed to be user-friendly, speedy and reliable, and accessible to the entire community.
 
 Large Model for All. See our [vision](https://github.com/OptimalScale/LMFlow#vision).
 
 <p align="center" width="100%">
 <img src="assets/features.png" alt="LMFlow-features" style="width: 100%; min-width: 300px; display: block; margin: auto;">
@@ -391,15 +391,15 @@
 
 Moreover, we aim to create an open and democratic LLM sharing platform where people can share their checkpoints and experiences to collectively improve the skills of the community. We welcome anyone who is interested in LLM to participate and join us in building an open and friendly community!
 
 Whether you are a beginner or an expert, we believe that you can benefit from this platform. Let's work together to build a vibrant and innovative LLM community!
 
 [![Embark](https://img.shields.io/badge/discord-LMFlow-%237289da.svg?logo=discord)](https://discord.gg/u9VJNpzhvA)
 [![slack badge](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/lmflow/shared_invite/zt-1s6egx12s-THlwHuCjF6~JGKmx7JoJPA)
-[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/05/23/V4aEoL.jpeg)
+[![WeChat badge](https://img.shields.io/badge/WeChat-Join-brightgreen?logo=wechat&amp)](https://i.imgloc.com/2023/06/01/Vki1CZ.jpeg)
 
 
 
 ## Acknowledgement
 LMFlow draws inspiration from various studies, including but not limited to:
 - Alpaca: https://github.com/tatsu-lab/stanford_alpaca
 - Vicuna: https://github.com/lm-sys/FastChat
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmflow-finetune Version: 0.0.2 Summary: LMFlow:
+Metadata-Version: 2.1 Name: lmflow-finetune Version: 0.0.3 Summary: LMFlow:
 Large Model Flow. Author: The LMFlow Team Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
 Content-Type: text/markdown License-File: LICENSE
                                    [LMFlow]
 # LMFlow
 *** English | ç®ä½ä¸­æ | EspaÃ±ol | æ¥æ¬èª | íêµ­ì´ | à¤¹à¤¿à¤à¤¦à¥
@@ -14,15 +14,15 @@
 (https://www.python.org/downloads/release/python-390/) [![Doc](https://
 img.shields.io/badge/Website-Doc-ff69b4.svg)](https://optimalscale.github.io/
 LMFlow/) [![Embark](https://img.shields.io/badge/Discord-LMFlow-
 %237289da.svg?logo=discord)](https://discord.gg/u9VJNpzhvA) [![slack badge]
 (https://img.shields.io/badge/Slack-Join-blueviolet?logo=slack&)](https://
 join.slack.com/t/lmflow/shared_invite/zt-1s6egx12s-THlwHuCjF6~JGKmx7JoJPA) [!
 [WeChat badge](https://img.shields.io/badge/WeChat-Join-
-brightgreen?logo=wechat&)](https://i.imgloc.com/2023/05/23/V4aEoL.jpeg) An
+brightgreen?logo=wechat&)](https://i.imgloc.com/2023/06/01/Vki1CZ.jpeg) An
 extensible, convenient, and efficient toolbox for finetuning large machine
 learning models, designed to be user-friendly, speedy and reliable, and
 accessible to the entire community. Large Model for All. See our [vision]
 (https://github.com/OptimalScale/LMFlow#vision).
                                [LMFlow-features]
 ## Latest News * [2023-05-15] :rocket: Release [LMFlow-data](http://lmflow.org:
 5000/lmflow_data.tar.gz), the training dataset of Robin-7B-v2. A new [test
@@ -243,16 +243,16 @@
 join us in building an open and friendly community! Whether you are a beginner
 or an expert, we believe that you can benefit from this platform. Let's work
 together to build a vibrant and innovative LLM community! [![Embark](https://
 img.shields.io/badge/discord-LMFlow-%237289da.svg?logo=discord)](https://
 discord.gg/u9VJNpzhvA) [![slack badge](https://img.shields.io/badge/Slack-join-
 blueviolet?logo=slack&)](https://join.slack.com/t/lmflow/shared_invite/zt-
 1s6egx12s-THlwHuCjF6~JGKmx7JoJPA) [![WeChat badge](https://img.shields.io/
-badge/WeChat-Join-brightgreen?logo=wechat&)](https://i.imgloc.com/2023/05/23/
-V4aEoL.jpeg) ## Acknowledgement LMFlow draws inspiration from various studies,
+badge/WeChat-Join-brightgreen?logo=wechat&)](https://i.imgloc.com/2023/06/01/
+Vki1CZ.jpeg) ## Acknowledgement LMFlow draws inspiration from various studies,
 including but not limited to: - Alpaca: https://github.com/tatsu-lab/
 stanford_alpaca - Vicuna: https://github.com/lm-sys/FastChat ## Support If you
 need any help, please submit a [Github](https://github.com/OptimalScale/LMFlow)
 issue. ## Contributors [https://contrib.rocks/image?repo=OptimalScale/LMFlow]
 ## Citation If you find this repository useful, please consider giving â­ and
 citing: ``` @misc{lmflow, author = {Shizhe Diao and Rui Pan and Hanze Dong and
 KaShun Shum and Jipeng Zhang and Wei Xiong and Tong Zhang}, title = {LMFlow: An
```

### Comparing `lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/SOURCES.txt` & `lmflow-finetune-0.0.3/src/lmflow_finetune.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -18,21 +18,24 @@
 src/lmflow/models/interfaces/__init__.py
 src/lmflow/models/interfaces/tunable.py
 src/lmflow/pipeline/__init__.py
 src/lmflow/pipeline/auto_pipeline.py
 src/lmflow/pipeline/base_aligner.py
 src/lmflow/pipeline/base_pipeline.py
 src/lmflow/pipeline/base_tuner.py
+src/lmflow/pipeline/evaluator.py
 src/lmflow/pipeline/finetuner.py
 src/lmflow/pipeline/inferencer.py
 src/lmflow/pipeline/raft_aligner.py
 src/lmflow/pipeline/utils/__init__.py
+src/lmflow/pipeline/utils/peft_trainer.py
 src/lmflow/pipeline/utils/raft_trainer.py
 src/lmflow/utils/__init__.py
 src/lmflow/utils/constants.py
+src/lmflow/utils/data_utils.py
 src/lmflow/utils/flash_attention/__init__.py
 src/lmflow/utils/flash_attention/gpt_neo_flash_attention.py
 src/lmflow/utils/flash_attention/llama_flash_attention.py
 src/lmflow_finetune.egg-info/PKG-INFO
 src/lmflow_finetune.egg-info/SOURCES.txt
 src/lmflow_finetune.egg-info/dependency_links.txt
 src/lmflow_finetune.egg-info/requires.txt
```

