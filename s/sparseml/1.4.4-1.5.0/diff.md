# Comparing `tmp/sparseml-1.4.4-py3-none-any.whl.zip` & `tmp/sparseml-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,350 +1,370 @@
-Zip file size: 906292 bytes, number of entries: 348
--rw-rw-r--  2.0 unx     1683 b- defN 23-Mar-24 18:52 sparseml/__init__.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Mar-24 18:52 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Mar-24 18:52 sparseml/log.py
--rw-rw-r--  2.0 unx     1510 b- defN 23-Mar-24 18:52 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Mar-24 18:52 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-Mar-24 18:52 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Mar-24 18:52 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Mar-24 18:52 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Mar-24 18:52 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Mar-24 18:52 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Mar-24 18:52 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Mar-24 18:52 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Mar-24 18:52 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Mar-24 18:52 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Mar-24 18:52 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     4684 b- defN 23-Mar-24 18:52 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2170 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7546 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4350 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/matmul_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx     8704 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14130 b- defN 23-Mar-24 18:52 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Mar-24 18:52 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Mar-24 18:52 sparseml/framework/info.py
--rw-rw-r--  2.0 unx      858 b- defN 23-Mar-24 18:52 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Mar-24 18:52 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Mar-24 18:52 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Mar-24 18:52 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Mar-24 18:52 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Mar-24 18:52 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Mar-24 18:52 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Mar-24 18:52 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Mar-24 18:52 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Mar-24 18:52 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Mar-24 18:52 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Mar-24 18:52 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Mar-24 18:52 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Mar-24 18:52 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Mar-24 18:52 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Mar-24 18:52 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Mar-24 18:52 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Mar-24 18:52 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Mar-24 18:52 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Mar-24 18:52 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Mar-24 18:52 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Mar-24 18:52 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Mar-24 18:52 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Mar-24 18:52 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Mar-24 18:52 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Mar-24 18:52 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Mar-24 18:52 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Mar-24 18:52 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Mar-24 18:52 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Mar-24 18:52 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Mar-24 18:52 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Mar-24 18:52 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Mar-24 18:52 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Mar-24 18:52 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Mar-24 18:52 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Mar-24 18:52 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Mar-24 18:52 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Mar-24 18:52 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Mar-24 18:52 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Mar-24 18:52 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Mar-24 18:52 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Mar-24 18:52 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Mar-24 18:52 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13274 b- defN 23-Mar-24 18:52 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19634 b- defN 23-Mar-24 18:52 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Mar-24 18:52 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Mar-24 18:52 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14520 b- defN 23-Mar-24 18:52 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Mar-24 18:52 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4514 b- defN 23-Mar-24 18:52 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Mar-24 18:52 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Mar-24 18:52 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Mar-24 18:52 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Mar-24 18:52 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Mar-24 18:52 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13002 b- defN 23-Mar-24 18:52 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-Mar-24 18:52 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Mar-24 18:52 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    41184 b- defN 23-Mar-24 18:52 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Mar-24 18:52 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31516 b- defN 23-Mar-24 18:52 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Mar-24 18:52 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Mar-24 18:52 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3694 b- defN 23-Mar-24 18:52 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Mar-24 18:52 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Mar-24 18:52 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Mar-24 18:52 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Mar-24 18:52 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Mar-24 18:52 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    23742 b- defN 23-Mar-24 18:52 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Mar-24 18:52 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Mar-24 18:52 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-Mar-24 18:52 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6173 b- defN 23-Mar-24 18:52 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Mar-24 18:52 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10826 b- defN 23-Mar-24 18:52 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Mar-24 18:52 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Mar-24 18:52 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Mar-24 18:52 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18258 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20912 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    11781 b- defN 23-Mar-24 18:52 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40335 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40931 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10190 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Mar-24 18:52 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Mar-24 18:52 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Mar-24 18:52 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Mar-24 18:52 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Mar-24 18:52 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Mar-24 18:52 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26711 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Mar-24 18:52 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Mar-24 18:52 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Mar-24 18:52 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Mar-24 18:52 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Mar-24 18:52 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14533 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63525 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    23769 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4580 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33543 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26253 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12560 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17476 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    67038 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Mar-24 18:52 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Mar-24 18:52 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Mar-24 18:52 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Mar-24 18:52 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Mar-24 18:52 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    40545 b- defN 23-Mar-24 18:52 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Mar-24 18:52 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Mar-24 18:52 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    30763 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    38943 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx    30536 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8382 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Mar-24 18:52 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Mar-24 18:52 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Mar-24 18:52 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Mar-24 18:52 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Mar-24 18:52 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Mar-24 18:52 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Mar-24 18:52 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Mar-24 18:52 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Mar-24 18:52 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Mar-24 18:52 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Mar-24 18:52 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Mar-24 18:52 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Mar-24 18:52 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Mar-24 18:52 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Mar-24 18:52 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Mar-24 18:52 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     4273 b- defN 23-Mar-24 18:52 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    19721 b- defN 23-Mar-24 18:52 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30936 b- defN 23-Mar-24 18:52 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36738 b- defN 23-Mar-24 18:52 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40358 b- defN 23-Mar-24 18:52 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34464 b- defN 23-Mar-24 18:52 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Mar-24 18:52 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Mar-24 18:52 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43523 b- defN 23-Mar-24 18:52 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Mar-24 18:52 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Mar-24 18:52 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Mar-24 18:52 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Mar-24 18:52 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    15797 b- defN 23-Mar-24 18:52 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Mar-24 18:52 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Mar-24 18:52 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26321 b- defN 23-Mar-24 18:52 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Mar-24 18:52 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Mar-24 18:52 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Mar-24 18:52 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Mar-24 18:52 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Mar-24 18:52 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Mar-24 18:52 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Mar-24 18:52 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Mar-24 18:52 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Mar-24 18:52 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Mar-24 18:52 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Mar-24 18:52 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Mar-24 18:52 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Mar-24 18:52 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     3908 b- defN 23-Mar-24 18:52 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Mar-24 18:52 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     3154 b- defN 23-Mar-24 18:52 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Mar-24 18:52 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Mar-24 18:52 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Mar-24 18:54 sparseml-1.4.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx    22025 b- defN 23-Mar-24 18:54 sparseml-1.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Mar-24 18:54 sparseml-1.4.4.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-24 18:54 sparseml-1.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2206 b- defN 23-Mar-24 18:54 sparseml-1.4.4.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Mar-24 18:54 sparseml-1.4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    34540 b- defN 23-Mar-24 18:54 sparseml-1.4.4.dist-info/RECORD
-348 files, 3311291 bytes uncompressed, 850396 bytes compressed:  74.3%
+Zip file size: 945565 bytes, number of entries: 368
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-02 02:44 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-02 02:44 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-02 02:44 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-02 02:44 sparseml/log.py
+-rw-rw-r--  2.0 unx     1510 b- defN 23-Jun-02 02:44 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jun-02 02:44 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-02 02:44 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-02 02:44 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jun-02 02:44 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-02 02:44 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-02 02:44 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-02 02:44 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-02 02:44 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-02 02:44 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-02 02:44 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-02 02:44 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     4751 b- defN 23-Jun-02 02:44 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2252 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4470 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4571 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx     8704 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-02 02:44 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-02 02:44 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx      970 b- defN 23-Jun-02 02:44 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-02 02:44 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jun-02 02:44 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-02 02:44 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-02 02:44 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-02 02:44 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-02 02:44 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-02 02:44 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jun-02 02:44 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-02 02:44 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-02 02:44 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-02 02:44 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-02 02:44 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-02 02:44 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-02 02:44 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jun-02 02:44 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-02 02:44 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jun-02 02:44 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-02 02:44 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-02 02:44 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-02 02:44 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-02 02:44 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-02 02:44 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-02 02:44 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-02 02:44 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jun-02 02:44 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-02 02:44 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jun-02 02:44 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-02 02:44 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13274 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19634 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14520 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4514 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jun-02 02:44 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-02 02:44 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-02 02:44 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-02 02:44 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13002 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    41311 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31586 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jun-02 02:44 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3694 b- defN 23-Jun-02 02:44 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-02 02:44 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-02 02:44 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jun-02 02:44 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-02 02:44 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-02 02:44 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-02 02:44 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-02 02:44 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-02 02:44 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Jun-02 02:44 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6173 b- defN 23-Jun-02 02:44 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-02 02:44 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10826 b- defN 23-Jun-02 02:44 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jun-02 02:44 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-02 02:44 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20912 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jun-02 02:44 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-02 02:44 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-02 02:44 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-02 02:44 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26253 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17591 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    69783 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    40790 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31056 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-02 02:44 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-02 02:44 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-02 02:44 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-02 02:44 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-02 02:44 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-02 02:44 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-02 02:44 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-02 02:44 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-02 02:44 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-02 02:44 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-02 02:44 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-02 02:44 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-02 02:44 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-02 02:44 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx      987 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-02 02:44 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    19721 b- defN 23-Jun-02 02:44 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-02 02:44 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-02 02:44 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40177 b- defN 23-Jun-02 02:44 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34284 b- defN 23-Jun-02 02:44 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-02 02:44 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-02 02:44 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43756 b- defN 23-Jun-02 02:44 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-02 02:44 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jun-02 02:44 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-02 02:44 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-02 02:44 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    15797 b- defN 23-Jun-02 02:44 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jun-02 02:44 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jun-02 02:44 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26321 b- defN 23-Jun-02 02:44 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-02 02:44 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-02 02:44 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-02 02:44 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-02 02:44 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-02 02:44 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-02 02:44 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-02 02:44 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-02 02:44 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-02 02:44 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-02 02:44 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-02 02:44 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-02 02:44 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-02 02:44 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5763 b- defN 23-Jun-02 02:44 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-02 02:44 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-02 02:44 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-02 02:44 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    34525 b- defN 23-Jun-02 02:44 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-02 02:44 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-02 02:44 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jun-02 02:44 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6298 b- defN 23-Jun-02 02:44 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-02 02:44 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21503 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    36457 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/RECORD
+368 files, 3422842 bytes uncompressed, 886595 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: sparseml/__init__.py
 Comment: 
 
+Filename: sparseml/analytics.py
+Comment: 
+
 Filename: sparseml/base.py
 Comment: 
 
 Filename: sparseml/log.py
 Comment: 
 
 Filename: sparseml/version.py
@@ -84,15 +87,18 @@
 
 Filename: sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/initializers_to_uint8.py
 Comment: 
 
-Filename: sparseml/exporters/transforms/matmul_to_matmulinteger_add_cast_mul.py
+Filename: sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+Comment: 
+
+Filename: sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/onnx_transform.py
 Comment: 
@@ -666,14 +672,17 @@
 
 Filename: sparseml/pytorch/sparsification/training/__init__.py
 Comment: 
 
 Filename: sparseml/pytorch/sparsification/training/modifier_epoch.py
 Comment: 
 
+Filename: sparseml/pytorch/sparsification/training/modifier_logging.py
+Comment: 
+
 Filename: sparseml/pytorch/sparsification/training/modifier_lr.py
 Comment: 
 
 Filename: sparseml/pytorch/sparsification/training/modifier_params.py
 Comment: 
 
 Filename: sparseml/pytorch/sparsification/training/modifier_regularizer.py
@@ -714,14 +723,17 @@
 
 Filename: sparseml/pytorch/utils/exporter.py
 Comment: 
 
 Filename: sparseml/pytorch/utils/helpers.py
 Comment: 
 
+Filename: sparseml/pytorch/utils/log_sparsification_info.py
+Comment: 
+
 Filename: sparseml/pytorch/utils/logger.py
 Comment: 
 
 Filename: sparseml/pytorch/utils/loss.py
 Comment: 
 
 Filename: sparseml/pytorch/utils/model.py
@@ -735,14 +747,26 @@
 
 Filename: sparseml/pytorch/utils/ssd_helpers.py
 Comment: 
 
 Filename: sparseml/pytorch/utils/yolo_helpers.py
 Comment: 
 
+Filename: sparseml/pytorch/utils/sparsification_info/__init__.py
+Comment: 
+
+Filename: sparseml/pytorch/utils/sparsification_info/configs.py
+Comment: 
+
+Filename: sparseml/pytorch/utils/sparsification_info/helpers.py
+Comment: 
+
+Filename: sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+Comment: 
+
 Filename: sparseml/recipe_template/__init__.py
 Comment: 
 
 Filename: sparseml/recipe_template/utils.py
 Comment: 
 
 Filename: sparseml/sparsification/__init__.py
@@ -1017,29 +1041,65 @@
 
 Filename: sparseml/yolov5/helpers.py
 Comment: 
 
 Filename: sparseml/yolov5/scripts.py
 Comment: 
 
-Filename: sparseml-1.4.4.dist-info/LICENSE
+Filename: sparseml/yolov5/yolov5.status.yaml
+Comment: 
+
+Filename: sparseml/yolov8/__init__.py
+Comment: 
+
+Filename: sparseml/yolov8/default.yaml
+Comment: 
+
+Filename: sparseml/yolov8/export.py
+Comment: 
+
+Filename: sparseml/yolov8/modules.py
+Comment: 
+
+Filename: sparseml/yolov8/train.py
+Comment: 
+
+Filename: sparseml/yolov8/trainers.py
+Comment: 
+
+Filename: sparseml/yolov8/val.py
+Comment: 
+
+Filename: sparseml/yolov8/validators.py
+Comment: 
+
+Filename: sparseml/yolov8/utils/__init__.py
+Comment: 
+
+Filename: sparseml/yolov8/utils/export_samples.py
+Comment: 
+
+Filename: sparseml/yolov8/utils/helpers.py
+Comment: 
+
+Filename: sparseml-1.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml-1.4.4.dist-info/METADATA
+Filename: sparseml-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: sparseml-1.4.4.dist-info/NOTICE
+Filename: sparseml-1.5.0.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml-1.4.4.dist-info/WHEEL
+Filename: sparseml-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml-1.4.4.dist-info/entry_points.txt
+Filename: sparseml-1.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml-1.4.4.dist-info/top_level.txt
+Filename: sparseml-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml-1.4.4.dist-info/RECORD
+Filename: sparseml-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/__init__.py

```diff
@@ -39,19 +39,11 @@
 )
 from .sparsification import (
     SparsificationInfo,
     sparsification_info,
     save_sparsification_info,
     load_sparsification_info,
 )
+from .analytics import sparseml_analytics as _analytics
 
-try:
-    from sparsezoo.package import check_package_version as _check_package_version
 
-    _check_package_version(
-        package_name=__name__ if is_release else f"{__name__}-nightly",
-        package_version=version,
-    )
-except Exception as err:
-    print(
-        f"Need sparsezoo version above 0.9.0 to run Neural Magic's latest-version check\n{err}"
-    )
+_analytics.send_event("python__init")
```

## sparseml/version.py

```diff
@@ -15,15 +15,15 @@
 """
 Functionality for storing and setting the version info for SparseML
 """
 
 from datetime import date
 
 
-version_base = "1.4.4"
+version_base = "1.5.0"
 is_release = True  # change to True to set the generated version as a release version
 
 
 def _generate_version():
     return (
         version_base
         if is_release
```

## sparseml/exporters/onnx_to_deepsparse.py

```diff
@@ -71,15 +71,16 @@
             sparseml_transforms.InitializersToUint8(),
             sparseml_transforms.FlattenQParams(),
             sparseml_transforms.FoldConvDivBn(),
             sparseml_transforms.DeleteRepeatedQdq(),
             sparseml_transforms.QuantizeQATEmbedding(),
             sparseml_transforms.PropagateEmbeddingQuantization(),
             sparseml_transforms.MatMulToQLinearMatMul(),
-            sparseml_transforms.MatMulToMatMulIntegerAddCastMul(),
+            sparseml_transforms.MatMulAddToMatMulIntegerAddCastMul(),
+            sparseml_transforms.MatMulToMatMulIntegerCastMul(),
             sparseml_transforms.FoldReLUQuants(),
             sparseml_transforms.ConvToQLinearConv()
             if use_qlinear_conv
             else sparseml_transforms.ConvToConvIntegerAddCastMul(),
             sparseml_transforms.GemmToQLinearMatMul(),
             sparseml_transforms.GemmToMatMulIntegerAddCastMul(),
             sparseml_transforms.QuantizeResiduals(),
```

## sparseml/exporters/transforms/__init__.py

```diff
@@ -34,14 +34,15 @@
 from .conv_to_qlinearconv import ConvToQLinearConv
 from .conv_to_convinteger_add_cast_mul import ConvToConvIntegerAddCastMul
 from .fold_conv_div_bn import FoldConvDivBn
 from .fold_relu_quants import FoldReLUQuants
 from .gemm_to_matmulinteger_add_cast_mul import GemmToMatMulIntegerAddCastMul
 from .gemm_to_qlinearmatmul import GemmToQLinearMatMul
 from .initializers_to_uint8 import InitializersToUint8
-from .matmul_to_matmulinteger_add_cast_mul import MatMulToMatMulIntegerAddCastMul
+from .matmul_add_to_matmulinteger_add_cast_mul import MatMulAddToMatMulIntegerAddCastMul
+from .matmul_to_matmulinteger_cast_mul import MatMulToMatMulIntegerCastMul
 from .propagate_embedding_quantization import PropagateEmbeddingQuantization
 from .quantize_qat_embedding import QuantizeQATEmbedding
 from .quantize_residuals import QuantizeResiduals
 from .remove_duplicate_qconv_weights import RemoveDuplicateQConvWeights
 from .remove_duplicate_quantize_ops import RemoveDuplicateQuantizeOps
 from .skip_input_quantize import SkipInputQuantize
```

## sparseml/exporters/transforms/gemm_to_qlinearmatmul.py

```diff
@@ -8,16 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import logging
-
 from onnx import ModelProto, helper, numpy_helper
 
 from sparseml.exporters.transforms.onnx_transform import OnnxTransform
 from sparseml.exporters.transforms.utils import (
     INITIALIZER_MATCH,
     MatchResult,
     any_of,
@@ -27,23 +25,22 @@
     quantize_array,
 )
 from sparseml.onnx.utils import ONNXGraph, get_node_attributes, get_node_output_nodes
 
 
 __all__ = ["GemmToQLinearMatMul"]
 
-_LOGGER = logging.getLogger(__name__)
-
 
 class GemmToQLinearMatMul(OnnxTransform):
     """
     Transforms Gemm nodes to QLinearMatMul.
 
     NOTE: Does not match if the structure is
-    `Gemm -> QuantizeLinear -> DequantizeLinear -> Gemm`
+    1. `Gemm -> QuantizeLinear -> DequantizeLinear -> Gemm`
+    2. `Gemm -> QuantizeLinear -> DequantizeLinear -> Softmax`
 
     Transforms
     ```
     |       weight (initializer)
     |         |
     | input   Q
     |   |     |
@@ -89,15 +86,18 @@
             if any(float(attribute) != 1.0 for attribute in gemm_attributes.values()):
                 # can only handle Gemm operations without alpha/beta/transB set
                 continue
 
             output_dequant = match.children[0][1]
             if output_dequant is not None:
                 output_dequant_child = graph.get_node_single_child(output_dequant)
-                if output_dequant_child and output_dequant_child.op_type == "Gemm":
+                if output_dequant_child and output_dequant_child.op_type in {
+                    "Gemm",
+                    "Softmax",
+                }:
                     # output quant is not a QDQ block for the current Gemm Node but,
                     # the input QDQ block for a new Gemm block this Gemm should be
                     # skipped and processed by _convert_quantizable_gemm_no_activations
                     continue
 
             self.log_match(match)
             self._transform_match(model, match)
```

## sparseml/exporters/transforms/utils/matching.py

```diff
@@ -374,15 +374,21 @@
 
         # NOTE: since these are before the current parent, we iterate backwards
         *head, tail = expected_op_sequence
 
         # NOTE: explicitly only matching against a single parent input here
         #       even though it could have multiple inputs
         sub_match = _match_structure(
-            graph, node=parent, op_type=tail, parent_ops=[head] if head else None
+            graph,
+            # NOTE: here's where we handle optional parent via the match.node is None
+            #       if we are on an optional node that didn't match, we keep using
+            #       `node` instead of recursing on `parent`.
+            node=node if match.node is None else parent,
+            op_type=tail,
+            parent_ops=[head] if head else None,
         )
         if sub_match is None:
             return False
         match.parents.append((sub_match.parents[0] if head else []) + [sub_match.node])
 
     return True
```

## sparseml/keras/__init__.py

```diff
@@ -14,10 +14,15 @@
 
 """
 Functionality for working with and sparsifying Models in the Keras framework
 """
 
 # flake8: noqa
 
+from sparseml.analytics import sparseml_analytics as _analytics
+
 from .base import *
 from .framework import detect_framework, framework_info, is_supported
 from .sparsification import sparsification_info
+
+
+_analytics.send_event("python__keras__init")
```

## sparseml/onnx/__init__.py

```diff
@@ -14,11 +14,16 @@
 
 """
 Functionality for working with and sparsifying Models in the ONNX/ONNXRuntime framework
 """
 
 # flake8: noqa
 
+from sparseml.analytics import sparseml_analytics as _analytics
+
 from .base import *
 from .benchmark import *
 from .framework import detect_framework, framework_info, is_supported
 from .sparsification import ModelInfo, get_analyzer_impls, sparsification_info
+
+
+_analytics.send_event("python__onnx__init")
```

## sparseml/onnx/utils/helpers.py

```diff
@@ -792,15 +792,19 @@
         for the outputs from the given node
     """
     nodes = []
 
     for output_id in get_node_outputs(model, node):
         nodes.extend(get_nodes_by_input_id(model, output_id))
 
-    return nodes
+    unique_nodes = []
+    for node in nodes:
+        if node not in unique_nodes:
+            unique_nodes.append(node)
+    return unique_nodes
 
 
 def is_prunable_node(model: ModelProto, node: NodeProto) -> bool:
     """
     :param model: the model the node is from
     :param node: an ONNX node or op_type string
     :return: True if the given node is prunable, False otherwise
```

## sparseml/onnx/utils/model.py

```diff
@@ -41,20 +41,20 @@
     is_foldable_node,
 )
 from sparsezoo import File, Model
 
 
 try:
     import deepsparse
-    from deepsparse import analyze_model, compile_model
+    from deepsparse import compile_model, model_debug_analysis
     from deepsparse.cpu import cpu_details
 except Exception:
     deepsparse = None
     compile_model = None
-    analyze_model = None
+    model_debug_analysis = None
     cpu_details = None
 
 
 try:
     from openvino.inference_engine import IECore, IENetwork, StatusCode, get_version
 except Exception:
     IENetwork, IECore, get_version, StatusCode = None, None, None, None
@@ -724,56 +724,56 @@
             continue
 
         node = get_node_by_id(model, node_id)
 
         if node is None:
             _LOGGER.warning(
                 (
-                    "node returned from deepsparse.analyze_model "
+                    "node returned from deepsparse.model_debug_analysis "
                     "was not found in the model graph; node id {}"
                 ).format(node_id)
             )
             continue
 
         if is_foldable_node(node):
             _LOGGER.debug(
                 "foldable node of id {} returned from "
-                "deepsparse.analyze_model api, matching to prunable node"
+                "deepsparse.model_debug_analysis api, matching to prunable node"
             )
             # traverse previous because incorrect node id will only be returned
             # for following foldable layers, not previous
             node = get_prunable_node_from_foldable(model, node, traverse_previous=True)
 
             if node is None:
                 _LOGGER.warning(
                     (
                         "could not find prunable node from a foldable node "
-                        "returned in the deepsparse.analyze_model api; "
+                        "returned in the deepsparse.model_debug_analysis api; "
                         "node id: {}"
                     ).format(node_id)
                 )
             else:
                 prunable_node_id = extract_node_id(node)
                 _LOGGER.debug(
                     (
                         "matched prunable node of id {} to foldable node {} as "
-                        "returned from deepsparse.analyze_model api"
+                        "returned from deepsparse.model_debug_analysis api"
                     ).format(prunable_node_id, node_id)
                 )
                 layer["canonical_name"] = prunable_node_id
 
 
 def split_canonical_names(nm_result: Dict):
     """
     Splits analysis layer results from grouped canonical names by individual nodes.
     Stores the original grouped canonical name in the 'meta_canonical_name' field.
 
     Will split on any canonical_name that includes ','.
 
-    :param nm_result: the result from the deepsparse.analyze_model api
+    :param nm_result: the result from the deepsparse.model_debug_analysis api
     """
     split_layer_infos = []
     for layer in nm_result["layer_info"]:
         if "," in layer["canonical_name"]:
             for sub_layer_name in layer["canonical_name"].split(","):
                 sub_layer_info = deepcopy(layer)
                 sub_layer_info["meta_canonical_name"] = layer["canonical_name"]
@@ -784,15 +784,15 @@
             split_layer_infos.append(layer)
     nm_result["layer_info"] = split_layer_infos
 
 
 class DeepSparseAnalyzeModelRunner(_DeepSparseBaseModelRunner):
     """
     Class for handling running inference for an ONNX model through Neural Magic's
-    analyze_model api
+    model_debug_analysis api
 
     :param model: the path to the ONNX model file or the loaded onnx.ModelProto
     :param batch_size: the size of the batch to create the model for
     :param num_cores: the number of physical cores to run the model on. Defaults
         to run on all available cores
     """
 
@@ -834,15 +834,15 @@
         :param num_warmup_iterations: number of iterations to run warmup for
             before benchmarking
         :param optimization_level: the optimization level to use in neural magic;
             1 for optimizations on, 0 for limited optimizations
         :param imposed_ks: kernel sparsity value to impose on all the prunable
             layers in the model. None or no imposed sparsity
         :return: a tuple containing the performance results for the run as returned
-            from the analyze_model function, total time to run them
+            from the model_debug_analysis function, total time to run them
         """
         _check_args(args, kwargs)
 
         return super().run(
             data_loader,
             desc,
             show_progress,
@@ -875,15 +875,15 @@
             layers in the model. None or no imposed sparsity
         :return: a tuple containing the result of the inference,
             the time to perform the inference
         """
         _check_args(args, kwargs)
         nm_batch = list(batch.values())
         pred_time = time.time()
-        nm_pred = analyze_model(
+        nm_pred = model_debug_analysis(
             self._model,
             nm_batch,
             self._batch_size,
             self._num_cores,
             num_iterations,
             num_warmup_iterations,
             optimization_level,
```

## sparseml/openpifpaf/__init__.py

```diff
@@ -7,7 +7,20 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from sparseml.analytics import sparseml_analytics as _analytics
+
+
+try:
+    import cv2 as _cv2  # noqa: F401
+
+    import openpifpaf as _openpifpaf  # noqa: F401
+except ImportError:
+    raise ImportError("Please install sparseml[openpifpaf] to use this pathway")
+
+
+_analytics.send_event("python__openpifpaf__init")
```

## sparseml/optim/manager.py

```diff
@@ -525,14 +525,75 @@
 
         return (
             min(mod.start_epoch for mod in quant_modifiers) < epoch + 1
             if quant_modifiers
             else False
         )
 
+    def phase(self, epoch: float) -> Optional[str]:
+        """
+        Computes the phase that the modifiers are in.
+
+        Example usage:
+
+        ```python
+        phase = BaseManager.compose_staged(
+            manager,
+            checkpoint_manager
+        ).phase()
+        if phase is not None:
+            checkpoint_name = "best_{phase}.pt"
+        ```
+
+        :return: One of the following strings based on the pruning and quantization
+            modifiers that this Manager contains.
+
+            0. None - if either pruning or quantization is currently in progress
+            1. "dense" - if no pruning or quantization
+            2. "dense_quantized" - if only quantization
+            3. "pruned" - if only pruning
+            4. "pruned_quantized" - if both pruning and quantization
+            5. "quantized_pruned" - if quantization was before pruning
+        """
+        pruners: List[BaseModifier] = self.pruning_modifiers
+        quantizers: List[BaseModifier] = self.quantization_modifiers
+
+        if len(pruners) == 0:
+            pruned = False
+            pruning_in_progress = False
+        else:
+            pruning_start = min(mod.start_epoch for mod in pruners)
+            pruning_end = max(mod.end_epoch for mod in pruners)
+            pruning_in_progress = pruning_start <= epoch <= pruning_end
+            pruned = epoch > pruning_end
+
+        if len(quantizers) == 0:
+            quantized = False
+            quantization_in_progress = False
+        else:
+            first_quant_epoch = min(mod.start_epoch for mod in quantizers)
+            last_quant_epoch = max(mod.start_epoch for mod in quantizers)
+            quantization_in_progress = first_quant_epoch <= epoch <= last_quant_epoch
+            quantized = epoch > last_quant_epoch
+
+        if pruning_in_progress or quantization_in_progress:
+            return None
+
+        if not pruned and not quantized:
+            return "dense"
+        elif quantized and not pruned:
+            return "dense_quantized"
+        elif pruned and not quantized:
+            return "pruned"
+        else:
+            if pruning_end < last_quant_epoch:
+                return "pruned_quantized"
+            else:
+                return "quantized_pruned"
+
     def get_start_end_epochs(self) -> Dict[str, Tuple[float, float]]:
         """
         Return an OrderedDict mapping each stage to its min and max epoch. If not a
         staged manager, map 'all' to the the min and max epochs
         """
         if isinstance(self.modifiers, List):
             return OrderedDict({"all": (self.min_epochs, self.max_epochs)})
```

## sparseml/pytorch/base.py

```diff
@@ -45,15 +45,15 @@
     "check_torchvision_install",
     "require_torch",
     "require_torchvision",
 ]
 
 
 _TORCH_MIN_VERSION = "1.0.0"
-_TORCH_MAX_VERSION = "1.12.100"  # set bug to 100 to support all future 1.9.X versions
+_TORCH_MAX_VERSION = "1.13.100"  # set bug to 100 to support all future 1.9.X versions
 
 
 def check_torch_install(
     min_version: Optional[str] = _TORCH_MIN_VERSION,
     max_version: Optional[str] = _TORCH_MAX_VERSION,
     raise_on_error: bool = True,
 ) -> bool:
```

## sparseml/pytorch/image_classification/__init__.py

```diff
@@ -7,7 +7,12 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from sparseml.analytics import sparseml_analytics as _analytics
+
+
+_analytics.send_event("python__pytorch__image_classification__init")
```

## sparseml/pytorch/image_classification/export.py

```diff
@@ -383,17 +383,16 @@
     )
 
     if labels_to_class_mapping is None:
         labels_to_class_mapping = helpers.label_to_class_mapping_from_dataset(dataset)
 
     if recipe is not None:
         ScheduledModifierManager.from_yaml(recipe).apply_structure(model)
-
-    if checkpoint_path:
-        load_model(checkpoint_path, model, strict=True)
+        if checkpoint_path:
+            load_model(checkpoint_path, model, strict=True)
 
     if one_shot is not None:
         ScheduledModifierManager.from_yaml(file_path=one_shot).apply(module=model)
 
     export(
         model=model,
         val_loader=val_loader,
```

## sparseml/pytorch/image_classification/utils/trainer.py

```diff
@@ -229,16 +229,19 @@
             self.recipe_path,
         )
 
         self.manager.apply(self.model)
         _LOGGER.info(f"Applied {self.recipe_path} to manager")
 
     def _initialize_module_tester(self):
+        # This uses self.model.module unlike the ModuleTrainer which uses self.model
+        # so that the validation runs on the local copy of the model on the rank 0 gpu
+        # rather than on the distributed model
         tester = ModuleTester(
-            module=self.model,
+            module=self.model.module if is_parallel_model(self.model) else self.model,
             device=self.device,
             loss=self.val_loss,
             loggers=self.loggers,
             log_steps=-1,
         )
         return tester
```

## sparseml/pytorch/models/classification/efficientnet.py

```diff
@@ -78,23 +78,20 @@
     def forward(self, a: Tensor, b: Tensor):
         if FloatFunctional:
             return self.functional.add(a, b)
         else:
             return torch.add(a, b)
 
 
-class QATSiLU(SiLU):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self.wrap_qat = True
-        self.qat_wrapper_kwargs = {
-            "num_inputs": 1,
-            "num_outputs": 1,
-        }
+class MulInput(Module):
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, x):
+        return x
 
 
 class _InvertedBottleneckBlock(Module):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
@@ -136,15 +133,15 @@
                         ),
                         (
                             "bn",
                             BatchNorm2d(num_features=expanded_channels, **bn_kwargs),
                         ),
                         (
                             "act",
-                            QATSiLU() if squeezed_channels else SiLU(),
+                            SiLU(),
                         ),
                     ]
                 )
             )
             if expanded_channels != in_channels
             else None
         )
@@ -164,15 +161,15 @@
                             groups=expanded_channels,
                             bias=False,
                         ),
                     ),
                     ("bn", BatchNorm2d(num_features=expanded_channels, **bn_kwargs)),
                     (
                         "act",
-                        QATSiLU() if squeezed_channels else SiLU(),
+                        SiLU(),
                     ),
                 ]
             )
         )
 
         if self._se_mod:
             self.se = (
@@ -183,14 +180,17 @@
         else:
             self.se = (
                 SqueezeExcite(expanded_channels, squeezed_channels, "silu")
                 if squeezed_channels
                 else None
             )
 
+        if self.se is not None:
+            self.mul_input = MulInput()
+
         self.project = Sequential(
             OrderedDict(
                 [
                     (
                         "conv",
                         Conv2d(
                             in_channels=expanded_channels,
@@ -214,19 +214,21 @@
 
         if self.expand is not None:
             out = self.expand(inp)
 
         out = self.spatial(out)
 
         if self.se is not None and not self._se_mod:
+            out = self.mul_input(out)
             out = out * self.se(out)
 
         out = self.project(out)
 
         if self.se is not None and self._se_mod:
+            out = self.mul_input(out)
             out = out * self.se(out)
 
         if self.add is not None:
             out = self.add(out, inp)
 
         return out
 
@@ -331,14 +333,15 @@
         super().__init__()
         self.conv = Conv2d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=1,
             bias=False,
         )
+
         if bn_kwargs is None:
             bn_kwargs = {}
         self.bn = BatchNorm2d(num_features=out_channels, **bn_kwargs)
         self.act = SiLU()
         self.pool = AdaptiveAvgPool2d(1)
         self.dropout = Dropout(p=dropout)
         self.fc = Linear(out_channels, classes)
```

## sparseml/pytorch/models/classification/resnet.py

```diff
@@ -136,34 +136,17 @@
         _init_batch_norm(self.bn)
 
     @staticmethod
     def required(in_channels: int, out_channels: int, stride: int) -> bool:
         return in_channels != out_channels or stride > 1
 
 
-class _AddReLU(Module):
-    """
-    Wrapper for the FloatFunctional class that enables QATWrapper used to
-    quantize the first input to the Add operation
-    """
-
-    def __init__(self, num_channels):
-        super().__init__()
-        if FloatFunctional:
-            self.functional = FloatFunctional()
-            self.wrap_qat = True
-            self.qat_wrapper_kwargs = {"num_inputs": 1, "num_outputs": 1}
-        else:
-            self.functional = ReLU(num_channels=num_channels, inplace=True)
-
-    def forward(self, x, y):
-        if isinstance(self.functional, FloatFunctional):
-            return self.functional.add_relu(x, y)
-        else:
-            return self.functional(x + y)
+class AddInput(Module):
+    def forward(self, x):
+        return x
 
 
 class _BasicBlock(Module):
     def __init__(self, in_channels: int, out_channels: int, stride: int = 1):
         super().__init__()
         self.conv1 = Conv2d(
             in_channels,
@@ -181,33 +164,34 @@
         self.bn2 = BatchNorm2d(out_channels)
         self.identity = (
             _IdentityModifier(in_channels, out_channels, stride)
             if _IdentityModifier.required(in_channels, out_channels, stride)
             else None
         )
 
-        # self.add_relu = _AddReLU(out_channels)
+        self.add_input_conv = AddInput()
+        self.add_input_identity = AddInput()
         if FloatFunctional:
             self.add_relu = FloatFunctional()
         else:
             self.add_relu = ReLU(num_channels=out_channels, inplace=True)
 
         self.initialize()
 
     def forward(self, inp: Tensor):
         out = self.conv1(inp)
         out = self.bn1(out)
         out = self.act1(out)
 
         out = self.conv2(out)
         out = self.bn2(out)
+        out = self.add_input_conv(out)
 
         identity_val = self.identity(inp) if self.identity is not None else inp
-        # out = self.add_relu(identity_val, out)
-        # return out
+        identity_val = self.add_input_identity(identity_val)
 
         if isinstance(self.add_relu, FloatFunctional):
             return self.add_relu.add_relu(identity_val, out)
         else:
             return self.add_relu(identity_val + out)
 
     def initialize(self):
@@ -246,15 +230,16 @@
         self.bn3 = BatchNorm2d(out_channels)
         self.identity = (
             _IdentityModifier(in_channels, out_channels, stride)
             if _IdentityModifier.required(in_channels, out_channels, stride)
             else None
         )
 
-        # self.add_relu = _AddReLU(out_channels)
+        self.add_input_conv = AddInput()
+        self.add_input_identity = AddInput()
         if FloatFunctional:
             self.add_relu = FloatFunctional()
         else:
             self.add_relu = ReLU(num_channels=out_channels, inplace=True)
 
         self.initialize()
 
@@ -265,19 +250,18 @@
 
         out = self.conv2(out)
         out = self.bn2(out)
         out = self.act2(out)
 
         out = self.conv3(out)
         out = self.bn3(out)
+        out = self.add_input_conv(out)
 
         identity_val = self.identity(inp) if self.identity is not None else inp
-
-        # out = self.add_relu(identity_val, out)
-        # return out
+        identity_val = self.add_input_identity(identity_val)
 
         if isinstance(self.add_relu, FloatFunctional):
             return self.add_relu.add_relu(identity_val, out)
         else:
             return self.add_relu(identity_val + out)
 
     def initialize(self):
@@ -311,28 +295,33 @@
 
         self.identity = (
             Conv2d(in_channels, out_channels, kernel_size=1, stride=stride, bias=False)
             if in_channels != out_channels or stride != 1
             else None
         )
 
+        self.add_input_conv = AddInput()
+        self.add_input_identity = AddInput()
+
         self.initialize()
 
     def forward(self, inp: Tensor):
         identity = inp
 
         out = self.bn1(inp)
         out = self.act1(out)
         if self.identity is not None:
             identity = self.identity(out)
+            identity = self.add_input_identity(identity)
         out = self.conv1(out)
 
         out = self.bn2(out)
         out = self.act2(out)
         out = self.conv2(out)
+        out = self.add_input_conv(out)
 
         out += identity
 
         return out
 
     def initialize(self):
         _init_conv(self.conv1)
@@ -373,33 +362,37 @@
         self.conv3 = Conv2d(proj_channels, out_channels, kernel_size=1, bias=False)
 
         self.identity = (
             Conv2d(in_channels, out_channels, kernel_size=1, stride=stride, bias=False)
             if in_channels != out_channels or stride != 1
             else None
         )
+        self.add_input_conv = AddInput()
+        self.add_input_identity = AddInput()
 
         self.initialize()
 
     def forward(self, inp: Tensor):
         identity = inp
 
         out = self.bn1(inp)
         out = self.act1(out)
         if self.identity is not None:
             identity = self.identity(out)
+            identity = self.add_input_identity(identity)
         out = self.conv1(out)
 
         out = self.bn2(out)
         out = self.act2(out)
         out = self.conv2(out)
 
         out = self.bn3(out)
         out = self.act3(out)
         out = self.conv3(out)
+        out = self.add_input_conv(out)
 
         out += identity
 
         return out
 
     def initialize(self):
         _init_batch_norm(self.bn1)
```

## sparseml/pytorch/models/detection/yolo_v3.py

```diff
@@ -174,15 +174,15 @@
         return out
 
     def initialize(self):
         _init_conv(self.conv)
 
         # smart bias initialization
         b = self.conv.bias.view(3, -1).detach()
-        b[:, 4] += math.log(8 / 640 ** 2)  # 8 objects per 640 image
+        b[:, 4] += math.log(8 / 640**2)  # 8 objects per 640 image
         b[:, 5:] += math.log(0.6 / (self.num_classes - 0.99))
         self.conv.bias = Parameter(b.view(-1), requires_grad=True)
 
 
 class YoloV3(Module):
     """
     Yolo v3 implementation matching standard Yolo v3 SPP configuration
```

## sparseml/pytorch/optim/manager.py

```diff
@@ -23,14 +23,15 @@
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 import torch
 from torch import Tensor
 from torch.nn import Module
 from torch.optim.optimizer import Optimizer
 
+from sparseml.analytics import sparseml_analytics
 from sparseml.optim import (
     BaseManager,
     add_framework_metadata,
     load_recipe_yaml_str,
     parse_recipe_variables,
     validate_metadata,
 )
@@ -299,14 +300,15 @@
         return manager
 
     def __init__(
         self,
         modifiers: List[ScheduledModifier],
         metadata: Optional[Dict[str, Any]] = None,
     ):
+        sparseml_analytics.send_event("python__pytorch__manager__init")
         super().__init__(modifiers=modifiers, metadata=metadata)
         self._initialize_epoch = 0
 
     def state_dict(self) -> Dict[str, Dict]:
         """
         :return: Dictionary to store any state variables for this manager.
             Includes all modifiers nested under this manager as sub keys in the dict.
@@ -471,15 +473,15 @@
 
         :param loggers: the logger manager to setup this manager with for logging
             important info and milestones to
         """
         super().initialize_loggers(loggers)
 
         for mod in self.iter_modifiers():
-            mod.initialize_loggers(loggers)
+            mod.initialize_loggers(self.loggers)
 
     def modify(
         self,
         module: Module,
         optimizer: Optimizer,
         steps_per_epoch: int,
         wrap_optim: Any = None,
```

## sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py

```diff
@@ -40,22 +40,27 @@
 _LOGGER = logging.getLogger(__name__)
 
 
 def kl_logsoftmax(
     x: Tensor, y: Tensor, temperature: Union[float, Tensor], dim: int = -1
 ) -> Tensor:
     number_items = x.numel() / y.size(dim)
+    if x.shape != y.shape:
+        raise ValueError(
+            "The teacher/student outputs must be of the same shape for distilation"
+            f" but got Tensors of size {x.shape} and {y.shape}"
+        )
     return (
         TF.kl_div(
             input=TF.log_softmax(x / temperature, dim=dim),
             target=TF.log_softmax(y / temperature, dim=dim),
             log_target=True,
             reduction="sum",
         )
-        * (temperature ** 2)
+        * (temperature**2)
         / number_items
     )
 
 
 def kldiv_loss(
     student_outputs,
     teacher_outputs,
```

## sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py

```diff
@@ -50,15 +50,15 @@
     "FisherInverseFast",
     "FisherInverseFastBlock",
     "FisherInverseFastPageSwap",
     "FisherInverseFastSmallBlocks",
 ]
 
 _LOGGER = logging.getLogger(__name__)
-BYTES_IN_MIB = 1024 ** 2
+BYTES_IN_MIB = 1024**2
 
 
 @PyTorchModifierYAML()
 class MFACPruningModifier(BaseGradualPruningModifier):
     """
     Gradually applies kernel sparsity to a given parameter or parameters from
     init_sparsity until final_sparsity is reached over a given amount of time
@@ -586,15 +586,15 @@
             fisher_block_size=self._fisher_block_size,
             num_pages=self._num_pages,
             available_devices=self._available_devices,
         )
         diag = h_inv.diag().to(non_pruned_weights.device)
 
         # compute global scores for non-pruned weights
-        global_scores = (non_pruned_weights ** 2) / (2.0 * diag)
+        global_scores = (non_pruned_weights**2) / (2.0 * diag)
         parameter_scores = []
         minimum_score = global_scores.min().item() - 1
 
         # map global scores to parameter weight shapes
         weights_idx = 0
         for idx, param in enumerate(self._params):
             indices = self._unpruned_idxs[idx]
@@ -1572,8 +1572,8 @@
 
 def _block_memory_size(block_size: int, element_size: int) -> int:
     """
     Calculate memory needed for H^-1 calculations of one block.
     """
     # B^2 * e_size - memory required for H^-1
     # 4*B * e_size - memory required for additional comp vectors
-    return (block_size ** 2 + 4 * block_size) * element_size
+    return (block_size**2 + 4 * block_size) * element_size
```

## sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py

```diff
@@ -11,18 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Modifier classes implementing the blockwise version of the Optimal Brain Surgeon
 pruning framework, optimized for small blocks. The algorithm is described in details
-in the Optimal BERT Surgeon paper https://arxiv.org/abs/2203.07259
+in the Optimal BERT Surgeon paper https://arxiv.org/abs/2203.07259.
+For more details check FAQ section at
+https://github.com/eldarkurtic/sparseml/tree/improve-obs-docs/research/optimal_BERT_surgeon_oBERT
 """
 import logging
 import math
+import os
 from typing import Any, Dict, List, Optional, Union
 
 import torch
 from torch import Tensor
 from torch.nn import Module, Parameter
 
 from sparseml.pytorch.sparsification.modifier import ModifierProp, PyTorchModifierYAML
@@ -30,15 +33,15 @@
     PruningMaskCreator,
     get_mask_creator_default,
 )
 from sparseml.pytorch.sparsification.pruning.modifier_pruning_base import (
     BaseGradualPruningModifier,
 )
 from sparseml.pytorch.sparsification.pruning.scorer import PruningParamsGradScorer
-from sparseml.pytorch.utils import GradSampler
+from sparseml.pytorch.utils import MEMORY_BOUNDED, GradSampler
 from sparseml.pytorch.utils.logger import BaseLogger
 from sparseml.utils import interpolate
 
 
 __all__ = [
     "OBSPruningModifier",
     "OBSPruningParamsScorer",
@@ -136,15 +139,15 @@
         params: Union[str, List[str]],
         leave_enabled: bool = True,
         inter_func: str = "cubic",
         global_sparsity: bool = True,
         mask_type: str = "unstructured",
         num_grads: int = 1024,
         damp: float = 1e-7,
-        fisher_block_size: int = 50,
+        fisher_block_size: int = 1,
         grad_sampler_kwargs: Optional[Dict[str, Any]] = None,
         num_recomputations: int = 1,
     ):
         super().__init__(
             params=params,
             init_sparsity=init_sparsity,
             final_sparsity=final_sparsity,
@@ -287,15 +290,14 @@
             super().check_mask_update(
                 module,
                 epoch,
                 steps_per_epoch,
                 recomputation_sparsity=recomputation_sparsity,
             )
 
-        torch.cuda.empty_cache()
         self._last_applied_sparsity = to_apply_sparsities
         if self._scorer._is_main_proc:
             self._scorer._enabled_grad_buffering = False
 
     def _get_mask_creator(
         self, param_names: List[str], params: List[Parameter]
     ) -> PruningMaskCreator:
@@ -355,14 +357,16 @@
         if self._mask_type not in self._supported_masks:
             raise ValueError(f"{self._mask_type} mask_type not supported")
 
         if self._mask_type == "block4" and self._fisher_block_size % 4 != 0:
             raise ValueError(
                 "fisher_block_size must be divisible by 4 for block4 pruning"
             )
+        if MEMORY_BOUNDED not in os.environ:
+            os.environ[MEMORY_BOUNDED] = "True"  # more safe for most users
 
 
 class OBSPruningParamsScorer(PruningParamsGradScorer):
     """
     Scores parameters using the equations introduced in the Optimal BERT Surgeon
     to solve for the optimal weight update in the Optimal Brain Surgeon (OBS)
     framework. Implements unstructured and semi-structured (block4) scoring and
@@ -379,15 +383,15 @@
         self,
         params: List[Parameter],
         num_grads: int,
         damp: float,
         fisher_block_size: int,
         mask_type: str,
     ):
-        super().__init__(params)
+        super().__init__(params, dist_backend="nccl")
         self._num_grads = num_grads
         self._damp = damp
         self._fisher_block_size = fisher_block_size
         self._mask_type = mask_type
 
         self._finvs = None  # type: List[EmpiricalBlockFisherInverse]
         self._enabled_grad_buffering = False
@@ -425,19 +429,21 @@
         scores = [None] * len(self._params)
         block_finv_w = [None] * len(self._params)
 
         if self._is_main_proc:
             for i, finv in enumerate(self._finvs):
                 if self._mask_type == "unstructured":
                     scores[i] = (
-                        (self._params[i].data.view(-1) ** 2).to(self._devices[i])
+                        (self._params[i].data.reshape(-1) ** 2).to(self._devices[i])
                         / (2.0 * finv.diag() + self._eps)
-                    ).view(self._params[i].shape)
+                    ).reshape(self._params[i].shape)
                 else:  # self._mask_type == "block4":
-                    block_w = self._params[i].data.view(-1, 4).to(finv.dev)  # (d/Q, Q)
+                    block_w = (
+                        self._params[i].data.reshape(-1, 4).to(finv.dev)
+                    )  # (d/Q, Q)
                     block_finv = (
                         torch.cat(
                             [
                                 finv.f_inv[:, i : i + 4, i : i + 4]
                                 for i in range(0, finv.B, 4)
                             ],
                             dim=1,
@@ -482,15 +488,15 @@
             return
 
         if self._finvs is None:
             self._setup_fisher_inverse(masks)
 
         for i, finv in enumerate(self._finvs):
             self._params[i].grad.mul_(masks[i])
-            finv.add_grad(self._params[i].grad.view(-1).to(self._devices[i]))
+            finv.add_grad(self._params[i].grad.reshape(-1).to(self._devices[i]))
 
     @torch.no_grad()
     def mask_update(self, masks: List[Tensor], mask_diffs: List[Tensor]):
         """
         Apply OBS weight update which zeros-out pruned weights and updates the
         remaining weights to preserve the loss.
 
@@ -502,28 +508,28 @@
         if self._is_main_proc:
             for i, param in enumerate(self._params):
                 if self._mask_type == "unstructured":
                     obs_updates[i] = (
                         self._finvs[i]
                         .mul(
                             (param.data * (mask_diffs[i] == -1))
-                            .view(-1)
+                            .reshape(-1)
                             .to(self._devices[i])
                             / (self._finvs[i].diag() + self._eps)
                         )
-                        .view(param.data.shape)
+                        .reshape(param.data.shape)
                     )
                 else:  # self._mask_type == "block4":
                     obs_updates[i] = (
                         self._finvs[i]
                         .mul(
-                            self._block_finv_w[i].view(-1)
-                            * (mask_diffs[i] == -1).view(-1).to(self._devices[i])
+                            self._block_finv_w[i].reshape(-1)
+                            * (mask_diffs[i] == -1).reshape(-1).to(self._devices[i])
                         )
-                        .view(param.data.shape)
+                        .reshape(param.data.shape)
                     )
 
         self._broadcast_list_from_main(obs_updates)
         # apply OBS update and manually zero-out pruned weights
         for i, param in enumerate(self._params):
             param.data -= obs_updates[i].to(param.data.device)
             param.data[mask_diffs[i] == -1] = 0.0
@@ -584,15 +590,15 @@
         # if 'd / B' is not integer, pad with zeros for batch calculations
         if g.numel() < self.num_blocks * self.B:
             g = torch.cat(
                 [g, torch.zeros(self.num_blocks * self.B - g.numel(), device=g.device)]
             )
 
         # prepare grad for batch calculations
-        g = g.view(self.num_blocks, self.B)
+        g = g.reshape(self.num_blocks, self.B)
 
         # batched f_inv x g: (batch, B, B) x (batch, B) -> (batch, B)
         finv_g = torch.einsum("bij,bj->bi", self.f_inv, g)
 
         # scalar denominator for each batch: (batch)
         alpha = (self.m + torch.einsum("bi,bi->b", g, finv_g)).sqrt().unsqueeze(1)
         finv_g /= alpha
@@ -613,9 +619,9 @@
         :return: result of the matrix-vector multiplication
         """
         if v.numel() < self.num_blocks * self.B:
             v = torch.cat(
                 [v, torch.zeros(self.num_blocks * self.B - v.numel(), device=v.device)]
             )
         return torch.bmm(
-            self.f_inv, v.view(self.num_blocks, self.B).unsqueeze_(2)
+            self.f_inv, v.reshape(self.num_blocks, self.B).unsqueeze_(2)
         ).flatten()[: self.d]
```

## sparseml/pytorch/sparsification/pruning/scorer.py

```diff
@@ -14,14 +14,15 @@
 
 """
 Classes for tracking and scoring model parameters to generate pruning scores
 """
 
 
 from abc import ABC, abstractmethod
+from datetime import timedelta
 from typing import Any, Dict, List, Optional
 
 import torch.distributed as dist
 from torch import Tensor
 from torch.nn import Parameter
 
 
@@ -108,15 +109,15 @@
         super().__init__(params=params)
 
         self._is_ddp = dist.is_initialized()
         self._is_main_proc = not self._is_ddp or dist.get_rank() == 0
 
         # create group to broadcast gradients across processes
         self._dist_group = (
-            dist.new_group(backend=dist_backend)
+            dist.new_group(backend=dist_backend, timeout=timedelta(seconds=7200))
             if self._is_ddp and dist_backend is not None
             else None
         )
 
         self._pickle_exclude_params = ["_is_ddp", "_is_main_proc", "_dist_group"]
 
     def __getstate__(self) -> Dict[str, Any]:
```

## sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py

```diff
@@ -500,14 +500,16 @@
         super().initialize(module, epoch, loggers, **kwargs)
         self._modules_to_quantize = []
         self._calibration_dataloader = calibration_dataloader
         self._calibration_function = calibration_function
         if self._submodules is not None:
             found_submodules = []
             for name, submodule in module.named_modules():
+                if name.startswith("module."):
+                    name = name[7:]
                 if name in self._submodules:
                     self._modules_to_quantize.append(_ModuleToQuantize(name, submodule))
                     found_submodules.append(name)
             if not len(found_submodules) == len(self._submodules):
                 raise RuntimeError(
                     "Could not find all provided submodules to quantize"
                     "given: {}, found: {}".format(
```

## sparseml/pytorch/sparsification/quantization/quantization_scheme.py

```diff
@@ -265,15 +265,15 @@
     bits = bits if bits else 8
     is_custom = bits != 8
     if dtype == torch.qint8:
         quant_min = -(2 ** (bits - 1))
         quant_max = (2 ** (bits - 1)) - 1
     elif dtype == torch.quint8:
         quant_min = 0
-        quant_max = (2 ** bits) - 1
+        quant_max = (2**bits) - 1
 
     return quant_min, quant_max, is_custom
 
 
 def get_observer(
     symmetric: bool,
     dtype: torch.dtype,
```

## sparseml/pytorch/sparsification/quantization/quantize.py

```diff
@@ -229,15 +229,19 @@
     (1.9+) includes its own logic for propagating including overriding set qconfigs
     for certain activations without the ability to disable this behavior
 
     :param module: module to add output activation observers to
     """
     # adapted from torch/ao/quantization/quantize.py::_add_observer_
     # source: https://github.com/pytorch/pytorch/blob/v1.13.0/torch/ao/quantization/quantize.py#L135  # noqa: E501
-    device = next(module.parameters()).device
+    try:
+        device = next(module.parameters()).device
+    except StopIteration:
+        # default to CPU if module has no parameters
+        device = "cpu"
 
     def _needs_observer(target_module: Module):
         # combines logic from multiple places of original implementation which
         # mostly checked for existnace of a qconfig and if the target was a leaf
         # module
         if not hasattr(target_module, "quantization_scheme") or isinstance(
             target_module, torch_quantization.QuantWrapper
```

## sparseml/pytorch/sparsification/quantization/quantize_qat_export.py

```diff
@@ -1569,14 +1569,15 @@
         model = deepcopy(model)
 
     _convert_single_constants_to_initializers(model)
     _fold_qat_conv_bns(model)
     _delete_repeated_qat_blocks(model)
     _quantize_qat_embedding(model)
     _propagate_mobilebert_embedding_quantization(model)
+    _propagate_through_split(model)
     _convert_quantizable_matmul(model)
     _convert_quantizable_matmul_and_add(model)
     _fold_relu_quants(model)
 
     # only convert to either ConvInteger or QLinearConv (legacy)
     if not use_qlinearconv:
         _convert_quantizable_conv_integer(model)
@@ -1832,7 +1833,82 @@
 
     graph.delete_unused_initializers()
 
     if converted_nodes > 0:
         _LOGGER.info(
             f"Propagated {converted_nodes} DequantizeLinear node(s) through Concat"
         )
+
+
+def _propagate_through_split(model: ModelProto):
+    """
+    A pass for propagating dequantization down through a split node
+    so if there are quantized operations after the split they can
+    be properly converted
+
+    Starting with:
+    |         INPUT
+    |              |
+    |       DequantizeLinear
+    |             |
+    |           Split
+    |         |   |   |
+
+    Converts to:
+    |                     INPUT
+    |                         |
+    |                       Split
+    |                |         |           |
+    | DequantizeLinear  DequantizeLinear  DequantizeLinear
+    |         |                |                |
+    """
+    new_nodes = []
+    to_remove = []
+    split_nodes = [n for n in model.graph.node if n.op_type in ["Split"]]
+    graph = ONNXGraph(model)
+    for split_node in split_nodes:
+        dequant_node = graph.get_node_single_parent(split_node, 0)
+        if not dequant_node or dequant_node.op_type != "DequantizeLinear":
+            continue
+
+        # Make input to dequantize linear node input to split node
+        split_node.input[0] = dequant_node.input[0]
+
+        # For every output of split create a dequantize linear node
+        dequant_id = 0
+        for other_node in get_node_output_nodes(model, split_node):
+            split_node_output = []
+            for out in split_node.output:
+                if out in other_node.input:
+                    split_node_output.append(out)
+            for out in split_node_output:
+                dequant_node_name = split_node.name + f"_dequant.{dequant_id}"
+                dequant_id += 1
+                dequant_node_output = dequant_node_name + "_output"
+                new_nodes.append(
+                    onnx.helper.make_node(
+                        "DequantizeLinear",
+                        [
+                            out,  # input
+                            dequant_node.input[1],  # scale
+                            dequant_node.input[2],  # zero point
+                        ],
+                        [dequant_node_output],
+                        dequant_node_name,
+                    )
+                )
+                for other_node_input_index, other_node_input in enumerate(
+                    other_node.input
+                ):
+                    if other_node_input == out:
+                        break
+                other_node.input[other_node_input_index] = dequant_node_output
+        to_remove.append(dequant_node)
+
+    model.graph.node.extend(new_nodes)
+    for node in to_remove:
+        model.graph.node.remove(node)
+
+    if len(to_remove) > 0:
+        _LOGGER.info(
+            f"Propagated {len(to_remove)} DequantizeLinear node(s) through Split"
+        )
```

## sparseml/pytorch/sparsification/training/__init__.py

```diff
@@ -11,10 +11,11 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .modifier_epoch import *
+from .modifier_logging import *
 from .modifier_lr import *
 from .modifier_params import *
 from .modifier_regularizer import *
```

## sparseml/pytorch/torchvision/__init__.py

```diff
@@ -7,7 +7,19 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from sparseml.analytics import sparseml_analytics as _analytics
+
+
+try:
+    import cv2 as _cv2  # noqa: F401
+    import torchvision as _torchvision  # noqa: F401
+except ImportError:
+    raise ImportError("Please install sparseml[torchvision] to use this pathway")
+
+
+_analytics.send_event("python__pytorch__torchvision__init")
```

## sparseml/pytorch/torchvision/train.py

```diff
@@ -36,24 +36,25 @@
 import click
 from sparseml.optim.helpers import load_recipe_yaml_str
 from sparseml.pytorch.models.registry import ModelRegistry
 from sparseml.pytorch.optim import ScheduledModifierManager
 from sparseml.pytorch.torchvision import presets, transforms, utils
 from sparseml.pytorch.torchvision.sampler import RASampler
 from sparseml.pytorch.utils.helpers import (
+    default_device,
     download_framework_model_by_recipe_type,
     torch_distributed_zero_first,
 )
 from sparseml.pytorch.utils.logger import (
     LoggerManager,
     PythonLogger,
     TensorBoardLogger,
     WANDBLogger,
 )
-from sparseml.pytorch.utils.model import load_model
+from sparseml.pytorch.utils.model import load_model, model_to_device
 from sparsezoo import Model
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def train_one_epoch(
@@ -175,15 +176,15 @@
     log_suffix="",
 ) -> utils.MetricLogger:
     model.eval()
     metric_logger = utils.MetricLogger(_LOGGER, delimiter="  ")
     header = f"Test: {log_suffix}"
 
     num_processed_samples = 0
-    with torch.inference_mode():
+    with torch.no_grad():
         for image, target in metric_logger.log_every(data_loader, print_freq, header):
             image = image.to(device, non_blocking=True)
             target = target.to(device, non_blocking=True)
             output = model(image)
             if isinstance(output, tuple):
                 output = output[0]
             loss = criterion(output, target)
@@ -328,15 +329,18 @@
 
     utils.init_distributed_mode(args)
     if not utils.is_main_process():
         _LOGGER.disabled = True
 
     _LOGGER.info(args)
 
-    device = torch.device(args.device)
+    if not args.device:
+        args.device = default_device()
+
+    device = args.device
 
     if args.use_deterministic_algorithms:
         torch.backends.cudnn.benchmark = False
         torch.use_deterministic_algorithms(True)
     else:
         torch.backends.cudnn.benchmark = True
 
@@ -378,37 +382,38 @@
         sampler=test_sampler,
         num_workers=args.workers,
         pin_memory=True,
     )
 
     _LOGGER.info("Creating model")
     local_rank = args.rank if args.distributed else None
-    model, arch_key = _create_model(
+    model, arch_key, maybe_dp_device = _create_model(
         arch_key=args.arch_key,
         local_rank=local_rank,
         pretrained=args.pretrained,
         checkpoint_path=args.checkpoint_path,
         pretrained_dataset=args.pretrained_dataset,
         device=device,
         num_classes=num_classes,
     )
 
     if args.distill_teacher not in ["self", "disable", None]:
         _LOGGER.info("Instantiating teacher")
-        distill_teacher, _ = _create_model(
+        distill_teacher, _, _ = _create_model(
             arch_key=args.teacher_arch_key,
             local_rank=local_rank,
             pretrained=True,  # teacher is always pretrained
             pretrained_dataset=args.pretrained_teacher_dataset,
             checkpoint_path=args.distill_teacher,
             device=device,
             num_classes=num_classes,
         )
     else:
         distill_teacher = args.distill_teacher
+    device = maybe_dp_device
 
     if args.distributed and args.sync_bn:
         model = torch.nn.SyncBatchNorm.convert_sync_batchnorm(model)
 
     if version.parse(torch.__version__) >= version.parse("1.10"):
         criterion = nn.CrossEntropyLoss(label_smoothing=args.label_smoothing)
     elif args.label_smoothing > 0:
@@ -707,15 +712,15 @@
                     else epoch + checkpoint_manager.max_epochs
                 )
                 checkpoint["recipe"] = str(
                     ScheduledModifierManager.compose_staged(checkpoint_manager, manager)
                 )
             else:
                 checkpoint["epoch"] = -1 if epoch == max_epochs - 1 else epoch
-                if str(manager) is not None:
+                if manager is not None:
                     checkpoint["recipe"] = str(manager)
 
             file_names = ["checkpoint.pth"]
             if is_new_best:
                 file_names.append("checkpoint-best.pth")
             _save_checkpoints(
                 epoch,
@@ -787,16 +792,16 @@
                     "classifier.bias",
                 ],
             )
     else:
         raise ValueError(
             f"Unable to find {arch_key} in ModelRegistry or in torchvision.models"
         )
-    model.to(device)
-    return model, arch_key
+    model, device, _ = model_to_device(model=model, device=device)
+    return model, arch_key, device
 
 
 def _get_lr_scheduler(args, optimizer, checkpoint=None, manager=None):
     lr_scheduler = None
 
     if manager is not None and manager.learning_rate_modifiers:
         lr_scheduler = None
@@ -946,17 +951,19 @@
         "The dataset to load pretrained weights for if pretrained is "
         "set. Load the default dataset for the architecture if set to None. "
         "examples:`imagenet`, `cifar10`, etc..."
     ),
 )
 @click.option(
     "--device",
-    default="cuda",
+    default=None,
     type=str,
-    help="device (Use cuda or cpu)",
+    help=(
+        "device (Use cuda for all gpus, else use `cuda:device_id,device_id` " "or cpu)"
+    ),
 )
 @click.option(
     "-b",
     "--batch-size",
     default=32,
     type=int,
     help="images per gpu, the total batch size is $NGPU x batch_size",
```

## sparseml/pytorch/utils/__init__.py

```diff
@@ -19,14 +19,15 @@
 # flake8: noqa
 
 from ..base import check_torch_install as _check_torch_install
 from .benchmarker import *
 from .distributed import *
 from .exporter import *
 from .helpers import *
+from .log_sparsification_info import *
 from .logger import *
 from .loss import *
 from .model import *
 from .module import *
 from .sparsification import *
 from .ssd_helpers import *
 from .yolo_helpers import *
```

## sparseml/pytorch/utils/exporter.py

```diff
@@ -244,49 +244,55 @@
         create_parent_dirs(path)
         if sample_batch:
             trace_model(path, self._module, sample_batch)
         else:
             script_model(path, self._module)
 
     def create_deployment_folder(
-        self, labels_to_class_mapping: Optional[Union[str, Dict[int, str]]] = None
-    ):
+        self,
+        labels_to_class_mapping: Optional[Union[str, Dict[int, str]]] = None,
+        onnx_model_name: Optional[str] = None,
+    ) -> str:
         """
         Create a deployment folder inside the `self._output_dir` directory.
 
         :param labels_to_class_mapping: information about the mapping
             from integer labels to string class names.
             Can be either a string (path to the .json serialized dictionary)
             or a dictionary. Default is None
+        :param onnx_model_name: name of the onnx model file. Defaults to `model.onnx`
+        :return path to the deployment folder
         """
         deployment_folder_dir = os.path.join(self._output_dir, "deployment")
 
         if os.path.isdir(deployment_folder_dir):
             shutil.rmtree(deployment_folder_dir)
         os.makedirs(deployment_folder_dir)
         _LOGGER.info(f"Created deployment folder at {deployment_folder_dir}")
 
         # copy over model onnx
-        expected_onnx_model_dir = os.path.join(self._output_dir, MODEL_ONNX_NAME)
-        deployment_onnx_model_dir = os.path.join(deployment_folder_dir, MODEL_ONNX_NAME)
+        onnx_model_name = onnx_model_name or MODEL_ONNX_NAME
+        expected_onnx_model_dir = os.path.join(self._output_dir, onnx_model_name)
+        deployment_onnx_model_dir = os.path.join(deployment_folder_dir, onnx_model_name)
         _copy_file(src=expected_onnx_model_dir, target=deployment_onnx_model_dir)
         _LOGGER.info(
-            f"Saved {MODEL_ONNX_NAME} in the deployment "
+            f"Saved {onnx_model_name} in the deployment "
             f"folder at {deployment_onnx_model_dir}"
         )
 
         # create config.json
         config_file_path = _create_config_file(save_dir=deployment_folder_dir)
 
         if labels_to_class_mapping:
             # append `labels_to_class_mapping` info to config.json
             _save_label_to_class_mapping(
                 labels_to_class_mapping=labels_to_class_mapping,
                 config_file_path=config_file_path,
             )
+        return deployment_folder_dir
 
     def export_pytorch(
         self,
         optimizer: Optional[Optimizer] = None,
         recipe: Optional[str] = None,
         epoch: Optional[int] = None,
         name: str = "model.pth",
```

## sparseml/pytorch/utils/helpers.py

```diff
@@ -96,14 +96,15 @@
     "get_layer_param",
     "set_deterministic_seeds",
     "torch_distributed_zero_first",
     "thin_model_from_checkpoint",
     "MEMORY_BOUNDED",
     "memory_aware_threshold",
     "download_framework_model_by_recipe_type",
+    "detach",
 ]
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 ##############################
@@ -1114,17 +1115,17 @@
     :return: k-th smallest value from the given tensor, where k=idx+1
     """
     try:
         if (
             MEMORY_BOUNDED in os.environ
             and os.environ[MEMORY_BOUNDED].lower() == "true"
         ):
-            return torch.kthvalue(tensor.view(-1), idx + 1)[0]
+            return torch.kthvalue(tensor.reshape(-1), idx + 1)[0]
         else:
-            return torch.sort(tensor.view(-1))[0][idx]
+            return torch.sort(tensor.reshape(-1))[0][idx]
     except RuntimeError:
         _LOGGER.warning(
             "Finding threshold from sparsity failed due to lack of memory, "
             "will attempt to recover. Consider setting env variable "
             f"{MEMORY_BOUNDED}=True in future runs."
         )
         torch.cuda.empty_cache()
@@ -1158,7 +1159,18 @@
 
     if framework_model is None:
         # fetching the model for inference or fall back if model.ckpt.pth doesn't exist
         model_name = f"model.{model_suffix}"
         framework_model = zoo_model.training.default.get_file(model_name)
 
     return framework_model.path
+
+
+def detach(x: Union[torch.Tensor, List, Tuple]):
+    if isinstance(x, torch.Tensor):
+        return x.detach()
+    elif isinstance(x, List):
+        return [detach(e) for e in x]
+    elif isinstance(x, Tuple):
+        return tuple([detach(e) for e in x])
+    else:
+        raise ValueError("Unexpected type to detach")
```

## sparseml/pytorch/utils/logger.py

```diff
@@ -44,17 +44,14 @@
 except Exception as err:
     wandb = None
     wandb_err = err
 
 from sparseml.utils import ALL_TOKEN, create_dirs
 
 
-_LOGGER = logging.getLogger(__name__)
-
-
 __all__ = [
     "BaseLogger",
     "LambdaLogger",
     "PythonLogger",
     "TensorBoardLogger",
     "WANDBLogger",
     "SparsificationGroupLogger",
@@ -327,42 +324,16 @@
     def __init__(
         self,
         logger: Logger = None,
         log_level: int = None,
         name: str = "python",
         enabled: bool = True,
     ):
-        if logger:
-            self._logger = logger
-        else:
-            self._logger = logging.getLogger(__name__)
-
-            base_log_path = (
-                os.environ.get("NM_TEST_LOG_DIR")
-                if os.environ.get("NM_TEST_MODE")
-                else "sparse_logs"
-            )
-            now = datetime.now()
-            dt_string = now.strftime("%d-%m-%Y_%H.%M.%S")
-            log_path = os.path.join(base_log_path, f"{dt_string}.log")
-            os.makedirs(base_log_path, exist_ok=True)
+        self._logger = logger or self._create_default_logger(log_level=log_level)
 
-            _LOGGER.info(f"Logging all SparseML modifier-level logs to {log_path}")
-
-            handler = logging.FileHandler(
-                log_path,
-                delay=True,
-            )
-            self._logger.addHandler(handler)
-            self._logger.propagate = False
-
-        if log_level is None:
-            log_level = logging.getLogger("sparseml").level
-        self.logger.setLevel(log_level)
-        self._log_level = log_level
         super().__init__(
             lambda_func=self._log_lambda,
             name=name,
             enabled=enabled,
         )
 
     def __getattr__(self, item):
@@ -371,14 +342,58 @@
     @property
     def logger(self) -> Logger:
         """
         :return: a logger instance to log to, if None then will create it's own
         """
         return self._logger
 
+    def _create_default_logger(self, log_level: Optional[int] = None) -> logging.Logger:
+        """
+        Create a default modifier logger, with a file handler logging at the debug level
+        and a stream handler logging to console at the specified level
+
+        :param log_level: logging level for the console logger
+        :return: logger
+        """
+        logger = logging.getLogger(__name__)
+
+        # File handler setup, for logging modifier debug statements
+        if not any(
+            isinstance(handler, logging.FileHandler) for handler in logger.handlers
+        ):
+            base_log_path = (
+                os.environ.get("NM_TEST_LOG_DIR")
+                if os.environ.get("NM_TEST_MODE")
+                else "sparse_logs"
+            )
+            now = datetime.now()
+            dt_string = now.strftime("%d-%m-%Y_%H.%M.%S")
+            log_path = os.path.join(base_log_path, f"{dt_string}.log")
+            os.makedirs(base_log_path, exist_ok=True)
+            file_handler = logging.FileHandler(
+                log_path,
+                delay=True,
+            )
+            file_handler.setLevel(LOGGING_LEVELS["debug"])
+            logger.addHandler(file_handler)
+            logger.info(f"Logging all SparseML modifier-level logs to {log_path}")
+
+        if not any(
+            isinstance(handler, logging.StreamHandler) for handler in logger.handlers
+        ):
+            # Console handler, for logging high level modifier logs
+            stream_handler = logging.StreamHandler()
+            stream_handler.setLevel(log_level or logging.getLogger("sparseml").level)
+            logger.addHandler(stream_handler)
+
+        logger.setLevel(LOGGING_LEVELS["debug"])
+        logger.propagate = False
+
+        return logger
+
     def _log_lambda(
         self,
         tag: Optional[str],
         value: Optional[Union[float, str]],
         values: Optional[Dict[str, float]],
         step: Optional[int],
         wall_time: Optional[float],
```

## sparseml/pytorch/utils/sparsification.py

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """
 Helper functions for retrieving information related to model sparsification
 """
 
 import json
+import logging
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     Iterable,
     Iterator,
@@ -42,14 +43,16 @@
 
 
 __all__ = [
     "ModuleSparsificationInfo",
     "GradSampler",
 ]
 
+_LOGGER = logging.getLogger(__name__)
+
 
 class ModuleSparsificationInfo:
     """
     Helper class for providing information related to torch Module parameters
     and the amount of sparsification applied. Includes information for pruning
     and quantization
 
@@ -250,8 +253,15 @@
                     # yield so gradients can be collected
                     computed_grads += 1
                     yield computed_grads
                     if progress_bar:
                         pbar.update(1)
                     if computed_grads >= num_grads:
                         break
+                if computed_grads < num_grads:
+                    _LOGGER.warning(
+                        f"The requested num_grads:{num_grads} is greater than allowed by the dataset. \
+                        Proceeding with less than requested. \
+                        Please reduce num_grads to suppress the warning."
+                    )
+                    break
         module.zero_grad()
```

## sparseml/tensorflow_v1/__init__.py

```diff
@@ -14,10 +14,15 @@
 
 """
 Functionality for working with and sparsifying Models in the TensorFlow 1.x framework
 """
 
 # flake8: noqa
 
+from sparseml.analytics import sparseml_analytics as _analytics
+
 from .base import *
 from .framework import detect_framework, framework_info, is_supported
 from .sparsification import sparsification_info
+
+
+_analytics.send_event("python__tensorflow_v1__init")
```

## sparseml/transformers/__init__.py

```diff
@@ -16,116 +16,35 @@
 Tools for integrating SparseML with transformers training flows
 """
 
 # flake8: noqa
 
 import logging as _logging
 
-import pkg_resources
+from sparseml.analytics import sparseml_analytics as _analytics
 
 
-_EXPECTED_VERSION = "4.23.1"
+try:
+    import datasets as _datasets
+    import transformers as _transformers
+except ImportError:
+    raise ImportError("Please install sparseml[transformers] to use this pathway")
 
 
-_LOGGER = _logging.getLogger(__name__)
-_NM_TRANSFORMERS_TAR_TEMPLATE = (
-    "https://github.com/neuralmagic/transformers/releases/download/"
-    "{version}/transformers-4.23.1-py3-none-any.whl"
-)
-_NM_TRANSFORMERS_NIGHTLY = _NM_TRANSFORMERS_TAR_TEMPLATE.format(version="nightly")
-
-
-def _install_transformers_and_deps():
-
-    import subprocess as _subprocess
-    import sys as _sys
-
-    import sparseml as _sparseml
-
-    nm_transformers_release = (
-        "nightly" if not _sparseml.is_release else f"v{_sparseml.version_major_minor}"
-    )
-    transformers_requirement = _NM_TRANSFORMERS_TAR_TEMPLATE.format(
-        version=nm_transformers_release
-    )
-    try:
-        _subprocess.check_call(
-            [
-                _sys.executable,
-                "-m",
-                "pip",
-                "install",
-                transformers_requirement,
-                "datasets<=1.18.4",
-                "scikit-learn",
-                "seqeval",
-            ]
-        )
+_analytics.send_event("python__transformers__init")
 
-        import transformers as _transformers
 
-        _LOGGER.info("sparseml-transformers and dependencies successfully installed")
-    except Exception:
-        raise ValueError(
-            "Unable to install and import sparseml-transformers dependencies check "
-            "that transformers is installed, if not, install via "
-            f"`pip install {_NM_TRANSFORMERS_NIGHTLY}`"
-        )
+_LOGGER = _logging.getLogger(__name__)
 
 
 def _check_transformers_install():
-    transformers_version = next(
-        (
-            pkg.version
-            for pkg in pkg_resources.working_set
-            if pkg.project_name.lower() == "transformers"
-        ),
-        None,
-    )
-
-    # Either no transformers install is found or wrong version installed
-    if transformers_version != _EXPECTED_VERSION:
-        import os
-
-        if os.getenv("NM_NO_AUTOINSTALL_TRANSFORMERS", False):
-            _LOGGER.warning(
-                "Unable to import, skipping auto installation "
-                "due to NM_NO_AUTOINSTALL_TRANSFORMERS"
-            )
-            # skip any further checks
-            return
-        else:
-            _LOGGER.warning(
-                f"sparseml-transformers v{_EXPECTED_VERSION} installation not "
-                f"detected. Installing  sparseml-transformers v{_EXPECTED_VERSION} "
-                "dependencies if transformers is already  installed in the "
-                "environment, it will be overwritten. Set  environment variable "
-                "NM_NO_AUTOINSTALL_TRANSFORMERS to disable"
-            )
-            _install_transformers_and_deps()
-
-    else:
-        import transformers as _transformers
-
-        # Edge case where user has expected version of transformers installed, but
-        # not the nm integrated one
-        if not _transformers.NM_INTEGRATED:
-            _install_transformers_and_deps()
-            raise RuntimeError(
-                "Installed transformers package has been overwritten with "
-                "sparseml-transformers. Stopping process as this is likely to cause "
-                "import issues. Please re-run command"
-            )
-
-    # re check import after potential install
-    try:
-        import transformers as _transformers
+    # check for NM integration in transformers version
+    import transformers as _transformers
 
-        assert _transformers.NM_INTEGRATED
-    except Exception:
+    if not _transformers.NM_INTEGRATED:
         _LOGGER.warning(
             "the neuralmagic fork of transformers may not be installed. it can be "
             "installed via "
             f"`pip install {_NM_TRANSFORMERS_NIGHTLY}`"
         )
```

## sparseml/transformers/masked_language_modeling.py

```diff
@@ -47,33 +47,28 @@
     AutoConfig,
     AutoTokenizer,
     DataCollatorForLanguageModeling,
     HfArgumentParser,
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
-from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 
 from sparseml.pytorch.utils.distributed import record
 from sparseml.transformers.sparsification import Trainer, TrainingArguments
 from sparseml.transformers.utils import SparseAutoModel, get_shared_tokenizer_src
 
 
 metadata_args = [
     "per_device_train_batch_size",
     "per_device_eval_batch_size",
     "fp16",
 ]
 
 
-# Will error if the minimal version of Transformers is not installed.
-# Remove at your own risks
-check_min_version("4.18.0.dev0")
-
 require_version(
     "datasets>=1.18.0",
     "To fix: pip install -r examples/pytorch/language-modeling/requirements.txt",
 )
 
 _LOGGER = logging.getLogger(__name__)
 MODEL_CONFIG_CLASSES = list(MODEL_FOR_MASKED_LM_MAPPING.keys())
```

## sparseml/transformers/question_answering.py

```diff
@@ -41,30 +41,25 @@
     EvalPrediction,
     HfArgumentParser,
     PreTrainedTokenizerFast,
     default_data_collator,
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
-from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 
 from sparseml.pytorch.utils.distributed import record
 from sparseml.transformers.sparsification import (
     QuestionAnsweringTrainer,
     TrainingArguments,
     postprocess_qa_predictions,
 )
 from sparseml.transformers.utils import SparseAutoModel, get_shared_tokenizer_src
 
 
-# Will error if the minimal version of Transformers is not installed. Remove at your
-# own risks.
-check_min_version("4.18.0.dev0")
-
 require_version(
     "datasets>=1.18.0",
     "To fix: pip install -r examples/pytorch/question-answering/requirements.txt",
 )
 
 
 _LOGGER = logging.getLogger(__name__)
```

## sparseml/transformers/text_classification.py

```diff
@@ -45,30 +45,25 @@
     EvalPrediction,
     HfArgumentParser,
     PretrainedConfig,
     default_data_collator,
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
-from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 
 from sparseml.pytorch.utils.distributed import record
 from sparseml.transformers.sparsification import Trainer, TrainingArguments
 from sparseml.transformers.utils import (
     SparseAutoModel,
     get_shared_tokenizer_src,
     multi_label_precision_recall_f1,
 )
 
 
-# Will error if the minimal version of Transformers is not installed.
-# Remove at your own risks.
-check_min_version("4.18.0.dev0")
-
 require_version(
     "datasets>=1.18.0",
     "To fix: pip install -r examples/pytorch/text-classification/requirements.txt",
 )
 
 _TASK_TO_KEYS = {
     "cola": ("sentence", None),
```

## sparseml/transformers/token_classification.py

```diff
@@ -44,26 +44,21 @@
     DataCollatorForTokenClassification,
     HfArgumentParser,
     PretrainedConfig,
     PreTrainedTokenizerFast,
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
-from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 
 from sparseml.pytorch.utils.distributed import record
 from sparseml.transformers.sparsification import Trainer, TrainingArguments
 from sparseml.transformers.utils import SparseAutoModel, get_shared_tokenizer_src
 
 
-# Will error if the minimal version of Transformers is not installed.
-# Remove at your own risks
-check_min_version("4.18.0.dev0")
-
 require_version(
     "datasets>=1.18.0",
     "To fix: pip install -r examples/pytorch/token-classification/requirements.txt",
 )
 
 _LOGGER: logging.Logger = logging.getLogger(__name__)
```

## sparseml/transformers/sparsification/trainer.py

```diff
@@ -201,15 +201,21 @@
             if not self.one_shot:
                 self.manager.apply_structure(self.model, epoch=epoch)
                 _LOGGER.info(
                     "Applied structure from SparseML recipe argument to model at "
                     f"epoch {epoch}"
                 )
             else:
-                self.manager.apply(self.model)
+                self.manager.apply(
+                    self.model,
+                    grad_sampler={
+                        "data_loader_builder": self._data_loader_builder,
+                        "loss_function": self._loss_function,
+                    },
+                )
                 self.manager_applied = True
                 _LOGGER.info(f"Applied one shot recipe {self.recipe} to the manager")
                 return True
 
         # reload the state dict for the model now that architecture matches expected
         load_path = checkpoint or self.model_state_path
         self._reload_model_state(load_path, orig_state_dict)
```

## sparseml/yolact/__init__.py

```diff
@@ -16,14 +16,18 @@
 Tools for integrating SparseML with yolact training flows
 """
 
 import importlib
 import logging as _logging
 from collections import namedtuple
 
+from sparseml.analytics import sparseml_analytics as _analytics
+
+
+_analytics.send_event("python__yolact__init")
 
 _LOGGER = _logging.getLogger(__name__)
 _NM_YOLACT_LINK_TEMPLATE = (
     "https://github.com/neuralmagic/yolact/releases/download/"
     "{version}/yolact-0.0.1-py3-none-any.whl"
 )
```

## sparseml/yolov5/__init__.py

```diff
@@ -15,92 +15,37 @@
 """
 Tools for integrating SparseML with yolov5 training flows
 """
 # flake8: noqa
 
 import logging as _logging
 
-from .helpers import *
+from sparseml.analytics import sparseml_analytics as _analytics
 
 
 try:
+    import cv2 as _cv2
+    import torchvision as _torchvision
+
     import yolov5 as _yolov5
+except ImportError:
+    raise ImportError("Please install sparseml[yolov5] to use this pathway")
 
-    _yolov5_import_error = None
-except Exception as _yolov5_import_err:
-    _yolov5_import_error = _yolov5_import_err
+_analytics.send_event("python__yolov5__init")
 
 _LOGGER = _logging.getLogger(__name__)
-_NM_YOLOV5_TAR_TEMPLATE = (
-    "https://github.com/neuralmagic/yolov5/releases/download/"
-    "{version}/yolov5-6.2.0-py3-none-any.whl"
-)
-_NM_YOLOV5_NIGHTLY = _NM_YOLOV5_TAR_TEMPLATE.format(version="nightly")
-
-
-def _install_yolov5_and_deps():
-
-    import subprocess as _subprocess
-    import sys as _sys
-
-    import sparseml as _sparseml
-
-    nm_yolov5_release = (
-        "nightly" if not _sparseml.is_release else f"v{_sparseml.version_major_minor}"
-    )
-
-    yolov5_requirement = _NM_YOLOV5_TAR_TEMPLATE.format(version=nm_yolov5_release)
-
-    try:
-        _subprocess.check_call(
-            [
-                _sys.executable,
-                "-m",
-                "pip",
-                "install",
-                yolov5_requirement,
-            ]
-        )
-
-        import yolov5 as _yolov5
-
-        _LOGGER.info("sparseml-yolov5 and dependencies successfully installed")
-    except Exception:
-        raise ValueError(
-            "Unable to install and import sparseml-yolov5 dependencies check "
-            "that yolov5 is installed, if not, install via "
-            f"`pip install {_NM_YOLOV5_NIGHTLY}`"
-        )
 
 
 def _check_yolov5_install():
-    if _yolov5_import_error is not None:
-        import os
-
-        if os.getenv("NM_NO_AUTOINSTALL_YOLOV5", False):
-            _LOGGER.warning(
-                "Unable to import, skipping auto installation "
-                "due to NM_NO_AUTOINSTALL_YOLOV5"
-            )
-            # skip any further checks
-            return
-        else:
-            _LOGGER.warning(
-                "sparseml-yolov5 installation not detected. Installing "
-                "sparseml-yolov5 dependencies if yolov5 is already "
-                "installed in the environment, it will be overwritten. Set "
-                "environment variable NM_NO_AUTOINSTALL_YOLOV5 to disable"
-            )
-            _install_yolov5_and_deps()
-
-    # re check import after potential install
+    # check nm-yolov5 is installed
     try:
         import yolov5 as _yolov5
     except Exception:
-        _LOGGER.warning(
-            "the neuralmagic fork of yolov5 may not be installed. it can be "
-            "installed via "
-            f"`pip install {_NM_YOLOV5_NIGHTLY}`"
+        raise ImportError(
+            "Unable to import the neuralmagic fork of yolov5 may not be installed. "
+            f"it can be installed via `pip install nn-yolov5`"
         )
 
 
 _check_yolov5_install()
+
+from .helpers import *
```

## Comparing `sparseml/exporters/transforms/matmul_to_matmulinteger_add_cast_mul.py` & `sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,34 +18,35 @@
 from sparseml.exporters.transforms.utils import (
     INITIALIZER_MATCH,
     MatchResult,
     add_quantized_conv_matmul_add_ops,
     any_of,
     get_quantization_params,
     get_structural_matches,
+    optional_node,
 )
 from sparseml.onnx.utils import ONNXGraph
 
 
-__all__ = ["MatMulToMatMulIntegerAddCastMul"]
+__all__ = ["MatMulAddToMatMulIntegerAddCastMul"]
 
 
-class MatMulToMatMulIntegerAddCastMul(OnnxTransform):
+class MatMulAddToMatMulIntegerAddCastMul(OnnxTransform):
     """
     A transform for converting a MatMul with kernel and bias into a
     quantized representation
 
     ```
     |     weight (initializer)
     |         |
     |         Q
     |         |
     | input   Dq
     |   |     |
-    |  Q/Dq   Transpose
+    |  Q/Dq   optional Transpose
     |     |   |
     |     MatMul  bias (initializer)
     |         |   |
     |         Add
     ```
     (where `Q` is QuantizeLinear, and `Dq` is DequantizeLinear)
     into
@@ -70,15 +71,15 @@
             parent_ops=[
                 [any_of("QuantizeLinear", "DequantizeLinear")],
                 [
                     # weight should be initializer
                     INITIALIZER_MATCH,
                     "QuantizeLinear",
                     "DequantizeLinear",
-                    "Transpose",
+                    optional_node("Transpose"),
                 ],
             ],
             children_ops=[["Add"]],
         )
         for match in matches:
             # NOTE: bias could be either input 0 or 1 of add node
             bias_init = graph.get_init_by_name(match.children[0][0].input[1])
@@ -96,15 +97,15 @@
         graph: ONNXGraph,
         model: ModelProto,
         match: MatchResult,
         bias_init: TensorProto,
     ):
         matmul = match.node
         (input_quant,) = match.parents[0]
-        weight_init, weight_quant, weight_dequant, transpose = match.parents[1]
+        weight_init, weight_quant, weight_dequant, opt_transpose = match.parents[1]
         (add,) = match.children[0]
 
         input_quantize_params = get_quantization_params(
             model, input_quant, include_target=False
         )
         weight_quantize_params = get_quantization_params(
             model, weight_quant, include_target=True
@@ -118,18 +119,19 @@
             input_quantize_node=input_quant,
             weight_quantize_node=weight_quant,
             input_quantize_params=input_quantize_params,
             weight_quantize_params=weight_quantize_params,
             bias_initializer=bias_init,
             bias_add_name=add.name,
             target_output=add.output[0],
-            transpose_weight=True,
+            transpose_weight=opt_transpose is not None,
         )
 
         # Clean up
         self.delete_node_deferred(weight_dequant)
         self.delete_node_deferred(weight_quant)
-        self.delete_node_deferred(transpose)
+        if opt_transpose is not None:
+            self.delete_node_deferred(opt_transpose)
         if len(graph.get_node_children(input_quant)) == 1:
             self.delete_node_deferred(input_quant)
         self.delete_node_deferred(matmul)
         self.delete_node_deferred(add)
```

## Comparing `sparseml-1.4.4.dist-info/LICENSE` & `sparseml-1.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml-1.4.4.dist-info/NOTICE` & `sparseml-1.5.0.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml-1.4.4.dist-info/entry_points.txt` & `sparseml-1.5.0.dist-info/entry_points.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 sparseml.transformers.question_answering = sparseml.transformers.question_answering:main
 sparseml.transformers.text_classification = sparseml.transformers.text_classification:main
 sparseml.transformers.token_classification = sparseml.transformers.token_classification:main
 sparseml.transformers.train.masked_language_modeling = sparseml.transformers.masked_language_modeling:main
 sparseml.transformers.train.question_answering = sparseml.transformers.question_answering:main
 sparseml.transformers.train.text_classification = sparseml.transformers.text_classification:main
 sparseml.transformers.train.token_classification = sparseml.transformers.token_classification:main
+sparseml.ultralytics.export_onnx = sparseml.yolov8.export:main
+sparseml.ultralytics.train = sparseml.yolov8.train:main
+sparseml.ultralytics.val = sparseml.yolov8.val:main
 sparseml.yolact.download = sparseml.yolact.scripts:download
 sparseml.yolact.export_onnx = sparseml.yolact.scripts:export
 sparseml.yolact.train = sparseml.yolact.scripts:train
 sparseml.yolact.validation = sparseml.yolact.scripts:val
 sparseml.yolov5.export_onnx = sparseml.yolov5.scripts:export
 sparseml.yolov5.train = sparseml.yolov5.scripts:train
 sparseml.yolov5.validation = sparseml.yolov5.scripts:val
```

## Comparing `sparseml-1.4.4.dist-info/RECORD` & `sparseml-1.5.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-sparseml/__init__.py,sha256=F8VVKeTRy1P4zWbt_9IP-BOnVbuo3vFuxohmRslIPXM,1683
+sparseml/__init__.py,sha256=nxuiUykjTFTYiw28TB9H75wWbdzr6Y0j-2h4dabdp54,1413
+sparseml/analytics.py,sha256=WhXdKgK1-ll9sRzn2n8z-FAikQ02J8rUeWmceiX5S7E,898
 sparseml/base.py,sha256=oOPiaU2JhI0beFwp8Obe7hbt3kUuNvI5XD1wTBCtLnc,10284
 sparseml/log.py,sha256=K5E3goPRIPY7Uc14JcX-4oLXVWu7ecOPf1NYBGHc1r0,2483
-sparseml/version.py,sha256=SlggZQgP30aO64jl3FXTc75chAHgHJh0m1Gi0iY74ec,1510
+sparseml/version.py,sha256=UZJVzd8NwptR2hTgM4HQP2UR7hIZZO7BSRFwFYA0rNc,1510
 sparseml/benchmark/__init__.py,sha256=WynUhMzXq3-iQAhPwcmcMOj2_xCa9brLubs7gxq9T3U,758
 sparseml/benchmark/info.py,sha256=yRA5QgKQNKjOZhQH9uNvVuWlqL4eXDVikA8pL5Mzha4,17631
 sparseml/benchmark/serialization.py,sha256=FPpcC93x5H86Fqil9YbERUpltu7qhhIQjsyYaSlW_20,10778
 sparseml/deepsparse/__init__.py,sha256=o5ITzTEOlH--61_SXMISrmPcRk4ci91FGlR-aQxwOn4,863
 sparseml/deepsparse/base.py,sha256=nRjU6TSao0J2iWXcdHwj62X6dVT9vl6TQ2y4Bdn3KN0,3516
 sparseml/deepsparse/framework/__init__.py,sha256=ZHrXXM3AMH78zKcF8Y40IBuy38UFy4fLrvytozw_bNY,801
 sparseml/deepsparse/framework/info.py,sha256=HVDPHFXggFeDqbpM20PkByf1nBccwKnjpTWh0EfrVas,6032
 sparseml/deepsparse/sparsification/__init__.py,sha256=re_2FtHWvO-iQQwRRJZDKz3l_pFZuwe266-4ZFxQqbY,813
 sparseml/deepsparse/sparsification/info.py,sha256=O5FJg5KMJvj-HcJn9W9iiKGZ6Z7_1SavOX-TstXRr6Q,1348
 sparseml/exporters/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
 sparseml/exporters/base_exporter.py,sha256=M1HEe9GNf51uYx1z-qxWjIYo5iGZ_Ish8uZ3mj6OZR8,1477
-sparseml/exporters/onnx_to_deepsparse.py,sha256=-Xa7-XECHjggxLv9EIOXzWzbeGsGNPIurcfQbVG_2M8,4684
-sparseml/exporters/transforms/__init__.py,sha256=aWe9RsizlhUcp97UIEd5kwR2BSXL6c1h_W_x821ua0Y,2170
+sparseml/exporters/onnx_to_deepsparse.py,sha256=X2yFfvJomwLOGHfe_ZmmosPc0Pa4Bjmw81q0uv_Rq18,4751
+sparseml/exporters/transforms/__init__.py,sha256=bitsfVa9RUFuZYVUD4oxEh_IqEyiQQuxIYaGA8rOt2w,2252
 sparseml/exporters/transforms/base_transform.py,sha256=IpvdUdEADl2SfqHawcp6-lcNgz-R3L0zpS05WaWF5h8,2333
 sparseml/exporters/transforms/constants_to_initializers.py,sha256=_PX3y16OC-q85d-6DeOOVpKAAMNIU1m5BdYTZlFV_tk,1388
 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py,sha256=9z2HRqJAM68HPiSfu2RMyrn93dr8HCTpMcMrh_1-x2w,3866
 sparseml/exporters/transforms/conv_to_qlinearconv.py,sha256=CwCXtIBCOQ1qX5Z2JZhsdXSDk683wRCIBILF_1vd0GI,5838
 sparseml/exporters/transforms/delete_repeated_qdq.py,sha256=YiIOrvKqrxYboOA4A8YTbQIQ4s4MDdmqeLNYHPP4kjs,2440
 sparseml/exporters/transforms/delete_trivial_onnx_adds.py,sha256=St3-PQP8tPXYoyQTFn8fvJi7JF3LoX9Vb9nc-Zbx4Wg,1842
 sparseml/exporters/transforms/flatten_qparams.py,sha256=u0POagPJ_sqaS-DMe2x1Fd40RdlS9nYlLFZqHdsXx4Y,2181
 sparseml/exporters/transforms/fold_conv_div_bn.py,sha256=ckYdMKO2Z31NKRxQk4C4EbMWlVrsuhUDtyeMTMTErE4,3553
 sparseml/exporters/transforms/fold_identity_initializers.py,sha256=Yfv46MvL_vMxNGmUYSvlbucbrWIIDnjWnifmFCzyILA,1669
 sparseml/exporters/transforms/fold_relu_quants.py,sha256=qDGl-6aGmaQ8lAii3v0NvqkjbqtZB1UgHEkd3RzvjXQ,2070
 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py,sha256=r1oVnnu-U0mISkqBJrebXO1o-cmbkSMbo1X4xA0l-t4,4418
-sparseml/exporters/transforms/gemm_to_qlinearmatmul.py,sha256=PxWNloG30hp-PDDoHGwwpZHmlkmL3CChxH-bZ2pIJ5c,7546
+sparseml/exporters/transforms/gemm_to_qlinearmatmul.py,sha256=ccrB80ymufz6c9znwIGz0rxvM6U-vmKqiCa7l0vKYfE,7629
 sparseml/exporters/transforms/initializers_to_uint8.py,sha256=GxveAKe1xSNBZh1hjUx61veL6LTf9Msnx663Mrhvtxg,1645
-sparseml/exporters/transforms/matmul_to_matmulinteger_add_cast_mul.py,sha256=KXSelW6JzsRGXXWJIoiO8QhlGficcqCp8trPIziTnQo,4350
+sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py,sha256=1YxX2xm2JC3IUj4AuRxRf2yXeOWj-esLLo-aoL_LtOo,4470
+sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py,sha256=l3JXoue_8Rs8DMGaH_MCNBR5RZRIzIhXiM5D_TRS81M,4571
 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py,sha256=Siii4mZ3LtqWY1blD1KT7ePVJud1oyLDrcr21YosU7E,4156
 sparseml/exporters/transforms/onnx_transform.py,sha256=o3jRAOag020HzYRtqQdp-CXEFReZm3yGng7tHvqWM5Q,3724
 sparseml/exporters/transforms/propagate_embedding_quantization.py,sha256=XTEiUTX5nzLUtndGs_0t7nTgjIad-FyjuNc0O4f6Xro,3398
 sparseml/exporters/transforms/quantize_qat_embedding.py,sha256=_v1dEEt5vCSaMF6dJkg9fVGof145-_Lmo0DMjpXsnUE,4464
 sparseml/exporters/transforms/quantize_residuals.py,sha256=f3kNF930ymHI5CmCA0OmYW7vDKvEm9sYhN0UX0UC1EQ,3869
 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py,sha256=mod-7bnlkg20LjerZ7tKKmp_7XyO3FKo13BtIZkDsmM,3331
 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py,sha256=2FSXzaY3jdxOgj3xBaUOUqtk-hzg4kwhheELhoOKpS8,2545
 sparseml/exporters/transforms/skip_input_quantize.py,sha256=ANiYDwSos9gPW4960fMwmGubTDgpAcqFVSIHKf_ffYw,3210
 sparseml/exporters/transforms/unwrap_batchnorms.py,sha256=ly7GHCXN_2r8Gnk8PABWCqcoS-NL3GMfquEK0hRlFCs,1373
 sparseml/exporters/transforms/utils/__init__.py,sha256=tXSSUnzdyIc_H73xQ5dYhHb1Gj4Nb7GLLDVwJds8c_s,730
 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py,sha256=lUutqioFTP3ZVa5IIA-Z5WbriNj_8m2mXut_QOyo_J0,8704
 sparseml/exporters/transforms/utils/helpers.py,sha256=vkEYL2Bdp_YNXlPg_TGd82Q2ef1EYEr11LVgmORQDiY,6457
-sparseml/exporters/transforms/utils/matching.py,sha256=h0DCUGRSy22LVTrwZEuo9XdJ662dt-SuyFCTalgjxd4,14130
+sparseml/exporters/transforms/utils/matching.py,sha256=CnVJLbJARBJwvFjoKh9vwYt6dLP4WXG3p7nCY5VUFaE,14429
 sparseml/framework/__init__.py,sha256=EcIX435yx552d7BkbxmAbQ_X3KAISInHVbD9X-AT1Uk,790
 sparseml/framework/info.py,sha256=TaZAMYdhBHcjl9Xyk3PWjJkDB6g3_f4vD3B6KmhgOl8,9479
-sparseml/keras/__init__.py,sha256=Xzt82FZ2iOD5g7dxYJqDCFX-9w9kHcC7yxlcUZSWWvk,858
+sparseml/keras/__init__.py,sha256=G-uSbckWq3vn9YUFr5pD0xbaO694SFgIlc5AVQMDafU,970
 sparseml/keras/base.py,sha256=yt1EO6KIeCkdg8rF37U5Y3FNGeAqOQLVGyxRANsyBy0,8054
 sparseml/keras/datasets/__init__.py,sha256=USLH-kFbXiubqgMW8IMkZfycVByQAOdAtzuPHzTok9I,943
 sparseml/keras/datasets/dataset.py,sha256=W6wdx4WXtyy4r1JVbc8fO0Xt5SM03zm8Vq306uNFkaw,3297
 sparseml/keras/datasets/helpers.py,sha256=PfDBKDMr3A8XG9wP0QRABu4h63eHZT15gDuO8naIXxY,2423
 sparseml/keras/datasets/registry.py,sha256=41aieOOADwl0V1n127OA6zyxhCwLwHy4jo7SkyzSUwo,2761
 sparseml/keras/datasets/classification/__init__.py,sha256=YGWvyTK6h32vDtAD3Vcr3bsNqGvfFXOiQy9wydvzEDc,786
 sparseml/keras/datasets/classification/imagefolder.py,sha256=Ay5xsUH4zR2xgTg6HM7qXiOMs02PMMg3-_pD0tgzzgE,8369
@@ -76,15 +78,15 @@
 sparseml/keras/sparsification/info.py,sha256=HVIGhKG2HHOaYxgvltQ7hjOQXbqbvT2DO3F4gBP1lbc,1356
 sparseml/keras/utils/__init__.py,sha256=JkMJHbL8sCUKcDOfOGNpqexmdsnq6vdQpNUQCbVMNY8,962
 sparseml/keras/utils/callbacks.py,sha256=WqycV-Wq2YEQ1uYuTmqEW-C_5Aeowt_DTB8C4oruOSk,8202
 sparseml/keras/utils/compat.py,sha256=oPMoTw2NKedJTk2PhA_75YBM6Nwxg_Yx0MyUdcgbisw,1022
 sparseml/keras/utils/exporter.py,sha256=mC-and9qFuOT5qVHRR3iBTvvwRpUUz_C8oR1WK078lM,5737
 sparseml/keras/utils/logger.py,sha256=xsOmL5qUHvWwFhGIRlNuQLAO8DMpx_-fxvr5N3QrQt8,6087
 sparseml/keras/utils/model.py,sha256=Or2Vijn7JPrE4QMTwBYX8zgmoucYRQK8y1VVDL9vJ1Q,1738
-sparseml/onnx/__init__.py,sha256=Z17rCpIq-GH4_UejqYRTksEDAvz7nEj9fYtaBgxgY6k,925
+sparseml/onnx/__init__.py,sha256=KeWF6EQ7cpX_b-fMhiG5n6pVPUvRxiWMpzpiI9EagFI,1036
 sparseml/onnx/base.py,sha256=Kv3YC0Xh1xlxpIuwh9916SHuz96phaf36KbL71DSZWk,6202
 sparseml/onnx/benchmark/__init__.py,sha256=tl8cy1ta02lUmMxwmDfRAYcVQfaj5OpU3igqYJHMGg8,743
 sparseml/onnx/benchmark/info.py,sha256=iCNry2VAuSmTLrPl3a8pxDU_R-U9-Lpcka40QIg5BZg,15366
 sparseml/onnx/framework/__init__.py,sha256=HpgplVizgXIPOmnE24RM1geQLp924227_T12jJjQCaA,823
 sparseml/onnx/framework/info.py,sha256=YzZmDaR6Z1y66xo_OKtmQGA1ZVFOozZNXBJ_Ec74ueU,6116
 sparseml/onnx/optim/__init__.py,sha256=EZeHGH5zDRfb0MrXqh4_3ci0ViBS2WWb8NqhAi8nd3A,820
 sparseml/onnx/optim/analyzer_model.py,sha256=NLxYEH9QaU-xl2h1SagMHyfQ3skEsuYRFTqeYpKTgIM,13274
@@ -98,30 +100,30 @@
 sparseml/onnx/sparsification/analyzer.py,sha256=DCKc8nYo0i3NDu73GVjvBYjuflXUZhkhB14FoFRlTBE,10209
 sparseml/onnx/sparsification/info.py,sha256=UnrwVgOuj-HErwTMc-19h-QOrs1yG_mM45O9VL8oiXU,1363
 sparseml/onnx/sparsification/model_info.py,sha256=Y0tpY9fWN3gr4KlkAdXv2QYJrrrjMvVZOCA-ujPJFPM,8009
 sparseml/onnx/utils/__init__.py,sha256=fGZED95Xmko70ZmTWlZWX3-C4dajmbZcKgaap3HXmVw,867
 sparseml/onnx/utils/data.py,sha256=6Rw3hkSG1DZ057USkzioSDFcYH92ZLwdHYlQY2PdkwQ,13002
 sparseml/onnx/utils/graph_editor.py,sha256=IBNbKWjOLy7oW-bjsxBkSw5HULHIoeVFQFs2ccYVTs0,16407
 sparseml/onnx/utils/graph_optimizer.py,sha256=AfS2zdxW1tJ6xYAe-2n3KdAdDenxiqslOFUIVAzD-cY,8133
-sparseml/onnx/utils/helpers.py,sha256=UnAFdVaqXKjd09ciC-M6rOYJcZsivES_1dgLBmYy_mE,41184
+sparseml/onnx/utils/helpers.py,sha256=NQmCHhRqb3qjs1cjK-LjorgfhEC7yroPvW_f1ajBZJE,41311
 sparseml/onnx/utils/loss.py,sha256=2njnY0qY2n6DS9HHB0kqLz7N8wgPaDTkAi6Z2DLYPLc,1958
-sparseml/onnx/utils/model.py,sha256=cK6oiwDZ_AZya9_wbxR6Cdu6pcLozIy_wP0PIF1xviA,31516
+sparseml/onnx/utils/model.py,sha256=ElcSfKhUnqvjpYusg4iD-pL-y77T14mvECDBPPGnNnQ,31586
 sparseml/onnx/utils/sparse_tensor.py,sha256=6Bu9fVJqLCtve3qpg9ScYGqcv4X7ZcRKhVrp8pCLBRI,5437
-sparseml/openpifpaf/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
+sparseml/openpifpaf/__init__.py,sha256=aGr1xneMg-zE7LNhYNjjmEznKB6-xHbpZCT91uv4j3c,931
 sparseml/openpifpaf/export.py,sha256=YkX06A384K17AfKYli1RcYHcoVg4gF79ttZ-73H_6rI,3694
 sparseml/openpifpaf/train.py,sha256=vl5ioCcnzep9XNVMOsveO9QRRrXSn8VDnEM1LGv71Ew,10950
 sparseml/openpifpaf/trainer.py,sha256=Du9W5fW9ImC3XlOVVWesbcBv1SjJOfP_D94_hBUR6VY,4211
 sparseml/optim/__init__.py,sha256=3oGQ4LY0MSrbTAwuyPHEOEyYiZ7JI7OX2BgWup5NPuw,882
 sparseml/optim/analyzer.py,sha256=LUYBYyvfVwaw_V1aAiOmaybUGJQk4vRK5RG3k3nD7pA,6302
 sparseml/optim/helpers.py,sha256=Zb7YPYe07vuVyYUhHJ-BlcMrZa-sxt1TUZ-Ec9Z6o_U,25563
-sparseml/optim/manager.py,sha256=DNw1V8cRhTIMyrTTexZmvIR4UkasieCBrgKHeSoDeoY,23742
+sparseml/optim/manager.py,sha256=KeDVHj9ea9EUaV908qfvq8ONwS8nUmAvQb1yXflOBWo,25984
 sparseml/optim/modifier.py,sha256=qYfVUL9thw94p4oEsNZgitUJ3y9izWYb8nUI3enyzOU,30708
 sparseml/optim/sensitivity.py,sha256=neMP_hTRqzDUV0MrATevC2-JQYnOIvNW_AlIf_y_ydw,26315
 sparseml/pytorch/__init__.py,sha256=3E40C1X1fjhlU0ZwdHZ-xhORHb-qDUtr7ALDv9xbzI0,1848
-sparseml/pytorch/base.py,sha256=NTBT19CSpUiQKvGDw-cUbSCkLvVobBbt6zpnxfB6cwc,6173
+sparseml/pytorch/base.py,sha256=-RvI-RM0ZynTCrsX0VaN_aoDPUdfCc1E1MeUY1VWFH8,6173
 sparseml/pytorch/opset.py,sha256=-BsKarkkKfq09HYJLZfxt_AEHEfuENpRDZF_J2va1Ck,933
 sparseml/pytorch/torch_to_onnx_exporter.py,sha256=hluxRT9RdpIeZmA4Z4KU-ajielvT_09rov-1MYDCR08,10826
 sparseml/pytorch/datasets/__init__.py,sha256=2xoH_fCMojldFY1RCWSkt9pGfa8SzHAxU5em-_ZiwV8,998
 sparseml/pytorch/datasets/generic.py,sha256=nl-fFlpd7u5sNswe1AORZvQUne3sqrrPWnNgOUp6_Fc,4193
 sparseml/pytorch/datasets/registry.py,sha256=cEA3d5ju5EMft92f2StVLWARnAxlRpidKZaozujmFdE,2814
 sparseml/pytorch/datasets/classification/__init__.py,sha256=GMKhziJkRwSC7E_1Nox8FxnxhPFozZ6MxQWUWi1BN_Y,828
 sparseml/pytorch/datasets/classification/cifar.py,sha256=k32Z552YrrJv7IlshH8AWylaRKCOUC8KSrzRLLTHTag,4017
@@ -135,54 +137,54 @@
 sparseml/pytorch/datasets/detection/voc.py,sha256=ntif1itgg0o4GRkZHHexBHIm_E9NaJh5opdPSG5jMeQ,10759
 sparseml/pytorch/datasets/image_classification/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py,sha256=yMUOho19OugY5yaH5oXOho41_uYYjkwmvfhzdAA1u4w,9512
 sparseml/pytorch/datasets/recommendation/__init__.py,sha256=Ngvu1hKPBJs8KQ-3f_FnGrp4Zw49VGrTg-3uQbYhIXo,684
 sparseml/pytorch/datasets/video/__init__.py,sha256=FCWCuDjr7Vs7u1UYDOfe0AJvJlGoskWv6Rx0kyc0i9M,693
 sparseml/pytorch/framework/__init__.py,sha256=9PE8aAdkuM75YAo4CKmDJZf49VcZu3d0g9ywcxQUiGE,814
 sparseml/pytorch/framework/info.py,sha256=bD9mZK163Ozqetr14_bwlzn4VJJ5RSUbfiP7V9sEy8o,5580
-sparseml/pytorch/image_classification/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
-sparseml/pytorch/image_classification/export.py,sha256=IDWzbwsWuppbPWRla3ePm9vOKO3buzPoej-TgoOQAbs,18258
+sparseml/pytorch/image_classification/__init__.py,sha256=tXi9ZUe6trd4y1XOeQYuOPPzFVlr_wjvhwc_dIwPc4o,753
+sparseml/pytorch/image_classification/export.py,sha256=FG3TIe06X5PYlubyGmDjNKWBZHsX24wQ19gbqXMT3BQ,18265
 sparseml/pytorch/image_classification/lr_analysis.py,sha256=qweXU51KeWjW86RJknvsavKPPXMd3PGAO7bcGosjTqE,15494
 sparseml/pytorch/image_classification/pr_sensitivity.py,sha256=RA64lC4NOmFm2H11MO4HSuiw2ImtiRwvixtIw7Rol0o,14444
 sparseml/pytorch/image_classification/train.py,sha256=-My1yUclgRA5wQoV4B_jtoOMRO1nQj389WfDkebu3fs,29287
 sparseml/pytorch/image_classification/utils/__init__.py,sha256=ambjlzpSCaSZ7ZadPk2vMAB6kaZCm7f_hVqOVSWz8k8,682
 sparseml/pytorch/image_classification/utils/cli_helpers.py,sha256=qypcmjezy-fZn2Cjozv9vumZoB44_9PDe_WXnChbvLg,4278
 sparseml/pytorch/image_classification/utils/constants.py,sha256=k01fijyL2BicSWLL1EzhhdvG07WYMMXHZeFz-9fxecM,1257
 sparseml/pytorch/image_classification/utils/helpers.py,sha256=0VtpB5TFfPp8oNtSVlyAk70mTSOBmhbjnYCP49j-Jmg,20912
-sparseml/pytorch/image_classification/utils/trainer.py,sha256=KuTNR9lc-HE0zmin6T0xJQqAO0vFwkV7fpjvyiI27RU,11781
+sparseml/pytorch/image_classification/utils/trainer.py,sha256=2WOP42hSlowDG2_DyCZOu8T5yohhV38e192ZxeWXj_A,12056
 sparseml/pytorch/models/__init__.py,sha256=Lj1KLciXTQiZObA5HHgrPMHNQ1bGYswrsP776eizaUc,976
 sparseml/pytorch/models/registry.py,sha256=cJLPsK8zzhVyZPvcJ8_Kj9-Ru9lTOywv61xuE50LiC8,14753
 sparseml/pytorch/models/classification/__init__.py,sha256=opnCtf6WMl1kuQ_vRAZRLl1eFZefpG9GFc9o729HndQ,901
 sparseml/pytorch/models/classification/darknet.py,sha256=rR4XXQu7shLADU4Th0D-eodnv-Z3AmA6kj8tDgHmtxU,11658
-sparseml/pytorch/models/classification/efficientnet.py,sha256=_TedHJr332qt-9etaVCYnk9eOvfeSane3RoToFHILN4,40335
+sparseml/pytorch/models/classification/efficientnet.py,sha256=Bs88xu2xX9P65TOZ_6rn_qO2CMa6oLsJm5xt-Y6gISI,40293
 sparseml/pytorch/models/classification/inception_v3.py,sha256=wxWU3ja6E0_ERhYniDlzcsnVWi-rvJVfgxmhsyrpuC4,16512
 sparseml/pytorch/models/classification/mnist.py,sha256=RyFLHgKzmbmSvI-7F4nkbUI7xkz5pKElT7ve1ZIn7VU,4164
 sparseml/pytorch/models/classification/mobilenet.py,sha256=0ffCRqolRchhz4YoDH--tyDzLuQ1vyVbXL5LpAkXuIM,9546
 sparseml/pytorch/models/classification/mobilenet_v2.py,sha256=e6SqGzdIuOEzwp_sbvEAXSwrv5eHPpYz-lgHACqrSXs,13014
-sparseml/pytorch/models/classification/resnet.py,sha256=gQzFigjFUWNfUSp6oQWrvKF0ak0HlFpsE5YuupX-HYc,40931
+sparseml/pytorch/models/classification/resnet.py,sha256=wvdwz-53nFlyFWCHGAm2w4KIlV5TQ2C86BmiNUZR528,40800
 sparseml/pytorch/models/classification/vgg.py,sha256=_7Dyaj58dSzvi7KcooOYlUEg8kJGkQsDLhxpIWFhnS0,16649
 sparseml/pytorch/models/detection/__init__.py,sha256=NIlqCw6brqzhSlo6SyGz3eHmj3W1njG0qyvR4n5E3ZM,824
 sparseml/pytorch/models/detection/ssd.py,sha256=38w-HWL9SiM3KvVN1KyPfpJVq-U1i-wx4zZeucxKvss,6820
 sparseml/pytorch/models/detection/ssd_lite.py,sha256=UoXcZlEsOxw_1chviAluKKYEJZajflYvuvLF5lsfsCM,8116
 sparseml/pytorch/models/detection/ssd_mobilenet.py,sha256=fDmIPuCnDh8jvNTV3F7TUZZSc3hugxO7wGFJxrIeF1o,4046
 sparseml/pytorch/models/detection/ssd_resnet.py,sha256=Im4m61GZfDdgwtemTqzVK1hduoCOSf8c_Fnif1zvGZQ,9069
-sparseml/pytorch/models/detection/yolo_v3.py,sha256=JMjZbIqx5uT1M2lbTVvTmZwkizrmcFsyreOAusa7f8c,10190
+sparseml/pytorch/models/detection/yolo_v3.py,sha256=18iwLZYstNkHu0JVi3Q9u62_e1zVly0KqmdgrtfLSN4,10188
 sparseml/pytorch/models/external/__init__.py,sha256=AiEtY-pE9G_KjBSauDEkvV4tmcDEqFrDNrx5aCuKHhQ,763
 sparseml/pytorch/models/external/torchvision.py,sha256=pa44NKWjGHmY7tP99PcOm3sZjciHNzWP21R_-Y2ICUs,6759
 sparseml/pytorch/models/recommendation/__init__.py,sha256=_UPdXBGXmCpAEg7pgJ-0rZjoBhUkFje1JxcItjktRK8,676
 sparseml/pytorch/nn/__init__.py,sha256=bd3tEwx7afmeU0yK0ywTsq4bI1QoxtjRA4Dq-C5ImMs,925
 sparseml/pytorch/nn/activations.py,sha256=dNDJaeZIUOqtQW-aAvARBVz0uE4MXKKZFbGt6_vu6Yk,8673
 sparseml/pytorch/nn/fatrelu.py,sha256=twbvUqaJsKkjplrUJaVm4mfq-OC63eN-IboG70nhZO8,11854
 sparseml/pytorch/nn/identity.py,sha256=vCs9du3P0fQS6clFFNCacHE-J_OGZiKcvsEz-iHZy4s,1690
 sparseml/pytorch/nn/se.py,sha256=kR9agk8OKTEq_iPRLX8NHlbFUJlZEVFt7Otgtk5LoXQ,2828
 sparseml/pytorch/optim/__init__.py,sha256=pV-8sO8TP23X6gS81BvCfEC9LCnRYws3ek-pylOnaHg,1243
 sparseml/pytorch/optim/analyzer_as.py,sha256=6WCMuxF-8rcFYNTNiNoQMNloISfJBrk_9bYbSiMK1-8,13638
 sparseml/pytorch/optim/analyzer_module.py,sha256=u8E3l-hvIhicNqsGcY4WTrT1hZBtPsIN2unqix8RAhI,17069
 sparseml/pytorch/optim/analyzer_pruning.py,sha256=V-VWmMgTU1nHgcLlVmyl3aNo4yeeG0HGleAfTkhNiyI,3955
-sparseml/pytorch/optim/manager.py,sha256=YVqmzFMCcsUumw8atHXkPXEcNIphVSvV1E8dmd1nXBk,26711
+sparseml/pytorch/optim/manager.py,sha256=abFJNGYSBohaZAq65ZVojG7dl45QuXALmhkJanIVyWg,26838
 sparseml/pytorch/optim/mask_creator_pruning.py,sha256=k0gHVM8fThZqLOBfdfte1l7zoylvDRpaAxfcM32eioc,36844
 sparseml/pytorch/optim/mask_pruning.py,sha256=QqBrPfskL0vJlFOsxrqZp0sCk8NQUf4srj5WNuWHyJY,23085
 sparseml/pytorch/optim/mask_pruning_scorer.py,sha256=IKiIegTFtez2taiWwDwaxJOMvEd8---GQ28CeZD24gI,10449
 sparseml/pytorch/optim/optimizer.py,sha256=f20_TaCsvNRybm0qqG1BqXu1KOQpDeQkIOZWiMvftJc,6605
 sparseml/pytorch/optim/sensitivity_as.py,sha256=9QJiRvMkFXCFCCQYuA77BwJgJRoHDtuQ4fxx3T3cwtY,14879
 sparseml/pytorch/optim/sensitivity_lr.py,sha256=j78fmJBoAhK-NKM8mVLdc78Hh8-6Jzyplba-UJp_Yfg,6101
 sparseml/pytorch/optim/sensitivity_pruning.py,sha256=9cxUlgVW2JFL69rVe2UYX6ID8m9_-d-x4_J6iSN-W1Y,9324
@@ -192,78 +194,84 @@
 sparseml/pytorch/recipe_template/main.py,sha256=o7sK_d3AXpdwn8ze-_bNClBgPp_lzM9TRl0HFbtLMCY,15943
 sparseml/pytorch/sparsification/__init__.py,sha256=ilePtrdbOlUDo54J3thfX_aWpaGmy081zfjAe1wLBVU,992
 sparseml/pytorch/sparsification/info.py,sha256=BWPbqg1ODqmoDxuPYzXes7A1hGMrMcH1rqnJapW36pY,1366
 sparseml/pytorch/sparsification/modifier.py,sha256=cEOpqCzfQpputxN4Xn2kWHabMxWbIzqTCuAv5pSkKFQ,32014
 sparseml/pytorch/sparsification/modifier_thinning.py,sha256=HLfbTZbqNTaqQ1fWu2y5J_QVqj57cKbK0p0zrdKu1MI,18952
 sparseml/pytorch/sparsification/distillation/__init__.py,sha256=btJ9Wl7isNbxgmzE7PjTeffGgRovVqTkcBfv9M1tV5U,705
 sparseml/pytorch/sparsification/distillation/modifier_distillation.py,sha256=o26xRGsPP0SIyKZ7j6THdfj5802WFlQHEDIeNbxrfUQ,4741
-sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py,sha256=qznm9EWML--DtVzvdqhmgMRFJxJHSK_SCu2yZ9KpWQc,14533
+sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py,sha256=8xffEKekDy6Hs_laCVYV6LB1aJVRVvv6q7dKpXGvXa0,14742
 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py,sha256=SzM-TDC2SS0hBLr3PbeVE01oBcbHGL2SvqT0awCiMVo,19177
 sparseml/pytorch/sparsification/pruning/__init__.py,sha256=cTCk2F5tGMUwKVDhTFSvjGtx42MRRxQR2ei_zn6djyg,1158
 sparseml/pytorch/sparsification/pruning/mask_creator.py,sha256=Ysq75fdYo5WQcvt6ox8HTKv6SVNQjy_Y4rSs1JeLsuI,29250
 sparseml/pytorch/sparsification/pruning/mask_params.py,sha256=Xfwjsl86zbBAvGnUCAE6MzU6ABB87eMYCvnAgoztqnI,22391
 sparseml/pytorch/sparsification/pruning/modifier_as.py,sha256=7JKrvWdm3-xHF4z8IUd046BuU08P0Z-Hqqbl5YwShog,13389
 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py,sha256=jRMApqylXjFHW31nZY_iMveu265uqQqIqNHrXGzmmyU,10455
 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py,sha256=HsLi7Mdu9Lty5A9w4nY9sTe9NgzDxgJRoM-LzFkl6Ao,33219
 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py,sha256=D3zx4rL5ccwi9kFGsIo1OoPW9zl--ditOu7JKb-9hGs,5757
 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py,sha256=giv8z84R0-nQ7MRfW6MrqBd0C19GFnFTUNjJz_5HlRo,8860
 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py,sha256=5W-H7scPflGySPoeLZaFwyvihbqsYcZP6xwMWsQ75WQ,15595
-sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py,sha256=wqjXEs-dabdED__dOHUngYtOn-A60X02I49dCEDJ65o,63525
+sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py,sha256=GFJy-obm0cvr2c1vNgCWaUXAhFplvHDxUfmun98rWmY,63519
 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py,sha256=gmRbalMpVEJ-U5xdL5Vh-XcTOhkfr8z_cWlKw_m1c9k,8774
-sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py,sha256=AD5pENo3WL9FbFyWpYAZjSt3p5h4tZcVrHwn4apEEno,23769
+sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py,sha256=bKZojNIl4aWvU0xXxfAvTZztFcS2Q5QCljt43icIux0,24121
 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py,sha256=h7ASPoik7zrBXE_lbdfBO3UkbrTeXG5gGE1Flg75h8s,18245
-sparseml/pytorch/sparsification/pruning/scorer.py,sha256=EmeyC_YenT1K1xEu53J3DnEeALmi8T5sKRgisC-aCwA,4580
+sparseml/pytorch/sparsification/pruning/scorer.py,sha256=8gyYSv611GOJwmpQeD7FsWVrLxF8jeM_f59zhQlC6f8,4644
 sparseml/pytorch/sparsification/quantization/__init__.py,sha256=OjbeCzzhoeFJEJQvLmXZc89pghO83sLRhmvNF7_q_oQ,813
 sparseml/pytorch/sparsification/quantization/constants.py,sha256=sla-j0QwLFq92AbDZkHkNLxugpGrNEQJIuLWoWqV3Ks,2220
 sparseml/pytorch/sparsification/quantization/helpers.py,sha256=MmY5iOMlBUBEMrotPyj3H5drzpXhf13v4FJjb1N2aaw,32271
-sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py,sha256=VDbm7BhpZQal_u26HSixmERKk3nZCW0gb3EMzdeAR6U,33543
+sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py,sha256=TToI4dGYZZEzB1q61m1YVg0THlvH7Ew1CZ2y-ajpTts,33626
 sparseml/pytorch/sparsification/quantization/modifier_quantization.py,sha256=VQnQZozal38sffuIZjL1vKs6LeDhmiy-BvKebzewYO4,26253
-sparseml/pytorch/sparsification/quantization/quantization_scheme.py,sha256=zNlQmvlJtyLCKLDqp12fA7swf_abKgsiSIVc-CtCwj4,12560
-sparseml/pytorch/sparsification/quantization/quantize.py,sha256=Pc1AB2xDQQnq89CxoBRQnDkruUlGYpGgs-9GTKlcSk4,17476
-sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=njDZqmxyFAnfC4Pd3zUWsYMrAZD_zcboXdylTeFV74Q,67038
-sparseml/pytorch/sparsification/training/__init__.py,sha256=KBFeVJ9Q8F2uNFGkN7UHVp2Y-fqbQvmTvAZDL8e2sXA,758
+sparseml/pytorch/sparsification/quantization/quantization_scheme.py,sha256=10KNttNCHqUTNq706kPB6k7u6mvvfV0WTvx5D5Uqd-Y,12558
+sparseml/pytorch/sparsification/quantization/quantize.py,sha256=4vWbjp2WfeZ0BUf1_3BtDqLlbJfAdcrRsnzwhB5OAz8,17591
+sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=LxqptXTzW2PhIN2FuaRVHmo2gtZMOGoLzsel7jUNPh0,69783
+sparseml/pytorch/sparsification/training/__init__.py,sha256=4GGhQf6KVSOYwtr_WL9Xcvx4mR-k8yKMVI_zuTBHGO4,790
 sparseml/pytorch/sparsification/training/modifier_epoch.py,sha256=_5p1EZk2qbwTnWsMXbVan3vRj1IRyIM4wYYZdLGA5GE,1778
+sparseml/pytorch/sparsification/training/modifier_logging.py,sha256=K1NMqhea5EBPko6yim8CThShbiSJKN5P_ca_TCyZXto,2883
 sparseml/pytorch/sparsification/training/modifier_lr.py,sha256=m_tCydo_BHiXCHMUKZu6iqKLAP24acAT8-NLjH9RIlE,24287
 sparseml/pytorch/sparsification/training/modifier_params.py,sha256=G_0eVqu0Cup8WNLFhkfPmYnKtJlNrxcJt0FcOOdq9tA,21497
 sparseml/pytorch/sparsification/training/modifier_regularizer.py,sha256=ezHbcwI8ITgq4vwkzsWXgnq_ls6NONW_D8jEN-YR7u8,6690
-sparseml/pytorch/torchvision/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
+sparseml/pytorch/torchvision/__init__.py,sha256=fD0HjvgSO8WgfyPPSn7r_Fej6xWAelVJVbgWfI9ypY4,943
 sparseml/pytorch/torchvision/export_onnx.py,sha256=oiittOzvPEWMBpyldcfX6Yr7GQjKiKkOH4IUX-QQ718,6490
 sparseml/pytorch/torchvision/presets.py,sha256=PMRKjg4sBm6_UdhAV29wSSeOdDR6QlCzjcJbQWSenUA,2870
 sparseml/pytorch/torchvision/sampler.py,sha256=VuebeOVoQWLsafwJEeGgKQrDfF8PxzimHWFLs9odGz8,2530
-sparseml/pytorch/torchvision/train.py,sha256=loEiOu5-mE9ek1UPjsl6Zkx-l1Dh6hO5x5pCO873SUA,40545
+sparseml/pytorch/torchvision/train.py,sha256=YwETS0-EgjpGvs9LzKRCbGkcSHh35Mv-iOBJPGatnnM,40790
 sparseml/pytorch/torchvision/transforms.py,sha256=_WfLKV2G9ZLt2zdpKvaHA1ricPGufVIF-lzgKaOL2Ec,7128
 sparseml/pytorch/torchvision/utils.py,sha256=weRmF78Qf9_Kgd-L7aAHERmXKoCVqUP4J8pbSZmav58,16675
-sparseml/pytorch/utils/__init__.py,sha256=SZ-ovxCBrryvoZmgMcDKN9AQ8PMSA8G7T4o_YNJ57io,1121
+sparseml/pytorch/utils/__init__.py,sha256=WWPrEPVj8YsCZN0JemnAF5z7hOf0nL203uixlqWoAeo,1160
 sparseml/pytorch/utils/benchmarker.py,sha256=Zw1pEj7wDe4ZU_-G0JOCymdLXydN19K1QZKzPJvBp9E,9706
 sparseml/pytorch/utils/callbacks.py,sha256=1z10T8xE0IY5mcL2ARSsHDt6sDWRVF-Nq6zVf9OvD0s,2846
 sparseml/pytorch/utils/distributed.py,sha256=lJtEvgMg6LvH9iUwhveCaWNrx_t7pjn-sOW9rfYViwI,1061
-sparseml/pytorch/utils/exporter.py,sha256=hjRKX_GrMwyn31kjOazIBQnEEyGATZc0EQKlX-Si1g8,30763
-sparseml/pytorch/utils/helpers.py,sha256=QDkl7HVbCe1rzt1BPqlB9h-WqEUxfewd58WC_ycPQ6g,38943
-sparseml/pytorch/utils/logger.py,sha256=aUm5peoBYQmMLISQLN-qV6yZV5wgTKX3r7ZOvtfn3O0,30536
+sparseml/pytorch/utils/exporter.py,sha256=KfoPciN46ZDHKgvVk7oYBR_cyZwihRPNcCm-EvPnpfg,31056
+sparseml/pytorch/utils/helpers.py,sha256=pCQMNjgVQN4jYuerj_6YJKGDFmOZ8-3eJMcLEw5V6-A,39284
+sparseml/pytorch/utils/log_sparsification_info.py,sha256=o9WdrrDU8W1J09NHLnW2cja5PXNq442UFzgpXf8po8M,1663
+sparseml/pytorch/utils/logger.py,sha256=KOhmFXNj46gmy5XovwQOZigBuHidVmNqDnVWMUXD7PE,31374
 sparseml/pytorch/utils/loss.py,sha256=RWFyThMBaB-7jAVuS3_CU5bmsWOVFG1jqzPciSpVsj8,27048
 sparseml/pytorch/utils/model.py,sha256=KCEZ6cNkIzLKd6N8KqJe7GX3GD-PoWErZk05nEbQuJc,11754
 sparseml/pytorch/utils/module.py,sha256=gWKNLqn8bI_q97u_QC95WkxBPAclMCwz3HmrZEHEYtU,39117
-sparseml/pytorch/utils/sparsification.py,sha256=tNsC2E9YAVplcjaqDKyLQOTy3xtyZkY8VGK9dt8IJYQ,8382
+sparseml/pytorch/utils/sparsification.py,sha256=BbH3ePC74YWGddSoLcSenLd0D_0nz-Xk5vx4Ui_KkzY,8809
 sparseml/pytorch/utils/ssd_helpers.py,sha256=05fySE5KNwrt7UF213niHp2STRSeprlU1NbLAjpYRaU,30059
 sparseml/pytorch/utils/yolo_helpers.py,sha256=nFlDPOEWfooq8GrUzKRpr7vS36m9NQMPGZSqCYmGMks,12337
+sparseml/pytorch/utils/sparsification_info/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
+sparseml/pytorch/utils/sparsification_info/configs.py,sha256=lq2RuJWYwrWbtnT2n4eNHtiLcstKyW9YaVhdTms6kqw,10457
+sparseml/pytorch/utils/sparsification_info/helpers.py,sha256=V9sT7dcuAUirBY7wieuwEFL2ENsEv7WdYpQ9lUyoKPg,4309
+sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py,sha256=pdP4gEyKmvV7oZBmkBnJkoR3XOKDouVyupOXWHhWYbU,2946
 sparseml/recipe_template/__init__.py,sha256=0HHlF01-zO71wTzxQ9AE8UvqmXbgoyEEykAVGcyVjWA,655
 sparseml/recipe_template/utils.py,sha256=_ASxYYYJPIkK-Ffsicn9hezlHt6dXBLObCPqh9Uz6zE,4788
 sparseml/sparsification/__init__.py,sha256=YmxZ5Gbbn3zfInFZDA2aH9gM-gK-JRgYTnOgXSNskAQ,1058
 sparseml/sparsification/analyzer.py,sha256=ky-GJNpDUssyN8HBxxqBC_LmUxnaL9eL9Rl2aVgbNgU,9387
 sparseml/sparsification/info.py,sha256=kH1RZJGpz0yHgFVvJaj0WEzID8WCozMjiJdQ5M08PTQ,9065
 sparseml/sparsification/model_info.py,sha256=fNOh_pVc9lGaBLcEf3YIemIbJfZxFNR4JuILvRN-pks,15565
 sparseml/sparsification/modifier_epoch.py,sha256=JKUM2cVQPYGx4vKbpF5IGwQFWM0NevFHc8dq8InQdbQ,2002
 sparseml/sparsification/modifier_lr.py,sha256=-3t0ozub6vfyh9NAgvgRgbyXIP1yu9_URuArr5TdTXg,10117
 sparseml/sparsification/modifier_params.py,sha256=n6O1tD4nsOTeeGJ5ym4hB7PQwSEWNduymW8_ObjAO7g,5505
 sparseml/sparsification/modifier_pruning.py,sha256=7_i4dzdkfOFcD7A_d8cublgX5KB-hyOGOJZtU41JUwU,12845
 sparseml/sparsification/oracle.py,sha256=9J8iIdr_aztwc06tRgw-2ZdGN_1RgJBYWZDY1ZfHhAY,3700
 sparseml/sparsification/recipe_builder.py,sha256=i8cFAkDemk8UXiPff5s9necHXECk6WO2AySnqiqr8MU,18570
 sparseml/sparsification/recipe_editor.py,sha256=6PqExzex1nmMj2a0jkE7JUeeuMTGA27GCH32C9B8V40,14413
 sparseml/sparsification/types.py,sha256=wi05A10SkgSBFmBUtzdHIIMTsY4lPTXP0ycZrBgbub0,1250
-sparseml/tensorflow_v1/__init__.py,sha256=8-ffiWbZ1u7dexBap4ypGN4NQ1-iXFinHiiaTwrFxnU,867
+sparseml/tensorflow_v1/__init__.py,sha256=JfUGMyYgBnal1xMpGR_i0oA4juUVt2QvkbcBZxFZG6w,987
 sparseml/tensorflow_v1/base.py,sha256=PHZOsjEtcG3gEGRdU7tu2jNRAYYo8KrCmPenZyo5IQo,7272
 sparseml/tensorflow_v1/datasets/__init__.py,sha256=X0o7cmzhXhLwjrawfN3pIqrFTKALH_xftMIerzWaLjQ,925
 sparseml/tensorflow_v1/datasets/dataset.py,sha256=t4OfviMyfbn63kNrNiH19blDvoxcxhyBiLgUh03Ryhc,8121
 sparseml/tensorflow_v1/datasets/helpers.py,sha256=mGy1YuQqERWRG-dknPmOspyWtzUinY9GUSEdSPycGF8,5600
 sparseml/tensorflow_v1/datasets/registry.py,sha256=2H2fG0iUQ0h41XVpZp-GHXM3Ti6axePI1O2LQKqSqhI,2768
 sparseml/tensorflow_v1/datasets/classification/__init__.py,sha256=xNLlq5y7_cssxlZZP95CuYioqEiU6TanVbzMCqoCVTo,807
 sparseml/tensorflow_v1/datasets/classification/cifar.py,sha256=_ETXHcC9cPtQbQIoBLgQQd2GC0Ue6kEO3XXpaZY54xg,12686
@@ -300,23 +308,23 @@
 sparseml/tensorflow_v1/utils/__init__.py,sha256=FhgTPE_G6lftVrwrOCUghTMxmi_1TbRwOX3TYJt5X7A,967
 sparseml/tensorflow_v1/utils/exporter.py,sha256=RqpSP-w21SrkA_ik9WoIWdIVAAui88AiBXxRWaDZJJs,10913
 sparseml/tensorflow_v1/utils/helpers.py,sha256=40eZgnejvIki_CdupK4V1gETAgGDE9rbEXEwuNg9ASA,996
 sparseml/tensorflow_v1/utils/loss.py,sha256=4AsXh70fjp1dDcxBUzgjjpLgndwVa1CBiMG1sYi5Was,1974
 sparseml/tensorflow_v1/utils/nets_utils.py,sha256=cOTKgw7PVPEjRVU-bvcsNLdBJGTi-A7djJaUaZQwsT4,8119
 sparseml/tensorflow_v1/utils/summary.py,sha256=A2ub7KDwzsaindIuCHa7N3cRpCU6d7QbD5uNHV-R6H8,1327
 sparseml/tensorflow_v1/utils/variable.py,sha256=6ziLaNOLnxQrSPWJ2RaINqg4w-4NK9reVJWH-weK3-k,12536
-sparseml/transformers/__init__.py,sha256=y1o6PAR5Ruz_f-Qqu7pYI1ENegRW8Ge2Hq5KLd4pO70,4273
+sparseml/transformers/__init__.py,sha256=8J1vljjZiybTTdNXN9e9senxvZUmKXKHAB5-H4D_4nY,1511
 sparseml/transformers/export.py,sha256=JR5cWm0u9pZsn5EiXpJkEZrIHuVLtzSB0js84GsoGn8,19721
-sparseml/transformers/masked_language_modeling.py,sha256=3NVCBveaLUI-BNgTqX5Pm97-apHNFVbyNUDr5z5x1cI,30936
-sparseml/transformers/question_answering.py,sha256=koobYWD4GBcGqWkW1L005QCw4huh5rbFa8rJp_wnWko,36738
-sparseml/transformers/text_classification.py,sha256=9uVAi6vGSl7rF5DHPS005lW0dxOpz2N4ZIXk5-50u8c,40358
-sparseml/transformers/token_classification.py,sha256=6BMBgmEpQvq_RoZzWhLdexQqK4oK9Iv69Qs0IOd-Qds,34464
+sparseml/transformers/masked_language_modeling.py,sha256=xV1H7jyWCWMKTiow501cI498I5ouNC68nF7g-QNuzjw,30756
+sparseml/transformers/question_answering.py,sha256=E_Ljec9bNDrZ2KD3unTlbcRxEpyYU6C9asuEynhh4AQ,36557
+sparseml/transformers/text_classification.py,sha256=NS5fQGq9-BhQB6YOE0lFKA7DpjN2Z04BBj90NCcT5dY,40177
+sparseml/transformers/token_classification.py,sha256=pkbFROBABVavoeCNYozuMLDD5YRYYqSp52TqDNWcAsk,34284
 sparseml/transformers/sparsification/__init__.py,sha256=22XZNePvLFXNxp5NrcUIXzjgynCZm6jvQOErpRGlQNY,833
 sparseml/transformers/sparsification/question_answering.py,sha256=FAXhtQ8MW_2ar1dix2tQ1x1RXZuSWMLHZbVHToNWwmo,19529
-sparseml/transformers/sparsification/trainer.py,sha256=JwbmevvYb5ddqou3b_j8970PQGO267bd37Zt1ahyN9Y,43523
+sparseml/transformers/sparsification/trainer.py,sha256=g2tP2s_W8Pmpef1CuCIsMD_teRkq9ZRIppR0Uq84Mpw,43756
 sparseml/transformers/sparsification/training_args.py,sha256=gGivIDchLi__PZMNQRmzDOaQcQLkUVFystq3LaVko3Y,1890
 sparseml/transformers/utils/__init__.py,sha256=dxyg6b2XznhBzOsduHdOalgTmoX1JC32Rb4AHns6rVk,794
 sparseml/transformers/utils/helpers.py,sha256=pgxtf0ygP7qJEVPse_dGxm7UpWSJ9JVebA_ex1c8Muw,3090
 sparseml/transformers/utils/metrics.py,sha256=ciZsxgdrzlSMnyzbgKOFE3spWsKql0z82BiYFRXiVOU,2536
 sparseml/transformers/utils/model.py,sha256=HlU7NMTEy34eDA1dyqX8AH34GHR3ClwE8DVWD7a5tNM,15797
 sparseml/utils/__init__.py,sha256=-WKBN4DERhw7rTJkarilkyAM9pw4rW8qkXGRPSEJ8SM,844
 sparseml/utils/frameworks.py,sha256=S-cGkbVc6DoWfI6Hu5AkIqF0Vi1PyxKX5GfhwRfpv_E,886
@@ -330,19 +338,31 @@
 sparseml/utils/datasets/coco.py,sha256=5w9Fm0O2kUtrC1upa6DCC4WZ13df-ZlORPUHEwGFDLc,3750
 sparseml/utils/datasets/helpers.py,sha256=1i1jiOoj1q-_Nef5dJBWHoO9v7ZjogggihDjBMNbf_A,1217
 sparseml/utils/datasets/imagenet.py,sha256=qAL7K6tmlfwBY7FI14wcVb-7g3Rzs4wtZIOV1kvoV0w,23366
 sparseml/utils/datasets/imagenette.py,sha256=AIxAI0wfUqu08XPJ1cG8SNUVocjoeFHVepQZDfsztFI,8967
 sparseml/utils/datasets/voc.py,sha256=CzSEnTe-KqWyOLwleame66PtYqF8vuq9EXaNgmms6u0,1009
 sparseml/yolact/COCO.sh,sha256=Q_1I3VZwS4N1e3AwOoimQH2plK2K0athUDWooWR4ZVQ,1875
 sparseml/yolact/COCO_test.sh,sha256=ZoA_h_68zM8EWF510o24_5xBaQtbJLMHenNjSzldYYc,1418
-sparseml/yolact/__init__.py,sha256=g3jqcuxdvDPBE14-ESOOfSFRV6TW3dNERyjkwLoHwd0,3908
+sparseml/yolact/__init__.py,sha256=5t9V0aePHnzJBik6z1r4W_3DsSn0lKpYjl3pIuZQft0,4020
 sparseml/yolact/scripts.py,sha256=7GE3xp_B8JJpa2H-Vum6rmiOJHcChyffuno4-yteUUw,1784
-sparseml/yolov5/__init__.py,sha256=GkDTxi-5WwAG8xjuGA7g5DRXbI9CWBI3bBJoAkNk_YU,3154
+sparseml/yolov5/__init__.py,sha256=LiVvIlHR1FF63Ixm2MabdDH1Ul8sFEUEIb3Sbs4awLI,1440
 sparseml/yolov5/helpers.py,sha256=jxzJrgKjsb0PHTeGevKICaL8iBOUzxwZXvPAyGyVE-c,4505
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
-sparseml-1.4.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml-1.4.4.dist-info/METADATA,sha256=dWJWFS6VeMIEjlJSpKQJ4OPN7jj3hoVKUUYZlw310-4,22025
-sparseml-1.4.4.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml-1.4.4.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml-1.4.4.dist-info/entry_points.txt,sha256=cleX1Ani7yuDYD_K-r1rLlZMRkvVtmroOAzQOj-JvbA,2206
-sparseml-1.4.4.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml-1.4.4.dist-info/RECORD,,
+sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
+sparseml/yolov8/__init__.py,sha256=l6f1TkolWl2ejQQ63jN3VFft7mMpQDURpWDIeflVKGQ,1115
+sparseml/yolov8/default.yaml,sha256=dVDQ77Px58l5jLoVJOdiNGbW-cDn-SdUioHkpG19CXg,5763
+sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
+sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
+sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
+sparseml/yolov8/trainers.py,sha256=-nCtUkmJNGOR48jMn_erjkV22ykd0lMp8PObI0v6Bzk,34525
+sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
+sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
+sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
+sparseml/yolov8/utils/export_samples.py,sha256=YbiV_0cv_W0xrhtZLg6ActLeSRYYikrOzHz0FqJ0LII,6298
+sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
+sparseml-1.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml-1.5.0.dist-info/METADATA,sha256=NNUqkAOG_hJCcHdVxNQw-1W3qWiE9iwF3l33wbPV1bs,21503
+sparseml-1.5.0.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml-1.5.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml-1.5.0.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
+sparseml-1.5.0.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml-1.5.0.dist-info/RECORD,,
```

