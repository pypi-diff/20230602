# Comparing `tmp/tumourkit-0.7.1.tar.gz` & `tmp/tumourkit-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumourkit-0.7.1.tar", last modified: Tue May 30 20:01:02 2023, max compression
+gzip compressed data, was "tumourkit-0.7.2.tar", last modified: Fri Jun  2 09:26:12 2023, max compression
```

## Comparing `tumourkit-0.7.1.tar` & `tumourkit-0.7.2.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.341325 tumourkit-0.7.1/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.7.1/LICENSE
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-30 20:01:02.340822 tumourkit-0.7.1/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1269 2023-03-25 17:22:23.000000 tumourkit-0.7.1/README.md
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.210515 tumourkit-0.7.1/docs/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.210246 tumourkit-0.7.1/docs/buildenv/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.228543 tumourkit-0.7.1/docs/buildenv/bin/
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2html.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2html4.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2html5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2latex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2man.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2odt.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2s5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2xetex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2xml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rstpep2html.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.229235 tumourkit-0.7.1/docs/source/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.7.1/docs/source/conf.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2282 2023-05-25 06:24:46.000000 tumourkit-0.7.1/pyproject.toml
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.7.1/requirements.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-30 20:01:02.341447 tumourkit-0.7.1/setup.cfg
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.248959 tumourkit-0.7.1/tests/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.7.1/tests/centroidspng2csv_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.7.1/tests/conf_matrix_sum_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.7.1/tests/cpairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.7.1/tests/example_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.7.1/tests/generate_centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.7.1/tests/generate_rswoosh.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.7.1/tests/get_conn_comp_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.7.1/tests/graph2centroids_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.7.1/tests/graph_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2183 2023-05-30 17:37:56.000000 tumourkit-0.7.1/tests/hov_prob_pipe_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.7.1/tests/hov_prob_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.7.1/tests/hovernet_patches_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.7.1/tests/metrics_pairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.7.1/tests/metrics_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.7.1/tests/png2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.7.1/tests/pngcsv2geojson_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.7.1/tests/pngcsv2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.7.1/tests/read_nodes_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.7.1/tests/remove_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.7.1/tests/rswoosh_test.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.256270 tumourkit-0.7.1/tumourkit/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-05-30 19:59:52.000000 tumourkit-0.7.1/tumourkit/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.266972 tumourkit-0.7.1/tumourkit/classification/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.7.1/tumourkit/classification/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1356 2023-05-18 07:19:54.000000 tumourkit-0.7.1/tumourkit/classification/compute_imbalance.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     8132 2023-05-30 18:36:23.000000 tumourkit-0.7.1/tumourkit/classification/evaluate.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6654 2023-05-30 18:28:05.000000 tumourkit-0.7.1/tumourkit/classification/infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.271271 tumourkit-0.7.1/tumourkit/classification/models/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.7.1/tumourkit/classification/models/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.7.1/tumourkit/classification/models/gat.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.7.1/tumourkit/classification/models/gcn.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.7.1/tumourkit/classification/models/hgao.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.7.1/tumourkit/classification/models/norm.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7575 2023-05-18 07:24:15.000000 tumourkit-0.7.1/tumourkit/classification/read_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    20658 2023-05-18 07:28:33.000000 tumourkit-0.7.1/tumourkit/classification/train_graphs.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    10426 2023-05-18 07:32:33.000000 tumourkit-0.7.1/tumourkit/classification/train_xgboost.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.272706 tumourkit-0.7.1/tumourkit/demo/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    17409 2023-05-30 18:03:04.000000 tumourkit-0.7.1/tumourkit/demo/app.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7305 2023-05-30 18:04:56.000000 tumourkit-0.7.1/tumourkit/eval_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     9512 2023-05-30 18:06:38.000000 tumourkit-0.7.1/tumourkit/infer_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4131 2023-05-30 18:12:51.000000 tumourkit-0.7.1/tumourkit/make_dirs.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.281880 tumourkit-0.7.1/tumourkit/postprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      195 2023-05-30 17:38:57.000000 tumourkit-0.7.1/tumourkit/postprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3411 2023-05-30 18:20:10.000000 tumourkit-0.7.1/tumourkit/postprocessing/draw_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6896 2023-05-30 17:55:03.000000 tumourkit-0.7.1/tumourkit/postprocessing/draw_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4198 2023-05-30 18:20:42.000000 tumourkit-0.7.1/tumourkit/postprocessing/join_graph_gt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6977 2023-05-30 18:21:29.000000 tumourkit-0.7.1/tumourkit/postprocessing/join_hovprob_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6510 2023-05-30 18:23:48.000000 tumourkit-0.7.1/tumourkit/postprocessing/merge_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2094 2023-05-30 18:24:14.000000 tumourkit-0.7.1/tumourkit/postprocessing/rswoosh.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.301299 tumourkit-0.7.1/tumourkit/preprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      666 2023-05-30 17:35:42.000000 tumourkit-0.7.1/tumourkit/preprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2307 2023-05-18 06:57:47.000000 tumourkit-0.7.1/tumourkit/preprocessing/centroids2png.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4660 2023-05-18 06:58:20.000000 tumourkit-0.7.1/tumourkit/preprocessing/centroidspng2csv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3892 2023-05-18 07:00:03.000000 tumourkit-0.7.1/tumourkit/preprocessing/geojson2pngcsv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3289 2023-05-18 07:00:16.000000 tumourkit-0.7.1/tumourkit/preprocessing/graph2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2825 2023-05-18 07:00:48.000000 tumourkit-0.7.1/tumourkit/preprocessing/hovernet2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3720 2023-05-18 07:01:18.000000 tumourkit-0.7.1/tumourkit/preprocessing/hovernet2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-05-18 07:02:17.000000 tumourkit-0.7.1/tumourkit/preprocessing/png2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2777 2023-05-18 07:02:32.000000 tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5041 2023-05-18 07:02:55.000000 tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4452 2023-05-30 18:18:32.000000 tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2434 2023-05-30 18:19:10.000000 tumourkit-0.7.1/tumourkit/preprocessing/remove_uncertain.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.302852 tumourkit-0.7.1/tumourkit/profiling/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2747 2023-05-18 07:35:28.000000 tumourkit-0.7.1/tumourkit/profiling/cpairs_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1915 2023-05-18 07:36:50.000000 tumourkit-0.7.1/tumourkit/profiling/rswoosh_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    18656 2023-05-30 18:35:31.000000 tumourkit-0.7.1/tumourkit/research_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.306229 tumourkit-0.7.1/tumourkit/segmentation/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.7.1/tumourkit/segmentation/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    14370 2023-05-30 18:17:43.000000 tumourkit-0.7.1/tumourkit/segmentation/evaluate.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.311297 tumourkit-0.7.1/tumourkit/segmentation/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/config.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.314455 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/augs.py
--rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/train_loader.py
--rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/extract_patches.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.316652 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/base.py
--rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/tile.py
--rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/wsi.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.317992 tumourkit-0.7.1/tumourkit/segmentation/hovernet/metrics/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/metrics/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/metrics/stats_utils.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.321515 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/patch_extractor.py
--rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/viz_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/wsi_handler.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.322050 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.328526 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/opt.py
--rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
--rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/targets.py
--rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.330104 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.332281 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
--rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
--rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
--rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/engine.py
--rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/train.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    12250 2023-05-30 18:35:15.000000 tumourkit-0.7.1/tumourkit/train_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.339837 tumourkit-0.7.1/tumourkit/utils/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.7.1/tumourkit/utils/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5934 2023-05-18 06:31:59.000000 tumourkit-0.7.1/tumourkit/utils/calibration_error.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5658 2023-05-18 06:37:18.000000 tumourkit-0.7.1/tumourkit/utils/classification.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3611 2023-05-18 06:39:27.000000 tumourkit-0.7.1/tumourkit/utils/folder2txt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5321 2023-05-18 06:43:10.000000 tumourkit-0.7.1/tumourkit/utils/nearest.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4402 2023-05-30 18:14:32.000000 tumourkit-0.7.1/tumourkit/utils/pipes.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7053 2023-05-18 06:46:21.000000 tumourkit-0.7.1/tumourkit/utils/postprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    21855 2023-05-18 06:54:22.000000 tumourkit-0.7.1/tumourkit/utils/preprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5798 2023-05-18 06:56:50.000000 tumourkit-0.7.1/tumourkit/utils/read_nodes.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.260659 tumourkit-0.7.1/tumourkit.egg-info/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4948 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/SOURCES.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/dependency_links.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1054 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/entry_points.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/requires.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/top_level.txt
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.492331 tumourkit-0.7.2/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.7.2/LICENSE
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-02 09:26:12.491775 tumourkit-0.7.2/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1580 2023-05-30 20:14:30.000000 tumourkit-0.7.2/README.md
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.387445 tumourkit-0.7.2/docs/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.387197 tumourkit-0.7.2/docs/buildenv/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.402289 tumourkit-0.7.2/docs/buildenv/bin/
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2html.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2html4.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2html5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2latex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2man.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2odt.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2s5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2xetex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rst2xml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.7.2/docs/buildenv/bin/rstpep2html.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.402977 tumourkit-0.7.2/docs/source/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.7.2/docs/source/conf.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2282 2023-05-25 06:24:46.000000 tumourkit-0.7.2/pyproject.toml
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.7.2/requirements.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-06-02 09:26:12.492478 tumourkit-0.7.2/setup.cfg
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.422828 tumourkit-0.7.2/tests/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.7.2/tests/centroidspng2csv_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.7.2/tests/conf_matrix_sum_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.7.2/tests/cpairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.7.2/tests/example_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.7.2/tests/generate_centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.7.2/tests/generate_rswoosh.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.7.2/tests/get_conn_comp_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.7.2/tests/graph2centroids_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.7.2/tests/graph_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2183 2023-05-30 17:37:56.000000 tumourkit-0.7.2/tests/hov_prob_pipe_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.7.2/tests/hov_prob_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.7.2/tests/hovernet_patches_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.7.2/tests/metrics_pairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.7.2/tests/metrics_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.7.2/tests/png2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.7.2/tests/pngcsv2geojson_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.7.2/tests/pngcsv2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.7.2/tests/read_nodes_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.7.2/tests/remove_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.7.2/tests/rswoosh_test.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.429090 tumourkit-0.7.2/tumourkit/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-06-02 09:25:23.000000 tumourkit-0.7.2/tumourkit/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.438178 tumourkit-0.7.2/tumourkit/classification/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.7.2/tumourkit/classification/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1356 2023-05-18 07:19:54.000000 tumourkit-0.7.2/tumourkit/classification/compute_imbalance.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     8132 2023-05-30 18:36:23.000000 tumourkit-0.7.2/tumourkit/classification/evaluate.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6654 2023-05-30 18:28:05.000000 tumourkit-0.7.2/tumourkit/classification/infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.441079 tumourkit-0.7.2/tumourkit/classification/models/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.7.2/tumourkit/classification/models/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.7.2/tumourkit/classification/models/gat.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.7.2/tumourkit/classification/models/gcn.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.7.2/tumourkit/classification/models/hgao.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.7.2/tumourkit/classification/models/norm.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7575 2023-05-18 07:24:15.000000 tumourkit-0.7.2/tumourkit/classification/read_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    20658 2023-05-18 07:28:33.000000 tumourkit-0.7.2/tumourkit/classification/train_graphs.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    10426 2023-05-18 07:32:33.000000 tumourkit-0.7.2/tumourkit/classification/train_xgboost.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.441749 tumourkit-0.7.2/tumourkit/demo/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    17409 2023-05-30 18:03:04.000000 tumourkit-0.7.2/tumourkit/demo/app.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    11480 2023-06-02 09:23:43.000000 tumourkit-0.7.2/tumourkit/eval_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     9512 2023-05-31 20:15:09.000000 tumourkit-0.7.2/tumourkit/infer_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4131 2023-05-30 18:12:51.000000 tumourkit-0.7.2/tumourkit/make_dirs.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.448458 tumourkit-0.7.2/tumourkit/postprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      195 2023-05-30 17:38:57.000000 tumourkit-0.7.2/tumourkit/postprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3411 2023-05-30 18:20:10.000000 tumourkit-0.7.2/tumourkit/postprocessing/draw_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6896 2023-05-30 17:55:03.000000 tumourkit-0.7.2/tumourkit/postprocessing/draw_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4198 2023-05-30 18:20:42.000000 tumourkit-0.7.2/tumourkit/postprocessing/join_graph_gt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6977 2023-05-30 18:21:29.000000 tumourkit-0.7.2/tumourkit/postprocessing/join_hovprob_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6510 2023-05-30 18:23:48.000000 tumourkit-0.7.2/tumourkit/postprocessing/merge_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2094 2023-05-30 18:24:14.000000 tumourkit-0.7.2/tumourkit/postprocessing/rswoosh.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.458030 tumourkit-0.7.2/tumourkit/preprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      666 2023-05-30 17:35:42.000000 tumourkit-0.7.2/tumourkit/preprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2307 2023-05-18 06:57:47.000000 tumourkit-0.7.2/tumourkit/preprocessing/centroids2png.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4660 2023-05-18 06:58:20.000000 tumourkit-0.7.2/tumourkit/preprocessing/centroidspng2csv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3892 2023-05-18 07:00:03.000000 tumourkit-0.7.2/tumourkit/preprocessing/geojson2pngcsv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3289 2023-05-18 07:00:16.000000 tumourkit-0.7.2/tumourkit/preprocessing/graph2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2825 2023-05-18 07:00:48.000000 tumourkit-0.7.2/tumourkit/preprocessing/hovernet2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3720 2023-05-18 07:01:18.000000 tumourkit-0.7.2/tumourkit/preprocessing/hovernet2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-05-18 07:02:17.000000 tumourkit-0.7.2/tumourkit/preprocessing/png2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2777 2023-05-18 07:02:32.000000 tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5041 2023-05-18 07:02:55.000000 tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4452 2023-05-30 18:18:32.000000 tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2434 2023-05-30 18:19:10.000000 tumourkit-0.7.2/tumourkit/preprocessing/remove_uncertain.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.459493 tumourkit-0.7.2/tumourkit/profiling/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2747 2023-05-18 07:35:28.000000 tumourkit-0.7.2/tumourkit/profiling/cpairs_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1915 2023-05-18 07:36:50.000000 tumourkit-0.7.2/tumourkit/profiling/rswoosh_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    18656 2023-05-30 18:35:31.000000 tumourkit-0.7.2/tumourkit/research_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.461249 tumourkit-0.7.2/tumourkit/segmentation/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.7.2/tumourkit/segmentation/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    14370 2023-05-30 18:17:43.000000 tumourkit-0.7.2/tumourkit/segmentation/evaluate.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.464259 tumourkit-0.7.2/tumourkit/segmentation/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/config.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.466417 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/augs.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/train_loader.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/extract_patches.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.469031 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/tile.py
+-rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/wsi.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.470274 tumourkit-0.7.2/tumourkit/segmentation/hovernet/metrics/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/metrics/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/metrics/stats_utils.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.473347 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/patch_extractor.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/viz_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/wsi_handler.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.473935 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.479717 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/opt.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
+-rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/targets.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.481348 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.483987 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/engine.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.7.2/tumourkit/segmentation/hovernet/train.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    12250 2023-05-30 18:35:15.000000 tumourkit-0.7.2/tumourkit/train_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.490841 tumourkit-0.7.2/tumourkit/utils/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.7.2/tumourkit/utils/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5934 2023-05-18 06:31:59.000000 tumourkit-0.7.2/tumourkit/utils/calibration_error.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5658 2023-05-18 06:37:18.000000 tumourkit-0.7.2/tumourkit/utils/classification.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3611 2023-05-18 06:39:27.000000 tumourkit-0.7.2/tumourkit/utils/folder2txt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5321 2023-05-18 06:43:10.000000 tumourkit-0.7.2/tumourkit/utils/nearest.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4402 2023-05-30 18:14:32.000000 tumourkit-0.7.2/tumourkit/utils/pipes.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7053 2023-05-18 06:46:21.000000 tumourkit-0.7.2/tumourkit/utils/postprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    21855 2023-05-18 06:54:22.000000 tumourkit-0.7.2/tumourkit/utils/preprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5798 2023-05-18 06:56:50.000000 tumourkit-0.7.2/tumourkit/utils/read_nodes.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-02 09:26:12.432666 tumourkit-0.7.2/tumourkit.egg-info/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4948 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/SOURCES.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/dependency_links.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1054 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/entry_points.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/requires.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-06-02 09:26:12.000000 tumourkit-0.7.2/tumourkit.egg-info/top_level.txt
```

### Comparing `tumourkit-0.7.1/LICENSE` & `tumourkit-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/PKG-INFO` & `tumourkit-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.7.1
+Version: 0.7.2
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,11 +683,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TumourKit
 [![Ubuntu tests](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-ubuntu.yml/badge.svg)](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-ubuntu.yml) [![Windows tests](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-windows.yml/badge.svg)](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-windows.yml) [![Documentation Status](https://readthedocs.org/projects/lung-tumour-study/badge/?version=latest)](https://lung-tumour-study.readthedocs.io/en/latest/?badge=latest) [![pyversion](https://raw.githubusercontent.com/Jerry-Master/badges/main/py_versions.svg)](https://www.python.org/) [![torchversion](https://raw.githubusercontent.com/Jerry-Master/badges/main/torch_version.svg)](https://pytorch.org/) [![dglversion](https://raw.githubusercontent.com/Jerry-Master/badges/main/dgl-1.0.1.svg)](https://www.dgl.ai/)
 
-Python package from my Bachelor's thesis. It is dedicated to aid in the study of tumours. It all started with lung tissue, thus the repository name. But it now supports any tissue with any number of classes. For more information, please visit the [official documentation](https://lung-tumour-study.readthedocs.io/en/latest/index.html)
+<p align="middle">
+  <img src="docs/source/imgs/example.png" width="30%" />
+  <img src="docs/source/imgs/overlay.png" width="30%" /> 
+  <img src="docs/source/imgs/graph-overlay.png" width="30%" />
+</p>
 
+Python package from my Bachelor's thesis. It is dedicated to aid in the study of tumours. It all started with lung tissue, thus the repository name. But it now supports any tissue with any number of classes. For more information, please visit the [official documentation](https://lung-tumour-study.readthedocs.io/en/latest/index.html). Pretrained models can be found on [Hugging Face](https://huggingface.co/Jerry-Master/Hovernet-plus-Graphs).
```

### Comparing `tumourkit-0.7.1/README.md` & `tumourkit-0.7.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,12 @@
 # TumourKit
 [![Ubuntu tests](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-ubuntu.yml/badge.svg)](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-ubuntu.yml) [![Windows tests](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-windows.yml/badge.svg)](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-windows.yml) [![Documentation Status](https://readthedocs.org/projects/lung-tumour-study/badge/?version=latest)](https://lung-tumour-study.readthedocs.io/en/latest/?badge=latest) [![pyversion](https://raw.githubusercontent.com/Jerry-Master/badges/main/py_versions.svg)](https://www.python.org/) [![torchversion](https://raw.githubusercontent.com/Jerry-Master/badges/main/torch_version.svg)](https://pytorch.org/) [![dglversion](https://raw.githubusercontent.com/Jerry-Master/badges/main/dgl-1.0.1.svg)](https://www.dgl.ai/)
 
-Python package from my Bachelor's thesis. It is dedicated to aid in the study of tumours. It all started with lung tissue, thus the repository name. But it now supports any tissue with any number of classes. For more information, please visit the [official documentation](https://lung-tumour-study.readthedocs.io/en/latest/index.html)
+<p align="middle">
+  <img src="docs/source/imgs/example.png" width="30%" />
+  <img src="docs/source/imgs/overlay.png" width="30%" /> 
+  <img src="docs/source/imgs/graph-overlay.png" width="30%" />
+</p>
 
+Python package from my Bachelor's thesis. It is dedicated to aid in the study of tumours. It all started with lung tissue, thus the repository name. But it now supports any tissue with any number of classes. For more information, please visit the [official documentation](https://lung-tumour-study.readthedocs.io/en/latest/index.html). Pretrained models can be found on [Hugging Face](https://huggingface.co/Jerry-Master/Hovernet-plus-Graphs).
```

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2html.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2html4.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2html5.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2latex.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2man.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2odt.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2odt_prepstyles.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2pseudoxml.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2s5.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2xetex.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rst2xml.py` & `tumourkit-0.7.2/docs/buildenv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/buildenv/bin/rstpep2html.py` & `tumourkit-0.7.2/docs/buildenv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/docs/source/conf.py` & `tumourkit-0.7.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/pyproject.toml` & `tumourkit-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/requirements.txt` & `tumourkit-0.7.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/centroidspng2csv_test.py` & `tumourkit-0.7.2/tests/centroidspng2csv_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/conf_matrix_sum_test.py` & `tumourkit-0.7.2/tests/conf_matrix_sum_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/cpairs_test.py` & `tumourkit-0.7.2/tests/cpairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/example_test.py` & `tumourkit-0.7.2/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/generate_centroids.py` & `tumourkit-0.7.2/tests/generate_centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/generate_rswoosh.py` & `tumourkit-0.7.2/tests/generate_rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/get_conn_comp_test.py` & `tumourkit-0.7.2/tests/get_conn_comp_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/graph2centroids_test.py` & `tumourkit-0.7.2/tests/graph2centroids_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/graph_idx_test.py` & `tumourkit-0.7.2/tests/graph_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/hov_prob_pipe_test.py` & `tumourkit-0.7.2/tests/hov_prob_pipe_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/hov_prob_test.py` & `tumourkit-0.7.2/tests/hov_prob_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/hovernet_patches_test.py` & `tumourkit-0.7.2/tests/hovernet_patches_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/metrics_pairs_test.py` & `tumourkit-0.7.2/tests/metrics_pairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/metrics_test.py` & `tumourkit-0.7.2/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/png2graph_test.py` & `tumourkit-0.7.2/tests/png2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/pngcsv2geojson_test.py` & `tumourkit-0.7.2/tests/pngcsv2geojson_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/pngcsv2graph_test.py` & `tumourkit-0.7.2/tests/pngcsv2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/read_nodes_test.py` & `tumourkit-0.7.2/tests/read_nodes_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/remove_idx_test.py` & `tumourkit-0.7.2/tests/remove_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tests/rswoosh_test.py` & `tumourkit-0.7.2/tests/rswoosh_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/compute_imbalance.py` & `tumourkit-0.7.2/tumourkit/classification/compute_imbalance.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/evaluate.py` & `tumourkit-0.7.2/tumourkit/classification/evaluate.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/infer.py` & `tumourkit-0.7.2/tumourkit/classification/infer.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/models/gat.py` & `tumourkit-0.7.2/tumourkit/classification/models/gat.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/models/gcn.py` & `tumourkit-0.7.2/tumourkit/classification/models/gcn.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/models/hgao.py` & `tumourkit-0.7.2/tumourkit/classification/models/hgao.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/models/norm.py` & `tumourkit-0.7.2/tumourkit/classification/models/norm.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/read_graph.py` & `tumourkit-0.7.2/tumourkit/classification/read_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/train_graphs.py` & `tumourkit-0.7.2/tumourkit/classification/train_graphs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/classification/train_xgboost.py` & `tumourkit-0.7.2/tumourkit/classification/train_xgboost.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/demo/app.py` & `tumourkit-0.7.2/tumourkit/demo/app.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/infer_pipe.py` & `tumourkit-0.7.2/tumourkit/infer_pipe.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/make_dirs.py` & `tumourkit-0.7.2/tumourkit/make_dirs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/postprocessing/draw_cells.py` & `tumourkit-0.7.2/tumourkit/postprocessing/draw_cells.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/postprocessing/draw_graph.py` & `tumourkit-0.7.2/tumourkit/postprocessing/draw_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/postprocessing/join_graph_gt.py` & `tumourkit-0.7.2/tumourkit/postprocessing/join_graph_gt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/postprocessing/join_hovprob_graph.py` & `tumourkit-0.7.2/tumourkit/postprocessing/join_hovprob_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/postprocessing/merge_cells.py` & `tumourkit-0.7.2/tumourkit/postprocessing/merge_cells.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/postprocessing/rswoosh.py` & `tumourkit-0.7.2/tumourkit/postprocessing/rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/__init__.py` & `tumourkit-0.7.2/tumourkit/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/centroids2png.py` & `tumourkit-0.7.2/tumourkit/preprocessing/centroids2png.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/centroidspng2csv.py` & `tumourkit-0.7.2/tumourkit/preprocessing/centroidspng2csv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/geojson2pngcsv.py` & `tumourkit-0.7.2/tumourkit/preprocessing/geojson2pngcsv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/graph2centroids.py` & `tumourkit-0.7.2/tumourkit/preprocessing/graph2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/hovernet2centroids.py` & `tumourkit-0.7.2/tumourkit/preprocessing/hovernet2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/hovernet2geojson.py` & `tumourkit-0.7.2/tumourkit/preprocessing/hovernet2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/png2graph.py` & `tumourkit-0.7.2/tumourkit/preprocessing/png2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2centroids.py` & `tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2geojson.py` & `tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2graph.py` & `tumourkit-0.7.2/tumourkit/preprocessing/pngcsv2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/preprocessing/remove_uncertain.py` & `tumourkit-0.7.2/tumourkit/preprocessing/remove_uncertain.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/profiling/cpairs_profile.py` & `tumourkit-0.7.2/tumourkit/profiling/cpairs_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/profiling/rswoosh_profile.py` & `tumourkit-0.7.2/tumourkit/profiling/rswoosh_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/research_pipe.py` & `tumourkit-0.7.2/tumourkit/research_pipe.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/evaluate.py` & `tumourkit-0.7.2/tumourkit/segmentation/evaluate.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/config.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/config.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/augs.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/augs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/infer_loader.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/infer_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/train_loader.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/dataloader/train_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/extract_patches.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/extract_patches.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/base.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/tile.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/tile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/wsi.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/infer/wsi.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/metrics/stats_utils.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/metrics/stats_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/patch_extractor.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/patch_extractor.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/utils.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/viz_utils.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/viz_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/wsi_handler.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/misc/wsi_handler.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/opt.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/opt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/targets.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/targets.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/utils.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/models/hovernet/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_infer.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_infer.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/engine.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/utils.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/run_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/segmentation/hovernet/train.py` & `tumourkit-0.7.2/tumourkit/segmentation/hovernet/train.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/train_pipe.py` & `tumourkit-0.7.2/tumourkit/train_pipe.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/utils/calibration_error.py` & `tumourkit-0.7.2/tumourkit/utils/calibration_error.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/utils/classification.py` & `tumourkit-0.7.2/tumourkit/utils/classification.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/utils/folder2txt.py` & `tumourkit-0.7.2/tumourkit/utils/folder2txt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/utils/nearest.py` & `tumourkit-0.7.2/tumourkit/utils/nearest.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/utils/pipes.py` & `tumourkit-0.7.2/tumourkit/utils/pipes.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/utils/postprocessing.py` & `tumourkit-0.7.2/tumourkit/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/utils/preprocessing.py` & `tumourkit-0.7.2/tumourkit/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit/utils/read_nodes.py` & `tumourkit-0.7.2/tumourkit/utils/read_nodes.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit.egg-info/PKG-INFO` & `tumourkit-0.7.2/tumourkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.7.1
+Version: 0.7.2
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,11 +683,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TumourKit
 [![Ubuntu tests](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-ubuntu.yml/badge.svg)](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-ubuntu.yml) [![Windows tests](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-windows.yml/badge.svg)](https://github.com/Jerry-Master/lung-tumour-study/actions/workflows/pytest-windows.yml) [![Documentation Status](https://readthedocs.org/projects/lung-tumour-study/badge/?version=latest)](https://lung-tumour-study.readthedocs.io/en/latest/?badge=latest) [![pyversion](https://raw.githubusercontent.com/Jerry-Master/badges/main/py_versions.svg)](https://www.python.org/) [![torchversion](https://raw.githubusercontent.com/Jerry-Master/badges/main/torch_version.svg)](https://pytorch.org/) [![dglversion](https://raw.githubusercontent.com/Jerry-Master/badges/main/dgl-1.0.1.svg)](https://www.dgl.ai/)
 
-Python package from my Bachelor's thesis. It is dedicated to aid in the study of tumours. It all started with lung tissue, thus the repository name. But it now supports any tissue with any number of classes. For more information, please visit the [official documentation](https://lung-tumour-study.readthedocs.io/en/latest/index.html)
+<p align="middle">
+  <img src="docs/source/imgs/example.png" width="30%" />
+  <img src="docs/source/imgs/overlay.png" width="30%" /> 
+  <img src="docs/source/imgs/graph-overlay.png" width="30%" />
+</p>
 
+Python package from my Bachelor's thesis. It is dedicated to aid in the study of tumours. It all started with lung tissue, thus the repository name. But it now supports any tissue with any number of classes. For more information, please visit the [official documentation](https://lung-tumour-study.readthedocs.io/en/latest/index.html). Pretrained models can be found on [Hugging Face](https://huggingface.co/Jerry-Master/Hovernet-plus-Graphs).
```

### Comparing `tumourkit-0.7.1/tumourkit.egg-info/SOURCES.txt` & `tumourkit-0.7.2/tumourkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit.egg-info/entry_points.txt` & `tumourkit-0.7.2/tumourkit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.1/tumourkit.egg-info/requires.txt` & `tumourkit-0.7.2/tumourkit.egg-info/requires.txt`

 * *Files identical despite different names*

