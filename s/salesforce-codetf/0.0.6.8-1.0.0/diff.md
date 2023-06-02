# Comparing `tmp/salesforce-codetf-0.0.6.8.tar.gz` & `tmp/salesforce-codetf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-codetf-0.0.6.8.tar", last modified: Fri Jun  2 21:20:36 2023, max compression
+gzip compressed data, was "salesforce-codetf-1.0.0.tar", last modified: Fri Jun  2 21:45:46 2023, max compression
```

## Comparing `salesforce-codetf-0.0.6.8.tar` & `salesforce-codetf-1.0.0.tar`

### file list

```diff
@@ -1,80 +1,93 @@
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.460514 salesforce-codetf-0.0.6.8/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    25730 2023-06-02 21:20:36.460882 salesforce-codetf-0.0.6.8/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)    22464 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/README.md
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.434543 salesforce-codetf-0.0.6.8/codetf/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-0.0.6.8/codetf/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.436346 salesforce-codetf-0.0.6.8/codetf/code_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.437181 salesforce-codetf-0.0.6.8/codetf/code_utility/apex/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/apex/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/apex/apex_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/ast_parser.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/base_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.438192 salesforce-codetf-0.0.6.8/codetf/code_utility/java/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/java/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/java/java_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/language_specific_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.439163 salesforce-codetf-0.0.6.8/codetf/code_utility/python/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/python/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/codetf/code_utility/python/python_code_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.440146 salesforce-codetf-0.0.6.8/codetf/common/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-0.0.6.8/codetf/common/registry.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.6.8/codetf/common/utils.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.443540 salesforce-codetf-0.0.6.8/codetf/data_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.8/codetf/data_utility/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/codetf/data_utility/apps_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.8/codetf/data_utility/base_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/codetf/data_utility/codexglue_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.8/codetf/data_utility/human_eval_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/codetf/data_utility/mpp_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.8/codetf/data_utility/util.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.444460 salesforce-codetf-0.0.6.8/codetf/models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3494 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/codetf/models/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2311 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/codetf/models/base_model.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.444889 salesforce-codetf-0.0.6.8/codetf/models/bert_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3184 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/codetf/models/bert_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.445306 salesforce-codetf-0.0.6.8/codetf/models/causal_lm_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3445 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/codetf/models/causal_lm_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.445750 salesforce-codetf-0.0.6.8/codetf/models/seq2seq_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3476 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/codetf/models/seq2seq_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.447153 salesforce-codetf-0.0.6.8/codetf/performance/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.8/codetf/performance/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.8/codetf/performance/evaluation_metric.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/codetf/performance/model_evaluator.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.448529 salesforce-codetf-0.0.6.8/codetf/trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.8/codetf/trainer/base_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/codetf/trainer/causal_lm_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/codetf/trainer/codet5_trainer.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.449074 salesforce-codetf-0.0.6.8/docs/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1982 2023-05-24 08:02:35.000000 salesforce-codetf-0.0.6.8/docs/conf.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.451837 salesforce-codetf-0.0.6.8/salesforce_codetf.egg-info/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    25730 2023-06-02 21:20:36.000000 salesforce-codetf-0.0.6.8/salesforce_codetf.egg-info/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2095 2023-06-02 21:20:36.000000 salesforce-codetf-0.0.6.8/salesforce_codetf.egg-info/SOURCES.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       96 2023-06-02 21:20:36.000000 salesforce-codetf-0.0.6.8/salesforce_codetf.egg-info/dependency_links.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:59:23.000000 salesforce-codetf-0.0.6.8/salesforce_codetf.egg-info/not-zip-safe
--rw-r--r--   0 nghi.bui   (503) staff       (20)      336 2023-06-02 21:20:36.000000 salesforce-codetf-0.0.6.8/salesforce_codetf.egg-info/requires.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)      101 2023-06-02 21:20:36.000000 salesforce-codetf-0.0.6.8/salesforce_codetf.egg-info/top_level.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-06-02 21:20:36.461517 salesforce-codetf-0.0.6.8/setup.cfg
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1609 2023-06-02 21:20:25.000000 salesforce-codetf-0.0.6.8/setup.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.454090 salesforce-codetf-0.0.6.8/test_code_utilities/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.6.8/test_code_utilities/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.8/test_code_utilities/test_extract_code_attributre.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.8/test_code_utilities/test_parse_code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.8/test_code_utilities/test_remove_comments.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1109 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/test_code_utilities/test_variable_renaming.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.454530 salesforce-codetf-0.0.6.8/test_dataset/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      406 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/test_dataset/test_load_codexgluedataset.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.455591 salesforce-codetf-0.0.6.8/test_evaluation/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.8/test_evaluation/test_evaluate_human_eval_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.8/test_evaluation/test_evaluate_human_eval_codet5.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.458780 salesforce-codetf-0.0.6.8/test_inference/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.6.8/test_inference/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.8/test_inference/test_codebert_embedding.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      467 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/test_inference/test_codegen_nl2code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1092 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/test_inference/test_codet5_multitask.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      139 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/test_inference/test_load_model_zoo.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      438 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/test_inference/test_starcoder_nl2code.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:20:36.460155 salesforce-codetf-0.0.6.8/test_trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1291 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/test_trainer/test_causal_lm_trainer_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1313 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.8/test_trainer/test_codet5_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-0.0.6.8/test_trainer/test_t5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.673999 salesforce-codetf-1.0.0/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       39 2023-06-02 21:30:18.000000 salesforce-codetf-1.0.0/MANIFEST.in
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    25728 2023-06-02 21:45:46.674499 salesforce-codetf-1.0.0/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    22464 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/README.md
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.630022 salesforce-codetf-1.0.0/codetf/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.0/codetf/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.632290 salesforce-codetf-1.0.0/codetf/code_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.633576 salesforce-codetf-1.0.0/codetf/code_utility/apex/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/apex/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/code_utility/apex/apex_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/code_utility/ast_parser.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/base_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.634248 salesforce-codetf-1.0.0/codetf/code_utility/java/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/java/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/code_utility/java/java_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/language_specific_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.635436 salesforce-codetf-1.0.0/codetf/code_utility/python/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-1.0.0/codetf/code_utility/python/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/code_utility/python/python_code_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.636526 salesforce-codetf-1.0.0/codetf/common/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-1.0.0/codetf/common/registry.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.0/codetf/common/utils.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.637521 salesforce-codetf-1.0.0/codetf/configs/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:28:24.000000 salesforce-codetf-1.0.0/codetf/configs/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.637972 salesforce-codetf-1.0.0/codetf/configs/dataset/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      328 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/configs/dataset/dataset.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      131 2023-03-20 20:11:15.000000 salesforce-codetf-1.0.0/codetf/configs/default.yaml
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.639390 salesforce-codetf-1.0.0/codetf/configs/inference/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      480 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/configs/inference/bert.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2852 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/configs/inference/causal_lm.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/configs/inference/codet5.yaml
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.640306 salesforce-codetf-1.0.0/codetf/configs/training/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      766 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/configs/training/causal_lm.yaml
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1020 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/configs/training/codet5.yaml
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.644650 salesforce-codetf-1.0.0/codetf/data_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.0/codetf/data_utility/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/data_utility/apps_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/data_utility/base_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/data_utility/codexglue_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/data_utility/human_eval_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/data_utility/mpp_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.0/codetf/data_utility/util.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.646035 salesforce-codetf-1.0.0/codetf/models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3494 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2311 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/base_model.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.646898 salesforce-codetf-1.0.0/codetf/models/bert_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3184 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/bert_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.647652 salesforce-codetf-1.0.0/codetf/models/causal_lm_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3445 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/causal_lm_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.648401 salesforce-codetf-1.0.0/codetf/models/seq2seq_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3476 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/codetf/models/seq2seq_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.650601 salesforce-codetf-1.0.0/codetf/performance/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.0/codetf/performance/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-1.0.0/codetf/performance/evaluation_metric.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/performance/model_evaluator.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.652963 salesforce-codetf-1.0.0/codetf/trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/codetf/trainer/base_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/trainer/causal_lm_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/codetf/trainer/codet5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.653779 salesforce-codetf-1.0.0/docs/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1982 2023-05-24 08:02:35.000000 salesforce-codetf-1.0.0/docs/conf.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.660054 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    25728 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2385 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/SOURCES.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       96 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/dependency_links.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:59:23.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/not-zip-safe
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      319 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/requires.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       42 2023-06-02 21:45:46.000000 salesforce-codetf-1.0.0/salesforce_codetf.egg-info/top_level.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-06-02 21:45:46.675522 salesforce-codetf-1.0.0/setup.cfg
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1644 2023-06-02 21:45:35.000000 salesforce-codetf-1.0.0/setup.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.664961 salesforce-codetf-1.0.0/test_code_utilities/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.0/test_code_utilities/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_code_utilities/test_extract_code_attributre.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_code_utilities/test_parse_code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_code_utilities/test_remove_comments.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1109 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_code_utilities/test_variable_renaming.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.665714 salesforce-codetf-1.0.0/test_dataset/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      406 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_dataset/test_load_codexgluedataset.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.667183 salesforce-codetf-1.0.0/test_evaluation/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_evaluation/test_evaluate_human_eval_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-1.0.0/test_evaluation/test_evaluate_human_eval_codet5.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.671255 salesforce-codetf-1.0.0/test_inference/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-1.0.0/test_inference/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-1.0.0/test_inference/test_codebert_embedding.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      467 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_inference/test_codegen_nl2code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1098 2023-06-02 21:45:21.000000 salesforce-codetf-1.0.0/test_inference/test_codet5_multitask.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      139 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_inference/test_load_model_zoo.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      438 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_inference/test_starcoder_nl2code.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 21:45:46.673349 salesforce-codetf-1.0.0/test_trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1291 2023-06-02 20:32:15.000000 salesforce-codetf-1.0.0/test_trainer/test_causal_lm_trainer_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1313 2023-06-02 21:34:03.000000 salesforce-codetf-1.0.0/test_trainer/test_codet5_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-1.0.0/test_trainer/test_t5_trainer.py
```

### Comparing `salesforce-codetf-0.0.6.8/PKG-INFO` & `salesforce-codetf-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 0.0.6.8
+Version: 1.0.0
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Description: 
             
         <p align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.6.8 Summary: CodeTF:
-A Transformer-based Library for Code Intelligence Home-page: https://
-github.com/Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0
-Description:
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.0 Summary: CodeTF: A
+Transformer-based Library for Code Intelligence Home-page: https://github.com/
+Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0 Description:
 
                               [assets/logo.png]
   [license] [license] [license] Technical_Report, Documentation, Examples, #
     CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
 ## Table of Contents - [Introduction](#introduction) - [Installation]
 (#installation-guide) - [Getting Started](#getting-started) - [Inferencing
 Pipeline](#inferencing-pipeline) - [Model Zoo](#model-zoo) - [Fine-Tuning Your
```

### Comparing `salesforce-codetf-0.0.6.8/README.md` & `salesforce-codetf-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/__init__.py` & `salesforce-codetf-1.0.0/codetf/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/code_utility/apex/apex_code_utility.py` & `salesforce-codetf-1.0.0/codetf/code_utility/apex/apex_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/code_utility/ast_parser.py` & `salesforce-codetf-1.0.0/codetf/code_utility/ast_parser.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/code_utility/base_utility.py` & `salesforce-codetf-1.0.0/codetf/code_utility/base_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/code_utility/java/java_code_utility.py` & `salesforce-codetf-1.0.0/codetf/code_utility/java/java_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/code_utility/python/python_code_utility.py` & `salesforce-codetf-1.0.0/codetf/code_utility/python/python_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/common/registry.py` & `salesforce-codetf-1.0.0/codetf/common/registry.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/common/utils.py` & `salesforce-codetf-1.0.0/codetf/common/utils.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/data_utility/apps_dataset.py` & `salesforce-codetf-1.0.0/codetf/data_utility/apps_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/data_utility/base_dataset.py` & `salesforce-codetf-1.0.0/codetf/data_utility/base_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/data_utility/codexglue_dataset.py` & `salesforce-codetf-1.0.0/codetf/data_utility/codexglue_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/data_utility/human_eval_dataset.py` & `salesforce-codetf-1.0.0/codetf/data_utility/human_eval_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/data_utility/mpp_dataset.py` & `salesforce-codetf-1.0.0/codetf/data_utility/mpp_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/data_utility/util.py` & `salesforce-codetf-1.0.0/codetf/data_utility/util.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/models/__init__.py` & `salesforce-codetf-1.0.0/codetf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/models/base_model.py` & `salesforce-codetf-1.0.0/codetf/models/base_model.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/models/bert_models/__init__.py` & `salesforce-codetf-1.0.0/codetf/models/bert_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/models/causal_lm_models/__init__.py` & `salesforce-codetf-1.0.0/codetf/models/causal_lm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/models/seq2seq_models/__init__.py` & `salesforce-codetf-1.0.0/codetf/models/seq2seq_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/performance/evaluation_metric.py` & `salesforce-codetf-1.0.0/codetf/performance/evaluation_metric.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/performance/model_evaluator.py` & `salesforce-codetf-1.0.0/codetf/performance/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/trainer/base_trainer.py` & `salesforce-codetf-1.0.0/codetf/trainer/base_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/trainer/causal_lm_trainer.py` & `salesforce-codetf-1.0.0/codetf/trainer/causal_lm_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/codetf/trainer/codet5_trainer.py` & `salesforce-codetf-1.0.0/codetf/trainer/codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/docs/conf.py` & `salesforce-codetf-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/salesforce_codetf.egg-info/PKG-INFO` & `salesforce-codetf-1.0.0/salesforce_codetf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 0.0.6.8
+Version: 1.0.0
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Description: 
             
         <p align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.6.8 Summary: CodeTF:
-A Transformer-based Library for Code Intelligence Home-page: https://
-github.com/Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0
-Description:
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.0 Summary: CodeTF: A
+Transformer-based Library for Code Intelligence Home-page: https://github.com/
+Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0 Description:
 
                               [assets/logo.png]
   [license] [license] [license] Technical_Report, Documentation, Examples, #
     CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
 ## Table of Contents - [Introduction](#introduction) - [Installation]
 (#installation-guide) - [Getting Started](#getting-started) - [Inferencing
 Pipeline](#inferencing-pipeline) - [Model Zoo](#model-zoo) - [Fine-Tuning Your
```

### Comparing `salesforce-codetf-0.0.6.8/salesforce_codetf.egg-info/SOURCES.txt` & `salesforce-codetf-1.0.0/salesforce_codetf.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 codetf/__init__.py
 codetf/code_utility/__init__.py
 codetf/code_utility/ast_parser.py
 codetf/code_utility/base_utility.py
@@ -10,14 +11,22 @@
 codetf/code_utility/apex/apex_code_utility.py
 codetf/code_utility/java/__init__.py
 codetf/code_utility/java/java_code_utility.py
 codetf/code_utility/python/__init__.py
 codetf/code_utility/python/python_code_utility.py
 codetf/common/registry.py
 codetf/common/utils.py
+codetf/configs/__init__.py
+codetf/configs/default.yaml
+codetf/configs/dataset/dataset.yaml
+codetf/configs/inference/bert.yaml
+codetf/configs/inference/causal_lm.yaml
+codetf/configs/inference/codet5.yaml
+codetf/configs/training/causal_lm.yaml
+codetf/configs/training/codet5.yaml
 codetf/data_utility/__init__.py
 codetf/data_utility/apps_dataset.py
 codetf/data_utility/base_dataset.py
 codetf/data_utility/codexglue_dataset.py
 codetf/data_utility/human_eval_dataset.py
 codetf/data_utility/mpp_dataset.py
 codetf/data_utility/util.py
```

### Comparing `salesforce-codetf-0.0.6.8/setup.py` & `salesforce-codetf-1.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     "evaluate==0.4.0",
     "huggingface-hub==0.14.1",
     "iopath==0.1.10",
     "nltk==3.8.1",
     "numpy==1.21.6",
     "omegaconf==2.3.0",
     "pandas==1.3.5",
-    "peft==0.4.0.dev0",
     "pyparsing==3.0.7",
     "PyYAML==6.0",
     "requests==2.31.0",
     "rouge-score==0.1.2",
     "sacrebleu==2.3.1",
     "scikit-learn==1.0.2",
     "torch==1.13.1",
@@ -28,24 +27,25 @@
 if platform.system() == "Windows":
     DEPENDENCY_LINKS.append("https://download.pytorch.org/whl/torch_stable.html")
 DEPENDENCY_LINKS.append("git+https://github.com/huggingface/transformers.git")
 DEPENDENCY_LINKS.append("git+https://github.com/huggingface/peft.git")
     
 setup(
   name = 'salesforce-codetf',
-  version = "0.0.6.8",
+  version = "1.0.0",
   py_modules = ['codetf'],
   description = 'CodeTF: A Transformer-based Library for Code Intelligence',
   author = 'Nghi D. Q. Bui',
+  package_dir={"codeff": "codetf"},
   long_description=open("README.md", "r", encoding="utf-8").read(),
   long_description_content_type="text/markdown",
   keywords="AI4Code, Code Intelligence, Generative AI, Deep Learning, Library, PyTorch, HuggingFace",
   license="Apache 2.0",
   url = 'https://github.com/Salesforce/CodeTF',
-  packages=find_namespace_packages(include="codetf.*"),
+  packages=find_packages(where=".", exclude=["tests", "assets", "datasets"]),
+  package_data={'codetf': ['configs/*']},
   install_requires=install_requires,
   include_package_data=True,
   zip_safe=False,
   python_requires=">=3.8.0",
-  package_data={'codetf': ['*.yaml']},
   dependency_links=DEPENDENCY_LINKS,
 )
```

### Comparing `salesforce-codetf-0.0.6.8/test_code_utilities/test_extract_code_attributre.py` & `salesforce-codetf-1.0.0/test_code_utilities/test_extract_code_attributre.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/test_code_utilities/test_parse_code.py` & `salesforce-codetf-1.0.0/test_code_utilities/test_parse_code.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/test_code_utilities/test_remove_comments.py` & `salesforce-codetf-1.0.0/test_code_utilities/test_remove_comments.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/test_code_utilities/test_variable_renaming.py` & `salesforce-codetf-1.0.0/test_code_utilities/test_variable_renaming.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/test_evaluation/test_evaluate_human_eval_codegen.py` & `salesforce-codetf-1.0.0/test_evaluation/test_evaluate_human_eval_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/test_evaluation/test_evaluate_human_eval_codet5.py` & `salesforce-codetf-1.0.0/test_evaluation/test_evaluate_human_eval_codet5.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/test_inference/test_codet5_multitask.py` & `salesforce-codetf-1.0.0/test_inference/test_codet5_multitask.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import sys
-from pathlib import Path
-sys.path.append(str(Path(".").absolute().parent))
+# import sys
+# from pathlib import Path
+# sys.path.append(str(Path(".").absolute().parent))
 from codetf.models import load_model_pipeline
 
-translation_model = load_model_pipeline(model_name="codet5", task="translate-cs-java",
+translation_model = load_model_pipeline(model_name="codet5", task="translate_cs_java",
             model_type="base", is_eval=True, 
             load_in_4bit=True, weight_sharding=False)
 
-summarization_model = load_model_pipeline(model_name="codet5", task="sum-python",
+summarization_model = load_model_pipeline(model_name="codet5", task="sum_python",
             model_type="base", is_eval=True,
             load_in_8bit=True, weight_sharding=False)
 
 code_snippets = """
     void bubbleSort(int arr[])
     {
         int n = arr.length;
```

### Comparing `salesforce-codetf-0.0.6.8/test_trainer/test_causal_lm_trainer_codegen.py` & `salesforce-codetf-1.0.0/test_trainer/test_causal_lm_trainer_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/test_trainer/test_codet5_trainer.py` & `salesforce-codetf-1.0.0/test_trainer/test_codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.8/test_trainer/test_t5_trainer.py` & `salesforce-codetf-1.0.0/test_trainer/test_t5_trainer.py`

 * *Files identical despite different names*

