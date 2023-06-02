# Comparing `tmp/draupnir-0.0.27.tar.gz` & `tmp/draupnir-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draupnir-0.0.27.tar", last modified: Sat Oct  8 16:58:05 2022, max compression
+gzip compressed data, was "draupnir-0.0.28.tar", last modified: Fri Jun  2 13:43:22 2023, max compression
```

## Comparing `draupnir-0.0.27.tar` & `draupnir-0.0.28.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2022-10-08 16:58:05.524002 draupnir-0.0.27/
--rw-r--r--   0 lys       (1000) lys       (1000)     1071 2022-02-03 12:22:28.000000 draupnir-0.0.27/LICENSE
--rw-r--r--   0 lys       (1000) lys       (1000)       15 2022-02-04 14:46:10.000000 draupnir-0.0.27/MANIFEST.in
--rw-rw-r--   0 lys       (1000) lys       (1000)    10360 2022-10-08 16:58:05.524002 draupnir-0.0.27/PKG-INFO
--rw-r--r--   0 lys       (1000) lys       (1000)     9570 2022-10-08 16:51:08.000000 draupnir-0.0.27/README.md
--rw-r--r--   0 lys       (1000) lys       (1000)      103 2022-02-03 12:19:06.000000 draupnir-0.0.27/pyproject.toml
--rw-r--r--   0 lys       (1000) lys       (1000)      748 2022-10-08 16:58:05.524002 draupnir-0.0.27/setup.cfg
--rw-r--r--   0 lys       (1000) lys       (1000)     3138 2022-10-08 15:50:36.000000 draupnir-0.0.27/setup.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2022-10-08 16:58:05.448002 draupnir-0.0.27/src/
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2022-10-08 16:58:05.460002 draupnir-0.0.27/src/draupnir/
--rw-r--r--   0 lys       (1000) lys       (1000)    15019 2022-03-01 17:48:39.000000 draupnir-0.0.27/src/draupnir/3D.py
--rw-r--r--   0 lys       (1000) lys       (1000)      496 2022-03-30 13:01:42.000000 draupnir-0.0.27/src/draupnir/__init__.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2022-10-08 16:58:05.460002 draupnir-0.0.27/src/draupnir/data/
--rw-r--r--   0 lys       (1000) lys       (1000)     1578 2021-07-28 14:11:37.000000 draupnir-0.0.27/src/draupnir/data/AA_properties.txt
--rw-r--r--   0 lys       (1000) lys       (1000) 32494553 2021-07-28 14:11:52.000000 draupnir-0.0.27/src/draupnir/data/PfamPdbMap.txt
--rw-r--r--   0 lys       (1000) lys       (1000)    37246 2022-10-08 16:43:04.000000 draupnir-0.0.27/src/draupnir/datasets.py
--rw-r--r--   0 lys       (1000) lys       (1000)     9362 2022-03-22 15:01:49.000000 draupnir-0.0.27/src/draupnir/draw_tree.py
--rw-r--r--   0 lys       (1000) lys       (1000)     8722 2022-06-27 13:16:05.000000 draupnir-0.0.27/src/draupnir/guides.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2022-10-08 16:58:05.524002 draupnir-0.0.27/src/draupnir/infer_angles/
--rw-r--r--   0 lys       (1000) lys       (1000)      330 2022-02-15 14:19:01.000000 draupnir-0.0.27/src/draupnir/infer_angles/__init__.py
--rw-r--r--   0 lys       (1000) lys       (1000)     5319 2021-08-19 13:41:22.000000 draupnir-0.0.27/src/draupnir/infer_angles/calculate_coords.py
--rw-r--r--   0 lys       (1000) lys       (1000)     1362 2021-08-13 17:18:45.000000 draupnir-0.0.27/src/draupnir/infer_angles/nerf.py
--rw-r--r--   0 lys       (1000) lys       (1000)     9437 2021-08-13 17:41:01.000000 draupnir-0.0.27/src/draupnir/infer_angles/pnerf.py
--rw-r--r--   0 lys       (1000) lys       (1000)    19190 2022-02-13 16:56:12.000000 draupnir-0.0.27/src/draupnir/infer_angles/superposition.py
--rw-r--r--   0 lys       (1000) lys       (1000)    59299 2022-10-07 18:02:03.000000 draupnir-0.0.27/src/draupnir/load_utils.py
--rw-r--r--   0 lys       (1000) lys       (1000)   183347 2022-10-08 16:33:40.000000 draupnir-0.0.27/src/draupnir/main.py
--rw-r--r--   0 lys       (1000) lys       (1000)    67482 2022-10-07 16:10:38.000000 draupnir-0.0.27/src/draupnir/models.py
--rw-r--r--   0 lys       (1000) lys       (1000)    22351 2022-10-07 17:51:32.000000 draupnir-0.0.27/src/draupnir/models_utils.py
--rw-r--r--   0 lys       (1000) lys       (1000)    17808 2022-03-29 15:41:27.000000 draupnir-0.0.27/src/draupnir/mutual_information.py
--rw-r--r--   0 lys       (1000) lys       (1000)    81700 2022-03-30 16:03:37.000000 draupnir-0.0.27/src/draupnir/plots.py
--rw-r--r--   0 lys       (1000) lys       (1000)     4493 2022-03-22 17:45:42.000000 draupnir-0.0.27/src/draupnir/train.py
--rw-r--r--   0 lys       (1000) lys       (1000)   108494 2022-10-08 15:40:04.000000 draupnir-0.0.27/src/draupnir/utils.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2022-10-08 16:58:05.460002 draupnir-0.0.27/src/draupnir.egg-info/
--rw-r--r--   0 lys       (1000) lys       (1000)    10360 2022-10-08 16:58:05.000000 draupnir-0.0.27/src/draupnir.egg-info/PKG-INFO
--rw-r--r--   0 lys       (1000) lys       (1000)      861 2022-10-08 16:58:05.000000 draupnir-0.0.27/src/draupnir.egg-info/SOURCES.txt
--rw-r--r--   0 lys       (1000) lys       (1000)        1 2022-10-08 16:58:05.000000 draupnir-0.0.27/src/draupnir.egg-info/dependency_links.txt
--rw-r--r--   0 lys       (1000) lys       (1000)        1 2022-03-02 13:52:18.000000 draupnir-0.0.27/src/draupnir.egg-info/not-zip-safe
--rw-r--r--   0 lys       (1000) lys       (1000)      229 2022-10-08 16:58:05.000000 draupnir-0.0.27/src/draupnir.egg-info/requires.txt
--rw-r--r--   0 lys       (1000) lys       (1000)      120 2022-10-08 16:58:05.000000 draupnir-0.0.27/src/draupnir.egg-info/top_level.txt
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-02 13:43:22.081260 draupnir-0.0.28/
+-rw-r--r--   0 lys       (1000) lys       (1000)     1071 2022-02-03 12:22:28.000000 draupnir-0.0.28/LICENSE
+-rw-r--r--   0 lys       (1000) lys       (1000)       15 2022-02-04 14:46:10.000000 draupnir-0.0.28/MANIFEST.in
+-rw-rw-r--   0 lys       (1000) lys       (1000)    10675 2023-06-02 13:43:22.081260 draupnir-0.0.28/PKG-INFO
+-rw-r--r--   0 lys       (1000) lys       (1000)     9922 2023-06-02 13:40:23.000000 draupnir-0.0.28/README.md
+-rw-r--r--   0 lys       (1000) lys       (1000)      103 2022-02-03 12:19:06.000000 draupnir-0.0.28/pyproject.toml
+-rw-r--r--   0 lys       (1000) lys       (1000)      748 2023-06-02 13:43:22.081260 draupnir-0.0.28/setup.cfg
+-rw-r--r--   0 lys       (1000) lys       (1000)     3138 2023-06-02 13:40:22.000000 draupnir-0.0.28/setup.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-02 13:43:22.021259 draupnir-0.0.28/src/
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-02 13:43:22.029259 draupnir-0.0.28/src/draupnir/
+-rw-r--r--   0 lys       (1000) lys       (1000)    15019 2022-03-01 17:48:39.000000 draupnir-0.0.28/src/draupnir/3D.py
+-rw-r--r--   0 lys       (1000) lys       (1000)      496 2022-03-30 13:01:42.000000 draupnir-0.0.28/src/draupnir/__init__.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-02 13:43:22.029259 draupnir-0.0.28/src/draupnir/data/
+-rw-r--r--   0 lys       (1000) lys       (1000)     1578 2021-07-28 14:11:37.000000 draupnir-0.0.28/src/draupnir/data/AA_properties.txt
+-rw-r--r--   0 lys       (1000) lys       (1000) 32494553 2021-07-28 14:11:52.000000 draupnir-0.0.28/src/draupnir/data/PfamPdbMap.txt
+-rw-r--r--   0 lys       (1000) lys       (1000)    37246 2022-10-08 16:43:04.000000 draupnir-0.0.28/src/draupnir/datasets.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     9362 2022-03-22 15:01:49.000000 draupnir-0.0.28/src/draupnir/draw_tree.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     8722 2022-06-27 13:16:05.000000 draupnir-0.0.28/src/draupnir/guides.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-02 13:43:22.081260 draupnir-0.0.28/src/draupnir/infer_angles/
+-rw-r--r--   0 lys       (1000) lys       (1000)      330 2022-02-15 14:19:01.000000 draupnir-0.0.28/src/draupnir/infer_angles/__init__.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     5319 2021-08-19 13:41:22.000000 draupnir-0.0.28/src/draupnir/infer_angles/calculate_coords.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     1362 2021-08-13 17:18:45.000000 draupnir-0.0.28/src/draupnir/infer_angles/nerf.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     9437 2021-08-13 17:41:01.000000 draupnir-0.0.28/src/draupnir/infer_angles/pnerf.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    19190 2022-02-13 16:56:12.000000 draupnir-0.0.28/src/draupnir/infer_angles/superposition.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    59299 2022-10-07 18:02:03.000000 draupnir-0.0.28/src/draupnir/load_utils.py
+-rw-r--r--   0 lys       (1000) lys       (1000)   183274 2022-10-18 18:37:56.000000 draupnir-0.0.28/src/draupnir/main.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    67482 2022-10-07 16:10:38.000000 draupnir-0.0.28/src/draupnir/models.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    22323 2022-10-14 12:25:08.000000 draupnir-0.0.28/src/draupnir/models_utils.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    17819 2023-05-10 11:36:14.000000 draupnir-0.0.28/src/draupnir/mutual_information.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    81700 2022-11-08 11:12:02.000000 draupnir-0.0.28/src/draupnir/plots.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     4493 2022-03-22 17:45:42.000000 draupnir-0.0.28/src/draupnir/train.py
+-rw-r--r--   0 lys       (1000) lys       (1000)   108500 2022-12-19 20:46:58.000000 draupnir-0.0.28/src/draupnir/utils.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-02 13:43:22.029259 draupnir-0.0.28/src/draupnir.egg-info/
+-rw-r--r--   0 lys       (1000) lys       (1000)    10675 2023-06-02 13:43:21.000000 draupnir-0.0.28/src/draupnir.egg-info/PKG-INFO
+-rw-r--r--   0 lys       (1000) lys       (1000)      951 2023-06-02 13:43:22.000000 draupnir-0.0.28/src/draupnir.egg-info/SOURCES.txt
+-rw-r--r--   0 lys       (1000) lys       (1000)        1 2023-06-02 13:43:21.000000 draupnir-0.0.28/src/draupnir.egg-info/dependency_links.txt
+-rw-r--r--   0 lys       (1000) lys       (1000)        1 2022-03-02 13:52:18.000000 draupnir-0.0.28/src/draupnir.egg-info/not-zip-safe
+-rw-r--r--   0 lys       (1000) lys       (1000)      229 2023-06-02 13:43:21.000000 draupnir-0.0.28/src/draupnir.egg-info/requires.txt
+-rw-r--r--   0 lys       (1000) lys       (1000)      120 2023-06-02 13:43:21.000000 draupnir-0.0.28/src/draupnir.egg-info/top_level.txt
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-02 13:43:22.081260 draupnir-0.0.28/tests/
+-rw-r--r--   0 lys       (1000) lys       (1000)     6414 2022-03-30 15:40:03.000000 draupnir-0.0.28/tests/test_accuracy.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     2173 2022-03-30 16:33:30.000000 draupnir-0.0.28/tests/test_examples.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     3793 2022-03-30 13:55:34.000000 draupnir-0.0.28/tests/test_load.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     4483 2022-03-29 19:20:16.000000 draupnir-0.0.28/tests/test_norworking.py
```

### Comparing `draupnir-0.0.27/LICENSE` & `draupnir-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/PKG-INFO` & `draupnir-0.0.28/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: draupnir
-Version: 0.0.27
+Version: 0.0.28
 Summary: Ancestral sequence reconstruction using a tree structured Ornstein Uhlenbeck variational autoencoder
 Home-page: https://github.com/LysSanzMoreta/DRAUPNIR_ASR
 Author: Lys Sanz Moreta
 Author-email: lys.sanz.moreta@outlook.com
-License: UNKNOWN
 Project-URL: Changelog, https://github.com/LysSanzMoreta/DRAUPNIR_ASR/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/LysSanzMoreta/DRAUPNIR_ASR/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 DRAUPNIR: "Beta library version for performing ASR using a tree-structured Variational Autoencoder"
@@ -62,17 +60,17 @@
 
 **Example**
 ```
 See Draupnir_example.py
 ```
 **Which guide to use?**
 
-By experience, use delta_map, the marginal results (Test folder) are the most stable.
+By experience, use delta_map, since the marginal results (Test folder) are the most stable.
 It is recommended to run the model both with the variational and the delta_map guides and compare outputs using the mutual information.
-If necessary run the variational guide longer than the delta_map, since it has more parameters to infere and takes longer.
+If necessary, run the variational guide longer than the delta_map, since it has more parameters to optimize and takes longer.
 
 **How long should I run my model?**
 
 0) Before training: 
    - It is recommended to train for at least 10000 epochs in datasets <800 leaves. See article for inspiration, the runtimes where extended to achieve maximum benchmarking accuracy, but it should not be necessary.
 1) While it is training:
    - Check for the Percent_ID.png plot, if the training accuracy has peaked to almost 100%, run for at least ~1000 epochs more to guarantee full learning
@@ -129,37 +127,41 @@
 | Simulation Sirtuin                                | 150              | 477              | simulations_sirtuins_1            |
 | Simulation SRC-kinase SH3 domain                  | 200              | 128              | simulations_src_sh3_3             |
 | Simulation PIGBOS                                 | 300              | 77               | simulations_PIGBOS_1              |
 | Simulation Insulin                                | 400              | 558              | simulations_insulin_2             |
 | Simulation SRC-kinase SH3 domain                  | 800              | 99               | simulations_src_sh3_2             |
 
 
-**What do the folders mean?**
+**What do the results folders mean?**
 
 1) If you selected **delta_map** guide:
-   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are samples obtained by using the MAP estimates of the logits.
-   2) Train_argmax_Plots: Single sequence per leaf obtained by the using the most likely amino acids indicated by the logits ("argmax the logits")
-   3) Test_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the marginal probability approach (equation 5 in the paper)
+   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are **samples** obtained by using the marginal probability approach (equation 5 in the paper).
+   2) Train_argmax_Plots: Single sequence per leaf obtained by the using the most likely amino acids indicated by the marginal logits ("argmax the logits") 
+   3) Test_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the **marginal probability** approach (equation 5 in the paper)
    4) Test_argmax_Plots: Contains the most voted sequence from the samples in Test_Plots.
-   5) Test2_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the MAP estimated of the logits. 
-   6) Test2_argmax_Plots:  Samples for the test sequences (ancestors). In this case they contain the most likely amino acids indicated by the logits ("argmax the logits") (equation 4 in the paper)
+   5) Test2_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the **MAP estimates** of the logits. 
+   6) Test2_argmax_Plots:  Samples for the test sequences (ancestors). In this case they contain the most likely amino acids indicated by the MAP logits ("argmax the logits") (equation 4 in the paper)
 2) If you selected **variational** guide:
-   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are samples obtained by using the MAP estimates of the logits.
+   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are **samples** obtained from sampling from the variational posterior (equation 6 in the paper).
    2) Train_argmax_Plots: Single sequence per leaf obtained by the using the most likely amino acids indicated by the logits ("argmax the logits")
    3) Test_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the full variational probability approach (equation 6 in the paper)
    4) Test_argmax_Plots: Contains the most voted sequence from the samples in Test_Plots.
    5) Test2_Plots == Test_Plots 
    6) Test2_argmax_Plots == Test_argmax_Plots
 
 **Where are my ancestral sequences?**
 
 - In each of the folders there should be a fasta file <dataset-name>_sampled_nodes_seq.fasta
 
 - Each of the sequences in the file should be identified as <node-name-input-tree>//<tree-level-order>\_sample\_<sample-number>
 
+    -Node-name-input-tree: Original name of the node in the given input tree
+
+    -Tree-level-order: Position of the node in tree-level order in the tree
+    
     >Node_A1//1.0_sample_0
 
     
 **If this library is useful for your research please cite:**
 
 ```
 @inproceedings{moreta2021ancestral,
@@ -167,14 +169,15 @@
   author={Moreta, Lys Sanz and R{\o}nning, Ola and Al-Sibahi, Ahmad Salim and Hein, Jotun and Theobald, Douglas and Hamelryck, Thomas},
   booktitle={International Conference on Learning Representations},
   year={2021}
 }
 ```
 
 
+**Do not hesitate to give input on how to improve the documentation of this library**
```

### Comparing `draupnir-0.0.27/README.md` & `draupnir-0.0.28/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 **Example**
 ```
 See Draupnir_example.py
 ```
 **Which guide to use?**
 
-By experience, use delta_map, the marginal results (Test folder) are the most stable.
+By experience, use delta_map, since the marginal results (Test folder) are the most stable.
 It is recommended to run the model both with the variational and the delta_map guides and compare outputs using the mutual information.
-If necessary run the variational guide longer than the delta_map, since it has more parameters to infere and takes longer.
+If necessary, run the variational guide longer than the delta_map, since it has more parameters to optimize and takes longer.
 
 **How long should I run my model?**
 
 0) Before training: 
    - It is recommended to train for at least 10000 epochs in datasets <800 leaves. See article for inspiration, the runtimes where extended to achieve maximum benchmarking accuracy, but it should not be necessary.
 1) While it is training:
    - Check for the Percent_ID.png plot, if the training accuracy has peaked to almost 100%, run for at least ~1000 epochs more to guarantee full learning
@@ -110,37 +110,41 @@
 | Simulation Sirtuin                                | 150              | 477              | simulations_sirtuins_1            |
 | Simulation SRC-kinase SH3 domain                  | 200              | 128              | simulations_src_sh3_3             |
 | Simulation PIGBOS                                 | 300              | 77               | simulations_PIGBOS_1              |
 | Simulation Insulin                                | 400              | 558              | simulations_insulin_2             |
 | Simulation SRC-kinase SH3 domain                  | 800              | 99               | simulations_src_sh3_2             |
 
 
-**What do the folders mean?**
+**What do the results folders mean?**
 
 1) If you selected **delta_map** guide:
-   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are samples obtained by using the MAP estimates of the logits.
-   2) Train_argmax_Plots: Single sequence per leaf obtained by the using the most likely amino acids indicated by the logits ("argmax the logits")
-   3) Test_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the marginal probability approach (equation 5 in the paper)
+   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are **samples** obtained by using the marginal probability approach (equation 5 in the paper).
+   2) Train_argmax_Plots: Single sequence per leaf obtained by the using the most likely amino acids indicated by the marginal logits ("argmax the logits") 
+   3) Test_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the **marginal probability** approach (equation 5 in the paper)
    4) Test_argmax_Plots: Contains the most voted sequence from the samples in Test_Plots.
-   5) Test2_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the MAP estimated of the logits. 
-   6) Test2_argmax_Plots:  Samples for the test sequences (ancestors). In this case they contain the most likely amino acids indicated by the logits ("argmax the logits") (equation 4 in the paper)
+   5) Test2_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the **MAP estimates** of the logits. 
+   6) Test2_argmax_Plots:  Samples for the test sequences (ancestors). In this case they contain the most likely amino acids indicated by the MAP logits ("argmax the logits") (equation 4 in the paper)
 2) If you selected **variational** guide:
-   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are samples obtained by using the MAP estimates of the logits.
+   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are **samples** obtained from sampling from the variational posterior (equation 6 in the paper).
    2) Train_argmax_Plots: Single sequence per leaf obtained by the using the most likely amino acids indicated by the logits ("argmax the logits")
    3) Test_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the full variational probability approach (equation 6 in the paper)
    4) Test_argmax_Plots: Contains the most voted sequence from the samples in Test_Plots.
    5) Test2_Plots == Test_Plots 
    6) Test2_argmax_Plots == Test_argmax_Plots
 
 **Where are my ancestral sequences?**
 
 - In each of the folders there should be a fasta file <dataset-name>_sampled_nodes_seq.fasta
 
 - Each of the sequences in the file should be identified as <node-name-input-tree>//<tree-level-order>\_sample\_<sample-number>
 
+    -Node-name-input-tree: Original name of the node in the given input tree
+
+    -Tree-level-order: Position of the node in tree-level order in the tree
+    
     >Node_A1//1.0_sample_0
 
     
 **If this library is useful for your research please cite:**
 
 ```
 @inproceedings{moreta2021ancestral,
@@ -148,14 +152,17 @@
   author={Moreta, Lys Sanz and R{\o}nning, Ola and Al-Sibahi, Ahmad Salim and Hein, Jotun and Theobald, Douglas and Hamelryck, Thomas},
   booktitle={International Conference on Learning Representations},
   year={2021}
 }
 ```
 
 
+**Do not hesitate to give input on how to improve the documentation of this library**
+
+
```

### Comparing `draupnir-0.0.27/setup.cfg` & `draupnir-0.0.28/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = draupnir-artistworking43
-version = 0.0.27
+version = 0.0.28
 author = Lys Sanz Moreta
 author_email = lys.sanz.moreta@outlook.com
 description = Draupnir: Ancestral protein sequence reconstruction using a tree-structured Ornstein-Uhlenbeck variational autoencoder
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/LysSanzMoreta/DRAUPNIR_ASR
 project_urls =
```

### Comparing `draupnir-0.0.27/setup.py` & `draupnir-0.0.28/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 setup(name='draupnir',
-      version='0.0.27',
+      version='0.0.28',
       # list folders, not files
       packages=find_packages('src'),
       package_dir={'': 'src'},
       py_modules=[splitext(basename(path))[0] for path in glob('src/draupnir/*.py')],
       #scripts=['bin/script1.py'],
       package_data={'draupnir': ['data/*']},
       description= 'Ancestral sequence reconstruction using a tree structured Ornstein Uhlenbeck variational autoencoder',
@@ -36,15 +36,15 @@
             #   5 - Production/Stable
             'Development Status :: 4 - Beta',
             # Pick your license as you wish
             'License :: OSI Approved :: MIT License',
             # Specify the Python versions you support here. In particular, ensure
             # that you indicate you support Python 3. These classifiers are *not*
             # checked by 'pip install'. See instead 'python_requires' below.
-            'Programming Language :: Python :: 3.7',
+            'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3 :: Only',
       ],
       python_requires='>=3.7, <4',
       project_urls={
             'Changelog': 'https://github.com/LysSanzMoreta/DRAUPNIR_ASR/blob/master/CHANGELOG.rst',
             'Issue Tracker': 'https://github.com/LysSanzMoreta/DRAUPNIR_ASR/issues',
       },
```

### Comparing `draupnir-0.0.27/src/draupnir/3D.py` & `draupnir-0.0.28/src/draupnir/3D.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/data/AA_properties.txt` & `draupnir-0.0.28/src/draupnir/data/AA_properties.txt`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/data/PfamPdbMap.txt` & `draupnir-0.0.28/src/draupnir/data/PfamPdbMap.txt`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/datasets.py` & `draupnir-0.0.28/src/draupnir/datasets.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/draw_tree.py` & `draupnir-0.0.28/src/draupnir/draw_tree.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/guides.py` & `draupnir-0.0.28/src/draupnir/guides.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/infer_angles/calculate_coords.py` & `draupnir-0.0.28/src/draupnir/infer_angles/calculate_coords.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/infer_angles/nerf.py` & `draupnir-0.0.28/src/draupnir/infer_angles/nerf.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/infer_angles/pnerf.py` & `draupnir-0.0.28/src/draupnir/infer_angles/pnerf.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/infer_angles/superposition.py` & `draupnir-0.0.28/src/draupnir/infer_angles/superposition.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/load_utils.py` & `draupnir-0.0.28/src/draupnir/load_utils.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/main.py` & `draupnir-0.0.28/src/draupnir/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,15 +528,15 @@
     """Fast version to calculate %ID among predictions and observed data, we are only using 1 sample, could use more but it's more memory expensive
     :param tensor dataset_true with shape [n_leaves,L+2,30]
     :param tensor aa_sequences_predictions"""
 
     #align_lenght = dataset_true[:, 2:, 0].shape[1]
     #aa_sequences_predictions = torch.cat((node_info, aa_sequences_predictions), dim=2)
     #aa_sequences_predictions = aa_sequences_predictions.permute(1, 0, 2) #[n_nodes,n_samples,L]
-    equal_aminoacids = (aa_sequences_predictions == dataset_true[:, 2:,0]).float()  # is correct #[n_samples,n_nodes,L] #TODO: Review this is correct because it only works because n-sample = 1
+    equal_aminoacids = (aa_sequences_predictions == dataset_true[:, 2:,0]).float()  # is correct #[n_samples,n_nodes,L]
     equal_aminoacids = (equal_aminoacids.sum(-1) / align_lenght)*100
     average_pid = equal_aminoacids.mean().cpu().numpy()
     std_pid = equal_aminoacids.std().cpu().numpy()
     return average_pid,std_pid
 def plot_percent_id(average_pid_list,std_pid_list,results_dir):
     """Plots percent id
     :param list average_pid_list
```

### Comparing `draupnir-0.0.27/src/draupnir/models.py` & `draupnir-0.0.28/src/draupnir/models.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/models_utils.py` & `draupnir-0.0.28/src/draupnir/models_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,22 +287,22 @@
     "Ancestral Inference from Functional Data: Statistical Methods and Numerical Examples"
     """
     def __init__(self, sigma_f, sigma_n, lamb):
         self.sigma_f = sigma_f
         self.sigma_n = sigma_n
         self.lamb = lamb
     def preforward(self,t1: torch.Tensor, t2: torch.Tensor) -> torch.Tensor:
-        diff = t1.unsqueeze(1) - t2.unsqueeze(0)
-        absdiff = diff.abs().sum(-1)
-        return absdiff
+        """Not used function"""
+
+        return torch.zeros((1,))
 
     def forward(self, t: torch.Tensor) -> torch.Tensor:
         #cov_b = torch.exp(-distance_matrix / _lambd) * _sigma_f ** 2 + _sigma_n + torch.eye(self.n_b*2, device=self.device) * 1e-5
         first_term = self.sigma_f ** 2
-        first_term = first_term.unsqueeze(-1).unsqueeze(-1)
+        first_term = first_term.unsqueeze(-1).unsqueeze(-1) #[:,None,None]
         lamb = self.lamb.unsqueeze(-1).unsqueeze(-1) #self.lamb[:, None, None]
         second_term = torch.exp(-t / lamb)
         noise = torch.eye(t.shape[0]) #distributes noise/stochascity to diagonal of the covariance
         sigma_n = self.sigma_n.unsqueeze(-1).unsqueeze(-1)
         return first_term * second_term + sigma_n ** 2 * noise
 class OUKernel_Fast_Sparse(GPKernel):
     """ Kernel that computes the covariance matrix for a z Ornstein Ulenbeck processes, in this case for a sparse Gaussian process. As stated in Equation 2.1 https://arxiv.org/pdf/1208.0628.pdf
```

### Comparing `draupnir-0.0.27/src/draupnir/mutual_information.py` & `draupnir-0.0.28/src/draupnir/mutual_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     print("calculating DIC coupling analysis")
     msa = parseMSA(fasta)
     #msa_refine = refineMSA(msa, label='RNAS2_HUMAN', rowocc=0.8, seqid=0.98)
     mi = buildDirectInfoMatrix(msa)
     return mi
 
 def correlation_coefficient(T1, T2):
-    """Correkation coefficient accross 2 matrices.
+    """Correlation coefficient accross 2 matrices.
     :param numpy-matrix T1
     :param numpy-matrix T2"""
     numerator = np.mean((T1 - T1.mean()) * (T2 - T2.mean()))
     denominator = T1.std() * T2.std()
     if denominator == 0:
         return 0
     else:
@@ -298,19 +298,19 @@
     :param str or None draupnir_folder_marginal: path to result of draupnir on a dataset using guide=delta_map, the results in <Test> folders are used
     :param str benchmark_folder
     :param only_root: If True it calculates MI only among the samples from the root, otherwise among all nodes
     :param only_variational: If True it will calculate DCA with a run only from the variational model, otherwise it requires to compare MAP, marginal and variational"""
     if all(v is None for v in [draupnir_folder_variational,draupnir_folder_MAP,draupnir_folder_marginal]):
         raise ValueError("Please provide at least the results for the variational guide")
     elif (draupnir_folder_MAP,draupnir_folder_variational) == (None,None) and draupnir_folder_marginal is not None:
-        warnings.warn("You have assigned draupnir_folder_MAP to None, therefore I am using the results from draupnir_folder_marginal. There are not variational guide results")
+        warnings.warn("You have assigned draupnir_folder_MAP to None, therefore I am using the results from draupnir_folder_marginal instead. There are not variational guide results")
         draupnir_folder_MAP = draupnir_folder_marginal
         MI_root_delta_map(args.name,draupnir_folder_MAP,draupnir_folder_marginal,results_dir)
     elif (draupnir_folder_marginal, draupnir_folder_variational) == (None, None) and draupnir_folder_MAP is not None:
-        warnings.warn("You have assigned draupnir_folder_marginal to None, therefore I am using the results from draupnir_folder_marginal. There are not variational guide results")
+        warnings.warn("You have assigned draupnir_folder_marginal to None, therefore I am using the results from draupnir_folder_MAP instead. There are not variational guide results")
         draupnir_folder_marginal = draupnir_folder_MAP
         MI_root_delta_map(args.name, draupnir_folder_MAP, draupnir_folder_marginal, results_dir)
     elif (draupnir_folder_MAP,draupnir_folder_marginal) == (None,None) and draupnir_folder_variational is not None:
         warnings.warn("You have assigned draupnir_folder_marginal and draupnir_folder_MAP to None. Only using variational guide results")
         MI_root_variational(args.name,draupnir_folder_variational,results_dir)
     else:
         MI_root(args.dataset_name,draupnir_folder_MAP, draupnir_folder_marginal, draupnir_folder_variational, results_dir)
```

### Comparing `draupnir-0.0.27/src/draupnir/plots.py` & `draupnir-0.0.28/src/draupnir/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,15 +519,15 @@
     #annotate = [True if latent_space.shape[0] < 100 else False][0]
     annotate = False
     stripped = False
     reducer = umap.UMAP()
     if stripped:
         clades_dict_all = additional_load.clades_dict_all
         #n_cols = DraupnirUtils.Define_batch_size(latent_space.shape[0], batch_size=False,benchmarking=True)
-        tsne_proj = reducer.fit_transform(latent_space[:, 1:])
+        umap_proj = reducer.fit_transform(latent_space[:, 1:])
 
         color_map21 = matplotlib.colors.ListedColormap(
             ["plum", "navy", "turquoise", "peachpuff", "palevioletred", "red", "darkorange", "yellow", "lime", "green",
              "dodgerblue", "blue", "purple", "magenta", "grey", "maroon", "lightcoral", "olive", "teal", "goldenrod",
              "black"])
 
         color_map_name = [color_map21 if len(clades_dict_all) <= 21 else 'nipy_spectral'][0] #nipy_spectral, gist_rainbow
@@ -535,45 +535,45 @@
         #n_cols = int(len(clades_dict_all.keys()) / 30) + 1
 
         fig, ax = plt.subplots(figsize=(22, 15),dpi=200)
 
         for idx,(clade, nodes) in enumerate(clades_dict_all.items()):
                 sequences = nodes["internal"] + nodes["leaves"]
                 indexes = (latent_space[:, 0][..., None] == sequences).any(-1)
-                ax.scatter(tsne_proj[indexes, 0], tsne_proj[indexes, 1], color=clrs(idx), label=clade.replace("_"," "), alpha=1,s=700)
+                ax.scatter(umap_proj[indexes, 0], umap_proj[indexes, 1], color=clrs(idx), label=clade.replace("_"," "), alpha=1,s=700)
                 if annotate:
-                    for name, point in zip(sequences, tsne_proj[indexes]):
+                    for name, point in zip(sequences, umap_proj[indexes]):
                         ax.annotate(name, xy=(point[0], point[1]), size=7)  # xytext=(1,1)
         #plt.legend(loc='upper left', prop={'size': 25},ncol=1, shadow=True)
         #plt.legend( bbox_to_anchor=(1.01, 1), loc='upper left', prop={'size': 25}, ncol=1, shadow=True)
         plt.tight_layout()
         plt.axis("off")
     else:
         clades_dict_all = additional_load.clades_dict_all
         # n_cols = DraupnirUtils.Define_batch_size(latent_space.shape[0], batch_size=False,benchmarking=True)
 
-        tsne_proj = reducer.fit_transform(latent_space[:, 1:])
+        umap_proj = reducer.fit_transform(latent_space[:, 1:])
         color_map21 = matplotlib.colors.ListedColormap(
             ["plum", "navy", "turquoise", "peachpuff", "palevioletred", "red", "darkorange", "yellow", "lime", "green",
              "dodgerblue", "blue", "purple", "magenta", "grey", "maroon", "lightcoral", "olive", "teal", "goldenrod",
              "black"])
 
         color_map_name = [color_map21 if len(clades_dict_all) <= 21 else 'nipy_spectral'][0]
         clrs = plt.get_cmap(color_map_name, len(clades_dict_all))
         # n_cols = int(len(clades_dict_all.keys()) / 30) + 1
 
         fig, ax = plt.subplots(figsize=(22, 15), dpi=200)
 
         for idx, (clade, nodes) in enumerate(clades_dict_all.items()):
             sequences = nodes["internal"] + nodes["leaves"]
             indexes = (latent_space[:, 0][..., None] == sequences).any(-1)
-            ax.scatter(tsne_proj[indexes, 0], tsne_proj[indexes, 1], color=clrs(idx), label=clade.replace("_", " "),
+            ax.scatter(umap_proj[indexes, 0], umap_proj[indexes, 1], color=clrs(idx), label=clade.replace("_", " "),
                        alpha=1, s=200)
             if annotate:
-                for name, point in zip(sequences, tsne_proj[indexes]):
+                for name, point in zip(sequences, umap_proj[indexes]):
                     ax.annotate(name, xy=(point[0], point[1]), size=7)  # xytext=(1,1)
         plt.legend(title='Clades', bbox_to_anchor=(1.01, 1), loc='upper left', prop={'size': 15},ncol=1,shadow=True,fontsize=15)
         plt.title("UMAP projection of the tree's latent space; \n" + "{}".format(additional_load.full_name),fontsize=20)
         plt.axis("off")
     plt.savefig("{}/UMAP_z_space_by_clade_epoch_{}.png".format(results_dir, epoch))
 def plot_latent_space_umap_by_clade_leaves(latent_space, additional_load, epoch, results_dir, triTSNE):
     """UMAP projection of a z-dimensional latent space onto a 2D space. The latent space represents the sequences in the tree. The latent space is coloured according to
```

### Comparing `draupnir-0.0.27/src/draupnir/train.py` & `draupnir-0.0.28/src/draupnir/train.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.27/src/draupnir/utils.py` & `draupnir-0.0.28/src/draupnir/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4554,2228 +4554,2229 @@
 00011c90: 5f70 6169 725f 7365 7128 7365 715f 7361  _pair_seq(seq_sa
 00011ca0: 6d70 6c65 645f 692c 7365 715f 7361 6d70  mpled_i,seq_samp
 00011cb0: 6c65 645f 6a29 0a20 2020 2020 2020 2020  led_j).         
 00011cc0: 2020 2020 2020 2020 2020 2062 6c6f 7320             blos 
 00011cd0: 3d20 7363 6f72 655f 7061 6972 7769 7365  = score_pairwise
 00011ce0: 2873 6571 5f73 616d 706c 6564 5f69 2c73  (seq_sampled_i,s
 00011cf0: 6571 5f73 616d 706c 6564 5f6a 2c62 6c6f  eq_sampled_j,blo
-00011d00: 7375 6d2c 6761 705f 733d 3131 2c20 6761  sum,gap_s=11, ga
-00011d10: 705f 653d 3129 0a20 2020 2020 2020 2020  p_e=1).         
-00011d20: 2020 2020 2020 2020 2020 2070 6572 6365             perce
-00011d30: 6e74 5f69 645f 692e 6170 7065 6e64 2870  nt_id_i.append(p
-00011d40: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
-00011d50: 2020 2020 2020 2020 626c 6f73 756d 5f73          blosum_s
-00011d60: 636f 7265 5f69 2e61 7070 656e 6428 626c  core_i.append(bl
-00011d70: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
-00011d80: 2020 2020 7374 6f72 6167 6528 290a 2020      storage().  
-00011d90: 2020 2020 2020 7265 7475 726e 2070 6572        return per
-00011da0: 6365 6e74 5f69 645f 5341 4d50 4c45 445f  cent_id_SAMPLED_
-00011db0: 5341 4d50 4c45 442c 626c 6f73 756d 5f53  SAMPLED,blosum_S
-00011dc0: 414d 504c 4544 5f53 414d 504c 4544 0a0a  AMPLED_SAMPLED..
-00011dd0: 2020 2020 6465 6620 5065 7263 656e 745f      def Percent_
-00011de0: 4944 5f54 6573 745f 5341 4d50 4c45 445f  ID_Test_SAMPLED_
-00011df0: 4f42 5345 5256 4544 286d 756c 7469 696e  OBSERVED(multiin
-00011e00: 6465 783d 4661 6c73 6529 3a0a 2020 2020  dex=False):.    
-00011e10: 2020 2020 2247 656e 6572 6174 6520 7468      "Generate th
-00011e20: 6520 4176 6572 6167 6520 616e 6420 5354  e Average and ST
-00011e30: 4420 2549 4420 616e 6420 426c 6f73 756d  D %ID and Blosum
-00011e40: 2073 636f 7265 206f 6620 7468 6520 7361   score of the sa
-00011e50: 6d70 6c65 6420 7365 7173 2076 7320 6f62  mpled seqs vs ob
-00011e60: 7320 7465 7374 220a 2020 2020 2020 2020  s test".        
-00011e70: 7065 7263 656e 745f 6964 5f53 414d 504c  percent_id_SAMPL
-00011e80: 4544 5f4f 4253 4552 5645 4420 3d20 6465  ED_OBSERVED = de
-00011e90: 6661 756c 7464 6963 7428 6c61 6d62 6461  faultdict(lambda
-00011ea0: 3a20 6465 6661 756c 7464 6963 7428 6c61  : defaultdict(la
-00011eb0: 6d62 6461 3a20 6465 6661 756c 7464 6963  mbda: defaultdic
-00011ec0: 7428 6469 6374 2929 290a 2020 2020 2020  t(dict))).      
-00011ed0: 2020 626c 6f73 756d 5f53 414d 504c 4544    blosum_SAMPLED
-00011ee0: 5f4f 4253 4552 5645 4420 3d20 6465 6661  _OBSERVED = defa
-00011ef0: 756c 7464 6963 7428 6c61 6d62 6461 3a20  ultdict(lambda: 
-00011f00: 6465 6661 756c 7464 6963 7428 6c61 6d62  defaultdict(lamb
-00011f10: 6461 3a20 6465 6661 756c 7464 6963 7428  da: defaultdict(
-00011f20: 6469 6374 2929 290a 2020 2020 2020 2020  dict))).        
-00011f30: 696e 636f 7272 6563 745f 5341 4d50 4c45  incorrect_SAMPLE
-00011f40: 445f 4f42 5345 5256 4544 203d 2064 6566  D_OBSERVED = def
-00011f50: 6175 6c74 6469 6374 286c 616d 6264 613a  aultdict(lambda:
-00011f60: 2064 6566 6175 6c74 6469 6374 286c 616d   defaultdict(lam
-00011f70: 6264 613a 2064 6566 6175 6c74 6469 6374  bda: defaultdict
-00011f80: 2864 6963 7429 2929 0a20 2020 2020 2020  (dict))).       
-00011f90: 2044 6174 6173 6574 5f74 6573 745f 736c   Dataset_test_sl
-00011fa0: 6963 6564 203d 2064 6174 6173 6574 5f74  iced = dataset_t
-00011fb0: 6573 745b 3a2c 323a 2c30 5d0a 2020 2020  est[:,2:,0].    
-00011fc0: 2020 2020 7072 6564 6963 7469 6f6e 735f      predictions_
-00011fd0: 7361 6d70 6c65 735f 736c 6963 6564 203d  samples_sliced =
-00011fe0: 2070 7265 6469 6374 696f 6e73 5f73 616d   predictions_sam
-00011ff0: 706c 6573 5b3a 2c3a 2c33 3a5d 0a20 2020  ples[:,:,3:].   
-00012000: 2020 2020 2069 6620 6d75 6c74 6969 6e64       if multiind
-00012010: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
-00012020: 6465 6620 7374 6f72 6167 6528 293a 0a20  def storage():. 
-00012030: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00012040: 6572 6365 6e74 5f69 645f 5341 4d50 4c45  ercent_id_SAMPLE
-00012050: 445f 4f42 5345 5256 4544 5b74 315d 5b74  D_OBSERVED[t1][t
-00012060: 325d 5b22 4176 6572 6167 6522 5d20 3d20  2]["Average"] = 
-00012070: 6e70 2e6d 6561 6e28 6e70 2e61 7272 6179  np.mean(np.array
-00012080: 2870 6572 6365 6e74 5f69 645f 6929 2c20  (percent_id_i), 
-00012090: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
-000120a0: 2020 2020 2020 2020 7065 7263 656e 745f          percent_
-000120b0: 6964 5f53 414d 504c 4544 5f4f 4253 4552  id_SAMPLED_OBSER
-000120c0: 5645 445b 7431 5d5b 7432 5d5b 2253 7464  VED[t1][t2]["Std
-000120d0: 225d 203d 206e 702e 7374 6428 6e70 2e61  "] = np.std(np.a
-000120e0: 7272 6179 2870 6572 6365 6e74 5f69 645f  rray(percent_id_
-000120f0: 6929 2c20 6178 6973 3d30 290a 2020 2020  i), axis=0).    
-00012100: 2020 2020 2020 2020 2020 2020 626c 6f73              blos
-00012110: 756d 5f53 414d 504c 4544 5f4f 4253 4552  um_SAMPLED_OBSER
-00012120: 5645 445b 7431 5d5b 7432 5d5b 2241 7665  VED[t1][t2]["Ave
-00012130: 7261 6765 225d 203d 206e 702e 6d65 616e  rage"] = np.mean
-00012140: 286e 702e 6172 7261 7928 626c 6f73 756d  (np.array(blosum
-00012150: 5f73 636f 7265 5f69 292c 2061 7869 733d  _score_i), axis=
-00012160: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-00012170: 2020 2062 6c6f 7375 6d5f 5341 4d50 4c45     blosum_SAMPLE
-00012180: 445f 4f42 5345 5256 4544 5b74 315d 5b74  D_OBSERVED[t1][t
-00012190: 325d 5b22 5374 6422 5d20 3d20 6e70 2e73  2]["Std"] = np.s
-000121a0: 7464 286e 702e 6172 7261 7928 626c 6f73  td(np.array(blos
-000121b0: 756d 5f73 636f 7265 5f69 292c 2061 7869  um_score_i), axi
-000121c0: 733d 3029 0a20 2020 2020 2020 2020 2020  s=0).           
-000121d0: 2020 2020 2023 2069 6e63 6f72 7265 6374       # incorrect
-000121e0: 5f53 414d 504c 4544 5f4f 4253 4552 5645  _SAMPLED_OBSERVE
-000121f0: 445b 6e6f 6465 5f6e 616d 6573 5b69 5d2e  D[node_names[i].
-00012200: 6974 656d 2829 5d5b 6e6f 6465 5f6e 616d  item()][node_nam
-00012210: 6573 5b6a 5d2e 6974 656d 2829 5d20 5b22  es[j].item()] ["
-00012220: 4176 6572 6167 6522 5d20 3d20 6e70 2e6d  Average"] = np.m
-00012230: 6561 6e28 6e70 2e61 7272 6179 2869 6e63  ean(np.array(inc
-00012240: 6f72 7265 6374 5f61 615f 6929 2c20 6178  orrect_aa_i), ax
-00012250: 6973 3d30 290a 2020 2020 2020 2020 2020  is=0).          
-00012260: 2020 2020 2020 2320 696e 636f 7272 6563        # incorrec
-00012270: 745f 5341 4d50 4c45 445f 4f42 5345 5256  t_SAMPLED_OBSERV
-00012280: 4544 5b6e 6f64 655f 6e61 6d65 735b 695d  ED[node_names[i]
-00012290: 2e69 7465 6d28 295d 5b6e 6f64 655f 6e61  .item()][node_na
-000122a0: 6d65 735b 6a5d 2e69 7465 6d28 295d 205b  mes[j].item()] [
-000122b0: 2253 7464 225d 203d 206e 702e 7374 6428  "Std"] = np.std(
-000122c0: 6e70 2e61 7272 6179 2869 6e63 6f72 7265  np.array(incorre
-000122d0: 6374 5f61 615f 6929 2c20 6178 6973 3d30  ct_aa_i), axis=0
-000122e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-000122f0: 2020 2020 2020 2020 2020 2020 6465 6620              def 
-00012300: 7374 6f72 6167 6528 293a 0a20 2020 2020  storage():.     
-00012310: 2020 2020 2020 2020 2020 2070 6572 6365             perce
-00012320: 6e74 5f69 645f 5341 4d50 4c45 445f 4f42  nt_id_SAMPLED_OB
-00012330: 5345 5256 4544 5b74 315d 5b74 325d 2020  SERVED[t1][t2]  
-00012340: 3d20 6e70 2e6d 6561 6e28 6e70 2e61 7272  = np.mean(np.arr
-00012350: 6179 2870 6572 6365 6e74 5f69 645f 6929  ay(percent_id_i)
-00012360: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
-00012370: 2020 2020 2020 2020 2020 626c 6f73 756d            blosum
-00012380: 5f53 414d 504c 4544 5f4f 4253 4552 5645  _SAMPLED_OBSERVE
-00012390: 445b 7431 5d5b 7432 5d20 203d 206e 702e  D[t1][t2]  = np.
-000123a0: 6d65 616e 286e 702e 6172 7261 7928 626c  mean(np.array(bl
-000123b0: 6f73 756d 5f73 636f 7265 5f69 292c 2061  osum_score_i), a
-000123c0: 7869 733d 3029 0a20 2020 2020 2020 2020  xis=0).         
-000123d0: 2020 2020 2020 2023 696e 636f 7272 6563         #incorrec
-000123e0: 745f 5341 4d50 4c45 445f 4f42 5345 5256  t_SAMPLED_OBSERV
-000123f0: 4544 5b6e 6f64 655f 6e61 6d65 735b 695d  ED[node_names[i]
-00012400: 2e69 7465 6d28 295d 5b6e 6f64 655f 6e61  .item()][node_na
-00012410: 6d65 735b 6a5d 2e69 7465 6d28 295d 2020  mes[j].item()]  
-00012420: 3d20 6e70 2e6d 6561 6e28 6e70 2e61 7272  = np.mean(np.arr
-00012430: 6179 2869 6e63 6f72 7265 6374 5f61 615f  ay(incorrect_aa_
-00012440: 6929 2c20 6178 6973 3d30 290a 2020 2020  i), axis=0).    
-00012450: 2020 2020 666f 7220 692c 2074 3120 696e      for i, t1 in
-00012460: 2065 6e75 6d65 7261 7465 286e 6f64 6573   enumerate(nodes
-00012470: 5f69 6e64 6578 6573 293a 0a20 2020 2020  _indexes):.     
-00012480: 2020 2020 2020 2074 6573 745f 6f62 735f         test_obs_
-00012490: 6920 3d20 636f 6e76 6572 745f 746f 5f6c  i = convert_to_l
-000124a0: 6574 7465 7273 2844 6174 6173 6574 5f74  etters(Dataset_t
-000124b0: 6573 745f 736c 6963 6564 5b69 5d2c 6161  est_sliced[i],aa
-000124c0: 5f70 726f 6273 290a 2020 2020 2020 2020  _probs).        
-000124d0: 2020 2020 666f 7220 6a2c 2074 3220 696e      for j, t2 in
-000124e0: 2065 6e75 6d65 7261 7465 286e 6f64 6573   enumerate(nodes
-000124f0: 5f69 6e64 6578 6573 5b69 3a5d 293a 2020  _indexes[i:]):  
-00012500: 2320 666f 7220 7465 7374 206e 6f64 650a  # for test node.
-00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012520: 616c 6c5f 7361 6d70 6c65 645f 7465 7374  all_sampled_test
-00012530: 203d 2070 7265 6469 6374 696f 6e73 5f73   = predictions_s
-00012540: 616d 706c 6573 5f73 6c69 6365 645b 3a2c  amples_sliced[:,
-00012550: 2069 2b6a 5d20 2023 2041 6c6c 2073 616d   i+j]  # All sam
-00012560: 706c 6573 2066 6f72 2074 6865 2073 616d  ples for the sam
-00012570: 6520 7465 7374 2073 6571 0a20 2020 2020  e test seq.     
-00012580: 2020 2020 2020 2020 2020 2070 6572 6365             perce
-00012590: 6e74 5f69 645f 6920 3d20 5b5d 0a20 2020  nt_id_i = [].   
-000125a0: 2020 2020 2020 2020 2020 2020 2062 6c6f               blo
-000125b0: 7375 6d5f 7363 6f72 655f 6920 3d20 5b5d  sum_score_i = []
-000125c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000125d0: 2023 696e 636f 7272 6563 745f 6161 5f69   #incorrect_aa_i
-000125e0: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-000125f0: 2020 2020 2020 666f 7220 7720 696e 2072        for w in r
-00012600: 616e 6765 286e 756d 5f73 616d 706c 6573  ange(num_samples
-00012610: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00012620: 2020 2020 2020 2073 6571 5f73 616d 706c         seq_sampl
-00012630: 6564 5f74 6573 7420 3d20 636f 6e76 6572  ed_test = conver
-00012640: 745f 746f 5f6c 6574 7465 7273 2861 6c6c  t_to_letters(all
-00012650: 5f73 616d 706c 6564 5f74 6573 745b 775d  _sampled_test[w]
-00012660: 2c61 615f 7072 6f62 7329 0a20 2020 2020  ,aa_probs).     
-00012670: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00012680: 6964 203d 2070 6572 635f 6964 656e 7469  id = perc_identi
-00012690: 7479 5f70 6169 725f 7365 7128 7465 7374  ty_pair_seq(test
-000126a0: 5f6f 6273 5f69 2c20 7365 715f 7361 6d70  _obs_i, seq_samp
-000126b0: 6c65 645f 7465 7374 290a 2020 2020 2020  led_test).      
-000126c0: 2020 2020 2020 2020 2020 2020 2020 2377                #w
-000126d0: 726f 6e67 5f70 7265 6420 3d20 696e 636f  rong_pred = inco
-000126e0: 7272 6563 746c 795f 7072 6564 6963 7465  rrectly_predicte
-000126f0: 645f 6161 2874 6573 745f 6f62 735f 692c  d_aa(test_obs_i,
-00012700: 7365 715f 7361 6d70 6c65 645f 7465 7374  seq_sampled_test
-00012710: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012720: 2020 2020 2020 626c 6f73 203d 2073 636f        blos = sco
-00012730: 7265 5f70 6169 7277 6973 6528 7465 7374  re_pairwise(test
-00012740: 5f6f 6273 5f69 2c20 7365 715f 7361 6d70  _obs_i, seq_samp
-00012750: 6c65 645f 7465 7374 2c20 626c 6f73 756d  led_test, blosum
-00012760: 2c20 6761 705f 733d 3131 2c20 6761 705f  , gap_s=11, gap_
-00012770: 653d 3129 0a20 2020 2020 2020 2020 2020  e=1).           
-00012780: 2020 2020 2020 2020 2070 6572 6365 6e74           percent
-00012790: 5f69 645f 692e 6170 7065 6e64 2870 6964  _id_i.append(pid
-000127a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000127b0: 2020 2020 2020 626c 6f73 756d 5f73 636f        blosum_sco
-000127c0: 7265 5f69 2e61 7070 656e 6428 626c 6f73  re_i.append(blos
-000127d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000127e0: 2020 2020 2020 2369 6e63 6f72 7265 6374        #incorrect
-000127f0: 5f61 615f 692e 6170 7065 6e64 2877 726f  _aa_i.append(wro
-00012800: 6e67 5f70 7265 6429 0a20 2020 2020 2020  ng_pred).       
-00012810: 2020 2020 2020 2020 2073 746f 7261 6765           storage
-00012820: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00012830: 6e20 7065 7263 656e 745f 6964 5f53 414d  n percent_id_SAM
-00012840: 504c 4544 5f4f 4253 4552 5645 442c 626c  PLED_OBSERVED,bl
-00012850: 6f73 756d 5f53 414d 504c 4544 5f4f 4253  osum_SAMPLED_OBS
-00012860: 4552 5645 442c 696e 636f 7272 6563 745f  ERVED,incorrect_
-00012870: 5341 4d50 4c45 445f 4f42 5345 5256 4544  SAMPLED_OBSERVED
-00012880: 0a0a 2020 2020 6465 6620 5065 7263 656e  ..    def Percen
-00012890: 745f 4944 5f54 6573 745f 4f42 535f 4f42  t_ID_Test_OBS_OB
-000128a0: 5345 5256 4544 2829 3a0a 2020 2020 2020  SERVED():.      
-000128b0: 2020 2247 656e 6572 6174 6520 7468 6520    "Generate the 
-000128c0: 4176 6572 6167 6520 616e 6420 5354 4420  Average and STD 
-000128d0: 2549 4420 616d 6f6e 6720 6f62 7320 7465  %ID among obs te
-000128e0: 7374 220a 2020 2020 2020 2020 7065 7263  st".        perc
-000128f0: 656e 745f 6964 5f4f 4253 203d 2064 6566  ent_id_OBS = def
-00012900: 6175 6c74 6469 6374 286c 616d 6264 613a  aultdict(lambda:
-00012910: 2064 6566 6175 6c74 6469 6374 286c 616d   defaultdict(lam
-00012920: 6264 613a 2064 6566 6175 6c74 6469 6374  bda: defaultdict
-00012930: 2864 6963 7429 2929 0a20 2020 2020 2020  (dict))).       
-00012940: 2062 6c6f 7375 6d5f 4f42 5320 3d20 6465   blosum_OBS = de
-00012950: 6661 756c 7464 6963 7428 6c61 6d62 6461  faultdict(lambda
-00012960: 3a20 6465 6661 756c 7464 6963 7428 6c61  : defaultdict(la
-00012970: 6d62 6461 3a20 6465 6661 756c 7464 6963  mbda: defaultdic
-00012980: 7428 6469 6374 2929 290a 0a20 2020 2020  t(dict)))..     
-00012990: 2020 2044 6174 6173 6574 5f74 6573 745f     Dataset_test_
-000129a0: 736c 6963 6564 203d 2064 6174 6173 6574  sliced = dataset
-000129b0: 5f74 6573 745b 3a2c 323a 2c30 5d0a 2020  _test[:,2:,0].  
-000129c0: 2020 2020 2020 666f 7220 692c 2074 3120        for i, t1 
-000129d0: 696e 2065 6e75 6d65 7261 7465 286e 6f64  in enumerate(nod
-000129e0: 6573 5f69 6e64 6578 6573 293a 0a20 2020  es_indexes):.   
-000129f0: 2020 2020 2020 2020 2074 6573 745f 6f62           test_ob
-00012a00: 735f 6920 3d20 636f 6e76 6572 745f 746f  s_i = convert_to
-00012a10: 5f6c 6574 7465 7273 2844 6174 6173 6574  _letters(Dataset
-00012a20: 5f74 6573 745f 736c 6963 6564 5b69 5d2c  _test_sliced[i],
-00012a30: 6161 5f70 726f 6273 290a 2020 2020 2020  aa_probs).      
-00012a40: 2020 2020 2020 2370 6572 6365 6e74 5f69        #percent_i
-00012a50: 645f 4f42 535b 4461 7461 7365 745f 7465  d_OBS[Dataset_te
-00012a60: 7374 5b69 2c20 302c 2031 5d2e 6974 656d  st[i, 0, 1].item
-00012a70: 2829 5d5b 4461 7461 7365 745f 7465 7374  ()][Dataset_test
-00012a80: 5b69 2c20 302c 2031 5d2e 6974 656d 2829  [i, 0, 1].item()
-00012a90: 5d20 3d20 7065 7263 5f69 6465 6e74 6974  ] = perc_identit
-00012aa0: 795f 7061 6972 5f73 6571 2874 6573 745f  y_pair_seq(test_
-00012ab0: 6f62 735f 692c 2074 6573 745f 6f62 735f  obs_i, test_obs_
-00012ac0: 6929 0a20 2020 2020 2020 2020 2020 2066  i).            f
-00012ad0: 6f72 206a 2c20 7432 2069 6e20 656e 756d  or j, t2 in enum
-00012ae0: 6572 6174 6528 6e6f 6465 735f 696e 6465  erate(nodes_inde
-00012af0: 7865 735b 693a 5d29 3a0a 2020 2020 2020  xes[i:]):.      
-00012b00: 2020 2020 2020 2020 2020 7465 7374 5f6f            test_o
-00012b10: 6273 5f6a 203d 2063 6f6e 7665 7274 5f74  bs_j = convert_t
-00012b20: 6f5f 6c65 7474 6572 7328 4461 7461 7365  o_letters(Datase
-00012b30: 745f 7465 7374 5f73 6c69 6365 645b 692b  t_test_sliced[i+
-00012b40: 6a5d 2c61 615f 7072 6f62 7329 0a20 2020  j],aa_probs).   
-00012b50: 2020 2020 2020 2020 2020 2020 2070 6964               pid
-00012b60: 5f73 636f 7265 203d 2070 6572 635f 6964  _score = perc_id
-00012b70: 656e 7469 7479 5f70 6169 725f 7365 7128  entity_pair_seq(
-00012b80: 7465 7374 5f6f 6273 5f69 2c74 6573 745f  test_obs_i,test_
-00012b90: 6f62 735f 6a29 0a20 2020 2020 2020 2020  obs_j).         
-00012ba0: 2020 2020 2020 2070 6572 6365 6e74 5f69         percent_i
-00012bb0: 645f 4f42 535b 7431 5d5b 7432 5d20 3d20  d_OBS[t1][t2] = 
-00012bc0: 7069 645f 7363 6f72 650a 2020 2020 2020  pid_score.      
-00012bd0: 2020 2020 2020 2020 2020 626c 6f73 756d            blosum
-00012be0: 5f73 636f 7265 203d 2073 636f 7265 5f70  _score = score_p
-00012bf0: 6169 7277 6973 6528 7465 7374 5f6f 6273  airwise(test_obs
-00012c00: 5f69 2c74 6573 745f 6f62 735f 6a2c 2062  _i,test_obs_j, b
-00012c10: 6c6f 7375 6d2c 2067 6170 5f73 3d31 312c  losum, gap_s=11,
-00012c20: 2067 6170 5f65 3d31 290a 2020 2020 2020   gap_e=1).      
-00012c30: 2020 2020 2020 2020 2020 626c 6f73 756d            blosum
-00012c40: 5f4f 4253 5b74 315d 5b74 325d 203d 2062  _OBS[t1][t2] = b
-00012c50: 6c6f 7375 6d5f 7363 6f72 650a 2020 2020  losum_score.    
-00012c60: 2020 2020 7265 7475 726e 2070 6572 6365      return perce
-00012c70: 6e74 5f69 645f 4f42 532c 626c 6f73 756d  nt_id_OBS,blosum
-00012c80: 5f4f 4253 0a0a 2020 2020 6465 6620 506c  _OBS..    def Pl
-00012c90: 6f74 5f48 6561 746d 6170 2864 662c 7469  ot_Heatmap(df,ti
-00012ca0: 746c 652c 7469 746c 6532 2c61 6e6e 6f74  tle,title2,annot
-00012cb0: 2c6d 6173 6b2c 766d 6178 293a 0a20 2020  ,mask,vmax):.   
-00012cc0: 2020 2020 2066 6967 2c61 7820 3d20 2070       fig,ax =  p
-00012cd0: 6c74 2e73 7562 706c 6f74 7328 312c 2031  lt.subplots(1, 1
-00012ce0: 2c66 6967 7369 7a65 3d28 3130 2c31 3029  ,figsize=(10,10)
-00012cf0: 290a 2020 2020 2020 2020 686d 6170 203d  ).        hmap =
-00012d00: 2073 6e73 2e68 6561 746d 6170 2864 662c   sns.heatmap(df,
-00012d10: 2063 6d61 703d 2253 7065 6374 7261 6c22   cmap="Spectral"
-00012d20: 2c61 6e6e 6f74 3d61 6e6e 6f74 2c61 6e6e  ,annot=annot,ann
-00012d30: 6f74 5f6b 7773 3d7b 2266 6f6e 7473 697a  ot_kws={"fontsiz
-00012d40: 6522 3a36 7d2c 6d61 736b 3d6d 6173 6b2c  e":6},mask=mask,
-00012d50: 766d 6178 3d76 6d61 7829 0a20 2020 2020  vmax=vmax).     
-00012d60: 2020 2061 782e 7365 745f 7469 746c 6528     ax.set_title(
-00012d70: 227b 7d20 3b5c 6e22 2e66 6f72 6d61 7428  "{} ;\n".format(
-00012d80: 7469 746c 6529 202b 2072 227b 7d22 2e66  title) + r"{}".f
-00012d90: 6f72 6d61 7428 6164 6469 7469 6f6e 616c  ormat(additional
-00012da0: 5f6c 6f61 642e 6675 6c6c 5f6e 616d 6529  _load.full_name)
-00012db0: 290a 2020 2020 2020 2020 6178 2e73 6574  ).        ax.set
-00012dc0: 5f78 6c61 6265 6c28 7469 746c 6532 2e73  _xlabel(title2.s
-00012dd0: 706c 6974 2822 5f22 295b 2d31 5d29 0a20  plit("_")[-1]). 
-00012de0: 2020 2020 2020 2061 782e 7365 745f 796c         ax.set_yl
-00012df0: 6162 656c 2874 6974 6c65 322e 7370 6c69  abel(title2.spli
-00012e00: 7428 225f 2229 5b2d 325d 290a 2020 2020  t("_")[-2]).    
-00012e10: 2020 2020 686d 6170 2e66 6967 7572 652e      hmap.figure.
-00012e20: 7361 7665 6669 6728 227b 7d2f 4865 6174  savefig("{}/Heat
-00012e30: 6d61 705f 7b7d 2e70 6e67 222e 666f 726d  map_{}.png".form
-00012e40: 6174 2872 6573 756c 7473 5f64 6972 6563  at(results_direc
-00012e50: 746f 7279 2c74 6974 6c65 3229 2c0a 2020  tory,title2),.  
-00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e70: 2020 2020 2020 2020 2020 666f 726d 6174            format
-00012e80: 3d27 706e 6727 2c0a 2020 2020 2020 2020  ='png',.        
+00011d00: 7375 6d2c 6761 705f 733d 2d31 312c 2067  sum,gap_s=-11, g
+00011d10: 6170 5f65 3d2d 3129 0a20 2020 2020 2020  ap_e=-1).       
+00011d20: 2020 2020 2020 2020 2020 2020 2070 6572               per
+00011d30: 6365 6e74 5f69 645f 692e 6170 7065 6e64  cent_id_i.append
+00011d40: 2870 6964 290a 2020 2020 2020 2020 2020  (pid).          
+00011d50: 2020 2020 2020 2020 2020 626c 6f73 756d            blosum
+00011d60: 5f73 636f 7265 5f69 2e61 7070 656e 6428  _score_i.append(
+00011d70: 626c 6f73 290a 2020 2020 2020 2020 2020  blos).          
+00011d80: 2020 2020 2020 7374 6f72 6167 6528 290a        storage().
+00011d90: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+00011da0: 6572 6365 6e74 5f69 645f 5341 4d50 4c45  ercent_id_SAMPLE
+00011db0: 445f 5341 4d50 4c45 442c 626c 6f73 756d  D_SAMPLED,blosum
+00011dc0: 5f53 414d 504c 4544 5f53 414d 504c 4544  _SAMPLED_SAMPLED
+00011dd0: 0a0a 2020 2020 6465 6620 5065 7263 656e  ..    def Percen
+00011de0: 745f 4944 5f54 6573 745f 5341 4d50 4c45  t_ID_Test_SAMPLE
+00011df0: 445f 4f42 5345 5256 4544 286d 756c 7469  D_OBSERVED(multi
+00011e00: 696e 6465 783d 4661 6c73 6529 3a0a 2020  index=False):.  
+00011e10: 2020 2020 2020 2247 656e 6572 6174 6520        "Generate 
+00011e20: 7468 6520 4176 6572 6167 6520 616e 6420  the Average and 
+00011e30: 5354 4420 2549 4420 616e 6420 426c 6f73  STD %ID and Blos
+00011e40: 756d 2073 636f 7265 206f 6620 7468 6520  um score of the 
+00011e50: 7361 6d70 6c65 6420 7365 7173 2076 7320  sampled seqs vs 
+00011e60: 6f62 7320 7465 7374 220a 2020 2020 2020  obs test".      
+00011e70: 2020 7065 7263 656e 745f 6964 5f53 414d    percent_id_SAM
+00011e80: 504c 4544 5f4f 4253 4552 5645 4420 3d20  PLED_OBSERVED = 
+00011e90: 6465 6661 756c 7464 6963 7428 6c61 6d62  defaultdict(lamb
+00011ea0: 6461 3a20 6465 6661 756c 7464 6963 7428  da: defaultdict(
+00011eb0: 6c61 6d62 6461 3a20 6465 6661 756c 7464  lambda: defaultd
+00011ec0: 6963 7428 6469 6374 2929 290a 2020 2020  ict(dict))).    
+00011ed0: 2020 2020 626c 6f73 756d 5f53 414d 504c      blosum_SAMPL
+00011ee0: 4544 5f4f 4253 4552 5645 4420 3d20 6465  ED_OBSERVED = de
+00011ef0: 6661 756c 7464 6963 7428 6c61 6d62 6461  faultdict(lambda
+00011f00: 3a20 6465 6661 756c 7464 6963 7428 6c61  : defaultdict(la
+00011f10: 6d62 6461 3a20 6465 6661 756c 7464 6963  mbda: defaultdic
+00011f20: 7428 6469 6374 2929 290a 2020 2020 2020  t(dict))).      
+00011f30: 2020 696e 636f 7272 6563 745f 5341 4d50    incorrect_SAMP
+00011f40: 4c45 445f 4f42 5345 5256 4544 203d 2064  LED_OBSERVED = d
+00011f50: 6566 6175 6c74 6469 6374 286c 616d 6264  efaultdict(lambd
+00011f60: 613a 2064 6566 6175 6c74 6469 6374 286c  a: defaultdict(l
+00011f70: 616d 6264 613a 2064 6566 6175 6c74 6469  ambda: defaultdi
+00011f80: 6374 2864 6963 7429 2929 0a20 2020 2020  ct(dict))).     
+00011f90: 2020 2044 6174 6173 6574 5f74 6573 745f     Dataset_test_
+00011fa0: 736c 6963 6564 203d 2064 6174 6173 6574  sliced = dataset
+00011fb0: 5f74 6573 745b 3a2c 323a 2c30 5d0a 2020  _test[:,2:,0].  
+00011fc0: 2020 2020 2020 7072 6564 6963 7469 6f6e        prediction
+00011fd0: 735f 7361 6d70 6c65 735f 736c 6963 6564  s_samples_sliced
+00011fe0: 203d 2070 7265 6469 6374 696f 6e73 5f73   = predictions_s
+00011ff0: 616d 706c 6573 5b3a 2c3a 2c33 3a5d 0a20  amples[:,:,3:]. 
+00012000: 2020 2020 2020 2069 6620 6d75 6c74 6969         if multii
+00012010: 6e64 6578 3a0a 2020 2020 2020 2020 2020  ndex:.          
+00012020: 2020 6465 6620 7374 6f72 6167 6528 293a    def storage():
+00012030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012040: 2070 6572 6365 6e74 5f69 645f 5341 4d50   percent_id_SAMP
+00012050: 4c45 445f 4f42 5345 5256 4544 5b74 315d  LED_OBSERVED[t1]
+00012060: 5b74 325d 5b22 4176 6572 6167 6522 5d20  [t2]["Average"] 
+00012070: 3d20 6e70 2e6d 6561 6e28 6e70 2e61 7272  = np.mean(np.arr
+00012080: 6179 2870 6572 6365 6e74 5f69 645f 6929  ay(percent_id_i)
+00012090: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
+000120a0: 2020 2020 2020 2020 2020 7065 7263 656e            percen
+000120b0: 745f 6964 5f53 414d 504c 4544 5f4f 4253  t_id_SAMPLED_OBS
+000120c0: 4552 5645 445b 7431 5d5b 7432 5d5b 2253  ERVED[t1][t2]["S
+000120d0: 7464 225d 203d 206e 702e 7374 6428 6e70  td"] = np.std(np
+000120e0: 2e61 7272 6179 2870 6572 6365 6e74 5f69  .array(percent_i
+000120f0: 645f 6929 2c20 6178 6973 3d30 290a 2020  d_i), axis=0).  
+00012100: 2020 2020 2020 2020 2020 2020 2020 626c                bl
+00012110: 6f73 756d 5f53 414d 504c 4544 5f4f 4253  osum_SAMPLED_OBS
+00012120: 4552 5645 445b 7431 5d5b 7432 5d5b 2241  ERVED[t1][t2]["A
+00012130: 7665 7261 6765 225d 203d 206e 702e 6d65  verage"] = np.me
+00012140: 616e 286e 702e 6172 7261 7928 626c 6f73  an(np.array(blos
+00012150: 756d 5f73 636f 7265 5f69 292c 2061 7869  um_score_i), axi
+00012160: 733d 3029 0a20 2020 2020 2020 2020 2020  s=0).           
+00012170: 2020 2020 2062 6c6f 7375 6d5f 5341 4d50       blosum_SAMP
+00012180: 4c45 445f 4f42 5345 5256 4544 5b74 315d  LED_OBSERVED[t1]
+00012190: 5b74 325d 5b22 5374 6422 5d20 3d20 6e70  [t2]["Std"] = np
+000121a0: 2e73 7464 286e 702e 6172 7261 7928 626c  .std(np.array(bl
+000121b0: 6f73 756d 5f73 636f 7265 5f69 292c 2061  osum_score_i), a
+000121c0: 7869 733d 3029 0a20 2020 2020 2020 2020  xis=0).         
+000121d0: 2020 2020 2020 2023 2069 6e63 6f72 7265         # incorre
+000121e0: 6374 5f53 414d 504c 4544 5f4f 4253 4552  ct_SAMPLED_OBSER
+000121f0: 5645 445b 6e6f 6465 5f6e 616d 6573 5b69  VED[node_names[i
+00012200: 5d2e 6974 656d 2829 5d5b 6e6f 6465 5f6e  ].item()][node_n
+00012210: 616d 6573 5b6a 5d2e 6974 656d 2829 5d20  ames[j].item()] 
+00012220: 5b22 4176 6572 6167 6522 5d20 3d20 6e70  ["Average"] = np
+00012230: 2e6d 6561 6e28 6e70 2e61 7272 6179 2869  .mean(np.array(i
+00012240: 6e63 6f72 7265 6374 5f61 615f 6929 2c20  ncorrect_aa_i), 
+00012250: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+00012260: 2020 2020 2020 2020 2320 696e 636f 7272          # incorr
+00012270: 6563 745f 5341 4d50 4c45 445f 4f42 5345  ect_SAMPLED_OBSE
+00012280: 5256 4544 5b6e 6f64 655f 6e61 6d65 735b  RVED[node_names[
+00012290: 695d 2e69 7465 6d28 295d 5b6e 6f64 655f  i].item()][node_
+000122a0: 6e61 6d65 735b 6a5d 2e69 7465 6d28 295d  names[j].item()]
+000122b0: 205b 2253 7464 225d 203d 206e 702e 7374   ["Std"] = np.st
+000122c0: 6428 6e70 2e61 7272 6179 2869 6e63 6f72  d(np.array(incor
+000122d0: 7265 6374 5f61 615f 6929 2c20 6178 6973  rect_aa_i), axis
+000122e0: 3d30 290a 2020 2020 2020 2020 656c 7365  =0).        else
+000122f0: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+00012300: 6620 7374 6f72 6167 6528 293a 0a20 2020  f storage():.   
+00012310: 2020 2020 2020 2020 2020 2020 2070 6572               per
+00012320: 6365 6e74 5f69 645f 5341 4d50 4c45 445f  cent_id_SAMPLED_
+00012330: 4f42 5345 5256 4544 5b74 315d 5b74 325d  OBSERVED[t1][t2]
+00012340: 2020 3d20 6e70 2e6d 6561 6e28 6e70 2e61    = np.mean(np.a
+00012350: 7272 6179 2870 6572 6365 6e74 5f69 645f  rray(percent_id_
+00012360: 6929 2c20 6178 6973 3d30 290a 2020 2020  i), axis=0).    
+00012370: 2020 2020 2020 2020 2020 2020 626c 6f73              blos
+00012380: 756d 5f53 414d 504c 4544 5f4f 4253 4552  um_SAMPLED_OBSER
+00012390: 5645 445b 7431 5d5b 7432 5d20 203d 206e  VED[t1][t2]  = n
+000123a0: 702e 6d65 616e 286e 702e 6172 7261 7928  p.mean(np.array(
+000123b0: 626c 6f73 756d 5f73 636f 7265 5f69 292c  blosum_score_i),
+000123c0: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
+000123d0: 2020 2020 2020 2020 2023 696e 636f 7272           #incorr
+000123e0: 6563 745f 5341 4d50 4c45 445f 4f42 5345  ect_SAMPLED_OBSE
+000123f0: 5256 4544 5b6e 6f64 655f 6e61 6d65 735b  RVED[node_names[
+00012400: 695d 2e69 7465 6d28 295d 5b6e 6f64 655f  i].item()][node_
+00012410: 6e61 6d65 735b 6a5d 2e69 7465 6d28 295d  names[j].item()]
+00012420: 2020 3d20 6e70 2e6d 6561 6e28 6e70 2e61    = np.mean(np.a
+00012430: 7272 6179 2869 6e63 6f72 7265 6374 5f61  rray(incorrect_a
+00012440: 615f 6929 2c20 6178 6973 3d30 290a 2020  a_i), axis=0).  
+00012450: 2020 2020 2020 666f 7220 692c 2074 3120        for i, t1 
+00012460: 696e 2065 6e75 6d65 7261 7465 286e 6f64  in enumerate(nod
+00012470: 6573 5f69 6e64 6578 6573 293a 0a20 2020  es_indexes):.   
+00012480: 2020 2020 2020 2020 2074 6573 745f 6f62           test_ob
+00012490: 735f 6920 3d20 636f 6e76 6572 745f 746f  s_i = convert_to
+000124a0: 5f6c 6574 7465 7273 2844 6174 6173 6574  _letters(Dataset
+000124b0: 5f74 6573 745f 736c 6963 6564 5b69 5d2c  _test_sliced[i],
+000124c0: 6161 5f70 726f 6273 290a 2020 2020 2020  aa_probs).      
+000124d0: 2020 2020 2020 666f 7220 6a2c 2074 3220        for j, t2 
+000124e0: 696e 2065 6e75 6d65 7261 7465 286e 6f64  in enumerate(nod
+000124f0: 6573 5f69 6e64 6578 6573 5b69 3a5d 293a  es_indexes[i:]):
+00012500: 2020 2320 666f 7220 7465 7374 206e 6f64    # for test nod
+00012510: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00012520: 2020 616c 6c5f 7361 6d70 6c65 645f 7465    all_sampled_te
+00012530: 7374 203d 2070 7265 6469 6374 696f 6e73  st = predictions
+00012540: 5f73 616d 706c 6573 5f73 6c69 6365 645b  _samples_sliced[
+00012550: 3a2c 2069 2b6a 5d20 2023 2041 6c6c 2073  :, i+j]  # All s
+00012560: 616d 706c 6573 2066 6f72 2074 6865 2073  amples for the s
+00012570: 616d 6520 7465 7374 2073 6571 0a20 2020  ame test seq.   
+00012580: 2020 2020 2020 2020 2020 2020 2070 6572               per
+00012590: 6365 6e74 5f69 645f 6920 3d20 5b5d 0a20  cent_id_i = []. 
+000125a0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+000125b0: 6c6f 7375 6d5f 7363 6f72 655f 6920 3d20  losum_score_i = 
+000125c0: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
+000125d0: 2020 2023 696e 636f 7272 6563 745f 6161     #incorrect_aa
+000125e0: 5f69 203d 205b 5d0a 2020 2020 2020 2020  _i = [].        
+000125f0: 2020 2020 2020 2020 666f 7220 7720 696e          for w in
+00012600: 2072 616e 6765 286e 756d 5f73 616d 706c   range(num_sampl
+00012610: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+00012620: 2020 2020 2020 2020 2073 6571 5f73 616d           seq_sam
+00012630: 706c 6564 5f74 6573 7420 3d20 636f 6e76  pled_test = conv
+00012640: 6572 745f 746f 5f6c 6574 7465 7273 2861  ert_to_letters(a
+00012650: 6c6c 5f73 616d 706c 6564 5f74 6573 745b  ll_sampled_test[
+00012660: 775d 2c61 615f 7072 6f62 7329 0a20 2020  w],aa_probs).   
+00012670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012680: 2070 6964 203d 2070 6572 635f 6964 656e   pid = perc_iden
+00012690: 7469 7479 5f70 6169 725f 7365 7128 7465  tity_pair_seq(te
+000126a0: 7374 5f6f 6273 5f69 2c20 7365 715f 7361  st_obs_i, seq_sa
+000126b0: 6d70 6c65 645f 7465 7374 290a 2020 2020  mpled_test).    
+000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126d0: 2377 726f 6e67 5f70 7265 6420 3d20 696e  #wrong_pred = in
+000126e0: 636f 7272 6563 746c 795f 7072 6564 6963  correctly_predic
+000126f0: 7465 645f 6161 2874 6573 745f 6f62 735f  ted_aa(test_obs_
+00012700: 692c 7365 715f 7361 6d70 6c65 645f 7465  i,seq_sampled_te
+00012710: 7374 290a 2020 2020 2020 2020 2020 2020  st).            
+00012720: 2020 2020 2020 2020 626c 6f73 203d 2073          blos = s
+00012730: 636f 7265 5f70 6169 7277 6973 6528 7465  core_pairwise(te
+00012740: 7374 5f6f 6273 5f69 2c20 7365 715f 7361  st_obs_i, seq_sa
+00012750: 6d70 6c65 645f 7465 7374 2c20 626c 6f73  mpled_test, blos
+00012760: 756d 2c20 6761 705f 733d 2d31 312c 2067  um, gap_s=-11, g
+00012770: 6170 5f65 3d2d 3129 0a20 2020 2020 2020  ap_e=-1).       
+00012780: 2020 2020 2020 2020 2020 2020 2070 6572               per
+00012790: 6365 6e74 5f69 645f 692e 6170 7065 6e64  cent_id_i.append
+000127a0: 2870 6964 290a 2020 2020 2020 2020 2020  (pid).          
+000127b0: 2020 2020 2020 2020 2020 626c 6f73 756d            blosum
+000127c0: 5f73 636f 7265 5f69 2e61 7070 656e 6428  _score_i.append(
+000127d0: 626c 6f73 290a 2020 2020 2020 2020 2020  blos).          
+000127e0: 2020 2020 2020 2020 2020 2369 6e63 6f72            #incor
+000127f0: 7265 6374 5f61 615f 692e 6170 7065 6e64  rect_aa_i.append
+00012800: 2877 726f 6e67 5f70 7265 6429 0a20 2020  (wrong_pred).   
+00012810: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+00012820: 7261 6765 2829 0a20 2020 2020 2020 2072  rage().        r
+00012830: 6574 7572 6e20 7065 7263 656e 745f 6964  eturn percent_id
+00012840: 5f53 414d 504c 4544 5f4f 4253 4552 5645  _SAMPLED_OBSERVE
+00012850: 442c 626c 6f73 756d 5f53 414d 504c 4544  D,blosum_SAMPLED
+00012860: 5f4f 4253 4552 5645 442c 696e 636f 7272  _OBSERVED,incorr
+00012870: 6563 745f 5341 4d50 4c45 445f 4f42 5345  ect_SAMPLED_OBSE
+00012880: 5256 4544 0a0a 2020 2020 6465 6620 5065  RVED..    def Pe
+00012890: 7263 656e 745f 4944 5f54 6573 745f 4f42  rcent_ID_Test_OB
+000128a0: 535f 4f42 5345 5256 4544 2829 3a0a 2020  S_OBSERVED():.  
+000128b0: 2020 2020 2020 2247 656e 6572 6174 6520        "Generate 
+000128c0: 7468 6520 4176 6572 6167 6520 616e 6420  the Average and 
+000128d0: 5354 4420 2549 4420 616d 6f6e 6720 6f62  STD %ID among ob
+000128e0: 7320 7465 7374 220a 2020 2020 2020 2020  s test".        
+000128f0: 7065 7263 656e 745f 6964 5f4f 4253 203d  percent_id_OBS =
+00012900: 2064 6566 6175 6c74 6469 6374 286c 616d   defaultdict(lam
+00012910: 6264 613a 2064 6566 6175 6c74 6469 6374  bda: defaultdict
+00012920: 286c 616d 6264 613a 2064 6566 6175 6c74  (lambda: default
+00012930: 6469 6374 2864 6963 7429 2929 0a20 2020  dict(dict))).   
+00012940: 2020 2020 2062 6c6f 7375 6d5f 4f42 5320       blosum_OBS 
+00012950: 3d20 6465 6661 756c 7464 6963 7428 6c61  = defaultdict(la
+00012960: 6d62 6461 3a20 6465 6661 756c 7464 6963  mbda: defaultdic
+00012970: 7428 6c61 6d62 6461 3a20 6465 6661 756c  t(lambda: defaul
+00012980: 7464 6963 7428 6469 6374 2929 290a 0a20  tdict(dict))).. 
+00012990: 2020 2020 2020 2044 6174 6173 6574 5f74         Dataset_t
+000129a0: 6573 745f 736c 6963 6564 203d 2064 6174  est_sliced = dat
+000129b0: 6173 6574 5f74 6573 745b 3a2c 323a 2c30  aset_test[:,2:,0
+000129c0: 5d0a 2020 2020 2020 2020 666f 7220 692c  ].        for i,
+000129d0: 2074 3120 696e 2065 6e75 6d65 7261 7465   t1 in enumerate
+000129e0: 286e 6f64 6573 5f69 6e64 6578 6573 293a  (nodes_indexes):
+000129f0: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
+00012a00: 745f 6f62 735f 6920 3d20 636f 6e76 6572  t_obs_i = conver
+00012a10: 745f 746f 5f6c 6574 7465 7273 2844 6174  t_to_letters(Dat
+00012a20: 6173 6574 5f74 6573 745f 736c 6963 6564  aset_test_sliced
+00012a30: 5b69 5d2c 6161 5f70 726f 6273 290a 2020  [i],aa_probs).  
+00012a40: 2020 2020 2020 2020 2020 2370 6572 6365            #perce
+00012a50: 6e74 5f69 645f 4f42 535b 4461 7461 7365  nt_id_OBS[Datase
+00012a60: 745f 7465 7374 5b69 2c20 302c 2031 5d2e  t_test[i, 0, 1].
+00012a70: 6974 656d 2829 5d5b 4461 7461 7365 745f  item()][Dataset_
+00012a80: 7465 7374 5b69 2c20 302c 2031 5d2e 6974  test[i, 0, 1].it
+00012a90: 656d 2829 5d20 3d20 7065 7263 5f69 6465  em()] = perc_ide
+00012aa0: 6e74 6974 795f 7061 6972 5f73 6571 2874  ntity_pair_seq(t
+00012ab0: 6573 745f 6f62 735f 692c 2074 6573 745f  est_obs_i, test_
+00012ac0: 6f62 735f 6929 0a20 2020 2020 2020 2020  obs_i).         
+00012ad0: 2020 2066 6f72 206a 2c20 7432 2069 6e20     for j, t2 in 
+00012ae0: 656e 756d 6572 6174 6528 6e6f 6465 735f  enumerate(nodes_
+00012af0: 696e 6465 7865 735b 693a 5d29 3a0a 2020  indexes[i:]):.  
+00012b00: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00012b10: 7374 5f6f 6273 5f6a 203d 2063 6f6e 7665  st_obs_j = conve
+00012b20: 7274 5f74 6f5f 6c65 7474 6572 7328 4461  rt_to_letters(Da
+00012b30: 7461 7365 745f 7465 7374 5f73 6c69 6365  taset_test_slice
+00012b40: 645b 692b 6a5d 2c61 615f 7072 6f62 7329  d[i+j],aa_probs)
+00012b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b60: 2070 6964 5f73 636f 7265 203d 2070 6572   pid_score = per
+00012b70: 635f 6964 656e 7469 7479 5f70 6169 725f  c_identity_pair_
+00012b80: 7365 7128 7465 7374 5f6f 6273 5f69 2c74  seq(test_obs_i,t
+00012b90: 6573 745f 6f62 735f 6a29 0a20 2020 2020  est_obs_j).     
+00012ba0: 2020 2020 2020 2020 2020 2070 6572 6365             perce
+00012bb0: 6e74 5f69 645f 4f42 535b 7431 5d5b 7432  nt_id_OBS[t1][t2
+00012bc0: 5d20 3d20 7069 645f 7363 6f72 650a 2020  ] = pid_score.  
+00012bd0: 2020 2020 2020 2020 2020 2020 2020 626c                bl
+00012be0: 6f73 756d 5f73 636f 7265 203d 2073 636f  osum_score = sco
+00012bf0: 7265 5f70 6169 7277 6973 6528 7465 7374  re_pairwise(test
+00012c00: 5f6f 6273 5f69 2c74 6573 745f 6f62 735f  _obs_i,test_obs_
+00012c10: 6a2c 2062 6c6f 7375 6d2c 2067 6170 5f73  j, blosum, gap_s
+00012c20: 3d2d 3131 2c20 6761 705f 653d 2d31 290a  =-11, gap_e=-1).
+00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c40: 626c 6f73 756d 5f4f 4253 5b74 315d 5b74  blosum_OBS[t1][t
+00012c50: 325d 203d 2062 6c6f 7375 6d5f 7363 6f72  2] = blosum_scor
+00012c60: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00012c70: 2070 6572 6365 6e74 5f69 645f 4f42 532c   percent_id_OBS,
+00012c80: 626c 6f73 756d 5f4f 4253 0a0a 2020 2020  blosum_OBS..    
+00012c90: 6465 6620 506c 6f74 5f48 6561 746d 6170  def Plot_Heatmap
+00012ca0: 2864 662c 7469 746c 652c 7469 746c 6532  (df,title,title2
+00012cb0: 2c61 6e6e 6f74 2c6d 6173 6b2c 766d 6178  ,annot,mask,vmax
+00012cc0: 293a 0a20 2020 2020 2020 2066 6967 2c61  ):.        fig,a
+00012cd0: 7820 3d20 2070 6c74 2e73 7562 706c 6f74  x =  plt.subplot
+00012ce0: 7328 312c 2031 2c66 6967 7369 7a65 3d28  s(1, 1,figsize=(
+00012cf0: 3130 2c31 3029 290a 2020 2020 2020 2020  10,10)).        
+00012d00: 686d 6170 203d 2073 6e73 2e68 6561 746d  hmap = sns.heatm
+00012d10: 6170 2864 662c 2063 6d61 703d 2253 7065  ap(df, cmap="Spe
+00012d20: 6374 7261 6c22 2c61 6e6e 6f74 3d61 6e6e  ctral",annot=ann
+00012d30: 6f74 2c61 6e6e 6f74 5f6b 7773 3d7b 2266  ot,annot_kws={"f
+00012d40: 6f6e 7473 697a 6522 3a36 7d2c 6d61 736b  ontsize":6},mask
+00012d50: 3d6d 6173 6b2c 766d 6178 3d76 6d61 7829  =mask,vmax=vmax)
+00012d60: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
+00012d70: 7469 746c 6528 227b 7d20 3b5c 6e22 2e66  title("{} ;\n".f
+00012d80: 6f72 6d61 7428 7469 746c 6529 202b 2072  ormat(title) + r
+00012d90: 227b 7d22 2e66 6f72 6d61 7428 6164 6469  "{}".format(addi
+00012da0: 7469 6f6e 616c 5f6c 6f61 642e 6675 6c6c  tional_load.full
+00012db0: 5f6e 616d 6529 290a 2020 2020 2020 2020  _name)).        
+00012dc0: 6178 2e73 6574 5f78 6c61 6265 6c28 7469  ax.set_xlabel(ti
+00012dd0: 746c 6532 2e73 706c 6974 2822 5f22 295b  tle2.split("_")[
+00012de0: 2d31 5d29 0a20 2020 2020 2020 2061 782e  -1]).        ax.
+00012df0: 7365 745f 796c 6162 656c 2874 6974 6c65  set_ylabel(title
+00012e00: 322e 7370 6c69 7428 225f 2229 5b2d 325d  2.split("_")[-2]
+00012e10: 290a 2020 2020 2020 2020 686d 6170 2e66  ).        hmap.f
+00012e20: 6967 7572 652e 7361 7665 6669 6728 227b  igure.savefig("{
+00012e30: 7d2f 4865 6174 6d61 705f 7b7d 2e70 6e67  }/Heatmap_{}.png
+00012e40: 222e 666f 726d 6174 2872 6573 756c 7473  ".format(results
+00012e50: 5f64 6972 6563 746f 7279 2c74 6974 6c65  _directory,title
+00012e60: 3229 2c0a 2020 2020 2020 2020 2020 2020  2),.            
+00012e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e80: 666f 726d 6174 3d27 706e 6727 2c0a 2020  format='png',.  
 00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ea0: 2020 2020 6470 693d 3135 3029 0a20 2020      dpi=150).   
-00012eb0: 2020 2020 2070 6c74 2e63 6c66 2829 0a20       plt.clf(). 
-00012ec0: 2020 2020 2020 2070 6c74 2e63 6c6f 7365         plt.close
-00012ed0: 2829 0a0a 2020 2020 6d75 6c74 6969 6e64  ()..    multiind
-00012ee0: 6578 3d46 616c 7365 0a20 2020 2069 6620  ex=False.    if 
-00012ef0: 6d75 6c74 6969 6e64 6578 3a0a 2020 2020  multiindex:.    
-00012f00: 2020 2020 2348 6967 686c 6967 6874 3a20      #Highlight: 
-00012f10: 7361 6d70 6c65 6420 7673 206f 6273 6572  sampled vs obser
-00012f20: 7665 640a 2020 2020 2020 2020 6469 6374  ved.        dict
-00012f30: 5f70 6964 5f53 414d 504c 4544 5f4f 4253  _pid_SAMPLED_OBS
-00012f40: 2c20 6469 6374 5f62 6c6f 7375 6d5f 5341  , dict_blosum_SA
-00012f50: 4d50 4c45 445f 4f42 532c 6469 6374 5f69  MPLED_OBS,dict_i
-00012f60: 6e63 6f72 7265 6374 5f53 414d 504c 4544  ncorrect_SAMPLED
-00012f70: 5f4f 4253 203d 2050 6572 6365 6e74 5f49  _OBS = Percent_I
-00012f80: 445f 5465 7374 5f53 414d 504c 4544 5f4f  D_Test_SAMPLED_O
-00012f90: 4253 4552 5645 4428 6d75 6c74 6969 6e64  BSERVED(multiind
-00012fa0: 6578 290a 2020 2020 2020 2020 6466 5f70  ex).        df_p
-00012fb0: 6964 5f53 414d 504c 4544 5f4f 4253 203d  id_SAMPLED_OBS =
-00012fc0: 2070 642e 636f 6e63 6174 287b 6b3a 2070   pd.concat({k: p
-00012fd0: 642e 4461 7461 4672 616d 652e 6672 6f6d  d.DataFrame.from
-00012fe0: 5f64 6963 7428 762c 2027 696e 6465 7827  _dict(v, 'index'
-00012ff0: 2920 666f 7220 6b2c 2076 2069 6e20 6469  ) for k, v in di
-00013000: 6374 5f70 6964 5f53 414d 504c 4544 5f4f  ct_pid_SAMPLED_O
-00013010: 4253 2e69 7465 6d73 2829 7d2c 2061 7869  BS.items()}, axi
-00013020: 733d 3029 0a20 2020 2020 2020 2064 665f  s=0).        df_
-00013030: 626c 6f73 756d 5f53 414d 504c 4544 5f4f  blosum_SAMPLED_O
-00013040: 4253 203d 2070 642e 636f 6e63 6174 287b  BS = pd.concat({
-00013050: 6b3a 2070 642e 4461 7461 4672 616d 652e  k: pd.DataFrame.
-00013060: 6672 6f6d 5f64 6963 7428 762c 2027 696e  from_dict(v, 'in
-00013070: 6465 7827 2920 666f 7220 6b2c 2076 2069  dex') for k, v i
-00013080: 6e20 6469 6374 5f62 6c6f 7375 6d5f 5341  n dict_blosum_SA
-00013090: 4d50 4c45 445f 4f42 532e 6974 656d 7328  MPLED_OBS.items(
-000130a0: 297d 2c61 7869 733d 3029 0a20 2020 2020  )},axis=0).     
-000130b0: 2020 2023 6466 5f69 6e63 6f72 7265 6374     #df_incorrect
-000130c0: 5f53 414d 504c 4544 5f4f 4253 203d 2070  _SAMPLED_OBS = p
-000130d0: 642e 636f 6e63 6174 287b 6b3a 2070 642e  d.concat({k: pd.
-000130e0: 4461 7461 4672 616d 652e 6672 6f6d 5f64  DataFrame.from_d
-000130f0: 6963 7428 762c 2027 696e 6465 7827 2920  ict(v, 'index') 
-00013100: 666f 7220 6b2c 2076 2069 6e20 6469 6374  for k, v in dict
-00013110: 5f69 6e63 6f72 7265 6374 5f53 414d 504c  _incorrect_SAMPL
-00013120: 4544 5f4f 4253 2e69 7465 6d73 2829 7d2c  ED_OBS.items()},
-00013130: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
-00013140: 2023 4869 6768 6c69 6768 743a 2053 616d   #Highlight: Sam
-00013150: 706c 6564 2076 7320 5361 6d70 6c65 640a  pled vs Sampled.
-00013160: 2020 2020 2020 2020 6469 6374 5f70 6964          dict_pid
-00013170: 5f53 414d 504c 4544 5f53 414d 504c 4544  _SAMPLED_SAMPLED
-00013180: 2c64 6963 745f 626c 6f73 756d 5f53 414d  ,dict_blosum_SAM
-00013190: 504c 4544 5f53 414d 504c 4544 3d50 6572  PLED_SAMPLED=Per
-000131a0: 6365 6e74 5f49 445f 5465 7374 5f53 414d  cent_ID_Test_SAM
-000131b0: 504c 4544 5f53 414d 504c 4544 286d 756c  PLED_SAMPLED(mul
-000131c0: 7469 696e 6465 7829 0a20 2020 2020 2020  tiindex).       
-000131d0: 2064 665f 7069 645f 5341 4d50 4c45 445f   df_pid_SAMPLED_
-000131e0: 5341 4d50 4c45 4420 3d20 7064 2e63 6f6e  SAMPLED = pd.con
-000131f0: 6361 7428 7b6b 3a20 7064 2e44 6174 6146  cat({k: pd.DataF
-00013200: 7261 6d65 2e66 726f 6d5f 6469 6374 2876  rame.from_dict(v
-00013210: 2c20 2769 6e64 6578 2729 2066 6f72 206b  , 'index') for k
-00013220: 2c20 7620 696e 2064 6963 745f 7069 645f  , v in dict_pid_
-00013230: 5341 4d50 4c45 445f 5341 4d50 4c45 442e  SAMPLED_SAMPLED.
-00013240: 6974 656d 7328 297d 2c20 6178 6973 3d30  items()}, axis=0
-00013250: 290a 2020 2020 2020 2020 6466 5f62 6c6f  ).        df_blo
-00013260: 7375 6d5f 5341 4d50 4c45 445f 5341 4d50  sum_SAMPLED_SAMP
-00013270: 4c45 4420 3d20 7064 2e63 6f6e 6361 7428  LED = pd.concat(
-00013280: 7b6b 3a20 7064 2e44 6174 6146 7261 6d65  {k: pd.DataFrame
-00013290: 2e66 726f 6d5f 6469 6374 2876 2c20 2769  .from_dict(v, 'i
-000132a0: 6e64 6578 2729 2066 6f72 206b 2c20 7620  ndex') for k, v 
-000132b0: 696e 2064 6963 745f 626c 6f73 756d 5f53  in dict_blosum_S
-000132c0: 414d 504c 4544 5f53 414d 504c 4544 2e69  AMPLED_SAMPLED.i
-000132d0: 7465 6d73 2829 7d2c 2061 7869 733d 3029  tems()}, axis=0)
-000132e0: 0a0a 2020 2020 656c 7365 3a0a 2020 2020  ..    else:.    
-000132f0: 2020 2020 2320 4869 6768 6c69 6768 743a      # Highlight:
-00013300: 2073 616d 706c 6564 2076 7320 6f62 7365   sampled vs obse
-00013310: 7276 6564 0a20 2020 2020 2020 2064 6963  rved.        dic
-00013320: 745f 7069 645f 5341 4d50 4c45 445f 4f42  t_pid_SAMPLED_OB
-00013330: 532c 2064 6963 745f 626c 6f73 756d 5f53  S, dict_blosum_S
-00013340: 414d 504c 4544 5f4f 4253 2c64 6963 745f  AMPLED_OBS,dict_
-00013350: 696e 636f 7272 6563 745f 5341 4d50 4c45  incorrect_SAMPLE
-00013360: 445f 4f42 5320 3d20 5065 7263 656e 745f  D_OBS = Percent_
-00013370: 4944 5f54 6573 745f 5341 4d50 4c45 445f  ID_Test_SAMPLED_
-00013380: 4f42 5345 5256 4544 286d 756c 7469 696e  OBSERVED(multiin
-00013390: 6465 7829 0a20 2020 2020 2020 2064 665f  dex).        df_
-000133a0: 7069 645f 5341 4d50 4c45 445f 4f42 5320  pid_SAMPLED_OBS 
-000133b0: 3d20 7064 2e44 6174 6146 7261 6d65 2864  = pd.DataFrame(d
-000133c0: 6963 745f 7069 645f 5341 4d50 4c45 445f  ict_pid_SAMPLED_
-000133d0: 4f42 5329 0a20 2020 2020 2020 2064 665f  OBS).        df_
-000133e0: 626c 6f73 756d 5f53 414d 504c 4544 5f4f  blosum_SAMPLED_O
-000133f0: 4253 203d 2070 642e 4461 7461 4672 616d  BS = pd.DataFram
-00013400: 6528 6469 6374 5f62 6c6f 7375 6d5f 5341  e(dict_blosum_SA
-00013410: 4d50 4c45 445f 4f42 5329 0a20 2020 2020  MPLED_OBS).     
-00013420: 2020 2023 6466 5f69 6e63 6f72 7265 6374     #df_incorrect
-00013430: 5f53 414d 504c 4544 5f4f 4253 203d 2070  _SAMPLED_OBS = p
-00013440: 642e 4461 7461 4672 616d 6528 6469 6374  d.DataFrame(dict
-00013450: 5f69 6e63 6f72 7265 6374 5f53 414d 504c  _incorrect_SAMPL
-00013460: 4544 5f4f 4253 292e 746f 5f6e 756d 7079  ED_OBS).to_numpy
-00013470: 2829 0a20 2020 2020 2020 2023 4869 6768  ().        #High
-00013480: 6c69 6768 743a 2053 616d 706c 6564 2076  light: Sampled v
-00013490: 7320 5361 6d70 6c65 640a 2020 2020 2020  s Sampled.      
-000134a0: 2020 6469 6374 5f70 6964 5f53 414d 504c    dict_pid_SAMPL
-000134b0: 4544 5f53 414d 504c 4544 2c20 6469 6374  ED_SAMPLED, dict
-000134c0: 5f62 6c6f 7375 6d5f 5341 4d50 4c45 445f  _blosum_SAMPLED_
-000134d0: 5341 4d50 4c45 4420 3d20 5065 7263 656e  SAMPLED = Percen
-000134e0: 745f 4944 5f54 6573 745f 5341 4d50 4c45  t_ID_Test_SAMPLE
-000134f0: 445f 5341 4d50 4c45 4428 6d75 6c74 6969  D_SAMPLED(multii
-00013500: 6e64 6578 290a 2020 2020 2020 2020 6466  ndex).        df
-00013510: 5f70 6964 5f53 414d 504c 4544 5f53 414d  _pid_SAMPLED_SAM
-00013520: 504c 4544 203d 2070 642e 4461 7461 4672  PLED = pd.DataFr
-00013530: 616d 6528 6469 6374 5f70 6964 5f53 414d  ame(dict_pid_SAM
-00013540: 504c 4544 5f53 414d 504c 4544 290a 2020  PLED_SAMPLED).  
-00013550: 2020 2020 2020 6466 5f62 6c6f 7375 6d5f        df_blosum_
-00013560: 5341 4d50 4c45 445f 5341 4d50 4c45 4420  SAMPLED_SAMPLED 
-00013570: 3d20 7064 2e44 6174 6146 7261 6d65 2864  = pd.DataFrame(d
-00013580: 6963 745f 626c 6f73 756d 5f53 414d 504c  ict_blosum_SAMPL
-00013590: 4544 5f53 414d 504c 4544 290a 0a0a 2020  ED_SAMPLED)...  
-000135a0: 2020 6469 6374 5f70 6964 5f4f 4253 5f4f    dict_pid_OBS_O
-000135b0: 4253 2c64 6963 745f 626c 6f73 756d 5f4f  BS,dict_blosum_O
-000135c0: 4253 5f4f 4253 203d 2050 6572 6365 6e74  BS_OBS = Percent
-000135d0: 5f49 445f 5465 7374 5f4f 4253 5f4f 4253  _ID_Test_OBS_OBS
-000135e0: 4552 5645 4428 290a 2020 2020 6466 5f70  ERVED().    df_p
-000135f0: 6964 5f4f 4253 5f4f 4253 203d 2070 642e  id_OBS_OBS = pd.
-00013600: 4461 7461 4672 616d 6528 6469 6374 5f70  DataFrame(dict_p
-00013610: 6964 5f4f 4253 5f4f 4253 290a 2020 2020  id_OBS_OBS).    
-00013620: 6466 5f62 6c6f 7375 6d5f 4f42 535f 4f42  df_blosum_OBS_OB
-00013630: 5320 3d20 7064 2e44 6174 6146 7261 6d65  S = pd.DataFrame
-00013640: 2864 6963 745f 626c 6f73 756d 5f4f 4253  (dict_blosum_OBS
-00013650: 5f4f 4253 290a 0a20 2020 2023 6466 5f6c  _OBS)..    #df_l
-00013660: 7420 3d20 6466 5f4f 4253 5f4f 4253 2e77  t = df_OBS_OBS.w
-00013670: 6865 7265 286e 702e 7472 696c 286e 702e  here(np.tril(np.
-00013680: 6f6e 6573 2864 665f 4f42 535f 4f42 532e  ones(df_OBS_OBS.
-00013690: 7368 6170 6529 292e 6173 7479 7065 286e  shape)).astype(n
-000136a0: 702e 626f 6f6c 2929 0a20 2020 2061 6e6e  p.bool)).    ann
-000136b0: 6f74 203d 2046 616c 7365 0a20 2020 2050  ot = False.    P
-000136c0: 6c6f 745f 4865 6174 6d61 7028 6466 5f70  lot_Heatmap(df_p
-000136d0: 6964 5f4f 4253 5f4f 4253 2c22 4f42 5320  id_OBS_OBS,"OBS 
-000136e0: 7365 7173 2076 7320 4f42 5320 7365 7173  seqs vs OBS seqs
-000136f0: 2025 4944 222c 2250 4944 5f7b 7d5f 4f42   %ID","PID_{}_OB
-00013700: 535f 4f42 5322 2e66 6f72 6d61 7428 666f  S_OBS".format(fo
-00013710: 6c64 6572 292c 616e 6e6f 743d 616e 6e6f  lder),annot=anno
-00013720: 742c 6d61 736b 3d4e 6f6e 652c 766d 6178  t,mask=None,vmax
-00013730: 3d31 3030 290a 2020 2020 506c 6f74 5f48  =100).    Plot_H
-00013740: 6561 746d 6170 2864 665f 7069 645f 5341  eatmap(df_pid_SA
-00013750: 4d50 4c45 445f 4f42 532c 2022 4f42 5320  MPLED_OBS, "OBS 
-00013760: 7673 2053 414d 504c 4544 2073 6571 7320  vs SAMPLED seqs 
-00013770: 4156 4552 4147 4520 2549 4422 2c20 2250  AVERAGE %ID", "P
-00013780: 4944 5f7b 7d5f 4f42 535f 5341 4d50 4c45  ID_{}_OBS_SAMPLE
-00013790: 4422 2e66 6f72 6d61 7428 666f 6c64 6572  D".format(folder
-000137a0: 292c 616e 6e6f 743d 616e 6e6f 742c 6d61  ),annot=annot,ma
-000137b0: 736b 3d4e 6f6e 652c 766d 6178 3d31 3030  sk=None,vmax=100
-000137c0: 290a 2020 2020 506c 6f74 5f48 6561 746d  ).    Plot_Heatm
-000137d0: 6170 2864 665f 7069 645f 5341 4d50 4c45  ap(df_pid_SAMPLE
-000137e0: 445f 5341 4d50 4c45 442c 2022 5341 4d50  D_SAMPLED, "SAMP
-000137f0: 4c45 4420 7673 2053 414d 504c 4544 2073  LED vs SAMPLED s
-00013800: 6571 7320 4156 4552 4147 4520 2549 4422  eqs AVERAGE %ID"
-00013810: 2c20 2250 4944 5f7b 7d5f 5341 4d50 4c45  , "PID_{}_SAMPLE
-00013820: 445f 5341 4d50 4c45 4422 2e66 6f72 6d61  D_SAMPLED".forma
-00013830: 7428 666f 6c64 6572 292c 616e 6e6f 743d  t(folder),annot=
-00013840: 616e 6e6f 742c 6d61 736b 3d4e 6f6e 652c  annot,mask=None,
-00013850: 766d 6178 3d31 3030 290a 0a20 2020 2076  vmax=100)..    v
-00013860: 6d61 7820 3d20 6d61 7828 5b64 665f 626c  max = max([df_bl
-00013870: 6f73 756d 5f4f 4253 5f4f 4253 2e6d 6178  osum_OBS_OBS.max
-00013880: 2829 2e6d 6178 2829 2c64 665f 626c 6f73  ().max(),df_blos
-00013890: 756d 5f53 414d 504c 4544 5f53 414d 504c  um_SAMPLED_SAMPL
-000138a0: 4544 2e6d 6178 2829 2e6d 6178 2829 2c64  ED.max().max(),d
-000138b0: 665f 626c 6f73 756d 5f53 414d 504c 4544  f_blosum_SAMPLED
-000138c0: 5f4f 4253 2e6d 6178 2829 2e6d 6178 2829  _OBS.max().max()
-000138d0: 5d29 0a20 2020 2050 6c6f 745f 4865 6174  ]).    Plot_Heat
-000138e0: 6d61 7028 6466 5f62 6c6f 7375 6d5f 4f42  map(df_blosum_OB
-000138f0: 535f 4f42 532c 2022 4f42 5320 7365 7173  S_OBS, "OBS seqs
-00013900: 2076 7320 4f42 5320 7365 7173 2042 6c6f   vs OBS seqs Blo
-00013910: 7375 6d20 5363 6f72 6522 2c20 2242 6c6f  sum Score", "Blo
-00013920: 7375 6d5f 7b7d 5f4f 4253 5f4f 4253 222e  sum_{}_OBS_OBS".
-00013930: 666f 726d 6174 2866 6f6c 6465 7229 2c61  format(folder),a
-00013940: 6e6e 6f74 3d61 6e6e 6f74 2c6d 6173 6b3d  nnot=annot,mask=
-00013950: 4e6f 6e65 2c76 6d61 783d 766d 6178 290a  None,vmax=vmax).
-00013960: 2020 2020 506c 6f74 5f48 6561 746d 6170      Plot_Heatmap
-00013970: 2864 665f 626c 6f73 756d 5f53 414d 504c  (df_blosum_SAMPL
-00013980: 4544 5f4f 4253 2c20 224f 4253 2076 7320  ED_OBS, "OBS vs 
-00013990: 5341 4d50 4c45 4420 7365 7173 2041 5645  SAMPLED seqs AVE
-000139a0: 5241 4745 2042 6c6f 7375 6d20 5363 6f72  RAGE Blosum Scor
-000139b0: 6522 2c20 2242 6c6f 7375 6d5f 7b7d 5f4f  e", "Blosum_{}_O
-000139c0: 4253 5f53 414d 504c 4544 222e 666f 726d  BS_SAMPLED".form
-000139d0: 6174 2866 6f6c 6465 7229 2c61 6e6e 6f74  at(folder),annot
-000139e0: 3d61 6e6e 6f74 2c6d 6173 6b3d 4e6f 6e65  =annot,mask=None
-000139f0: 2c76 6d61 783d 766d 6178 290a 2020 2020  ,vmax=vmax).    
-00013a00: 506c 6f74 5f48 6561 746d 6170 2864 665f  Plot_Heatmap(df_
-00013a10: 626c 6f73 756d 5f53 414d 504c 4544 5f53  blosum_SAMPLED_S
-00013a20: 414d 504c 4544 2c20 2253 414d 504c 4544  AMPLED, "SAMPLED
-00013a30: 2076 7320 5341 4d50 4c45 4420 7365 7173   vs SAMPLED seqs
-00013a40: 2041 5645 5241 4745 2042 6c6f 7375 6d20   AVERAGE Blosum 
-00013a50: 5363 6f72 6522 2c20 2242 6c6f 7375 6d5f  Score", "Blosum_
-00013a60: 7b7d 5f53 414d 504c 4544 5f53 414d 504c  {}_SAMPLED_SAMPL
-00013a70: 4544 222e 666f 726d 6174 2866 6f6c 6465  ED".format(folde
-00013a80: 7229 2c61 6e6e 6f74 3d61 6e6e 6f74 2c6d  r),annot=annot,m
-00013a90: 6173 6b3d 4e6f 6e65 2c76 6d61 7820 3d20  ask=None,vmax = 
-00013aa0: 766d 6178 290a 6465 6620 6275 696c 645f  vmax).def build_
-00013ab0: 6461 7461 6672 616d 6573 5f6f 7665 726c  dataframes_overl
-00013ac0: 6170 7069 6e67 5f68 6973 746f 6772 616d  apping_histogram
-00013ad0: 7328 6161 5f73 6571 7565 6e63 6573 5f70  s(aa_sequences_p
-00013ae0: 7265 6469 6374 696f 6e73 2c20 6461 7461  redictions, data
-00013af0: 7365 745f 7472 6169 6e2c 6461 7461 7365  set_train,datase
-00013b00: 745f 7465 7374 2c20 6e61 6d65 2c20 6e5f  t_test, name, n_
-00013b10: 7361 6d70 6c65 732c 6e6f 6465 735f 696e  samples,nodes_in
-00013b20: 6465 7865 732c 7265 7375 6c74 735f 6469  dexes,results_di
-00013b30: 7265 6374 6f72 792c 6161 5f70 726f 6273  rectory,aa_probs
-00013b40: 2c63 6f72 7265 7370 6f6e 6465 6e63 655f  ,correspondence_
-00013b50: 6469 6374 3d4e 6f6e 6529 3a0a 2020 2020  dict=None):.    
-00013b60: 2222 2250 6c6f 7420 6869 7374 6f67 7261  """Plot histogra
-00013b70: 6d20 7768 6f73 6520 6261 7273 2072 6570  m whose bars rep
-00013b80: 7265 7365 6e74 2074 6865 2070 6572 6365  resent the perce
-00013b90: 6e74 6167 6520 6964 656e 7469 7479 2062  ntage identity b
-00013ba0: 6574 7765 656e 2074 6865 2074 7275 6520  etween the true 
-00013bb0: 616e 6365 7374 6f72 7320 7673 2074 7275  ancestors vs tru
-00013bc0: 6520 6c65 6176 6573 2061 6e64 2074 6865  e leaves and the
-00013bd0: 2070 7265 6469 6374 6564 2061 6e63 6573   predicted ances
-00013be0: 746f 7273 2076 7320 7472 7565 206c 6561  tors vs true lea
-00013bf0: 7665 730a 2020 2020 3a70 6172 616d 2074  ves.    :param t
-00013c00: 656e 736f 7220 6161 5f73 6571 7565 6e63  ensor aa_sequenc
-00013c10: 6573 5f70 7265 6469 6374 696f 6e73 3a0a  es_predictions:.
-00013c20: 2020 2020 3a70 6172 616d 2074 656e 736f      :param tenso
-00013c30: 7220 6461 7461 7365 745f 7472 6169 6e0a  r dataset_train.
-00013c40: 2020 2020 3a70 6172 616d 2074 656e 736f      :param tenso
-00013c50: 7220 6461 7461 7365 745f 7465 7374 0a20  r dataset_test. 
-00013c60: 2020 203a 7061 7261 6d20 7374 7220 6e61     :param str na
-00013c70: 6d65 3a20 6461 7461 7365 7420 6e61 6d65  me: dataset name
-00013c80: 2070 726f 6a65 6374 0a20 2020 203a 7061   project.    :pa
-00013c90: 7261 6d20 7465 6e73 6f72 2061 615f 7365  ram tensor aa_se
-00013ca0: 7175 656e 6365 735f 7072 6564 6963 7469  quences_predicti
-00013cb0: 6f6e 730a 2020 2020 3a70 6172 616d 2069  ons.    :param i
-00013cc0: 6e74 206e 5f73 616d 706c 6573 3a20 6e75  nt n_samples: nu
-00013cd0: 6d62 6572 206f 6620 7361 6d70 6c65 6420  mber of sampled 
-00013ce0: 7072 6564 6963 7469 6f6e 730a 2020 2020  predictions.    
-00013cf0: 3a70 6172 616d 206e 6f64 6573 5f69 6e64  :param nodes_ind
-00013d00: 6578 6573 3a0a 2020 2020 3a70 6172 616d  exes:.    :param
-00013d10: 2073 7472 2072 6573 756c 7473 5f64 6972   str results_dir
-00013d20: 6563 746f 7279 0a20 2020 203a 7061 7261  ectory.    :para
-00013d30: 6d20 696e 7420 6161 5f70 726f 623a 2061  m int aa_prob: a
-00013d40: 6d69 6e6f 2061 6369 6420 7072 6f62 6162  mino acid probab
-00013d50: 696c 6974 6965 7320 2869 2e65 2032 3129  ilities (i.e 21)
-00013d60: 0a20 2020 203a 7061 7261 6d20 6469 6374  .    :param dict
-00013d70: 2063 6f72 7265 7370 6f6e 6465 6e63 655f   correspondence_
-00013d80: 6469 6374 3a20 636f 7272 6573 706f 6e64  dict: correspond
-00013d90: 656e 6365 2062 6574 7765 656e 2074 6865  ence between the
-00013da0: 2074 7265 6520 6c65 7665 6c20 6f72 6465   tree level orde
-00013db0: 7220 696e 6465 7865 7320 616e 6420 7468  r indexes and th
-00013dc0: 6520 2d2d 3e20 6f6e 6c79 2075 7365 6675  e --> only usefu
-00013dd0: 6c20 666f 7220 6265 6e63 686d 6172 6b5f  l for benchmark_
-00013de0: 7261 6e64 616c 6c5f 6f72 6967 696e 616c  randall_original
-00013df0: 5f6e 616d 696e 670a 2020 2020 2222 220a  _naming.    """.
-00013e00: 2020 2020 2268 7474 7073 3a2f 2f6d 6174      "https://mat
-00013e10: 706c 6f74 6c69 622e 6f72 672f 332e 312e  plotlib.org/3.1.
-00013e20: 312f 6761 6c6c 6572 792f 756e 6974 732f  1/gallery/units/
-00013e30: 6261 725f 756e 6974 5f64 656d 6f2e 6874  bar_unit_demo.ht
-00013e40: 6d6c 2373 7068 782d 676c 722d 6761 6c6c  ml#sphx-glr-gall
-00013e50: 6572 792d 756e 6974 732d 6261 722d 756e  ery-units-bar-un
-00013e60: 6974 2d64 656d 6f2d 7079 220a 2020 2020  it-demo-py".    
-00013e70: 7072 696e 7428 2242 7569 6c64 696e 6720  print("Building 
-00013e80: 4f76 6572 6c61 7070 696e 6720 4869 7374  Overlapping Hist
-00013e90: 6f67 7261 6d2e 2e2e 2229 0a20 2020 206e  ogram...").    n
-00013ea0: 5f63 6869 6c64 7265 6e20 3d20 6c65 6e28  _children = len(
-00013eb0: 6e6f 6465 735f 696e 6465 7865 7329 0a20  nodes_indexes). 
-00013ec0: 2020 2064 6566 2050 6572 6365 6e74 5f49     def Percent_I
-00013ed0: 445f 4f42 535f 4f42 5328 293a 0a20 2020  D_OBS_OBS():.   
-00013ee0: 2020 2020 2022 4765 6e65 7261 7465 2074       "Generate t
-00013ef0: 6865 2020 2549 4420 6f66 2074 6865 204f  he  %ID of the O
-00013f00: 4253 2054 4553 5420 7365 7175 656e 6365  BS TEST sequence
-00013f10: 7320 6167 6169 6e73 7420 7468 6520 4f42  s against the OB
-00013f20: 5320 7472 6169 6e22 0a20 2020 2020 2020  S train".       
-00013f30: 2070 6572 6365 6e74 5f69 645f 4f42 5320   percent_id_OBS 
-00013f40: 3d20 6469 6374 2e66 726f 6d6b 6579 7328  = dict.fromkeys(
-00013f50: 6461 7461 7365 745f 7472 6169 6e5b 3a2c  dataset_train[:,
-00013f60: 302c 315d 2e74 6f6c 6973 7428 292c 2064  0,1].tolist(), d
-00013f70: 6963 742e 6672 6f6d 6b65 7973 2864 6174  ict.fromkeys(dat
-00013f80: 6173 6574 5f74 6573 745b 3a2c 302c 315d  aset_test[:,0,1]
-00013f90: 2e74 6f6c 6973 7428 292c 5b5d 2929 0a20  .tolist(),[])). 
-00013fa0: 2020 2020 2020 2066 6f72 2069 2c74 7261         for i,tra
-00013fb0: 696e 7365 7120 696e 2065 6e75 6d65 7261  inseq in enumera
-00013fc0: 7465 2864 6174 6173 6574 5f74 7261 696e  te(dataset_train
-00013fd0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00013fe0: 6571 5f54 5241 494e 5f6f 6273 5f6c 6574  eq_TRAIN_obs_let
-00013ff0: 7465 7273 5f69 203d 2063 6f6e 7665 7274  ters_i = convert
-00014000: 5f74 6f5f 6c65 7474 6572 7328 6461 7461  _to_letters(data
-00014010: 7365 745f 7472 6169 6e5b 692c 2032 3a2c  set_train[i, 2:,
-00014020: 305d 2c61 615f 7072 6f62 7329 0a20 2020  0],aa_probs).   
-00014030: 2020 2020 2020 2020 2066 6f72 206a 2c74           for j,t
-00014040: 6573 7473 6571 2069 6e20 656e 756d 6572  estseq in enumer
-00014050: 6174 6528 6461 7461 7365 745f 7465 7374  ate(dataset_test
-00014060: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014070: 2020 2073 6571 5f54 4553 545f 6f62 735f     seq_TEST_obs_
-00014080: 6c65 7474 6572 735f 6920 3d20 636f 6e76  letters_i = conv
-00014090: 6572 745f 746f 5f6c 6574 7465 7273 2864  ert_to_letters(d
-000140a0: 6174 6173 6574 5f74 6573 745b 6a2c 2032  ataset_test[j, 2
-000140b0: 3a2c 305d 2c61 615f 7072 6f62 7329 0a20  :,0],aa_probs). 
-000140c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000140d0: 6964 203d 7065 7263 5f69 6465 6e74 6974  id =perc_identit
-000140e0: 795f 7061 6972 5f73 6571 2873 6571 5f54  y_pair_seq(seq_T
-000140f0: 5241 494e 5f6f 6273 5f6c 6574 7465 7273  RAIN_obs_letters
-00014100: 5f69 2c73 6571 5f54 4553 545f 6f62 735f  _i,seq_TEST_obs_
-00014110: 6c65 7474 6572 735f 6929 0a20 2020 2020  letters_i).     
-00014120: 2020 2020 2020 2020 2020 2070 6572 6365             perce
-00014130: 6e74 5f69 645f 4f42 535b 6461 7461 7365  nt_id_OBS[datase
-00014140: 745f 7472 6169 6e5b 692c 302c 315d 2e69  t_train[i,0,1].i
-00014150: 7465 6d28 295d 5b64 6174 6173 6574 5f74  tem()][dataset_t
-00014160: 6573 745b 6a2c 302c 315d 2e69 7465 6d28  est[j,0,1].item(
-00014170: 295d 203d 2070 6964 0a20 2020 2020 2020  )] = pid.       
-00014180: 2072 6574 7572 6e20 7065 7263 656e 745f   return percent_
-00014190: 6964 5f4f 4253 0a20 2020 2064 6566 2050  id_OBS.    def P
-000141a0: 6572 6365 6e74 5f49 445f 5052 4544 5f4f  ercent_ID_PRED_O
-000141b0: 4253 2829 3a0a 2020 2020 2020 2020 2247  BS():.        "G
-000141c0: 656e 6572 6174 6520 7468 6520 4176 6572  enerate the Aver
-000141d0: 6167 6520 616e 6420 5354 4420 2549 4420  age and STD %ID 
-000141e0: 6f66 2074 6865 2073 616d 706c 6564 2073  of the sampled s
-000141f0: 6571 7565 6e63 6573 2061 6761 696e 7374  equences against
-00014200: 2074 6865 204f 4253 2074 7261 696e 220a   the OBS train".
-00014210: 2020 2020 2020 2020 2370 6572 6365 6e74          #percent
-00014220: 5f69 645f 5052 4544 203d 2064 6963 742e  _id_PRED = dict.
-00014230: 6672 6f6d 6b65 7973 2844 6174 6173 6574  fromkeys(Dataset
-00014240: 5f74 7261 696e 5b3a 2c30 2c31 5d2e 746f  _train[:,0,1].to
-00014250: 6c69 7374 2829 2c20 6469 6374 2e66 726f  list(), dict.fro
-00014260: 6d6b 6579 7328 7072 6564 6963 7469 6f6e  mkeys(prediction
-00014270: 735f 7361 6d70 6c65 735b 302c 3a2c 315d  s_samples[0,:,1]
-00014280: 2e74 6f6c 6973 7428 292c 7b22 4176 6572  .tolist(),{"Aver
-00014290: 6167 6522 3a5b 5d2c 2253 7464 223a 5b5d  age":[],"Std":[]
-000142a0: 7d29 2920 237b 2241 7665 7261 6765 223a  })) #{"Average":
-000142b0: 5b5d 2c22 5374 6422 3a5b 5d7d 0a20 2020  [],"Std":[]}.   
-000142c0: 2020 2020 2070 6572 6365 6e74 5f69 645f       percent_id_
-000142d0: 5052 4544 203d 2064 6566 6175 6c74 6469  PRED = defaultdi
-000142e0: 6374 286c 616d 6264 613a 2064 6566 6175  ct(lambda: defau
-000142f0: 6c74 6469 6374 286c 616d 6264 613a 2064  ltdict(lambda: d
-00014300: 6566 6175 6c74 6469 6374 2864 6963 7429  efaultdict(dict)
-00014310: 2929 0a20 2020 2020 2020 2066 6f72 2069  )).        for i
-00014320: 2c20 7365 7120 696e 2065 6e75 6d65 7261  , seq in enumera
-00014330: 7465 2864 6174 6173 6574 5f74 7261 696e  te(dataset_train
-00014340: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00014350: 6571 5f54 5241 494e 5f6f 6273 5f6c 6574  eq_TRAIN_obs_let
-00014360: 7465 7273 5f69 203d 2063 6f6e 7665 7274  ters_i = convert
-00014370: 5f74 6f5f 6c65 7474 6572 7328 6461 7461  _to_letters(data
-00014380: 7365 745f 7472 6169 6e5b 692c 2032 3a2c  set_train[i, 2:,
-00014390: 305d 2c61 615f 7072 6f62 7329 0a20 2020  0],aa_probs).   
-000143a0: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-000143b0: 6e20 7261 6e67 6528 6e5f 6368 696c 6472  n range(n_childr
-000143c0: 656e 293a 2366 6f72 2074 6573 7420 6e6f  en):#for test no
-000143d0: 6465 2023 6e5f 6368 696c 6472 656e 0a20  de #n_children. 
-000143e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000143f0: 6c6c 5f73 616d 706c 6564 5f69 6e64 6578  ll_sampled_index
-00014400: 203d 2061 615f 7365 7175 656e 6365 735f   = aa_sequences_
-00014410: 7072 6564 6963 7469 6f6e 735b 3a2c 6a2c  predictions[:,j,
-00014420: 333a 5d20 2023 2041 6c6c 2073 616d 706c  3:]  # All sampl
-00014430: 6573 2066 6f72 2073 616d 6520 7465 7374  es for same test
-00014440: 2073 6571 0a20 2020 2020 2020 2020 2020   seq.           
-00014450: 2020 2020 2070 6572 6365 6e74 5f69 645f       percent_id_
-00014460: 693d 5b5d 2023 616c 6c20 7361 6d70 6c65  i=[] #all sample
-00014470: 7320 666f 7220 7468 6520 7361 6d65 2074  s for the same t
-00014480: 6573 7420 7365 7175 656e 6365 0a20 2020  est sequence.   
-00014490: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000144a0: 2077 2069 6e20 7261 6e67 6528 6e5f 7361   w in range(n_sa
-000144b0: 6d70 6c65 7329 3a0a 2020 2020 2020 2020  mples):.        
-000144c0: 2020 2020 2020 2020 2020 2020 7365 715f              seq_
-000144d0: 7361 6d70 6c65 645f 7465 7374 203d 2063  sampled_test = c
-000144e0: 6f6e 7665 7274 5f74 6f5f 6c65 7474 6572  onvert_to_letter
-000144f0: 7328 616c 6c5f 7361 6d70 6c65 645f 696e  s(all_sampled_in
-00014500: 6465 785b 775d 2c61 615f 7072 6f62 7329  dex[w],aa_probs)
-00014510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014520: 2020 2020 2070 6964 203d 2070 6572 635f       pid = perc_
-00014530: 6964 656e 7469 7479 5f70 6169 725f 7365  identity_pair_se
-00014540: 7128 7365 715f 5452 4149 4e5f 6f62 735f  q(seq_TRAIN_obs_
-00014550: 6c65 7474 6572 735f 692c 2073 6571 5f73  letters_i, seq_s
-00014560: 616d 706c 6564 5f74 6573 7429 0a20 2020  ampled_test).   
-00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014580: 2070 6572 6365 6e74 5f69 645f 692e 6170   percent_id_i.ap
-00014590: 7065 6e64 2870 6964 290a 2020 2020 2020  pend(pid).      
-000145a0: 2020 2020 2020 2020 2020 7065 7263 656e            percen
-000145b0: 745f 6964 5f50 5245 445b 6461 7461 7365  t_id_PRED[datase
-000145c0: 745f 7472 6169 6e5b 692c 302c 315d 2e69  t_train[i,0,1].i
-000145d0: 7465 6d28 295d 5b61 615f 7365 7175 656e  tem()][aa_sequen
-000145e0: 6365 735f 7072 6564 6963 7469 6f6e 735b  ces_predictions[
-000145f0: 302c 6a2c 315d 5d5b 2241 7665 7261 6765  0,j,1]]["Average
-00014600: 225d 203d 206e 702e 6d65 616e 286e 702e  "] = np.mean(np.
-00014610: 6172 7261 7928 7065 7263 656e 745f 6964  array(percent_id
-00014620: 5f69 292c 6178 6973 3d30 290a 2020 2020  _i),axis=0).    
-00014630: 2020 2020 2020 2020 2020 2020 7065 7263              perc
-00014640: 656e 745f 6964 5f50 5245 445b 6461 7461  ent_id_PRED[data
-00014650: 7365 745f 7472 6169 6e5b 692c 302c 315d  set_train[i,0,1]
-00014660: 2e69 7465 6d28 295d 5b61 615f 7365 7175  .item()][aa_sequ
-00014670: 656e 6365 735f 7072 6564 6963 7469 6f6e  ences_prediction
-00014680: 735b 302c 6a2c 315d 5d5b 2253 7464 225d  s[0,j,1]]["Std"]
-00014690: 203d 206e 702e 7374 6428 6e70 2e61 7272   = np.std(np.arr
-000146a0: 6179 2870 6572 6365 6e74 5f69 645f 6929  ay(percent_id_i)
-000146b0: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
-000146c0: 2020 7265 7475 726e 2070 6572 6365 6e74    return percent
-000146d0: 5f69 645f 5052 4544 0a0a 0a20 2020 2070  _id_PRED...    p
-000146e0: 6572 6365 6e74 5f69 645f 5052 4544 203d  ercent_id_PRED =
-000146f0: 2050 6572 6365 6e74 5f49 445f 5052 4544   Percent_ID_PRED
-00014700: 5f4f 4253 2829 0a20 2020 2070 6572 6365  _OBS().    perce
-00014710: 6e74 5f69 645f 4f42 5320 3d20 5065 7263  nt_id_OBS = Perc
-00014720: 656e 745f 4944 5f4f 4253 5f4f 4253 2829  ent_ID_OBS_OBS()
-00014730: 0a0a 2020 2020 6669 6720 3d20 706c 742e  ..    fig = plt.
-00014740: 6669 6775 7265 2866 6967 7369 7a65 3d28  figure(figsize=(
-00014750: 3138 2c20 3529 290a 2020 2020 6178 203d  18, 5)).    ax =
-00014760: 2066 6967 2e61 6464 5f73 7562 706c 6f74   fig.add_subplot
-00014770: 2831 3131 290a 0a20 2020 2023 2320 496e  (111)..    ## In
-00014780: 6465 7865 7320 7768 6572 6520 7468 6520  dexes where the 
-00014790: 6261 7273 2077 696c 6c20 676f 0a20 2020  bars will go.   
-000147a0: 2069 6e64 5f6c 696e 6573 203d 206e 702e   ind_lines = np.
-000147b0: 6172 616e 6765 2831 302c 6c65 6e28 6461  arange(10,len(da
-000147c0: 7461 7365 745f 7472 6169 6e29 2a31 302c  taset_train)*10,
-000147d0: 3130 2029 0a20 2020 2069 6e64 5f74 7261  10 ).    ind_tra
-000147e0: 696e 203d 206e 702e 6172 616e 6765 2835  in = np.arange(5
-000147f0: 2c6c 656e 2864 6174 6173 6574 5f74 7261  ,len(dataset_tra
-00014800: 696e 292a 3130 2c31 3020 2920 2023 2074  in)*10,10 )  # t
-00014810: 6865 2078 206c 6f63 6174 696f 6e73 2066  he x locations f
-00014820: 6f72 2074 6865 2074 7261 696e 206e 6f64  or the train nod
-00014830: 6573 0a20 2020 2077 6964 7468 203d 2031  es.    width = 1
-00014840: 302f 6c65 6e28 6461 7461 7365 745f 7465  0/len(dataset_te
-00014850: 7374 2920 2d30 2e33 2023 2074 6865 2077  st) -0.3 # the w
-00014860: 6964 7468 206f 6620 7468 6520 6261 7273  idth of the bars
-00014870: 0a20 2020 2069 6e64 5f74 6573 7420 3d20  .    ind_test = 
-00014880: 6e70 2e61 7261 6e67 6528 302c 3130 2c77  np.arange(0,10,w
-00014890: 6964 7468 202b 2030 2e33 2920 2023 2074  idth + 0.3)  # t
-000148a0: 6865 2078 206c 6f63 6174 696f 6e73 2066  he x locations f
-000148b0: 6f72 2074 6865 2074 6573 7420 6e6f 6465  or the test node
-000148c0: 732c 2074 616b 696e 6720 696e 746f 2061  s, taking into a
-000148d0: 6363 6f75 6e74 2074 6865 2073 7061 6365  ccount the space
-000148e0: 2062 6574 7765 656e 2074 6865 6d3f 0a20   between them?. 
-000148f0: 2020 2073 7461 7274 203d 2030 0a20 2020     start = 0.   
-00014900: 2062 6c75 652c 203d 2073 6e73 2e63 6f6c   blue, = sns.col
-00014910: 6f72 5f70 616c 6574 7465 2822 6d75 7465  or_palette("mute
-00014920: 6422 2c20 3129 0a20 2020 2066 6f72 2074  d", 1).    for t
-00014930: 7261 696e 5f6e 6f64 6520 696e 2064 6174  rain_node in dat
-00014940: 6173 6574 5f74 7261 696e 5b3a 2c30 2c31  aset_train[:,0,1
-00014950: 5d3a 0a20 2020 2020 2020 2066 6f72 2069  ]:.        for i
-00014960: 6478 2c74 6573 745f 6e6f 6465 2069 6e20  dx,test_node in 
-00014970: 656e 756d 6572 6174 6528 6461 7461 7365  enumerate(datase
-00014980: 745f 7465 7374 5b3a 2c30 2c31 5d29 3a20  t_test[:,0,1]): 
-00014990: 2354 4f44 4f3a 206f 7574 206f 6620 7261  #TODO: out of ra
-000149a0: 6e67 650a 2020 2020 2020 2020 2020 2020  nge.            
-000149b0: 7265 6374 7332 203d 2061 782e 6261 7228  rects2 = ax.bar(
-000149c0: 696e 645f 7465 7374 5b69 6478 5d20 2b20  ind_test[idx] + 
-000149d0: 7374 6172 7420 2c0a 2020 2020 2020 2020  start ,.        
+00012ea0: 2020 2020 2020 2020 2020 6470 693d 3135            dpi=15
+00012eb0: 3029 0a20 2020 2020 2020 2070 6c74 2e63  0).        plt.c
+00012ec0: 6c66 2829 0a20 2020 2020 2020 2070 6c74  lf().        plt
+00012ed0: 2e63 6c6f 7365 2829 0a0a 2020 2020 6d75  .close()..    mu
+00012ee0: 6c74 6969 6e64 6578 3d46 616c 7365 0a20  ltiindex=False. 
+00012ef0: 2020 2069 6620 6d75 6c74 6969 6e64 6578     if multiindex
+00012f00: 3a0a 2020 2020 2020 2020 2348 6967 686c  :.        #Highl
+00012f10: 6967 6874 3a20 7361 6d70 6c65 6420 7673  ight: sampled vs
+00012f20: 206f 6273 6572 7665 640a 2020 2020 2020   observed.      
+00012f30: 2020 6469 6374 5f70 6964 5f53 414d 504c    dict_pid_SAMPL
+00012f40: 4544 5f4f 4253 2c20 6469 6374 5f62 6c6f  ED_OBS, dict_blo
+00012f50: 7375 6d5f 5341 4d50 4c45 445f 4f42 532c  sum_SAMPLED_OBS,
+00012f60: 6469 6374 5f69 6e63 6f72 7265 6374 5f53  dict_incorrect_S
+00012f70: 414d 504c 4544 5f4f 4253 203d 2050 6572  AMPLED_OBS = Per
+00012f80: 6365 6e74 5f49 445f 5465 7374 5f53 414d  cent_ID_Test_SAM
+00012f90: 504c 4544 5f4f 4253 4552 5645 4428 6d75  PLED_OBSERVED(mu
+00012fa0: 6c74 6969 6e64 6578 290a 2020 2020 2020  ltiindex).      
+00012fb0: 2020 6466 5f70 6964 5f53 414d 504c 4544    df_pid_SAMPLED
+00012fc0: 5f4f 4253 203d 2070 642e 636f 6e63 6174  _OBS = pd.concat
+00012fd0: 287b 6b3a 2070 642e 4461 7461 4672 616d  ({k: pd.DataFram
+00012fe0: 652e 6672 6f6d 5f64 6963 7428 762c 2027  e.from_dict(v, '
+00012ff0: 696e 6465 7827 2920 666f 7220 6b2c 2076  index') for k, v
+00013000: 2069 6e20 6469 6374 5f70 6964 5f53 414d   in dict_pid_SAM
+00013010: 504c 4544 5f4f 4253 2e69 7465 6d73 2829  PLED_OBS.items()
+00013020: 7d2c 2061 7869 733d 3029 0a20 2020 2020  }, axis=0).     
+00013030: 2020 2064 665f 626c 6f73 756d 5f53 414d     df_blosum_SAM
+00013040: 504c 4544 5f4f 4253 203d 2070 642e 636f  PLED_OBS = pd.co
+00013050: 6e63 6174 287b 6b3a 2070 642e 4461 7461  ncat({k: pd.Data
+00013060: 4672 616d 652e 6672 6f6d 5f64 6963 7428  Frame.from_dict(
+00013070: 762c 2027 696e 6465 7827 2920 666f 7220  v, 'index') for 
+00013080: 6b2c 2076 2069 6e20 6469 6374 5f62 6c6f  k, v in dict_blo
+00013090: 7375 6d5f 5341 4d50 4c45 445f 4f42 532e  sum_SAMPLED_OBS.
+000130a0: 6974 656d 7328 297d 2c61 7869 733d 3029  items()},axis=0)
+000130b0: 0a20 2020 2020 2020 2023 6466 5f69 6e63  .        #df_inc
+000130c0: 6f72 7265 6374 5f53 414d 504c 4544 5f4f  orrect_SAMPLED_O
+000130d0: 4253 203d 2070 642e 636f 6e63 6174 287b  BS = pd.concat({
+000130e0: 6b3a 2070 642e 4461 7461 4672 616d 652e  k: pd.DataFrame.
+000130f0: 6672 6f6d 5f64 6963 7428 762c 2027 696e  from_dict(v, 'in
+00013100: 6465 7827 2920 666f 7220 6b2c 2076 2069  dex') for k, v i
+00013110: 6e20 6469 6374 5f69 6e63 6f72 7265 6374  n dict_incorrect
+00013120: 5f53 414d 504c 4544 5f4f 4253 2e69 7465  _SAMPLED_OBS.ite
+00013130: 6d73 2829 7d2c 2061 7869 733d 3029 0a20  ms()}, axis=0). 
+00013140: 2020 2020 2020 2023 4869 6768 6c69 6768         #Highligh
+00013150: 743a 2053 616d 706c 6564 2076 7320 5361  t: Sampled vs Sa
+00013160: 6d70 6c65 640a 2020 2020 2020 2020 6469  mpled.        di
+00013170: 6374 5f70 6964 5f53 414d 504c 4544 5f53  ct_pid_SAMPLED_S
+00013180: 414d 504c 4544 2c64 6963 745f 626c 6f73  AMPLED,dict_blos
+00013190: 756d 5f53 414d 504c 4544 5f53 414d 504c  um_SAMPLED_SAMPL
+000131a0: 4544 3d50 6572 6365 6e74 5f49 445f 5465  ED=Percent_ID_Te
+000131b0: 7374 5f53 414d 504c 4544 5f53 414d 504c  st_SAMPLED_SAMPL
+000131c0: 4544 286d 756c 7469 696e 6465 7829 0a20  ED(multiindex). 
+000131d0: 2020 2020 2020 2064 665f 7069 645f 5341         df_pid_SA
+000131e0: 4d50 4c45 445f 5341 4d50 4c45 4420 3d20  MPLED_SAMPLED = 
+000131f0: 7064 2e63 6f6e 6361 7428 7b6b 3a20 7064  pd.concat({k: pd
+00013200: 2e44 6174 6146 7261 6d65 2e66 726f 6d5f  .DataFrame.from_
+00013210: 6469 6374 2876 2c20 2769 6e64 6578 2729  dict(v, 'index')
+00013220: 2066 6f72 206b 2c20 7620 696e 2064 6963   for k, v in dic
+00013230: 745f 7069 645f 5341 4d50 4c45 445f 5341  t_pid_SAMPLED_SA
+00013240: 4d50 4c45 442e 6974 656d 7328 297d 2c20  MPLED.items()}, 
+00013250: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+00013260: 6466 5f62 6c6f 7375 6d5f 5341 4d50 4c45  df_blosum_SAMPLE
+00013270: 445f 5341 4d50 4c45 4420 3d20 7064 2e63  D_SAMPLED = pd.c
+00013280: 6f6e 6361 7428 7b6b 3a20 7064 2e44 6174  oncat({k: pd.Dat
+00013290: 6146 7261 6d65 2e66 726f 6d5f 6469 6374  aFrame.from_dict
+000132a0: 2876 2c20 2769 6e64 6578 2729 2066 6f72  (v, 'index') for
+000132b0: 206b 2c20 7620 696e 2064 6963 745f 626c   k, v in dict_bl
+000132c0: 6f73 756d 5f53 414d 504c 4544 5f53 414d  osum_SAMPLED_SAM
+000132d0: 504c 4544 2e69 7465 6d73 2829 7d2c 2061  PLED.items()}, a
+000132e0: 7869 733d 3029 0a0a 2020 2020 656c 7365  xis=0)..    else
+000132f0: 3a0a 2020 2020 2020 2020 2320 4869 6768  :.        # High
+00013300: 6c69 6768 743a 2073 616d 706c 6564 2076  light: sampled v
+00013310: 7320 6f62 7365 7276 6564 0a20 2020 2020  s observed.     
+00013320: 2020 2064 6963 745f 7069 645f 5341 4d50     dict_pid_SAMP
+00013330: 4c45 445f 4f42 532c 2064 6963 745f 626c  LED_OBS, dict_bl
+00013340: 6f73 756d 5f53 414d 504c 4544 5f4f 4253  osum_SAMPLED_OBS
+00013350: 2c64 6963 745f 696e 636f 7272 6563 745f  ,dict_incorrect_
+00013360: 5341 4d50 4c45 445f 4f42 5320 3d20 5065  SAMPLED_OBS = Pe
+00013370: 7263 656e 745f 4944 5f54 6573 745f 5341  rcent_ID_Test_SA
+00013380: 4d50 4c45 445f 4f42 5345 5256 4544 286d  MPLED_OBSERVED(m
+00013390: 756c 7469 696e 6465 7829 0a20 2020 2020  ultiindex).     
+000133a0: 2020 2064 665f 7069 645f 5341 4d50 4c45     df_pid_SAMPLE
+000133b0: 445f 4f42 5320 3d20 7064 2e44 6174 6146  D_OBS = pd.DataF
+000133c0: 7261 6d65 2864 6963 745f 7069 645f 5341  rame(dict_pid_SA
+000133d0: 4d50 4c45 445f 4f42 5329 0a20 2020 2020  MPLED_OBS).     
+000133e0: 2020 2064 665f 626c 6f73 756d 5f53 414d     df_blosum_SAM
+000133f0: 504c 4544 5f4f 4253 203d 2070 642e 4461  PLED_OBS = pd.Da
+00013400: 7461 4672 616d 6528 6469 6374 5f62 6c6f  taFrame(dict_blo
+00013410: 7375 6d5f 5341 4d50 4c45 445f 4f42 5329  sum_SAMPLED_OBS)
+00013420: 0a20 2020 2020 2020 2023 6466 5f69 6e63  .        #df_inc
+00013430: 6f72 7265 6374 5f53 414d 504c 4544 5f4f  orrect_SAMPLED_O
+00013440: 4253 203d 2070 642e 4461 7461 4672 616d  BS = pd.DataFram
+00013450: 6528 6469 6374 5f69 6e63 6f72 7265 6374  e(dict_incorrect
+00013460: 5f53 414d 504c 4544 5f4f 4253 292e 746f  _SAMPLED_OBS).to
+00013470: 5f6e 756d 7079 2829 0a20 2020 2020 2020  _numpy().       
+00013480: 2023 4869 6768 6c69 6768 743a 2053 616d   #Highlight: Sam
+00013490: 706c 6564 2076 7320 5361 6d70 6c65 640a  pled vs Sampled.
+000134a0: 2020 2020 2020 2020 6469 6374 5f70 6964          dict_pid
+000134b0: 5f53 414d 504c 4544 5f53 414d 504c 4544  _SAMPLED_SAMPLED
+000134c0: 2c20 6469 6374 5f62 6c6f 7375 6d5f 5341  , dict_blosum_SA
+000134d0: 4d50 4c45 445f 5341 4d50 4c45 4420 3d20  MPLED_SAMPLED = 
+000134e0: 5065 7263 656e 745f 4944 5f54 6573 745f  Percent_ID_Test_
+000134f0: 5341 4d50 4c45 445f 5341 4d50 4c45 4428  SAMPLED_SAMPLED(
+00013500: 6d75 6c74 6969 6e64 6578 290a 2020 2020  multiindex).    
+00013510: 2020 2020 6466 5f70 6964 5f53 414d 504c      df_pid_SAMPL
+00013520: 4544 5f53 414d 504c 4544 203d 2070 642e  ED_SAMPLED = pd.
+00013530: 4461 7461 4672 616d 6528 6469 6374 5f70  DataFrame(dict_p
+00013540: 6964 5f53 414d 504c 4544 5f53 414d 504c  id_SAMPLED_SAMPL
+00013550: 4544 290a 2020 2020 2020 2020 6466 5f62  ED).        df_b
+00013560: 6c6f 7375 6d5f 5341 4d50 4c45 445f 5341  losum_SAMPLED_SA
+00013570: 4d50 4c45 4420 3d20 7064 2e44 6174 6146  MPLED = pd.DataF
+00013580: 7261 6d65 2864 6963 745f 626c 6f73 756d  rame(dict_blosum
+00013590: 5f53 414d 504c 4544 5f53 414d 504c 4544  _SAMPLED_SAMPLED
+000135a0: 290a 0a0a 2020 2020 6469 6374 5f70 6964  )...    dict_pid
+000135b0: 5f4f 4253 5f4f 4253 2c64 6963 745f 626c  _OBS_OBS,dict_bl
+000135c0: 6f73 756d 5f4f 4253 5f4f 4253 203d 2050  osum_OBS_OBS = P
+000135d0: 6572 6365 6e74 5f49 445f 5465 7374 5f4f  ercent_ID_Test_O
+000135e0: 4253 5f4f 4253 4552 5645 4428 290a 2020  BS_OBSERVED().  
+000135f0: 2020 6466 5f70 6964 5f4f 4253 5f4f 4253    df_pid_OBS_OBS
+00013600: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
+00013610: 6469 6374 5f70 6964 5f4f 4253 5f4f 4253  dict_pid_OBS_OBS
+00013620: 290a 2020 2020 6466 5f62 6c6f 7375 6d5f  ).    df_blosum_
+00013630: 4f42 535f 4f42 5320 3d20 7064 2e44 6174  OBS_OBS = pd.Dat
+00013640: 6146 7261 6d65 2864 6963 745f 626c 6f73  aFrame(dict_blos
+00013650: 756d 5f4f 4253 5f4f 4253 290a 0a20 2020  um_OBS_OBS)..   
+00013660: 2023 6466 5f6c 7420 3d20 6466 5f4f 4253   #df_lt = df_OBS
+00013670: 5f4f 4253 2e77 6865 7265 286e 702e 7472  _OBS.where(np.tr
+00013680: 696c 286e 702e 6f6e 6573 2864 665f 4f42  il(np.ones(df_OB
+00013690: 535f 4f42 532e 7368 6170 6529 292e 6173  S_OBS.shape)).as
+000136a0: 7479 7065 286e 702e 626f 6f6c 2929 0a20  type(np.bool)). 
+000136b0: 2020 2061 6e6e 6f74 203d 2046 616c 7365     annot = False
+000136c0: 0a20 2020 2050 6c6f 745f 4865 6174 6d61  .    Plot_Heatma
+000136d0: 7028 6466 5f70 6964 5f4f 4253 5f4f 4253  p(df_pid_OBS_OBS
+000136e0: 2c22 4f42 5320 7365 7173 2076 7320 4f42  ,"OBS seqs vs OB
+000136f0: 5320 7365 7173 2025 4944 222c 2250 4944  S seqs %ID","PID
+00013700: 5f7b 7d5f 4f42 535f 4f42 5322 2e66 6f72  _{}_OBS_OBS".for
+00013710: 6d61 7428 666f 6c64 6572 292c 616e 6e6f  mat(folder),anno
+00013720: 743d 616e 6e6f 742c 6d61 736b 3d4e 6f6e  t=annot,mask=Non
+00013730: 652c 766d 6178 3d31 3030 290a 2020 2020  e,vmax=100).    
+00013740: 506c 6f74 5f48 6561 746d 6170 2864 665f  Plot_Heatmap(df_
+00013750: 7069 645f 5341 4d50 4c45 445f 4f42 532c  pid_SAMPLED_OBS,
+00013760: 2022 4f42 5320 7673 2053 414d 504c 4544   "OBS vs SAMPLED
+00013770: 2073 6571 7320 4156 4552 4147 4520 2549   seqs AVERAGE %I
+00013780: 4422 2c20 2250 4944 5f7b 7d5f 4f42 535f  D", "PID_{}_OBS_
+00013790: 5341 4d50 4c45 4422 2e66 6f72 6d61 7428  SAMPLED".format(
+000137a0: 666f 6c64 6572 292c 616e 6e6f 743d 616e  folder),annot=an
+000137b0: 6e6f 742c 6d61 736b 3d4e 6f6e 652c 766d  not,mask=None,vm
+000137c0: 6178 3d31 3030 290a 2020 2020 506c 6f74  ax=100).    Plot
+000137d0: 5f48 6561 746d 6170 2864 665f 7069 645f  _Heatmap(df_pid_
+000137e0: 5341 4d50 4c45 445f 5341 4d50 4c45 442c  SAMPLED_SAMPLED,
+000137f0: 2022 5341 4d50 4c45 4420 7673 2053 414d   "SAMPLED vs SAM
+00013800: 504c 4544 2073 6571 7320 4156 4552 4147  PLED seqs AVERAG
+00013810: 4520 2549 4422 2c20 2250 4944 5f7b 7d5f  E %ID", "PID_{}_
+00013820: 5341 4d50 4c45 445f 5341 4d50 4c45 4422  SAMPLED_SAMPLED"
+00013830: 2e66 6f72 6d61 7428 666f 6c64 6572 292c  .format(folder),
+00013840: 616e 6e6f 743d 616e 6e6f 742c 6d61 736b  annot=annot,mask
+00013850: 3d4e 6f6e 652c 766d 6178 3d31 3030 290a  =None,vmax=100).
+00013860: 0a20 2020 2076 6d61 7820 3d20 6d61 7828  .    vmax = max(
+00013870: 5b64 665f 626c 6f73 756d 5f4f 4253 5f4f  [df_blosum_OBS_O
+00013880: 4253 2e6d 6178 2829 2e6d 6178 2829 2c64  BS.max().max(),d
+00013890: 665f 626c 6f73 756d 5f53 414d 504c 4544  f_blosum_SAMPLED
+000138a0: 5f53 414d 504c 4544 2e6d 6178 2829 2e6d  _SAMPLED.max().m
+000138b0: 6178 2829 2c64 665f 626c 6f73 756d 5f53  ax(),df_blosum_S
+000138c0: 414d 504c 4544 5f4f 4253 2e6d 6178 2829  AMPLED_OBS.max()
+000138d0: 2e6d 6178 2829 5d29 0a20 2020 2050 6c6f  .max()]).    Plo
+000138e0: 745f 4865 6174 6d61 7028 6466 5f62 6c6f  t_Heatmap(df_blo
+000138f0: 7375 6d5f 4f42 535f 4f42 532c 2022 4f42  sum_OBS_OBS, "OB
+00013900: 5320 7365 7173 2076 7320 4f42 5320 7365  S seqs vs OBS se
+00013910: 7173 2042 6c6f 7375 6d20 5363 6f72 6522  qs Blosum Score"
+00013920: 2c20 2242 6c6f 7375 6d5f 7b7d 5f4f 4253  , "Blosum_{}_OBS
+00013930: 5f4f 4253 222e 666f 726d 6174 2866 6f6c  _OBS".format(fol
+00013940: 6465 7229 2c61 6e6e 6f74 3d61 6e6e 6f74  der),annot=annot
+00013950: 2c6d 6173 6b3d 4e6f 6e65 2c76 6d61 783d  ,mask=None,vmax=
+00013960: 766d 6178 290a 2020 2020 506c 6f74 5f48  vmax).    Plot_H
+00013970: 6561 746d 6170 2864 665f 626c 6f73 756d  eatmap(df_blosum
+00013980: 5f53 414d 504c 4544 5f4f 4253 2c20 224f  _SAMPLED_OBS, "O
+00013990: 4253 2076 7320 5341 4d50 4c45 4420 7365  BS vs SAMPLED se
+000139a0: 7173 2041 5645 5241 4745 2042 6c6f 7375  qs AVERAGE Blosu
+000139b0: 6d20 5363 6f72 6522 2c20 2242 6c6f 7375  m Score", "Blosu
+000139c0: 6d5f 7b7d 5f4f 4253 5f53 414d 504c 4544  m_{}_OBS_SAMPLED
+000139d0: 222e 666f 726d 6174 2866 6f6c 6465 7229  ".format(folder)
+000139e0: 2c61 6e6e 6f74 3d61 6e6e 6f74 2c6d 6173  ,annot=annot,mas
+000139f0: 6b3d 4e6f 6e65 2c76 6d61 783d 766d 6178  k=None,vmax=vmax
+00013a00: 290a 2020 2020 506c 6f74 5f48 6561 746d  ).    Plot_Heatm
+00013a10: 6170 2864 665f 626c 6f73 756d 5f53 414d  ap(df_blosum_SAM
+00013a20: 504c 4544 5f53 414d 504c 4544 2c20 2253  PLED_SAMPLED, "S
+00013a30: 414d 504c 4544 2076 7320 5341 4d50 4c45  AMPLED vs SAMPLE
+00013a40: 4420 7365 7173 2041 5645 5241 4745 2042  D seqs AVERAGE B
+00013a50: 6c6f 7375 6d20 5363 6f72 6522 2c20 2242  losum Score", "B
+00013a60: 6c6f 7375 6d5f 7b7d 5f53 414d 504c 4544  losum_{}_SAMPLED
+00013a70: 5f53 414d 504c 4544 222e 666f 726d 6174  _SAMPLED".format
+00013a80: 2866 6f6c 6465 7229 2c61 6e6e 6f74 3d61  (folder),annot=a
+00013a90: 6e6e 6f74 2c6d 6173 6b3d 4e6f 6e65 2c76  nnot,mask=None,v
+00013aa0: 6d61 7820 3d20 766d 6178 290a 6465 6620  max = vmax).def 
+00013ab0: 6275 696c 645f 6461 7461 6672 616d 6573  build_dataframes
+00013ac0: 5f6f 7665 726c 6170 7069 6e67 5f68 6973  _overlapping_his
+00013ad0: 746f 6772 616d 7328 6161 5f73 6571 7565  tograms(aa_seque
+00013ae0: 6e63 6573 5f70 7265 6469 6374 696f 6e73  nces_predictions
+00013af0: 2c20 6461 7461 7365 745f 7472 6169 6e2c  , dataset_train,
+00013b00: 6461 7461 7365 745f 7465 7374 2c20 6e61  dataset_test, na
+00013b10: 6d65 2c20 6e5f 7361 6d70 6c65 732c 6e6f  me, n_samples,no
+00013b20: 6465 735f 696e 6465 7865 732c 7265 7375  des_indexes,resu
+00013b30: 6c74 735f 6469 7265 6374 6f72 792c 6161  lts_directory,aa
+00013b40: 5f70 726f 6273 2c63 6f72 7265 7370 6f6e  _probs,correspon
+00013b50: 6465 6e63 655f 6469 6374 3d4e 6f6e 6529  dence_dict=None)
+00013b60: 3a0a 2020 2020 2222 2250 6c6f 7420 6869  :.    """Plot hi
+00013b70: 7374 6f67 7261 6d20 7768 6f73 6520 6261  stogram whose ba
+00013b80: 7273 2072 6570 7265 7365 6e74 2074 6865  rs represent the
+00013b90: 2070 6572 6365 6e74 6167 6520 6964 656e   percentage iden
+00013ba0: 7469 7479 2062 6574 7765 656e 2074 6865  tity between the
+00013bb0: 2074 7275 6520 616e 6365 7374 6f72 7320   true ancestors 
+00013bc0: 7673 2074 7275 6520 6c65 6176 6573 2061  vs true leaves a
+00013bd0: 6e64 2074 6865 2070 7265 6469 6374 6564  nd the predicted
+00013be0: 2061 6e63 6573 746f 7273 2076 7320 7472   ancestors vs tr
+00013bf0: 7565 206c 6561 7665 730a 2020 2020 3a70  ue leaves.    :p
+00013c00: 6172 616d 2074 656e 736f 7220 6161 5f73  aram tensor aa_s
+00013c10: 6571 7565 6e63 6573 5f70 7265 6469 6374  equences_predict
+00013c20: 696f 6e73 3a0a 2020 2020 3a70 6172 616d  ions:.    :param
+00013c30: 2074 656e 736f 7220 6461 7461 7365 745f   tensor dataset_
+00013c40: 7472 6169 6e0a 2020 2020 3a70 6172 616d  train.    :param
+00013c50: 2074 656e 736f 7220 6461 7461 7365 745f   tensor dataset_
+00013c60: 7465 7374 0a20 2020 203a 7061 7261 6d20  test.    :param 
+00013c70: 7374 7220 6e61 6d65 3a20 6461 7461 7365  str name: datase
+00013c80: 7420 6e61 6d65 2070 726f 6a65 6374 0a20  t name project. 
+00013c90: 2020 203a 7061 7261 6d20 7465 6e73 6f72     :param tensor
+00013ca0: 2061 615f 7365 7175 656e 6365 735f 7072   aa_sequences_pr
+00013cb0: 6564 6963 7469 6f6e 730a 2020 2020 3a70  edictions.    :p
+00013cc0: 6172 616d 2069 6e74 206e 5f73 616d 706c  aram int n_sampl
+00013cd0: 6573 3a20 6e75 6d62 6572 206f 6620 7361  es: number of sa
+00013ce0: 6d70 6c65 6420 7072 6564 6963 7469 6f6e  mpled prediction
+00013cf0: 730a 2020 2020 3a70 6172 616d 206e 6f64  s.    :param nod
+00013d00: 6573 5f69 6e64 6578 6573 3a0a 2020 2020  es_indexes:.    
+00013d10: 3a70 6172 616d 2073 7472 2072 6573 756c  :param str resul
+00013d20: 7473 5f64 6972 6563 746f 7279 0a20 2020  ts_directory.   
+00013d30: 203a 7061 7261 6d20 696e 7420 6161 5f70   :param int aa_p
+00013d40: 726f 623a 2061 6d69 6e6f 2061 6369 6420  rob: amino acid 
+00013d50: 7072 6f62 6162 696c 6974 6965 7320 2869  probabilities (i
+00013d60: 2e65 2032 3129 0a20 2020 203a 7061 7261  .e 21).    :para
+00013d70: 6d20 6469 6374 2063 6f72 7265 7370 6f6e  m dict correspon
+00013d80: 6465 6e63 655f 6469 6374 3a20 636f 7272  dence_dict: corr
+00013d90: 6573 706f 6e64 656e 6365 2062 6574 7765  espondence betwe
+00013da0: 656e 2074 6865 2074 7265 6520 6c65 7665  en the tree leve
+00013db0: 6c20 6f72 6465 7220 696e 6465 7865 7320  l order indexes 
+00013dc0: 616e 6420 7468 6520 2d2d 3e20 6f6e 6c79  and the --> only
+00013dd0: 2075 7365 6675 6c20 666f 7220 6265 6e63   useful for benc
+00013de0: 686d 6172 6b5f 7261 6e64 616c 6c5f 6f72  hmark_randall_or
+00013df0: 6967 696e 616c 5f6e 616d 696e 670a 2020  iginal_naming.  
+00013e00: 2020 2222 220a 2020 2020 2268 7474 7073    """.    "https
+00013e10: 3a2f 2f6d 6174 706c 6f74 6c69 622e 6f72  ://matplotlib.or
+00013e20: 672f 332e 312e 312f 6761 6c6c 6572 792f  g/3.1.1/gallery/
+00013e30: 756e 6974 732f 6261 725f 756e 6974 5f64  units/bar_unit_d
+00013e40: 656d 6f2e 6874 6d6c 2373 7068 782d 676c  emo.html#sphx-gl
+00013e50: 722d 6761 6c6c 6572 792d 756e 6974 732d  r-gallery-units-
+00013e60: 6261 722d 756e 6974 2d64 656d 6f2d 7079  bar-unit-demo-py
+00013e70: 220a 2020 2020 7072 696e 7428 2242 7569  ".    print("Bui
+00013e80: 6c64 696e 6720 4f76 6572 6c61 7070 696e  lding Overlappin
+00013e90: 6720 4869 7374 6f67 7261 6d2e 2e2e 2229  g Histogram...")
+00013ea0: 0a20 2020 206e 5f63 6869 6c64 7265 6e20  .    n_children 
+00013eb0: 3d20 6c65 6e28 6e6f 6465 735f 696e 6465  = len(nodes_inde
+00013ec0: 7865 7329 0a20 2020 2064 6566 2050 6572  xes).    def Per
+00013ed0: 6365 6e74 5f49 445f 4f42 535f 4f42 5328  cent_ID_OBS_OBS(
+00013ee0: 293a 0a20 2020 2020 2020 2022 4765 6e65  ):.        "Gene
+00013ef0: 7261 7465 2074 6865 2020 2549 4420 6f66  rate the  %ID of
+00013f00: 2074 6865 204f 4253 2054 4553 5420 7365   the OBS TEST se
+00013f10: 7175 656e 6365 7320 6167 6169 6e73 7420  quences against 
+00013f20: 7468 6520 4f42 5320 7472 6169 6e22 0a20  the OBS train". 
+00013f30: 2020 2020 2020 2070 6572 6365 6e74 5f69         percent_i
+00013f40: 645f 4f42 5320 3d20 6469 6374 2e66 726f  d_OBS = dict.fro
+00013f50: 6d6b 6579 7328 6461 7461 7365 745f 7472  mkeys(dataset_tr
+00013f60: 6169 6e5b 3a2c 302c 315d 2e74 6f6c 6973  ain[:,0,1].tolis
+00013f70: 7428 292c 2064 6963 742e 6672 6f6d 6b65  t(), dict.fromke
+00013f80: 7973 2864 6174 6173 6574 5f74 6573 745b  ys(dataset_test[
+00013f90: 3a2c 302c 315d 2e74 6f6c 6973 7428 292c  :,0,1].tolist(),
+00013fa0: 5b5d 2929 0a20 2020 2020 2020 2066 6f72  [])).        for
+00013fb0: 2069 2c74 7261 696e 7365 7120 696e 2065   i,trainseq in e
+00013fc0: 6e75 6d65 7261 7465 2864 6174 6173 6574  numerate(dataset
+00013fd0: 5f74 7261 696e 293a 0a20 2020 2020 2020  _train):.       
+00013fe0: 2020 2020 2073 6571 5f54 5241 494e 5f6f       seq_TRAIN_o
+00013ff0: 6273 5f6c 6574 7465 7273 5f69 203d 2063  bs_letters_i = c
+00014000: 6f6e 7665 7274 5f74 6f5f 6c65 7474 6572  onvert_to_letter
+00014010: 7328 6461 7461 7365 745f 7472 6169 6e5b  s(dataset_train[
+00014020: 692c 2032 3a2c 305d 2c61 615f 7072 6f62  i, 2:,0],aa_prob
+00014030: 7329 0a20 2020 2020 2020 2020 2020 2066  s).            f
+00014040: 6f72 206a 2c74 6573 7473 6571 2069 6e20  or j,testseq in 
+00014050: 656e 756d 6572 6174 6528 6461 7461 7365  enumerate(datase
+00014060: 745f 7465 7374 293a 0a20 2020 2020 2020  t_test):.       
+00014070: 2020 2020 2020 2020 2073 6571 5f54 4553           seq_TES
+00014080: 545f 6f62 735f 6c65 7474 6572 735f 6920  T_obs_letters_i 
+00014090: 3d20 636f 6e76 6572 745f 746f 5f6c 6574  = convert_to_let
+000140a0: 7465 7273 2864 6174 6173 6574 5f74 6573  ters(dataset_tes
+000140b0: 745b 6a2c 2032 3a2c 305d 2c61 615f 7072  t[j, 2:,0],aa_pr
+000140c0: 6f62 7329 0a20 2020 2020 2020 2020 2020  obs).           
+000140d0: 2020 2020 2070 6964 203d 7065 7263 5f69       pid =perc_i
+000140e0: 6465 6e74 6974 795f 7061 6972 5f73 6571  dentity_pair_seq
+000140f0: 2873 6571 5f54 5241 494e 5f6f 6273 5f6c  (seq_TRAIN_obs_l
+00014100: 6574 7465 7273 5f69 2c73 6571 5f54 4553  etters_i,seq_TES
+00014110: 545f 6f62 735f 6c65 7474 6572 735f 6929  T_obs_letters_i)
+00014120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014130: 2070 6572 6365 6e74 5f69 645f 4f42 535b   percent_id_OBS[
+00014140: 6461 7461 7365 745f 7472 6169 6e5b 692c  dataset_train[i,
+00014150: 302c 315d 2e69 7465 6d28 295d 5b64 6174  0,1].item()][dat
+00014160: 6173 6574 5f74 6573 745b 6a2c 302c 315d  aset_test[j,0,1]
+00014170: 2e69 7465 6d28 295d 203d 2070 6964 0a20  .item()] = pid. 
+00014180: 2020 2020 2020 2072 6574 7572 6e20 7065         return pe
+00014190: 7263 656e 745f 6964 5f4f 4253 0a20 2020  rcent_id_OBS.   
+000141a0: 2064 6566 2050 6572 6365 6e74 5f49 445f   def Percent_ID_
+000141b0: 5052 4544 5f4f 4253 2829 3a0a 2020 2020  PRED_OBS():.    
+000141c0: 2020 2020 2247 656e 6572 6174 6520 7468      "Generate th
+000141d0: 6520 4176 6572 6167 6520 616e 6420 5354  e Average and ST
+000141e0: 4420 2549 4420 6f66 2074 6865 2073 616d  D %ID of the sam
+000141f0: 706c 6564 2073 6571 7565 6e63 6573 2061  pled sequences a
+00014200: 6761 696e 7374 2074 6865 204f 4253 2074  gainst the OBS t
+00014210: 7261 696e 220a 2020 2020 2020 2020 2370  rain".        #p
+00014220: 6572 6365 6e74 5f69 645f 5052 4544 203d  ercent_id_PRED =
+00014230: 2064 6963 742e 6672 6f6d 6b65 7973 2844   dict.fromkeys(D
+00014240: 6174 6173 6574 5f74 7261 696e 5b3a 2c30  ataset_train[:,0
+00014250: 2c31 5d2e 746f 6c69 7374 2829 2c20 6469  ,1].tolist(), di
+00014260: 6374 2e66 726f 6d6b 6579 7328 7072 6564  ct.fromkeys(pred
+00014270: 6963 7469 6f6e 735f 7361 6d70 6c65 735b  ictions_samples[
+00014280: 302c 3a2c 315d 2e74 6f6c 6973 7428 292c  0,:,1].tolist(),
+00014290: 7b22 4176 6572 6167 6522 3a5b 5d2c 2253  {"Average":[],"S
+000142a0: 7464 223a 5b5d 7d29 2920 237b 2241 7665  td":[]})) #{"Ave
+000142b0: 7261 6765 223a 5b5d 2c22 5374 6422 3a5b  rage":[],"Std":[
+000142c0: 5d7d 0a20 2020 2020 2020 2070 6572 6365  ]}.        perce
+000142d0: 6e74 5f69 645f 5052 4544 203d 2064 6566  nt_id_PRED = def
+000142e0: 6175 6c74 6469 6374 286c 616d 6264 613a  aultdict(lambda:
+000142f0: 2064 6566 6175 6c74 6469 6374 286c 616d   defaultdict(lam
+00014300: 6264 613a 2064 6566 6175 6c74 6469 6374  bda: defaultdict
+00014310: 2864 6963 7429 2929 0a20 2020 2020 2020  (dict))).       
+00014320: 2066 6f72 2069 2c20 7365 7120 696e 2065   for i, seq in e
+00014330: 6e75 6d65 7261 7465 2864 6174 6173 6574  numerate(dataset
+00014340: 5f74 7261 696e 293a 0a20 2020 2020 2020  _train):.       
+00014350: 2020 2020 2073 6571 5f54 5241 494e 5f6f       seq_TRAIN_o
+00014360: 6273 5f6c 6574 7465 7273 5f69 203d 2063  bs_letters_i = c
+00014370: 6f6e 7665 7274 5f74 6f5f 6c65 7474 6572  onvert_to_letter
+00014380: 7328 6461 7461 7365 745f 7472 6169 6e5b  s(dataset_train[
+00014390: 692c 2032 3a2c 305d 2c61 615f 7072 6f62  i, 2:,0],aa_prob
+000143a0: 7329 0a20 2020 2020 2020 2020 2020 2066  s).            f
+000143b0: 6f72 206a 2069 6e20 7261 6e67 6528 6e5f  or j in range(n_
+000143c0: 6368 696c 6472 656e 293a 2366 6f72 2074  children):#for t
+000143d0: 6573 7420 6e6f 6465 2023 6e5f 6368 696c  est node #n_chil
+000143e0: 6472 656e 0a20 2020 2020 2020 2020 2020  dren.           
+000143f0: 2020 2020 2061 6c6c 5f73 616d 706c 6564       all_sampled
+00014400: 5f69 6e64 6578 203d 2061 615f 7365 7175  _index = aa_sequ
+00014410: 656e 6365 735f 7072 6564 6963 7469 6f6e  ences_prediction
+00014420: 735b 3a2c 6a2c 333a 5d20 2023 2041 6c6c  s[:,j,3:]  # All
+00014430: 2073 616d 706c 6573 2066 6f72 2073 616d   samples for sam
+00014440: 6520 7465 7374 2073 6571 0a20 2020 2020  e test seq.     
+00014450: 2020 2020 2020 2020 2020 2070 6572 6365             perce
+00014460: 6e74 5f69 645f 693d 5b5d 2023 616c 6c20  nt_id_i=[] #all 
+00014470: 7361 6d70 6c65 7320 666f 7220 7468 6520  samples for the 
+00014480: 7361 6d65 2074 6573 7420 7365 7175 656e  same test sequen
+00014490: 6365 0a20 2020 2020 2020 2020 2020 2020  ce.             
+000144a0: 2020 2066 6f72 2077 2069 6e20 7261 6e67     for w in rang
+000144b0: 6528 6e5f 7361 6d70 6c65 7329 3a0a 2020  e(n_samples):.  
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144d0: 2020 7365 715f 7361 6d70 6c65 645f 7465    seq_sampled_te
+000144e0: 7374 203d 2063 6f6e 7665 7274 5f74 6f5f  st = convert_to_
+000144f0: 6c65 7474 6572 7328 616c 6c5f 7361 6d70  letters(all_samp
+00014500: 6c65 645f 696e 6465 785b 775d 2c61 615f  led_index[w],aa_
+00014510: 7072 6f62 7329 0a20 2020 2020 2020 2020  probs).         
+00014520: 2020 2020 2020 2020 2020 2070 6964 203d             pid =
+00014530: 2070 6572 635f 6964 656e 7469 7479 5f70   perc_identity_p
+00014540: 6169 725f 7365 7128 7365 715f 5452 4149  air_seq(seq_TRAI
+00014550: 4e5f 6f62 735f 6c65 7474 6572 735f 692c  N_obs_letters_i,
+00014560: 2073 6571 5f73 616d 706c 6564 5f74 6573   seq_sampled_tes
+00014570: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00014580: 2020 2020 2020 2070 6572 6365 6e74 5f69         percent_i
+00014590: 645f 692e 6170 7065 6e64 2870 6964 290a  d_i.append(pid).
+000145a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145b0: 7065 7263 656e 745f 6964 5f50 5245 445b  percent_id_PRED[
+000145c0: 6461 7461 7365 745f 7472 6169 6e5b 692c  dataset_train[i,
+000145d0: 302c 315d 2e69 7465 6d28 295d 5b61 615f  0,1].item()][aa_
+000145e0: 7365 7175 656e 6365 735f 7072 6564 6963  sequences_predic
+000145f0: 7469 6f6e 735b 302c 6a2c 315d 5d5b 2241  tions[0,j,1]]["A
+00014600: 7665 7261 6765 225d 203d 206e 702e 6d65  verage"] = np.me
+00014610: 616e 286e 702e 6172 7261 7928 7065 7263  an(np.array(perc
+00014620: 656e 745f 6964 5f69 292c 6178 6973 3d30  ent_id_i),axis=0
+00014630: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014640: 2020 7065 7263 656e 745f 6964 5f50 5245    percent_id_PRE
+00014650: 445b 6461 7461 7365 745f 7472 6169 6e5b  D[dataset_train[
+00014660: 692c 302c 315d 2e69 7465 6d28 295d 5b61  i,0,1].item()][a
+00014670: 615f 7365 7175 656e 6365 735f 7072 6564  a_sequences_pred
+00014680: 6963 7469 6f6e 735b 302c 6a2c 315d 5d5b  ictions[0,j,1]][
+00014690: 2253 7464 225d 203d 206e 702e 7374 6428  "Std"] = np.std(
+000146a0: 6e70 2e61 7272 6179 2870 6572 6365 6e74  np.array(percent
+000146b0: 5f69 645f 6929 2c20 6178 6973 3d30 290a  _id_i), axis=0).
+000146c0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+000146d0: 6572 6365 6e74 5f69 645f 5052 4544 0a0a  ercent_id_PRED..
+000146e0: 0a20 2020 2070 6572 6365 6e74 5f69 645f  .    percent_id_
+000146f0: 5052 4544 203d 2050 6572 6365 6e74 5f49  PRED = Percent_I
+00014700: 445f 5052 4544 5f4f 4253 2829 0a20 2020  D_PRED_OBS().   
+00014710: 2070 6572 6365 6e74 5f69 645f 4f42 5320   percent_id_OBS 
+00014720: 3d20 5065 7263 656e 745f 4944 5f4f 4253  = Percent_ID_OBS
+00014730: 5f4f 4253 2829 0a0a 2020 2020 6669 6720  _OBS()..    fig 
+00014740: 3d20 706c 742e 6669 6775 7265 2866 6967  = plt.figure(fig
+00014750: 7369 7a65 3d28 3138 2c20 3529 290a 2020  size=(18, 5)).  
+00014760: 2020 6178 203d 2066 6967 2e61 6464 5f73    ax = fig.add_s
+00014770: 7562 706c 6f74 2831 3131 290a 0a20 2020  ubplot(111)..   
+00014780: 2023 2320 496e 6465 7865 7320 7768 6572   ## Indexes wher
+00014790: 6520 7468 6520 6261 7273 2077 696c 6c20  e the bars will 
+000147a0: 676f 0a20 2020 2069 6e64 5f6c 696e 6573  go.    ind_lines
+000147b0: 203d 206e 702e 6172 616e 6765 2831 302c   = np.arange(10,
+000147c0: 6c65 6e28 6461 7461 7365 745f 7472 6169  len(dataset_trai
+000147d0: 6e29 2a31 302c 3130 2029 0a20 2020 2069  n)*10,10 ).    i
+000147e0: 6e64 5f74 7261 696e 203d 206e 702e 6172  nd_train = np.ar
+000147f0: 616e 6765 2835 2c6c 656e 2864 6174 6173  ange(5,len(datas
+00014800: 6574 5f74 7261 696e 292a 3130 2c31 3020  et_train)*10,10 
+00014810: 2920 2023 2074 6865 2078 206c 6f63 6174  )  # the x locat
+00014820: 696f 6e73 2066 6f72 2074 6865 2074 7261  ions for the tra
+00014830: 696e 206e 6f64 6573 0a20 2020 2077 6964  in nodes.    wid
+00014840: 7468 203d 2031 302f 6c65 6e28 6461 7461  th = 10/len(data
+00014850: 7365 745f 7465 7374 2920 2d30 2e33 2023  set_test) -0.3 #
+00014860: 2074 6865 2077 6964 7468 206f 6620 7468   the width of th
+00014870: 6520 6261 7273 0a20 2020 2069 6e64 5f74  e bars.    ind_t
+00014880: 6573 7420 3d20 6e70 2e61 7261 6e67 6528  est = np.arange(
+00014890: 302c 3130 2c77 6964 7468 202b 2030 2e33  0,10,width + 0.3
+000148a0: 2920 2023 2074 6865 2078 206c 6f63 6174  )  # the x locat
+000148b0: 696f 6e73 2066 6f72 2074 6865 2074 6573  ions for the tes
+000148c0: 7420 6e6f 6465 732c 2074 616b 696e 6720  t nodes, taking 
+000148d0: 696e 746f 2061 6363 6f75 6e74 2074 6865  into account the
+000148e0: 2073 7061 6365 2062 6574 7765 656e 2074   space between t
+000148f0: 6865 6d3f 0a20 2020 2073 7461 7274 203d  hem?.    start =
+00014900: 2030 0a20 2020 2062 6c75 652c 203d 2073   0.    blue, = s
+00014910: 6e73 2e63 6f6c 6f72 5f70 616c 6574 7465  ns.color_palette
+00014920: 2822 6d75 7465 6422 2c20 3129 0a20 2020  ("muted", 1).   
+00014930: 2066 6f72 2074 7261 696e 5f6e 6f64 6520   for train_node 
+00014940: 696e 2064 6174 6173 6574 5f74 7261 696e  in dataset_train
+00014950: 5b3a 2c30 2c31 5d3a 0a20 2020 2020 2020  [:,0,1]:.       
+00014960: 2066 6f72 2069 6478 2c74 6573 745f 6e6f   for idx,test_no
+00014970: 6465 2069 6e20 656e 756d 6572 6174 6528  de in enumerate(
+00014980: 6461 7461 7365 745f 7465 7374 5b3a 2c30  dataset_test[:,0
+00014990: 2c31 5d29 3a20 2354 4f44 4f3a 206f 7574  ,1]): #TODO: out
+000149a0: 206f 6620 7261 6e67 650a 2020 2020 2020   of range.      
+000149b0: 2020 2020 2020 7265 6374 7332 203d 2061        rects2 = a
+000149c0: 782e 6261 7228 696e 645f 7465 7374 5b69  x.bar(ind_test[i
+000149d0: 6478 5d20 2b20 7374 6172 7420 2c0a 2020  dx] + start ,.  
 000149e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149f0: 2020 2020 7065 7263 656e 745f 6964 5f4f      percent_id_O
-00014a00: 4253 5b74 7261 696e 5f6e 6f64 652e 6974  BS[train_node.it
-00014a10: 656d 2829 5d5b 7465 7374 5f6e 6f64 652e  em()][test_node.
-00014a20: 6974 656d 2829 5d2c 0a20 2020 2020 2020  item()],.       
+000149f0: 2020 2020 2020 2020 2020 7065 7263 656e            percen
+00014a00: 745f 6964 5f4f 4253 5b74 7261 696e 5f6e  t_id_OBS[train_n
+00014a10: 6f64 652e 6974 656d 2829 5d5b 7465 7374  ode.item()][test
+00014a20: 5f6e 6f64 652e 6974 656d 2829 5d2c 0a20  _node.item()],. 
 00014a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a40: 2020 2020 2077 6964 7468 2c0a 2020 2020       width,.    
-00014a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a60: 2020 2020 2020 2020 636f 6c6f 723d 2767          color='g
-00014a70: 7265 656e 272c 0a20 2020 2020 2020 2020  reen',.         
+00014a40: 2020 2020 2020 2020 2020 2077 6964 7468             width
+00014a50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014a60: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00014a70: 6c6f 723d 2767 7265 656e 272c 0a20 2020  lor='green',.   
 00014a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a90: 2020 2079 6572 723d 5b30 5d2c 0a20 2020     yerr=[0],.   
-00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ab0: 2020 2020 2020 2020 2065 7272 6f72 5f6b           error_k
-00014ac0: 773d 6469 6374 2865 6c69 6e65 7769 6474  w=dict(elinewidt
-00014ad0: 683d 302e 3031 2c20 6563 6f6c 6f72 3d27  h=0.01, ecolor='
-00014ae0: 7265 6427 292c 0a20 2020 2020 2020 2020  red'),.         
+00014a90: 2020 2020 2020 2020 2079 6572 723d 5b30           yerr=[0
+00014aa0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00014ab0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00014ac0: 7272 6f72 5f6b 773d 6469 6374 2865 6c69  rror_kw=dict(eli
+00014ad0: 6e65 7769 6474 683d 302e 3031 2c20 6563  newidth=0.01, ec
+00014ae0: 6f6c 6f72 3d27 7265 6427 292c 0a20 2020  olor='red'),.   
 00014af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b00: 2020 206c 6162 656c 3d22 4f42 5345 5256     label="OBSERV
-00014b10: 4544 2229 0a20 2020 2020 2020 2020 2020  ED").           
-00014b20: 2072 6563 7473 3120 3d20 6178 2e62 6172   rects1 = ax.bar
-00014b30: 2869 6e64 5f74 6573 745b 6964 785d 202b  (ind_test[idx] +
-00014b40: 2073 7461 7274 2c0a 2020 2020 2020 2020   start,.        
+00014b00: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
+00014b10: 4f42 5345 5256 4544 2229 0a20 2020 2020  OBSERVED").     
+00014b20: 2020 2020 2020 2072 6563 7473 3120 3d20         rects1 = 
+00014b30: 6178 2e62 6172 2869 6e64 5f74 6573 745b  ax.bar(ind_test[
+00014b40: 6964 785d 202b 2073 7461 7274 2c0a 2020  idx] + start,.  
 00014b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b60: 2020 2020 7065 7263 656e 745f 6964 5f50      percent_id_P
-00014b70: 5245 445b 7472 6169 6e5f 6e6f 6465 2e69  RED[train_node.i
-00014b80: 7465 6d28 295d 5b74 6573 745f 6e6f 6465  tem()][test_node
-00014b90: 2e69 7465 6d28 295d 5b22 4176 6572 6167  .item()]["Averag
-00014ba0: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
+00014b60: 2020 2020 2020 2020 2020 7065 7263 656e            percen
+00014b70: 745f 6964 5f50 5245 445b 7472 6169 6e5f  t_id_PRED[train_
+00014b80: 6e6f 6465 2e69 7465 6d28 295d 5b74 6573  node.item()][tes
+00014b90: 745f 6e6f 6465 2e69 7465 6d28 295d 5b22  t_node.item()]["
+00014ba0: 4176 6572 6167 6522 5d2c 0a20 2020 2020  Average"],.     
 00014bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bc0: 2077 6964 7468 2c0a 2020 2020 2020 2020   width,.        
+00014bc0: 2020 2020 2020 2077 6964 7468 2c0a 2020         width,.  
 00014bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014be0: 2020 2020 636f 6c6f 723d 226f 7261 6e67      color="orang
-00014bf0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00014be0: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
+00014bf0: 226f 7261 6e67 6522 2c0a 2020 2020 2020  "orange",.      
 00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c10: 616c 7068 613d 312c 0a20 2020 2020 2020  alpha=1,.       
+00014c10: 2020 2020 2020 616c 7068 613d 312c 0a20        alpha=1,. 
 00014c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c30: 2020 2020 2079 6572 723d 7065 7263 656e       yerr=percen
-00014c40: 745f 6964 5f50 5245 445b 7472 6169 6e5f  t_id_PRED[train_
-00014c50: 6e6f 6465 2e69 7465 6d28 295d 5b74 6573  node.item()][tes
-00014c60: 745f 6e6f 6465 2e69 7465 6d28 295d 5b22  t_node.item()]["
-00014c70: 5374 6422 5d2c 0a20 2020 2020 2020 2020  Std"],.         
+00014c30: 2020 2020 2020 2020 2020 2079 6572 723d             yerr=
+00014c40: 7065 7263 656e 745f 6964 5f50 5245 445b  percent_id_PRED[
+00014c50: 7472 6169 6e5f 6e6f 6465 2e69 7465 6d28  train_node.item(
+00014c60: 295d 5b74 6573 745f 6e6f 6465 2e69 7465  )][test_node.ite
+00014c70: 6d28 295d 5b22 5374 6422 5d2c 0a20 2020  m()]["Std"],.   
 00014c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c90: 2020 2065 7272 6f72 5f6b 773d 6469 6374     error_kw=dict
-00014ca0: 2865 6c69 6e65 7769 6474 683d 302e 3031  (elinewidth=0.01
-00014cb0: 2c20 6563 6f6c 6f72 3d27 7265 6427 292c  , ecolor='red'),
-00014cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014cd0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-00014ce0: 656c 3d22 5341 4d50 4c45 4422 290a 0a20  el="SAMPLED").. 
-00014cf0: 2020 2020 2020 2073 7461 7274 202b 3d20         start += 
-00014d00: 3130 0a20 2020 2023 2061 7865 7320 616e  10.    # axes an
-00014d10: 6420 6c61 6265 6c73 0a20 2020 2061 782e  d labels.    ax.
-00014d20: 7365 745f 786c 696d 282d 7769 6474 682c  set_xlim(-width,
-00014d30: 206e 702e 6d61 7828 696e 645f 7472 6169   np.max(ind_trai
-00014d40: 6e29 202b 3529 0a20 2020 2061 782e 7365  n) +5).    ax.se
-00014d50: 745f 796c 696d 2830 2c20 3130 3029 0a20  t_ylim(0, 100). 
-00014d60: 2020 2061 782e 7365 745f 796c 6162 656c     ax.set_ylabel
-00014d70: 2827 2549 4427 290a 2020 2020 6178 2e73  ('%ID').    ax.s
-00014d80: 6574 5f74 6974 6c65 2827 4f76 6572 6c61  et_title('Overla
-00014d90: 7070 696e 6720 4869 7374 6f67 7261 6d27  pping Histogram'
-00014da0: 290a 2020 2020 7854 6963 6b4d 6172 6b73  ).    xTickMarks
-00014db0: 203d 205b 2754 7261 696e 4e6f 6465 5f7b   = ['TrainNode_{
-00014dc0: 7d27 2e66 6f72 6d61 7428 696e 7428 692e  }'.format(int(i.
-00014dd0: 6974 656d 2829 2929 2066 6f72 2069 2069  item())) for i i
-00014de0: 6e20 6461 7461 7365 745f 7472 6169 6e5b  n dataset_train[
-00014df0: 3a2c 302c 315d 5d0a 2020 2020 6178 2e73  :,0,1]].    ax.s
-00014e00: 6574 5f78 7469 636b 7328 696e 645f 7472  et_xticks(ind_tr
-00014e10: 6169 6e29 0a20 2020 2078 7469 636b 4e61  ain).    xtickNa
-00014e20: 6d65 7320 3d20 6178 2e73 6574 5f78 7469  mes = ax.set_xti
-00014e30: 636b 6c61 6265 6c73 2878 5469 636b 4d61  cklabels(xTickMa
-00014e40: 726b 7329 0a20 2020 2070 6c74 2e73 6574  rks).    plt.set
-00014e50: 7028 7874 6963 6b4e 616d 6573 2c20 726f  p(xtickNames, ro
-00014e60: 7461 7469 6f6e 3d34 352c 2066 6f6e 7473  tation=45, fonts
-00014e70: 697a 653d 3629 0a20 2020 2070 6c74 2e76  ize=6).    plt.v
-00014e80: 6c69 6e65 7328 696e 645f 6c69 6e65 732c  lines(ind_lines,
-00014e90: 796d 696e 3d30 2c79 6d61 783d 3130 3029  ymin=0,ymax=100)
-00014ea0: 0a20 2020 2023 2320 6164 6420 6120 6c65  .    ## add a le
-00014eb0: 6765 6e64 2d2d 3e20 4e6f 7420 776f 726b  gend--> Not work
-00014ec0: 696e 6720 2869 6e73 6964 6520 6f72 206f  ing (inside or o
-00014ed0: 7574 7369 6465 206c 6f6f 7029 0a20 2020  utside loop).   
-00014ee0: 2061 782e 6c65 6765 6e64 2828 7265 6374   ax.legend((rect
-00014ef0: 7331 2c72 6563 7473 3229 2c20 2827 5361  s1,rects2), ('Sa
-00014f00: 6d70 6c65 6427 2c22 4f62 7365 7276 6564  mpled',"Observed
-00014f10: 2229 2c6c 6f63 3d31 2c62 626f 785f 746f  "),loc=1,bbox_to
-00014f20: 5f61 6e63 686f 723d 2831 2e31 352c 2031  _anchor=(1.15, 1
-00014f30: 2e31 2929 0a20 2020 2070 6c74 2e73 6176  .1)).    plt.sav
-00014f40: 6566 6967 2822 7b7d 2f4f 7665 726c 6170  efig("{}/Overlap
-00014f50: 7069 6e67 4869 7374 6f67 7261 6d22 2e66  pingHistogram".f
-00014f60: 6f72 6d61 7428 7265 7375 6c74 735f 6469  ormat(results_di
-00014f70: 7265 6374 6f72 7929 290a 6465 6620 7472  rectory)).def tr
-00014f80: 6565 5f70 6f73 6974 696f 6e61 6c5f 656d  ee_positional_em
-00014f90: 6265 6464 696e 6773 2861 6e63 6573 746f  beddings(ancesto
-00014fa0: 725f 696e 666f 5f64 6963 742c 7472 6565  r_info_dict,tree
-00014fb0: 5f62 795f 6c65 7665 6c73 5f64 6963 7429  _by_levels_dict)
-00014fc0: 3a0a 2020 2020 2222 2254 6865 206e 6f64  :.    """The nod
-00014fd0: 6573 206f 7264 6572 6564 2062 7920 7472  es ordered by tr
-00014fe0: 6565 206c 6576 656c 206f 7264 6572 2061  ee level order a
-00014ff0: 7265 2063 6f6e 7665 7274 6564 2069 6e74  re converted int
-00015000: 6f20 736f 6d65 7768 6174 206f 6e65 2d68  o somewhat one-h
-00015010: 6f74 2065 6e63 6f64 6564 206c 696b 6520  ot encoded like 
-00015020: 656d 6265 6464 696e 6773 0a20 2020 2049  embeddings.    I
-00015030: 6d70 6c65 6d65 6e74 6174 6564 2066 6f6c  mplementated fol
-00015040: 6c6f 7769 6e67 0a20 2020 2068 7474 7073  lowing.    https
-00015050: 3a2f 2f70 6170 6572 732e 6e69 7073 2e63  ://papers.nips.c
-00015060: 632f 7061 7065 722f 3230 3139 2f66 696c  c/paper/2019/fil
-00015070: 652f 3665 3039 3137 3436 3932 3134 6438  e/6e0917469214d8
-00015080: 6662 6438 6335 3137 6463 6463 3662 3864  fbd8c517dcdc6b8d
-00015090: 6366 2d50 6170 6572 2e70 6466 0a20 2020  cf-Paper.pdf.   
-000150a0: 2049 6e70 7574 3a20 5472 6565 2062 7920   Input: Tree by 
-000150b0: 6c65 7665 6c73 2069 6e20 7472 6176 6572  levels in traver
-000150c0: 7361 6c20 6f72 6465 720a 2020 2020 4f75  sal order.    Ou
-000150d0: 7470 7574 3a20 5265 7072 6573 656e 7461  tput: Representa
-000150e0: 7469 6f6e 7320 6f66 2074 6865 2070 6f73  tions of the pos
-000150f0: 6974 696f 6e20 6f66 2074 6865 206e 6f64  ition of the nod
-00015100: 6520 696e 2074 6865 2074 7265 6520 696e  e in the tree in
-00015110: 206f 6e65 2068 6f74 2062 6974 2065 6e63   one hot bit enc
-00015120: 6f64 696e 672e 2054 6865 7920 7265 7072  oding. They repr
-00015130: 6573 656e 7420 7468 6520 6f6e 6520 686f  esent the one ho
-00015140: 7420 656e 636f 6465 6420 7061 7468 2066  t encoded path f
-00015150: 726f 6d20 726f 6f74 2074 6f20 7468 6520  rom root to the 
-00015160: 6e6f 6465 2022 2222 0a20 2020 2064 6567  node """.    deg
-00015170: 7265 655f 7472 6565 203d 320a 2020 2020  ree_tree =2.    
-00015180: 6e5f 6c65 7665 6c73 203d 206c 656e 2874  n_levels = len(t
-00015190: 7265 655f 6279 5f6c 6576 656c 735f 6469  ree_by_levels_di
-000151a0: 6374 290a 2020 2020 6e6f 6465 735f 7265  ct).    nodes_re
-000151b0: 7072 6573 656e 7461 7469 6f6e 733d 6465  presentations=de
-000151c0: 6661 756c 7464 6963 7428 290a 2020 2020  faultdict().    
-000151d0: 6e6f 6465 5f72 6570 7265 7365 6e74 6174  node_representat
-000151e0: 696f 6e20 3d20 5b30 5d2a 2864 6567 7265  ion = [0]*(degre
-000151f0: 655f 7472 6565 2a6e 5f6c 6576 656c 7329  e_tree*n_levels)
-00015200: 2023 696e 6974 6961 7465 2074 6865 2072   #initiate the r
-00015210: 6f6f 7420 746f 2061 6c6c 2030 0a20 2020  oot to all 0.   
-00015220: 2066 6f72 206c 6576 656c 5f6e 616d 652c   for level_name,
-00015230: 206c 6576 656c 5f6e 6f64 6573 2069 6e20   level_nodes in 
-00015240: 736f 7274 6564 2874 7265 655f 6279 5f6c  sorted(tree_by_l
-00015250: 6576 656c 735f 6469 6374 2e69 7465 6d73  evels_dict.items
-00015260: 2829 293a 0a20 2020 2020 2020 2061 6c6c  ()):.        all
-00015270: 5f61 6e63 6573 746f 7273 5f69 6e5f 6c65  _ancestors_in_le
-00015280: 7665 6c20 3d20 7b69 6e64 6578 3a61 6e63  vel = {index:anc
-00015290: 6573 746f 725f 696e 666f 5f64 6963 745b  estor_info_dict[
-000152a0: 6e6f 6465 5d20 666f 7220 696e 6465 782c  node] for index,
-000152b0: 6e6f 6465 2069 6e20 656e 756d 6572 6174  node in enumerat
-000152c0: 6528 6c65 7665 6c5f 6e6f 6465 7329 7d20  e(level_nodes)} 
-000152d0: 2366 696e 6420 7468 6520 696e 6465 7865  #find the indexe
-000152e0: 7320 6f66 2074 6865 206e 6f64 6573 2073  s of the nodes s
-000152f0: 6861 7269 6e67 2074 6865 2073 616d 6520  haring the same 
-00015300: 616e 6365 7374 6f72 730a 2020 2020 2020  ancestors.      
-00015310: 2020 6966 206e 702e 6e61 6e20 696e 2061    if np.nan in a
-00015320: 6c6c 5f61 6e63 6573 746f 7273 5f69 6e5f  ll_ancestors_in_
-00015330: 6c65 7665 6c2e 7661 6c75 6573 2829 3a23  level.values():#
-00015340: 6964 656e 7469 6679 2072 6f6f 742c 2062  identify root, b
-00015350: 6563 6175 7365 2069 7420 6861 7320 6e61  ecause it has na
-00015360: 6e20 6173 2061 6e20 616e 6365 7374 6f72  n as an ancestor
-00015370: 0a20 2020 2020 2020 2020 2020 206e 6f64  .            nod
-00015380: 6573 5f72 6570 7265 7365 6e74 6174 696f  es_representatio
-00015390: 6e73 5b6c 6576 656c 5f6e 6f64 6573 5b30  ns[level_nodes[0
-000153a0: 5d5d 203d 206e 6f64 655f 7265 7072 6573  ]] = node_repres
-000153b0: 656e 7461 7469 6f6e 0a20 2020 2020 2020  entation.       
-000153c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000153d0: 2020 206e 6f64 655f 7265 7072 6573 656e     node_represen
-000153e0: 7461 7469 6f6e 203d 206e 6f64 655f 7265  tation = node_re
-000153f0: 7072 6573 656e 7461 7469 6f6e 5b3a 2d64  presentation[:-d
-00015400: 6567 7265 655f 7472 6565 5d0a 2020 2020  egree_tree].    
-00015410: 2020 2020 2020 2020 6c65 7665 6c5f 7061          level_pa
-00015420: 6972 7320 3d20 5b6c 6576 656c 5f6e 6f64  irs = [level_nod
-00015430: 6573 5b69 3a69 202b 2064 6567 7265 655f  es[i:i + degree_
-00015440: 7472 6565 5d20 666f 7220 6920 696e 2072  tree] for i in r
-00015450: 616e 6765 2830 2c20 6c65 6e28 6c65 7665  ange(0, len(leve
-00015460: 6c5f 6e6f 6465 7329 2c20 6465 6772 6565  l_nodes), degree
-00015470: 5f74 7265 6529 5d20 2344 6976 6964 6520  _tree)] #Divide 
-00015480: 6c65 7665 6c20 696e 2067 726f 7570 7320  level in groups 
-00015490: 6f66 2032 2c20 7468 6520 7472 6565 2069  of 2, the tree i
-000154a0: 7320 696e 2074 7265 6520 7472 6176 6572  s in tree traver
-000154b0: 7361 6c2c 2073 6f20 6576 6572 7974 6869  sal, so everythi
-000154c0: 6e67 2073 686f 7564 6c20 6265 206f 7264  ng shoudl be ord
-000154d0: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
-000154e0: 2066 6f72 206c 6576 656c 5f70 6169 7220   for level_pair 
-000154f0: 696e 206c 6576 656c 5f70 6169 7273 3a20  in level_pairs: 
-00015500: 2374 6865 7365 2070 6169 7273 2068 6176  #these pairs hav
-00015510: 6520 7361 6d65 2061 6e63 6573 746f 7220  e same ancestor 
-00015520: 6265 6361 7573 6520 6f66 2074 7265 6520  because of tree 
-00015530: 6c65 7665 6c73 2061 7265 206f 7267 616e  levels are organ
-00015540: 697a 6564 2069 6e20 7472 6176 6572 7361  ized in traversa
-00015550: 6c20 6f72 6465 720a 2020 2020 2020 2020  l order.        
-00015560: 2020 2020 2020 2020 2367 6574 2074 6865          #get the
-00015570: 2061 6e63 6573 746f 7220 6e6f 6465 2072   ancestor node r
-00015580: 6570 7265 7365 6e74 6174 696f 6e0a 2020  epresentation.  
-00015590: 2020 2020 2020 2020 2020 2020 2020 616e                an
-000155a0: 6365 7374 6f72 203d 2061 6e63 6573 746f  cestor = ancesto
-000155b0: 725f 696e 666f 5f64 6963 745b 6c65 7665  r_info_dict[leve
-000155c0: 6c5f 7061 6972 5b30 5d5d 2023 6a75 7374  l_pair[0]] #just
-000155d0: 2075 7365 206f 6e65 206f 6620 7468 656d   use one of them
-000155e0: 2074 6f20 6765 7420 7468 6520 616e 6365   to get the ance
-000155f0: 7374 6f72 0a20 2020 2020 2020 2020 2020  stor.           
-00015600: 2020 2020 206e 6f64 655f 7265 7072 6573       node_repres
-00015610: 656e 7461 7469 6f6e 203d 206e 6f64 6573  entation = nodes
-00015620: 5f72 6570 7265 7365 6e74 6174 696f 6e73  _representations
-00015630: 5b61 6e63 6573 746f 725d 5b3a 2d64 6567  [ancestor][:-deg
-00015640: 7265 655f 7472 6565 5d0a 2020 2020 2020  ree_tree].      
-00015650: 2020 2020 2020 2020 2020 6164 6465 645f            added_
-00015660: 7265 7072 6573 656e 7461 7469 6f6e 203d  representation =
-00015670: 5b30 5d2a 320a 2020 2020 2020 2020 2020  [0]*2.          
-00015680: 2020 2020 2020 666f 7220 696e 6465 782c        for index,
-00015690: 6e6f 6465 2069 6e20 656e 756d 6572 6174  node in enumerat
-000156a0: 6528 6c65 7665 6c5f 7061 6972 293a 0a20  e(level_pair):. 
-000156b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156c0: 2020 2061 6464 6564 5f72 6570 7265 7365     added_represe
-000156d0: 6e74 6174 696f 6e5b 696e 6465 785d 203d  ntation[index] =
-000156e0: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-000156f0: 2020 2020 2020 6e6f 6465 5f72 6570 7265        node_repre
-00015700: 7365 6e74 6174 696f 6e20 3d20 6164 6465  sentation = adde
-00015710: 645f 7265 7072 6573 656e 7461 7469 6f6e  d_representation
-00015720: 202b 206e 6f64 655f 7265 7072 6573 656e   + node_represen
-00015730: 7461 7469 6f6e 0a20 2020 2020 2020 2020  tation.         
-00015740: 2020 2020 2020 2020 2020 206e 6f64 6573             nodes
-00015750: 5f72 6570 7265 7365 6e74 6174 696f 6e73  _representations
-00015760: 5b6e 6f64 655d 203d 206e 6f64 655f 7265  [node] = node_re
-00015770: 7072 6573 656e 7461 7469 6f6e 0a20 2020  presentation.   
-00015780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015790: 2061 6464 6564 5f72 6570 7265 7365 6e74   added_represent
-000157a0: 6174 696f 6e20 3d20 5b30 5d20 2a20 3220  ation = [0] * 2 
-000157b0: 2372 6573 7461 7274 0a20 2020 2020 2020  #restart.       
-000157c0: 2020 2020 2020 2020 2020 2020 206e 6f64               nod
-000157d0: 655f 7265 7072 6573 656e 7461 7469 6f6e  e_representation
-000157e0: 203d 206e 6f64 6573 5f72 6570 7265 7365   = nodes_represe
-000157f0: 6e74 6174 696f 6e73 5b61 6e63 6573 746f  ntations[ancesto
-00015800: 725d 5b3a 2d64 6567 7265 655f 7472 6565  r][:-degree_tree
-00015810: 5d20 2372 6573 7461 7274 0a20 2020 206e  ] #restart.    n
-00015820: 6f64 6573 5f72 6570 7265 7365 6e74 6174  odes_representat
-00015830: 696f 6e73 5f61 7272 6179 203d 206e 702e  ions_array = np.
-00015840: 7673 7461 636b 286c 6973 7428 6e6f 6465  vstack(list(node
-00015850: 735f 7265 7072 6573 656e 7461 7469 6f6e  s_representation
-00015860: 732e 7661 6c75 6573 2829 2929 0a20 2020  s.values())).   
-00015870: 206e 6f64 6573 5f72 6570 7265 7365 6e74   nodes_represent
-00015880: 6174 696f 6e73 5f61 7272 6179 203d 206e  ations_array = n
-00015890: 702e 635f 5b20 6e70 2e61 7272 6179 286c  p.c_[ np.array(l
-000158a0: 6973 7428 6e6f 6465 735f 7265 7072 6573  ist(nodes_repres
-000158b0: 656e 7461 7469 6f6e 732e 6b65 7973 2829  entations.keys()
-000158c0: 2929 5b3a 2c4e 6f6e 655d 2c20 6e6f 6465  ))[:,None], node
-000158d0: 735f 7265 7072 6573 656e 7461 7469 6f6e  s_representation
-000158e0: 735f 6172 7261 795d 0a20 2020 2072 6574  s_array].    ret
-000158f0: 7572 6e20 6e6f 6465 735f 7265 7072 6573  urn nodes_repres
-00015900: 656e 7461 7469 6f6e 735f 6172 7261 790a  entations_array.
-00015910: 6465 6620 6578 7472 615f 7072 6f63 6573  def extra_proces
-00015920: 7369 6e67 2861 6e63 6573 746f 725f 696e  sing(ancestor_in
-00015930: 666f 2c70 6174 7269 7374 6963 5f6d 6174  fo,patristic_mat
-00015940: 7269 782c 7265 7375 6c74 735f 6469 722c  rix,results_dir,
-00015950: 6172 6773 2c62 7569 6c64 5f63 6f6e 6669  args,build_confi
-00015960: 6729 3a0a 2020 2020 2222 2243 6f6d 7075  g):.    """Compu
-00015970: 7465 7320 736f 6d65 2064 6963 7469 6f6e  tes some diction
-00015980: 6172 6965 7320 7769 7468 2074 6865 206e  aries with the n
-00015990: 6f64 6573 206f 7264 6572 6564 2069 6e20  odes ordered in 
-000159a0: 7472 6565 206c 6576 656c 206f 7264 6572  tree level order
-000159b0: 2c20 7072 6f63 6573 7365 7320 7468 6520  , processes the 
-000159c0: 626c 6f73 756d 206d 6174 7269 7820 616e  blosum matrix an
-000159d0: 6420 6275 696c 6420 6120 6772 6170 6820  d build a graph 
-000159e0: 7769 7468 2074 6865 2074 7265 6520 6e6f  with the tree no
-000159f0: 6465 7320 616e 6420 7468 6520 6272 616e  des and the bran
-00015a00: 6368 206c 656e 6774 6873 2061 7320 6564  ch lengths as ed
-00015a10: 6765 730a 2020 2020 203a 7061 7261 6d20  ges.     :param 
-00015a20: 6e61 6d65 6474 7570 6c65 2061 6e63 6573  namedtuple ances
-00015a30: 746f 725f 696e 666f 0a20 2020 2020 3a70  tor_info.     :p
-00015a40: 6172 616d 2074 656e 736f 7220 7061 7472  aram tensor patr
-00015a50: 6973 7469 635f 6d61 7472 6978 3a20 5b6e  istic_matrix: [n
-00015a60: 5f6c 6561 7665 7320 2b20 6e5f 696e 7465  _leaves + n_inte
-00015a70: 726e 616c 202b 2031 2c20 6e5f 6c65 6176  rnal + 1, n_leav
-00015a80: 6573 202b 206e 5f69 6e74 6572 6e61 6c20  es + n_internal 
-00015a90: 2b20 315d 0a20 2020 2020 3a70 6172 616d  + 1].     :param
-00015aa0: 2073 7472 2072 6573 756c 7473 5f64 6972   str results_dir
-00015ab0: 0a20 2020 2020 3a70 6172 616d 206e 616d  .     :param nam
-00015ac0: 6564 7475 706c 6520 6172 6773 0a20 2020  edtuple args.   
-00015ad0: 2020 3a70 6172 616d 206e 616d 6564 7475    :param namedtu
-00015ae0: 706c 6520 6275 696c 645f 636f 6e66 6967  ple build_config
-00015af0: 2222 220a 2020 2020 4164 6469 7469 6f6e  """.    Addition
-00015b00: 616c 496e 666f 203d 206e 616d 6564 7475  alInfo = namedtu
-00015b10: 706c 6528 2241 6464 6974 696f 6e61 6c49  ple("AdditionalI
-00015b20: 6e66 6f22 2c0a 2020 2020 2020 2020 2020  nfo",.          
+00014c90: 2020 2020 2020 2020 2065 7272 6f72 5f6b           error_k
+00014ca0: 773d 6469 6374 2865 6c69 6e65 7769 6474  w=dict(elinewidt
+00014cb0: 683d 302e 3031 2c20 6563 6f6c 6f72 3d27  h=0.01, ecolor='
+00014cc0: 7265 6427 292c 0a20 2020 2020 2020 2020  red'),.         
+00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ce0: 2020 206c 6162 656c 3d22 5341 4d50 4c45     label="SAMPLE
+00014cf0: 4422 290a 0a20 2020 2020 2020 2073 7461  D")..        sta
+00014d00: 7274 202b 3d20 3130 0a20 2020 2023 2061  rt += 10.    # a
+00014d10: 7865 7320 616e 6420 6c61 6265 6c73 0a20  xes and labels. 
+00014d20: 2020 2061 782e 7365 745f 786c 696d 282d     ax.set_xlim(-
+00014d30: 7769 6474 682c 206e 702e 6d61 7828 696e  width, np.max(in
+00014d40: 645f 7472 6169 6e29 202b 3529 0a20 2020  d_train) +5).   
+00014d50: 2061 782e 7365 745f 796c 696d 2830 2c20   ax.set_ylim(0, 
+00014d60: 3130 3029 0a20 2020 2061 782e 7365 745f  100).    ax.set_
+00014d70: 796c 6162 656c 2827 2549 4427 290a 2020  ylabel('%ID').  
+00014d80: 2020 6178 2e73 6574 5f74 6974 6c65 2827    ax.set_title('
+00014d90: 4f76 6572 6c61 7070 696e 6720 4869 7374  Overlapping Hist
+00014da0: 6f67 7261 6d27 290a 2020 2020 7854 6963  ogram').    xTic
+00014db0: 6b4d 6172 6b73 203d 205b 2754 7261 696e  kMarks = ['Train
+00014dc0: 4e6f 6465 5f7b 7d27 2e66 6f72 6d61 7428  Node_{}'.format(
+00014dd0: 696e 7428 692e 6974 656d 2829 2929 2066  int(i.item())) f
+00014de0: 6f72 2069 2069 6e20 6461 7461 7365 745f  or i in dataset_
+00014df0: 7472 6169 6e5b 3a2c 302c 315d 5d0a 2020  train[:,0,1]].  
+00014e00: 2020 6178 2e73 6574 5f78 7469 636b 7328    ax.set_xticks(
+00014e10: 696e 645f 7472 6169 6e29 0a20 2020 2078  ind_train).    x
+00014e20: 7469 636b 4e61 6d65 7320 3d20 6178 2e73  tickNames = ax.s
+00014e30: 6574 5f78 7469 636b 6c61 6265 6c73 2878  et_xticklabels(x
+00014e40: 5469 636b 4d61 726b 7329 0a20 2020 2070  TickMarks).    p
+00014e50: 6c74 2e73 6574 7028 7874 6963 6b4e 616d  lt.setp(xtickNam
+00014e60: 6573 2c20 726f 7461 7469 6f6e 3d34 352c  es, rotation=45,
+00014e70: 2066 6f6e 7473 697a 653d 3629 0a20 2020   fontsize=6).   
+00014e80: 2070 6c74 2e76 6c69 6e65 7328 696e 645f   plt.vlines(ind_
+00014e90: 6c69 6e65 732c 796d 696e 3d30 2c79 6d61  lines,ymin=0,yma
+00014ea0: 783d 3130 3029 0a20 2020 2023 2320 6164  x=100).    ## ad
+00014eb0: 6420 6120 6c65 6765 6e64 2d2d 3e20 4e6f  d a legend--> No
+00014ec0: 7420 776f 726b 696e 6720 2869 6e73 6964  t working (insid
+00014ed0: 6520 6f72 206f 7574 7369 6465 206c 6f6f  e or outside loo
+00014ee0: 7029 0a20 2020 2061 782e 6c65 6765 6e64  p).    ax.legend
+00014ef0: 2828 7265 6374 7331 2c72 6563 7473 3229  ((rects1,rects2)
+00014f00: 2c20 2827 5361 6d70 6c65 6427 2c22 4f62  , ('Sampled',"Ob
+00014f10: 7365 7276 6564 2229 2c6c 6f63 3d31 2c62  served"),loc=1,b
+00014f20: 626f 785f 746f 5f61 6e63 686f 723d 2831  box_to_anchor=(1
+00014f30: 2e31 352c 2031 2e31 2929 0a20 2020 2070  .15, 1.1)).    p
+00014f40: 6c74 2e73 6176 6566 6967 2822 7b7d 2f4f  lt.savefig("{}/O
+00014f50: 7665 726c 6170 7069 6e67 4869 7374 6f67  verlappingHistog
+00014f60: 7261 6d22 2e66 6f72 6d61 7428 7265 7375  ram".format(resu
+00014f70: 6c74 735f 6469 7265 6374 6f72 7929 290a  lts_directory)).
+00014f80: 6465 6620 7472 6565 5f70 6f73 6974 696f  def tree_positio
+00014f90: 6e61 6c5f 656d 6265 6464 696e 6773 2861  nal_embeddings(a
+00014fa0: 6e63 6573 746f 725f 696e 666f 5f64 6963  ncestor_info_dic
+00014fb0: 742c 7472 6565 5f62 795f 6c65 7665 6c73  t,tree_by_levels
+00014fc0: 5f64 6963 7429 3a0a 2020 2020 2222 2254  _dict):.    """T
+00014fd0: 6865 206e 6f64 6573 206f 7264 6572 6564  he nodes ordered
+00014fe0: 2062 7920 7472 6565 206c 6576 656c 206f   by tree level o
+00014ff0: 7264 6572 2061 7265 2063 6f6e 7665 7274  rder are convert
+00015000: 6564 2069 6e74 6f20 736f 6d65 7768 6174  ed into somewhat
+00015010: 206f 6e65 2d68 6f74 2065 6e63 6f64 6564   one-hot encoded
+00015020: 206c 696b 6520 656d 6265 6464 696e 6773   like embeddings
+00015030: 0a20 2020 2049 6d70 6c65 6d65 6e74 6174  .    Implementat
+00015040: 6564 2066 6f6c 6c6f 7769 6e67 0a20 2020  ed following.   
+00015050: 2068 7474 7073 3a2f 2f70 6170 6572 732e   https://papers.
+00015060: 6e69 7073 2e63 632f 7061 7065 722f 3230  nips.cc/paper/20
+00015070: 3139 2f66 696c 652f 3665 3039 3137 3436  19/file/6e091746
+00015080: 3932 3134 6438 6662 6438 6335 3137 6463  9214d8fbd8c517dc
+00015090: 6463 3662 3864 6366 2d50 6170 6572 2e70  dc6b8dcf-Paper.p
+000150a0: 6466 0a20 2020 2049 6e70 7574 3a20 5472  df.    Input: Tr
+000150b0: 6565 2062 7920 6c65 7665 6c73 2069 6e20  ee by levels in 
+000150c0: 7472 6176 6572 7361 6c20 6f72 6465 720a  traversal order.
+000150d0: 2020 2020 4f75 7470 7574 3a20 5265 7072      Output: Repr
+000150e0: 6573 656e 7461 7469 6f6e 7320 6f66 2074  esentations of t
+000150f0: 6865 2070 6f73 6974 696f 6e20 6f66 2074  he position of t
+00015100: 6865 206e 6f64 6520 696e 2074 6865 2074  he node in the t
+00015110: 7265 6520 696e 206f 6e65 2068 6f74 2062  ree in one hot b
+00015120: 6974 2065 6e63 6f64 696e 672e 2054 6865  it encoding. The
+00015130: 7920 7265 7072 6573 656e 7420 7468 6520  y represent the 
+00015140: 6f6e 6520 686f 7420 656e 636f 6465 6420  one hot encoded 
+00015150: 7061 7468 2066 726f 6d20 726f 6f74 2074  path from root t
+00015160: 6f20 7468 6520 6e6f 6465 2022 2222 0a20  o the node """. 
+00015170: 2020 2064 6567 7265 655f 7472 6565 203d     degree_tree =
+00015180: 320a 2020 2020 6e5f 6c65 7665 6c73 203d  2.    n_levels =
+00015190: 206c 656e 2874 7265 655f 6279 5f6c 6576   len(tree_by_lev
+000151a0: 656c 735f 6469 6374 290a 2020 2020 6e6f  els_dict).    no
+000151b0: 6465 735f 7265 7072 6573 656e 7461 7469  des_representati
+000151c0: 6f6e 733d 6465 6661 756c 7464 6963 7428  ons=defaultdict(
+000151d0: 290a 2020 2020 6e6f 6465 5f72 6570 7265  ).    node_repre
+000151e0: 7365 6e74 6174 696f 6e20 3d20 5b30 5d2a  sentation = [0]*
+000151f0: 2864 6567 7265 655f 7472 6565 2a6e 5f6c  (degree_tree*n_l
+00015200: 6576 656c 7329 2023 696e 6974 6961 7465  evels) #initiate
+00015210: 2074 6865 2072 6f6f 7420 746f 2061 6c6c   the root to all
+00015220: 2030 0a20 2020 2066 6f72 206c 6576 656c   0.    for level
+00015230: 5f6e 616d 652c 206c 6576 656c 5f6e 6f64  _name, level_nod
+00015240: 6573 2069 6e20 736f 7274 6564 2874 7265  es in sorted(tre
+00015250: 655f 6279 5f6c 6576 656c 735f 6469 6374  e_by_levels_dict
+00015260: 2e69 7465 6d73 2829 293a 0a20 2020 2020  .items()):.     
+00015270: 2020 2061 6c6c 5f61 6e63 6573 746f 7273     all_ancestors
+00015280: 5f69 6e5f 6c65 7665 6c20 3d20 7b69 6e64  _in_level = {ind
+00015290: 6578 3a61 6e63 6573 746f 725f 696e 666f  ex:ancestor_info
+000152a0: 5f64 6963 745b 6e6f 6465 5d20 666f 7220  _dict[node] for 
+000152b0: 696e 6465 782c 6e6f 6465 2069 6e20 656e  index,node in en
+000152c0: 756d 6572 6174 6528 6c65 7665 6c5f 6e6f  umerate(level_no
+000152d0: 6465 7329 7d20 2366 696e 6420 7468 6520  des)} #find the 
+000152e0: 696e 6465 7865 7320 6f66 2074 6865 206e  indexes of the n
+000152f0: 6f64 6573 2073 6861 7269 6e67 2074 6865  odes sharing the
+00015300: 2073 616d 6520 616e 6365 7374 6f72 730a   same ancestors.
+00015310: 2020 2020 2020 2020 6966 206e 702e 6e61          if np.na
+00015320: 6e20 696e 2061 6c6c 5f61 6e63 6573 746f  n in all_ancesto
+00015330: 7273 5f69 6e5f 6c65 7665 6c2e 7661 6c75  rs_in_level.valu
+00015340: 6573 2829 3a23 6964 656e 7469 6679 2072  es():#identify r
+00015350: 6f6f 742c 2062 6563 6175 7365 2069 7420  oot, because it 
+00015360: 6861 7320 6e61 6e20 6173 2061 6e20 616e  has nan as an an
+00015370: 6365 7374 6f72 0a20 2020 2020 2020 2020  cestor.         
+00015380: 2020 206e 6f64 6573 5f72 6570 7265 7365     nodes_represe
+00015390: 6e74 6174 696f 6e73 5b6c 6576 656c 5f6e  ntations[level_n
+000153a0: 6f64 6573 5b30 5d5d 203d 206e 6f64 655f  odes[0]] = node_
+000153b0: 7265 7072 6573 656e 7461 7469 6f6e 0a20  representation. 
+000153c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000153d0: 2020 2020 2020 2020 206e 6f64 655f 7265           node_re
+000153e0: 7072 6573 656e 7461 7469 6f6e 203d 206e  presentation = n
+000153f0: 6f64 655f 7265 7072 6573 656e 7461 7469  ode_representati
+00015400: 6f6e 5b3a 2d64 6567 7265 655f 7472 6565  on[:-degree_tree
+00015410: 5d0a 2020 2020 2020 2020 2020 2020 6c65  ].            le
+00015420: 7665 6c5f 7061 6972 7320 3d20 5b6c 6576  vel_pairs = [lev
+00015430: 656c 5f6e 6f64 6573 5b69 3a69 202b 2064  el_nodes[i:i + d
+00015440: 6567 7265 655f 7472 6565 5d20 666f 7220  egree_tree] for 
+00015450: 6920 696e 2072 616e 6765 2830 2c20 6c65  i in range(0, le
+00015460: 6e28 6c65 7665 6c5f 6e6f 6465 7329 2c20  n(level_nodes), 
+00015470: 6465 6772 6565 5f74 7265 6529 5d20 2344  degree_tree)] #D
+00015480: 6976 6964 6520 6c65 7665 6c20 696e 2067  ivide level in g
+00015490: 726f 7570 7320 6f66 2032 2c20 7468 6520  roups of 2, the 
+000154a0: 7472 6565 2069 7320 696e 2074 7265 6520  tree is in tree 
+000154b0: 7472 6176 6572 7361 6c2c 2073 6f20 6576  traversal, so ev
+000154c0: 6572 7974 6869 6e67 2073 686f 7564 6c20  erything shoudl 
+000154d0: 6265 206f 7264 6572 6564 0a20 2020 2020  be ordered.     
+000154e0: 2020 2020 2020 2066 6f72 206c 6576 656c         for level
+000154f0: 5f70 6169 7220 696e 206c 6576 656c 5f70  _pair in level_p
+00015500: 6169 7273 3a20 2374 6865 7365 2070 6169  airs: #these pai
+00015510: 7273 2068 6176 6520 7361 6d65 2061 6e63  rs have same anc
+00015520: 6573 746f 7220 6265 6361 7573 6520 6f66  estor because of
+00015530: 2074 7265 6520 6c65 7665 6c73 2061 7265   tree levels are
+00015540: 206f 7267 616e 697a 6564 2069 6e20 7472   organized in tr
+00015550: 6176 6572 7361 6c20 6f72 6465 720a 2020  aversal order.  
+00015560: 2020 2020 2020 2020 2020 2020 2020 2367                #g
+00015570: 6574 2074 6865 2061 6e63 6573 746f 7220  et the ancestor 
+00015580: 6e6f 6465 2072 6570 7265 7365 6e74 6174  node representat
+00015590: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000155a0: 2020 2020 616e 6365 7374 6f72 203d 2061      ancestor = a
+000155b0: 6e63 6573 746f 725f 696e 666f 5f64 6963  ncestor_info_dic
+000155c0: 745b 6c65 7665 6c5f 7061 6972 5b30 5d5d  t[level_pair[0]]
+000155d0: 2023 6a75 7374 2075 7365 206f 6e65 206f   #just use one o
+000155e0: 6620 7468 656d 2074 6f20 6765 7420 7468  f them to get th
+000155f0: 6520 616e 6365 7374 6f72 0a20 2020 2020  e ancestor.     
+00015600: 2020 2020 2020 2020 2020 206e 6f64 655f             node_
+00015610: 7265 7072 6573 656e 7461 7469 6f6e 203d  representation =
+00015620: 206e 6f64 6573 5f72 6570 7265 7365 6e74   nodes_represent
+00015630: 6174 696f 6e73 5b61 6e63 6573 746f 725d  ations[ancestor]
+00015640: 5b3a 2d64 6567 7265 655f 7472 6565 5d0a  [:-degree_tree].
+00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015660: 6164 6465 645f 7265 7072 6573 656e 7461  added_representa
+00015670: 7469 6f6e 203d 5b30 5d2a 320a 2020 2020  tion =[0]*2.    
+00015680: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00015690: 696e 6465 782c 6e6f 6465 2069 6e20 656e  index,node in en
+000156a0: 756d 6572 6174 6528 6c65 7665 6c5f 7061  umerate(level_pa
+000156b0: 6972 293a 0a20 2020 2020 2020 2020 2020  ir):.           
+000156c0: 2020 2020 2020 2020 2061 6464 6564 5f72           added_r
+000156d0: 6570 7265 7365 6e74 6174 696f 6e5b 696e  epresentation[in
+000156e0: 6465 785d 203d 310a 2020 2020 2020 2020  dex] =1.        
+000156f0: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+00015700: 5f72 6570 7265 7365 6e74 6174 696f 6e20  _representation 
+00015710: 3d20 6164 6465 645f 7265 7072 6573 656e  = added_represen
+00015720: 7461 7469 6f6e 202b 206e 6f64 655f 7265  tation + node_re
+00015730: 7072 6573 656e 7461 7469 6f6e 0a20 2020  presentation.   
+00015740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015750: 206e 6f64 6573 5f72 6570 7265 7365 6e74   nodes_represent
+00015760: 6174 696f 6e73 5b6e 6f64 655d 203d 206e  ations[node] = n
+00015770: 6f64 655f 7265 7072 6573 656e 7461 7469  ode_representati
+00015780: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00015790: 2020 2020 2020 2061 6464 6564 5f72 6570         added_rep
+000157a0: 7265 7365 6e74 6174 696f 6e20 3d20 5b30  resentation = [0
+000157b0: 5d20 2a20 3220 2372 6573 7461 7274 0a20  ] * 2 #restart. 
+000157c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157d0: 2020 206e 6f64 655f 7265 7072 6573 656e     node_represen
+000157e0: 7461 7469 6f6e 203d 206e 6f64 6573 5f72  tation = nodes_r
+000157f0: 6570 7265 7365 6e74 6174 696f 6e73 5b61  epresentations[a
+00015800: 6e63 6573 746f 725d 5b3a 2d64 6567 7265  ncestor][:-degre
+00015810: 655f 7472 6565 5d20 2372 6573 7461 7274  e_tree] #restart
+00015820: 0a20 2020 206e 6f64 6573 5f72 6570 7265  .    nodes_repre
+00015830: 7365 6e74 6174 696f 6e73 5f61 7272 6179  sentations_array
+00015840: 203d 206e 702e 7673 7461 636b 286c 6973   = np.vstack(lis
+00015850: 7428 6e6f 6465 735f 7265 7072 6573 656e  t(nodes_represen
+00015860: 7461 7469 6f6e 732e 7661 6c75 6573 2829  tations.values()
+00015870: 2929 0a20 2020 206e 6f64 6573 5f72 6570  )).    nodes_rep
+00015880: 7265 7365 6e74 6174 696f 6e73 5f61 7272  resentations_arr
+00015890: 6179 203d 206e 702e 635f 5b20 6e70 2e61  ay = np.c_[ np.a
+000158a0: 7272 6179 286c 6973 7428 6e6f 6465 735f  rray(list(nodes_
+000158b0: 7265 7072 6573 656e 7461 7469 6f6e 732e  representations.
+000158c0: 6b65 7973 2829 2929 5b3a 2c4e 6f6e 655d  keys()))[:,None]
+000158d0: 2c20 6e6f 6465 735f 7265 7072 6573 656e  , nodes_represen
+000158e0: 7461 7469 6f6e 735f 6172 7261 795d 0a20  tations_array]. 
+000158f0: 2020 2072 6574 7572 6e20 6e6f 6465 735f     return nodes_
+00015900: 7265 7072 6573 656e 7461 7469 6f6e 735f  representations_
+00015910: 6172 7261 790a 6465 6620 6578 7472 615f  array.def extra_
+00015920: 7072 6f63 6573 7369 6e67 2861 6e63 6573  processing(ances
+00015930: 746f 725f 696e 666f 2c70 6174 7269 7374  tor_info,patrist
+00015940: 6963 5f6d 6174 7269 782c 7265 7375 6c74  ic_matrix,result
+00015950: 735f 6469 722c 6172 6773 2c62 7569 6c64  s_dir,args,build
+00015960: 5f63 6f6e 6669 6729 3a0a 2020 2020 2222  _config):.    ""
+00015970: 2243 6f6d 7075 7465 7320 736f 6d65 2064  "Computes some d
+00015980: 6963 7469 6f6e 6172 6965 7320 7769 7468  ictionaries with
+00015990: 2074 6865 206e 6f64 6573 206f 7264 6572   the nodes order
+000159a0: 6564 2069 6e20 7472 6565 206c 6576 656c  ed in tree level
+000159b0: 206f 7264 6572 2c20 7072 6f63 6573 7365   order, processe
+000159c0: 7320 7468 6520 626c 6f73 756d 206d 6174  s the blosum mat
+000159d0: 7269 7820 616e 6420 6275 696c 6420 6120  rix and build a 
+000159e0: 6772 6170 6820 7769 7468 2074 6865 2074  graph with the t
+000159f0: 7265 6520 6e6f 6465 7320 616e 6420 7468  ree nodes and th
+00015a00: 6520 6272 616e 6368 206c 656e 6774 6873  e branch lengths
+00015a10: 2061 7320 6564 6765 730a 2020 2020 203a   as edges.     :
+00015a20: 7061 7261 6d20 6e61 6d65 6474 7570 6c65  param namedtuple
+00015a30: 2061 6e63 6573 746f 725f 696e 666f 0a20   ancestor_info. 
+00015a40: 2020 2020 3a70 6172 616d 2074 656e 736f      :param tenso
+00015a50: 7220 7061 7472 6973 7469 635f 6d61 7472  r patristic_matr
+00015a60: 6978 3a20 5b6e 5f6c 6561 7665 7320 2b20  ix: [n_leaves + 
+00015a70: 6e5f 696e 7465 726e 616c 202b 2031 2c20  n_internal + 1, 
+00015a80: 6e5f 6c65 6176 6573 202b 206e 5f69 6e74  n_leaves + n_int
+00015a90: 6572 6e61 6c20 2b20 315d 0a20 2020 2020  ernal + 1].     
+00015aa0: 3a70 6172 616d 2073 7472 2072 6573 756c  :param str resul
+00015ab0: 7473 5f64 6972 0a20 2020 2020 3a70 6172  ts_dir.     :par
+00015ac0: 616d 206e 616d 6564 7475 706c 6520 6172  am namedtuple ar
+00015ad0: 6773 0a20 2020 2020 3a70 6172 616d 206e  gs.     :param n
+00015ae0: 616d 6564 7475 706c 6520 6275 696c 645f  amedtuple build_
+00015af0: 636f 6e66 6967 2222 220a 2020 2020 4164  config""".    Ad
+00015b00: 6469 7469 6f6e 616c 496e 666f 203d 206e  ditionalInfo = n
+00015b10: 616d 6564 7475 706c 6528 2241 6464 6974  amedtuple("Addit
+00015b20: 696f 6e61 6c49 6e66 6f22 2c0a 2020 2020  ionalInfo",.    
 00015b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b40: 2020 5b22 626c 6f73 756d 2220 2c22 626c    ["blosum" ,"bl
-00015b50: 6f73 756d 5f64 6963 7422 2c22 6368 696c  osum_dict","chil
-00015b60: 6472 656e 5f64 6963 7422 2c22 616e 6365  dren_dict","ance
-00015b70: 7374 6f72 5f69 6e66 6f5f 6469 6374 222c  stor_info_dict",
-00015b80: 2022 7472 6565 5f62 795f 6c65 7665 6c73   "tree_by_levels
-00015b90: 5f64 6963 7422 2c20 2274 7265 655f 6279  _dict", "tree_by
-00015ba0: 5f6c 6576 656c 735f 6172 7261 7922 2c0a  _levels_array",.
-00015bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015bc0: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-00015bd0: 7472 6973 7469 635f 696e 666f 222c 2022  tristic_info", "
-00015be0: 6772 6170 685f 636f 6f22 2c22 7061 7472  graph_coo","patr
-00015bf0: 6973 7469 635f 6675 6c6c 5f73 7061 7273  istic_full_spars
-00015c00: 6522 2c22 6e6f 6465 735f 7265 7072 6573  e","nodes_repres
-00015c10: 656e 7461 7469 6f6e 735f 6172 7261 7922  entations_array"
-00015c20: 2c22 6467 6c5f 6772 6170 6822 5d29 0a0a  ,"dgl_graph"])..
-00015c30: 2020 2020 616e 6365 7374 6f72 5f69 6e66      ancestor_inf
-00015c40: 6f5f 6469 6374 203d 2064 6963 7428 7a69  o_dict = dict(zi
-00015c50: 7028 616e 6365 7374 6f72 5f69 6e66 6f5b  p(ancestor_info[
-00015c60: 3a2c 305d 2e74 6f6c 6973 7428 292c 616e  :,0].tolist(),an
-00015c70: 6365 7374 6f72 5f69 6e66 6f5b 3a2c 325d  cestor_info[:,2]
-00015c80: 2e74 6f6c 6973 7428 2929 290a 2020 2020  .tolist())).    
-00015c90: 7069 636b 6c65 2e64 756d 7028 616e 6365  pickle.dump(ance
-00015ca0: 7374 6f72 5f69 6e66 6f5f 6469 6374 2c20  stor_info_dict, 
-00015cb0: 6f70 656e 2827 7b7d 2f41 6e63 6573 746f  open('{}/Ancesto
-00015cc0: 725f 696e 666f 5f64 6963 742e 7027 2e66  r_info_dict.p'.f
-00015cd0: 6f72 6d61 7428 7265 7375 6c74 735f 6469  ormat(results_di
-00015ce0: 7229 2c20 2777 6227 292c 2070 726f 746f  r), 'wb'), proto
-00015cf0: 636f 6c3d 7069 636b 6c65 2e48 4947 4845  col=pickle.HIGHE
-00015d00: 5354 5f50 524f 544f 434f 4c29 0a20 2020  ST_PROTOCOL).   
-00015d10: 2069 6620 6973 696e 7374 616e 6365 2870   if isinstance(p
-00015d20: 6174 7269 7374 6963 5f6d 6174 7269 782c  atristic_matrix,
-00015d30: 6e70 2e6e 6461 7272 6179 293a 0a20 2020  np.ndarray):.   
-00015d40: 2020 2020 2070 6174 7269 7374 6963 5f69       patristic_i
-00015d50: 6e66 6f20 3d20 6469 6374 287a 6970 286c  nfo = dict(zip(l
-00015d60: 6973 7428 7261 6e67 6528 6c65 6e28 7061  ist(range(len(pa
-00015d70: 7472 6973 7469 635f 6d61 7472 6978 292d  tristic_matrix)-
-00015d80: 3129 292c 7061 7472 6973 7469 635f 6d61  1)),patristic_ma
-00015d90: 7472 6978 5b31 3a2c 305d 2e61 7374 7970  trix[1:,0].astyp
-00015da0: 6528 696e 7429 2e74 6f6c 6973 7428 2929  e(int).tolist())
-00015db0: 2920 2353 6b69 7020 7468 6520 6661 6b65  ) #Skip the fake
-00015dc0: 2068 6561 6465 720a 2020 2020 656c 7365   header.    else
-00015dd0: 3a0a 0a20 2020 2020 2020 2070 6174 7269  :..        patri
-00015de0: 7374 6963 5f69 6e66 6f20 3d64 6963 7428  stic_info =dict(
-00015df0: 7a69 7028 6c69 7374 2872 616e 6765 286c  zip(list(range(l
-00015e00: 656e 2870 6174 7269 7374 6963 5f6d 6174  en(patristic_mat
-00015e10: 7269 7829 2d31 2929 2c70 6174 7269 7374  rix)-1)),patrist
-00015e20: 6963 5f6d 6174 7269 785b 313a 2c30 5d2e  ic_matrix[1:,0].
-00015e30: 7479 7065 2874 6f72 6368 2e69 6e74 292e  type(torch.int).
-00015e40: 746f 6c69 7374 2829 2929 0a0a 2020 2020  tolist()))..    
-00015e50: 616e 6365 7374 6f72 735f 696e 666f 5f66  ancestors_info_f
-00015e60: 6c69 7070 6564 203d 206e 702e 666c 6970  lipped = np.flip
-00015e70: 2861 6e63 6573 746f 725f 696e 666f 2c20  (ancestor_info, 
-00015e80: 6178 6973 3d31 2920 2353 6f20 7765 2063  axis=1) #So we c
-00015e90: 616e 2065 7661 6c75 6174 6520 696e 2072  an evaluate in r
-00015ea0: 6576 6572 7365 2c20 7765 2073 7461 7274  everse, we start
-00015eb0: 2077 6974 6820 7468 6520 6c61 7374 2063   with the last c
-00015ec0: 6f6c 756d 6e0a 0a20 2020 2074 7265 655f  olumn..    tree_
-00015ed0: 6279 5f6c 6576 656c 7320 3d20 5b5d 0a20  by_levels = []. 
-00015ee0: 2020 2066 6f72 2063 6f6c 756d 6e20 696e     for column in
-00015ef0: 2061 6e63 6573 746f 7273 5f69 6e66 6f5f   ancestors_info_
-00015f00: 666c 6970 7065 642e 543a 0a20 2020 2020  flipped.T:.     
-00015f10: 2020 2069 6e64 6578 6573 203d 206e 702e     indexes = np.
-00015f20: 7768 6572 6528 636f 6c75 6d6e 203d 3d20  where(column == 
-00015f30: 3029 0a20 2020 2020 2020 206c 6576 656c  0).        level
-00015f40: 203d 2061 6e63 6573 746f 7273 5f69 6e66   = ancestors_inf
-00015f50: 6f5f 666c 6970 7065 642e 545b 2d31 5d5b  o_flipped.T[-1][
-00015f60: 696e 6465 7865 735d 0a20 2020 2020 2020  indexes].       
-00015f70: 2074 7265 655f 6279 5f6c 6576 656c 732e   tree_by_levels.
-00015f80: 6170 7065 6e64 286c 6576 656c 290a 0a20  append(level).. 
-00015f90: 2020 2074 7265 655f 6279 5f6c 6576 656c     tree_by_level
-00015fa0: 7320 3d20 7472 6565 5f62 795f 6c65 7665  s = tree_by_leve
-00015fb0: 6c73 5b3a 2d31 5d20 2374 6865 2072 6f6f  ls[:-1] #the roo
-00015fc0: 7420 6765 7473 2061 6464 6564 2074 7769  t gets added twi
-00015fd0: 6365 2062 6563 6175 7365 2074 6865 2066  ce because the f
-00015fe0: 6972 7374 2063 6f6c 756d 6e20 6172 6520  irst column are 
-00015ff0: 7468 6520 6e6f 6465 2069 6e64 6578 6573  the node indexes
-00016000: 2c20 6361 6e6e 6f74 2062 6520 6669 7865  , cannot be fixe
-00016010: 642c 206f 7468 6572 7769 7365 2077 6520  d, otherwise we 
-00016020: 6361 6e6e 6f74 2064 6f20 7468 6520 7472  cannot do the tr
-00016030: 6963 6b0a 0a20 2020 2074 7265 655f 6279  ick..    tree_by
-00016040: 5f6c 6576 656c 735f 6469 6374 203d 2064  _levels_dict = d
-00016050: 6963 7428 7a69 7028 6c69 7374 2872 6576  ict(zip(list(rev
-00016060: 6572 7365 6428 7261 6e67 6528 6c65 6e28  ersed(range(len(
-00016070: 7472 6565 5f62 795f 6c65 7665 6c73 2929  tree_by_levels))
-00016080: 2929 2c74 7265 655f 6279 5f6c 6576 656c  )),tree_by_level
-00016090: 7329 290a 2020 2020 7069 636b 6c65 2e64  s)).    pickle.d
-000160a0: 756d 7028 7472 6565 5f62 795f 6c65 7665  ump(tree_by_leve
-000160b0: 6c73 5f64 6963 742c 206f 7065 6e28 277b  ls_dict, open('{
-000160c0: 7d2f 5472 6565 5f62 795f 6c65 7665 6c73  }/Tree_by_levels
-000160d0: 5f64 6963 742e 7027 2e66 6f72 6d61 7428  _dict.p'.format(
-000160e0: 7265 7375 6c74 735f 6469 7229 2c20 2777  results_dir), 'w
-000160f0: 6227 292c 2070 726f 746f 636f 6c3d 7069  b'), protocol=pi
-00016100: 636b 6c65 2e48 4947 4845 5354 5f50 524f  ckle.HIGHEST_PRO
-00016110: 544f 434f 4c29 0a0a 2020 2020 6c65 6e67  TOCOL)..    leng
-00016120: 7468 203d 206d 6178 286d 6170 286c 656e  th = max(map(len
-00016130: 2c20 7472 6565 5f62 795f 6c65 7665 6c73  , tree_by_levels
-00016140: 5f64 6963 742e 7661 6c75 6573 2829 2929  _dict.values()))
-00016150: 0a20 2020 2074 7265 655f 6279 5f6c 6576  .    tree_by_lev
-00016160: 656c 735f 6172 7261 7920 3d20 6e70 2e61  els_array = np.a
-00016170: 7272 6179 285b 7869 2e74 6f6c 6973 7428  rray([xi.tolist(
-00016180: 2920 2b20 5b4e 6f6e 655d 202a 2028 6c65  ) + [None] * (le
-00016190: 6e67 7468 202d 206c 656e 2878 6929 2920  ngth - len(xi)) 
-000161a0: 666f 7220 7869 2069 6e20 7472 6565 5f62  for xi in tree_b
-000161b0: 795f 6c65 7665 6c73 5d29 0a20 2020 2023  y_levels]).    #
-000161c0: 2074 7265 655f 6c65 7665 6c73 5f32 203d   tree_levels_2 =
-000161d0: 2043 7265 6174 655f 7472 6565 5f62 795f   Create_tree_by_
-000161e0: 6c65 7665 6c73 2863 6869 6c64 7265 6e5f  levels(children_
-000161f0: 6469 6374 290a 0a20 2020 2063 6869 6c64  dict)..    child
-00016200: 7265 6e5f 6469 6374 203d 207b 7d0a 2020  ren_dict = {}.  
-00016210: 2020 666f 7220 6b2c 2076 2069 6e20 616e    for k, v in an
-00016220: 6365 7374 6f72 5f69 6e66 6f5f 6469 6374  cestor_info_dict
-00016230: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00016240: 2020 6368 696c 6472 656e 5f64 6963 745b    children_dict[
-00016250: 765d 203d 2063 6869 6c64 7265 6e5f 6469  v] = children_di
-00016260: 6374 2e67 6574 2876 2c20 5b5d 290a 2020  ct.get(v, []).  
-00016270: 2020 2020 2020 6368 696c 6472 656e 5f64        children_d
-00016280: 6963 745b 765d 2e61 7070 656e 6428 6b29  ict[v].append(k)
-00016290: 0a20 2020 2070 6963 6b6c 652e 6475 6d70  .    pickle.dump
-000162a0: 2863 6869 6c64 7265 6e5f 6469 6374 2c20  (children_dict, 
-000162b0: 6f70 656e 2827 7b7d 2f43 6869 6c64 7265  open('{}/Childre
-000162c0: 6e5f 6469 6374 2e70 272e 666f 726d 6174  n_dict.p'.format
-000162d0: 2872 6573 756c 7473 5f64 6972 292c 2027  (results_dir), '
-000162e0: 7762 2729 2c0a 2020 2020 2020 2020 2020  wb'),.          
-000162f0: 2020 2020 2020 7072 6f74 6f63 6f6c 3d70        protocol=p
-00016300: 6963 6b6c 652e 4849 4748 4553 545f 5052  ickle.HIGHEST_PR
-00016310: 4f54 4f43 4f4c 290a 0a20 2020 2023 2268  OTOCOL)..    #"h
-00016320: 7474 7073 3a2f 2f70 7974 6f72 6368 2d67  ttps://pytorch-g
-00016330: 656f 6d65 7472 6963 2e72 6561 6474 6865  eometric.readthe
-00016340: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00016350: 742f 6e6f 7465 732f 696e 7472 6f64 7563  t/notes/introduc
-00016360: 7469 6f6e 2e68 746d 6c22 0a20 2020 2023  tion.html".    #
-00016370: 4869 6768 6c69 6768 743a 4275 696c 6420  Highlight:Build 
-00016380: 7468 6520 6d61 7472 6978 2072 6570 7265  the matrix repre
-00016390: 7365 6e74 6174 696f 6e20 6f66 2074 6865  sentation of the
-000163a0: 2074 7265 6520 6772 6170 683a 2044 6972   tree graph: Dir
-000163b0: 6563 7465 6420 2872 6f6f 742d 3e20 6c65  ected (root-> le
-000163c0: 6176 6573 2920 7765 6967 6874 6564 2028  aves) weighted (
-000163d0: 7061 7472 6973 7469 6320 6469 7374 2920  patristic dist) 
-000163e0: 6772 6170 680a 2020 2020 6966 2062 7569  graph.    if bui
-000163f0: 6c64 5f63 6f6e 6669 672e 6275 696c 645f  ld_config.build_
-00016400: 6772 6170 683a 2023 544f 444f 3a20 4669  graph: #TODO: Fi
-00016410: 7820 696e 2073 6572 7665 720a 2020 2020  x in server.    
-00016420: 2020 2020 7072 696e 7428 2242 7569 6c64      print("Build
-00016430: 696e 6720 6120 7472 6565 2d67 7261 7068  ing a tree-graph
-00016440: 2229 0a20 2020 2020 2020 2023 6d61 6b65  ").        #make
-00016450: 2067 7261 7068 2061 646a 6163 656e 7420   graph adjacent 
-00016460: 6d61 7472 6978 0a20 2020 2020 2020 2070  matrix.        p
-00016470: 6174 7269 7374 6963 5f6d 6174 7269 7820  atristic_matrix 
-00016480: 3d20 7061 7472 6973 7469 635f 6d61 7472  = patristic_matr
-00016490: 6978 5b70 6174 7269 7374 6963 5f6d 6174  ix[patristic_mat
-000164a0: 7269 785b 3a2c 2030 5d2e 6172 6773 6f72  rix[:, 0].argsor
-000164b0: 7428 295d 0a20 2020 2020 2020 2070 6174  t()].        pat
-000164c0: 7269 7374 6963 5f6d 6174 7269 7820 3d20  ristic_matrix = 
-000164d0: 7061 7472 6973 7469 635f 6d61 7472 6978  patristic_matrix
-000164e0: 5b3a 2c20 7061 7472 6973 7469 635f 6d61  [:, patristic_ma
-000164f0: 7472 6978 5b30 2c20 3a5d 2e61 7267 736f  trix[0, :].argso
-00016500: 7274 2829 5d0a 0a20 2020 2020 2020 2067  rt()]..        g
-00016510: 7261 7068 5f6e 6f64 655f 6d61 7472 6978  raph_node_matrix
-00016520: 203d 206e 702e 7a65 726f 735f 6c69 6b65   = np.zeros_like
-00016530: 2870 6174 7269 7374 6963 5f6d 6174 7269  (patristic_matri
-00016540: 7829 2023 4469 7265 6374 6564 2028 726f  x) #Directed (ro
-00016550: 6f74 2d3e 206c 6561 7665 7329 204e 4f54  ot-> leaves) NOT
-00016560: 2077 6569 6768 7465 6420 6772 6170 680a   weighted graph.
-00016570: 2020 2020 2020 2020 6564 6765 5f77 6569          edge_wei
-00016580: 6768 745f 6d61 7472 6978 203d 206e 702e  ght_matrix = np.
-00016590: 7a65 726f 735f 6c69 6b65 2870 6174 7269  zeros_like(patri
-000165a0: 7374 6963 5f6d 6174 7269 7829 2023 4469  stic_matrix) #Di
-000165b0: 7265 6374 6564 2028 726f 6f74 2d3e 206c  rected (root-> l
-000165c0: 6561 7665 7329 2077 6569 6768 7465 6420  eaves) weighted 
-000165d0: 2870 6174 7269 7374 6963 2064 6973 7429  (patristic dist)
-000165e0: 2067 7261 7068 0a20 2020 2020 2020 2067   graph.        g
-000165f0: 7261 7068 5f6e 6f64 655f 6d61 7472 6978  raph_node_matrix
-00016600: 5b30 2c3a 5d20 3d20 7061 7472 6973 7469  [0,:] = patristi
-00016610: 635f 6d61 7472 6978 5b30 2c3a 5d0a 2020  c_matrix[0,:].  
-00016620: 2020 2020 2020 6772 6170 685f 6e6f 6465        graph_node
-00016630: 5f6d 6174 7269 785b 3a2c 305d 203d 2070  _matrix[:,0] = p
-00016640: 6174 7269 7374 6963 5f6d 6174 7269 785b  atristic_matrix[
-00016650: 3a2c 305d 0a20 2020 2020 2020 2065 6467  :,0].        edg
-00016660: 655f 7765 6967 6874 5f6d 6174 7269 785b  e_weight_matrix[
-00016670: 302c 203a 5d20 3d20 7061 7472 6973 7469  0, :] = patristi
-00016680: 635f 6d61 7472 6978 5b30 2c20 3a5d 0a20  c_matrix[0, :]. 
-00016690: 2020 2020 2020 2065 6467 655f 7765 6967         edge_weig
-000166a0: 6874 5f6d 6174 7269 785b 3a2c 2030 5d20  ht_matrix[:, 0] 
-000166b0: 3d20 7061 7472 6973 7469 635f 6d61 7472  = patristic_matr
-000166c0: 6978 5b3a 2c20 305d 0a20 2020 2020 2020  ix[:, 0].       
-000166d0: 2066 6f72 2061 6e63 6573 746f 722c 6368   for ancestor,ch
-000166e0: 696c 6472 656e 2069 6e20 6368 696c 6472  ildren in childr
-000166f0: 656e 5f64 6963 742e 6974 656d 7328 293a  en_dict.items():
-00016700: 0a20 2020 2020 2020 2020 2020 2061 6e63  .            anc
-00016710: 6573 746f 725f 6964 7820 3d20 6e70 2e69  estor_idx = np.i
-00016720: 6e31 6428 6772 6170 685f 6e6f 6465 5f6d  n1d(graph_node_m
-00016730: 6174 7269 785b 302c 3a5d 2c20 616e 6365  atrix[0,:], ance
-00016740: 7374 6f72 292e 6e6f 6e7a 6572 6f28 295b  stor).nonzero()[
-00016750: 305d 0a20 2020 2020 2020 2020 2020 2063  0].            c
-00016760: 6869 6c64 7265 6e5f 6964 783d 206e 702e  hildren_idx= np.
-00016770: 696e 3164 2867 7261 7068 5f6e 6f64 655f  in1d(graph_node_
-00016780: 6d61 7472 6978 5b30 2c3a 5d2c 2063 6869  matrix[0,:], chi
-00016790: 6c64 7265 6e29 2e6e 6f6e 7a65 726f 2829  ldren).nonzero()
-000167a0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-000167b0: 6772 6170 685f 6e6f 6465 5f6d 6174 7269  graph_node_matri
-000167c0: 785b 616e 6365 7374 6f72 5f69 6478 2c63  x[ancestor_idx,c
-000167d0: 6869 6c64 7265 6e5f 6964 785d 203d 2031  hildren_idx] = 1
-000167e0: 2023 636f 6e74 6169 6e73 206e 6f20 6564   #contains no ed
-000167f0: 6765 7320 7765 6967 6874 730a 2020 2020  ges weights.    
-00016800: 2020 2020 2020 2020 6772 6170 685f 6e6f          graph_no
-00016810: 6465 5f6d 6174 7269 785b 6368 696c 6472  de_matrix[childr
-00016820: 656e 5f69 6478 2c61 6e63 6573 746f 725f  en_idx,ancestor_
-00016830: 6964 785d 203d 2031 0a20 2020 2020 2020  idx] = 1.       
-00016840: 2020 2020 2065 6467 655f 7765 6967 6874       edge_weight
-00016850: 5f6d 6174 7269 785b 616e 6365 7374 6f72  _matrix[ancestor
-00016860: 5f69 6478 2c20 6368 696c 6472 656e 5f69  _idx, children_i
-00016870: 6478 5d20 3d20 7061 7472 6973 7469 635f  dx] = patristic_
-00016880: 6d61 7472 6978 5b61 6e63 6573 746f 725f  matrix[ancestor_
-00016890: 6964 782c 2063 6869 6c64 7265 6e5f 6964  idx, children_id
-000168a0: 785d 0a20 2020 2020 2020 2020 2020 2023  x].            #
-000168b0: 6564 6765 5f77 6569 6768 745f 6d61 7472  edge_weight_matr
-000168c0: 6978 5b63 6869 6c64 7265 6e5f 6964 782c  ix[children_idx,
-000168d0: 2061 6e63 6573 746f 725f 6964 785d 203d   ancestor_idx] =
-000168e0: 2070 6174 7269 7374 6963 5f6d 6174 7269   patristic_matri
-000168f0: 785b 6368 696c 6472 656e 5f69 6478 2c20  x[children_idx, 
-00016900: 616e 6365 7374 6f72 5f69 6478 5d20 2348  ancestor_idx] #H
-00016910: 6967 686c 6967 6874 3a20 4e6f 7420 7573  ighlight: Not us
-00016920: 6520 746f 2061 766f 6964 2063 7265 6174  e to avoid creat
-00016930: 696e 6720 6120 7365 6c66 206c 6f6f 7065  ing a self loope
-00016940: 6420 6772 6170 6820 6f72 2062 6964 6972  d graph or bidir
-00016950: 6563 7469 6f6e 616c 2067 7261 7068 730a  ectional graphs.
-00016960: 2020 2020 2020 2020 2343 7265 6174 6520          #Create 
-00016970: 6120 636f 6f72 6469 6e61 7465 7320 6d61  a coordinates ma
-00016980: 7472 6978 2c20 6261 7369 6361 6c6c 7920  trix, basically 
-00016990: 706f 696e 7473 206f 7574 2077 6869 6368  points out which
-000169a0: 2072 6567 696f 6e73 2066 726f 6d20 7468   regions from th
-000169b0: 6520 6d61 7472 6978 2064 6f20 6e6f 7420  e matrix do not 
-000169c0: 6861 7665 2030 2076 616c 7565 7320 616e  have 0 values an
-000169d0: 6420 7468 6572 6566 6f72 6520 6172 6520  d therefore are 
-000169e0: 636f 6e6e 6563 7465 640a 2020 2020 2020  connected.      
-000169f0: 2020 7765 6967 6874 735f 636f 6f20 3d20    weights_coo = 
-00016a00: 636f 6f5f 6d61 7472 6978 2865 6467 655f  coo_matrix(edge_
-00016a10: 7765 6967 6874 5f6d 6174 7269 785b 313a  weight_matrix[1:
-00016a20: 2c31 3a5d 290a 2020 2020 2020 2020 7472  ,1:]).        tr
-00016a30: 793a 0a20 2020 2020 2020 2020 2020 2023  y:.            #
-00016a40: 5468 6520 6772 6170 6820 636f 6e6e 6563  The graph connec
-00016a50: 7469 7669 7479 2028 6564 6765 2069 6e64  tivity (edge ind
-00016a60: 6578 2920 7368 6f75 6c64 2062 6520 636f  ex) should be co
-00016a70: 6e66 696e 6564 2077 6974 6820 7468 6520  nfined with the 
-00016a80: 434f 4f20 666f 726d 6174 2c0a 2020 2020  COO format,.    
-00016a90: 2020 2020 2020 2020 2320 692e 652e 2074          # i.e. t
-00016aa0: 6865 2066 6972 7374 206c 6973 7420 636f  he first list co
-00016ab0: 6e74 6169 6e73 2074 6865 2069 6e64 6578  ntains the index
-00016ac0: 206f 6620 7468 6520 736f 7572 6365 206e   of the source n
-00016ad0: 6f64 6573 2c20 7768 696c 6520 7468 6520  odes, while the 
-00016ae0: 696e 6465 7820 6f66 2074 6172 6765 7420  index of target 
-00016af0: 6e6f 6465 7320 6973 2073 7065 6369 6669  nodes is specifi
-00016b00: 6564 2069 6e20 7468 6520 7365 636f 6e64  ed in the second
-00016b10: 206c 6973 742e 0a20 2020 2020 2020 2020   list..         
-00016b20: 2020 2023 4e6f 7465 2074 6861 7420 7468     #Note that th
-00016b30: 6520 6f72 6465 7220 6f66 2074 6865 2065  e order of the e
-00016b40: 6467 6520 696e 6465 7820 6973 2069 7272  dge index is irr
-00016b50: 656c 6576 616e 7420 746f 2074 6865 2044  elevant to the D
-00016b60: 6174 6120 6f62 6a65 6374 2079 6f75 2063  ata object you c
-00016b70: 7265 6174 6520 7369 6e63 6520 7375 6368  reate since such
-00016b80: 2069 6e66 6f72 6d61 7469 6f6e 2069 7320   information is 
-00016b90: 6f6e 6c79 2066 6f72 2063 6f6d 7075 7469  only for computi
-00016ba0: 6e67 2074 6865 2061 646a 6163 656e 6379  ng the adjacency
-00016bb0: 206d 6174 7269 782e 0a20 2020 2020 2020   matrix..       
-00016bc0: 2020 2020 2066 726f 6d20 746f 7263 685f       from torch_
-00016bd0: 6765 6f6d 6574 7269 632e 7574 696c 732e  geometric.utils.
-00016be0: 636f 6e76 6572 7420 696d 706f 7274 2066  convert import f
-00016bf0: 726f 6d5f 7363 6970 795f 7370 6172 7365  rom_scipy_sparse
-00016c00: 5f6d 6174 7269 780a 2020 2020 2020 2020  _matrix.        
-00016c10: 2020 2020 6564 6765 5f69 6e64 6578 2c65      edge_index,e
-00016c20: 6467 655f 7765 6967 6874 203d 2066 726f  dge_weight = fro
-00016c30: 6d5f 7363 6970 795f 7370 6172 7365 5f6d  m_scipy_sparse_m
-00016c40: 6174 7269 7828 7765 6967 6874 735f 636f  atrix(weights_co
-00016c50: 6f29 0a20 2020 2020 2020 2020 2020 2023  o).            #
-00016c60: 2064 676c 5f67 7261 7068 203d 2064 676c   dgl_graph = dgl
-00016c70: 2e44 474c 4772 6170 6828 2920 2367 7261  .DGLGraph() #gra
-00016c80: 7068 2066 6f72 2054 7265 654c 5354 4d0a  ph for TreeLSTM.
-00016c90: 2020 2020 2020 2020 2020 2020 2320 6467              # dg
-00016ca0: 6c5f 6772 6170 6820 3d20 6467 6c2e 4447  l_graph = dgl.DG
-00016cb0: 4c48 6574 6572 6f47 7261 7068 2829 0a20  LHeteroGraph(). 
-00016cc0: 2020 2020 2020 2020 2020 2023 2064 676c             # dgl
-00016cd0: 5f67 7261 7068 2e61 6464 5f6e 6f64 6573  _graph.add_nodes
-00016ce0: 2870 6174 7269 7374 6963 5f6d 6174 7269  (patristic_matri
-00016cf0: 785b 313a 2c20 313a 5d2e 7368 6170 655b  x[1:, 1:].shape[
-00016d00: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-00016d10: 2320 6467 6c5f 6772 6170 682e 6164 645f  # dgl_graph.add_
-00016d20: 6564 6765 7328 6564 6765 5f69 6e64 6578  edges(edge_index
-00016d30: 5b30 5d2e 6375 6461 2829 2c20 6564 6765  [0].cuda(), edge
-00016d40: 5f69 6e64 6578 5b31 5d2e 6375 6461 2829  _index[1].cuda()
-00016d50: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-00016d60: 6467 6c5f 6772 6170 682e 6564 6174 615b  dgl_graph.edata[
-00016d70: 2779 275d 203d 2065 6467 655f 7765 6967  'y'] = edge_weig
-00016d80: 6874 2e63 7564 6128 290a 2020 2020 2020  ht.cuda().      
-00016d90: 2020 2020 2020 6966 2061 7267 732e 7573        if args.us
-00016da0: 655f 6375 6461 3a0a 2020 2020 2020 2020  e_cuda:.        
-00016db0: 2020 2020 2020 2020 6772 6170 685f 636f          graph_co
-00016dc0: 6f20 3d20 2865 6467 655f 696e 6465 782e  o = (edge_index.
-00016dd0: 6375 6461 2829 2c20 6564 6765 5f77 6569  cuda(), edge_wei
-00016de0: 6768 742e 6375 6461 2829 2920 2023 2067  ght.cuda())  # g
-00016df0: 7261 7068 2066 6f72 2070 7974 6f72 6368  raph for pytorch
-00016e00: 2067 656f 6d65 7472 6963 2066 6f72 2047   geometric for G
-00016e10: 4e4e 0a20 2020 2020 2020 2020 2020 2020  NN.             
-00016e20: 2020 2064 676c 5f67 7261 7068 203d 2064     dgl_graph = d
-00016e30: 676c 2e63 6f6e 7665 7274 2e66 726f 6d5f  gl.convert.from_
-00016e40: 7363 6970 7928 7765 6967 6874 735f 636f  scipy(weights_co
-00016e50: 6f29 2e74 6f28 2263 7564 6122 290a 2020  o).to("cuda").  
-00016e60: 2020 2020 2020 2020 2020 2020 2020 6467                dg
-00016e70: 6c5f 6772 6170 682e 6564 6174 615b 2779  l_graph.edata['y
-00016e80: 275d 203d 2065 6467 655f 7765 6967 6874  '] = edge_weight
-00016e90: 2e74 6f28 2263 7564 6122 290a 2020 2020  .to("cuda").    
-00016ea0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00016eb0: 2020 2020 2020 2020 2020 2020 2020 6772                gr
-00016ec0: 6170 685f 636f 6f20 3d20 2865 6467 655f  aph_coo = (edge_
-00016ed0: 696e 6465 782e 6370 7528 292c 2065 6467  index.cpu(), edg
-00016ee0: 655f 7765 6967 6874 2e63 7075 2829 2920  e_weight.cpu()) 
-00016ef0: 2023 2067 7261 7068 2066 6f72 2070 7974   # graph for pyt
-00016f00: 6f72 6368 2067 656f 6d65 7472 6963 2066  orch geometric f
-00016f10: 6f72 2047 4e4e 0a20 2020 2020 2020 2020  or GNN.         
-00016f20: 2020 2020 2020 2064 676c 5f67 7261 7068         dgl_graph
-00016f30: 203d 2064 676c 2e63 6f6e 7665 7274 2e66   = dgl.convert.f
-00016f40: 726f 6d5f 7363 6970 7928 7765 6967 6874  rom_scipy(weight
-00016f50: 735f 636f 6f29 2e74 6f28 2263 7075 2229  s_coo).to("cpu")
-00016f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016f70: 2064 676c 5f67 7261 7068 2e65 6461 7461   dgl_graph.edata
-00016f80: 5b27 7927 5d20 3d20 6564 6765 5f77 6569  ['y'] = edge_wei
-00016f90: 6768 742e 6370 7528 290a 2020 2020 2020  ght.cpu().      
-00016fa0: 2020 2020 2020 7072 696e 7428 2274 7265        print("tre
-00016fb0: 652d 6772 6170 6820 6669 6e69 7368 6564  e-graph finished
-00016fc0: 2229 0a0a 2020 2020 2020 2020 6578 6365  ")..        exce
-00016fd0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-00016fe0: 6772 6170 685f 636f 6f20 3d20 4e6f 6e65  graph_coo = None
-00016ff0: 0a20 2020 2020 2020 2020 2020 2064 676c  .            dgl
-00017000: 5f67 7261 7068 203d 204e 6f6e 650a 0a20  _graph = None.. 
-00017010: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00017020: 2067 7261 7068 5f63 6f6f 3d4e 6f6e 650a   graph_coo=None.
-00017030: 2020 2020 2020 2020 6564 6765 5f77 6569          edge_wei
-00017040: 6768 745f 6d61 7472 6978 3d4e 6f6e 650a  ght_matrix=None.
-00017050: 2020 2020 2020 2020 6467 6c5f 6772 6170          dgl_grap
-00017060: 6820 3d20 4e6f 6e65 0a20 2020 2062 6c6f  h = None.    blo
-00017070: 7375 6d5f 6172 7261 792c 626c 6f73 756d  sum_array,blosum
-00017080: 5f64 6963 7420 3d20 6372 6561 7465 5f62  _dict = create_b
-00017090: 6c6f 7375 6d28 6275 696c 645f 636f 6e66  losum(build_conf
-000170a0: 6967 2e61 615f 7072 6f62 732c 6172 6773  ig.aa_probs,args
-000170b0: 2e73 7562 735f 6d61 7472 6978 290a 0a20  .subs_matrix).. 
-000170c0: 2020 2023 6467 6c5f 6772 6170 682e 6e64     #dgl_graph.nd
-000170d0: 6174 615b 2778 275d 203d 2074 6f72 6368  ata['x'] = torch
-000170e0: 2e7a 6572 6f73 2828 332c 2035 2929 2023  .zeros((3, 5)) #
-000170f0: 746f 2061 6464 206c 6174 6572 2069 6e20  to add later in 
-00017100: 7468 6520 6d6f 6465 6c20 6974 2077 696c  the model it wil
-00017110: 6c20 6265 2074 6865 206c 6174 656e 7420  l be the latent 
-00017120: 7370 6163 6520 7468 6174 2067 6574 7320  space that gets 
-00017130: 7472 616e 7366 6f72 6d65 6420 746f 206c  transformed to l
-00017140: 6f67 6974 730a 2020 2020 2347 2e6e 6f64  ogits.    #G.nod
-00017150: 6573 5b5b 302c 2032 5d5d 2e64 6174 615b  es[[0, 2]].data[
-00017160: 2778 275d 203d 2074 682e 6f6e 6573 2828  'x'] = th.ones((
-00017170: 322c 2035 2929 0a0a 2020 2020 6e6f 6465  2, 5))..    node
-00017180: 735f 7265 7072 6573 656e 7461 7469 6f6e  s_representation
-00017190: 735f 6172 7261 7920 3d20 7472 6565 5f70  s_array = tree_p
-000171a0: 6f73 6974 696f 6e61 6c5f 656d 6265 6464  ositional_embedd
-000171b0: 696e 6773 2861 6e63 6573 746f 725f 696e  ings(ancestor_in
-000171c0: 666f 5f64 6963 742c 7472 6565 5f62 795f  fo_dict,tree_by_
-000171d0: 6c65 7665 6c73 5f64 6963 7429 0a20 2020  levels_dict).   
-000171e0: 2061 6464 6974 696f 6e61 6c5f 696e 666f   additional_info
-000171f0: 203d 2041 6464 6974 696f 6e61 6c49 6e66   = AdditionalInf
-00017200: 6f28 626c 6f73 756d 3d74 6f72 6368 2e66  o(blosum=torch.f
-00017210: 726f 6d5f 6e75 6d70 7928 626c 6f73 756d  rom_numpy(blosum
-00017220: 5f61 7272 6179 292c 0a20 2020 2020 2020  _array),.       
+00015b40: 2020 2020 2020 2020 5b22 626c 6f73 756d          ["blosum
+00015b50: 2220 2c22 626c 6f73 756d 5f64 6963 7422  " ,"blosum_dict"
+00015b60: 2c22 6368 696c 6472 656e 5f64 6963 7422  ,"children_dict"
+00015b70: 2c22 616e 6365 7374 6f72 5f69 6e66 6f5f  ,"ancestor_info_
+00015b80: 6469 6374 222c 2022 7472 6565 5f62 795f  dict", "tree_by_
+00015b90: 6c65 7665 6c73 5f64 6963 7422 2c20 2274  levels_dict", "t
+00015ba0: 7265 655f 6279 5f6c 6576 656c 735f 6172  ree_by_levels_ar
+00015bb0: 7261 7922 2c0a 2020 2020 2020 2020 2020  ray",.          
+00015bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015bd0: 2020 2022 7061 7472 6973 7469 635f 696e     "patristic_in
+00015be0: 666f 222c 2022 6772 6170 685f 636f 6f22  fo", "graph_coo"
+00015bf0: 2c22 7061 7472 6973 7469 635f 6675 6c6c  ,"patristic_full
+00015c00: 5f73 7061 7273 6522 2c22 6e6f 6465 735f  _sparse","nodes_
+00015c10: 7265 7072 6573 656e 7461 7469 6f6e 735f  representations_
+00015c20: 6172 7261 7922 2c22 6467 6c5f 6772 6170  array","dgl_grap
+00015c30: 6822 5d29 0a0a 2020 2020 616e 6365 7374  h"])..    ancest
+00015c40: 6f72 5f69 6e66 6f5f 6469 6374 203d 2064  or_info_dict = d
+00015c50: 6963 7428 7a69 7028 616e 6365 7374 6f72  ict(zip(ancestor
+00015c60: 5f69 6e66 6f5b 3a2c 305d 2e74 6f6c 6973  _info[:,0].tolis
+00015c70: 7428 292c 616e 6365 7374 6f72 5f69 6e66  t(),ancestor_inf
+00015c80: 6f5b 3a2c 325d 2e74 6f6c 6973 7428 2929  o[:,2].tolist())
+00015c90: 290a 2020 2020 7069 636b 6c65 2e64 756d  ).    pickle.dum
+00015ca0: 7028 616e 6365 7374 6f72 5f69 6e66 6f5f  p(ancestor_info_
+00015cb0: 6469 6374 2c20 6f70 656e 2827 7b7d 2f41  dict, open('{}/A
+00015cc0: 6e63 6573 746f 725f 696e 666f 5f64 6963  ncestor_info_dic
+00015cd0: 742e 7027 2e66 6f72 6d61 7428 7265 7375  t.p'.format(resu
+00015ce0: 6c74 735f 6469 7229 2c20 2777 6227 292c  lts_dir), 'wb'),
+00015cf0: 2070 726f 746f 636f 6c3d 7069 636b 6c65   protocol=pickle
+00015d00: 2e48 4947 4845 5354 5f50 524f 544f 434f  .HIGHEST_PROTOCO
+00015d10: 4c29 0a20 2020 2069 6620 6973 696e 7374  L).    if isinst
+00015d20: 616e 6365 2870 6174 7269 7374 6963 5f6d  ance(patristic_m
+00015d30: 6174 7269 782c 6e70 2e6e 6461 7272 6179  atrix,np.ndarray
+00015d40: 293a 0a20 2020 2020 2020 2070 6174 7269  ):.        patri
+00015d50: 7374 6963 5f69 6e66 6f20 3d20 6469 6374  stic_info = dict
+00015d60: 287a 6970 286c 6973 7428 7261 6e67 6528  (zip(list(range(
+00015d70: 6c65 6e28 7061 7472 6973 7469 635f 6d61  len(patristic_ma
+00015d80: 7472 6978 292d 3129 292c 7061 7472 6973  trix)-1)),patris
+00015d90: 7469 635f 6d61 7472 6978 5b31 3a2c 305d  tic_matrix[1:,0]
+00015da0: 2e61 7374 7970 6528 696e 7429 2e74 6f6c  .astype(int).tol
+00015db0: 6973 7428 2929 2920 2353 6b69 7020 7468  ist())) #Skip th
+00015dc0: 6520 6661 6b65 2068 6561 6465 720a 2020  e fake header.  
+00015dd0: 2020 656c 7365 3a0a 0a20 2020 2020 2020    else:..       
+00015de0: 2070 6174 7269 7374 6963 5f69 6e66 6f20   patristic_info 
+00015df0: 3d64 6963 7428 7a69 7028 6c69 7374 2872  =dict(zip(list(r
+00015e00: 616e 6765 286c 656e 2870 6174 7269 7374  ange(len(patrist
+00015e10: 6963 5f6d 6174 7269 7829 2d31 2929 2c70  ic_matrix)-1)),p
+00015e20: 6174 7269 7374 6963 5f6d 6174 7269 785b  atristic_matrix[
+00015e30: 313a 2c30 5d2e 7479 7065 2874 6f72 6368  1:,0].type(torch
+00015e40: 2e69 6e74 292e 746f 6c69 7374 2829 2929  .int).tolist()))
+00015e50: 0a0a 2020 2020 616e 6365 7374 6f72 735f  ..    ancestors_
+00015e60: 696e 666f 5f66 6c69 7070 6564 203d 206e  info_flipped = n
+00015e70: 702e 666c 6970 2861 6e63 6573 746f 725f  p.flip(ancestor_
+00015e80: 696e 666f 2c20 6178 6973 3d31 2920 2353  info, axis=1) #S
+00015e90: 6f20 7765 2063 616e 2065 7661 6c75 6174  o we can evaluat
+00015ea0: 6520 696e 2072 6576 6572 7365 2c20 7765  e in reverse, we
+00015eb0: 2073 7461 7274 2077 6974 6820 7468 6520   start with the 
+00015ec0: 6c61 7374 2063 6f6c 756d 6e0a 0a20 2020  last column..   
+00015ed0: 2074 7265 655f 6279 5f6c 6576 656c 7320   tree_by_levels 
+00015ee0: 3d20 5b5d 0a20 2020 2066 6f72 2063 6f6c  = [].    for col
+00015ef0: 756d 6e20 696e 2061 6e63 6573 746f 7273  umn in ancestors
+00015f00: 5f69 6e66 6f5f 666c 6970 7065 642e 543a  _info_flipped.T:
+00015f10: 0a20 2020 2020 2020 2069 6e64 6578 6573  .        indexes
+00015f20: 203d 206e 702e 7768 6572 6528 636f 6c75   = np.where(colu
+00015f30: 6d6e 203d 3d20 3029 0a20 2020 2020 2020  mn == 0).       
+00015f40: 206c 6576 656c 203d 2061 6e63 6573 746f   level = ancesto
+00015f50: 7273 5f69 6e66 6f5f 666c 6970 7065 642e  rs_info_flipped.
+00015f60: 545b 2d31 5d5b 696e 6465 7865 735d 0a20  T[-1][indexes]. 
+00015f70: 2020 2020 2020 2074 7265 655f 6279 5f6c         tree_by_l
+00015f80: 6576 656c 732e 6170 7065 6e64 286c 6576  evels.append(lev
+00015f90: 656c 290a 0a20 2020 2074 7265 655f 6279  el)..    tree_by
+00015fa0: 5f6c 6576 656c 7320 3d20 7472 6565 5f62  _levels = tree_b
+00015fb0: 795f 6c65 7665 6c73 5b3a 2d31 5d20 2374  y_levels[:-1] #t
+00015fc0: 6865 2072 6f6f 7420 6765 7473 2061 6464  he root gets add
+00015fd0: 6564 2074 7769 6365 2062 6563 6175 7365  ed twice because
+00015fe0: 2074 6865 2066 6972 7374 2063 6f6c 756d   the first colum
+00015ff0: 6e20 6172 6520 7468 6520 6e6f 6465 2069  n are the node i
+00016000: 6e64 6578 6573 2c20 6361 6e6e 6f74 2062  ndexes, cannot b
+00016010: 6520 6669 7865 642c 206f 7468 6572 7769  e fixed, otherwi
+00016020: 7365 2077 6520 6361 6e6e 6f74 2064 6f20  se we cannot do 
+00016030: 7468 6520 7472 6963 6b0a 0a20 2020 2074  the trick..    t
+00016040: 7265 655f 6279 5f6c 6576 656c 735f 6469  ree_by_levels_di
+00016050: 6374 203d 2064 6963 7428 7a69 7028 6c69  ct = dict(zip(li
+00016060: 7374 2872 6576 6572 7365 6428 7261 6e67  st(reversed(rang
+00016070: 6528 6c65 6e28 7472 6565 5f62 795f 6c65  e(len(tree_by_le
+00016080: 7665 6c73 2929 2929 2c74 7265 655f 6279  vels)))),tree_by
+00016090: 5f6c 6576 656c 7329 290a 2020 2020 7069  _levels)).    pi
+000160a0: 636b 6c65 2e64 756d 7028 7472 6565 5f62  ckle.dump(tree_b
+000160b0: 795f 6c65 7665 6c73 5f64 6963 742c 206f  y_levels_dict, o
+000160c0: 7065 6e28 277b 7d2f 5472 6565 5f62 795f  pen('{}/Tree_by_
+000160d0: 6c65 7665 6c73 5f64 6963 742e 7027 2e66  levels_dict.p'.f
+000160e0: 6f72 6d61 7428 7265 7375 6c74 735f 6469  ormat(results_di
+000160f0: 7229 2c20 2777 6227 292c 2070 726f 746f  r), 'wb'), proto
+00016100: 636f 6c3d 7069 636b 6c65 2e48 4947 4845  col=pickle.HIGHE
+00016110: 5354 5f50 524f 544f 434f 4c29 0a0a 2020  ST_PROTOCOL)..  
+00016120: 2020 6c65 6e67 7468 203d 206d 6178 286d    length = max(m
+00016130: 6170 286c 656e 2c20 7472 6565 5f62 795f  ap(len, tree_by_
+00016140: 6c65 7665 6c73 5f64 6963 742e 7661 6c75  levels_dict.valu
+00016150: 6573 2829 2929 0a20 2020 2074 7265 655f  es())).    tree_
+00016160: 6279 5f6c 6576 656c 735f 6172 7261 7920  by_levels_array 
+00016170: 3d20 6e70 2e61 7272 6179 285b 7869 2e74  = np.array([xi.t
+00016180: 6f6c 6973 7428 2920 2b20 5b4e 6f6e 655d  olist() + [None]
+00016190: 202a 2028 6c65 6e67 7468 202d 206c 656e   * (length - len
+000161a0: 2878 6929 2920 666f 7220 7869 2069 6e20  (xi)) for xi in 
+000161b0: 7472 6565 5f62 795f 6c65 7665 6c73 5d29  tree_by_levels])
+000161c0: 0a20 2020 2023 2074 7265 655f 6c65 7665  .    # tree_leve
+000161d0: 6c73 5f32 203d 2043 7265 6174 655f 7472  ls_2 = Create_tr
+000161e0: 6565 5f62 795f 6c65 7665 6c73 2863 6869  ee_by_levels(chi
+000161f0: 6c64 7265 6e5f 6469 6374 290a 0a20 2020  ldren_dict)..   
+00016200: 2063 6869 6c64 7265 6e5f 6469 6374 203d   children_dict =
+00016210: 207b 7d0a 2020 2020 666f 7220 6b2c 2076   {}.    for k, v
+00016220: 2069 6e20 616e 6365 7374 6f72 5f69 6e66   in ancestor_inf
+00016230: 6f5f 6469 6374 2e69 7465 6d73 2829 3a0a  o_dict.items():.
+00016240: 2020 2020 2020 2020 6368 696c 6472 656e          children
+00016250: 5f64 6963 745b 765d 203d 2063 6869 6c64  _dict[v] = child
+00016260: 7265 6e5f 6469 6374 2e67 6574 2876 2c20  ren_dict.get(v, 
+00016270: 5b5d 290a 2020 2020 2020 2020 6368 696c  []).        chil
+00016280: 6472 656e 5f64 6963 745b 765d 2e61 7070  dren_dict[v].app
+00016290: 656e 6428 6b29 0a20 2020 2070 6963 6b6c  end(k).    pickl
+000162a0: 652e 6475 6d70 2863 6869 6c64 7265 6e5f  e.dump(children_
+000162b0: 6469 6374 2c20 6f70 656e 2827 7b7d 2f43  dict, open('{}/C
+000162c0: 6869 6c64 7265 6e5f 6469 6374 2e70 272e  hildren_dict.p'.
+000162d0: 666f 726d 6174 2872 6573 756c 7473 5f64  format(results_d
+000162e0: 6972 292c 2027 7762 2729 2c0a 2020 2020  ir), 'wb'),.    
+000162f0: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
+00016300: 6f63 6f6c 3d70 6963 6b6c 652e 4849 4748  ocol=pickle.HIGH
+00016310: 4553 545f 5052 4f54 4f43 4f4c 290a 0a20  EST_PROTOCOL).. 
+00016320: 2020 2023 2268 7474 7073 3a2f 2f70 7974     #"https://pyt
+00016330: 6f72 6368 2d67 656f 6d65 7472 6963 2e72  orch-geometric.r
+00016340: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00016350: 2f6c 6174 6573 742f 6e6f 7465 732f 696e  /latest/notes/in
+00016360: 7472 6f64 7563 7469 6f6e 2e68 746d 6c22  troduction.html"
+00016370: 0a20 2020 2023 4869 6768 6c69 6768 743a  .    #Highlight:
+00016380: 4275 696c 6420 7468 6520 6d61 7472 6978  Build the matrix
+00016390: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+000163a0: 6f66 2074 6865 2074 7265 6520 6772 6170  of the tree grap
+000163b0: 683a 2044 6972 6563 7465 6420 2872 6f6f  h: Directed (roo
+000163c0: 742d 3e20 6c65 6176 6573 2920 7765 6967  t-> leaves) weig
+000163d0: 6874 6564 2028 7061 7472 6973 7469 6320  hted (patristic 
+000163e0: 6469 7374 2920 6772 6170 680a 2020 2020  dist) graph.    
+000163f0: 6966 2062 7569 6c64 5f63 6f6e 6669 672e  if build_config.
+00016400: 6275 696c 645f 6772 6170 683a 2023 544f  build_graph: #TO
+00016410: 444f 3a20 4669 7820 696e 2073 6572 7665  DO: Fix in serve
+00016420: 720a 2020 2020 2020 2020 7072 696e 7428  r.        print(
+00016430: 2242 7569 6c64 696e 6720 6120 7472 6565  "Building a tree
+00016440: 2d67 7261 7068 2229 0a20 2020 2020 2020  -graph").       
+00016450: 2023 6d61 6b65 2067 7261 7068 2061 646a   #make graph adj
+00016460: 6163 656e 7420 6d61 7472 6978 0a20 2020  acent matrix.   
+00016470: 2020 2020 2070 6174 7269 7374 6963 5f6d       patristic_m
+00016480: 6174 7269 7820 3d20 7061 7472 6973 7469  atrix = patristi
+00016490: 635f 6d61 7472 6978 5b70 6174 7269 7374  c_matrix[patrist
+000164a0: 6963 5f6d 6174 7269 785b 3a2c 2030 5d2e  ic_matrix[:, 0].
+000164b0: 6172 6773 6f72 7428 295d 0a20 2020 2020  argsort()].     
+000164c0: 2020 2070 6174 7269 7374 6963 5f6d 6174     patristic_mat
+000164d0: 7269 7820 3d20 7061 7472 6973 7469 635f  rix = patristic_
+000164e0: 6d61 7472 6978 5b3a 2c20 7061 7472 6973  matrix[:, patris
+000164f0: 7469 635f 6d61 7472 6978 5b30 2c20 3a5d  tic_matrix[0, :]
+00016500: 2e61 7267 736f 7274 2829 5d0a 0a20 2020  .argsort()]..   
+00016510: 2020 2020 2067 7261 7068 5f6e 6f64 655f       graph_node_
+00016520: 6d61 7472 6978 203d 206e 702e 7a65 726f  matrix = np.zero
+00016530: 735f 6c69 6b65 2870 6174 7269 7374 6963  s_like(patristic
+00016540: 5f6d 6174 7269 7829 2023 4469 7265 6374  _matrix) #Direct
+00016550: 6564 2028 726f 6f74 2d3e 206c 6561 7665  ed (root-> leave
+00016560: 7329 204e 4f54 2077 6569 6768 7465 6420  s) NOT weighted 
+00016570: 6772 6170 680a 2020 2020 2020 2020 6564  graph.        ed
+00016580: 6765 5f77 6569 6768 745f 6d61 7472 6978  ge_weight_matrix
+00016590: 203d 206e 702e 7a65 726f 735f 6c69 6b65   = np.zeros_like
+000165a0: 2870 6174 7269 7374 6963 5f6d 6174 7269  (patristic_matri
+000165b0: 7829 2023 4469 7265 6374 6564 2028 726f  x) #Directed (ro
+000165c0: 6f74 2d3e 206c 6561 7665 7329 2077 6569  ot-> leaves) wei
+000165d0: 6768 7465 6420 2870 6174 7269 7374 6963  ghted (patristic
+000165e0: 2064 6973 7429 2067 7261 7068 0a20 2020   dist) graph.   
+000165f0: 2020 2020 2067 7261 7068 5f6e 6f64 655f       graph_node_
+00016600: 6d61 7472 6978 5b30 2c3a 5d20 3d20 7061  matrix[0,:] = pa
+00016610: 7472 6973 7469 635f 6d61 7472 6978 5b30  tristic_matrix[0
+00016620: 2c3a 5d0a 2020 2020 2020 2020 6772 6170  ,:].        grap
+00016630: 685f 6e6f 6465 5f6d 6174 7269 785b 3a2c  h_node_matrix[:,
+00016640: 305d 203d 2070 6174 7269 7374 6963 5f6d  0] = patristic_m
+00016650: 6174 7269 785b 3a2c 305d 0a20 2020 2020  atrix[:,0].     
+00016660: 2020 2065 6467 655f 7765 6967 6874 5f6d     edge_weight_m
+00016670: 6174 7269 785b 302c 203a 5d20 3d20 7061  atrix[0, :] = pa
+00016680: 7472 6973 7469 635f 6d61 7472 6978 5b30  tristic_matrix[0
+00016690: 2c20 3a5d 0a20 2020 2020 2020 2065 6467  , :].        edg
+000166a0: 655f 7765 6967 6874 5f6d 6174 7269 785b  e_weight_matrix[
+000166b0: 3a2c 2030 5d20 3d20 7061 7472 6973 7469  :, 0] = patristi
+000166c0: 635f 6d61 7472 6978 5b3a 2c20 305d 0a20  c_matrix[:, 0]. 
+000166d0: 2020 2020 2020 2066 6f72 2061 6e63 6573         for ances
+000166e0: 746f 722c 6368 696c 6472 656e 2069 6e20  tor,children in 
+000166f0: 6368 696c 6472 656e 5f64 6963 742e 6974  children_dict.it
+00016700: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+00016710: 2020 2061 6e63 6573 746f 725f 6964 7820     ancestor_idx 
+00016720: 3d20 6e70 2e69 6e31 6428 6772 6170 685f  = np.in1d(graph_
+00016730: 6e6f 6465 5f6d 6174 7269 785b 302c 3a5d  node_matrix[0,:]
+00016740: 2c20 616e 6365 7374 6f72 292e 6e6f 6e7a  , ancestor).nonz
+00016750: 6572 6f28 295b 305d 0a20 2020 2020 2020  ero()[0].       
+00016760: 2020 2020 2063 6869 6c64 7265 6e5f 6964       children_id
+00016770: 783d 206e 702e 696e 3164 2867 7261 7068  x= np.in1d(graph
+00016780: 5f6e 6f64 655f 6d61 7472 6978 5b30 2c3a  _node_matrix[0,:
+00016790: 5d2c 2063 6869 6c64 7265 6e29 2e6e 6f6e  ], children).non
+000167a0: 7a65 726f 2829 5b30 5d0a 2020 2020 2020  zero()[0].      
+000167b0: 2020 2020 2020 6772 6170 685f 6e6f 6465        graph_node
+000167c0: 5f6d 6174 7269 785b 616e 6365 7374 6f72  _matrix[ancestor
+000167d0: 5f69 6478 2c63 6869 6c64 7265 6e5f 6964  _idx,children_id
+000167e0: 785d 203d 2031 2023 636f 6e74 6169 6e73  x] = 1 #contains
+000167f0: 206e 6f20 6564 6765 7320 7765 6967 6874   no edges weight
+00016800: 730a 2020 2020 2020 2020 2020 2020 6772  s.            gr
+00016810: 6170 685f 6e6f 6465 5f6d 6174 7269 785b  aph_node_matrix[
+00016820: 6368 696c 6472 656e 5f69 6478 2c61 6e63  children_idx,anc
+00016830: 6573 746f 725f 6964 785d 203d 2031 0a20  estor_idx] = 1. 
+00016840: 2020 2020 2020 2020 2020 2065 6467 655f             edge_
+00016850: 7765 6967 6874 5f6d 6174 7269 785b 616e  weight_matrix[an
+00016860: 6365 7374 6f72 5f69 6478 2c20 6368 696c  cestor_idx, chil
+00016870: 6472 656e 5f69 6478 5d20 3d20 7061 7472  dren_idx] = patr
+00016880: 6973 7469 635f 6d61 7472 6978 5b61 6e63  istic_matrix[anc
+00016890: 6573 746f 725f 6964 782c 2063 6869 6c64  estor_idx, child
+000168a0: 7265 6e5f 6964 785d 0a20 2020 2020 2020  ren_idx].       
+000168b0: 2020 2020 2023 6564 6765 5f77 6569 6768       #edge_weigh
+000168c0: 745f 6d61 7472 6978 5b63 6869 6c64 7265  t_matrix[childre
+000168d0: 6e5f 6964 782c 2061 6e63 6573 746f 725f  n_idx, ancestor_
+000168e0: 6964 785d 203d 2070 6174 7269 7374 6963  idx] = patristic
+000168f0: 5f6d 6174 7269 785b 6368 696c 6472 656e  _matrix[children
+00016900: 5f69 6478 2c20 616e 6365 7374 6f72 5f69  _idx, ancestor_i
+00016910: 6478 5d20 2348 6967 686c 6967 6874 3a20  dx] #Highlight: 
+00016920: 4e6f 7420 7573 6520 746f 2061 766f 6964  Not use to avoid
+00016930: 2063 7265 6174 696e 6720 6120 7365 6c66   creating a self
+00016940: 206c 6f6f 7065 6420 6772 6170 6820 6f72   looped graph or
+00016950: 2062 6964 6972 6563 7469 6f6e 616c 2067   bidirectional g
+00016960: 7261 7068 730a 2020 2020 2020 2020 2343  raphs.        #C
+00016970: 7265 6174 6520 6120 636f 6f72 6469 6e61  reate a coordina
+00016980: 7465 7320 6d61 7472 6978 2c20 6261 7369  tes matrix, basi
+00016990: 6361 6c6c 7920 706f 696e 7473 206f 7574  cally points out
+000169a0: 2077 6869 6368 2072 6567 696f 6e73 2066   which regions f
+000169b0: 726f 6d20 7468 6520 6d61 7472 6978 2064  rom the matrix d
+000169c0: 6f20 6e6f 7420 6861 7665 2030 2076 616c  o not have 0 val
+000169d0: 7565 7320 616e 6420 7468 6572 6566 6f72  ues and therefor
+000169e0: 6520 6172 6520 636f 6e6e 6563 7465 640a  e are connected.
+000169f0: 2020 2020 2020 2020 7765 6967 6874 735f          weights_
+00016a00: 636f 6f20 3d20 636f 6f5f 6d61 7472 6978  coo = coo_matrix
+00016a10: 2865 6467 655f 7765 6967 6874 5f6d 6174  (edge_weight_mat
+00016a20: 7269 785b 313a 2c31 3a5d 290a 2020 2020  rix[1:,1:]).    
+00016a30: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00016a40: 2020 2020 2023 5468 6520 6772 6170 6820       #The graph 
+00016a50: 636f 6e6e 6563 7469 7669 7479 2028 6564  connectivity (ed
+00016a60: 6765 2069 6e64 6578 2920 7368 6f75 6c64  ge index) should
+00016a70: 2062 6520 636f 6e66 696e 6564 2077 6974   be confined wit
+00016a80: 6820 7468 6520 434f 4f20 666f 726d 6174  h the COO format
+00016a90: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+00016aa0: 692e 652e 2074 6865 2066 6972 7374 206c  i.e. the first l
+00016ab0: 6973 7420 636f 6e74 6169 6e73 2074 6865  ist contains the
+00016ac0: 2069 6e64 6578 206f 6620 7468 6520 736f   index of the so
+00016ad0: 7572 6365 206e 6f64 6573 2c20 7768 696c  urce nodes, whil
+00016ae0: 6520 7468 6520 696e 6465 7820 6f66 2074  e the index of t
+00016af0: 6172 6765 7420 6e6f 6465 7320 6973 2073  arget nodes is s
+00016b00: 7065 6369 6669 6564 2069 6e20 7468 6520  pecified in the 
+00016b10: 7365 636f 6e64 206c 6973 742e 0a20 2020  second list..   
+00016b20: 2020 2020 2020 2020 2023 4e6f 7465 2074           #Note t
+00016b30: 6861 7420 7468 6520 6f72 6465 7220 6f66  hat the order of
+00016b40: 2074 6865 2065 6467 6520 696e 6465 7820   the edge index 
+00016b50: 6973 2069 7272 656c 6576 616e 7420 746f  is irrelevant to
+00016b60: 2074 6865 2044 6174 6120 6f62 6a65 6374   the Data object
+00016b70: 2079 6f75 2063 7265 6174 6520 7369 6e63   you create sinc
+00016b80: 6520 7375 6368 2069 6e66 6f72 6d61 7469  e such informati
+00016b90: 6f6e 2069 7320 6f6e 6c79 2066 6f72 2063  on is only for c
+00016ba0: 6f6d 7075 7469 6e67 2074 6865 2061 646a  omputing the adj
+00016bb0: 6163 656e 6379 206d 6174 7269 782e 0a20  acency matrix.. 
+00016bc0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
+00016bd0: 746f 7263 685f 6765 6f6d 6574 7269 632e  torch_geometric.
+00016be0: 7574 696c 732e 636f 6e76 6572 7420 696d  utils.convert im
+00016bf0: 706f 7274 2066 726f 6d5f 7363 6970 795f  port from_scipy_
+00016c00: 7370 6172 7365 5f6d 6174 7269 780a 2020  sparse_matrix.  
+00016c10: 2020 2020 2020 2020 2020 6564 6765 5f69            edge_i
+00016c20: 6e64 6578 2c65 6467 655f 7765 6967 6874  ndex,edge_weight
+00016c30: 203d 2066 726f 6d5f 7363 6970 795f 7370   = from_scipy_sp
+00016c40: 6172 7365 5f6d 6174 7269 7828 7765 6967  arse_matrix(weig
+00016c50: 6874 735f 636f 6f29 0a20 2020 2020 2020  hts_coo).       
+00016c60: 2020 2020 2023 2064 676c 5f67 7261 7068       # dgl_graph
+00016c70: 203d 2064 676c 2e44 474c 4772 6170 6828   = dgl.DGLGraph(
+00016c80: 2920 2367 7261 7068 2066 6f72 2054 7265  ) #graph for Tre
+00016c90: 654c 5354 4d0a 2020 2020 2020 2020 2020  eLSTM.          
+00016ca0: 2020 2320 6467 6c5f 6772 6170 6820 3d20    # dgl_graph = 
+00016cb0: 6467 6c2e 4447 4c48 6574 6572 6f47 7261  dgl.DGLHeteroGra
+00016cc0: 7068 2829 0a20 2020 2020 2020 2020 2020  ph().           
+00016cd0: 2023 2064 676c 5f67 7261 7068 2e61 6464   # dgl_graph.add
+00016ce0: 5f6e 6f64 6573 2870 6174 7269 7374 6963  _nodes(patristic
+00016cf0: 5f6d 6174 7269 785b 313a 2c20 313a 5d2e  _matrix[1:, 1:].
+00016d00: 7368 6170 655b 305d 290a 2020 2020 2020  shape[0]).      
+00016d10: 2020 2020 2020 2320 6467 6c5f 6772 6170        # dgl_grap
+00016d20: 682e 6164 645f 6564 6765 7328 6564 6765  h.add_edges(edge
+00016d30: 5f69 6e64 6578 5b30 5d2e 6375 6461 2829  _index[0].cuda()
+00016d40: 2c20 6564 6765 5f69 6e64 6578 5b31 5d2e  , edge_index[1].
+00016d50: 6375 6461 2829 290a 2020 2020 2020 2020  cuda()).        
+00016d60: 2020 2020 2320 6467 6c5f 6772 6170 682e      # dgl_graph.
+00016d70: 6564 6174 615b 2779 275d 203d 2065 6467  edata['y'] = edg
+00016d80: 655f 7765 6967 6874 2e63 7564 6128 290a  e_weight.cuda().
+00016d90: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00016da0: 7267 732e 7573 655f 6375 6461 3a0a 2020  rgs.use_cuda:.  
+00016db0: 2020 2020 2020 2020 2020 2020 2020 6772                gr
+00016dc0: 6170 685f 636f 6f20 3d20 2865 6467 655f  aph_coo = (edge_
+00016dd0: 696e 6465 782e 6375 6461 2829 2c20 6564  index.cuda(), ed
+00016de0: 6765 5f77 6569 6768 742e 6375 6461 2829  ge_weight.cuda()
+00016df0: 2920 2023 2067 7261 7068 2066 6f72 2070  )  # graph for p
+00016e00: 7974 6f72 6368 2067 656f 6d65 7472 6963  ytorch geometric
+00016e10: 2066 6f72 2047 4e4e 0a20 2020 2020 2020   for GNN.       
+00016e20: 2020 2020 2020 2020 2064 676c 5f67 7261           dgl_gra
+00016e30: 7068 203d 2064 676c 2e63 6f6e 7665 7274  ph = dgl.convert
+00016e40: 2e66 726f 6d5f 7363 6970 7928 7765 6967  .from_scipy(weig
+00016e50: 6874 735f 636f 6f29 2e74 6f28 2263 7564  hts_coo).to("cud
+00016e60: 6122 290a 2020 2020 2020 2020 2020 2020  a").            
+00016e70: 2020 2020 6467 6c5f 6772 6170 682e 6564      dgl_graph.ed
+00016e80: 6174 615b 2779 275d 203d 2065 6467 655f  ata['y'] = edge_
+00016e90: 7765 6967 6874 2e74 6f28 2263 7564 6122  weight.to("cuda"
+00016ea0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00016eb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00016ec0: 2020 2020 6772 6170 685f 636f 6f20 3d20      graph_coo = 
+00016ed0: 2865 6467 655f 696e 6465 782e 6370 7528  (edge_index.cpu(
+00016ee0: 292c 2065 6467 655f 7765 6967 6874 2e63  ), edge_weight.c
+00016ef0: 7075 2829 2920 2023 2067 7261 7068 2066  pu())  # graph f
+00016f00: 6f72 2070 7974 6f72 6368 2067 656f 6d65  or pytorch geome
+00016f10: 7472 6963 2066 6f72 2047 4e4e 0a20 2020  tric for GNN.   
+00016f20: 2020 2020 2020 2020 2020 2020 2064 676c               dgl
+00016f30: 5f67 7261 7068 203d 2064 676c 2e63 6f6e  _graph = dgl.con
+00016f40: 7665 7274 2e66 726f 6d5f 7363 6970 7928  vert.from_scipy(
+00016f50: 7765 6967 6874 735f 636f 6f29 2e74 6f28  weights_coo).to(
+00016f60: 2263 7075 2229 0a20 2020 2020 2020 2020  "cpu").         
+00016f70: 2020 2020 2020 2064 676c 5f67 7261 7068         dgl_graph
+00016f80: 2e65 6461 7461 5b27 7927 5d20 3d20 6564  .edata['y'] = ed
+00016f90: 6765 5f77 6569 6768 742e 6370 7528 290a  ge_weight.cpu().
+00016fa0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00016fb0: 7428 2274 7265 652d 6772 6170 6820 6669  t("tree-graph fi
+00016fc0: 6e69 7368 6564 2229 0a0a 2020 2020 2020  nished")..      
+00016fd0: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+00016fe0: 2020 2020 2020 6772 6170 685f 636f 6f20        graph_coo 
+00016ff0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00017000: 2020 2064 676c 5f67 7261 7068 203d 204e     dgl_graph = N
+00017010: 6f6e 650a 0a20 2020 2065 6c73 653a 0a20  one..    else:. 
+00017020: 2020 2020 2020 2067 7261 7068 5f63 6f6f         graph_coo
+00017030: 3d4e 6f6e 650a 2020 2020 2020 2020 6564  =None.        ed
+00017040: 6765 5f77 6569 6768 745f 6d61 7472 6978  ge_weight_matrix
+00017050: 3d4e 6f6e 650a 2020 2020 2020 2020 6467  =None.        dg
+00017060: 6c5f 6772 6170 6820 3d20 4e6f 6e65 0a20  l_graph = None. 
+00017070: 2020 2062 6c6f 7375 6d5f 6172 7261 792c     blosum_array,
+00017080: 626c 6f73 756d 5f64 6963 7420 3d20 6372  blosum_dict = cr
+00017090: 6561 7465 5f62 6c6f 7375 6d28 6275 696c  eate_blosum(buil
+000170a0: 645f 636f 6e66 6967 2e61 615f 7072 6f62  d_config.aa_prob
+000170b0: 732c 6172 6773 2e73 7562 735f 6d61 7472  s,args.subs_matr
+000170c0: 6978 290a 0a20 2020 2023 6467 6c5f 6772  ix)..    #dgl_gr
+000170d0: 6170 682e 6e64 6174 615b 2778 275d 203d  aph.ndata['x'] =
+000170e0: 2074 6f72 6368 2e7a 6572 6f73 2828 332c   torch.zeros((3,
+000170f0: 2035 2929 2023 746f 2061 6464 206c 6174   5)) #to add lat
+00017100: 6572 2069 6e20 7468 6520 6d6f 6465 6c20  er in the model 
+00017110: 6974 2077 696c 6c20 6265 2074 6865 206c  it will be the l
+00017120: 6174 656e 7420 7370 6163 6520 7468 6174  atent space that
+00017130: 2067 6574 7320 7472 616e 7366 6f72 6d65   gets transforme
+00017140: 6420 746f 206c 6f67 6974 730a 2020 2020  d to logits.    
+00017150: 2347 2e6e 6f64 6573 5b5b 302c 2032 5d5d  #G.nodes[[0, 2]]
+00017160: 2e64 6174 615b 2778 275d 203d 2074 682e  .data['x'] = th.
+00017170: 6f6e 6573 2828 322c 2035 2929 0a0a 2020  ones((2, 5))..  
+00017180: 2020 6e6f 6465 735f 7265 7072 6573 656e    nodes_represen
+00017190: 7461 7469 6f6e 735f 6172 7261 7920 3d20  tations_array = 
+000171a0: 7472 6565 5f70 6f73 6974 696f 6e61 6c5f  tree_positional_
+000171b0: 656d 6265 6464 696e 6773 2861 6e63 6573  embeddings(ances
+000171c0: 746f 725f 696e 666f 5f64 6963 742c 7472  tor_info_dict,tr
+000171d0: 6565 5f62 795f 6c65 7665 6c73 5f64 6963  ee_by_levels_dic
+000171e0: 7429 0a20 2020 2061 6464 6974 696f 6e61  t).    additiona
+000171f0: 6c5f 696e 666f 203d 2041 6464 6974 696f  l_info = Additio
+00017200: 6e61 6c49 6e66 6f28 626c 6f73 756d 3d74  nalInfo(blosum=t
+00017210: 6f72 6368 2e66 726f 6d5f 6e75 6d70 7928  orch.from_numpy(
+00017220: 626c 6f73 756d 5f61 7272 6179 292c 0a20  blosum_array),. 
 00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017240: 2020 2020 2020 2020 2020 2020 2020 626c                bl
-00017250: 6f73 756d 5f64 6963 743d 626c 6f73 756d  osum_dict=blosum
-00017260: 5f64 6963 742c 0a20 2020 2020 2020 2020  _dict,.         
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2020 2020 626c 6f73 756d 5f64 6963 743d      blosum_dict=
+00017260: 626c 6f73 756d 5f64 6963 742c 0a20 2020  blosum_dict,.   
 00017270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017280: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00017290: 6472 656e 5f64 6963 7420 3d20 6368 696c  dren_dict = chil
-000172a0: 6472 656e 5f64 6963 742c 0a20 2020 2020  dren_dict,.     
-000172b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017290: 2020 6368 696c 6472 656e 5f64 6963 7420    children_dict 
+000172a0: 3d20 6368 696c 6472 656e 5f64 6963 742c  = children_dict,
+000172b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000172c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172d0: 616e 6365 7374 6f72 5f69 6e66 6f5f 6469  ancestor_info_di
-000172e0: 6374 3d61 6e63 6573 746f 725f 696e 666f  ct=ancestor_info
-000172f0: 5f64 6963 742c 0a20 2020 2020 2020 2020  _dict,.         
+000172d0: 2020 2020 2020 616e 6365 7374 6f72 5f69        ancestor_i
+000172e0: 6e66 6f5f 6469 6374 3d61 6e63 6573 746f  nfo_dict=ancesto
+000172f0: 725f 696e 666f 5f64 6963 742c 0a20 2020  r_info_dict,.   
 00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017310: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-00017320: 5f62 795f 6c65 7665 6c73 5f64 6963 743d  _by_levels_dict=
-00017330: 7472 6565 5f62 795f 6c65 7665 6c73 5f64  tree_by_levels_d
-00017340: 6963 742c 0a20 2020 2020 2020 2020 2020  ict,.           
+00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017320: 2020 7472 6565 5f62 795f 6c65 7665 6c73    tree_by_levels
+00017330: 5f64 6963 743d 7472 6565 5f62 795f 6c65  _dict=tree_by_le
+00017340: 7665 6c73 5f64 6963 742c 0a20 2020 2020  vels_dict,.     
 00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017360: 2020 2020 2020 2020 2020 7472 6565 5f62            tree_b
-00017370: 795f 6c65 7665 6c73 5f61 7272 6179 3d74  y_levels_array=t
-00017380: 7265 655f 6279 5f6c 6576 656c 735f 6172  ree_by_levels_ar
-00017390: 7261 792c 0a20 2020 2020 2020 2020 2020  ray,.           
+00017360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017370: 7472 6565 5f62 795f 6c65 7665 6c73 5f61  tree_by_levels_a
+00017380: 7272 6179 3d74 7265 655f 6279 5f6c 6576  rray=tree_by_lev
+00017390: 656c 735f 6172 7261 792c 0a20 2020 2020  els_array,.     
 000173a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173b0: 2020 2020 2020 2020 2020 7061 7472 6973            patris
-000173c0: 7469 635f 696e 666f 3d70 6174 7269 7374  tic_info=patrist
-000173d0: 6963 5f69 6e66 6f2c 0a20 2020 2020 2020  ic_info,.       
+000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173c0: 7061 7472 6973 7469 635f 696e 666f 3d70  patristic_info=p
+000173d0: 6174 7269 7374 6963 5f69 6e66 6f2c 0a20  atristic_info,. 
 000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 2020 2020 2020 2020 2020 2020 2020 6772                gr
-00017400: 6170 685f 636f 6f3d 6772 6170 685f 636f  aph_coo=graph_co
-00017410: 6f2c 0a20 2020 2020 2020 2020 2020 2020  o,.             
+000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017400: 2020 2020 6772 6170 685f 636f 6f3d 6772      graph_coo=gr
+00017410: 6170 685f 636f 6f2c 0a20 2020 2020 2020  aph_coo,.       
 00017420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017430: 2020 2020 2020 2020 7061 7472 6973 7469          patristi
-00017440: 635f 6675 6c6c 5f73 7061 7273 6520 3d20  c_full_sparse = 
-00017450: 6564 6765 5f77 6569 6768 745f 6d61 7472  edge_weight_matr
-00017460: 6978 2c0a 2020 2020 2020 2020 2020 2020  ix,.            
+00017430: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00017440: 7472 6973 7469 635f 6675 6c6c 5f73 7061  tristic_full_spa
+00017450: 7273 6520 3d20 6564 6765 5f77 6569 6768  rse = edge_weigh
+00017460: 745f 6d61 7472 6978 2c0a 2020 2020 2020  t_matrix,.      
 00017470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017480: 2020 2020 2020 2020 206e 6f64 6573 5f72           nodes_r
-00017490: 6570 7265 7365 6e74 6174 696f 6e73 5f61  epresentations_a
-000174a0: 7272 6179 3d74 6f72 6368 2e66 726f 6d5f  rray=torch.from_
-000174b0: 6e75 6d70 7928 6e6f 6465 735f 7265 7072  numpy(nodes_repr
-000174c0: 6573 656e 7461 7469 6f6e 735f 6172 7261  esentations_arra
-000174d0: 7929 2c0a 2020 2020 2020 2020 2020 2020  y),.            
+00017480: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00017490: 6f64 6573 5f72 6570 7265 7365 6e74 6174  odes_representat
+000174a0: 696f 6e73 5f61 7272 6179 3d74 6f72 6368  ions_array=torch
+000174b0: 2e66 726f 6d5f 6e75 6d70 7928 6e6f 6465  .from_numpy(node
+000174c0: 735f 7265 7072 6573 656e 7461 7469 6f6e  s_representation
+000174d0: 735f 6172 7261 7929 2c0a 2020 2020 2020  s_array),.      
 000174e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174f0: 2020 2020 2020 2020 2064 676c 5f67 7261           dgl_gra
-00017500: 7068 3d64 676c 5f67 7261 7068 290a 0a0a  ph=dgl_graph)...
-00017510: 2020 2020 7265 7475 726e 2061 6464 6974      return addit
-00017520: 696f 6e61 6c5f 696e 666f 0a64 6566 2063  ional_info.def c
-00017530: 7265 6174 655f 7472 6565 5f62 795f 6c65  reate_tree_by_le
-00017540: 7665 6c73 2863 6869 6c64 7265 6e5f 6469  vels(children_di
-00017550: 6374 293a 0a20 2020 2022 2222 416c 7465  ct):.    """Alte
-00017560: 726e 6174 6976 6520 6d65 7468 6f64 2074  rnative method t
-00017570: 6f20 6275 696c 6420 7468 6520 7472 6565  o build the tree
-00017580: 2062 7920 6c65 7665 6c73 2061 7320 7375   by levels as su
-00017590: 6767 6573 7465 6420 6279 2052 6f62 6572  ggested by Rober
-000175a0: 7422 2222 0a20 2020 2074 7265 655f 6c65  t""".    tree_le
-000175b0: 7665 6c73 203d 205b 5b30 5d5d 0a20 2020  vels = [[0]].   
-000175c0: 2063 7572 7265 6e74 5f6e 6f64 6573 203d   current_nodes =
-000175d0: 205b 305d 0a20 2020 2077 6869 6c65 206c   [0].    while l
-000175e0: 656e 2863 7572 7265 6e74 5f6e 6f64 6573  en(current_nodes
-000175f0: 2920 3e20 303a 0a20 2020 2020 2020 2063  ) > 0:.        c
-00017600: 6869 6c64 7265 6e5f 6e6f 6465 7320 3d20  hildren_nodes = 
-00017610: 5b5d 0a20 2020 2020 2020 2066 6f72 206e  [].        for n
-00017620: 6f64 6520 696e 2063 7572 7265 6e74 5f6e  ode in current_n
-00017630: 6f64 6573 3a0a 2020 2020 2020 2020 2020  odes:.          
-00017640: 2020 6966 206e 6f64 6520 696e 2063 6869    if node in chi
-00017650: 6c64 7265 6e5f 6469 6374 2e6b 6579 7328  ldren_dict.keys(
-00017660: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017670: 2020 2063 6869 6c64 7265 6e5f 6e6f 6465     children_node
-00017680: 7320 2b3d 2063 6869 6c64 7265 6e5f 6469  s += children_di
-00017690: 6374 5b6e 6f64 655d 0a0a 2020 2020 2020  ct[node]..      
-000176a0: 2020 7472 6565 5f6c 6576 656c 732e 6170    tree_levels.ap
-000176b0: 7065 6e64 2863 6869 6c64 7265 6e5f 6e6f  pend(children_no
-000176c0: 6465 7329 0a20 2020 2020 2020 2063 7572  des).        cur
-000176d0: 7265 6e74 5f6e 6f64 6573 203d 2063 6869  rent_nodes = chi
-000176e0: 6c64 7265 6e5f 6e6f 6465 730a 0a20 2020  ldren_nodes..   
-000176f0: 2072 6574 7572 6e20 7472 6565 5f6c 6576   return tree_lev
-00017700: 656c 730a 636c 6173 7320 4d79 4461 7461  els.class MyData
-00017710: 7365 7428 4461 7461 7365 7429 3a23 544f  set(Dataset):#TO
-00017720: 444f 3a20 7265 6d6f 7665 0a20 2020 2064  DO: remove.    d
-00017730: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00017740: 2c6c 6162 656c 732c 6461 7461 5f61 7272  ,labels,data_arr
-00017750: 6179 7329 3a0a 2020 2020 2020 2020 7365  ays):.        se
-00017760: 6c66 2e6c 6162 656c 7320 3d20 6c61 6265  lf.labels = labe
-00017770: 6c73 0a20 2020 2020 2020 2073 656c 662e  ls.        self.
-00017780: 6461 7461 5f61 7272 6179 7320 3d20 6461  data_arrays = da
-00017790: 7461 5f61 7272 6179 730a 0a20 2020 2064  ta_arrays..    d
-000177a0: 6566 205f 5f67 6574 6974 656d 5f5f 2873  ef __getitem__(s
-000177b0: 656c 662c 2069 6e64 6578 293a 2023 7365  elf, index): #se
-000177c0: 7473 2061 5b69 5d0a 2020 2020 2020 2020  ts a[i].        
-000177d0: 6c61 6265 6c20 3d20 7365 6c66 2e6c 6162  label = self.lab
-000177e0: 656c 735b 696e 6465 785d 0a20 2020 2020  els[index].     
-000177f0: 2020 2064 6174 6120 3d20 7365 6c66 2e64     data = self.d
-00017800: 6174 615f 6172 7261 7973 5b69 6e64 6578  ata_arrays[index
-00017810: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-00017820: 207b 2766 616d 696c 795f 6e61 6d65 273a   {'family_name':
-00017830: 206c 6162 656c 2c20 2766 616d 696c 795f   label, 'family_
-00017840: 6461 7461 273a 2064 6174 617d 0a20 2020  data': data}.   
-00017850: 2064 6566 205f 5f6c 656e 5f5f 2873 656c   def __len__(sel
-00017860: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00017870: 726e 206c 656e 2873 656c 662e 6c61 6265  rn len(self.labe
-00017880: 6c73 290a 6465 6620 6465 6669 6e65 5f62  ls).def define_b
-00017890: 6174 6368 5f73 697a 6528 6e2c 6261 7463  atch_size(n,batc
-000178a0: 685f 7369 7a65 3d54 7275 652c 2062 656e  h_size=True, ben
-000178b0: 6368 6d61 726b 696e 673d 4661 6c73 6529  chmarking=False)
-000178c0: 3a0a 2020 2020 2222 2241 7574 6f6d 6174  :.    """Automat
-000178d0: 6963 2063 616c 6375 6c61 7469 6f6e 2074  ic calculation t
-000178e0: 6865 2061 7661 696c 6162 6c65 2064 6976  he available div
-000178f0: 6973 6f72 7320 6f66 2074 6865 206e 756d  isors of the num
-00017900: 6265 7220 6f66 2074 7261 696e 696e 6720  ber of training 
-00017910: 6461 7461 2070 6f69 6e74 7320 286e 292e  data points (n).
-00017920: 0a20 2020 2054 6869 7320 6865 6c70 7320  .    This helps 
-00017930: 746f 2073 7567 6765 7374 2061 6e20 6170  to suggest an ap
-00017940: 7072 6f70 6961 7465 2069 6e74 6567 6572  propiate integer
-00017950: 2062 6174 6368 2073 697a 6520 6e75 6d62   batch size numb
-00017960: 6572 2c20 7468 6174 2073 706c 6974 7320  er, that splits 
-00017970: 6576 656e 6c79 2074 6865 2064 6174 610a  evenly the data.
-00017980: 2020 2020 3a70 6172 616d 2069 6e74 206e      :param int n
-00017990: 3a20 6e75 6d62 6572 206f 6620 7365 7175  : number of sequ
-000179a0: 656e 6365 730a 2020 2020 3a70 6172 616d  ences.    :param
-000179b0: 2062 6f6f 6c20 6261 7463 685f 7369 7a65   bool batch_size
-000179c0: 0a20 2020 203a 7061 7261 6d20 6265 6e63  .    :param benc
-000179d0: 686d 6172 6b69 6e67 2222 220a 2020 2020  hmarking""".    
-000179e0: 6966 206e 6f74 2062 656e 6368 6d61 726b  if not benchmark
-000179f0: 696e 673a 0a20 2020 2020 2020 2061 7373  ing:.        ass
-00017a00: 6572 7420 6e20 3e3d 2031 3030 202c 224e  ert n >= 100 ,"N
-00017a10: 6f74 2077 6f72 7468 2062 6174 6368 696e  ot worth batchin
-00017a20: 672c 206e 756d 6265 7220 6f66 2073 6571  g, number of seq
-00017a30: 7565 6e63 6573 2069 7320 3c20 3130 3020  uences is < 100 
-00017a40: 220a 2020 2020 6469 7669 736f 7273 203d  ".    divisors =
-00017a50: 2044 7261 7570 6e69 724d 6f64 656c 5574   DraupnirModelUt
-00017a60: 696c 732e 7072 696e 745f 6469 7669 736f  ils.print_diviso
-00017a70: 7273 286e 290a 2020 2020 6e5f 6469 6769  rs(n).    n_digi
-00017a80: 7473 203d 206c 656e 286c 6973 7428 7374  ts = len(list(st
-00017a90: 7228 6e29 2929 2023 2031 3030 2068 6173  r(n))) # 100 has
-00017aa0: 2033 2064 6967 6974 732c 2031 3030 3020   3 digits, 1000 
-00017ab0: 6861 7320 3420 6469 6769 7473 2c20 3130  has 4 digits, 10
-00017ac0: 3030 3020 6861 7320 3520 6469 6769 7473  000 has 5 digits
-00017ad0: 2061 6e64 2073 6f20 6f6e 0a20 2020 206e   and so on.    n
-00017ae0: 5f63 6875 6e6b 7320 3d20 5b6d 696e 2864  _chunks = [min(d
-00017af0: 6976 6973 6f72 735b 6e5f 6469 6769 7473  ivisors[n_digits
-00017b00: 2d31 3a5d 2920 6966 206c 656e 2864 6976  -1:]) if len(div
-00017b10: 6973 6f72 7329 203e 206e 5f64 6967 6974  isors) > n_digit
-00017b20: 732d 3120 656c 7365 2031 5d5b 305d 2020  s-1 else 1][0]  
-00017b30: 2320 736d 616c 6c65 7374 2064 6976 6973  # smallest divis
-00017b40: 6f72 2074 6861 7420 6973 206e 6f74 2031  or that is not 1
-00017b50: 2c20 6f72 206a 7573 7420 7573 6520 3120  , or just use 1 
-00017b60: 2c20 7768 656e 206e 6f20 6f74 6865 7220  , when no other 
-00017b70: 6469 7669 736f 7273 2061 7265 2061 7661  divisors are ava
-00017b80: 696c 6162 6c65 2028 7072 696d 6520 6e75  ilable (prime nu
-00017b90: 6d62 6572 7329 0a20 2020 2062 6174 6368  mbers).    batch
-00017ba0: 7369 7a65 203d 2069 6e74 2844 7261 7570  size = int(Draup
-00017bb0: 6e69 724d 6f64 656c 5574 696c 732e 696e  nirModelUtils.in
-00017bc0: 7465 7276 616c 7328 6e5f 6368 756e 6b73  tervals(n_chunks
-00017bd0: 2c20 6e29 5b30 5d5b 315d 290a 2020 2020  , n)[0][1]).    
-00017be0: 6966 2062 6174 6368 5f73 697a 653a 7265  if batch_size:re
-00017bf0: 7475 726e 2062 6174 6368 7369 7a65 0a20  turn batchsize. 
-00017c00: 2020 2065 6c73 653a 7265 7475 726e 206e     else:return n
-00017c10: 5f63 6875 6e6b 730a 6465 6620 636f 7661  _chunks.def cova
-00017c20: 7269 616e 6365 2878 2c79 293a 0a20 2020  riance(x,y):.   
-00017c30: 2022 2222 436f 6d70 7574 6573 2063 726f   """Computes cro
-00017c40: 7373 2d63 6f76 6172 6961 6e63 6520 6265  ss-covariance be
-00017c50: 7477 6565 6e20 7665 6374 6f72 732c 2061  tween vectors, a
-00017c60: 6e64 2069 7320 6465 6669 6e65 6420 6279  nd is defined by
-00017c70: 2063 6f76 5b58 2c59 5d3d 455b 2858 e288   cov[X,Y]=E[(X..
-00017c80: 92ce bc58 2928 59e2 8892 cebc 5929 545d  ...X)(Y.....Y)T]
-00017c90: 2222 220a 2020 2020 4120 3d20 746f 7263  """.    A = torc
-00017ca0: 682e 7371 7274 2874 6f72 6368 2e61 7261  h.sqrt(torch.ara
-00017cb0: 6e67 6528 3132 292e 7265 7368 6170 6528  nge(12).reshape(
-00017cc0: 332c 2034 2929 2020 2320 736f 6d65 2033  3, 4))  # some 3
-00017cd0: 2062 7920 3420 6172 7261 790a 2020 2020   by 4 array.    
-00017ce0: 6220 3d20 746f 7263 682e 7465 6e73 6f72  b = torch.tensor
-00017cf0: 285b 5b32 5d2c 205b 345d 2c20 5b35 5d5d  ([[2], [4], [5]]
-00017d00: 2920 2023 2073 6f6d 6520 3320 6279 2031  )  # some 3 by 1
-00017d10: 2076 6563 746f 720a 2020 2020 636f 7620   vector.    cov 
-00017d20: 3d20 746f 7263 682e 646f 7428 622e 5420  = torch.dot(b.T 
-00017d30: 2d20 622e 6d65 616e 2829 2c20 4120 2d20  - b.mean(), A - 
-00017d40: 412e 6d65 616e 2864 696d 3d30 2929 202f  A.mean(dim=0)) /
-00017d50: 2028 622e 7368 6170 655b 305d 202d 2031   (b.shape[0] - 1
-00017d60: 290a 2020 2020 7265 7475 726e 2063 6f76  ).    return cov
-00017d70: 0a64 6566 2066 696e 645f 6e61 6e28 6172  .def find_nan(ar
-00017d80: 7261 792c 6e61 6e3d 5472 7565 293a 0a20  ray,nan=True):. 
-00017d90: 2020 2022 2222 4472 6f70 7320 726f 7773     """Drops rows
-00017da0: 2069 6e20 6120 7465 6e73 6f72 2063 6f6e   in a tensor con
-00017db0: 7461 696e 696e 6720 616e 7920 6e61 6e20  taining any nan 
-00017dc0: 7661 6c75 6573 0a20 2020 203a 7061 7261  values.    :para
-00017dd0: 6d20 7465 6e73 6f72 2061 7272 6179 2222  m tensor array""
-00017de0: 220a 2020 2020 7368 6170 6520 3d20 6172  ".    shape = ar
-00017df0: 7261 792e 7368 6170 650a 2020 2020 7465  ray.shape.    te
-00017e00: 6e73 6f72 5f72 6573 6861 7065 6420 3d20  nsor_reshaped = 
-00017e10: 6172 7261 792e 7265 7368 6170 6528 7368  array.reshape(sh
-00017e20: 6170 655b 305d 2c20 2d31 290a 2020 2020  ape[0], -1).    
-00017e30: 2320 4472 6f70 2061 6c6c 2072 6f77 7320  # Drop all rows 
-00017e40: 636f 6e74 6169 6e69 6e67 2061 6e79 206e  containing any n
-00017e50: 616e 3a0a 2020 2020 6966 206e 6f74 206e  an:.    if not n
-00017e60: 616e 3a0a 2020 2020 2020 2020 7465 6e73  an:.        tens
-00017e70: 6f72 5f72 6573 6861 7065 6420 3d20 7465  or_reshaped = te
-00017e80: 6e73 6f72 5f72 6573 6861 7065 645b 7e74  nsor_reshaped[~t
-00017e90: 6f72 6368 2e61 6e79 2874 656e 736f 725f  orch.any(tensor_
-00017ea0: 7265 7368 6170 6564 2e69 736e 616e 2829  reshaped.isnan()
-00017eb0: 2c20 6469 6d3d 3129 5d0a 2020 2020 656c  , dim=1)].    el
-00017ec0: 7365 3a0a 2020 2020 2020 2020 7465 6e73  se:.        tens
-00017ed0: 6f72 5f72 6573 6861 7065 6420 3d20 7465  or_reshaped = te
-00017ee0: 6e73 6f72 5f72 6573 6861 7065 645b 746f  nsor_reshaped[to
-00017ef0: 7263 682e 616e 7928 7465 6e73 6f72 5f72  rch.any(tensor_r
-00017f00: 6573 6861 7065 642e 6973 6e61 6e28 292c  eshaped.isnan(),
-00017f10: 2064 696d 3d31 295d 0a20 2020 2023 2052   dim=1)].    # R
-00017f20: 6573 6861 7065 2062 6163 6b3a 0a20 2020  eshape back:.   
-00017f30: 2061 7272 6179 203d 2074 656e 736f 725f   array = tensor_
-00017f40: 7265 7368 6170 6564 2e72 6573 6861 7065  reshaped.reshape
-00017f50: 2874 656e 736f 725f 7265 7368 6170 6564  (tensor_reshaped
-00017f60: 2e73 6861 7065 5b30 5d2c 202a 7368 6170  .shape[0], *shap
-00017f70: 655b 313a 5d29 0a20 2020 2072 6574 7572  e[1:]).    retur
-00017f80: 6e20 6172 7261 790a 6465 6620 7261 6d61  n array.def rama
-00017f90: 6368 616e 6472 616e 5f70 6c6f 7428 2064  chandran_plot( d
-00017fa0: 6174 615f 616e 676c 6573 2c73 6176 655f  ata_angles,save_
-00017fb0: 6469 7265 6374 6f72 792c 706c 6f74 5f74  directory,plot_t
-00017fc0: 6974 6c65 2c20 6f6e 655f 686f 745f 656e  itle, one_hot_en
-00017fd0: 636f 6465 6420 3d20 4661 6c73 6520 293a  coded = False ):
-00017fe0: 0a20 2020 2022 2222 506c 6f74 7320 5261  .    """Plots Ra
-00017ff0: 6d61 6368 616e 6472 616e 2070 6c6f 7473  machandran plots
-00018000: 2062 6574 7765 656e 2074 6865 2070 6869   between the phi
-00018010: 2061 6e64 2070 7369 2061 6e67 6c65 7320   and psi angles 
-00018020: 696e 2074 6865 2064 6174 6173 6574 0a20  in the dataset. 
-00018030: 2020 203a 7061 7261 6d20 6e75 6d70 792d     :param numpy-
-00018040: 6172 7261 7920 6461 7461 5f61 6e67 6c65  array data_angle
-00018050: 7320 3a20 3364 2061 7272 6179 205b 6e5f  s : 3d array [n_
-00018060: 7365 712c 2061 6c69 676e 5f6c 656e 2c20  seq, align_len, 
-00018070: 3330 5d2c 2077 6865 7265 2063 6f6c 756d  30], where colum
-00018080: 6e73 2031 2061 6e64 2032 206f 7220 3231  ns 1 and 2 or 21
-00018090: 2061 6e64 2032 3220 636f 6e74 6169 6e20   and 22 contain 
-000180a0: 7468 6520 616e 676c 6573 2069 6e20 7468  the angles in th
-000180b0: 6520 6361 7365 206f 6620 4e4f 5420 6f6e  e case of NOT on
-000180c0: 652d 686f 7420 656e 636f 6465 6420 616e  e-hot encoded an
-000180d0: 6420 6f6e 652d 686f 7420 656e 636f 6465  d one-hot encode
-000180e0: 642c 2072 6573 7065 6374 6976 656c 790a  d, respectively.
-000180f0: 2020 2020 3a70 6172 616d 2073 7472 2073      :param str s
-00018100: 6176 655f 6469 7265 6374 6f72 793a 2070  ave_directory: p
-00018110: 6174 6820 746f 2073 6176 696e 6720 6469  ath to saving di
-00018120: 7265 6374 6f72 790a 2020 2020 3a70 6172  rectory.    :par
-00018130: 616d 2073 7472 2070 6c6f 745f 7469 746c  am str plot_titl
-00018140: 650a 2020 2020 3a70 6172 616d 2062 6f6f  e.    :param boo
-00018150: 6c20 6f6e 655f 686f 745f 656e 636f 6465  l one_hot_encode
-00018160: 640a 2020 2020 2222 220a 2020 2020 706c  d.    """.    pl
-00018170: 742e 636c 6628 290a 2020 2020 6966 206f  t.clf().    if o
-00018180: 6e65 5f68 6f74 5f65 6e63 6f64 6564 3a0a  ne_hot_encoded:.
-00018190: 2020 2020 2020 2020 7068 6920 3d20 6461          phi = da
-000181a0: 7461 5f61 6e67 6c65 735b 3a2c 3a2c 3231  ta_angles[:,:,21
-000181b0: 5d2e 7265 7368 6170 6528 2864 6174 615f  ].reshape((data_
-000181c0: 616e 676c 6573 2e73 6861 7065 5b30 5d2a  angles.shape[0]*
-000181d0: 6461 7461 5f61 6e67 6c65 732e 7368 6170  data_angles.shap
-000181e0: 655b 315d 2929 2e61 7374 7970 6528 666c  e[1])).astype(fl
-000181f0: 6f61 7429 2023 2d20 6e70 2e70 690a 0a20  oat) #- np.pi.. 
-00018200: 2020 2020 2020 2070 7369 203d 2064 6174         psi = dat
-00018210: 615f 616e 676c 6573 5b3a 2c3a 2c32 325d  a_angles[:,:,22]
-00018220: 2e72 6573 6861 7065 2828 6461 7461 5f61  .reshape((data_a
-00018230: 6e67 6c65 732e 7368 6170 655b 305d 2a64  ngles.shape[0]*d
-00018240: 6174 615f 616e 676c 6573 2e73 6861 7065  ata_angles.shape
-00018250: 5b31 5d29 292e 6173 7479 7065 2866 6c6f  [1])).astype(flo
-00018260: 6174 2920 232d 206e 702e 7069 0a20 2020  at) #- np.pi.   
-00018270: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
-00018280: 6869 203d 2064 6174 615f 616e 676c 6573  hi = data_angles
-00018290: 5b3a 2c3a 2c31 5d2e 7265 7368 6170 6528  [:,:,1].reshape(
-000182a0: 2864 6174 615f 616e 676c 6573 2e73 6861  (data_angles.sha
-000182b0: 7065 5b30 5d2a 6461 7461 5f61 6e67 6c65  pe[0]*data_angle
-000182c0: 732e 7368 6170 655b 315d 2929 2e61 7374  s.shape[1])).ast
-000182d0: 7970 6528 666c 6f61 7429 0a20 2020 2020  ype(float).     
-000182e0: 2020 2070 7369 203d 2064 6174 615f 616e     psi = data_an
-000182f0: 676c 6573 5b3a 2c3a 2c32 5d2e 7265 7368  gles[:,:,2].resh
-00018300: 6170 6528 2864 6174 615f 616e 676c 6573  ape((data_angles
-00018310: 2e73 6861 7065 5b30 5d2a 6461 7461 5f61  .shape[0]*data_a
-00018320: 6e67 6c65 732e 7368 6170 655b 315d 2929  ngles.shape[1]))
-00018330: 2e61 7374 7970 6528 666c 6f61 7429 0a0a  .astype(float)..
-00018340: 2020 2020 6669 6720 3d20 706c 742e 6669      fig = plt.fi
-00018350: 6775 7265 2866 6967 7369 7a65 3d28 352c  gure(figsize=(5,
-00018360: 3529 290a 2020 2020 706c 742e 6869 7374  5)).    plt.hist
-00018370: 3264 2820 7068 692c 2070 7369 2c20 6269  2d( phi, psi, bi
-00018380: 6e73 203d 2036 3238 2c20 6e6f 726d 203d  ns = 628, norm =
-00018390: 204c 6f67 4e6f 726d 2829 2923 2c20 636d   LogNorm())#, cm
-000183a0: 6170 203d 2070 6c74 2e63 6d2e 6a65 7420  ap = plt.cm.jet 
-000183b0: 290a 2020 2020 706c 742e 796c 696d 282d  ).    plt.ylim(-
-000183c0: 6e70 2e70 692c 206e 702e 7069 290a 2020  np.pi, np.pi).  
-000183d0: 2020 706c 742e 786c 696d 282d 6e70 2e70    plt.xlim(-np.p
-000183e0: 692c 206e 702e 7069 290a 2020 2020 706c  i, np.pi).    pl
-000183f0: 742e 7469 746c 6528 706c 6f74 5f74 6974  t.title(plot_tit
-00018400: 6c65 2c66 6f6e 7473 697a 653d 3132 290a  le,fontsize=12).
-00018410: 2020 2020 706c 742e 786c 6162 656c 2827      plt.xlabel('
-00018420: cf86 2729 0a20 2020 2070 6c74 2e79 6c61  ..').    plt.yla
-00018430: 6265 6c28 27cf 8827 290a 2020 2020 706c  bel('..').    pl
-00018440: 742e 7361 7665 6669 6728 7361 7665 5f64  t.savefig(save_d
-00018450: 6972 6563 746f 7279 290a 2020 2020 706c  irectory).    pl
-00018460: 742e 636c 6628 290a 2020 2020 706c 742e  t.clf().    plt.
-00018470: 636c 6f73 6528 6669 6729 0a64 6566 2072  close(fig).def r
-00018480: 616d 6163 6861 6e64 7261 6e5f 706c 6f74  amachandran_plot
-00018490: 5f73 616d 706c 6564 2870 6869 2c70 7369  _sampled(phi,psi
-000184a0: 2c73 6176 655f 6469 7265 6374 6f72 792c  ,save_directory,
-000184b0: 706c 6f74 5f74 6974 6c65 2c70 6c6f 745f  plot_title,plot_
-000184c0: 6b61 7070 6173 3d46 616c 7365 293a 0a20  kappas=False):. 
-000184d0: 2020 2022 2222 506c 6f74 7320 5261 6d61     """Plots Rama
-000184e0: 6368 616e 6472 616e 2070 6c6f 7473 2062  chandran plots b
-000184f0: 6574 7765 656e 2074 6865 2070 6869 2061  etween the phi a
-00018500: 6e64 2070 7369 2061 6e67 6c65 7320 696e  nd psi angles in
-00018510: 2074 6865 2064 6174 6173 6574 0a20 2020   the dataset.   
-00018520: 203a 7061 7261 6d20 7465 6e73 6f72 2070   :param tensor p
-00018530: 6869 0a20 2020 203a 7061 7261 6d20 7465  hi.    :param te
-00018540: 6e73 6f72 2070 7369 0a20 2020 203a 7061  nsor psi.    :pa
-00018550: 7261 6d20 7374 7220 7361 7665 5f64 6972  ram str save_dir
-00018560: 6563 746f 7279 3a20 7061 7468 2074 6f20  ectory: path to 
-00018570: 7361 7669 6e67 2064 6972 6563 746f 7279  saving directory
-00018580: 0a20 2020 203a 7061 7261 6d20 7374 7220  .    :param str 
-00018590: 706c 6f74 5f74 6974 6c65 0a20 2020 203a  plot_title.    :
-000185a0: 7061 7261 6d20 626f 6f6c 2070 6c6f 745f  param bool plot_
-000185b0: 6b61 7070 6173 0a20 2020 2022 2222 0a20  kappas.    """. 
-000185c0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000185d0: 2870 6869 2c74 6f72 6368 2e54 656e 736f  (phi,torch.Tenso
-000185e0: 7229 3a0a 2020 2020 2020 2020 7068 6920  r):.        phi 
-000185f0: 3d20 7068 692e 7669 6577 282d 3129 2e63  = phi.view(-1).c
-00018600: 7075 2829 2e64 6574 6163 6828 292e 6e75  pu().detach().nu
-00018610: 6d70 7928 290a 2020 2020 2020 2020 7073  mpy().        ps
-00018620: 6920 3d20 7073 692e 7669 6577 282d 3129  i = psi.view(-1)
-00018630: 2e63 7075 2829 2e64 6574 6163 6828 292e  .cpu().detach().
-00018640: 6e75 6d70 7928 290a 2020 2020 2361 7865  numpy().    #axe
-00018650: 7320 3d20 5b5b 2d6e 702e 7069 2c20 6e70  s = [[-np.pi, np
-00018660: 2e70 695d 2c20 5b2d 6e70 2e70 692c 206e  .pi], [-np.pi, n
-00018670: 702e 7069 5d5d 0a20 2020 2070 6c74 2e66  p.pi]].    plt.f
-00018680: 6967 7572 6528 6669 6773 697a 653d 2835  igure(figsize=(5
-00018690: 2c35 2929 0a20 2020 2070 6c74 2e68 6973  ,5)).    plt.his
-000186a0: 7432 6428 2070 6869 2c20 7073 692c 2062  t2d( phi, psi, b
-000186b0: 696e 7320 3d20 3632 382c 206e 6f72 6d20  ins = 628, norm 
-000186c0: 3d20 4c6f 674e 6f72 6d28 2929 232c 2063  = LogNorm())#, c
-000186d0: 6d61 7020 3d20 706c 742e 636d 2e6a 6574  map = plt.cm.jet
-000186e0: 2029 0a20 2020 2069 6620 706c 6f74 5f6b   ).    if plot_k
-000186f0: 6170 7061 733a 0a20 2020 2020 2020 2070  appas:.        p
-00018700: 6c74 2e78 6c61 6265 6c28 274b 6170 7061  lt.xlabel('Kappa
-00018710: 20cf 8627 290a 2020 2020 2020 2020 706c   ..').        pl
-00018720: 742e 796c 6162 656c 2827 4b61 7070 6120  t.ylabel('Kappa 
-00018730: cf88 2729 0a20 2020 2065 6c73 653a 0a20  ..').    else:. 
-00018740: 2020 2020 2020 2070 6c74 2e79 6c69 6d28         plt.ylim(
-00018750: 2d6e 702e 7069 2c20 6e70 2e70 6929 0a20  -np.pi, np.pi). 
-00018760: 2020 2020 2020 2070 6c74 2e78 6c69 6d28         plt.xlim(
-00018770: 2d6e 702e 7069 2c20 6e70 2e70 6929 0a20  -np.pi, np.pi). 
-00018780: 2020 2020 2020 2070 6c74 2e78 6c61 6265         plt.xlabe
-00018790: 6c28 27cf 8627 290a 2020 2020 2020 2020  l('..').        
-000187a0: 706c 742e 796c 6162 656c 2827 cf88 2729  plt.ylabel('..')
-000187b0: 0a20 2020 2070 6c74 2e74 6974 6c65 2870  .    plt.title(p
-000187c0: 6c6f 745f 7469 746c 652c 666f 6e74 7369  lot_title,fontsi
-000187d0: 7a65 3d31 3229 0a20 2020 2070 6c74 2e73  ze=12).    plt.s
-000187e0: 6176 6566 6967 2873 6176 655f 6469 7265  avefig(save_dire
-000187f0: 6374 6f72 7929 0a20 2020 2070 6c74 2e63  ctory).    plt.c
-00018800: 6c66 2829 0a20 2020 2070 6c74 2e63 6c6f  lf().    plt.clo
-00018810: 7365 2829 0a64 6566 2067 7261 6469 656e  se().def gradien
-00018820: 7473 5f70 6c6f 7428 6772 6164 6965 6e74  ts_plot(gradient
-00018830: 5f6e 6f72 6d73 2c65 706f 6368 732c 6469  _norms,epochs,di
-00018840: 7265 6374 6f72 7929 3a0a 2020 2020 2222  rectory):.    ""
-00018850: 2256 6973 7561 6c69 7a61 7469 6f6e 206f  "Visualization o
-00018860: 6620 7468 6520 6772 6164 6965 6e74 2064  f the gradient d
-00018870: 6573 6365 6e74 2070 6572 206d 6f64 656c  escent per model
-00018880: 2070 6172 616d 6574 6572 0a20 2020 203a   parameter.    :
-00018890: 7061 7261 6d20 6469 6374 2067 7261 6469  param dict gradi
-000188a0: 656e 745f 6e6f 726d 733a 2064 6963 7469  ent_norms: dicti
-000188b0: 6f6e 6172 7920 7769 7468 2074 6865 206d  onary with the m
-000188c0: 6f64 656c 2070 6172 616d 6574 6572 7320  odel parameters 
-000188d0: 616e 6420 7468 6520 7061 7274 6961 6c20  and the partial 
-000188e0: 6465 7269 7661 7469 7665 730a 2020 2020  derivatives.    
-000188f0: 3a70 6172 616d 2069 6e74 2065 706f 6368  :param int epoch
-00018900: 7322 2222 0a0a 2020 2020 6669 6720 3d20  s"""..    fig = 
-00018910: 706c 742e 6669 6775 7265 2866 6967 7369  plt.figure(figsi
-00018920: 7a65 3d28 3136 2c20 3929 2c20 6470 693d  ze=(16, 9), dpi=
-00018930: 3130 3029 2e73 6574 5f66 6163 6563 6f6c  100).set_facecol
-00018940: 6f72 2827 7768 6974 6527 290a 2020 2020  or('white').    
-00018950: 6178 203d 2070 6c74 2e73 7562 706c 6f74  ax = plt.subplot
-00018960: 2831 3231 290a 2020 2020 636f 6c6f 725f  (121).    color_
-00018970: 6d61 7020 3d20 636d 2e72 6169 6e62 6f77  map = cm.rainbow
-00018980: 286e 702e 6c69 6e73 7061 6365 2830 2c20  (np.linspace(0, 
-00018990: 312c 2034 3229 290a 2020 2020 666f 7220  1, 42)).    for 
-000189a0: 286e 616d 655f 692c 2067 7261 645f 6e6f  (name_i, grad_no
-000189b0: 726d 7329 2c20 636f 6c6f 7220 696e 207a  rms), color in z
-000189c0: 6970 2867 7261 6469 656e 745f 6e6f 726d  ip(gradient_norm
-000189d0: 732e 6974 656d 7328 292c 2063 6f6c 6f72  s.items(), color
-000189e0: 5f6d 6170 293a 0a20 2020 2020 2020 2061  _map):.        a
-000189f0: 782e 706c 6f74 2867 7261 645f 6e6f 726d  x.plot(grad_norm
-00018a00: 732c 206c 6162 656c 3d6e 616d 655f 692c  s, label=name_i,
-00018a10: 2063 3d63 6f6c 6f72 290a 2020 2020 706c   c=color).    pl
-00018a20: 742e 786c 6162 656c 2827 6974 6572 7327  t.xlabel('iters'
-00018a30: 290a 2020 2020 706c 742e 796c 6162 656c  ).    plt.ylabel
-00018a40: 2827 6772 6164 6965 6e74 206e 6f72 6d27  ('gradient norm'
-00018a50: 290a 2020 2020 706c 742e 7973 6361 6c65  ).    plt.yscale
-00018a60: 2827 6c6f 6727 290a 2020 2020 6178 2e6c  ('log').    ax.l
-00018a70: 6567 656e 6428 6c6f 633d 2775 7070 6572  egend(loc='upper
-00018a80: 2063 656e 7465 7227 2c20 6262 6f78 5f74   center', bbox_t
-00018a90: 6f5f 616e 6368 6f72 3d28 312e 352c 2031  o_anchor=(1.5, 1
-00018aa0: 292c 2073 6861 646f 773d 5472 7565 2c20  ), shadow=True, 
-00018ab0: 6e63 6f6c 3d31 2c20 7072 6f70 3d7b 2773  ncol=1, prop={'s
-00018ac0: 697a 6527 3a20 387d 290a 2020 2020 706c  ize': 8}).    pl
-00018ad0: 742e 7469 746c 6528 2747 7261 6469 656e  t.title('Gradien
-00018ae0: 7420 6e6f 726d 7320 6475 7269 6e67 2053  t norms during S
-00018af0: 5649 2729 0a20 2020 2070 6c74 2e73 6176  VI').    plt.sav
-00018b00: 6566 6967 2822 7b7d 2f47 7261 6469 656e  efig("{}/Gradien
-00018b10: 7473 5f7b 7d5f 6570 6f63 6873 2e70 6e67  ts_{}_epochs.png
-00018b20: 222e 666f 726d 6174 2864 6972 6563 746f  ".format(directo
-00018b30: 7279 2c65 706f 6368 7329 290a 2020 2020  ry,epochs)).    
-00018b40: 706c 742e 636c 6628 290a 2020 2020 706c  plt.clf().    pl
-00018b50: 742e 636c 6f73 6528 290a 0a64 6566 2072  t.close()..def r
-00018b60: 656e 616d 696e 6728 7472 6565 293a 0a20  enaming(tree):. 
-00018b70: 2020 2020 2020 2022 2222 5265 6e61 6d65         """Rename
-00018b80: 2074 6865 2069 6e74 6572 6e61 6c20 6e6f   the internal no
-00018b90: 6465 732c 2075 6e6c 6573 7320 7468 6520  des, unless the 
-00018ba0: 6769 7665 6e20 6e65 7769 636b 2066 696c  given newick fil
-00018bb0: 6520 616c 7265 6164 7920 6861 7320 7468  e already has th
-00018bc0: 6520 6e61 6d65 7320 6f6e 2069 740a 2020  e names on it.  
-00018bd0: 2020 2020 2020 3a70 6172 616d 2074 7265        :param tre
-00018be0: 653a 2065 7465 3320 666f 726d 6174 2031  e: ete3 format 1
-00018bf0: 2074 7265 6522 2222 0a20 2020 2020 2020   tree""".       
-00018c00: 2023 5265 6e61 6d65 2074 6865 2069 6e74   #Rename the int
-00018c10: 6572 6e61 6c20 6e6f 6465 730a 2020 2020  ernal nodes.    
-00018c20: 2020 2020 6c65 6166 735f 6e61 6d65 7320      leafs_names 
-00018c30: 3d20 7472 6565 2e67 6574 5f6c 6561 665f  = tree.get_leaf_
-00018c40: 6e61 6d65 7328 290a 2020 2020 2020 2020  names().        
-00018c50: 6564 6765 203d 206c 656e 286c 6561 6673  edge = len(leafs
-00018c60: 5f6e 616d 6573 290a 2020 2020 2020 2020  _names).        
-00018c70: 696e 7465 726e 616c 5f6e 6f64 6573 5f6e  internal_nodes_n
-00018c80: 616d 6573 203d 205b 5d0a 2020 2020 2020  ames = [].      
-00018c90: 2020 666f 7220 6e6f 6465 2069 6e20 7472    for node in tr
-00018ca0: 6565 2e74 7261 7665 7273 6528 293a 2023  ee.traverse(): #
-00018cb0: 6c65 7665 6c6f 7264 6572 2028 6e6f 6465  levelorder (node
-00018cc0: 7320 6172 6520 7669 7369 7465 6420 696e  s are visited in
-00018cd0: 207a 6967 207a 6167 206f 7264 6572 2066   zig zag order f
-00018ce0: 726f 6d20 726f 6f74 2074 6f20 6c65 6176  rom root to leav
-00018cf0: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
-00018d00: 6966 206e 6f74 206e 6f64 652e 6973 5f6c  if not node.is_l
-00018d10: 6561 6628 293a 0a20 2020 2020 2020 2020  eaf():.         
-00018d20: 2020 2020 2020 206e 6f64 652e 6e61 6d65         node.name
-00018d30: 203d 2022 4125 6422 2025 2065 6467 650a   = "A%d" % edge.
-00018d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d50: 696e 7465 726e 616c 5f6e 6f64 6573 5f6e  internal_nodes_n
-00018d60: 616d 6573 2e61 7070 656e 6428 6e6f 6465  ames.append(node
-00018d70: 2e6e 616d 6529 0a20 2020 2020 2020 2020  .name).         
-00018d80: 2020 2020 2020 2065 6467 6520 2b3d 2031         edge += 1
-00018d90: 0a0a 6465 6620 6361 6c63 756c 6174 655f  ..def calculate_
-00018da0: 6161 5f66 7265 7175 656e 6369 6573 2864  aa_frequencies(d
-00018db0: 6174 6173 6574 2c66 7265 715f 6269 6e73  ataset,freq_bins
-00018dc0: 293a 0a20 2020 2022 2222 4361 6c63 756c  ):.    """Calcul
-00018dd0: 6174 6573 2061 2066 7265 7175 656e 6379  ates a frequency
-00018de0: 2066 6f72 2065 6163 6820 6f66 2074 6865   for each of the
-00018df0: 2061 6120 2620 6761 7020 6174 2065 6163   aa & gap at eac
-00018e00: 6820 706f 7369 7469 6f6e 2e54 6865 206e  h position.The n
-00018e10: 756d 6265 7220 6f66 2062 696e 7320 286f  umber of bins (o
-00018e20: 6620 7369 7a65 2031 2920 6973 206f 6e65  f size 1) is one
-00018e30: 206c 6172 6765 7220 7468 616e 2074 6865   larger than the
-00018e40: 206c 6172 6765 7374 2076 616c 7565 2069   largest value i
-00018e50: 6e20 782e 2054 6869 7320 6973 2064 6f6e  n x. This is don
-00018e60: 6520 666f 7220 6e75 6d70 7920 6172 7261  e for numpy arra
-00018e70: 7973 0a20 2020 203a 7061 7261 6d20 7465  ys.    :param te
-00018e80: 6e73 6f72 2064 6174 6173 6574 0a20 2020  nsor dataset.   
-00018e90: 203a 7061 7261 6d20 696e 7420 6672 6571   :param int freq
-00018ea0: 5f62 696e 730a 2020 2020 2222 220a 2020  _bins.    """.  
-00018eb0: 2020 6672 6571 7320 3d20 6e70 2e61 7070    freqs = np.app
-00018ec0: 6c79 5f61 6c6f 6e67 5f61 7869 7328 6c61  ly_along_axis(la
-00018ed0: 6d62 6461 2078 3a20 6e70 2e62 696e 636f  mbda x: np.binco
-00018ee0: 756e 7428 782c 206d 696e 6c65 6e67 7468  unt(x, minlength
-00018ef0: 3d66 7265 715f 6269 6e73 292c 2061 7869  =freq_bins), axi
-00018f00: 733d 302c 2061 7272 3d64 6174 6173 6574  s=0, arr=dataset
-00018f10: 2e61 7374 7970 6528 2269 6e74 3634 2229  .astype("int64")
-00018f20: 292e 540a 2020 2020 6672 6571 7320 3d20  ).T.    freqs = 
-00018f30: 6672 6571 732f 6461 7461 7365 742e 7368  freqs/dataset.sh
-00018f40: 6170 655b 305d 0a20 2020 2072 6574 7572  ape[0].    retur
-00018f50: 6e20 6672 6571 730a 6465 6620 6361 6c63  n freqs.def calc
-00018f60: 756c 6174 655f 6161 5f66 7265 7175 656e  ulate_aa_frequen
-00018f70: 6369 6573 5f74 6f72 6368 2864 6174 6173  cies_torch(datas
-00018f80: 6574 2c66 7265 715f 6269 6e73 293a 0a20  et,freq_bins):. 
-00018f90: 2020 2022 2222 4361 6c63 756c 6174 6573     """Calculates
-00018fa0: 2061 2066 7265 7175 656e 6379 2066 6f72   a frequency for
-00018fb0: 2065 6163 6820 6f66 2074 6865 2061 6120   each of the aa 
-00018fc0: 2620 6761 7020 6174 2065 6163 6820 706f  & gap at each po
-00018fd0: 7369 7469 6f6e 2e54 6865 206e 756d 6265  sition.The numbe
-00018fe0: 7220 6f66 2062 696e 7320 286f 6620 7369  r of bins (of si
-00018ff0: 7a65 2031 2920 6973 206f 6e65 206c 6172  ze 1) is one lar
-00019000: 6765 7220 7468 616e 2074 6865 206c 6172  ger than the lar
-00019010: 6765 7374 2076 616c 7565 2069 6e20 782e  gest value in x.
-00019020: 2054 6869 7320 6973 2064 6f6e 6520 666f   This is done fo
-00019030: 7220 746f 7263 6820 7465 6e73 6f72 730a  r torch tensors.
-00019040: 2020 2020 3a70 6172 616d 2074 656e 736f      :param tenso
-00019050: 7220 6461 7461 7365 740a 2020 2020 3a70  r dataset.    :p
-00019060: 6172 616d 2069 6e74 2066 7265 715f 6269  aram int freq_bi
-00019070: 6e73 0a20 2020 2022 2222 0a20 2020 2066  ns.    """.    f
-00019080: 7265 7173 203d 2074 6f72 6368 2e73 7461  reqs = torch.sta
-00019090: 636b 285b 746f 7263 682e 6269 6e63 6f75  ck([torch.bincou
-000190a0: 6e74 2878 5f69 2c20 6d69 6e6c 656e 6774  nt(x_i, minlengt
-000190b0: 683d 6672 6571 5f62 696e 7329 2066 6f72  h=freq_bins) for
-000190c0: 2069 2c20 785f 6920 696e 2065 6e75 6d65   i, x_i in enume
-000190d0: 7261 7465 2874 6f72 6368 2e75 6e62 696e  rate(torch.unbin
-000190e0: 6428 6461 7461 7365 742e 7479 7065 2874  d(dataset.type(t
-000190f0: 6f72 6368 2e69 6e74 3634 292c 2064 696d  orch.int64), dim
-00019100: 3d31 292c 2030 295d 2c20 6469 6d3d 3129  =1), 0)], dim=1)
-00019110: 0a20 2020 2066 7265 7173 203d 2066 7265  .    freqs = fre
-00019120: 7173 2e54 0a20 2020 2066 7265 7173 203d  qs.T.    freqs =
-00019130: 2066 7265 7173 202f 2064 6174 6173 6574   freqs / dataset
-00019140: 2e73 6861 7065 5b30 5d0a 2020 2020 7265  .shape[0].    re
-00019150: 7475 726e 2066 7265 7173 0a64 6566 2063  turn freqs.def c
-00019160: 6f6d 7061 7265 5f74 7265 6573 2874 312c  ompare_trees(t1,
-00019170: 7432 293a 0a20 2020 2022 2222 436f 6d70  t2):.    """Comp
-00019180: 7574 6573 2074 6865 2052 6620 6469 7374  utes the Rf dist
-00019190: 616e 6365 2061 6d6f 6e67 2074 776f 2074  ance among two t
-000191a0: 7265 652c 2069 7420 6361 6c63 756c 6174  ree, it calculat
-000191b0: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
-000191c0: 2063 6861 6e67 6573 2072 6571 7569 7265   changes require
-000191d0: 7320 746f 2074 7261 6e73 666f 726d 206f  s to transform o
-000191e0: 6e65 2074 7265 6520 696e 746f 2074 6865  ne tree into the
-000191f0: 206f 7468 6572 0a20 2020 203a 7061 7261   other.    :para
-00019200: 6d20 7374 7220 7431 3a20 7061 7468 2074  m str t1: path t
-00019210: 6f20 6669 7273 7420 6e65 7477 6963 6b20  o first netwick 
-00019220: 7472 6565 0a20 2020 203a 7061 7261 6d20  tree.    :param 
-00019230: 7374 7220 7432 3a20 7061 7468 2074 6f20  str t2: path to 
-00019240: 7365 636f 6e64 206e 6574 7769 636b 2074  second netwick t
-00019250: 7265 6522 2222 0a20 2020 2063 6f6c 756d  ree""".    colum
-00019260: 6e73 203d 205b 2252 4620 6469 7374 616e  ns = ["RF distan
-00019270: 6365 222c 224d 6178 696d 756d 2052 4620  ce","Maximum RF 
-00019280: 6469 7374 616e 6365 222c 2243 6f6d 6d6f  distance","Commo
-00019290: 6e20 6c65 6176 6573 222c 2250 6172 7469  n leaves","Parti
-000192a0: 7469 6f6e 7349 6e5f 7431 5f4e 4f54 5f74  tionsIn_t1_NOT_t
-000192b0: 3222 2c22 5061 7274 6974 696f 6e73 496e  2","PartitionsIn
-000192c0: 5f74 325f 4e4f 545f 7431 222c 2244 6973  _t2_NOT_t1","Dis
-000192d0: 6361 7264 6564 5f70 6172 7469 7469 6f6e  carded_partition
-000192e0: 735f 7431 222c 2244 6973 6361 7264 6564  s_t1","Discarded
-000192f0: 5f70 6172 7469 7469 6f6e 735f 7432 225d  _partitions_t2"]
-00019300: 0a20 2020 2023 2074 3120 203d 2054 7265  .    # t1  = Tre
-00019310: 6545 7465 3328 7431 290a 2020 2020 2320  eEte3(t1).    # 
-00019320: 7432 203d 2054 7265 6545 7465 3328 7432  t2 = TreeEte3(t2
-00019330: 290a 2020 2020 2320 7265 7375 6c74 7320  ).    # results 
-00019340: 3d20 7431 2e72 6f62 696e 736f 6e5f 666f  = t1.robinson_fo
-00019350: 756c 6473 2874 322c 756e 726f 6f74 6564  ulds(t2,unrooted
-00019360: 5f74 7265 6573 3d54 7275 6529 0a20 2020  _trees=True).   
-00019370: 2063 6f6d 6d61 6e64 203d 2027 5273 6372   command = 'Rscr
-00019380: 6970 7427 0a20 2020 2070 6174 6832 7363  ipt'.    path2sc
-00019390: 7269 7074 203d 2027 2f68 6f6d 652f 6c79  ript = '/home/ly
-000193a0: 732f 4472 6f70 626f 782f 5068 442f 4452  s/Dropbox/PhD/DR
-000193b0: 4155 504e 4952 2f54 7265 655f 4469 7374  AUPNIR/Tree_Dist
-000193c0: 616e 6365 2e52 270a 2020 2020 2320 4275  ance.R'.    # Bu
-000193d0: 696c 6420 7375 6270 726f 6365 7373 2063  ild subprocess c
-000193e0: 6f6d 6d61 6e64 0a20 2020 2061 7267 7320  ommand.    args 
-000193f0: 3d5b 7431 2c74 325d 0a20 2020 2063 6d64  =[t1,t2].    cmd
-00019400: 203d 205b 636f 6d6d 616e 642c 2070 6174   = [command, pat
-00019410: 6832 7363 7269 7074 5d20 2b20 6172 6773  h2script] + args
-00019420: 0a20 2020 2064 6973 7461 6e63 6520 3d20  .    distance = 
-00019430: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-00019440: 5f6f 7574 7075 7428 636d 642c 2075 6e69  _output(cmd, uni
-00019450: 7665 7273 616c 5f6e 6577 6c69 6e65 733d  versal_newlines=
-00019460: 5472 7565 290a 2020 2020 7265 7475 726e  True).    return
-00019470: 2064 6973 7461 6e63 650a 0a64 6566 2072   distance..def r
-00019480: 656d 6f76 655f 7374 6f70 5f63 6f64 6f6e  emove_stop_codon
-00019490: 7328 7365 7175 656e 6365 5f66 696c 652c  s(sequence_file,
-000194a0: 6973 5f70 726f 743d 4661 6c73 6529 3a0a  is_prot=False):.
-000194b0: 2020 2020 2222 2252 656d 6f76 6520 7468      """Remove th
-000194c0: 6520 7374 6f70 2063 6f64 6f6e 7328 2a29  e stop codons(*)
-000194d0: 2066 726f 6d20 616e 2061 6c69 676e 6d65   from an alignme
-000194e0: 6e74 2066 696c 6522 2222 0a20 2020 2069  nt file""".    i
-000194f0: 6620 6973 5f70 726f 743a 0a20 2020 2020  f is_prot:.     
-00019500: 2020 2070 7269 6e74 2822 5265 6d6f 7669     print("Removi
-00019510: 6e67 2073 746f 7020 636f 646f 6e73 2066  ng stop codons f
-00019520: 726f 6d20 7072 6f74 6569 6e22 290a 2020  rom protein").  
-00019530: 2020 2020 2020 7072 696e 7428 7365 7175        print(sequ
-00019540: 656e 6365 5f66 696c 6529 0a20 2020 2020  ence_file).     
-00019550: 2020 2073 6571 5f66 696c 6520 3d20 6f70     seq_file = op
-00019560: 656e 2873 6571 7565 6e63 655f 6669 6c65  en(sequence_file
-00019570: 2c20 2772 2b27 290a 2020 2020 2020 2020  , 'r+').        
-00019580: 7365 7120 3d20 7365 715f 6669 6c65 2e72  seq = seq_file.r
-00019590: 6561 6428 290a 2020 2020 2020 2020 7365  ead().        se
-000195a0: 715f 6669 6c65 2e73 6565 6b28 3029 0a20  q_file.seek(0). 
-000195b0: 2020 2020 2020 206e 6f5f 636f 646f 6e73         no_codons
-000195c0: 203d 205b 6920 6966 2069 213d 222a 2220   = [i if i!="*" 
-000195d0: 656c 7365 2022 2d22 2066 6f72 2069 2069  else "-" for i i
-000195e0: 6e20 7365 715d 2023 7265 706c 6163 6520  n seq] #replace 
-000195f0: 666f 7220 6120 6761 700a 2020 2020 2020  for a gap.      
-00019600: 2020 2354 4f44 4f3a 2054 7275 6e63 6174    #TODO: Truncat
-00019610: 6520 7468 6520 7365 7175 656e 6365 2069  e the sequence i
-00019620: 6620 7468 6572 6520 6973 2061 2073 746f  f there is a sto
-00019630: 7020 636f 646f 6e20 696e 2074 6865 206d  p codon in the m
-00019640: 6964 646c 6520 2873 746f 7020 6164 6469  iddle (stop addi
-00019650: 6e67 2067 6170 7320 7768 656e 205c 6e20  ng gaps when \n 
-00019660: 6973 2072 6561 6368 6564 290a 2020 2020  is reached).    
-00019670: 2020 2020 2320 6e6f 5f63 6f64 6f6e 733d      # no_codons=
-00019680: 205b 5d0a 2020 2020 2020 2020 2320 666f   [].        # fo
-00019690: 7220 696e 6465 782c 6920 696e 2065 6e75  r index,i in enu
-000196a0: 6d65 7261 7465 2873 6571 293a 0a20 2020  merate(seq):.   
-000196b0: 2020 2020 2023 2020 2020 2069 6620 6920       #     if i 
-000196c0: 3d3d 2022 2a22 3a0a 2020 2020 2020 2020  == "*":.        
-000196d0: 2320 2020 2020 2020 2020 693d 2022 2d22  #         i= "-"
-000196e0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-000196f0: 2020 206e 6578 745f 6272 6561 6b5f 696e     next_break_in
-00019700: 6465 7820 3d20 7365 715b 696e 6465 783a  dex = seq[index:
-00019710: 5d2e 696e 6465 7828 225c 6e22 290a 2020  ].index("\n").  
-00019720: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-00019730: 7365 715b 696e 6465 783a 6e65 7874 5f62  seq[index:next_b
-00019740: 7265 616b 5f69 6e64 6578 5d20 3d20 222d  reak_index] = "-
-00019750: 222a 286e 6578 745f 6272 6561 6b5f 696e  "*(next_break_in
-00019760: 6465 782d 696e 6465 7829 0a0a 2020 2020  dex-index)..    
-00019770: 2020 2020 7365 715f 6669 6c65 2e77 7269      seq_file.wri
-00019780: 7465 2822 222e 6a6f 696e 286e 6f5f 636f  te("".join(no_co
-00019790: 646f 6e73 2929 0a20 2020 2020 2020 2073  dons)).        s
-000197a0: 6571 5f66 696c 652e 7472 756e 6361 7465  eq_file.truncate
-000197b0: 2829 2020 2320 7265 6d6f 7665 2063 6f6e  ()  # remove con
-000197c0: 7465 6e74 730a 2020 2020 656c 7365 3a0a  tents.    else:.
-000197d0: 2020 2020 2020 2020 7374 6f70 5f63 6f64          stop_cod
-000197e0: 6f6e 7320 3d20 5b22 5447 4122 2c22 5441  ons = ["TGA","TA
-000197f0: 4722 2c22 5441 4122 5d0a 2020 2020 2020  G","TAA"].      
-00019800: 2020 7365 715f 6669 6c65 203d 206f 7065    seq_file = ope
-00019810: 6e28 7365 7175 656e 6365 5f66 696c 652c  n(sequence_file,
-00019820: 2027 722b 2729 0a20 2020 2020 2020 2073   'r+').        s
-00019830: 6571 203d 2073 6571 5f66 696c 652e 7265  eq = seq_file.re
-00019840: 6164 2829 0a20 2020 2020 2020 2073 6571  ad().        seq
-00019850: 5f66 696c 652e 7365 656b 2830 290a 2020  _file.seek(0).  
-00019860: 2020 2020 2020 2363 6f64 696e 675f 646e        #coding_dn
-00019870: 6120 3d20 5365 7128 7365 7129 0a20 2020  a = Seq(seq).   
-00019880: 2020 2020 2023 7072 6f74 6569 6e20 3d20       #protein = 
-00019890: 636f 6469 6e67 5f64 6e61 2e74 7261 6e73  coding_dna.trans
-000198a0: 6c61 7465 2829 0a20 2020 2020 2020 2063  late().        c
-000198b0: 6f64 6f6e 7320 3d20 5b73 6571 5b69 3a69  odons = [seq[i:i
-000198c0: 2b33 5d20 666f 7220 6920 696e 2072 616e  +3] for i in ran
-000198d0: 6765 2830 2c20 6c65 6e28 7365 7129 2c20  ge(0, len(seq), 
-000198e0: 3329 5d0a 2020 2020 2020 2020 636f 646f  3)].        codo
-000198f0: 6e73 203d 5b63 6f64 2066 6f72 2063 6f64  ns =[cod for cod
-00019900: 2069 6e20 636f 646f 6e73 2069 6620 6c65   in codons if le
-00019910: 6e28 636f 6429 203d 3d33 2061 6e64 2063  n(cod) ==3 and c
-00019920: 6f64 206e 6f74 2069 6e20 7374 6f70 5f63  od not in stop_c
-00019930: 6f64 6f6e 735d 0a20 2020 2020 2020 2023  odons].        #
-00019940: 6368 6563 6b20 3d20 616e 7928 6974 656d  check = any(item
-00019950: 2069 6e20 636f 646f 6e73 2066 6f72 2069   in codons for i
-00019960: 7465 6d20 696e 2073 746f 705f 636f 646f  tem in stop_codo
-00019970: 6e73 290a 2020 2020 2020 2020 7365 715f  ns).        seq_
-00019980: 6669 6c65 2e77 7269 7465 2822 222e 6a6f  file.write("".jo
-00019990: 696e 2863 6f64 6f6e 7329 290a 2020 2020  in(codons)).    
-000199a0: 2020 2020 7365 715f 6669 6c65 2e74 7275      seq_file.tru
-000199b0: 6e63 6174 6528 2920 2023 2072 656d 6f76  ncate()  # remov
-000199c0: 6520 636f 6e74 656e 7473 0a0a 6465 6620  e contents..def 
-000199d0: 636f 6e76 6572 745f 746f 5f69 6e74 6567  convert_to_integ
-000199e0: 6572 7328 6461 7461 7365 742c 6161 5f70  ers(dataset,aa_p
-000199f0: 726f 6273 2c61 7869 7329 3a0a 2020 2020  robs,axis):.    
-00019a00: 2222 2254 7261 6e73 666f 726d 7320 6f6e  """Transforms on
-00019a10: 6520 686f 7420 656e 636f 6465 6420 616d  e hot encoded am
-00019a20: 696e 6f20 6163 6964 7320 696e 746f 2030  ino acids into 0
-00019a30: 2d69 6e64 6578 6564 2069 6e74 6567 6572  -indexed integer
-00019a40: 7320 692e 6520 5b31 2c30 2c30 2c30 5d20  s i.e [1,0,0,0] 
-00019a50: 2d2d 3e20 3020 205b 302c 312c 302c 305d  --> 0  [0,1,0,0]
-00019a60: 202d 3e20 310a 2020 2020 3a70 6172 616d   -> 1.    :param
-00019a70: 206e 756d 7079 2064 6174 6173 6574 0a20   numpy dataset. 
-00019a80: 2020 203a 7061 7261 6d20 6161 5f70 726f     :param aa_pro
-00019a90: 6273 3a20 616d 696e 6f20 6163 6964 2070  bs: amino acid p
-00019aa0: 726f 6261 6269 6c69 7469 6573 2c20 6469  robabilities, di
-00019ab0: 6d65 6e73 696f 6e73 206f 6620 7468 6520  mensions of the 
-00019ac0: 6f6e 652d 686f 7420 656e 636f 6469 6e67  one-hot encoding
-00019ad0: 2222 220a 2020 2020 6966 2061 7869 733d  """.    if axis=
-00019ae0: 3d33 3a23 7573 6520 666f 7220 7072 6564  =3:#use for pred
-00019af0: 6963 7469 6f6e 730a 2020 2020 2020 2020  ictions.        
-00019b00: 6220 3d20 746f 7263 682e 6172 676d 6178  b = torch.argmax
-00019b10: 2864 6174 6173 6574 2c20 6469 6d3d 6178  (dataset, dim=ax
-00019b20: 6973 290a 2020 2020 656c 7365 3a0a 2020  is).    else:.  
-00019b30: 2020 2020 2020 696e 7465 6765 7273 203d        integers =
-00019b40: 2074 6f72 6368 2e61 7267 6d61 7828 6461   torch.argmax(da
-00019b50: 7461 7365 745b 3a2c 323a 2c30 3a61 615f  taset[:,2:,0:aa_
-00019b60: 7072 6f62 735d 2c64 696d 3d61 7869 7329  probs],dim=axis)
-00019b70: 0a20 2020 2020 2020 2062 203d 2074 6f72  .        b = tor
-00019b80: 6368 2e7a 6572 6f73 2864 6174 6173 6574  ch.zeros(dataset
-00019b90: 5b3a 2c3a 2c30 5d2e 7368 6170 6520 2b20  [:,:,0].shape + 
-00019ba0: 2833 302c 2929 2e63 7075 2829 0a20 2020  (30,)).cpu().   
-00019bb0: 2020 2020 2023 6220 3d20 6e70 2e7a 6572       #b = np.zer
-00019bc0: 6f73 2844 6174 6173 6574 5b3a 2c3a 2c30  os(Dataset[:,:,0
-00019bd0: 5d2e 7368 6170 6520 2b20 2833 302c 2929  ].shape + (30,))
-00019be0: 0a20 2020 2020 2020 2062 5b3a 2c20 323a  .        b[:, 2:
-00019bf0: 2c20 305d 203d 2069 6e74 6567 6572 730a  , 0] = integers.
-00019c00: 2020 2020 2020 2020 625b 3a2c 3a32 5d20          b[:,:2] 
-00019c10: 3d20 6461 7461 7365 745b 3a2c 3a32 5d0a  = dataset[:,:2].
-00019c20: 2020 2020 7265 7475 726e 2062 0a64 6566      return b.def
-00019c30: 2070 726f 6365 7373 5f62 6c6f 7375 6d28   process_blosum(
-00019c40: 626c 6f73 756d 2c61 615f 6672 6571 732c  blosum,aa_freqs,
-00019c50: 616c 6967 6e5f 7365 715f 6c65 6e2c 6161  align_seq_len,aa
-00019c60: 5f70 726f 6273 293a 0a20 2020 2022 2222  _probs):.    """
-00019c70: 0a20 2020 2043 6f6d 7075 7465 7320 7468  .    Computes th
-00019c80: 6520 6d61 7472 6963 6573 2072 6571 7569  e matrices requi
-00019c90: 7265 6420 746f 2062 7569 6c64 2061 2062  red to build a b
-00019ca0: 6c6f 7375 6d20 656d 6265 6464 696e 670a  losum embedding.
-00019cb0: 2020 2020 3a70 6172 616d 2074 656e 736f      :param tenso
-00019cc0: 7220 626c 6f73 756d 3a20 424c 4f53 554d  r blosum: BLOSUM
-00019cd0: 206c 696b 656c 6968 6f6f 6420 2073 636f   likelihood  sco
-00019ce0: 7265 730a 2020 2020 3a70 6172 616d 2074  res.    :param t
-00019cf0: 656e 736f 7220 6161 5f66 7265 7173 203a  ensor aa_freqs :
-00019d00: 2061 6d69 6e6f 2061 6369 6420 6672 6571   amino acid freq
-00019d10: 7565 6e63 6965 7320 7065 7220 706f 7369  uencies per posi
-00019d20: 7469 6f6e 0a20 2020 203a 7061 7261 6d20  tion.    :param 
-00019d30: 616c 6967 6e5f 7365 715f 6c65 6e3a 2061  align_seq_len: a
-00019d40: 6c69 676e 6d65 6e74 206c 656e 6774 680a  lignment length.
-00019d50: 2020 2020 3a70 6172 616d 2061 615f 7072      :param aa_pr
-00019d60: 6f62 733a 2061 6d69 6e6f 2061 6369 6420  obs: amino acid 
-00019d70: 7072 6f62 6162 696c 6974 6965 732c 2074  probabilities, t
-00019d80: 7970 6573 206f 6620 616d 696e 6f20 6163  ypes of amino ac
-00019d90: 6964 7320 696e 2074 6865 2061 6c69 676e  ids in the align
-00019da0: 6d65 6e74 0a20 2020 203a 6f75 7420 7465  ment.    :out te
-00019db0: 6e73 6f72 2062 6c6f 7375 6d5f 6d61 7820  nsor blosum_max 
-00019dc0: 5b61 6c69 676e 5f6c 656e 2c61 615f 7072  [align_len,aa_pr
-00019dd0: 6f62 5d3a 2062 6c6f 7375 6d20 6c69 6b65  ob]: blosum like
-00019de0: 6c69 686f 6f64 2073 636f 7265 7320 666f  lihood scores fo
-00019df0: 7220 7468 6520 6d6f 7374 2066 7265 7175  r the most frequ
-00019e00: 656e 7420 6161 2069 6e20 7468 6520 616c  ent aa in the al
-00019e10: 6967 6e6d 656e 7420 706f 7369 7469 6f6e  ignment position
-00019e20: 0a20 2020 203a 6f75 7420 7465 6e73 6f72  .    :out tensor
-00019e30: 2062 6c6f 7375 6d5f 7765 6967 6874 6564   blosum_weighted
-00019e40: 205b 616c 6967 6e5f 6c65 6e2c 6161 5f70   [align_len,aa_p
-00019e50: 726f 623a 2077 6569 6768 7465 6420 6176  rob: weighted av
-00019e60: 6572 6167 6520 6f66 2062 6c6f 7375 6d20  erage of blosum 
-00019e70: 6c69 6b65 6c69 686f 6f64 7320 6163 636f  likelihoods acco
-00019e80: 7264 696e 6720 746f 2074 6865 2061 6120  rding to the aa 
-00019e90: 6672 6571 7565 6e63 790a 2020 2020 3a6f  frequency.    :o
-00019ea0: 7574 2076 6172 6961 626c 655f 636f 7265  ut variable_core
-00019eb0: 3a20 5b61 6c69 676e 5f6c 656e 5d20 3a20  : [align_len] : 
-00019ec0: 636f 756e 7473 2074 6865 206e 756d 6265  counts the numbe
-00019ed0: 7220 6f66 2064 6966 6665 7265 6e74 2065  r of different e
-00019ee0: 6c65 6d65 6e74 7320 2861 6d69 6e6f 2061  lements (amino a
-00019ef0: 6369 6420 6469 7665 7273 6974 7929 2070  cid diversity) p
-00019f00: 6572 2061 6c69 676e 6d65 6e74 2070 6f73  er alignment pos
-00019f10: 6974 696f 6e22 2222 0a0a 2020 2020 6161  ition"""..    aa
-00019f20: 5f66 7265 7173 5f6d 6178 203d 2074 6f72  _freqs_max = tor
-00019f30: 6368 2e61 7267 6d61 7828 6161 5f66 7265  ch.argmax(aa_fre
-00019f40: 7173 2c20 6469 6d3d 3129 2e72 6570 6561  qs, dim=1).repea
-00019f50: 7428 6161 5f70 726f 6273 2c20 3129 2e70  t(aa_probs, 1).p
-00019f60: 6572 6d75 7465 2831 2c20 3029 2023 5b6d  ermute(1, 0) #[m
-00019f70: 6178 5f6c 656e 2c20 6161 5f70 726f 6273  ax_len, aa_probs
-00019f80: 5d0a 2020 2020 626c 6f73 756d 5f65 7870  ].    blosum_exp
-00019f90: 616e 6465 6420 3d20 626c 6f73 756d 5b31  anded = blosum[1
-00019fa0: 3a2c 2031 3a5d 2e72 6570 6561 7428 616c  :, 1:].repeat(al
-00019fb0: 6967 6e5f 7365 715f 6c65 6e2c 2031 2c20  ign_seq_len, 1, 
-00019fc0: 3129 2020 2320 5b6d 6178 5f6c 656e 2c61  1)  # [max_len,a
-00019fd0: 615f 7072 6f62 732c 6161 5f70 726f 6273  a_probs,aa_probs
-00019fe0: 5d0a 2020 2020 626c 6f73 756d 5f6d 6178  ].    blosum_max
-00019ff0: 203d 2062 6c6f 7375 6d5f 6578 7061 6e64   = blosum_expand
-0001a000: 6564 2e67 6174 6865 7228 312c 2061 615f  ed.gather(1, aa_
-0001a010: 6672 6571 735f 6d61 782e 756e 7371 7565  freqs_max.unsque
-0001a020: 657a 6528 3129 292e 7371 7565 657a 6528  eze(1)).squeeze(
-0001a030: 3129 2020 2320 5b61 6c69 676e 5f73 6571  1)  # [align_seq
-0001a040: 5f6c 656e 2c32 315d 2053 6565 6d73 2063  _len,21] Seems c
-0001a050: 6f72 7265 6374 0a0a 2020 2020 626c 6f73  orrect..    blos
-0001a060: 756d 5f77 6569 6768 7465 6420 3d20 6161  um_weighted = aa
-0001a070: 5f66 7265 7173 5b3a 2c3a 2c4e 6f6e 655d  _freqs[:,:,None]
-0001a080: 2a62 6c6f 7375 6d5f 6578 7061 6e64 6564  *blosum_expanded
-0001a090: 2023 2d2d 3e20 7265 706c 6163 6520 3020   #--> replace 0 
-0001a0a0: 7769 7468 206e 616e 733f 206f 7468 6572  with nans? other
-0001a0b0: 7769 7365 2074 6865 2030 2061 7265 2069  wise the 0 are i
-0001a0c0: 6e20 7468 6520 6d65 616e 2061 7320 7765  n the mean as we
-0001a0d0: 6c6c 2e2e 2e2e 0a20 2020 2062 6c6f 7375  ll.....    blosu
-0001a0e0: 6d5f 7765 6967 6874 6564 203d 2062 6c6f  m_weighted = blo
-0001a0f0: 7375 6d5f 7765 6967 6874 6564 2e6d 6561  sum_weighted.mea
-0001a100: 6e28 6469 6d3d 3129 0a0a 2020 2020 7661  n(dim=1)..    va
-0001a110: 7269 6162 6c65 5f73 636f 7265 203d 2074  riable_score = t
-0001a120: 6f72 6368 2e63 6f75 6e74 5f6e 6f6e 7a65  orch.count_nonze
-0001a130: 726f 2861 615f 6672 6571 732c 2064 696d  ro(aa_freqs, dim
-0001a140: 3d31 292f 6161 5f70 726f 6273 2023 6869  =1)/aa_probs #hi
-0001a150: 6768 6572 2073 636f 7265 2c20 6d6f 7265  gher score, more
-0001a160: 2076 6172 6961 626c 650a 0a20 2020 2072   variable..    r
-0001a170: 6574 7572 6e20 626c 6f73 756d 5f6d 6178  eturn blosum_max
-0001a180: 2c62 6c6f 7375 6d5f 7765 6967 6874 6564  ,blosum_weighted
-0001a190: 2c20 7661 7269 6162 6c65 5f73 636f 7265  , variable_score
-0001a1a0: 0a64 6566 2062 6c6f 7375 6d5f 656d 6265  .def blosum_embe
-0001a1b0: 6464 696e 675f 656e 636f 6465 7228 626c  dding_encoder(bl
-0001a1c0: 6f73 756d 2c61 615f 6672 6571 732c 616c  osum,aa_freqs,al
-0001a1d0: 6967 6e5f 7365 715f 6c65 6e2c 6161 5f70  ign_seq_len,aa_p
-0001a1e0: 726f 6273 2c64 6174 6173 6574 5f74 7261  robs,dataset_tra
-0001a1f0: 696e 2c20 6f6e 655f 686f 745f 656e 636f  in, one_hot_enco
-0001a200: 6469 6e67 293a 0a20 2020 2022 2222 5472  ding):.    """Tr
-0001a210: 616e 7366 6f72 6d73 2074 6865 2074 7261  ansforms the tra
-0001a220: 696e 2064 6174 6173 6574 2c20 7768 6963  in dataset, whic
-0001a230: 6820 6973 2066 6f72 6d65 6420 6279 2061  h is formed by a
-0001a240: 2074 656e 736f 7220 6f66 2069 6e74 6567   tensor of integ
-0001a250: 6572 7320 7468 6174 2072 6570 7265 7365  ers that represe
-0001a260: 6e74 2074 6865 2061 6d69 6e6f 2061 6369  nt the amino aci
-0001a270: 6473 2c20 696e 746f 2061 2064 6174 6173  ds, into a datas
-0001a280: 6574 2077 6865 7265 2065 6163 6820 616d  et where each am
-0001a290: 696e 6f20 6163 6964 2028 696e 7465 6765  ino acid (intege
-0001a2a0: 7229 2069 7320 6578 6368 616e 6765 6420  r) is exchanged 
-0001a2b0: 7769 7468 2069 7473 2062 6c6f 7375 6d20  with its blosum 
-0001a2c0: 7363 6f72 650a 2020 2020 3a6f 7574 2074  score.    :out t
-0001a2d0: 656e 736f 7220 6161 5f74 7261 696e 5f62  ensor aa_train_b
-0001a2e0: 6c6f 7375 6d20 3a20 5472 6169 6e69 6e67  losum : Training
-0001a2f0: 2064 6174 6173 6574 2077 6974 6820 7468   dataset with th
-0001a300: 6520 626c 6f73 756d 2076 6563 746f 7273  e blosum vectors
-0001a310: 2069 6e73 7465 6164 206f 6620 7468 6520   instead of the 
-0001a320: 616d 696e 6f20 6163 6964 7320 286e 756d  amino acids (num
-0001a330: 6265 7273 206f 7220 6f6e 6520 686f 7420  bers or one hot 
-0001a340: 7265 7072 6573 656e 7461 7469 6f6e 2922  representation)"
-0001a350: 2222 0a20 2020 2069 6620 6f6e 655f 686f  "".    if one_ho
-0001a360: 745f 656e 636f 6469 6e67 3a0a 2020 2020  t_encoding:.    
-0001a370: 2020 2020 6461 7461 7365 745f 7472 6169      dataset_trai
-0001a380: 6e20 3d20 636f 6e76 6572 745f 746f 5f69  n = convert_to_i
-0001a390: 6e74 6567 6572 7328 6461 7461 7365 745f  ntegers(dataset_
-0001a3a0: 7472 6169 6e2c 6161 5f70 726f 6273 2c61  train,aa_probs,a
-0001a3b0: 7869 733d 3229 0a20 2020 2061 6d69 6e6f  xis=2).    amino
-0001a3c0: 6163 6964 735f 7365 7173 203d 2064 6174  acids_seqs = dat
-0001a3d0: 6173 6574 5f74 7261 696e 5b3a 2c32 3a2c  aset_train[:,2:,
-0001a3e0: 305d 2e72 6570 6561 7428 6161 5f70 726f  0].repeat(aa_pro
-0001a3f0: 6273 2c31 2c31 292e 7065 726d 7574 6528  bs,1,1).permute(
-0001a400: 312c 322c 3029 2023 5b4e 2c6d 6178 5f6c  1,2,0) #[N,max_l
-0001a410: 656e 2c61 6120 7265 7065 6174 6564 2061  en,aa repeated a
-0001a420: 615f 7072 6f62 7320 7469 6d65 735d 2d2d  a_probs times]--
-0001a430: 7365 656d 7320 636f 7272 6563 740a 2020  seems correct.  
-0001a440: 2020 626c 6f73 756d 5f65 7870 616e 6465    blosum_expande
-0001a450: 6420 3d20 626c 6f73 756d 5b31 3a2c 2031  d = blosum[1:, 1
-0001a460: 3a5d 2e72 6570 6561 7428 6461 7461 7365  :].repeat(datase
-0001a470: 745f 7472 6169 6e2e 7368 6170 655b 305d  t_train.shape[0]
-0001a480: 2c61 6c69 676e 5f73 6571 5f6c 656e 2c20  ,align_seq_len, 
-0001a490: 312c 2031 2920 2023 205b 4e2c 6d61 785f  1, 1)  # [N,max_
-0001a4a0: 6c65 6e2c 6161 5f70 726f 6273 2c61 615f  len,aa_probs,aa_
-0001a4b0: 7072 6f62 735d 0a20 2020 2061 615f 7472  probs].    aa_tr
-0001a4c0: 6169 6e5f 626c 6f73 756d 203d 2062 6c6f  ain_blosum = blo
-0001a4d0: 7375 6d5f 6578 7061 6e64 6564 2e67 6174  sum_expanded.gat
-0001a4e0: 6865 7228 332c 2061 6d69 6e6f 6163 6964  her(3, aminoacid
-0001a4f0: 735f 7365 7173 2e74 6f28 746f 7263 682e  s_seqs.to(torch.
-0001a500: 696e 7436 3429 2e75 6e73 7175 6565 7a65  int64).unsqueeze
-0001a510: 2833 2929 2e73 7175 6565 7a65 282d 3129  (3)).squeeze(-1)
-0001a520: 2020 235b 4e2c 6d61 785f 6c65 6e2c 6161    #[N,max_len,aa
-0001a530: 5f70 726f 6273 5d0a 0a0a 2020 2020 7265  _probs]...    re
-0001a540: 7475 726e 2061 615f 7472 6169 6e5f 626c  turn aa_train_bl
-0001a550: 6f73 756d 0a0a 6465 6620 7374 7232 626f  osum..def str2bo
-0001a560: 6f6c 2876 293a 0a20 2020 2022 2222 436f  ol(v):.    """Co
-0001a570: 6e76 6572 7473 2061 2073 7472 696e 6720  nverts a string 
-0001a580: 696e 746f 2061 2062 6f6f 6c65 616e 2c20  into a boolean, 
-0001a590: 7573 6566 756c 2066 6f72 2062 6f6f 6c65  useful for boole
-0001a5a0: 616e 2061 7267 756d 656e 7473 0a20 2020  an arguments.   
-0001a5b0: 203a 7061 7261 6d20 7374 7220 7622 2222   :param str v"""
-0001a5c0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-0001a5d0: 6365 2876 2c20 626f 6f6c 293a 0a20 2020  ce(v, bool):.   
-0001a5e0: 2020 2020 2072 6574 7572 6e20 760a 2020       return v.  
-0001a5f0: 2020 6966 2076 2e6c 6f77 6572 2829 2069    if v.lower() i
-0001a600: 6e20 2827 7965 7327 2c20 2774 7275 6527  n ('yes', 'true'
-0001a610: 2c20 2774 272c 2027 7927 2c20 2731 272c  , 't', 'y', '1',
-0001a620: 2754 7275 6527 293a 0a20 2020 2020 2020  'True'):.       
-0001a630: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-0001a640: 2065 6c69 6620 762e 6c6f 7765 7228 2920   elif v.lower() 
-0001a650: 696e 2028 276e 6f27 2c20 2766 616c 7365  in ('no', 'false
-0001a660: 272c 2027 6627 2c20 276e 272c 2027 3027  ', 'f', 'n', '0'
-0001a670: 2c27 4661 6c73 6527 293a 0a20 2020 2020  ,'False'):.     
-0001a680: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0001a690: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001a6a0: 2020 7261 6973 6520 6172 6770 6172 7365    raise argparse
-0001a6b0: 2e41 7267 756d 656e 7454 7970 6545 7272  .ArgumentTypeErr
-0001a6c0: 6f72 2827 426f 6f6c 6561 6e20 7661 6c75  or('Boolean valu
-0001a6d0: 6520 6578 7065 6374 6564 2e27 290a 6465  e expected.').de
-0001a6e0: 6620 7374 7232 4e6f 6e65 2876 293a 0a20  f str2None(v):. 
-0001a6f0: 2020 2022 2222 436f 6e76 6572 7473 2061     """Converts a
-0001a700: 2073 7472 696e 6720 696e 746f 204e 6f6e   string into Non
-0001a710: 650a 2020 2020 3a70 6172 616d 2073 7472  e.    :param str
-0001a720: 2076 2222 220a 0a20 2020 2069 6620 762e   v"""..    if v.
-0001a730: 6c6f 7765 7228 2920 696e 2028 274e 6f6e  lower() in ('Non
-0001a740: 6527 2c27 6e6f 6e65 2729 3a0a 2020 2020  e','none'):.    
-0001a750: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-0001a760: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-0001a770: 6e63 6528 762c 7374 7229 3a0a 2020 2020  nce(v,str):.    
-0001a780: 2020 2020 7265 7475 726e 2076 0a20 2020      return v.   
-0001a790: 2065 6c73 653a 0a20 2020 2020 2020 2076   else:.        v
-0001a7a0: 203d 2061 7374 2e6c 6974 6572 616c 5f65   = ast.literal_e
-0001a7b0: 7661 6c28 7629 0a20 2020 2020 2020 2072  val(v).        r
-0001a7c0: 6574 7572 6e20 760a 0a0a 0a0a 0a0a       eturn v.......
+000174f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00017500: 676c 5f67 7261 7068 3d64 676c 5f67 7261  gl_graph=dgl_gra
+00017510: 7068 290a 0a0a 2020 2020 7265 7475 726e  ph)...    return
+00017520: 2061 6464 6974 696f 6e61 6c5f 696e 666f   additional_info
+00017530: 0a64 6566 2063 7265 6174 655f 7472 6565  .def create_tree
+00017540: 5f62 795f 6c65 7665 6c73 2863 6869 6c64  _by_levels(child
+00017550: 7265 6e5f 6469 6374 293a 0a20 2020 2022  ren_dict):.    "
+00017560: 2222 416c 7465 726e 6174 6976 6520 6d65  ""Alternative me
+00017570: 7468 6f64 2074 6f20 6275 696c 6420 7468  thod to build th
+00017580: 6520 7472 6565 2062 7920 6c65 7665 6c73  e tree by levels
+00017590: 2061 7320 7375 6767 6573 7465 6420 6279   as suggested by
+000175a0: 2052 6f62 6572 7422 2222 0a20 2020 2074   Robert""".    t
+000175b0: 7265 655f 6c65 7665 6c73 203d 205b 5b30  ree_levels = [[0
+000175c0: 5d5d 0a20 2020 2063 7572 7265 6e74 5f6e  ]].    current_n
+000175d0: 6f64 6573 203d 205b 305d 0a20 2020 2077  odes = [0].    w
+000175e0: 6869 6c65 206c 656e 2863 7572 7265 6e74  hile len(current
+000175f0: 5f6e 6f64 6573 2920 3e20 303a 0a20 2020  _nodes) > 0:.   
+00017600: 2020 2020 2063 6869 6c64 7265 6e5f 6e6f       children_no
+00017610: 6465 7320 3d20 5b5d 0a20 2020 2020 2020  des = [].       
+00017620: 2066 6f72 206e 6f64 6520 696e 2063 7572   for node in cur
+00017630: 7265 6e74 5f6e 6f64 6573 3a0a 2020 2020  rent_nodes:.    
+00017640: 2020 2020 2020 2020 6966 206e 6f64 6520          if node 
+00017650: 696e 2063 6869 6c64 7265 6e5f 6469 6374  in children_dict
+00017660: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+00017670: 2020 2020 2020 2020 2063 6869 6c64 7265           childre
+00017680: 6e5f 6e6f 6465 7320 2b3d 2063 6869 6c64  n_nodes += child
+00017690: 7265 6e5f 6469 6374 5b6e 6f64 655d 0a0a  ren_dict[node]..
+000176a0: 2020 2020 2020 2020 7472 6565 5f6c 6576          tree_lev
+000176b0: 656c 732e 6170 7065 6e64 2863 6869 6c64  els.append(child
+000176c0: 7265 6e5f 6e6f 6465 7329 0a20 2020 2020  ren_nodes).     
+000176d0: 2020 2063 7572 7265 6e74 5f6e 6f64 6573     current_nodes
+000176e0: 203d 2063 6869 6c64 7265 6e5f 6e6f 6465   = children_node
+000176f0: 730a 0a20 2020 2072 6574 7572 6e20 7472  s..    return tr
+00017700: 6565 5f6c 6576 656c 730a 636c 6173 7320  ee_levels.class 
+00017710: 4d79 4461 7461 7365 7428 4461 7461 7365  MyDataset(Datase
+00017720: 7429 3a23 544f 444f 3a20 7265 6d6f 7665  t):#TODO: remove
+00017730: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00017740: 5f28 7365 6c66 2c6c 6162 656c 732c 6461  _(self,labels,da
+00017750: 7461 5f61 7272 6179 7329 3a0a 2020 2020  ta_arrays):.    
+00017760: 2020 2020 7365 6c66 2e6c 6162 656c 7320      self.labels 
+00017770: 3d20 6c61 6265 6c73 0a20 2020 2020 2020  = labels.       
+00017780: 2073 656c 662e 6461 7461 5f61 7272 6179   self.data_array
+00017790: 7320 3d20 6461 7461 5f61 7272 6179 730a  s = data_arrays.
+000177a0: 0a20 2020 2064 6566 205f 5f67 6574 6974  .    def __getit
+000177b0: 656d 5f5f 2873 656c 662c 2069 6e64 6578  em__(self, index
+000177c0: 293a 2023 7365 7473 2061 5b69 5d0a 2020  ): #sets a[i].  
+000177d0: 2020 2020 2020 6c61 6265 6c20 3d20 7365        label = se
+000177e0: 6c66 2e6c 6162 656c 735b 696e 6465 785d  lf.labels[index]
+000177f0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00017800: 7365 6c66 2e64 6174 615f 6172 7261 7973  self.data_arrays
+00017810: 5b69 6e64 6578 5d0a 2020 2020 2020 2020  [index].        
+00017820: 7265 7475 726e 207b 2766 616d 696c 795f  return {'family_
+00017830: 6e61 6d65 273a 206c 6162 656c 2c20 2766  name': label, 'f
+00017840: 616d 696c 795f 6461 7461 273a 2064 6174  amily_data': dat
+00017850: 617d 0a20 2020 2064 6566 205f 5f6c 656e  a}.    def __len
+00017860: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00017870: 2020 7265 7475 726e 206c 656e 2873 656c    return len(sel
+00017880: 662e 6c61 6265 6c73 290a 6465 6620 6465  f.labels).def de
+00017890: 6669 6e65 5f62 6174 6368 5f73 697a 6528  fine_batch_size(
+000178a0: 6e2c 6261 7463 685f 7369 7a65 3d54 7275  n,batch_size=Tru
+000178b0: 652c 2062 656e 6368 6d61 726b 696e 673d  e, benchmarking=
+000178c0: 4661 6c73 6529 3a0a 2020 2020 2222 2241  False):.    """A
+000178d0: 7574 6f6d 6174 6963 2063 616c 6375 6c61  utomatic calcula
+000178e0: 7469 6f6e 2074 6865 2061 7661 696c 6162  tion the availab
+000178f0: 6c65 2064 6976 6973 6f72 7320 6f66 2074  le divisors of t
+00017900: 6865 206e 756d 6265 7220 6f66 2074 7261  he number of tra
+00017910: 696e 696e 6720 6461 7461 2070 6f69 6e74  ining data point
+00017920: 7320 286e 292e 0a20 2020 2054 6869 7320  s (n)..    This 
+00017930: 6865 6c70 7320 746f 2073 7567 6765 7374  helps to suggest
+00017940: 2061 6e20 6170 7072 6f70 6961 7465 2069   an appropiate i
+00017950: 6e74 6567 6572 2062 6174 6368 2073 697a  nteger batch siz
+00017960: 6520 6e75 6d62 6572 2c20 7468 6174 2073  e number, that s
+00017970: 706c 6974 7320 6576 656e 6c79 2074 6865  plits evenly the
+00017980: 2064 6174 610a 2020 2020 3a70 6172 616d   data.    :param
+00017990: 2069 6e74 206e 3a20 6e75 6d62 6572 206f   int n: number o
+000179a0: 6620 7365 7175 656e 6365 730a 2020 2020  f sequences.    
+000179b0: 3a70 6172 616d 2062 6f6f 6c20 6261 7463  :param bool batc
+000179c0: 685f 7369 7a65 0a20 2020 203a 7061 7261  h_size.    :para
+000179d0: 6d20 6265 6e63 686d 6172 6b69 6e67 2222  m benchmarking""
+000179e0: 220a 2020 2020 6966 206e 6f74 2062 656e  ".    if not ben
+000179f0: 6368 6d61 726b 696e 673a 0a20 2020 2020  chmarking:.     
+00017a00: 2020 2061 7373 6572 7420 6e20 3e3d 2031     assert n >= 1
+00017a10: 3030 202c 224e 6f74 2077 6f72 7468 2062  00 ,"Not worth b
+00017a20: 6174 6368 696e 672c 206e 756d 6265 7220  atching, number 
+00017a30: 6f66 2073 6571 7565 6e63 6573 2069 7320  of sequences is 
+00017a40: 3c20 3130 3020 220a 2020 2020 6469 7669  < 100 ".    divi
+00017a50: 736f 7273 203d 2044 7261 7570 6e69 724d  sors = DraupnirM
+00017a60: 6f64 656c 5574 696c 732e 7072 696e 745f  odelUtils.print_
+00017a70: 6469 7669 736f 7273 286e 290a 2020 2020  divisors(n).    
+00017a80: 6e5f 6469 6769 7473 203d 206c 656e 286c  n_digits = len(l
+00017a90: 6973 7428 7374 7228 6e29 2929 2023 2031  ist(str(n))) # 1
+00017aa0: 3030 2068 6173 2033 2064 6967 6974 732c  00 has 3 digits,
+00017ab0: 2031 3030 3020 6861 7320 3420 6469 6769   1000 has 4 digi
+00017ac0: 7473 2c20 3130 3030 3020 6861 7320 3520  ts, 10000 has 5 
+00017ad0: 6469 6769 7473 2061 6e64 2073 6f20 6f6e  digits and so on
+00017ae0: 0a20 2020 206e 5f63 6875 6e6b 7320 3d20  .    n_chunks = 
+00017af0: 5b6d 696e 2864 6976 6973 6f72 735b 6e5f  [min(divisors[n_
+00017b00: 6469 6769 7473 2d31 3a5d 2920 6966 206c  digits-1:]) if l
+00017b10: 656e 2864 6976 6973 6f72 7329 203e 206e  en(divisors) > n
+00017b20: 5f64 6967 6974 732d 3120 656c 7365 2031  _digits-1 else 1
+00017b30: 5d5b 305d 2020 2320 736d 616c 6c65 7374  ][0]  # smallest
+00017b40: 2064 6976 6973 6f72 2074 6861 7420 6973   divisor that is
+00017b50: 206e 6f74 2031 2c20 6f72 206a 7573 7420   not 1, or just 
+00017b60: 7573 6520 3120 2c20 7768 656e 206e 6f20  use 1 , when no 
+00017b70: 6f74 6865 7220 6469 7669 736f 7273 2061  other divisors a
+00017b80: 7265 2061 7661 696c 6162 6c65 2028 7072  re available (pr
+00017b90: 696d 6520 6e75 6d62 6572 7329 0a20 2020  ime numbers).   
+00017ba0: 2062 6174 6368 7369 7a65 203d 2069 6e74   batchsize = int
+00017bb0: 2844 7261 7570 6e69 724d 6f64 656c 5574  (DraupnirModelUt
+00017bc0: 696c 732e 696e 7465 7276 616c 7328 6e5f  ils.intervals(n_
+00017bd0: 6368 756e 6b73 2c20 6e29 5b30 5d5b 315d  chunks, n)[0][1]
+00017be0: 290a 2020 2020 6966 2062 6174 6368 5f73  ).    if batch_s
+00017bf0: 697a 653a 7265 7475 726e 2062 6174 6368  ize:return batch
+00017c00: 7369 7a65 0a20 2020 2065 6c73 653a 7265  size.    else:re
+00017c10: 7475 726e 206e 5f63 6875 6e6b 730a 6465  turn n_chunks.de
+00017c20: 6620 636f 7661 7269 616e 6365 2878 2c79  f covariance(x,y
+00017c30: 293a 0a20 2020 2022 2222 436f 6d70 7574  ):.    """Comput
+00017c40: 6573 2063 726f 7373 2d63 6f76 6172 6961  es cross-covaria
+00017c50: 6e63 6520 6265 7477 6565 6e20 7665 6374  nce between vect
+00017c60: 6f72 732c 2061 6e64 2069 7320 6465 6669  ors, and is defi
+00017c70: 6e65 6420 6279 2063 6f76 5b58 2c59 5d3d  ned by cov[X,Y]=
+00017c80: 455b 2858 e288 92ce bc58 2928 59e2 8892  E[(X.....X)(Y...
+00017c90: cebc 5929 545d 2222 220a 2020 2020 4120  ..Y)T]""".    A 
+00017ca0: 3d20 746f 7263 682e 7371 7274 2874 6f72  = torch.sqrt(tor
+00017cb0: 6368 2e61 7261 6e67 6528 3132 292e 7265  ch.arange(12).re
+00017cc0: 7368 6170 6528 332c 2034 2929 2020 2320  shape(3, 4))  # 
+00017cd0: 736f 6d65 2033 2062 7920 3420 6172 7261  some 3 by 4 arra
+00017ce0: 790a 2020 2020 6220 3d20 746f 7263 682e  y.    b = torch.
+00017cf0: 7465 6e73 6f72 285b 5b32 5d2c 205b 345d  tensor([[2], [4]
+00017d00: 2c20 5b35 5d5d 2920 2023 2073 6f6d 6520  , [5]])  # some 
+00017d10: 3320 6279 2031 2076 6563 746f 720a 2020  3 by 1 vector.  
+00017d20: 2020 636f 7620 3d20 746f 7263 682e 646f    cov = torch.do
+00017d30: 7428 622e 5420 2d20 622e 6d65 616e 2829  t(b.T - b.mean()
+00017d40: 2c20 4120 2d20 412e 6d65 616e 2864 696d  , A - A.mean(dim
+00017d50: 3d30 2929 202f 2028 622e 7368 6170 655b  =0)) / (b.shape[
+00017d60: 305d 202d 2031 290a 2020 2020 7265 7475  0] - 1).    retu
+00017d70: 726e 2063 6f76 0a64 6566 2066 696e 645f  rn cov.def find_
+00017d80: 6e61 6e28 6172 7261 792c 6e61 6e3d 5472  nan(array,nan=Tr
+00017d90: 7565 293a 0a20 2020 2022 2222 4472 6f70  ue):.    """Drop
+00017da0: 7320 726f 7773 2069 6e20 6120 7465 6e73  s rows in a tens
+00017db0: 6f72 2063 6f6e 7461 696e 696e 6720 616e  or containing an
+00017dc0: 7920 6e61 6e20 7661 6c75 6573 0a20 2020  y nan values.   
+00017dd0: 203a 7061 7261 6d20 7465 6e73 6f72 2061   :param tensor a
+00017de0: 7272 6179 2222 220a 2020 2020 7368 6170  rray""".    shap
+00017df0: 6520 3d20 6172 7261 792e 7368 6170 650a  e = array.shape.
+00017e00: 2020 2020 7465 6e73 6f72 5f72 6573 6861      tensor_resha
+00017e10: 7065 6420 3d20 6172 7261 792e 7265 7368  ped = array.resh
+00017e20: 6170 6528 7368 6170 655b 305d 2c20 2d31  ape(shape[0], -1
+00017e30: 290a 2020 2020 2320 4472 6f70 2061 6c6c  ).    # Drop all
+00017e40: 2072 6f77 7320 636f 6e74 6169 6e69 6e67   rows containing
+00017e50: 2061 6e79 206e 616e 3a0a 2020 2020 6966   any nan:.    if
+00017e60: 206e 6f74 206e 616e 3a0a 2020 2020 2020   not nan:.      
+00017e70: 2020 7465 6e73 6f72 5f72 6573 6861 7065    tensor_reshape
+00017e80: 6420 3d20 7465 6e73 6f72 5f72 6573 6861  d = tensor_resha
+00017e90: 7065 645b 7e74 6f72 6368 2e61 6e79 2874  ped[~torch.any(t
+00017ea0: 656e 736f 725f 7265 7368 6170 6564 2e69  ensor_reshaped.i
+00017eb0: 736e 616e 2829 2c20 6469 6d3d 3129 5d0a  snan(), dim=1)].
+00017ec0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00017ed0: 2020 7465 6e73 6f72 5f72 6573 6861 7065    tensor_reshape
+00017ee0: 6420 3d20 7465 6e73 6f72 5f72 6573 6861  d = tensor_resha
+00017ef0: 7065 645b 746f 7263 682e 616e 7928 7465  ped[torch.any(te
+00017f00: 6e73 6f72 5f72 6573 6861 7065 642e 6973  nsor_reshaped.is
+00017f10: 6e61 6e28 292c 2064 696d 3d31 295d 0a20  nan(), dim=1)]. 
+00017f20: 2020 2023 2052 6573 6861 7065 2062 6163     # Reshape bac
+00017f30: 6b3a 0a20 2020 2061 7272 6179 203d 2074  k:.    array = t
+00017f40: 656e 736f 725f 7265 7368 6170 6564 2e72  ensor_reshaped.r
+00017f50: 6573 6861 7065 2874 656e 736f 725f 7265  eshape(tensor_re
+00017f60: 7368 6170 6564 2e73 6861 7065 5b30 5d2c  shaped.shape[0],
+00017f70: 202a 7368 6170 655b 313a 5d29 0a20 2020   *shape[1:]).   
+00017f80: 2072 6574 7572 6e20 6172 7261 790a 6465   return array.de
+00017f90: 6620 7261 6d61 6368 616e 6472 616e 5f70  f ramachandran_p
+00017fa0: 6c6f 7428 2064 6174 615f 616e 676c 6573  lot( data_angles
+00017fb0: 2c73 6176 655f 6469 7265 6374 6f72 792c  ,save_directory,
+00017fc0: 706c 6f74 5f74 6974 6c65 2c20 6f6e 655f  plot_title, one_
+00017fd0: 686f 745f 656e 636f 6465 6420 3d20 4661  hot_encoded = Fa
+00017fe0: 6c73 6520 293a 0a20 2020 2022 2222 506c  lse ):.    """Pl
+00017ff0: 6f74 7320 5261 6d61 6368 616e 6472 616e  ots Ramachandran
+00018000: 2070 6c6f 7473 2062 6574 7765 656e 2074   plots between t
+00018010: 6865 2070 6869 2061 6e64 2070 7369 2061  he phi and psi a
+00018020: 6e67 6c65 7320 696e 2074 6865 2064 6174  ngles in the dat
+00018030: 6173 6574 0a20 2020 203a 7061 7261 6d20  aset.    :param 
+00018040: 6e75 6d70 792d 6172 7261 7920 6461 7461  numpy-array data
+00018050: 5f61 6e67 6c65 7320 3a20 3364 2061 7272  _angles : 3d arr
+00018060: 6179 205b 6e5f 7365 712c 2061 6c69 676e  ay [n_seq, align
+00018070: 5f6c 656e 2c20 3330 5d2c 2077 6865 7265  _len, 30], where
+00018080: 2063 6f6c 756d 6e73 2031 2061 6e64 2032   columns 1 and 2
+00018090: 206f 7220 3231 2061 6e64 2032 3220 636f   or 21 and 22 co
+000180a0: 6e74 6169 6e20 7468 6520 616e 676c 6573  ntain the angles
+000180b0: 2069 6e20 7468 6520 6361 7365 206f 6620   in the case of 
+000180c0: 4e4f 5420 6f6e 652d 686f 7420 656e 636f  NOT one-hot enco
+000180d0: 6465 6420 616e 6420 6f6e 652d 686f 7420  ded and one-hot 
+000180e0: 656e 636f 6465 642c 2072 6573 7065 6374  encoded, respect
+000180f0: 6976 656c 790a 2020 2020 3a70 6172 616d  ively.    :param
+00018100: 2073 7472 2073 6176 655f 6469 7265 6374   str save_direct
+00018110: 6f72 793a 2070 6174 6820 746f 2073 6176  ory: path to sav
+00018120: 696e 6720 6469 7265 6374 6f72 790a 2020  ing directory.  
+00018130: 2020 3a70 6172 616d 2073 7472 2070 6c6f    :param str plo
+00018140: 745f 7469 746c 650a 2020 2020 3a70 6172  t_title.    :par
+00018150: 616d 2062 6f6f 6c20 6f6e 655f 686f 745f  am bool one_hot_
+00018160: 656e 636f 6465 640a 2020 2020 2222 220a  encoded.    """.
+00018170: 2020 2020 706c 742e 636c 6628 290a 2020      plt.clf().  
+00018180: 2020 6966 206f 6e65 5f68 6f74 5f65 6e63    if one_hot_enc
+00018190: 6f64 6564 3a0a 2020 2020 2020 2020 7068  oded:.        ph
+000181a0: 6920 3d20 6461 7461 5f61 6e67 6c65 735b  i = data_angles[
+000181b0: 3a2c 3a2c 3231 5d2e 7265 7368 6170 6528  :,:,21].reshape(
+000181c0: 2864 6174 615f 616e 676c 6573 2e73 6861  (data_angles.sha
+000181d0: 7065 5b30 5d2a 6461 7461 5f61 6e67 6c65  pe[0]*data_angle
+000181e0: 732e 7368 6170 655b 315d 2929 2e61 7374  s.shape[1])).ast
+000181f0: 7970 6528 666c 6f61 7429 2023 2d20 6e70  ype(float) #- np
+00018200: 2e70 690a 0a20 2020 2020 2020 2070 7369  .pi..        psi
+00018210: 203d 2064 6174 615f 616e 676c 6573 5b3a   = data_angles[:
+00018220: 2c3a 2c32 325d 2e72 6573 6861 7065 2828  ,:,22].reshape((
+00018230: 6461 7461 5f61 6e67 6c65 732e 7368 6170  data_angles.shap
+00018240: 655b 305d 2a64 6174 615f 616e 676c 6573  e[0]*data_angles
+00018250: 2e73 6861 7065 5b31 5d29 292e 6173 7479  .shape[1])).asty
+00018260: 7065 2866 6c6f 6174 2920 232d 206e 702e  pe(float) #- np.
+00018270: 7069 0a20 2020 2065 6c73 653a 0a20 2020  pi.    else:.   
+00018280: 2020 2020 2070 6869 203d 2064 6174 615f       phi = data_
+00018290: 616e 676c 6573 5b3a 2c3a 2c31 5d2e 7265  angles[:,:,1].re
+000182a0: 7368 6170 6528 2864 6174 615f 616e 676c  shape((data_angl
+000182b0: 6573 2e73 6861 7065 5b30 5d2a 6461 7461  es.shape[0]*data
+000182c0: 5f61 6e67 6c65 732e 7368 6170 655b 315d  _angles.shape[1]
+000182d0: 2929 2e61 7374 7970 6528 666c 6f61 7429  )).astype(float)
+000182e0: 0a20 2020 2020 2020 2070 7369 203d 2064  .        psi = d
+000182f0: 6174 615f 616e 676c 6573 5b3a 2c3a 2c32  ata_angles[:,:,2
+00018300: 5d2e 7265 7368 6170 6528 2864 6174 615f  ].reshape((data_
+00018310: 616e 676c 6573 2e73 6861 7065 5b30 5d2a  angles.shape[0]*
+00018320: 6461 7461 5f61 6e67 6c65 732e 7368 6170  data_angles.shap
+00018330: 655b 315d 2929 2e61 7374 7970 6528 666c  e[1])).astype(fl
+00018340: 6f61 7429 0a0a 2020 2020 6669 6720 3d20  oat)..    fig = 
+00018350: 706c 742e 6669 6775 7265 2866 6967 7369  plt.figure(figsi
+00018360: 7a65 3d28 352c 3529 290a 2020 2020 706c  ze=(5,5)).    pl
+00018370: 742e 6869 7374 3264 2820 7068 692c 2070  t.hist2d( phi, p
+00018380: 7369 2c20 6269 6e73 203d 2036 3238 2c20  si, bins = 628, 
+00018390: 6e6f 726d 203d 204c 6f67 4e6f 726d 2829  norm = LogNorm()
+000183a0: 2923 2c20 636d 6170 203d 2070 6c74 2e63  )#, cmap = plt.c
+000183b0: 6d2e 6a65 7420 290a 2020 2020 706c 742e  m.jet ).    plt.
+000183c0: 796c 696d 282d 6e70 2e70 692c 206e 702e  ylim(-np.pi, np.
+000183d0: 7069 290a 2020 2020 706c 742e 786c 696d  pi).    plt.xlim
+000183e0: 282d 6e70 2e70 692c 206e 702e 7069 290a  (-np.pi, np.pi).
+000183f0: 2020 2020 706c 742e 7469 746c 6528 706c      plt.title(pl
+00018400: 6f74 5f74 6974 6c65 2c66 6f6e 7473 697a  ot_title,fontsiz
+00018410: 653d 3132 290a 2020 2020 706c 742e 786c  e=12).    plt.xl
+00018420: 6162 656c 2827 cf86 2729 0a20 2020 2070  abel('..').    p
+00018430: 6c74 2e79 6c61 6265 6c28 27cf 8827 290a  lt.ylabel('..').
+00018440: 2020 2020 706c 742e 7361 7665 6669 6728      plt.savefig(
+00018450: 7361 7665 5f64 6972 6563 746f 7279 290a  save_directory).
+00018460: 2020 2020 706c 742e 636c 6628 290a 2020      plt.clf().  
+00018470: 2020 706c 742e 636c 6f73 6528 6669 6729    plt.close(fig)
+00018480: 0a64 6566 2072 616d 6163 6861 6e64 7261  .def ramachandra
+00018490: 6e5f 706c 6f74 5f73 616d 706c 6564 2870  n_plot_sampled(p
+000184a0: 6869 2c70 7369 2c73 6176 655f 6469 7265  hi,psi,save_dire
+000184b0: 6374 6f72 792c 706c 6f74 5f74 6974 6c65  ctory,plot_title
+000184c0: 2c70 6c6f 745f 6b61 7070 6173 3d46 616c  ,plot_kappas=Fal
+000184d0: 7365 293a 0a20 2020 2022 2222 506c 6f74  se):.    """Plot
+000184e0: 7320 5261 6d61 6368 616e 6472 616e 2070  s Ramachandran p
+000184f0: 6c6f 7473 2062 6574 7765 656e 2074 6865  lots between the
+00018500: 2070 6869 2061 6e64 2070 7369 2061 6e67   phi and psi ang
+00018510: 6c65 7320 696e 2074 6865 2064 6174 6173  les in the datas
+00018520: 6574 0a20 2020 203a 7061 7261 6d20 7465  et.    :param te
+00018530: 6e73 6f72 2070 6869 0a20 2020 203a 7061  nsor phi.    :pa
+00018540: 7261 6d20 7465 6e73 6f72 2070 7369 0a20  ram tensor psi. 
+00018550: 2020 203a 7061 7261 6d20 7374 7220 7361     :param str sa
+00018560: 7665 5f64 6972 6563 746f 7279 3a20 7061  ve_directory: pa
+00018570: 7468 2074 6f20 7361 7669 6e67 2064 6972  th to saving dir
+00018580: 6563 746f 7279 0a20 2020 203a 7061 7261  ectory.    :para
+00018590: 6d20 7374 7220 706c 6f74 5f74 6974 6c65  m str plot_title
+000185a0: 0a20 2020 203a 7061 7261 6d20 626f 6f6c  .    :param bool
+000185b0: 2070 6c6f 745f 6b61 7070 6173 0a20 2020   plot_kappas.   
+000185c0: 2022 2222 0a20 2020 2069 6620 6973 696e   """.    if isin
+000185d0: 7374 616e 6365 2870 6869 2c74 6f72 6368  stance(phi,torch
+000185e0: 2e54 656e 736f 7229 3a0a 2020 2020 2020  .Tensor):.      
+000185f0: 2020 7068 6920 3d20 7068 692e 7669 6577    phi = phi.view
+00018600: 282d 3129 2e63 7075 2829 2e64 6574 6163  (-1).cpu().detac
+00018610: 6828 292e 6e75 6d70 7928 290a 2020 2020  h().numpy().    
+00018620: 2020 2020 7073 6920 3d20 7073 692e 7669      psi = psi.vi
+00018630: 6577 282d 3129 2e63 7075 2829 2e64 6574  ew(-1).cpu().det
+00018640: 6163 6828 292e 6e75 6d70 7928 290a 2020  ach().numpy().  
+00018650: 2020 2361 7865 7320 3d20 5b5b 2d6e 702e    #axes = [[-np.
+00018660: 7069 2c20 6e70 2e70 695d 2c20 5b2d 6e70  pi, np.pi], [-np
+00018670: 2e70 692c 206e 702e 7069 5d5d 0a20 2020  .pi, np.pi]].   
+00018680: 2070 6c74 2e66 6967 7572 6528 6669 6773   plt.figure(figs
+00018690: 697a 653d 2835 2c35 2929 0a20 2020 2070  ize=(5,5)).    p
+000186a0: 6c74 2e68 6973 7432 6428 2070 6869 2c20  lt.hist2d( phi, 
+000186b0: 7073 692c 2062 696e 7320 3d20 3632 382c  psi, bins = 628,
+000186c0: 206e 6f72 6d20 3d20 4c6f 674e 6f72 6d28   norm = LogNorm(
+000186d0: 2929 232c 2063 6d61 7020 3d20 706c 742e  ))#, cmap = plt.
+000186e0: 636d 2e6a 6574 2029 0a20 2020 2069 6620  cm.jet ).    if 
+000186f0: 706c 6f74 5f6b 6170 7061 733a 0a20 2020  plot_kappas:.   
+00018700: 2020 2020 2070 6c74 2e78 6c61 6265 6c28       plt.xlabel(
+00018710: 274b 6170 7061 20cf 8627 290a 2020 2020  'Kappa ..').    
+00018720: 2020 2020 706c 742e 796c 6162 656c 2827      plt.ylabel('
+00018730: 4b61 7070 6120 cf88 2729 0a20 2020 2065  Kappa ..').    e
+00018740: 6c73 653a 0a20 2020 2020 2020 2070 6c74  lse:.        plt
+00018750: 2e79 6c69 6d28 2d6e 702e 7069 2c20 6e70  .ylim(-np.pi, np
+00018760: 2e70 6929 0a20 2020 2020 2020 2070 6c74  .pi).        plt
+00018770: 2e78 6c69 6d28 2d6e 702e 7069 2c20 6e70  .xlim(-np.pi, np
+00018780: 2e70 6929 0a20 2020 2020 2020 2070 6c74  .pi).        plt
+00018790: 2e78 6c61 6265 6c28 27cf 8627 290a 2020  .xlabel('..').  
+000187a0: 2020 2020 2020 706c 742e 796c 6162 656c        plt.ylabel
+000187b0: 2827 cf88 2729 0a20 2020 2070 6c74 2e74  ('..').    plt.t
+000187c0: 6974 6c65 2870 6c6f 745f 7469 746c 652c  itle(plot_title,
+000187d0: 666f 6e74 7369 7a65 3d31 3229 0a20 2020  fontsize=12).   
+000187e0: 2070 6c74 2e73 6176 6566 6967 2873 6176   plt.savefig(sav
+000187f0: 655f 6469 7265 6374 6f72 7929 0a20 2020  e_directory).   
+00018800: 2070 6c74 2e63 6c66 2829 0a20 2020 2070   plt.clf().    p
+00018810: 6c74 2e63 6c6f 7365 2829 0a64 6566 2067  lt.close().def g
+00018820: 7261 6469 656e 7473 5f70 6c6f 7428 6772  radients_plot(gr
+00018830: 6164 6965 6e74 5f6e 6f72 6d73 2c65 706f  adient_norms,epo
+00018840: 6368 732c 6469 7265 6374 6f72 7929 3a0a  chs,directory):.
+00018850: 2020 2020 2222 2256 6973 7561 6c69 7a61      """Visualiza
+00018860: 7469 6f6e 206f 6620 7468 6520 6772 6164  tion of the grad
+00018870: 6965 6e74 2064 6573 6365 6e74 2070 6572  ient descent per
+00018880: 206d 6f64 656c 2070 6172 616d 6574 6572   model parameter
+00018890: 0a20 2020 203a 7061 7261 6d20 6469 6374  .    :param dict
+000188a0: 2067 7261 6469 656e 745f 6e6f 726d 733a   gradient_norms:
+000188b0: 2064 6963 7469 6f6e 6172 7920 7769 7468   dictionary with
+000188c0: 2074 6865 206d 6f64 656c 2070 6172 616d   the model param
+000188d0: 6574 6572 7320 616e 6420 7468 6520 7061  eters and the pa
+000188e0: 7274 6961 6c20 6465 7269 7661 7469 7665  rtial derivative
+000188f0: 730a 2020 2020 3a70 6172 616d 2069 6e74  s.    :param int
+00018900: 2065 706f 6368 7322 2222 0a0a 2020 2020   epochs"""..    
+00018910: 6669 6720 3d20 706c 742e 6669 6775 7265  fig = plt.figure
+00018920: 2866 6967 7369 7a65 3d28 3136 2c20 3929  (figsize=(16, 9)
+00018930: 2c20 6470 693d 3130 3029 2e73 6574 5f66  , dpi=100).set_f
+00018940: 6163 6563 6f6c 6f72 2827 7768 6974 6527  acecolor('white'
+00018950: 290a 2020 2020 6178 203d 2070 6c74 2e73  ).    ax = plt.s
+00018960: 7562 706c 6f74 2831 3231 290a 2020 2020  ubplot(121).    
+00018970: 636f 6c6f 725f 6d61 7020 3d20 636d 2e72  color_map = cm.r
+00018980: 6169 6e62 6f77 286e 702e 6c69 6e73 7061  ainbow(np.linspa
+00018990: 6365 2830 2c20 312c 2034 3229 290a 2020  ce(0, 1, 42)).  
+000189a0: 2020 666f 7220 286e 616d 655f 692c 2067    for (name_i, g
+000189b0: 7261 645f 6e6f 726d 7329 2c20 636f 6c6f  rad_norms), colo
+000189c0: 7220 696e 207a 6970 2867 7261 6469 656e  r in zip(gradien
+000189d0: 745f 6e6f 726d 732e 6974 656d 7328 292c  t_norms.items(),
+000189e0: 2063 6f6c 6f72 5f6d 6170 293a 0a20 2020   color_map):.   
+000189f0: 2020 2020 2061 782e 706c 6f74 2867 7261       ax.plot(gra
+00018a00: 645f 6e6f 726d 732c 206c 6162 656c 3d6e  d_norms, label=n
+00018a10: 616d 655f 692c 2063 3d63 6f6c 6f72 290a  ame_i, c=color).
+00018a20: 2020 2020 706c 742e 786c 6162 656c 2827      plt.xlabel('
+00018a30: 6974 6572 7327 290a 2020 2020 706c 742e  iters').    plt.
+00018a40: 796c 6162 656c 2827 6772 6164 6965 6e74  ylabel('gradient
+00018a50: 206e 6f72 6d27 290a 2020 2020 706c 742e   norm').    plt.
+00018a60: 7973 6361 6c65 2827 6c6f 6727 290a 2020  yscale('log').  
+00018a70: 2020 6178 2e6c 6567 656e 6428 6c6f 633d    ax.legend(loc=
+00018a80: 2775 7070 6572 2063 656e 7465 7227 2c20  'upper center', 
+00018a90: 6262 6f78 5f74 6f5f 616e 6368 6f72 3d28  bbox_to_anchor=(
+00018aa0: 312e 352c 2031 292c 2073 6861 646f 773d  1.5, 1), shadow=
+00018ab0: 5472 7565 2c20 6e63 6f6c 3d31 2c20 7072  True, ncol=1, pr
+00018ac0: 6f70 3d7b 2773 697a 6527 3a20 387d 290a  op={'size': 8}).
+00018ad0: 2020 2020 706c 742e 7469 746c 6528 2747      plt.title('G
+00018ae0: 7261 6469 656e 7420 6e6f 726d 7320 6475  radient norms du
+00018af0: 7269 6e67 2053 5649 2729 0a20 2020 2070  ring SVI').    p
+00018b00: 6c74 2e73 6176 6566 6967 2822 7b7d 2f47  lt.savefig("{}/G
+00018b10: 7261 6469 656e 7473 5f7b 7d5f 6570 6f63  radients_{}_epoc
+00018b20: 6873 2e70 6e67 222e 666f 726d 6174 2864  hs.png".format(d
+00018b30: 6972 6563 746f 7279 2c65 706f 6368 7329  irectory,epochs)
+00018b40: 290a 2020 2020 706c 742e 636c 6628 290a  ).    plt.clf().
+00018b50: 2020 2020 706c 742e 636c 6f73 6528 290a      plt.close().
+00018b60: 0a64 6566 2072 656e 616d 696e 6728 7472  .def renaming(tr
+00018b70: 6565 293a 0a20 2020 2020 2020 2022 2222  ee):.        """
+00018b80: 5265 6e61 6d65 2074 6865 2069 6e74 6572  Rename the inter
+00018b90: 6e61 6c20 6e6f 6465 732c 2075 6e6c 6573  nal nodes, unles
+00018ba0: 7320 7468 6520 6769 7665 6e20 6e65 7769  s the given newi
+00018bb0: 636b 2066 696c 6520 616c 7265 6164 7920  ck file already 
+00018bc0: 6861 7320 7468 6520 6e61 6d65 7320 6f6e  has the names on
+00018bd0: 2069 740a 2020 2020 2020 2020 3a70 6172   it.        :par
+00018be0: 616d 2074 7265 653a 2065 7465 3320 666f  am tree: ete3 fo
+00018bf0: 726d 6174 2031 2074 7265 6522 2222 0a20  rmat 1 tree""". 
+00018c00: 2020 2020 2020 2023 5265 6e61 6d65 2074         #Rename t
+00018c10: 6865 2069 6e74 6572 6e61 6c20 6e6f 6465  he internal node
+00018c20: 730a 2020 2020 2020 2020 6c65 6166 735f  s.        leafs_
+00018c30: 6e61 6d65 7320 3d20 7472 6565 2e67 6574  names = tree.get
+00018c40: 5f6c 6561 665f 6e61 6d65 7328 290a 2020  _leaf_names().  
+00018c50: 2020 2020 2020 6564 6765 203d 206c 656e        edge = len
+00018c60: 286c 6561 6673 5f6e 616d 6573 290a 2020  (leafs_names).  
+00018c70: 2020 2020 2020 696e 7465 726e 616c 5f6e        internal_n
+00018c80: 6f64 6573 5f6e 616d 6573 203d 205b 5d0a  odes_names = [].
+00018c90: 2020 2020 2020 2020 666f 7220 6e6f 6465          for node
+00018ca0: 2069 6e20 7472 6565 2e74 7261 7665 7273   in tree.travers
+00018cb0: 6528 293a 2023 6c65 7665 6c6f 7264 6572  e(): #levelorder
+00018cc0: 2028 6e6f 6465 7320 6172 6520 7669 7369   (nodes are visi
+00018cd0: 7465 6420 696e 207a 6967 207a 6167 206f  ted in zig zag o
+00018ce0: 7264 6572 2066 726f 6d20 726f 6f74 2074  rder from root t
+00018cf0: 6f20 6c65 6176 6573 290a 2020 2020 2020  o leaves).      
+00018d00: 2020 2020 2020 6966 206e 6f74 206e 6f64        if not nod
+00018d10: 652e 6973 5f6c 6561 6628 293a 0a20 2020  e.is_leaf():.   
+00018d20: 2020 2020 2020 2020 2020 2020 206e 6f64               nod
+00018d30: 652e 6e61 6d65 203d 2022 4125 6422 2025  e.name = "A%d" %
+00018d40: 2065 6467 650a 2020 2020 2020 2020 2020   edge.          
+00018d50: 2020 2020 2020 696e 7465 726e 616c 5f6e        internal_n
+00018d60: 6f64 6573 5f6e 616d 6573 2e61 7070 656e  odes_names.appen
+00018d70: 6428 6e6f 6465 2e6e 616d 6529 0a20 2020  d(node.name).   
+00018d80: 2020 2020 2020 2020 2020 2020 2065 6467               edg
+00018d90: 6520 2b3d 2031 0a0a 6465 6620 6361 6c63  e += 1..def calc
+00018da0: 756c 6174 655f 6161 5f66 7265 7175 656e  ulate_aa_frequen
+00018db0: 6369 6573 2864 6174 6173 6574 2c66 7265  cies(dataset,fre
+00018dc0: 715f 6269 6e73 293a 0a20 2020 2022 2222  q_bins):.    """
+00018dd0: 4361 6c63 756c 6174 6573 2061 2066 7265  Calculates a fre
+00018de0: 7175 656e 6379 2066 6f72 2065 6163 6820  quency for each 
+00018df0: 6f66 2074 6865 2061 6120 2620 6761 7020  of the aa & gap 
+00018e00: 6174 2065 6163 6820 706f 7369 7469 6f6e  at each position
+00018e10: 2e54 6865 206e 756d 6265 7220 6f66 2062  .The number of b
+00018e20: 696e 7320 286f 6620 7369 7a65 2031 2920  ins (of size 1) 
+00018e30: 6973 206f 6e65 206c 6172 6765 7220 7468  is one larger th
+00018e40: 616e 2074 6865 206c 6172 6765 7374 2076  an the largest v
+00018e50: 616c 7565 2069 6e20 782e 2054 6869 7320  alue in x. This 
+00018e60: 6973 2064 6f6e 6520 666f 7220 6e75 6d70  is done for nump
+00018e70: 7920 6172 7261 7973 0a20 2020 203a 7061  y arrays.    :pa
+00018e80: 7261 6d20 7465 6e73 6f72 2064 6174 6173  ram tensor datas
+00018e90: 6574 0a20 2020 203a 7061 7261 6d20 696e  et.    :param in
+00018ea0: 7420 6672 6571 5f62 696e 730a 2020 2020  t freq_bins.    
+00018eb0: 2222 220a 2020 2020 6672 6571 7320 3d20  """.    freqs = 
+00018ec0: 6e70 2e61 7070 6c79 5f61 6c6f 6e67 5f61  np.apply_along_a
+00018ed0: 7869 7328 6c61 6d62 6461 2078 3a20 6e70  xis(lambda x: np
+00018ee0: 2e62 696e 636f 756e 7428 782c 206d 696e  .bincount(x, min
+00018ef0: 6c65 6e67 7468 3d66 7265 715f 6269 6e73  length=freq_bins
+00018f00: 292c 2061 7869 733d 302c 2061 7272 3d64  ), axis=0, arr=d
+00018f10: 6174 6173 6574 2e61 7374 7970 6528 2269  ataset.astype("i
+00018f20: 6e74 3634 2229 292e 540a 2020 2020 6672  nt64")).T.    fr
+00018f30: 6571 7320 3d20 6672 6571 732f 6461 7461  eqs = freqs/data
+00018f40: 7365 742e 7368 6170 655b 305d 0a20 2020  set.shape[0].   
+00018f50: 2072 6574 7572 6e20 6672 6571 730a 6465   return freqs.de
+00018f60: 6620 6361 6c63 756c 6174 655f 6161 5f66  f calculate_aa_f
+00018f70: 7265 7175 656e 6369 6573 5f74 6f72 6368  requencies_torch
+00018f80: 2864 6174 6173 6574 2c66 7265 715f 6269  (dataset,freq_bi
+00018f90: 6e73 293a 0a20 2020 2022 2222 4361 6c63  ns):.    """Calc
+00018fa0: 756c 6174 6573 2061 2066 7265 7175 656e  ulates a frequen
+00018fb0: 6379 2066 6f72 2065 6163 6820 6f66 2074  cy for each of t
+00018fc0: 6865 2061 6120 2620 6761 7020 6174 2065  he aa & gap at e
+00018fd0: 6163 6820 706f 7369 7469 6f6e 2e54 6865  ach position.The
+00018fe0: 206e 756d 6265 7220 6f66 2062 696e 7320   number of bins 
+00018ff0: 286f 6620 7369 7a65 2031 2920 6973 206f  (of size 1) is o
+00019000: 6e65 206c 6172 6765 7220 7468 616e 2074  ne larger than t
+00019010: 6865 206c 6172 6765 7374 2076 616c 7565  he largest value
+00019020: 2069 6e20 782e 2054 6869 7320 6973 2064   in x. This is d
+00019030: 6f6e 6520 666f 7220 746f 7263 6820 7465  one for torch te
+00019040: 6e73 6f72 730a 2020 2020 3a70 6172 616d  nsors.    :param
+00019050: 2074 656e 736f 7220 6461 7461 7365 740a   tensor dataset.
+00019060: 2020 2020 3a70 6172 616d 2069 6e74 2066      :param int f
+00019070: 7265 715f 6269 6e73 0a20 2020 2022 2222  req_bins.    """
+00019080: 0a20 2020 2066 7265 7173 203d 2074 6f72  .    freqs = tor
+00019090: 6368 2e73 7461 636b 285b 746f 7263 682e  ch.stack([torch.
+000190a0: 6269 6e63 6f75 6e74 2878 5f69 2c20 6d69  bincount(x_i, mi
+000190b0: 6e6c 656e 6774 683d 6672 6571 5f62 696e  nlength=freq_bin
+000190c0: 7329 2066 6f72 2069 2c20 785f 6920 696e  s) for i, x_i in
+000190d0: 2065 6e75 6d65 7261 7465 2874 6f72 6368   enumerate(torch
+000190e0: 2e75 6e62 696e 6428 6461 7461 7365 742e  .unbind(dataset.
+000190f0: 7479 7065 2874 6f72 6368 2e69 6e74 3634  type(torch.int64
+00019100: 292c 2064 696d 3d31 292c 2030 295d 2c20  ), dim=1), 0)], 
+00019110: 6469 6d3d 3129 0a20 2020 2066 7265 7173  dim=1).    freqs
+00019120: 203d 2066 7265 7173 2e54 0a20 2020 2066   = freqs.T.    f
+00019130: 7265 7173 203d 2066 7265 7173 202f 2064  reqs = freqs / d
+00019140: 6174 6173 6574 2e73 6861 7065 5b30 5d0a  ataset.shape[0].
+00019150: 2020 2020 7265 7475 726e 2066 7265 7173      return freqs
+00019160: 0a64 6566 2063 6f6d 7061 7265 5f74 7265  .def compare_tre
+00019170: 6573 2874 312c 7432 293a 0a20 2020 2022  es(t1,t2):.    "
+00019180: 2222 436f 6d70 7574 6573 2074 6865 2052  ""Computes the R
+00019190: 6620 6469 7374 616e 6365 2061 6d6f 6e67  f distance among
+000191a0: 2074 776f 2074 7265 652c 2069 7420 6361   two tree, it ca
+000191b0: 6c63 756c 6174 6573 2074 6865 206e 756d  lculates the num
+000191c0: 6265 7220 6f66 2063 6861 6e67 6573 2072  ber of changes r
+000191d0: 6571 7569 7265 7320 746f 2074 7261 6e73  equires to trans
+000191e0: 666f 726d 206f 6e65 2074 7265 6520 696e  form one tree in
+000191f0: 746f 2074 6865 206f 7468 6572 0a20 2020  to the other.   
+00019200: 203a 7061 7261 6d20 7374 7220 7431 3a20   :param str t1: 
+00019210: 7061 7468 2074 6f20 6669 7273 7420 6e65  path to first ne
+00019220: 7477 6963 6b20 7472 6565 0a20 2020 203a  twick tree.    :
+00019230: 7061 7261 6d20 7374 7220 7432 3a20 7061  param str t2: pa
+00019240: 7468 2074 6f20 7365 636f 6e64 206e 6574  th to second net
+00019250: 7769 636b 2074 7265 6522 2222 0a20 2020  wick tree""".   
+00019260: 2063 6f6c 756d 6e73 203d 205b 2252 4620   columns = ["RF 
+00019270: 6469 7374 616e 6365 222c 224d 6178 696d  distance","Maxim
+00019280: 756d 2052 4620 6469 7374 616e 6365 222c  um RF distance",
+00019290: 2243 6f6d 6d6f 6e20 6c65 6176 6573 222c  "Common leaves",
+000192a0: 2250 6172 7469 7469 6f6e 7349 6e5f 7431  "PartitionsIn_t1
+000192b0: 5f4e 4f54 5f74 3222 2c22 5061 7274 6974  _NOT_t2","Partit
+000192c0: 696f 6e73 496e 5f74 325f 4e4f 545f 7431  ionsIn_t2_NOT_t1
+000192d0: 222c 2244 6973 6361 7264 6564 5f70 6172  ","Discarded_par
+000192e0: 7469 7469 6f6e 735f 7431 222c 2244 6973  titions_t1","Dis
+000192f0: 6361 7264 6564 5f70 6172 7469 7469 6f6e  carded_partition
+00019300: 735f 7432 225d 0a20 2020 2023 2074 3120  s_t2"].    # t1 
+00019310: 203d 2054 7265 6545 7465 3328 7431 290a   = TreeEte3(t1).
+00019320: 2020 2020 2320 7432 203d 2054 7265 6545      # t2 = TreeE
+00019330: 7465 3328 7432 290a 2020 2020 2320 7265  te3(t2).    # re
+00019340: 7375 6c74 7320 3d20 7431 2e72 6f62 696e  sults = t1.robin
+00019350: 736f 6e5f 666f 756c 6473 2874 322c 756e  son_foulds(t2,un
+00019360: 726f 6f74 6564 5f74 7265 6573 3d54 7275  rooted_trees=Tru
+00019370: 6529 0a20 2020 2063 6f6d 6d61 6e64 203d  e).    command =
+00019380: 2027 5273 6372 6970 7427 0a20 2020 2070   'Rscript'.    p
+00019390: 6174 6832 7363 7269 7074 203d 2027 2f68  ath2script = '/h
+000193a0: 6f6d 652f 6c79 732f 4472 6f70 626f 782f  ome/lys/Dropbox/
+000193b0: 5068 442f 4452 4155 504e 4952 2f54 7265  PhD/DRAUPNIR/Tre
+000193c0: 655f 4469 7374 616e 6365 2e52 270a 2020  e_Distance.R'.  
+000193d0: 2020 2320 4275 696c 6420 7375 6270 726f    # Build subpro
+000193e0: 6365 7373 2063 6f6d 6d61 6e64 0a20 2020  cess command.   
+000193f0: 2061 7267 7320 3d5b 7431 2c74 325d 0a20   args =[t1,t2]. 
+00019400: 2020 2063 6d64 203d 205b 636f 6d6d 616e     cmd = [comman
+00019410: 642c 2070 6174 6832 7363 7269 7074 5d20  d, path2script] 
+00019420: 2b20 6172 6773 0a20 2020 2064 6973 7461  + args.    dista
+00019430: 6e63 6520 3d20 7375 6270 726f 6365 7373  nce = subprocess
+00019440: 2e63 6865 636b 5f6f 7574 7075 7428 636d  .check_output(cm
+00019450: 642c 2075 6e69 7665 7273 616c 5f6e 6577  d, universal_new
+00019460: 6c69 6e65 733d 5472 7565 290a 2020 2020  lines=True).    
+00019470: 7265 7475 726e 2064 6973 7461 6e63 650a  return distance.
+00019480: 0a64 6566 2072 656d 6f76 655f 7374 6f70  .def remove_stop
+00019490: 5f63 6f64 6f6e 7328 7365 7175 656e 6365  _codons(sequence
+000194a0: 5f66 696c 652c 6973 5f70 726f 743d 4661  _file,is_prot=Fa
+000194b0: 6c73 6529 3a0a 2020 2020 2222 2252 656d  lse):.    """Rem
+000194c0: 6f76 6520 7468 6520 7374 6f70 2063 6f64  ove the stop cod
+000194d0: 6f6e 7328 2a29 2066 726f 6d20 616e 2061  ons(*) from an a
+000194e0: 6c69 676e 6d65 6e74 2066 696c 6522 2222  lignment file"""
+000194f0: 0a20 2020 2069 6620 6973 5f70 726f 743a  .    if is_prot:
+00019500: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00019510: 5265 6d6f 7669 6e67 2073 746f 7020 636f  Removing stop co
+00019520: 646f 6e73 2066 726f 6d20 7072 6f74 6569  dons from protei
+00019530: 6e22 290a 2020 2020 2020 2020 7072 696e  n").        prin
+00019540: 7428 7365 7175 656e 6365 5f66 696c 6529  t(sequence_file)
+00019550: 0a20 2020 2020 2020 2073 6571 5f66 696c  .        seq_fil
+00019560: 6520 3d20 6f70 656e 2873 6571 7565 6e63  e = open(sequenc
+00019570: 655f 6669 6c65 2c20 2772 2b27 290a 2020  e_file, 'r+').  
+00019580: 2020 2020 2020 7365 7120 3d20 7365 715f        seq = seq_
+00019590: 6669 6c65 2e72 6561 6428 290a 2020 2020  file.read().    
+000195a0: 2020 2020 7365 715f 6669 6c65 2e73 6565      seq_file.see
+000195b0: 6b28 3029 0a20 2020 2020 2020 206e 6f5f  k(0).        no_
+000195c0: 636f 646f 6e73 203d 205b 6920 6966 2069  codons = [i if i
+000195d0: 213d 222a 2220 656c 7365 2022 2d22 2066  !="*" else "-" f
+000195e0: 6f72 2069 2069 6e20 7365 715d 2023 7265  or i in seq] #re
+000195f0: 706c 6163 6520 666f 7220 6120 6761 700a  place for a gap.
+00019600: 2020 2020 2020 2020 2354 4f44 4f3a 2054          #TODO: T
+00019610: 7275 6e63 6174 6520 7468 6520 7365 7175  runcate the sequ
+00019620: 656e 6365 2069 6620 7468 6572 6520 6973  ence if there is
+00019630: 2061 2073 746f 7020 636f 646f 6e20 696e   a stop codon in
+00019640: 2074 6865 206d 6964 646c 6520 2873 746f   the middle (sto
+00019650: 7020 6164 6469 6e67 2067 6170 7320 7768  p adding gaps wh
+00019660: 656e 205c 6e20 6973 2072 6561 6368 6564  en \n is reached
+00019670: 290a 2020 2020 2020 2020 2320 6e6f 5f63  ).        # no_c
+00019680: 6f64 6f6e 733d 205b 5d0a 2020 2020 2020  odons= [].      
+00019690: 2020 2320 666f 7220 696e 6465 782c 6920    # for index,i 
+000196a0: 696e 2065 6e75 6d65 7261 7465 2873 6571  in enumerate(seq
+000196b0: 293a 0a20 2020 2020 2020 2023 2020 2020  ):.        #    
+000196c0: 2069 6620 6920 3d3d 2022 2a22 3a0a 2020   if i == "*":.  
+000196d0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+000196e0: 693d 2022 2d22 0a20 2020 2020 2020 2023  i= "-".        #
+000196f0: 2020 2020 2020 2020 206e 6578 745f 6272           next_br
+00019700: 6561 6b5f 696e 6465 7820 3d20 7365 715b  eak_index = seq[
+00019710: 696e 6465 783a 5d2e 696e 6465 7828 225c  index:].index("\
+00019720: 6e22 290a 2020 2020 2020 2020 2320 2020  n").        #   
+00019730: 2020 2020 2020 7365 715b 696e 6465 783a        seq[index:
+00019740: 6e65 7874 5f62 7265 616b 5f69 6e64 6578  next_break_index
+00019750: 5d20 3d20 222d 222a 286e 6578 745f 6272  ] = "-"*(next_br
+00019760: 6561 6b5f 696e 6465 782d 696e 6465 7829  eak_index-index)
+00019770: 0a0a 2020 2020 2020 2020 7365 715f 6669  ..        seq_fi
+00019780: 6c65 2e77 7269 7465 2822 222e 6a6f 696e  le.write("".join
+00019790: 286e 6f5f 636f 646f 6e73 2929 0a20 2020  (no_codons)).   
+000197a0: 2020 2020 2073 6571 5f66 696c 652e 7472       seq_file.tr
+000197b0: 756e 6361 7465 2829 2020 2320 7265 6d6f  uncate()  # remo
+000197c0: 7665 2063 6f6e 7465 6e74 730a 2020 2020  ve contents.    
+000197d0: 656c 7365 3a0a 2020 2020 2020 2020 7374  else:.        st
+000197e0: 6f70 5f63 6f64 6f6e 7320 3d20 5b22 5447  op_codons = ["TG
+000197f0: 4122 2c22 5441 4722 2c22 5441 4122 5d0a  A","TAG","TAA"].
+00019800: 2020 2020 2020 2020 7365 715f 6669 6c65          seq_file
+00019810: 203d 206f 7065 6e28 7365 7175 656e 6365   = open(sequence
+00019820: 5f66 696c 652c 2027 722b 2729 0a20 2020  _file, 'r+').   
+00019830: 2020 2020 2073 6571 203d 2073 6571 5f66       seq = seq_f
+00019840: 696c 652e 7265 6164 2829 0a20 2020 2020  ile.read().     
+00019850: 2020 2073 6571 5f66 696c 652e 7365 656b     seq_file.seek
+00019860: 2830 290a 2020 2020 2020 2020 2363 6f64  (0).        #cod
+00019870: 696e 675f 646e 6120 3d20 5365 7128 7365  ing_dna = Seq(se
+00019880: 7129 0a20 2020 2020 2020 2023 7072 6f74  q).        #prot
+00019890: 6569 6e20 3d20 636f 6469 6e67 5f64 6e61  ein = coding_dna
+000198a0: 2e74 7261 6e73 6c61 7465 2829 0a20 2020  .translate().   
+000198b0: 2020 2020 2063 6f64 6f6e 7320 3d20 5b73       codons = [s
+000198c0: 6571 5b69 3a69 2b33 5d20 666f 7220 6920  eq[i:i+3] for i 
+000198d0: 696e 2072 616e 6765 2830 2c20 6c65 6e28  in range(0, len(
+000198e0: 7365 7129 2c20 3329 5d0a 2020 2020 2020  seq), 3)].      
+000198f0: 2020 636f 646f 6e73 203d 5b63 6f64 2066    codons =[cod f
+00019900: 6f72 2063 6f64 2069 6e20 636f 646f 6e73  or cod in codons
+00019910: 2069 6620 6c65 6e28 636f 6429 203d 3d33   if len(cod) ==3
+00019920: 2061 6e64 2063 6f64 206e 6f74 2069 6e20   and cod not in 
+00019930: 7374 6f70 5f63 6f64 6f6e 735d 0a20 2020  stop_codons].   
+00019940: 2020 2020 2023 6368 6563 6b20 3d20 616e       #check = an
+00019950: 7928 6974 656d 2069 6e20 636f 646f 6e73  y(item in codons
+00019960: 2066 6f72 2069 7465 6d20 696e 2073 746f   for item in sto
+00019970: 705f 636f 646f 6e73 290a 2020 2020 2020  p_codons).      
+00019980: 2020 7365 715f 6669 6c65 2e77 7269 7465    seq_file.write
+00019990: 2822 222e 6a6f 696e 2863 6f64 6f6e 7329  ("".join(codons)
+000199a0: 290a 2020 2020 2020 2020 7365 715f 6669  ).        seq_fi
+000199b0: 6c65 2e74 7275 6e63 6174 6528 2920 2023  le.truncate()  #
+000199c0: 2072 656d 6f76 6520 636f 6e74 656e 7473   remove contents
+000199d0: 0a0a 6465 6620 636f 6e76 6572 745f 746f  ..def convert_to
+000199e0: 5f69 6e74 6567 6572 7328 6461 7461 7365  _integers(datase
+000199f0: 742c 6161 5f70 726f 6273 2c61 7869 7329  t,aa_probs,axis)
+00019a00: 3a0a 2020 2020 2222 2254 7261 6e73 666f  :.    """Transfo
+00019a10: 726d 7320 6f6e 6520 686f 7420 656e 636f  rms one hot enco
+00019a20: 6465 6420 616d 696e 6f20 6163 6964 7320  ded amino acids 
+00019a30: 696e 746f 2030 2d69 6e64 6578 6564 2069  into 0-indexed i
+00019a40: 6e74 6567 6572 7320 692e 6520 5b31 2c30  ntegers i.e [1,0
+00019a50: 2c30 2c30 5d20 2d2d 3e20 3020 205b 302c  ,0,0] --> 0  [0,
+00019a60: 312c 302c 305d 202d 3e20 310a 2020 2020  1,0,0] -> 1.    
+00019a70: 3a70 6172 616d 206e 756d 7079 2064 6174  :param numpy dat
+00019a80: 6173 6574 0a20 2020 203a 7061 7261 6d20  aset.    :param 
+00019a90: 6161 5f70 726f 6273 3a20 616d 696e 6f20  aa_probs: amino 
+00019aa0: 6163 6964 2070 726f 6261 6269 6c69 7469  acid probabiliti
+00019ab0: 6573 2c20 6469 6d65 6e73 696f 6e73 206f  es, dimensions o
+00019ac0: 6620 7468 6520 6f6e 652d 686f 7420 656e  f the one-hot en
+00019ad0: 636f 6469 6e67 2222 220a 2020 2020 6966  coding""".    if
+00019ae0: 2061 7869 733d 3d33 3a23 7573 6520 666f   axis==3:#use fo
+00019af0: 7220 7072 6564 6963 7469 6f6e 730a 2020  r predictions.  
+00019b00: 2020 2020 2020 6220 3d20 746f 7263 682e        b = torch.
+00019b10: 6172 676d 6178 2864 6174 6173 6574 2c20  argmax(dataset, 
+00019b20: 6469 6d3d 6178 6973 290a 2020 2020 656c  dim=axis).    el
+00019b30: 7365 3a0a 2020 2020 2020 2020 696e 7465  se:.        inte
+00019b40: 6765 7273 203d 2074 6f72 6368 2e61 7267  gers = torch.arg
+00019b50: 6d61 7828 6461 7461 7365 745b 3a2c 323a  max(dataset[:,2:
+00019b60: 2c30 3a61 615f 7072 6f62 735d 2c64 696d  ,0:aa_probs],dim
+00019b70: 3d61 7869 7329 0a20 2020 2020 2020 2062  =axis).        b
+00019b80: 203d 2074 6f72 6368 2e7a 6572 6f73 2864   = torch.zeros(d
+00019b90: 6174 6173 6574 5b3a 2c3a 2c30 5d2e 7368  ataset[:,:,0].sh
+00019ba0: 6170 6520 2b20 2833 302c 2929 2e63 7075  ape + (30,)).cpu
+00019bb0: 2829 0a20 2020 2020 2020 2023 6220 3d20  ().        #b = 
+00019bc0: 6e70 2e7a 6572 6f73 2844 6174 6173 6574  np.zeros(Dataset
+00019bd0: 5b3a 2c3a 2c30 5d2e 7368 6170 6520 2b20  [:,:,0].shape + 
+00019be0: 2833 302c 2929 0a20 2020 2020 2020 2062  (30,)).        b
+00019bf0: 5b3a 2c20 323a 2c20 305d 203d 2069 6e74  [:, 2:, 0] = int
+00019c00: 6567 6572 730a 2020 2020 2020 2020 625b  egers.        b[
+00019c10: 3a2c 3a32 5d20 3d20 6461 7461 7365 745b  :,:2] = dataset[
+00019c20: 3a2c 3a32 5d0a 2020 2020 7265 7475 726e  :,:2].    return
+00019c30: 2062 0a64 6566 2070 726f 6365 7373 5f62   b.def process_b
+00019c40: 6c6f 7375 6d28 626c 6f73 756d 2c61 615f  losum(blosum,aa_
+00019c50: 6672 6571 732c 616c 6967 6e5f 7365 715f  freqs,align_seq_
+00019c60: 6c65 6e2c 6161 5f70 726f 6273 293a 0a20  len,aa_probs):. 
+00019c70: 2020 2022 2222 0a20 2020 2043 6f6d 7075     """.    Compu
+00019c80: 7465 7320 7468 6520 6d61 7472 6963 6573  tes the matrices
+00019c90: 2072 6571 7569 7265 6420 746f 2062 7569   required to bui
+00019ca0: 6c64 2061 2062 6c6f 7375 6d20 656d 6265  ld a blosum embe
+00019cb0: 6464 696e 670a 2020 2020 3a70 6172 616d  dding.    :param
+00019cc0: 2074 656e 736f 7220 626c 6f73 756d 3a20   tensor blosum: 
+00019cd0: 424c 4f53 554d 206c 696b 656c 6968 6f6f  BLOSUM likelihoo
+00019ce0: 6420 2073 636f 7265 730a 2020 2020 3a70  d  scores.    :p
+00019cf0: 6172 616d 2074 656e 736f 7220 6161 5f66  aram tensor aa_f
+00019d00: 7265 7173 203a 2061 6d69 6e6f 2061 6369  reqs : amino aci
+00019d10: 6420 6672 6571 7565 6e63 6965 7320 7065  d frequencies pe
+00019d20: 7220 706f 7369 7469 6f6e 0a20 2020 203a  r position.    :
+00019d30: 7061 7261 6d20 616c 6967 6e5f 7365 715f  param align_seq_
+00019d40: 6c65 6e3a 2061 6c69 676e 6d65 6e74 206c  len: alignment l
+00019d50: 656e 6774 680a 2020 2020 3a70 6172 616d  ength.    :param
+00019d60: 2061 615f 7072 6f62 733a 2061 6d69 6e6f   aa_probs: amino
+00019d70: 2061 6369 6420 7072 6f62 6162 696c 6974   acid probabilit
+00019d80: 6965 732c 2074 7970 6573 206f 6620 616d  ies, types of am
+00019d90: 696e 6f20 6163 6964 7320 696e 2074 6865  ino acids in the
+00019da0: 2061 6c69 676e 6d65 6e74 0a20 2020 203a   alignment.    :
+00019db0: 6f75 7420 7465 6e73 6f72 2062 6c6f 7375  out tensor blosu
+00019dc0: 6d5f 6d61 7820 5b61 6c69 676e 5f6c 656e  m_max [align_len
+00019dd0: 2c61 615f 7072 6f62 5d3a 2062 6c6f 7375  ,aa_prob]: blosu
+00019de0: 6d20 6c69 6b65 6c69 686f 6f64 2073 636f  m likelihood sco
+00019df0: 7265 7320 666f 7220 7468 6520 6d6f 7374  res for the most
+00019e00: 2066 7265 7175 656e 7420 6161 2069 6e20   frequent aa in 
+00019e10: 7468 6520 616c 6967 6e6d 656e 7420 706f  the alignment po
+00019e20: 7369 7469 6f6e 0a20 2020 203a 6f75 7420  sition.    :out 
+00019e30: 7465 6e73 6f72 2062 6c6f 7375 6d5f 7765  tensor blosum_we
+00019e40: 6967 6874 6564 205b 616c 6967 6e5f 6c65  ighted [align_le
+00019e50: 6e2c 6161 5f70 726f 623a 2077 6569 6768  n,aa_prob: weigh
+00019e60: 7465 6420 6176 6572 6167 6520 6f66 2062  ted average of b
+00019e70: 6c6f 7375 6d20 6c69 6b65 6c69 686f 6f64  losum likelihood
+00019e80: 7320 6163 636f 7264 696e 6720 746f 2074  s according to t
+00019e90: 6865 2061 6120 6672 6571 7565 6e63 790a  he aa frequency.
+00019ea0: 2020 2020 3a6f 7574 2076 6172 6961 626c      :out variabl
+00019eb0: 655f 636f 7265 3a20 5b61 6c69 676e 5f6c  e_core: [align_l
+00019ec0: 656e 5d20 3a20 636f 756e 7473 2074 6865  en] : counts the
+00019ed0: 206e 756d 6265 7220 6f66 2064 6966 6665   number of diffe
+00019ee0: 7265 6e74 2065 6c65 6d65 6e74 7320 2861  rent elements (a
+00019ef0: 6d69 6e6f 2061 6369 6420 6469 7665 7273  mino acid divers
+00019f00: 6974 7929 2070 6572 2061 6c69 676e 6d65  ity) per alignme
+00019f10: 6e74 2070 6f73 6974 696f 6e22 2222 0a0a  nt position"""..
+00019f20: 2020 2020 6161 5f66 7265 7173 5f6d 6178      aa_freqs_max
+00019f30: 203d 2074 6f72 6368 2e61 7267 6d61 7828   = torch.argmax(
+00019f40: 6161 5f66 7265 7173 2c20 6469 6d3d 3129  aa_freqs, dim=1)
+00019f50: 2e72 6570 6561 7428 6161 5f70 726f 6273  .repeat(aa_probs
+00019f60: 2c20 3129 2e70 6572 6d75 7465 2831 2c20  , 1).permute(1, 
+00019f70: 3029 2023 5b6d 6178 5f6c 656e 2c20 6161  0) #[max_len, aa
+00019f80: 5f70 726f 6273 5d0a 2020 2020 626c 6f73  _probs].    blos
+00019f90: 756d 5f65 7870 616e 6465 6420 3d20 626c  um_expanded = bl
+00019fa0: 6f73 756d 5b31 3a2c 2031 3a5d 2e72 6570  osum[1:, 1:].rep
+00019fb0: 6561 7428 616c 6967 6e5f 7365 715f 6c65  eat(align_seq_le
+00019fc0: 6e2c 2031 2c20 3129 2020 2320 5b6d 6178  n, 1, 1)  # [max
+00019fd0: 5f6c 656e 2c61 615f 7072 6f62 732c 6161  _len,aa_probs,aa
+00019fe0: 5f70 726f 6273 5d0a 2020 2020 626c 6f73  _probs].    blos
+00019ff0: 756d 5f6d 6178 203d 2062 6c6f 7375 6d5f  um_max = blosum_
+0001a000: 6578 7061 6e64 6564 2e67 6174 6865 7228  expanded.gather(
+0001a010: 312c 2061 615f 6672 6571 735f 6d61 782e  1, aa_freqs_max.
+0001a020: 756e 7371 7565 657a 6528 3129 292e 7371  unsqueeze(1)).sq
+0001a030: 7565 657a 6528 3129 2020 2320 5b61 6c69  ueeze(1)  # [ali
+0001a040: 676e 5f73 6571 5f6c 656e 2c32 315d 2053  gn_seq_len,21] S
+0001a050: 6565 6d73 2063 6f72 7265 6374 0a0a 2020  eems correct..  
+0001a060: 2020 626c 6f73 756d 5f77 6569 6768 7465    blosum_weighte
+0001a070: 6420 3d20 6161 5f66 7265 7173 5b3a 2c3a  d = aa_freqs[:,:
+0001a080: 2c4e 6f6e 655d 2a62 6c6f 7375 6d5f 6578  ,None]*blosum_ex
+0001a090: 7061 6e64 6564 2023 2d2d 3e20 7265 706c  panded #--> repl
+0001a0a0: 6163 6520 3020 7769 7468 206e 616e 733f  ace 0 with nans?
+0001a0b0: 206f 7468 6572 7769 7365 2074 6865 2030   otherwise the 0
+0001a0c0: 2061 7265 2069 6e20 7468 6520 6d65 616e   are in the mean
+0001a0d0: 2061 7320 7765 6c6c 2e2e 2e2e 0a20 2020   as well.....   
+0001a0e0: 2062 6c6f 7375 6d5f 7765 6967 6874 6564   blosum_weighted
+0001a0f0: 203d 2062 6c6f 7375 6d5f 7765 6967 6874   = blosum_weight
+0001a100: 6564 2e6d 6561 6e28 6469 6d3d 3129 0a0a  ed.mean(dim=1)..
+0001a110: 2020 2020 7661 7269 6162 6c65 5f73 636f      variable_sco
+0001a120: 7265 203d 2074 6f72 6368 2e63 6f75 6e74  re = torch.count
+0001a130: 5f6e 6f6e 7a65 726f 2861 615f 6672 6571  _nonzero(aa_freq
+0001a140: 732c 2064 696d 3d31 292f 6161 5f70 726f  s, dim=1)/aa_pro
+0001a150: 6273 2023 6869 6768 6572 2073 636f 7265  bs #higher score
+0001a160: 2c20 6d6f 7265 2076 6172 6961 626c 650a  , more variable.
+0001a170: 0a20 2020 2072 6574 7572 6e20 626c 6f73  .    return blos
+0001a180: 756d 5f6d 6178 2c62 6c6f 7375 6d5f 7765  um_max,blosum_we
+0001a190: 6967 6874 6564 2c20 7661 7269 6162 6c65  ighted, variable
+0001a1a0: 5f73 636f 7265 0a64 6566 2062 6c6f 7375  _score.def blosu
+0001a1b0: 6d5f 656d 6265 6464 696e 675f 656e 636f  m_embedding_enco
+0001a1c0: 6465 7228 626c 6f73 756d 2c61 615f 6672  der(blosum,aa_fr
+0001a1d0: 6571 732c 616c 6967 6e5f 7365 715f 6c65  eqs,align_seq_le
+0001a1e0: 6e2c 6161 5f70 726f 6273 2c64 6174 6173  n,aa_probs,datas
+0001a1f0: 6574 5f74 7261 696e 2c20 6f6e 655f 686f  et_train, one_ho
+0001a200: 745f 656e 636f 6469 6e67 293a 0a20 2020  t_encoding):.   
+0001a210: 2022 2222 5472 616e 7366 6f72 6d73 2074   """Transforms t
+0001a220: 6865 2074 7261 696e 2064 6174 6173 6574  he train dataset
+0001a230: 2c20 7768 6963 6820 6973 2066 6f72 6d65  , which is forme
+0001a240: 6420 6279 2061 2074 656e 736f 7220 6f66  d by a tensor of
+0001a250: 2069 6e74 6567 6572 7320 7468 6174 2072   integers that r
+0001a260: 6570 7265 7365 6e74 2074 6865 2061 6d69  epresent the ami
+0001a270: 6e6f 2061 6369 6473 2c20 696e 746f 2061  no acids, into a
+0001a280: 2064 6174 6173 6574 2077 6865 7265 2065   dataset where e
+0001a290: 6163 6820 616d 696e 6f20 6163 6964 2028  ach amino acid (
+0001a2a0: 696e 7465 6765 7229 2069 7320 6578 6368  integer) is exch
+0001a2b0: 616e 6765 6420 7769 7468 2069 7473 2062  anged with its b
+0001a2c0: 6c6f 7375 6d20 7363 6f72 650a 2020 2020  losum score.    
+0001a2d0: 3a6f 7574 2074 656e 736f 7220 6161 5f74  :out tensor aa_t
+0001a2e0: 7261 696e 5f62 6c6f 7375 6d20 3a20 5472  rain_blosum : Tr
+0001a2f0: 6169 6e69 6e67 2064 6174 6173 6574 2077  aining dataset w
+0001a300: 6974 6820 7468 6520 626c 6f73 756d 2076  ith the blosum v
+0001a310: 6563 746f 7273 2069 6e73 7465 6164 206f  ectors instead o
+0001a320: 6620 7468 6520 616d 696e 6f20 6163 6964  f the amino acid
+0001a330: 7320 286e 756d 6265 7273 206f 7220 6f6e  s (numbers or on
+0001a340: 6520 686f 7420 7265 7072 6573 656e 7461  e hot representa
+0001a350: 7469 6f6e 2922 2222 0a20 2020 2069 6620  tion)""".    if 
+0001a360: 6f6e 655f 686f 745f 656e 636f 6469 6e67  one_hot_encoding
+0001a370: 3a0a 2020 2020 2020 2020 6461 7461 7365  :.        datase
+0001a380: 745f 7472 6169 6e20 3d20 636f 6e76 6572  t_train = conver
+0001a390: 745f 746f 5f69 6e74 6567 6572 7328 6461  t_to_integers(da
+0001a3a0: 7461 7365 745f 7472 6169 6e2c 6161 5f70  taset_train,aa_p
+0001a3b0: 726f 6273 2c61 7869 733d 3229 0a20 2020  robs,axis=2).   
+0001a3c0: 2061 6d69 6e6f 6163 6964 735f 7365 7173   aminoacids_seqs
+0001a3d0: 203d 2064 6174 6173 6574 5f74 7261 696e   = dataset_train
+0001a3e0: 5b3a 2c32 3a2c 305d 2e72 6570 6561 7428  [:,2:,0].repeat(
+0001a3f0: 6161 5f70 726f 6273 2c31 2c31 292e 7065  aa_probs,1,1).pe
+0001a400: 726d 7574 6528 312c 322c 3029 2023 5b4e  rmute(1,2,0) #[N
+0001a410: 2c6d 6178 5f6c 656e 2c61 6120 7265 7065  ,max_len,aa repe
+0001a420: 6174 6564 2061 615f 7072 6f62 7320 7469  ated aa_probs ti
+0001a430: 6d65 735d 2d2d 7365 656d 7320 636f 7272  mes]--seems corr
+0001a440: 6563 740a 2020 2020 626c 6f73 756d 5f65  ect.    blosum_e
+0001a450: 7870 616e 6465 6420 3d20 626c 6f73 756d  xpanded = blosum
+0001a460: 5b31 3a2c 2031 3a5d 2e72 6570 6561 7428  [1:, 1:].repeat(
+0001a470: 6461 7461 7365 745f 7472 6169 6e2e 7368  dataset_train.sh
+0001a480: 6170 655b 305d 2c61 6c69 676e 5f73 6571  ape[0],align_seq
+0001a490: 5f6c 656e 2c20 312c 2031 2920 2023 205b  _len, 1, 1)  # [
+0001a4a0: 4e2c 6d61 785f 6c65 6e2c 6161 5f70 726f  N,max_len,aa_pro
+0001a4b0: 6273 2c61 615f 7072 6f62 735d 0a20 2020  bs,aa_probs].   
+0001a4c0: 2061 615f 7472 6169 6e5f 626c 6f73 756d   aa_train_blosum
+0001a4d0: 203d 2062 6c6f 7375 6d5f 6578 7061 6e64   = blosum_expand
+0001a4e0: 6564 2e67 6174 6865 7228 332c 2061 6d69  ed.gather(3, ami
+0001a4f0: 6e6f 6163 6964 735f 7365 7173 2e74 6f28  noacids_seqs.to(
+0001a500: 746f 7263 682e 696e 7436 3429 2e75 6e73  torch.int64).uns
+0001a510: 7175 6565 7a65 2833 2929 2e73 7175 6565  queeze(3)).squee
+0001a520: 7a65 282d 3129 2020 235b 4e2c 6d61 785f  ze(-1)  #[N,max_
+0001a530: 6c65 6e2c 6161 5f70 726f 6273 5d0a 0a0a  len,aa_probs]...
+0001a540: 2020 2020 7265 7475 726e 2061 615f 7472      return aa_tr
+0001a550: 6169 6e5f 626c 6f73 756d 0a0a 6465 6620  ain_blosum..def 
+0001a560: 7374 7232 626f 6f6c 2876 293a 0a20 2020  str2bool(v):.   
+0001a570: 2022 2222 436f 6e76 6572 7473 2061 2073   """Converts a s
+0001a580: 7472 696e 6720 696e 746f 2061 2062 6f6f  tring into a boo
+0001a590: 6c65 616e 2c20 7573 6566 756c 2066 6f72  lean, useful for
+0001a5a0: 2062 6f6f 6c65 616e 2061 7267 756d 656e   boolean argumen
+0001a5b0: 7473 0a20 2020 203a 7061 7261 6d20 7374  ts.    :param st
+0001a5c0: 7220 7622 2222 0a20 2020 2069 6620 6973  r v""".    if is
+0001a5d0: 696e 7374 616e 6365 2876 2c20 626f 6f6c  instance(v, bool
+0001a5e0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0001a5f0: 6e20 760a 2020 2020 6966 2076 2e6c 6f77  n v.    if v.low
+0001a600: 6572 2829 2069 6e20 2827 7965 7327 2c20  er() in ('yes', 
+0001a610: 2774 7275 6527 2c20 2774 272c 2027 7927  'true', 't', 'y'
+0001a620: 2c20 2731 272c 2754 7275 6527 293a 0a20  , '1','True'):. 
+0001a630: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+0001a640: 7565 0a20 2020 2065 6c69 6620 762e 6c6f  ue.    elif v.lo
+0001a650: 7765 7228 2920 696e 2028 276e 6f27 2c20  wer() in ('no', 
+0001a660: 2766 616c 7365 272c 2027 6627 2c20 276e  'false', 'f', 'n
+0001a670: 272c 2027 3027 2c27 4661 6c73 6527 293a  ', '0','False'):
+0001a680: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a690: 4661 6c73 650a 2020 2020 656c 7365 3a0a  False.    else:.
+0001a6a0: 2020 2020 2020 2020 7261 6973 6520 6172          raise ar
+0001a6b0: 6770 6172 7365 2e41 7267 756d 656e 7454  gparse.ArgumentT
+0001a6c0: 7970 6545 7272 6f72 2827 426f 6f6c 6561  ypeError('Boolea
+0001a6d0: 6e20 7661 6c75 6520 6578 7065 6374 6564  n value expected
+0001a6e0: 2e27 290a 6465 6620 7374 7232 4e6f 6e65  .').def str2None
+0001a6f0: 2876 293a 0a20 2020 2022 2222 436f 6e76  (v):.    """Conv
+0001a700: 6572 7473 2061 2073 7472 696e 6720 696e  erts a string in
+0001a710: 746f 204e 6f6e 650a 2020 2020 3a70 6172  to None.    :par
+0001a720: 616d 2073 7472 2076 2222 220a 0a20 2020  am str v"""..   
+0001a730: 2069 6620 762e 6c6f 7765 7228 2920 696e   if v.lower() in
+0001a740: 2028 274e 6f6e 6527 2c27 6e6f 6e65 2729   ('None','none')
+0001a750: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001a760: 204e 6f6e 650a 2020 2020 656c 6966 2069   None.    elif i
+0001a770: 7369 6e73 7461 6e63 6528 762c 7374 7229  sinstance(v,str)
+0001a780: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001a790: 2076 0a20 2020 2065 6c73 653a 0a20 2020   v.    else:.   
+0001a7a0: 2020 2020 2076 203d 2061 7374 2e6c 6974       v = ast.lit
+0001a7b0: 6572 616c 5f65 7661 6c28 7629 0a20 2020  eral_eval(v).   
+0001a7c0: 2020 2020 2072 6574 7572 6e20 760a 0a0a       return v...
+0001a7d0: 0a0a 0a0a                                ....
```

### Comparing `draupnir-0.0.27/src/draupnir.egg-info/PKG-INFO` & `draupnir-0.0.28/src/draupnir.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: draupnir
-Version: 0.0.27
+Version: 0.0.28
 Summary: Ancestral sequence reconstruction using a tree structured Ornstein Uhlenbeck variational autoencoder
 Home-page: https://github.com/LysSanzMoreta/DRAUPNIR_ASR
 Author: Lys Sanz Moreta
 Author-email: lys.sanz.moreta@outlook.com
-License: UNKNOWN
 Project-URL: Changelog, https://github.com/LysSanzMoreta/DRAUPNIR_ASR/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/LysSanzMoreta/DRAUPNIR_ASR/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 DRAUPNIR: "Beta library version for performing ASR using a tree-structured Variational Autoencoder"
@@ -62,17 +60,17 @@
 
 **Example**
 ```
 See Draupnir_example.py
 ```
 **Which guide to use?**
 
-By experience, use delta_map, the marginal results (Test folder) are the most stable.
+By experience, use delta_map, since the marginal results (Test folder) are the most stable.
 It is recommended to run the model both with the variational and the delta_map guides and compare outputs using the mutual information.
-If necessary run the variational guide longer than the delta_map, since it has more parameters to infere and takes longer.
+If necessary, run the variational guide longer than the delta_map, since it has more parameters to optimize and takes longer.
 
 **How long should I run my model?**
 
 0) Before training: 
    - It is recommended to train for at least 10000 epochs in datasets <800 leaves. See article for inspiration, the runtimes where extended to achieve maximum benchmarking accuracy, but it should not be necessary.
 1) While it is training:
    - Check for the Percent_ID.png plot, if the training accuracy has peaked to almost 100%, run for at least ~1000 epochs more to guarantee full learning
@@ -129,37 +127,41 @@
 | Simulation Sirtuin                                | 150              | 477              | simulations_sirtuins_1            |
 | Simulation SRC-kinase SH3 domain                  | 200              | 128              | simulations_src_sh3_3             |
 | Simulation PIGBOS                                 | 300              | 77               | simulations_PIGBOS_1              |
 | Simulation Insulin                                | 400              | 558              | simulations_insulin_2             |
 | Simulation SRC-kinase SH3 domain                  | 800              | 99               | simulations_src_sh3_2             |
 
 
-**What do the folders mean?**
+**What do the results folders mean?**
 
 1) If you selected **delta_map** guide:
-   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are samples obtained by using the MAP estimates of the logits.
-   2) Train_argmax_Plots: Single sequence per leaf obtained by the using the most likely amino acids indicated by the logits ("argmax the logits")
-   3) Test_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the marginal probability approach (equation 5 in the paper)
+   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are **samples** obtained by using the marginal probability approach (equation 5 in the paper).
+   2) Train_argmax_Plots: Single sequence per leaf obtained by the using the most likely amino acids indicated by the marginal logits ("argmax the logits") 
+   3) Test_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the **marginal probability** approach (equation 5 in the paper)
    4) Test_argmax_Plots: Contains the most voted sequence from the samples in Test_Plots.
-   5) Test2_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the MAP estimated of the logits. 
-   6) Test2_argmax_Plots:  Samples for the test sequences (ancestors). In this case they contain the most likely amino acids indicated by the logits ("argmax the logits") (equation 4 in the paper)
+   5) Test2_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the **MAP estimates** of the logits. 
+   6) Test2_argmax_Plots:  Samples for the test sequences (ancestors). In this case they contain the most likely amino acids indicated by the MAP logits ("argmax the logits") (equation 4 in the paper)
 2) If you selected **variational** guide:
-   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are samples obtained by using the MAP estimates of the logits.
+   1) Train_Plots: Contains information related to the inference of the train sequences (the leaves). They are **samples** obtained from sampling from the variational posterior (equation 6 in the paper).
    2) Train_argmax_Plots: Single sequence per leaf obtained by the using the most likely amino acids indicated by the logits ("argmax the logits")
    3) Test_Plots: Samples for the test sequences (ancestors). In this case they contain the sequences sampled using the full variational probability approach (equation 6 in the paper)
    4) Test_argmax_Plots: Contains the most voted sequence from the samples in Test_Plots.
    5) Test2_Plots == Test_Plots 
    6) Test2_argmax_Plots == Test_argmax_Plots
 
 **Where are my ancestral sequences?**
 
 - In each of the folders there should be a fasta file <dataset-name>_sampled_nodes_seq.fasta
 
 - Each of the sequences in the file should be identified as <node-name-input-tree>//<tree-level-order>\_sample\_<sample-number>
 
+    -Node-name-input-tree: Original name of the node in the given input tree
+
+    -Tree-level-order: Position of the node in tree-level order in the tree
+    
     >Node_A1//1.0_sample_0
 
     
 **If this library is useful for your research please cite:**
 
 ```
 @inproceedings{moreta2021ancestral,
@@ -167,14 +169,15 @@
   author={Moreta, Lys Sanz and R{\o}nning, Ola and Al-Sibahi, Ahmad Salim and Hein, Jotun and Theobald, Douglas and Hamelryck, Thomas},
   booktitle={International Conference on Learning Representations},
   year={2021}
 }
 ```
 
 
+**Do not hesitate to give input on how to improve the documentation of this library**
```

### Comparing `draupnir-0.0.27/src/draupnir.egg-info/SOURCES.txt` & `draupnir-0.0.28/src/draupnir.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,12 @@
 src/draupnir.egg-info/top_level.txt
 src/draupnir/data/AA_properties.txt
 src/draupnir/data/PfamPdbMap.txt
 src/draupnir/infer_angles/__init__.py
 src/draupnir/infer_angles/calculate_coords.py
 src/draupnir/infer_angles/nerf.py
 src/draupnir/infer_angles/pnerf.py
-src/draupnir/infer_angles/superposition.py
+src/draupnir/infer_angles/superposition.py
+tests/test_accuracy.py
+tests/test_examples.py
+tests/test_load.py
+tests/test_norworking.py
```

