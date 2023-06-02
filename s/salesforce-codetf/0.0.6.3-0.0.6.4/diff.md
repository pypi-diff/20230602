# Comparing `tmp/salesforce-codetf-0.0.6.3.tar.gz` & `tmp/salesforce-codetf-0.0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-codetf-0.0.6.3.tar", last modified: Fri Jun  2 20:55:05 2023, max compression
+gzip compressed data, was "salesforce-codetf-0.0.6.4.tar", last modified: Fri Jun  2 20:59:23 2023, max compression
```

## Comparing `salesforce-codetf-0.0.6.3.tar` & `salesforce-codetf-0.0.6.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.950037 salesforce-codetf-0.0.6.3/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    25730 2023-06-02 20:55:05.950581 salesforce-codetf-0.0.6.3/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)    22464 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/README.md
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.915340 salesforce-codetf-0.0.6.3/codetf/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-0.0.6.3/codetf/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.917432 salesforce-codetf-0.0.6.3/codetf/code_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.918474 salesforce-codetf-0.0.6.3/codetf/code_utility/apex/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/apex/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/apex/apex_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/ast_parser.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/base_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.919328 salesforce-codetf-0.0.6.3/codetf/code_utility/java/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/java/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/java/java_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/language_specific_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.920278 salesforce-codetf-0.0.6.3/codetf/code_utility/python/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/python/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/codetf/code_utility/python/python_code_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.921253 salesforce-codetf-0.0.6.3/codetf/common/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-0.0.6.3/codetf/common/registry.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.6.3/codetf/common/utils.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.924898 salesforce-codetf-0.0.6.3/codetf/data_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.3/codetf/data_utility/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/codetf/data_utility/apps_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.3/codetf/data_utility/base_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/codetf/data_utility/codexglue_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.3/codetf/data_utility/human_eval_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/codetf/data_utility/mpp_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.3/codetf/data_utility/util.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.926025 salesforce-codetf-0.0.6.3/codetf/models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3494 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/codetf/models/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2311 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/codetf/models/base_model.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.926681 salesforce-codetf-0.0.6.3/codetf/models/bert_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3184 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/codetf/models/bert_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.927209 salesforce-codetf-0.0.6.3/codetf/models/causal_lm_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3445 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/codetf/models/causal_lm_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.927699 salesforce-codetf-0.0.6.3/codetf/models/seq2seq_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3476 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/codetf/models/seq2seq_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.929034 salesforce-codetf-0.0.6.3/codetf/performance/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.3/codetf/performance/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.3/codetf/performance/evaluation_metric.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/codetf/performance/model_evaluator.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.930665 salesforce-codetf-0.0.6.3/codetf/trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.3/codetf/trainer/base_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/codetf/trainer/causal_lm_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/codetf/trainer/codet5_trainer.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.931325 salesforce-codetf-0.0.6.3/docs/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1982 2023-05-24 08:02:35.000000 salesforce-codetf-0.0.6.3/docs/conf.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.936171 salesforce-codetf-0.0.6.3/salesforce_codetf.egg-info/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    25730 2023-06-02 20:55:05.000000 salesforce-codetf-0.0.6.3/salesforce_codetf.egg-info/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2095 2023-06-02 20:55:05.000000 salesforce-codetf-0.0.6.3/salesforce_codetf.egg-info/SOURCES.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:55:05.000000 salesforce-codetf-0.0.6.3/salesforce_codetf.egg-info/dependency_links.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:55:05.000000 salesforce-codetf-0.0.6.3/salesforce_codetf.egg-info/not-zip-safe
--rw-r--r--   0 nghi.bui   (503) staff       (20)      386 2023-06-02 20:55:05.000000 salesforce-codetf-0.0.6.3/salesforce_codetf.egg-info/requires.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       96 2023-06-02 20:55:05.000000 salesforce-codetf-0.0.6.3/salesforce_codetf.egg-info/top_level.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-06-02 20:55:05.951593 salesforce-codetf-0.0.6.3/setup.cfg
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1485 2023-06-02 20:54:54.000000 salesforce-codetf-0.0.6.3/setup.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.940086 salesforce-codetf-0.0.6.3/test_code_utilities/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.6.3/test_code_utilities/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.3/test_code_utilities/test_extract_code_attributre.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.3/test_code_utilities/test_parse_code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.3/test_code_utilities/test_remove_comments.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1109 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/test_code_utilities/test_variable_renaming.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.940889 salesforce-codetf-0.0.6.3/test_dataset/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      406 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/test_dataset/test_load_codexgluedataset.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.942720 salesforce-codetf-0.0.6.3/test_evaluation/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.3/test_evaluation/test_evaluate_human_eval_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.3/test_evaluation/test_evaluate_human_eval_codet5.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.947111 salesforce-codetf-0.0.6.3/test_inference/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.6.3/test_inference/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.3/test_inference/test_codebert_embedding.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      467 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/test_inference/test_codegen_nl2code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1092 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/test_inference/test_codet5_multitask.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      139 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/test_inference/test_load_model_zoo.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      438 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/test_inference/test_starcoder_nl2code.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:55:05.949270 salesforce-codetf-0.0.6.3/test_trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1291 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/test_trainer/test_causal_lm_trainer_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1313 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.3/test_trainer/test_codet5_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-0.0.6.3/test_trainer/test_t5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.430411 salesforce-codetf-0.0.6.4/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    25730 2023-06-02 20:59:23.430701 salesforce-codetf-0.0.6.4/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    22464 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/README.md
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.386828 salesforce-codetf-0.0.6.4/codetf/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-0.0.6.4/codetf/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.389609 salesforce-codetf-0.0.6.4/codetf/code_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.391109 salesforce-codetf-0.0.6.4/codetf/code_utility/apex/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/apex/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/apex/apex_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/ast_parser.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/base_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.392620 salesforce-codetf-0.0.6.4/codetf/code_utility/java/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/java/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/java/java_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/language_specific_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.394309 salesforce-codetf-0.0.6.4/codetf/code_utility/python/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/python/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/codetf/code_utility/python/python_code_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.395954 salesforce-codetf-0.0.6.4/codetf/common/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-0.0.6.4/codetf/common/registry.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.6.4/codetf/common/utils.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.402237 salesforce-codetf-0.0.6.4/codetf/data_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.4/codetf/data_utility/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/codetf/data_utility/apps_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.4/codetf/data_utility/base_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/codetf/data_utility/codexglue_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.4/codetf/data_utility/human_eval_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/codetf/data_utility/mpp_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.4/codetf/data_utility/util.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.404412 salesforce-codetf-0.0.6.4/codetf/models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3494 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/codetf/models/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2311 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/codetf/models/base_model.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.405407 salesforce-codetf-0.0.6.4/codetf/models/bert_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3184 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/codetf/models/bert_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.406362 salesforce-codetf-0.0.6.4/codetf/models/causal_lm_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3445 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/codetf/models/causal_lm_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.407395 salesforce-codetf-0.0.6.4/codetf/models/seq2seq_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3476 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/codetf/models/seq2seq_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.410039 salesforce-codetf-0.0.6.4/codetf/performance/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.4/codetf/performance/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.6.4/codetf/performance/evaluation_metric.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/codetf/performance/model_evaluator.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.412815 salesforce-codetf-0.0.6.4/codetf/trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.4/codetf/trainer/base_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/codetf/trainer/causal_lm_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/codetf/trainer/codet5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.413665 salesforce-codetf-0.0.6.4/docs/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1982 2023-05-24 08:02:35.000000 salesforce-codetf-0.0.6.4/docs/conf.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.418644 salesforce-codetf-0.0.6.4/salesforce_codetf.egg-info/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    25730 2023-06-02 20:59:23.000000 salesforce-codetf-0.0.6.4/salesforce_codetf.egg-info/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2095 2023-06-02 20:59:23.000000 salesforce-codetf-0.0.6.4/salesforce_codetf.egg-info/SOURCES.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:59:23.000000 salesforce-codetf-0.0.6.4/salesforce_codetf.egg-info/dependency_links.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:59:23.000000 salesforce-codetf-0.0.6.4/salesforce_codetf.egg-info/not-zip-safe
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      386 2023-06-02 20:59:23.000000 salesforce-codetf-0.0.6.4/salesforce_codetf.egg-info/requires.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       96 2023-06-02 20:59:23.000000 salesforce-codetf-0.0.6.4/salesforce_codetf.egg-info/top_level.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-06-02 20:59:23.431280 salesforce-codetf-0.0.6.4/setup.cfg
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1485 2023-06-02 20:57:33.000000 salesforce-codetf-0.0.6.4/setup.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.422556 salesforce-codetf-0.0.6.4/test_code_utilities/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.6.4/test_code_utilities/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.4/test_code_utilities/test_extract_code_attributre.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.4/test_code_utilities/test_parse_code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.4/test_code_utilities/test_remove_comments.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1109 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/test_code_utilities/test_variable_renaming.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.423336 salesforce-codetf-0.0.6.4/test_dataset/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      406 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/test_dataset/test_load_codexgluedataset.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.424807 salesforce-codetf-0.0.6.4/test_evaluation/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.4/test_evaluation/test_evaluate_human_eval_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.6.4/test_evaluation/test_evaluate_human_eval_codet5.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.428037 salesforce-codetf-0.0.6.4/test_inference/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.6.4/test_inference/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.6.4/test_inference/test_codebert_embedding.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      467 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/test_inference/test_codegen_nl2code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1092 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/test_inference/test_codet5_multitask.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      139 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/test_inference/test_load_model_zoo.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      438 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/test_inference/test_starcoder_nl2code.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:59:23.429975 salesforce-codetf-0.0.6.4/test_trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1291 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/test_trainer/test_causal_lm_trainer_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1313 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.6.4/test_trainer/test_codet5_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-0.0.6.4/test_trainer/test_t5_trainer.py
```

### Comparing `salesforce-codetf-0.0.6.3/PKG-INFO` & `salesforce-codetf-0.0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Description: 
             
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.6.3 Summary: CodeTF:
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.6.4 Summary: CodeTF:
 A Transformer-based Library for Code Intelligence Home-page: https://
 github.com/Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0
 Description:
 
                               [assets/logo.png]
   [license] [license] [license] Technical_Report, Documentation, Examples, #
     CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
```

### Comparing `salesforce-codetf-0.0.6.3/README.md` & `salesforce-codetf-0.0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/__init__.py` & `salesforce-codetf-0.0.6.4/codetf/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/code_utility/apex/apex_code_utility.py` & `salesforce-codetf-0.0.6.4/codetf/code_utility/apex/apex_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/code_utility/ast_parser.py` & `salesforce-codetf-0.0.6.4/codetf/code_utility/ast_parser.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/code_utility/base_utility.py` & `salesforce-codetf-0.0.6.4/codetf/code_utility/base_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/code_utility/java/java_code_utility.py` & `salesforce-codetf-0.0.6.4/codetf/code_utility/java/java_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/code_utility/python/python_code_utility.py` & `salesforce-codetf-0.0.6.4/codetf/code_utility/python/python_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/common/registry.py` & `salesforce-codetf-0.0.6.4/codetf/common/registry.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/common/utils.py` & `salesforce-codetf-0.0.6.4/codetf/common/utils.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/data_utility/apps_dataset.py` & `salesforce-codetf-0.0.6.4/codetf/data_utility/apps_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/data_utility/base_dataset.py` & `salesforce-codetf-0.0.6.4/codetf/data_utility/base_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/data_utility/codexglue_dataset.py` & `salesforce-codetf-0.0.6.4/codetf/data_utility/codexglue_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/data_utility/human_eval_dataset.py` & `salesforce-codetf-0.0.6.4/codetf/data_utility/human_eval_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/data_utility/mpp_dataset.py` & `salesforce-codetf-0.0.6.4/codetf/data_utility/mpp_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/data_utility/util.py` & `salesforce-codetf-0.0.6.4/codetf/data_utility/util.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/models/__init__.py` & `salesforce-codetf-0.0.6.4/codetf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/models/base_model.py` & `salesforce-codetf-0.0.6.4/codetf/models/base_model.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/models/bert_models/__init__.py` & `salesforce-codetf-0.0.6.4/codetf/models/bert_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/models/causal_lm_models/__init__.py` & `salesforce-codetf-0.0.6.4/codetf/models/causal_lm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/models/seq2seq_models/__init__.py` & `salesforce-codetf-0.0.6.4/codetf/models/seq2seq_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/performance/evaluation_metric.py` & `salesforce-codetf-0.0.6.4/codetf/performance/evaluation_metric.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/performance/model_evaluator.py` & `salesforce-codetf-0.0.6.4/codetf/performance/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/trainer/base_trainer.py` & `salesforce-codetf-0.0.6.4/codetf/trainer/base_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/trainer/causal_lm_trainer.py` & `salesforce-codetf-0.0.6.4/codetf/trainer/causal_lm_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/codetf/trainer/codet5_trainer.py` & `salesforce-codetf-0.0.6.4/codetf/trainer/codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/docs/conf.py` & `salesforce-codetf-0.0.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/salesforce_codetf.egg-info/PKG-INFO` & `salesforce-codetf-0.0.6.4/salesforce_codetf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Description: 
             
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.6.3 Summary: CodeTF:
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.6.4 Summary: CodeTF:
 A Transformer-based Library for Code Intelligence Home-page: https://
 github.com/Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0
 Description:
 
                               [assets/logo.png]
   [license] [license] [license] Technical_Report, Documentation, Examples, #
     CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
```

### Comparing `salesforce-codetf-0.0.6.3/salesforce_codetf.egg-info/SOURCES.txt` & `salesforce-codetf-0.0.6.4/salesforce_codetf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/setup.py` & `salesforce-codetf-0.0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 DEPENDENCY_LINKS = []
 if platform.system() == "Windows":
     DEPENDENCY_LINKS.append("https://download.pytorch.org/whl/torch_stable.html")
     
 setup(
   name = 'salesforce-codetf',
-  version = "0.0.6.3",
+  version = "0.0.6.4",
   py_modules = ['codetf'],
   description = 'CodeTF: A Transformer-based Library for Code Intelligence',
   author = 'Nghi D. Q. Bui',
   long_description=open("README.md", "r", encoding="utf-8").read(),
   long_description_content_type="text/markdown",
   keywords="AI4Code, Code Intelligence, Generative AI, Deep Learning, Library, PyTorch, HuggingFace",
   license="Apache 2.0",
```

### Comparing `salesforce-codetf-0.0.6.3/test_code_utilities/test_extract_code_attributre.py` & `salesforce-codetf-0.0.6.4/test_code_utilities/test_extract_code_attributre.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/test_code_utilities/test_parse_code.py` & `salesforce-codetf-0.0.6.4/test_code_utilities/test_parse_code.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/test_code_utilities/test_remove_comments.py` & `salesforce-codetf-0.0.6.4/test_code_utilities/test_remove_comments.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/test_code_utilities/test_variable_renaming.py` & `salesforce-codetf-0.0.6.4/test_code_utilities/test_variable_renaming.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/test_evaluation/test_evaluate_human_eval_codegen.py` & `salesforce-codetf-0.0.6.4/test_evaluation/test_evaluate_human_eval_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/test_evaluation/test_evaluate_human_eval_codet5.py` & `salesforce-codetf-0.0.6.4/test_evaluation/test_evaluate_human_eval_codet5.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/test_inference/test_codet5_multitask.py` & `salesforce-codetf-0.0.6.4/test_inference/test_codet5_multitask.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/test_trainer/test_causal_lm_trainer_codegen.py` & `salesforce-codetf-0.0.6.4/test_trainer/test_causal_lm_trainer_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/test_trainer/test_codet5_trainer.py` & `salesforce-codetf-0.0.6.4/test_trainer/test_codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.6.3/test_trainer/test_t5_trainer.py` & `salesforce-codetf-0.0.6.4/test_trainer/test_t5_trainer.py`

 * *Files identical despite different names*

