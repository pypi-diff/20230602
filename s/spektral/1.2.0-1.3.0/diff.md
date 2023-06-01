# Comparing `tmp/spektral-1.2.0.tar.gz` & `tmp/spektral-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spektral-1.2.0.tar", last modified: Fri Jul 22 15:02:18 2022, max compression
+gzip compressed data, was "spektral-1.3.0.tar", last modified: Thu Jun  1 22:13:53 2023, max compression
```

## Comparing `spektral-1.2.0.tar` & `spektral-1.3.0.tar`

### file list

```diff
@@ -1,112 +1,109 @@
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.671711 spektral-1.2.0/
--rw-r--r--   0 phait      (501) staff       (20)     1075 2022-03-03 13:47:36.000000 spektral-1.2.0/LICENSE
--rw-r--r--   0 phait      (501) staff       (20)     5446 2022-07-22 15:02:18.671595 spektral-1.2.0/PKG-INFO
--rw-r--r--   0 phait      (501) staff       (20)     4981 2022-03-03 13:47:36.000000 spektral-1.2.0/README.md
--rw-r--r--   0 phait      (501) staff       (20)       80 2022-07-22 15:00:38.000000 spektral-1.2.0/pyproject.toml
--rw-r--r--   0 phait      (501) staff       (20)       38 2022-07-22 15:02:18.671749 spektral-1.2.0/setup.cfg
--rw-r--r--   0 phait      (501) staff       (20)      910 2022-07-22 15:01:59.000000 spektral-1.2.0/setup.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.655779 spektral-1.2.0/spektral/
--rw-r--r--   0 phait      (501) staff       (20)       61 2022-07-22 15:01:59.000000 spektral-1.2.0/spektral/__init__.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.657342 spektral-1.2.0/spektral/data/
--rw-r--r--   0 phait      (501) staff       (20)      186 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/data/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)    10278 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/data/dataset.py
--rw-r--r--   0 phait      (501) staff       (20)     5610 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/data/graph.py
--rw-r--r--   0 phait      (501) staff       (20)    21819 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/data/loaders.py
--rw-r--r--   0 phait      (501) staff       (20)    10658 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/data/utils.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.659976 spektral-1.2.0/spektral/datasets/
--rw-r--r--   0 phait      (501) staff       (20)      303 2022-07-22 07:45:09.000000 spektral-1.2.0/spektral/datasets/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)     6593 2022-07-21 13:41:15.000000 spektral-1.2.0/spektral/datasets/citation.py
--rw-r--r--   0 phait      (501) staff       (20)     2869 2022-07-22 07:45:09.000000 spektral-1.2.0/spektral/datasets/dblp.py
--rw-r--r--   0 phait      (501) staff       (20)     2891 2022-07-22 07:45:09.000000 spektral-1.2.0/spektral/datasets/flickr.py
--rw-r--r--   0 phait      (501) staff       (20)     6936 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/datasets/graphsage.py
--rw-r--r--   0 phait      (501) staff       (20)     3021 2022-03-03 14:08:01.000000 spektral-1.2.0/spektral/datasets/mnist.py
--rw-r--r--   0 phait      (501) staff       (20)     3257 2022-03-03 14:08:01.000000 spektral-1.2.0/spektral/datasets/modelnet.py
--rw-r--r--   0 phait      (501) staff       (20)     1116 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/datasets/ogb.py
--rw-r--r--   0 phait      (501) staff       (20)     1562 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/datasets/qm7.py
--rw-r--r--   0 phait      (501) staff       (20)     3361 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/datasets/qm9.py
--rw-r--r--   0 phait      (501) staff       (20)     8090 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/datasets/tudataset.py
--rw-r--r--   0 phait      (501) staff       (20)     1405 2022-03-03 14:08:01.000000 spektral-1.2.0/spektral/datasets/utils.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.660277 spektral-1.2.0/spektral/layers/
--rw-r--r--   0 phait      (501) staff       (20)       90 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)     8949 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/base.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.663857 spektral-1.2.0/spektral/layers/convolutional/
--rw-r--r--   0 phait      (501) staff       (20)      693 2022-07-22 14:31:49.000000 spektral-1.2.0/spektral/layers/convolutional/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)     2666 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/layers/convolutional/agnn_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     5096 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/convolutional/appnp_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     8046 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/convolutional/arma_conv.py
--rw-r--r--   0 phait      (501) staff       (20)    10487 2022-07-21 15:12:38.000000 spektral-1.2.0/spektral/layers/convolutional/censnet_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     4461 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/convolutional/cheb_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     2918 2022-06-07 16:59:30.000000 spektral-1.2.0/spektral/layers/convolutional/conv.py
--rw-r--r--   0 phait      (501) staff       (20)     3723 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/layers/convolutional/crystal_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     5941 2022-07-22 14:11:59.000000 spektral-1.2.0/spektral/layers/convolutional/diffusion_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     6992 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/layers/convolutional/ecc_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     4203 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/layers/convolutional/edge_conv.py
--rw-r--r--   0 phait      (501) staff       (20)    10279 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/layers/convolutional/gat_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     4252 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/convolutional/gated_graph_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     3693 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/convolutional/gcn_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     3850 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/convolutional/gcs_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     5433 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/convolutional/general_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     5343 2022-07-22 14:32:49.000000 spektral-1.2.0/spektral/layers/convolutional/gin_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     3939 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/convolutional/graphsage_conv.py
--rw-r--r--   0 phait      (501) staff       (20)     7175 2022-06-07 16:59:30.000000 spektral-1.2.0/spektral/layers/convolutional/message_passing.py
--rw-r--r--   0 phait      (501) staff       (20)     3770 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/layers/convolutional/tag_conv.py
--rw-r--r--   0 phait      (501) staff       (20)    13758 2022-07-22 14:31:49.000000 spektral-1.2.0/spektral/layers/convolutional/xenet_conv.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.665243 spektral-1.2.0/spektral/layers/ops/
--rw-r--r--   0 phait      (501) staff       (20)      128 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/ops/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)     2116 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/ops/graph.py
--rw-r--r--   0 phait      (501) staff       (20)     6354 2022-06-07 16:59:30.000000 spektral-1.2.0/spektral/layers/ops/matmul.py
--rw-r--r--   0 phait      (501) staff       (20)     3567 2022-07-22 08:54:42.000000 spektral-1.2.0/spektral/layers/ops/modes.py
--rw-r--r--   0 phait      (501) staff       (20)     3729 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/ops/ops.py
--rw-r--r--   0 phait      (501) staff       (20)     8807 2022-06-07 16:59:30.000000 spektral-1.2.0/spektral/layers/ops/scatter.py
--rw-r--r--   0 phait      (501) staff       (20)     7920 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/layers/ops/sparse.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.666985 spektral-1.2.0/spektral/layers/pooling/
--rw-r--r--   0 phait      (501) staff       (20)      410 2022-07-22 07:45:09.000000 spektral-1.2.0/spektral/layers/pooling/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)     5704 2022-07-22 07:45:09.000000 spektral-1.2.0/spektral/layers/pooling/diff_pool.py
--rw-r--r--   0 phait      (501) staff       (20)     7204 2022-07-22 07:45:09.000000 spektral-1.2.0/spektral/layers/pooling/dmon_pool.py
--rw-r--r--   0 phait      (501) staff       (20)    14217 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/layers/pooling/global_pool.py
--rw-r--r--   0 phait      (501) staff       (20)     5950 2022-07-22 07:45:09.000000 spektral-1.2.0/spektral/layers/pooling/just_balance_pool.py
--rw-r--r--   0 phait      (501) staff       (20)     6279 2022-06-07 16:59:30.000000 spektral-1.2.0/spektral/layers/pooling/la_pool.py
--rw-r--r--   0 phait      (501) staff       (20)     6104 2022-07-22 07:45:09.000000 spektral-1.2.0/spektral/layers/pooling/mincut_pool.py
--rw-r--r--   0 phait      (501) staff       (20)     3285 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/layers/pooling/sag_pool.py
--rw-r--r--   0 phait      (501) staff       (20)    12671 2022-06-07 16:59:30.000000 spektral-1.2.0/spektral/layers/pooling/src.py
--rw-r--r--   0 phait      (501) staff       (20)     6197 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/layers/pooling/topk_pool.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.667838 spektral-1.2.0/spektral/models/
--rw-r--r--   0 phait      (501) staff       (20)       97 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/models/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)     2705 2022-04-13 09:46:22.000000 spektral-1.2.0/spektral/models/gcn.py
--rw-r--r--   0 phait      (501) staff       (20)     6997 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/models/general_gnn.py
--rw-r--r--   0 phait      (501) staff       (20)    13718 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/models/gnn_explainer.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.669690 spektral-1.2.0/spektral/transforms/
--rw-r--r--   0 phait      (501) staff       (20)      463 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)      289 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/adj_to_sp_tensor.py
--rw-r--r--   0 phait      (501) staff       (20)      673 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/clustering_coefficient.py
--rw-r--r--   0 phait      (501) staff       (20)      500 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/constant.py
--rw-r--r--   0 phait      (501) staff       (20)     1056 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/degree.py
--rw-r--r--   0 phait      (501) staff       (20)     1022 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/delaunay.py
--rw-r--r--   0 phait      (501) staff       (20)      692 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/gcn_filter.py
--rw-r--r--   0 phait      (501) staff       (20)      992 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/laplacian_pe.py
--rw-r--r--   0 phait      (501) staff       (20)      566 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/layer_preprocess.py
--rw-r--r--   0 phait      (501) staff       (20)      519 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/normalize_adj.py
--rw-r--r--   0 phait      (501) staff       (20)      392 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/normalize_one.py
--rw-r--r--   0 phait      (501) staff       (20)      538 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/normalize_sphere.py
--rw-r--r--   0 phait      (501) staff       (20)      996 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/transforms/one_hot.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.670636 spektral-1.2.0/spektral/utils/
--rw-r--r--   0 phait      (501) staff       (20)      110 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/utils/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)    11683 2022-06-07 16:59:30.000000 spektral-1.2.0/spektral/utils/convolution.py
--rw-r--r--   0 phait      (501) staff       (20)    12807 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/utils/io.py
--rw-r--r--   0 phait      (501) staff       (20)     1372 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/utils/keras.py
--rw-r--r--   0 phait      (501) staff       (20)     2314 2022-03-03 14:08:01.000000 spektral-1.2.0/spektral/utils/logging.py
--rw-r--r--   0 phait      (501) staff       (20)     2923 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/utils/misc.py
--rw-r--r--   0 phait      (501) staff       (20)     2843 2022-03-03 13:47:36.000000 spektral-1.2.0/spektral/utils/sparse.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.656275 spektral-1.2.0/spektral.egg-info/
--rw-r--r--   0 phait      (501) staff       (20)     5446 2022-07-22 15:02:18.000000 spektral-1.2.0/spektral.egg-info/PKG-INFO
--rw-r--r--   0 phait      (501) staff       (20)     3125 2022-07-22 15:02:18.000000 spektral-1.2.0/spektral.egg-info/SOURCES.txt
--rw-r--r--   0 phait      (501) staff       (20)        1 2022-07-22 15:02:18.000000 spektral-1.2.0/spektral.egg-info/dependency_links.txt
--rw-r--r--   0 phait      (501) staff       (20)       85 2022-07-22 15:02:18.000000 spektral-1.2.0/spektral.egg-info/requires.txt
--rw-r--r--   0 phait      (501) staff       (20)       15 2022-07-22 15:02:18.000000 spektral-1.2.0/spektral.egg-info/top_level.txt
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.670839 spektral-1.2.0/tests/
--rw-r--r--   0 phait      (501) staff       (20)        0 2022-03-03 13:47:36.000000 spektral-1.2.0/tests/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)     1702 2022-07-22 07:45:09.000000 spektral-1.2.0/tests/test_datasets.py
-drwxr-xr-x   0 phait      (501) staff       (20)        0 2022-07-22 15:02:18.671277 spektral-1.2.0/tests/test_layers/
--rw-r--r--   0 phait      (501) staff       (20)        0 2022-03-03 13:47:36.000000 spektral-1.2.0/tests/test_layers/__init__.py
--rw-r--r--   0 phait      (501) staff       (20)     2107 2022-03-03 13:47:36.000000 spektral-1.2.0/tests/test_layers/test_base.py
--rw-r--r--   0 phait      (501) staff       (20)    14364 2022-07-22 14:02:45.000000 spektral-1.2.0/tests/test_layers/test_ops.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.100108 spektral-1.3.0/
+-rw-r--r--   0 phait      (501) staff       (20)     1075 2023-02-11 12:09:50.000000 spektral-1.3.0/LICENSE
+-rw-r--r--   0 phait      (501) staff       (20)     5512 2023-06-01 22:13:53.099435 spektral-1.3.0/PKG-INFO
+-rw-r--r--   0 phait      (501) staff       (20)     4981 2023-02-11 12:09:50.000000 spektral-1.3.0/README.md
+-rw-r--r--   0 phait      (501) staff       (20)      920 2023-06-01 22:13:37.000000 spektral-1.3.0/pyproject.toml
+-rw-r--r--   0 phait      (501) staff       (20)       38 2023-06-01 22:13:53.100291 spektral-1.3.0/setup.cfg
+-rw-r--r--   0 phait      (501) staff       (20)       69 2023-06-01 22:04:57.000000 spektral-1.3.0/setup.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.025522 spektral-1.3.0/spektral/
+-rw-r--r--   0 phait      (501) staff       (20)       61 2023-06-01 22:13:35.000000 spektral-1.3.0/spektral/__init__.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.033348 spektral-1.3.0/spektral/data/
+-rw-r--r--   0 phait      (501) staff       (20)      186 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/data/__init__.py
+-rw-r--r--   0 phait      (501) staff       (20)    10277 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/data/dataset.py
+-rw-r--r--   0 phait      (501) staff       (20)     5610 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/data/graph.py
+-rw-r--r--   0 phait      (501) staff       (20)    21819 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/data/loaders.py
+-rw-r--r--   0 phait      (501) staff       (20)    10658 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/data/utils.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.041896 spektral-1.3.0/spektral/datasets/
+-rw-r--r--   0 phait      (501) staff       (20)      303 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/datasets/__init__.py
+-rw-r--r--   0 phait      (501) staff       (20)     6590 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/datasets/citation.py
+-rw-r--r--   0 phait      (501) staff       (20)     2869 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/datasets/dblp.py
+-rw-r--r--   0 phait      (501) staff       (20)     2891 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/datasets/flickr.py
+-rw-r--r--   0 phait      (501) staff       (20)     6927 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/datasets/graphsage.py
+-rw-r--r--   0 phait      (501) staff       (20)     3018 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/datasets/mnist.py
+-rw-r--r--   0 phait      (501) staff       (20)     3257 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/datasets/modelnet.py
+-rw-r--r--   0 phait      (501) staff       (20)     1116 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/datasets/ogb.py
+-rw-r--r--   0 phait      (501) staff       (20)     1562 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/datasets/qm7.py
+-rw-r--r--   0 phait      (501) staff       (20)     3361 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/datasets/qm9.py
+-rw-r--r--   0 phait      (501) staff       (20)     8089 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/datasets/tudataset.py
+-rw-r--r--   0 phait      (501) staff       (20)     1405 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/datasets/utils.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.043289 spektral-1.3.0/spektral/layers/
+-rw-r--r--   0 phait      (501) staff       (20)       90 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/__init__.py
+-rw-r--r--   0 phait      (501) staff       (20)     8948 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/base.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.061398 spektral-1.3.0/spektral/layers/convolutional/
+-rw-r--r--   0 phait      (501) staff       (20)      723 2023-06-01 22:05:03.000000 spektral-1.3.0/spektral/layers/convolutional/__init__.py
+-rw-r--r--   0 phait      (501) staff       (20)     2666 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/convolutional/agnn_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     5098 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/appnp_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     8048 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/arma_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)    10489 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/censnet_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     4463 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/cheb_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     2918 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/convolutional/conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     3725 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/crystal_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     5944 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/diffusion_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     6994 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/ecc_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     4206 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/edge_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)    10281 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/gat_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     4254 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/gated_graph_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     3695 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/gcn_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     3852 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/gcs_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     5435 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/general_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     5345 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/gin_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     3941 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/graphsage_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     6767 2023-06-01 22:10:19.000000 spektral-1.3.0/spektral/layers/convolutional/gtv_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)     7175 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/convolutional/message_passing.py
+-rw-r--r--   0 phait      (501) staff       (20)     3772 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/tag_conv.py
+-rw-r--r--   0 phait      (501) staff       (20)    13762 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/convolutional/xenet_conv.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.067382 spektral-1.3.0/spektral/layers/ops/
+-rw-r--r--   0 phait      (501) staff       (20)      128 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/ops/__init__.py
+-rw-r--r--   0 phait      (501) staff       (20)     2116 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/ops/graph.py
+-rw-r--r--   0 phait      (501) staff       (20)     6354 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/ops/matmul.py
+-rw-r--r--   0 phait      (501) staff       (20)     3567 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/ops/modes.py
+-rw-r--r--   0 phait      (501) staff       (20)     3729 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/ops/ops.py
+-rw-r--r--   0 phait      (501) staff       (20)     8807 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/ops/scatter.py
+-rw-r--r--   0 phait      (501) staff       (20)     7920 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/ops/sparse.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.077218 spektral-1.3.0/spektral/layers/pooling/
+-rw-r--r--   0 phait      (501) staff       (20)      464 2023-06-01 22:05:03.000000 spektral-1.3.0/spektral/layers/pooling/__init__.py
+-rw-r--r--   0 phait      (501) staff       (20)     8006 2023-06-01 22:10:19.000000 spektral-1.3.0/spektral/layers/pooling/asym_cheeger_cut_pool.py
+-rw-r--r--   0 phait      (501) staff       (20)     5706 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/pooling/diff_pool.py
+-rw-r--r--   0 phait      (501) staff       (20)     7204 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/pooling/dmon_pool.py
+-rw-r--r--   0 phait      (501) staff       (20)    14218 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/pooling/global_pool.py
+-rw-r--r--   0 phait      (501) staff       (20)     5952 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/pooling/just_balance_pool.py
+-rw-r--r--   0 phait      (501) staff       (20)     6279 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/pooling/la_pool.py
+-rw-r--r--   0 phait      (501) staff       (20)     6106 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/pooling/mincut_pool.py
+-rw-r--r--   0 phait      (501) staff       (20)     3287 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/pooling/sag_pool.py
+-rw-r--r--   0 phait      (501) staff       (20)    12671 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/layers/pooling/src.py
+-rw-r--r--   0 phait      (501) staff       (20)     6199 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/layers/pooling/topk_pool.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.081274 spektral-1.3.0/spektral/models/
+-rw-r--r--   0 phait      (501) staff       (20)       97 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/models/__init__.py
+-rw-r--r--   0 phait      (501) staff       (20)     2705 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/models/gcn.py
+-rw-r--r--   0 phait      (501) staff       (20)     6997 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/models/general_gnn.py
+-rw-r--r--   0 phait      (501) staff       (20)    13718 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/models/gnn_explainer.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.091069 spektral-1.3.0/spektral/transforms/
+-rw-r--r--   0 phait      (501) staff       (20)      463 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/__init__.py
+-rw-r--r--   0 phait      (501) staff       (20)      289 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/adj_to_sp_tensor.py
+-rw-r--r--   0 phait      (501) staff       (20)      673 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/clustering_coefficient.py
+-rw-r--r--   0 phait      (501) staff       (20)      500 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/constant.py
+-rw-r--r--   0 phait      (501) staff       (20)     1056 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/degree.py
+-rw-r--r--   0 phait      (501) staff       (20)     1022 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/delaunay.py
+-rw-r--r--   0 phait      (501) staff       (20)      692 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/gcn_filter.py
+-rw-r--r--   0 phait      (501) staff       (20)      992 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/laplacian_pe.py
+-rw-r--r--   0 phait      (501) staff       (20)      566 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/layer_preprocess.py
+-rw-r--r--   0 phait      (501) staff       (20)      519 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/normalize_adj.py
+-rw-r--r--   0 phait      (501) staff       (20)      392 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/normalize_one.py
+-rw-r--r--   0 phait      (501) staff       (20)      538 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/normalize_sphere.py
+-rw-r--r--   0 phait      (501) staff       (20)      996 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/transforms/one_hot.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.097793 spektral-1.3.0/spektral/utils/
+-rw-r--r--   0 phait      (501) staff       (20)      110 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/utils/__init__.py
+-rw-r--r--   0 phait      (501) staff       (20)    11683 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/utils/convolution.py
+-rw-r--r--   0 phait      (501) staff       (20)    12804 2023-06-01 22:04:57.000000 spektral-1.3.0/spektral/utils/io.py
+-rw-r--r--   0 phait      (501) staff       (20)     1372 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/utils/keras.py
+-rw-r--r--   0 phait      (501) staff       (20)     2314 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/utils/logging.py
+-rw-r--r--   0 phait      (501) staff       (20)     2923 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/utils/misc.py
+-rw-r--r--   0 phait      (501) staff       (20)     2843 2023-02-11 12:09:50.000000 spektral-1.3.0/spektral/utils/sparse.py
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.029174 spektral-1.3.0/spektral.egg-info/
+-rw-r--r--   0 phait      (501) staff       (20)     5512 2023-06-01 22:13:53.000000 spektral-1.3.0/spektral.egg-info/PKG-INFO
+-rw-r--r--   0 phait      (501) staff       (20)     3107 2023-06-01 22:13:53.000000 spektral-1.3.0/spektral.egg-info/SOURCES.txt
+-rw-r--r--   0 phait      (501) staff       (20)        1 2023-06-01 22:13:53.000000 spektral-1.3.0/spektral.egg-info/dependency_links.txt
+-rw-r--r--   0 phait      (501) staff       (20)      236 2023-06-01 22:13:53.000000 spektral-1.3.0/spektral.egg-info/requires.txt
+-rw-r--r--   0 phait      (501) staff       (20)        9 2023-06-01 22:13:53.000000 spektral-1.3.0/spektral.egg-info/top_level.txt
+drwxr-xr-x   0 phait      (501) staff       (20)        0 2023-06-01 22:13:53.098566 spektral-1.3.0/tests/
+-rw-r--r--   0 phait      (501) staff       (20)     1702 2023-02-11 12:09:50.000000 spektral-1.3.0/tests/test_datasets.py
```

### Comparing `spektral-1.2.0/LICENSE` & `spektral-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/PKG-INFO` & `spektral-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: spektral
-Version: 1.2.0
-Summary: Graph Neural Networks with Keras and Tensorflow 2.
-Home-page: https://github.com/danielegrattarola/spektral
-Author: Daniele Grattarola
-Author-email: daniele.grattarola@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Version: 1.3.0
+Summary: Graph Neural Networks with Keras and TensorFlow.
+Author-email: Daniele Grattarola <daniele.grattarola@gmail.com>
+Project-URL: homepage, https://github.com/danielegrattarola/spektral
+Project-URL: documentation, https://graphneural.network
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://danielegrattarola.github.io/spektral/img/logo_dark.svg" style="max-width: 400px; width: 100%;"/>
 
 # Welcome to Spektral
 Spektral is a Python library for graph deep learning, based on the Keras API and TensorFlow 2.
```

### Comparing `spektral-1.2.0/README.md` & `spektral-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/data/dataset.py` & `spektral-1.3.0/spektral/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ```py
     class MyDataset(Dataset):
         def read(self):
             return [Graph(x=x, adj=adj, y=y) for x, adj, y in some_magic_list]
     ```
 
     The `download()` method is automatically called if the path returned by
-    `Dataset.path` does not exists (default `~/.spektral/datasets/ClassName/`).
+    `Dataset.path` does not exists (default `~/spektral/datasets/ClassName/`).
 
     In this case, `download()` will be called before `read()`.
 
     Datasets should generally behave like Numpy arrays for any operation that
     uses simple 1D indexing:
 
     ```py
```

### Comparing `spektral-1.2.0/spektral/data/graph.py` & `spektral-1.3.0/spektral/data/graph.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/data/loaders.py` & `spektral-1.3.0/spektral/data/loaders.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/data/utils.py` & `spektral-1.3.0/spektral/data/utils.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/datasets/citation.py` & `spektral-1.3.0/spektral/datasets/citation.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
     return load_binary(full_fname)
 
 
 def _idx_to_mask(idx, l):
     mask = np.zeros(l)
     mask[idx] = 1
-    return np.array(mask, dtype=np.bool)
+    return np.array(mask, dtype=bool)
 
 
 def _preprocess_features(features):
     rowsum = np.array(features.sum(1))
     r_inv = np.power(rowsum, -1).flatten()
     r_inv[np.isinf(r_inv)] = 0.0
     r_mat_inv = sp.diags(r_inv)
```

### Comparing `spektral-1.2.0/spektral/datasets/dblp.py` & `spektral-1.3.0/spektral/datasets/dblp.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/datasets/flickr.py` & `spektral-1.3.0/spektral/datasets/flickr.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/datasets/graphsage.py` & `spektral-1.3.0/spektral/datasets/graphsage.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,16 +199,16 @@
         [id_map[k] for k in id_map if k in G.nodes and G.nodes[k]["val"]],
         dtype=np.int32,
     )
     idx_te = np.array(
         [id_map[k] for k in id_map if k in G.nodes and G.nodes[k]["test"]],
         dtype=np.int32,
     )
-    mask_tr = np.ones(n, dtype=np.bool)
-    mask_va = np.zeros(n, dtype=np.bool)
-    mask_te = np.zeros(n, dtype=np.bool)
+    mask_tr = np.ones(n, dtype=bool)
+    mask_va = np.zeros(n, dtype=bool)
+    mask_te = np.zeros(n, dtype=bool)
     mask_tr[idx_va] = False
     mask_tr[idx_te] = False
     mask_va[idx_va] = True
     mask_te[idx_te] = True
 
     return x, adj, y, mask_tr, mask_va, mask_te
```

### Comparing `spektral-1.2.0/spektral/datasets/mnist.py` & `spektral-1.3.0/spektral/datasets/mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     return A
 
 
 def _flip_random_edges(A, p_swap):
     if not A.shape[0] == A.shape[1]:
         raise ValueError("A must be a square matrix.")
     dtype = A.dtype
-    A = sp.lil_matrix(A).astype(np.bool)
+    A = sp.lil_matrix(A).astype(bool)
     n_elem = A.shape[0] ** 2
     n_elem_to_flip = round(p_swap * n_elem)
     unique_idx = np.random.choice(n_elem, replace=False, size=n_elem_to_flip)
     row_idx = unique_idx // A.shape[0]
     col_idx = unique_idx % A.shape[0]
     idxs = np.stack((row_idx, col_idx)).T
     for i in idxs:
```

### Comparing `spektral-1.2.0/spektral/datasets/modelnet.py` & `spektral-1.3.0/spektral/datasets/modelnet.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/datasets/ogb.py` & `spektral-1.3.0/spektral/datasets/ogb.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/datasets/qm7.py` & `spektral-1.3.0/spektral/datasets/qm7.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/datasets/qm9.py` & `spektral-1.3.0/spektral/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/datasets/tudataset.py` & `spektral-1.3.0/spektral/datasets/tudataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     - edge attributes, if available;
     - edge labels, if available, one-hot encoded.
 
     Graph labels are provided for each dataset.
 
     Specific details about each individual dataset can be found in
-    `~/.spektral/datasets/TUDataset/<dataset name>/README.md`, after the dataset
+    `~/spektral/datasets/TUDataset/<dataset name>/README.md`, after the dataset
     has been downloaded locally (datasets are downloaded automatically upon
     calling `TUDataset('<dataset name>')` the first time).
 
     **Arguments**
 
     - `name`: str, name of the dataset to load (see `TUD.available_datasets`).
     - `clean`: if `True`, rload a version of the dataset with no isomorphic
```

### Comparing `spektral-1.2.0/spektral/datasets/utils.py` & `spektral-1.3.0/spektral/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/base.py` & `spektral-1.3.0/spektral/layers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,16 @@
     def __init__(
         self,
         trainable_kernel=False,
         activation=None,
         kernel_initializer="glorot_uniform",
         kernel_regularizer=None,
         kernel_constraint=None,
-        **kwargs
+        **kwargs,
     ):
-
         super().__init__(**kwargs)
         self.trainable_kernel = trainable_kernel
         self.activation = activations.get(activation)
         self.kernel_initializer = initializers.get(kernel_initializer)
         self.kernel_regularizer = regularizers.get(kernel_regularizer)
         self.kernel_constraint = constraints.get(kernel_constraint)
 
@@ -180,15 +179,14 @@
 
     - Tensor of shape `(n_nodes, n_nodes)`.
 
     :param activation: activation function;
     """
 
     def __init__(self, activation=None, **kwargs):
-
         super().__init__(**kwargs)
         self.activation = activations.get(activation)
 
     def build(self, input_shape):
         assert len(input_shape) >= 2
         self.built = True
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/__init__.py` & `spektral-1.3.0/spektral/layers/convolutional/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 from .gat_conv import GATConv
 from .gated_graph_conv import GatedGraphConv
 from .gcn_conv import GCNConv
 from .gcs_conv import GCSConv
 from .general_conv import GeneralConv
 from .gin_conv import GINConv, GINConvBatch
 from .graphsage_conv import GraphSageConv
+from .gtv_conv import GTVConv
 from .message_passing import MessagePassing
 from .tag_conv import TAGConv
 from .xenet_conv import XENetConv, XENetConvBatch
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/agnn_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/agnn_conv.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/convolutional/appnp_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/appnp_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,27 +69,27 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.mlp_hidden = mlp_hidden if mlp_hidden else []
         self.alpha = alpha
         self.propagations = propagations
         self.mlp_activation = activations.get(mlp_activation)
         self.dropout_rate = dropout_rate
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/arma_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/arma_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,27 +78,27 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.iterations = iterations
         self.order = order
         self.share_weights = share_weights
         self.gcn_activation = activations.get(gcn_activation)
         self.dropout_rate = dropout_rate
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/censnet_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/censnet_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,27 +70,27 @@
         edge_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         node_constraint=None,
         edge_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
 
         self.node_channels = node_channels
         self.edge_channels = edge_channels
 
         self.__node_initializer = tf.keras.initializers.get(node_initializer)
         self.__node_regularizer = tf.keras.regularizers.get(node_regularizer)
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/cheb_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/cheb_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,27 +68,27 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.K = K
 
     def build(self, input_shape):
         assert len(input_shape) >= 2
         input_dim = input_shape[0][-1]
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/conv.py` & `spektral-1.3.0/spektral/layers/convolutional/conv.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/convolutional/crystal_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/crystal_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,28 +57,28 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             aggregate=aggregate,
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
 
     def build(self, input_shape):
         assert len(input_shape) >= 2
         layer_kwargs = dict(
             kernel_initializer=self.kernel_initializer,
             bias_initializer=self.bias_initializer,
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/diffusion_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/diffusion_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def __init__(
         self,
         num_diffusion_steps,
         kernel_initializer,
         kernel_regularizer,
         kernel_constraint,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.K = num_diffusion_steps
         self.kernel_initializer = kernel_initializer
         self.kernel_regularizer = kernel_regularizer
         self.kernel_constraint = kernel_constraint
@@ -120,22 +120,22 @@
         self,
         channels,
         K=6,
         activation="tanh",
         kernel_initializer="glorot_uniform",
         kernel_regularizer=None,
         kernel_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             kernel_initializer=kernel_initializer,
             kernel_regularizer=kernel_regularizer,
             kernel_constraint=kernel_constraint,
-            **kwargs
+            **kwargs,
         )
 
         self.channels = channels
         self.K = K + 1
 
     def build(self, input_shape):
         self.filters = [
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/ecc_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/ecc_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,27 +72,27 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.kernel_network = kernel_network
         self.root = root
 
     def build(self, input_shape):
         F = input_shape[0][-1]
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/edge_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/edge_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,28 +62,28 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             aggregate=aggregate,
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.mlp_hidden = mlp_hidden if mlp_hidden else []
         self.mlp_activation = activations.get(mlp_activation)
 
     def build(self, input_shape):
         assert len(input_shape) >= 2
@@ -103,15 +103,15 @@
                 for channels in self.mlp_hidden
             ]
             + [
                 Dense(
                     self.channels,
                     self.activation,
                     use_bias=self.use_bias,
-                    **layer_kwargs
+                    **layer_kwargs,
                 )
             ]
         )
 
         self.built = True
 
     def message(self, x, **kwargs):
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/gat_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/gat_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,27 +91,27 @@
         kernel_regularizer=None,
         bias_regularizer=None,
         attn_kernel_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
         attn_kernel_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.attn_heads = attn_heads
         self.concat_heads = concat_heads
         self.dropout_rate = dropout_rate
         self.return_attn_coef = return_attn_coef
         self.add_self_loops = add_self_loops
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/gated_graph_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/gated_graph_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,27 +60,27 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.n_layers = n_layers
 
     def build(self, input_shape):
         assert len(input_shape) >= 2
         self.kernel = self.add_weight(
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/gcn_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/gcn_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,27 +54,27 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
 
     def build(self, input_shape):
         assert len(input_shape) >= 2
         input_dim = input_shape[0][-1]
         self.kernel = self.add_weight(
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/gcs_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/gcs_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,27 +51,27 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
 
     def build(self, input_shape):
         assert len(input_shape) >= 2
         input_dim = input_shape[0][-1]
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/general_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/general_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,28 +84,28 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             aggregate=aggregate,
             activation=None,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.dropout_rate = dropout
         self.use_batch_norm = batch_norm
         if activation == "prelu" or "prelu" in kwargs:
             self.activation = PReLU()
         else:
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/gin_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/gin_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,28 +70,28 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             aggregate=aggregate,
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.epsilon = epsilon
         self.mlp_hidden = mlp_hidden if mlp_hidden else []
         self.mlp_activation = activations.get(mlp_activation)
         self.mlp_batchnorm = mlp_batchnorm
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/graphsage_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/graphsage_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,28 +60,28 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             aggregate=aggregate,
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
 
     def build(self, input_shape):
         assert len(input_shape) >= 2
         input_dim = input_shape[0][-1]
         self.kernel = self.add_weight(
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/message_passing.py` & `spektral-1.3.0/spektral/layers/convolutional/message_passing.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/convolutional/tag_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/tag_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,28 +57,28 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             aggregate=aggregate,
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.channels = channels
         self.K = K
         self.linear = Dense(
             channels,
             activation=activation,
             use_bias=use_bias,
```

### Comparing `spektral-1.2.0/spektral/layers/convolutional/xenet_conv.py` & `spektral-1.3.0/spektral/layers/convolutional/xenet_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,27 +75,27 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             aggregate=aggregate,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.stack_channels = stack_channels
         self.node_channels = node_channels
         self.edge_channels = edge_channels
         self.attention = attention
         self.node_activation = node_activation
         self.edge_activation = edge_activation
@@ -233,27 +233,27 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             aggregate=aggregate,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.stack_channels = stack_channels
         self.node_channels = node_channels
         self.edge_channels = edge_channels
         self.attention = attention
         self.node_activation = node_activation
         self.edge_activation = edge_activation
```

### Comparing `spektral-1.2.0/spektral/layers/ops/graph.py` & `spektral-1.3.0/spektral/layers/ops/graph.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/ops/matmul.py` & `spektral-1.3.0/spektral/layers/ops/matmul.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/ops/modes.py` & `spektral-1.3.0/spektral/layers/ops/modes.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/ops/ops.py` & `spektral-1.3.0/spektral/layers/ops/ops.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/ops/scatter.py` & `spektral-1.3.0/spektral/layers/ops/scatter.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/ops/sparse.py` & `spektral-1.3.0/spektral/layers/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/pooling/diff_pool.py` & `spektral-1.3.0/spektral/layers/pooling/diff_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,22 +72,22 @@
         k,
         channels=None,
         return_selection=False,
         activation=None,
         kernel_initializer="glorot_uniform",
         kernel_regularizer=None,
         kernel_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             return_selection=return_selection,
             kernel_initializer=kernel_initializer,
             kernel_regularizer=kernel_regularizer,
             kernel_constraint=kernel_constraint,
-            **kwargs
+            **kwargs,
         )
         self.k = k
         self.channels = channels
         self.activation = activations.get(activation)
 
     def build(self, input_shape):
         in_channels = input_shape[0][-1]
```

### Comparing `spektral-1.2.0/spektral/layers/pooling/dmon_pool.py` & `spektral-1.3.0/spektral/layers/pooling/dmon_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,28 +80,28 @@
         collapse_regularization=0.1,
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             k=k,
             mlp_hidden=mlp_hidden,
             mlp_activation=mlp_activation,
             return_selection=return_selection,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
 
         self.k = k
         self.mlp_hidden = mlp_hidden if mlp_hidden is not None else []
         self.mlp_activation = mlp_activation
         self.collapse_regularization = collapse_regularization
 
@@ -158,15 +158,14 @@
     def reduce_index(self, i, s, **kwargs):
         i_mean = tf.math.segment_mean(i, i)
         i_pool = ops.repeat(i_mean, tf.ones_like(i_mean) * self.k)
 
         return i_pool
 
     def modularity_loss(self, a, s, a_pool):
-
         if K.is_sparse(a):
             n_edges = tf.cast(len(a.values), dtype=s.dtype)
 
             degrees = tf.sparse.reduce_sum(a, axis=-1)
             degrees = tf.reshape(degrees, (-1, 1))
         else:
             n_edges = tf.cast(tf.math.count_nonzero(a, axis=(-2, -1)), dtype=s.dtype)
```

### Comparing `spektral-1.2.0/spektral/layers/pooling/global_pool.py` & `spektral-1.3.0/spektral/layers/pooling/global_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from tensorflow.keras.layers import Dense, Layer
 
 from spektral.layers import ops
 
 
 class GlobalPool(Layer):
     def __init__(self, **kwargs):
-
         super().__init__(**kwargs)
         self.supports_masking = True
         self.pooling_op = None
         self.batch_pooling_op = None
 
     def build(self, input_shape):
         if isinstance(input_shape, list) and len(input_shape) == 2:
@@ -177,15 +176,15 @@
         channels,
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(**kwargs)
         self.channels = channels
         self.kernel_initializer = initializers.get(kernel_initializer)
         self.bias_initializer = initializers.get(bias_initializer)
         self.kernel_regularizer = regularizers.get(kernel_regularizer)
         self.bias_regularizer = regularizers.get(bias_regularizer)
@@ -286,15 +285,15 @@
     """
 
     def __init__(
         self,
         attn_kernel_initializer="glorot_uniform",
         attn_kernel_regularizer=None,
         attn_kernel_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(**kwargs)
         self.attn_kernel_initializer = initializers.get(attn_kernel_initializer)
         self.attn_kernel_regularizer = regularizers.get(attn_kernel_regularizer)
         self.attn_kernel_constraint = constraints.get(attn_kernel_constraint)
 
     def build(self, input_shape):
```

### Comparing `spektral-1.2.0/spektral/layers/pooling/just_balance_pool.py` & `spektral-1.3.0/spektral/layers/pooling/just_balance_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,25 +81,25 @@
         return_selection=False,
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             return_selection=return_selection,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
         self.k = k
         self.mlp_hidden = mlp_hidden if mlp_hidden else []
         self.mlp_activation = mlp_activation
         self.normalized_loss = normalized_loss
 
     def build(self, input_shape):
```

### Comparing `spektral-1.2.0/spektral/layers/pooling/la_pool.py` & `spektral-1.3.0/spektral/layers/pooling/la_pool.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/pooling/mincut_pool.py` & `spektral-1.3.0/spektral/layers/pooling/mincut_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,25 +79,25 @@
         return_selection=False,
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             return_selection=return_selection,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
-            **kwargs
+            **kwargs,
         )
 
         self.k = k
         self.mlp_hidden = mlp_hidden if mlp_hidden is not None else []
         self.mlp_activation = mlp_activation
 
     def build(self, input_shape):
```

### Comparing `spektral-1.2.0/spektral/layers/pooling/sag_pool.py` & `spektral-1.3.0/spektral/layers/pooling/sag_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,25 +63,25 @@
         ratio,
         return_selection=False,
         return_score=False,
         sigmoid_gating=False,
         kernel_initializer="glorot_uniform",
         kernel_regularizer=None,
         kernel_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             ratio,
             return_selection=return_selection,
             return_score=return_score,
             sigmoid_gating=sigmoid_gating,
             kernel_initializer=kernel_initializer,
             kernel_regularizer=kernel_regularizer,
             kernel_constraint=kernel_constraint,
-            **kwargs
+            **kwargs,
         )
 
     def call(self, inputs):
         x, a, i = self.get_inputs(inputs)
 
         # Graph filter for GNN
         if K.is_sparse(a):
```

### Comparing `spektral-1.2.0/spektral/layers/pooling/src.py` & `spektral-1.3.0/spektral/layers/pooling/src.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/layers/pooling/topk_pool.py` & `spektral-1.3.0/spektral/layers/pooling/topk_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,22 +66,22 @@
         ratio,
         return_selection=False,
         return_score=False,
         sigmoid_gating=False,
         kernel_initializer="glorot_uniform",
         kernel_regularizer=None,
         kernel_constraint=None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             return_selection=return_selection,
             kernel_initializer=kernel_initializer,
             kernel_regularizer=kernel_regularizer,
             kernel_constraint=kernel_constraint,
-            **kwargs
+            **kwargs,
         )
         self.ratio = ratio
         self.return_score = return_score
         self.sigmoid_gating = sigmoid_gating
         self.gating_op = K.sigmoid if self.sigmoid_gating else K.tanh
 
     def build(self, input_shape):
```

### Comparing `spektral-1.2.0/spektral/models/gcn.py` & `spektral-1.3.0/spektral/models/gcn.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/models/general_gnn.py` & `spektral-1.3.0/spektral/models/general_gnn.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/models/gnn_explainer.py` & `spektral-1.3.0/spektral/models/gnn_explainer.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/transforms/clustering_coefficient.py` & `spektral-1.3.0/spektral/transforms/clustering_coefficient.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/transforms/degree.py` & `spektral-1.3.0/spektral/transforms/degree.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/transforms/delaunay.py` & `spektral-1.3.0/spektral/transforms/delaunay.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/transforms/gcn_filter.py` & `spektral-1.3.0/spektral/transforms/gcn_filter.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/transforms/laplacian_pe.py` & `spektral-1.3.0/spektral/transforms/laplacian_pe.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/transforms/layer_preprocess.py` & `spektral-1.3.0/spektral/transforms/layer_preprocess.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/transforms/normalize_adj.py` & `spektral-1.3.0/spektral/transforms/normalize_adj.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/transforms/normalize_sphere.py` & `spektral-1.3.0/spektral/transforms/normalize_sphere.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/transforms/one_hot.py` & `spektral-1.3.0/spektral/transforms/one_hot.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/utils/convolution.py` & `spektral-1.3.0/spektral/utils/convolution.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/utils/io.py` & `spektral-1.3.0/spektral/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 elem[k] = ast.literal_eval(v)
             except ValueError:
                 elem[k] = str(v)
             except SyntaxError:
                 # Probably a numpy array
                 elem[k] = np.array(
                     " ".join(v.lstrip("[").rstrip("]").split()).split(" ")
-                ).astype(np.float)
+                ).astype(float)
 
     for elem in output.edges().values():
         for k, v in elem.items():
             try:
                 elem[k] = ast.literal_eval(v)
             except ValueError:
                 elem[k] = str(v)
```

### Comparing `spektral-1.2.0/spektral/utils/keras.py` & `spektral-1.3.0/spektral/utils/keras.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/utils/logging.py` & `spektral-1.3.0/spektral/utils/logging.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/utils/misc.py` & `spektral-1.3.0/spektral/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral/utils/sparse.py` & `spektral-1.3.0/spektral/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `spektral-1.2.0/spektral.egg-info/PKG-INFO` & `spektral-1.3.0/spektral.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: spektral
-Version: 1.2.0
-Summary: Graph Neural Networks with Keras and Tensorflow 2.
-Home-page: https://github.com/danielegrattarola/spektral
-Author: Daniele Grattarola
-Author-email: daniele.grattarola@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Version: 1.3.0
+Summary: Graph Neural Networks with Keras and TensorFlow.
+Author-email: Daniele Grattarola <daniele.grattarola@gmail.com>
+Project-URL: homepage, https://github.com/danielegrattarola/spektral
+Project-URL: documentation, https://graphneural.network
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://danielegrattarola.github.io/spektral/img/logo_dark.svg" style="max-width: 400px; width: 100%;"/>
 
 # Welcome to Spektral
 Spektral is a Python library for graph deep learning, based on the Keras API and TensorFlow 2.
```

### Comparing `spektral-1.2.0/spektral.egg-info/SOURCES.txt` & `spektral-1.3.0/spektral.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -41,25 +41,27 @@
 spektral/layers/convolutional/gat_conv.py
 spektral/layers/convolutional/gated_graph_conv.py
 spektral/layers/convolutional/gcn_conv.py
 spektral/layers/convolutional/gcs_conv.py
 spektral/layers/convolutional/general_conv.py
 spektral/layers/convolutional/gin_conv.py
 spektral/layers/convolutional/graphsage_conv.py
+spektral/layers/convolutional/gtv_conv.py
 spektral/layers/convolutional/message_passing.py
 spektral/layers/convolutional/tag_conv.py
 spektral/layers/convolutional/xenet_conv.py
 spektral/layers/ops/__init__.py
 spektral/layers/ops/graph.py
 spektral/layers/ops/matmul.py
 spektral/layers/ops/modes.py
 spektral/layers/ops/ops.py
 spektral/layers/ops/scatter.py
 spektral/layers/ops/sparse.py
 spektral/layers/pooling/__init__.py
+spektral/layers/pooling/asym_cheeger_cut_pool.py
 spektral/layers/pooling/diff_pool.py
 spektral/layers/pooling/dmon_pool.py
 spektral/layers/pooling/global_pool.py
 spektral/layers/pooling/just_balance_pool.py
 spektral/layers/pooling/la_pool.py
 spektral/layers/pooling/mincut_pool.py
 spektral/layers/pooling/sag_pool.py
@@ -85,12 +87,8 @@
 spektral/utils/__init__.py
 spektral/utils/convolution.py
 spektral/utils/io.py
 spektral/utils/keras.py
 spektral/utils/logging.py
 spektral/utils/misc.py
 spektral/utils/sparse.py
-tests/__init__.py
-tests/test_datasets.py
-tests/test_layers/__init__.py
-tests/test_layers/test_base.py
-tests/test_layers/test_ops.py
+tests/test_datasets.py
```

### Comparing `spektral-1.2.0/tests/test_datasets.py` & `spektral-1.3.0/tests/test_datasets.py`

 * *Files identical despite different names*

