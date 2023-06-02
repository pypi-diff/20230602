# Comparing `tmp/salesforce-codetf-0.0.3.tar.gz` & `tmp/salesforce-codetf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-codetf-0.0.3.tar", last modified: Tue May 23 19:08:03 2023, max compression
+gzip compressed data, was "salesforce-codetf-0.0.4.tar", last modified: Fri Jun  2 20:34:15 2023, max compression
```

## Comparing `salesforce-codetf-0.0.3.tar` & `salesforce-codetf-0.0.4.tar`

### file list

```diff
@@ -1,77 +1,80 @@
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.087437 salesforce-codetf-0.0.3/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    19491 2023-05-23 19:08:03.087672 salesforce-codetf-0.0.3/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)    16625 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/README.md
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.073322 salesforce-codetf-0.0.3/codetf/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-0.0.3/codetf/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.074365 salesforce-codetf-0.0.3/codetf/code_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.3/codetf/code_utility/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.074858 salesforce-codetf-0.0.3/codetf/code_utility/apex/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.3/codetf/code_utility/apex/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/code_utility/apex/apex_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/codetf/code_utility/ast_parser.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.3/codetf/code_utility/base_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.075365 salesforce-codetf-0.0.3/codetf/code_utility/java/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.3/codetf/code_utility/java/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/code_utility/java/java_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.3/codetf/code_utility/language_specific_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.075859 salesforce-codetf-0.0.3/codetf/code_utility/python/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.3/codetf/code_utility/python/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/code_utility/python/python_code_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.076398 salesforce-codetf-0.0.3/codetf/common/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-0.0.3/codetf/common/registry.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.3/codetf/common/utils.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.078240 salesforce-codetf-0.0.3/codetf/data_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.3/codetf/data_utility/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/data_utility/apps_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/codetf/data_utility/base_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/data_utility/codexglue_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/codetf/data_utility/human_eval_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/data_utility/mpp_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.3/codetf/data_utility/util.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.078782 salesforce-codetf-0.0.3/codetf/models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3204 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/codetf/models/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2262 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.3/codetf/models/base_model.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.079059 salesforce-codetf-0.0.3/codetf/models/bert_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2773 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/codetf/models/bert_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.079336 salesforce-codetf-0.0.3/codetf/models/causal_lm_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3062 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/models/causal_lm_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.079617 salesforce-codetf-0.0.3/codetf/models/codet5_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3096 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/models/codet5_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.080387 salesforce-codetf-0.0.3/codetf/performance/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.3/codetf/performance/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.3/codetf/performance/evaluation_metric.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/performance/model_evaluator.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.081211 salesforce-codetf-0.0.3/codetf/trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/codetf/trainer/base_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/trainer/causal_lm_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/codetf/trainer/codet5_trainer.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.082916 salesforce-codetf-0.0.3/salesforce_codetf.egg-info/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    19491 2023-05-23 19:08:03.000000 salesforce-codetf-0.0.3/salesforce_codetf.egg-info/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2043 2023-05-23 19:08:03.000000 salesforce-codetf-0.0.3/salesforce_codetf.egg-info/SOURCES.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-05-23 19:08:03.000000 salesforce-codetf-0.0.3/salesforce_codetf.egg-info/dependency_links.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-05-22 21:32:45.000000 salesforce-codetf-0.0.3/salesforce_codetf.egg-info/not-zip-safe
--rw-r--r--   0 nghi.bui   (503) staff       (20)      350 2023-05-23 19:08:03.000000 salesforce-codetf-0.0.3/salesforce_codetf.egg-info/requires.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)      101 2023-05-23 19:08:03.000000 salesforce-codetf-0.0.3/salesforce_codetf.egg-info/top_level.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-05-23 19:08:03.088198 salesforce-codetf-0.0.3/setup.cfg
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1527 2023-05-23 19:07:43.000000 salesforce-codetf-0.0.3/setup.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.084234 salesforce-codetf-0.0.3/test_code_utilities/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.3/test_code_utilities/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/test_code_utilities/test_extract_code_attributre.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/test_code_utilities/test_parse_code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/test_code_utilities/test_remove_comments.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1066 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/test_code_utilities/test_variable_renaming.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.084506 salesforce-codetf-0.0.3/test_dataset/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      791 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/test_dataset/test_load_codexgluedataset.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.085065 salesforce-codetf-0.0.3/test_evaluation/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/test_evaluation/test_evaluate_human_eval_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/test_evaluation/test_evaluate_human_eval_codet5.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.086365 salesforce-codetf-0.0.3/test_inference/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.3/test_inference/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/test_inference/test_codebert_embedding.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      468 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/test_inference/test_codegen_nl2code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1129 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/test_inference/test_codet5_multitask.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      452 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/test_inference/test_starcoder_nl2code.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:08:03.087185 salesforce-codetf-0.0.3/test_trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.3/test_trainer/test_causal_lm_trainer_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1373 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.3/test_trainer/test_codet5_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-0.0.3/test_trainer/test_t5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.733528 salesforce-codetf-0.0.4/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    25730 2023-06-02 20:34:15.733819 salesforce-codetf-0.0.4/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    22464 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/README.md
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.692443 salesforce-codetf-0.0.4/codetf/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-0.0.4/codetf/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.695509 salesforce-codetf-0.0.4/codetf/code_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.4/codetf/code_utility/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.697081 salesforce-codetf-0.0.4/codetf/code_utility/apex/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.4/codetf/code_utility/apex/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/codetf/code_utility/apex/apex_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.4/codetf/code_utility/ast_parser.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.4/codetf/code_utility/base_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.698565 salesforce-codetf-0.0.4/codetf/code_utility/java/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.4/codetf/code_utility/java/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/codetf/code_utility/java/java_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.4/codetf/code_utility/language_specific_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.700213 salesforce-codetf-0.0.4/codetf/code_utility/python/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.4/codetf/code_utility/python/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/codetf/code_utility/python/python_code_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.702587 salesforce-codetf-0.0.4/codetf/common/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-0.0.4/codetf/common/registry.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.4/codetf/common/utils.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.709176 salesforce-codetf-0.0.4/codetf/data_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.4/codetf/data_utility/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/codetf/data_utility/apps_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.4/codetf/data_utility/base_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/codetf/data_utility/codexglue_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.4/codetf/data_utility/human_eval_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/codetf/data_utility/mpp_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.4/codetf/data_utility/util.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.710921 salesforce-codetf-0.0.4/codetf/models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3494 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/codetf/models/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2311 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/codetf/models/base_model.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.711617 salesforce-codetf-0.0.4/codetf/models/bert_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3184 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/codetf/models/bert_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.712476 salesforce-codetf-0.0.4/codetf/models/causal_lm_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3445 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/codetf/models/causal_lm_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.713269 salesforce-codetf-0.0.4/codetf/models/seq2seq_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3476 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/codetf/models/seq2seq_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.715509 salesforce-codetf-0.0.4/codetf/performance/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.4/codetf/performance/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.4/codetf/performance/evaluation_metric.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/codetf/performance/model_evaluator.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.718168 salesforce-codetf-0.0.4/codetf/trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.4/codetf/trainer/base_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/codetf/trainer/causal_lm_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/codetf/trainer/codet5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.718924 salesforce-codetf-0.0.4/docs/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1982 2023-05-24 08:02:35.000000 salesforce-codetf-0.0.4/docs/conf.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.723499 salesforce-codetf-0.0.4/salesforce_codetf.egg-info/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    25730 2023-06-02 20:34:15.000000 salesforce-codetf-0.0.4/salesforce_codetf.egg-info/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2095 2023-06-02 20:34:15.000000 salesforce-codetf-0.0.4/salesforce_codetf.egg-info/SOURCES.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-06-02 20:34:15.000000 salesforce-codetf-0.0.4/salesforce_codetf.egg-info/dependency_links.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-05-22 21:32:45.000000 salesforce-codetf-0.0.4/salesforce_codetf.egg-info/not-zip-safe
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      386 2023-06-02 20:34:15.000000 salesforce-codetf-0.0.4/salesforce_codetf.egg-info/requires.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      101 2023-06-02 20:34:15.000000 salesforce-codetf-0.0.4/salesforce_codetf.egg-info/top_level.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-06-02 20:34:15.734481 salesforce-codetf-0.0.4/setup.cfg
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1661 2023-06-02 20:34:03.000000 salesforce-codetf-0.0.4/setup.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.726725 salesforce-codetf-0.0.4/test_code_utilities/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.4/test_code_utilities/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.4/test_code_utilities/test_extract_code_attributre.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.4/test_code_utilities/test_parse_code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.4/test_code_utilities/test_remove_comments.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1109 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/test_code_utilities/test_variable_renaming.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.727162 salesforce-codetf-0.0.4/test_dataset/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      406 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/test_dataset/test_load_codexgluedataset.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.728443 salesforce-codetf-0.0.4/test_evaluation/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.4/test_evaluation/test_evaluate_human_eval_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.4/test_evaluation/test_evaluate_human_eval_codet5.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.731444 salesforce-codetf-0.0.4/test_inference/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.4/test_inference/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.4/test_inference/test_codebert_embedding.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      467 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/test_inference/test_codegen_nl2code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1092 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/test_inference/test_codet5_multitask.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      139 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/test_inference/test_load_model_zoo.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      438 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/test_inference/test_starcoder_nl2code.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-06-02 20:34:15.733067 salesforce-codetf-0.0.4/test_trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1291 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/test_trainer/test_causal_lm_trainer_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1313 2023-06-02 20:32:15.000000 salesforce-codetf-0.0.4/test_trainer/test_codet5_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-0.0.4/test_trainer/test_t5_trainer.py
```

### Comparing `salesforce-codetf-0.0.3/PKG-INFO` & `salesforce-codetf-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,319 +1,357 @@
-Metadata-Version: 2.1
-Name: salesforce-codetf
-Version: 0.0.3
-Summary: CodeTF: A Transformer-based Library for Code Intelligence
-Home-page: https://github.com/Salesforce/CodeTF
-Author: Nghi D. Q. Bui
-License: 3-Clause BSD
-Description: 
+
+    
+<p align="center">
+    <br>
+    <img src="assets/logo.png" width="500"/>
+    <br>
+<p>
+<div align="center">
+  <a href="https://opensource.org/license/apache-2-0/">
+  <img alt="license" src="https://img.shields.io/badge/License-Apache%202.0-green.svg"/>
+  </a>
+   <a href="https://www.python.org/downloads/release/python-380/">
+  <img alt="license" src="https://img.shields.io/badge/python-3.8+-yellow.svg"/>
+  </a> 
+   <a href="https://pypi.org/project/salesforce-codetf/">
+  <img alt="license" src="https://static.pepy.tech/badge/salesforce-codetf"/>
+  </a> 
+
+<a href="https://arxiv.org/pdf/2306.00029.pdf">Technical Report</a>,
+<a href="https://opensource.salesforce.com/CodeTF/latest/index.html">Documentation</a>,
+<a href="https://github.com/salesforce/CodeTF/tree/main/test_inference">Examples</a>,
+    
+# CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
+
+<!-- 
+[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/bdqnghi/CodeTF_personal/blob/main/LICENSE)
+[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) -->
+ </div>   
+    
+## Table of Contents
+  - [Introduction](#introduction)
+  - [Installation](#installation-guide)
+  - [Getting Started](#getting-started)
+    - [Inferencing Pipeline](#inferencing-pipeline)
+    - [Model Zoo](#model-zoo)
+    - [Fine-Tuning Your Own Model](#fine-tuning-pipeline)
+    - [Evaluate On Well-Known Benchmarks](#evaluate-on-well-known-benchmarks)
+    - [Utilities to Manipulate Source Code Based on AST](#code-utilities)
+        - [AST Parser in Multiple Languages](#ast-parser-in-multiple-languages)
+        - [Extract Code Attributes](#extract-code-attributes)
+        - [Remove Comments](#remove-comments)
+  - [Ethical and Responsible Use](#ethical-and-responsible-use) 
+  - [License](#license)
+
+## Introduction
+CodeTF is a one-stop Python transformer-based library for ***code large language models (Code LLMs)*** and ***code intelligence***, provides a seamless interface for training and inferencing on code intelligence tasks like code summarization, translation, code generation and so on. It aims to facilitate easy integration of SOTA CodeLLMs into real-world applications.
+
+In addition to the core LLMs's features for code, CodeTF offers utilities for code manipulation across various languages, including easy extraction of code attributes. Using tree-sitter as its core AST parser, it enables parsing of attributes such as function names, comments, and variable names. Pre-built libraries for numerous languages are provided, eliminating the need for complicated parser setup. CodeTF thus ensures a user-friendly and accessible environment for code intelligence tasks.
+
+The current version of the library offers:
+
+- **Fast Model Serving**: We support an easy-to-use interface for rapid inferencing with **pre-quantized models** (int8, int16, float16). CodeTF handles all aspects of device management, so users do not have to worry about that aspect. If your model is large, we offer advanced features such as weight sharding across GPUs to serve the models more quickly.
+- **Fine-Tuning Your Own Models**: We provide an API for quickly fine-tuning your own LLMs for code using SOTA techniques for **parameter-efficient fine-tuning** (HuggingFace PEFT) on distributed environments.
+- **Supported Tasks**: nl2code, code summarization, code completion, code translation, code refinement, clone detection, defect prediction.
+- **Datasets+**: We have preprocessed well-known benchmarks (**Human-Eval, MBPP, CodeXGLUE, APPS, etc.**) and offer an easy-to-load feature for these datasets.
+- **Model Evaluator**: We provide interface to evaluate models on well-known benchmarks (e.g. Human-Eval) on popular metrics (e.g., pass@k) with little effort (**~15 LOCs**).
+- **Pretrained Models**: We supply pretrained checkpoints of state-of-the-art foundational language models of code (CodeBERT, CodeT5, CodeGen, CodeT5+, Incoder, StarCoder, etc.).
+- **Fine-Tuned Models**: We furnish fine-tuned checkpoints for 8+ downstream tasks.
+- **Utility to Manipulate Source Code**: We provide utilities to easily manipulate source code, such as user-friendly AST parsers (based on tree-sitter) in **15+ programming languages**, to extract important code features, such as function name, identifiers, etc.
+
+The following table shows the supported models with sizes and the tasks that the models support. This is a continuing effort and we are working on further growing the list.
+    
+| Model        | Size                                                                                                                          | Tasks                                                                                                                                                                                                     |
+|--------------|-------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
+| CodeT5       | Base, Base-multi-sum, Base-translate-cs, Base-translate-java, Base-sum, Base-clone, Base-defect                              | Pretrained, NL to Code, Refine, Translation (CS to Java, Java to CS), Summarization (Python, Go, PHP, JavaScript, Java, Ruby), Clone detection, Defect prediction |
+| CodeT5+      | Plus-instruct-16B, Plus-16B, Plus-6B, Plus-2B, Plus-770M-python, Plus-770M, Plus-220M                                      | Pretrained, NL to Code, Refine , Defect prediction |
+| CodeGen      | Mono: 350M, 2B, 6B, 1B, 3.7B, 7B, 16B<br>Multi: 350M, 2B, 6B<br>NL: 350M, 2B                                           | Pretrained |
+| StarCoder    | 15.5B                                                                                                                         | Pretrained |
+| SantaCoder   | 1.1B                                                                                                                          | Pretrained |
+| GPT-NeoX     | 20B                                                                                                                           | Pretrained |
+| GPT-Neo      | 1.3B                                                                                                                          | Pretrained |
+| GPT-J        | 6B                                                                                                                            | Pretrained |
+| Incoder      | 6B                                                                                                                            | Pretrained |
+| CodeParrot   | Small-python (110M), Small-multi(110M), 1.5B                                                                                   | Pretrained |
+| CodeBERT     | CodeBERT-base, UnixCoder-base, CodeBERTa-small                                                                                 | Pretrained |
+
+
+## Installation Guide
+
+1. (Optional) Creating conda environment
+
+```bash
+conda create -n codetf python=3.8
+conda activate codetf
+```
+
+2. Install from [PyPI](https://pypi.org/project/salesforce-codetf/):
+```bash
+pip install salesforce-codetf
+```
+    
+3. Alternatively, build CodeTF from source:
+
+```bash
+git clone https://github.com/salesforce/CodeTF.git
+cd CodeTF
+pip install -e .
+```
+
+## Getting Started
+### Inferencing Pipeline
+    
+Getting started with CodeTF is simple and quick with our model loading pipeline function ``load_model_pipeline()``. Here's an example showing how to load codet5+ model and perform inference on code generation task:
+    
+```python
+from codetf.models import load_model_pipeline
+
+code_generation_model = load_model_pipeline(model_name="codet5", task="pretrained",
+            model_type="plus-220M", is_eval=True,
+            load_in_8bit=True, weight_sharding=False)
             
-        <p align="center">
-            <br>
-            <img src="assets/logo.png" width="500"/>
-            <br>
-        <p>
-        <div align="center">
-          <a href="https://opensource.org/licenses/BSD-3-Clause">
-          <img alt="license" src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg"/>
-          </a>
-           <a href="https://www.python.org/downloads/release/python-380/">
-          <img alt="license" src="https://img.shields.io/badge/python-3.8+-blue.svg"/>
-          </a> 
-          
-        # CodeTF - A Comprehensive Transformer-based Library for Code LLM & Code Intelligence
-        
-        <!-- 
-        [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/bdqnghi/CodeTF_personal/blob/main/LICENSE)
-        [![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) -->
-         </div>   
-            
-        ## Table of Contents
-          - [Introduction](#introduction)
-          - [Installation](#installation-guide)
-          - [Getting Started](#getting-started)
-          - [Code Utilities](#code-utilities)
-          - [License](#license)
-        
-        ## Introduction
-        CodeTF is a one-stop Python library for code intelligence tasks (AI4Code), provides a seamless interface for training and inferencing on code intelligence tasks like code summarization, translation, and generation. It aims to facilitate easy integration of cutting-edge language models into real-world applications.
-        
-        In addition to the core tasks, CodeTF offers utilities for code manipulation across various languages, including easy extraction of code attributes. Using tree-sitter as its core parser, it enables parsing of attributes such as function names, comments, and variable names. Pre-built libraries for numerous languages are provided, eliminating the need for complicated parser setup. CodeTF thus ensures a user-friendly and accessible environment for code intelligence tasks.
-        
-        The current version of the library offers:
-        
-        - **Fast Model Serving**: We support an easy-to-use interface for rapid inferencing with **pre-quantized models** (int8, int16, float16).
-        - **Fine-Tuning Your Own Models with Custom Datasets**: We provide an API for quickly fine-tuning your own LLMs for code using SOTA techniques for **parameter-efficient fine-tuning** (HuggingFace PEFT) on distributed environments.
-        - **Supported Tasks**: nl2code, code summarization, code completion, code translation, code refinement, clone detection, defect prediction.
-        - **Datasets+**: We have preprocessed well-known benchmarks (**Human-Eval, MBPP, CodeXGLUE, APPS, etc.**) and offer an easy-to-load feature for these datasets.
-        - **Model Evaluator**: We provide interface to evaluate models on well-known benchmarks (e.g. Human-Eval) on popular metrics (e.g., pass@k) with little effort (**~15 LOCs**).
-        - **Pretrained Models**: We supply pretrained checkpoints of state-of-the-art foundational language models of code (CodeBERT, CodeT5, CodeGen, CodeT5+, Incoder, StarCoder, etc.).
-        - **Fine-Tuned Models**: We furnish fine-tuned checkpoints for 8+ downstream tasks.
-        - **Utility to Manipulate Source Code**: We provide utilities to easily manipulate source code, such as user-friendly AST parsers (based on tree-sitter) in **15+ programming languages**, to extract important code features, such as function name, identifiers, etc.
-        
-        Important notes:
-        - CodeTF is designed to complement and enhance the capabilities of HuggingFace, rather than replace it. It serves as a specialized layer specifically tailored for code intelligence tasks, such as fine-tuning language models with code-specific features and evaluating on well-known code intelligence benchmarks. If users require more customization, they are encouraged to write their own training code from scratch.
-        - CodeTF leverages the powerful functionality provided by [Accelerate](https://github.com/huggingface/accelerate) for both inference and training. With Accelerate, users do not need to manually manage GPUs or CPU devices for most operations, allowing for a streamlined and efficient workflow.
-        
-        The following table shows the supported models with sizes and the tasks that the models support. This is a continuing effort and we are working on further growing the list.
-            
-        | Model      | Type              | Size                                      | Tasks                                                                                      |
-        |------------|-------------------|-------------------------------------------|--------------------------------------------------------------------------------------------|
-        | CodeBERT   | Encoder           | Base (160M), Small (84M)                  | Pretrained, MLM                                                                            |
-        | CodeGen    | Decoder           | 350M, 2B, 6B, 16B                         | Pretrained                                                                                 |
-        | SantaCoder | Decoder           | 1.1B                                      | Pretrained                                                                                 |
-        | StarCoder  | Decoder           | 15.5B                                     | Pretrained                                                                                 |
-        | GPT        | Decoder           | j (1.3B), j (6B), Neox (20B)              | Pretrained                                                                                 |
-        | GPT-Neo    | Decoder           | 1.3B                                      | Pretrained                                                                                 |
-        | BLOOM      | Decoder           | 560M, 1.1B, 1.7B, 3B, 7.1B                | Pretrained                                                                                 |
-        | Incoder    | Decoder           | 1B, 6B                                    | Pretrained                                                                                 |
-        | CodeT5     | Encoder-Decoder   | Small (125M), Medium (220M), Large (770M) | Pretrained, Code Sum, Code Generation, Code Refinement, Defect Prediction, Clone Detection |
-        | CodeT5+    | Encoder-Decoder   | 220M, 770M, 2B, 6B, 16B                   | Pretrained                                                                                 |
-        
-        
-        ## Installation Guide
-        
-        1. (Optional) Creating conda environment
-        
-        ```bash
-        conda create -n codetf python=3.8
-        conda activate codetf
-        ```
-        
-        2. Install from [PyPI](https://pypi.org/project/salesforce-codetf/):
-        ```bash
-        pip install codetf
-        ```
-            
-        3. Alternatively, build CodeTF from source:
-        
-        ```bash
-        git clone https://github.com/salesforce/CodeTF.git
-        cd CodeTF
-        pip install -e .
-        ```
-        
-        ## Getting Started
-        ### Inferencing Pipeline
-            
-        Getting started with CodeTF is simple and quick with our model loading pipeline function ``load_model_pipeline()``. Here's an example showing how to load codet5 models and perform inference on code translation and code summarization:
-            
-        ```python
-        from codetf.models import load_model_pipeline
-        
-        translation_model = load_model_pipeline(model_name="codet5", task="translate-cs-java",
-                    model_type="base", is_eval=True,
-                    load_in_8bit=True, weight_sharding=False)
-        
-        summarization_model = load_model_pipeline(model_name="codet5", task="sum-python",
-                    model_type="base", is_eval=True,
-                    load_in_8bit=True, weight_sharding=False)
-        
-        code_snippets = """
-            void bubbleSort(int arr[])
-            {
-                int n = arr.length;
-                for (int i = 0; i < n - 1; i++)
-                    for (int j = 0; j < n - i - 1; j++)
-                        if (arr[j] > arr[j + 1]) {
-                            // swap arr[j+1] and arr[j]
-                            int temp = arr[j];
-                            arr[j] = arr[j + 1];
-                            arr[j + 1] = temp;
-                        }
-            }
-        """
-        
-        translated_code_snippets = translation_model.predict([code_snippets])
-        
-        print(translated_code_snippets)
-        
-        summaries = summarization_model.predict([code_snippets])
-        print(summaries)
-        ```
-        There are a few notable arguments that need to be considered:
-        -  ``model_name``: the name of the model, currently support ``codet5`` and ``causal-lm``. 
-        -  ``model_type``: type of model for each model name, e.g. ``base``, ``codegen-350M-mono``, ``j-6B``, etc.
-        -  ``load_in_8bit``: inherit the ``load_in_8bit" feature from [Huggingface Quantization](https://huggingface.co/docs/transformers/main/main_classes/quantization).
-        -  ``weight_sharding``: our advance feature that leverate [HuggingFace Sharded Checkpoint](https://huggingface.co/docs/accelerate/v0.19.0/en/package_reference/big_modeling#accelerate.load_checkpoint_and_dispatch) to split a large model in several smaller shards in different GPUs. Please consider using this if you are dealing with large models.
-        
-        ### Training Custom Model Using Our Trainer
-        Want to train a custom LLM for code? We've got you covered. Below is an example using the ``CausalLMTrainer``, along with our dataset utilities, make it easy to fine-tune your models using the CodeXGLUE dataset. Here's an example:
-            
-        ```python
-        from codetf.trainer.causal_lm_trainer import CausalLMTrainer
-        from codetf.data_utility.codexglue_dataset import CodeXGLUEDataset
-        from codetf.models import load_model_pipeline
-        from codetf.performance.evaluate import EvaluationMetric
-        
-        model_class = load_model_pipeline(model_name="causal-lm", task="pretrained",
-                        model_type="starcoder-15.5B", is_eval=False,
-                        load_in_8bit=False, weight_sharding=False)
-        
-        
-        dataloader = CodeXGLUEDataset(tokenizer=model_class.get_tokenizer())
-        train_dataset, test_dataset, val_dataset = dataloader.load(subset="text-to-code")
-        
-        evaluator = EvaluationMetric(metric="bleu", tokenizer=model_class.tokenizer)
-        
-        # peft can be in ["lora", "prefixtuning"]
-        trainer = CausalLMTrainer(train_dataset=train_dataset, 
+result = code_generation_model.predict(["def print_hello_world():"])
+print(result)
+```
+There are a few notable arguments that need to be considered:
+-  ``model_name``: the name of the model, currently support ``codet5`` and ``causal-lm``. 
+-  ``model_type``: type of model for each model name, e.g. ``base``, ``codegen-350M-mono``, ``j-6B``, etc.
+-  ``load_in_8bit``: inherit the ``load_in_8bit" feature from [Huggingface Quantization](https://huggingface.co/docs/transformers/main/main_classes/quantization).
+-  ``weight_sharding``: our advance feature that leverate [HuggingFace Sharded Checkpoint](https://huggingface.co/docs/accelerate/v0.19.0/en/package_reference/big_modeling#accelerate.load_checkpoint_and_dispatch) to split a large model in several smaller shards in different GPUs. Please consider using this if you are dealing with large models.
+
+### Model Zoo
+You might want to view all of the supported models. To do this, you can use the ``model_zoo()``:
+```python
+from codetf.models import model_zoo
+print(model_zoo)
+# ============================================================================================================
+# Architectures                  Types                           Tasks
+# ============================================================================================================
+# causallm                       codegen-350M-mono              pretrained
+#                                codegen-350M-multi             pretrained
+#                                codegen-350M-nl                pretrained
+#                                codegen-2B-mono                pretrained
+#                                codegen-2B-multi               pretrained
+#                                codegen-2B-nl                  pretrained
+#                                codegen-6B-mono                pretrained
+#                                codegen-6B-nl                  pretrained
+#                                codegen-6B-multi               pretrained
+#                                starcoder-15.5B                pretrained
+#                                gpt-neox-20B                   pretrained
+#                                gpt-neo-1.3B                   pretrained
+#                                gpt-j-6B                       pretrained
+#                                incoder-6B                     pretrained
+#                                codegen2-1B                    pretrained
+#                                codegen2-3.7B                  pretrained
+#                                codegen2-7B                    pretrained
+#                                codegen2-16B                   pretrained
+# codet5                         base-multi-sum                 pretrained
+#                                base                           nl2code
+#                                base                           refine
+#                                base                           translate_cs_java
+#                                base                           translate_java_cs
+#                                base                           sum_python
+#                                base                           sum_go
+#                                base                           sum_php
+#                                base                           sum_javascript
+#                                base                           sum_java
+#                                base                           sum_ruby
+#                                base                           clone
+#                                base                           defect
+#                                plus-instruct-16B              pretrained
+#                                plus-16B                       pretrained
+#                                plus-6B                        pretrained
+#                                plus-2B                        pretrained
+#                                plus-770M-python               pretrained
+#                                plus-770M                      pretrained
+#                                plus-220M                      pretrained
+# bert                           codebert-base                  pretrained
+#                                unixcoder-base                 pretrained
+#                                codeberta-small                pretrained
+```
+
+### Fine-Tuning Pipeline
+Want to train a custom LLM for code? We've got you covered. Below is an example using the ``Seq2SeqTrainer`` to fine-tune a [CodeT5+ pretrained model](https://github.com/salesforce/CodeT5), along with our dataset utilities, make it easy to fine-tune your models using the CodeXGLUE dataset. Here's an example:
+    
+```python
+from codetf.trainer.codet5_trainer import CodeT5Seq2SeqTrainer
+from codetf.data_utility.codexglue_dataset import CodeXGLUEDataset
+from codetf.models import load_model_pipeline
+from codetf.performance.evaluation_metric import EvaluationMetric
+from codetf.data_utility.base_dataset import CustomDataset
+
+model_class = load_model_pipeline(model_name="codet5", task="pretrained",
+            model_type="plus-220M", is_eval=True)
+
+dataset = CodeXGLUEDataset(tokenizer=model_class.get_tokenizer())
+train, test, validation = dataset.load(subset="text-to-code")
+
+train_dataset= CustomDataset(train[0], train[1])
+test_dataset= CustomDataset(test[0], test[1])
+val_dataset= CustomDataset(validation[0], validation[1])
+
+evaluator = EvaluationMetric(metric="bleu", tokenizer=model_class.tokenizer)
+
+# peft can be in ["lora", "prefixtuning"]
+trainer = CodeT5Seq2SeqTrainer(train_dataset=train_dataset, 
                                 validation_dataset=val_dataset, 
-                                peft=None,
+                                peft="lora",
                                 pretrained_model_or_path=model_class.get_model(),
-                                tokenizer=model_class.get_tokenizer())
-        trainer.train()
-        # trainer.evaluate(test_dataset=test_dataset)
-        ```
-        
-        Comparing to [this script from StarCoder](https://github.com/bigcode-project/starcoder/blob/main/finetune/finetune.py), which requires ~300 LOCs to fine-tune a model, we only need 14 LOCs to do the same !!!
-        
-        
-        ### Evaluate on Well-Known Benchmarks
-        Planning to reproduce the results of well-known benchmarks like ``Human-Eval``, but struggling with not achieving the same numbers as reported in the original papers? Worried about the complicated evaluation process? Don't worry, we've got you covered with an intuitive, easy-to-use interface. Here's a sample snippet demonstrating how to evaluate Human Eval using pass@k (k=[1,10,100]) as the metric:
-        ```
-        from codetf.models import load_model_pipeline
-        from codetf.data_utility.human_eval_dataset import HumanEvalDataset
-        from codetf.performance.model_evaluator import ModelEvaluator
-        
-        os.environ["HF_ALLOW_CODE_EVAL"] = "1"
-        os.environ["TOKENIZERS_PARALLELISM"] = "true"
-        
-        model_class = load_model_pipeline(model_name="causal-lm", task="pretrained",
-                    model_type="codegen-350M-mono", is_eval=True,
-                    load_in_8bit=True, weight_sharding=False)
-        
-        dataset = HumanEvalDataset(tokenizer=model_class.get_tokenizer())
-        prompt_token_ids, prompt_attention_masks, references= dataset.load()
-        
-        problems = TensorDataset(prompt_token_ids, prompt_attention_masks)
-        
-        evaluator = ModelEvaluator(model_class)
-        avg_pass_at_k = evaluator.evaluate_pass_k(problems=problems, unit_tests=references)
-        print("Pass@k: ", avg_pass_at_k)
-        ```
-        
-        Comparing to [this script from HuggingFace](https://github.com/huggingface/transformers/blob/main/examples/research_projects/codeparrot/scripts/human_eval.py), which requires ~230 LOCs to evaluate on pass@k, we only need 14 LOCs to do the same !!!
-        
-        ### Loading Preprocessed Data
-        CodeTF provides the Dataset utility for several well-known datasets, such as CodeXGLUE, Human Eval, MBPP, and APPS. The following is an example of how to load the CodeXGLUE dataset:  
-        
-        ```python
-        from codetf.data_utility.codexglue_dataset import CodeXGLUEDataset
-        from transformers import RobertaTokenizer
-        
-        tokenizer = RobertaTokenizer.from_pretrained("Salesforce/codet5-base", use_fast=True)
-        dataset = CodeXGLUEDataset(tokenizer=tokenizer)
-        train, test, validation = dataset.load(subset="text-to-code")
-        ```
-        
-        The ``train``, ``test``, ``validation`` are returned in form of [Pytorch tensor](https://pytorch.org/docs/stable/tensors.html) to provide the flexilbity for the users to wrap it into higher-lever wrapper for their own use cases.
-        
-        ### Code Utilities
-        In addition to providing utilities for LLMs, CodeTF also equips users with tools for effective source code manipulation. This is crucial in the code intelligence pipeline, where operations like parsing code into an Abstract Syntax Tree (AST) or extracting code attributes (such as function names or identifiers) are often required (CodeT5). These tasks can be challenging to execute, especially when setup and multi-language support is needed. Our code utility interface offers a streamlined solution, facilitating easy parsing and attribute extraction from code across 15+ languages.
-        
-        
-        #### AST Parser in Multiple Languages
-        
-        CodeTF includes AST parsers compatible with numerous programming languages. Here's an example showcasing the parsing of Apex code into an AST:
-        ```python
-        from codetf.code_utility.apex.apex_code_utility import ApexCodeUtility
-        
-        apex_code_utility = ApexCodeUtility()
-        
-        sample_code = """
-            public class SampleClass {    
-                public Integer myNumber;
-                
-                **
-                * This is a method that returns the value of myNumber.
-                * @return An integer value
-                */
-                public Integer getMyNumber() {
-                    // Return the current value of myNumber
-                    return this.myNumber;
-                }
-            }
-        """
-        ast = apex_code_utility.parse(sample_code)
-        
-        # This will print the tree-sitter AST object
-        print(ast)
-        ```
-        
-        Then you can traverse the tree using the interface from [py-tree-sitter](https://github.com/tree-sitter/py-tree-sitter
-        ```
-        root_node = ast.root_node
-        assert root_node.type == 'module'
-        assert root_node.start_point == (1, 0)
-        assert root_node.end_point == (3, 13)
-        ```
-        
-        There are also other utilities for Java, Python, etc, that can perform the same operations. 
-        
-        #### Extract Code Attributes
-        
-        CodeTF provides an interface to easily extract code attributes. The following is a sample for extracting the function name of a Python function:
-        
-        ```python
-        code_attributes = apex_code_utility.get_code_attributes(sample_code)
-        print(code_attributes)
-        ```
-        
-        This will print:
-        ``
-        {'class_names': ['AccountWithContacts'], 'method_names': ['getAccountsWithContacts'], 'comments': [], 'variable_names': ['acc', 'accounts', 'con', 'System', 'debug', 'Contacts', 'Id', 'Name', 'Account', 'Email', 'LastName']}
-        ``
-        
-        ### Remove Comments
-        There are other existing utilities, such as removing comments from code:
-        ```python
-        new_code_snippet = apex_code_utility.remove_comments(sample_code)
-        print(new_code_snippet)
-        ```
-        
-        This will print:
-        ```
-        public class SampleClass {    
-                public Integer myNumber;
-                public Integer getMyNumber() {
-                    // Return the current value of myNumber
-                    return this.myNumber;
-                }
-            }
-         ```
-        
-        Note that this is an ongoing process, we will add more features to extract complicated code attributes in the future. More examples can be found [here](https://github.com/salesforce/CodeTF/tree/main/test_code_utilities).
-        
-        ## More Examples
-        You can find more examples for each use case:
-        - [Fine-tuning](https://github.com/salesforce/CodeTF/tree/main/test_trainer)
-        - [Inferencing](https://github.com/salesforce/CodeTF/tree/main/test_inference)
-        - [Model Evaluate](https://github.com/salesforce/CodeTF/tree/main/test_evaluator)
-        - [Code Utility](https://github.com/salesforce/CodeTF/tree/main/test_code_utilities)
-        
-        ## Technical Report and Citing CodeTF
-        You can find more details in our [technical report](https://arxiv.org/abs/2209.09019).
-        
-        If you're using CodeTF in your research or applications, please cite using this BibTeX:
-        ```bibtex
-        @misc{nghi2023codetf,
-              title={CodeTF: A Transformer-based Library for CodeLLM & Code Intelligence}, 
-              author={Nghi D. Q. Bui, Henry Le, Yue Wang, Akhilesh Deepak Gotmare, Junna Li, Steven Hoi.},
-              year={2023},
-              eprint={2209.09019},
-              archivePrefix={arXiv},
-              primaryClass={cs.CV}
+                                tokenizer=model_class.tokenizer)
+trainer.train()
+```
+
+Comparing to [this script from StarCoder](https://github.com/bigcode-project/starcoder/blob/main/finetune/finetune.py), which requires ~300 LOCs to fine-tune a model, we only need 14 LOCs to do the same !!!
+
+
+### Evaluate on Well-Known Benchmarks
+Planning to reproduce the results of well-known benchmarks like ``Human-Eval``, but struggling with not achieving the same numbers as reported in the original papers? Worried about the complicated evaluation process? Don't worry, we've got you covered with an intuitive, easy-to-use interface. Here's a sample snippet demonstrating how to evaluate Human Eval using pass@k (k=[1,10,100]) as the metric:
+```python
+from codetf.models import load_model_pipeline
+from codetf.data_utility.human_eval_dataset import HumanEvalDataset
+from codetf.performance.model_evaluator import ModelEvaluator
+
+os.environ["HF_ALLOW_CODE_EVAL"] = "1"
+os.environ["TOKENIZERS_PARALLELISM"] = "true"
+
+model_class = load_model_pipeline(model_name="causal-lm", task="pretrained",
+            model_type="codegen-350M-mono", is_eval=True,
+            load_in_8bit=True, weight_sharding=False)
+
+dataset = HumanEvalDataset(tokenizer=model_class.get_tokenizer())
+prompt_token_ids, prompt_attention_masks, references= dataset.load()
+
+problems = TensorDataset(prompt_token_ids, prompt_attention_masks)
+
+evaluator = ModelEvaluator(model_class)
+avg_pass_at_k = evaluator.evaluate_pass_k(problems=problems, unit_tests=references)
+print("Pass@k: ", avg_pass_at_k)
+```
+
+Comparing to [this script from HuggingFace](https://github.com/huggingface/transformers/blob/main/examples/research_projects/codeparrot/scripts/human_eval.py), which requires ~230 LOCs to evaluate on pass@k, we only need 14 LOCs to do the same !!!
+
+### Loading Preprocessed Data
+CodeTF provides the Dataset utility for several well-known datasets, such as CodeXGLUE, Human Eval, MBPP, and APPS. The following is an example of how to load the CodeXGLUE dataset:  
+
+```python
+from codetf.data_utility.codexglue_dataset import CodeXGLUEDataset
+from transformers import RobertaTokenizer
+
+tokenizer = RobertaTokenizer.from_pretrained("Salesforce/codet5-base", use_fast=True)
+dataset = CodeXGLUEDataset(tokenizer=tokenizer)
+train, test, validation = dataset.load(subset="text-to-code")
+```
+
+The ``train``, ``test``, ``validation`` are returned in form of [Pytorch tensor](https://pytorch.org/docs/stable/tensors.html) to provide the flexilbity for the users to wrap it into higher-lever wrapper for their own use cases.
+
+### Code Utilities
+In addition to providing utilities for LLMs, CodeTF also equips users with tools for effective source code manipulation. This is crucial in the code intelligence pipeline, where operations like parsing code into an Abstract Syntax Tree (AST) or extracting code attributes (such as function names or identifiers) are often required (CodeT5). These tasks can be challenging to execute, especially when setup and multi-language support is needed. Our code utility interface offers a streamlined solution, facilitating easy parsing and attribute extraction from code across 15+ languages.
+
+
+#### AST Parser in Multiple Languages
+
+CodeTF includes AST parsers compatible with numerous programming languages. Here's an example showcasing the parsing of Apex code into an AST:
+```python
+from codetf.code_utility.apex.apex_code_utility import ApexCodeUtility
+
+apex_code_utility = ApexCodeUtility()
+
+sample_code = """
+    public class SampleClass {    
+        public Integer myNumber;
+        
+        **
+        * This is a method that returns the value of myNumber.
+        * @return An integer value
+        */
+        public Integer getMyNumber() {
+            // Return the current value of myNumber
+            return this.myNumber;
         }
-        ```
-                  |
-        ## Contact us
-        If you have any questions, comments or suggestions, please do not hesitate to contact us at codetf@salesforce.com.
-        
-        ## License
-        [BSD 3-Clause License](LICENSE.txt)
-        
-Keywords: AI4Code,Code Intelligence,Generative AI,Deep Learning,Library,PyTorch,HuggingFace
-Platform: UNKNOWN
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
+    }
+"""
+ast = apex_code_utility.parse(sample_code)
+
+# This will print the tree-sitter AST object
+print(ast)
+```
+
+Then you can traverse the tree using the interface from [py-tree-sitter](https://github.com/tree-sitter/py-tree-sitter)
+```
+root_node = ast.root_node
+assert root_node.type == 'module'
+assert root_node.start_point == (1, 0)
+assert root_node.end_point == (3, 13)
+```
+
+There are also other utilities for Java, Python, etc, that can perform the same operations. 
+
+#### Extract Code Attributes
+
+CodeTF provides an interface to easily extract code attributes. The following is a sample for extracting the function name of a Python function:
+
+```python
+code_attributes = apex_code_utility.get_code_attributes(sample_code)
+print(code_attributes)
+```
+
+This will print:
+``
+{'class_names': ['AccountWithContacts'], 'method_names': ['getAccountsWithContacts'], 'comments': [], 'variable_names': ['acc', 'accounts', 'con', 'System', 'debug', 'Contacts', 'Id', 'Name', 'Account', 'Email', 'LastName']}
+``
+
+### Remove Comments
+There are other existing utilities, such as removing comments from code:
+```python
+new_code_snippet = apex_code_utility.remove_comments(sample_code)
+print(new_code_snippet)
+```
+
+This will print:
+```java
+public class SampleClass {    
+        public Integer myNumber;
+        public Integer getMyNumber() {
+            return this.myNumber;
+        }
+    }
+ ```
+
+Note that this is an ongoing process, we will add more features to extract complicated code attributes in the future. More examples can be found [here](https://github.com/salesforce/CodeTF/tree/main/test_code_utilities).
+
+## More Examples
+You can find more examples for each use case:
+- [Fine-tuning](https://github.com/salesforce/CodeTF/tree/main/test_trainer)
+- [Inferencing](https://github.com/salesforce/CodeTF/tree/main/test_inference)
+- [Model Evaluate](https://github.com/salesforce/CodeTF/tree/main/test_evaluator)
+- [Code Utility](https://github.com/salesforce/CodeTF/tree/main/test_code_utilities)
+
+## Notes
+- CodeTF is designed to complement and enhance the capabilities of [HuggingFace Transformers](https://huggingface.co/docs/transformers/index), rather than replace it. It serves as a specialized layer specifically tailored for code intelligence tasks, such as fine-tuning language models with code-specific features and evaluating on well-known code intelligence benchmarks. If users require more customization, they are encouraged to write their own training code from scratch.
+- CodeTF leverages the powerful functionality provided by [Accelerate](https://github.com/huggingface/accelerate) for both inference and training. With Accelerate, users do not need to manually manage GPUs or CPU devices for most operations, allowing for a streamlined and efficient workflow.
+
+## Ethical and Responsible Use
+CodeTF, while powerful, does not guarantee infallible code intelligence capabilities. Users may encounter inaccuracies or biases, possibly leading to misinterpretations or undesired behaviors. Risks include the generation of insecure code, propagation of poor coding practices, or inadvertent revelation of sensitive data. We strongly advise users to examine the pretrained models and system before practical adoption. CodeTF facilitates effective code analysis, prediction, and debugging, promoting reproducible research and development. We encourage its responsible use for enhancing software quality and developer productivity.
+
+However, misuse can lead to unethical outcomes such as unauthorized code manipulation, privacy breaches, or insecure coding practices. Users should familiarize themselves with guidelines for responsible AI before using CodeTF. Our commitment is to continually refine the library by identifying and mitigating potential biases and inappropriate behaviors. Users should review the models and system before practical implementation, and contribute towards refining the library to ensure ethical usage.
+
+## Technical Report and Citing CodeTF
+You can find more details in our [technical report](https://arxiv.org).
+
+If you're using CodeTF in your research or applications, please cite using this BibTeX:
+```bibtex
+@misc{nghi2023codetf,
+      title={CodeTF: A Transformer-based Library for CodeLLM & Code Intelligence}, 
+      author={Nghi D. Q. Bui, Henry Le, Yue Wang, Akhilesh Deepak Gotmare, Junnan Li, Steven Hoi.},
+      year={2023},
+      eprint={2209.09019},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+```
+
+## Contact us
+If you have any questions, comments or suggestions, please do not hesitate to contact us at codetf@salesforce.com.
+
+## License
+[Apache License Version 2.0](LICENSE.txt)
```

#### html2text {}

```diff
@@ -1,125 +1,143 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.3 Summary: CodeTF: A
-Transformer-based Library for Code Intelligence Home-page: https://github.com/
-Salesforce/CodeTF Author: Nghi D. Q. Bui License: 3-Clause BSD Description:
 
                               [assets/logo.png]
- [license] [license] # CodeTF - A Comprehensive Transformer-based Library for
-                         Code LLM & Code Intelligence
+  [license] [license] [license] Technical_Report, Documentation, Examples, #
+    CodeTF - A One-stop Transformer Library for State-of-the-art Code LLM
 ## Table of Contents - [Introduction](#introduction) - [Installation]
-(#installation-guide) - [Getting Started](#getting-started) - [Code Utilities]
-(#code-utilities) - [License](#license) ## Introduction CodeTF is a one-stop
-Python library for code intelligence tasks (AI4Code), provides a seamless
+(#installation-guide) - [Getting Started](#getting-started) - [Inferencing
+Pipeline](#inferencing-pipeline) - [Model Zoo](#model-zoo) - [Fine-Tuning Your
+Own Model](#fine-tuning-pipeline) - [Evaluate On Well-Known Benchmarks]
+(#evaluate-on-well-known-benchmarks) - [Utilities to Manipulate Source Code
+Based on AST](#code-utilities) - [AST Parser in Multiple Languages](#ast-
+parser-in-multiple-languages) - [Extract Code Attributes](#extract-code-
+attributes) - [Remove Comments](#remove-comments) - [Ethical and Responsible
+Use](#ethical-and-responsible-use) - [License](#license) ## Introduction CodeTF
+is a one-stop Python transformer-based library for ***code large language
+models (Code LLMs)*** and ***code intelligence***, provides a seamless
 interface for training and inferencing on code intelligence tasks like code
-summarization, translation, and generation. It aims to facilitate easy
-integration of cutting-edge language models into real-world applications. In
-addition to the core tasks, CodeTF offers utilities for code manipulation
-across various languages, including easy extraction of code attributes. Using
-tree-sitter as its core parser, it enables parsing of attributes such as
-function names, comments, and variable names. Pre-built libraries for numerous
-languages are provided, eliminating the need for complicated parser setup.
-CodeTF thus ensures a user-friendly and accessible environment for code
-intelligence tasks. The current version of the library offers: - **Fast Model
-Serving**: We support an easy-to-use interface for rapid inferencing with
-**pre-quantized models** (int8, int16, float16). - **Fine-Tuning Your Own
-Models with Custom Datasets**: We provide an API for quickly fine-tuning your
-own LLMs for code using SOTA techniques for **parameter-efficient fine-tuning**
-(HuggingFace PEFT) on distributed environments. - **Supported Tasks**: nl2code,
-code summarization, code completion, code translation, code refinement, clone
+summarization, translation, code generation and so on. It aims to facilitate
+easy integration of SOTA CodeLLMs into real-world applications. In addition to
+the core LLMs's features for code, CodeTF offers utilities for code
+manipulation across various languages, including easy extraction of code
+attributes. Using tree-sitter as its core AST parser, it enables parsing of
+attributes such as function names, comments, and variable names. Pre-built
+libraries for numerous languages are provided, eliminating the need for
+complicated parser setup. CodeTF thus ensures a user-friendly and accessible
+environment for code intelligence tasks. The current version of the library
+offers: - **Fast Model Serving**: We support an easy-to-use interface for rapid
+inferencing with **pre-quantized models** (int8, int16, float16). CodeTF
+handles all aspects of device management, so users do not have to worry about
+that aspect. If your model is large, we offer advanced features such as weight
+sharding across GPUs to serve the models more quickly. - **Fine-Tuning Your Own
+Models**: We provide an API for quickly fine-tuning your own LLMs for code
+using SOTA techniques for **parameter-efficient fine-tuning** (HuggingFace
+PEFT) on distributed environments. - **Supported Tasks**: nl2code, code
+summarization, code completion, code translation, code refinement, clone
 detection, defect prediction. - **Datasets+**: We have preprocessed well-known
 benchmarks (**Human-Eval, MBPP, CodeXGLUE, APPS, etc.**) and offer an easy-to-
 load feature for these datasets. - **Model Evaluator**: We provide interface to
 evaluate models on well-known benchmarks (e.g. Human-Eval) on popular metrics
 (e.g., pass@k) with little effort (**~15 LOCs**). - **Pretrained Models**: We
 supply pretrained checkpoints of state-of-the-art foundational language models
 of code (CodeBERT, CodeT5, CodeGen, CodeT5+, Incoder, StarCoder, etc.). -
 **Fine-Tuned Models**: We furnish fine-tuned checkpoints for 8+ downstream
 tasks. - **Utility to Manipulate Source Code**: We provide utilities to easily
 manipulate source code, such as user-friendly AST parsers (based on tree-
 sitter) in **15+ programming languages**, to extract important code features,
-such as function name, identifiers, etc. Important notes: - CodeTF is designed
-to complement and enhance the capabilities of HuggingFace, rather than replace
-it. It serves as a specialized layer specifically tailored for code
-intelligence tasks, such as fine-tuning language models with code-specific
-features and evaluating on well-known code intelligence benchmarks. If users
-require more customization, they are encouraged to write their own training
-code from scratch. - CodeTF leverages the powerful functionality provided by
-[Accelerate](https://github.com/huggingface/accelerate) for both inference and
-training. With Accelerate, users do not need to manually manage GPUs or CPU
-devices for most operations, allowing for a streamlined and efficient workflow.
-The following table shows the supported models with sizes and the tasks that
-the models support. This is a continuing effort and we are working on further
-growing the list. | Model | Type | Size | Tasks | |------------|---------------
-----|-------------------------------------------|------------------------------
---------------------------------------------------------------| | CodeBERT |
-Encoder | Base (160M), Small (84M) | Pretrained, MLM | | CodeGen | Decoder |
-350M, 2B, 6B, 16B | Pretrained | | SantaCoder | Decoder | 1.1B | Pretrained | |
-StarCoder | Decoder | 15.5B | Pretrained | | GPT | Decoder | j (1.3B), j (6B),
-Neox (20B) | Pretrained | | GPT-Neo | Decoder | 1.3B | Pretrained | | BLOOM |
-Decoder | 560M, 1.1B, 1.7B, 3B, 7.1B | Pretrained | | Incoder | Decoder | 1B,
-6B | Pretrained | | CodeT5 | Encoder-Decoder | Small (125M), Medium (220M),
-Large (770M) | Pretrained, Code Sum, Code Generation, Code Refinement, Defect
-Prediction, Clone Detection | | CodeT5+ | Encoder-Decoder | 220M, 770M, 2B, 6B,
-16B | Pretrained | ## Installation Guide 1. (Optional) Creating conda
-environment ```bash conda create -n codetf python=3.8 conda activate codetf ```
-2. Install from [PyPI](https://pypi.org/project/salesforce-codetf/): ```bash
-pip install codetf ``` 3. Alternatively, build CodeTF from source: ```bash git
-clone https://github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ```
-## Getting Started ### Inferencing Pipeline Getting started with CodeTF is
-simple and quick with our model loading pipeline function ``load_model_pipeline
-()``. Here's an example showing how to load codet5 models and perform inference
-on code translation and code summarization: ```python from codetf.models import
-load_model_pipeline translation_model = load_model_pipeline
-(model_name="codet5", task="translate-cs-java", model_type="base",
-is_eval=True, load_in_8bit=True, weight_sharding=False) summarization_model =
-load_model_pipeline(model_name="codet5", task="sum-python", model_type="base",
-is_eval=True, load_in_8bit=True, weight_sharding=False) code_snippets = """
-void bubbleSort(int arr[]) { int n = arr.length; for (int i = 0; i < n - 1;
-i++) for (int j = 0; j < n - i - 1; j++) if (arr[j] > arr[j + 1]) { // swap arr
-[j+1] and arr[j] int temp = arr[j]; arr[j] = arr[j + 1]; arr[j + 1] = temp; } }
-""" translated_code_snippets = translation_model.predict([code_snippets]) print
-(translated_code_snippets) summaries = summarization_model.predict(
-[code_snippets]) print(summaries) ``` There are a few notable arguments that
-need to be considered: - ``model_name``: the name of the model, currently
+such as function name, identifiers, etc. The following table shows the
+supported models with sizes and the tasks that the models support. This is a
+continuing effort and we are working on further growing the list. | Model |
+Size | Tasks | |--------------|------------------------------------------------
+-------------------------------------------------------------------------------
+|------------------------------------------------------------------------------
+-------------------------------------------------------------------| | CodeT5 |
+Base, Base-multi-sum, Base-translate-cs, Base-translate-java, Base-sum, Base-
+clone, Base-defect | Pretrained, NL to Code, Refine, Translation (CS to Java,
+Java to CS), Summarization (Python, Go, PHP, JavaScript, Java, Ruby), Clone
+detection, Defect prediction | | CodeT5+ | Plus-instruct-16B, Plus-16B, Plus-
+6B, Plus-2B, Plus-770M-python, Plus-770M, Plus-220M | Pretrained, NL to Code,
+Refine , Defect prediction | | CodeGen | Mono: 350M, 2B, 6B, 1B, 3.7B, 7B, 16B
+Multi: 350M, 2B, 6B
+NL: 350M, 2B | Pretrained | | StarCoder | 15.5B | Pretrained | | SantaCoder |
+1.1B | Pretrained | | GPT-NeoX | 20B | Pretrained | | GPT-Neo | 1.3B |
+Pretrained | | GPT-J | 6B | Pretrained | | Incoder | 6B | Pretrained | |
+CodeParrot | Small-python (110M), Small-multi(110M), 1.5B | Pretrained | |
+CodeBERT | CodeBERT-base, UnixCoder-base, CodeBERTa-small | Pretrained | ##
+Installation Guide 1. (Optional) Creating conda environment ```bash conda
+create -n codetf python=3.8 conda activate codetf ``` 2. Install from [PyPI]
+(https://pypi.org/project/salesforce-codetf/): ```bash pip install salesforce-
+codetf ``` 3. Alternatively, build CodeTF from source: ```bash git clone https:
+//github.com/salesforce/CodeTF.git cd CodeTF pip install -e . ``` ## Getting
+Started ### Inferencing Pipeline Getting started with CodeTF is simple and
+quick with our model loading pipeline function ``load_model_pipeline()``.
+Here's an example showing how to load codet5+ model and perform inference on
+code generation task: ```python from codetf.models import load_model_pipeline
+code_generation_model = load_model_pipeline(model_name="codet5",
+task="pretrained", model_type="plus-220M", is_eval=True, load_in_8bit=True,
+weight_sharding=False) result = code_generation_model.predict(["def
+print_hello_world():"]) print(result) ``` There are a few notable arguments
+that need to be considered: - ``model_name``: the name of the model, currently
 support ``codet5`` and ``causal-lm``. - ``model_type``: type of model for each
 model name, e.g. ``base``, ``codegen-350M-mono``, ``j-6B``, etc. -
 ``load_in_8bit``: inherit the ``load_in_8bit" feature from [Huggingface
 Quantization](https://huggingface.co/docs/transformers/main/main_classes/
 quantization). - ``weight_sharding``: our advance feature that leverate
 [HuggingFace Sharded Checkpoint](https://huggingface.co/docs/accelerate/
 v0.19.0/en/package_reference/
 big_modeling#accelerate.load_checkpoint_and_dispatch) to split a large model in
 several smaller shards in different GPUs. Please consider using this if you are
-dealing with large models. ### Training Custom Model Using Our Trainer Want to
-train a custom LLM for code? We've got you covered. Below is an example using
-the ``CausalLMTrainer``, along with our dataset utilities, make it easy to
-fine-tune your models using the CodeXGLUE dataset. Here's an example: ```python
-from codetf.trainer.causal_lm_trainer import CausalLMTrainer from
+dealing with large models. ### Model Zoo You might want to view all of the
+supported models. To do this, you can use the ``model_zoo()``: ```python from
+codetf.models import model_zoo print(model_zoo) #
+============================================================================================================
+# Architectures Types Tasks #
+============================================================================================================
+# causallm codegen-350M-mono pretrained # codegen-350M-multi pretrained #
+codegen-350M-nl pretrained # codegen-2B-mono pretrained # codegen-2B-multi
+pretrained # codegen-2B-nl pretrained # codegen-6B-mono pretrained # codegen-
+6B-nl pretrained # codegen-6B-multi pretrained # starcoder-15.5B pretrained #
+gpt-neox-20B pretrained # gpt-neo-1.3B pretrained # gpt-j-6B pretrained #
+incoder-6B pretrained # codegen2-1B pretrained # codegen2-3.7B pretrained #
+codegen2-7B pretrained # codegen2-16B pretrained # codet5 base-multi-sum
+pretrained # base nl2code # base refine # base translate_cs_java # base
+translate_java_cs # base sum_python # base sum_go # base sum_php # base
+sum_javascript # base sum_java # base sum_ruby # base clone # base defect #
+plus-instruct-16B pretrained # plus-16B pretrained # plus-6B pretrained # plus-
+2B pretrained # plus-770M-python pretrained # plus-770M pretrained # plus-220M
+pretrained # bert codebert-base pretrained # unixcoder-base pretrained #
+codeberta-small pretrained ``` ### Fine-Tuning Pipeline Want to train a custom
+LLM for code? We've got you covered. Below is an example using the
+``Seq2SeqTrainer`` to fine-tune a [CodeT5+ pretrained model](https://
+github.com/salesforce/CodeT5), along with our dataset utilities, make it easy
+to fine-tune your models using the CodeXGLUE dataset. Here's an example:
+```python from codetf.trainer.codet5_trainer import CodeT5Seq2SeqTrainer from
 codetf.data_utility.codexglue_dataset import CodeXGLUEDataset from
-codetf.models import load_model_pipeline from codetf.performance.evaluate
-import EvaluationMetric model_class = load_model_pipeline(model_name="causal-
-lm", task="pretrained", model_type="starcoder-15.5B", is_eval=False,
-load_in_8bit=False, weight_sharding=False) dataloader = CodeXGLUEDataset
-(tokenizer=model_class.get_tokenizer()) train_dataset, test_dataset,
-val_dataset = dataloader.load(subset="text-to-code") evaluator =
-EvaluationMetric(metric="bleu", tokenizer=model_class.tokenizer) # peft can be
-in ["lora", "prefixtuning"] trainer = CausalLMTrainer
-(train_dataset=train_dataset, validation_dataset=val_dataset, peft=None,
-pretrained_model_or_path=model_class.get_model(),
-tokenizer=model_class.get_tokenizer()) trainer.train() # trainer.evaluate
-(test_dataset=test_dataset) ``` Comparing to [this script from StarCoder]
-(https://github.com/bigcode-project/starcoder/blob/main/finetune/finetune.py),
-which requires ~300 LOCs to fine-tune a model, we only need 14 LOCs to do the
-same !!! ### Evaluate on Well-Known Benchmarks Planning to reproduce the
-results of well-known benchmarks like ``Human-Eval``, but struggling with not
-achieving the same numbers as reported in the original papers? Worried about
-the complicated evaluation process? Don't worry, we've got you covered with an
-intuitive, easy-to-use interface. Here's a sample snippet demonstrating how to
-evaluate Human Eval using pass@k (k=[1,10,100]) as the metric: ``` from
 codetf.models import load_model_pipeline from
+codetf.performance.evaluation_metric import EvaluationMetric from
+codetf.data_utility.base_dataset import CustomDataset model_class =
+load_model_pipeline(model_name="codet5", task="pretrained", model_type="plus-
+220M", is_eval=True) dataset = CodeXGLUEDataset
+(tokenizer=model_class.get_tokenizer()) train, test, validation = dataset.load
+(subset="text-to-code") train_dataset= CustomDataset(train[0], train[1])
+test_dataset= CustomDataset(test[0], test[1]) val_dataset= CustomDataset
+(validation[0], validation[1]) evaluator = EvaluationMetric(metric="bleu",
+tokenizer=model_class.tokenizer) # peft can be in ["lora", "prefixtuning"]
+trainer = CodeT5Seq2SeqTrainer(train_dataset=train_dataset,
+validation_dataset=val_dataset, peft="lora",
+pretrained_model_or_path=model_class.get_model(),
+tokenizer=model_class.tokenizer) trainer.train() ``` Comparing to [this script
+from StarCoder](https://github.com/bigcode-project/starcoder/blob/main/
+finetune/finetune.py), which requires ~300 LOCs to fine-tune a model, we only
+need 14 LOCs to do the same !!! ### Evaluate on Well-Known Benchmarks Planning
+to reproduce the results of well-known benchmarks like ``Human-Eval``, but
+struggling with not achieving the same numbers as reported in the original
+papers? Worried about the complicated evaluation process? Don't worry, we've
+got you covered with an intuitive, easy-to-use interface. Here's a sample
+snippet demonstrating how to evaluate Human Eval using pass@k (k=[1,10,100]) as
+the metric: ```python from codetf.models import load_model_pipeline from
 codetf.data_utility.human_eval_dataset import HumanEvalDataset from
 codetf.performance.model_evaluator import ModelEvaluator os.environ
 ["HF_ALLOW_CODE_EVAL"] = "1" os.environ["TOKENIZERS_PARALLELISM"] = "true"
 model_class = load_model_pipeline(model_name="causal-lm", task="pretrained",
 model_type="codegen-350M-mono", is_eval=True, load_in_8bit=True,
 weight_sharding=False) dataset = HumanEvalDataset
 (tokenizer=model_class.get_tokenizer()) prompt_token_ids,
@@ -154,42 +172,65 @@
 codetf.code_utility.apex.apex_code_utility import ApexCodeUtility
 apex_code_utility = ApexCodeUtility() sample_code = """ public class
 SampleClass { public Integer myNumber; ** * This is a method that returns the
 value of myNumber. * @return An integer value */ public Integer getMyNumber()
 { // Return the current value of myNumber return this.myNumber; } } """ ast =
 apex_code_utility.parse(sample_code) # This will print the tree-sitter AST
 object print(ast) ``` Then you can traverse the tree using the interface from
-[py-tree-sitter](https://github.com/tree-sitter/py-tree-sitter ``` root_node =
+[py-tree-sitter](https://github.com/tree-sitter/py-tree-sitter) ``` root_node =
 ast.root_node assert root_node.type == 'module' assert root_node.start_point ==
 (1, 0) assert root_node.end_point == (3, 13) ``` There are also other utilities
 for Java, Python, etc, that can perform the same operations. #### Extract Code
 Attributes CodeTF provides an interface to easily extract code attributes. The
 following is a sample for extracting the function name of a Python function:
 ```python code_attributes = apex_code_utility.get_code_attributes(sample_code)
 print(code_attributes) ``` This will print: `` {'class_names':
 ['AccountWithContacts'], 'method_names': ['getAccountsWithContacts'],
 'comments': [], 'variable_names': ['acc', 'accounts', 'con', 'System', 'debug',
 'Contacts', 'Id', 'Name', 'Account', 'Email', 'LastName']} `` ### Remove
 Comments There are other existing utilities, such as removing comments from
 code: ```python new_code_snippet = apex_code_utility.remove_comments
-(sample_code) print(new_code_snippet) ``` This will print: ``` public class
-SampleClass { public Integer myNumber; public Integer getMyNumber() { // Return
-the current value of myNumber return this.myNumber; } } ``` Note that this is
-an ongoing process, we will add more features to extract complicated code
-attributes in the future. More examples can be found [here](https://github.com/
-salesforce/CodeTF/tree/main/test_code_utilities). ## More Examples You can find
-more examples for each use case: - [Fine-tuning](https://github.com/salesforce/
-CodeTF/tree/main/test_trainer) - [Inferencing](https://github.com/salesforce/
-CodeTF/tree/main/test_inference) - [Model Evaluate](https://github.com/
-salesforce/CodeTF/tree/main/test_evaluator) - [Code Utility](https://
-github.com/salesforce/CodeTF/tree/main/test_code_utilities) ## Technical Report
-and Citing CodeTF You can find more details in our [technical report](https://
-arxiv.org/abs/2209.09019). If you're using CodeTF in your research or
-applications, please cite using this BibTeX: ```bibtex @misc{nghi2023codetf,
-title={CodeTF: A Transformer-based Library for CodeLLM & Code Intelligence},
-author={Nghi D. Q. Bui, Henry Le, Yue Wang, Akhilesh Deepak Gotmare, Junna Li,
-Steven Hoi.}, year={2023}, eprint={2209.09019}, archivePrefix={arXiv},
-primaryClass={cs.CV} } ``` | ## Contact us If you have any questions, comments
-or suggestions, please do not hesitate to contact us at codetf@salesforce.com.
-## License [BSD 3-Clause License](LICENSE.txt) Keywords: AI4Code,Code
-Intelligence,Generative AI,Deep Learning,Library,PyTorch,HuggingFace Platform:
-UNKNOWN Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
+(sample_code) print(new_code_snippet) ``` This will print: ```java public class
+SampleClass { public Integer myNumber; public Integer getMyNumber() { return
+this.myNumber; } } ``` Note that this is an ongoing process, we will add more
+features to extract complicated code attributes in the future. More examples
+can be found [here](https://github.com/salesforce/CodeTF/tree/main/
+test_code_utilities). ## More Examples You can find more examples for each use
+case: - [Fine-tuning](https://github.com/salesforce/CodeTF/tree/main/
+test_trainer) - [Inferencing](https://github.com/salesforce/CodeTF/tree/main/
+test_inference) - [Model Evaluate](https://github.com/salesforce/CodeTF/tree/
+main/test_evaluator) - [Code Utility](https://github.com/salesforce/CodeTF/
+tree/main/test_code_utilities) ## Notes - CodeTF is designed to complement and
+enhance the capabilities of [HuggingFace Transformers](https://huggingface.co/
+docs/transformers/index), rather than replace it. It serves as a specialized
+layer specifically tailored for code intelligence tasks, such as fine-tuning
+language models with code-specific features and evaluating on well-known code
+intelligence benchmarks. If users require more customization, they are
+encouraged to write their own training code from scratch. - CodeTF leverages
+the powerful functionality provided by [Accelerate](https://github.com/
+huggingface/accelerate) for both inference and training. With Accelerate, users
+do not need to manually manage GPUs or CPU devices for most operations,
+allowing for a streamlined and efficient workflow. ## Ethical and Responsible
+Use CodeTF, while powerful, does not guarantee infallible code intelligence
+capabilities. Users may encounter inaccuracies or biases, possibly leading to
+misinterpretations or undesired behaviors. Risks include the generation of
+insecure code, propagation of poor coding practices, or inadvertent revelation
+of sensitive data. We strongly advise users to examine the pretrained models
+and system before practical adoption. CodeTF facilitates effective code
+analysis, prediction, and debugging, promoting reproducible research and
+development. We encourage its responsible use for enhancing software quality
+and developer productivity. However, misuse can lead to unethical outcomes such
+as unauthorized code manipulation, privacy breaches, or insecure coding
+practices. Users should familiarize themselves with guidelines for responsible
+AI before using CodeTF. Our commitment is to continually refine the library by
+identifying and mitigating potential biases and inappropriate behaviors. Users
+should review the models and system before practical implementation, and
+contribute towards refining the library to ensure ethical usage. ## Technical
+Report and Citing CodeTF You can find more details in our [technical report]
+(https://arxiv.org). If you're using CodeTF in your research or applications,
+please cite using this BibTeX: ```bibtex @misc{nghi2023codetf, title={CodeTF: A
+Transformer-based Library for CodeLLM & Code Intelligence}, author={Nghi D. Q.
+Bui, Henry Le, Yue Wang, Akhilesh Deepak Gotmare, Junnan Li, Steven Hoi.},
+year={2023}, eprint={2209.09019}, archivePrefix={arXiv}, primaryClass={cs.CV} }
+``` ## Contact us If you have any questions, comments or suggestions, please do
+not hesitate to contact us at codetf@salesforce.com. ## License [Apache License
+Version 2.0](LICENSE.txt)
```

### Comparing `salesforce-codetf-0.0.3/codetf/__init__.py` & `salesforce-codetf-0.0.4/codetf/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/code_utility/apex/apex_code_utility.py` & `salesforce-codetf-0.0.4/codetf/code_utility/apex/apex_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/code_utility/ast_parser.py` & `salesforce-codetf-0.0.4/codetf/code_utility/ast_parser.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/code_utility/base_utility.py` & `salesforce-codetf-0.0.4/codetf/code_utility/base_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/code_utility/java/java_code_utility.py` & `salesforce-codetf-0.0.4/codetf/code_utility/java/java_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/code_utility/python/python_code_utility.py` & `salesforce-codetf-0.0.4/codetf/code_utility/python/python_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/common/registry.py` & `salesforce-codetf-0.0.4/codetf/common/registry.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/common/utils.py` & `salesforce-codetf-0.0.4/codetf/common/utils.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/data_utility/apps_dataset.py` & `salesforce-codetf-0.0.4/codetf/data_utility/apps_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/data_utility/base_dataset.py` & `salesforce-codetf-0.0.4/codetf/data_utility/base_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/data_utility/codexglue_dataset.py` & `salesforce-codetf-0.0.4/codetf/data_utility/codexglue_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/data_utility/human_eval_dataset.py` & `salesforce-codetf-0.0.4/codetf/data_utility/human_eval_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/data_utility/mpp_dataset.py` & `salesforce-codetf-0.0.4/codetf/data_utility/mpp_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/data_utility/util.py` & `salesforce-codetf-0.0.4/codetf/data_utility/util.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/models/__init__.py` & `salesforce-codetf-0.0.4/codetf/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,101 @@
 import sys
 from pathlib import Path
 sys.path.append(str(Path(".").absolute().parent))
 import logging
 from omegaconf import OmegaConf
 from codetf.common.registry import registry
 from codetf.models.base_model import BaseModel
-from codetf.models.codet5_models import CodeT5Seq2SeqModel
+from codetf.models.seq2seq_models import Seq2SeqModel
 from codetf.models.causal_lm_models import CausalLMModel
 from codetf.models.bert_models import BertModel
-
+from codetf.common.utils import get_abs_path
 
 __all__ = [
-    "CodeT5Seq2SeqModel",
+    "Seq2SeqModel",
     "CausalLMModel",
     "BertModel"
 ]
 
-# card_name_mapper = {
-#     "codet5_translation": "codet5",
-#     "codet5_summarization": "codet5",
-#     "codet5_nl2code": "codet5",
-#     "codet5_clone": "codet5",
-#     "codet5_defect": "codet5"
-# }
-
-def get_model_config(model_name, model_type="base"):
-    import json
-
-    from omegaconf import OmegaConf
-
-    config_path = registry.get_model_class(model_name).PRETRAINED_MODEL_CONFIG_DICT[
-        model_type
-    ]
-
-    config = OmegaConf.load(config_path)
-    config = OmegaConf.to_container(config)
-
-    # print(json.dumps(config, indent=4, sort_keys=True))
-
-    return config
-
-
 def construct_model_card(model_name, model_type=None, task=None, 
-                        dataset=None, language=None,
-                        quantize=None, quantize_algo=None):
+                        dataset=None, language=None):
     model_card_parts = [model_name]
 
     if model_type:
         model_card_parts.append(model_type)
 
     if dataset:
         model_card_parts.append(dataset)
 
     if task:
         model_card_parts.append(task)
 
     if language:
         model_card_parts.append(language)
     
-    if quantize_algo:
-        if quantize_algo is not "bitsandbyte":
-            model_card_parts.append(quantize_algo)
-
-    if quantize:
-        model_card_parts.append(quantize)
-    
     model_card_name = "-".join(model_card_parts)
     return model_card_name
 
 def get_model_class_name(model_name, task):
     class_name = f"{model_name}_{task}"
     return class_name
 
 def load_model_pipeline(model_name, model_type="base", task="sum",
             dataset=None, language=None, is_eval=True, 
-            load_in_8bit=True, weight_sharding=True):
+            load_in_8bit=False, load_in_4bit=False, weight_sharding=False):
     
     model_cls = registry.get_model_class(model_name)
     model_card = construct_model_card(model_name, model_type, task, dataset, language)
-    model = model_cls.from_pretrained(model_card=model_card, load_in_8bit=load_in_8bit, weight_sharding=weight_sharding)
+    model = model_cls.from_pretrained(model_card=model_card, load_in_8bit=load_in_8bit, load_in_4bit=load_in_4bit, weight_sharding=weight_sharding)
     if is_eval:
         model.eval()
 
     return model
 
 
-# class ModelZoo:
-#     def __init__(self) -> None:
-#         self.model_zoo = {
-#             k: list(v.PRETRAINED_MODEL_CONFIG_DICT.keys())
-#             for k, v in registry.mapping["model_name_mapping"].items()
-#         }
-
-#     def __str__(self) -> str:
-#         return (
-#             "=" * 50
-#             + "\n"
-#             + f"{'Architectures':<30} {'Types'}\n"
-#             + "=" * 50
-#             + "\n"
-#             + "\n".join(
-#                 [
-#                     f"{name:<30} {', '.join(types)}"
-#                     for name, types in self.model_zoo.items()
-#                 ]
-#             )
-#         )
-
-#     def __iter__(self):
-#         return iter(self.model_zoo.items())
-
-#     def __len__(self):
-#         return sum([len(v) for v in self.model_zoo.values()])
-
-
-# model_zoo = ModelZoo()
+class ModelZoo:
+    def __init__(self, config_files):
+        self.config_files = config_files
+        self.models = self.load_models()
+
+    def load_models(self):
+        models = {}
+
+        for file in self.config_files:
+            try:
+                data = OmegaConf.load(get_abs_path(file))
+                for model in data:
+                    model_name, model_type, task = self.parse_model_key(model)
+                    if model_name not in models:
+                        models[model_name] = []
+                    models[model_name].append((model_type, task))
+            except Exception as exc:
+                print(exc)
+
+        return models
+
+    @staticmethod
+    def parse_model_key(key):
+        parts = key.split("-")
+        model_name = parts[0]
+        model_type = "-".join(parts[1:-1])
+        task = parts[-1]
+        return model_name, model_type, task
+
+    def __str__(self):
+        output = "============================================================================================================\n"
+        output += "Architectures                  Types                           Tasks\n"
+        output += "============================================================================================================\n"
+        for model_name, model_infos in self.models.items():
+            for i, model_info in enumerate(model_infos):
+                model_type, task = model_info
+                if i == 0:
+                    output += f"{model_name:<30} {model_type:<30} {task:<30}\n"
+                else:
+                    output += f"{'':<30} {model_type:<30} {task:<30}\n"
+        return output
+
+
+# instantiate the ModelZoo at the module level
+model_zoo = ModelZoo(["configs/inference/causal_lm.yaml", 
+                      "configs/inference/codet5.yaml", 
+                      "configs/inference/bert.yaml"])
```

### Comparing `salesforce-codetf-0.0.3/codetf/models/base_model.py` & `salesforce-codetf-0.0.4/codetf/models/base_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,20 +36,20 @@
         self.accelerator = Accelerator()
 
     @property
     def device(self):
         return list(self.parameters())[0].device
     
     @classmethod
-    def from_pretrained(model_class, model_card, load_in_8bit=True, weight_sharding=True):
+    def from_pretrained(model_class, model_card, load_in_8bit=False, load_in_4bit=False, weight_sharding=False):
         """
         Build a pretrained model from default configuration file, specified by model_type.
         """
         model_config = OmegaConf.load(get_abs_path(model_class.MODEL_DICT))[model_card]
-        model_cls = model_class.load_model_from_config(model_config=model_config, load_in_8bit=load_in_8bit, weight_sharding=weight_sharding)
+        model_cls = model_class.load_model_from_config(model_config=model_config, load_in_8bit=load_in_8bit, load_in_4bit=load_in_4bit, weight_sharding=weight_sharding)
 
         return model_cls
 
     def get_model(self):
         return self.model
     
     def get_tokenizer(self):
```

### Comparing `salesforce-codetf-0.0.3/codetf/models/bert_models/__init__.py` & `salesforce-codetf-0.0.4/codetf/models/bert_models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,20 @@
 
     @classmethod
     def init_tokenizer(cls, model):
         tokenizer = RobertaTokenizer.from_pretrained(model)
         return tokenizer
     
     @classmethod
-    def load_model_from_config(model_class, model_config, load_in_8bit=True, weight_sharding=True):
+    def load_model_from_config(model_class, model_config, load_in_8bit=False, load_in_4bit=False, weight_sharding=False):
         checkpoint = model_config["huggingface_url"]
+
+        if load_in_8bit and load_in_4bit:
+            raise ValueError("Only one of load_in_8bit or load_in_4bit can be True. Please choose one.")
+        
         if weight_sharding:
             weights_location = hf_hub_download(checkpoint, "pytorch_model.bin")
             config = RobertaConfig.from_pretrained(checkpoint)
             with init_empty_weights():
                 model = RobertaModel.from_config(config)
 
             model.tie_weights()            
@@ -43,14 +47,18 @@
                 model, weights_location, device_map="auto", no_split_module_classes=["GPTJBlock"]
             )
         else:
             if load_in_8bit:
                 model = RobertaModel.from_pretrained(checkpoint, 
                                             load_in_8bit=load_in_8bit, 
                                             device_map="auto")
+            elif load_in_4bit:
+                model = RobertaModel.from_pretrained(checkpoint, 
+                                            load_in_4bit=load_in_4bit, 
+                                            device_map="auto")
             else:
                 model = RobertaModel.from_pretrained(checkpoint, 
                                             device_map="auto")
 
 
         tokenizer = model_class.init_tokenizer(model_config["tokenizer_url"])
```

### Comparing `salesforce-codetf-0.0.3/codetf/models/causal_lm_models/__init__.py` & `salesforce-codetf-0.0.4/codetf/models/causal_lm_models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import sys
 from pathlib import Path
 sys.path.append(str(Path(".").absolute().parent))
 from transformers import AutoTokenizer, AutoModelForCausalLM, AutoConfig
 from codetf.models.base_model import BaseModel
 from codetf.common.registry import registry
-from accelerate import Accelerator
 from collections import defaultdict
 from tqdm import tqdm
 import torch
 from accelerate import init_empty_weights, load_checkpoint_and_dispatch
 from huggingface_hub import hf_hub_download
 import torch
 
-@registry.register_model("causal-lm")
+@registry.register_model("causallm")
 class CausalLMModel(BaseModel):
 
     MODEL_DICT = "configs/inference/causal_lm.yaml"
     
 
     def __init__(self, model, model_config, tokenizer):
         super().__init__()
@@ -26,16 +25,20 @@
 
     @classmethod
     def init_tokenizer(cls, model):
         tokenizer = AutoTokenizer.from_pretrained(model)
         return tokenizer
     
     @classmethod
-    def load_model_from_config(model_class, model_config, load_in_8bit=True, weight_sharding=True):
+    def load_model_from_config(model_class, model_config, load_in_8bit=False, load_in_4bit=False, weight_sharding=False):
         checkpoint = model_config["huggingface_url"]
+
+        if load_in_8bit and load_in_4bit:
+            raise ValueError("Only one of load_in_8bit or load_in_4bit can be True. Please choose one.")
+        
         if weight_sharding:
             weights_location = hf_hub_download(checkpoint, "pytorch_model.bin")
             config = AutoConfig.from_pretrained(checkpoint)
             with init_empty_weights():
                 model = AutoModelForCausalLM.from_config(config)
 
             model.tie_weights()            
@@ -43,14 +46,18 @@
                 model, weights_location, device_map="auto", no_split_module_classes=["GPTJBlock"]
             )
         else:
             if load_in_8bit:
                 model = AutoModelForCausalLM.from_pretrained(checkpoint, 
                                             load_in_8bit=load_in_8bit, 
                                             device_map="auto")
+            elif load_in_4bit:
+                model = AutoModelForCausalLM.from_pretrained(checkpoint, 
+                                            load_in_4bit=load_in_4bit, 
+                                            device_map="auto")
             else:
                 model = AutoModelForCausalLM.from_pretrained(checkpoint, 
                                             device_map="auto")
 
 
         tokenizer = model_class.init_tokenizer(model_config["tokenizer_url"])
```

### Comparing `salesforce-codetf-0.0.3/codetf/models/codet5_models/__init__.py` & `salesforce-codetf-0.0.4/codetf/models/seq2seq_models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 from pathlib import Path
 sys.path.append(str(Path(".").absolute().parent))
 from transformers import RobertaTokenizer
 from codetf.models.base_model import BaseModel
-from transformers import T5ForConditionalGeneration, T5Config
+from transformers import AutoModelForSeq2SeqLM, AutoConfig
 from codetf.common.registry import registry
 from accelerate import Accelerator
 
 @registry.register_model("codet5")
-class CodeT5Seq2SeqModel(BaseModel):
+class Seq2SeqModel(BaseModel):
     
     MODEL_DICT = "configs/inference/codet5.yaml"
      
     def __init__(self, model, model_config, tokenizer):
         super().__init__()
         self.model = model
         self.tokenizer = tokenizer
@@ -22,47 +22,55 @@
 
     @classmethod
     def init_tokenizer(cls, model):
         return RobertaTokenizer.from_pretrained(model)
     
   
     @classmethod
-    def load_model_from_config(model_class, model_config, load_in_8bit=True, weight_sharding=True):
+    def load_model_from_config(model_class, model_config, load_in_8bit=False, load_in_4bit=False, weight_sharding=False):
         
         checkpoint = model_config["huggingface_url"]
+
+        if load_in_8bit and load_in_4bit:
+            raise ValueError("Only one of load_in_8bit or load_in_4bit can be True. Please choose one.")
+
         if weight_sharding:
             weights_location = hf_hub_download(checkpoint, "pytorch_model.bin")
-            config = T5Config.from_pretrained(checkpoint)
+            config = AutoConfig.from_pretrained(checkpoint)
             with init_empty_weights():
-                model = AutoModelForCausalLM.from_config(config)
+                model = AutoModelForSeq2SeqLM.from_config(config)
 
             model.tie_weights()            
             model = load_checkpoint_and_dispatch(
                 model, weights_location, device_map="auto", no_split_module_classes=["GPTJBlock"]
             )
         else:
             if load_in_8bit:
-                model = T5ForConditionalGeneration.from_pretrained(checkpoint, 
+                model = AutoModelForSeq2SeqLM.from_pretrained(checkpoint, 
                                             load_in_8bit=load_in_8bit, 
                                             device_map="auto")
+            elif load_in_4bit:
+                model = AutoModelForSeq2SeqLM.from_pretrained(checkpoint, 
+                                            load_in_4bit=load_in_4bit, 
+                                            device_map="auto")
             else:
-                model = T5ForConditionalGeneration.from_pretrained(checkpoint, 
+                model = AutoModelForSeq2SeqLM.from_pretrained(checkpoint, 
                                             device_map="auto")
 
            
         tokenizer = model_class.init_tokenizer(model_config.get("tokenizer_url"))
 
         return model_class(
             model=model,
             model_config=model_config,
             tokenizer=tokenizer
         )
     
 
-    def forward_seq2seq(self, sources):
+    def forward(self, sources):
         encoding = self.tokenizer(sources, return_tensors='pt')
         input_ids = encoding.input_ids.to(self.device)
         attention_mask = encoding.attention_mask.to(self.device)
         generated_ids = self.model.generate(input_ids, attention_mask=attention_mask,
                                             max_length=self.max_prediction_length, 
                                             num_beams=self.beam_size)
 
@@ -70,10 +78,10 @@
         return predictions
     
 
     def predict(self, sources):
         
         input_for_net = [' '.join(source.strip().split()).replace('\n', ' ') for source in sources]
         # if self.task in ["sum", "translate", "nl2code", "refine"]:
-        output = self.forward_seq2seq(input_for_net)
+        output = self.forward(input_for_net)
        
         return output
```

### Comparing `salesforce-codetf-0.0.3/codetf/performance/evaluation_metric.py` & `salesforce-codetf-0.0.4/codetf/performance/evaluation_metric.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/performance/model_evaluator.py` & `salesforce-codetf-0.0.4/codetf/performance/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/trainer/base_trainer.py` & `salesforce-codetf-0.0.4/codetf/trainer/base_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/trainer/causal_lm_trainer.py` & `salesforce-codetf-0.0.4/codetf/trainer/causal_lm_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/codetf/trainer/codet5_trainer.py` & `salesforce-codetf-0.0.4/codetf/trainer/codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/salesforce_codetf.egg-info/SOURCES.txt` & `salesforce-codetf-0.0.4/salesforce_codetf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 codetf/data_utility/human_eval_dataset.py
 codetf/data_utility/mpp_dataset.py
 codetf/data_utility/util.py
 codetf/models/__init__.py
 codetf/models/base_model.py
 codetf/models/bert_models/__init__.py
 codetf/models/causal_lm_models/__init__.py
-codetf/models/codet5_models/__init__.py
+codetf/models/seq2seq_models/__init__.py
 codetf/performance/__init__.py
 codetf/performance/evaluation_metric.py
 codetf/performance/model_evaluator.py
 codetf/trainer/base_trainer.py
 codetf/trainer/causal_lm_trainer.py
 codetf/trainer/codet5_trainer.py
+docs/conf.py
 salesforce_codetf.egg-info/PKG-INFO
 salesforce_codetf.egg-info/SOURCES.txt
 salesforce_codetf.egg-info/dependency_links.txt
 salesforce_codetf.egg-info/not-zip-safe
 salesforce_codetf.egg-info/requires.txt
 salesforce_codetf.egg-info/top_level.txt
 test_code_utilities/__init__.py
@@ -46,11 +47,12 @@
 test_dataset/test_load_codexgluedataset.py
 test_evaluation/test_evaluate_human_eval_codegen.py
 test_evaluation/test_evaluate_human_eval_codet5.py
 test_inference/__init__.py
 test_inference/test_codebert_embedding.py
 test_inference/test_codegen_nl2code.py
 test_inference/test_codet5_multitask.py
+test_inference/test_load_model_zoo.py
 test_inference/test_starcoder_nl2code.py
 test_trainer/test_causal_lm_trainer_codegen.py
 test_trainer/test_codet5_trainer.py
 test_trainer/test_t5_trainer.py
```

### Comparing `salesforce-codetf-0.0.3/setup.py` & `salesforce-codetf-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 from setuptools import setup, find_packages, find_namespace_packages
 import platform
 
-install_requires = [
-    "accelerate==0.19.0",
-    "datasets==2.12.0",
-    "evaluate==0.4.0",
-    "huggingface-hub==0.14.1",
-    "iopath==0.1.10",
-    "nltk==3.8.1",
-    "numpy==1.21.5",
-    "omegaconf==2.3.0",
-    "pandas==1.3.5",
-    "peft==0.3.0",
-    "pyparsing==3.0.7",
-    "PyYAML==6.0",
-    "requests==2.27.1",
-    "rouge-score==0.1.2",
-    "sacrebleu==2.3.1",
-    "scikit-learn==1.0.2",
-    "torch==1.13.1",
-    "torchvision==0.14.1",
-    "tqdm==4.63.0",
-    "transformers==4.29.2",
-    "tree-sitter==0.20.1"
-]
+# install_requires = [
+#     "accelerate==0.19.0",
+#     "datasets==2.12.0",
+#     "evaluate==0.4.0",
+#     "huggingface-hub==0.14.1",
+#     "iopath==0.1.10",
+#     "nltk==3.8.1",
+#     "numpy==1.22.0",
+#     "omegaconf==2.3.0",
+#     "pandas==1.3.5",
+#     "peft==0.3.0",
+#     "pyparsing==3.0.7",
+#     "PyYAML==6.0",
+#     "requests==2.31.0",
+#     "rouge-score==0.1.2",
+#     "sacrebleu==2.3.1",
+#     "scikit-learn==1.0.2",
+#     "torch==1.13.1",
+#     "torchvision==0.14.1",
+#     "tqdm==4.63.0",
+#     "transformers==4.29.2",
+#     "tree-sitter==0.20.1"
+# ]
+
+def read_requirements():
+    with open('requirements.txt', 'r') as req:
+        content = req.read()
+        requirements = content.split('\n')
+
+    return requirements
+
+install_requires = read_requirements()
+
 DEPENDENCY_LINKS = []
 if platform.system() == "Windows":
     DEPENDENCY_LINKS.append("https://download.pytorch.org/whl/torch_stable.html")
     
-def fetch_requirements(filename):
-    with open(filename) as f:
-        return [ln.strip() for ln in f.read().split("\n")]
 
 setup(
   name = 'salesforce-codetf',
-  version = "0.0.3",
+  version = "0.0.4",
   py_modules = ['codetf'],
   description = 'CodeTF: A Transformer-based Library for Code Intelligence',
   author = 'Nghi D. Q. Bui',
   long_description=open("README.md", "r", encoding="utf-8").read(),
   long_description_content_type="text/markdown",
   keywords="AI4Code, Code Intelligence, Generative AI, Deep Learning, Library, PyTorch, HuggingFace",
   license="3-Clause BSD",
```

### Comparing `salesforce-codetf-0.0.3/test_code_utilities/test_extract_code_attributre.py` & `salesforce-codetf-0.0.4/test_code_utilities/test_extract_code_attributre.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/test_code_utilities/test_parse_code.py` & `salesforce-codetf-0.0.4/test_code_utilities/test_parse_code.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/test_code_utilities/test_remove_comments.py` & `salesforce-codetf-0.0.4/test_code_utilities/test_remove_comments.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/test_code_utilities/test_variable_renaming.py` & `salesforce-codetf-0.0.4/test_code_utilities/test_variable_renaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 from pathlib import Path
 sys.path.append(str(Path(".").absolute().parent))
 # sys.path.append(str(Path(__file__).resolve().parents[2]))
 from codetf.code_utility.apex.apex_code_utility import ApexCodeUtility
 
 apex_code_utility = ApexCodeUtility()
 
-sample_code = 
-    """
+sample_code = """
     public class AccountWithContacts {
     // Method to fetch accounts and their related contacts
-    public static void getAccountsWithContacts() {
-        // Query to fetch accounts with related contacts
-        List<Account> accounts = [SELECT Id, Name, (SELECT Id, LastName, Email FROM Contacts) FROM Account LIMIT 10];
-
-        // Iterate through accounts and print account and contact information to the debug log
-        for (Account acc : accounts) {
-            System.debug('Account Name: ' + acc.Name);
-
-            for (Contact con : acc.Contacts) {
-                System.debug('Contact Name: ' + con.LastName + ', Email: ' + con.Email);
+        public static void getAccountsWithContacts() {
+            // Query to fetch accounts with related contacts
+            List<Account> accounts = [SELECT Id, Name, (SELECT Id, LastName, Email FROM Contacts) FROM Account LIMIT 10];
+
+            // Iterate through accounts and print account and contact information to the debug log
+            for (Account acc : accounts) {
+                System.debug('Account Name: ' + acc.Name);
+
+                for (Contact con : acc.Contacts) {
+                    System.debug('Contact Name: ' + con.LastName + ', Email: ' + con.Email);
+                }
             }
         }
     }
-}
     """
 
 new_code_snippet = apex_code_utility.rename_identifiers(sample_code)
 print(new_code_snippet)
```

### Comparing `salesforce-codetf-0.0.3/test_evaluation/test_evaluate_human_eval_codegen.py` & `salesforce-codetf-0.0.4/test_evaluation/test_evaluate_human_eval_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/test_evaluation/test_evaluate_human_eval_codet5.py` & `salesforce-codetf-0.0.4/test_evaluation/test_evaluate_human_eval_codet5.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.3/test_inference/test_codet5_multitask.py` & `salesforce-codetf-0.0.4/test_inference/test_codet5_multitask.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import sys
 from pathlib import Path
 sys.path.append(str(Path(".").absolute().parent))
-# sys.path.append("../")
-import torch
 from codetf.models import load_model_pipeline
 
 translation_model = load_model_pipeline(model_name="codet5", task="translate-cs-java",
-            model_type="base", is_eval=True,
-            load_in_8bit=True, weight_sharding=False)
+            model_type="base", is_eval=True, 
+            load_in_4bit=True, weight_sharding=False)
 
 summarization_model = load_model_pipeline(model_name="codet5", task="sum-python",
             model_type="base", is_eval=True,
             load_in_8bit=True, weight_sharding=False)
 
 code_snippets = """
     void bubbleSort(int arr[])
```

### Comparing `salesforce-codetf-0.0.3/test_trainer/test_causal_lm_trainer_codegen.py` & `salesforce-codetf-0.0.4/test_trainer/test_causal_lm_trainer_codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import torch
 from codetf.trainer.causal_lm_trainer import CausalLMTrainer
 from codetf.data_utility.codexglue_dataset import CodeXGLUEDataset
 from codetf.models import load_model_pipeline
 from codetf.performance.evaluation_metric import EvaluationMetric
 from codetf.data_utility.base_dataset import CustomDataset
 
-model_class = load_model_pipeline(model_name="causal-lm", task="pretrained",
-            model_type="codegen-350M-mono", is_eval=False,
-            load_in_8bit=False, weight_sharding=False)
+model_class = load_model_pipeline(model_name="causallm", task="pretrained",
+            model_type="codegen-350M-mono", is_eval=False)
 
 
 dataset = CodeXGLUEDataset(tokenizer=model_class.get_tokenizer())
 train, test, validation = dataset.load(subset="text-to-code")
 
 train_dataset = CustomDataset(train[0], train[1])
 test_dataset= CustomDataset(test[0], test[1])
```

### Comparing `salesforce-codetf-0.0.3/test_trainer/test_codet5_trainer.py` & `salesforce-codetf-0.0.4/test_trainer/test_codet5_trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import torch
 from codetf.trainer.codet5_trainer import CodeT5Seq2SeqTrainer
 from codetf.data_utility.codexglue_dataset import CodeXGLUEDataset
 from codetf.models import load_model_pipeline
 from codetf.performance.evaluation_metric import EvaluationMetric
 from codetf.data_utility.base_dataset import CustomDataset
 
-model_class = load_model_pipeline(model_name="codet5", task="multi-sum-pretrained",
-            model_type="base", is_eval=True,
-            load_in_8bit=False, weight_sharding=False)
+model_class = load_model_pipeline(model_name="codet5", task="pretrained",
+            model_type="plus-220M", is_eval=True)
 
 dataset = CodeXGLUEDataset(tokenizer=model_class.get_tokenizer())
 train, test, validation = dataset.load(subset="text-to-code")
 
 train_dataset= CustomDataset(train[0], train[1])
 test_dataset= CustomDataset(test[0], test[1])
 val_dataset= CustomDataset(validation[0], validation[1])
```

### Comparing `salesforce-codetf-0.0.3/test_trainer/test_t5_trainer.py` & `salesforce-codetf-0.0.4/test_trainer/test_t5_trainer.py`

 * *Files identical despite different names*

