# Comparing `tmp/autogluon.multimodal-0.7.1b20230601.tar.gz` & `tmp/autogluon.multimodal-0.7.1b20230602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.7.1b20230601.tar", last modified: Thu Jun  1 09:04:05 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.7.1b20230602.tar", last modified: Fri Jun  2 09:04:01 2023, max compression
```

## Comparing `autogluon.multimodal-0.7.1b20230601.tar` & `autogluon.multimodal-0.7.1b20230602.tar`

### file list

```diff
@@ -1,153 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.205301 autogluon.multimodal-0.7.1b20230601/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-01 09:04:05.201301 autogluon.multimodal-0.7.1b20230601/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:04:05.205301 autogluon.multimodal-0.7.1b20230601/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.185301 autogluon.multimodal-0.7.1b20230601/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.185301 autogluon.multimodal-0.7.1b20230601/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8x8_300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.193301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.193301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.193301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    82611 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.197301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.197301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.197301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   118889 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.201301 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-01 09:03:27.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 09:04:05.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:04:05.189301 autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-01 09:04:05.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-01 09:04:05.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:04:05.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:04:05.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-01 09:04:05.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:04:05.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:04:05.000000 autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.901665 autogluon.multimodal-0.7.1b20230602/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-02 09:04:01.901665 autogluon.multimodal-0.7.1b20230602/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:04:01.901665 autogluon.multimodal-0.7.1b20230602/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.885664 autogluon.multimodal-0.7.1b20230602/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.885664 autogluon.multimodal-0.7.1b20230602/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33147 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82611 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.897664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.897664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.897664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118702 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.901665 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53333 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.7.1b20230601/PKG-INFO` & `autogluon.multimodal-0.7.1b20230602/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230601
+Version: 0.7.1b20230602
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230601/setup.py` & `autogluon.multimodal-0.7.1b20230602/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "sentencepiece>=0.1.95,<0.2.0",
     f"autogluon.core[raytune]=={version}",
     f"autogluon.features=={version}",
     f"autogluon.common=={version}",
     "pytorch-metric-learning>=1.3.0,<2.0",
     "nlpaug>=1.1.10,<1.2.0",
     "nltk>=3.4.5,<4.0.0",
-    "openmim>0.1.5,<0.4.0",
+    "openmim>=0.3.7,<0.4.0",
     "defusedxml>=0.7.1,<0.7.2",
     "jinja2>=3.0.3,<3.2",
     "tensorboard>=2.9,<3",
     "pytesseract>=0.3.9,<0.3.11",
     "PyMuPDF<=1.21.1",
 ]
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,148 +1,111 @@
-_base_ = ["../schedule_1x.py", "../default_runtime.py"]
+_base_ = ["../schedule_1x.py", "../default_runtime.py", "./yolox_tta.py"]
 
-img_scale = (640, 640)  # height, width
+img_scale = (640, 640)  # width, height
 
 # model settings
 model = dict(
     type="YOLOX",
-    input_size=img_scale,
-    random_size_range=(15, 25),
-    random_size_interval=10,
-    backbone=dict(type="CSPDarknet", deepen_factor=0.33, widen_factor=0.5),
-    neck=dict(type="YOLOXPAFPN", in_channels=[128, 256, 512], out_channels=128, num_csp_blocks=1),
-    bbox_head=dict(type="YOLOXHead", num_classes=80, in_channels=128, feat_channels=128),
+    data_preprocessor=dict(
+        type="DetDataPreprocessor",
+        pad_size_divisor=32,
+        batch_augments=[
+            dict(type="BatchSyncRandomResize", random_size_range=(480, 800), size_divisor=32, interval=10)
+        ],
+    ),
+    backbone=dict(
+        type="CSPDarknet",
+        deepen_factor=0.33,
+        widen_factor=0.5,
+        out_indices=(2, 3, 4),
+        use_depthwise=False,
+        spp_kernal_sizes=(5, 9, 13),
+        norm_cfg=dict(type="BN", momentum=0.03, eps=0.001),
+        act_cfg=dict(type="Swish"),
+    ),
+    neck=dict(
+        type="YOLOXPAFPN",
+        in_channels=[128, 256, 512],
+        out_channels=128,
+        num_csp_blocks=1,
+        use_depthwise=False,
+        upsample_cfg=dict(scale_factor=2, mode="nearest"),
+        norm_cfg=dict(type="BN", momentum=0.03, eps=0.001),
+        act_cfg=dict(type="Swish"),
+    ),
+    bbox_head=dict(
+        type="YOLOXHead",
+        num_classes=80,
+        in_channels=128,
+        feat_channels=128,
+        stacked_convs=2,
+        strides=(8, 16, 32),
+        use_depthwise=False,
+        norm_cfg=dict(type="BN", momentum=0.03, eps=0.001),
+        act_cfg=dict(type="Swish"),
+        loss_cls=dict(type="CrossEntropyLoss", use_sigmoid=True, reduction="sum", loss_weight=1.0),
+        loss_bbox=dict(type="IoULoss", mode="square", eps=1e-16, reduction="sum", loss_weight=5.0),
+        loss_obj=dict(type="CrossEntropyLoss", use_sigmoid=True, reduction="sum", loss_weight=1.0),
+        loss_l1=dict(type="L1Loss", reduction="sum", loss_weight=1.0),
+    ),
     train_cfg=dict(assigner=dict(type="SimOTAAssigner", center_radius=2.5)),
     # In order to align the source code, the threshold of the val phase is
     # 0.01, and the threshold of the test phase is 0.001.
     test_cfg=dict(score_thr=0.01, nms=dict(type="nms", iou_threshold=0.65)),
 )
 
-# dataset settings
-data_root = "data/coco/"
-dataset_type = "CocoDataset"
-
 loading_pipeline = [
     dict(type="LoadImageFromFile"),
     dict(type="LoadAnnotations", with_bbox=True),
 ]
 
 multi_image_mix_dataset = dict(
     mosaic=dict(
-        img_scale=(640, 640),
+        img_scale=img_scale,
         center_ratio_range=(0.5, 1.5),
-        min_bbox_size=0,
         bbox_clip_border=True,
-        skip_filter=True,
-        pad_val=114,
+        pad_val=114.0,
         prob=0.5,
     ),
+    # TODO: add random affine    dict(
+    # RandomAffine=dict(
+    #     scaling_ratio_range=(0.1, 2),
+    #     # img_scale is (width, height)
+    #     border=(-img_scale[0] // 2, -img_scale[1] // 2),
+    # ),
     mixup=dict(
-        img_scale=(640, 640),
+        img_scale=img_scale,
         ratio_range=(0.8, 1.6),
         flip_ratio=0.5,
-        pad_val=114,
+        pad_val=114.0,
         max_iters=15,
-        min_bbox_size=5,
-        min_area_ratio=0.2,
-        max_aspect_ratio=20,
         bbox_clip_border=True,
-        skip_filter=True,
-        prob=0.5,
     ),
 )
 
 train_pipeline = [
     dict(type="YOLOXHSVRandomAug"),
-    dict(type="RandomFlip", flip_ratio=0.5),
+    dict(type="RandomFlip", prob=0.5),
     # According to the official implementation, multi-scale
     # training is not considered here but in the
     # 'mmdet/models/detectors/yolox.py'.
-    dict(type="Resize", img_scale=img_scale, keep_ratio=True),
+    # Resize and Pad are for the last 15 epochs when Mosaic,
+    # RandomAffine, and MixUp are closed by YOLOXModeSwitchHook.
+    dict(type="Resize", scale=img_scale, keep_ratio=True),
     dict(
         type="Pad",
         pad_to_square=True,
         # If the image is three-channel, the pad value needs
         # to be set separately for each channel.
         pad_val=dict(img=(114.0, 114.0, 114.0)),
     ),
     dict(type="FilterAnnotations", min_gt_bbox_wh=(1, 1), keep_empty=False),
-    dict(type="DefaultFormatBundle"),
-    dict(type="Collect", keys=["img", "gt_bboxes", "gt_labels"]),
+    dict(type="PackDetInputs"),
 ]
 
 test_pipeline = [
     dict(type="LoadImageFromFile"),
-    dict(
-        type="MultiScaleFlipAug",
-        img_scale=img_scale,
-        flip=False,
-        transforms=[
-            dict(type="Resize", keep_ratio=True),
-            dict(type="RandomFlip"),
-            dict(type="Pad", pad_to_square=True, pad_val=dict(img=(114.0, 114.0, 114.0))),
-            dict(type="DefaultFormatBundle"),
-            dict(type="Collect", keys=["img"]),
-        ],
-    ),
-]
-
-data = dict(
-    train=dict(dataset=dict(pipeline=train_pipeline)),
-    val=dict(pipeline=test_pipeline),
-    test=dict(pipeline=test_pipeline),
-)
-
-# optimizer
-# default 8 gpu
-optimizer = dict(
-    type="SGD",
-    lr=0.01,
-    momentum=0.9,
-    weight_decay=5e-4,
-    nesterov=True,
-    paramwise_cfg=dict(norm_decay_mult=0.0, bias_decay_mult=0.0),
-)
-optimizer_config = dict(grad_clip=None)
-
-max_epochs = 300
-num_last_epochs = 15
-resume_from = None
-interval = 10
-
-# learning policy
-lr_config = dict(
-    _delete_=True,
-    policy="YOLOX",
-    warmup="exp",
-    by_epoch=False,
-    warmup_by_epoch=True,
-    warmup_ratio=1,
-    warmup_iters=5,  # 5 epoch
-    num_last_epochs=num_last_epochs,
-    min_lr_ratio=0.05,
-)
-
-runner = dict(type="EpochBasedRunner", max_epochs=max_epochs)
-
-custom_hooks = [
-    dict(type="YOLOXModeSwitchHook", num_last_epochs=num_last_epochs, priority=48),
-    dict(type="SyncNormHook", num_last_epochs=num_last_epochs, interval=interval, priority=48),
-    dict(type="ExpMomentumEMAHook", resume_from=resume_from, momentum=0.0001, priority=49),
+    dict(type="Resize", scale=img_scale, keep_ratio=True),
+    dict(type="Pad", pad_to_square=True, pad_val=dict(img=(114.0, 114.0, 114.0))),
+    dict(type="LoadAnnotations", with_bbox=True),
+    dict(type="PackDetInputs", meta_keys=("img_id", "img_path", "ori_shape", "img_shape", "scale_factor")),
 ]
-checkpoint_config = dict(interval=interval)
-evaluation = dict(
-    save_best="auto",
-    # The evaluation interval is 'interval' when running epoch is
-    # less than ‘max_epochs - num_last_epochs’.
-    # The evaluation interval is 1 when running epoch is greater than
-    # or equal to ‘max_epochs - num_last_epochs’.
-    interval=interval,
-    dynamic_intervals=[(max_epochs - num_last_epochs, 1)],
-    metric="bbox",
-)
-log_config = dict(interval=50)
-
-# NOTE: `auto_scale_lr` is for automatically scaling LR,
-# USER SHOULD NOT CHANGE ITS VALUES.
-# base_batch_size = (8 GPUs) x (8 samples per GPU)
-auto_scale_lr = dict(base_batch_size=64)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 import collections
 import copy
 import logging
-from typing import Dict, List, Optional, Union
+import math
+from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import torch
+from numpy import random
 
-from ...constants import AUTOMM, GET_ITEM_ERROR_RETRY, MULTI_IMAGE_MIX_DATASET, ROIS
+from ...constants import GET_ITEM_ERROR_RETRY, MULTI_IMAGE_MIX_DATASET, ROIS
 from ..preprocess_dataframe import MultiModalFeaturePreprocessor
 from ..utils import apply_data_processor, apply_df_preprocessor, get_per_sample_features
 
 logger = logging.getLogger(__name__)
 
 try:
     import mmcv
     from mmcv.utils import Config as MMCVConfig
-    from mmdet.core import find_inside_bboxes
-    from mmdet.utils import log_img_scale  # inline import to avoid mmdet uninstall error for other tasks
 except:
     MMCVConfig = None
 
+try:
+    from mmcv.transforms import BaseTransform
+    from mmcv.transforms.utils import cache_randomness
+except:
+    pass
+
+try:
+    from mmengine.dataset import BaseDataset
+except:
+    pass
+
+try:
+    from mmdet.structures.bbox import autocast_box_type
+    from mmdet.utils import log_img_scale  # inline import to avoid mmdet uninstall error for other tasks
+except:
+    pass
+
 
 class MultiImageMixDataset(torch.utils.data.Dataset):
     """
     A Pytorch DataSet class to process a multimodal pd.DataFrame. It first uses a preprocessor to
     produce model-agnostic features. Then, each processor prepares customized data for one modality
     per model. For code simplicity, here we treat ground-truth label as one modality. This class is
     independent of specific data modalities and models.
@@ -212,16 +229,16 @@
                 is_training=True,  # This dataset is used only in training
             )
         )
 
         return results
 
 
-class Mosaic:
-    """Mosaic augmentation. Code retrieved from mmdetection and modified.
+class Mosaic(BaseTransform):
+    """Mosaic augmentation.
 
     Given 4 images, mosaic transform combines them into
     one output image. The output image is composed of the parts from each sub-
     image.
 
     .. code:: text
 
@@ -245,172 +262,164 @@
      The mosaic transform steps are as follows:
 
          1. Choose the mosaic center as the intersections of 4 images
          2. Get the left top image according to the index, and randomly
             sample another 3 images from the custom dataset.
          3. Sub image will be cropped if image is larger than mosaic patch
 
+    Required Keys:
+
+    - img
+    - gt_bboxes (BaseBoxes[torch.float32]) (optional)
+    - gt_bboxes_labels (np.int64) (optional)
+    - gt_ignore_flags (bool) (optional)
+    - mix_results (List[dict])
+
+    Modified Keys:
+
+    - img
+    - img_shape
+    - gt_bboxes (optional)
+    - gt_bboxes_labels (optional)
+    - gt_ignore_flags (optional)
+
     Args:
         img_scale (Sequence[int]): Image size after mosaic pipeline of single
-            image. The shape order should be (height, width).
-            Default to (640, 640).
+            image. The shape order should be (width, height).
+            Defaults to (640, 640).
         center_ratio_range (Sequence[float]): Center ratio range of mosaic
-            output. Default to (0.5, 1.5).
-        min_bbox_size (int | float): The minimum pixel for filtering
-            invalid bboxes after the mosaic pipeline. Default to 0.
+            output. Defaults to (0.5, 1.5).
         bbox_clip_border (bool, optional): Whether to clip the objects outside
             the border of the image. In some dataset like MOT17, the gt bboxes
             are allowed to cross the border of images. Therefore, we don't
             need to clip the gt bboxes in these cases. Defaults to True.
-        skip_filter (bool): Whether to skip filtering rules. If it
-            is True, the filter rule will not be applied, and the
-            `min_bbox_size` is invalid. Default to True.
-        pad_val (int): Pad value. Default to 114.
+        pad_val (int): Pad value. Defaults to 114.
         prob (float): Probability of applying this transformation.
-            Default to 1.0.
+            Defaults to 1.0.
     """
 
     def __init__(
         self,
-        img_scale=(640, 640),
-        center_ratio_range=(0.5, 1.5),
-        min_bbox_size=0,
-        bbox_clip_border=True,
-        skip_filter=True,
-        pad_val=114,
-        prob=1.0,
-    ):
-
+        img_scale: Tuple[int, int] = (640, 640),
+        center_ratio_range: Tuple[float, float] = (0.5, 1.5),
+        bbox_clip_border: bool = True,
+        pad_val: float = 114.0,
+        prob: float = 1.0,
+    ) -> None:
         assert isinstance(img_scale, tuple)
         assert 0 <= prob <= 1.0, "The probability should be in range [0,1]. " f"got {prob}."
 
-        log_img_scale(img_scale, skip_square=True)
+        log_img_scale(img_scale, skip_square=True, shape_order="wh")
         self.img_scale = img_scale
         self.center_ratio_range = center_ratio_range
-        self.min_bbox_size = min_bbox_size
         self.bbox_clip_border = bbox_clip_border
-        self.skip_filter = skip_filter
         self.pad_val = pad_val
         self.prob = prob
 
-    def __call__(self, results):
-        """Call function to make a mosaic of image.
-
-        Args:
-            results (dict): Result dict.
-
-        Returns:
-            dict: Result dict with mosaic transformed.
-        """
-
-        if np.random.uniform(0, 1) > self.prob:
-            return results
-
-        results = self._mosaic_transform(results)
-        return results
-
-    def get_indexes(self, dataset):
+    @cache_randomness
+    def get_indexes(self, dataset: BaseDataset) -> int:
         """Call function to collect indexes.
 
         Args:
             dataset (:obj:`MultiImageMixDataset`): The dataset.
 
         Returns:
             list: indexes.
         """
 
-        indexes = [np.random.randint(0, len(dataset)) for _ in range(3)]
+        indexes = [random.randint(0, len(dataset)) for _ in range(3)]
         return indexes
 
-    def _mosaic_transform(self, results):
+    @autocast_box_type()
+    def transform(self, results: dict) -> dict:
         """Mosaic transform function.
 
         Args:
             results (dict): Result dict.
 
         Returns:
             dict: Updated result dict.
         """
+        if random.uniform(0, 1) > self.prob:
+            return results
 
         assert "mix_results" in results
-        mosaic_labels = []
         mosaic_bboxes = []
-        img = results["img"]  # CHW in torch tensor to HWC in numpy
-        if len(img.shape) == 3:
+        mosaic_bboxes_labels = []
+        mosaic_ignore_flags = []
+        if len(results["img"].shape) == 3:
             mosaic_img = np.full(
-                (int(self.img_scale[0] * 2), int(self.img_scale[1] * 2), 3), self.pad_val, dtype=img.dtype
+                (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2), 3), self.pad_val, dtype=results["img"].dtype
             )
         else:
             mosaic_img = np.full(
-                (int(self.img_scale[0] * 2), int(self.img_scale[1] * 2)), self.pad_val, dtype=img.dtype
+                (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2)), self.pad_val, dtype=results["img"].dtype
             )
 
         # mosaic center x, y
-        center_x = int(np.random.uniform(*self.center_ratio_range) * self.img_scale[1])
-        center_y = int(np.random.uniform(*self.center_ratio_range) * self.img_scale[0])
+        center_x = int(random.uniform(*self.center_ratio_range) * self.img_scale[0])
+        center_y = int(random.uniform(*self.center_ratio_range) * self.img_scale[1])
         center_position = (center_x, center_y)
 
         loc_strs = ("top_left", "top_right", "bottom_left", "bottom_right")
         for i, loc in enumerate(loc_strs):
             if loc == "top_left":
                 results_patch = copy.deepcopy(results)
             else:
                 results_patch = copy.deepcopy(results["mix_results"][i - 1])
 
             img_i = results_patch["img"]
             h_i, w_i = img_i.shape[:2]
             # keep_ratio resize
-            scale_ratio_i = min(self.img_scale[0] / h_i, self.img_scale[1] / w_i)
+            scale_ratio_i = min(self.img_scale[1] / h_i, self.img_scale[0] / w_i)
             img_i = mmcv.imresize(img_i, (int(w_i * scale_ratio_i), int(h_i * scale_ratio_i)))
 
             # compute the combine parameters
             paste_coord, crop_coord = self._mosaic_combine(loc, center_position, img_i.shape[:2][::-1])
             x1_p, y1_p, x2_p, y2_p = paste_coord
             x1_c, y1_c, x2_c, y2_c = crop_coord
 
             # crop and paste image
             mosaic_img[y1_p:y2_p, x1_p:x2_p] = img_i[y1_c:y2_c, x1_c:x2_c]
 
             # adjust coordinate
             gt_bboxes_i = results_patch["gt_bboxes"]
-            gt_labels_i = results_patch["gt_labels"]
-
-            if gt_bboxes_i.shape[0] > 0:
-                padw = x1_p - x1_c
-                padh = y1_p - y1_c
-                gt_bboxes_i[:, 0::2] = scale_ratio_i * gt_bboxes_i[:, 0::2] + padw
-                gt_bboxes_i[:, 1::2] = scale_ratio_i * gt_bboxes_i[:, 1::2] + padh
+            gt_bboxes_labels_i = results_patch["gt_bboxes_labels"]
+            gt_ignore_flags_i = results_patch["gt_ignore_flags"]
 
+            padw = x1_p - x1_c
+            padh = y1_p - y1_c
+            gt_bboxes_i.rescale_([scale_ratio_i, scale_ratio_i])
+            gt_bboxes_i.translate_([padw, padh])
             mosaic_bboxes.append(gt_bboxes_i)
-            mosaic_labels.append(gt_labels_i)
+            mosaic_bboxes_labels.append(gt_bboxes_labels_i)
+            mosaic_ignore_flags.append(gt_ignore_flags_i)
 
-        if len(mosaic_labels) > 0:
-            mosaic_bboxes = np.concatenate(mosaic_bboxes, 0)
-            mosaic_labels = np.concatenate(mosaic_labels, 0)
-
-            if self.bbox_clip_border:
-                mosaic_bboxes[:, 0::2] = np.clip(mosaic_bboxes[:, 0::2], 0, 2 * self.img_scale[1])
-                mosaic_bboxes[:, 1::2] = np.clip(mosaic_bboxes[:, 1::2], 0, 2 * self.img_scale[0])
-
-            if not self.skip_filter:
-                mosaic_bboxes, mosaic_labels = self._filter_box_candidates(mosaic_bboxes, mosaic_labels)
+        mosaic_bboxes = mosaic_bboxes[0].cat(mosaic_bboxes, 0)
+        mosaic_bboxes_labels = np.concatenate(mosaic_bboxes_labels, 0)
+        mosaic_ignore_flags = np.concatenate(mosaic_ignore_flags, 0)
 
+        if self.bbox_clip_border:
+            mosaic_bboxes.clip_([2 * self.img_scale[1], 2 * self.img_scale[0]])
         # remove outside bboxes
-        inside_inds = find_inside_bboxes(mosaic_bboxes, 2 * self.img_scale[0], 2 * self.img_scale[1])
+        inside_inds = mosaic_bboxes.is_inside([2 * self.img_scale[1], 2 * self.img_scale[0]]).numpy()
         mosaic_bboxes = mosaic_bboxes[inside_inds]
-        mosaic_labels = mosaic_labels[inside_inds]
+        mosaic_bboxes_labels = mosaic_bboxes_labels[inside_inds]
+        mosaic_ignore_flags = mosaic_ignore_flags[inside_inds]
 
         results["img"] = mosaic_img
-        results["img_shape"] = mosaic_img.shape
+        results["img_shape"] = mosaic_img.shape[:2]
         results["gt_bboxes"] = mosaic_bboxes
-        results["gt_labels"] = mosaic_labels
-
+        results["gt_bboxes_labels"] = mosaic_bboxes_labels
+        results["gt_ignore_flags"] = mosaic_ignore_flags
         return results
 
-    def _mosaic_combine(self, loc, center_position_xy, img_shape_wh):
+    def _mosaic_combine(
+        self, loc: str, center_position_xy: Sequence[float], img_shape_wh: Sequence[int]
+    ) -> Tuple[Tuple[int], Tuple[int]]:
         """Calculate global coordinate of mosaic image and local coordinate of
         cropped sub-image.
 
         Args:
             loc (str): Index for the sub-image, loc in ('top_left',
               'top_right', 'bottom_left', 'bottom_right').
             center_position_xy (Sequence[float]): Mixing center for 4 images,
@@ -435,62 +444,53 @@
             crop_coord = img_shape_wh[0] - (x2 - x1), img_shape_wh[1] - (y2 - y1), img_shape_wh[0], img_shape_wh[1]
 
         elif loc == "top_right":
             # index1 to top right part of image
             x1, y1, x2, y2 = (
                 center_position_xy[0],
                 max(center_position_xy[1] - img_shape_wh[1], 0),
-                min(center_position_xy[0] + img_shape_wh[0], self.img_scale[1] * 2),
+                min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
                 center_position_xy[1],
             )
             crop_coord = 0, img_shape_wh[1] - (y2 - y1), min(img_shape_wh[0], x2 - x1), img_shape_wh[1]
 
         elif loc == "bottom_left":
             # index2 to bottom left part of image
             x1, y1, x2, y2 = (
                 max(center_position_xy[0] - img_shape_wh[0], 0),
                 center_position_xy[1],
                 center_position_xy[0],
-                min(self.img_scale[0] * 2, center_position_xy[1] + img_shape_wh[1]),
+                min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
             )
             crop_coord = img_shape_wh[0] - (x2 - x1), 0, img_shape_wh[0], min(y2 - y1, img_shape_wh[1])
 
         else:
             # index3 to bottom right part of image
             x1, y1, x2, y2 = (
                 center_position_xy[0],
                 center_position_xy[1],
-                min(center_position_xy[0] + img_shape_wh[0], self.img_scale[1] * 2),
-                min(self.img_scale[0] * 2, center_position_xy[1] + img_shape_wh[1]),
+                min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
+                min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
             )
             crop_coord = 0, 0, min(img_shape_wh[0], x2 - x1), min(y2 - y1, img_shape_wh[1])
 
         paste_coord = x1, y1, x2, y2
         return paste_coord, crop_coord
 
-    def _filter_box_candidates(self, bboxes, labels):
-        """Filter out bboxes too small after Mosaic."""
-        bbox_w = bboxes[:, 2] - bboxes[:, 0]
-        bbox_h = bboxes[:, 3] - bboxes[:, 1]
-        valid_inds = (bbox_w > self.min_bbox_size) & (bbox_h > self.min_bbox_size)
-        valid_inds = np.nonzero(valid_inds)[0]
-        return bboxes[valid_inds], labels[valid_inds]
-
     def __repr__(self):
         repr_str = self.__class__.__name__
-        repr_str += f"img_scale={self.img_scale}, "
+        repr_str += f"(img_scale={self.img_scale}, "
         repr_str += f"center_ratio_range={self.center_ratio_range}, "
         repr_str += f"pad_val={self.pad_val}, "
-        repr_str += f"min_bbox_size={self.min_bbox_size}, "
-        repr_str += f"skip_filter={self.skip_filter})"
+        repr_str += f"prob={self.prob})"
         return repr_str
 
 
-class MixUp:
-    """MixUp data augmentation. Code retrieved from mmdetection and modified.
+class MixUp(BaseTransform):
+    """MixUp data augmentation.
 
     .. code:: text
 
                          mixup transform
                 +------------------------------+
                 | mixup image   |              |
                 |      +--------|--------+     |
@@ -507,108 +507,84 @@
      The mixup transform steps are as follows:
 
         1. Another random image is picked by dataset and embedded in
            the top left patch(after padding and resizing)
         2. The target of mixup transform is the weighted average of mixup
            image and origin image.
 
+    Required Keys:
+
+    - img
+    - gt_bboxes (BaseBoxes[torch.float32]) (optional)
+    - gt_bboxes_labels (np.int64) (optional)
+    - gt_ignore_flags (bool) (optional)
+    - mix_results (List[dict])
+
+
+    Modified Keys:
+
+    - img
+    - img_shape
+    - gt_bboxes (optional)
+    - gt_bboxes_labels (optional)
+    - gt_ignore_flags (optional)
+
+
     Args:
         img_scale (Sequence[int]): Image output size after mixup pipeline.
-            The shape order should be (height, width). Default: (640, 640).
+            The shape order should be (width, height). Defaults to (640, 640).
         ratio_range (Sequence[float]): Scale ratio of mixup image.
-            Default: (0.5, 1.5).
+            Defaults to (0.5, 1.5).
         flip_ratio (float): Horizontal flip ratio of mixup image.
-            Default: 0.5.
-        pad_val (int): Pad value. Default: 114.
+            Defaults to 0.5.
+        pad_val (int): Pad value. Defaults to 114.
         max_iters (int): The maximum number of iterations. If the number of
             iterations is greater than `max_iters`, but gt_bbox is still
-            empty, then the iteration is terminated. Default: 15.
-        min_bbox_size (float): Width and height threshold to filter bboxes.
-            If the height or width of a box is smaller than this value, it
-            will be removed. Default: 5.
-        min_area_ratio (float): Threshold of area ratio between
-            original bboxes and wrapped bboxes. If smaller than this value,
-            the box will be removed. Default: 0.2.
-        max_aspect_ratio (float): Aspect ratio of width and height
-            threshold to filter bboxes. If max(h/w, w/h) larger than this
-            value, the box will be removed. Default: 20.
+            empty, then the iteration is terminated. Defaults to 15.
         bbox_clip_border (bool, optional): Whether to clip the objects outside
             the border of the image. In some dataset like MOT17, the gt bboxes
             are allowed to cross the border of images. Therefore, we don't
             need to clip the gt bboxes in these cases. Defaults to True.
-        skip_filter (bool): Whether to skip filtering rules. If it
-            is True, the filter rule will not be applied, and the
-            `min_bbox_size` and `min_area_ratio` and `max_aspect_ratio`
-            is invalid. Default to True.
     """
 
     def __init__(
         self,
-        img_scale=(640, 640),
-        ratio_range=(0.5, 1.5),
-        flip_ratio=0.5,
-        pad_val=114,
-        max_iters=15,
-        min_bbox_size=5,
-        min_area_ratio=0.2,
-        max_aspect_ratio=20,
-        bbox_clip_border=True,
-        skip_filter=True,
-        prob=1.0,
-    ):
-        import mmcv
-        from mmdet.core import find_inside_bboxes
-        from mmdet.utils import log_img_scale  # inline import to avoid mmdet uninstall error for other tasks
-
+        img_scale: Tuple[int, int] = (640, 640),
+        ratio_range: Tuple[float, float] = (0.5, 1.5),
+        flip_ratio: float = 0.5,
+        pad_val: float = 114.0,
+        max_iters: int = 15,
+        bbox_clip_border: bool = True,
+    ) -> None:
         assert isinstance(img_scale, tuple)
-        assert 0 <= prob <= 1.0, "The probability should be in range [0,1]. " f"got {prob}."
-
-        log_img_scale(img_scale, skip_square=True)
+        log_img_scale(img_scale, skip_square=True, shape_order="wh")
         self.dynamic_scale = img_scale
         self.ratio_range = ratio_range
         self.flip_ratio = flip_ratio
         self.pad_val = pad_val
         self.max_iters = max_iters
-        self.min_bbox_size = min_bbox_size
-        self.min_area_ratio = min_area_ratio
-        self.max_aspect_ratio = max_aspect_ratio
         self.bbox_clip_border = bbox_clip_border
-        self.skip_filter = skip_filter
-        self.prob = prob
-
-    def __call__(self, results):
-        """Call function to make a mixup of image.
 
-        Args:
-            results (dict): Result dict.
-
-        Returns:
-            dict: Result dict with mixup transformed.
-        """
-        if np.random.uniform(0, 1) > self.prob:
-            return results
-
-        results = self._mixup_transform(results)
-        return results
-
-    def get_indexes(self, dataset):
+    @cache_randomness
+    def get_indexes(self, dataset: BaseDataset) -> int:
         """Call function to collect indexes.
 
         Args:
             dataset (:obj:`MultiImageMixDataset`): The dataset.
 
         Returns:
             list: indexes.
         """
 
         index = [np.random.randint(0, len(dataset)) for _ in range(1)]
 
         return index
 
-    def _mixup_transform(self, results):
+    @autocast_box_type()
+    def transform(self, results: dict) -> dict:
         """MixUp transform function.
 
         Args:
             results (dict): Result dict.
 
         Returns:
             dict: Updated result dict.
@@ -620,26 +596,26 @@
         if results["mix_results"][0]["gt_bboxes"].shape[0] == 0:
             # empty bbox
             return results
 
         retrieve_results = results["mix_results"][0]
         retrieve_img = retrieve_results["img"]
 
-        jit_factor = np.random.uniform(*self.ratio_range)
-        is_filp = np.random.uniform(0, 1) < self.flip_ratio
+        jit_factor = random.uniform(*self.ratio_range)
+        is_filp = random.uniform(0, 1) > self.flip_ratio
 
         if len(retrieve_img.shape) == 3:
             out_img = (
-                np.ones((self.dynamic_scale[0], self.dynamic_scale[1], 3), dtype=retrieve_img.dtype) * self.pad_val
+                np.ones((self.dynamic_scale[1], self.dynamic_scale[0], 3), dtype=retrieve_img.dtype) * self.pad_val
             )
         else:
-            out_img = np.ones(self.dynamic_scale, dtype=retrieve_img.dtype) * self.pad_val
+            out_img = np.ones(self.dynamic_scale[::-1], dtype=retrieve_img.dtype) * self.pad_val
 
         # 1. keep_ratio resize
-        scale_ratio = min(self.dynamic_scale[0] / retrieve_img.shape[0], self.dynamic_scale[1] / retrieve_img.shape[1])
+        scale_ratio = min(self.dynamic_scale[1] / retrieve_img.shape[0], self.dynamic_scale[0] / retrieve_img.shape[1])
         retrieve_img = mmcv.imresize(
             retrieve_img, (int(retrieve_img.shape[1] * scale_ratio), int(retrieve_img.shape[0] * scale_ratio))
         )
 
         # 2. paste
         out_img[: retrieve_img.shape[0], : retrieve_img.shape[1]] = retrieve_img
 
@@ -651,91 +627,224 @@
         if is_filp:
             out_img = out_img[:, ::-1, :]
 
         # 5. random crop
         ori_img = results["img"]
         origin_h, origin_w = out_img.shape[:2]
         target_h, target_w = ori_img.shape[:2]
-        padded_img = np.zeros((max(origin_h, target_h), max(origin_w, target_w), 3)).astype(np.uint8)
+        padded_img = np.ones((max(origin_h, target_h), max(origin_w, target_w), 3)) * self.pad_val
+        padded_img = padded_img.astype(np.uint8)
         padded_img[:origin_h, :origin_w] = out_img
 
         x_offset, y_offset = 0, 0
         if padded_img.shape[0] > target_h:
-            y_offset = np.random.randint(0, padded_img.shape[0] - target_h)
+            y_offset = random.randint(0, padded_img.shape[0] - target_h)
         if padded_img.shape[1] > target_w:
-            x_offset = np.random.randint(0, padded_img.shape[1] - target_w)
+            x_offset = random.randint(0, padded_img.shape[1] - target_w)
         padded_cropped_img = padded_img[y_offset : y_offset + target_h, x_offset : x_offset + target_w]
 
         # 6. adjust bbox
         retrieve_gt_bboxes = retrieve_results["gt_bboxes"]
-        retrieve_gt_bboxes[:, 0::2] = retrieve_gt_bboxes[:, 0::2] * scale_ratio
-        retrieve_gt_bboxes[:, 1::2] = retrieve_gt_bboxes[:, 1::2] * scale_ratio
+        retrieve_gt_bboxes.rescale_([scale_ratio, scale_ratio])
         if self.bbox_clip_border:
-            retrieve_gt_bboxes[:, 0::2] = np.clip(retrieve_gt_bboxes[:, 0::2], 0, origin_w)
-            retrieve_gt_bboxes[:, 1::2] = np.clip(retrieve_gt_bboxes[:, 1::2], 0, origin_h)
+            retrieve_gt_bboxes.clip_([origin_h, origin_w])
 
         if is_filp:
-            retrieve_gt_bboxes[:, 0::2] = origin_w - retrieve_gt_bboxes[:, 0::2][:, ::-1]
+            retrieve_gt_bboxes.flip_([origin_h, origin_w], direction="horizontal")
 
         # 7. filter
-        cp_retrieve_gt_bboxes = retrieve_gt_bboxes.copy()
-        cp_retrieve_gt_bboxes[:, 0::2] = cp_retrieve_gt_bboxes[:, 0::2] - x_offset
-        cp_retrieve_gt_bboxes[:, 1::2] = cp_retrieve_gt_bboxes[:, 1::2] - y_offset
+        cp_retrieve_gt_bboxes = retrieve_gt_bboxes.clone()
+        cp_retrieve_gt_bboxes.translate_([-x_offset, -y_offset])
         if self.bbox_clip_border:
-            cp_retrieve_gt_bboxes[:, 0::2] = np.clip(cp_retrieve_gt_bboxes[:, 0::2], 0, target_w)
-            cp_retrieve_gt_bboxes[:, 1::2] = np.clip(cp_retrieve_gt_bboxes[:, 1::2], 0, target_h)
+            cp_retrieve_gt_bboxes.clip_([target_h, target_w])
 
         # 8. mix up
         ori_img = ori_img.astype(np.float32)
         mixup_img = 0.5 * ori_img + 0.5 * padded_cropped_img.astype(np.float32)
 
-        retrieve_gt_labels = retrieve_results["gt_labels"]
-        if not self.skip_filter:
-            keep_list = self._filter_box_candidates(retrieve_gt_bboxes.T, cp_retrieve_gt_bboxes.T)
-
-            retrieve_gt_labels = retrieve_gt_labels[keep_list]
-            cp_retrieve_gt_bboxes = cp_retrieve_gt_bboxes[keep_list]
+        retrieve_gt_bboxes_labels = retrieve_results["gt_bboxes_labels"]
+        retrieve_gt_ignore_flags = retrieve_results["gt_ignore_flags"]
 
-        mixup_gt_bboxes = np.concatenate((results["gt_bboxes"], cp_retrieve_gt_bboxes), axis=0)
-        mixup_gt_labels = np.concatenate((results["gt_labels"], retrieve_gt_labels), axis=0)
+        mixup_gt_bboxes = cp_retrieve_gt_bboxes.cat((results["gt_bboxes"], cp_retrieve_gt_bboxes), dim=0)
+        mixup_gt_bboxes_labels = np.concatenate((results["gt_bboxes_labels"], retrieve_gt_bboxes_labels), axis=0)
+        mixup_gt_ignore_flags = np.concatenate((results["gt_ignore_flags"], retrieve_gt_ignore_flags), axis=0)
 
         # remove outside bbox
-        inside_inds = find_inside_bboxes(mixup_gt_bboxes, target_h, target_w)
+        inside_inds = mixup_gt_bboxes.is_inside([target_h, target_w]).numpy()
         mixup_gt_bboxes = mixup_gt_bboxes[inside_inds]
-        mixup_gt_labels = mixup_gt_labels[inside_inds]
+        mixup_gt_bboxes_labels = mixup_gt_bboxes_labels[inside_inds]
+        mixup_gt_ignore_flags = mixup_gt_ignore_flags[inside_inds]
 
         results["img"] = mixup_img.astype(np.uint8)
-        results["img_shape"] = mixup_img.shape
+        results["img_shape"] = mixup_img.shape[:2]
         results["gt_bboxes"] = mixup_gt_bboxes
-        results["gt_labels"] = mixup_gt_labels
+        results["gt_bboxes_labels"] = mixup_gt_bboxes_labels
+        results["gt_ignore_flags"] = mixup_gt_ignore_flags
 
         return results
 
-    def _filter_box_candidates(self, bbox1, bbox2):
-        """Compute candidate boxes which include following 5 things:
-
-        bbox1 before augment, bbox2 after augment, min_bbox_size (pixels),
-        min_area_ratio, max_aspect_ratio.
-        """
-
-        w1, h1 = bbox1[2] - bbox1[0], bbox1[3] - bbox1[1]
-        w2, h2 = bbox2[2] - bbox2[0], bbox2[3] - bbox2[1]
-        ar = np.maximum(w2 / (h2 + 1e-16), h2 / (w2 + 1e-16))
-        return (
-            (w2 > self.min_bbox_size)
-            & (h2 > self.min_bbox_size)
-            & (w2 * h2 / (w1 * h1 + 1e-16) > self.min_area_ratio)
-            & (ar < self.max_aspect_ratio)
-        )
-
     def __repr__(self):
         repr_str = self.__class__.__name__
-        repr_str += f"dynamic_scale={self.dynamic_scale}, "
+        repr_str += f"(dynamic_scale={self.dynamic_scale}, "
         repr_str += f"ratio_range={self.ratio_range}, "
         repr_str += f"flip_ratio={self.flip_ratio}, "
         repr_str += f"pad_val={self.pad_val}, "
         repr_str += f"max_iters={self.max_iters}, "
-        repr_str += f"min_bbox_size={self.min_bbox_size}, "
-        repr_str += f"min_area_ratio={self.min_area_ratio}, "
-        repr_str += f"max_aspect_ratio={self.max_aspect_ratio}, "
-        repr_str += f"skip_filter={self.skip_filter})"
+        repr_str += f"bbox_clip_border={self.bbox_clip_border})"
+        return repr_str
+
+
+class RandomAffine(BaseTransform):
+    """Random affine transform data augmentation.
+
+    This operation randomly generates affine transform matrix which including
+    rotation, translation, shear and scaling transforms.
+
+    Required Keys:
+
+    - img
+    - gt_bboxes (BaseBoxes[torch.float32]) (optional)
+    - gt_bboxes_labels (np.int64) (optional)
+    - gt_ignore_flags (bool) (optional)
+
+    Modified Keys:
+
+    - img
+    - img_shape
+    - gt_bboxes (optional)
+    - gt_bboxes_labels (optional)
+    - gt_ignore_flags (optional)
+
+    Args:
+        max_rotate_degree (float): Maximum degrees of rotation transform.
+            Defaults to 10.
+        max_translate_ratio (float): Maximum ratio of translation.
+            Defaults to 0.1.
+        scaling_ratio_range (tuple[float]): Min and max ratio of
+            scaling transform. Defaults to (0.5, 1.5).
+        max_shear_degree (float): Maximum degrees of shear
+            transform. Defaults to 2.
+        border (tuple[int]): Distance from width and height sides of input
+            image to adjust output shape. Only used in mosaic dataset.
+            Defaults to (0, 0).
+        border_val (tuple[int]): Border padding values of 3 channels.
+            Defaults to (114, 114, 114).
+        bbox_clip_border (bool, optional): Whether to clip the objects outside
+            the border of the image. In some dataset like MOT17, the gt bboxes
+            are allowed to cross the border of images. Therefore, we don't
+            need to clip the gt bboxes in these cases. Defaults to True.
+    """
+
+    def __init__(
+        self,
+        max_rotate_degree: float = 10.0,
+        max_translate_ratio: float = 0.1,
+        scaling_ratio_range: Tuple[float, float] = (0.5, 1.5),
+        max_shear_degree: float = 2.0,
+        border: Tuple[int, int] = (0, 0),
+        border_val: Tuple[int, int, int] = (114, 114, 114),
+        bbox_clip_border: bool = True,
+    ) -> None:
+        assert 0 <= max_translate_ratio <= 1
+        assert scaling_ratio_range[0] <= scaling_ratio_range[1]
+        assert scaling_ratio_range[0] > 0
+        self.max_rotate_degree = max_rotate_degree
+        self.max_translate_ratio = max_translate_ratio
+        self.scaling_ratio_range = scaling_ratio_range
+        self.max_shear_degree = max_shear_degree
+        self.border = border
+        self.border_val = border_val
+        self.bbox_clip_border = bbox_clip_border
+
+    @cache_randomness
+    def _get_random_homography_matrix(self, height, width):
+        # Rotation
+        rotation_degree = random.uniform(-self.max_rotate_degree, self.max_rotate_degree)
+        rotation_matrix = self._get_rotation_matrix(rotation_degree)
+
+        # Scaling
+        scaling_ratio = random.uniform(self.scaling_ratio_range[0], self.scaling_ratio_range[1])
+        scaling_matrix = self._get_scaling_matrix(scaling_ratio)
+
+        # Shear
+        x_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
+        y_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
+        shear_matrix = self._get_shear_matrix(x_degree, y_degree)
+
+        # Translation
+        trans_x = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * width
+        trans_y = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * height
+        translate_matrix = self._get_translation_matrix(trans_x, trans_y)
+
+        warp_matrix = translate_matrix @ shear_matrix @ rotation_matrix @ scaling_matrix
+        return warp_matrix
+
+    @autocast_box_type()
+    def transform(self, results: dict) -> dict:
+        import cv2  # TODO: support random affine requires cv2
+
+        img = results["img"]
+        height = img.shape[0] + self.border[1] * 2
+        width = img.shape[1] + self.border[0] * 2
+
+        warp_matrix = self._get_random_homography_matrix(height, width)
+
+        img = cv2.warpPerspective(img, warp_matrix, dsize=(width, height), borderValue=self.border_val)
+        results["img"] = img
+        results["img_shape"] = img.shape[:2]
+
+        bboxes = results["gt_bboxes"]
+        num_bboxes = len(bboxes)
+        if num_bboxes:
+            bboxes.project_(warp_matrix)
+            if self.bbox_clip_border:
+                bboxes.clip_([height, width])
+            # remove outside bbox
+            valid_index = bboxes.is_inside([height, width]).numpy()
+            results["gt_bboxes"] = bboxes[valid_index]
+            results["gt_bboxes_labels"] = results["gt_bboxes_labels"][valid_index]
+            results["gt_ignore_flags"] = results["gt_ignore_flags"][valid_index]
+
+            if "gt_masks" in results:
+                raise NotImplementedError("RandomAffine only supports bbox.")
+        return results
+
+    def __repr__(self):
+        repr_str = self.__class__.__name__
+        repr_str += f"(max_rotate_degree={self.max_rotate_degree}, "
+        repr_str += f"max_translate_ratio={self.max_translate_ratio}, "
+        repr_str += f"scaling_ratio_range={self.scaling_ratio_range}, "
+        repr_str += f"max_shear_degree={self.max_shear_degree}, "
+        repr_str += f"border={self.border}, "
+        repr_str += f"border_val={self.border_val}, "
+        repr_str += f"bbox_clip_border={self.bbox_clip_border})"
         return repr_str
+
+    @staticmethod
+    def _get_rotation_matrix(rotate_degrees: float) -> np.ndarray:
+        radian = math.radians(rotate_degrees)
+        rotation_matrix = np.array(
+            [[np.cos(radian), -np.sin(radian), 0.0], [np.sin(radian), np.cos(radian), 0.0], [0.0, 0.0, 1.0]],
+            dtype=np.float32,
+        )
+        return rotation_matrix
+
+    @staticmethod
+    def _get_scaling_matrix(scale_ratio: float) -> np.ndarray:
+        scaling_matrix = np.array(
+            [[scale_ratio, 0.0, 0.0], [0.0, scale_ratio, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
+        )
+        return scaling_matrix
+
+    @staticmethod
+    def _get_shear_matrix(x_shear_degrees: float, y_shear_degrees: float) -> np.ndarray:
+        x_radian = math.radians(x_shear_degrees)
+        y_radian = math.radians(y_shear_degrees)
+        shear_matrix = np.array(
+            [[1, np.tan(x_radian), 0.0], [np.tan(y_radian), 1, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
+        )
+        return shear_matrix
+
+    @staticmethod
+    def _get_translation_matrix(x: float, y: float) -> np.ndarray:
+        translation_matrix = np.array([[1, 0.0, x], [0.0, 1, y], [0.0, 0.0, 1.0]], dtype=np.float32)
+        return translation_matrix
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 try:
     from torchvision.transforms import InterpolationMode
 
     BICUBIC = InterpolationMode.BICUBIC
 except ImportError:
     BICUBIC = PIL.Image.BICUBIC
 
-try:
-    from mmdet.datasets.pipelines import Compose
-except ImportError as e:
-    mmdet = None
-
 from ..utils import is_rois_input
 from .process_mmlab_base import MMLabProcessor
 
+try:
+    from mmcv.transforms import Compose
+except ImportError as e:
+    pass
+
 logger = logging.getLogger(__name__)
 ImageFile.LOAD_TRUNCATED_IMAGES = True
 
 
 class MMDetProcessor(MMLabProcessor):
     """
     Prepare rois data for mmdetection models.
@@ -49,27 +49,61 @@
             - skip
                 Skip this sample
             -zero
                 Use an image with zero pixels.
         requires_column_info
             Whether to require feature column information in dataloader.
         """
-        from ...utils import CollateMMDet
+        from ...utils import CollateMMDet, check_if_packages_installed
+
+        check_if_packages_installed(package_names=["mmcv", "mmengine", "mmdet"])
 
         super().__init__(
             model=model,
             collate_func=CollateMMDet,
             max_img_num_per_col=max_img_num_per_col,
             missing_value_strategy=missing_value_strategy,
             requires_column_info=requires_column_info,
         )
 
+        # for yolox we seperate loading pipeline to support multi_image_mix_dataset
         if "loading_pipeline" in self.cfg.keys():
             self.load_processor = Compose(self.cfg.loading_pipeline)
 
+    def prepare_one_sample(
+        self,
+        image_paths: Dict[str, List[str]],
+        is_training: bool,
+    ):
+        mm_data = dict(img_prefix=None, bbox_fields=[])
+
+        for per_col_name, per_col_content in image_paths.items():
+            if is_rois_input(per_col_content):
+                rois = np.array(per_col_content)
+                # https://github.com/open-mmlab/mmdetection/blob/ecac3a77becc63f23d9f6980b2a36f86acd00a8a/mmdet/datasets/transforms/loading.py#L155
+                mm_data["instances"] = []
+                for roi in rois:
+                    mm_data["instances"].append(
+                        {
+                            "bbox": roi[:4],
+                            "bbox_label": roi[4],
+                            "ignore_flag": 0,
+                        }
+                    )
+            else:
+                with PIL.Image.open(per_col_content[0]) as img:
+                    # mm_data["img_info"] = dict(filename=per_col_content[0], height=img.height, width=img.width)
+                    mm_data["img_path"] = per_col_content[0]
+        if self.requires_column_info:
+            pass  # TODO
+
+        mm_data["img_id"] = 0  # TODO: use a non trivial image id for TTA (test time augmentation)
+
+        return mm_data
+
     def load_one_sample(
         self,
         image_paths: Dict[str, List[str]],
         is_training: bool,
     ) -> Dict:
         """
         Read images, process them, and stack them. One sample can have multiple images,
@@ -83,29 +117,16 @@
         is_training
             Whether to process images in the training mode.
 
         Returns
         -------
         A dictionary containing one sample's images and their number.
         """
-        mm_data = dict(img_prefix=None, bbox_fields=[])
-        ret = {}
-
-        for per_col_name, per_col_content in image_paths.items():
-            if is_rois_input(per_col_content):
-                rois = np.array(per_col_content)
-                mm_data["ann_info"] = dict(bboxes=rois[:, :4], labels=rois[:, 4])
-            else:
-                with PIL.Image.open(per_col_content[0]) as img:
-                    mm_data["img_info"] = dict(filename=per_col_content[0], height=img.height, width=img.width)
-        if self.requires_column_info:
-            pass  # TODO
-
-        ret.update({self.image_key: self.load_processor(mm_data)})
-
+        mm_data = self.prepare_one_sample(image_paths=image_paths, is_training=is_training)
+        ret = {self.image_key: self.load_processor(mm_data)}
         return ret
 
     def process_one_loaded_sample(
         self,
         image_paths: Dict[str, List[str]],
         is_training: bool,
     ) -> Dict:
@@ -146,29 +167,16 @@
             inside each image column.
         is_training
             Whether to process images in the training mode.
         Returns
         -------
         A dictionary containing one sample's images and their number.
         """
-        mm_data = dict(img_prefix=None, bbox_fields=[])
-        ret = {}
-
-        for per_col_name, per_col_content in image_paths.items():
-            if is_rois_input(per_col_content):
-                rois = np.array(per_col_content)
-                mm_data["ann_info"] = dict(bboxes=rois[:, :4], labels=rois[:, 4])
-            else:
-                with PIL.Image.open(per_col_content[0]) as img:
-                    mm_data["img_info"] = dict(filename=per_col_content[0], height=img.height, width=img.width)
-        if self.requires_column_info:
-            pass  # TODO
-
-        ret.update({self.image_key: self.train_processor(mm_data) if is_training else self.val_processor(mm_data)})
-
+        mm_data = self.prepare_one_sample(image_paths=image_paths, is_training=is_training)
+        ret = {self.image_key: self.train_processor(mm_data) if is_training else self.val_processor(mm_data)}
         return ret
 
     def __call__(
         self,
         images: Dict[str, List[str]],
         feature_modalities: Dict[str, Union[int, float, list]],
         is_training: bool,
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 
 import numpy as np
 import PIL
 from PIL import ImageFile
 from torch import nn
 
 try:
+    from torchvision.transforms import InterpolationMode
+
+    BICUBIC = InterpolationMode.BICUBIC
+except ImportError:
+    BICUBIC = PIL.Image.BICUBIC
+
+from ...constants import AUTOMM, COLUMN, IMAGE, IMAGE_VALID_NUM, MMDET_IMAGE
+from ..collator import StackCollator
+from ..utils import is_rois_input
+
+try:
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         import mmcv
-    from mmcv.parallel import collate
+    from mmcv.transforms import Compose
 except ImportError as e:
     mmcv = None
 
 try:
     import mmdet
-    from mmdet.datasets import replace_ImageToTensor
-    from mmdet.datasets.pipelines import Compose
+    from mmdet.datasets.transforms import ImageToTensor
 except ImportError as e:
     mmdet = None
 
 try:
     import mmocr
 except ImportError:
     mmocr = None
 
-try:
-    from torchvision.transforms import InterpolationMode
-
-    BICUBIC = InterpolationMode.BICUBIC
-except ImportError:
-    BICUBIC = PIL.Image.BICUBIC
-
-from ...constants import AUTOMM, COLUMN, IMAGE, IMAGE_VALID_NUM, MMDET_IMAGE
-from ..collator import StackCollator
-from ..utils import is_rois_input
 
 logger = logging.getLogger(__name__)
 ImageFile.LOAD_TRUNCATED_IMAGES = True
 
 
 class MMLabProcessor:
     """
@@ -70,39 +70,37 @@
             - skip
                 Skip this sample
             -zero
                 Use an image with zero pixels.
         requires_column_info
             Whether to require feature column information in dataloader.
         """
+        from ...utils import check_if_packages_installed
+
+        check_if_packages_installed(package_names=["mmcv"])
 
         self.prefix = model.prefix
         self.missing_value_strategy = missing_value_strategy
         self.requires_column_info = requires_column_info
         self.collate_func = collate_func
 
         self.max_img_num_per_col = max_img_num_per_col
         if max_img_num_per_col <= 0:
             logger.debug(f"max_img_num_per_col {max_img_num_per_col} is reset to 1")
             max_img_num_per_col = 1
         self.max_img_num_per_col = max_img_num_per_col
         logger.debug(f"max_img_num_per_col: {max_img_num_per_col}")
 
         if self.prefix.lower().startswith(MMDET_IMAGE):
-            assert mmdet is not None, 'Please install MMDetection by: pip install "mmdet>=2.28, <3.0.0".'
+            check_if_packages_installed(package_names=["mmdet"])
         else:
             assert mmocr is not None, "Please install MMOCR by: pip install mmocr."
         self.cfg = model.model.cfg
-        # TODO: remove hardcode here
-        try:  # yolov3
-            training_pipeline = self.cfg.data.train.dataset.pipeline
-        except:  # faster_rcnn
-            training_pipeline = self.cfg.data.train.pipeline
-        self.val_processor = Compose(replace_ImageToTensor(self.cfg.data.val.pipeline))
-        self.train_processor = Compose(replace_ImageToTensor(training_pipeline))
+        self.val_processor = Compose(self.cfg.test_pipeline)
+        self.train_processor = Compose(self.cfg.train_pipeline)
 
     @property
     def image_key(self):
         return f"{self.prefix}_{IMAGE}"
 
     @property
     def image_valid_num_key(self):
@@ -119,22 +117,21 @@
         The valid image numbers of samples will be stacked into a vector.
         This function will be used when creating Pytorch DataLoader.
 
         Returns
         -------
         A dictionary containing one model's collator function for image data.
         """
+
         fn = {}
         if self.requires_column_info:
             assert image_column_names, "Empty image column names."
             for col_name in image_column_names:
                 fn[f"{self.image_column_prefix}_{col_name}"] = StackCollator()
 
-        assert mmcv is not None, "Please install mmcv-full by: mim install mmcv-full."
-
         fn.update(
             {
                 self.image_key: self.collate_func(samples_per_gpu=per_gpu_batch_size),
             }
         )
 
         return fn
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,49 +3,30 @@
 import time
 import warnings
 from typing import Optional
 
 import torch
 from torch import nn
 
-try:
-    import warnings
+from ..constants import BBOX, BBOX_FORMATS, COLUMN, IMAGE, IMAGE_VALID_NUM, LABEL, XYXY
+from .utils import freeze_model_layers, lookup_mmdet_config, update_mmdet_config
 
+try:
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         import mmcv
-    from mmcv.ops import RoIPool
-    from mmcv.parallel import scatter
-    from mmcv.runner import load_checkpoint
-except ImportError as e:
-    mmcv = None
-
-try:
     import mmdet
-    from mmdet.core import get_classes
-    from mmdet.models import build_detector
+    import mmengine
+    from mmdet.registry import MODELS
+    from mmengine.runner import load_checkpoint
 except ImportError as e:
+    mmcv = None
     mmdet = None
+    mmengine = None
 
-from ..constants import (
-    AUTOMM,
-    BBOX,
-    BBOX_FORMATS,
-    COLUMN,
-    COLUMN_FEATURES,
-    FEATURES,
-    IMAGE,
-    IMAGE_VALID_NUM,
-    LABEL,
-    LOGITS,
-    MASKS,
-    XYWH,
-    XYXY,
-)
-from .utils import freeze_model_layers, lookup_mmdet_config, update_mmdet_config
 
 logger = logging.getLogger(__name__)
 
 
 class MMDetAutoModelForObjectDetection(nn.Module):
     """
     Support MMDET object detection models.
@@ -72,23 +53,29 @@
         checkpoint_name
             Name of the mmdet checkpoint.
         classes
             All classes in this dataset.
         pretrained
             Whether using the pretrained mmdet models. If pretrained=True, download the pretrained model.
         """
+        from ..utils import check_if_packages_installed
+
+        check_if_packages_installed(package_names=["mmcv", "mmengine", "mmdet"])
+
         super().__init__()
         self.prefix = prefix
         self.pretrained = pretrained
         self.checkpoint = None
         self.checkpoint_name = checkpoint_name
         self.config_file = config_file
         self.classes = classes
         self.frozen_layers = frozen_layers
 
+        self.device = None
+
         if output_bbox_format.lower() in BBOX_FORMATS:
             self.output_bbox_format = output_bbox_format.lower()
         else:
             raise ValueError(
                 f"Not supported bounding box output format for object detection: {output_bbox_format}. All supported bounding box output formats are: {BBOX_FORMATS}."
             )
 
@@ -119,17 +106,27 @@
             if not self.num_classes:
                 raise ValueError("Cannot retrieve num_classes for current model structure.")
             self.classes = None
         self.id2label = dict(zip(range(self.num_classes), range(self.num_classes)))
         return
 
     def _load_checkpoint(self, checkpoint_file):
+
         # build model and load pretrained weights
-        assert mmdet is not None, 'Please install MMDetection by: pip install "mmdet>=2.28, <3.0.0".'
-        self.model = build_detector(self.config.model, test_cfg=self.config.get("test_cfg"))
+        from mmdet.utils import register_all_modules
+
+        register_all_modules()  # https://github.com/open-mmlab/mmdetection/issues/9719
+
+        self.model = MODELS.build(self.config.model)
+        # yolox use self.config.model.data_preprocessor, yolov3 use self.config.data_preprocessor
+        self.data_preprocessor = MODELS.build(
+            self.config.data_preprocessor
+            if "data_preprocessor" in self.config
+            else self.config.model.data_preprocessor
+        )
 
         if self.pretrained and checkpoint_file is not None:  # TODO: enable training from scratch
             self.checkpoint = load_checkpoint(self.model, checkpoint_file, map_location="cpu")
 
         # save the config and classes in the model for convenience
         self.model.cfg = self.config
         if self.classes:
@@ -143,14 +140,20 @@
                 self.model.CLASSES = self.checkpoint["meta"]["CLASSES"]
             else:
                 raise ValueError("Classes need to be specified.")
 
         self.name_to_id = self.get_layer_ids()
         self.head_layer_names = [n for n, layer_id in self.name_to_id.items() if layer_id <= 0]
 
+    def set_data_preprocessor_device(self):
+        if not self.device:
+            self.device = next(self.model.parameters()).device
+        if self.device != self.data_preprocessor.device:
+            self.data_preprocessor.to(self.device)
+
     def save(self, save_path: str = "./", tokenizers: Optional[dict] = None):
 
         weights_save_path = os.path.join(save_path, "model.pth")
         configs_save_path = os.path.join(save_path, "config.py")
 
         self._save_weights(save_path=weights_save_path)
         self._save_configs(save_path=configs_save_path)
@@ -184,43 +187,43 @@
         mmdet_configs_dir = get_pretrain_configs_dir(subfolder="detection")
 
         AG_CUSTOM_MODELS = {
             "faster_rcnn_r50_fpn_1x_voc0712": {
                 "url": "https://automl-mm-bench.s3.amazonaws.com/voc_script/faster_rcnn_r50_fpn_1x_voc0712_20220320_192712-54bef0f3.pth",
                 "config_file": os.path.join(mmdet_configs_dir, "voc", "faster_rcnn_r50_fpn_1x_voc0712.py"),
             },
-            "yolox_nano_8x8_300e_coco": {
+            "yolox_nano": {
                 "url": "https://github.com/Megvii-BaseDetection/YOLOX/releases/download/0.1.1rc0/yolox_nano.pth",
-                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_nano_8x8_300e_coco.py"),
+                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_nano_8xb8-300e_coco.py"),
                 "source": "MegVii",
             },
-            "yolox_tiny_8x8_300e_coco": {
+            "yolox_tiny": {
                 "url": "https://download.openmmlab.com/mmdetection/v2.0/yolox/yolox_tiny_8x8_300e_coco/yolox_tiny_8x8_300e_coco_20211124_171234-b4047906.pth",
-                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_tiny_8x8_300e_coco.py"),
+                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_tiny_8xb8-300e_coco.py"),
             },
-            "yolox_s_8x8_300e_coco": {
+            "yolox_s": {
                 "url": "https://download.openmmlab.com/mmdetection/v2.0/yolox/yolox_s_8x8_300e_coco/yolox_s_8x8_300e_coco_20211121_095711-4592a793.pth",
-                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_s_8x8_300e_coco.py"),
+                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_s_8xb8-300e_coco.py"),
             },
-            "yolox_m_8x8_300e_coco": {
+            "yolox_m": {
                 "url": "https://github.com/Megvii-BaseDetection/YOLOX/releases/download/0.1.1rc0/yolox_m.pth",  # Megvii weight, need more verifications
-                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_m_8x8_300e_coco.py"),
+                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_m_8xb8-300e_coco.py"),
                 "source": "MegVii",
             },
-            "yolox_l_8x8_300e_coco": {
+            "yolox_l": {
                 "url": "https://download.openmmlab.com/mmdetection/v2.0/yolox/yolox_l_8x8_300e_coco/yolox_l_8x8_300e_coco_20211126_140236-d3bd2b23.pth",
-                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_l_8x8_300e_coco.py"),
+                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_l_8xb8-300e_coco.py"),
             },
             "yolox_l_objects365": {  # TODO: update with better pretrained weights
                 "url": "https://automl-mm-bench.s3.amazonaws.com/object_detection/checkpoints/yolox/yolox_l_objects365_temp.pth",
-                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_l_8x8_300e_coco.py"),
+                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_l_8xb8-300e_coco.py"),
             },
-            "yolox_x_8x8_300e_coco": {
+            "yolox_x": {
                 "url": "https://download.openmmlab.com/mmdetection/v2.0/yolox/yolox_x_8x8_300e_coco/yolox_x_8x8_300e_coco_20211126_140254-1ef88d67.pth",
-                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_x_8x8_300e_coco.py"),
+                "config_file": os.path.join(mmdet_configs_dir, "yolox", "yolox_x_8xb8-300e_coco.py"),
             },
         }
 
         if os.path.isfile(checkpoint_name):
             checkpoint_file = checkpoint_name
         elif os.path.isdir(checkpoint_name):
             checkpoint_file = os.path.join(checkpoint_name, "model.pth")
@@ -248,26 +251,24 @@
                 config_file = AG_CUSTOM_MODELS[checkpoint_name]["config_file"]
             else:
                 try:
                     # download config and checkpoint files using openmim
                     mimdownload(package="mmdet", configs=[checkpoint_name], dest_root=".")
                     config_file = checkpoint_name + ".py"
                 except Exception as e:
-                    print(e)
                     raise ValueError(f"Invalid checkpoint_name ({checkpoint_name}) or config_file ({config_file}): ")
 
         self.checkpoint_name = checkpoint_name
         self.checkpoint_file = checkpoint_file
         self.config_file = config_file
 
     def _load_config(self):
         # read config files
-        assert mmcv is not None, "Please install mmcv-full by: mim install mmcv-full."
         if isinstance(self.config_file, str):
-            self.config = mmcv.Config.fromfile(self.config_file)
+            self.config = mmengine.Config.fromfile(self.config_file)
         else:
             if not isinstance(self.config_file, dict):
                 raise ValueError(
                     f"The variable config_file has type {type(self.config_file)}."
                     f"Detection Model's config_file should either be a str of file path, or a dict as config."
                 )
 
@@ -289,53 +290,47 @@
 
     @property
     def image_feature_dim(self):
         return self.model.num_features
 
     def forward(
         self,
-        batch: dict,
+        batch,
+        mode,
     ):
         """
         Parameters
         ----------
         batch
             A dictionary containing the input mini-batch data.
             We need to use the keys with the model prefix to index required data.
+        mode
+            "loss" or "predict". TODO: support "tensor"
+            https://github.com/open-mmlab/mmdetection/blob/main/mmdet/models/detectors/base.py#L58C1
 
         Returns
         -------
             A dictionary with bounding boxes.
         """
-        # TODO: refactor this to work like forward() in MMDet, and support realtime predict
-        logger.warning("MMDetAutoModelForObjectDetection.forward() is deprecated since it does not support multi gpu.")
-
-        data = batch[self.image_key]
 
-        data["img_metas"] = [img_metas.data[0] for img_metas in data["img_metas"]]
-        data["img"] = [img.data[0] for img in data["img"]]
-
-        device = next(self.model.parameters()).device  # model device
-        if next(self.model.parameters()).is_cuda:
-            # scatter to specified GPU
-            data = scatter(data, [device])[0]
+        self.set_data_preprocessor_device()
+        data = self.data_preprocessor(batch)
+        rets = self.model(
+            inputs=data["inputs"],
+            data_samples=data["data_samples"],
+            mode=mode,
+        )
+
+        if mode == "loss":
+            return rets
+        elif mode == "predict":
+            # for detailed data structure, see https://github.com/open-mmlab/mmdetection/blob/main/mmdet/structures/det_data_sample.py
+            return [{BBOX: ret.pred_instances, LABEL: ret.gt_instances} for ret in rets]
         else:
-            for m in self.model.modules():
-                assert not isinstance(m, RoIPool), "CPU inference with RoIPool is not supported currently."
-
-        results = self.model(return_loss=False, rescale=True, **data)
-
-        ret = {BBOX: results}
-        return {self.prefix: ret}
-
-    def forward_test(self, imgs, img_metas, rescale=True):
-        return self.model.forward_test(imgs=imgs, img_metas=img_metas, rescale=rescale)
-
-    def forward_train(self, img, img_metas, gt_bboxes, gt_labels):
-        return self.model.forward_train(img=img, img_metas=img_metas, gt_bboxes=gt_bboxes, gt_labels=gt_labels)
+            raise ValueError(f"{mode} mode is not supported.")
 
     def _parse_losses(self, losses):
         return self.model._parse_losses(losses)
 
     def get_layer_ids(
         self,
     ):
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict, List, Optional, Tuple
 
 import torch
 from torch import nn
 from torch.nn.modules.loss import _Loss
 from transformers import AutoConfig, AutoModel
 
-from ..constants import AUTOMM, COLUMN_FEATURES, FEATURES, LOGITS, MASKS, REGRESSION
+from ..constants import AUTOMM, COLUMN_FEATURES, FEATURES, LOGITS, MASKS, OCR, REGRESSION
 from .adaptation_layers import IA3Linear, IA3LoRALinear, LoRALinear
 
 logger = logging.getLogger(__name__)
 
 
 class DummyLayer(nn.Module):
     """
@@ -618,42 +618,33 @@
     checkpoint_name
         A model checkpoint name.
 
     Returns
     -------
     An MMOCR config and model.
     """
-    try:
-        import warnings
+    from ..utils import check_if_packages_installed
 
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            import mmcv
-        from mmcv.runner import load_checkpoint
-    except ImportError as e:
-        warnings.warn(f"Encountered error while import mmcv: {e}")
-        mmcv = None
+    check_if_packages_installed(package_names=["mmcv"])
     try:
         import mmocr
         from mmocr.models import build_detector
     except ImportError:
         mmocr = None
     from mim.commands.download import download
 
     checkpoints = download(package="mmocr", configs=[checkpoint_name], dest_root=".")
 
     # read config files
-    assert mmcv is not None, "Please install mmcv-full by: mim install mmcv-full."
+    check_if_packages_installed(problem_type=OCR)
     config_file = checkpoint_name + ".py"
     if isinstance(config_file, str):
         config = mmcv.Config.fromfile(config_file)
 
     # build model and load pretrained weights
-    assert mmocr is not None, 'Please install MMOCR by: pip install "mmocr<1.0".'
-
     checkpoint = checkpoints[0]
     model = build_detector(config.model, test_cfg=config.get("test_cfg"))
     if checkpoint is not None:
         checkpoint = load_checkpoint(model, checkpoint, map_location="cpu")
     return config, model
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import logging
-from typing import Callable, Dict, List, Optional, Union
+from typing import Callable, Optional, Union
 
-import numpy as np
 import pytorch_lightning as pl
-import torch
 import torchmetrics
 from omegaconf import DictConfig
 from torch import nn
 from torch.nn.modules.loss import _Loss
 from torchmetrics.aggregation import BaseAggregator
 
-try:
-    import mmdet
-    from mmcv import ConfigDict
-except ImportError as e:
-    import warnings
-
-    pass
-
-from ..constants import AUTOMM, IMAGE, LABEL
-from ..utils import unpack_datacontainers
+from ..constants import BBOX, IMAGE, LABEL
 from .utils import (
     apply_layerwise_lr_decay,
     apply_single_lr,
     apply_two_stages_lr,
     get_lr_scheduler,
     get_optimizer,
     remove_parameters_without_grad,
 )
 
+try:
+    import mmdet
+    from mmcv import ConfigDict
+except ImportError as e:
+    mmdet = None
+    ConfigDict = None
+
 logger = logging.getLogger(__name__)
 
 
 class MMDetLitModule(pl.LightningModule):
     def __init__(
         self,
         model,
@@ -66,178 +62,101 @@
         self.validation_metric = validation_metric
         self.validation_metric_name = f"val_{validation_metric_name}"
         self.use_loss = isinstance(validation_metric, BaseAggregator)
         self.id2label = self.model.id2label
         self.input_data_key = self.model.prefix + "_" + IMAGE
         self.input_label_key = self.model.prefix + "_" + LABEL
 
-    def _predict_step(self, batch, batch_idx=0, return_loss=False):
-        pred_results = self.model.model(
-            return_loss=False,
-            rescale=True,
-            img=batch[self.input_data_key]["imgs"],
-            img_metas=batch[self.input_data_key]["img_metas"],
-        )
+    def _base_step(self, batch, mode):
+        ret = self.model(batch=batch[self.input_data_key], mode=mode)
 
-        return pred_results
+        return ret
 
-    def _loss_step(self, img, img_metas, gt_bboxes, gt_labels):
-        loss, log_vars = self.compute_loss(
-            img=img,
-            img_metas=img_metas,
-            gt_bboxes=gt_bboxes,
-            gt_labels=gt_labels,
-        )
+    def _predict_step(self, batch):
+        return self._base_step(batch=batch, mode="predict")
+
+    def _loss_step(self, batch):
+        return self._base_step(batch=batch, mode="loss")
 
-        return loss, log_vars
+    def _get_map_input(self, pred_results):
 
-    def _get_map_input(self, pred_results, sample):
         preds = []
-        for img_idx, img_result in enumerate(pred_results):
-            img_result = img_result
-            boxes = []
-            scores = []
-            labels = []
-            if isinstance(img_result[0], list):
+        target = []
+
+        batch_size = len(pred_results)
+
+        for i in range(batch_size):
+            if hasattr(pred_results[i][BBOX], "masks"):
                 # has one additional dimension with 2 outputs: img_result=img_result[0], mask_result=img_result[1]
                 raise NotImplementedError(
                     "Do not support training for models with masks like mask r-cnn, "
                     "because most custom datasets do not have a ground truth mask."
                     " However, you can still inference with this model."
                 )
-            for category_idx, category_result in enumerate(img_result):
-                for item_idx, item_result in enumerate(category_result):
-                    boxes.append(item_result[:4])
-                    scores.append(float(item_result[4]))
-                    labels.append(category_idx)
             preds.append(
                 dict(
-                    boxes=torch.tensor(np.array(boxes).astype(float)).float().to(self.device),
-                    scores=torch.tensor(scores).float().to(self.device),
-                    labels=torch.tensor(labels).long().to(self.device),
+                    boxes=pred_results[i][BBOX].bboxes,  # .float().to(self.device)?
+                    scores=pred_results[i][BBOX].scores,  # .float().to(self.device)?
+                    labels=pred_results[i][BBOX].labels,  # .long().to(self.device)?
                 )
             )
-
-        target = []
-
-        batch_size = len(preds)
-        batch = unpack_datacontainers(sample)
-        gt = batch[self.input_label_key]  # batch_size, (n, 5)
-        for i in range(batch_size):
-            img_gt = np.array(gt[i])
-            boxes = img_gt[:, :4]
-            labels = img_gt[:, 4]
             target.append(
                 dict(
-                    boxes=torch.tensor(boxes).float().to(self.device),
-                    labels=torch.tensor(labels).long().to(self.device),
+                    boxes=pred_results[i][LABEL].bboxes,
+                    labels=pred_results[i][LABEL].labels,
                 )
             )
 
         return preds, target
 
     def evaluate(self, sample, stage=None):
         """
         sample: dict
             Single data sample.
         """
         pred_results = self._predict_step(sample)
 
-        preds, target = self._get_map_input(pred_results, sample)
+        preds, target = self._get_map_input(pred_results)
 
         # use MeanAveragePrecision, example code: https://github.com/Lightning-AI/metrics/blob/master/examples/detection_map.py
         self.validation_metric.update(preds, target)
 
         return pred_results
 
-    def compute_loss(self, img, img_metas, gt_bboxes, gt_labels, *args, **kwargs):
-        """
-        Equivalent to `val_step` and `train_step` of `self.model`.
-        https://github.com/open-mmlab/mmdetection/blob/56e42e72cdf516bebb676e586f408b98f854d84c/mmdet/models/detectors/base.py#L221
-        https://github.com/open-mmlab/mmdetection/blob/56e42e72cdf516bebb676e586f408b98f854d84c/mmdet/models/detectors/base.py#L256
-        Parameters
-        ----------
-        img
-            Image Tensor
-            torch.Tensor, Size: [batch_size, C, W, H]
-        img_metas
-            List of image metadata dict
-            [
-                {
-                    'filename': 'data/VOCdevkit/VOC2007/JPEGImages/000001.jpg',
-                    'ori_filename': 'JPEGImages/000001.jpg',
-                    'ori_shape': (500, 353, 3),
-                    ...
-                },
-                ...(batch size times)
-            ]
-        gt_bboxes
-            List of ground-truth bounding boxes position tensors
-            [
-                torch.Tensor, Size: [# objects in image, 4],
-                ...(batch size times)
-            ]
-        gt_labels
-            List of ground-truth bounding boxes label tensors
-            [
-                torch.Tensor, Size: [# objects in image],
-                ...(batch size times)
-            ]
-        """
-        losses = self.model.forward_train(
-            img=img,
-            img_metas=img_metas,
-            gt_bboxes=gt_bboxes,
-            gt_labels=gt_labels,
-            *args,
-            **kwargs,
-        )
-        return self.parse_losses(losses)
+    def sum_and_log_step_results(self, losses, logging=True):
+        # losses is a dict of several type of losses, e.g. ['loss_cls', 'loss_conf', 'loss_xy', 'loss_wh']
+        # each type of losses may have multiple channels due to multiple resolution settings
+        total_loss = 0.0
+        for loss_key, loss_values in losses.items():
+            curr_loss = 0.0
+            if isinstance(loss_values, list) or isinstance(loss_values, tuple):  # is a collection of shape 0 tensors
+                for loss_chanel_idx, loss_val in enumerate(loss_values):
+                    if logging:
+                        self.log(f"step/{loss_key}_{loss_chanel_idx}", loss_val)
+                    curr_loss += loss_val
+            else:  # is a tensor
+                curr_loss += loss_values.sum()
+
+            if logging:
+                self.log(f"step/{loss_key}", curr_loss)
+            total_loss += curr_loss
 
-    def parse_losses(self, losses):
-        # `_parse_losses`: https://github.com/open-mmlab/mmdetection/blob/
-        # 56e42e72cdf516bebb676e586f408b98f854d84c/mmdet/models/detectors/base.py#L176
-        loss, log_vars = self.model._parse_losses(losses)
-        return loss, log_vars
-
-    def log_step_results(self, losses):
-        map_loss_names = {
-            "loss": "total_loss",
-            "acc": "classification-accuracy",
-            "loss_rpn_cls": "loss/rpn_cls",
-            "loss_rpn_bbox": "loss/rpn_bbox",
-            "loss_bbox": "loss/bbox_reg",
-            "loss_cls": "loss/classification",
-        }
-        for key in losses:
-            # map metric names same name with epoch-wise metrics defined in:
-            # `configs/vision/object-detection/mmdet/mmdet-base.yaml`
-            loss_name = map_loss_names.get(key, key)
-            self.log(f"step/{loss_name}", losses[key])
+        return total_loss
 
     def training_step(self, batch, batch_idx):
-        loss, log_vars = self._loss_step(
-            img=batch[self.input_data_key]["img"],
-            img_metas=batch[self.input_data_key]["img_metas"],
-            gt_bboxes=batch[self.input_data_key]["gt_bboxes"],
-            gt_labels=batch[self.input_data_key]["gt_labels"],
-        )
-        # log step losses
-        self.log_step_results(log_vars)
-        return loss
+        losses = self._loss_step(batch=batch)
+        # sum and log step losses
+        total_loss = self.sum_and_log_step_results(losses)
+        return total_loss
 
     def validation_step(self, batch, batch_idx, dataloader_idx=0):
         if self.use_loss:
-            val_loss, log_vars = self._loss_step(
-                img=batch[self.input_data_key]["img"],
-                img_metas=batch[self.input_data_key]["img_metas"],
-                gt_bboxes=batch[self.input_data_key]["gt_bboxes"],
-                gt_labels=batch[self.input_data_key]["gt_labels"],
-            )
-            self.validation_metric.update(val_loss)
+            losses = self._loss_step(batch=batch)
+            total_loss = self.sum_and_log_step_results(losses, logging=False)
+            self.validation_metric.update(total_loss)
         else:
             self.evaluate(batch, "val")
 
     def validation_epoch_end(self, validation_step_outputs):
         val_result = self.validation_metric.compute()
         if self.use_loss:
             self.log_dict({"val_direct_loss": val_result}, sync_dist=True)
@@ -248,19 +167,17 @@
             self.log_dict(mAPs, sync_dist=True)
         self.validation_metric.reset()
 
     def test_step(self, batch, batch_idx, dataloader_idx=0):
         raise NotImplementedError("test with lit_mmdet is not implemented yet.")
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
-        pred = self._predict_step(batch, batch_idx)
-        if "mmdet_image_label" in batch:
-            return {"bbox": pred, "label": batch[self.input_label_key]}
-        else:
-            return {"bbox": pred}
+        pred = self._predict_step(batch)
+
+        return pred
 
     def configure_optimizers(self):
         """
         Configure optimizer. This function is registered by pl.LightningModule.
         Refer to https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html#configure-optimizers
         Returns
         -------
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1770,23 +1770,16 @@
 
                 if strategy == "ddp":
                     if evaluator.global_rank != 0:
                         sys.exit(f"Prediction finished, exit the process with global_rank={evaluator.global_rank}...")
                     else:
                         outputs = pred_writer.collect_all_gpu_results(num_gpus=num_gpus)
                 elif self._problem_type == OBJECT_DETECTION:
-                    # reformat single gpu output for object detection
-                    # outputs shape: num_batch, 1(["bbox"]), batch_size, 80, n, 5
-                    # output LABEL if exists for evaluations
-                    outputs = [
-                        {BBOX: bbox, LABEL: ele[LABEL][i]} if LABEL in ele else {BBOX: bbox}
-                        for ele in outputs
-                        for i, bbox in enumerate(ele[BBOX])
-                    ]
-
+                    # Unpack outputs for object detection while using single gpu
+                    outputs = [output for batch_outputs in outputs for output in batch_outputs]
         return outputs
 
     def _on_predict_start(
         self,
         data: Union[pd.DataFrame, dict, list],
         requires_label: bool,
     ):
@@ -2192,15 +2185,17 @@
                 pred=pred,
                 data=data,
                 detection_classes=self._model.model.CLASSES,
                 result_path=result_path,
             )
 
         if (as_pandas is None and isinstance(data, pd.DataFrame)) or as_pandas is True:
-            if self._problem_type == OBJECT_DETECTION:
+            if (
+                self._problem_type == OBJECT_DETECTION
+            ):  # TODO: add prediction output in COCO format if as_pandas is False
                 pred = save_result_df(
                     pred=pred,
                     data=data,
                     detection_classes=self._model.model.CLASSES,
                     result_path=None,
                 )
             elif (
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
     hyperparameters
         The hyperparameters for a given preset.
     hyperparameter_tune_kwargs
         The hyperparameter tuning kwargs.
     """
     hyperparameters = {
         "model.names": ["mmdet_image"],
-        "model.mmdet_image.checkpoint_name": "yolox_s_8x8_300e_coco",
+        "model.mmdet_image.checkpoint_name": "yolox_s",
         "env.eval_batch_size_ratio": 1,
         "env.precision": 32,
         "env.strategy": "ddp",
         "env.auto_select_gpus": False,  # Have to turn off for detection!
         "env.num_gpus": -1,
         "env.per_gpu_batch_size": 8,  # Works on 8G GPU
         "env.num_workers": 2,
@@ -395,27 +395,27 @@
                 "optimization.val_check_interval": 1.0,
                 "optimization.check_val_every_n_epoch": 3,
             }
         )
     elif presets in [DEFAULT, HIGH_QUALITY]:
         hyperparameters.update(
             {
-                "model.mmdet_image.checkpoint_name": "yolox_l_8x8_300e_coco",
+                "model.mmdet_image.checkpoint_name": "yolox_l",
                 "env.per_gpu_batch_size": 2,  # Works on 8G GPU
                 "optimization.learning_rate": 5e-5,
                 "optimization.patience": 3,
                 "optimization.max_epochs": 50,
                 "optimization.val_check_interval": 1.0,
                 "optimization.check_val_every_n_epoch": 3,
             }
         )
     elif presets == BEST_QUALITY:
         hyperparameters.update(
             {
-                "model.mmdet_image.checkpoint_name": "yolox_x_8x8_300e_coco",
+                "model.mmdet_image.checkpoint_name": "yolox_x",
                 "env.per_gpu_batch_size": 1,  # Works on 8G GPU
                 "optimization.learning_rate": 1e-5,
                 "optimization.patience": 20,
                 "optimization.max_epochs": 50,
             }
         )
     else:
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from .inference import extract_from_output, infer_batch, predict, process_batch, use_realtime
 from .load import CustomUnpickler, get_dir_ckpt_paths, get_load_ckpt_paths, load_text_tokenizers
 from .log import LogFilter, apply_log_filter, get_fit_complete_message, get_fit_start_message, make_exp_dir
 from .map import MeanAveragePrecision
 from .matcher import compute_semantic_similarity, convert_data_for_ranking, create_siamese_model, semantic_search
 from .metric import compute_ranking_score, compute_score, get_minmax_mode, get_stopping_threshold, infer_metrics
 from .misc import logits_to_prob, merge_bio_format, shopee_dataset, tensor_to_ndarray, visualize_ner
-from .mmcv import CollateMMDet, CollateMMOcr, send_datacontainers_to_device, unpack_datacontainers
+from .mmcv import CollateMMDet, CollateMMOcr
 from .model import create_fusion_model, create_model, list_timm_models, modify_duplicate_model_names, select_model
 from .object_detection import (
     COCODataset,
     bbox_ratio_xywh_to_index_xyxy,
     bbox_xyxy_to_xywh,
     cocoeval,
     convert_pred_to_xywh,
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import torch
 from pytorch_lightning.accelerators import find_usable_cuda_devices
 from torch import nn
 
 from autogluon.common.utils.resource_utils import ResourceManager
 
 from ..constants import AUTOMM, OBJECT_DETECTION, OCR
-from .mmcv import DataContainer
 
 logger = logging.getLogger(__name__)
 
 
 def is_interactive():
     """
     Return whether the current process is running under the interactive mode.
@@ -150,15 +149,15 @@
             res[k] = move_to_device(v, device)
         return res
     elif isinstance(obj, list) or isinstance(obj, tuple):
         res = []
         for v in obj:
             res.append(move_to_device(v, device))
         return res
-    elif isinstance(obj, (int, float, str, DataContainer)):
+    elif isinstance(obj, (int, float, str)):
         return obj
     else:
         raise TypeError(
             f"Invalid type {type(obj)} for move_to_device. "
             f"Make sure the object is one of these: a Pytorch tensor, a Pytorch module, "
             f"a dict or list of tensors or modules."
         )
@@ -237,53 +236,83 @@
         return torch.autocast(device_type=device_type, dtype=torch.bfloat16 if precision == "bf16" else torch.half)
     elif precision == 64:
         return double_precision_context()
     else:
         raise ValueError(f"Unknown precision: {precision}")
 
 
-def check_if_packages_installed(problem_type: str):
+def check_if_packages_installed(problem_type: str = None, package_names: List[str] = None):
     """
     Check if necessary packages are installed for some problem types.
     Raise an error if an package can't be imported.
 
     Parameters
     ----------
     problem_type
         Problem type
     """
-    if not problem_type:
-        return
-
-    problem_type = problem_type.lower()
-    if any(p in problem_type for p in [OBJECT_DETECTION, OCR]):
-        try:
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore")
-                import mmcv
-        except ImportError as e:
-            raise ValueError(
-                f"Encountered error while importing mmcv: {e}. Try to install mmcv: mim install mmcv-full."
-            )
-
-        try:
-            import mmdet
-        except ImportError as e:
-            raise ValueError(
-                f'Encountered error while importing mmdet: {e}. Try to install mmdet: pip install "mmdet>=2.28, <3.0.0".'
-            )
+    if problem_type:
+        problem_type = problem_type.lower()
+        if any(p in problem_type for p in [OBJECT_DETECTION, OCR]):
+            try:
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore")
+                    import mmcv
+            except ImportError as e:
+                raise ValueError(
+                    f"Encountered error while importing mmcv: {e}. {_get_mmlab_installation_guide('mmcv')}"
+                )
 
-        if OCR in problem_type:
             try:
-                import mmocr
+                import mmdet
             except ImportError as e:
                 raise ValueError(
-                    f'Encountered error while importing mmocr: {e}. Try to install mmocr: pip install "mmocr<1.0".'
+                    f"Encountered error while importing mmdet: {e}. {_get_mmlab_installation_guide('mmdet')}"
                 )
 
+            if OCR in problem_type:
+                try:
+                    import mmocr
+                except ImportError as e:
+                    raise ValueError(
+                        f'Encountered error while importing mmocr: {e}. Try to install mmocr: pip install "mmocr<1.0".'
+                    )
+
+    if package_names:
+        for package_name in package_names:
+            if package_name == "mmcv":
+                try:
+                    with warnings.catch_warnings():
+                        warnings.simplefilter("ignore")
+                        import mmcv
+                    from mmcv import ConfigDict
+                    from mmcv.runner import load_checkpoint
+                    from mmcv.transforms import Compose
+                except ImportError as e:
+                    f"Encountered error while importing {package_name}: {e}. {_get_mmlab_installation_guide(package_name)}"
+            elif package_name == "mmdet":
+                try:
+                    import mmdet
+                    from mmdet.datasets.transforms import ImageToTensor
+                    from mmdet.registry import MODELS
+                except ImportError as e:
+                    f"Encountered error while importing {package_name}: {e}. {_get_mmlab_installation_guide(package_name)}"
+            elif package_name == "mmengine":
+                try:
+                    import mmengine
+                    from mmengine.dataset import pseudo_collate as collate
+                    from mmengine.runner import load_checkpoint
+                except ImportError as e:
+                    warnings.warn(e)
+                    raise ValueError(
+                        f"Encountered error while importing {package_name}: {e}. {_get_mmlab_installation_guide(package_name)}"
+                    )
+            else:
+                raise ValueError(f"package_name {package_name} is not required.")
+
 
 def get_available_devices(num_gpus: int, auto_select_gpus: bool, use_ray_lightning: Optional[bool] = False):
     """
     Get the available devices.
 
     Parameters
     ----------
@@ -303,7 +332,20 @@
             devices = find_usable_cuda_devices(num_gpus)
         else:
             devices = num_gpus
     else:
         devices = None
 
     return devices
+
+
+def _get_mmlab_installation_guide(package_name):
+    if package_name == "mmdet":
+        err_msg = 'Please install MMDetection by: pip install "mmdet>=3.0.0".'
+    elif package_name == "mmcv":
+        err_msg = "Please install MMCV by: mim install mmcv"
+    elif package_name == "mmengine":
+        err_msg = "Please install MMCV by: mim install mmengine"
+    else:
+        raise ValueError("Available package_name are: mmdet, mmcv, mmengine.")
+
+    return err_msg
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/map.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/map.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/object_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import defusedxml.ElementTree as ET
 import numpy as np
 import pandas as pd
 import PIL
 
 from ..constants import (
     AUTOMM,
+    BBOX,
+    LABEL,
     MAP,
     MAP_50,
     MAP_75,
     MAP_LARGE,
     MAP_MEDIUM,
     MAP_SMALL,
     MAR_1,
@@ -851,25 +853,26 @@
         save_path
             The save path given to store COCO format output.
         """
         coco_format_result = []
 
         for i, row in data.reset_index(drop=True).iterrows():
             image_id = self.get_image_id_from_path(row["image"])
-            for j, res in enumerate(ret[i]):
-                category_id = self.category_ids[j]
-                for bbox in res:
-                    coco_format_result.append(
-                        {
-                            "image_id": image_id,
-                            "category_id": category_id,
-                            "bbox": bbox_xyxy_to_xywh(bbox[:4].astype(float).tolist()),
-                            "score": float(bbox[4]),
-                        }
-                    )
+
+            pred_result = ret[i]
+            N_pred = len(pred_result["bboxes"])
+            for bbox_idx in range(N_pred):
+                coco_format_result.append(
+                    {
+                        "image_id": image_id,
+                        "category_id": self.category_ids[int(pred_result["labels"][bbox_idx].item())],
+                        "bbox": bbox_xyxy_to_xywh(pred_result["bboxes"][bbox_idx].tolist()),
+                        "score": pred_result["scores"][bbox_idx].item(),
+                    }
+                )
 
         with open(save_path, "w") as f:
             print(f"saving file at {save_path}")
             json.dump(coco_format_result, f)
 
 
 def cocoeval_torchmetrics(outputs: List):
@@ -890,39 +893,27 @@
 
     from . import MeanAveragePrecision
 
     map_metric = MeanAveragePrecision(box_format="xyxy", iou_type="bbox", class_metrics=False)
 
     preds = []
     target = []
-    for img_idx, img_output in enumerate(outputs):  # TODO: refactor here
-        img_result = img_output["bbox"]
-        boxes = []
-        scores = []
-        labels = []
-        for category_idx, category_result in enumerate(img_result):
-            for item_idx, item_result in enumerate(category_result):
-                boxes.append(item_result[:4])
-                scores.append(float(item_result[4]))
-                labels.append(category_idx)
+    for per_img_outputs in outputs:  # TODO: refactor here
         preds.append(
             dict(
-                boxes=torch.tensor(np.array(boxes).astype(float)).float().to("cpu"),
-                scores=torch.tensor(scores).float().to("cpu"),
-                labels=torch.tensor(labels).long().to("cpu"),
+                boxes=per_img_outputs[BBOX]["bboxes"].to("cpu"),
+                scores=per_img_outputs[BBOX]["scores"].to("cpu"),
+                labels=per_img_outputs[BBOX]["labels"].to("cpu"),
             )
         )
 
-        img_gt = np.array(img_output["label"])
-        boxes = img_gt[:, :4]
-        labels = img_gt[:, 4]
         target.append(
             dict(
-                boxes=torch.tensor(boxes).float().to("cpu"),
-                labels=torch.tensor(labels).long().to("cpu"),
+                boxes=per_img_outputs[LABEL]["bboxes"].to("cpu"),
+                labels=per_img_outputs[LABEL]["labels"].to("cpu"),
             )
         )
 
     map_metric.update(preds, target)
 
     return map_metric.compute()
 
@@ -1526,25 +1517,29 @@
     else:
         image_names = data["image"].to_list()
     results = []
     idx2classname = {i: classname for (i, classname) in enumerate(detection_classes)}
 
     for image_pred, image_name in zip(pred, image_names):
         box_info = []
-        for class_idx, bboxes in enumerate(image_pred):
-            pred_class = idx2classname[class_idx]
-
-            for bbox in bboxes:
-                box_info.append({"class": pred_class, "bbox": list(bbox[:4]), "score": bbox[4]})
+        N_preds = len(image_pred["bboxes"])
+        for i in range(N_preds):
+            box_info.append(
+                {
+                    "class": idx2classname[image_pred["labels"][i].item()],
+                    "class_id": image_pred["labels"][i].item(),
+                    "bbox": image_pred["bboxes"][i].tolist(),
+                    "score": image_pred["scores"][i].item(),
+                }
+            )
         results.append([image_name, box_info])
     result_df = pd.DataFrame(results, columns=["image", "bboxes"])
     if result_path:
         result_df.to_csv(result_path, index=False)
         logger.info("Saved detection results to {}".format(result_path))
-        print("Saved detection results to {}".format(result_path))
     return result_df
 
 
 def save_result_coco_format(detection_data_path, pred, result_path):
     coco_dataset = COCODataset(detection_data_path)
     result_name, _ = os.path.splitext(result_path)
     result_path = result_name + ".json"
@@ -1652,13 +1647,10 @@
         raise TypeError(f"Expected train_data to have type str or pd.DataFrame, but got type: {type(train_data)}")
     return train_data, tuning_data
 
 
 def convert_pred_to_xywh(pred: Optional[List]):
     if not pred:
         return pred
-    num_images = len(pred)
-    num_categories = len(pred[0])
-    for i in range(num_images):
-        for j in range(num_categories):
-            pred[i][j][:, :4] = bbox_xyxy_to_xywh(pred[i][j][:, :4])
+    for i, pred_per_image in enumerate(pred):
+        pred[i]["bboxes"] = bbox_xyxy_to_xywh(pred_per_image["bboxes"].detach().numpy())
     return pred
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230601
+Version: 0.7.1b20230602
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,20 +24,21 @@
 src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
 src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
 src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
 src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
 src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
 src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
 src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
-src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8x8_300e_coco.py
-src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8x8_300e_coco.py
-src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py
-src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py
-src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py
-src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8x8_300e_coco.py
+src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
 src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
 src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
 src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
 src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
 src/autogluon/multimodal/data/__init__.py
 src/autogluon/multimodal/data/collator.py
 src/autogluon/multimodal/data/datamodule.py
```

### Comparing `autogluon.multimodal-0.7.1b20230601/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<0.12.0,>=0.11.0
 transformers<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
 sentencepiece<0.2.0,>=0.1.95
-autogluon.core[raytune]==0.7.1b20230601
-autogluon.features==0.7.1b20230601
-autogluon.common==0.7.1b20230601
+autogluon.core[raytune]==0.7.1b20230602
+autogluon.features==0.7.1b20230602
+autogluon.common==0.7.1b20230602
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
-openmim<0.4.0,>0.1.5
+openmim<0.4.0,>=0.3.7
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
 pytesseract<0.3.11,>=0.3.9
 PyMuPDF<=1.21.1
 
 [tests]
```

