# Comparing `tmp/intel_extension_for_transformers-1.0a0.tar.gz` & `tmp/intel_extension_for_transformers-1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intel_extension_for_transformers-1.0a0.tar", last modified: Wed Nov 23 15:50:11 2022, max compression
+gzip compressed data, was "intel_extension_for_transformers-1.0b0.tar", last modified: Sun Dec 11 05:19:15 2022, max compression
```

## Comparing `intel_extension_for_transformers-1.0a0.tar` & `intel_extension_for_transformers-1.0b0.tar`

### file list

```diff
@@ -1,153 +1,176 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/
--rw-r--r--   0 root         (0) root         (0)    11359 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10744 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9952 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.256497 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/
--rw-r--r--   0 root         (0) root         (0)     1561 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.256497 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/
--rw-r--r--   0 root         (0) root         (0)      631 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.256497 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/
--rw-r--r--   0 root         (0) root         (0)      631 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/bin/
--rw-r--r--   0 root         (0) root         (0)      885 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/bin/neural_engine
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.256497 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/
--rw-r--r--   0 root         (0) root         (0)      661 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2105 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.256497 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/
--rw-r--r--   0 root         (0) root         (0)      665 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1285 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/extractor.py
--rw-r--r--   0 root         (0) root         (0)     5079 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/onnx_extractor.py
--rw-r--r--   0 root         (0) root         (0)     2120 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/tf_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.256497 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/graph/
--rw-r--r--   0 root         (0) root         (0)      657 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51748 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    43928 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/graph_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.256497 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/
--rw-r--r--   0 root         (0) root         (0)      659 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1494 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/loader.py
--rw-r--r--   0 root         (0) root         (0)     4247 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/logger.py
--rw-r--r--   0 root         (0) root         (0)     8758 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/onnx_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.260498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/
--rw-r--r--   0 root         (0) root         (0)     1055 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)      960 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/all.py
--rw-r--r--   0 root         (0) root         (0)      966 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/assert.py
--rw-r--r--   0 root         (0) root         (0)     1035 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/batch_matmul.py
--rw-r--r--   0 root         (0) root         (0)     1098 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/batch_matmul_v2.py
--rw-r--r--   0 root         (0) root         (0)     1155 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/bias_add.py
--rw-r--r--   0 root         (0) root         (0)     1363 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/cast.py
--rw-r--r--   0 root         (0) root         (0)     1111 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/concat.py
--rw-r--r--   0 root         (0) root         (0)    10467 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/empty_ops.py
--rw-r--r--   0 root         (0) root         (0)     1160 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     1051 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_batch_matmul_v2.py
--rw-r--r--   0 root         (0) root         (0)     1138 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_batch_norm_v3.py
--rw-r--r--   0 root         (0) root         (0)     2147 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_gemm.py
--rw-r--r--   0 root         (0) root         (0)     1870 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_matmul.py
--rw-r--r--   0 root         (0) root         (0)     2326 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gather.py
--rw-r--r--   0 root         (0) root         (0)     1217 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gelu.py
--rw-r--r--   0 root         (0) root         (0)     1890 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gemm.py
--rw-r--r--   0 root         (0) root         (0)     1666 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/iterator_get_next.py
--rw-r--r--   0 root         (0) root         (0)     1498 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/iterator_v2.py
--rw-r--r--   0 root         (0) root         (0)     1128 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/layer_normalization.py
--rw-r--r--   0 root         (0) root         (0)     1514 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/map_and_batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1168 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/matmul.py
--rw-r--r--   0 root         (0) root         (0)     1195 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/mean.py
--rw-r--r--   0 root         (0) root         (0)     1215 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/mkl_layer_norm.py
--rw-r--r--   0 root         (0) root         (0)     1502 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/model_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1268 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/one_hot.py
--rw-r--r--   0 root         (0) root         (0)     1539 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/onnx_input.py
--rw-r--r--   0 root         (0) root         (0)     4265 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/op.py
--rw-r--r--   0 root         (0) root         (0)     1508 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/optimize_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1399 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/pack.py
--rw-r--r--   0 root         (0) root         (0)     1256 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/placeholder.py
--rw-r--r--   0 root         (0) root         (0)     1051 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_linear.py
--rw-r--r--   0 root         (0) root         (0)     1227 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_v2.py
--rw-r--r--   0 root         (0) root         (0)     2210 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_fused_matmul_and_dequantize.py
--rw-r--r--   0 root         (0) root         (0)     1412 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_matmul_with_bias_and_dequantize.py
--rw-r--r--   0 root         (0) root         (0)     1668 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     1316 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reshape.py
--rw-r--r--   0 root         (0) root         (0)     1463 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/softmax.py
--rw-r--r--   0 root         (0) root         (0)     1308 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/split.py
--rw-r--r--   0 root         (0) root         (0)     1404 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/squeeze.py
--rw-r--r--   0 root         (0) root         (0)     2004 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/strided_slice.py
--rw-r--r--   0 root         (0) root         (0)     3007 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/tensor.py
--rw-r--r--   0 root         (0) root         (0)     2044 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/transpose.py
--rw-r--r--   0 root         (0) root         (0)     1131 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/unpack.py
--rw-r--r--   0 root         (0) root         (0)     1158 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/unsqueeze.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.264498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/
--rw-r--r--   0 root         (0) root         (0)     1093 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7351 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/add_embeddings.py
--rw-r--r--   0 root         (0) root         (0)     8565 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_reshape.py
--rw-r--r--   0 root         (0) root         (0)    18129 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/collect_quant_info.py
--rw-r--r--   0 root         (0) root         (0)     4696 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/embeddingbag.py
--rw-r--r--   0 root         (0) root         (0)     2917 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/gelu.py
--rw-r--r--   0 root         (0) root         (0)     5809 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_data.py
--rw-r--r--   0 root         (0) root         (0)     1584 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_file.py
--rw-r--r--   0 root         (0) root         (0)     4037 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_bf16_node.py
--rw-r--r--   0 root         (0) root         (0)    11933 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_quant_node.py
--rw-r--r--   0 root         (0) root         (0)     7158 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/interact_features.py
--rw-r--r--   0 root         (0) root         (0)     8895 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/last_layer_shape.py
--rw-r--r--   0 root         (0) root         (0)     8129 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/layer_norm.py
--rw-r--r--   0 root         (0) root         (0)     4023 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/layer_norm_with_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     2974 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias.py
--rw-r--r--   0 root         (0) root         (0)     2966 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_add.py
--rw-r--r--   0 root         (0) root         (0)     2862 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_gelu.py
--rw-r--r--   0 root         (0) root         (0)     2844 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_relu.py
--rw-r--r--   0 root         (0) root         (0)     2943 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_sigmoid.py
--rw-r--r--   0 root         (0) root         (0)     2844 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_tanh.py
--rw-r--r--   0 root         (0) root         (0)     3076 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/merged_embeddingbag.py
--rw-r--r--   0 root         (0) root         (0)     1351 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/output_data.py
--rw-r--r--   0 root         (0) root         (0)    11653 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/padding_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2739 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/pattern.py
--rw-r--r--   0 root         (0) root         (0)     9896 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings.py
--rw-r--r--   0 root         (0) root         (0)     6625 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings_v1.py
--rw-r--r--   0 root         (0) root         (0)     8866 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/qkv_reshape.py
--rw-r--r--   0 root         (0) root         (0)     3844 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/quantize_fusion.py
--rw-r--r--   0 root         (0) root         (0)     3079 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/start_end_logits.py
--rw-r--r--   0 root         (0) root         (0)     5013 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/subgraph_matcher.py
--rw-r--r--   0 root         (0) root         (0)    14130 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings.py
--rw-r--r--   0 root         (0) root         (0)     7606 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings_v1.py
--rw-r--r--   0 root         (0) root         (0)     9043 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/transpose_batch_matmul.py
--rw-r--r--   0 root         (0) root         (0)     9791 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/word_embeddings.py
--rw-r--r--   0 root         (0) root         (0)     7122 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/tf_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.264498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/
--rw-r--r--   0 root         (0) root         (0)      631 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6090 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/benchmark.py
--rw-r--r--   0 root         (0) root         (0)    25394 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/config.py
--rw-r--r--   0 root         (0) root         (0)     1501 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/distillation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/dynamic/
--rw-r--r--   0 root         (0) root         (0)      630 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/dynamic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2386 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/dynamic/drop_and_restore_utils.py
--rw-r--r--   0 root         (0) root         (0)     7471 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/dynamic/evolution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/mixture/
--rw-r--r--   0 root         (0) root         (0)      631 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/mixture/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22251 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/mixture/auto_distillation.py
--rw-r--r--   0 root         (0) root         (0)    10724 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/model.py
--rw-r--r--   0 root         (0) root         (0)    12108 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/optimizer.py
--rw-r--r--   0 root         (0) root         (0)    23897 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/optimizer_tf.py
--rw-r--r--   0 root         (0) root         (0)     2994 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2193 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/pruning.py
--rw-r--r--   0 root         (0) root         (0)     1143 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/quantization.py
--rw-r--r--   0 root         (0) root         (0)   101681 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/
--rw-r--r--   0 root         (0) root         (0)      631 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1008 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/models/
--rw-r--r--   0 root         (0) root         (0)      630 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89251 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/models/modeling_bert_dynamic.py
--rw-r--r--   0 root         (0) root         (0)    77174 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/models/modeling_roberta_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     1223 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/objectives.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)     2839 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/utility_tf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/preprocessing/
--rw-r--r--   0 root         (0) root         (0)      631 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/preprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13018 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/preprocessing/data_augmentation.py
--rw-r--r--   0 root         (0) root         (0)     1404 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/preprocessing/utils.py
--rw-r--r--   0 root         (0) root         (0)      653 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10744 2022-11-23 15:50:11.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10670 2022-11-23 15:50:11.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-23 15:50:11.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2022-11-23 15:50:11.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       50 2022-11-23 15:50:11.000000 intel_extension_for_transformers-1.0a0/intel_extension_for_transformers.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-23 15:50:11.268498 intel_extension_for_transformers-1.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6527 2022-11-23 15:37:27.000000 intel_extension_for_transformers-1.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/
+-rw-r--r--   0 root         (0) root         (0)    11359 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    16294 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15496 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.237546 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/
+-rw-r--r--   0 root         (0) root         (0)     1571 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.237546 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.237546 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/bin/
+-rw-r--r--   0 root         (0) root         (0)      889 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/bin/neural_engine
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.237546 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/
+-rw-r--r--   0 root         (0) root         (0)      691 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.237546 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/
+-rw-r--r--   0 root         (0) root         (0)      715 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/extractor.py
+-rw-r--r--   0 root         (0) root         (0)     5204 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/onnx_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/tf_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.237546 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/graph/
+-rw-r--r--   0 root         (0) root         (0)      703 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65770 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    44637 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/graph_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.237546 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/
+-rw-r--r--   0 root         (0) root         (0)      712 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/loader.py
+-rw-r--r--   0 root         (0) root         (0)     4679 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/logger.py
+-rw-r--r--   0 root         (0) root         (0)     9681 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/onnx_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.241546 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/
+-rw-r--r--   0 root         (0) root         (0)     1105 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1166 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/all.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/assert.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/batch_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/batch_matmul_v2.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/bias_add.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/cast.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/concat.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/conv.py
+-rw-r--r--   0 root         (0) root         (0)    16529 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/empty_ops.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_batch_matmul_v2.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_batch_norm_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_gemm.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gather.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gather_elements.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gelu.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gemm.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/iterator_get_next.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/iterator_v2.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/layer_normalization.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/map_and_batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/matmul.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/mean.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/mkl_layer_norm.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/model_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/one_hot.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/onnx_input.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/op.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/optimize_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/pack.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/placeholder.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_linear.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_fused_matmul_and_dequantize.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_matmul_with_bias_and_dequantize.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reduce_sum.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     1299 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/scatter_elements.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/softmax.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/split.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/squeeze.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/strided_slice.py
+-rw-r--r--   0 root         (0) root         (0)     3645 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/top_k.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/transpose.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/unsqueeze.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.245547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/
+-rw-r--r--   0 root         (0) root         (0)     1136 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5872 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/add_cls_token.py
+-rw-r--r--   0 root         (0) root         (0)     8210 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/add_embeddings.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_mask_length_adaptive_keep_indices.py
+-rw-r--r--   0 root         (0) root         (0)     8070 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_output_layer_norm_length_adaptive_keep_indices.py
+-rw-r--r--   0 root         (0) root         (0)    10905 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_reshape.py
+-rw-r--r--   0 root         (0) root         (0)    18472 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/collect_quant_info.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/conv_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/embeddingbag.py
+-rw-r--r--   0 root         (0) root         (0)     3217 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/gelu.py
+-rw-r--r--   0 root         (0) root         (0)     3083 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/generate_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_data.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_file.py
+-rw-r--r--   0 root         (0) root         (0)     4374 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_bf16_node.py
+-rw-r--r--   0 root         (0) root         (0)    12273 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_quant_node.py
+-rw-r--r--   0 root         (0) root         (0)     7501 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/interact_features.py
+-rw-r--r--   0 root         (0) root         (0)     9223 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/last_layer_shape.py
+-rw-r--r--   0 root         (0) root         (0)     8444 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/layer_norm.py
+-rw-r--r--   0 root         (0) root         (0)     4380 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/layer_norm_with_reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_add.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_gelu.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_relu.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_sigmoid.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_tanh.py
+-rw-r--r--   0 root         (0) root         (0)     3418 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/merged_embeddingbag.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/output_data.py
+-rw-r--r--   0 root         (0) root         (0)    12652 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/padding_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/pattern.py
+-rw-r--r--   0 root         (0) root         (0)    10238 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings.py
+-rw-r--r--   0 root         (0) root         (0)     6973 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings_v1.py
+-rw-r--r--   0 root         (0) root         (0)    14769 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/qkv_merge.py
+-rw-r--r--   0 root         (0) root         (0)    10330 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/qkv_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     4179 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/quantize_fusion.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/reshape_after_restore_hidden_states.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/reshape_before_and_after_attention_out_layer_norm_gather_elements.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/reshape_before_restore_hidden_states.py
+-rw-r--r--   0 root         (0) root         (0)     8248 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/reshape_fusion.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/restore_hidden_states_in_length_adaptive_update_indices.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/start_end_logits.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/subgraph_matcher.py
+-rw-r--r--   0 root         (0) root         (0)    14475 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings.py
+-rw-r--r--   0 root         (0) root         (0)     7957 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings_v1.py
+-rw-r--r--   0 root         (0) root         (0)    10711 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/transpose_batch_matmul.py
+-rw-r--r--   0 root         (0) root         (0)    10121 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/word_embeddings.py
+-rw-r--r--   0 root         (0) root         (0)     7168 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/tf_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6398 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)    31616 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/config.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/distillation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/dynamic/
+-rw-r--r--   0 root         (0) root         (0)      630 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/dynamic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/dynamic/drop_and_restore_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7471 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/dynamic/evolution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/mixture/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/mixture/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25192 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/mixture/auto_distillation.py
+-rw-r--r--   0 root         (0) root         (0)    11343 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/model.py
+-rw-r--r--   0 root         (0) root         (0)    12156 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)    33067 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/optimizer_tf.py
+-rw-r--r--   0 root         (0) root         (0)     3105 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pruning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pytorch_pruner/
+-rw-r--r--   0 root         (0) root         (0)      630 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pytorch_pruner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17233 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pytorch_pruner/patterns.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pytorch_pruner/prune_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6853 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pytorch_pruner/pruner.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pytorch_pruner/pruning.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pytorch_pruner/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/quantization.py
+-rw-r--r--   0 root         (0) root         (0)   104711 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/models/
+-rw-r--r--   0 root         (0) root         (0)      630 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89251 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/models/modeling_bert_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)    77174 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/models/modeling_roberta_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/objectives.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/utility_tf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13018 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/preprocessing/data_augmentation.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/preprocessing/utils.py
+-rw-r--r--   0 root         (0) root         (0)      692 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16294 2022-12-11 05:19:15.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12776 2022-12-11 05:19:15.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-11 05:19:15.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2022-12-11 05:19:15.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2022-12-11 05:19:15.000000 intel_extension_for_transformers-1.0b0/intel_extension_for_transformers.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-11 05:19:15.249547 intel_extension_for_transformers-1.0b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8331 2022-12-11 05:15:19.000000 intel_extension_for_transformers-1.0b0/setup.py
```

### Comparing `intel_extension_for_transformers-1.0a0/LICENSE` & `intel_extension_for_transformers-1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/PKG-INFO` & `intel_extension_for_transformers-1.0b0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,672 +1,969 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 696e 7465  : 2.1.Name: inte
-00000020: 6c5f 6578 7465 6e73 696f 6e5f 666f 725f  l_extension_for_
-00000030: 7472 616e 7366 6f72 6d65 7273 0a56 6572  transformers.Ver
-00000040: 7369 6f6e 3a20 312e 3061 300a 5375 6d6d  sion: 1.0a0.Summ
-00000050: 6172 793a 2052 6570 6f73 6974 6f72 7920  ary: Repository 
-00000060: 6f66 2049 6e74 656c c2ae 2045 7874 656e  of Intel.. Exten
-00000070: 7369 6f6e 2066 6f72 2054 7261 6e73 666f  sion for Transfo
-00000080: 726d 6572 730a 486f 6d65 2d70 6167 653a  rmers.Home-page:
-00000090: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000000a0: 636f 6d2f 696e 7465 6c2f 0a41 7574 686f  com/intel/.Autho
-000000b0: 723a 2049 6e74 656c 2041 4941 2f41 4950  r: Intel AIA/AIP
-000000c0: 4320 5465 616d 0a41 7574 686f 722d 656d  C Team.Author-em
-000000d0: 6169 6c3a 2066 656e 672e 7469 616e 4069  ail: feng.tian@i
-000000e0: 6e74 656c 2e63 6f6d 2c20 6861 6968 616f  ntel.com, haihao
-000000f0: 2e73 6865 6e40 696e 7465 6c2e 636f 6d2c  .shen@intel.com,
-00000100: 6861 6e77 656e 2e63 6861 6e67 4069 6e74  hanwen.chang@int
-00000110: 656c 2e63 6f6d 2c20 7065 6e67 6875 692e  el.com, penghui.
-00000120: 6368 656e 6740 696e 7465 6c2e 636f 6d0a  cheng@intel.com.
-00000130: 4c69 6365 6e73 653a 2041 7061 6368 6520  License: Apache 
-00000140: 322e 300a 4b65 7977 6f72 6473 3a20 7175  2.0.Keywords: qu
-00000150: 616e 7469 7a61 7469 6f6e 2c61 7574 6f2d  antization,auto-
-00000160: 7475 6e69 6e67 2c70 6f73 742d 7472 6169  tuning,post-trai
-00000170: 6e69 6e67 2073 7461 7469 6320 7175 616e  ning static quan
-00000180: 7469 7a61 7469 6f6e 2c70 6f73 742d 7472  tization,post-tr
-00000190: 6169 6e69 6e67 2064 796e 616d 6963 2071  aining dynamic q
-000001a0: 7561 6e74 697a 6174 696f 6e2c 7175 616e  uantization,quan
-000001b0: 7469 7a61 7469 6f6e 2d61 7761 7265 2074  tization-aware t
-000001c0: 7261 696e 696e 672c 7475 6e69 6e67 2073  raining,tuning s
-000001d0: 7472 6174 6567 790a 436c 6173 7369 6669  trategy.Classifi
-000001e0: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
-000001f0: 6965 6e63 6520 3a3a 2053 6369 656e 6365  ience :: Science
-00000200: 2f52 6573 6561 7263 680a 436c 6173 7369  /Research.Classi
-00000210: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000220: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000230: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
-00000240: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000250: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-00000260: 6572 696e 6720 3a3a 2041 7274 6966 6963  ering :: Artific
-00000270: 6961 6c20 496e 7465 6c6c 6967 656e 6365  ial Intelligence
-00000280: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
-00000290: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000002a0: 6f76 6564 203a 3a20 4170 6163 6865 2053  oved :: Apache S
-000002b0: 6f66 7477 6172 6520 4c69 6365 6e73 650a  oftware License.
-000002c0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-000002d0: 203e 3d33 2e37 2e30 0a44 6573 6372 6970   >=3.7.0.Descrip
-000002e0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-000002f0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-00000300: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-00000310: 4943 454e 5345 0a0a 2320 496e 7465 6cc2  ICENSE..# Intel.
-00000320: ae20 4578 7465 6e73 696f 6e20 666f 7220  . Extension for 
-00000330: 5472 616e 7366 6f72 6d65 7273 3a20 4163  Transformers: Ac
-00000340: 6365 6c65 7261 7469 6e67 2054 7261 6e73  celerating Trans
-00000350: 666f 726d 6572 2d62 6173 6564 204d 6f64  former-based Mod
-00000360: 656c 7320 6f6e 2049 6e74 656c 2050 6c61  els on Intel Pla
-00000370: 7466 6f72 6d73 0a49 6e74 656c c2ae 2045  tforms.Intel.. E
-00000380: 7874 656e 7369 6f6e 2066 6f72 2054 7261  xtension for Tra
-00000390: 6e73 666f 726d 6572 7320 6973 2061 6e20  nsformers is an 
-000003a0: 696e 6e6f 7661 7469 7665 2074 6f6f 6c6b  innovative toolk
-000003b0: 6974 2074 6f20 6163 6365 6c65 7261 7465  it to accelerate
-000003c0: 2054 7261 6e73 666f 726d 6572 2d62 6173   Transformer-bas
-000003d0: 6564 206d 6f64 656c 7320 6f6e 2049 6e74  ed models on Int
-000003e0: 656c 2070 6c61 7466 6f72 6d73 2e20 5468  el platforms. Th
-000003f0: 6520 746f 6f6c 6b69 7420 6865 6c70 7320  e toolkit helps 
-00000400: 6465 7665 6c6f 7065 7273 2074 6f20 696d  developers to im
-00000410: 7072 6f76 6520 7468 6520 7072 6f64 7563  prove the produc
-00000420: 7469 7669 7479 2074 6872 6f75 6768 2065  tivity through e
-00000430: 6173 652d 6f66 2d75 7365 206d 6f64 656c  ase-of-use model
-00000440: 2063 6f6d 7072 6573 7369 6f6e 2041 5049   compression API
-00000450: 7320 6279 2065 7874 656e 6469 6e67 2048  s by extending H
-00000460: 7567 6769 6e67 2046 6163 6520 7472 616e  ugging Face tran
-00000470: 7366 6f72 6d65 7273 2041 5049 732e 2054  sformers APIs. T
-00000480: 6865 2063 6f6d 7072 6573 7369 6f6e 2069  he compression i
-00000490: 6e66 7261 7374 7275 6374 7572 6520 6c65  nfrastructure le
-000004a0: 7665 7261 6765 7320 496e 7465 6cc2 ae20  verages Intel.. 
-000004b0: 4e65 7572 616c 2043 6f6d 7072 6573 736f  Neural Compresso
-000004c0: 7220 7768 6963 6820 7072 6f76 6964 6573  r which provides
-000004d0: 2061 2072 6963 6820 7365 7420 6f66 206d   a rich set of m
-000004e0: 6f64 656c 2063 6f6d 7072 6573 7369 6f6e  odel compression
-000004f0: 2074 6563 686e 6971 7565 733a 2071 7561   techniques: qua
-00000500: 6e74 697a 6174 696f 6e2c 2070 7275 6e69  ntization, pruni
-00000510: 6e67 2c20 6469 7374 696c 6c61 7469 6f6e  ng, distillation
-00000520: 2061 6e64 2073 6f20 6f6e 2e20 5468 6520   and so on. The 
-00000530: 746f 6f6c 6b69 7420 7072 6f76 6964 6573  toolkit provides
-00000540: 2054 7261 6e73 666f 726d 6572 732d 6163   Transformers-ac
-00000550: 6365 6c65 7261 7465 6420 4c69 6272 6172  celerated Librar
-00000560: 6965 7320 616e 6420 4e65 7572 616c 2045  ies and Neural E
-00000570: 6e67 696e 6520 746f 2064 656d 6f6e 7374  ngine to demonst
-00000580: 7261 7465 2074 6865 2070 6572 666f 726d  rate the perform
-00000590: 616e 6365 206f 6620 6578 7472 656d 656c  ance of extremel
-000005a0: 7920 636f 6d70 7265 7373 6564 206d 6f64  y compressed mod
-000005b0: 656c 732c 2061 6e64 2074 6865 7265 666f  els, and therefo
-000005c0: 7265 2073 6967 6e69 6669 6361 6e74 6c79  re significantly
-000005d0: 2069 6d70 726f 7665 2074 6865 2069 6e66   improve the inf
-000005e0: 6572 656e 6365 2065 6666 6963 6965 6e63  erence efficienc
-000005f0: 7920 6f6e 2049 6e74 656c 2070 6c61 7466  y on Intel platf
-00000600: 6f72 6d73 2e20 536f 6d65 206f 6620 7468  orms. Some of th
-00000610: 6520 6b65 7920 6665 6174 7572 6573 2068  e key features h
-00000620: 6176 6520 6265 656e 2070 7562 6c69 7368  ave been publish
-00000630: 6564 2069 6e20 4e65 7572 4950 5320 3230  ed in NeurIPS 20
-00000640: 3231 2061 6e64 2032 3032 322e 0a0a 2323  21 and 2022...##
-00000650: 2057 6861 7420 646f 6573 2049 6e74 656c   What does Intel
-00000660: c2ae 2045 7874 656e 7369 6f6e 2066 6f72  .. Extension for
-00000670: 2054 7261 6e73 666f 726d 6572 7320 6f66   Transformers of
-00000680: 6665 723f 0a54 6869 7320 746f 6f6c 6b69  fer?.This toolki
-00000690: 7420 6865 6c70 7320 6465 7665 6c6f 7065  t helps develope
-000006a0: 7273 2074 6f20 696d 7072 6f76 6520 7468  rs to improve th
-000006b0: 6520 7072 6f64 7563 7469 7669 7479 206f  e productivity o
-000006c0: 6620 696e 6665 7265 6e63 6520 6465 706c  f inference depl
-000006d0: 6f79 6d65 6e74 2062 7920 6578 7465 6e64  oyment by extend
-000006e0: 696e 6720 4875 6767 696e 6720 4661 6365  ing Hugging Face
-000006f0: 2074 7261 6e73 666f 726d 6572 7320 4150   transformers AP
-00000700: 4973 2066 6f72 2054 7261 6e73 666f 726d  Is for Transform
-00000710: 6572 2d62 6173 6564 206d 6f64 656c 7320  er-based models 
-00000720: 696e 206e 6174 7572 616c 206c 616e 6775  in natural langu
-00000730: 6167 6520 7072 6f63 6573 7369 6e67 2028  age processing (
-00000740: 4e4c 5029 2064 6f6d 6169 6e2e 2057 6974  NLP) domain. Wit
-00000750: 6820 6578 7472 656d 656c 7920 636f 6d70  h extremely comp
-00000760: 7265 7373 6564 206d 6f64 656c 732c 2074  ressed models, t
-00000770: 6865 2074 6f6f 6c6b 6974 2063 616e 2067  he toolkit can g
-00000780: 7265 6174 6c79 2069 6d70 726f 7665 2074  reatly improve t
-00000790: 6865 2069 6e66 6572 656e 6365 2065 6666  he inference eff
-000007a0: 6963 6965 6e63 7920 6f6e 2049 6e74 656c  iciency on Intel
-000007b0: 2070 6c61 7466 6f72 6d73 2e0a 0a2d 204d   platforms...- M
-000007c0: 6f64 656c 2043 6f6d 7072 6573 7369 6f6e  odel Compression
-000007d0: 0a0a 2020 2020 7c46 7261 6d65 776f 726b  ..    |Framework
-000007e0: 2020 2020 2020 2020 2020 7c51 7561 6e74            |Quant
-000007f0: 697a 6174 696f 6e20 7c50 7275 6e69 6e67  ization |Pruning
-00000800: 2f53 7061 7273 6974 7920 7c44 6973 7469  /Sparsity |Disti
-00000810: 6c6c 6174 696f 6e20 7c4e 6575 7261 6c20  llation |Neural 
-00000820: 4172 6368 6974 6563 7475 7265 2053 6561  Architecture Sea
-00000830: 7263 6820 7c0a 2020 2020 7c2d 2d2d 2d2d  rch |.    |-----
-00000840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a  --------------|:
-00000850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
-00000860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a  -------------:|:
-00000870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
-00000880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000890: 2d2d 2d2d 2d2d 2d3a 7c0a 2020 2020 7c50  -------:|.    |P
-000008a0: 7954 6f72 6368 2020 2020 2020 2020 2020  yTorch          
-000008b0: 2020 7c26 2331 3030 3034 3b20 2020 2020    |&#10004;     
-000008c0: 7c26 2331 3030 3034 3b20 2020 2020 2020  |&#10004;       
-000008d0: 2020 7c26 2331 3030 3034 3b20 2020 2020    |&#10004;     
-000008e0: 7c26 2331 3030 3034 3b20 2020 2020 2020  |&#10004;       
-000008f0: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
-00000900: 2020 7c54 656e 736f 7246 6c6f 7720 2020    |TensorFlow   
-00000910: 2020 2020 2020 7c26 2331 3030 3034 3b20        |&#10004; 
-00000920: 2020 2020 7c26 2331 3030 3034 3b20 2020      |&#10004;   
-00000930: 2020 2020 2020 7c26 2331 3030 3034 3b20        |&#10004; 
-00000940: 2020 2020 7c53 7461 7920 7475 6e65 6420      |Stay tuned 
-00000950: 3a73 7461 723a 2020 2020 2020 2020 2020  :star:          
-00000960: 7c0a 0a2d 2044 6174 6120 4175 676d 656e  |..- Data Augmen
-00000970: 7461 7469 6f6e 2066 6f72 204e 4c50 2044  tation for NLP D
-00000980: 6174 6173 6574 730a 2d20 5472 616e 7366  atasets.- Transf
-00000990: 6f72 6d65 7273 2d61 6363 656c 6572 6174  ormers-accelerat
-000009a0: 6564 204e 6575 7261 6c20 456e 6769 6e65  ed Neural Engine
-000009b0: 0a2d 2054 7261 6e73 666f 726d 6572 732d  .- Transformers-
-000009c0: 6163 6365 6c65 7261 7465 6420 4c69 6272  accelerated Libr
-000009d0: 6172 6965 730a 2d20 446f 6d61 696e 2041  aries.- Domain A
-000009e0: 6c67 6f72 6974 686d 730a 2020 2020 7c4c  lgorithms.    |L
-000009f0: 656e 6774 6820 4164 6170 7469 7665 2054  ength Adaptive T
-00000a00: 7261 6e73 666f 726d 6572 207c 0a20 2020  ransformer |.   
-00000a10: 207c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |:-------------
-00000a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a  -------------:|.
-00000a30: 2020 2020 7c50 7954 6f72 6368 2026 2331      |PyTorch &#1
-00000a40: 3030 3034 3b20 2020 2020 2020 2020 2020  0004;           
-00000a50: 207c 0a0a 2d20 4172 6368 6974 6563 7475   |..- Architectu
-00000a60: 7265 206f 6620 496e 7465 6cc2 ae20 4578  re of Intel.. Ex
-00000a70: 7465 6e73 696f 6e20 666f 7220 5472 616e  tension for Tran
-00000a80: 7366 6f72 6d65 7273 0a3c 696d 6720 7372  sformers.<img sr
-00000a90: 633d 2264 6f63 732f 696d 6773 2f61 7263  c="docs/imgs/arc
-00000aa0: 682e 706e 6722 2077 6964 7468 3d36 3931  h.png" width=691
-00000ab0: 2068 6569 6768 743d 3434 3420 616c 743d   height=444 alt=
-00000ac0: 2261 7263 6822 3e0a 3c2f 6272 3e0a 0a23  "arch">.</br>..#
-00000ad0: 2320 496e 7374 616c 6c61 7469 6f6e 0a23  # Installation.#
-00000ae0: 2323 2320 496e 7374 616c 6c20 4465 7065  ### Install Depe
-00000af0: 6e64 656e 6379 0a60 6060 6261 7368 0a70  ndency.```bash.p
-00000b00: 6970 2069 6e73 7461 6c6c 202d 7220 7265  ip install -r re
-00000b10: 7175 6972 656d 656e 7473 2e74 7874 0a60  quirements.txt.`
-00000b20: 6060 0a0a 2323 2323 2049 6e73 7461 6c6c  ``..#### Install
-00000b30: 2049 6e74 656c c2ae 2045 7874 656e 7369   Intel.. Extensi
-00000b40: 6f6e 2066 6f72 2054 7261 6e73 666f 726d  on for Transform
-00000b50: 6572 730a 6060 6062 6173 680a 6769 7420  ers.```bash.git 
-00000b60: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
-00000b70: 7468 7562 2e63 6f6d 2f69 6e74 656c 2f69  thub.com/intel/i
-00000b80: 6e74 656c 2d65 7874 656e 7369 6f6e 2d66  ntel-extension-f
-00000b90: 6f72 2d74 7261 6e73 666f 726d 6572 732e  or-transformers.
-00000ba0: 6769 7420 696e 7465 6c5f 6578 7465 6e73  git intel_extens
-00000bb0: 696f 6e5f 666f 725f 7472 616e 7366 6f72  ion_for_transfor
-00000bc0: 6d65 7273 0a63 6420 696e 7465 6c5f 6578  mers.cd intel_ex
-00000bd0: 7465 6e73 696f 6e5f 666f 725f 7472 616e  tension_for_tran
-00000be0: 7366 6f72 6d65 7273 0a67 6974 2073 7562  sformers.git sub
-00000bf0: 6d6f 6475 6c65 2075 7064 6174 6520 2d2d  module update --
-00000c00: 696e 6974 202d 2d72 6563 7572 7369 7665  init --recursive
-00000c10: 0a70 7974 686f 6e20 7365 7475 702e 7079  .python setup.py
-00000c20: 2069 6e73 7461 6c6c 0a60 6060 0a0a 2323   install.```..##
-00000c30: 2047 6574 7469 6e67 2053 7461 7274 6564   Getting Started
-00000c40: 0a23 2323 2051 7561 6e74 697a 6174 696f  .### Quantizatio
-00000c50: 6e0a 6060 6070 7974 686f 6e0a 6672 6f6d  n.```python.from
-00000c60: 2069 6e74 656c 5f65 7874 656e 7369 6f6e   intel_extension
-00000c70: 5f66 6f72 5f74 7261 6e73 666f 726d 6572  _for_transformer
-00000c80: 7320 696d 706f 7274 2051 7561 6e74 697a  s import Quantiz
-00000c90: 6174 696f 6e43 6f6e 6669 672c 206d 6574  ationConfig, met
-00000ca0: 7269 632c 206f 626a 6563 7469 7665 730a  ric, objectives.
-00000cb0: 6672 6f6d 2069 6e74 656c 5f65 7874 656e  from intel_exten
-00000cc0: 7369 6f6e 5f66 6f72 5f74 7261 6e73 666f  sion_for_transfo
-00000cd0: 726d 6572 732e 6f70 7469 6d69 7a61 7469  rmers.optimizati
-00000ce0: 6f6e 2e74 7261 696e 6572 2069 6d70 6f72  on.trainer impor
-00000cf0: 7420 4e4c 5054 7261 696e 6572 0a0a 2320  t NLPTrainer..# 
-00000d00: 5265 706c 6163 6520 7472 616e 7366 6f72  Replace transfor
-00000d10: 6d65 7273 2e54 7261 696e 6572 2077 6974  mers.Trainer wit
-00000d20: 6820 4e4c 5054 7261 696e 6572 0a23 2074  h NLPTrainer.# t
-00000d30: 7261 696e 6572 203d 2074 7261 6e73 666f  rainer = transfo
-00000d40: 726d 6572 732e 5472 6169 6e65 7228 2e2e  rmers.Trainer(..
-00000d50: 2e29 0a74 7261 696e 6572 203d 204e 4c50  .).trainer = NLP
-00000d60: 5472 6169 6e65 7228 2e2e 2e29 0a6d 6574  Trainer(...).met
-00000d70: 7269 6320 3d20 6d65 7472 6963 732e 4d65  ric = metrics.Me
-00000d80: 7472 6963 286e 616d 653d 2265 7661 6c5f  tric(name="eval_
-00000d90: 6631 222c 2069 735f 7265 6c61 7469 7665  f1", is_relative
-00000da0: 3d54 7275 652c 2063 7269 7465 7269 6f6e  =True, criterion
-00000db0: 3d30 2e30 3129 0a71 5f63 6f6e 6669 6720  =0.01).q_config 
-00000dc0: 3d20 5175 616e 7469 7a61 7469 6f6e 436f  = QuantizationCo
-00000dd0: 6e66 6967 280a 2020 2020 6170 7072 6f61  nfig(.    approa
-00000de0: 6368 3d22 506f 7374 5472 6169 6e69 6e67  ch="PostTraining
-00000df0: 5374 6174 6963 222c 0a20 2020 206d 6574  Static",.    met
-00000e00: 7269 6373 3d5b 6d65 7472 6963 5d2c 0a20  rics=[metric],. 
-00000e10: 2020 206f 626a 6563 7469 7665 733d 5b6f     objectives=[o
-00000e20: 626a 6563 7469 7665 732e 7065 7266 6f72  bjectives.perfor
-00000e30: 6d61 6e63 655d 0a29 0a6d 6f64 656c 203d  mance].).model =
-00000e40: 2074 7261 696e 6572 2e71 7561 6e74 697a   trainer.quantiz
-00000e50: 6528 7175 616e 745f 636f 6e66 6967 3d71  e(quant_config=q
-00000e60: 5f63 6f6e 6669 6729 0a60 6060 0a0a 506c  _config).```..Pl
-00000e70: 6561 7365 2072 6566 6572 2074 6f20 5b71  ease refer to [q
-00000e80: 7561 6e74 697a 6174 696f 6e20 646f 6375  uantization docu
-00000e90: 6d65 6e74 5d28 646f 6373 2f71 7561 6e74  ment](docs/quant
-00000ea0: 697a 6174 696f 6e2e 6d64 2920 666f 7220  ization.md) for 
-00000eb0: 6d6f 7265 2064 6574 6169 6c73 2e0a 0a23  more details...#
-00000ec0: 2323 2050 7275 6e69 6e67 0a60 6060 7079  ## Pruning.```py
-00000ed0: 7468 6f6e 0a66 726f 6d20 696e 7465 6c5f  thon.from intel_
-00000ee0: 6578 7465 6e73 696f 6e5f 666f 725f 7472  extension_for_tr
-00000ef0: 616e 7366 6f72 6d65 7273 2069 6d70 6f72  ansformers impor
-00000f00: 7420 5072 756e 6572 436f 6e66 6967 2c20  t PrunerConfig, 
-00000f10: 5072 756e 696e 6743 6f6e 6669 670a 6672  PruningConfig.fr
-00000f20: 6f6d 2069 6e74 656c 5f65 7874 656e 7369  om intel_extensi
-00000f30: 6f6e 5f66 6f72 5f74 7261 6e73 666f 726d  on_for_transform
-00000f40: 6572 732e 6f70 7469 6d69 7a61 7469 6f6e  ers.optimization
-00000f50: 2e74 7261 696e 6572 2069 6d70 6f72 7420  .trainer import 
-00000f60: 4e4c 5054 7261 696e 6572 0a0a 2320 5265  NLPTrainer..# Re
-00000f70: 706c 6163 6520 7472 616e 7366 6f72 6d65  place transforme
-00000f80: 7273 2e54 7261 696e 6572 2077 6974 6820  rs.Trainer with 
-00000f90: 4e4c 5054 7261 696e 6572 0a23 2074 7261  NLPTrainer.# tra
-00000fa0: 696e 6572 203d 2074 7261 6e73 666f 726d  iner = transform
-00000fb0: 6572 732e 5472 6169 6e65 7228 2e2e 2e29  ers.Trainer(...)
-00000fc0: 0a74 7261 696e 6572 203d 204e 4c50 5472  .trainer = NLPTr
-00000fd0: 6169 6e65 7228 2e2e 2e29 0a6d 6574 7269  ainer(...).metri
-00000fe0: 6320 3d20 6d65 7472 6963 732e 4d65 7472  c = metrics.Metr
-00000ff0: 6963 286e 616d 653d 2265 7661 6c5f 6163  ic(name="eval_ac
-00001000: 6375 7261 6379 2229 0a70 7275 6e65 725f  curacy").pruner_
-00001010: 636f 6e66 6967 203d 2050 7275 6e65 7243  config = PrunerC
-00001020: 6f6e 6669 6728 7072 756e 655f 7479 7065  onfig(prune_type
-00001030: 3d27 4261 7369 634d 6167 6e69 7475 6465  ='BasicMagnitude
-00001040: 272c 2074 6172 6765 745f 7370 6172 7369  ', target_sparsi
-00001050: 7479 5f72 6174 696f 3d30 2e39 290a 705f  ty_ratio=0.9).p_
-00001060: 636f 6e66 203d 2050 7275 6e69 6e67 436f  conf = PruningCo
-00001070: 6e66 6967 2870 7275 6e65 725f 636f 6e66  nfig(pruner_conf
-00001080: 6967 3d5b 7072 756e 6572 5f63 6f6e 6669  ig=[pruner_confi
-00001090: 675d 2c20 6d65 7472 6963 733d 6d65 7472  g], metrics=metr
-000010a0: 6963 290a 6d6f 6465 6c20 3d20 7472 6169  ic).model = trai
-000010b0: 6e65 722e 7072 756e 6528 7072 756e 696e  ner.prune(prunin
-000010c0: 675f 636f 6e66 6967 3d70 5f63 6f6e 6629  g_config=p_conf)
-000010d0: 0a60 6060 0a0a 506c 6561 7365 2072 6566  .```..Please ref
-000010e0: 6572 2074 6f20 5b70 7275 6e69 6e67 2064  er to [pruning d
-000010f0: 6f63 756d 656e 745d 2864 6f63 732f 7072  ocument](docs/pr
-00001100: 756e 696e 672e 6d64 2920 666f 7220 6d6f  uning.md) for mo
-00001110: 7265 2064 6574 6169 6c73 2e0a 0a23 2323  re details...###
-00001120: 2044 6973 7469 6c6c 6174 696f 6e0a 6060   Distillation.``
-00001130: 6070 7974 686f 6e0a 6672 6f6d 2069 6e74  `python.from int
-00001140: 656c 5f65 7874 656e 7369 6f6e 5f66 6f72  el_extension_for
-00001150: 5f74 7261 6e73 666f 726d 6572 7320 696d  _transformers im
-00001160: 706f 7274 2044 6973 7469 6c6c 6174 696f  port Distillatio
-00001170: 6e43 6f6e 6669 672c 2043 7269 7465 7269  nConfig, Criteri
-00001180: 6f6e 0a66 726f 6d20 696e 7465 6c5f 6578  on.from intel_ex
-00001190: 7465 6e73 696f 6e5f 666f 725f 7472 616e  tension_for_tran
-000011a0: 7366 6f72 6d65 7273 2e6f 7074 696d 697a  sformers.optimiz
-000011b0: 6174 696f 6e2e 7472 6169 6e65 7220 696d  ation.trainer im
-000011c0: 706f 7274 204e 4c50 5472 6169 6e65 720a  port NLPTrainer.
-000011d0: 0a23 2052 6570 6c61 6365 2074 7261 6e73  .# Replace trans
-000011e0: 666f 726d 6572 732e 5472 6169 6e65 7220  formers.Trainer 
-000011f0: 7769 7468 204e 4c50 5472 6169 6e65 720a  with NLPTrainer.
-00001200: 2320 7472 6169 6e65 7220 3d20 7472 616e  # trainer = tran
-00001210: 7366 6f72 6d65 7273 2e54 7261 696e 6572  sformers.Trainer
-00001220: 282e 2e2e 290a 7465 6163 6865 725f 6d6f  (...).teacher_mo
-00001230: 6465 6c20 3d20 2e2e 2e20 2320 6578 6973  del = ... # exis
-00001240: 7420 6d6f 6465 6c0a 7472 6169 6e65 7220  t model.trainer 
-00001250: 3d20 4e4c 5054 7261 696e 6572 282e 2e2e  = NLPTrainer(...
-00001260: 290a 6d65 7472 6963 203d 206d 6574 7269  ).metric = metri
-00001270: 6373 2e4d 6574 7269 6328 6e61 6d65 3d22  cs.Metric(name="
-00001280: 6576 616c 5f61 6363 7572 6163 7922 290a  eval_accuracy").
-00001290: 645f 636f 6e66 203d 2044 6973 7469 6c6c  d_conf = Distill
-000012a0: 6174 696f 6e43 6f6e 6669 6728 6d65 7472  ationConfig(metr
-000012b0: 6963 733d 6d65 7472 6963 290a 6d6f 6465  ics=metric).mode
-000012c0: 6c20 3d20 7472 6169 6e65 722e 6469 7374  l = trainer.dist
-000012d0: 696c 6c28 6469 7374 696c 6c61 7469 6f6e  ill(distillation
-000012e0: 5f63 6f6e 6669 673d 645f 636f 6e66 2c20  _config=d_conf, 
-000012f0: 7465 6163 6865 725f 6d6f 6465 6c3d 7465  teacher_model=te
-00001300: 6163 6865 725f 6d6f 6465 6c29 0a60 6060  acher_model).```
-00001310: 0a0a 506c 6561 7365 2072 6566 6572 2074  ..Please refer t
-00001320: 6f20 5b64 6973 7469 6c6c 6174 696f 6e20  o [distillation 
-00001330: 646f 6375 6d65 6e74 5d28 646f 6373 2f64  document](docs/d
-00001340: 6973 7469 6c6c 6174 696f 6e2e 6d64 2920  istillation.md) 
-00001350: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
-00001360: 2e0a 0a23 2323 2044 6174 6120 4175 676d  ...### Data Augm
-00001370: 656e 7461 7469 6f6e 0a44 6174 6120 6175  entation.Data au
-00001380: 676d 656e 7461 7469 6f6e 2070 726f 7669  gmentation provi
-00001390: 6465 7320 7468 6520 6661 6369 6c69 7469  des the faciliti
-000013a0: 6573 2074 6f20 6765 6e65 7261 7465 2073  es to generate s
-000013b0: 796e 7468 6573 697a 6564 204e 4c50 2064  ynthesized NLP d
-000013c0: 6174 6173 6574 2066 6f72 2066 7572 7468  ataset for furth
-000013d0: 6572 206d 6f64 656c 206f 7074 696d 697a  er model optimiz
-000013e0: 6174 696f 6e2e 2054 6865 2064 6174 6120  ation. The data 
-000013f0: 6175 676d 656e 7461 7469 6f6e 2073 7570  augmentation sup
-00001400: 706f 7274 7320 7465 7874 2067 656e 6572  ports text gener
-00001410: 6174 696f 6e20 6f6e 2070 6f70 756c 6172  ation on popular
-00001420: 2066 696e 652d 7475 6e65 6420 6d6f 6465   fine-tuned mode
-00001430: 6c73 206c 696b 6520 4750 542c 2047 5054  ls like GPT, GPT
-00001440: 322c 2061 6e64 206f 7468 6572 2074 6578  2, and other tex
-00001450: 7420 7379 6e74 6865 7369 7320 6170 7072  t synthesis appr
-00001460: 6f61 6368 6573 2066 726f 6d20 5b6e 6c70  oaches from [nlp
-00001470: 6175 675d 2868 7474 7073 3a2f 2f67 6974  aug](https://git
-00001480: 6875 622e 636f 6d2f 6d61 6b63 6564 7761  hub.com/makcedwa
-00001490: 7264 2f6e 6c70 6175 6729 2e0a 0a60 6060  rd/nlpaug)...```
-000014a0: 7079 7468 6f6e 0a66 726f 6d20 696e 7465  python.from inte
-000014b0: 6c5f 6578 7465 6e73 696f 6e5f 666f 725f  l_extension_for_
-000014c0: 7472 616e 7366 6f72 6d65 7273 2e70 7265  transformers.pre
-000014d0: 7072 6f63 6573 7369 6e67 2e64 6174 615f  processing.data_
-000014e0: 6175 676d 656e 7461 7469 6f6e 2069 6d70  augmentation imp
-000014f0: 6f72 7420 4461 7461 4175 676d 656e 7461  ort DataAugmenta
-00001500: 7469 6f6e 0a61 7567 203d 2044 6174 6141  tion.aug = DataA
-00001510: 7567 6d65 6e74 6174 696f 6e28 6175 676d  ugmentation(augm
-00001520: 656e 7465 725f 7479 7065 3d22 5465 7874  enter_type="Text
-00001530: 4765 6e65 7261 7469 6f6e 4175 6722 290a  GenerationAug").
-00001540: 6175 672e 696e 7075 745f 6461 7461 7365  aug.input_datase
-00001550: 7420 3d20 226f 7269 6769 6e61 6c5f 6461  t = "original_da
-00001560: 7461 7365 742e 6373 7622 2023 2065 7861  taset.csv" # exa
-00001570: 6d70 6c65 3a20 6874 7470 733a 2f2f 6875  mple: https://hu
-00001580: 6767 696e 6766 6163 652e 636f 2f64 6174  ggingface.co/dat
-00001590: 6173 6574 732f 676c 7565 2f76 6965 7765  asets/glue/viewe
-000015a0: 722f 7373 7432 2f74 7261 696e 0a61 7567  r/sst2/train.aug
-000015b0: 2e63 6f6c 756d 6e5f 6e61 6d65 7320 3d20  .column_names = 
-000015c0: 2273 656e 7465 6e63 6522 0a61 7567 2e6f  "sentence".aug.o
-000015d0: 7574 7075 745f 7061 7468 203d 206f 732e  utput_path = os.
-000015e0: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e72  path.join(self.r
-000015f0: 6573 756c 745f 7061 7468 2c20 2274 6573  esult_path, "tes
-00001600: 7432 2e63 7673 2229 0a61 7567 2e61 7567  t2.cvs").aug.aug
-00001610: 6d65 6e74 6572 5f61 7267 756d 656e 7473  menter_arguments
-00001620: 203d 207b 276d 6f64 656c 5f6e 616d 655f   = {'model_name_
-00001630: 6f72 5f70 6174 6827 3a20 2767 7074 322d  or_path': 'gpt2-
-00001640: 6d65 6469 756d 277d 0a61 7567 2e64 6174  medium'}.aug.dat
-00001650: 615f 6175 676d 656e 7428 290a 7261 775f  a_augment().raw_
-00001660: 6461 7461 7365 7473 203d 206c 6f61 645f  datasets = load_
-00001670: 6461 7461 7365 7428 2263 7376 222c 2064  dataset("csv", d
-00001680: 6174 615f 6669 6c65 733d 6175 672e 6f75  ata_files=aug.ou
-00001690: 7470 7574 5f70 6174 682c 2064 656c 696d  tput_path, delim
-000016a0: 6974 6572 3d22 5c74 222c 2073 706c 6974  iter="\t", split
-000016b0: 3d22 7472 6169 6e22 290a 6060 600a 0a50  ="train").```..P
-000016c0: 6c65 6173 6520 7265 6665 7220 746f 205b  lease refer to [
-000016d0: 6461 7461 2061 7567 6d65 6e74 6174 696f  data augmentatio
-000016e0: 6e20 646f 6375 6d65 6e74 5d28 646f 6373  n document](docs
-000016f0: 2f64 6174 615f 6175 676d 656e 7461 7469  /data_augmentati
-00001700: 6f6e 2e6d 6429 2066 6f72 206d 6f72 6520  on.md) for more 
-00001710: 6465 7461 696c 732e 0a0a 2323 2320 5175  details...### Qu
-00001720: 616e 7469 7a65 6420 4c65 6e67 7468 2041  antized Length A
-00001730: 6461 7074 6976 6520 5472 616e 7366 6f72  daptive Transfor
-00001740: 6d65 720a 5175 616e 7469 7a65 6420 4c65  mer.Quantized Le
-00001750: 6e67 7468 2041 6461 7074 6976 6520 5472  ngth Adaptive Tr
-00001760: 616e 7366 6f72 6d65 7220 6c65 7665 7261  ansformer levera
-00001770: 6765 7320 7365 7175 656e 6365 2d6c 656e  ges sequence-len
-00001780: 6774 6820 7265 6475 6374 696f 6e20 616e  gth reduction an
-00001790: 6420 6c6f 772d 6269 7420 7265 7072 6573  d low-bit repres
-000017a0: 656e 7461 7469 6f6e 2074 6563 686e 6971  entation techniq
-000017b0: 7565 7320 746f 2066 7572 7468 6572 2065  ues to further e
-000017c0: 6e68 616e 6365 206d 6f64 656c 2069 6e66  nhance model inf
-000017d0: 6572 656e 6365 2070 6572 666f 726d 616e  erence performan
-000017e0: 6365 2c20 656e 6162 6c69 6e67 2061 6461  ce, enabling ada
-000017f0: 7074 6976 6520 7365 7175 656e 6365 2d6c  ptive sequence-l
-00001800: 656e 6774 6820 7369 7a65 7320 746f 2061  ength sizes to a
-00001810: 6363 6f6d 6d6f 6461 7465 2064 6966 6665  ccommodate diffe
-00001820: 7265 6e74 2063 6f6d 7075 7461 7469 6f6e  rent computation
-00001830: 616c 2062 7564 6765 7420 7265 7175 6972  al budget requir
-00001840: 656d 656e 7473 2077 6974 6820 616e 206f  ements with an o
-00001850: 7074 696d 616c 2061 6363 7572 6163 7920  ptimal accuracy 
-00001860: 6566 6669 6369 656e 6379 2074 7261 6465  efficiency trade
-00001870: 6f66 662e 0a60 6060 7079 7468 6f6e 0a66  off..```python.f
-00001880: 726f 6d20 696e 7465 6c5f 6578 7465 6e73  rom intel_extens
-00001890: 696f 6e5f 666f 725f 7472 616e 7366 6f72  ion_for_transfor
-000018a0: 6d65 7273 2069 6d70 6f72 7420 5175 616e  mers import Quan
-000018b0: 7469 7a61 7469 6f6e 436f 6e66 6967 2c20  tizationConfig, 
-000018c0: 4479 6e61 6d69 634c 656e 6774 6843 6f6e  DynamicLengthCon
-000018d0: 6669 672c 206d 6574 7269 632c 206f 626a  fig, metric, obj
-000018e0: 6563 7469 7665 730a 6672 6f6d 2069 6e74  ectives.from int
-000018f0: 656c 5f65 7874 656e 7369 6f6e 5f66 6f72  el_extension_for
-00001900: 5f74 7261 6e73 666f 726d 6572 732e 6f70  _transformers.op
-00001910: 7469 6d69 7a61 7469 6f6e 2e74 7261 696e  timization.train
-00001920: 6572 2069 6d70 6f72 7420 4e4c 5054 7261  er import NLPTra
-00001930: 696e 6572 0a0a 2320 5265 706c 6163 6520  iner..# Replace 
-00001940: 7472 616e 7366 6f72 6d65 7273 2e54 7261  transformers.Tra
-00001950: 696e 6572 2077 6974 6820 4e4c 5054 7261  iner with NLPTra
-00001960: 696e 6572 0a23 2074 7261 696e 6572 203d  iner.# trainer =
-00001970: 2074 7261 6e73 666f 726d 6572 732e 5472   transformers.Tr
-00001980: 6169 6e65 7228 2e2e 2e29 0a74 7261 696e  ainer(...).train
-00001990: 6572 203d 204e 4c50 5472 6169 6e65 7228  er = NLPTrainer(
-000019a0: 2e2e 2e29 0a6d 6574 7269 6320 3d20 6d65  ...).metric = me
-000019b0: 7472 6963 732e 4d65 7472 6963 286e 616d  trics.Metric(nam
-000019c0: 653d 2265 7661 6c5f 6631 222c 2069 735f  e="eval_f1", is_
-000019d0: 7265 6c61 7469 7665 3d54 7275 652c 2063  relative=True, c
-000019e0: 7269 7465 7269 6f6e 3d30 2e30 3129 0a71  riterion=0.01).q
-000019f0: 5f63 6f6e 6669 6720 3d20 5175 616e 7469  _config = Quanti
-00001a00: 7a61 7469 6f6e 436f 6e66 6967 280a 2020  zationConfig(.  
-00001a10: 2020 6170 7072 6f61 6368 3d22 506f 7374    approach="Post
-00001a20: 5472 6169 6e69 6e67 5374 6174 6963 222c  TrainingStatic",
-00001a30: 0a20 2020 206d 6574 7269 6373 3d5b 6d65  .    metrics=[me
-00001a40: 7472 6963 5d2c 0a20 2020 206f 626a 6563  tric],.    objec
-00001a50: 7469 7665 733d 5b6f 626a 6563 7469 7665  tives=[objective
-00001a60: 732e 7065 7266 6f72 6d61 6e63 655d 0a29  s.performance].)
-00001a70: 0a23 2041 7070 6c79 2074 6865 206c 656e  .# Apply the len
-00001a80: 6774 6820 636f 6e66 6967 0a64 796e 616d  gth config.dynam
-00001a90: 6963 5f6c 656e 6774 685f 636f 6e66 6967  ic_length_config
-00001aa0: 203d 2044 796e 616d 6963 4c65 6e67 7468   = DynamicLength
-00001ab0: 436f 6e66 6967 286c 656e 6774 685f 636f  Config(length_co
-00001ac0: 6e66 6967 3d6c 656e 6774 685f 636f 6e66  nfig=length_conf
-00001ad0: 6967 290a 7472 6169 6e65 722e 7365 745f  ig).trainer.set_
-00001ae0: 6479 6e61 6d69 635f 636f 6e66 6967 2864  dynamic_config(d
-00001af0: 796e 616d 6963 5f63 6f6e 6669 673d 6479  ynamic_config=dy
-00001b00: 6e61 6d69 635f 6c65 6e67 7468 5f63 6f6e  namic_length_con
-00001b10: 6669 6729 0a23 2051 7561 6e74 697a 6174  fig).# Quantizat
-00001b20: 696f 6e0a 6d6f 6465 6c20 3d20 7472 6169  ion.model = trai
-00001b30: 6e65 722e 7175 616e 7469 7a65 2871 7561  ner.quantize(qua
-00001b40: 6e74 5f63 6f6e 6669 673d 715f 636f 6e66  nt_config=q_conf
-00001b50: 6967 290a 6060 600a 0a50 6c65 6173 6520  ig).```..Please 
-00001b60: 7265 6665 7220 746f 2070 6170 6572 205b  refer to paper [
-00001b70: 5175 614c 412d 4d69 6e69 4c4d 5d28 6874  QuaLA-MiniLM](ht
-00001b80: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00001b90: 7064 662f 3232 3130 2e31 3731 3134 2e70  pdf/2210.17114.p
-00001ba0: 6466 2920 616e 6420 5b63 6f64 655d 2865  df) and [code](e
-00001bb0: 7861 6d70 6c65 732f 6f70 7469 6d69 7a61  xamples/optimiza
-00001bc0: 7469 6f6e 2f70 7974 6f72 6368 2f68 7567  tion/pytorch/hug
-00001bd0: 6769 6e67 6661 6365 2f71 7565 7374 696f  gingface/questio
-00001be0: 6e2d 616e 7377 6572 696e 672f 6479 6e61  n-answering/dyna
-00001bf0: 6d69 6329 2066 6f72 2064 6574 6169 6c73  mic) for details
-00001c00: 0a0a 0a23 2323 2054 7261 6e73 666f 726d  ...### Transform
-00001c10: 6572 732d 6163 6365 6c65 7261 7465 6420  ers-accelerated 
-00001c20: 4e65 7572 616c 2045 6e67 696e 650a 5472  Neural Engine.Tr
-00001c30: 616e 7366 6f72 6d65 7273 2d61 6363 656c  ansformers-accel
-00001c40: 6572 6174 6564 204e 6575 7261 6c20 456e  erated Neural En
-00001c50: 6769 6e65 2069 7320 6f6e 6520 6f66 2072  gine is one of r
-00001c60: 6566 6572 656e 6365 2064 6570 6c6f 796d  eference deploym
-00001c70: 656e 7473 2074 6861 7420 496e 7465 6cc2  ents that Intel.
-00001c80: ae20 4578 7465 6e73 696f 6e20 666f 7220  . Extension for 
-00001c90: 5472 616e 7366 6f72 6d65 7273 2070 726f  Transformers pro
-00001ca0: 7669 6465 732e 204e 6575 7261 6c20 456e  vides. Neural En
-00001cb0: 6769 6e65 2061 696d 7320 746f 2064 656d  gine aims to dem
-00001cc0: 6f6e 7374 7261 7465 2074 6865 206f 7074  onstrate the opt
-00001cd0: 696d 616c 2070 6572 666f 726d 616e 6365  imal performance
-00001ce0: 206f 6620 6578 7472 656d 656c 7920 636f   of extremely co
-00001cf0: 6d70 7265 7373 6564 204e 4c50 206d 6f64  mpressed NLP mod
-00001d00: 656c 7320 6279 2065 7870 6c6f 7269 6e67  els by exploring
-00001d10: 2074 6865 206f 7074 696d 697a 6174 696f   the optimizatio
-00001d20: 6e20 6f70 706f 7274 756e 6974 6965 7320  n opportunities 
-00001d30: 6672 6f6d 2062 6f74 6820 4857 2061 6e64  from both HW and
-00001d40: 2053 572e 0a0a 6060 6070 7974 686f 6e0a   SW...```python.
-00001d50: 6672 6f6d 2069 6e74 656c 5f65 7874 656e  from intel_exten
-00001d60: 7369 6f6e 5f66 6f72 5f74 7261 6e73 666f  sion_for_transfo
-00001d70: 726d 6572 732e 6261 636b 656e 6473 2e6e  rmers.backends.n
-00001d80: 6575 7261 6c5f 656e 6769 6e65 2e63 6f6d  eural_engine.com
-00001d90: 7069 6c65 2069 6d70 6f72 7420 636f 6d70  pile import comp
-00001da0: 696c 650a 2320 2f70 6174 682f 746f 2f79  ile.# /path/to/y
-00001db0: 6f75 722f 6d6f 6465 6c20 6973 2061 2054  our/model is a T
-00001dc0: 656e 736f 7246 6c6f 7720 7062 206d 6f64  ensorFlow pb mod
-00001dd0: 656c 206f 7220 4f4e 4e58 206d 6f64 656c  el or ONNX model
-00001de0: 0a6d 6f64 656c 203d 2063 6f6d 7069 6c65  .model = compile
-00001df0: 2827 2f70 6174 682f 746f 2f79 6f75 722f  ('/path/to/your/
-00001e00: 6d6f 6465 6c27 290a 696e 7075 7473 203d  model').inputs =
-00001e10: 202e 2e2e 2023 205b 696e 7075 745f 6964   ... # [input_id
-00001e20: 732c 2073 6567 6d65 6e74 5f69 6473 2c20  s, segment_ids, 
-00001e30: 696e 7075 745f 6d61 736b 5d0a 6d6f 6465  input_mask].mode
-00001e40: 6c2e 696e 6665 7265 6e63 6528 696e 7075  l.inference(inpu
-00001e50: 7473 290a 6060 600a 0a50 6c65 6173 6520  ts).```..Please 
-00001e60: 7265 6665 7220 746f 205b 6578 616d 706c  refer to [exampl
-00001e70: 655d 2865 7861 6d70 6c65 732f 6465 706c  e](examples/depl
-00001e80: 6f79 6d65 6e74 2f6e 6575 7261 6c5f 656e  oyment/neural_en
-00001e90: 6769 6e65 2f73 7061 7273 652f 6469 7374  gine/sparse/dist
-00001ea0: 696c 6265 7274 5f62 6173 655f 756e 6361  ilbert_base_unca
-00001eb0: 7365 642f 2920 696e 205b 5472 616e 7366  sed/) in [Transf
-00001ec0: 6f72 6d65 7273 2d61 6363 656c 6572 6174  ormers-accelerat
-00001ed0: 6564 204e 6575 7261 6c20 456e 6769 6e65  ed Neural Engine
-00001ee0: 5d28 6578 616d 706c 6573 2f64 6570 6c6f  ](examples/deplo
-00001ef0: 796d 656e 742f 2920 616e 6420 7061 7065  yment/) and pape
-00001f00: 7220 5b46 6173 7420 4469 7374 696c 6265  r [Fast Distilbe
-00001f10: 7274 206f 6e20 4350 5573 5d28 6874 7470  rt on CPUs](http
-00001f20: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-00001f30: 732f 3232 3131 2e30 3737 3135 2920 666f  s/2211.07715) fo
-00001f40: 7220 6d6f 7265 2064 6574 6169 6c73 2e0a  r more details..
-00001f50: 0a23 2323 2054 7261 6e73 666f 726d 6572  .### Transformer
-00001f60: 732d 6163 6365 6c65 7261 7465 6420 4c69  s-accelerated Li
-00001f70: 6272 6172 6965 730a 5472 616e 7366 6f72  braries.Transfor
-00001f80: 6d65 7273 2d61 6363 656c 6572 6174 6564  mers-accelerated
-00001f90: 204c 6962 7261 7269 6573 2069 7320 6120   Libraries is a 
-00001fa0: 6869 6768 2d70 6572 666f 726d 616e 6365  high-performance
-00001fb0: 206f 7065 7261 746f 7220 636f 6d70 7574   operator comput
-00001fc0: 696e 6720 6c69 6272 6172 7920 696d 706c  ing library impl
-00001fd0: 656d 656e 7465 6420 6279 2061 7373 656d  emented by assem
-00001fe0: 626c 792e 2054 7261 6e73 666f 726d 6572  bly. Transformer
-00001ff0: 732d 6163 6365 6c65 7261 7465 6420 4c69  s-accelerated Li
-00002000: 6272 6172 6965 7320 636f 6e74 6169 6e73  braries contains
-00002010: 2061 204a 4954 2064 6f6d 6169 6e2c 2061   a JIT domain, a
-00002020: 206b 6572 6e65 6c20 646f 6d61 696e 2c20   kernel domain, 
-00002030: 616e 6420 6120 7363 6865 6475 6c69 6e67  and a scheduling
-00002040: 2070 726f 7879 2066 7261 6d65 776f 726b   proxy framework
-00002050: 2e0a 0a60 6060 432b 2b0a 2369 6e63 6c75  ...```C++.#inclu
-00002060: 6465 2022 696e 7465 7266 6163 652e 6870  de "interface.hp
-00002070: 7022 0a20 202e 2e2e 0a20 206f 7065 7261  p".  ....  opera
-00002080: 746f 725f 6465 7363 206f 705f 6465 7363  tor_desc op_desc
-00002090: 286b 6572 5f6b 696e 642c 206b 6572 5f70  (ker_kind, ker_p
-000020a0: 726f 702c 2065 6e67 5f6b 696e 642c 2074  rop, eng_kind, t
-000020b0: 735f 6465 7363 732c 206f 705f 6174 7472  s_descs, op_attr
-000020c0: 7329 3b0a 2020 7370 6172 7365 5f6d 6174  s);.  sparse_mat
-000020d0: 6d75 6c5f 6465 7363 2073 706d 6d5f 6465  mul_desc spmm_de
-000020e0: 7363 286f 705f 6465 7363 293b 0a20 2073  sc(op_desc);.  s
-000020f0: 7061 7273 655f 6d61 746d 756c 2073 706d  parse_matmul spm
-00002100: 6d5f 6b65 726e 2873 706d 6d5f 6465 7363  m_kern(spmm_desc
-00002110: 293b 0a20 2073 7464 3a3a 7665 6374 6f72  );.  std::vector
-00002120: 3c63 6f6e 7374 2076 6f69 642a 3e20 7274  <const void*> rt
-00002130: 5f64 6174 6120 3d20 7b64 6174 6130 2c20  _data = {data0, 
-00002140: 6461 7461 312c 2064 6174 6132 2c20 6461  data1, data2, da
-00002150: 7461 332c 2064 6174 6134 7d3b 0a20 2073  ta3, data4};.  s
-00002160: 706d 6d5f 6b65 726e 2e65 7865 6375 7465  pmm_kern.execute
-00002170: 2872 745f 6461 7461 293b 0a60 6060 0a50  (rt_data);.```.P
-00002180: 6c65 6173 6520 7265 6665 7220 746f 205b  lease refer to [
-00002190: 5472 616e 7366 6f72 6d65 7273 2d61 6363  Transformers-acc
-000021a0: 656c 6572 6174 6564 204c 6962 7261 7269  elerated Librari
-000021b0: 6573 5d28 696e 7465 6c5f 6578 7465 6e73  es](intel_extens
-000021c0: 696f 6e5f 666f 725f 7472 616e 7366 6f72  ion_for_transfor
-000021d0: 6d65 7273 2f62 6163 6b65 6e64 732f 6e65  mers/backends/ne
-000021e0: 7572 616c 5f65 6e67 696e 652f 4b65 726e  ural_engine/Kern
-000021f0: 656c 732f 5245 4144 4d45 2e6d 6429 2066  els/README.md) f
-00002200: 6f72 206d 6f72 6520 6465 7461 696c 732e  or more details.
-00002210: 0a0a 0a23 2320 5379 7374 656d 2052 6571  ...## System Req
-00002220: 7569 7265 6d65 6e74 730a 2323 2320 5661  uirements.### Va
-00002230: 6c69 6461 7465 6420 4861 7264 7761 7265  lidated Hardware
-00002240: 2045 6e76 6972 6f6e 6d65 6e74 0a49 6e74   Environment.Int
-00002250: 656c c2ae 2045 7874 656e 7369 6f6e 2066  el.. Extension f
-00002260: 6f72 2054 7261 6e73 666f 726d 6572 7320  or Transformers 
-00002270: 7375 7070 6f72 7473 2073 7973 7465 6d73  supports systems
-00002280: 2062 6173 6564 206f 6e20 5b49 6e74 656c   based on [Intel
-00002290: 2036 3420 6172 6368 6974 6563 7475 7265   64 architecture
-000022a0: 206f 7220 636f 6d70 6174 6962 6c65 2070   or compatible p
-000022b0: 726f 6365 7373 6f72 735d 2868 7474 7073  rocessors](https
-000022c0: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-000022d0: 6f72 672f 7769 6b69 2f58 3836 2d36 3429  org/wiki/X86-64)
-000022e0: 2074 6861 7420 6172 6520 7370 6563 6966   that are specif
-000022f0: 6963 616c 6c79 206f 7074 696d 697a 6564  ically optimized
-00002300: 2066 6f72 2074 6865 2066 6f6c 6c6f 7769   for the followi
-00002310: 6e67 2043 5055 733a 0a0a 2a20 496e 7465  ng CPUs:..* Inte
-00002320: 6c20 5865 6f6e 2053 6361 6c61 626c 6520  l Xeon Scalable 
-00002330: 7072 6f63 6573 736f 7220 2866 6f72 6d65  processor (forme
-00002340: 726c 7920 4361 7363 6164 6520 4c61 6b65  rly Cascade Lake
-00002350: 2c20 4963 656c 616b 6529 0a2a 2046 7574  , Icelake).* Fut
-00002360: 7572 6520 496e 7465 6c20 5865 6f6e 2053  ure Intel Xeon S
-00002370: 6361 6c61 626c 6520 7072 6f63 6573 736f  calable processo
-00002380: 7220 2863 6f64 6520 6e61 6d65 2053 6170  r (code name Sap
-00002390: 7068 6972 6520 5261 7069 6473 290a 0a23  phire Rapids)..#
-000023a0: 2323 2056 616c 6964 6174 6564 2053 6f66  ## Validated Sof
-000023b0: 7477 6172 6520 456e 7669 726f 6e6d 656e  tware Environmen
-000023c0: 740a 0a2a 204f 5320 7665 7273 696f 6e3a  t..* OS version:
-000023d0: 2043 656e 744f 5320 382e 342c 2055 6275   CentOS 8.4, Ubu
-000023e0: 6e74 7520 3230 2e30 3420 200a 2a20 5079  ntu 20.04  .* Py
-000023f0: 7468 6f6e 2076 6572 7369 6f6e 3a20 332e  thon version: 3.
-00002400: 372c 2033 2e38 2c20 332e 392c 2033 2e31  7, 3.8, 3.9, 3.1
-00002410: 3020 200a 0a3c 7461 626c 6520 636c 6173  0  ..<table clas
-00002420: 733d 2264 6f63 7574 696c 7322 3e0a 3c74  s="docutils">.<t
-00002430: 6865 6164 3e0a 2020 3c74 723e 0a20 2020  head>.  <tr>.   
-00002440: 203c 7468 3e46 7261 6d65 776f 726b 3c2f   <th>Framework</
-00002450: 7468 3e0a 2020 2020 3c74 683e 5465 6e73  th>.    <th>Tens
-00002460: 6f72 466c 6f77 3c2f 7468 3e0a 2020 2020  orFlow</th>.    
-00002470: 3c74 683e 496e 7465 6c20 5465 6e73 6f72  <th>Intel Tensor
-00002480: 466c 6f77 3c2f 7468 3e0a 2020 2020 3c74  Flow</th>.    <t
-00002490: 683e 5079 546f 7263 683c 2f74 683e 0a20  h>PyTorch</th>. 
-000024a0: 2020 203c 7468 3e49 5045 583c 2f74 683e     <th>IPEX</th>
-000024b0: 0a20 203c 2f74 723e 0a3c 2f74 6865 6164  .  </tr>.</thead
-000024c0: 3e0a 3c74 626f 6479 3e0a 2020 3c74 7220  >.<tbody>.  <tr 
-000024d0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-000024e0: 2020 2020 3c74 683e 5665 7273 696f 6e3c      <th>Version<
-000024f0: 2f74 683e 0a20 2020 203c 7464 2063 6c61  /th>.    <td cla
-00002500: 7373 3d22 7467 2d37 7a72 6c22 3e3c 6120  ss="tg-7zrl"><a 
-00002510: 6872 6566 3d68 7474 7073 3a2f 2f67 6974  href=https://git
-00002520: 6875 622e 636f 6d2f 7465 6e73 6f72 666c  hub.com/tensorfl
-00002530: 6f77 2f74 656e 736f 7266 6c6f 772f 7472  ow/tensorflow/tr
-00002540: 6565 2f76 322e 3130 2e30 3e32 2e31 302e  ee/v2.10.0>2.10.
-00002550: 303c 2f61 3e3c 6272 3e0a 2020 2020 3c61  0</a><br>.    <a
-00002560: 2068 7265 663d 6874 7470 733a 2f2f 6769   href=https://gi
-00002570: 7468 7562 2e63 6f6d 2f74 656e 736f 7266  thub.com/tensorf
-00002580: 6c6f 772f 7465 6e73 6f72 666c 6f77 2f74  low/tensorflow/t
-00002590: 7265 652f 7632 2e39 2e31 3e32 2e39 2e31  ree/v2.9.1>2.9.1
-000025a0: 3c2f 613e 3c62 723e 0a20 2020 203c 7464  </a><br>.    <td
-000025b0: 2063 6c61 7373 3d22 7467 2d37 7a72 6c22   class="tg-7zrl"
-000025c0: 3e3c 6120 6872 6566 3d68 7474 7073 3a2f  ><a href=https:/
-000025d0: 2f67 6974 6875 622e 636f 6d2f 496e 7465  /github.com/Inte
-000025e0: 6c2d 7465 6e73 6f72 666c 6f77 2f74 656e  l-tensorflow/ten
-000025f0: 736f 7266 6c6f 772f 7472 6565 2f76 322e  sorflow/tree/v2.
-00002600: 3130 2e30 3e32 2e31 302e 303c 2f61 3e3c  10.0>2.10.0</a><
-00002610: 6272 3e0a 2020 2020 3c61 2068 7265 663d  br>.    <a href=
-00002620: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002630: 6f6d 2f49 6e74 656c 2d74 656e 736f 7266  om/Intel-tensorf
-00002640: 6c6f 772f 7465 6e73 6f72 666c 6f77 2f74  low/tensorflow/t
-00002650: 7265 652f 7632 2e39 2e31 3e32 2e39 2e31  ree/v2.9.1>2.9.1
-00002660: 3c2f 613e 3c62 723e 0a20 2020 203c 7464  </a><br>.    <td
-00002670: 2063 6c61 7373 3d22 7467 2d37 7a72 6c22   class="tg-7zrl"
-00002680: 3e3c 6120 6872 6566 3d68 7474 7073 3a2f  ><a href=https:/
-00002690: 2f64 6f77 6e6c 6f61 642e 7079 746f 7263  /download.pytorc
-000026a0: 682e 6f72 672f 7768 6c2f 746f 7263 685f  h.org/whl/torch_
-000026b0: 7374 6162 6c65 2e68 746d 6c3e 312e 3133  stable.html>1.13
-000026c0: 2e30 2b63 7075 3c2f 613e 3c62 723e 0a20  .0+cpu</a><br>. 
-000026d0: 2020 203c 6120 6872 6566 3d68 7474 7073     <a href=https
-000026e0: 3a2f 2f64 6f77 6e6c 6f61 642e 7079 746f  ://download.pyto
-000026f0: 7263 682e 6f72 672f 7768 6c2f 746f 7263  rch.org/whl/torc
-00002700: 685f 7374 6162 6c65 2e68 746d 6c3e 312e  h_stable.html>1.
-00002710: 3132 2e30 2b63 7075 3c2f 613e 3c62 723e  12.0+cpu</a><br>
-00002720: 0a20 2020 203c 7464 2063 6c61 7373 3d22  .    <td class="
-00002730: 7467 2d37 7a72 6c22 3e3c 6120 6872 6566  tg-7zrl"><a href
-00002740: 3d68 7474 7073 3a2f 2f67 6974 6875 622e  =https://github.
-00002750: 636f 6d2f 696e 7465 6c2f 696e 7465 6c2d  com/intel/intel-
-00002760: 6578 7465 6e73 696f 6e2d 666f 722d 7079  extension-for-py
-00002770: 746f 7263 682f 7472 6565 2f31 2e31 312e  torch/tree/1.11.
-00002780: 303e 312e 3133 2e30 3c2f 613e 3c62 723e  0>1.13.0</a><br>
-00002790: 0a20 2020 203c 6120 6872 6566 3d68 7474  .    <a href=htt
-000027a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000027b0: 696e 7465 6c2f 696e 7465 6c2d 6578 7465  intel/intel-exte
-000027c0: 6e73 696f 6e2d 666f 722d 7079 746f 7263  nsion-for-pytorc
-000027d0: 682f 7472 6565 2f76 312e 3130 2e30 3e31  h/tree/v1.10.0>1
-000027e0: 2e31 322e 303c 2f61 3e3c 2f74 643e 0a20  .12.0</a></td>. 
-000027f0: 203c 2f74 723e 0a3c 2f74 626f 6479 3e0a   </tr>.</tbody>.
-00002800: 3c2f 7461 626c 653e 0a0a 0a23 2320 5365  </table>...## Se
-00002810: 6c65 6374 6564 2050 7562 6c69 6361 7469  lected Publicati
-00002820: 6f6e 732f 4576 656e 7473 0a2a 204e 6575  ons/Events.* Neu
-00002830: 7249 5053 2732 3032 323a 205b 4661 7374  rIPS'2022: [Fast
-00002840: 2044 6973 7469 6c62 6572 7420 6f6e 2043   Distilbert on C
-00002850: 5055 735d 2868 7474 7073 3a2f 2f61 7278  PUs](https://arx
-00002860: 6976 2e6f 7267 2f61 6273 2f32 3231 312e  iv.org/abs/2211.
-00002870: 3037 3731 3529 2028 4e6f 7620 3230 3232  07715) (Nov 2022
-00002880: 290a 2a20 4e65 7572 4950 5327 3230 3232  ).* NeurIPS'2022
-00002890: 3a20 5b51 7561 4c41 2d4d 696e 694c 4d3a  : [QuaLA-MiniLM:
-000028a0: 2061 2051 7561 6e74 697a 6564 204c 656e   a Quantized Len
-000028b0: 6774 6820 4164 6170 7469 7665 204d 696e  gth Adaptive Min
-000028c0: 694c 4d5d 2868 7474 7073 3a2f 2f61 7278  iLM](https://arx
-000028d0: 6976 2e6f 7267 2f61 6273 2f32 3231 302e  iv.org/abs/2210.
-000028e0: 3137 3131 3429 2028 4e6f 7620 3230 3232  17114) (Nov 2022
-000028f0: 290a 2a20 426c 6f67 2070 7562 6c69 7368  ).* Blog publish
-00002900: 6564 2062 7920 416c 6962 6162 613a 205b  ed by Alibaba: [
-00002910: 4465 6570 206c 6561 726e 696e 6720 696e  Deep learning in
-00002920: 6665 7265 6e63 6520 6f70 7469 6d69 7a61  ference optimiza
-00002930: 7469 6f6e 2066 6f72 2041 6464 7265 7373  tion for Address
-00002940: 2050 7572 6966 6963 6174 696f 6e5d 2868   Purification](h
-00002950: 7474 7073 3a2f 2f7a 6875 616e 6c61 6e2e  ttps://zhuanlan.
-00002960: 7a68 6968 752e 636f 6d2f 702f 3535 3234  zhihu.com/p/5524
-00002970: 3834 3431 3329 2028 4175 6720 3230 3232  84413) (Aug 2022
-00002980: 290a 2a20 4e65 7572 4950 5327 3230 3231  ).* NeurIPS'2021
-00002990: 3a20 5b50 7275 6e65 204f 6e63 6520 666f  : [Prune Once fo
-000029a0: 7220 416c 6c3a 2053 7061 7273 6520 5072  r All: Sparse Pr
-000029b0: 652d 5472 6169 6e65 6420 4c61 6e67 7561  e-Trained Langua
-000029c0: 6765 204d 6f64 656c 735d 2868 7474 7073  ge Models](https
-000029d0: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-000029e0: 2f32 3131 312e 3035 3735 3429 2028 4e6f  /2111.05754) (No
-000029f0: 7620 3230 3231 290a                      v 2021).
+00000000: 2320 496e 7465 6cc2 ae20 4578 7465 6e73  # Intel.. Extens
+00000010: 696f 6e20 666f 7220 5472 616e 7366 6f72  ion for Transfor
+00000020: 6d65 7273 3a20 4163 6365 6c65 7261 7469  mers: Accelerati
+00000030: 6e67 2054 7261 6e73 666f 726d 6572 2d62  ng Transformer-b
+00000040: 6173 6564 204d 6f64 656c 7320 6f6e 2049  ased Models on I
+00000050: 6e74 656c 2050 6c61 7466 6f72 6d73 0a49  ntel Platforms.I
+00000060: 6e74 656c c2ae 2045 7874 656e 7369 6f6e  ntel.. Extension
+00000070: 2066 6f72 2054 7261 6e73 666f 726d 6572   for Transformer
+00000080: 7320 6973 2061 6e20 696e 6e6f 7661 7469  s is an innovati
+00000090: 7665 2074 6f6f 6c6b 6974 2074 6f20 6163  ve toolkit to ac
+000000a0: 6365 6c65 7261 7465 2054 7261 6e73 666f  celerate Transfo
+000000b0: 726d 6572 2d62 6173 6564 206d 6f64 656c  rmer-based model
+000000c0: 7320 6f6e 2049 6e74 656c 2070 6c61 7466  s on Intel platf
+000000d0: 6f72 6d73 2e20 5468 6520 746f 6f6c 6b69  orms. The toolki
+000000e0: 7420 6865 6c70 7320 6465 7665 6c6f 7065  t helps develope
+000000f0: 7273 2074 6f20 696d 7072 6f76 6520 7468  rs to improve th
+00000100: 6520 7072 6f64 7563 7469 7669 7479 2074  e productivity t
+00000110: 6872 6f75 6768 2065 6173 652d 6f66 2d75  hrough ease-of-u
+00000120: 7365 206d 6f64 656c 2063 6f6d 7072 6573  se model compres
+00000130: 7369 6f6e 2041 5049 7320 6279 2065 7874  sion APIs by ext
+00000140: 656e 6469 6e67 2048 7567 6769 6e67 2046  ending Hugging F
+00000150: 6163 6520 7472 616e 7366 6f72 6d65 7273  ace transformers
+00000160: 2041 5049 732e 2054 6865 2063 6f6d 7072   APIs. The compr
+00000170: 6573 7369 6f6e 2069 6e66 7261 7374 7275  ession infrastru
+00000180: 6374 7572 6520 6c65 7665 7261 6765 7320  cture leverages 
+00000190: 496e 7465 6cc2 ae20 4e65 7572 616c 2043  Intel.. Neural C
+000001a0: 6f6d 7072 6573 736f 7220 7768 6963 6820  ompressor which 
+000001b0: 7072 6f76 6964 6573 2061 2072 6963 6820  provides a rich 
+000001c0: 7365 7420 6f66 206d 6f64 656c 2063 6f6d  set of model com
+000001d0: 7072 6573 7369 6f6e 2074 6563 686e 6971  pression techniq
+000001e0: 7565 733a 2071 7561 6e74 697a 6174 696f  ues: quantizatio
+000001f0: 6e2c 2070 7275 6e69 6e67 2c20 6469 7374  n, pruning, dist
+00000200: 696c 6c61 7469 6f6e 2061 6e64 2073 6f20  illation and so 
+00000210: 6f6e 2e20 5468 6520 746f 6f6c 6b69 7420  on. The toolkit 
+00000220: 7072 6f76 6964 6573 2054 7261 6e73 666f  provides Transfo
+00000230: 726d 6572 732d 6163 6365 6c65 7261 7465  rmers-accelerate
+00000240: 6420 4c69 6272 6172 6965 7320 616e 6420  d Libraries and 
+00000250: 4e65 7572 616c 2045 6e67 696e 6520 746f  Neural Engine to
+00000260: 2064 656d 6f6e 7374 7261 7465 2074 6865   demonstrate the
+00000270: 2070 6572 666f 726d 616e 6365 206f 6620   performance of 
+00000280: 6578 7472 656d 656c 7920 636f 6d70 7265  extremely compre
+00000290: 7373 6564 206d 6f64 656c 732c 2061 6e64  ssed models, and
+000002a0: 2074 6865 7265 666f 7265 2073 6967 6e69   therefore signi
+000002b0: 6669 6361 6e74 6c79 2069 6d70 726f 7665  ficantly improve
+000002c0: 2074 6865 2069 6e66 6572 656e 6365 2065   the inference e
+000002d0: 6666 6963 6965 6e63 7920 6f6e 2049 6e74  fficiency on Int
+000002e0: 656c 2070 6c61 7466 6f72 6d73 2e20 536f  el platforms. So
+000002f0: 6d65 206f 6620 7468 6520 6b65 7920 6665  me of the key fe
+00000300: 6174 7572 6573 2068 6176 6520 6265 656e  atures have been
+00000310: 2070 7562 6c69 7368 6564 2069 6e20 4e65   published in Ne
+00000320: 7572 4950 5320 3230 3231 2061 6e64 2032  urIPS 2021 and 2
+00000330: 3032 322e 0a0a 2323 2057 6861 7420 646f  022...## What do
+00000340: 6573 2049 6e74 656c c2ae 2045 7874 656e  es Intel.. Exten
+00000350: 7369 6f6e 2066 6f72 2054 7261 6e73 666f  sion for Transfo
+00000360: 726d 6572 7320 6f66 6665 723f 0a54 6869  rmers offer?.Thi
+00000370: 7320 746f 6f6c 6b69 7420 6865 6c70 7320  s toolkit helps 
+00000380: 6465 7665 6c6f 7065 7273 2074 6f20 696d  developers to im
+00000390: 7072 6f76 6520 7468 6520 7072 6f64 7563  prove the produc
+000003a0: 7469 7669 7479 206f 6620 696e 6665 7265  tivity of infere
+000003b0: 6e63 6520 6465 706c 6f79 6d65 6e74 2062  nce deployment b
+000003c0: 7920 6578 7465 6e64 696e 6720 4875 6767  y extending Hugg
+000003d0: 696e 6720 4661 6365 2074 7261 6e73 666f  ing Face transfo
+000003e0: 726d 6572 7320 4150 4973 2066 6f72 2054  rmers APIs for T
+000003f0: 7261 6e73 666f 726d 6572 2d62 6173 6564  ransformer-based
+00000400: 206d 6f64 656c 7320 696e 206e 6174 7572   models in natur
+00000410: 616c 206c 616e 6775 6167 6520 7072 6f63  al language proc
+00000420: 6573 7369 6e67 2028 4e4c 5029 2064 6f6d  essing (NLP) dom
+00000430: 6169 6e2e 2057 6974 6820 6578 7472 656d  ain. With extrem
+00000440: 656c 7920 636f 6d70 7265 7373 6564 206d  ely compressed m
+00000450: 6f64 656c 732c 2074 6865 2074 6f6f 6c6b  odels, the toolk
+00000460: 6974 2063 616e 2067 7265 6174 6c79 2069  it can greatly i
+00000470: 6d70 726f 7665 2074 6865 2069 6e66 6572  mprove the infer
+00000480: 656e 6365 2065 6666 6963 6965 6e63 7920  ence efficiency 
+00000490: 6f6e 2049 6e74 656c 2070 6c61 7466 6f72  on Intel platfor
+000004a0: 6d73 2e0a 0a2d 204d 6f64 656c 2043 6f6d  ms...- Model Com
+000004b0: 7072 6573 7369 6f6e 0a0a 2020 2020 7c46  pression..    |F
+000004c0: 7261 6d65 776f 726b 2020 2020 2020 2020  ramework        
+000004d0: 2020 7c51 7561 6e74 697a 6174 696f 6e20    |Quantization 
+000004e0: 7c50 7275 6e69 6e67 2f53 7061 7273 6974  |Pruning/Sparsit
+000004f0: 7920 7c44 6973 7469 6c6c 6174 696f 6e20  y |Distillation 
+00000500: 7c4e 6575 7261 6c20 4172 6368 6974 6563  |Neural Architec
+00000510: 7475 7265 2053 6561 7263 6820 7c0a 2020  ture Search |.  
+00000520: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
+00000530: 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d  ------|:--------
+00000540: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00000550: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
+00000560: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00000570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+00000580: 7c0a 2020 2020 7c50 7954 6f72 6368 2020  |.    |PyTorch  
+00000590: 2020 2020 2020 2020 2020 7c26 2331 3030            |&#100
+000005a0: 3034 3b20 2020 2020 7c26 2331 3030 3034  04;     |&#10004
+000005b0: 3b20 2020 2020 2020 2020 7c26 2331 3030  ;         |&#100
+000005c0: 3034 3b20 2020 2020 7c26 2331 3030 3034  04;     |&#10004
+000005d0: 3b20 2020 2020 2020 2020 2020 2020 2020  ;               
+000005e0: 2020 2020 7c0a 2020 2020 7c54 656e 736f      |.    |Tenso
+000005f0: 7246 6c6f 7720 2020 2020 2020 2020 7c26  rFlow         |&
+00000600: 2331 3030 3034 3b20 2020 2020 7c26 2331  #10004;     |&#1
+00000610: 3030 3034 3b20 2020 2020 2020 2020 7c26  0004;         |&
+00000620: 2331 3030 3034 3b20 2020 2020 7c53 7461  #10004;     |Sta
+00000630: 7920 7475 6e65 6420 3a73 7461 723a 2020  y tuned :star:  
+00000640: 2020 2020 2020 2020 7c0a 0a2d 2044 6174          |..- Dat
+00000650: 6120 4175 676d 656e 7461 7469 6f6e 2066  a Augmentation f
+00000660: 6f72 204e 4c50 2044 6174 6173 6574 730a  or NLP Datasets.
+00000670: 2d20 5472 616e 7366 6f72 6d65 7273 2d61  - Transformers-a
+00000680: 6363 656c 6572 6174 6564 204e 6575 7261  ccelerated Neura
+00000690: 6c20 456e 6769 6e65 0a2d 2054 7261 6e73  l Engine.- Trans
+000006a0: 666f 726d 6572 732d 6163 6365 6c65 7261  formers-accelera
+000006b0: 7465 6420 4c69 6272 6172 6965 730a 2d20  ted Libraries.- 
+000006c0: 446f 6d61 696e 2041 6c67 6f72 6974 686d  Domain Algorithm
+000006d0: 730a 2020 2020 7c4c 656e 6774 6820 4164  s.    |Length Ad
+000006e0: 6170 7469 7665 2054 7261 6e73 666f 726d  aptive Transform
+000006f0: 6572 207c 0a20 2020 207c 3a2d 2d2d 2d2d  er |.    |:-----
+00000700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000710: 2d2d 2d2d 2d3a 7c0a 2020 2020 7c50 7954  -----:|.    |PyT
+00000720: 6f72 6368 2026 2331 3030 3034 3b20 2020  orch &#10004;   
+00000730: 2020 2020 2020 2020 207c 0a0a 2d20 4172           |..- Ar
+00000740: 6368 6974 6563 7475 7265 206f 6620 496e  chitecture of In
+00000750: 7465 6cc2 ae20 4578 7465 6e73 696f 6e20  tel.. Extension 
+00000760: 666f 7220 5472 616e 7366 6f72 6d65 7273  for Transformers
+00000770: 0a3c 696d 6720 7372 633d 2264 6f63 732f  .<img src="docs/
+00000780: 696d 6773 2f61 7263 682e 706e 6722 2077  imgs/arch.png" w
+00000790: 6964 7468 3d36 3931 2068 6569 6768 743d  idth=691 height=
+000007a0: 3434 3420 616c 743d 2261 7263 6822 3e0a  444 alt="arch">.
+000007b0: 3c2f 6272 3e0a 0a0a 2323 2044 6f63 756d  </br>...## Docum
+000007c0: 656e 7461 7469 6f6e 0a3c 7461 626c 653e  entation.<table>
+000007d0: 0a3c 7468 6561 643e 0a20 203c 7472 3e0a  .<thead>.  <tr>.
+000007e0: 2020 2020 3c74 6820 636f 6c73 7061 6e3d      <th colspan=
+000007f0: 2236 2220 616c 6967 6e3d 2263 656e 7465  "6" align="cente
+00000800: 7222 3e4f 5645 5256 4945 573c 2f74 683e  r">OVERVIEW</th>
+00000810: 0a20 203c 2f74 723e 0a3c 2f74 6865 6164  .  </tr>.</thead
+00000820: 3e0a 3c74 626f 6479 3e0a 2020 3c74 723e  >.<tbody>.  <tr>
+00000830: 0a20 2020 203c 7464 2061 6c69 676e 3d22  .    <td align="
+00000840: 6365 6e74 6572 223e 3c61 2068 7265 663d  center"><a href=
+00000850: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000860: 636f 6d2f 696e 7465 6c2f 696e 7465 6c2d  com/intel/intel-
+00000870: 6578 7465 6e73 696f 6e2d 666f 722d 7472  extension-for-tr
+00000880: 616e 7366 6f72 6d65 7273 2f74 7265 652f  ansformers/tree/
+00000890: 6d61 696e 2f64 6f63 7322 3e4d 6f64 656c  main/docs">Model
+000008a0: 266e 6273 703b 266e 6273 703b 266e 6273  &nbsp;&nbsp;&nbs
+000008b0: 703b 436f 6d70 7265 7373 696f 6e3c 2f61  p;Compression</a
+000008c0: 3e3c 2f74 643e 0a20 2020 203c 7464 2063  ></td>.    <td c
+000008d0: 6f6c 7370 616e 3d22 3222 2061 6c69 676e  olspan="2" align
+000008e0: 3d22 6365 6e74 6572 223e 3c61 2068 7265  ="center"><a hre
+000008f0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000900: 622e 636f 6d2f 696e 7465 6c2f 696e 7465  b.com/intel/inte
+00000910: 6c2d 6578 7465 6e73 696f 6e2d 666f 722d  l-extension-for-
+00000920: 7472 616e 7366 6f72 6d65 7273 2f74 7265  transformers/tre
+00000930: 652f 6d61 696e 2f69 6e74 656c 5f65 7874  e/main/intel_ext
+00000940: 656e 7369 6f6e 5f66 6f72 5f74 7261 6e73  ension_for_trans
+00000950: 666f 726d 6572 732f 6261 636b 656e 6473  formers/backends
+00000960: 2f6e 6575 7261 6c5f 656e 6769 6e65 2f64  /neural_engine/d
+00000970: 6f63 7322 3e54 7261 6e73 666f 726d 6572  ocs">Transformer
+00000980: 732d 6163 6365 6c65 7261 7465 6426 6e62  s-accelerated&nb
+00000990: 7370 3b26 6e62 7370 3b26 6e62 7370 3b4e  sp;&nbsp;&nbsp;N
+000009a0: 6575 7261 6c20 456e 6769 6e65 3c2f 613e  eural Engine</a>
+000009b0: 3c2f 7464 3e0a 2020 2020 3c74 6420 636f  </td>.    <td co
+000009c0: 6c73 7061 6e3d 2232 2220 616c 6967 6e3d  lspan="2" align=
+000009d0: 2263 656e 7465 7222 3e3c 6120 6872 6566  "center"><a href
+000009e0: 3d22 696e 7465 6c5f 6578 7465 6e73 696f  ="intel_extensio
+000009f0: 6e5f 666f 725f 7472 616e 7366 6f72 6d65  n_for_transforme
+00000a00: 7273 2f62 6163 6b65 6e64 732f 6e65 7572  rs/backends/neur
+00000a10: 616c 5f65 6e67 696e 652f 6b65 726e 656c  al_engine/kernel
+00000a20: 732f 5245 4144 4d45 2e6d 6422 3e54 7261  s/README.md">Tra
+00000a30: 6e73 666f 726d 6572 732d 6163 6365 6c65  nsformers-accele
+00000a40: 7261 7465 6426 6e62 7370 3b26 6e62 7370  rated&nbsp;&nbsp
+00000a50: 3b26 6e62 7370 3b4c 6962 7261 7269 6573  ;&nbsp;Libraries
+00000a60: 3c2f 613e 3c2f 7464 3e0a 2020 2020 3c74  </a></td>.    <t
+00000a70: 6420 616c 6967 6e3d 2263 656e 7465 7222  d align="center"
+00000a80: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+00000a90: 2f2f 6769 7468 7562 2e63 6f6d 2f69 6e74  //github.com/int
+00000aa0: 656c 2f69 6e74 656c 2d65 7874 656e 7369  el/intel-extensi
+00000ab0: 6f6e 2d66 6f72 2d74 7261 6e73 666f 726d  on-for-transform
+00000ac0: 6572 732f 7472 6565 2f6d 6169 6e2f 6578  ers/tree/main/ex
+00000ad0: 616d 706c 6573 223e 4578 616d 706c 6573  amples">Examples
+00000ae0: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
+00000af0: 3e0a 2020 3c74 723e 0a20 2020 203c 7468  >.  <tr>.    <th
+00000b00: 2063 6f6c 7370 616e 3d22 3622 2061 6c69   colspan="6" ali
+00000b10: 676e 3d22 6365 6e74 6572 223e 4241 5349  gn="center">BASI
+00000b20: 4320 4150 493c 2f74 683e 0a20 203c 2f74  C API</th>.  </t
+00000b30: 723e 0a20 203c 7472 3e0a 2020 2020 3c74  r>.  <tr>.    <t
+00000b40: 6420 616c 6967 6e3d 2263 656e 7465 7222  d align="center"
+00000b50: 3e3c 6120 6872 6566 3d22 646f 6373 2f65  ><a href="docs/e
+00000b60: 7870 6f72 742e 6d64 223e 4578 706f 7274  xport.md">Export
+00000b70: 3c2f 613e 3c2f 7464 3e0a 2020 2020 3c74  </a></td>.    <t
+00000b80: 6420 616c 6967 6e3d 2263 656e 7465 7222  d align="center"
+00000b90: 3e3c 6120 6872 6566 3d22 646f 6373 2f6d  ><a href="docs/m
+00000ba0: 6574 7269 6373 2e6d 6422 3e4d 6574 7269  etrics.md">Metri
+00000bb0: 633c 2f61 3e3c 2f74 643e 0a20 2020 203c  c</a></td>.    <
+00000bc0: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+00000bd0: 223e 3c61 2068 7265 663d 2264 6f63 732f  "><a href="docs/
+00000be0: 7069 7065 6c69 6e65 2e6d 6422 3e50 6970  pipeline.md">Pip
+00000bf0: 656c 696e 653c 2f61 3e3c 2f74 643e 0a20  eline</a></td>. 
+00000c00: 2020 203c 7464 2061 6c69 676e 3d22 6365     <td align="ce
+00000c10: 6e74 6572 223e 3c61 2068 7265 663d 2264  nter"><a href="d
+00000c20: 6f63 732f 6f62 6a65 6374 6976 6573 2e6d  ocs/objectives.m
+00000c30: 6422 3e4f 626a 6563 7469 7665 3c2f 613e  d">Objective</a>
+00000c40: 3c2f 7464 3e0a 2020 2020 3c74 6420 616c  </td>.    <td al
+00000c50: 6967 6e3d 2263 656e 7465 7222 2063 6f6c  ign="center" col
+00000c60: 7370 616e 3d22 3222 3e3c 6120 6872 6566  span="2"><a href
+00000c70: 3d22 646f 6373 2f64 6174 615f 6175 676d  ="docs/data_augm
+00000c80: 656e 7461 7469 6f6e 2e6d 6422 3e44 6174  entation.md">Dat
+00000c90: 6120 4175 676d 656e 7461 7469 6f6e 3c2f  a Augmentation</
+00000ca0: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
+00000cb0: 2020 3c74 723e 0a20 2020 203c 7464 2063    <tr>.    <td c
+00000cc0: 6f6c 7370 616e 3d22 3222 2061 6c69 676e  olspan="2" align
+00000cd0: 3d22 6365 6e74 6572 223e 3c61 2068 7265  ="center"><a hre
+00000ce0: 663d 2269 6e74 656c 5f65 7874 656e 7369  f="intel_extensi
+00000cf0: 6f6e 5f66 6f72 5f74 7261 6e73 666f 726d  on_for_transform
+00000d00: 6572 732f 6261 636b 656e 6473 2f6e 6575  ers/backends/neu
+00000d10: 7261 6c5f 656e 6769 6e65 2f64 6f63 732f  ral_engine/docs/
+00000d20: 6f6e 6e78 5f63 6f6d 7069 6c65 2e6d 6422  onnx_compile.md"
+00000d30: 3e43 6f6d 7069 6c65 2028 4f4e 4e58 2f54  >Compile (ONNX/T
+00000d40: 656e 736f 7246 6c6f 7729 3c2f 613e 3c2f  ensorFlow)</a></
+00000d50: 7464 3e0a 2020 2020 3c74 6420 636f 6c73  td>.    <td cols
+00000d60: 7061 6e3d 2232 2220 616c 6967 6e3d 2263  pan="2" align="c
+00000d70: 656e 7465 7222 3e3c 6120 6872 6566 3d22  enter"><a href="
+00000d80: 696e 7465 6c5f 6578 7465 6e73 696f 6e5f  intel_extension_
+00000d90: 666f 725f 7472 616e 7366 6f72 6d65 7273  for_transformers
+00000da0: 2f62 6163 6b65 6e64 732f 6e65 7572 616c  /backends/neural
+00000db0: 5f65 6e67 696e 652f 646f 6373 2f44 6570  _engine/docs/Dep
+00000dc0: 6c6f 7920 616e 6420 496e 7465 6772 6174  loy and Integrat
+00000dd0: 696f 6e2e 6d64 223e 4465 706c 6f79 2061  ion.md">Deploy a
+00000de0: 6e64 2049 6e74 6567 7261 7469 6f6e 3c2f  nd Integration</
+00000df0: 613e 3c2f 7464 3e0a 2020 2020 3c74 6420  a></td>.    <td 
+00000e00: 636f 6c73 7061 6e3d 2232 2220 616c 6967  colspan="2" alig
+00000e10: 6e3d 2263 656e 7465 7222 3e3c 6120 6872  n="center"><a hr
+00000e20: 6566 3d22 696e 7465 6c5f 6578 7465 6e73  ef="intel_extens
+00000e30: 696f 6e5f 666f 725f 7472 616e 7366 6f72  ion_for_transfor
+00000e40: 6d65 7273 2f62 6163 6b65 6e64 732f 6e65  mers/backends/ne
+00000e50: 7572 616c 5f65 6e67 696e 652f 646f 6373  ural_engine/docs
+00000e60: 2f61 6464 5f63 7573 746f 6d69 7a65 645f  /add_customized_
+00000e70: 7061 7474 6572 6e2e 6d64 223e 4164 6420  pattern.md">Add 
+00000e80: 4375 7374 6f6d 697a 6520 7061 7474 6572  Customize patter
+00000e90: 6e3c 2f61 3e3c 2f74 643e 0a20 203c 2f74  n</a></td>.  </t
+00000ea0: 723e 0a20 203c 7472 3e0a 2020 2020 3c74  r>.  <tr>.    <t
+00000eb0: 6820 636f 6c73 7061 6e3d 2236 2220 616c  h colspan="6" al
+00000ec0: 6967 6e3d 2263 656e 7465 7222 3e44 4545  ign="center">DEE
+00000ed0: 5020 4449 5645 3c2f 7468 3e0a 2020 3c2f  P DIVE</th>.  </
+00000ee0: 7472 3e0a 2020 3c74 723e 0a20 2020 203c  tr>.  <tr>.    <
+00000ef0: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+00000f00: 223e 3c61 2068 7265 663d 2264 6f63 732f  "><a href="docs/
+00000f10: 7175 616e 7469 7a61 7469 6f6e 2e6d 6422  quantization.md"
+00000f20: 3e51 7561 6e74 697a 6174 696f 6e3c 2f61  >Quantization</a
+00000f30: 3e3c 2f74 643e 0a20 2020 203c 7464 2061  ></td>.    <td a
+00000f40: 6c69 676e 3d22 6365 6e74 6572 223e 3c61  lign="center"><a
+00000f50: 2068 7265 663d 2264 6f63 732f 7072 756e   href="docs/prun
+00000f60: 696e 672e 6d64 223e 5072 756e 696e 673c  ing.md">Pruning<
+00000f70: 2f61 3e3c 2f74 643e 0a20 2020 203c 7464  /a></td>.    <td
+00000f80: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
+00000f90: 636f 6c73 7061 6e3d 2232 223e 3c61 2068  colspan="2"><a h
+00000fa0: 7265 663d 2264 6f63 732f 6469 7374 696c  ref="docs/distil
+00000fb0: 6c61 7469 6f6e 2e6d 6422 3e44 6973 7469  lation.md">Disti
+00000fc0: 6c6c 6174 696f 6e3c 2f61 3e3c 2f74 643e  llation</a></td>
+00000fd0: 0a20 2020 203c 7464 2061 6c69 676e 3d22  .    <td align="
+00000fe0: 6365 6e74 6572 2220 636f 6c73 7061 6e3d  center" colspan=
+00000ff0: 2232 223e 3c61 2068 7265 663d 2268 7474  "2"><a href="htt
+00001000: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001010: 696e 7465 6c2f 696e 7465 6c2d 6578 7465  intel/intel-exte
+00001020: 6e73 696f 6e2d 666f 722d 7472 616e 7366  nsion-for-transf
+00001030: 6f72 6d65 7273 2f62 6c6f 622f 6d61 696e  ormers/blob/main
+00001040: 2f65 7861 6d70 6c65 732f 6f70 7469 6d69  /examples/optimi
+00001050: 7a61 7469 6f6e 2f70 7974 6f72 6368 2f68  zation/pytorch/h
+00001060: 7567 6769 6e67 6661 6365 2f74 6578 742d  uggingface/text-
+00001070: 636c 6173 7369 6669 6361 7469 6f6e 2f6f  classification/o
+00001080: 7263 6865 7374 7261 7465 5f6f 7074 696d  rchestrate_optim
+00001090: 697a 6174 696f 6e73 2f52 4541 444d 452e  izations/README.
+000010a0: 6d64 223e 4f72 6368 6573 7472 6174 696f  md">Orchestratio
+000010b0: 6e3c 2f61 3e3c 2f74 643e 0a20 203c 2f74  n</a></td>.  </t
+000010c0: 723e 0a20 203c 7472 3e0a 2020 2020 3c74  r>.  <tr>.    <t
+000010d0: 6420 616c 6967 6e3d 2263 656e 7465 7222  d align="center"
+000010e0: 2063 6f6c 7370 616e 3d22 3322 3e3c 6120   colspan="3"><a 
+000010f0: 6872 6566 3d22 696e 7465 6c5f 6578 7465  href="intel_exte
+00001100: 6e73 696f 6e5f 666f 725f 7472 616e 7366  nsion_for_transf
+00001110: 6f72 6d65 7273 2f62 6163 6b65 6e64 732f  ormers/backends/
+00001120: 6e65 7572 616c 5f65 6e67 696e 6522 3e54  neural_engine">T
+00001130: 7261 6e73 666f 726d 6572 732d 6163 6365  ransformers-acce
+00001140: 6c65 7261 7465 6426 6e62 7370 3b4e 6575  lerated&nbsp;Neu
+00001150: 7261 6c20 456e 6769 6e65 3c2f 613e 3c2f  ral Engine</a></
+00001160: 7464 3e0a 2020 2020 3c74 6420 616c 6967  td>.    <td alig
+00001170: 6e3d 2263 656e 7465 7222 2063 6f6c 7370  n="center" colsp
+00001180: 616e 3d22 3322 3e3c 6120 6872 6566 3d22  an="3"><a href="
+00001190: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000011a0: 6f6d 2f69 6e74 656c 2f69 6e74 656c 2d65  om/intel/intel-e
+000011b0: 7874 656e 7369 6f6e 2d66 6f72 2d74 7261  xtension-for-tra
+000011c0: 6e73 666f 726d 6572 732f 7472 6565 2f6d  nsformers/tree/m
+000011d0: 6169 6e2f 696e 7465 6c5f 6578 7465 6e73  ain/intel_extens
+000011e0: 696f 6e5f 666f 725f 7472 616e 7366 6f72  ion_for_transfor
+000011f0: 6d65 7273 2f62 6163 6b65 6e64 732f 6e65  mers/backends/ne
+00001200: 7572 616c 5f65 6e67 696e 652f 6b65 726e  ural_engine/kern
+00001210: 656c 732f 646f 6373 2f6b 6572 6e65 6c5f  els/docs/kernel_
+00001220: 6465 7363 223e 4b65 726e 656c 7320 2841  desc">Kernels (A
+00001230: 4d58 2f41 5658 2f56 4e4e 4929 3c2f 613e  MX/AVX/VNNI)</a>
+00001240: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
+00001250: 3c74 723e 0a20 2020 203c 7468 2063 6f6c  <tr>.    <th col
+00001260: 7370 616e 3d22 3622 2061 6c69 676e 3d22  span="6" align="
+00001270: 6365 6e74 6572 223e 4144 5641 4e43 4544  center">ADVANCED
+00001280: 2041 4c47 4f52 4954 484d 3c2f 7468 3e0a   ALGORITHM</th>.
+00001290: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
+000012a0: 2020 203c 7464 2061 6c69 676e 3d22 6365     <td align="ce
+000012b0: 6e74 6572 2220 636f 6c73 7061 6e3d 2232  nter" colspan="2
+000012c0: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+000012d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 696e  ://github.com/in
+000012e0: 7465 6c2f 696e 7465 6c2d 6578 7465 6e73  tel/intel-extens
+000012f0: 696f 6e2d 666f 722d 7472 616e 7366 6f72  ion-for-transfor
+00001300: 6d65 7273 2f62 6c6f 622f 6d61 696e 2f65  mers/blob/main/e
+00001310: 7861 6d70 6c65 732f 6f70 7469 6d69 7a61  xamples/optimiza
+00001320: 7469 6f6e 2f70 7974 6f72 6368 2f68 7567  tion/pytorch/hug
+00001330: 6769 6e67 6661 6365 2f71 7565 7374 696f  gingface/questio
+00001340: 6e2d 616e 7377 6572 696e 672f 6479 6e61  n-answering/dyna
+00001350: 6d69 632f 5245 4144 4d45 2e6d 6422 3e4c  mic/README.md">L
+00001360: 656e 6774 6820 4164 6170 7469 7665 3c2f  ength Adaptive</
+00001370: 613e 3c2f 7464 3e0a 2020 2020 3c74 6420  a></td>.    <td 
+00001380: 616c 6967 6e3d 2263 656e 7465 7222 2063  align="center" c
+00001390: 6f6c 7370 616e 3d22 3222 3e3c 6120 6872  olspan="2"><a hr
+000013a0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000013b0: 7562 2e63 6f6d 2f69 6e74 656c 2f69 6e74  ub.com/intel/int
+000013c0: 656c 2d65 7874 656e 7369 6f6e 2d66 6f72  el-extension-for
+000013d0: 2d74 7261 6e73 666f 726d 6572 732f 7472  -transformers/tr
+000013e0: 6565 2f6d 6169 6e2f 6578 616d 706c 6573  ee/main/examples
+000013f0: 2f6f 7074 696d 697a 6174 696f 6e2f 7079  /optimization/py
+00001400: 746f 7263 682f 6875 6767 696e 6766 6163  torch/huggingfac
+00001410: 652f 6c61 6e67 7561 6765 2d6d 6f64 656c  e/language-model
+00001420: 696e 672f 6175 746f 5f64 6973 7469 6c6c  ing/auto_distill
+00001430: 6174 696f 6e22 3e4e 4153 2028 4175 746f  ation">NAS (Auto
+00001440: 2044 6973 7469 6c6c 6174 696f 6e29 3c2f   Distillation)</
+00001450: 613e 3c2f 7464 3e0a 2020 2020 3c74 6420  a></td>.    <td 
+00001460: 616c 6967 6e3d 2263 656e 7465 7222 2063  align="center" c
+00001470: 6f6c 7370 616e 3d22 3222 3e3c 6120 6872  olspan="2"><a hr
+00001480: 6566 3d22 223e 5365 7420 4669 743c 2f61  ef="">Set Fit</a
+00001490: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
+000014a0: 203c 7472 3e0a 2020 2020 3c74 6820 636f   <tr>.    <th co
+000014b0: 6c73 7061 6e3d 2233 2220 616c 6967 6e3d  lspan="3" align=
+000014c0: 2263 656e 7465 7222 3e50 524f 4649 4c49  "center">PROFILI
+000014d0: 4e47 2041 4e44 2042 454e 4348 4d41 524b  NG AND BENCHMARK
+000014e0: 3c2f 613e 3c2f 7468 3e0a 2020 2020 3c74  </a></th>.    <t
+000014f0: 6820 636f 6c73 7061 6e3d 2233 2220 616c  h colspan="3" al
+00001500: 6967 6e3d 2263 656e 7465 7222 3e56 414c  ign="center">VAL
+00001510: 4944 4154 4544 204d 4f44 454c 5320 414e  IDATED MODELS AN
+00001520: 4420 4441 5441 3c2f 7468 3e0a 2020 3c2f  D DATA</th>.  </
+00001530: 7472 3e0a 2020 3c74 723e 0a20 2020 203c  tr>.  <tr>.    <
+00001540: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+00001550: 223e 3c61 2068 7265 663d 2264 6f63 732f  "><a href="docs/
+00001560: 6265 6e63 686d 6172 6b2e 6d64 223e 4d6f  benchmark.md">Mo
+00001570: 6465 6c20 436f 6d70 7265 7373 696f 6e3c  del Compression<
+00001580: 2f61 3e3c 2f74 643e 0a20 2020 203c 7464  /a></td>.    <td
+00001590: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000015a0: 3c61 2068 7265 663d 2269 6e74 656c 5f65  <a href="intel_e
+000015b0: 7874 656e 7369 6f6e 5f66 6f72 5f74 7261  xtension_for_tra
+000015c0: 6e73 666f 726d 6572 732f 6261 636b 656e  nsformers/backen
+000015d0: 6473 2f6e 6575 7261 6c5f 656e 6769 6e65  ds/neural_engine
+000015e0: 2f64 6f63 732f 7072 6f66 696c 696e 672e  /docs/profiling.
+000015f0: 6d64 223e 5472 616e 7366 6f72 6d65 7273  md">Transformers
+00001600: 2d61 6363 656c 6572 6174 6564 266e 6273  -accelerated&nbs
+00001610: 703b 4e65 7572 616c 2045 6e67 696e 653c  p;Neural Engine<
+00001620: 2f61 3e3c 2f74 643e 0a20 2020 203c 7464  /a></td>.    <td
+00001630: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00001640: 5472 616e 7366 6f72 6d65 7273 2d61 6363  Transformers-acc
+00001650: 656c 6572 6174 6564 266e 6273 703b 4c69  elerated&nbsp;Li
+00001660: 6272 6172 6965 7320 3c61 2068 7265 663d  braries <a href=
+00001670: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00001680: 636f 6d2f 696e 7465 6c2f 696e 7465 6c2d  com/intel/intel-
+00001690: 6578 7465 6e73 696f 6e2d 666f 722d 7472  extension-for-tr
+000016a0: 616e 7366 6f72 6d65 7273 2f74 7265 652f  ansformers/tree/
+000016b0: 6d61 696e 2f20 2069 6e74 656c 5f65 7874  main/  intel_ext
+000016c0: 656e 7369 6f6e 5f66 6f72 5f74 7261 6e73  ension_for_trans
+000016d0: 666f 726d 6572 732f 6261 636b 656e 6473  formers/backends
+000016e0: 2f6e 6575 7261 6c5f 656e 6769 6e65 2f6b  /neural_engine/k
+000016f0: 6572 6e65 6c73 2f64 6f63 732f 223e 5072  ernels/docs/">Pr
+00001700: 6f66 696c 696e 673c 2f61 3e2f 203c 6120  ofiling</a>/ <a 
+00001710: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001720: 7468 7562 2e63 6f6d 2f69 6e74 656c 2f69  thub.com/intel/i
+00001730: 6e74 656c 2d65 7874 656e 7369 6f6e 2d66  ntel-extension-f
+00001740: 6f72 2d74 7261 6e73 666f 726d 6572 732f  or-transformers/
+00001750: 7472 6565 2f6d 6169 6e2f 2020 696e 7465  tree/main/  inte
+00001760: 6c5f 6578 7465 6e73 696f 6e5f 666f 725f  l_extension_for_
+00001770: 7472 616e 7366 6f72 6d65 7273 2f62 6163  transformers/bac
+00001780: 6b65 6e64 732f 6e65 7572 616c 5f65 6e67  kends/neural_eng
+00001790: 696e 652f 6b65 726e 656c 732f 646f 6373  ine/kernels/docs
+000017a0: 2f22 3e42 656e 6368 6d61 726b 3c2f 2020  /">Benchmark</  
+000017b0: 613e 3c2f 7464 3e0a 2020 2020 3c74 6420  a></td>.    <td 
+000017c0: 616c 6967 6e3d 2263 656e 7465 7222 3e3c  align="center"><
+000017d0: 6120 6872 6566 3d22 646f 6373 2f65 7861  a href="docs/exa
+000017e0: 6d70 6c65 732e 6d64 223e 5375 7070 6f72  mples.md">Suppor
+000017f0: 7465 6420 4d6f 6465 6c73 3c2f 613e 3c2f  ted Models</a></
+00001800: 7464 3e0a 2020 2020 3c74 6420 616c 6967  td>.    <td alig
+00001810: 6e3d 2263 656e 7465 7222 3e3c 6120 6872  n="center"><a hr
+00001820: 6566 3d22 696e 7465 6c5f 6578 7465 6e73  ef="intel_extens
+00001830: 696f 6e5f 666f 725f 7472 616e 7366 6f72  ion_for_transfor
+00001840: 6d65 7273 2f62 6163 6b65 6e64 732f 6e65  mers/backends/ne
+00001850: 7572 616c 5f65 6e67 696e 652f 646f 6373  ural_engine/docs
+00001860: 2f76 616c 6964 6174 6564 5f6d 6f64 656c  /validated_model
+00001870: 2e6d 6422 3e53 7061 7273 6520 4177 6172  .md">Sparse Awar
+00001880: 6520 496e 6665 7265 6e63 653c 2f61 3e3c  e Inference</a><
+00001890: 2f74 643e 0a20 2020 203c 7464 2061 6c69  /td>.    <td ali
+000018a0: 676e 3d22 6365 6e74 6572 223e 3c61 2068  gn="center"><a h
+000018b0: 7265 663d 2269 6e74 656c 5f65 7874 656e  ref="intel_exten
+000018c0: 7369 6f6e 5f66 6f72 5f74 7261 6e73 666f  sion_for_transfo
+000018d0: 726d 6572 732f 6261 636b 656e 6473 2f6e  rmers/backends/n
+000018e0: 6575 7261 6c5f 656e 6769 6e65 2f6b 6572  eural_engine/ker
+000018f0: 6e65 6c73 2f64 6f63 732f 7661 6c69 6461  nels/docs/valida
+00001900: 7465 645f 6461 7461 2e6d 6422 3e53 7061  ted_data.md">Spa
+00001910: 7273 6520 4b65 726e 656c 2044 6174 613c  rse Kernel Data<
+00001920: 2f61 3e3c 2f74 643e 0a20 203c 2f74 723e  /a></td>.  </tr>
+00001930: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
+00001940: 636f 6c73 7061 6e3d 2236 2220 616c 6967  colspan="6" alig
+00001950: 6e3d 2263 656e 7465 7222 3e3c 6120 6872  n="center"><a hr
+00001960: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001970: 7562 2e63 6f6d 2f69 6e74 656c 2f69 6e74  ub.com/intel/int
+00001980: 656c 2d65 7874 656e 7369 6f6e 2d66 6f72  el-extension-for
+00001990: 2d74 7261 6e73 666f 726d 6572 732f 7472  -transformers/tr
+000019a0: 6565 2f6d 6169 6e2f 646f 6373 2f74 7574  ee/main/docs/tut
+000019b0: 6f72 6961 6c73 2f70 7974 6f72 6368 223e  orials/pytorch">
+000019c0: 5455 544f 5249 414c 533c 2f61 3e3c 2f74  TUTORIALS</a></t
+000019d0: 643e 0a20 203c 2f74 723e 0a3c 2f74 626f  d>.  </tr>.</tbo
+000019e0: 6479 3e0a 3c2f 7461 626c 653e 0a0a 0a23  dy>.</table>...#
+000019f0: 2320 496e 7374 616c 6c61 7469 6f6e 0a23  # Installation.#
+00001a00: 2323 2052 656c 6561 7365 2042 696e 6172  ## Release Binar
+00001a10: 7920 496e 7374 616c 6c0a 6060 6062 6173  y Install.```bas
+00001a20: 680a 7069 7020 696e 7374 616c 6c20 696e  h.pip install in
+00001a30: 7465 6c2d 6578 7465 6e73 696f 6e2d 666f  tel-extension-fo
+00001a40: 722d 7472 616e 7366 6f72 6d65 7273 0a60  r-transformers.`
+00001a50: 6060 0a0a 2323 2320 496e 7374 616c 6c20  ``..### Install 
+00001a60: 4672 6f6d 2053 6f75 7263 650a 2323 2323  From Source.####
+00001a70: 2049 6e73 7461 6c6c 2049 6e74 656c c2ae   Install Intel..
+00001a80: 2045 7874 656e 7369 6f6e 2066 6f72 2054   Extension for T
+00001a90: 7261 6e73 666f 726d 6572 730a 6060 6062  ransformers.```b
+00001aa0: 6173 680a 6769 7420 636c 6f6e 6520 6874  ash.git clone ht
+00001ab0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001ac0: 2f69 6e74 656c 2f69 6e74 656c 2d65 7874  /intel/intel-ext
+00001ad0: 656e 7369 6f6e 2d66 6f72 2d74 7261 6e73  ension-for-trans
+00001ae0: 666f 726d 6572 732e 6769 7420 696e 7465  formers.git inte
+00001af0: 6c5f 6578 7465 6e73 696f 6e5f 666f 725f  l_extension_for_
+00001b00: 7472 616e 7366 6f72 6d65 7273 0a63 6420  transformers.cd 
+00001b10: 696e 7465 6c5f 6578 7465 6e73 696f 6e5f  intel_extension_
+00001b20: 666f 725f 7472 616e 7366 6f72 6d65 7273  for_transformers
+00001b30: 0a23 2049 6e73 7461 6c6c 2044 6570 656e  .# Install Depen
+00001b40: 6465 6e63 790a 7069 7020 696e 7374 616c  dency.pip instal
+00001b50: 6c20 2d72 2072 6571 7569 7265 6d65 6e74  l -r requirement
+00001b60: 732e 7478 740a 6769 7420 7375 626d 6f64  s.txt.git submod
+00001b70: 756c 6520 7570 6461 7465 202d 2d69 6e69  ule update --ini
+00001b80: 7420 2d2d 7265 6375 7273 6976 650a 2320  t --recursive.# 
+00001b90: 496e 7374 616c 6c20 696e 7465 6c5f 6578  Install intel_ex
+00001ba0: 7465 6e73 696f 6e5f 666f 725f 7472 616e  tension_for_tran
+00001bb0: 7366 6f72 6d65 7273 0a70 7974 686f 6e20  sformers.python 
+00001bc0: 7365 7475 702e 7079 2069 6e73 7461 6c6c  setup.py install
+00001bd0: 0a60 6060 0a0a 2323 2047 6574 7469 6e67  .```..## Getting
+00001be0: 2053 7461 7274 6564 0a23 2323 2051 7561   Started.### Qua
+00001bf0: 6e74 697a 6174 696f 6e0a 6060 6070 7974  ntization.```pyt
+00001c00: 686f 6e0a 6672 6f6d 2069 6e74 656c 5f65  hon.from intel_e
+00001c10: 7874 656e 7369 6f6e 5f66 6f72 5f74 7261  xtension_for_tra
+00001c20: 6e73 666f 726d 6572 7320 696d 706f 7274  nsformers import
+00001c30: 2051 7561 6e74 697a 6174 696f 6e43 6f6e   QuantizationCon
+00001c40: 6669 672c 206d 6574 7269 632c 206f 626a  fig, metric, obj
+00001c50: 6563 7469 7665 730a 6672 6f6d 2069 6e74  ectives.from int
+00001c60: 656c 5f65 7874 656e 7369 6f6e 5f66 6f72  el_extension_for
+00001c70: 5f74 7261 6e73 666f 726d 6572 732e 6f70  _transformers.op
+00001c80: 7469 6d69 7a61 7469 6f6e 2e74 7261 696e  timization.train
+00001c90: 6572 2069 6d70 6f72 7420 4e4c 5054 7261  er import NLPTra
+00001ca0: 696e 6572 0a0a 2320 5265 706c 6163 6520  iner..# Replace 
+00001cb0: 7472 616e 7366 6f72 6d65 7273 2e54 7261  transformers.Tra
+00001cc0: 696e 6572 2077 6974 6820 4e4c 5054 7261  iner with NLPTra
+00001cd0: 696e 6572 0a23 2074 7261 696e 6572 203d  iner.# trainer =
+00001ce0: 2074 7261 6e73 666f 726d 6572 732e 5472   transformers.Tr
+00001cf0: 6169 6e65 7228 2e2e 2e29 0a74 7261 696e  ainer(...).train
+00001d00: 6572 203d 204e 4c50 5472 6169 6e65 7228  er = NLPTrainer(
+00001d10: 2e2e 2e29 0a6d 6574 7269 6320 3d20 6d65  ...).metric = me
+00001d20: 7472 6963 732e 4d65 7472 6963 286e 616d  trics.Metric(nam
+00001d30: 653d 2265 7661 6c5f 6631 222c 2069 735f  e="eval_f1", is_
+00001d40: 7265 6c61 7469 7665 3d54 7275 652c 2063  relative=True, c
+00001d50: 7269 7465 7269 6f6e 3d30 2e30 3129 0a71  riterion=0.01).q
+00001d60: 5f63 6f6e 6669 6720 3d20 5175 616e 7469  _config = Quanti
+00001d70: 7a61 7469 6f6e 436f 6e66 6967 280a 2020  zationConfig(.  
+00001d80: 2020 6170 7072 6f61 6368 3d22 506f 7374    approach="Post
+00001d90: 5472 6169 6e69 6e67 5374 6174 6963 222c  TrainingStatic",
+00001da0: 0a20 2020 206d 6574 7269 6373 3d5b 6d65  .    metrics=[me
+00001db0: 7472 6963 5d2c 0a20 2020 206f 626a 6563  tric],.    objec
+00001dc0: 7469 7665 733d 5b6f 626a 6563 7469 7665  tives=[objective
+00001dd0: 732e 7065 7266 6f72 6d61 6e63 655d 0a29  s.performance].)
+00001de0: 0a6d 6f64 656c 203d 2074 7261 696e 6572  .model = trainer
+00001df0: 2e71 7561 6e74 697a 6528 7175 616e 745f  .quantize(quant_
+00001e00: 636f 6e66 6967 3d71 5f63 6f6e 6669 6729  config=q_config)
+00001e10: 0a60 6060 0a0a 506c 6561 7365 2072 6566  .```..Please ref
+00001e20: 6572 2074 6f20 5b71 7561 6e74 697a 6174  er to [quantizat
+00001e30: 696f 6e20 646f 6375 6d65 6e74 5d28 646f  ion document](do
+00001e40: 6373 2f71 7561 6e74 697a 6174 696f 6e2e  cs/quantization.
+00001e50: 6d64 2920 666f 7220 6d6f 7265 2064 6574  md) for more det
+00001e60: 6169 6c73 2e0a 0a23 2323 2050 7275 6e69  ails...### Pruni
+00001e70: 6e67 0a60 6060 7079 7468 6f6e 0a66 726f  ng.```python.fro
+00001e80: 6d20 696e 7465 6c5f 6578 7465 6e73 696f  m intel_extensio
+00001e90: 6e5f 666f 725f 7472 616e 7366 6f72 6d65  n_for_transforme
+00001ea0: 7273 2069 6d70 6f72 7420 5072 756e 6572  rs import Pruner
+00001eb0: 436f 6e66 6967 2c20 5072 756e 696e 6743  Config, PruningC
+00001ec0: 6f6e 6669 670a 6672 6f6d 2069 6e74 656c  onfig.from intel
+00001ed0: 5f65 7874 656e 7369 6f6e 5f66 6f72 5f74  _extension_for_t
+00001ee0: 7261 6e73 666f 726d 6572 732e 6f70 7469  ransformers.opti
+00001ef0: 6d69 7a61 7469 6f6e 2e74 7261 696e 6572  mization.trainer
+00001f00: 2069 6d70 6f72 7420 4e4c 5054 7261 696e   import NLPTrain
+00001f10: 6572 0a0a 2320 5265 706c 6163 6520 7472  er..# Replace tr
+00001f20: 616e 7366 6f72 6d65 7273 2e54 7261 696e  ansformers.Train
+00001f30: 6572 2077 6974 6820 4e4c 5054 7261 696e  er with NLPTrain
+00001f40: 6572 0a23 2074 7261 696e 6572 203d 2074  er.# trainer = t
+00001f50: 7261 6e73 666f 726d 6572 732e 5472 6169  ransformers.Trai
+00001f60: 6e65 7228 2e2e 2e29 0a74 7261 696e 6572  ner(...).trainer
+00001f70: 203d 204e 4c50 5472 6169 6e65 7228 2e2e   = NLPTrainer(..
+00001f80: 2e29 0a6d 6574 7269 6320 3d20 6d65 7472  .).metric = metr
+00001f90: 6963 732e 4d65 7472 6963 286e 616d 653d  ics.Metric(name=
+00001fa0: 2265 7661 6c5f 6163 6375 7261 6379 2229  "eval_accuracy")
+00001fb0: 0a70 7275 6e65 725f 636f 6e66 6967 203d  .pruner_config =
+00001fc0: 2050 7275 6e65 7243 6f6e 6669 6728 7072   PrunerConfig(pr
+00001fd0: 756e 655f 7479 7065 3d27 4261 7369 634d  une_type='BasicM
+00001fe0: 6167 6e69 7475 6465 272c 2074 6172 6765  agnitude', targe
+00001ff0: 745f 7370 6172 7369 7479 5f72 6174 696f  t_sparsity_ratio
+00002000: 3d30 2e39 290a 705f 636f 6e66 203d 2050  =0.9).p_conf = P
+00002010: 7275 6e69 6e67 436f 6e66 6967 2870 7275  runingConfig(pru
+00002020: 6e65 725f 636f 6e66 6967 3d5b 7072 756e  ner_config=[prun
+00002030: 6572 5f63 6f6e 6669 675d 2c20 6d65 7472  er_config], metr
+00002040: 6963 733d 6d65 7472 6963 290a 6d6f 6465  ics=metric).mode
+00002050: 6c20 3d20 7472 6169 6e65 722e 7072 756e  l = trainer.prun
+00002060: 6528 7072 756e 696e 675f 636f 6e66 6967  e(pruning_config
+00002070: 3d70 5f63 6f6e 6629 0a60 6060 0a0a 506c  =p_conf).```..Pl
+00002080: 6561 7365 2072 6566 6572 2074 6f20 5b70  ease refer to [p
+00002090: 7275 6e69 6e67 2064 6f63 756d 656e 745d  runing document]
+000020a0: 2864 6f63 732f 7072 756e 696e 672e 6d64  (docs/pruning.md
+000020b0: 2920 666f 7220 6d6f 7265 2064 6574 6169  ) for more detai
+000020c0: 6c73 2e0a 0a23 2323 2044 6973 7469 6c6c  ls...### Distill
+000020d0: 6174 696f 6e0a 6060 6070 7974 686f 6e0a  ation.```python.
+000020e0: 6672 6f6d 2069 6e74 656c 5f65 7874 656e  from intel_exten
+000020f0: 7369 6f6e 5f66 6f72 5f74 7261 6e73 666f  sion_for_transfo
+00002100: 726d 6572 7320 696d 706f 7274 2044 6973  rmers import Dis
+00002110: 7469 6c6c 6174 696f 6e43 6f6e 6669 672c  tillationConfig,
+00002120: 2043 7269 7465 7269 6f6e 0a66 726f 6d20   Criterion.from 
+00002130: 696e 7465 6c5f 6578 7465 6e73 696f 6e5f  intel_extension_
+00002140: 666f 725f 7472 616e 7366 6f72 6d65 7273  for_transformers
+00002150: 2e6f 7074 696d 697a 6174 696f 6e2e 7472  .optimization.tr
+00002160: 6169 6e65 7220 696d 706f 7274 204e 4c50  ainer import NLP
+00002170: 5472 6169 6e65 720a 0a23 2052 6570 6c61  Trainer..# Repla
+00002180: 6365 2074 7261 6e73 666f 726d 6572 732e  ce transformers.
+00002190: 5472 6169 6e65 7220 7769 7468 204e 4c50  Trainer with NLP
+000021a0: 5472 6169 6e65 720a 2320 7472 6169 6e65  Trainer.# traine
+000021b0: 7220 3d20 7472 616e 7366 6f72 6d65 7273  r = transformers
+000021c0: 2e54 7261 696e 6572 282e 2e2e 290a 7465  .Trainer(...).te
+000021d0: 6163 6865 725f 6d6f 6465 6c20 3d20 2e2e  acher_model = ..
+000021e0: 2e20 2320 6578 6973 7420 6d6f 6465 6c0a  . # exist model.
+000021f0: 7472 6169 6e65 7220 3d20 4e4c 5054 7261  trainer = NLPTra
+00002200: 696e 6572 282e 2e2e 290a 6d65 7472 6963  iner(...).metric
+00002210: 203d 206d 6574 7269 6373 2e4d 6574 7269   = metrics.Metri
+00002220: 6328 6e61 6d65 3d22 6576 616c 5f61 6363  c(name="eval_acc
+00002230: 7572 6163 7922 290a 645f 636f 6e66 203d  uracy").d_conf =
+00002240: 2044 6973 7469 6c6c 6174 696f 6e43 6f6e   DistillationCon
+00002250: 6669 6728 6d65 7472 6963 733d 6d65 7472  fig(metrics=metr
+00002260: 6963 290a 6d6f 6465 6c20 3d20 7472 6169  ic).model = trai
+00002270: 6e65 722e 6469 7374 696c 6c28 6469 7374  ner.distill(dist
+00002280: 696c 6c61 7469 6f6e 5f63 6f6e 6669 673d  illation_config=
+00002290: 645f 636f 6e66 2c20 7465 6163 6865 725f  d_conf, teacher_
+000022a0: 6d6f 6465 6c3d 7465 6163 6865 725f 6d6f  model=teacher_mo
+000022b0: 6465 6c29 0a60 6060 0a0a 506c 6561 7365  del).```..Please
+000022c0: 2072 6566 6572 2074 6f20 5b64 6973 7469   refer to [disti
+000022d0: 6c6c 6174 696f 6e20 646f 6375 6d65 6e74  llation document
+000022e0: 5d28 646f 6373 2f64 6973 7469 6c6c 6174  ](docs/distillat
+000022f0: 696f 6e2e 6d64 2920 666f 7220 6d6f 7265  ion.md) for more
+00002300: 2064 6574 6169 6c73 2e0a 0a23 2323 2044   details...### D
+00002310: 6174 6120 4175 676d 656e 7461 7469 6f6e  ata Augmentation
+00002320: 0a44 6174 6120 6175 676d 656e 7461 7469  .Data augmentati
+00002330: 6f6e 2070 726f 7669 6465 7320 7468 6520  on provides the 
+00002340: 6661 6369 6c69 7469 6573 2074 6f20 6765  facilities to ge
+00002350: 6e65 7261 7465 2073 796e 7468 6573 697a  nerate synthesiz
+00002360: 6564 204e 4c50 2064 6174 6173 6574 2066  ed NLP dataset f
+00002370: 6f72 2066 7572 7468 6572 206d 6f64 656c  or further model
+00002380: 206f 7074 696d 697a 6174 696f 6e2e 2054   optimization. T
+00002390: 6865 2064 6174 6120 6175 676d 656e 7461  he data augmenta
+000023a0: 7469 6f6e 2073 7570 706f 7274 7320 7465  tion supports te
+000023b0: 7874 2067 656e 6572 6174 696f 6e20 6f6e  xt generation on
+000023c0: 2070 6f70 756c 6172 2066 696e 652d 7475   popular fine-tu
+000023d0: 6e65 6420 6d6f 6465 6c73 206c 696b 6520  ned models like 
+000023e0: 4750 542c 2047 5054 322c 2061 6e64 206f  GPT, GPT2, and o
+000023f0: 7468 6572 2074 6578 7420 7379 6e74 6865  ther text synthe
+00002400: 7369 7320 6170 7072 6f61 6368 6573 2066  sis approaches f
+00002410: 726f 6d20 5b6e 6c70 6175 675d 2868 7474  rom [nlpaug](htt
+00002420: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002430: 6d61 6b63 6564 7761 7264 2f6e 6c70 6175  makcedward/nlpau
+00002440: 6729 2e0a 0a60 6060 7079 7468 6f6e 0a66  g)...```python.f
+00002450: 726f 6d20 696e 7465 6c5f 6578 7465 6e73  rom intel_extens
+00002460: 696f 6e5f 666f 725f 7472 616e 7366 6f72  ion_for_transfor
+00002470: 6d65 7273 2e70 7265 7072 6f63 6573 7369  mers.preprocessi
+00002480: 6e67 2e64 6174 615f 6175 676d 656e 7461  ng.data_augmenta
+00002490: 7469 6f6e 2069 6d70 6f72 7420 4461 7461  tion import Data
+000024a0: 4175 676d 656e 7461 7469 6f6e 0a61 7567  Augmentation.aug
+000024b0: 203d 2044 6174 6141 7567 6d65 6e74 6174   = DataAugmentat
+000024c0: 696f 6e28 6175 676d 656e 7465 725f 7479  ion(augmenter_ty
+000024d0: 7065 3d22 5465 7874 4765 6e65 7261 7469  pe="TextGenerati
+000024e0: 6f6e 4175 6722 290a 6175 672e 696e 7075  onAug").aug.inpu
+000024f0: 745f 6461 7461 7365 7420 3d20 226f 7269  t_dataset = "ori
+00002500: 6769 6e61 6c5f 6461 7461 7365 742e 6373  ginal_dataset.cs
+00002510: 7622 2023 2065 7861 6d70 6c65 3a20 6874  v" # example: ht
+00002520: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00002530: 652e 636f 2f64 6174 6173 6574 732f 676c  e.co/datasets/gl
+00002540: 7565 2f76 6965 7765 722f 7373 7432 2f74  ue/viewer/sst2/t
+00002550: 7261 696e 0a61 7567 2e63 6f6c 756d 6e5f  rain.aug.column_
+00002560: 6e61 6d65 7320 3d20 2273 656e 7465 6e63  names = "sentenc
+00002570: 6522 0a61 7567 2e6f 7574 7075 745f 7061  e".aug.output_pa
+00002580: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+00002590: 6e28 7365 6c66 2e72 6573 756c 745f 7061  n(self.result_pa
+000025a0: 7468 2c20 2274 6573 7432 2e63 7673 2229  th, "test2.cvs")
+000025b0: 0a61 7567 2e61 7567 6d65 6e74 6572 5f61  .aug.augmenter_a
+000025c0: 7267 756d 656e 7473 203d 207b 276d 6f64  rguments = {'mod
+000025d0: 656c 5f6e 616d 655f 6f72 5f70 6174 6827  el_name_or_path'
+000025e0: 3a20 2767 7074 322d 6d65 6469 756d 277d  : 'gpt2-medium'}
+000025f0: 0a61 7567 2e64 6174 615f 6175 676d 656e  .aug.data_augmen
+00002600: 7428 290a 7261 775f 6461 7461 7365 7473  t().raw_datasets
+00002610: 203d 206c 6f61 645f 6461 7461 7365 7428   = load_dataset(
+00002620: 2263 7376 222c 2064 6174 615f 6669 6c65  "csv", data_file
+00002630: 733d 6175 672e 6f75 7470 7574 5f70 6174  s=aug.output_pat
+00002640: 682c 2064 656c 696d 6974 6572 3d22 5c74  h, delimiter="\t
+00002650: 222c 2073 706c 6974 3d22 7472 6169 6e22  ", split="train"
+00002660: 290a 6060 600a 0a50 6c65 6173 6520 7265  ).```..Please re
+00002670: 6665 7220 746f 205b 6461 7461 2061 7567  fer to [data aug
+00002680: 6d65 6e74 6174 696f 6e20 646f 6375 6d65  mentation docume
+00002690: 6e74 5d28 646f 6373 2f64 6174 615f 6175  nt](docs/data_au
+000026a0: 676d 656e 7461 7469 6f6e 2e6d 6429 2066  gmentation.md) f
+000026b0: 6f72 206d 6f72 6520 6465 7461 696c 732e  or more details.
+000026c0: 0a0a 2323 2320 4e65 7572 616c 2045 6e67  ..### Neural Eng
+000026d0: 696e 650a 4e65 7572 616c 2045 6e67 696e  ine.Neural Engin
+000026e0: 6520 6973 206f 6e65 206f 6620 7265 6665  e is one of refe
+000026f0: 7265 6e63 6520 6465 706c 6f79 6d65 6e74  rence deployment
+00002700: 7320 7468 6174 2049 6e74 656c 2045 7874  s that Intel Ext
+00002710: 656e 7369 6f6e 2066 6f72 2054 7261 6e73  ension for Trans
+00002720: 666f 726d 6572 7320 7072 6f76 6964 6573  formers provides
+00002730: 2e20 4e65 7572 616c 2045 6e67 696e 6520  . Neural Engine 
+00002740: 6169 6d73 2074 6f20 6465 6d6f 6e73 7472  aims to demonstr
+00002750: 6174 6520 7468 6520 6f70 7469 6d61 6c20  ate the optimal 
+00002760: 7065 7266 6f72 6d61 6e63 6520 6f66 2065  performance of e
+00002770: 7874 7265 6d65 6c79 2063 6f6d 7072 6573  xtremely compres
+00002780: 7365 6420 4e4c 5020 6d6f 6465 6c73 2062  sed NLP models b
+00002790: 7920 6578 706c 6f72 696e 6720 7468 6520  y exploring the 
+000027a0: 6f70 7469 6d69 7a61 7469 6f6e 206f 7070  optimization opp
+000027b0: 6f72 7475 6e69 7469 6573 2066 726f 6d20  ortunities from 
+000027c0: 626f 7468 2048 5720 616e 6420 5357 2e0a  both HW and SW..
+000027d0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+000027e0: 696e 7465 6c5f 6578 7465 6e73 696f 6e5f  intel_extension_
+000027f0: 666f 725f 7472 616e 7366 6f72 6d65 7273  for_transformers
+00002800: 2e62 6163 6b65 6e64 732e 6e65 7572 616c  .backends.neural
+00002810: 5f65 6e67 696e 652e 636f 6d70 696c 6520  _engine.compile 
+00002820: 696d 706f 7274 2063 6f6d 7069 6c65 0a23  import compile.#
+00002830: 202f 7061 7468 2f74 6f2f 796f 7572 2f6d   /path/to/your/m
+00002840: 6f64 656c 2069 7320 6120 5465 6e73 6f72  odel is a Tensor
+00002850: 466c 6f77 2070 6220 6d6f 6465 6c20 6f72  Flow pb model or
+00002860: 204f 4e4e 5820 6d6f 6465 6c0a 6d6f 6465   ONNX model.mode
+00002870: 6c20 3d20 636f 6d70 696c 6528 272f 7061  l = compile('/pa
+00002880: 7468 2f74 6f2f 796f 7572 2f6d 6f64 656c  th/to/your/model
+00002890: 2729 0a69 6e70 7574 7320 3d20 2e2e 2e20  ').inputs = ... 
+000028a0: 2320 5b69 6e70 7574 5f69 6473 2c20 7365  # [input_ids, se
+000028b0: 676d 656e 745f 6964 732c 2069 6e70 7574  gment_ids, input
+000028c0: 5f6d 6173 6b5d 0a6d 6f64 656c 2e69 6e66  _mask].model.inf
+000028d0: 6572 656e 6365 2869 6e70 7574 7329 0a60  erence(inputs).`
+000028e0: 6060 0a0a 506c 6561 7365 2072 6566 6572  ``..Please refer
+000028f0: 2074 6f20 5b4e 6575 7261 6c20 456e 6769   to [Neural Engi
+00002900: 6e65 5d28 6578 616d 706c 6573 2f64 6570  ne](examples/dep
+00002910: 6c6f 796d 656e 742f 2920 666f 7220 6d6f  loyment/) for mo
+00002920: 7265 2064 6574 6169 6c73 2e0a 0a23 2323  re details...###
+00002930: 2051 7561 6e74 697a 6564 204c 656e 6774   Quantized Lengt
+00002940: 6820 4164 6170 7469 7665 2054 7261 6e73  h Adaptive Trans
+00002950: 666f 726d 6572 0a51 7561 6e74 697a 6564  former.Quantized
+00002960: 204c 656e 6774 6820 4164 6170 7469 7665   Length Adaptive
+00002970: 2054 7261 6e73 666f 726d 6572 206c 6576   Transformer lev
+00002980: 6572 6167 6573 2073 6571 7565 6e63 652d  erages sequence-
+00002990: 6c65 6e67 7468 2072 6564 7563 7469 6f6e  length reduction
+000029a0: 2061 6e64 206c 6f77 2d62 6974 2072 6570   and low-bit rep
+000029b0: 7265 7365 6e74 6174 696f 6e20 7465 6368  resentation tech
+000029c0: 6e69 7175 6573 2074 6f20 6675 7274 6865  niques to furthe
+000029d0: 7220 656e 6861 6e63 6520 6d6f 6465 6c20  r enhance model 
+000029e0: 696e 6665 7265 6e63 6520 7065 7266 6f72  inference perfor
+000029f0: 6d61 6e63 652c 2065 6e61 626c 696e 6720  mance, enabling 
+00002a00: 6164 6170 7469 7665 2073 6571 7565 6e63  adaptive sequenc
+00002a10: 652d 6c65 6e67 7468 2073 697a 6573 2074  e-length sizes t
+00002a20: 6f20 6163 636f 6d6d 6f64 6174 6520 6469  o accommodate di
+00002a30: 6666 6572 656e 7420 636f 6d70 7574 6174  fferent computat
+00002a40: 696f 6e61 6c20 6275 6467 6574 2072 6571  ional budget req
+00002a50: 7569 7265 6d65 6e74 7320 7769 7468 2061  uirements with a
+00002a60: 6e20 6f70 7469 6d61 6c20 6163 6375 7261  n optimal accura
+00002a70: 6379 2065 6666 6963 6965 6e63 7920 7472  cy efficiency tr
+00002a80: 6164 656f 6666 2e0a 6060 6070 7974 686f  adeoff..```pytho
+00002a90: 6e0a 6672 6f6d 2069 6e74 656c 5f65 7874  n.from intel_ext
+00002aa0: 656e 7369 6f6e 5f66 6f72 5f74 7261 6e73  ension_for_trans
+00002ab0: 666f 726d 6572 7320 696d 706f 7274 2051  formers import Q
+00002ac0: 7561 6e74 697a 6174 696f 6e43 6f6e 6669  uantizationConfi
+00002ad0: 672c 2044 796e 616d 6963 4c65 6e67 7468  g, DynamicLength
+00002ae0: 436f 6e66 6967 2c20 6d65 7472 6963 2c20  Config, metric, 
+00002af0: 6f62 6a65 6374 6976 6573 0a66 726f 6d20  objectives.from 
+00002b00: 696e 7465 6c5f 6578 7465 6e73 696f 6e5f  intel_extension_
+00002b10: 666f 725f 7472 616e 7366 6f72 6d65 7273  for_transformers
+00002b20: 2e6f 7074 696d 697a 6174 696f 6e2e 7472  .optimization.tr
+00002b30: 6169 6e65 7220 696d 706f 7274 204e 4c50  ainer import NLP
+00002b40: 5472 6169 6e65 720a 0a23 2052 6570 6c61  Trainer..# Repla
+00002b50: 6365 2074 7261 6e73 666f 726d 6572 732e  ce transformers.
+00002b60: 5472 6169 6e65 7220 7769 7468 204e 4c50  Trainer with NLP
+00002b70: 5472 6169 6e65 720a 2320 7472 6169 6e65  Trainer.# traine
+00002b80: 7220 3d20 7472 616e 7366 6f72 6d65 7273  r = transformers
+00002b90: 2e54 7261 696e 6572 282e 2e2e 290a 7472  .Trainer(...).tr
+00002ba0: 6169 6e65 7220 3d20 4e4c 5054 7261 696e  ainer = NLPTrain
+00002bb0: 6572 282e 2e2e 290a 6d65 7472 6963 203d  er(...).metric =
+00002bc0: 206d 6574 7269 6373 2e4d 6574 7269 6328   metrics.Metric(
+00002bd0: 6e61 6d65 3d22 6576 616c 5f66 3122 2c20  name="eval_f1", 
+00002be0: 6973 5f72 656c 6174 6976 653d 5472 7565  is_relative=True
+00002bf0: 2c20 6372 6974 6572 696f 6e3d 302e 3031  , criterion=0.01
+00002c00: 290a 715f 636f 6e66 6967 203d 2051 7561  ).q_config = Qua
+00002c10: 6e74 697a 6174 696f 6e43 6f6e 6669 6728  ntizationConfig(
+00002c20: 0a20 2020 2061 7070 726f 6163 683d 2250  .    approach="P
+00002c30: 6f73 7454 7261 696e 696e 6753 7461 7469  ostTrainingStati
+00002c40: 6322 2c0a 2020 2020 6d65 7472 6963 733d  c",.    metrics=
+00002c50: 5b6d 6574 7269 635d 2c0a 2020 2020 6f62  [metric],.    ob
+00002c60: 6a65 6374 6976 6573 3d5b 6f62 6a65 6374  jectives=[object
+00002c70: 6976 6573 2e70 6572 666f 726d 616e 6365  ives.performance
+00002c80: 5d0a 290a 2320 4170 706c 7920 7468 6520  ].).# Apply the 
+00002c90: 6c65 6e67 7468 2063 6f6e 6669 670a 6479  length config.dy
+00002ca0: 6e61 6d69 635f 6c65 6e67 7468 5f63 6f6e  namic_length_con
+00002cb0: 6669 6720 3d20 4479 6e61 6d69 634c 656e  fig = DynamicLen
+00002cc0: 6774 6843 6f6e 6669 6728 6c65 6e67 7468  gthConfig(length
+00002cd0: 5f63 6f6e 6669 673d 6c65 6e67 7468 5f63  _config=length_c
+00002ce0: 6f6e 6669 6729 0a74 7261 696e 6572 2e73  onfig).trainer.s
+00002cf0: 6574 5f64 796e 616d 6963 5f63 6f6e 6669  et_dynamic_confi
+00002d00: 6728 6479 6e61 6d69 635f 636f 6e66 6967  g(dynamic_config
+00002d10: 3d64 796e 616d 6963 5f6c 656e 6774 685f  =dynamic_length_
+00002d20: 636f 6e66 6967 290a 2320 5175 616e 7469  config).# Quanti
+00002d30: 7a61 7469 6f6e 0a6d 6f64 656c 203d 2074  zation.model = t
+00002d40: 7261 696e 6572 2e71 7561 6e74 697a 6528  rainer.quantize(
+00002d50: 7175 616e 745f 636f 6e66 6967 3d71 5f63  quant_config=q_c
+00002d60: 6f6e 6669 6729 0a60 6060 0a0a 506c 6561  onfig).```..Plea
+00002d70: 7365 2072 6566 6572 2074 6f20 7061 7065  se refer to pape
+00002d80: 7220 5b51 7561 4c41 2d4d 696e 694c 4d5d  r [QuaLA-MiniLM]
+00002d90: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
+00002da0: 7267 2f70 6466 2f32 3231 302e 3137 3131  rg/pdf/2210.1711
+00002db0: 342e 7064 6629 2061 6e64 205b 636f 6465  4.pdf) and [code
+00002dc0: 5d28 6578 616d 706c 6573 2f6f 7074 696d  ](examples/optim
+00002dd0: 697a 6174 696f 6e2f 7079 746f 7263 682f  ization/pytorch/
+00002de0: 6875 6767 696e 6766 6163 652f 7175 6573  huggingface/ques
+00002df0: 7469 6f6e 2d61 6e73 7765 7269 6e67 2f64  tion-answering/d
+00002e00: 796e 616d 6963 2920 666f 7220 6465 7461  ynamic) for deta
+00002e10: 696c 730a 0a0a 2323 2320 5472 616e 7366  ils...### Transf
+00002e20: 6f72 6d65 7273 2d61 6363 656c 6572 6174  ormers-accelerat
+00002e30: 6564 204e 6575 7261 6c20 456e 6769 6e65  ed Neural Engine
+00002e40: 0a54 7261 6e73 666f 726d 6572 732d 6163  .Transformers-ac
+00002e50: 6365 6c65 7261 7465 6420 4e65 7572 616c  celerated Neural
+00002e60: 2045 6e67 696e 6520 6973 206f 6e65 206f   Engine is one o
+00002e70: 6620 7265 6665 7265 6e63 6520 6465 706c  f reference depl
+00002e80: 6f79 6d65 6e74 7320 7468 6174 2049 6e74  oyments that Int
+00002e90: 656c c2ae 2045 7874 656e 7369 6f6e 2066  el.. Extension f
+00002ea0: 6f72 2054 7261 6e73 666f 726d 6572 7320  or Transformers 
+00002eb0: 7072 6f76 6964 6573 2e20 4e65 7572 616c  provides. Neural
+00002ec0: 2045 6e67 696e 6520 6169 6d73 2074 6f20   Engine aims to 
+00002ed0: 6465 6d6f 6e73 7472 6174 6520 7468 6520  demonstrate the 
+00002ee0: 6f70 7469 6d61 6c20 7065 7266 6f72 6d61  optimal performa
+00002ef0: 6e63 6520 6f66 2065 7874 7265 6d65 6c79  nce of extremely
+00002f00: 2063 6f6d 7072 6573 7365 6420 4e4c 5020   compressed NLP 
+00002f10: 6d6f 6465 6c73 2062 7920 6578 706c 6f72  models by explor
+00002f20: 696e 6720 7468 6520 6f70 7469 6d69 7a61  ing the optimiza
+00002f30: 7469 6f6e 206f 7070 6f72 7475 6e69 7469  tion opportuniti
+00002f40: 6573 2066 726f 6d20 626f 7468 2048 5720  es from both HW 
+00002f50: 616e 6420 5357 2e0a 0a60 6060 7079 7468  and SW...```pyth
+00002f60: 6f6e 0a66 726f 6d20 696e 7465 6c5f 6578  on.from intel_ex
+00002f70: 7465 6e73 696f 6e5f 666f 725f 7472 616e  tension_for_tran
+00002f80: 7366 6f72 6d65 7273 2e62 6163 6b65 6e64  sformers.backend
+00002f90: 732e 6e65 7572 616c 5f65 6e67 696e 652e  s.neural_engine.
+00002fa0: 636f 6d70 696c 6520 696d 706f 7274 2063  compile import c
+00002fb0: 6f6d 7069 6c65 0a23 202f 7061 7468 2f74  ompile.# /path/t
+00002fc0: 6f2f 796f 7572 2f6d 6f64 656c 2069 7320  o/your/model is 
+00002fd0: 6120 5465 6e73 6f72 466c 6f77 2070 6220  a TensorFlow pb 
+00002fe0: 6d6f 6465 6c20 6f72 204f 4e4e 5820 6d6f  model or ONNX mo
+00002ff0: 6465 6c0a 6d6f 6465 6c20 3d20 636f 6d70  del.model = comp
+00003000: 696c 6528 272f 7061 7468 2f74 6f2f 796f  ile('/path/to/yo
+00003010: 7572 2f6d 6f64 656c 2729 0a69 6e70 7574  ur/model').input
+00003020: 7320 3d20 2e2e 2e20 2320 5b69 6e70 7574  s = ... # [input
+00003030: 5f69 6473 2c20 7365 676d 656e 745f 6964  _ids, segment_id
+00003040: 732c 2069 6e70 7574 5f6d 6173 6b5d 0a6d  s, input_mask].m
+00003050: 6f64 656c 2e69 6e66 6572 656e 6365 2869  odel.inference(i
+00003060: 6e70 7574 7329 0a60 6060 0a0a 506c 6561  nputs).```..Plea
+00003070: 7365 2072 6566 6572 2074 6f20 5b65 7861  se refer to [exa
+00003080: 6d70 6c65 5d28 6578 616d 706c 6573 2f64  mple](examples/d
+00003090: 6570 6c6f 796d 656e 742f 6e65 7572 616c  eployment/neural
+000030a0: 5f65 6e67 696e 652f 7370 6172 7365 2f64  _engine/sparse/d
+000030b0: 6973 7469 6c62 6572 745f 6261 7365 5f75  istilbert_base_u
+000030c0: 6e63 6173 6564 2f29 2069 6e20 5b54 7261  ncased/) in [Tra
+000030d0: 6e73 666f 726d 6572 732d 6163 6365 6c65  nsformers-accele
+000030e0: 7261 7465 6420 4e65 7572 616c 2045 6e67  rated Neural Eng
+000030f0: 696e 655d 2865 7861 6d70 6c65 732f 6465  ine](examples/de
+00003100: 706c 6f79 6d65 6e74 2f29 2061 6e64 2070  ployment/) and p
+00003110: 6170 6572 205b 4661 7374 2044 6973 7469  aper [Fast Disti
+00003120: 6c62 6572 7420 6f6e 2043 5055 735d 2868  lbert on CPUs](h
+00003130: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00003140: 2f61 6273 2f32 3231 312e 3037 3731 3529  /abs/2211.07715)
+00003150: 2066 6f72 206d 6f72 6520 6465 7461 696c   for more detail
+00003160: 732e 0a0a 2323 2320 5472 616e 7366 6f72  s...### Transfor
+00003170: 6d65 7273 2d61 6363 656c 6572 6174 6564  mers-accelerated
+00003180: 204c 6962 7261 7269 6573 0a54 7261 6e73   Libraries.Trans
+00003190: 666f 726d 6572 732d 6163 6365 6c65 7261  formers-accelera
+000031a0: 7465 6420 4c69 6272 6172 6965 7320 6973  ted Libraries is
+000031b0: 2061 2068 6967 682d 7065 7266 6f72 6d61   a high-performa
+000031c0: 6e63 6520 6f70 6572 6174 6f72 2063 6f6d  nce operator com
+000031d0: 7075 7469 6e67 206c 6962 7261 7279 2069  puting library i
+000031e0: 6d70 6c65 6d65 6e74 6564 2062 7920 6173  mplemented by as
+000031f0: 7365 6d62 6c79 2e20 5472 616e 7366 6f72  sembly. Transfor
+00003200: 6d65 7273 2d61 6363 656c 6572 6174 6564  mers-accelerated
+00003210: 204c 6962 7261 7269 6573 2063 6f6e 7461   Libraries conta
+00003220: 696e 7320 6120 4a49 5420 646f 6d61 696e  ins a JIT domain
+00003230: 2c20 6120 6b65 726e 656c 2064 6f6d 6169  , a kernel domai
+00003240: 6e2c 2061 6e64 2061 2073 6368 6564 756c  n, and a schedul
+00003250: 696e 6720 7072 6f78 7920 6672 616d 6577  ing proxy framew
+00003260: 6f72 6b2e 0a0a 6060 6043 2b2b 0a23 696e  ork...```C++.#in
+00003270: 636c 7564 6520 2269 6e74 6572 6661 6365  clude "interface
+00003280: 2e68 7070 220a 2020 2e2e 2e0a 2020 6f70  .hpp".  ....  op
+00003290: 6572 6174 6f72 5f64 6573 6320 6f70 5f64  erator_desc op_d
+000032a0: 6573 6328 6b65 725f 6b69 6e64 2c20 6b65  esc(ker_kind, ke
+000032b0: 725f 7072 6f70 2c20 656e 675f 6b69 6e64  r_prop, eng_kind
+000032c0: 2c20 7473 5f64 6573 6373 2c20 6f70 5f61  , ts_descs, op_a
+000032d0: 7474 7273 293b 0a20 2073 7061 7273 655f  ttrs);.  sparse_
+000032e0: 6d61 746d 756c 5f64 6573 6320 7370 6d6d  matmul_desc spmm
+000032f0: 5f64 6573 6328 6f70 5f64 6573 6329 3b0a  _desc(op_desc);.
+00003300: 2020 7370 6172 7365 5f6d 6174 6d75 6c20    sparse_matmul 
+00003310: 7370 6d6d 5f6b 6572 6e28 7370 6d6d 5f64  spmm_kern(spmm_d
+00003320: 6573 6329 3b0a 2020 7374 643a 3a76 6563  esc);.  std::vec
+00003330: 746f 723c 636f 6e73 7420 766f 6964 2a3e  tor<const void*>
+00003340: 2072 745f 6461 7461 203d 207b 6461 7461   rt_data = {data
+00003350: 302c 2064 6174 6131 2c20 6461 7461 322c  0, data1, data2,
+00003360: 2064 6174 6133 2c20 6461 7461 347d 3b0a   data3, data4};.
+00003370: 2020 7370 6d6d 5f6b 6572 6e2e 6578 6563    spmm_kern.exec
+00003380: 7574 6528 7274 5f64 6174 6129 3b0a 6060  ute(rt_data);.``
+00003390: 600a 506c 6561 7365 2072 6566 6572 2074  `.Please refer t
+000033a0: 6f20 5b54 7261 6e73 666f 726d 6572 732d  o [Transformers-
+000033b0: 6163 6365 6c65 7261 7465 6420 4c69 6272  accelerated Libr
+000033c0: 6172 6965 735d 2869 6e74 656c 5f65 7874  aries](intel_ext
+000033d0: 656e 7369 6f6e 5f66 6f72 5f74 7261 6e73  ension_for_trans
+000033e0: 666f 726d 6572 732f 6261 636b 656e 6473  formers/backends
+000033f0: 2f6e 6575 7261 6c5f 656e 6769 6e65 2f6b  /neural_engine/k
+00003400: 6572 6e65 6c73 2f52 4541 444d 452e 6d64  ernels/README.md
+00003410: 2920 666f 7220 6d6f 7265 2064 6574 6169  ) for more detai
+00003420: 6c73 2e0a 0a0a 2323 2053 7973 7465 6d20  ls....## System 
+00003430: 5265 7175 6972 656d 656e 7473 0a23 2323  Requirements.###
+00003440: 2056 616c 6964 6174 6564 2048 6172 6477   Validated Hardw
+00003450: 6172 6520 456e 7669 726f 6e6d 656e 740a  are Environment.
+00003460: 496e 7465 6cc2 ae20 4578 7465 6e73 696f  Intel.. Extensio
+00003470: 6e20 666f 7220 5472 616e 7366 6f72 6d65  n for Transforme
+00003480: 7273 2073 7570 706f 7274 7320 7379 7374  rs supports syst
+00003490: 656d 7320 6261 7365 6420 6f6e 205b 496e  ems based on [In
+000034a0: 7465 6c20 3634 2061 7263 6869 7465 6374  tel 64 architect
+000034b0: 7572 6520 6f72 2063 6f6d 7061 7469 626c  ure or compatibl
+000034c0: 6520 7072 6f63 6573 736f 7273 5d28 6874  e processors](ht
+000034d0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+000034e0: 6961 2e6f 7267 2f77 696b 692f 5838 362d  ia.org/wiki/X86-
+000034f0: 3634 2920 7468 6174 2061 7265 2073 7065  64) that are spe
+00003500: 6369 6669 6361 6c6c 7920 6f70 7469 6d69  cifically optimi
+00003510: 7a65 6420 666f 7220 7468 6520 666f 6c6c  zed for the foll
+00003520: 6f77 696e 6720 4350 5573 3a0a 0a2a 2049  owing CPUs:..* I
+00003530: 6e74 656c 2058 656f 6e20 5363 616c 6162  ntel Xeon Scalab
+00003540: 6c65 2070 726f 6365 7373 6f72 2028 666f  le processor (fo
+00003550: 726d 6572 6c79 2043 6173 6361 6465 204c  rmerly Cascade L
+00003560: 616b 652c 2049 6365 6c61 6b65 290a 2a20  ake, Icelake).* 
+00003570: 4675 7475 7265 2049 6e74 656c 2058 656f  Future Intel Xeo
+00003580: 6e20 5363 616c 6162 6c65 2070 726f 6365  n Scalable proce
+00003590: 7373 6f72 2028 636f 6465 206e 616d 6520  ssor (code name 
+000035a0: 5361 7070 6869 7265 2052 6170 6964 7329  Sapphire Rapids)
+000035b0: 0a0a 2323 2320 5661 6c69 6461 7465 6420  ..### Validated 
+000035c0: 536f 6674 7761 7265 2045 6e76 6972 6f6e  Software Environ
+000035d0: 6d65 6e74 0a0a 2a20 4f53 2076 6572 7369  ment..* OS versi
+000035e0: 6f6e 3a20 4365 6e74 4f53 2038 2e34 2c20  on: CentOS 8.4, 
+000035f0: 5562 756e 7475 2032 302e 3034 2020 0a2a  Ubuntu 20.04  .*
+00003600: 2050 7974 686f 6e20 7665 7273 696f 6e3a   Python version:
+00003610: 2033 2e37 2c20 332e 382c 2033 2e39 2c20   3.7, 3.8, 3.9, 
+00003620: 332e 3130 2020 0a0a 3c74 6162 6c65 2063  3.10  ..<table c
+00003630: 6c61 7373 3d22 646f 6375 7469 6c73 223e  lass="docutils">
+00003640: 0a3c 7468 6561 643e 0a20 203c 7472 3e0a  .<thead>.  <tr>.
+00003650: 2020 2020 3c74 683e 4672 616d 6577 6f72      <th>Framewor
+00003660: 6b3c 2f74 683e 0a20 2020 203c 7468 3e54  k</th>.    <th>T
+00003670: 656e 736f 7246 6c6f 773c 2f74 683e 0a20  ensorFlow</th>. 
+00003680: 2020 203c 7468 3e49 6e74 656c 2054 656e     <th>Intel Ten
+00003690: 736f 7246 6c6f 773c 2f74 683e 0a20 2020  sorFlow</th>.   
+000036a0: 203c 7468 3e50 7954 6f72 6368 3c2f 7468   <th>PyTorch</th
+000036b0: 3e0a 2020 2020 3c74 683e 4950 4558 3c2f  >.    <th>IPEX</
+000036c0: 7468 3e0a 2020 3c2f 7472 3e0a 3c2f 7468  th>.  </tr>.</th
+000036d0: 6561 643e 0a3c 7462 6f64 793e 0a20 203c  ead>.<tbody>.  <
+000036e0: 7472 2061 6c69 676e 3d22 6365 6e74 6572  tr align="center
+000036f0: 223e 0a20 2020 203c 7468 3e56 6572 7369  ">.    <th>Versi
+00003700: 6f6e 3c2f 7468 3e0a 2020 2020 3c74 6420  on</th>.    <td 
+00003710: 636c 6173 733d 2274 672d 377a 726c 223e  class="tg-7zrl">
+00003720: 3c61 2068 7265 663d 6874 7470 733a 2f2f  <a href=https://
+00003730: 6769 7468 7562 2e63 6f6d 2f74 656e 736f  github.com/tenso
+00003740: 7266 6c6f 772f 7465 6e73 6f72 666c 6f77  rflow/tensorflow
+00003750: 2f74 7265 652f 7632 2e31 302e 303e 322e  /tree/v2.10.0>2.
+00003760: 3130 2e30 3c2f 613e 3c62 723e 0a20 2020  10.0</a><br>.   
+00003770: 203c 6120 6872 6566 3d68 7474 7073 3a2f   <a href=https:/
+00003780: 2f67 6974 6875 622e 636f 6d2f 7465 6e73  /github.com/tens
+00003790: 6f72 666c 6f77 2f74 656e 736f 7266 6c6f  orflow/tensorflo
+000037a0: 772f 7472 6565 2f76 322e 392e 313e 322e  w/tree/v2.9.1>2.
+000037b0: 392e 313c 2f61 3e3c 6272 3e0a 2020 2020  9.1</a><br>.    
+000037c0: 3c74 6420 636c 6173 733d 2274 672d 377a  <td class="tg-7z
+000037d0: 726c 223e 3c61 2068 7265 663d 6874 7470  rl"><a href=http
+000037e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f49  s://github.com/I
+000037f0: 6e74 656c 2d74 656e 736f 7266 6c6f 772f  ntel-tensorflow/
+00003800: 7465 6e73 6f72 666c 6f77 2f74 7265 652f  tensorflow/tree/
+00003810: 7632 2e31 302e 303e 322e 3130 2e30 3c2f  v2.10.0>2.10.0</
+00003820: 613e 3c62 723e 0a20 2020 203c 6120 6872  a><br>.    <a hr
+00003830: 6566 3d68 7474 7073 3a2f 2f67 6974 6875  ef=https://githu
+00003840: 622e 636f 6d2f 496e 7465 6c2d 7465 6e73  b.com/Intel-tens
+00003850: 6f72 666c 6f77 2f74 656e 736f 7266 6c6f  orflow/tensorflo
+00003860: 772f 7472 6565 2f76 322e 392e 313e 322e  w/tree/v2.9.1>2.
+00003870: 392e 313c 2f61 3e3c 6272 3e0a 2020 2020  9.1</a><br>.    
+00003880: 3c74 6420 636c 6173 733d 2274 672d 377a  <td class="tg-7z
+00003890: 726c 223e 3c61 2068 7265 663d 6874 7470  rl"><a href=http
+000038a0: 733a 2f2f 646f 776e 6c6f 6164 2e70 7974  s://download.pyt
+000038b0: 6f72 6368 2e6f 7267 2f77 686c 2f74 6f72  orch.org/whl/tor
+000038c0: 6368 5f73 7461 626c 652e 6874 6d6c 3e31  ch_stable.html>1
+000038d0: 2e31 332e 302b 6370 753c 2f61 3e3c 6272  .13.0+cpu</a><br
+000038e0: 3e0a 2020 2020 3c61 2068 7265 663d 6874  >.    <a href=ht
+000038f0: 7470 733a 2f2f 646f 776e 6c6f 6164 2e70  tps://download.p
+00003900: 7974 6f72 6368 2e6f 7267 2f77 686c 2f74  ytorch.org/whl/t
+00003910: 6f72 6368 5f73 7461 626c 652e 6874 6d6c  orch_stable.html
+00003920: 3e31 2e31 322e 302b 6370 753c 2f61 3e3c  >1.12.0+cpu</a><
+00003930: 6272 3e0a 2020 2020 3c74 6420 636c 6173  br>.    <td clas
+00003940: 733d 2274 672d 377a 726c 223e 3c61 2068  s="tg-7zrl"><a h
+00003950: 7265 663d 6874 7470 733a 2f2f 6769 7468  ref=https://gith
+00003960: 7562 2e63 6f6d 2f69 6e74 656c 2f69 6e74  ub.com/intel/int
+00003970: 656c 2d65 7874 656e 7369 6f6e 2d66 6f72  el-extension-for
+00003980: 2d70 7974 6f72 6368 2f74 7265 652f 312e  -pytorch/tree/1.
+00003990: 3131 2e30 3e31 2e31 332e 303c 2f61 3e3c  11.0>1.13.0</a><
+000039a0: 6272 3e0a 2020 2020 3c61 2068 7265 663d  br>.    <a href=
+000039b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000039c0: 6f6d 2f69 6e74 656c 2f69 6e74 656c 2d65  om/intel/intel-e
+000039d0: 7874 656e 7369 6f6e 2d66 6f72 2d70 7974  xtension-for-pyt
+000039e0: 6f72 6368 2f74 7265 652f 7631 2e31 302e  orch/tree/v1.10.
+000039f0: 303e 312e 3132 2e30 3c2f 613e 3c2f 7464  0>1.12.0</a></td
+00003a00: 3e0a 2020 3c2f 7472 3e0a 3c2f 7462 6f64  >.  </tr>.</tbod
+00003a10: 793e 0a3c 2f74 6162 6c65 3e0a 0a0a 2323  y>.</table>...##
+00003a20: 2053 656c 6563 7465 6420 5075 626c 6963   Selected Public
+00003a30: 6174 696f 6e73 2f45 7665 6e74 730a 2a20  ations/Events.* 
+00003a40: 4e65 7572 4950 5327 3230 3232 3a20 5b46  NeurIPS'2022: [F
+00003a50: 6173 7420 4469 7374 696c 6265 7274 206f  ast Distilbert o
+00003a60: 6e20 4350 5573 5d28 6874 7470 733a 2f2f  n CPUs](https://
+00003a70: 6172 7869 762e 6f72 672f 6162 732f 3232  arxiv.org/abs/22
+00003a80: 3131 2e30 3737 3135 2920 284e 6f76 2032  11.07715) (Nov 2
+00003a90: 3032 3229 0a2a 204e 6575 7249 5053 2732  022).* NeurIPS'2
+00003aa0: 3032 323a 205b 5175 614c 412d 4d69 6e69  022: [QuaLA-Mini
+00003ab0: 4c4d 3a20 6120 5175 616e 7469 7a65 6420  LM: a Quantized 
+00003ac0: 4c65 6e67 7468 2041 6461 7074 6976 6520  Length Adaptive 
+00003ad0: 4d69 6e69 4c4d 5d28 6874 7470 733a 2f2f  MiniLM](https://
+00003ae0: 6172 7869 762e 6f72 672f 6162 732f 3232  arxiv.org/abs/22
+00003af0: 3130 2e31 3731 3134 2920 284e 6f76 2032  10.17114) (Nov 2
+00003b00: 3032 3229 0a2a 2042 6c6f 6720 7075 626c  022).* Blog publ
+00003b10: 6973 6865 6420 6279 2043 6f68 6572 653a  ished by Cohere:
+00003b20: 205b 546f 7020 4e4c 5020 5061 7065 7273   [Top NLP Papers
+00003b30: e280 944e 6f76 656d 6265 7220 3230 3232  ...November 2022
+00003b40: 5d28 6874 7470 733a 2f2f 7478 742e 636f  ](https://txt.co
+00003b50: 6865 7265 2e61 692f 746f 702d 6e6c 702d  here.ai/top-nlp-
+00003b60: 7061 7065 7273 2d6e 6f76 656d 6265 722d  papers-november-
+00003b70: 3230 3232 2f29 2028 4e6f 7620 3230 3232  2022/) (Nov 2022
+00003b80: 290a 2a20 426c 6f67 2070 7562 6c69 7368  ).* Blog publish
+00003b90: 6564 2062 7920 416c 6962 6162 613a 205b  ed by Alibaba: [
+00003ba0: 4465 6570 206c 6561 726e 696e 6720 696e  Deep learning in
+00003bb0: 6665 7265 6e63 6520 6f70 7469 6d69 7a61  ference optimiza
+00003bc0: 7469 6f6e 2066 6f72 2041 6464 7265 7373  tion for Address
+00003bd0: 2050 7572 6966 6963 6174 696f 6e5d 2868   Purification](h
+00003be0: 7474 7073 3a2f 2f7a 6875 616e 6c61 6e2e  ttps://zhuanlan.
+00003bf0: 7a68 6968 752e 636f 6d2f 702f 3535 3234  zhihu.com/p/5524
+00003c00: 3834 3431 3329 2028 4175 6720 3230 3232  84413) (Aug 2022
+00003c10: 290a 2a20 4e65 7572 4950 5327 3230 3231  ).* NeurIPS'2021
+00003c20: 3a20 5b50 7275 6e65 204f 6e63 6520 666f  : [Prune Once fo
+00003c30: 7220 416c 6c3a 2053 7061 7273 6520 5072  r All: Sparse Pr
+00003c40: 652d 5472 6169 6e65 6420 4c61 6e67 7561  e-Trained Langua
+00003c50: 6765 204d 6f64 656c 735d 2868 7474 7073  ge Models](https
+00003c60: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
+00003c70: 2f32 3131 312e 3035 3735 3429 2028 4e6f  /2111.05754) (No
+00003c80: 7620 3230 3231 290a                      v 2021).
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/__init__.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # limitations under the License.
 
 
 from .optimization.config import (
     AutoDistillationConfig,
     DistillationConfig,
     FlashDistillationConfig,
-    NncfConfig,
+    TFDistillationConfig,
     Provider,
     PruningConfig,
     QuantizationConfig,
     WEIGHTS_NAME,
     DynamicLengthConfig,
 )
 from .optimization.distillation import (
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/__init__.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/dynamic/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
+# limitations under the License.
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/__init__.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/models/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
+# limitations under the License.
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/bin/neural_engine` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/bin/neural_engine`

 * *Files 11% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 import subprocess
 import sys
 import intel_extension_for_transformers
 
 if __name__ == '__main__':
     path = intel_extension_for_transformers.__path__[0]
-    command = [path + '/../neural_engine']
+    command = [path + '/../neural_engine_bin']
     command.extend(sys.argv)
     subprocess.call(command)
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/__init__.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The module of compile."""
+
 from .compile import compile
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/compile.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/compile.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,50 +10,74 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-1. First use model loader to get the computation graph with corresponding framework.
-   The graph contains nodes and edges, the node is op and the edge is the tensor.
-2. Then extract the ops in the graph and pack them to our form.
-3. Next exploit these above ops to consist sub-graph, which can see as "a new big op", like
-   LayerNorm. Note that there may have different computation flow in one subgraph.
-4. Finally, convert them to .yaml file and .bin file for model configuration and inference.
-"""
+
+"""The neural engine compile module."""
 
 from collections import OrderedDict
 from .loaders.loader import Loader
 from .extractors.extractor import Extractor
 from .sub_graph.subgraph_matcher import SubGraphMatcher
 from .graph_utils import get_model_fwk_name
 
 COMPILES = OrderedDict({
     'loader': Loader,
     'extractor': Extractor,
     'sub_graph': SubGraphMatcher,
 })
 
 
+def _config_validation(config):
+    """The validation of the input config."""
+    if config == None:
+        return None
+
+    import yaml
+    from schema import Schema
+
+    with open(config, 'r') as conf_file:
+        conf = yaml.safe_load(conf_file)
+
+    conf_schema = Schema(
+        {'pattern_switch': Schema({str: bool}, error='You should provide correct fused_patterns.')})
+
+    return conf_schema.validate(conf)
+
+
 def start_pipeline(model, config=None):
+    """The compile pipeline."""
     compile_list = []
     # initialize the compile
     for compile_type in COMPILES.keys():
         compile_ = COMPILES[compile_type]()
         compile_list.append(compile_)
     # convert the model
     for compile_ in compile_list:
-        model = compile_(model)
+        model = compile_(model, pattern_config=config)
     return model
 
 
 def compile(model, config=None):
+    """The compile interface.
+
+    Firstly, use model loader to get the computation graph with corresponding framework. 
+    The graph contains nodes and edges, the node is op and the edge is the tensor.
+    Then extract the ops in the graph and pack them to our form.
+    Next exploit these above ops to consist sub-graph, which can see as "a new big op", like LayerNorm.
+
+    Note:
+        There may have different computation flow in one subgraph.
+    Finally, convert them to .yaml file and .bin file for model configuration and inference.
+    """
     if get_model_fwk_name(model) == 'neural engine':
         from .graph import Graph
         graph = Graph()
         graph.graph_init(model + '/conf.yaml', model + '/model.bin')
         model = graph
     else:
+        config = _config_validation(config)
         model = start_pipeline(model, config=config)
     return model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/__init__.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .extractor import Extractor
+"""The neural engine version file."""
+
+__version__ = "1.0b"
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/extractor.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/extractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine base extractor file."""
+
 from .tf_extractor import TensorflowExtractor
 from .onnx_extractor import ONNXExtractor
 from .. import logger
 from ..graph_utils import get_model_fwk_name
 
 EXTRACTORS = {
     'tensorflow': TensorflowExtractor,
     'onnxruntime': ONNXExtractor,
 }
 
 
 class Extractor(object):
-    """
+    """Extractor base class.
+
     A super class for an operation extractor.
     Do additional extraction of operation attributes without modifying of graph topology.
     """
 
-    def __call__(self, model):
+    def __call__(self, model, pattern_config = None):
+        """The __call__ funtion of the base extractor class."""
         framework = model[1]
         extractor = EXTRACTORS[framework]()
         model = extractor(model[0])
         logger.info('Extract {} model done...'.format(framework))
         return model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/onnx_extractor.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/onnx_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,36 +11,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine onnx extractor file."""
 
 from .. import logger
 from ..graph.graph import Graph
 from ..ops.op import OPERATORS
 from ..onnx_utils import graph_node_names_details
 from ..graph_utils import names_from_input
 from intel_extension_for_transformers.backends.neural_engine.compile.ops.tensor import Tensor
 
 
 class ONNXExtractor(object):
-    """
+    """The ONNXExtractor class.
+
     Decorate the node in model.graph_def, and the new node has the attributes like input_tensors
     and output_tensors, these tensors record the source/dest op name. All of these nodes 
     (in a list) will compose a graph, which is Graph class, as the return object.
+
     Args:
         model: ONNXModel
+
     Return:
         Graph: Graph class, the new graph object
-
     """
     @classmethod
     def __call__(self, model):
+        """The __call__ function of the extractor."""
         # onnx_consts = model.initializer()
         graph_nodes_dict = graph_node_names_details(model)
         logger.info('Start to extarct onnx model ops...')
         new_graph = Graph()
         new_graph.framework = 'onnxruntime'
         for graph_input in model.graph.input:
             op_type = 'ONNXINPUT'
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/tf_extractor.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/extractors/tf_extractor.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,35 +11,39 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine tensorflow extractor file."""
 
 from .. import logger
 from ..graph.graph import Graph
 from ..ops.op import OPERATORS
 from ..tf_utils import graph_node_names_details
 from ..graph_utils import names_from_input
 
 
 class TensorflowExtractor(object):
-    """
+    """The tensorflowExtractor Class.
+
     Decorate the node in model.graph_def, and the new node has the attributes like input_tensors
     and output_tensors, these tensors record the source/dest op name. All of these nodes
     (in a list) will compose a graph, which is Graph class, as the return object.
+    
     Args:
         model: TensorflowModel
+
     Return:
         Graph: Graph class, the new graph object
-
     """
     @classmethod
     def __call__(self, model):
+        """The __call__ function of the extractor."""
         nodes = model.graph_def.node
         graph_nodes_dict = graph_node_names_details(nodes)
         logger.info('Start to extarct tensorflow model ops...')
         new_graph = Graph()
         new_graph.framework = 'tensorflow'
         for node in nodes:
             # ignore the Const nodes, they have no source inputs
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/graph/__init__.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/graph/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The module of the neural engine graph."""
+
 from .graph import Graph
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/graph/graph.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/graph/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,77 +11,112 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine graph file."""
+
 import re
-from collections import OrderedDict
+from collections import OrderedDict, namedtuple
 from .. import logger
 import numpy as np
 import yaml
 import os
 import copy
 import time
 
 
 class Graph(object):
+    """The defintion of the neural engine graph."""
     def __init__(self):
+        """The graph initialization."""
         self._nodes = []
         self._node_id = {}
         self._engine = None
+        self._execution_options = None
+        self._refresh_execution_options = False
 
     @property
     def nodes(self):
+        """Get nodes."""
         return self._nodes
 
     @nodes.setter
     def nodes(self, new_nodes):
+        """Nodes assignment."""
         self._nodes = new_nodes
 
+    @property
+    def execution_options(self):
+        """The options for execution."""
+        logger.warning("execution_options' option values are constants. " \
+                    "Please reset the execution_option property if you want change some " \
+                    "options when inference, like 'graph.execution_options = your_new_options'. " \
+                    "Do not use 'graph.execution_options.some_option = value' directly!")
+        import neural_engine_py as dp
+        options = dp.ExecutionOptions()
+        options_list = [option for option in dir(options)
+                            if not option.startswith("__") and not option.startswith("__")]
+        execution_option_ret = namedtuple("ExecutionOptions", options_list)
+        values = [None] * len(options_list)
+        if self._execution_options:
+            values = [getattr(self._execution_options, option) for option in options_list]
+        return execution_option_ret._make(values)
+
+    @execution_options.setter
+    def execution_options(self, options):
+        self._execution_options = options
+        self._refresh_execution_options = True
+
     def insert_nodes(self, index, nodes):
+        """Insert nodes to neural engine IR."""
         idx = index
         for node in nodes:
             node = self.modify_node_connections(node, mode='insert')
             self._nodes.insert(idx, node)
             self._node_id[node.name] = idx
             for i in range(idx + 1, len(self._nodes)):
                 self._node_id[self._nodes[i].name] += 1
             idx += 1
         self._engine = None
 
     def remove_nodes(self, node_names):
+        """Remove nodes from neural engine IR."""
         for node_name in node_names:
             if node_name not in self._node_id.keys():
                 continue
             node = self.get_node_by_name(node_name)
             _ = self.modify_node_connections(node, mode='remove')
             index = self.get_node_id(node_name)
             for i in range(index + 1, len(self._nodes)):
                 self._node_id[self._nodes[i].name] -= 1
             self._nodes.pop(index)
             self._node_id.pop(node_name)
         self._engine = None
 
     def get_node_id(self, node_name):
+        """Get the node id according to the node name."""
         try:
             index = self._node_id[node_name]
             return index
         except BaseException:
             raise ValueError('There is no node named {}, please check the input name.'.format(node_name))
 
     def get_node_by_name(self, node_name):
+        """Get the node according to the node name."""
         index = self.get_node_id(node_name)
         if index is not None:
             return self._nodes[index]
         else:
             return None
 
     def rename_node(self, old_name, new_name):
+        """Modify the node name."""
         index = self.get_node_id(old_name)
         for i in range(len(self._nodes[index].input_tensors)):
             self._nodes[index].input_tensors[i].dest_op = [new_name]
             for pre_node_name in self._nodes[index].input_tensors[i].source_op:
                 tensor_idx = self.get_tensor_idx(pre_node_name, self._nodes[index].input_tensors[i].name)
                 pre_node_idx = self._node_id[pre_node_name]
                 self._nodes[pre_node_idx].output_tensors[tensor_idx].dest_op.remove(old_name)
@@ -97,14 +132,15 @@
 
         self._nodes[index].name = new_name
         self._node_id.pop(old_name)
         self._node_id[new_name] = index
         self._engine = None
 
     def change_node_input_tensors(self, node_name, index, tensor=None, mode='modify'):
+        """Modify the input tensors of the node."""
         assert mode in ['insert', 'remove', 'modify'], 'Wrong mode'
         node = self.get_node_by_name(node_name)
         index = index if index >= 0 else len(node.input_tensors) + index
         node_index = self.get_node_id(node_name)
         source_node_idx = None
         tensor_idx = None
         if mode == 'remove':
@@ -128,14 +164,15 @@
 
         else:
             self.change_node_input_tensors(node_name, index, mode='remove')
             self.change_node_input_tensors(node_name, index, tensor=tensor, mode='insert')
         self._engine = None
 
     def change_node_output_tensors(self, node_name, index, tensor=None, mode='modify'):
+        """Modify the output tensors of the node."""
         assert mode in ['insert', 'remove', 'modify'], 'Wrong mode'
         node = self.get_node_by_name(node_name)
         index = index if index >= 0 else len(node.input_tensors) + index
         node_index = self.get_node_id(node_name)
         if mode == 'remove':
             tensor = node.output_tensors[index]
         assert tensor is not None
@@ -146,32 +183,35 @@
         elif mode == 'remove':
             self._nodes[node_index].output_tensors.pop(index)
         else:
             self._nodes[node_index].output_tensors[index] = tensor
         self._engine = None
 
     def get_pre_node_names(self, node_name):
+        """Get the previous node name."""
         pre_node_names = []
         node = self.get_node_by_name(node_name)
         for input_tensor in node.input_tensors:
             if input_tensor.source_op != []:
                 pre_node_names.extend(input_tensor.source_op)
 
         return pre_node_names
 
     def get_next_node_names(self, node_name):
+        """Get the next node name."""
         next_node_names = []
         node = self.get_node_by_name(node_name)
         for output_tensor in node.output_tensors:
             if output_tensor.dest_op != []:
                 next_node_names.extend(output_tensor.dest_op)
 
         return next_node_names
 
     def get_tensor_idx(self, node_name, tensor_name, from_output=True):
+        """Get the index of tensor."""
         target_node = self.get_node_by_name(node_name)
         tensor_idx = -1
         if from_output:
             target_tensors = target_node.output_tensors
         else:
             target_tensors = target_node.input_tensors
         for j in range(len(target_tensors)):
@@ -182,14 +222,15 @@
                 continue
         # assert tensor_idx != -1, 'Graph does not has tensor {}, '\
         #'please check it.'.format(tensor_name)
 
         return tensor_idx
 
     def modify_node_connections(self, node, mode='insert'):
+        """Modify the order of nodes."""
         assert mode in ['insert', 'remove'], 'Wrong mode {}'.format(mode)
         # modify the input_tensors' source_op
         for i in range(len(node.input_tensors)):
             node.input_tensors[i].dest_op = [node.name]
             t = node.input_tensors[i]
             if t.source_op != [] and t.source_op[0] in self._node_id.keys():
                 source_node_idx = self.get_node_id(t.source_op[0])
@@ -218,17 +259,17 @@
                         tensor_idx = self.get_tensor_idx(dest_op_name, t.name, from_output=False)
                         if tensor_idx != -1:
                             self._nodes[dest_node_idx].input_tensors[tensor_idx].source_op = [node.name]
         self._engine = None
 
         return node
 
-    # get the weight_bytes to bin file
     @property
     def weight_data(self):
+        """Get the weight_bytes to bin file."""
         consts_info = OrderedDict()
         weight_bytes = bytearray()
         non_consts_len = 0
         for t in self._nodes[0].output_tensors:
             assert self._nodes[0].op_type == 'Input', 'The graph must have input data'
             if t.source_op == [] and isinstance(t.data, np.ndarray):
                 break
@@ -244,28 +285,29 @@
                     data_bytes = data.tobytes()
                     weight_bytes.extend(data_bytes)
                     offset = len(data_bytes)
                     self._nodes[i].input_tensors[j].location = [start, offset]
                     self._nodes[0].output_tensors.append(self._nodes[i].input_tensors[j])
         weight_bytes = bytes(weight_bytes)
         return weight_bytes
-
-    # get the network config dict to yaml file
+ 
     @property
     def net_config(self):
+        """Get the network config dict to yaml file."""
         net_info = OrderedDict()
         net_info['model'] = OrderedDict()
         net_info['model']['name'] = 'model'
         net_info['model']['operator'] = OrderedDict()
         for node in self._nodes:
             net_info['model']['operator'][node.name] = node.config
 
         return net_info
 
     def dump_tensor(self, tensor_list=[]):
+        """Dump tensors to the bin and yaml file."""
         weight_data = self.weight_data
         net_info = self.net_config
         if tensor_list == []:
             for node in net_info['model']['operator']:
                 if 'output' in net_info['model']['operator'][node].keys():
                     for tensor in net_info['model']['operator'][node]['output']:
                         if 'location' in \
@@ -281,16 +323,16 @@
                     for tensor_name in operator[node]['output']:
                         search = re.search(tensor, tensor_name, re.I)
                         if search is not None:
                             net_info['model']['operator']['output_data']['input'][tensor_name] = {}
 
         return net_info
 
-    # pybind engine executor
     def engine_init(self, net_info={}, weight_data=b""):
+        """Pybind engine executor."""
         import neural_engine_py as dp
         if not weight_data:
             weight_data = self.weight_data
         if not net_info:
             net_info = self.net_config
         op_configs = []
         tensor_output = []
@@ -330,44 +372,51 @@
                     attr_maps[str(k)] = str(v)
                 attr_map_item = dp.attrs_config(attr_maps)
                 attr_map_list.append(attr_map_item)
             else:
                 attr_map = dp.attrs_config({})
                 attr_map_list.append(attr_map)
             op_type = net_info['model']['operator'][node]['type']
-            op_config = dp.op_config(str(node), str(op_type), tensor_input[-1], tensor_output[-1], attr_map_list[-1])
+            op_config = dp.op_config(str(node), str(op_type), tensor_input[-1], tensor_output[-1],
+                                     attr_map_list[-1])
             op_configs.append(op_config)
 
         model_config = dp.model_config(net_info['model']['name'], op_configs)
         output_list = []
         for node in net_info['model']['operator']['output_data']['input']:
             output_list.append(node)
-        model = dp.Model(model_config, weight_data)
+        if self._execution_options:
+            model = dp.Model(model_config, weight_data, self._execution_options)
+        else:
+            model = dp.Model(model_config, weight_data)
         self._engine = [model, output_list, op_configs, tensor_output, tensor_input, attr_map_list]
 
     def inference(self, input_data):
-        if self._engine is None:
+        """The inference API of the neural engine."""
+        if self._refresh_execution_options or self._engine is None:
             self.engine_init()
+            self._refresh_execution_options = False
         output = self._engine[0].forward(input_data)
         index = 0
         output_dict = OrderedDict()
         for node in self._engine[1]:
             output_dict[node] = output[index]
             index += 1
 
         return output_dict
 
     def graph_init(self, config, weight_data=None):
-        '''
-        example:
+        """The initialization of the neural engine graph.
+
+        for example:
                 from intel_extension_for_transformers.backends.neural_engine.compile.graph import Graph
                 newgraph = Graph()
                 newgraph.graph_init('./ir/conf.yaml', './ir/model.bin')
                 out = newgraph.inference([input_0, input_1, input_2])
-        '''
+        """
         from ..ops import Tensor
         import yaml
         from .. import graph_utils as util
         import copy
         self._nodes = []
         self._node_id = {}
         self._engine = None
@@ -408,16 +457,16 @@
                             "u8": np.uint8,
                             "bf16": np.uint16,
                         }
                         tensor_data = np.frombuffer(tensor_data, dtype=DTYPES_DICT[tensor_dtype]).\
                         reshape(tensor_shape)
                     tensorclass = Tensor()
                     if tensor_location == None:
-                        tensorclass = Tensor(tensor_name, ['input_data'], [], tensor_shape, tensor_data, tensor_dtype,
-                                             tensor_location)
+                        tensorclass = Tensor(tensor_name, ['input_data'], [], tensor_shape, tensor_data,
+                                             tensor_dtype, tensor_location)
                     else:
                         tensorclass = Tensor(tensor_name, [], [], tensor_shape, tensor_data, tensor_dtype,
                                              tensor_location)
                     tensor_name_2_class[tensor_name] = tensorclass
                     output_tensors.append(tensorclass)
                 op = util.construct_node(node, 'Input', [], copy.deepcopy(output_tensors))
 
@@ -440,19 +489,20 @@
                 for tensor_name in d['model']['operator'][node]['input']:
                     tensor = tensor_name_2_class[tensor_name]
                     tensor.dest_op.append(node)
                     input_tensors.append(tensor)
                 if 'attr' in d['model']['operator'][node].keys():
                     attr = d['model']['operator'][node]['attr']
 
-                op = util.construct_node(node, optype, copy.deepcopy(input_tensors), copy.deepcopy(output_tensors),
-                                         attr)
+                op = util.construct_node(node, optype, copy.deepcopy(input_tensors),
+                                         copy.deepcopy(output_tensors), attr)
             self.insert_nodes(len(self.nodes), [op])
 
     def save(self, output_dir=None):
+        """Save the model IR to the bin and ymal file."""
         logger.info("Start to emit the intermediate representation of model...")
         if output_dir is None:
             dir_name = os.getcwd()
             output_dir = os.path.join(dir_name, 'ir/')
 
         output_dir = os.path.abspath(output_dir)
         if not os.path.exists(output_dir):
@@ -481,25 +531,27 @@
             yaml.add_representer(list, list_representer)
             yaml.add_representer(OrderedDict, dict_representer)
             yaml.dump(net_info, f, default_flow_style=False, sort_keys=False)
 
         logger.info("Emit done...")
 
     def graph_dispatch(self, tune=True, inputs_shape=[]):
+        """The graph dispatch for difference nodes."""
         sparse_nodes_name = self.get_sparse_nodes_name()
         if tune:
             logger.info("Tuning graph start ...")
             self._tune_onednn_graph(inputs_shape)
             self._tune_sparse_graph(inputs_shape, sparse_nodes_name)
             logger.info("Tuning graph end ...")
         else:
             # if not tune, map to sparse graph directly
             self.transpose_mode_int8(sparse_nodes_name)
 
     def _tune_onednn_graph(self, inputs_shape=[]):
+        """The onednn graph tuning."""
         onednn_graph_nodes_map = self._get_onednn_graph_nodes()
         if onednn_graph_nodes_map == {"InnerProduct": [], "Softmax": []}:
             pass
         else:
             onednn_graph_nodes_name_list = self._generate_onednn_graph_nodes_name_list(onednn_graph_nodes_map)
             golden_onednn_graph_nodes_name = []
             min_latency = float("inf")
@@ -514,47 +566,51 @@
                 # update min latency and transpose nodes name
                 if curr_latency < min_latency:
                     min_latency = curr_latency
                     golden_onednn_graph_nodes_name = onednn_graph_nodes_name
             self._generate_onednn_graph_nodes(golden_onednn_graph_nodes_name)
 
     def _get_onednn_graph_nodes(self):
-        # onednn graph only support fp32 inner_product and softmax
+        """Onednn graph only support fp32 inner_product and softmax."""
         onednn_graph_nodes_map = {"InnerProduct": [], "Softmax": []}
         for node in self.nodes:
             if node.op_type == "InnerProduct":
                 weight = node.input_tensors[1]
                 if type(weight.data) == np.ndarray and \
                     weight.data.dtype == "float32":
                     onednn_graph_nodes_map["InnerProduct"].append(node.name)
             elif node.op_type == "Softmax":
                 if node.attr.get("output_dtype", "float32") == "float32":
                     onednn_graph_nodes_map["Softmax"].append(node.name)
         return onednn_graph_nodes_map
 
     def _generate_onednn_graph_nodes_name_list(self, onednn_graph_nodes_map):
-        # strategy:
-        # 1.softmax: all nodes map to onednn graph or not
-        # 2.innerproduct: tune accorording weight shape
+        """Strategy.
+
+        1.softmax: all nodes map to onednn graph or not
+        2.innerproduct: tune accorording weight shape
+        """
         ip_nodes_name_list = self._generate_transpose_nodes_name_list(onednn_graph_nodes_map["InnerProduct"])
         onednn_graph_nodes_name_list = []
         for ip_nodes_name in ip_nodes_name_list:
             onednn_graph_nodes_name_list.append(ip_nodes_name)
             onednn_graph_nodes_name_list.append(ip_nodes_name + onednn_graph_nodes_map["Softmax"])
         return onednn_graph_nodes_name_list
 
     def _generate_onednn_graph_nodes(self, onednn_graph_nodes_name):
+        """The onednn graph ndoes generation."""
         for node in self.nodes:
             if node.name in onednn_graph_nodes_name:
                 if node.op_type == "InnerProduct":
                     node.op_type = "InnerProductGraph"
                 elif node.op_type == "Softmax":
                     node.op_type = "SoftmaxGraph"
 
     def _tune_sparse_graph(self, inputs_shape=[], sparse_nodes_name=[]):
+        """The sparse graph tuning."""
         if sparse_nodes_name == []:
             pass
         else:
             trans_nodes_name_list = self._generate_transpose_nodes_name_list(sparse_nodes_name)
             golden_trans_nodes_name = []
             min_latency = float("inf")
             for trans_nodes_name in trans_nodes_name_list:
@@ -568,14 +624,15 @@
                 # update min latency and transpose nodes name
                 if curr_latency < min_latency:
                     min_latency = curr_latency
                     golden_trans_nodes_name = trans_nodes_name
             self.transpose_mode_int8(golden_trans_nodes_name)
 
     def get_sparse_nodes_name(self, threshold=0.7):
+        """According to the sparsity threshold to list all sparse nodes."""
         def get_zero_ratio(matrix, block):
             sparse_ratio = -1
             if matrix.ndim == 2 and len(block) == 2:
                 zero_block_count = 0
                 block_row = int(matrix.shape[0] / block[0])
                 block_col = int(matrix.shape[1] / block[1])
                 for mr in range(block_row):
@@ -612,30 +669,31 @@
                         zero_ratio = get_zero_ratio(weight.data, [1, 4])
                         if zero_ratio >= threshold:
                             sparse_nodes_name.append(node.name)
 
         return sparse_nodes_name
 
     def _generate_transpose_nodes_name_list(self, sparse_nodes_name):
+        """The name list of transpose nodes generation."""
         transpose_nodes_list = []
         if sparse_nodes_name == []:
             return transpose_nodes_list
         # switch the nodes which has the same weight shape and pose op
         weight_shape_map = {}
         for node in self.nodes:
             if node.name in sparse_nodes_name:
                 weight = node.input_tensors[1]
                 weight_shape = tuple(weight.shape)  # list to tuple for dict key
                 if weight_shape in weight_shape_map.keys():
                     weight_shape_map[weight_shape].append(node.name)
                 else:
                     weight_shape_map[weight_shape] = [node.name]
 
-        # binary reflected gray code to generate the all combinations fo the n elements
         def brgd(n):
+            """Binary reflected gray code to generate the all combinations fo the n elements."""
             if n == 1:
                 return ["0", "1"]
             L1 = brgd(n - 1)
             L2 = copy.deepcopy(L1)
             L2.reverse()
             L1 = ["0" + l for l in L1]
             L2 = ["1" + l for l in L2]
@@ -649,14 +707,15 @@
                 if transpose_mask[idx] == "1":
                     transpose_nodes += weight_shape_map[weight_shape]
             transpose_nodes_list.append(transpose_nodes)
 
         return transpose_nodes_list
 
     def _generate_inputs(self, inputs_shape=[]):
+        """The input of nodes generation."""
         dtype_map = {
             "float32": np.float32,
             "int8": np.int8,
             "int32": np.int32,
             "int64": np.int64,
             "uint8": np.uint8,
         }
@@ -673,42 +732,46 @@
                         dtype = dtype_map[tensor.dtype]
                         input = np.random.uniform(low=0, high=10, size=shape).astype(dtype)
                         inputs.append(input)
                         id += 1
         return inputs
 
     def _get_latency(self, inputs_shape=[], iterations=10, warm_up=5):
+        """Calculate the latency."""
         inputs = self._generate_inputs(inputs_shape)
         iter_latency = []
         for _ in range(iterations):
             start_time = time.time()
             result = self.inference(inputs)
             end_time = time.time()
             iter_latency.append(end_time - start_time)
         latency = np.array(iter_latency[warm_up:]).mean()
         return result, latency
 
     def transpose_mode_int8(self, node_name_list=None):
+        """Transpose innerproduct nodes to the sparse mode by inserting reorder nodes."""
         from ..ops import Tensor
         from .. import graph_utils as util
         import copy
         logger.info("Start to transpose_mode_int8 ......")
         reorder_dict = {}
 
         def _modify_attr_perm(node):
+            """Transpose the node attr perm."""
             if node.attr.get("src0_perm") == '0,2,1,3' and node.attr.get("src1_perm") == '0,2,3,1':
                 node.attr["src0_perm"] = '2,0,3,1'
                 node.attr["src1_perm"] = '2,0,1,3'
             if node.attr.get("src1_perm") == '0,2,1,3' and node.attr.get("dst_perm") == '0,2,1,3':
                 node.attr["src1_perm"] = '2,0,3,1'
                 node.attr["dst_perm"] = '1,3,0,2'
             if 'reshape' in node.attr:
                 _reorder_shape_list(node, 'reshape')
 
         def _innerproduct_type_check(node):
+            """Check the innerproduct node type."""
             innerproduct_type = {
                 # general_node
                 "general": "general",
 
                 # InnerProduct Nodes
                 "QKV_innerproduct": 'add_innerproduct_0',
                 'output_dense_bias': 'add_innerproduct_1',
@@ -728,17 +791,15 @@
 
             if node.op_type == 'Matmul':
                 return innerproduct_type['matmul_type']
             else:
                 return innerproduct_type['general']
 
         def _create_new_attr(node, mode=None):
-            '''
-                If there is a dtype, the output_dtype of the inserted reorder node is the same as the input node dtype
-            '''
+            """The output_dtype of the inserted reorder node is the same as the input node dtype if dtype exists."""
             if mode == 'Reorder_Post':
                 new_attr = OrderedDict({'src_perm': '0,1', 'dst_perm': '1,0'})
                 if 'output_dtype' in node.attr:
                     new_attr['output_dtype'] = node.attr['output_dtype']
                 return new_attr
 
             if mode == 'Reorder_Recover':
@@ -749,20 +810,21 @@
                     else:
                         logger.info('The length of value_list is wrong')
                 else:
                     new_attr = OrderedDict({'src_perm': '0,1', 'dst_perm': '1,0'})
 
                 if 'output_dtype' in node.attr:
                     new_attr['output_dtype'] = node.attr['output_dtype']
-                
+
                 return new_attr
 
             return False
 
         def _dfs_search(node, target_node_type):
+            """Use the deep-first algorithm to search the node accroding to the its type."""
             target_node = []
 
             def dfs(node):
                 if node.op_type == target_node_type:
                     return node
                 if node.output_tensors[0].dest_op == []:
                     return None
@@ -778,28 +840,32 @@
             dfs(node)
             if target_node == []:
                 return None
             else:
                 return target_node[0]
 
         def _reorder_shape_list(node, attr_name='dst_shape'):
+            """Transpose the shape attribute."""
             value_list = node.attr[attr_name].split(',')
             if len(value_list) == 4:
                 value = value_list[2] + ',' + value_list[3] + ',' + value_list[0] + ', ' + value_list[1]
 
             if len(value_list) == 2:
                 value = value_list[1] + ',' + value_list[0]
 
             node.attr[attr_name] = value
 
         def _reorder_node_insert(node, idx, insert_pos=None):
-            '''
-                idx: the position of variables that need to be transposed in node.input_tensors
-                insert_pos: the position of insert
-            '''
+            """Reorder node insert.
+            
+            Args:
+                node: the current innerproduct node.
+                idx: the position of variables that need to be transposed in node.input_tensors.
+                insert_pos: the position of insert.
+            """
             # check the node whether has been reordered
             for index_node, reorder_node in reorder_dict.items():
                 if node.input_tensors[idx].name == reorder_node.input_tensors[0].name:
                     # the variable that need to be transposed has been reordered.
                     node.input_tensors[idx] = reorder_node.output_tensors[0]
                     # append the current node to the reorder node output_tensors[0].dest_op
                     reorder_node.output_tensors[0].dest_op.append(node.name)
@@ -825,17 +891,15 @@
             if insert_pos != None:
                 reorder_dict[insert_pos.name] = reorder_node
             else:
                 reorder_dict[node.name] = reorder_node
             return reorder_node
 
         def _swap_innertproduct_input(node, data_swap_list=[0, 1], swap_list_2=[], swap_list_3=[]):
-            '''
-                modify innertproduct nodes and the folloing reshape nodes.
-            '''
+            """Modify innertproduct nodes and the folloing reshape nodes."""
             input_0 = data_swap_list[0]
             input_1 = data_swap_list[1]
             # swap(input_0, input1)
             node.input_tensors[input_1].data = np.ascontiguousarray(node.input_tensors[input_1].data.T)
             node.input_tensors[input_1].shape = list(node.input_tensors[input_1].data.shape)
             tmp_node = copy.deepcopy(node.input_tensors[input_1])
             node.input_tensors[input_1] = node.input_tensors[input_0]
@@ -853,18 +917,29 @@
             node.input_tensors[input_4] = node.input_tensors[input_6]
             node.input_tensors[input_6] = tmp_node
             if 'src1_perm' in node.attr:
                 node.attr.pop('src1_perm')
             if 'reshape' in node.attr:
                 _reorder_shape_list(node, 'reshape')
 
-        def reorder_recover_node_insert(node, pre_node=None):
-            '''
-                pre_node: the first predecessor node of the reorder_recover node
-            '''
+        def _modify_post_node_attr(post_node, attr_name='axis'):
+            """Modify the post node attribute."""
+            if attr_name in post_node.attr:
+                if post_node.attr[attr_name] == 0:
+                    post_node.attr[attr_name] = 1
+                elif post_node.attr[attr_name] == 1:
+                    post_node.attr[attr_name] = 0
+
+        def _reorder_recover_node_insert(node, pre_node=None):
+            """Reorder_recover node insert.
+            
+            Args:
+                node: the current innerproduct node.
+                pre_node: the first predecessor node of the reorder_recover node.
+            """
             post_node = self.get_node_by_name(node.output_tensors[0].dest_op[0])
             if len(node.output_tensors[0].dest_op) != 1:
                 logger.info("the post node is not only one.")
             reorder_recover_node_name = node.name + '_Reorder_Recover'
 
             if pre_node != None:
                 pre_node_output = pre_node.output_tensors[0]
@@ -892,132 +967,117 @@
             for _ in post_node.input_tensors:
                 if node.output_tensors[0].name == _.name:
                     break
                 else:
                     idx = idx + 1
 
             post_node.input_tensors[idx] = reorder_output_tensor
+            _modify_post_node_attr(post_node, 'axis')
             return reorder_recover_node
 
-        def modify_post_node_input_tensor(post_node, node, node_input_tensors_idx=0):
-            '''
+        def _modify_post_node_input_tensor(post_node, node, node_input_tensors_idx=0):
+            """Modify the input tensors of the post node.
+
+            Args:
                 post_node: the post node of the second parameter
                 node: the source of input_tensors
                 node_input_tensors_idx: assign the index of node.input_tensors to post_node.input_tensors
-            '''
+            """
             idx = 0
             for _ in post_node.input_tensors:
                 if node.output_tensors[0].name == _.name:
                     break
                 else:
                     idx = idx + 1
             post_node.input_tensors[idx] = node.input_tensors[node_input_tensors_idx]
             return
 
         def _del_current_node_and_modify_post_node(node):
+            """Delete the current node and then modify input tensors of the post node."""
             pre_node = self.get_node_by_name(node.input_tensors[0].source_op[0])
             for post_node_name in node.output_tensors[0].dest_op:
                 post_node = self.get_node_by_name(post_node_name)
-                modify_post_node_input_tensor(post_node, node, 0)
+                _modify_post_node_input_tensor(post_node, node, 0)
             self.remove_nodes([node.name])
             for post_node_name in node.output_tensors[0].dest_op:
                 post_node = self.get_node_by_name(post_node_name)
+                _modify_post_node_attr(post_node, 'axis')
                 pre_node.output_tensors[0].dest_op.append(post_node.name)
 
-        if node_name_list == None:
-            logger.info("The node_name_list is None. Start to get sparse nodes name...")
-            node_name_list = self.get_sparse_nodes_name()
-        
-        logger.info('node_name_list: %s', node_name_list)
-
-        if node_name_list == []:
-            logger.info("The node_name_list is [].")
-            return
-
-        def node_name_list_convert(node_name_list):
-            type_list = ''
+        def _node_name_list_convert(node_name_list):
+            """List all innerproduct node types."""
+            merge_matmul_node_name_list = []
+            innerproduct_type = []
             for node_name in node_name_list:
                 node = self.get_node_by_name(node_name)
                 node_type = _innerproduct_type_check(node)
-                if node_type == 'add_innerproduct_0':
-                    type_list += '0'
-                if node_type == 'add_innerproduct_1':
-                    type_list += '1'
-                if node_type == 'mul_innerproduct_0':
-                    type_list += '2'
-            return type_list
+                innerproduct_type.append(node_type)
+                if node_type == 'add_innerproduct_0' or node_type == 'mul_innerproduct_0':
+                    if 'merge_matmul' in node.name:
+                        merge_matmul_node_name_list.append(node_name)
 
-        type_list = node_name_list_convert(node_name_list)
+            return innerproduct_type, merge_matmul_node_name_list
 
-        def _patthen_match(type_list, pattern):
+        def _pattern_matching(innerproduct_type_list, pattern):
+            """Matching the pattern accroding to innerproduct node types."""
             matched_idx = []
-            idx = type_list.find(pattern)
-            while idx != -1:
-                matched_idx.append(idx)
-                idx = type_list.find(pattern, idx + 1)
+            pattern_length = len(pattern)
+
+            left = 0
+            N = len(innerproduct_type_list)
+            while left < N:
+
+                def _check(left):
+                    if pattern == innerproduct_type_list[left:left + pattern_length]:
+                        return True
+                    return False
+
+                if _check(left) == True:
+                    matched_idx.append(left)
+                left += 1
 
             return matched_idx
 
         def _matched_node_name_list(node_name_list, matched_idx, range=4):
+            """The list of matched nodes."""
             tmp_node_name_list = []
             for node_idx in matched_idx:
                 tmp_node_name_list.append(node_name_list[node_idx:node_idx + range])
             node_name_list = [i for item in tmp_node_name_list for i in item]
             return node_name_list
 
-        QKV_and_bias = '0001'
-        matched_idx = _patthen_match(type_list, QKV_and_bias)
-        QKV_node_name_list = _matched_node_name_list(node_name_list, matched_idx, 4)
-
-        geluTanh_and_sum = '21'
-        matched_idx = _patthen_match(type_list, geluTanh_and_sum)
-        post_process_node_name_list = _matched_node_name_list(node_name_list, matched_idx, 2)
-
-        def _check_layernorm_fusion_node(post_process_node_name_list, start_idx, range):
+        def _search_layernorm_fusion_node(ffn_lin_node_name_list, start_idx, range, node_name_list=[]):
+            """Search nodes related to layernorm that can be fused."""
             layernorm_node = []
-            for node_name in post_process_node_name_list[start_idx:][::range]:
+            # pcik all add_innerproduct_1 nodes from ffn_lin_node_name_list
+            for node_name in ffn_lin_node_name_list[start_idx:][::range]:
+                # The node_name_list here is also to identify the merge matmul pattern.
+                if node_name_list != []:
+                    split_node_name = self.get_node_by_name(node_name).output_tensors[0].dest_op[0]
+                    length_of_split_node_output = len(self.get_node_by_name(split_node_name).output_tensors)
+                    if length_of_split_node_output == 3:
+                        node_name = node_name_list[node_name_list.index(node_name) + 1]
+                    elif length_of_split_node_output == 2:
+                        node_name = node_name_list[node_name_list.index(node_name) + 2]
+                    else:
+                        logger.warning('The output of the split node is not expected.')
+
                 layernorm_node_name = self.get_node_by_name(node_name).input_tensors[3].source_op[0]
                 node = self.get_node_by_name(layernorm_node_name)
                 if node.op_type != 'LayerNorm':
-                    logger.warning('Post Process Pattern matching wrong')
+                    logger.warning('Post Process Pattern matching is not expected')
                 else:
                     layernorm_node.append(node.name)
             return layernorm_node
 
-        layernorm_fusion_node = _check_layernorm_fusion_node(post_process_node_name_list, 1, 2)
-        layernorm_fusion_node += _check_layernorm_fusion_node(QKV_node_name_list, 3, 4)
-
-        for node_name in node_name_list:
-            node = self.get_node_by_name(node_name)
-            node_type = _innerproduct_type_check(node)
-            if node_type == 'general':
-                continue
-
-            if node_type == 'add_innerproduct_0' or node_type == 'mul_innerproduct_0':
-                _reorder_node_insert(node, 0)
-                _swap_innertproduct_input(node, [0, 1], [3, 5], [4, 6])
-                reorder_recover_node_insert(node)
-
-            if node_type == 'add_innerproduct_1':
-                reorder_node = _reorder_node_insert(node, 0)
-                reorder_node.attr['output_dtype'] = 'u8'
-                _reorder_node_insert(node, 3, reorder_node)
-
-                _swap_innertproduct_input(node, [0, 1], [4, 6], [5, 7])
-                reorder_recover_node_insert(node)
-
-        for node_name in reorder_dict:
-            insert_idx = self.get_node_id(node_name)
-            self.insert_nodes(insert_idx, [reorder_dict[node_name]])
- 
         def _consecutive_reorder_fusion():
-            '''
-                Fusion 1: 
-                eliminate the two reorder nodes if a tensor passes through reorder_recover + reorder_post consecutively
-            '''
+            """Fusion 1.
+            
+            eliminate the two reorder nodes if a tensor passes through reorder_recover + reorder_post consecutively
+            """
             for node in self._nodes:
                 if node.op_type == 'Reorder' and 'recover_reorder' in node.output_tensors[0].name:
                     if 'Reorder_Post' in node.name:
                         pre_node = self.get_node_by_name(node.input_tensors[0].source_op[0])
                         if 'Reorder_Recover' in pre_node.name and pre_node.op_type == 'Reorder':
                             post_node = self.get_node_by_name(node.output_tensors[0].dest_op[0])
                             idx = 0
@@ -1026,75 +1086,101 @@
                                     break
                                 else:
                                     idx = idx + 1
                             post_node.input_tensors[idx] = pre_node.input_tensors[0]
                             self.remove_nodes([pre_node.name, node.name])
                             pre_node.input_tensors[0].dest_op.append(post_node.name)
 
-        _consecutive_reorder_fusion()
-
-        reorder_dict = {}
-
         def _reorder_post_fusion():
-            '''
-                Fusion 2: 
-                Place reorder_post nodes before the quantize node, especially for QKV and output dense
-            '''
-            def _check_QKV_fusion(node):
-                post_node = self.get_node_by_name(node.output_tensors[0].dest_op[0])
-                node_type = _innerproduct_type_check(post_node)
+            """Fusion 2.
+            
+            This fusion is used to place reorder_post nodes before the quantize node.
+            Conditions:
+                Only fusion if all QKV nodes meet the sparsity ratio
+
+            E.g.
+                original: quantize + reorder_post + innerproduct: K + innerproduct: Q + innerproduct: v
+                fusion: reorder_post + quantize + innerproduct: K + innerproduct: Q + innerproduct: v
+            """
+            # check the current reorder_post_node whether need place reorder_post nodes before the quantize node
+            def _check_QKV_fusion(reorder_post_node):
+                innerproduct_node = self.get_node_by_name(reorder_post_node.output_tensors[0].dest_op[0])
+                node_type = _innerproduct_type_check(innerproduct_node)
+
+                # This branch is used to check type of the attention out node.
                 if node_type == 'mul_innerproduct_0':
                     return True
-                for post_node_name in node.output_tensors[0].dest_op:
-                    if post_node_name in QKV_node_name_list:
+
+                # The dest_op of reorder_post_node.output_tensors[0] are QKV nodes.
+                for QKV_node_name in reorder_post_node.output_tensors[0].dest_op:
+                    if QKV_node_name in QKV_node_name_list:
                         continue
                     else:
                         return False
+                # only when all QKV nodes are in the QKV node name list return true
+                return True
+
+            def _check_merged_matmul(reorder_post_node):
+                """Check if the node is in the merged matmul node name list."""
+                innerproduct_node = self.get_node_by_name(reorder_post_node.output_tensors[0].dest_op[0])
+                if innerproduct_node.name not in merge_matmul_node_name_list:
+                    return False
                 return True
 
             for node in self._nodes:
+                # search all Reorder_Post nodes
                 if node.op_type == 'Reorder' and 'Reorder_Post' in node.name:
-                    pre_node = self.get_node_by_name(node.input_tensors[0].source_op[0])
                     if _check_QKV_fusion(node) == False:
-                        continue
+                        if _check_merged_matmul(node) == False:
+                            continue
+
+                    pre_node = self.get_node_by_name(node.input_tensors[0].source_op[0])
                     if pre_node.op_type == 'Quantize':
                         # swap the pre_node and the current node
                         for post_node_name in node.output_tensors[0].dest_op:
                             post_node = self.get_node_by_name(post_node_name)
-                            modify_post_node_input_tensor(post_node, node, 0)
+                            _modify_post_node_input_tensor(post_node, node, 0)
                         self.remove_nodes([node.name])
                         reorder_node = _reorder_node_insert(pre_node, 0)
                         layernorm_node = self.get_node_by_name(reorder_node.input_tensors[0].source_op[0])
+                        if layernorm_node.op_type != 'LayerNorm':
+                            logger.warning('The node.op_type = {} is not expected.'.format(
+                                layernorm_node.op_type))
 
+                        # the dest_op of layernorm_node.output_tensors[0] is reorder_post node for attention out node.
                         if 'Reorder_Post' in layernorm_node.output_tensors[0].dest_op[0]:
-                            reorder_post_node = self.get_node_by_name(layernorm_node.output_tensors[0].dest_op[0])
-                            post_node = self.get_node_by_name(reorder_post_node.output_tensors[0].dest_op[0])
+                            reorder_post_node = self.get_node_by_name(
+                                layernorm_node.output_tensors[0].dest_op[0])
+                            attention_out_node = self.get_node_by_name(
+                                reorder_post_node.output_tensors[0].dest_op[0])
                             self.remove_nodes([reorder_post_node.name])
                             # append the new reorder_node
                             layernorm_node.output_tensors[0].dest_op.append(reorder_node.name)
-                            reorder_node.output_tensors[0].dest_op.append(post_node.name)
+                            reorder_node.output_tensors[0].dest_op.append(attention_out_node.name)
 
             for node_name in reorder_dict:
                 insert_idx = self.get_node_id(node_name)
                 self.insert_nodes(insert_idx, [reorder_dict[node_name]])
 
-        _reorder_post_fusion()
-
         def _reorder_recover_fusion():
-            '''
-                Fusion 3: place the reorder_recover nodes after reshape and matmul nodes
-            '''
+            """Fusion 3: place the reorder_recover nodes after reshape and matmul nodes.
+
+            This fusion deletes the reorder_recover nodes that follow Q, K, V and attention out nodes
+            and the post modify add_matmul and transpose_matmul nodes.
+            """
             for node in self._nodes:
                 # step1: delte all recover nodes of innerProduct nodes and modify reshape inputs
                 node_type = _innerproduct_type_check(node)
                 if node_type == 'add_innerproduct_0' and node.name in QKV_node_name_list:
                     post_node = self.get_node_by_name(node.output_tensors[0].dest_op[0])
                     # innerproduct + reorder_recover + reshape
                     if 'Reorder_Recover' in post_node.name:
                         _del_current_node_and_modify_post_node(post_node)
+
+                        # This conditional branch will be skipped if the innerproduct node fuses the reshape node.
                         reshape_node = self.get_node_by_name(post_node.output_tensors[0].dest_op[0])
                         if reshape_node.op_type == 'Reshape':
                             _reorder_shape_list(reshape_node)
 
                         # step2 : modify add_matmul and transpose_matmul nodes
                         target_node = _dfs_search(node, 'Matmul')
                         if _innerproduct_type_check(target_node) == 'matmul_0':
@@ -1102,28 +1188,196 @@
                             def _transpose_and_matmul_nodes_modification(node):
                                 _modify_attr_perm(node)
                                 reshape_node = self.get_node_by_name(node.output_tensors[0].dest_op[0])
                                 if reshape_node.op_type == "Reshape":
                                     _reorder_shape_list(reshape_node)
 
                                 reorder_node = _dfs_search(node, 'Reorder')
-                                innerproduct_node = self.get_node_by_name(reorder_node.output_tensors[0].dest_op[0])
+                                innerproduct_node = self.get_node_by_name(
+                                    reorder_node.output_tensors[0].dest_op[0])
                                 if 'Reorder_Post' in reorder_node.name and innerproduct_node.op_type == "InnerProduct":
                                     _del_current_node_and_modify_post_node(reorder_node)
 
                             _transpose_and_matmul_nodes_modification(target_node)
-
-        _reorder_recover_fusion()
+                    else:
+                        logger.warning('The node op_type == {} is not expected.'.format(post_node.name))
 
         def _layernorm_reorder_fusion():
+            """The fusion of layernorm reorder."""
             for node in self._nodes:
                 if node.op_type == 'LayerNorm' and node.name in layernorm_fusion_node:
                     reorder_recover_node = self.get_node_by_name(node.input_tensors[0].source_op[0])
                     reorder_post_node = self.get_node_by_name(node.output_tensors[0].dest_op[0])
+
                     if 'Reorder_Recover' in reorder_recover_node.name and 'Reorder_Post' in reorder_post_node.name:
                         node.attr['transpose_mode'] = '1, 0'
                         _del_current_node_and_modify_post_node(reorder_recover_node)
                         _del_current_node_and_modify_post_node(reorder_post_node)
 
+        def _merged_matmul_fusion():
+            """The fusition of merged matmul."""
+            def _transpose_matmul_modification(node):
+                reorder_node = self.get_node_by_name(node.output_tensors[0].dest_op[0])
+                attention_out_node = self.get_node_by_name(reorder_node.output_tensors[0].dest_op[0])
+                if attention_out_node.op_type == "InnerProduct":
+                    _del_current_node_and_modify_post_node(reorder_node)
+                else:
+                    logger.warning('The attention_out_node.op_type = {} is not expected'.format(
+                        attention_out_node.op_type))
+
+            for node_name in node_name_list:
+                node = self.get_node_by_name(node_name)
+
+                if 'merge_matmul' not in node.name:
+                    continue
+
+                reorder_recover_node = self.get_node_by_name(node.output_tensors[0].dest_op[0])
+
+                if 'Reorder_Recover' in reorder_recover_node.name:
+                    _del_current_node_and_modify_post_node(reorder_recover_node)
+                    split_node = self.get_node_by_name(reorder_recover_node.output_tensors[0].dest_op[0])
+
+                    def mergedQK_modify(split_node):
+                        for post_tensor in split_node.output_tensors:
+                            post_node = self.get_node_by_name(post_tensor.dest_op[0])
+
+                            # Reshape + Matmul + Softmax
+                            if post_node.op_type == 'Reshape':
+                                _reorder_shape_list(post_node)
+                                post_node_of_reshape = self.get_node_by_name(
+                                    post_node.output_tensors[0].dest_op[0])
+                                if post_node_of_reshape.op_type == 'Matmul':
+                                    _modify_attr_perm(post_node_of_reshape)
+
+                        # InnerProduct V + Matmul + InnerProduct Attention_output
+                        # delete the recover node of InnerProduct v
+                        split_node_id = self.get_node_id(split_node.name)
+                        next_node_id = split_node_id + 1
+                        v = self._nodes[next_node_id]
+
+                        if v.op_type == 'InnerProduct':
+                            recover_node = self.get_node_by_name(v.output_tensors[0].dest_op[0])
+                            _del_current_node_and_modify_post_node(recover_node)
+                        else:
+                            logger.warning('The v.op_type is not expected.')
+
+                        # modify the matmul node
+                        post_node_of_v = self.get_node_by_name(v.output_tensors[0].dest_op[0])
+                        # This branch is only used if there is no reshaping + innerproduct fusion.
+                        if post_node_of_v.op_type == 'Reshape':
+                            _reorder_shape_list(post_node_of_v)
+                            post_node_of_reshape = self.get_node_by_name(
+                                post_node_of_v.output_tensors[0].dest_op[0])
+                            if post_node_of_reshape.op_type == 'Matmul':
+                                _modify_attr_perm(post_node_of_reshape)
+                                tmp_node = self.get_node_by_name(
+                                    post_node_of_reshape.output_tensors[0].dest_op[0])
+                                if tmp_node.op_type == "Reshape":
+                                    _reorder_shape_list(tmp_node)
+                                    _transpose_matmul_modification(tmp_node)
+                        elif post_node_of_v.op_type == 'Matmul':
+                            _modify_attr_perm(post_node_of_v)
+                            _transpose_matmul_modification(post_node_of_v)
+                        else:
+                            logger.warning('The mergedQK fusion is not expected.')
+
+                    def mergedQKV_modify(split_node):
+                        for post_tensor in split_node.output_tensors:
+                            post_node = self.get_node_by_name(post_tensor.dest_op[0])
+                            # 3 * Reshape + Matmul + Innerproduct_Sum
+                            if post_node.op_type == 'Reshape':
+                                _reorder_shape_list(post_node)
+                                matmul_node = self.get_node_by_name(post_node.output_tensors[0].dest_op[0])
+                                if matmul_node.op_type == 'Matmul':
+                                    _modify_attr_perm(matmul_node)
+                                    post_node_of_matmul = self.get_node_by_name(
+                                        matmul_node.output_tensors[0].dest_op[0])
+                                    # post_node_of_matmul could also be softmax.
+                                    if post_node_of_matmul.op_type == 'Reorder':
+                                        _del_current_node_and_modify_post_node(post_node_of_matmul)
+                                else:
+                                    logger.warning('The post_node_of_reshape is not Matmul.')
+
+                    if len(split_node.output_tensors) == 2:
+                        mergedQK_modify(split_node)
+
+                    if len(split_node.output_tensors) == 3:
+                        mergedQKV_modify(split_node)
+
+        for node in self._nodes:
+            if node.op_type == 'Reorder':
+                logger.info('The current IR is reordered, No need to do transpose.')
+                return
+
+        if node_name_list == None:
+            logger.info("The node_name_list is None. Start to get sparse nodes name...")
+            node_name_list = self.get_sparse_nodes_name()
+
+        logger.info('node_name_list: %s', node_name_list)
+
+        if node_name_list == []:
+            logger.info("The node_name_list is [].")
+            return
+
+        innerproduct_type_list, merge_matmul_node_name_list = _node_name_list_convert(node_name_list)
+        logger.debug('merge_matmul_node_name_list = {}'.format(merge_matmul_node_name_list))
+
+        QKV_and_AttentionOut = [
+            'add_innerproduct_0', 'add_innerproduct_0', 'add_innerproduct_0', 'add_innerproduct_1'
+        ]
+        matched_idx = _pattern_matching(innerproduct_type_list, QKV_and_AttentionOut)
+        QKV_node_name_list = _matched_node_name_list(node_name_list, matched_idx, 4)
+        logger.debug('QKV_node_name_list = {}'.format(QKV_node_name_list))
+
+        ffn_lin = ['mul_innerproduct_0', 'add_innerproduct_1']
+        matched_idx = _pattern_matching(innerproduct_type_list, ffn_lin)
+        ffn_lin_node_name_list = _matched_node_name_list(node_name_list, matched_idx, 2)
+        logger.debug('ffn_lin_node_name_list = {}'.format(ffn_lin_node_name_list))
+
+        layernorm_fusion_node = _search_layernorm_fusion_node(ffn_lin_node_name_list, 1, 2)
+        layernorm_fusion_node += _search_layernorm_fusion_node(QKV_node_name_list, 3, 4)
+        if merge_matmul_node_name_list != []:
+            layernorm_fusion_node += _search_layernorm_fusion_node(merge_matmul_node_name_list, 0, 1,
+                                                                   node_name_list)
+        logger.debug('layernorm_fusion_node = {}'.format(layernorm_fusion_node))
+
+        for node_name in node_name_list:
+            node = self.get_node_by_name(node_name)
+            node_type = _innerproduct_type_check(node)
+
+            if node_type == 'general':
+                continue
+
+            if node_type == 'add_innerproduct_0' or node_type == 'mul_innerproduct_0':
+                _reorder_node_insert(node, 0)
+                _swap_innertproduct_input(node, [0, 1], [3, 5], [4, 6])
+                _reorder_recover_node_insert(node)
+
+            if node_type == 'add_innerproduct_1':
+                reorder_node = _reorder_node_insert(node, 0)
+                reorder_node.attr['output_dtype'] = 'u8'
+                _reorder_node_insert(node, 3, reorder_node)
+
+                _swap_innertproduct_input(node, [0, 1], [4, 6], [5, 7])
+                _reorder_recover_node_insert(node)
+
+        for node_name in reorder_dict:
+            insert_idx = self.get_node_id(node_name)
+            self.insert_nodes(insert_idx, [reorder_dict[node_name]])
+
+        _consecutive_reorder_fusion()
+
+        reorder_dict = {}
+        _reorder_post_fusion()
+
+        _reorder_recover_fusion()
+
         _layernorm_reorder_fusion()
 
+        if merge_matmul_node_name_list == []:
+            logger.info('No mergedMatmul nodes, No need do merged matmul fusion')
+            return
+
+        reorder_dict = {}
+        _merged_matmul_fusion()
+
         logger.info("Transpose_mode_int8 done")
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/graph_utils.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/graph_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine graph utils."""
+
 from . import logger 
 import copy
 import re
 import os
 import numpy as np
 from collections import namedtuple, OrderedDict
 from schema import Schema, And, Or
@@ -33,16 +35,18 @@
                "uint8": "u8",
                "uint16": "bf16",
                }
 
 
 def names_from_input(name):
     """Static method that get the valid node / tensor name from input name.
+
     Args:
         name (string): name defined in the input field.
+
     Returns:
         string tuple: (node's name, tensor's name)
 
     for example: In NodeDef.input, the name from list is tensor name, may not end with ':0',
                 which can not be used for tensor name in the new Graph class. If it end with ':0',
                 it can not also be used for node name in the new Graph class
     """
@@ -58,53 +62,61 @@
         node_name = m.group(1)
         tensor_name = name
 
     return (node_name, tensor_name)
 
 
 def get_data_dtype(data):
-    """Get the const data dtype
+    """Get the const data dtype.
+
     Args:
        data (numpy data): a const data to model
+
     Returns:
        dtype (String): the value in DTYPES_DICT
     """
     dtype = None
     if np.issubdtype(data.dtype, np.integer) or np.issubdtype(data.dtype, np.floating):
         try:
             dtype = DTYPES_DICT[str(data.dtype[0])]
         except BaseException:
             dtype = DTYPES_DICT[str(data.dtype)]
 
     return dtype
 
 def quant_info_init(): 
+    """Initialize the quant info."""
     global _quant_info
     _quant_info = {}
 
 def insert_quant_info(key, value):
+    """Modify the quant info."""
     _quant_info[key] = value
  
 def get_quant_info():
+    """Get the quant info."""
     return _quant_info
 
 def search_straight_pattern(input_pattern, graph):
-    """search user specified patterns on internal grpah structure.
+    """Search user specified patterns on internal grpah structure.
+
     Attention: the input computation chain in the graph which can be called pattern, there must be
                 straight (or sequence). It means it has not any subgraph nodes. Otherwise this
                 function returns []
+
     Args:
         input_pattern (list): Contains the op_type of the nodes in pattern. The element of the
         list could be string/list/tuple, string or list means the specified op_type are mandatory
         while tuple stands for optional.
         For example, a input pattern mybe like this:
         ['Mul', 'Mul', ['Add', 'AddV2']] it equals to below patterns:
         'Mul' + 'Mul' + 'Add'
         'Mul' + 'Mul' + 'AddV2'
         graph: Graph Class, the new graph generated from extractor.
+
     Returns: [string list]. The length is the matched pattern results in the graph, for example,
             the graph has 24 layers and each layer has a 'LayerNorm' pattern, then the length is
             24. Each match pattern result is still a list contains the node names, and the last
             element is the op_type list corresponding to the former node names.
             For example, the return result maybe like this:
             [
                 ['Mul' node name,
@@ -117,42 +129,46 @@
                 'AddV2' node name,
                 ['Mul', 'Mul', 'AddV2']],
 
                 ...
             ]
     """
     def _validate_input(data, creteria):
+        """Validation of input data."""
         if isinstance(creteria, str) and data == creteria:
             return True
 
         if isinstance(creteria, (list, tuple)) and data in creteria:
             return True
 
         return False
 
     def _compare_list(list_a, list_b):
         """Check list a is a subset of list b.
+
         e.g, list a is ['a', 'b', 'c'] while list b is ['a', 'b', 'c', 'd'],
         then list a is subset of list b.
         Args:
             list_a ([Any]): list A
             list_b ([Any]): list B
+
         Returns:
             [bool]: list a is a subset of list b or not.
         """
         assert isinstance(list_a, list)
         assert isinstance(list_b, list)
         is_subset = True
 
         for index, value in enumerate(list_a):
             is_subset &= value == list_b[index]
 
         return is_subset
 
     def _dfs(op_names, op_types, node, pattern):
+        """Use depth-first algorithm to search for patterns according to node types."""
         if pattern == []:
             return
         start_index = 0
         end_index = len(pattern) - 1
         matched_flag = False
         while start_index <= end_index:
             matched_flag = _validate_input(node.op_type, pattern[end_index])
@@ -248,14 +264,15 @@
             final_output.append(i)
 
     return final_output
 
 
 def search_pattern(pattern_list, graph):
     """Search the complete pattern in the graph.
+
     Args:
         pattern_list: a list contains  pattern representation. The pattern representation is also
                       a list and each node in the list is a tuple, its form is like "(op_idx,
                       op_type)". However, due to a few complicated patterns, they have sub-graph
                       computation flow. Therefore in a pattern representation, using the fist list
                       represents the main top-down computation flow (from pattern head op to tail
                       op), the left lists represent sub-graphs (their tail nodes must in the main
@@ -265,15 +282,15 @@
                         (4, 'Rsqrt'), (5, 'Mul'), (7 ,'Mul'), (8, 'Sub'), (9, 'AddV2')],
                         [(5, 'Mul'), (6, 'Mul'), (9, 'AddV2')] ]
 
         graph: Graph Class, the new graph generated from extractor
 
     Returns: [string list], as same as search_straight_pattern func.
 
-    NOTE:
+    Note:
         1. The op_idx follows the order in the original frozen model, which means you had better
            not identify them on your own casually.
         2. the main top-down computation flow follows the "tf control flow". It's a straight chain
            from start to end in the pattern. Mostly, it has the longest path. Sometimes, this main
            flow may have sub connection. But you don't need to represent them. A sub-graph must
            have one op at least that doesn't exist in the main chain. For example, in the above
            LayerNorm pattern, (0, 'Mean') has a connection with (7 ,'Mul'). But you don't need to
@@ -313,24 +330,23 @@
         For now, the algorithm just support the sub-graph's input /output ops are all in pattern.
         You can set the sub-graph input as (), but the results need you to check. Mostly, this
         sub-graph is a part of the pattern.
         As for pattern match / search, apply dfs to every graph list, then check the sub-graph's
         connection with the main computation flow. The idx would make the returned string list
         with right order.
     """
-    # parse the pattern_list and match sub-graph
     def _search_subgraph(subgraph):
+        """Parse the pattern_list and match sub-graph."""
         p_subgraph = [c[1] for c in subgraph]
         subgraph_idx = [c[0] for c in subgraph]
         m_subgraph = search_straight_pattern(p_subgraph, graph)
         return (m_subgraph, subgraph_idx)
 
-    # avoid splicing error when sub_graphs with totally same op types and tail node (#7)
-    # double check node idx and name
     def _has_duplicated_names_in_main_chain(sub_chain, main_chain, sub_chain_node_idx, has_head):
+        """Avoid splicing error when sub_graphs with totally same op types and tail node."""
         main_chain_node_names = [main_chain[i][0] for i in main_chain.keys()]
         ret_flag = False
         if has_head:
             sub_chain_node_names = sub_chain[1:-2]
             sub_chain_node_index = sub_chain_node_idx[1:-1]
         else:
             sub_chain_node_names = sub_chain[:-2]
@@ -345,16 +361,16 @@
                     ret_flag = True
                     break
                 else:
                     continue
 
         return ret_flag
 
-    # splicing the main_chain and sub_chain
     def _check_subgraph(iter_ret, m_subgraph, sub_graph_idx, has_head):
+        """Splicing the main_chain and sub_chain."""
         flag = [0] * len(iter_ret)
         for each_sub in m_subgraph:
             for i in range(len(iter_ret)):
                 if flag[i] == 0:
                     # get the sub-graph head and tail ops' names
                     tail_idx = sub_graph_idx[-1]
                     tail_name = iter_ret[i][tail_idx][0]
@@ -384,19 +400,22 @@
                                 # each sub-graph just can be matched more than one main_chain
                             flag[i] = 1
                             # break
                 else:
                     continue
         return iter_ret
 
-    # remove the duplicated results due to the complicated symmetric issues (#6)
-    # lists may have same nodes names between each other
-    # if has symmetric chains, they must appear consecutively
-    # just keep the first one
     def _rm_duplicated_rets(results):
+        """Remove the duplicated results due to the complicated symmetric issues.
+        
+        Note:
+            lists may have same nodes names between each other
+            if has symmetric chains, they must appear consecutively
+            just keep the first one
+        """
         if len(results) <= 1:
             return results
         keep_index = []
         i = 0
         length = len(results)
         while i < length:
             keep_index.append(i)
@@ -481,20 +500,22 @@
 
     # if has no sub-graph, like MatMul_BiasAdd
     else:
         return m_main_chain
 
 
 def construct_node(node_name, op_type, input_tensors=[], output_tensors=[], attr=OrderedDict()):
-    """construct node with engine op_type
+    """Construct node with engine op_type.
+
     Args:
         node_name: string, name of the node
         op_type: string, type of the node
         input_tensors: list, contains the input tensors of the node
         output_tensors: list, contains the output tensors of the node
+
     Returns:
         new_node: Operator class
     """
     from .ops.op import OPERATORS, Operator
     from .ops.tensor import Tensor
     if op_type in OPERATORS.keys():
         new_node = OPERATORS[op_type]()
@@ -503,14 +524,15 @@
         return new_node
     else:
         raise ValueError('the {} operation does not support now...'.format(op_type))
 
 
 def insert_pattern(target_node_names, new_nodes, graph):
     """Replace the specific pattern matched from the new constructed graph with new pattern.
+
     Args:
         target_node_names: A string list ccontains the names of nodes that will be replaced
         new_nodes: a list contains nodes with Operator class
         graph: The Graph class
 
     Returns:
         graph: The Graph class which some nodes inside have been replaced.
@@ -571,19 +593,21 @@
     # insert new_nodes
     graph.insert_nodes(index, new_nodes)
 
     return graph
 
 
 def pattern_mapping(pattern_name, mapping_dict, graph):
-    """
+    """The pattern mapping function.
+
     Args:
         pattern_name:  the name of the customized pattern representation, for example, 'LayerNorm'
         mapping_dict: a element in mapping_config[pattern_name], config for pattern mapping.
         graph: Graph class.
+
     Returns:
         tuple, the first element is the new nodes insert start idx, the second element is a new
         node list, the third is a list contains required old nodes need to be returned from origin
         pattern.
 
     A example of mapping_dict:
     mapping_dict: 
@@ -631,16 +655,16 @@
 
     Note that the pattern after fusion (n->n / n->1)is must be sequence pattern like 
     [a->b->c->d->e], or [a]. That means if one pattern is too complicated, or the pattern after 
     fusion is too complicated, you had better decompose it.
 
     """
 
-    # search pattern and get the in_pattern match_result and info for out_pattern
     def _get_pattern_info():
+        """Search pattern and get the in_pattern match_result and info for out_pattern."""
         in_pattern = mapping_dict['patterns']['in']
         search_mode = mapping_dict['search_mode']
         assert search_mode in ['op_type', 'node_name'], 'Unsupported mode'
         in_match_result = []
         if search_mode == 'op_type':
             in_match_result = search_pattern(in_pattern, graph)
             num_match = len(in_match_result)
@@ -759,16 +783,16 @@
             for idx in returns_inference:
                 node = graph.get_node_by_name(in_match_result[i][idx])
                 ret_tmp.append(copy.deepcopy(node))
             ret_old_nodes.append(ret_tmp)
 
         return (in_match_result, new_node_names, input_tensors, output_tensors, ret_old_nodes)
 
-    # created the new nodes in out_pattern
     def _create_out_pattern(new_node_names, input_tensors_list, output_tensors_list):
+        """Created the new nodes in out_pattern."""
         from .ops.tensor import Tensor
         out_pattern = mapping_dict['patterns']['out']
         # sequence = mapping_dict['sequence']
         sequence = True if len(out_pattern[0]) > 1 else False
         num_pattern = len(new_node_names)
         new_node_types = []
         new_nodes = []
@@ -825,16 +849,16 @@
                 if sequence:
                     pre_node = new_node
 
             new_nodes.append(one_p)
 
         return new_nodes
 
-    # replace the in_pattern with out_pattern
     def _replace_pattern(in_match_result, new_nodes, graph):
+        """Replace the in_pattern with out_pattern."""
         assert len(in_match_result) == len(
             new_nodes), 'out_pattern should have as some num as in_pattern in graph.'
         for i in range(len(in_match_result)):
             each_ret = in_match_result[i][:-1]
             insert_nodes = new_nodes[i]
             graph = insert_pattern(each_ret, insert_nodes, graph)
 
@@ -850,37 +874,42 @@
     # 4. remove the nodes in in_pattern, and insert the nodes in out_pattern
     graph = _replace_pattern(in_match_result, new_nodes, graph)
     # 5. return graph after pattern mapping
     return (graph, new_node_names, ret_old_nodes)
 
 
 def list2str(src_perm):
-    """convert the shape list to str for emitting yaml
+    """Convert the shape list to str for emitting yaml.
+
     Args:
         src_perm: list, for example [1,2,3,4]
+
     Returns:
         ret: str, for example '1,2,3,4'
     """
     ret = ','.join(str(i) for i in list(src_perm))
     return ret
 
 
 def str2list(src_str):
-    """convert the str to shape list
+    """Convert the str to shape list.
+
     Args:
         src_str: for example '1,2,3,4'
+
     Returns:
         ret: list, for example [1,2,3,4]
     """
     ret = []
     s_list = src_str.split(',')
     ret = [int(i) for i in s_list]
     return ret
 
 def pattern_mapping_conf_validation(conf_dict):
+    """The validation of the pattern mapping config."""
     dict_schema = Schema({
     'patterns' : Schema({
         'in' : And(
             list,
             lambda s: all(Schema([(), (int, Or(str, Schema([str])))]).validate(p) for p in s),
             lambda s: all((len(t)==2 for t in p[1:]) for p in s[1:]),
             error='The in pattern must supply the node index and op_type, and only the head node'\
@@ -941,75 +970,83 @@
      'old node index for set attr of new node later'),
 
     },  ignore_extra_keys=True)
 
     return dict_schema.validate(conf_dict)
 
 class LazyImport(object):
-    """Lazy import python module till use
-       Args:
-           module_name (string): The name of module imported later
+    """Lazy import python module till use.
+
+    Args:
+        module_name (string): The name of module imported later
     """
     def __init__(self, module_name):
+        """The module name initialization."""
         self.module_name = module_name
         self.module = None
 
     def __getattr__(self, name):
+        """The __getattr__ function."""
         try:
             self.module = importlib.import_module(self.module_name)
             mod = getattr(self.module, name)
         except:
             spec = importlib.util.find_spec(str(self.module_name + '.' + name))
             mod = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(mod)
         return mod
 
     def __call__(self, *args, **kwargs):
+        """The __call__ function."""
         function_name = self.module_name.split('.')[-1]
         module_name = self.module_name.split(f'.{function_name}')[0]
         self.module = importlib.import_module(module_name)
         function = getattr(self.module, function_name)
         return function(*args, **kwargs)
 
 def get_model_fwk_name(model):
-    """Detect the input model belongs to which framework
+    """Detect the input model belongs to which framework.
+
     Args:
         model (string): framework name that supported by Neural Engine, 
                         if there's no available fwk info, then return 'NA'.
     """
     onnx = LazyImport('onnx')
     tf = LazyImport('tensorflow')
     def _is_onnxruntime(model):
+        """Check if the model is onnxruntime."""
         try:
             if isinstance(model, str):
                 graph = onnx.load(model)
                 assert(len(graph.graph.node) != 0)
             else:
                 graph = model.graph
         except:
             pass
         else:
             return 'onnxruntime'
         return 'NA'
 
     def _is_tensorflow(model):
+        """Check if the model is tensorflow."""
         try:
             if isinstance(model, str):
                 graph_def = tf.compat.v1.GraphDef()
                 with open(model, 'rb') as f:
                     graph_def.ParseFromString(f.read())
             else:
                 graph = model.graph_def
         except:
             pass
         else:
             return 'tensorflow'
         return 'NA'
 
     def _is_neural_engine(model):
+        """Check if the model is neural engine."""
         if model and os.path.isdir(model):
             file_list = os.listdir(model)
             is_engine = True
             if len(file_list) == 2:
                 for file_name in file_list:
                     file_ext= os.path.splitext(file_name)
                     front, ext = file_ext
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/__init__.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The module of the neural engine graph loader."""
+
 from .loader import Loader
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/loader.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/loaders/loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,29 +11,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The loader file."""
+
 from ..graph_utils import LazyImport, get_model_fwk_name
 
 onnx = LazyImport('onnx')
 tf = LazyImport('tensorflow')
 
+
 class Loader(object):
-    def __call__(self, model):
+    """Load the model into the frontend of different inference frameworks."""
+    def __call__(self, model, pattern_config=None):
+        """Chceck if the model is the tensorflow or onnxruntime."""
         framework = get_model_fwk_name(model)
-        if framework =='tensorflow':
+        """Extract the node attr from tensorflow."""
+        if framework == 'tensorflow':
             if isinstance(model, str):
                 graph = tf.Graph()
                 graph_def = tf.compat.v1.GraphDef()
                 with open(model, 'rb') as f:
                     graph_def.ParseFromString(f.read())
                     with graph.as_default():
                         tf.import_graph_def(graph_def, name='')
                 config = tf.compat.v1.ConfigProto()
                 model = tf.compat.v1.Session(graph=graph, config=config)
-        if framework =='onnxruntime':
+        """Extract the node attr from onnxruntime."""
+        if framework == 'onnxruntime':
             if isinstance(model, str):
                 model = onnx.load(model)
         return model, framework
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/logger.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine logger file."""
+
 import os
 import logging
 
 
 class Logger(object):
+    """The logger class."""
     __instance = None
 
     def __new__(cls):
+        """The __new__ function."""
         if Logger.__instance is None:
             Logger.__instance = object.__new__(cls)
             Logger.__instance._log()
         return Logger.__instance
 
     def _log(self):
         LOGLEVEL = os.environ.get('LOGLEVEL', 'INFO').upper()
@@ -38,14 +42,15 @@
             "%Y-%m-%d %H:%M:%S")
         streamHandler = logging.StreamHandler()
         streamHandler.setFormatter(formatter)
         self._logger.addHandler(streamHandler)
         self._logger.propagate = False
 
     def get_logger(self):
+        """Get logger."""
         return self._logger
 
 
 def _pretty_dict(value, indent=0):
     prefix = '\n' + ' ' * (indent + 4)
     if isinstance(value, dict):
         items = [
@@ -70,60 +75,67 @@
 
 
 level = Logger().get_logger().level
 DEBUG = logging.DEBUG
 
 
 def log(level, msg, *args, **kwargs):
+    """The format for the log level."""
     if isinstance(msg, dict):
         for _, line in enumerate(_pretty_dict(msg).split('\n')):
             Logger().get_logger().log(level, line, *args, **kwargs)
     else:
         Logger().get_logger().log(level, msg, *args, **kwargs)
 
 
 def debug(msg, *args, **kwargs):
+    """The format for the debug level."""
     if isinstance(msg, dict):
         for _, line in enumerate(_pretty_dict(msg).split('\n')):
             Logger().get_logger().debug(line, *args, **kwargs)
     else:
         Logger().get_logger().debug(msg, *args, **kwargs)
 
 
 def error(msg, *args, **kwargs):
+    """The format for the error level."""
     if isinstance(msg, dict):
         for _, line in enumerate(_pretty_dict(msg).split('\n')):
             Logger().get_logger().error(line, *args, **kwargs)
     else:
         Logger().get_logger().error(msg, *args, **kwargs)
 
 
 def fatal(msg, *args, **kwargs):
+    """The format for the fatal level."""
     if isinstance(msg, dict):
         for _, line in enumerate(_pretty_dict(msg).split('\n')):
             Logger().get_logger().fatal(line, *args, **kwargs)
     else:
         Logger().get_logger().fatal(msg, *args, **kwargs)
 
 
 def info(msg, *args, **kwargs):
+    """The format for the info level."""
     if isinstance(msg, dict):
         for _, line in enumerate(_pretty_dict(msg).split('\n')):
             Logger().get_logger().info(line, *args, **kwargs)
     else:
         Logger().get_logger().info(msg, *args, **kwargs)
 
 
 def warn(msg, *args, **kwargs):
+    """The format for the warn level."""
     if isinstance(msg, dict):
         for _, line in enumerate(_pretty_dict(msg).split('\n')):
             Logger().get_logger().warning(line, *args, **kwargs)
     else:
         Logger().get_logger().warning(msg, *args, **kwargs)
 
 
 def warning(msg, *args, **kwargs):
+    """The format for the warning level."""
     if isinstance(msg, dict):
         for _, line in enumerate(_pretty_dict(msg).split('\n')):
             Logger().get_logger().warning(line, *args, **kwargs)
     else:
         Logger().get_logger().warning(msg, *args, **kwargs)
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/onnx_utils.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/onnx_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,77 +11,83 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine onnx utils."""
 
 import numpy as np
 import re
 from collections import namedtuple, OrderedDict
 from . import logger
 from .ops.tensor import Tensor
 from . import graph_utils as util
 
 def get_children(node, input_name_to_nodes=None):
+    """Get the node's output nodes in the graph."""
     if input_name_to_nodes is None:
         input_name_to_nodes = {}
 
     children = []
     for output in node.output:
         if output in input_name_to_nodes:
             for child in input_name_to_nodes[output]:
                 children.append(child)
     return children
 
 def get_node_children_names(model, node):
-    """Get the node's output nodes' name in the graph
+    """Get the node's output nodes' name in the graph.
+
     Args:
         model: ONNXModel
         node: NodeProto in onnx model
+
     Returns:
         outputs: names list
     """
-
     output_nodes = get_children(node)
     outputs = [node.name for node in output_nodes]
     return outputs
 
 
 def get_initializer_children_names(model, initializer):
-    """Get the initializer's output nodes' name in the graph
+    """Get the initializer's output nodes' name in the graph.
+
     Args:
         model: ONNXModel
         initializer: initializer in onnx model
+
     Returns:
         outputs: names list
     """
     output_nodes = []
     for node in model.graph.node:
         for node_input in node.input:
             if node_input == initializer.name:
                 output_nodes.append(node)
     outputs = [node.name for node in output_nodes]
     return outputs
 
 
 def graph_node_names_details(model):
     """Parse the graph nodes ans get the graph_nodes_dict.
+
     Be used for Grpah class with cerating a new graph.
     The node_name is the key, node in value is for getting the Const
     tensor value and the input_tensor source op; output_names in value
     is the node ouput name list; outputs in value is for output_tensor dest op
     Args:
         model: ONNXModel
+        
     Returns:
         node_names_details: the graph node info dict
 
     """
-
     node_details = namedtuple('node_details', ['node', 'outputs'])
     node_names_details = {}
     for initializer in model.graph.initializer:
         initializer_name = initializer.name
         each_node = node_details(node=initializer, outputs=[])
         if initializer_name not in node_names_details:
             each_node.outputs.extend(get_initializer_children_names(model, initializer))
@@ -110,32 +116,52 @@
                 continue
         each_node = node_details(node=graph_input, outputs=outputs)
         # if node_name not in node_names_details:
         node_names_details[node_name] = each_node
 
     return node_names_details
 
+def is_supported_onnx_graph(graph):
+    """Check if the onnx graph supported."""
+    for node in graph.node:
+        if not is_supported_onnx_node(node.op_type):
+            return False
+    return True
+
+def is_supported_onnx_node(node_name):
+    """Check if the node type is supported."""
+    supported_ops_type = ["Add", "Softmax", "Slice", "ReduceMean", "Reshape",
+                        "Concat", "Gather", "QuantizeLinear", "Transpose", "MatMul",
+                        "Sqrt", "Unsqueeze", "Shape", "Erf", "Pow", "DequantizeLinear",
+                        "Cast", "Tanh", "Div", "Mul", "Sub", "Constant", "Relu", "Conv",
+                        "Identity", "Split", "TopK"]
+    if node_name in supported_ops_type:
+        return True
+    else:
+        return False
 
 def change_num_name(tensor_name):
-    # for number string
+    """For number string."""
     try:
         if str(int(tensor_name)) == tensor_name:
             tensor_name += '_tensor'
     except BaseException:
         pass
     return tensor_name
 
 
 def bias_to_int32(bias_node, a_scale, b_scale):
-    """convert the int8 bias to int32 bias
+    """Convert the int8 bias to int32 bias.
+
     Args:
         bias_node: bias_add in graph (from onnx framework)
         a_scale: matmul node input matrice a scale tensor
         b_scale: matmul node input matrice b scale tensor
         model: Grpah class
+
     Returns:
         int32 bias numpy array
 
     fp32_bias = (int8_bias - int8_bias_zero_point) * int8_bias_scale
     int32_bias = fp32_bias / (a_scale * b_scale)
     """
     dtype_list = [np.int8, np.uint8]
@@ -157,15 +183,16 @@
     b_scale = float(b_scale)
     int32_bias = np.round((fp32_bias / (a_scale * b_scale))).astype(np.int32)
 
     return int32_bias
 
 
 def onnx_extract_operator(node, model, nodes_dict):
-    """decorate the operator in onnx
+    """Decorate the operator in onnx.
+
     Args:
         node: NodeProto
         model: ONNXModel
         nodes_dict: dict, return value from graph_node_names_details
         tf_dtypes: dict, for get the dtype string
 
     Returns:
@@ -175,17 +202,19 @@
     """
     from onnx.numpy_helper import to_array
 
     op_type = node.op_type
     input_tensors = []
     output_tensors = []
 
-    """ input_tensors
-    each input_tensor has its own soure op, but same dest op
-    so both have single string
+    """Input_tensors
+
+    Note:
+        each input_tensor has its own soure op, but same dest op
+        so both have single string
     """
     input_names = []
     # name list
     input_tensor_names = node.input
     for input_tensor_name in input_tensor_names:
         origin_tensor_name, input_tensor_name = util.names_from_input(input_tensor_name)
         try:
@@ -220,16 +249,18 @@
                                   shape=None,
                                   data=None,
                                   dtype=None
                                   )
             input_tensors.append(input_tensor)
         input_names.append(node.name)
 
-    """ output_tensors
-    in onnx, NodeProto has the output attribute
+    """Output_tensors.
+    
+    Note:
+        in onnx, NodeProto has the output attribute
     """
     output_tensor_names = node.output
     for output_tensor_name in output_tensor_names:
         output_tensor_name = util.names_from_input(output_tensor_name)[1]
         output_tensor = Tensor(name=output_tensor_name,
                                source_op=[node.name],
                                dest_op=nodes_dict[node.name].outputs,
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/__init__.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The module of the neural engine operators."""
+
 from .op import OPERATORS, Operator, operator_registry
 from .tensor import Tensor
 from os.path import dirname, basename, isfile, join
 import glob
 
 modules = glob.glob(join(dirname(__file__), "*.py"))
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/all.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/assert.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,19 +11,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
-@operator_registry(operator_type='All')
-class All(Operator):
+@operator_registry(operator_type='Assert')
+class Assert(Operator):
+    """Parse the Assert operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
-            self._attr['keep_dims'] = node.attr['keep_dims'].b
+            self._attr['summarize'] = node.attr['summarize'].i
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/assert.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_v2.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,19 +11,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
-@operator_registry(operator_type='Assert')
-class Assert(Operator):
+# get the matmul op scale, in bert_mlperf_int8.pb model, this op has several outputs
+# but the other output tensors has empty shape except the first one, and don't be used by other ops
+# so just keep the first one as the output_tensor
+@operator_registry(operator_type='QuantizeV2')
+class QuantizeV2(Operator):
+    """Parse the QuantizeV2 operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
+        self._op_type = 'Quantize'
         if framework == 'tensorflow':
-            self._attr['summarize'] = node.attr['summarize'].i
+            self._attr['output_dtype'] = 'u8'
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/batch_matmul.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/matmul.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,20 +11,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
-@operator_registry(operator_type='BatchMatMul')
-class BatchMatMul(Operator):
+@operator_registry(operator_type='MatMul')
+class MatMul(Operator):
+    """Parse the MatMul operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
-            self._attr['transpose_a'] = node.attr['adj_x'].b
-            self._attr['transpose_b'] = node.attr['adj_y'].b
+            self._attr['transpose_a'] = node.attr['transpose_a'].b
+            self._attr['transpose_b'] = node.attr['transpose_b'].b
+        """Extract the node attr from onnxruntime."""
+        if framework == 'onnxruntime':
+            self._attr['transpose_a'] = False
+            self._attr['transpose_b'] = False
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/batch_matmul_v2.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/batch_matmul_v2.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # TF BatchMatMulV2 support broadcasting in batch dimension
 @operator_registry(operator_type='BatchMatMulV2')
 class BatchMatMulV2(Operator):
+    """Parse the BatchMatMulV2 operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             self._attr['transpose_a'] = node.attr['adj_x'].b
             self._attr['transpose_b'] = node.attr['adj_y'].b
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/bias_add.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/bias_add.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # BiasAdd op behind MatMul op
 # tf.nn.bias_add(value, bias, data_format=None, name=None)
 # This is a special case of tf.add where bias is restricted to be 1-D
 @operator_registry(operator_type='BiasAdd')
 class BiasAdd(Operator):
+    """Parse the BiasAdd operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             self._attr['data_format'] = str(node.attr['data_format'].s, encoding="utf-8")
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/cast.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/pack.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,28 +11,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
-# tf.cast(x, dtype, name=None)
-# input dtype -> dest stype
-@operator_registry(operator_type='Cast')
-class Cast(Operator):
+# tf 1.0 changes tf.pack -> tf.stack
+# tf.stack(values, axis=0, name='stack')
+# Packs the list of tensors in values into a tensor with
+# rank one higher than each tensor in values,
+# by packing them along the axis dimension.
+# An int. The axis to stack along. Defaults to the first dimension. Negative values wrap around,
+# so the valid range is [-(D+1), D]
+# See also tf.concat, tf.tile, tf.repeat.
+@operator_registry(operator_type='Pack')
+class Pack(Operator):
+    """Parse the Pack operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
-            from ..tf_utils import TF_DTYPE_ID
-            self._attr['SrcT'] = TF_DTYPE_ID[node.attr['SrcT'].type]
-            self._attr['DstT'] = TF_DTYPE_ID[node.attr['DstT'].type]
-            self._attr['Truncate'] = node.attr['Truncate'].b
-        if framework == 'onnxruntime':
-            from ..onnx_utils import ONNX_DTYPE_ID
-            self._attr['DstT'] = ONNX_DTYPE_ID[node.attribute[0].i]
+            self._attr['axis'] = node.attr['axis'].i
+            self._attr['N'] = node.attr['N'].i
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/concat.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/concat.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 @operator_registry(operator_type='Concat')
 class Concat(Operator):
+    """Parse the Concat operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-
+        """Extract the node attr from onnxruntime."""
         if framework == "onnxruntime":
             if node.attribute[0].type == 2:
                 self._attr['axis'] = node.attribute[0].i
             elif node.attribute[0].type == 7:
                 self._attr['axis'] = node.attribute[0].ints
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/expand_dims.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/all.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
-# tf.expand_dims(input, axis, name=None)
-# Returns a tensor with a length 1 axis inserted at index axis.
-# Given an input of D dimensions, axis must be in range [-(D+1), D] (inclusive).
-@operator_registry(operator_type='ExpandDims')
-class ExpandDims(Operator):
+@operator_registry(operator_type='All')
+class All(Operator):
+    """Parse the All operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
-            self._attr['dim'] = self._input_tensors[1].data[0]
+            self._attr['keep_dims'] = node.attr['keep_dims'].b
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_batch_matmul_v2.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/mkl_layer_norm.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,20 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
-@operator_registry(operator_type='_FusedBatchMatMulV2')
-class _FusedBatchMatMulV2(Operator):
+@operator_registry(operator_type='_MklLayerNorm')
+class _MklLayerNorm(Operator):
+    """Parse the _MklLayerNorm operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        self._op_type = 'LayerNorm'
+        if framework == "onnxruntime":
+            axis = node.attribute[1].i
+            if axis != -1:
+                self._attr['axis'] = axis
+            self._attr['epsilon'] = node.attribute[2].f
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
-            self._attr['transpose_a'] = node.attr['adj_x'].b
-            self._attr['transpose_b'] = node.attr['adj_y'].b
+            self._attr['epsilon'] = node.attr['epsilon'].f
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_batch_norm_v3.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/split.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# Copyright (c) 2021 Intel Corporation
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from .op import Operator, operator_registry
-from .tensor import Tensor
-
-
-@operator_registry(operator_type='FusedBatchNormV3')
-class FusedBatchNormV3(Operator):
-    def __init__(self):
-        super().__init__()
-
-    def set_attr(self, framework, node):
-        if framework == 'tensorflow':
-            self._attr['epsilon'] = node.attr['epsilon'].f
-            self._attr['exponential_avg_factor'] = node.attr['exponential_avg_factor'].i
-            self._attr['is_training'] = node.attr['is_training'].b
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+#
+# Copyright (c) 2021 Intel Corporation
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""The neural engine operator mapping file."""
+
+from .op import Operator, operator_registry
+from .tensor import Tensor
+from ..graph_utils import list2str
+
+
+@operator_registry(operator_type='Split')
+class Split(Operator):
+    """Parse the Split operator to the neural engine."""
+    def __init__(self):
+        """The init function of this operator."""
+        super().__init__()
+    def set_attr(self, framework, node):
+        """Extract the node attr from onnxruntime."""
+        if framework == 'onnxruntime':
+            axis = node.attribute[0].i
+            self._attr['axis'] = axis
+            if len(node.attribute) > 1:
+                split = node.attribute[1].ints
+                self._attr['split'] = list2str(split)
+            else:
+                split = node.attribute[0].i
+                self._attr['split'] = list2str([split])
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_gemm.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_gemm.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # The inputs must be two-dimensional matrices
 @operator_registry(operator_type='FusedGemm')
 class FusedGemm(Operator):
+    """Parse the FusedGemm operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from frameworks."""
         activation_dict = {'Tanh': 'tanh'}
         self._op_type = 'InnerProduct'
         if framework == 'onnxruntime':
             activation = None
             transpose_a = False
             transpose_b = False
             alpha = 1.0
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gather.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gather.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,24 +11,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 @operator_registry(operator_type='Gather')
 class Gather(Operator):
+    """Parse the Gather operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from frameworks."""
         self._op_type = 'Gather'
         if framework == 'tensorflow':
             self._attr['batch_dims'] = node.attr['batch_dims'].i
             try:
                 axis = int(self._input_tensors[2].data)
             except BaseException:
                 axis = 0
@@ -46,18 +51,21 @@
 # argument validate_indices is deprecated
 # indices must be an integer tensor of any dimension (usually 0-D or 1-D).
 # Produces an output tensor with shape
 # params.shape[:axis] + indices.shape[batch_dims:] + params.shape[axis + 1:]
 # see: https://www.tensorflow.org/api_docs/python/tf/gather
 @operator_registry(operator_type='GatherV2')
 class GatherV2(Operator):
+    """Parse the GatherV2 operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from frameworks."""
         self._op_type = 'Gather'
         if framework == 'tensorflow':
             self._attr['batch_dims'] = node.attr['batch_dims'].i
             try:
                 axis = int(self._input_tensors[2].data)
             except BaseException:
                 axis = 0
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gelu.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gelu.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # tf.nn.gelu(features, approximate=False, name=None)
 # approximate=True: return x * cdf
 # cdf = 0.5 * (1.0 + tf.tanh((np.sqrt(2 / np.pi) * (x + 0.044715 * tf.pow(x, 3)))))
 # approximate=False: return x * 0.5 * (1.0 + math_ops.erf(x / math.sqrt(2.0)))
 @operator_registry(operator_type='Gelu')
 class Gelu(Operator):
+    """Parse the Gelu operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             self._attr['approximate'] = node.attr['approximate'].b
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gemm.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/gemm.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # The inputs must be two-dimensional matrices
 @operator_registry(operator_type='Gemm')
 class Gemm(Operator):
+    """Parse the Gemm operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from frameworks."""
         self._op_type = 'MatMulWithBias'
         if framework == 'onnxruntime':
             transpose_a = False
             transpose_b = False
             alpha = 1.0
             beta = 1.0
             for attr in node.attribute:
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/iterator_get_next.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/iterator_get_next.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # tf.placeholder(dtype, shape=None, name=None)
 @operator_registry(operator_type='IteratorGetNext')
 class IteratorGetNext(Operator):
+    """Parse the IteratorGetNext operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             from ..tf_utils import TF_DTYPE_ID
             output_shapes = []
             shape_list = node.attr['output_shapes'].list.shape
             for each in shape_list:
                 tmp = []
                 shape = each.dim
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/iterator_v2.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/map_and_batch_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,24 +11,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
-@operator_registry(operator_type='IteratorV2')
-class IteratorV2(Operator):
+@operator_registry(operator_type='MapAndBatchDataset')
+class MapAndBatchDataset(Operator):
+    """Parse the MapAndBatchDataset operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             from ..tf_utils import TF_DTYPE_ID
             output_shapes = []
             shape_list = node.attr['output_shapes'].list.shape
             for each in shape_list:
                 tmp = []
                 shape = each.dim
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/layer_normalization.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/layer_normalization.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,23 +11,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 @operator_registry(operator_type='LayerNormalization')
 class LayerNormalization(Operator):
+    """Parse the LayerNormalization operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from frameworks."""
         self._op_type = 'LayerNorm'
         if framework == "onnxruntime":
             axis = node.attribute[1].i
             if axis != -1:
                 self._attr['axis'] = axis
             self._attr['epsilon'] = node.attribute[2].f
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/matmul.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reduce_sum.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,23 +11,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
+from ..graph_utils import list2str
 
 
-@operator_registry(operator_type='MatMul')
-class MatMul(Operator):
+@operator_registry(operator_type='ReduceSum')
+class ReduceSum(Operator):
+    """Parse the ReduceSum operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-        if framework == 'tensorflow':
-            self._attr['transpose_a'] = node.attr['transpose_a'].b
-            self._attr['transpose_b'] = node.attr['transpose_b'].b
+        """Extract the node attr from onnxruntime."""
         if framework == 'onnxruntime':
-            self._attr['transpose_a'] = False
-            self._attr['transpose_b'] = False
+            for attribute in node.attribute:
+                if attribute.name == 'axes':
+                    self._attr['axis'] = list2str(attribute.ints)
+                if attribute.name == 'keepdims':
+                    self._attr['keep_dims'] = bool(attribute.i)
+            # ai.onnx v14
+            if 'axis' not in self._attr:
+                if len(self._input_tensors[1].data) == 1:
+                   self._attr['axis'] = int(self._input_tensors[1].data)
+                else:
+                   self._attr['axis'] = list2str(self._input_tensors[1].data)
+                self._input_tensors.pop()
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/mean.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/mean.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,22 +11,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # tf.math.reduce_mean(input_tensor, axis=None, keepdims=False, name=None)
 # If axis is None, all dimensions are reduced, and a tensor with a single element is returned.
 @operator_registry(operator_type='Mean')
 class Mean(Operator):
+    """Parse the Mean operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             self._attr['axis'] = self._input_tensors[1].data[0]
             self._attr['keep_dims'] = node.attr['keep_dims'].b
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/mkl_layer_norm.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/unpack.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
-@operator_registry(operator_type='_MklLayerNorm')
-class _MklLayerNorm(Operator):
+# tf.unstack(value, num=None, axis=0, name='unstack')
+# Unpacks tensors from value by chipping it along the axis dimension.
+@operator_registry(operator_type='Unpack')
+class Unpack(Operator):
+    """Parse the Unpack operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-        self._op_type = 'LayerNorm'
-        if framework == "onnxruntime":
-            axis = node.attribute[1].i
-            if axis != -1:
-                self._attr['axis'] = axis
-            self._attr['epsilon'] = node.attribute[2].f
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
-            self._attr['epsilon'] = node.attr['epsilon'].f
+            self._attr['axis'] = node.attr['axis'].i
+            self._attr['num'] = node.attr['num'].i
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/model_dataset.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/optimize_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,24 +11,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
-@operator_registry(operator_type='ModelDataset')
-class ModelDataset(Operator):
+@operator_registry(operator_type='OptimizeDataset')
+class OptimizeDataset(Operator):
+    """Parse the OptimizeDataset operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             from ..tf_utils import TF_DTYPE_ID
             output_shapes = []
             shape_list = node.attr['output_shapes'].list.shape
             for each in shape_list:
                 tmp = []
                 shape = each.dim
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/one_hot.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/one_hot.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,24 +11,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 import copy
 
 
 @operator_registry(operator_type='OneHot')
 class OneHot(Operator):
+    """Parse the OneHot operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             self._attr['axis'] = node.attr['axis'].i
             self._attr['depth'] = int(self._input_tensors[1].data)
             self._attr['on_value'] = int(self._input_tensors[2].data)  # float
             self._attr['off_value'] = int(self._input_tensors[3].data)  # float
             self._input_tensors = [copy.deepcopy(self._input_tensors[0])]
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/onnx_input.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reshape.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,35 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
-from ..graph_utils import names_from_input
+import numpy as np
+from ..graph_utils import list2str
 
 
-# graph.input
-@operator_registry(operator_type='ONNXINPUT')
-class ONNXINPUT(Operator):
+# tf.reshape(tensor, shape, name=None)
+# param shape is s Tensor. Must be one of the following types: int32, int64.
+# defines the shape of the output tensor.
+@operator_registry(operator_type='Reshape')
+class Reshape(Operator):
+    """Parse the Reshape operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
-    def extract(self, framework, node, model, nodes_dict):
-        from ..onnx_utils import ONNX_DTYPE_ID
-        self._name = node.name
-        self._op_type = 'ONNXINPUT'
-        output_tensor_name = names_from_input(self._name)[1]
-        shape_len = len(node.type.tensor_type.shape.dim)
-        shape = [-1] * shape_len
-        dtype = ONNX_DTYPE_ID[node.type.tensor_type.elem_type]
-        output_tensor = Tensor(
-            name=output_tensor_name,
-            shape=shape,
-            dtype=dtype,
-            source_op=[self._name],
-            dest_op=nodes_dict[self._name].outputs,
-        )
-
-        self._output_tensors = [output_tensor]
+    def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
+        #if framework == 'tensorflow':
+        if self.input_tensors[1].source_op == []:
+            dst_shape = list2str(self._input_tensors[1].data)
+            self._attr['dst_shape'] = dst_shape
+            self.input_tensors.pop()
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/op.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/op.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator file."""
+
 from abc import abstractmethod
 from collections import namedtuple, OrderedDict
 from .tensor import Tensor
 
 
 OPERATORS = {}
 
@@ -39,90 +41,103 @@
         OPERATORS[operator_type] = cls
         return cls
 
     return decorator_operator
 
 
 class Operator(object):
+    """The class of neural engine operator."""
     def __init__(self):
+        """The init function of this operator."""
         self._name = ''
         self._op_type = ''
         self._input_tensors = []
         self._output_tensors = []
         self._attr = OrderedDict()
 
     @property
     def name(self):
+        """Get the operator name."""
         return self._name
 
     @name.setter
     def name(self, name):
+        """Name assignment."""
         self._name = name
 
     @property
     def op_type(self):
+        """Get op_type."""
         return self._op_type
 
     @op_type.setter
     def op_type(self, op_type):
+        """Op_type assignment."""
         self._op_type = op_type
 
     @property
     def input_tensors(self):
+        """Get input_tensors."""
         return self._input_tensors
 
     @input_tensors.setter
     def input_tensors(self, input_tensors):
+        """Input tensor assignment."""
         self._input_tensors = input_tensors
 
     @property
     def output_tensors(self):
+        """Get output tensor."""
         return self._output_tensors
 
     @output_tensors.setter
     def output_tensors(self, output_tensors):
+        """Output_tensor assignment."""
         self._output_tensors = output_tensors
 
     @property
     def attr(self):
+        """Get attr."""
         return self._attr
 
     @attr.setter
     def attr(self, attr):
+        """Attr assignment."""
         self._attr = attr
 
     def set_attr(self, framework, node):
+        """Attr initialization."""
         self._attr = OrderedDict()
 
-    # extract the op from framework
     def extract(self, framework, node, model, nodes_dict):
+        """Extract the op from framework."""
         from ..tf_utils import tf_extract_operator
         from ..onnx_utils import onnx_extract_operator
 
         OP_EXTRACTORS = {
             'tensorflow': tf_extract_operator,
             'onnxruntime': onnx_extract_operator,
         }
         
         self._name = node.name
         self._op_type, self._input_tensors, self._output_tensors = OP_EXTRACTORS[framework](
             node, model, nodes_dict)
         self.set_attr(framework, node)
 
-    # make the op by set the attributes
     def construct(self, name, op_type, input_tensors=[], output_tensors=[], attr=OrderedDict()):
+        """Make the op by set the attributes."""
         self._name = name
         self._op_type = op_type
         self._input_tensors = input_tensors
         self._output_tensors = output_tensors
         self._attr = attr
 
-    # get the op config in graph
     @property
     def config(self):
+        """Get the op config in the graph."""
         conf_dict = OrderedDict()
         # conf_dict['type'] = self._op_type
         conf_dict['type'] = self._op_type
         if len(self._input_tensors) > 0:
             conf_dict['input'] = OrderedDict()
             for input_tensor in self._input_tensors:
                 if self._op_type == 'Input':
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/placeholder.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/placeholder.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # tf.placeholder(dtype, shape=None, name=None)
 @operator_registry(operator_type='Placeholder')
 class Placeholder(Operator):
+    """Parse the Placeholder operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             from ..tf_utils import TF_DTYPE_ID
             try:
                 self._output_tensors[0].shape = [i.size for i in node.attr['shape'].shape.dim]
             except BaseException:
                 pass
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_linear.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_linear.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 @operator_registry(operator_type='QuantizeLinear')
 class QuantizeLinear(Operator):
+    """Parse the QuantizeLinear operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from onnxruntime."""
         self._op_type = 'Quantize'
         if framework == 'onnxruntime':
             self._attr['output_dtype'] = 'u8'
             self._attr['quant_mode'] = 'zp_scale'
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_v2.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/top_k.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,23 +11,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
+from ..graph_utils import list2str
 
 
-# get the matmul op scale, in bert_mlperf_int8.pb model, this op has several outputs
-# but the other output tensors has empty shape except the first one, and don't be used by other ops
-# so just keep the first one as the output_tensor
-@operator_registry(operator_type='QuantizeV2')
-class QuantizeV2(Operator):
+@operator_registry(operator_type='TopK')
+class TopK(Operator):
+    """Parse the TopK operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-        self._op_type = 'Quantize'
-        if framework == 'tensorflow':
-            self._attr['output_dtype'] = 'u8'
+        """Extract the node attr from onnxruntime."""
+        if framework == 'onnxruntime':
+            for attribute in node.attribute:
+                if attribute.name == 'axis':
+                    self._attr['axis'] = attribute.i
+                if attribute.name == 'largest':
+                    self._attr['largest'] = attribute.i
+                if attribute.name == 'sorted':
+                    self._attr['sorted'] = attribute.i
+            # write the K value into attr if it's const
+            if self._input_tensors[1].data:
+                self._attr['k'] = int(self._input_tensors[1].data)
+                self._input_tensors.pop()
+            # remove the data output_tensor, just keep indices
+            self._output_tensors = [self._output_tensors[1]]
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_fused_matmul_and_dequantize.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_fused_matmul_and_dequantize.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,29 +11,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # The inputs must be two-dimensional matrices
 @operator_registry(operator_type='_QuantizedFusedMatMulAndDequantize')
 class _QuantizedFusedMatMulAndDequantize(Operator):
+    """Parse the _QuantizedFusedMatMulAndDequantize operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
 
         # for baremetal, if QuantizedMatMulWithBiasAndDequantize has post op
         # its output_dtype maybe the origin dtype in attributes, float32
         # but if it has not, use int8 (s8) for performance consideration
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             self._attr['output_dtype'] = 'fp32'  # 's8'
             transpose_a = node.attr['transpose_a'].b
             transpose_b = node.attr['transpose_b'].b
             if transpose_a:
                 self._attr['src0_perm'] = '1,0'
             if not transpose_b:
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_matmul_with_bias_and_dequantize.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_matmul_with_bias_and_dequantize.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 
 
 # The inputs must be two-dimensional matrices
 @operator_registry(operator_type='QuantizedMatMulWithBiasAndDequantize')
 class QuantizedMatMulWithBiasAndDequantize(Operator):
+    """Parse the QuantizedMatMulWithBiasAndDequantize operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
         # for baremetal, if QuantizedMatMulWithBiasAndDequantize has post op
         # its output_dtype maybe the origin dtype in attributes, float32
         # but if it has not, use int8 (s8) for performance consideration
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             self._attr['output_dtype'] = 's8'
             self._attr['transpose_a'] = node.attr['transpose_a'].b
             self._attr['transpose_b'] = node.attr['transpose_b'].b
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reduce_mean.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reduce_mean.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,30 +11,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 from ..graph_utils import list2str
 
 
 # tf.math.reduce_mean(input_tensor, axis=None, keepdims=False, name=None)
 # If axis is None, all dimensions are reduced, and a tensor with a single element is returned.
 @operator_registry(operator_type='ReduceMean')
 class ReduceMean(Operator):
+    """Parse the ReduceMean operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             self._attr['axis'] = self._input_tensors[1].data[0]
             self._attr['keep_dims'] = node.attr['keep_dims'].b
+        """Extract the node attr from onnxruntime."""
         if framework == 'onnxruntime':
             if len(node.attribute) == 2:
                 axis = node.attribute[1].ints
                 self._attr['keep_dims'] = bool(node.attribute[0].i)
             if len(node.attribute) == 1:
                axis = node.attribute[0].ints
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/reshape.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_batch_matmul_v2.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,27 +11,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
-import numpy as np
-from ..graph_utils import list2str
 
 
-# tf.reshape(tensor, shape, name=None)
-# param shape is s Tensor. Must be one of the following types: int32, int64.
-# defines the shape of the output tensor.
-@operator_registry(operator_type='Reshape')
-class Reshape(Operator):
+@operator_registry(operator_type='_FusedBatchMatMulV2')
+class _FusedBatchMatMulV2(Operator):
+    """Parse the _FusedBatchMatMulV2 operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-        # if framework == 'tensorflow':
-        if self.input_tensors[1].source_op == []:
-            dst_shape = list2str(self._input_tensors[1].data)
-            self._attr['dst_shape'] = dst_shape
-            self.input_tensors.pop()
+        """Extract the node attr from tensorflow."""
+        if framework == 'tensorflow':
+            self._attr['transpose_a'] = node.attr['adj_x'].b
+            self._attr['transpose_b'] = node.attr['adj_y'].b
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/softmax.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/softmax.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,28 +11,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 import copy
 
 
 # Computes softmax activations.
 # tf.nn.softmax(logits, axis=None, name=None)
 @operator_registry(operator_type='Softmax')
 @operator_registry(operator_type='SoftmaxGraph')
 class Softmax(Operator):
+    """Parse the Softmax operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
+        """Extract the node attr from frameworks."""
         if framework == "tensorflow":
             # last_dim = len(self._input_tensors[0].shape) - 1
             try:
                 axis = self._input_tensors[1].data[0]
                 self._input_tensors = [copy.deepcopy(self._input_tensors[0])]
             except BaseException:
                 axis = -1
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/split.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/expand_dims.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# Copyright (c) 2021 Intel Corporation
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from .op import Operator, operator_registry
-from .tensor import Tensor
-from ..graph_utils import list2str
-
-
-@operator_registry(operator_type='Split')
-class Split(Operator):
-    def __init__(self):
-        super().__init__()
-    def set_attr(self, framework, node):
-        if framework == 'onnxruntime':
-            axis = node.attribute[0].i
-            self._attr['axis'] = axis
-            if len(node.attribute) > 1:
-                split = node.attribute[1].ints
-                self._attr['split'] = list2str(split)
-            else:
-                split = node.attribute[0].i
-                self._attr['split'] = list2str([split])
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+#
+# Copyright (c) 2021 Intel Corporation
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""The neural engine operator mapping file."""
+
+from .op import Operator, operator_registry
+from .tensor import Tensor
+
+
+# tf.expand_dims(input, axis, name=None)
+# Returns a tensor with a length 1 axis inserted at index axis.
+# Given an input of D dimensions, axis must be in range [-(D+1), D] (inclusive).
+@operator_registry(operator_type='ExpandDims')
+class ExpandDims(Operator):
+    """Parse the ExpandDims operator to the neural engine."""
+    def __init__(self):
+        """The init function of this operator."""
+        super().__init__()
+
+    def set_attr(self, framework, node):
+        """Extract the node attr from tensorflow."""
+        if framework == 'tensorflow':
+            self._attr['dim'] = self._input_tensors[1].data[0]
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/squeeze.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/unsqueeze.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 from ..graph_utils import list2str
 
 
 # This operation creates a tensor of shape dims and fills it with value.
 # tf.fill(dims, value, name=None)
-@operator_registry(operator_type='Squeeze')
-class Squeeze(Operator):
+@operator_registry(operator_type='Unsqueeze')
+class Unsqueeze(Operator):
+    """Parse the Unsqueeze operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-        if framework == 'tensorflow':
-            self._attr['squeeze_dims'] = node.attr['squeeze_dims'].list.i
+        """Extract the node attr from onnxruntime."""
         if framework == 'onnxruntime':
+            # ai.onnx v11
             if len(node.attribute):
-                axis = node.attribute[0].ints
-                if len(axis) == 1:
-                    self._attr['axis'] = axis[0]
+                self._attr['axis'] = list2str(node.attribute[0].ints)
+            # ai.onnx v14
+            else:
+                if len(self._input_tensors[1].data) == 1:
+                   self._attr['axis'] = int(self._input_tensors[1].data)
                 else:
-                    self._attr['axis'] = list2str(axis)
+                   self._attr['axis'] = list2str(self._input_tensors[1].data)
+                self._input_tensors.pop()
+
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/strided_slice.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/strided_slice.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,28 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 from ..graph_utils import list2str
 
 
 # tf.strided_slice(input_, begin, end, strides=None, begin_mask=0, end_mask=0,
 # ellipsis_mask=0,new_axis_mask=0, shrink_axis_mask=0, var=None, name=None)
 @operator_registry(operator_type='StridedSlice')
 class StridedSlice(Operator):
+    """Parse the StridedSlice operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-
+        """Extract the node attr from tensorflow."""
         if framework == 'tensorflow':
             self._attr['begin_mask'] = node.attr['begin_mask'].i
             self._attr['ellipsis_mask'] = node.attr['ellipsis_mask'].i
             self._attr['end_mask'] = node.attr['end_mask'].i
             self._attr['new_axis_mask'] = node.attr['new_axis_mask'].i
             self._attr['shrink_axis_mask'] = node.attr['shrink_axis_mask'].i
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/ops/transpose.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/ops/transpose.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,33 +11,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine operator mapping file."""
+
 from .op import Operator, operator_registry
 from .tensor import Tensor
 from ..graph_utils import list2str
 
 
 # tf.transpose(a, perm=None, conjugate=False, name='transpose')
 # The returned tensor's dimension i will correspond to the input dimension perm[i].
 # If perm is not given, it is set to (n-1...0), where n is the rank of the input tensor.
 # Hence by default, this operation performs a regular matrix transpose on 2-D input Tensors.
 # If conjugate is True and a.dtype is either complex64 or complex128 then the values of a are
 # conjugated and transposed.
 # normally, we don't need the param 'conjugate'
 @operator_registry(operator_type='Transpose')
 class Transpose(Operator):
+    """Parse the Transpose operator to the neural engine."""
     def __init__(self):
+        """The init function of this operator."""
         super().__init__()
 
     def set_attr(self, framework, node):
-
+        """Extract the node attr from onnxruntime."""
         if framework == "tensorflow":
             if self._input_tensors[1].source_op == []:
                 dst_perm = list(self._input_tensors[1].data)
                 self._attr['dst_perm'] = list2str(dst_perm)
                 src_perm = [i for i in range(len(dst_perm))]
                 self._attr['src_perm'] = list2str(src_perm)
                 _ = self._input_tensors.pop()
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/__init__.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine sub_graph module."""
+
 from .pattern import PATTERNS, Pattern, pattern_registry
 from .subgraph_matcher import SubGraphMatcher
 
 from os.path import dirname, basename, isfile, join
 import glob
 
 modules = glob.glob(join(dirname(__file__), "*.py"))
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/add_embeddings.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/add_embeddings.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The AddEmbeddings Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='AddEmbeddings')
 class AddEmbeddings(Pattern):
-    def __call__(self, model):
+    """The AddEmbeddings pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'AddEmbeddings' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'AddEmbeddings': [
                 {
                     'patterns': {
                         'in': [[(0, ['AddV2', 'Add']), (1, ['AddV2', 'Add']), (2, 'LayerNorm'),
                                 (3, 'Reshape')]],
                         'out': [[(0, 'BinaryAdd'), (1, 'Reshape'), (2, 'Reshape'),
@@ -104,14 +111,15 @@
                         }], [[0], 1]]
                     },
                     'returns': [0, 2]
                 },
 
 
                 # distil_bert_base
+                # vit: only need 1 reshape node in 'out'
                 {
                     'patterns': {
                         'in': [[(0, ['AddV2', 'Add']), (1, 'LayerNorm')]],
                         'out': [[(0, 'BinaryAdd'), (1, 'Reshape'), (2, 'Reshape'),
                                 (3, 'LayerNorm')]]
                     },
                     'search_mode': 'op_type',
@@ -132,27 +140,27 @@
                             'input_data': [0]
                         }], [[1], 2]],
                         2: [[], [[], 1]],
                         3: [[{1: [1]}, {1: [2]}],
                             [[1, 2], 3]]
                     },
                     'output_tensors': {
-                        0: [[], [[], 1]],
+                        0: [[ {0: [0]}], [[0], 1]],
                         1: [[], [[], 1]],
                         2: [[], [[], 1]],
                         3: [[{
                             1: [0]
                         }], [[0], 1]]
                     },
                     'returns': [0, 1]
                 },
             ]
         }
 
-        def _set_attr(hidden_size, epsilon, node_names, model):
+        def _set_attr(hidden_size, epsilon, node_names, model, is_vit = False):
             attr1 = OrderedDict()
             attr1['append_op'] = 'sum'
             attr2 = OrderedDict()
             attr2['dst_shape'] = '-1,-1,' + str(hidden_size)
             attr2['dims'] = '0,1'
             attr3 = OrderedDict()
             attr3['dst_shape'] = '-1,' + str(hidden_size)
@@ -163,28 +171,36 @@
             model.nodes[binary_add_node_idx].attr = attr1
 
             reshape_1_node_idx = model.get_node_id(node_names[1])
             model.nodes[reshape_1_node_idx].attr = attr2
 
             reshape_2_node_idx = model.get_node_id(node_names[2])
             model.nodes[reshape_2_node_idx].attr = attr3
+            # In vit we need to remove the first reshape node
+            if is_vit:
+                model.nodes[reshape_2_node_idx].input_tensors = model.nodes[binary_add_node_idx].output_tensors
+                model.remove_nodes([node_names[1]])
 
             ln_node_idx = model.get_node_id(node_names[3])
             model.nodes[ln_node_idx].attr = attr4
 
         for i in range(len(pattern_mapping_config['AddEmbeddings'])):
             pattern_dict = pattern_mapping_config['AddEmbeddings'][i]
             model, new_node_names, ret_old_nodes = util.pattern_mapping("AddEmbeddings", 
                                                                         pattern_dict, model)
             if len(new_node_names) != 0:
                 for j in range(len(new_node_names)):
                     ln_node = ret_old_nodes[j][1]
+                    add_node = ret_old_nodes[j][0]
+                    is_vit = False
+                    if add_node.input_tensors[-1].data is not None:
+                        is_vit = True
                     hidden_size = int(ln_node.input_tensors[-1].shape[-1])
                     epsilon = ln_node.attr['epsilon']
-                    _set_attr(hidden_size, epsilon, new_node_names[j], model)
+                    _set_attr(hidden_size, epsilon, new_node_names[j], model, is_vit)
                     if len(pattern_dict['patterns']['in'][0]) == 2:
                         binary_add_node_idx = model.get_node_id(new_node_names[j][0])
                         model.nodes[binary_add_node_idx].attr = OrderedDict()
 
                 return model
 
         return model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_reshape.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_reshape.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The AttentionReshape Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 import copy
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='AttentionReshape')
 class AttentionReshape(Pattern):
-    def __call__(self, model):
+    """The AttentionReshape pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'AttentionReshape' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'AttentionReshape': [
                 {
                     'patterns': {
                         'in': [[(0, 'Mul'), (1, 'Pack'), (2, 'Reshape')]],
                         'out': [[(0, 'Reshape')]]
                     },
@@ -78,14 +85,50 @@
                         1: [[{
                             8: [0]
                         }], [[0], 1]]
                     },
                     'returns': [6, 8]
                 },
 
+                # Shira new model Reshape_128, 373, 618
+                {
+                    'patterns': {
+                        'in': [[(0, 'Transpose'), (1, 'Shape'), (2, 'Gather'), (3, 'Unsqueeze'), (4, 'Concat'),
+                                (5, 'Reshape'),(6, 'MatMulWithBias')]
+                                ],
+                        'out': [[(0, 'Transpose'), (1, 'Reshape'), (2, 'MatMulWithBias')]]
+                    },
+                    'search_mode': 'op_type',
+                    'node_names': {
+                        0: 0,
+                        1: 5,
+                        2: 6,
+                    },
+                    'input_tensors': {
+                        0: [[{
+                            0: [0]
+                        }], [[0], 1]],
+                        1: [[], [[],1]],
+                        2: [[
+                        {6: [1]},{6: [2]}
+                        ],[[1, 2],3]],
+                    },
+                    'output_tensors': {
+                        0: [[], [[],1]],
+
+                        1: [[{
+                        5:[0]
+                        }],[[0],1]],
+                        2: [[{
+                            6: [0]
+                        }], [[0], 1]]
+                    },
+                    'returns': [0,4,6]
+                },
+
                 # bert_mini_int8
                 {
                     'patterns': {
                         'in': [[(0, 'Shape'), (1, 'Gather'), (2, 'Gather'), (3, 'Unsqueeze'), (6, 'Concat'),
                                 (7, 'Reshape'), (8, 'MatMulWithBias')],
                                 [(1, 'Gather'), (4, 'Gather'), (5, 'Unsqueeze'),
                                 (6, 'Concat')]],
@@ -174,49 +217,57 @@
                         }], [[0], 1]]
                     },
                     'returns': [0, 1]
                 },
             ]
         }
 
-        def _set_attr(hidden_size, node_names, model):
+        def _set_attr(hidden_size, node_names, model, reshape_idx=0):
             attr = OrderedDict()
             attr['dst_shape'] = '-1,' + str(hidden_size)
-            reshape_node_idx = model.get_node_id(node_names[0])
+            reshape_node_idx = model.get_node_id(node_names[reshape_idx])
             model.nodes[reshape_node_idx].attr = attr
 
         for i in range(len(pattern_mapping_config['AttentionReshape'])-1):
             pattern_dict = pattern_mapping_config['AttentionReshape'][i]
             model, new_node_names, ret_old_nodes = util.pattern_mapping("AttentionReshape",
                                                                         pattern_dict, model)
+
             if len(new_node_names) != 0:
                 for j in range(len(new_node_names)):
-                    pack_node = ret_old_nodes[j][0]
-                    hidden_size = int(pack_node.input_tensors[-1].data)
-                    _set_attr(hidden_size, new_node_names[j], model)
-                    if len(ret_old_nodes[j]) == 2:
+                    if len(ret_old_nodes[j]) == 3:
+                        pack_node = ret_old_nodes[j][1]
+                        hidden_size = int(pack_node.input_tensors[-1].data)
+                        _set_attr(hidden_size, new_node_names[j], model,reshape_idx=1)
+
+                        assert ret_old_nodes[j][0].op_type == 'Transpose'
+                        trans_node_idx = model.get_node_id(new_node_names[j][0])
+                        model.nodes[trans_node_idx].attr = ret_old_nodes[j][0].attr
+
+                        assert ret_old_nodes[j][2].op_type == 'MatMulWithBias'
+                        mat_node_idx = model.get_node_id(new_node_names[j][2])
+                        model.nodes[mat_node_idx].attr = ret_old_nodes[j][2].attr
+
+                    elif len(ret_old_nodes[j]) == 2:
+                        pack_node = ret_old_nodes[j][0]
+                        hidden_size = int(pack_node.input_tensors[-1].data)
+                        _set_attr(hidden_size, new_node_names[j], model)
                         assert ret_old_nodes[j][1].op_type == 'MatMulWithBias'
                         mat_node_idx = model.get_node_id(new_node_names[j][1])
                         model.nodes[mat_node_idx].attr = ret_old_nodes[j][1].attr
 
-                return model
-
-        # special reshape node, like has '0,0,768' dst_shape attr
+        # special reshape node, like has '0,0,768' or '-1,369,384' dst_shape attr
         pattern_dict = pattern_mapping_config['AttentionReshape'][-1]
         model, new_node_names, ret_old_nodes = util.pattern_mapping("AttentionReshape",
                                                                     pattern_dict, model)
+
         if len(new_node_names) != 0:
             for j in range(len(new_node_names)):
                 reshape_node = ret_old_nodes[j][0]
-                try:
-                    dst_shape = reshape_node.attr['dst_shape']
-                except:
-                    dst_shape = None
-                if dst_shape != None and dst_shape.split(',')[0] == '0':
+                dst_shape = reshape_node.attr.get('dst_shape', None)
+                if dst_shape != None and dst_shape.split(',')[0] == '0' or '-1':
                     hidden_size = int(dst_shape.split(',')[-1])
                     _set_attr(hidden_size, new_node_names[j], model)
                 mat_node_idx = model.get_node_id(new_node_names[j][1])
                 model.nodes[mat_node_idx].attr = ret_old_nodes[j][1].attr
 
-            return model
-
         return model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/collect_quant_info.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/collect_quant_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,26 +11,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The CollectQuantInfo Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 from .subgraph_matcher import EXECUTOR_TYPE
 import numpy as np
 import copy
 
 @pattern_registry(pattern_type='CollectQuantInfo')
 class CollectQuantInfo(Pattern):
+    """The CollectQuantInfo pattern.
 
-    def __call__(self, model):
+    Fuse the original sub-graph into the custom acceleration 'CollectQuantInfo' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
 
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'CollectQDQInfo': [
                 {
                     'patterns': {
                         'in': [[(0, 'Quantize'), (1, ['DequantizeLinear'])]],
                     },
                 },
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/embeddingbag.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/embeddingbag.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The EmbeddingBag Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='EmbeddingBag')
 class EmbeddingBag(Pattern):
-    def __call__(self, model):
+    """The EmbeddingBag pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'EmbeddingBag' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'EmbeddingBag': [
                 # DLRM onnx model
                 {
                     'patterns': {
                         'in': [[(0, 'Shape'), (1, 'Gather'), (3, 'Unsqueeze'), (4, 'Concat'),
                                 (5, 'Slice'), (6, 'Shape'), (7, 'Gather'), (8, 'Loop')],
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/gelu.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/gelu.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The Gelu Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 import copy
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='Gelu')
 class Gelu(Pattern):
-    def __call__(self, model):
+    """The Gelu pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'Gelu' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'Gelu': [
                 {
                     'patterns': {
                         'in': [[(0,'Pow'), (1, 'Mul'), (2, 'AddV2'), (3, 'Mul'), (4, 'Tanh'),
                                 (5, 'AddV2'), (6, 'Mul'), (7, 'Mul')]],
                         'out': [[(0, 'Gelu')]]
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_data.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,23 +11,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The InputData Pattern."""
+
+import copy
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='InputData')
 class InputData(Pattern):
-    def __call__(self, model):
+    """The InputData pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'InputData' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'InputData': [
                 {
                     'patterns': {
                         'in': [[(0, 'input_ids'), (1, 'segment_ids'), (2, 'input_mask')]],
                         'out': [[(0, 'Input')]]
                     },
@@ -145,14 +153,57 @@
                         }, {
                             1: [0]
                         }
                         ], [[0, 1], 2]]
                     },
                     'returns': []
                 },
+                
+                # minilmv2-lat-roberta
+                {
+                    'patterns': {
+                        'in': [[(0, 'input_ids'), (1, 'input_mask') ]],
+                        'out': [[(0, 'Input')]]
+                    },
+                    'search_mode': 'node_name',
+                    'node_names': {
+                        0: 'input_data'
+                    },
+                    'input_tensors': {
+                        0: [[], [[], 0]]
+                    },
+                    'output_tensors': {
+                        0: [[{
+                            0: [0]
+                        }, {
+                            1: [0]
+                        }
+                        ], [[0, 1], 2]]
+                    },
+                    'returns': []
+                },
+
+                # vit
+                {
+                    'patterns': {
+                        'in': [[(0, ['input', 'pixel_values'])]],
+                        'out': [[(0, 'Input')]]
+                    },
+                    'search_mode': 'node_name',
+                    'node_names': {
+                        0: 'input_data'
+                    },
+                    'input_tensors': {
+                        0: [[], [[], 0]]
+                    },
+                    'output_tensors': {
+                        0: [[{0: [0]}], [[0], 1]]
+                    },
+                    'returns': [0]
+                },
 
             ]
         }
 
         for i in range(len(pattern_mapping_config['InputData'])):
             pattern_dict = pattern_mapping_config['InputData'][i]
             model, new_node_names, ret_old_nodes = util.pattern_mapping("InputData",
@@ -161,8 +212,24 @@
                 model.nodes[0].attr = None
                 for j in range(len(model.nodes[0].output_tensors)):
                     if model.nodes[0].output_tensors[j].shape is None:
                         model.nodes[0].output_tensors[j].shape = [-1, -1]
 
                 return model
 
+        # if no input_data, insert input node for subgraph
+        if model.nodes[0].op_type != "Input":
+            onnx_input_nodes_list = []
+            model_input_tensors = []
+            for node in model.nodes:
+                if node.op_type == "ONNXINPUT":
+                    onnx_input_nodes_list.append(node.name)
+                    for input_tensor in node.output_tensors:
+                         model_input_tensors.append(copy.deepcopy(input_tensor))
+            input_data_node = util.construct_node('input_data',
+                                                   'Input',
+                                                   output_tensors=model_input_tensors)
+            model.insert_nodes(0, [input_data_node])
+            model.nodes[0].attr = None
+            model.remove_nodes(onnx_input_nodes_list)
+        
         return model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_file.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The InputFile Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 # remove the input_file patterns in tensorflow model if it has
 @pattern_registry(pattern_type='InputFile')
 class InputFile(Pattern):
-    def __call__(self, model):
+    """The InputFile pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'InputFile' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         patterns = {
             'InputFile': [
                 [[(0, 'Placeholder'), (2, 'Reshape'), (3, 'TensorSliceDataset'),
                   (4, 'FlatMapDataset'), (5, 'MapAndBatchDataset'), (6, 'OptimizeDataset'),
                   (7, 'ModelDataset'), (9, 'MakeIterator')],
                  [(), (1, 'Placeholder'), (5, 'MapAndBatchDataset')],
                  [(), (8, 'IteratorV2'), (9, 'MakeIterator')]],
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_bf16_node.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_bf16_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The InsertBF16Node Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 from ..ops import Tensor
 from .subgraph_matcher import EXECUTOR_TYPE
 import numpy as np
 
 
 @pattern_registry(pattern_type='InsertBF16Node')
 class InsertBF16Node(Pattern):
+    """The InsertBF16Node pattern.
 
-    def __call__(self, model):
+    Fuse the original sub-graph into the custom acceleration 'InsertBF16Node' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
 
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         def fp32_to_bf16(fp32_np):
             assert(fp32_np.dtype==np.float32)
             int32_np = fp32_np.view(dtype=np.int32)
             int32_np = int32_np >> 16
             bf16_np = int32_np.astype(np.uint16)
             return bf16_np
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_quant_node.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_quant_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The InsertQuantNode Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 from ..ops import Tensor
 from .subgraph_matcher import EXECUTOR_TYPE
 import numpy as np
 
 
 @pattern_registry(pattern_type='InsertQuantNode')
 class InsertQuantNode(Pattern):
+    """The InsertQuantNode pattern.
 
-    def __call__(self, model):
+    Fuse the original sub-graph into the custom acceleration 'InsertQuantNode' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
 
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         def get_scale_zp(tensor_min_data, tensor_max_data, dtype):
             # for asym quant
             if (dtype == 'u8'):
                 max_sub_min = tensor_max_data - tensor_min_data
                 scale = np.where(max_sub_min == 0., 0., 255. / max_sub_min)
                 zero_point = -tensor_min_data * scale
             # for sym quant
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/interact_features.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/interact_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The InteractFeatures Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='InteractFeatures')
 class InteractFeatures(Pattern):
-    def __call__(self, model):
+    """The InteractFeatures pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'InteractFeatures' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'InteractFeatures': [
                 # DLRM onnx model
                 {
                     'patterns': {
                         'in': [[(0, 'Relu'), (1, 'Shape'), (2, 'Gather'), (3, 'Unsqueeze'), 
                                 (7, 'Concat'), (9, 'Reshape')],
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/last_layer_shape.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/last_layer_shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The LastLayerShape Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 import copy
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='LastLayerShape')
 class LastLayerShape(Pattern):
-    def __call__(self, model):
+    """The LastLayerShape pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'LastLayerShape' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'LastLayerShape': [
                 {
                     'patterns': {
                         'in': [[(0, 'Pack'), (1, 'Reshape'), (2, 'Shape'), (3, 'StridedSlice'),
                                 (5, 'Mul'), (6, 'Pack'), (7, 'Reshape'), (8, 'MatMulWithBias'),
                                 (10, 'Reshape')], [(2, 'Shape'), (4, 'StridedSlice'), (5, 'Mul')],
@@ -191,15 +198,15 @@
                 mat_node = ret_old_nodes[i][1]
                 hidden_size = int(ln_node.input_tensors[-1].shape[-1])
 
                 ln_node_idx = model.get_node_id(new_node_names[i][0])
                 model.nodes[ln_node_idx].attr = ln_node.attr
                 reshape_0_node_idx = model.get_node_id(new_node_names[i][1])
                 model.nodes[reshape_0_node_idx].attr = OrderedDict({
-                    'dst_shape': '-1,-1,' + str(hidden_size), 'dims': '0,1'})
+                    'dst_shape': '-1,-1,' + str(hidden_size), 'dims': '0'})
                 strided_slice_node_idx = model.get_node_id(new_node_names[i][2])
                 model.nodes[strided_slice_node_idx].attr = OrderedDict({
                     'begin_mask': 5, 'ellipsis_mask': 0, 'end_mask': 5, 'new_axis_mask': 0,
                     'shrink_axis_mask': 0, 'begin': '0,0,0',  'end': '0,1,0', 'strides': '1,1,1'})
                 reshape_1_node_idx = model.get_node_id(new_node_names[i][3])
                 model.nodes[reshape_1_node_idx].attr = OrderedDict({
                         'dst_shape': '-1,' + str(hidden_size)})
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/layer_norm.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/layer_norm.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,32 +11,39 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The LayerNorm Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='LayerNorm')
 class LayerNorm(Pattern):
+    """The LayerNorm pattern.
+
+    Fuse the original sub-graph into the custom acceleration 'LayerNorm' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
     """
     Different model has the different layer_norm pattern,
     which means they have differrnt nodes order even though they all follow the formula.
     For exmaple:
 
     LayerNorm(src, gamma, beta)
         = gamma * (src-mean) / sqrt(variance+c) + beta  # 1, like transformer_lt
         = src * gamma / sqrt(variance+c) + (beta-mean*gamma/sqrt(variance+c)) # 2, like bert_large
     """
     def __call__(self, model):
-
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'LayerNorm': [
 
                 # bert_base has two layer_norm patterns
                 {
                     'patterns': {
                         'in': [[(0, 'Shape'), (1, 'StridedSlice'), (2, 'Mul'), (4, 'Mul'),
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/layer_norm_with_reduce_mean.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/layer_norm_with_reduce_mean.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The LayerNormWithReduceMean Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='LayerNormWithReduceMean')
 class LayerNormWithReduceMean(Pattern):
-    def __call__(self, model):
+    """The LayerNormWithReduceMean pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'LayerNormWithReduceMean' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'LayerNormWithReduceMean': [
                 {
                     'patterns': {
                         'in': [[(0, 'LayerNorm'), (1, 'ReduceMean')]],
                         'out': [[(0, 'LayerNorm'), (1, 'Reshape'), (2, 'ReduceMean'),
                                 (3, 'Reshape')]]
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,25 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The MatMulWithBias pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 from ..onnx_utils import bias_to_int32
 import copy
 
 
 @pattern_registry(pattern_type='MatMulWithBias')
 class MatMulWithBias(Pattern):
-    def __call__(self, model):
+    """The MatMulWithBias pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'MatMulWithBias' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'MatMulWithBias': [
                 {
                     'patterns': {
                         'in': [[(0, 'MatMul'), (1, ['BiasAdd', 'Add'])]],
                         'out': [[(0, 'MatMulWithBias')]]
                     },
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_add.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_tanh.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,46 +11,49 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The MatmulWithBiasTanh pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
-from ..onnx_utils import bias_to_int32
-import copy
 
 
-@pattern_registry(pattern_type='MatMulWithBiasAdd')
-class MatMulWithBiasAdd(Pattern):
+@pattern_registry(pattern_type='MatMulWithBiasTanh')
+class MatmulWithBiasTanh(Pattern):
+    """The MatmulWithBiasTanh pattern.
+
+    Fuse the original sub-graph into the custom acceleration 'MatmulWithBiasTanh' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
     def __call__(self, model):
-
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
-            'MatMulWithBiasAdd': [
+            'MatMulWithBiasTanh': [
                 {
                     'patterns': {
-                        'in': [[(0, 'MatMulWithBias'), (1, ['Add', 'AddV2'])]],
-                        'out': [[(0, 'MatMulWithBiasAdd')]]
+                        'in': [[(0, 'MatMulWithBias'), (1, ['Tanh'])]],
+                        'out': [[(0, 'MatMulWithBiasTanh')]]
                     },
                     'search_mode': 'op_type',
                     'node_names': {
                         0: 1
                     },
                     'input_tensors': {
                         0: [[{
                             0: [0]
                         }, {
                             0: [1]
                         }, {
                             0: [2]
-                        }, {
-                            1: [0, 1]
-                        }], [[0, 1, 2, 3], 4]]
+                        }], [[0, 1, 2], 3]]
                     },
                     'output_tensors': {
                         0: [[{
                             1: [0]
                         }], [[0], 1]]
                     },
                     'returns': [0]
@@ -62,19 +65,19 @@
             for i in range(len(new_node_names)):
                 mat_node_idx = model.get_node_id(new_node_names[i][0])
                 attr = OrderedDict()
                 if 'src0_perm' in ret_old_nodes[i][0].attr.keys():
                     attr['src0_perm'] = ret_old_nodes[i][0].attr['src0_perm']
                 if 'src1_perm' in ret_old_nodes[i][0].attr.keys():
                     attr['src1_perm'] = ret_old_nodes[i][0].attr['src1_perm']
-                attr['append_op'] = 'sum'
+                attr['append_op'] = 'tanh'
                 model.nodes[mat_node_idx].attr = attr
 
-        pattern_dict = pattern_mapping_config['MatMulWithBiasAdd'][0]
-        model, new_node_names, ret_old_nodes = util.pattern_mapping("MatMulWithBiasAdd",
+        pattern_dict = pattern_mapping_config['MatMulWithBiasTanh'][0]
+        model, new_node_names, ret_old_nodes = util.pattern_mapping("MatMulWithBiasTanh", 
                                                                     pattern_dict, model)
         if len(new_node_names) != 0:
             _set_attr(new_node_names, ret_old_nodes, model)
 
             return model
 
         return model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_gelu.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_gelu.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The MatMulWithBiasGelu Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 import copy
 
 
 @pattern_registry(pattern_type='MatMulWithBiasGelu')
 class MatMulWithBiasGelu(Pattern):
-    def __call__(self, model):
+    """The MatMulWithBiasGelu pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'MatMulWithBiasGelu' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'MatMulWithBiasGelu': [
                 {
                     'patterns': {
                         'in': [[(0, 'MatMulWithBias'), (1, ['Gelu'])]],
                         'out': [[(0, 'MatMulWithBiasGelu')]]
                     },
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_relu.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_add.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,41 +11,53 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The MatMulWithBiasAdd Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
+from ..onnx_utils import bias_to_int32
+import copy
+
 
+@pattern_registry(pattern_type='MatMulWithBiasAdd')
+class MatMulWithBiasAdd(Pattern):
+    """The MatMulWithBiasAdd pattern.
 
-@pattern_registry(pattern_type='MatMulWithBiasRelu')
-class MatMulWithBiasRelu(Pattern):
+    Fuse the original sub-graph into the custom acceleration 'MatMulWithBiasAdd' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
     def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
-            'MatMulWithBiasRelu': [
+            'MatMulWithBiasAdd': [
                 {
                     'patterns': {
-                        'in': [[(0, 'MatMulWithBias'), (1, ['Relu'])]],
-                        'out': [[(0, 'MatMulWithBiasRelu')]]
+                        'in': [[(0, 'MatMulWithBias'), (1, ['Add', 'AddV2'])]],
+                        'out': [[(0, 'MatMulWithBiasAdd')]]
                     },
                     'search_mode': 'op_type',
                     'node_names': {
                         0: 1
                     },
                     'input_tensors': {
                         0: [[{
                             0: [0]
                         }, {
                             0: [1]
                         }, {
                             0: [2]
-                        }], [[0, 1, 2], 3]]
+                        }, {
+                            1: [0, 1]
+                        }], [[0, 1, 2, 3], 4]]
                     },
                     'output_tensors': {
                         0: [[{
                             1: [0]
                         }], [[0], 1]]
                     },
                     'returns': [0]
@@ -57,19 +69,19 @@
             for i in range(len(new_node_names)):
                 mat_node_idx = model.get_node_id(new_node_names[i][0])
                 attr = OrderedDict()
                 if 'src0_perm' in ret_old_nodes[i][0].attr.keys():
                     attr['src0_perm'] = ret_old_nodes[i][0].attr['src0_perm']
                 if 'src1_perm' in ret_old_nodes[i][0].attr.keys():
                     attr['src1_perm'] = ret_old_nodes[i][0].attr['src1_perm']
-                attr['append_op'] = 'relu'
+                attr['append_op'] = 'sum'
                 model.nodes[mat_node_idx].attr = attr
 
-        pattern_dict = pattern_mapping_config['MatMulWithBiasRelu'][0]
-        model, new_node_names, ret_old_nodes = util.pattern_mapping("MatMulWithBiasRelu", 
+        pattern_dict = pattern_mapping_config['MatMulWithBiasAdd'][0]
+        model, new_node_names, ret_old_nodes = util.pattern_mapping("MatMulWithBiasAdd",
                                                                     pattern_dict, model)
         if len(new_node_names) != 0:
             _set_attr(new_node_names, ret_old_nodes, model)
 
             return model
 
         return model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_sigmoid.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_sigmoid.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,22 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The MatMulWithBiasSigmoid pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='MatMulWithBiasSigmoid')
 class MatMulWithBiasSigmoid(Pattern):
+    """The MatMulWithBiasSigmoid pattern.
+
+    Fuse the original sub-graph into the custom acceleration 'MatMulWithBiasSigmoid' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
     def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'MatMulWithBiasSigmoid': [
                 {
                     'patterns': {
                         'in': [[(0, 'MatMulWithBias'), (1, ['Sigmoid'])]],
                         'out': [[(0, 'MatMulWithBiasSigmoid')]]
                     },
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/merged_embeddingbag.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/merged_embeddingbag.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The MergedEmbeddingbag pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='MergedEmbeddingbag')
 class MergedEmbeddingbag(Pattern):
-    def __call__(self, model):
+    """The MergedEmbeddingbag pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'MergedEmbeddingbag' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'MergedEmbeddingbag': [
                 # DLRM onnx model
                 {
                     'patterns': {
                         'in': [[(0, 'Split'), (1, 'Squeeze'), (2, 'Shape'),
                                 (3, 'Gather'), (5, 'Unsqueeze'), (6, 'Concat'),
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/output_data.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/output_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,27 +11,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The OutputData Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 import copy
 
 
 @pattern_registry(pattern_type='OutputData')
 class OutputData(Pattern):
-    def __call__(self, model):
+    """The OutputData pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'OutputData' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         # make the output_data node in graph
-        last_node = model.nodes[-1]
-        input_tensors = copy.deepcopy(last_node.output_tensors)
+        model_output_tensors = []
+        for node in model.nodes:
+            for output_tensor in node.output_tensors:
+                if not output_tensor.dest_op:
+                    model_output_tensors.append(copy.deepcopy(output_tensor))
         output_data_node = util.construct_node('output_data',
                                                'Output',
-                                               input_tensors=input_tensors)
+                                               input_tensors=model_output_tensors)
         model.insert_nodes(len(model.nodes), [output_data_node])
         model.nodes[-1].attr = None
-        
+
         return model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/padding_sequence.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/padding_sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The PaddingSequence pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 import copy
 from .. import graph_utils as util
 from ..ops.tensor import Tensor
 
 
 @pattern_registry(pattern_type='PaddingSequence')
 class PaddingSequence(Pattern):
+    """The PaddingSequence pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'PaddingSequence' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
     def __call__(self, model):
-
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'PaddingSequence': [
                 {
                     'patterns': {
                         'in': [[(1, 'Shape'), (2, 'StridedSlice'), (5, 'Pack'), (6, 'Reshape'),
                                 (7, 'ExpandDims'), (8, 'Sub'), (9, 'Mul'), (10, ['Add', 'AddV2'])],
                                [(), (3, 'Shape'), (4, 'StridedSlice'), (5, 'Pack')],
@@ -80,41 +86,37 @@
                     'output_tensors': {
                         0: [[{
                             11: [0]
                         }], [[0], 1]]
                     },
                     'returns': []
                 },
-
                 # geminet, bert_related in huggingface
                 {
                     'patterns': {
                         'in': [[(0, 'Unsqueeze'), (1, 'Unsqueeze'), (2, 'Cast'), (3, 'Sub'),
-                                (4, 'Mul'), (5, 'Add')]],
-                        'out': [[(0, 'AddV2')]]
+                                (4, 'Mul')]],
+                        'out': [[(0, 'PaddingSequence')]]
                     },
                     'search_mode': 'op_type',
                     'node_names': {
-                        0: 5
+                        0: 4
                     },
                     'input_tensors': {
                         0: [[{
-                            5: [0]
-                        }, {
-                            'padding_sequence': [0]
-                        }], [[0, 1], 2]]
+                            'input_data': [-1]
+                        }], [[0], 1]]
                     },
                     'output_tensors': {
                         0: [[{
-                            5: [0]
+                            4: [0]
                         }], [[0], 1]]
                     },
                     'returns': []
                 },
-
                 # distil_bert_base
                 {
                     'patterns': {
                         'in': [[(1, 'Unsqueeze'), (3, 'Concat'), (4, 'Reshape'), (6, 'Expand'),
                                 (7, 'Cast'), (8, 'Where')], [(), (2, 'Unsqueeze'), (3, 'Concat')],
                                [(), (5, 'Shape'), (6, 'Expand')], [(), (0, 'Equal'),
                                                                    (4, 'Reshape')]],
@@ -181,15 +183,19 @@
             input_data = model.nodes[0]
             if len(input_data.output_tensors) > tensor_idx:
                 input_tensors = [copy.deepcopy(input_data.output_tensors[tensor_idx])]
             else:
                 input_tensors = [Tensor()]
             output_tensors = [Tensor(name=node_name + ':0', source_op=[node_name], dest_op=[])]
             attr = OrderedDict()
-            attr['dst_shape'] = '-1,' + str(heads_num) + ',0,-1'
+            if not is_lat_model(model):
+                attr['dst_shape'] = '-1,' + str(heads_num) + ',0,-1'
+            else:
+                attr['dst_shape'] = '-1,' + str(1) + ',1,-1'
+
             attr['dims'] = 1
             padding_sequence_node = util.construct_node(node_name,
                                                         'PaddingSequence',
                                                         input_tensors=input_tensors,
                                                         output_tensors=output_tensors,
                                                         attr=attr)
 
@@ -205,14 +211,21 @@
             if len(match_result) != 0:
                 mat_node = model.get_node_by_name(match_result[0][mat_idx])
                 hidden_size = int(mat_node.input_tensors[1].shape[-1])
             else:
                 hidden_size = -1
             return hidden_size
 
+        def is_lat_model(model, p=None):
+            if p == None:
+                p = [[(0, 'TopK'),(1, 'Unsqueeze'),(2, 'Unsqueeze'),(3, 'Expand'),
+                    (4, 'GatherElements')]]
+            match_result = util.search_pattern(p, model)
+            return len(match_result) != 0
+
         pattern_dict = pattern_mapping_config['PaddingSequence'][0]
         model = _make_padding_sequence_node(2, 1024, model)
         model, new_node_names, ret_old_nodes = util.pattern_mapping("PaddingSequence",
                                                                     pattern_dict, model)
         if len(new_node_names) != 0:
             return model
         else:
@@ -233,15 +246,21 @@
             model = _make_padding_sequence_node(2, hidden_size, model)
         else:
             model = _make_padding_sequence_node(1, hidden_size, model)
         model, new_node_names, ret_old_nodes = util.pattern_mapping("PaddingSequence",
                                                                     pattern_dict, model)
 
         if len(new_node_names) != 0:
-            assert hidden_size != -1, "Wrong hidden size in padding_sequence!"
+            assert hidden_size!=-1, "Wrong hidden size in padding_sequence!"
+            ps_attr = model.get_node_by_name('padding_sequence').attr
+            for j in range(len(new_node_names)):
+                ps_node_id = model.get_node_id(new_node_names[j][0])
+                model.nodes[ps_node_id].attr = ps_attr
+            # remove fake node
+            model.remove_nodes(['padding_sequence'])
             return model
         else:
             model.remove_nodes(['padding_sequence'])
 
         pattern_dict = pattern_mapping_config['PaddingSequence'][3]
         model = _make_padding_sequence_node(1, 768, model)
         model, new_node_names, ret_old_nodes = util.pattern_mapping("PaddingSequence",
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/pattern.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/pattern.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The supported pattern file."""
+
 from abc import abstractmethod
 
 # for complicated pattern, use a several lists and tuple to represent the main computation flow
 # and sub-graphs
 # for example, layer_norm pattern in bert_large:
 # pattern: [ [(0, 'Mean'), (1, 'SquaredDifference'), (2, 'Mean'), (3, 'AddV2'), (4, 'Rsqrt'),
 #             (5, 'Mul'),
@@ -34,33 +36,44 @@
     'WordEmbeddings',
     'MergedEmbeddingbag',
     'EmbeddingBag',
     'TokenTypeEmbeddings',
     'TokenTypeEmbeddingsV1',
     'PositionEmbeddings',
     'PositionEmbeddingsV1',
+    'GenerateSequence',
     'PaddingSequence',
+    'AttentionMaskLengthAdaptiveExpandIndices',
     'MatMulWithBias',
     'LastLayerShape',
     'InteractFeatures',
     'AttentionReshape',
     'QKVReshape',
+    'ConvReshape',
+    'AddClsToken',
     'TransposeBatchMatMul',
     'Gelu',
     'MatMulWithBiasGelu',
     'MatMulWithBiasAdd',
     'AddEmbeddings',
     'MatMulWithBiasTanh',
     'MatMulWithBiasRelu',
     'MatMulWithBiasSigmoid',
+    "RestoreHiddenStatesInLengthAdaptiveUpdateIndices",
+    "AttentionOutputLayerNormLengthAdaptiveExpandIndices",
+    "ReshapeBeforeAndAfterAttentionOutLayerNormGatherElements",
+    "ReshapeBeforeRestoreHiddenStates",
+    "ReshapeAfterRestoreHiddenStates",
     'LayerNormWithReduceMean',
     'StartEndLogits',
     'InsertQuantNode',
     'InsertBF16Node',
     'QunatizeFusion',
+    'QKVMerge',
+    'ReshapeFusion',
     'OutputData',
 ]
 
 # for superbert, superbert patterns are huge patterns based on supported patterns
 superbert_patterns = []
 
 PATTERNS = {}
@@ -73,19 +86,22 @@
         cls (class): The class of register.
         pattern_type (str): The pattern registration name
 
     Returns:
         cls: The class of register.
     """
     def decorator_pattern(cls):
+        """The pattern decorator."""
         if pattern_type in PATTERNS:
             raise ValueError('Cannot have two patterns with the same name')
         PATTERNS[pattern_type] = cls
         return cls
 
     return decorator_pattern
 
 
 class Pattern(object):
+    """The bass pattern class."""
     @abstractmethod
     def __call__(self, model, *args, **kwargs):
+        """The __call__ function of the pattern class."""
         raise NotImplementedError
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The PositionEmbeddings pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='PositionEmbeddings')
 class PositionEmbeddings(Pattern):
-    def __call__(self, model):
+    """The PositionEmbeddings pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'PositionEmbeddings' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'PositionEmbeddings': [
                 {
                     'patterns': {
                         'in': [[(0, 'Shape'), (1, 'StridedSlice'), (2, 'Pack'), (3, 'Slice'),
                                 (5, 'Reshape')], [(1, 'StridedSlice'), (4, 'Pack'),
                                                   (5, 'Reshape')]],
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings_v1.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings_v1.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The PositionEmbeddingsV1 pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='PositionEmbeddingsV1')
 class PositionEmbeddingsV1(Pattern):
-    def __call__(self, model):
+    """The PositionEmbeddingsV1 pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'PositionEmbeddingsV1' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'PositionEmbeddingsV1': [
                 # roberta_base
                 {
                     'patterns': {
                         'in': [[(0, 'Equal'), (1, 'Not'), (2, 'Cast'), (3, 'CumSum'), 
                                 (4, 'Add'), (5, 'Mul'), (6, 'Cast'), (7, 'Add'), (8, 'Gather')]],
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/qkv_reshape.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_output_layer_norm_length_adaptive_keep_indices.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,219 +11,191 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The AttentionOutputLayerNormLengthAdaptiveExpandIndices Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
-import copy
 from .. import graph_utils as util
+import numpy as np
 
 
-@pattern_registry(pattern_type='QKVReshape')
-class QKVReshape(Pattern):
+@pattern_registry(pattern_type='AttentionOutputLayerNormLengthAdaptiveExpandIndices')
+class AttentionOutputLayerNormLengthAdaptiveExpandIndices(Pattern):
+    """The AttentionOutputLayerNormLengthAdaptiveExpandIndices pattern.
 
-    def __call__(self, model):
+    Fuse the original sub-graph into the custom acceleration graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
 
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
-            'QKVReshape': [
+            'AttentionOutputLayerNormLengthAdaptiveExpandIndices': [
+                # minilmv2-lat-roberta-2-seq
                 {
                     'patterns': {
-                        'in': [[(0, 'Shape'), (1, 'StridedSlice'), (3, 'Pack'), (4, 'Reshape')],
-                               [(0, 'Shape'), (2, 'StridedSlice'), (3, 'Pack')]],
-                        'out': [[(0, 'Reshape')]]
+                        'in': [[(0, 'Shape'), (1, 'Gather'), (2, 'Unsqueeze'), (6, 'Concat'),
+                                (7, 'Reshape'), (8, 'Shape'), (9, 'ConstantOfShape'), (10, 'Mul'),
+                                (11, 'Equal'), (12, 'Where'), (14, 'Expand')],
+                               [(), (3, 'Shape'), (4, 'Gather'), (5, 'Unsqueeze'), (6, 'Concat')],
+                               [(), (13, 'Unsqueeze'), (14, 'Expand')]],
+                        'out': [[(0, 'ExpandIndices')]]
                     },
                     'search_mode': 'op_type',
                     'node_names': {
-                        0: 4
+                        0: 14,
                     },
                     'input_tensors': {
                         0: [[{
-                            4: [0]
+                            13: [0]
                         }, {
-                            'input_data': [0]
-                        }], [[0, 1], 2]]
+                            0: [0]
+                        }], [[0, 1], 2]],
                     },
                     'output_tensors': {
                         0: [[{
-                            4: [0]
-                        }], [[0], 1]]
+                            14: [0]
+                        }], [[0], 1]],
                     },
-                    'returns': [3]
+                    'returns': [13]
                 },
-
-                # bert_base_mrpc
+                # minilmv2-lat-roberta-1-seq
+                # concat 155
                 {
                     'patterns': {
-                        'in': [[(0, 'Shape'), (1, 'StridedSlice'), (2, 'Pack'), (3, 'Reshape')]],
-                        'out': [[(0, 'Reshape')]]
+                        'in': [[(0, 'Shape'), (1, 'Gather'), (2, 'Unsqueeze'), (3, 'Concat'),
+                                (4, 'Reshape'), (5, 'Shape'), (6, 'ConstantOfShape'), (7, 'Mul'),
+                                (8, 'Equal'), (9, 'Where'), (10, 'Expand')],
+                               [(), (11, 'Unsqueeze'), (10, 'Expand')]],
+                        'out': [[(0, 'ExpandIndices')]]
                     },
                     'search_mode': 'op_type',
                     'node_names': {
-                        0: 3
+                        0: 10,
                     },
                     'input_tensors': {
                         0: [[{
-                            3: [0]
+                            11: [0]
                         }, {
-                            'input_data': [0]
-                        }], [[0, 1], 2]]
+                            0: [0]
+                        }], [[0, 1], 2]],
                     },
                     'output_tensors': {
                         0: [[{
-                            3: [0]
-                        }], [[0], 1]]
+                            10: [0]
+                        }], [[0], 1]],
                     },
-                    'returns': [2]
+                    'returns': [11]
                 },
-
-                # bert_base_sparse
+                # ConstantOfShape_573,323
                 {
                     'patterns': {
-                        'in': [[(0, 'MatMulWithBias'), (1, 'Shape'), (2, 'Gather'),
-                                (3, 'Unsqueeze'), (7, 'Concat'), (8, 'Reshape')],
-                               [(), (4, 'Shape'), (5, 'Gather'), (6, 'Unsqueeze'), (7, 'Concat')]],
-                        'out': [[(0, 'MatMulWithBias'), (1, 'Reshape')]]
+                        'in': [[(0, 'ConstantOfShape'), (1, 'Mul'),
+                                (2, 'Equal'), (3, 'Where'), (4, 'Expand'), (5, 'GatherElements')],
+                               [(), (6, 'Unsqueeze'), (7, 'Unsqueeze'), (4, 'Expand')]],
+                        'out': [[(0, 'ExpandIndices'), (1, 'GatherElements')]]
                     },
                     'search_mode': 'op_type',
                     'node_names': {
-                        0: 0,
-                        1: 8
+                        0: 4,
+                        1: 5,
                     },
                     'input_tensors': {
                         0: [[{
-                            0: [0]
+                            6: [0]
                         }, {
-                            0: [1]
-                        }, {
-                            0: [2]
-                        }], [[0, 1, 2], 3]],
+                            5: [0]
+                        }], [[0, 1], 2]],
+
                         1: [[{
-                            'input_data': [0]
-                        }], [[1], 2]],
+                            5: [0]
+                        },
+
+                        ], [[0], 2]],
                     },
                     'output_tensors': {
                         0: [[], [[], 1]],
                         1: [[{
-                            8: [0]
-                        }], [[0], 1]]
+                            5: [0]
+                        }], [[0], 1]],
                     },
-                    'returns': [7, 0]
+                    'returns': [5,6,7]
                 },
-
-                # distil_bert_base
+                # ConstantOfShape_272, 517
                 {
                     'patterns': {
-                        'in': [[(0, 'Shape'), (1, 'Gather'), (2, 'Unsqueeze'), (3, 'Concat'),
-                                (4, 'Reshape')]],
-                        'out': [[(0, 'Reshape')]]
+                        'in': [[(0, 'ConstantOfShape'), (1, 'Mul'),
+                                (2, 'Equal'), (3, 'Where'), (4, 'Expand'), (5, 'GatherElements')],
+                               [(), (6, 'Unsqueeze'), (4, 'Expand')]],
+                        'out': [[(0, 'ExpandIndices'), (1, 'GatherElements')]]
                     },
                     'search_mode': 'op_type',
                     'node_names': {
-                        0: 4
+                        0: 4,
+                        1: 5,
                     },
                     'input_tensors': {
                         0: [[{
-                            4: [0]
+                            6: [0]
                         }, {
-                            'input_data': [0]
-                        }], [[0, 1], 2]]
-                    },
-                    'output_tensors': {
-                        0: [[{
-                            4: [0]
-                        }], [[0], 1]]
-                    },
-                    'returns': [3]
-                },
+                            5: [0]
+                        }], [[0, 1], 2]],
 
-                # geminet
-                {
-                    'patterns': {
-                        'in': [[(0, 'MatMulWithBias'), (1, 'Reshape')]],
-                        'out': [[(0, 'MatMulWithBias'), (1, 'Reshape')]]
-                    },
-                    'search_mode': 'op_type',
-                    'node_names': {
-                        0: 0,
-                        1: 1
-                    },
-                    'input_tensors': {
-                        0: [[{
-                            0: [0]
-                        }, {
-                            0: [1]
-                        }, {
-                            0: [2]
-                        }], [[0, 1, 2], 3]],
                         1: [[{
-                            'input_data': [0]
-                        }], [[1], 2]],
+                            5: [0]
+                        },
+
+                        ], [[0], 2]],
                     },
                     'output_tensors': {
-                        0: [[{
-                            0: [0]
-                        }], [[0], 1]],
+                        0: [[], [[], 1]],
                         1: [[{
-                            1: [0]
-                        }], [[0], 1]]
+                            5: [0]
+                        }], [[0], 1]],
                     },
-                    'returns': [0, 1]
+                    'returns': [5,6]
                 },
             ]
         }
 
-        def _set_attr(head_num, head_size, node_names, model):
-            attr = OrderedDict()
-            attr['dst_shape'] = '-1,-1,' + str(head_num) + ',' + str(head_size)
-            attr['dims'] = '0'
-
-            reshape_node_idx = model.get_node_id(node_names[0])
-            model.nodes[reshape_node_idx].attr = attr
+        # minilmv2-lat-roberta
+        #for _, pattern_dict in pattern_mapping_config.items():
+        for idx in range(len(pattern_mapping_config[
+            'AttentionOutputLayerNormLengthAdaptiveExpandIndices'])):
 
-        for i in range(len(pattern_mapping_config['QKVReshape']) - 1):
-            pattern_dict = pattern_mapping_config['QKVReshape'][i]
+            pattern_dict = pattern_mapping_config[
+                'AttentionOutputLayerNormLengthAdaptiveExpandIndices'][idx]
             model, new_node_names, ret_old_nodes = util.pattern_mapping(
-                "QKVReshape", pattern_dict, model)
+                 'AttentionOutputLayerNormLengthAdaptiveExpandIndices', pattern_dict, model)
             if len(new_node_names) != 0:
-                for j in range(len(new_node_names)):
-                    pack_node = ret_old_nodes[j][0]
-                    head_size = int(pack_node.input_tensors[-1].data)
-                    head_num = int(pack_node.input_tensors[-2].data)
-                    _set_attr(head_num, head_size, new_node_names[j], model)
-                    if len(ret_old_nodes[j]) == 2:
-                        assert ret_old_nodes[j][1].op_type == 'MatMulWithBias'
-                        mat_node_idx = model.get_node_id(new_node_names[j][0])
-                        model.nodes[mat_node_idx].attr = ret_old_nodes[j][1].attr
-                        reshape_node_idx = model.get_node_id(new_node_names[j][1])
-                        model.nodes[reshape_node_idx].attr = OrderedDict({
-                            'dst_shape': '-1,-1,' + str(head_num) + ',' + str(head_size),
-                            'dims': '0'
-                        })
-                return model
-
-        # special reshape node, like has '0,0,12,64' dst_shape attr
-        pattern_dict = pattern_mapping_config['QKVReshape'][-1]
-        model, new_node_names, ret_old_nodes = util.pattern_mapping("QKVReshape", pattern_dict,
-                                                                    model)
-        if len(new_node_names) != 0:
-            for j in range(len(new_node_names)):
-                reshape_node = ret_old_nodes[j][1]
-                try:
-                    dst_shape = reshape_node.attr['dst_shape']
-                except:
-                    dst_shape = None
-                if dst_shape != None and dst_shape.split(',')[0] == '0':
-                    head_num = int(dst_shape.split(',')[-2])
-                    reshape_node_idx = model.get_node_id(new_node_names[j][1])
-                    model.nodes[reshape_node_idx].attr = OrderedDict({
-                        'dst_shape': '-1,-1,' + str(head_num) + ',64',
-                        'dims': '0'
-                    })
-                mat_node_idx = model.get_node_id(new_node_names[j][0])
-                model.nodes[mat_node_idx].attr = ret_old_nodes[j][0].attr
+                for i in range(len(new_node_names)):
+                    attr = OrderedDict()
+                    attr_gather = OrderedDict()
+                    input_indices = []
+                    axis_gather = []
+                    for ret_old_node in ret_old_nodes[i]:
+                        if ret_old_node.op_type == 'Unsqueeze':
+                           input_indices.append(int(ret_old_node.attr['axis']))
+                        elif ret_old_node.op_type == 'GatherElements':
+                            axis_gather.append(int(ret_old_node.attr['axis']))
+
+
+                    attr['position'] = util.list2str(input_indices)
+                    keep_indices_node_idx = model.get_node_id(new_node_names[i][0])
+                    model.nodes[keep_indices_node_idx].attr = attr
+
+                    # set attr for gather_elements
+                    if 1 < len(new_node_names[i]):
+                       attr_gather['axis'] = util.list2str(axis_gather)
+                       gather_element_node_idx = model.get_node_id(new_node_names[i][1])
+                       model.nodes[gather_element_node_idx].attr = attr_gather
+
+
 
-            return model
+                #return model
 
         return model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/quantize_fusion.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/quantize_fusion.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,26 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The QunatizeFusion Pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 from ..ops import Tensor
 from .subgraph_matcher import EXECUTOR_TYPE
 
 
 @pattern_registry(pattern_type='QunatizeFusion')
 class QunatizeFusion(Pattern):
+    """The QunatizeFusion pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'QunatizeFusion' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
     def __call__(self, model):
-
+        """The __call__ function of this pattern class."""
         def search_quant_fusion(node):
             if node.input_tensors[0].source_op == []:
                 return (None, False)
             pre_node = model.get_node_by_name(node.input_tensors[0].source_op[0])
             if pre_node.name in quant_info or (pre_node.op_type == "Softmax") \
                or (not quant_info and pre_node.op_type in EXECUTOR_TYPE \
                    and (EXECUTOR_TYPE[pre_node.op_type] == "InnerProduct" or \
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/start_end_logits.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/start_end_logits.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The StartEndLogits pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 import copy
 from .. import graph_utils as util
 from ..ops.tensor import Tensor
 
 
 @pattern_registry(pattern_type='StartEndLogits')
 class StartEndLogits(Pattern):
-    def __call__(self, model):
+    """The StartEndLogits pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'StartEndLogits' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         patterns = {
             'StartEndLogits': [
                 # bert_large_sparse_model in squadv1 dataset
                 [[(0, 'Transpose'), (1, 'Unpack'), (2, 'Identity')]],
                 # bert_large_squad from huggingface in squadv1 dataset
                 [[(0, 'Split'), (1, 'Squeeze')]],
             ]
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/subgraph_matcher.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/subgraph_matcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine subgraph matcher file."""
+
 import time
 import copy
 import numpy as np
 from tqdm import tqdm
 from .pattern import supported_patterns, superbert_patterns, PATTERNS
 from .. import logger
 
@@ -26,14 +28,15 @@
     "MatMulWithBias": "InnerProduct",
     "MatMulWithBiasAdd": "InnerProduct",
     "MatMulWithBiasGelu": "InnerProduct",
     "MatMulWithBiasTanh": "InnerProduct",
     "MatMulWithBiasRelu": "InnerProduct",
     "MatMulWithBiasSigmoid": "InnerProduct",
     "MatMul": "InnerProduct",
+    "Conv": "Convolution",
     "QuantizedMatMulWithBiasAndDequantize": "InnerProduct",
     "TransposeBatchMatMul": "Matmul",
     "BatchMatMul": "Matmul",
     "BatchMatMulV2": "Matmul",
     "Add": "BinaryAdd",
     "AddV2": "BinaryAdd",
     "AddWithAdd": "BinaryAdd",
@@ -48,26 +51,42 @@
     "FusedGemm": "InnerProduct",
     "_QuantizedFusedMatMulAndDequantize": "InnerProduct",
     "_FusedMatMul": "InnerProduct",
     "_MklLayerNorm": "LayerNorm",
 }
 
 class SubGraphMatcher(object):
-    def __call__(self, model, tune = False):
+    """The SubGraphMatcher class."""
+    def __call__(self, model, tune = False, pattern_config = None):
+        """The __call__ function of SubGraphMatcher class."""
         logger.info('Start to implement Sub-Graph matching and replacing...') 
         if tune:
             self._tune_patterns(model)
         else:
-            self._fuse_patterns(model)
+            self._fuse_patterns(model, pattern_config=pattern_config)
         logger.info('Sub-Graph match and replace done...')
         return model
 
-    def _fuse_patterns(self, model, supported_patterns=supported_patterns, pattern_mask=None):
+    def _fuse_patterns(self, model, supported_patterns=supported_patterns, pattern_mask=None, pattern_config=None):
         pattern_mask = [True for _ in range(len(supported_patterns))] \
-                        if pattern_mask == None else pattern_mask
+                if pattern_mask == None else pattern_mask
+        
+        for index in range(len(supported_patterns)):
+            pattern_name = supported_patterns[index]
+            if pattern_name == 'QKVMerge':
+                pattern_mask[index] = False
+
+        # modify the pattern mask according to pattern_config
+        if pattern_config != None:
+            for index in range(len(supported_patterns)):
+                pattern_name = supported_patterns[index]
+                if pattern_name in pattern_config['pattern_switch']:
+                    status = pattern_config['pattern_switch'][pattern_name]
+                    pattern_mask[index] = status
+
         for pattern_id, pattern in enumerate(supported_patterns):
             if pattern in PATTERNS and pattern_mask[pattern_id]:
                 p_fusion = PATTERNS[pattern]()
                 model = p_fusion(model)
         self._remove_identity(model) 
          
     def _tune_patterns(self, model, iterations = 10, warm_up = 5):
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The TokenTypeEmbeddings pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='TokenTypeEmbeddings')
 class TokenTypeEmbeddings(Pattern):
-    def __call__(self, model):
+    """The TokenTypeEmbeddings pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'TokenTypeEmbeddings' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'TokenTypeEmbeddings': [
                 {
                     'patterns': {
                         'in': [[(0, 'Reshape'), (1, 'Gather'), (4, 'Reshape')],
                                [(), (2, 'StridedSlice'), (3, 'Pack'), (4, 'Reshape')]],
                         'out': [[(0, 'Reshape'), (1, 'Gather'), (2, 'Reshape'), (3, 'Reshape')]]
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings_v1.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The TokenTypeEmbeddingsV1 pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 import numpy as np
 
 
 @pattern_registry(pattern_type='TokenTypeEmbeddingsV1')
 class TokenTypeEmbeddingsV1(Pattern):
-    def __call__(self, model):
+    """The TokenTypeEmbeddingsV1 pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'TokenTypeEmbeddingsV1' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'TokenTypeEmbeddingsV1': [
                 # roberta_base
                 {
                     'patterns': {
                         'in': [[(2, 'Shape'), (3, 'Gather'), (7, 'Unsqueeze'), (8, 'Concat'),
                                 (9, 'Reshape'), (10, 'Shape'), (11, 'ConstantOfShape'),
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/transpose_batch_matmul.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/transpose_batch_matmul.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The TransposeBatchMatMul pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 import copy
 from .. import graph_utils as util
 import copy
 
 
 @pattern_registry(pattern_type='TransposeBatchMatMul')
 class TransposeBatchMatMul(Pattern):
-    def __call__(self, model):
+    """The TransposeBatchMatMul pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'TransposeBatchMatMul' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'TransposeBatchMatMul': [
                 {
                 'patterns': {
                     'in': [[(0, 'Transpose'), (2, ['BatchMatMul', 'BatchMatMulV2']), (3, 'Mul'),
                             (4, ['AddV2', 'Add'])],
                            [(), (1, 'Transpose'), (2, ['BatchMatMul', 'BatchMatMulV2'])]],
@@ -108,14 +115,45 @@
                     0: [[{
                         4: [0]
                     }], [[0], 1]]
                 },
                 'returns': [0, 1, 2, 3]
             },
 
+            # vit
+            {
+                'patterns': {
+                    'in': [[(0, 'Transpose'), (2, 'MatMul'), (3, 'Div'), (4, 'Softmax')],
+                           [(), (1, 'Transpose'), (2, 'MatMul')]],
+                    'out': [[(0, 'TransposeBatchMatMul'), (1, 'Softmax')]]
+                },
+                'search_mode': 'op_type',
+                'node_names': {
+                    0: 2,
+                    1: 4
+                },
+                'input_tensors': {
+                    0: [[{
+                        0: [0]
+                    }, {
+                        1: [0]
+                    }], [[0, 1], 2]],
+                    1: [[], [[], 1]]
+                },
+                'output_tensors': {
+                    0: [[{
+                        3: [0]
+                    }], [[0], 1]],
+                    1: [[{
+                        4: [0]
+                    }], [[0], 1]]
+                },
+                'returns': [0, 1, 2, 3, 4]
+            },
+
             # geminet
             {
                 'patterns': {
                     'in': [[(0, 'Transpose'), (2, 'FusedMatMul'), (3, ['AddV2', 'Add'])],
                            [(), (1, 'Transpose'), (2, 'FusedMatMul')]],
                     'out': [[(0, 'TransposeBatchMatMul')]]
                 },
@@ -199,15 +237,20 @@
                     else:
                         if ret_old_nodes[j][3].op_type == 'Div':
                             output_scale = 1.0 / ret_old_nodes[j][3].input_tensors[1].data
                         else:
                             output_scale = ret_old_nodes[j][3].input_tensors[1].data
                     attr['output_scale'] = float(output_scale)
                     attr['format_any'] = False
-                    attr['append_op'] = 'binary_add'
+                    if len(ret_old_nodes[j]) == 5 \
+                        and ret_old_nodes[j][4].op_type == 'Softmax':
+                        softmax_node_idx = model.get_node_id(new_node_names[j][1])
+                        model.nodes[softmax_node_idx].attr = ret_old_nodes[j][4].attr
+                    else:
+                        attr['append_op'] = 'binary_add'
                     tb_node_idx = model.get_node_id(new_node_names[j][0])
                     model.nodes[tb_node_idx].attr = attr
 
         pattern_dict = pattern_mapping_config['TransposeBatchMatMul'][-1]
         model, new_node_names, ret_old_nodes = util.pattern_mapping("TransposeBatchMatMul",
                                                                     pattern_dict, model)
         if len(new_node_names) != 0:
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/word_embeddings.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/word_embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The WordEmbeddings pattern."""
+
 from .pattern import Pattern, pattern_registry
 from collections import namedtuple, OrderedDict
 from .. import graph_utils as util
 
 
 @pattern_registry(pattern_type='WordEmbeddings')
 class WordEmbeddings(Pattern):
-    def __call__(self, model):
+    """The WordEmbeddings pattern.
 
+    Fuse the original sub-graph into the custom acceleration 'WordEmbeddings' graph.
+    The fusion strategy is based on 'AddClsToken' pattern map configurations and different kinds of models.
+    """
+    def __call__(self, model):
+        """The __call__ function of this pattern class."""
         pattern_mapping_config = {
             'WordEmbeddings': [
                 {
                     'patterns': {
                         'in': [[(0, 'ExpandDims'), (3, 'Shape'), (4, 'StridedSlice'), (6, 'Pack'),
                                 (7, 'Reshape')], [(3, 'Shape'), (5, 'StridedSlice'), (6, 'Pack')],
                                [(0, 'ExpandDims'), (1, 'Reshape'), (2, 'Gather'), (7, 'Reshape')]],
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/backends/neural_engine/compile/tf_utils.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/backends/neural_engine/compile/tf_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""The neural engine tensorflow utils."""
 
 import numpy as np
 import re
 from collections import namedtuple, OrderedDict
 from . import logger
 from .ops.tensor import Tensor
 from . import graph_utils as util
 
 
 def create_tf_node(op, name, inputs):
-    """Create a nodedef object
+    """Create a nodedef object.
+
     Args:
         op (string): op type
         name (string): op name
         inputs (string list): op's inputs name
+
     Returns:
         nodedef: the created nodedef object
     """
     from tensorflow.core.framework import node_def_pb2
 
     new_node = node_def_pb2.NodeDef()
     new_node.op = op
@@ -41,20 +44,22 @@
     for input_name in inputs:
         new_node.input.extend([input_name])
     return new_node
 
 
 def graph_node_names_details(nodes):
     """Parse the graph nodes ans get the graph_nodes_dict.
+
     Be used for Grpah class with cerating a new graph.
     The node_name is the key, node in value is for getting the Const
     tensor value and the input_tensor source op; outputs in value is for
     output_tensor dest op.
     Args:
         nodes (tendorflow graph_def.node): NodeDef list
+
     Returns:
         node_names_details: the graph node info dict
 
     """
     # nodes = model.graph_def.node
     # some node may have several output edges
     # use tensor represents edge in graph
@@ -75,35 +80,38 @@
                 inputs.append(each_input)
         for each_i in inputs:
             node_names_details[each_i].outputs.append(name)
     return node_names_details
 
 
 def get_tensor_dest_op(node_name, tensor_name, nodes_dict):
-    """get the tensor dest op name
-       Args:
+    """Get the tensor dest op name.
+
+    Args:
         node_name: string, the source node name of tensor
         tensor_name: string, with ':0' or something like it
         nodes_dict: dict returned by the graph_node_names_details function
-       Returns:
+
+    Returns:
         dest_op_names: list, store the tensor's dest op names
     """
     dest_op_names = []
     post_node_names = nodes_dict[node_name].outputs
     for n_name in post_node_names:
         for input_name in nodes_dict[n_name].node.input:
             if util.names_from_input(input_name)[1] == tensor_name:
                 dest_op_names.append(n_name)
             else:
                 continue
     return dest_op_names
 
 
 def tf_extract_operator(node, model, nodes_dict):
-    """decorate the operator in tensorflow
+    """Decorate the operator in tensorflow.
+
     Args:
         node: NodeDef
         model: TensorflowModel
         nodes_dict: dict, return value from graph_node_names_details
         tf_dtypes: dict, for get the dtype string
 
     Returns:
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/benchmark.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Benchmark: provide the inference functions for PyTorchBenchmark and ExecutorBenchmark."""
+
 import os
 from transformers import PyTorchBenchmark
 from transformers.benchmark.benchmark import *
 from transformers.benchmark.benchmark_utils import *
 from .model import OptimizedModel
 
 
 def _prepare_inference_func(self, model_name: str, batch_size: int, sequence_length: int) -> Callable[[], None]:
+    """Prepare the inference function."""
     config = self.config_dict[model_name]
 
     if self.args.torchscript:
         config.torchscript = True
 
     logger.warning("Function transformers.PyTorchBenchmark._prepare_inference_func is replaced "
                     "by intel_extension_for_transformers.optimization.benchmark to support int8 models.")
@@ -86,14 +89,15 @@
     return _forward
 
 PyTorchBenchmark._prepare_inference_func = _prepare_inference_func
 
 
 origin_func = PyTorchBenchmark.run
 def run(self):
+    """Print the table headers and run the Pytorch benchmark."""
     output = origin_func(self)
     self.print_fn("\n" + 20 * "=" + ("INFERENCE - MODEL SIZE - RESULT").center(40) + 20 * "=")
     self.print_fn(80 * "-")
     self.print_fn("Model Name".center(60) + "Model Size in MB".center(15))
     self.print_fn(80 * "-")
     for model_name in self.args.model_names:
         self.print_fn(model_name[:50].center(60), 
@@ -104,15 +108,15 @@
 PyTorchBenchmark.run = run
 
 
 ExecutorBenchmarkArguments = PyTorchBenchmarkArguments
 
 
 class ExecutorBenchmark(PyTorchBenchmark):
-
+    """ExecutorBenchmark: overwrite the _prepare_inference_func in PyTorchBenchmark to support executor."""
     args: ExecutorBenchmarkArguments
     configs: PretrainedConfig
     framework: str = "Executor"
 
     def _prepare_inference_func(self, model_name: str, batch_size: int, sequence_length: int) -> Callable[[], None]:
         config = self.config_dict[model_name]
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/config.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Config: provide config classes for optimization processes."""
+
 from enum import Enum
 from neural_compressor.conf.config import (
     Distillation_Conf, Pruner, Pruning_Conf, Quantization_Conf
 )
 from neural_compressor.conf.dotdict import DotDict
 from intel_extension_for_transformers.optimization.utils.metrics import Metric
 from intel_extension_for_transformers.optimization.utils.objectives import Objective, performance
@@ -26,30 +28,29 @@
 from intel_extension_for_transformers.optimization.distillation import (
     Criterion, DistillationCriterionMode, SUPPORTED_DISTILLATION_CRITERION_MODE
 )
 from intel_extension_for_transformers.optimization.utils.utility import LazyImport
 from typing import List, Union
 from xmlrpc.client import boolean
 
-nncf = LazyImport("nncf")
-
 
 WEIGHTS_NAME = "pytorch_model.bin"
 
 
 class Provider(Enum):
+    """Optimization functionalities provider: INC or NNCF."""
     INC = "inc"
-    NNCF = "nncf"
 
 
 class DynamicLengthConfig(object):
+    """Configure the dynamic length config for Quantized Length Adaptive Transformer."""
     def __init__(
         self,
         max_length: int = None,
-        length_config: bool = None,
+        length_config: str = None,
         const_rate: float = None,
         num_sandwich: int = 2,
         length_drop_ratio_bound: float = 0.2,
         layer_dropout_prob: float = None,
         layer_dropout_bound: int = 0,
         dynamic_training: bool = False,
         load_store_file: str = None,
@@ -59,14 +60,36 @@
         mutation_prob: float = 0.5,
         crossover_size: int = 30,
         num_cpus: int = 48,
         distributed_world_size: int = 5,
         latency_constraint: bool = True,
         evo_eval_metric = 'eval_f1'
     ):
+        """Init a DynamicLengthConfig object.
+
+        Args:
+            max_length: Limit the maximum length of each layer
+            length_config: The length number for each layer
+            const_rate: Length drop ratio
+            num_sandwich: Sandwich num used in training
+            length_drop_ratio_bound: Length dropout ratio list
+            layer_dropout_prob: The layer dropout with probability
+            layer_dropout_bound: Length dropout ratio
+            dynamic_training: Whether to use dynamic training
+            load_store_file: The path for store file
+            evo_iter: Iterations for evolution search
+            population_size: Population limitation for evolution search
+            mutation_size: Mutation limitation for evolution search
+            mutation_prob: Mutation probability used in evolution search
+            crossover_size: Crossover limitation for evolution search
+            num_cpus: The cpu nums used in evolution search
+            distributed_world_size: Distributed world size in evolution search training
+            latency_constraint: Latency constraint used in evolution search
+            evo_eval_metric: The metric name used in evolution search
+        """
         super().__init__()
 
         self.length_config = length_config
         self.const_rate = const_rate
         self.max_length = max_length
         self.num_sandwich = num_sandwich
         self.length_drop_ratio_bound = length_drop_ratio_bound
@@ -82,26 +105,40 @@
         self.num_cpus = num_cpus
         self.distributed_world_size = distributed_world_size
         self.latency_constraint = latency_constraint
         self.evo_eval_metric = evo_eval_metric
 
 
 class QuantizationConfig(object):
+    """Configure the quantization process."""
     def __init__(
         self,
         framework: str = "pytorch",
         approach: str = "PostTrainingStatic",
         timeout: int = 0,
         max_trials: int = 100,
         metrics: Union[Metric, List] = None,
         objectives: Union[Objective, List] = performance,
         config_file: str = None,
         sampling_size: int = 100,
-        use_bf16: bool = True,
+        use_bf16: bool = False,
     ):
+        """Init a QuantizationConfig object.
+
+        Args:
+            framework: Which framework you used
+            approach: Which quantization approach to use
+            timeout: Tuning timeout(seconds), 0 means early stop. Combined with max_trials field to decide when to exit
+            max_trials: Max tune times
+            metrics: Used to evaluate accuracy of tuning model, no need for NoTrainerOptimize
+            objectives: Objective with accuracy constraint guaranteed
+            config_file: Path to the config file
+            sampling_size: How many samples to use
+            use_bf16: Whether to use bf16
+        """
         super().__init__()
         if config_file is None:
             self.inc_config = Quantization_Conf()
         else:
             self.inc_config = Quantization_Conf(config_file)
         self.framework = framework
         if approach is not None:
@@ -120,48 +157,56 @@
             self._objectives = None
         if sampling_size is not None:
             self.sampling_size = sampling_size
         self.inc_config.usr_cfg.use_bf16 = use_bf16
 
     @property
     def approach(self):
+        """Get the quantization approach."""
         return self.inc_config.usr_cfg.quantization.approach
 
     @approach.setter
     def approach(self, approach):
+        """Set the quantization approach."""
         approach = approach.upper()
         assert approach in SUPPORTED_QUANT_MODE, \
             f"quantization approach: {approach} is not support!" + \
             "PostTrainingStatic, PostTrainingDynamic and QuantizationAwareTraining are supported!"
         self.inc_config.usr_cfg.quantization.approach = QuantizationMode[approach].value
 
     @property
     def input_names(self):
+        """Get the input names."""
         return self.inc_config.usr_cfg.model.inputs
 
     @input_names.setter
     def input_names(self, input_names):
+        """Set the input names."""
         assert isinstance(input_names, list), "input_names must be a list"
         self.inc_config.usr_cfg.model.inputs = input_names
 
     @property
     def output_names(self):
+        """Get the output names."""
         return self.inc_config.usr_cfg.model.outputs
 
     @output_names.setter
     def output_names(self, output_names):
+        """Set the output names."""
         assert isinstance(output_names, list), "output_names must be a list"
         self.inc_config.usr_cfg.model.outputs = output_names
 
     @property
     def metrics(self):
+        """Get the metrics."""
         return self._metrics
 
     @metrics.setter
     def metrics(self, metrics: Union[Metric, List]):
+        """Set the metrics."""
         self._metrics = metrics
         rel_or_abs = {True: "relative", False: "absolute"}
         assert isinstance(metrics[0] if isinstance(metrics, list) else metrics, Metric), \
             "metric should be a Metric calss!"
         if isinstance(metrics, Metric) or len(metrics) == 1:
             self.inc_config.usr_cfg.tuning.accuracy_criterion = {
                 rel_or_abs[metrics[0].is_relative]
@@ -187,28 +232,32 @@
             self.inc_config.usr_cfg.tuning.accuracy_criterion = {
                 rel_or_abs[metrics[0].is_relative]: metrics[0].criterion,
                 "higher_is_better": metrics[0].greater_is_better
             }
 
     @property
     def framework(self):
+        """Get the framework."""
         return self.inc_config.usr_cfg.model.framework
 
     @framework.setter
     def framework(self, framework):
+        """Set the framework."""
         assert framework in ["pytorch", "pytorch_fx", "pytorch_ipex", "tensorflow"], \
             "framework: {} is not support!".format(framework)
         self.inc_config.usr_cfg.model.framework = framework
 
     @property
     def objectives(self):
+        """Get the objectives."""
         return self._objectives
 
     @objectives.setter
     def objectives(self, objectives: Union[List, Objective]):
+        """Set the objectives."""
         self._objectives = objectives
         if isinstance(objectives, Objective) or len(objectives) == 1:
             self.inc_config.usr_cfg.tuning.objective = objectives.name \
                 if isinstance(objectives, Objective) else objectives[0].name
         else:
             weights = [objective.weight_ratio for objective in objectives]
             if not any(weights):
@@ -222,119 +271,153 @@
                 "objective": [objective.name for objective in objectives],
                 "higher_is_better": [objective.greater_is_better for objective in objectives],
                 "weight": [objective.weight_ratio for objective in objectives],
             }
 
     @property
     def strategy(self):
+        """Get the strategy."""
         return self.inc_config.usr_cfg.tuning.strategy.name
 
     @strategy.setter
     def strategy(self, strategy):
+        """Set the strategy."""
         assert strategy in ["basic", "bayesian", "mse"], \
             "strategy: {} is not support!".format(strategy)
         self.inc_config.usr_cfg.tuning.strategy.name = strategy
 
     @property
     def timeout(self):
+        """Get the timeout."""
         return self.inc_config.usr_cfg.tuning.exit_policy.timeout
 
     @timeout.setter
     def timeout(self, timeout):
+        """Set the timeout."""
         assert isinstance(timeout, int), "timeout should be integer!"
         self.inc_config.usr_cfg.tuning.exit_policy.timeout = timeout
 
     @property
     def op_wise(self):
+        """Get the op_wise dict."""
         return self.inc_config.usr_cfg.quantization.op_wise
 
     @op_wise.setter
     def op_wise(self, op_wise):
+        """Set the op_wise dict."""
         self.inc_config.usr_cfg.quantization.op_wise = op_wise
 
     @property
     def max_trials(self):
+        """Get the number of maximum trials."""
         return self.inc_config.usr_cfg.tuning.exit_policy.max_trials
 
     @max_trials.setter
     def max_trials(self, max_trials):
+        """Set the number of maximum trials."""
         assert isinstance(max_trials, int), "max_trials should be integer!"
         self.inc_config.usr_cfg.tuning.exit_policy.max_trials = max_trials
 
     @property
     def performance_only(self):
+        """Get the boolean whether to use performance only."""
         return self.inc_config.usr_cfg.tuning.exit_policy.performance_only
 
     @performance_only.setter
     def performance_only(self, performance_only):
+        """Set the boolean whether to use performance only."""
         assert isinstance(performance_only, boolean), "performance_only should be boolean!"
         self.inc_config.usr_cfg.tuning.exit_policy.performance_only = performance_only
 
     @property
     def random_seed(self):
+        """Get the random seed."""
         return self.inc_config.usr_cfg.tuning.random_seed
 
     @random_seed.setter
     def random_seed(self, random_seed):
+        """Set the random seed."""
         assert isinstance(random_seed, int), "random_seed should be integer!"
         self.inc_config.usr_cfg.tuning.random_seed = random_seed
 
     @property
     def tensorboard(self):
+        """Get the boolean whether to use tensorboard."""
         return self.inc_config.usr_cfg.tuning.tensorboard
 
     @tensorboard.setter
     def tensorboard(self, tensorboard):
+        """Set the boolean whether to use tensorboard."""
         assert isinstance(tensorboard, boolean), "tensorboard should be boolean!"
         self.inc_config.usr_cfg.tuning.tensorboard = tensorboard
 
     @property
     def output_dir(self):
+        """Get the output directory."""
         return self.inc_config.usr_cfg.tuning.workspace.path
 
     @output_dir.setter
     def output_dir(self, path):
+        """Set the output directory."""
         assert isinstance(path, str), "save_path should be a string of directory!"
         self.inc_config.usr_cfg.tuning.workspace.path = path
 
     @property
     def resume_path(self):
+        """Get the resume path."""
         return self.inc_config.usr_cfg.tuning.workspace.resume
 
     @resume_path.setter
     def resume_path(self, path):
+        """Set the resume path."""
         assert isinstance(path, str), "resume_path should be a string of directory!"
         self.inc_config.usr_cfg.tuning.workspace.resume = path
 
     @property
     def sampling_size(self):
+        """Get the sampling size."""
         return self.inc_config.usr_cfg.quantization.calibration.sampling_size
 
     @sampling_size.setter
     def sampling_size(self, sampling_size):
+        """Set the sampling size."""
         if isinstance(sampling_size, int):
             self.inc_config.usr_cfg.quantization.calibration.sampling_size = [sampling_size]
         elif isinstance(sampling_size, list):
             self.inc_config.usr_cfg.quantization.calibration.sampling_size = sampling_size
         else:
             assert False, "The sampling_size must be a list of int numbers"
 
 
 class PruningConfig(object):
+    """Configure the pruning process."""
     def __init__(
         self,
         framework: str = "pytorch",
         epochs: int = 1,
         epoch_range: List = [0, 4],
         initial_sparsity_ratio: float=0.0,
         target_sparsity_ratio: float = 0.97,
         metrics: Metric = None,
         pruner_config: Union[List, Pruner] = None,
         config_file: str = None
     ):
+        """Init a PruningConfig object.
+
+        Args:
+            framework: Which framework you used
+            epochs: How many epochs to prune
+            epoch_range: Epoch range list
+            initial_sparsity_ratio: Initial sparsity goal, and not needed if pruner_config argument is defined
+            target_sparsity_ratio: Target sparsity goal, and not needed if pruner_config argument is defined
+            metrics: Used to evaluate accuracy of tuning model, not needed for NoTrainerOptimizer
+            pruner_config: Defined pruning behavior, if it is None, then NLP wil create a default pruner with
+                'BasicMagnitude' pruning typel
+            config_file: Path to the config file
+        """
         super().__init__()
         self.inc_config = Pruning_Conf(config_file)
         self.framework = framework
 
         if initial_sparsity_ratio is not None:
             self.initial_sparsity_ratio = initial_sparsity_ratio
         if target_sparsity_ratio is not None:
@@ -349,122 +432,151 @@
             self.pruner_config = pruner_config
         else:
             self.init_prune_config()
         self.epochs = epochs
 
 
     def init_prune_config(self):
+        """Init the pruning config."""
         pruner_config = Pruner()
         self.inc_config.usr_cfg.pruning.approach.weight_compression['pruners'] = [pruner_config]
 
     @property
     def pruner_config(self):
+        """Get the pruner config."""
         return self.inc_config.usr_cfg.pruning.approach.weight_compression.pruners
 
     @pruner_config.setter
     def pruner_config(self, pruner_config):
+        """Set the pruner config."""
         if isinstance(pruner_config, list):
             self.inc_config.usr_cfg.pruning.approach.weight_compression.pruners = pruner_config
         else:
             self.inc_config.usr_cfg.pruning.approach.weight_compression.pruners = [pruner_config]
 
     @property
     def target_sparsity_ratio(self):
+        """Get the target sparsity ratio."""
         return self.inc_config.usr_cfg.pruning.approach.weight_compression.target_sparsity
 
     @target_sparsity_ratio.setter
     def target_sparsity_ratio(self, target_sparsity_ratio):
+        """Set the target sparsity ratio."""
         self.inc_config.usr_cfg.pruning.approach.weight_compression.target_sparsity = \
             target_sparsity_ratio
 
     @property
     def initial_sparsity_ratio(self):
+        """Get the initial sparsity ratio."""
         return self.inc_config.usr_cfg.pruning.approach.weight_compression.initial_sparsity
 
     @initial_sparsity_ratio.setter
     def initial_sparsity_ratio(self, initial_sparsity_ratio):
+        """Set the initial sparsity ratio."""
         self.inc_config.usr_cfg.pruning.approach.weight_compression.initial_sparsity = \
             initial_sparsity_ratio
 
     @property
     def epoch_range(self):
+        """Get the epoch range."""
         return [self.inc_config.usr_cfg.pruning.approach.weight_compression.start_epoch,
                 self.inc_config.usr_cfg.pruning.approach.weight_compression.end_epoch]
 
     @epoch_range.setter
     def epoch_range(self, epoch_range):
+        """Set the epoch range."""
         assert isinstance(epoch_range, list) and len(epoch_range) == 2, \
           "You should set epoch_range like [a,b] format to match the pruning start and end epoch."
         self.inc_config.usr_cfg.pruning.approach.weight_compression.start_epoch = epoch_range[0]
         self.inc_config.usr_cfg.pruning.approach.weight_compression.end_epoch = epoch_range[1]
 
     @property
     def epochs(self):
+        """Get the epochs."""
         eps = self.inc_config.usr_cfg.pruning.train.epoch \
             if hasattr(self.inc_config.usr_cfg.pruning, "train") else 1
         return eps
 
     @epochs.setter
     def epochs(self, epochs):
+        """Set the epochs."""
         assert isinstance(epochs, int) and epochs > 0, \
           "You should set epochs > 0 and int, not {}.".format(epochs)
         self.inc_config.usr_cfg.pruning["train"] = {"epoch": epochs}
 
     @property
     def framework(self):
+        """Get the framework."""
         return self.inc_config.usr_cfg.model.framework
 
     @framework.setter
     def framework(self, framework):
+        """Set the framework."""
         assert framework.lower() in ["pytorch", "pytorch_fx", "tensorflow"], \
             "framework: {} is not support!".format(framework)
         self.inc_config.usr_cfg.model.framework = framework.lower()
 
     @property
     def metrics(self):
+        """Get the metrics."""
         return self._metrics
 
     @metrics.setter
     def metrics(self, metrics: Metric):
+        """Set the metrics."""
         self._metrics = metrics
 
 
 class DistillationConfig(object):
+    """Configure the distillation process."""
     def __init__(
         self,
         framework: str = "pytorch",
         criterion: Criterion = None,
         metrics: Metric = None,
+        inc_config = None
     ):
+        """Init a DistillationConfig object.
+
+        Args:
+            framework: Which framework you used
+            criterion: Criterion of training, example: "KnowledgeLoss"
+            metrics: Metrics for distillation
+            inc_config: Distillation config
+        """
         super().__init__()
-        self.inc_config = Distillation_Conf()
+        self.inc_config = Distillation_Conf(inc_config)
         self.framework = framework
         if criterion is not None:
             self.criterion = criterion
         if metrics is not None:
             self.metrics = metrics
         else:
             self._metrics = None
 
     @property
     def framework(self):
+        """Get the framework."""
         return self.inc_config.usr_cfg.model.framework
 
     @framework.setter
     def framework(self, framework):
+        """Set the framework."""
         assert framework in ["pytorch", "pytorch_fx", "tensorflow"], \
             "framework: {} is not support!".format(framework)
         self.inc_config.usr_cfg.model.framework = framework
 
     @property
     def criterion(self):
+        """Get the criterion."""
         return self.inc_config.usr_cfg.distillation.train.criterion
 
     @criterion.setter
     def criterion(self, criterion: Criterion):
+        """Set the criterion."""
         assert criterion.name.upper() in SUPPORTED_DISTILLATION_CRITERION_MODE, \
             "The criterion name must be in ['KnowledgeLoss', 'IntermediateLayersLoss']"
         if criterion.name.upper() == DistillationCriterionMode.KNOWLEDGELOSS.name:
             assert criterion.temperature is not None, \
                 "Please pass the temperature to Criterion.temperature!"
             assert criterion.loss_types is not None, \
                 "Please pass the loss_types to Criterion.loss_types!"
@@ -494,54 +606,97 @@
                     "loss_weights": criterion.loss_weight_ratio,
                     "add_origin_loss": criterion.add_origin_loss
                 }
             }
 
     @property
     def metrics(self):
+        """Get the metrics."""
         return self._metrics
 
     @metrics.setter
     def metrics(self, metrics):
+        """Set the metrics."""
         assert isinstance(metrics, Metric), \
             "metric should be a Metric calss!"
         self._metrics = metrics
 
 
+class TFDistillationConfig(object):
+    """Configure the distillation process for Tensorflow."""
+    def __init__(
+        self,
+        loss_types: list = [],
+        loss_weights: list = [],
+        train_steps: list = [],
+        temperature: float = 1.0
+    ):
+        """Init a TFDistillationConfig object.
+
+        Args:
+            loss_types: Type of loss
+            loss_weights: Weight ratio of loss
+            train_steps: Steps of training
+            temperature: Parameter for KnowledgeDistillationLoss
+        """
+        super().__init__()
+        self.loss_types = loss_types
+        self.loss_weights = loss_weights
+        self.train_steps = train_steps
+        self.temperature = temperature
+
+
 class FlashDistillationConfig(object):
+    """The flash distillation configuration used by AutoDistillationConfig."""
     def __init__(
         self,
         block_names: list = [],
         layer_mappings_for_knowledge_transfer: list = [],
         loss_types: list = [],
         loss_weights: list = [],
         add_origin_loss: list = [],
         train_steps: list = [],
     ):
+        """Init a FlashDistillationConfig object."""
         super().__init__()
         self.block_names = block_names
         self.layer_mappings_for_knowledge_transfer = layer_mappings_for_knowledge_transfer
         self.loss_types = loss_types
         self.loss_weights = loss_weights
         self.add_origin_loss = add_origin_loss
         self.train_steps = train_steps
 
 
 class AutoDistillationConfig(object):
+    """Configure the auto disillation process."""
     def __init__(
         self,
         framework: str = "pytorch",
         search_space: dict = {},
         search_algorithm: str = "BO",
         metrics: Union[List, Metric] = None,
         max_trials: int = None,
         seed: int = None,
         knowledge_transfer: FlashDistillationConfig = None,
         regular_distillation: FlashDistillationConfig = None,
     ):
+        """Init a AutoDistillationConfig object.
+
+        Args:
+            framework: Which framework you used
+            search_space: Search space of NAS
+            search_algorithm: Search algorithm used in NAS, e.g. Bayesian Optimization
+            metrics: Metrics used to evaluate the performance of the model architecture candidate
+            max_trials: Maximum trials in NAS process
+            seed: Seed of random process
+            knowledge_transfer: Configuration controlling the behavior of knowledge transfer stage
+                in the autodistillation
+            regular_distillation: Configuration controlling the behavior of regular distillation stage
+                in the autodistillation
+        """
         super().__init__()
         self.config = DotDict({
             'model':{'name': 'AutoDistillation'},
             'auto_distillation':{
                 'search':{},
                 'flash_distillation':{
                     'knowledge_transfer':{},
@@ -562,140 +717,103 @@
         if regular_distillation is not None:
             self.regular_distillation = regular_distillation
         if metrics is not None:
             self._metrics = metrics
 
     @property
     def knowledge_transfer(self):
+        """Get the knowledge transfer."""
         return self.config.auto_distillation.flash_distillation.knowledge_transfer
 
     @knowledge_transfer.setter
     def knowledge_transfer(self, knowledge_transfer):
+        """Set the knowledge transfer."""
         if knowledge_transfer is None:
             knowledge_transfer = FlashDistillationConfig()
         for k, v in knowledge_transfer.__dict__.items():
             if v:
                 self.config.auto_distillation.flash_distillation.knowledge_transfer[k] = v
 
     @property
     def regular_distillation(self):
+        """Get the regular distillation."""
         return self.config.auto_distillation.flash_distillation.regular_distillation
 
     @regular_distillation.setter
     def regular_distillation(self, regular_distillation):
+        """Set the regular distillation."""
         if regular_distillation is None:
             regular_distillation = FlashDistillationConfig()
         for k, v in regular_distillation.__dict__.items():
             if v:
                 self.config.auto_distillation.flash_distillation.regular_distillation[k] = v
 
     @property
     def framework(self):
+        """Get the framework."""
         return self.config.model.framework
 
     @framework.setter
     def framework(self, framework):
+        """Set the framework."""
         assert framework in ["pytorch"], \
             "framework: {} is not support!".format(framework)
         self.config.model.framework = framework
 
     @property
     def search_space(self):
+        """Get the search space."""
         return self.config.auto_distillation.search.search_space
 
     @search_space.setter
     def search_space(self, search_space: dict):
+        """Set the search space."""
         self.config.auto_distillation.search.search_space = search_space
 
     @property
     def search_algorithm(self):
+        """Get the search algorithm."""
         return self.config.auto_distillation.search.search_algorithm
 
     @search_algorithm.setter
     def search_algorithm(self, search_algorithm: str):
+        """Set the search algorithm."""
         self.config.auto_distillation.search.search_algorithm = search_algorithm
 
     @property
     def max_trials(self):
+        """Get the max trials."""
         return self.config.auto_distillation.search.max_trials
 
     @max_trials.setter
     def max_trials(self, max_trials: int):
+        """Set the max trials."""
         self.config.auto_distillation.search.max_trials = max_trials
 
     @property
     def seed(self):
+        """Get the seed."""
         return self.config.auto_distillation.search.seed
 
     @seed.setter
     def seed(self, seed: int):
+        """Set the seed."""
         self.config.auto_distillation.search.seed = seed
 
     @property
     def metrics(self):
+        """Get the metrics."""
         return self._metrics
 
     @metrics.setter
     def metrics(self, metrics: Union[List, Metric]):
+        """Set the metrics."""
         self._metrics = metrics
         if isinstance(metrics, Metric):
             metrics = [metrics]
         self.config.auto_distillation.search.metrics = []
         self.config.auto_distillation.search.higher_is_better = []
         for metric in metrics:
             self.config.auto_distillation.search.metrics.append(metric.name)
             self.config.auto_distillation.search.higher_is_better.append(
                 metric.greater_is_better
                 )
-
-
-# pylint: disable=E0401
-class NncfConfig(object):   # pragma: no cover
-    def __init__(
-        self,
-        nncf_config,
-        distributed: bool = False,
-        to_onnx: bool = False,
-        metrics: Union[List, Metric] = None,
-    ):
-        super().__init__()
-        from nncf import NNCFConfig
-        assert isinstance(nncf_config, NNCFConfig)
-        self.nncf_config = nncf_config
-        if metrics is not None:
-            self._metrics = metrics
-        self._distributed = distributed
-        self._to_onnx = to_onnx
-
-
-    @property
-    def distributed(self):
-        return self._distributed
-
-    @distributed.setter
-    def distributed(self, distributed):
-        self._distributed = distributed
-
-    @property
-    def to_onnx(self):
-        return self._to_onnx
-
-    @to_onnx.setter
-    def to_onnx(self, to_onnx):
-        self._to_onnx = to_onnx
-
-    @property
-    def metrics(self):
-        return self._metrics
-
-    @metrics.setter
-    def metrics(self, metrics):
-        self._metrics = metrics
-
-    @property
-    def nncf_config(self):
-        return self._nncf_config
-
-    @nncf_config.setter
-    def nncf_config(self, nncf_config):
-        self._nncf_config = nncf_config
-
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/distillation.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/distillation.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/dynamic/drop_and_restore_utils.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/dynamic/drop_and_restore_utils.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/dynamic/evolution.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/dynamic/evolution.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/mixture/auto_distillation.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/mixture/auto_distillation.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from pickletools import optimize
 import numpy as np
 import os
 import random
 import shutil
+import tempfile
 
 from functools import partial
 from neural_compressor.conf.config import Conf, schema
 from neural_compressor.conf.dotdict import DotDict
 from neural_compressor.experimental import Distillation
 from neural_compressor.strategy.bayesian import BayesianOptimization
 from neural_compressor.utils import logger
@@ -43,65 +45,80 @@
         model_builder (function obj): A function to build model instance with the specified 
             model architecture parameters.
         conf_fname_or_obj (string or obj): The path to the YAML configuration file or
             a configuration object containing search setting, flash distillation settings, etc.
 
     """
 
-    def __init__(self, model_builder, conf_fname_or_obj):
+    def __init__(self, model_builder, conf_fname_or_obj, framework='pytorch'):
         self.search_space = {}
         self.model_builder = model_builder
         self._advisor = None
         self._train_func = None
         self._eval_func = None
         self.search_results = {}
         self.best_model_archs = None
         self.seed = None
+        self.framework = framework.lower()
         self.init_by_cfg(conf_fname_or_obj)
 
     def model_arch_proposition(self):
         """Propose architecture of the model based on search algorithm for next search iteration.
 
         Returns:
             Model architecture description.
         """
         model_arch_paras = self.advisor.suggestion()
         assert self.search_space_keys and isinstance(model_arch_paras, dict) and \
             self.search_space_keys == list(model_arch_paras.keys()), \
             "Keys of model_arch_paras should be the same with search_space_keys."
         return model_arch_paras
 
-    def search(self, res_save_path=None):
+    def search(self, res_save_path=None, model_cls=None):
         """AutoDistillation search process.
         
         Returns:
             Best model architecture found in search process.
         """
+        def reload_tf_model(model):
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                model.save_pretrained(tmp_dir)
+                assert model_cls, 'model_cls should not be None'
+                model = model_cls.from_pretrained(tmp_dir)
+            return model
+
         if res_save_path is None or not os.path.isdir(res_save_path):
             res_save_path = os.getcwd()
         save_path = os.path.join(res_save_path, 'AutoDistillationResults')
         self.model_paras_num = {}
+        logger.info(f'search save_path = {save_path}')
         self.load_search_results(save_path)
         os.makedirs(save_path, exist_ok=True)
 
         for i in range(self.max_trials):
             logger.info(
                 "{fix} Trial {n} starts, {r} trials to go {fix}".format(
                     n=i+1, r=self.max_trials-i-1, fix="="*30
                 )
             )
-            if not torch.distributed.is_initialized() or torch.distributed.get_rank() == 0:
+            if self.framework == 'pytorch':
+                if not torch.distributed.is_initialized() or torch.distributed.get_rank() == 0:
+                    model_arch_paras = self.model_arch_proposition()
+                    logger.info("Model architecture {} proposed.".format(model_arch_paras))
+                if torch.distributed.is_initialized():
+                    model_arch_paras_sync = [model_arch_paras] \
+                        if torch.distributed.get_rank() == 0 else [None]
+                    torch.distributed.broadcast_object_list(model_arch_paras_sync, src=0)
+                    model_arch_paras = model_arch_paras_sync[0]
+            else:
                 model_arch_paras = self.model_arch_proposition()
-                logger.info("Model architecture {} proposed.".format(model_arch_paras))
-            if torch.distributed.is_initialized():
-                model_arch_paras_sync = [model_arch_paras] \
-                    if torch.distributed.get_rank() == 0 else [None]
-                torch.distributed.broadcast_object_list(model_arch_paras_sync, src=0)
-                model_arch_paras = model_arch_paras_sync[0]
             model = self.model_builder(model_arch_paras)
+            if self.framework == 'tensorflow':
+                model = reload_tf_model(model)
+                
             model_paras = self.count_model_parameters(model)
             logger.info(
                 "***** Number of model parameters: {:.2f}M *****".format(model_paras / 10**6)
             )
             self.model_paras_num[tuple(model_arch_paras.values())] = model_paras
             if tuple(model_arch_paras.values()) in self.search_results:
                 logger.info("Skip evaluated model architecture {}.".format(model_arch_paras))
@@ -114,26 +131,31 @@
             else:
                 logger.info("Assessing model architecture: {}.".format(model_arch_paras))
                 metrics = self.estimate(model)
             logger.info(
                 "Metrics of model architecture {} is {}.".format(model_arch_paras, metrics)
             )
             self.search_results[tuple(model_arch_paras.values())] = metrics
-            if not torch.distributed.is_initialized() or torch.distributed.get_rank() == 0:
+            if (self.framework != "pytorch" or not torch.distributed.is_initialized() 
+              or torch.distributed.get_rank() == 0):
                 self.advisor.feedback(sum(self.metrics_conversion(metrics)))
+                print(f'res_save_path: {res_save_path}, save_path = {save_path}')
+                os.makedirs(save_path, exist_ok=True)
                 self.dump_search_results(
                     os.path.join(save_path, 'Trial_{}_results.txt'.format(i+1))
                 )
 
-        if not torch.distributed.is_initialized() or torch.distributed.get_rank() == 0:
+        if self.framework != "pytorch" or not torch.distributed.is_initialized() or torch.distributed.get_rank() == 0:
             for model_arch_vec in self.resumed_search_results:
                 if model_arch_vec not in self.search_results:
                     self.search_results[model_arch_vec] = \
                         self.resumed_search_results[model_arch_vec]
                     model = self.model_builder(self.params_vec2params_dict(model_arch_vec))
+                    if self.framework == 'tensorflow':
+                        model = reload_tf_model(model)
                     self.model_paras_num[model_arch_vec] = self.count_model_parameters(model)
             self.dump_search_results(os.path.join(save_path, 'Final_results.txt'.format(i+1)))
         self.find_best_model_archs()
         logger.info(
             "{fix} Found {n} best model architectures {fix}".format(
                 n=len(self.best_model_archs), fix="="*30
             )
@@ -150,28 +172,31 @@
         """
         assert self._train_func is not None and self._eval_func is not None, \
             "train_func and eval_func must be set."
         model = self._train_func(model)
         return self._eval_func(model)
 
     def count_model_parameters(self, model):
-        if isinstance(model, torch.nn.Module):
-            return sum(p.numel() for p in model.parameters())
-        else: # pragma: no cover
-            raise NotImplementedError("Only support torch model now.")
+        if self.framework == 'pytorch':
+            if isinstance(model, torch.nn.Module):
+                return sum(p.numel() for p in model.parameters())
+            else: # pragma: no cover
+                raise NotImplementedError("Only support torch model now.")
+        elif self.framework == 'tensorflow':
+            return model.num_parameters()
 
     def load_search_results(self, path):
         self.resumed_search_results = {}
         lastest_results_record = os.path.join(path, 'lastest_results.npy')
         if not os.path.exists(path) or not os.path.exists(lastest_results_record):
             return
         self.resumed_search_results = np.load(lastest_results_record, allow_pickle=True).item()
-        if torch.distributed.is_initialized():
+        if self.framework == "pytorch" and torch.distributed.is_initialized():
             torch.distributed.barrier()
-        if not torch.distributed.is_initialized() or torch.distributed.get_rank() == 0:
+        if self.framework != "pytorch" or not torch.distributed.is_initialized() or torch.distributed.get_rank() == 0:
             os.makedirs(os.path.join(path, 'previous_results'), exist_ok=True)
             for f in os.listdir(path):
                 if os.path.isfile(os.path.join(path, f)):
                     shutil.move(os.path.join(path, f), os.path.join(path, 'previous_results', f))
         logger.info("Loaded previous results.")
 
     def dump_search_results(self, path):
@@ -233,15 +258,16 @@
                 self.config = Conf(conf_fname_or_obj).usr_cfg
             else:
                 raise FileNotFoundError(
                     "{} is not a file, please provide a file path.".format(conf_fname_or_obj)
                 )
         elif isinstance(conf_fname_or_obj, AutoDistillationConfig):
             self.config = conf_fname_or_obj.config
-            schema.validate(self.config)
+            if self.framework == 'pytorch':
+                schema.validate(self.config)
         else: # pragma: no cover
             raise NotImplementedError(
                 "Please provide a str path to config file or a config dict."
             )
         assert self.config.auto_distillation is not None, "auto_distillation section must be set"
         auto_distillation_cfg = self.config.auto_distillation
         # search related
@@ -275,14 +301,34 @@
             self.advisor = BayesianOptimizationSearcher(self.search_space, self.seed)
         else: # pragma: no cover
             raise NotImplementedError(
                 'Unsupported \'{}\' search algorithm'.format(self.search_algorithm)
             )
 
     def create_distillers(self):
+        def create_tf_distiller(distillation_cfg):
+            block_names = distillation_cfg.block_names \
+                if distillation_cfg.block_names else ['']
+            train_steps = distillation_cfg.train_steps \
+                if distillation_cfg.train_steps else [500]
+            conf = DotDict({
+                'model':{
+                    'name': 'flash_distillation_{}'.format(0), 'framework': self.framework
+                },
+                'distillation':{
+                    'train':{'optimizer': {'SGD':{'learning_rate': 1e-4}},
+                            'criterion': {'KnowledgeDistillationLoss':
+                                        {'temperature': distillation_cfg.temperature,
+                                        'loss_types': distillation_cfg.loss_types,
+                                        'loss_weights': distillation_cfg.loss_weights,
+                                        }}}
+                }
+            })
+            return [Distillation(conf)], block_names, train_steps
+
         def create_distiller(distillation_cfg):
             distillers = []
             assert distillation_cfg.layer_mappings_for_knowledge_transfer, \
                 'layer_mappings_for_knowledge_transfer should be defined in flash_distillation'
             layer_mappings = \
                 distillation_cfg.layer_mappings_for_knowledge_transfer
             block_names = distillation_cfg.block_names \
@@ -292,50 +338,60 @@
             loss_weights = distillation_cfg.loss_weights \
                 if distillation_cfg.loss_weights else [[1.0 / len(_)] * len(_) \
                     for _ in layer_mappings]
             add_origin_loss = distillation_cfg.add_origin_loss \
                 if distillation_cfg.add_origin_loss else [False] * len(layer_mappings)
             train_steps = distillation_cfg.train_steps \
                 if distillation_cfg.train_steps else [500] * len(layer_mappings)
+            temperatures = distillation_cfg.temperatures \
+                if distillation_cfg.temperatures else [1.0] * len(layer_mappings)
             assert len(layer_mappings) == len(block_names) == len(loss_types) == \
                 len(loss_weights) == len(add_origin_loss) == len(train_steps), \
                 "lengths of layer_mappings_for_knowledge_transfer, block_names, " + \
                 "loss_types, loss_weights, add_origin_loss and train_steps should be the same."
             distillers = []
             for i, lm in enumerate(layer_mappings):
                 conf = DotDict({
                     'model':{
-                        'name': 'flash_distillation_{}'.format(i), 'framework': 'pytorch'
+                        'name': 'flash_distillation_{}'.format(i), 'framework': self.framework
                     },
                     'distillation':{
                         'train':{'optimizer': {'SGD':{'learning_rate': 1e-4}},
-                                 'criterion': {'IntermediateLayersKnowledgeDistillationLoss':
-                                               {'layer_mappings': lm,
+                                'criterion': {'IntermediateLayersKnowledgeDistillationLoss':
+                                            {'layer_mappings': lm,
                                                 'loss_types': loss_types[i],
                                                 'loss_weights': loss_weights[i],
                                                 'add_origin_loss': add_origin_loss[i]}}}
-                    }        
+                    }
                 })
                 distillers.append(Distillation(conf))
             return distillers, block_names, train_steps
 
         flash_distillation_config = self.flash_distillation_config
         # knowledge transfer related
         self.flash_distillers = []
         if flash_distillation_config.knowledge_transfer:
             knowledge_transfer_cfg = flash_distillation_config.knowledge_transfer
-            self.flash_distillers, self.flash_block_names, self.flash_train_steps = \
-                create_distiller(knowledge_transfer_cfg)
+            if self.framework == 'pytorch':
+                self.flash_distillers, self.flash_block_names, self.flash_train_steps = \
+                    create_distiller(knowledge_transfer_cfg)
+            else:
+                self.flash_distillers, self.flash_block_names, self.flash_train_steps = \
+                    create_tf_distiller(knowledge_transfer_cfg)
 
         # regular distillation related
         self.regular_distillers = []
         if flash_distillation_config.regular_distillation:
             regular_distillation_cfg = flash_distillation_config.regular_distillation
-            self.regular_distillers, self.regular_block_names, self.regular_train_steps = \
-                create_distiller(regular_distillation_cfg)
+            if self.framework == 'pytorch':
+                self.regular_distillers, self.regular_block_names, self.regular_train_steps = \
+                    create_distiller(regular_distillation_cfg)
+            else:
+                self.regular_distillers, self.regular_block_names, self.regular_train_steps = \
+                    create_tf_distiller(regular_distillation_cfg)
 
     @property
     def teacher_model(self):
         return self._teacher_model
 
     @teacher_model.setter
     def teacher_model(self, user_model):
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/model.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,36 +11,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""OptimizedModel: provides the from_pretrained function."""
+
 import copy
 import os
 import transformers
 from .config import WEIGHTS_NAME
 from neural_compressor.utils import logger
 from intel_extension_for_transformers.optimization.utils.utility import LazyImport
 from packaging.version import Version
 from transformers import AutoConfig
 
 torch = LazyImport("torch")
 
 
 class OptimizedModel:
+    """Provide the from_pretrained function."""
     def __init__(self, *args, **kwargs):  # pragma: no cover
+        """Only use from_pretrained to instantiate a model."""
         raise EnvironmentError(
             f"{self.__class__.__name__} is designed to be instantiated using the"
             f"`{self.__class__.__name__}.from_pretrained(model_name_or_path)` method.")
 
     @classmethod
     def from_pretrained(cls, model_name_or_path: str, **kwargs):
-        """
-        Instantiate a quantized pytorch model from a given Intel Neural Compressor (INC) configuration file.
+        """Instantiate a quantized pytorch model from a given Intel Neural Compressor (INC) configuration file.
+
         Args:
             model_name_or_path (:obj:`str`):
                 Repository name in the Hugging Face Hub or path to a local directory hosting the model.
             cache_dir (:obj:`str`, `optional`):
                 Path to a directory in which a downloaded configuration should be cached if the standard cache should
                 not be used.
             force_download (:obj:`bool`, `optional`, defaults to :obj:`False`):
@@ -49,14 +53,15 @@
             resume_download (:obj:`bool`, `optional`, defaults to :obj:`False`):
                 Whether or not to delete incompletely received file. Attempts to resume the download if such a file
                 exists.
             revision(:obj:`str`, `optional`):
                 The specific model version to use. It can be a branch name, a tag name, or a commit id, since we use a
                 git-based system for storing models and other artifacts on huggingface.co, so ``revision`` can be any
                 identifier allowed by git.
+
         Returns:
             q_model: Quantized model.
         """
         from neural_compressor.utils.pytorch import load
         from neural_compressor import __version__
         config = kwargs.pop("config", None)
         cache_dir = kwargs.pop("cache_dir", None)
@@ -73,14 +78,21 @@
                 resume_download=resume_download,
                 use_auth_token=use_auth_token,
                 revision=revision,
                 **kwargs,
             )
 
         model_class = eval(f'transformers.{config.architectures[0]}')
+        if os.path.exists(os.path.join(model_name_or_path, "best_model.pt")):
+            import intel_extension_for_pytorch    # pylint: disable=E0401
+            logger.info("the INC IPEX quantization optimized model is loading.")
+            weight_file = os.path.join(model_name_or_path, "best_model.pt")
+            q_model = torch.jit.load(weight_file)
+            q_model = torch.jit.freeze(q_model.eval())
+            return q_model
         if config.torch_dtype is not torch.int8:
             model = model_class.from_pretrained(
                 model_name_or_path,
                 cache_dir=cache_dir,
                 force_download=force_download,
                 resume_download=resume_download,
                 use_auth_token=use_auth_token,
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/optimizer.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/optimizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Optimization: provides the orchestrate optimizer for Pytorch."""
+
 import logging
 import os
 
 from neural_compressor.experimental import(
     common,
     Component,
     Distillation,
@@ -28,45 +30,40 @@
     DistillationConfig,
     Provider,
     QuantizationConfig,
     PruningConfig
 )
 from intel_extension_for_transformers.optimization.utils.utility import LazyImport
 from intel_extension_for_transformers.optimization.quantization import QuantizationMode
-from transformers import PreTrainedModel
+from transformers import PreTrainedModel, PretrainedConfig
 from transformers.file_utils import WEIGHTS_NAME
 from typing import Callable, Optional, Union, List
 
 torch = LazyImport("torch")
 
 logger = logging.getLogger(__name__)
 
 
 class Orchestrate_optimizer:
+    """Orchestrate_optimizer aggregates and orchestrates components such as Quantization, Pruning and Distillation."""
     def __init__(
         self,
         model,
         components: Optional[List[Component]] = [],
         eval_func: Optional[Callable] = None,
         train_func: Optional[Callable] = None,
     ):
-        """
+        """Init an orchestrate optimizer.
+
         Args:
-            model (:obj:`Union[PreTrainedModel, torch.nn.Module]`):
-                Model to quantize and/or prune.
-            components (List[:obj:`Component`], `optional`):
-                List of Component objects which contains Quantization, 
-                Pruning, Distillation objects.
-            eval_func (:obj:`Callable`, `optional`):
-                Evaluation function to evaluate the tuning objective.
-            train_func (:obj:`Callable`, `optional`):
-                Training function which will be combined with pruning.
+            model: Model to quantize and/or prune.
+            components: List of Component objects which contains Quantization, Pruning, Distillation objects.
+            eval_func: Evaluation function to evaluate the tuning objective.
+            train_func: Training function which will be combined with pruning.
         """
-
-
         if len(components) == 0:
             raise RuntimeError("`NLPOptimizer` requires at least one `Quantization`, "
                                "`Pruning` or `Distillation` object")
 
         self.scheduler = Scheduler()
         self.scheduler.model = common.Model(model)
 
@@ -79,85 +76,100 @@
                     agent.criterion = component.criterion
             print(agent)
             self.scheduler.append(agent)
         else:
             self.scheduler.append(*components)
 
     def fit(self):
+        """Run the scheduler."""
         opt_model = self.scheduler()
         return opt_model
 
 
 
 class NoTrainerOptimizer:   # pragma: no cover
+    """Optimizer without using Trainer."""
     def __init__(
         self,
         model,
         output_dir: Optional[str] = "saved_results",
     ):
-        """
+        """Init a NoTrainerOptimizer object.
+
         Args:
-            model (:obj:`Union[PreTrainedModel, torch.nn.Module]`):
-                FP32 model specified for low precision tuning.
-            output_dir (:obj:`string`, `optional`):
-                The folder for saving the results.
+            model: FP32 model specified for low precision tuning.
+            output_dir: The folder for saving the results.
         """
-
         self.model = model
         self.teacher_model = None
         self._eval_func = None
         self._train_func = None
+        self._calib_func = None
         self._calib_dataloader = None
         self.output_dir = output_dir
         self.quant_config = None
         self.pruning_config = None
         self.distillation_config = None
         self._provider = Provider.INC.value
         self.pruner = None
         self.quantizer = None
         self.distiller = None
         self.in_training = False
 
     @property
     def eval_func(self):
+        """Get the evaluation function."""
         return self._eval_func
 
     @property
     def train_func(self):
+        """Get the train function."""
         return self._train_func
 
     @property
+    def calib_func(self):
+        """Get the calib function."""
+        return self._calib_func
+
+    @property
     def provider(self):
+        """Get the provider."""
         return self._provider
 
     @property
     def calib_dataloader(self):
+        """Get the calibration dataloader."""
         return self._calib_dataloader
 
     @eval_func.setter
     def eval_func(self, func: Callable):
+        """Set the evaluation function."""
         self._eval_func = func
 
     @train_func.setter
     def train_func(self, func: Callable):
+        """Set the train function."""
         self._train_func = func
 
     @provider.setter
     def provider(self, provider):
+        """Set the provider."""
         self._provider = provider
 
     @calib_dataloader.setter
     def calib_dataloader(self, dataloader):
+        """Set the calibration dataloader."""
         self._calib_dataloader = dataloader
 
     def init_quantizer(
         self,
         quant_config,
         provider: str = Provider.INC.value,
     ):
+        """Init a Quantization object with config."""
         from neural_compressor.experimental import Quantization
 
         assert isinstance(quant_config, QuantizationConfig), \
             "Please pass QuantizationConfig instance to trainer.quantize!"
         self.quant_config = quant_config
         self.metrics = self.quant_config.metrics
         self._provider = Provider[provider.upper()].value
@@ -171,51 +183,26 @@
 
         quantizer = Quantization(self.quant_config.inc_config)
         quantizer.model = common.Model(self.model)
 
         self.quantizer = quantizer
         return quantizer
 
-    # pylint: disable=E0401
-    def _nncf_quantize(self):   # pragma: no cover
-        from intel_extension_for_transformers import NncfConfig
-        from nncf import create_compressed_model
-        compression_state = None
-        assert isinstance(self.quant_config, NncfConfig), \
-            "Please pass a NNCFConfig instance to trainer.quantize!"
-        
-        self.metrics = self.quant_config.metrics
-        nncf_compression_state_file = self.quant_config.compression_state
-
-        if os.path.isfile(nncf_compression_state_file):
-            compression_state = torch.load(nncf_compression_state_file)
-        else:
-            compression_state = None
-
-        compression_algo_controller, model = create_compressed_model(
-            self.model, self.quant_config.nncf_config,
-            compression_state=compression_state
-        )
-
-        self.compression_ctrl = \
-            compression_algo_controller.distributed() \
-            if self.quant_config.distributed else compression_algo_controller
-
-        self.model = self._train_func(model)
-
     def _inc_quantize(
         self,
         quant_config,
         provider: str = Provider.INC.value,
     ):
+        """Do the quantization."""
         if self.quantizer is None:
             self.init_quantizer(quant_config=quant_config, provider=provider)
         if self._eval_func is not None:
             self.quantizer.eval_func = self._eval_func
-
+        if self._calib_func is not None:
+            self.quantizer.calib_func = self._calib_func
         if self.quant_config.approach == QuantizationMode.POSTTRAININGSTATIC.value:
             assert self._calib_dataloader is not None, \
                 "Please pass calib_dataloader to NoTrainerOptimizer.calib_dataloader"
             self.quantizer.calib_dataloader = self._calib_dataloader
         elif self.quant_config.approach == QuantizationMode.QUANTIZATIONAWARETRAINING.value:
             assert self._train_func is not None, \
                 "Please pass train_func to NoTrainerOptimizer.train_func"
@@ -230,38 +217,41 @@
 
     def quantize(
         self,
         quant_config: QuantizationConfig = None,
         provider: str = Provider.INC.value,
         eval_func: Optional[Callable] = None,
         train_func: Optional[Callable] = None,
+        calib_func: Optional[Callable] = None,
         calib_dataloader=None,
     ):
+        """Prepare for invoking the _inc_quantize function."""
         if eval_func is not None:
             self._eval_func = eval_func
         if train_func is not None:
             self._train_func = train_func
+        if calib_func is not None:
+            self._calib_func = calib_func
         if calib_dataloader is not None:
             self._calib_dataloader = calib_dataloader
 
         if self.quantizer is None:
             self._provider = Provider[provider.upper()].value
 
-        if self._provider == Provider.NNCF.value:
-            return self._nncf_quantize()
-        elif self._provider == Provider.INC.value:
+        if self._provider == Provider.INC.value:
             return self._inc_quantize(quant_config=quant_config, provider=provider)
         else:
             assert False, "Unsupport provider:{}".format(self._provider)
 
     def init_pruner(
         self,
         pruning_config = None,
         provider: str = Provider.INC.value,
     ):
+        """Init a Pruning object with config."""
         from neural_compressor.experimental import Pruning
         self.pruning_config = pruning_config
         self.metrics = self.pruning_config.metrics
         self._provider = Provider[provider.upper()].value
 
         assert isinstance(self.pruning_config, PruningConfig), \
             "please pass a instance of PruningConfig to trainer.prune!"
@@ -275,14 +265,15 @@
     def prune(
         self,
         pruning_config = None,
         provider: str = Provider.INC.value,
         eval_func: Optional[Callable] = None,
         train_func: Optional[Callable] = None,
     ):
+        """Do the pruning."""
         if self.pruner is None:
             self.init_pruner(pruning_config=pruning_config, provider=provider)
         if eval_func is not None:
             self._eval_func = eval_func
         if train_func is not None:
             self._train_func = train_func
 
@@ -296,14 +287,15 @@
 
     def init_distiller(
         self,
         distillation_config,
         teacher_model,
         provider: str = Provider.INC.value,
     ):
+        """Init a Distillation object with config and the teacher model."""
         from neural_compressor.experimental import Distillation, common
         assert isinstance(distillation_config, DistillationConfig), \
             "please pass a instance of PruningConfig to trainer.prune!"
         self.distillation_config = distillation_config
         self._provider = Provider[provider.upper()].value
         self.metrics = self.distillation_config.metrics
         self.teacher_model = teacher_model
@@ -319,14 +311,15 @@
         self,
         distillation_config,
         teacher_model,
         provider: str = Provider.INC.value,
         eval_func: Optional[Callable] = None,
         train_func: Optional[Callable] = None,
     ):
+        """Do the distillation."""
         if self.distiller is None:
             self.init_distiller(
                 distillation_config=distillation_config,
                 teacher_model=teacher_model,
                 provider=provider
             )
         if eval_func is not None:
@@ -339,16 +332,19 @@
         self.distiller.create_criterion()
 
         self.opt_model = self.distiller.fit()
 
         return self.opt_model
 
     def _save_inc_int8(self, opt_model, output_dir):
+        """Save the optimized model in the output directory."""
+        os.makedirs(output_dir, exist_ok=True)
         self.model.config.architectures = [self.model.__class__.__name__]
         self.model.config.torch_dtype = "int8"
-        self.model.config.save_pretrained(output_dir)
+        if isinstance(self.model.config, PretrainedConfig):
+            self.model.config.save_pretrained(output_dir)
         weights_file = os.path.join(os.path.abspath(
           os.path.expanduser(output_dir)), WEIGHTS_NAME)
         torch.save(opt_model.quantized_state_dict(), weights_file)
         logger.info(
             "quantized model and configure file have saved to {}".format(weights_file)
         )
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/optimizer_tf.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/optimizer_tf.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,55 +11,70 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""TFOptimization: provides the optimization class for Tensorflow."""
+
 import logging
+import pstats
 import numpy as np
 import os
 import time
 from neural_compressor import __version__
 from neural_compressor.experimental import common
 from neural_compressor.model.model import saved_model_session
 from neural_compressor.model.model import get_model_type
-from intel_extension_for_transformers import (DistillationConfig, QuantizationConfig, PruningConfig)
+from intel_extension_for_transformers import (DistillationConfig, QuantizationConfig, PruningConfig, AutoDistillation)
 from intel_extension_for_transformers.optimization.quantization import QuantizationMode
 from intel_extension_for_transformers.optimization.utils.metrics import Metric
 from intel_extension_for_transformers.optimization.utils.utility import LazyImport
 from packaging import version
 from transformers import PreTrainedModel
 from transformers.training_args_tf import TFTrainingArguments
 from typing import Callable, Optional, List
 from .utils.utility_tf import TFDataloader, TMPPATH, TEACHERPATH, get_filepath
 
+from functools import partial
+
 tf = LazyImport("tensorflow")
 logger = logging.getLogger(__name__)
 
 
 class TFOptimization:
+    """TFOptimization is the entry class for Tensorflow to use the optimization techniques in neural compressor."""
     def __init__(self,
                  model: PreTrainedModel,
                  args: TFTrainingArguments,
                  train_dataset=None,
                  eval_dataset=None,
                  compute_metrics: Optional[Callable] = None,
                  criterion=None,
                  optimizer=None,
                  task_type=None,
-                 task_id=None):
-        """
+                 task_id=None,
+                 strategy=None):
+        """Init a TFOptimziation object.
+
         Args:
-            model (:obj:`PreTrainedModel`):
-                FP32 model specified for low precision tuning.
-            output_dir (:obj:`string`, `optional`):
-                The folder for saving the results.
+            model: FP32 model specified for low precision tuning
+            args: Training arguments for TF
+            train_dataset: Training datas
+            eval_dataset: Evaluation data
+            compute_metrics: Metrics computing function during the evaluation process
+            criterion: Tuning criterion
+            optimizer: The optimizer you used
+            task_type: Used for distributed multi-node settings. Default set as "worker"
+            task_id: Used for distributed multi-node settings.
+                Set as 0 on the leader node and 1, 2, 3... on the followers
+            strategy: Equals to MultiWorkerMirroredStrategy if use distributed distributed multi-node settings,
+                otherwise None
         """
-
         self.model = model
         self.teacher_model = None
         self.component = None
         self.eval_dataset = eval_dataset
         self.train_dataset = train_dataset
         self._eval_func = None
         self._train_func = None
@@ -81,78 +96,92 @@
         self.criterion = criterion if criterion is not None else \
             self.model.loss if hasattr(self.model, "loss") else None
         self.model.save_pretrained(get_filepath(TMPPATH, self.task_type, self.task_id), saved_model=True)
         _, self.input_names, self.output_names = saved_model_session(
             os.path.join(get_filepath(TMPPATH, self.task_type, self.task_id), "saved_model/1"), input_tensor_names=[],
              output_tensor_names=[])
         self.eval_distributed = False
+        self.strategy = strategy
 
     @property
     def inputs(self):
+        """Get the inputs."""
         return self._inputs
 
     @inputs.setter
     def inputs(self, inputs: dict):
+        """Set the inputs."""
         self._inputs = inputs
 
     @property
     def input_names(self):
+        """Get the input names."""
         return self._input_names
 
     @input_names.setter
     def input_names(self, input_names: List):
+        """Set the input names."""
         self._input_names = input_names
 
     @property
     def output_names(self):
+        """Get the output names."""
         return self._output_names
 
     @output_names.setter
     def output_names(self, output_names: List):
+        """Set the output names."""
         self._output_names = output_names
 
     @property
     def eval_func(self):
+        """Get the evaluation function."""
         return self._eval_func
 
     @eval_func.setter
     def eval_func(self, func: Callable):
+        """Set the evaluation function."""
         self._eval_func = func
 
     @property
     def train_func(self):
+        """Get the training function."""
         return self._train_func
 
     @train_func.setter
     def train_func(self, func: Callable):
+        """Set the training function."""
         self._train_func = func
 
     @property
     def train_dataset(self):
+        """Get the training dataset."""
         return self._train_dataset
 
     @train_dataset.setter
     def train_dataset(self, train_dataset):
+        """Set the training dataset."""
         assert isinstance(train_dataset, tf.data.Dataset) or train_dataset is None, \
             "train_dataset should be obj of tf.data.Dataset"
         self._train_dataset = train_dataset
 
     @property
     def eval_dataset(self):
+        """Get the evaluation dataset."""
         return self._eval_dataset
 
     @eval_dataset.setter
     def eval_dataset(self, eval_dataset):
+        """Set the evaluation dataset."""
         assert isinstance(eval_dataset, tf.data.Dataset) or eval_dataset is None, \
             "eval_dataset should be obj of tf.data.Dataset"
         self._eval_dataset = eval_dataset
 
     def builtin_eval_func(self, model):
-        """
-        Custom Evaluate function to inference the model for specified metric on validation dataset.
+        """Customize Evaluate function to inference the model for specified metric on the validation dataset.
 
         Args:
             model ([tf.saved_model.load]): The model will be the class of tf.saved_model.load(quantized_model_path).
 
         Returns:
             [float]: evaluation result, the larger is better.
         """
@@ -311,14 +340,15 @@
             logger.info("Throughput: {} samples/sec".format(num_examples / total_time))
             return result
 
     def init_quantizer(
         self,
         quant_config,
     ):
+        """Init a Quantization object with config."""
         from neural_compressor.experimental import Quantization
 
         self.quant_config = QuantizationConfig() if quant_config is None else quant_config
         self.quant_config.framework = "tensorflow"
         self.metrics = self.quant_config.metrics
 
         quantizer = Quantization(self.quant_config.inc_config)
@@ -328,14 +358,15 @@
         self.quantizer = quantizer
         return quantizer
 
     def _inc_quantize(
         self,
         quant_config,
     ):
+        """Do the quantization."""
         if self.quantizer is None:
             self.init_quantizer(quant_config=quant_config)
         if self._eval_func is not None:
             self.quantizer.eval_func = self._eval_func
         else:
             assert self.metrics is not None, \
                 "Please pass the metrics to QuantizationConfig.metrics!"
@@ -367,14 +398,15 @@
         self,
         quant_config: QuantizationConfig = None,
         eval_func: Optional[Callable] = None,
         train_func: Optional[Callable] = None,
         train_dataset=None,
         eval_dataset=None,
     ):
+        """Prepare for invoking INC quantize function."""
         if eval_func is not None:
             self._eval_func = eval_func
         if train_func is not None:
             self._train_func = train_func
         if train_dataset is not None:
             self.train_dataset = train_dataset
 
@@ -383,14 +415,15 @@
 
         return self._inc_quantize(quant_config=quant_config)
 
     def init_pruner(
         self,
         pruning_config=None,
     ):
+        """Init a Pruning object with config."""
         from neural_compressor.experimental import Pruning
         if pruning_config.framework != 'tensorflow':
             logger.warning('pruning_config.framework is {}, should be tensorflow'.format(pruning_config.framework))
             pruning_config.framework = 'tensorflow'
         self.pruning_config = pruning_config
         self.metrics = self.pruning_config.metrics
 
@@ -409,14 +442,15 @@
         self,
         pruning_config=None,
         eval_func: Optional[Callable] = None,
         train_func: Optional[Callable] = None,
         train_dataset=None,
         eval_dataset=None,
     ):
+        """Do the pruning."""
         if self.pruner is None:
             self.init_pruner(pruning_config=pruning_config)
         if eval_func is not None:
             self.eval_func = eval_func
         if train_func is not None:
             self.train_func = train_func
 
@@ -452,15 +486,16 @@
         )
         return opt_model.model
 
     def init_distiller(
         self,
         distillation_config,
         teacher_model: PreTrainedModel,
-    ):  
+    ):
+        """Init a Distillation object with config and the teacher model."""
         from neural_compressor.experimental import Distillation
         assert isinstance(distillation_config, DistillationConfig), \
             "please pass a instance of DistillationConfig to trainer.distill!"
 
         def train_step(data):
             if len(data) == 3:
                 x, y, sample_weight = data  # pragma: no cover
@@ -483,16 +518,16 @@
                                           self.model.trainable_variables,
                                           tape=tape)
             return self.model.compute_metrics(x, y, y_pred, sample_weight)
 
         self.model.train_step = train_step
         # re-compile
         self.model.compile(
-            optimizer=self.model.optimizer, 
-            loss=self.model.loss, 
+            optimizer=self.model.optimizer,
+            loss=self.model.loss,
             metrics=self.model.compiled_metrics._user_metrics
             )
 
         if distillation_config.framework != 'tensorflow':
             logger.warning(
                 'distillation_config.framework is {}, should be tensorflow'.
                 format(distillation_config.framework))
@@ -514,15 +549,16 @@
 
     def distill(
         self,
         distillation_config,
         teacher_model: PreTrainedModel,
         eval_func: Optional[Callable] = None,
         train_func: Optional[Callable] = None,
-    ):  
+    ):
+        """Do the distillation."""
         if self.distiller is None:
             self.init_distiller(
                 distillation_config=distillation_config,
                 teacher_model=teacher_model,
             )
         if eval_func is not None:
             self._eval_func = eval_func
@@ -539,15 +575,170 @@
         opt_model.save(self.args.output_dir)
         logger.info(
             "distilled model have saved to {}".format(self.args.output_dir)
         )
 
         return opt_model.model
 
+    def model_builder_builtin(self, arch_paras=None, model_cls=None):
+        """Specify model_cls to use the built-in model builder."""
+        config = self.model.config
+        if arch_paras is not None:
+            assert isinstance(arch_paras, dict), "Expect arch_paras to be a dict."
+            for k in arch_paras:
+                if hasattr(config, k):
+                    config.__setattr__(k, arch_paras[k])
+                    # for MobileBERT, 'intra_bottleneck_size' is associated with
+                    # 'true_hidden_size', and must have the same values.
+                    if k == 'intra_bottleneck_size':
+                        config.__setattr__('true_hidden_size', arch_paras[k])
+        return model_cls.from_config(config)
+
+
+    def autodistill(
+        self,
+        autodistillation_config,
+        teacher_model: PreTrainedModel,
+        model_builder: Optional[Callable] = None,
+        model_cls: Optional[Callable] = None,
+        eval_func: Optional[Callable] = None,
+        train_func: Optional[Callable] = None
+        ):
+        """Do the auto distillation."""
+        self.autodistillation_config = autodistillation_config
+        if model_builder is None:
+            assert model_cls is not None, "Must specify model_cls to use the built-in " + \
+                "model_builder, e.g. model_cls=AutoModelForPreTraining, or you can use " + \
+                "the customized model_builder."
+            model_builder = partial(self.model_builder_builtin, model_cls=model_cls)
+        agent = AutoDistillation(model_builder, self.autodistillation_config, framework='tensorflow')
+
+        def train_func_builtin(model):
+            def run_distillers(
+                model,
+                distillers,
+                train_steps,
+                block_names,
+                presentation='flash distillation'
+            ):
+
+                for i, elements in enumerate(zip(distillers, train_steps, block_names)):
+                    distiller, ts, bln = elements
+                    logger.info(' '.join(
+                        ['=' * 30, 'Step {} of'.format(i + 1), presentation, '=' * 30]))
+
+                    def train_step(data):
+                        if len(data) == 3:
+                            x, y, sample_weight = data  # pragma: no cover
+                        else:
+                            sample_weight = None
+                            x, y = data
+                        with tf.GradientTape() as tape:
+                            y_pred = model(x)
+                            teacher_outputs = distiller.criterion.teacher_model_forward(
+                                input=x, teacher_model=teacher_model)
+
+                            loss = model.compute_loss(x, y, y_pred, sample_weight)
+                            # _on_after_compute_loss(self, input, student_output, student_loss, teacher_output=None)
+                            # TODO: check, combile
+                            loss = distiller.on_after_compute_loss(
+                                x, y_pred.logits, loss, teacher_outputs.logits)
+                        model._validate_target_and_loss(y, loss)
+                        # Run backwards pass.
+                        optimizer = self.model.optimizer
+                        optimizer.minimize(
+                            loss,
+                            model.trainable_variables,
+                            tape=tape)
+                        return model.compute_metrics(x, y, y_pred, sample_weight)
+
+                    model.save_pretrained(get_filepath(TMPPATH, self.task_type, self.task_id), saved_model=True)
+
+                    # re-build optimizer
+                    opt_kwargs = {}
+                    for k, v in self.model.optimizer.__dict__.items():
+                        if not k.startswith('_'):
+                            opt_kwargs[k] = v
+                    optimizer = self.model.optimizer.__class__(**opt_kwargs)
+                    if self.strategy:  # pragma: no cover
+                        with self.strategy.scope():
+                            model = model_cls.from_pretrained(get_filepath(TMPPATH, self.task_type, self.task_id))
+                            model.compile(
+                                    optimizer=optimizer,
+                                    loss=self.model.loss,
+                                    metrics=self.model.compiled_metrics._user_metrics
+                                    )
+                            model.train_step = train_step
+                    else:
+                        model.train_step = train_step
+                        model.compile(
+                            optimizer=optimizer,
+                            loss=self.model.loss,
+                            metrics=self.model.compiled_metrics._user_metrics)
+                    self.model = model
+
+                    distiller.model = os.path.join(TMPPATH, "saved_model/1")
+                    distiller.model.model_type = "saved_model"
+                    teacher_model.save_pretrained(TEACHERPATH, saved_model=True)
+                    distiller.teacher_model = os.path.join(TEACHERPATH, "saved_model/1")
+                    distiller.teacher_model.model_type = "saved_model"
+
+                    if eval_func is not None:
+                        self._eval_func = eval_func
+                    else:
+                        self._eval_func = self.builtin_eval_func
+                    if train_func is not None:
+                        self._train_func = train_func
+                    else:
+                        self._train_func = self.build_train_func
+
+                    distiller.eval_func = self._eval_func
+                    distiller.train_func = self._train_func
+                    distiller.create_criterion()
+
+                    self.component = self.distiller = distiller
+
+                    opt_model = distiller.fit()
+                    opt_model.save(self.args.output_dir)
+                    return opt_model
+
+            agent.create_distillers()
+            # run flash_distillers
+            ori_model = model
+            if agent.flash_distillers:
+                model = run_distillers(ori_model, agent.flash_distillers,
+                                       agent.flash_train_steps,
+                                       agent.flash_block_names)
+            # run regular_distillers
+            if agent.regular_distillers:
+                model = run_distillers(ori_model,
+                                       agent.regular_distillers,
+                                       agent.regular_train_steps,
+                                       agent.regular_block_names,
+                                       presentation='regular distillation')
+            return model.model
+
+        def eval_func_builtin(model):
+            if self._eval_func:
+                result = self._eval_func(model)
+            else:
+                result = self.builtin_eval_func(model)  # pragma: no cover
+            return {'metric': result}
+
+        agent.framework = 'tensorflow'
+        agent.train_func = train_func \
+            if train_func else train_func_builtin
+        agent.eval_func = eval_func \
+            if eval_func else eval_func_builtin
+        # pylint: disable=E1101
+        os.makedirs(self.args.output_dir, exist_ok=True)
+        return agent.search(self.args.output_dir, model_cls)
+
     def build_train_func(self, model):
+        """Build the training function for pruning or distillation."""
         tf.random.set_seed(1)
         epochs = 1
         if 'distillation' in self.component.cfg:
             epochs = max(epochs, self.component.cfg.distillation.train.get("epoch", 1))
             hooks = self.component.hooks
         if 'pruning' in self.component.cfg:
             epochs = max(epochs, self.component.cfg.pruning.train.get("epoch", 1))
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/pipeline.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Pipeline: import transformers.pipelines and support int8 model loading based on infer_framework_load_model."""
+
 import importlib
 from transformers import AutoConfig, pipeline
 from transformers.pipelines import *
 from typing import Dict, Optional, Tuple
 from .model import OptimizedModel
 
 
@@ -30,16 +32,15 @@
     model,
     config: AutoConfig,
     model_classes: Optional[Dict[str, Tuple[type]]] = None,
     task: Optional[str] = None,
     framework: Optional[str] = None,
     **model_kwargs
 ):
-    """
-    Support int8 model loading based on infer_framework_load_model
+    """Support int8 model loading based on infer_framework_load_model.
 
     Returns:
         `Tuple`: A tuple framework, model.
     """
     logger.warning("Function transformers.pipelines.base.infer_framework_load_model is replaced "
                     "by intel_extension_for_transformers.optimization.pipeline.")
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/pruning.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/pruning.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,34 +11,51 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Pruning: specify the supported pruning mode."""
+
 from enum import Enum
 from neural_compressor.conf.config import Pruner as INCPruner
 from neural_compressor.pruners import PRUNERS
 from typing import Dict, List
 
 
 class PruningMode(Enum):
+    """Currently support three pruning modes."""
     BASICMAGNITUDE = "basic_magnitude"
     PATTERNLOCK = "pattern_lock"
     GROUPLASSO = "group_lasso"
 
 
 SUPPORTED_PRUNING_MODE = set([approach.name for approach in PruningMode])
 
 
 class PrunerConfig(INCPruner):
+    """Pruner configuration."""
     def __init__(self, epoch_range: List=[0, 4], initial_sparsity_ratio: float=0.0,
                  target_sparsity_ratio: float=0.97, update_frequency: int=1,
                  prune_type: str='BasicMagnitude', method: str='per_tensor',
                  names: List=[], parameters: Dict=None):
+        """Init the pruner config.
+
+        Args:
+            epoch_range: A list with length of 2. The first element is the start epoch and the second element
+                is the end epoch. Pruning will be done from the start epoch to the end epoch.
+            initial_sparsity_ratio: Initial sparsity goal
+            target_sparsity_ratio: Target sparsity goal
+            update_frequency: How many epochs to update once
+            prune_type: "BasicMagnitude", "PatternLock", or "GroupLasso"
+            method: TODO (Remove this parameter)
+            names: A list of layer names that need to be pruned
+            parameters: A dictionary of extra parameters
+        """
         if epoch_range is not None:
             assert len(epoch_range) == 2, "Please set the epoch_range as [start_epoch, end_epoch]"
             self.start_epoch = epoch_range[0]
             self.end_epoch = epoch_range[1]
         else:
             self.start_epoch = None
             self.end_epoch = None
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/quantization.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/quantization.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Quantization: specify the supported quantization mode."""
+
 from enum import Enum
 from transformers.utils.versions import require_version
 
 try:
     require_version("neural_compressor>=1.9.0")
 except:
     require_version("neural_compressor_full>=1.9.0", "To fix: pip install neural_compressor")
 
 
 class QuantizationMode(Enum):
-
+    """Currently support three quantization modes."""
     POSTTRAININGSTATIC = "post_training_static_quant"
     POSTTRAININGDYNAMIC = "post_training_dynamic_quant"
     QUANTIZATIONAWARETRAINING = "quant_aware_training"
 
 
 SUPPORTED_QUANT_MODE = set([approach.name for approach in QuantizationMode])
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/trainer.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import ast
 import collections
 import inspect
 import math
 import numpy as np
 import os
 import copy
 import sys
@@ -119,15 +118,14 @@
         self.distiller = None
         self.fp32_model = None
         # This flag is set for the engine in the export_to_int8_onnx API.
         self.enable_executor = False
         self.enable_bf16 = False
         self.orchestrate_opt = False
         self.dynamic_config = None
-        
 
     @property
     def resuming_checkpoint(self):
         return self._resuming_checkpoint
 
     @resuming_checkpoint.setter
     def resuming_checkpoint(self, path: str):
@@ -232,39 +230,14 @@
 
         quantizer = Quantization(self.quant_config.inc_config)
         quantizer.model = common.Model(self.model)
 
         self.quantizer = quantizer
         return quantizer
 
-    # pylint: disable=E0401
-    def _nncf_quantize(self):  # pragma: no cover
-        from intel_extension_for_transformers import NncfConfig
-        from nncf import create_compressed_model
-        compression_state = None
-        assert isinstance(self.quant_config, NncfConfig), \
-            "Please pass a NNCFConfig instance to trainer.quantize!"
-
-        self.metrics = self.quant_config.metrics
-        nncf_compression_state_file = self.quant_config.compression_state
-
-        if os.path.isfile(nncf_compression_state_file):
-            compression_state = torch.load(nncf_compression_state_file)
-        else:
-            compression_state = None
-
-        compression_algo_controller, model = create_compressed_model(
-            self.model, self.quant_config.nncf_config, compression_state=compression_state)
-
-        self.compression_ctrl = \
-            compression_algo_controller.distributed() \
-            if self.quant_config.distributed else compression_algo_controller
-
-        self.model = self._train_func(model)
-
     def _inc_quantize(
         self,
         quant_config,
         provider: str = Provider.INC.value,
     ):
         try:
             # we do deepcopy to keep the fp32 model for the export_to_int8_onnx API.
@@ -309,17 +282,15 @@
         self._train_func = self.builtin_train_func if train_func is None else train_func
         if calib_dataloader is not None:
             self._calib_dataloader = calib_dataloader
 
         if self.quantizer is None:
             self._provider = Provider[provider.upper()].value
 
-        if self._provider == Provider.NNCF.value:  # pragma: no cover
-            return self._nncf_quantize()
-        elif self._provider == Provider.INC.value:
+        if self._provider == Provider.INC.value:
             return self._inc_quantize(quant_config=quant_config, provider=provider)
         else:
             assert False, "Unsupport provider:{}".format(self._provider)
 
     def _save_inc_int8(self, opt_model, output_dir):
         if isinstance(opt_model, PyTorchIpexModel):
             opt_model.save(output_dir)
@@ -977,23 +948,14 @@
             # reset tr_loss to zero
             tr_loss -= tr_loss
 
             logs["loss"] = round(
                 tr_loss_scalar / (self.state.global_step - self._globalstep_last_logged), 4)
             logs["learning_rate"] = self._get_learning_rate()
 
-            # pylint: disable=E0401
-            if self.compression_ctrl is not None:
-                from nncf.common.utils.tensorboard import prepare_for_tensorboard
-                logs["compression_loss"] = self.compression_ctrl.loss().item()
-                compression_stats = self.compression_ctrl.statistics()
-                for key, value in prepare_for_tensorboard(compression_stats).items():
-                    logs["compression/statistics/{0}".format(key)] = value
-                print(compression_stats.to_str())
-
             self._total_loss_scalar += tr_loss_scalar
             self._globalstep_last_logged = self.state.global_step
             self.store_flos()
 
             self.log(logs)
 
         metrics = None
@@ -1104,15 +1066,15 @@
             inputs (:obj:`Dict[str, Union[torch.Tensor, Any]]`):
                 The inputs and targets of the model.
                 The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
                 argument :obj:`labels`. Check your model's documentation for all accepted arguments.
         Return:
             :obj:`torch.Tensor`: The tensor with training loss on this batch.
         """
-    
+
         model.train()
         inputs = self._prepare_inputs(inputs)
         tr_loss_sum = 0.0
 
         # compute loss of full model
 
         # pylint: disable=E0401
@@ -1138,15 +1100,14 @@
             # deepspeed handles loss scaling by gradient_accumulation_steps in its `backward`
             loss = loss / self.args.gradient_accumulation_steps
 
         if self.compression_ctrl is not None:  # TODO- should be added here?
             compression_loss = self.compression_ctrl.loss()
             loss += compression_loss
 
- 
         loss = loss / (self.dynamic_config.num_sandwich + 2)
         tr_loss_sum += loss
 
         ## backward
 
         # pylint: disable=E0401
         if version.parse(__version__) < version.parse("4.20"):
@@ -1167,15 +1128,15 @@
                 with amp.scale_loss(loss, self.optimizer) as scaled_loss:
                     scaled_loss.backward()
             elif self.deepspeed:
                 # loss gets scaled under gradient_accumulation_steps in deepspeed
                 loss = self.deepspeed.backward(loss)
             else:
                 loss.backward()
-       
+
         # inplace distillation
         for i in range(self.dynamic_config.num_sandwich + 1):
             ## prepare inputs for sub-models
             num_h_layers = model.config.num_hidden_layers if hasattr(model, "config") else \
                                 model.module.config.num_hidden_layers
 
             layer_config = sample_layer_configuration(
@@ -1235,15 +1196,15 @@
             loss = loss / (self.dynamic_config.num_sandwich + 2)
             tr_loss_sum += loss
 
 
             ## backward
 
             # pylint: disable=E0401
-            
+
             if version.parse(__version__) < version.parse("4.20"):
                 if self.use_amp:
                     self.scaler.scale(loss).backward()
                 elif self.use_apex:
                     with amp.scale_loss(loss, self.optimizer) as scaled_loss:
                         scaled_loss.backward()
                 elif self.deepspeed:
@@ -1262,30 +1223,28 @@
                     loss = self.deepspeed.backward(loss)
                 else:
                     loss.backward()
 
 
         return tr_loss_sum.detach()
 
-
-
     # pylint: disable=E1101
     def compute_loss(self, model, inputs, return_outputs=False):  # pragma: no cover
         """
         How the loss is computed by Trainer. By default, all models return the loss in the first element.
 
         Subclass and override for custom behavior.
         """
         labels = inputs.pop("labels") \
             if self.label_smoother is not None and "labels" in inputs else None
 
         teacher_logits = inputs.pop("teacher_logits") if "teacher_logits" in inputs else None
 
         outputs = model(**inputs)
-    
+
         if self.in_training and hasattr(self, "component") and \
            hasattr(self.component, "criterion"):
             qa_output_merger = lambda outputs: torch.vstack([
                 torch.vstack([sl, el])
                 for sl, el in zip(outputs["start_logits"], outputs["end_logits"])
             ])
             qa_output_spliter = lambda outputs: (outputs[0::2], outputs[1::2])
@@ -1367,18 +1326,15 @@
                                dataset: "datasets.Dataset",
                                description: Optional[str] = None):  # pragma: no cover
         # pylint: disable=E1101
         if not self.args.remove_unused_columns:
             return dataset
         if self._signature_columns is None:
             # Inspect model forward signature to keep only the arguments it accepts.
-            if self._provider == "nncf":
-                signature = inspect.signature(self.model.get_nncf_wrapped_model().forward)
-            else:
-                signature = inspect.signature(self.model.forward)
+            signature = inspect.signature(self.model.forward)
             self._signature_columns = list(signature.parameters.keys())
             # Labels may be named label or label_ids, the default data collator handles that.
             self._signature_columns += ["label", "label_ids", "teacher_logits"]
         columns = [k for k in self._signature_columns if k in dataset.column_names]
         ignored_columns = list(set(dataset.column_names) - set(self._signature_columns))
         if len(ignored_columns) > 0:
             dset_description = "" if description is None else f"in the {description} set "
@@ -1709,19 +1665,15 @@
         output_dir = output_dir if output_dir is not None else self.args.output_dir
         os.makedirs(output_dir, exist_ok=True)
         logger.info(f"Saving model checkpoint to {output_dir}")
         # Save a trained model and configuration using `save_pretrained()`.
         # They can then be reloaded using `from_pretrained()`
         if not isinstance(self.model, PreTrainedModel):  # pragma: no cover
             unwrapped_model = unwrap_model(self.model)
-            if self._provider == "nncf":
-                is_pretrained = isinstance(unwrapped_model.get_nncf_wrapped_model(),
-                                           PreTrainedModel)
-            else:
-                is_pretrained = isinstance(unwrapped_model, PreTrainedModel)
+            is_pretrained = isinstance(unwrapped_model, PreTrainedModel)
 
             if is_pretrained:
                 if state_dict is None:
                     state_dict = unwrapped_model.state_dict()
                 unwrapped_model.save_pretrained(output_dir, state_dict=state_dict)
             else:
                 logger.info(
@@ -1849,14 +1801,15 @@
         self,
         save_path=None,
         quant_format='QDQ',
         dtype='S8S8',
         opset_version=14,
         sample_size=100,
         calibrate_method='minmax',
+        scale_mapping=False,
     ):
         if self.provider != 'inc':  # pragma: no cover
             logger.error("export_to_onnx API only supports INC model right now.")
             sys.exit(0)
 
         if self.enable_executor:
             # Will deprecate after engine supports QDQ format and other op_types.
@@ -1893,20 +1846,38 @@
         # pylint: disable=E1101
         onnx_save_path = save_path if save_path \
           else os.path.join(self.args.output_dir, 'int8-model.onnx')
         self.export_to_fp32_onnx(fp32_path,
                                  opset_version=opset_version,
                                  do_constant_folding=False,
                                  verbose=False)
+        # Fix onnx accuracy drop when trasformers > 4.21.0 
+        if version.parse(__version__) > version.parse("4.21.0"):
+            from onnx import TensorProto
+            model = onnx.load(fp32_path)
+            for node in model.graph.node:
+                if node.op_type == 'Constant' and len(node.attribute) != 0:
+                    constant_value = onnx.numpy_helper.to_array(node.attribute[0].t)
+                    if constant_value.shape == () and \
+                        constant_value == torch.finfo(torch.float32).min:
+                        new_tensor = onnx.helper.make_tensor(
+                            name=node.output[0],
+                            data_type=TensorProto.FLOAT,
+                            dims=[],
+                            vals=[-10000],
+                        )
+                        model.graph.initializer.append(new_tensor)
+                        model.graph.node.remove(node)
+            onnx.save(model, fp32_path)
         model = onnx.load(fp32_path)
 
-        if self.opt_model.q_config['approach'] is 'quant_aware_training':
+        int8_model_dict = {}
+        if self.opt_model.q_config['approach'] == 'quant_aware_training':
             # collect weights, bias from int8 QAT PT model
             model_dict = self.opt_model.model.state_dict()
-            int8_model_dict = {}
             for name, param in model_dict.items():
                 # '_packed_params._packed_weight' is specific for quantized Embedding
                 if '_packed_params._packed_weight' in name:
                     name = name.replace('._packed_params._packed_weight', '').split('.module')[0]
                     int8_model_dict[name + '.weight'] = param.dequantize()
                 # '_packed_params._packed_params' is specific for quantized Linear
                 elif '_packed_params._packed_params' in name and isinstance(param, tuple):
@@ -1933,26 +1904,57 @@
                         dims=tensor.dims,
                         vals=np_tensor,
                     )
                     model.graph.initializer.remove(tensor)
                     model.graph.initializer.append(new_tensor)
             onnx.save(model, fp32_path)
 
+        if scale_mapping and \
+          self.opt_model.q_config['approach'] != 'post_training_dynamic_quant':  # pragma: no cover
+            # get output scale and zp from module
+            import torch.nn.quantized.modules as q_modules
+            for name, module in self.opt_model.model.named_modules():
+                if isinstance(module, q_modules.Conv1d) or \
+                  isinstance(module, q_modules.Conv2d) or \
+                  isinstance(module, q_modules.Linear):
+                    int8_model_dict[name] = {
+                        'output_scale': module.scale,
+                        'output_zeropoint': module.zero_point,
+                    }
+
+            # a name mapping to avoid '_' and '.' mismatch, we only use '.'.
+            new_name_mapping = {}
+            for name in int8_model_dict.keys():
+                new_name = name.replace("_", '.')
+                new_name_mapping.update({new_name: name})
+
+            # get input scale and zp from q_config
+            for name, value in self.opt_model.q_config['get_attr'].items():
+                node_name, node_target = name.split('--')
+                if 'scale' in name:
+                    value_dict = {'input_scale': value}
+                if 'zero_point' in name:
+                    value_dict = {'input_zeropoint': value}
+                tmp_name = node_name + '.' + node_target.split('_input_')[0]
+                tmp_name = tmp_name.replace("_", '.')
+                node_name = new_name_mapping[tmp_name]
+                int8_model_dict[node_name].update(value_dict)
+
         from neural_compressor.adaptor.onnxrt import ONNXRTAdaptor
         # pylint: disable=E1120
         inc_model = ONNXRTAdaptor._replace_gemm_with_matmul(model)
         model = inc_model.model
         onnx.save(model, fp32_path)
 
         # Get weight name from onnx initializer
         weight_name_list = []
         for tensor in model.graph.initializer:
             weight_name_list.append(tensor.name)
 
-        # Match weight name with onnx node name
+        # Match weight name with onnx node name with fp32 model
         quantize_nodes = []
         tmp_node_mapping = {}
         module_node_mapping = {}
         for node in model.graph.node:
             if node.op_type not in op_types_to_quantize:
                 for inp in node.input:
                     if inp in weight_name_list and 'weight' in inp:
@@ -2001,15 +2003,15 @@
             # So U8S8(acitvation|weight) option is not workable for best performance.
             logger.error("Right now, we don't support dtype: {}, \
                           please use U8U8/U8S8/S8S8.".format(dtype))
             sys.exit(0)
         logger.info("Weight type: {}.".format(weight_type))
         logger.info("Activation type: {}.".format(activation_type))
 
-        # Calibrate_method, min/max method as default. 
+        # Calibrate_method, min/max method as default.
         if 'minmax' in calibrate_method:
             calibrate_method = ortq.CalibrationMethod.MinMax
         elif 'percentile' in calibrate_method:
             calibrate_method = ortq.CalibrationMethod.Percentile
         elif 'entropy' in calibrate_method:
             calibrate_method = ortq.CalibrationMethod.Entropy
 
@@ -2057,14 +2059,55 @@
                 activation_type=activation_type,
                 nodes_to_quantize=quantize_nodes,
                 nodes_to_exclude=[],
                 #op_types_to_quantize=op_types_to_quantize,
                 calibrate_method=calibrate_method,
                 extra_options={})
 
+            if scale_mapping:  # pragma: no cover
+                node_module_mapping = {}
+                for module_name, node_name in module_node_mapping.items():
+                    node_module_mapping[node_name] = module_name
+                # match scale and zeropoint from PyTorch to ONNX node
+                scale_zp_dict = {}
+                for node in model.graph.node:
+                    if node.name in node_module_mapping:
+                        module_name = node_module_mapping[node.name]
+                        if module_name not in int8_model_dict:
+                            module_name = module_name + '.module'
+                        if module_name in int8_model_dict:
+                            recoder = int8_model_dict[module_name]
+                            input_scale_args = node.input[0] + '_scale'
+                            input_zp_args = node.input[0] + '_zero_point'
+                            scale_zp_dict[input_scale_args] = recoder['input_scale']
+                            scale_zp_dict[input_zp_args] = recoder['input_zeropoint']
+                            # We need Matmul+Add to match Linear for output scale and zero-point
+                            # output_scale_args = node.output[0] + '_scale'
+                            # output_zp_args = node.output[0] + '_zero_point'
+                            # scale_zp_dict[output_scale_args] = recoder['output_scale']
+                            # scale_zp_dict[output_zp_args] = recoder['output_zeropoint']
+                # set scale and zeropoint from PyTorch int8 model to ONNX int8 model
+                from onnx import helper
+                int8_model = onnx.load(onnx_save_path)
+                tensor_list = [tensor for tensor in int8_model.graph.initializer]
+                for tensor in tensor_list:
+                    if tensor.name in scale_zp_dict:
+                        value = scale_zp_dict[tensor.name]
+                        if 'zero_point' in tensor.name and activation_type == ortq.QuantType.QInt8:
+                            value -= 128
+                        new_tensor = helper.make_tensor(
+                            name=tensor.name,
+                            data_type=tensor.data_type,
+                            dims=tensor.dims,
+                            vals=[value],
+                        )
+                        int8_model.graph.initializer.remove(tensor)
+                        int8_model.graph.initializer.append(new_tensor)
+                onnx.save(int8_model, onnx_save_path)
+
         if os.path.isfile(fp32_path):
             os.remove(fp32_path)
 
         info = "The ONNX Model is exported to path: {0}".format(onnx_save_path)
         logger.info("*" * len(info))
         logger.info(info)
         logger.info("*" * len(info))
@@ -2099,42 +2142,42 @@
         dynamic_config: DynamicLengthConfig,
     ):
 
         self.dynamic_config = dynamic_config
         lc = None
 
         if self.dynamic_config.length_config is not None:
+            import ast
             lc = ast.literal_eval(self.dynamic_config.length_config)
         else:
             assert self.dynamic_config.max_length is not None, \
             """
             Please set max_length DynamicLengthConfig
             """
             if self.dynamic_config.const_rate is not None:
                 lc = sample_length_configuration(
                         self.dynamic_config.max_length,
                         self.model.config.num_hidden_layers,
                         length_drop_ratio=self.dynamic_config.const_rate,
                     )
-        
+
         if lc is not None:
             # set the model with length config
             if self.model.config.model_type == "distilbert":
                 bert = self.model.distilbert
             elif self.model.config.model_type == "roberta":
                 bert = self.model.roberta
             else:
                 assert hasattr(self.model, "bert")
                 bert = self.model.bert
 
             print("setting length config to - " + str(lc))
             bert.set_length_config(lc)
             bert.set_output_attentions(True)
 
-           
     def run_evolutionary_search(self):
         assert self.dynamic_config is not None, \
             """
             Please set a DynamicLengthConfig to run evo-search
             """
         evolution = Evolution(self.model, self.dynamic_config.max_length, self.args.device, self.evaluate, \
                                 eval_metric=self.dynamic_config.evo_eval_metric)
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/metrics.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/models/modeling_bert_dynamic.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/models/modeling_bert_dynamic.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/models/modeling_roberta_dynamic.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/models/modeling_roberta_dynamic.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/objectives.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/objectives.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/utility.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/utility.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/optimization/utils/utility_tf.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/optimization/utils/utility_tf.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import json
 from collections import OrderedDict, UserDict
+from neural_compressor.experimental import common
 
 TMPPATH = os.path.join('tmp', 'model')
 TEACHERPATH = os.path.join('tmp', 'teacher_model')
 class TFDataloader(object):
     """
        Args:
            dataset (string): Dataset
@@ -74,7 +75,13 @@
 def get_filepath(base_dirpath, task_type, task_id):
     if task_type is None:    # single node
         return base_dirpath
     elif _is_chief(task_type, task_id):
         return os.path.join(base_dirpath, 'chief')
     else:
         return os.path.join(base_dirpath, 'worker_' + str(task_id))
+
+
+# convert a Keras model to SavedModel
+def keras2SavedModel(model):   # pragma: no cover
+    model = common.Model(model)
+    return model.model
```

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/preprocessing/data_augmentation.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/preprocessing/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers/preprocessing/utils.py` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `intel_extension_for_transformers-1.0a0/intel_extension_for_transformers.egg-info/SOURCES.txt` & `intel_extension_for_transformers-1.0b0/intel_extension_for_transformers.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/all.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/assert.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/batch_matmul.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/batch_matmul_v2.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/bias_add.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/cast.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/concat.py
+./intel_extension_for_transformers/backends/neural_engine/compile/ops/conv.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/empty_ops.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/expand_dims.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_batch_matmul_v2.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_batch_norm_v3.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_gemm.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/fused_matmul.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/gather.py
+./intel_extension_for_transformers/backends/neural_engine/compile/ops/gather_elements.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/gelu.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/gemm.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/iterator_get_next.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/iterator_v2.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/layer_normalization.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/map_and_batch_dataset.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/matmul.py
@@ -51,29 +53,37 @@
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/pack.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/placeholder.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_linear.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/quantize_v2.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_fused_matmul_and_dequantize.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/quantized_matmul_with_bias_and_dequantize.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/reduce_mean.py
+./intel_extension_for_transformers/backends/neural_engine/compile/ops/reduce_sum.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/reshape.py
+./intel_extension_for_transformers/backends/neural_engine/compile/ops/scatter_elements.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/softmax.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/split.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/squeeze.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/strided_slice.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/tensor.py
+./intel_extension_for_transformers/backends/neural_engine/compile/ops/top_k.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/transpose.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/unpack.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/ops/unsqueeze.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/__init__.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/add_cls_token.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/add_embeddings.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_mask_length_adaptive_keep_indices.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_output_layer_norm_length_adaptive_keep_indices.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/attention_reshape.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/collect_quant_info.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/conv_reshape.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/embeddingbag.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/gelu.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/generate_sequence.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_data.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/input_file.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_bf16_node.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/insert_quant_node.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/interact_features.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/last_layer_shape.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/layer_norm.py
@@ -86,16 +96,22 @@
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/matmul_with_bias_tanh.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/merged_embeddingbag.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/output_data.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/padding_sequence.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/pattern.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/position_embeddings_v1.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/qkv_merge.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/qkv_reshape.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/quantize_fusion.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/reshape_after_restore_hidden_states.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/reshape_before_and_after_attention_out_layer_norm_gather_elements.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/reshape_before_restore_hidden_states.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/reshape_fusion.py
+./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/restore_hidden_states_in_length_adaptive_update_indices.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/start_end_logits.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/subgraph_matcher.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/token_type_embeddings_v1.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/transpose_batch_matmul.py
 ./intel_extension_for_transformers/backends/neural_engine/compile/sub_graph/word_embeddings.py
 ./intel_extension_for_transformers/optimization/__init__.py
@@ -110,14 +126,20 @@
 ./intel_extension_for_transformers/optimization/quantization.py
 ./intel_extension_for_transformers/optimization/trainer.py
 ./intel_extension_for_transformers/optimization/dynamic/__init__.py
 ./intel_extension_for_transformers/optimization/dynamic/drop_and_restore_utils.py
 ./intel_extension_for_transformers/optimization/dynamic/evolution.py
 ./intel_extension_for_transformers/optimization/mixture/__init__.py
 ./intel_extension_for_transformers/optimization/mixture/auto_distillation.py
+./intel_extension_for_transformers/optimization/pytorch_pruner/__init__.py
+./intel_extension_for_transformers/optimization/pytorch_pruner/patterns.py
+./intel_extension_for_transformers/optimization/pytorch_pruner/prune_utils.py
+./intel_extension_for_transformers/optimization/pytorch_pruner/pruner.py
+./intel_extension_for_transformers/optimization/pytorch_pruner/pruning.py
+./intel_extension_for_transformers/optimization/pytorch_pruner/scheduler.py
 ./intel_extension_for_transformers/optimization/utils/__init__.py
 ./intel_extension_for_transformers/optimization/utils/metrics.py
 ./intel_extension_for_transformers/optimization/utils/objectives.py
 ./intel_extension_for_transformers/optimization/utils/utility.py
 ./intel_extension_for_transformers/optimization/utils/utility_tf.py
 ./intel_extension_for_transformers/optimization/utils/models/__init__.py
 ./intel_extension_for_transformers/optimization/utils/models/modeling_bert_dynamic.py
```

### Comparing `intel_extension_for_transformers-1.0a0/setup.py` & `intel_extension_for_transformers-1.0b0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Setup and install modules."""
 from io import open
 from setuptools import find_packages, setup, Extension
 from setuptools.command.build_ext import build_ext
 import os
 import re
 import sys
 import shutil
@@ -15,45 +16,45 @@
     with open(filepath) as version_file:
         __version__, = re.findall('__version__ = "(.*)"', version_file.read())
 except Exception as error:
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 def which(thefile):
+    """Get the path where the file is located."""
     path = os.environ.get("PATH", os.defpath).split(os.pathsep)
     if path == None:
-      return None
+        return None
     for d in path:
         fname = os.path.join(d, thefile)
         fnames = [fname]
         if sys.platform == 'win32':
             exts = os.environ.get('PATHEXT', '').split(os.pathsep)
             if exts == None:
-              return None
+                return None
             fnames += [fname + ext for ext in exts]
         for name in fnames:
             if os.access(name, os.F_OK | os.X_OK) and not os.path.isdir(name):
                 return name
     return None
 
 
 def get_version(cmd):
-    "Returns cmake version."
+    """Returns cmake version."""
     try:
         for line in check_output([cmd, '--version']).decode('utf-8').split('\n'):
             if 'version' in line:
                 print(line.strip().split(' ')[2])
                 return Version(line.strip().split(' ')[2])
     except Exception as error:
         return Version('0.0.0')
 
 
 def get_cmake_command():
-    "Returns cmake command."
-
+    """Returns cmake command."""
     cmake_command = 'cmake'
     if sys.platform == 'win32':
         return cmake_command
     cmake3 = which('cmake3')
     cmake = which('cmake')
     if cmake3 is not None:
         if cmake is not None:
@@ -64,47 +65,93 @@
             cmake_command = 'cmake3'
     elif cmake is None:
         raise RuntimeError('no cmake or cmake3 found')
     return cmake_command
 
 
 class build_ext(build_ext):
+    """Extension builder."""
     def build_extension(self, ext):
+        """Build the neural engine extension."""
         if not sys.platform.startswith("win"):
             import pathlib
             cwd = pathlib.Path().absolute()
 
             build_temp = pathlib.Path(self.build_temp)
             build_temp.mkdir(parents=True, exist_ok=True)
             extdir = pathlib.Path(self.get_ext_fullpath(ext.name))
             executable_path = extdir.parent.absolute()
+            executable_path.mkdir(parents=True,exist_ok=True)
             cmake_args = [
-                '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=' + str(extdir.parent.absolute()),
+                '-DCMAKE_BUILD_TYPE=Release',
+                '-DNE_WITH_SPARSELIB=ON',
+                '-DNE_WITH_TESTS=OFF',
                 '-DPYTHON_EXECUTABLE={}'.format(sys.executable)
             ]
 
             build_args = ['-j']
             cmake_command = get_cmake_command()
             os.chdir(str(build_temp))
             self.spawn([cmake_command, ext.sourcedir] + cmake_args)
             self.spawn(['make'] + build_args)
-            if os.path.exists('neural_engine'):
-                shutil.copy('neural_engine', executable_path)
+
+            import glob
+            bin_lists=glob.glob('bin/neural_engine*')
+            bin_lists.extend(glob.glob('lib/*.so*'))
+            for path in bin_lists:
+                shutil.copy(path, executable_path, follow_symlinks=False)
+                print(path)
             os.chdir(str(cwd))
         else:
-            print("Neural Engine is not support windows for now")
+            import pathlib
+            cwd = pathlib.Path().absolute()
+    
+            build_temp = pathlib.Path(self.build_temp)
+            build_temp.mkdir(parents=True, exist_ok=True)
+            extdir = pathlib.Path(self.get_ext_fullpath(ext.name))
+            executable_path = extdir.parent.absolute()
+            executable_path.mkdir(parents=True,exist_ok=True)
+            cmake_args = [
+                '-G Ninja',
+                '-DCMAKE_BUILD_TYPE=Release',
+                '-DNE_WITH_SPARSELIB=ON',
+                '-DNE_WITH_TESTS=OFF',
+                "-DCMAKE_C_COMPILER=cl.exe",
+                "-DCMAKE_CXX_COMPILER=cl.exe",
+                '-DPYTHON_EXECUTABLE={}'.format(sys.executable)
+            ]
+            build_args = [
+                '--build',
+                './',
+                '-j'
+            ]
+            cmake_command = get_cmake_command() 
+            os.chdir(str(build_temp))
+            self.spawn([cmake_command, ext.sourcedir] + cmake_args)
+            self.spawn(['cmake'] + build_args)
+            import glob
+            
+            bin_lists=glob.glob('bin/*.exe')
+            bin_lists.extend(glob.glob('bin/*.dll'))
+            bin_lists.extend(glob.glob('lib/*.pyd'))
+            for path in bin_lists:
+                shutil.copy(path, executable_path, follow_symlinks=False)
+            os.chdir(str(cwd))
 
 
 class CMakeExtension(Extension):
+    """CMakeExtension class."""
     def __init__(self, name, sourcedir=""):
+        """Init a CMakeExtension object."""
         Extension.__init__(self, name, sources=[])
         self.sourcedir = os.path.abspath(sourcedir)
 
 
 def check_submodules():
+    """Check submodules information."""
     def check_for_files(folder, files):
         if not any(os.path.exists(os.path.join(folder, f)) for f in files):
             report("Could not find any of {} in {}".format(", ".join(files), folder))
             report("Did you run 'git submodule update --init --recursive'?")
             sys.exit(1)
 
     def not_exists_or_empty(folder):
@@ -139,28 +186,25 @@
 
     setup(
         name="intel_extension_for_transformers",
         version=__version__,
         author="Intel AIA/AIPC Team",
         author_email=
         "feng.tian@intel.com, haihao.shen@intel.com,hanwen.chang@intel.com, penghui.cheng@intel.com",
-        description="Repository of Intel® Extension for Transformers",
+        description="Repository of Intel® Intel Extension for Transformers",
         long_description=open("README.md", "r", encoding='utf-8').read(),
         long_description_content_type="text/markdown",
         keywords=
         'quantization, auto-tuning, post-training static quantization, post-training dynamic quantization, quantization-aware training, tuning strategy',
         license='Apache 2.0',
         url="https://github.com/intel/",
-        ext_modules=[
-            CMakeExtension("neural_engine_py",
-                           str(cwd) + '/intel_extension_for_transformers/backends/neural_engine/executor/')
-        ],
-        packages=find_packages(),
-        include_package_data=True,
-        package_dir={'': '.'},
+        ext_modules=[CMakeExtension("neural_engine_py", str(cwd) + '/intel_extension_for_transformers/backends/neural_engine/')],
+        packages = find_packages(),
+        include_package_data = True,
+        package_dir = {'':'.'},
         package_data={
             '': ['*.py', '*.yaml'],
             'executor': ['*.py'],
         },
         cmdclass={
             'build_ext': build_ext,
         },
```

