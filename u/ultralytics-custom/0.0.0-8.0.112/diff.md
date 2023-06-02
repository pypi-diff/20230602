# Comparing `tmp/ultralytics_custom-0.0.0.tar.gz` & `tmp/ultralytics_custom-8.0.112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics_custom-0.0.0.tar", last modified: Fri Jun  2 16:20:28 2023, max compression
+gzip compressed data, was "ultralytics_custom-8.0.112.tar", last modified: Fri Jun  2 03:19:24 2023, max compression
```

## Comparing `ultralytics_custom-0.0.0.tar` & `ultralytics_custom-8.0.112.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.630513 ultralytics_custom-0.0.0/
--rw-rw-rw-   0        0        0     5739 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    35184 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      221 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    26237 2023-06-02 16:20:28.630513 ultralytics_custom-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    24496 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/README.md
--rw-rw-rw-   0        0        0    23487 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/README.zh-CN.md
--rw-rw-rw-   0        0        0     1110 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0      723 2023-06-02 16:20:28.635508 ultralytics_custom-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3226 2023-06-02 16:20:23.000000 ultralytics_custom-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.548509 ultralytics_custom-0.0.0/ultralytics/
--rw-rw-rw-   0        0        0      394 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.549508 ultralytics_custom-0.0.0/ultralytics/assets/
--rw-rw-rw-   0        0        0   137419 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/assets/bus.jpg
--rw-rw-rw-   0        0        0    50427 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/assets/zidane.jpg
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.557509 ultralytics_custom-0.0.0/ultralytics/datasets/
--rw-rw-rw-   0        0        0     2824 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/Argoverse.yaml
--rw-rw-rw-   0        0        0     1972 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/GlobalWheat2020.yaml
--rw-rw-rw-   0        0        0    44464 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/ImageNet.yaml
--rw-rw-rw-   0        0        0     9713 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/Objects365.yaml
--rw-rw-rw-   0        0        0     2495 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/SKU-110K.yaml
--rw-rw-rw-   0        0        0     3612 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/VOC.yaml
--rw-rw-rw-   0        0        0     3085 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/VisDrone.yaml
--rw-rw-rw-   0        0        0     1585 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/coco-pose.yaml
--rw-rw-rw-   0        0        0     2641 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/coco.yaml
--rw-rw-rw-   0        0        0     1963 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/coco128-seg.yaml
--rw-rw-rw-   0        0        0     1947 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/coco128.yaml
--rw-rw-rw-   0        0        0      920 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/coco8-pose.yaml
--rw-rw-rw-   0        0        0     1898 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/coco8-seg.yaml
--rw-rw-rw-   0        0        0     1878 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/coco8.yaml
--rw-rw-rw-   0        0        0     5331 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/datasets/xView.yaml
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.559508 ultralytics_custom-0.0.0/ultralytics/hub/
--rw-rw-rw-   0        0        0     4338 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/hub/__init__.py
--rw-rw-rw-   0        0        0     5348 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/hub/auth.py
--rw-rw-rw-   0        0        0     8668 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/hub/session.py
--rw-rw-rw-   0        0        0     9374 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/hub/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.540497 ultralytics_custom-0.0.0/ultralytics/models/
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.559508 ultralytics_custom-0.0.0/ultralytics/models/rt-detr/
--rw-rw-rw-   0        0        0     2020 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/rt-detr/rt-detr-l.yaml
--rw-rw-rw-   0        0        0     2231 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/rt-detr/rt-detr-x.yaml
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.561509 ultralytics_custom-0.0.0/ultralytics/models/v3/
--rw-rw-rw-   0        0        0     1598 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v3/yolov3-spp.yaml
--rw-rw-rw-   0        0        0     1291 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v3/yolov3-tiny.yaml
--rw-rw-rw-   0        0        0     1585 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v3/yolov3.yaml
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.562508 ultralytics_custom-0.0.0/ultralytics/models/v5/
--rw-rw-rw-   0        0        0     1984 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v5/yolov5-p6.yaml
--rw-rw-rw-   0        0        0     1600 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v5/yolov5.yaml
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.562508 ultralytics_custom-0.0.0/ultralytics/models/v6/
--rw-rw-rw-   0        0        0     1733 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v6/yolov6.yaml
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.565509 ultralytics_custom-0.0.0/ultralytics/models/v8/
--rw-rw-rw-   0        0        0      949 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-cls.yaml
--rw-rw-rw-   0        0        0     1805 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-p2.yaml
--rw-rw-rw-   0        0        0     1912 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-p6.yaml
--rw-rw-rw-   0        0        0     2003 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-pose-p6.yaml
--rw-rw-rw-   0        0        0     1627 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-pose.yaml
--rw-rw-rw-   0        0        0     1536 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-seg.yaml
--rw-rw-rw-   0        0        0     1959 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8.yaml
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.568523 ultralytics_custom-0.0.0/ultralytics/nn/
--rw-rw-rw-   0        0        0      564 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/__init__.py
--rw-rw-rw-   0        0        0    24709 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/autobackend.py
--rw-rw-rw-   0        0        0    12752 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/autoshape.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.571509 ultralytics_custom-0.0.0/ultralytics/nn/modules/
--rw-rw-rw-   0        0        0     1616 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/modules/__init__.py
--rw-rw-rw-   0        0        0    12120 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/modules/block.py
--rw-rw-rw-   0        0        0    11944 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/modules/conv.py
--rw-rw-rw-   0        0        0    17480 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/modules/head.py
--rw-rw-rw-   0        0        0    16785 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/modules/transformer.py
--rw-rw-rw-   0        0        0     3322 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/modules/utils.py
--rw-rw-rw-   0        0        0    34740 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/nn/tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.572508 ultralytics_custom-0.0.0/ultralytics/tracker/
--rw-rw-rw-   0        0        0      208 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.572508 ultralytics_custom-0.0.0/ultralytics/tracker/cfg/
--rw-rw-rw-   0        0        0      908 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/cfg/botsort.yaml
--rw-rw-rw-   0        0        0      705 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/cfg/bytetrack.yaml
--rw-rw-rw-   0        0        0     2374 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/track.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.574509 ultralytics_custom-0.0.0/ultralytics/tracker/trackers/
--rw-rw-rw-   0        0        0      177 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/trackers/__init__.py
--rw-rw-rw-   0        0        0     1680 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/trackers/basetrack.py
--rw-rw-rw-   0        0        0     5832 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/trackers/bot_sort.py
--rw-rw-rw-   0        0        0    14812 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/trackers/byte_tracker.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.576509 ultralytics_custom-0.0.0/ultralytics/tracker/utils/
--rw-rw-rw-   0        0        0        0 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/utils/__init__.py
--rw-rw-rw-   0        0        0    12533 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/utils/gmc.py
--rw-rw-rw-   0        0        0    18882 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/utils/kalman_filter.py
--rw-rw-rw-   0        0        0     8928 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/tracker/utils/matching.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.577509 ultralytics_custom-0.0.0/ultralytics/vit/
--rw-rw-rw-   0        0        0      155 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.578508 ultralytics_custom-0.0.0/ultralytics/vit/rtdetr/
--rw-rw-rw-   0        0        0      204 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/rtdetr/__init__.py
--rw-rw-rw-   0        0        0     4722 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/rtdetr/model.py
--rw-rw-rw-   0        0        0     1946 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/rtdetr/predict.py
--rw-rw-rw-   0        0        0     4904 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/rtdetr/val.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.581508 ultralytics_custom-0.0.0/ultralytics/vit/sam/
--rw-rw-rw-   0        0        0      133 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/__init__.py
--rw-rw-rw-   0        0        0    13615 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/amg.py
--rw-rw-rw-   0        0        0     3970 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/autosize.py
--rw-rw-rw-   0        0        0     3906 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/build.py
--rw-rw-rw-   0        0        0     1853 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/model.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.585509 ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/
--rw-rw-rw-   0        0        0        0 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/__init__.py
--rw-rw-rw-   0        0        0     6512 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/decoders.py
--rw-rw-rw-   0        0        0    23083 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/encoders.py
--rw-rw-rw-   0        0        0    15601 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/mask_generator.py
--rw-rw-rw-   0        0        0    11441 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/prompt_predictor.py
--rw-rw-rw-   0        0        0     7285 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/sam.py
--rw-rw-rw-   0        0        0     8722 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/transformer.py
--rw-rw-rw-   0        0        0     2191 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/vit/sam/predict.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.585509 ultralytics_custom-0.0.0/ultralytics/yolo/
--rw-rw-rw-   0        0        0       99 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.586508 ultralytics_custom-0.0.0/ultralytics/yolo/cfg/
--rw-rw-rw-   0        0        0    18463 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/cfg/__init__.py
--rw-rw-rw-   0        0        0     6452 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/cfg/default.yaml
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.591508 ultralytics_custom-0.0.0/ultralytics/yolo/data/
--rw-rw-rw-   0        0        0      467 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/__init__.py
--rw-rw-rw-   0        0        0     2392 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/annotator.py
--rw-rw-rw-   0        0        0    38062 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/augment.py
--rw-rw-rw-   0        0        0    12935 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/base.py
--rw-rw-rw-   0        0        0     6744 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/build.py
--rw-rw-rw-   0        0        0     9420 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/converter.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.593509 ultralytics_custom-0.0.0/ultralytics/yolo/data/dataloaders/
--rw-rw-rw-   0        0        0        0 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/dataloaders/__init__.py
--rw-rw-rw-   0        0        0    15276 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-rw-rw-   0        0        0    18053 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-rw-rw-   0        0        0    52369 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-rw-rw-   0        0        0    13646 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/dataset.py
--rw-rw-rw-   0        0        0     1829 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/dataset_wrappers.py
--rw-rw-rw-   0        0        0    24569 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.596508 ultralytics_custom-0.0.0/ultralytics/yolo/engine/
--rw-rw-rw-   0        0        0        0 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/engine/__init__.py
--rw-rw-rw-   0        0        0    41118 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/engine/exporter.py
--rw-rw-rw-   0        0        0    22612 2023-06-02 10:20:10.000000 ultralytics_custom-0.0.0/ultralytics/yolo/engine/model.py
--rw-rw-rw-   0        0        0    16549 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/engine/predictor.py
--rw-rw-rw-   0        0        0    24867 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/engine/results.py
--rw-rw-rw-   0        0        0    33053 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/engine/trainer.py
--rw-rw-rw-   0        0        0    11991 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/engine/validator.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.605508 ultralytics_custom-0.0.0/ultralytics/yolo/utils/
--rw-rw-rw-   0        0        0    28625 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/__init__.py
--rw-rw-rw-   0        0        0     3936 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/autobatch.py
--rw-rw-rw-   0        0        0    15781 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/benchmarks.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.610509 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/
--rw-rw-rw-   0        0        0      219 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/__init__.py
--rw-rw-rw-   0        0        0     5755 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/base.py
--rw-rw-rw-   0        0        0     6045 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/clearml.py
--rw-rw-rw-   0        0        0    13345 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/comet.py
--rw-rw-rw-   0        0        0     3397 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/hub.py
--rw-rw-rw-   0        0        0     2563 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/mlflow.py
--rw-rw-rw-   0        0        0     3802 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/neptune.py
--rw-rw-rw-   0        0        0      515 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/raytune.py
--rw-rw-rw-   0        0        0     1572 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-rw-rw-   0        0        0     2230 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/wb.py
--rw-rw-rw-   0        0        0    15388 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/checks.py
--rw-rw-rw-   0        0        0     2663 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/dist.py
--rw-rw-rw-   0        0        0    12260 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/downloads.py
--rw-rw-rw-   0        0        0      327 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/errors.py
--rw-rw-rw-   0        0        0     3688 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/files.py
--rw-rw-rw-   0        0        0    15051 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/instance.py
--rw-rw-rw-   0        0        0    18601 2023-06-02 10:10:14.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/loss.py
--rw-rw-rw-   0        0        0    46867 2023-06-02 10:10:13.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/metrics.py
--rw-rw-rw-   0        0        0    28979 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/ops.py
--rw-rw-rw-   0        0        0     1286 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/patches.py
--rw-rw-rw-   0        0        0    24946 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/plotting.py
--rw-rw-rw-   0        0        0    13921 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/tal.py
--rw-rw-rw-   0        0        0    22693 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/torch_utils.py
--rw-rw-rw-   0        0        0     2326 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/utils/tuner.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.610509 ultralytics_custom-0.0.0/ultralytics/yolo/v8/
--rw-rw-rw-   0        0        0      163 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.612508 ultralytics_custom-0.0.0/ultralytics/yolo/v8/classify/
--rw-rw-rw-   0        0        0      398 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/classify/__init__.py
--rw-rw-rw-   0        0        0     1980 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/classify/predict.py
--rw-rw-rw-   0        0        0     7090 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/classify/train.py
--rw-rw-rw-   0        0        0     4785 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/classify/val.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.614508 ultralytics_custom-0.0.0/ultralytics/yolo/v8/detect/
--rw-rw-rw-   0        0        0      284 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/detect/__init__.py
--rw-rw-rw-   0        0        0     1902 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/detect/predict.py
--rw-rw-rw-   0        0        0     7342 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/detect/train.py
--rw-rw-rw-   0        0        0    15011 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/detect/val.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.616508 ultralytics_custom-0.0.0/ultralytics/yolo/v8/pose/
--rw-rw-rw-   0        0        0      254 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/pose/__init__.py
--rw-rw-rw-   0        0        0     2433 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/pose/predict.py
--rw-rw-rw-   0        0        0     2867 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/pose/train.py
--rw-rw-rw-   0        0        0    11141 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/pose/val.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.618515 ultralytics_custom-0.0.0/ultralytics/yolo/v8/segment/
--rw-rw-rw-   0        0        0      302 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/segment/__init__.py
--rw-rw-rw-   0        0        0     2902 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/segment/predict.py
--rw-rw-rw-   0        0        0     2564 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/segment/train.py
--rw-rw-rw-   0        0        0    13143 2023-06-02 09:23:23.000000 ultralytics_custom-0.0.0/ultralytics/yolo/v8/segment/val.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:20:28.630513 ultralytics_custom-0.0.0/ultralytics_custom.egg-info/
--rw-rw-rw-   0        0        0    26237 2023-06-02 16:20:28.000000 ultralytics_custom-0.0.0/ultralytics_custom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5496 2023-06-02 16:20:28.000000 ultralytics_custom-0.0.0/ultralytics_custom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 16:20:28.000000 ultralytics_custom-0.0.0/ultralytics_custom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-06-02 16:20:28.000000 ultralytics_custom-0.0.0/ultralytics_custom.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      369 2023-06-02 16:20:28.000000 ultralytics_custom-0.0.0/ultralytics_custom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-02 16:20:28.000000 ultralytics_custom-0.0.0/ultralytics_custom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 03:06:23.626196 ultralytics_custom-8.0.112/
+-rw-rw-rw-   0        0        0     5739 2023-06-01 19:51:45.000000 ultralytics_custom-8.0.112/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    35184 2023-06-01 19:51:45.000000 ultralytics_custom-8.0.112/LICENSE
+-rw-rw-rw-   0        0        0      221 2023-06-01 19:51:45.000000 ultralytics_custom-8.0.112/MANIFEST.in
+-rw-rw-rw-   0        0        0    26239 2023-06-02 03:19:24.640005 ultralytics_custom-8.0.112/PKG-INFO
+-rw-rw-rw-   0        0        0    24496 2023-06-01 19:51:45.000000 ultralytics_custom-8.0.112/README.md
+-rw-rw-rw-   0        0        0    23487 2023-06-01 19:51:45.000000 ultralytics_custom-8.0.112/README.zh-CN.md
+-rw-rw-rw-   0        0        0     1110 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/requirements.txt
+-rw-rw-rw-   0        0        0      723 2023-06-02 03:19:24.640005 ultralytics_custom-8.0.112/setup.cfg
+-rw-rw-rw-   0        0        0     3218 2023-06-02 03:03:58.000000 ultralytics_custom-8.0.112/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.343655 ultralytics_custom-8.0.112/ultralytics/
+-rw-rw-rw-   0        0        0      394 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.348658 ultralytics_custom-8.0.112/ultralytics/assets/
+-rw-rw-rw-   0        0        0   137419 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/assets/bus.jpg
+-rw-rw-rw-   0        0        0    50427 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/assets/zidane.jpg
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.451658 ultralytics_custom-8.0.112/ultralytics/datasets/
+-rw-rw-rw-   0        0        0     2824 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/Argoverse.yaml
+-rw-rw-rw-   0        0        0     1972 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-rw-rw-   0        0        0    44464 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/ImageNet.yaml
+-rw-rw-rw-   0        0        0     9713 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/Objects365.yaml
+-rw-rw-rw-   0        0        0     2495 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/SKU-110K.yaml
+-rw-rw-rw-   0        0        0     3612 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/VOC.yaml
+-rw-rw-rw-   0        0        0     3085 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/VisDrone.yaml
+-rw-rw-rw-   0        0        0     1585 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/coco-pose.yaml
+-rw-rw-rw-   0        0        0     2641 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/coco.yaml
+-rw-rw-rw-   0        0        0     1963 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/coco128-seg.yaml
+-rw-rw-rw-   0        0        0     1947 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/coco128.yaml
+-rw-rw-rw-   0        0        0      920 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/coco8-pose.yaml
+-rw-rw-rw-   0        0        0     1898 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/coco8-seg.yaml
+-rw-rw-rw-   0        0        0     1878 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/coco8.yaml
+-rw-rw-rw-   0        0        0     5331 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/datasets/xView.yaml
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.459659 ultralytics_custom-8.0.112/ultralytics/hub/
+-rw-rw-rw-   0        0        0     4338 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/hub/__init__.py
+-rw-rw-rw-   0        0        0     5348 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/hub/auth.py
+-rw-rw-rw-   0        0        0     8668 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/hub/session.py
+-rw-rw-rw-   0        0        0     9374 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/hub/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.313099 ultralytics_custom-8.0.112/ultralytics/models/
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.467658 ultralytics_custom-8.0.112/ultralytics/models/rt-detr/
+-rw-rw-rw-   0        0        0     2020 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/rt-detr/rt-detr-l.yaml
+-rw-rw-rw-   0        0        0     2231 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/rt-detr/rt-detr-x.yaml
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.480655 ultralytics_custom-8.0.112/ultralytics/models/v3/
+-rw-rw-rw-   0        0        0     1598 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v3/yolov3-spp.yaml
+-rw-rw-rw-   0        0        0     1291 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-rw-rw-   0        0        0     1585 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v3/yolov3.yaml
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.488658 ultralytics_custom-8.0.112/ultralytics/models/v5/
+-rw-rw-rw-   0        0        0     1984 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v5/yolov5-p6.yaml
+-rw-rw-rw-   0        0        0     1600 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v5/yolov5.yaml
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.492658 ultralytics_custom-8.0.112/ultralytics/models/v6/
+-rw-rw-rw-   0        0        0     1733 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v6/yolov6.yaml
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.513654 ultralytics_custom-8.0.112/ultralytics/models/v8/
+-rw-rw-rw-   0        0        0      949 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-cls.yaml
+-rw-rw-rw-   0        0        0     1805 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-p2.yaml
+-rw-rw-rw-   0        0        0     1912 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-p6.yaml
+-rw-rw-rw-   0        0        0     2003 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-rw-rw-   0        0        0     1627 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-pose.yaml
+-rw-rw-rw-   0        0        0     1536 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-seg.yaml
+-rw-rw-rw-   0        0        0     1959 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8.yaml
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.521654 ultralytics_custom-8.0.112/ultralytics/nn/
+-rw-rw-rw-   0        0        0      564 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/__init__.py
+-rw-rw-rw-   0        0        0    24709 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/autobackend.py
+-rw-rw-rw-   0        0        0    12752 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/autoshape.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.524654 ultralytics_custom-8.0.112/ultralytics/nn/modules/
+-rw-rw-rw-   0        0        0     1616 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0    12120 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/modules/block.py
+-rw-rw-rw-   0        0        0    11944 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/modules/conv.py
+-rw-rw-rw-   0        0        0    17480 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/modules/head.py
+-rw-rw-rw-   0        0        0    16785 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/modules/transformer.py
+-rw-rw-rw-   0        0        0     3322 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/modules/utils.py
+-rw-rw-rw-   0        0        0    34740 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/nn/tasks.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.533658 ultralytics_custom-8.0.112/ultralytics/tracker/
+-rw-rw-rw-   0        0        0      208 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.541653 ultralytics_custom-8.0.112/ultralytics/tracker/cfg/
+-rw-rw-rw-   0        0        0      908 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/cfg/botsort.yaml
+-rw-rw-rw-   0        0        0      705 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-rw-rw-   0        0        0     2374 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/track.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.561658 ultralytics_custom-8.0.112/ultralytics/tracker/trackers/
+-rw-rw-rw-   0        0        0      177 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/trackers/__init__.py
+-rw-rw-rw-   0        0        0     1680 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/trackers/basetrack.py
+-rw-rw-rw-   0        0        0     5832 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/trackers/bot_sort.py
+-rw-rw-rw-   0        0        0    14812 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/trackers/byte_tracker.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.576653 ultralytics_custom-8.0.112/ultralytics/tracker/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/utils/__init__.py
+-rw-rw-rw-   0        0        0    12533 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/utils/gmc.py
+-rw-rw-rw-   0        0        0    18882 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/utils/kalman_filter.py
+-rw-rw-rw-   0        0        0     8928 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/tracker/utils/matching.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.577654 ultralytics_custom-8.0.112/ultralytics/vit/
+-rw-rw-rw-   0        0        0      155 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.579659 ultralytics_custom-8.0.112/ultralytics/vit/rtdetr/
+-rw-rw-rw-   0        0        0      204 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/rtdetr/__init__.py
+-rw-rw-rw-   0        0        0     4722 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/rtdetr/model.py
+-rw-rw-rw-   0        0        0     1946 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/rtdetr/predict.py
+-rw-rw-rw-   0        0        0     4904 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/rtdetr/val.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.582654 ultralytics_custom-8.0.112/ultralytics/vit/sam/
+-rw-rw-rw-   0        0        0      133 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/__init__.py
+-rw-rw-rw-   0        0        0    13615 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/amg.py
+-rw-rw-rw-   0        0        0     3970 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/autosize.py
+-rw-rw-rw-   0        0        0     3906 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/build.py
+-rw-rw-rw-   0        0        0     1853 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/model.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.586654 ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/
+-rw-rw-rw-   0        0        0        0 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/__init__.py
+-rw-rw-rw-   0        0        0     6512 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/decoders.py
+-rw-rw-rw-   0        0        0    23083 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/encoders.py
+-rw-rw-rw-   0        0        0    15601 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/mask_generator.py
+-rw-rw-rw-   0        0        0    11441 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/prompt_predictor.py
+-rw-rw-rw-   0        0        0     7285 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/sam.py
+-rw-rw-rw-   0        0        0     8722 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/transformer.py
+-rw-rw-rw-   0        0        0     2191 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/vit/sam/predict.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.586654 ultralytics_custom-8.0.112/ultralytics/yolo/
+-rw-rw-rw-   0        0        0       99 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.587654 ultralytics_custom-8.0.112/ultralytics/yolo/cfg/
+-rw-rw-rw-   0        0        0    18463 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/cfg/__init__.py
+-rw-rw-rw-   0        0        0     6452 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/cfg/default.yaml
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.602654 ultralytics_custom-8.0.112/ultralytics/yolo/data/
+-rw-rw-rw-   0        0        0      467 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/annotator.py
+-rw-rw-rw-   0        0        0    38062 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/augment.py
+-rw-rw-rw-   0        0        0    12935 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/base.py
+-rw-rw-rw-   0        0        0     6744 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/build.py
+-rw-rw-rw-   0        0        0     9420 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/converter.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.604655 ultralytics_custom-8.0.112/ultralytics/yolo/data/dataloaders/
+-rw-rw-rw-   0        0        0        0 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-rw-rw-   0        0        0    15276 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-rw-rw-   0        0        0    18053 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-rw-rw-   0        0        0    52369 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-rw-rw-   0        0        0    13646 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/dataset.py
+-rw-rw-rw-   0        0        0     1829 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/dataset_wrappers.py
+-rw-rw-rw-   0        0        0    24569 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.609658 ultralytics_custom-8.0.112/ultralytics/yolo/engine/
+-rw-rw-rw-   0        0        0        0 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/engine/__init__.py
+-rw-rw-rw-   0        0        0    41118 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/engine/exporter.py
+-rw-rw-rw-   0        0        0    22608 2023-06-02 02:02:10.000000 ultralytics_custom-8.0.112/ultralytics/yolo/engine/model.py
+-rw-rw-rw-   0        0        0    16549 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/engine/predictor.py
+-rw-rw-rw-   0        0        0    24867 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/engine/results.py
+-rw-rw-rw-   0        0        0    33053 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/engine/trainer.py
+-rw-rw-rw-   0        0        0    11991 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/engine/validator.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.631658 ultralytics_custom-8.0.112/ultralytics/yolo/utils/
+-rw-rw-rw-   0        0        0    28625 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/__init__.py
+-rw-rw-rw-   0        0        0     3936 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/autobatch.py
+-rw-rw-rw-   0        0        0    15781 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/benchmarks.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.637654 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/
+-rw-rw-rw-   0        0        0      219 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     5755 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/base.py
+-rw-rw-rw-   0        0        0     6045 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-rw-rw-   0        0        0    13345 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/comet.py
+-rw-rw-rw-   0        0        0     3397 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/hub.py
+-rw-rw-rw-   0        0        0     2563 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/mlflow.py
+-rw-rw-rw-   0        0        0     3802 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/neptune.py
+-rw-rw-rw-   0        0        0      515 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/raytune.py
+-rw-rw-rw-   0        0        0     1572 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-rw-rw-   0        0        0     2230 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/wb.py
+-rw-rw-rw-   0        0        0    15388 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/checks.py
+-rw-rw-rw-   0        0        0     2663 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/dist.py
+-rw-rw-rw-   0        0        0    12260 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/downloads.py
+-rw-rw-rw-   0        0        0      327 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/errors.py
+-rw-rw-rw-   0        0        0     3688 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/files.py
+-rw-rw-rw-   0        0        0    15051 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/instance.py
+-rw-rw-rw-   0        0        0    18790 2023-06-02 00:18:55.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/loss.py
+-rw-rw-rw-   0        0        0    55228 2023-06-02 00:47:36.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/metrics.py
+-rw-rw-rw-   0        0        0    28977 2023-06-02 00:23:29.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/ops.py
+-rw-rw-rw-   0        0        0     1286 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/patches.py
+-rw-rw-rw-   0        0        0    24946 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/plotting.py
+-rw-rw-rw-   0        0        0    13921 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/tal.py
+-rw-rw-rw-   0        0        0    22693 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/torch_utils.py
+-rw-rw-rw-   0        0        0     2326 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/utils/tuner.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.637654 ultralytics_custom-8.0.112/ultralytics/yolo/v8/
+-rw-rw-rw-   0        0        0      163 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.639654 ultralytics_custom-8.0.112/ultralytics/yolo/v8/classify/
+-rw-rw-rw-   0        0        0      398 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/classify/__init__.py
+-rw-rw-rw-   0        0        0     1980 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/classify/predict.py
+-rw-rw-rw-   0        0        0     7090 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/classify/train.py
+-rw-rw-rw-   0        0        0     4785 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/classify/val.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.641654 ultralytics_custom-8.0.112/ultralytics/yolo/v8/detect/
+-rw-rw-rw-   0        0        0      284 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/detect/__init__.py
+-rw-rw-rw-   0        0        0     1902 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/detect/predict.py
+-rw-rw-rw-   0        0        0     7391 2023-06-02 01:42:05.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/detect/train.py
+-rw-rw-rw-   0        0        0    15011 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/detect/val.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.643654 ultralytics_custom-8.0.112/ultralytics/yolo/v8/pose/
+-rw-rw-rw-   0        0        0      254 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/pose/__init__.py
+-rw-rw-rw-   0        0        0     2433 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/pose/predict.py
+-rw-rw-rw-   0        0        0     2867 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/pose/train.py
+-rw-rw-rw-   0        0        0    11141 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/pose/val.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:45:11.645654 ultralytics_custom-8.0.112/ultralytics/yolo/v8/segment/
+-rw-rw-rw-   0        0        0      302 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/segment/__init__.py
+-rw-rw-rw-   0        0        0     2902 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/segment/predict.py
+-rw-rw-rw-   0        0        0     2564 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/segment/train.py
+-rw-rw-rw-   0        0        0    13143 2023-06-01 19:51:46.000000 ultralytics_custom-8.0.112/ultralytics/yolo/v8/segment/val.py
+drwxrwxrwx   0        0        0        0 2023-06-02 03:19:24.639003 ultralytics_custom-8.0.112/ultralytics_custom.egg-info/
+-rw-rw-rw-   0        0        0    26239 2023-06-02 03:19:24.000000 ultralytics_custom-8.0.112/ultralytics_custom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5496 2023-06-02 03:19:24.000000 ultralytics_custom-8.0.112/ultralytics_custom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 03:19:24.000000 ultralytics_custom-8.0.112/ultralytics_custom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-06-02 03:19:24.000000 ultralytics_custom-8.0.112/ultralytics_custom.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      369 2023-06-02 03:19:24.000000 ultralytics_custom-8.0.112/ultralytics_custom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 03:19:24.000000 ultralytics_custom-8.0.112/ultralytics_custom.egg-info/top_level.txt
```

### Comparing `ultralytics_custom-0.0.0/CONTRIBUTING.md` & `ultralytics_custom-8.0.112/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/LICENSE` & `ultralytics_custom-8.0.112/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/PKG-INFO` & `ultralytics_custom-8.0.112/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics_custom
-Version: 0.0.0
+Version: 8.0.112
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics_custom Version: 0.0.0 Summary:
+Metadata-Version: 2.1 Name: ultralytics_custom Version: 8.0.112 Summary:
 Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance
 segmentation, pose estimation and image classification. Home-page: https://
 github.com/ultralytics/ultralytics Author: Ultralytics Author-email:
 hello@ultralytics.com License: AGPL-3.0 Project-URL: Bug Reports, https://
 github.com/ultralytics/ultralytics/issues Project-URL: Funding, https://
 ultralytics.com Project-URL: Source, https://github.com/ultralytics/ultralytics
 Keywords: machine-learning,deep-
```

### Comparing `ultralytics_custom-0.0.0/README.md` & `ultralytics_custom-8.0.112/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/README.zh-CN.md` & `ultralytics_custom-8.0.112/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/requirements.txt` & `ultralytics_custom-8.0.112/requirements.txt`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/setup.cfg` & `ultralytics_custom-8.0.112/setup.cfg`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/setup.py` & `ultralytics_custom-8.0.112/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 import pkg_resources as pkg
 from setuptools import find_packages, setup
 
 # Settings
 FILE = Path(__file__).resolve()
 PARENT = FILE.parent  # root directory
 README = (PARENT / 'README.md').read_text(encoding='utf-8')
-REQUIREMENTS = [f'{x.name}{x.specifier}' for x in pkg.parse_requirements((PARENT / 'requirements.txt').read_text())]
+REQUIREMENTS = [f'{x.name}{x.specifier}' for x in pkg.parse_requirements((PARENT / 'requirements.txt').read_text(encoding='utf-8'))]
 
 
 def get_version():
     file = PARENT / 'ultralytics/__init__.py'
     return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', file.read_text(encoding='utf-8'), re.M)[1]
 
 
 setup(
     name='ultralytics_custom',  # name of pypi package
-    # version=get_version(),  # version of pypi package
-    version='0.0.0',
+    version=get_version(),  # version of pypi package
     python_requires='>=3.7',
     license='AGPL-3.0',
     description=('Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, '
                  'pose estimation and image classification.'),
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/ultralytics/ultralytics',
```

### Comparing `ultralytics_custom-0.0.0/ultralytics/assets/bus.jpg` & `ultralytics_custom-8.0.112/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/assets/zidane.jpg` & `ultralytics_custom-8.0.112/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/Argoverse.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/GlobalWheat2020.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/ImageNet.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/Objects365.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/SKU-110K.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/VOC.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/VisDrone.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/coco-pose.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/coco.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/coco128-seg.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/coco128.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/coco8-pose.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/coco8-seg.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/coco8.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/datasets/xView.yaml` & `ultralytics_custom-8.0.112/ultralytics/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/hub/__init__.py` & `ultralytics_custom-8.0.112/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/hub/auth.py` & `ultralytics_custom-8.0.112/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/hub/session.py` & `ultralytics_custom-8.0.112/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/hub/utils.py` & `ultralytics_custom-8.0.112/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/rt-detr/rt-detr-l.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/rt-detr/rt-detr-l.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/rt-detr/rt-detr-x.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/rt-detr/rt-detr-x.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v3/yolov3-spp.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v3/yolov3-tiny.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v3/yolov3.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v5/yolov5-p6.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v5/yolov5.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v6/yolov6.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-cls.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-p2.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-p6.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-pose-p6.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-pose.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8-seg.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/models/v8/yolov8.yaml` & `ultralytics_custom-8.0.112/ultralytics/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/__init__.py` & `ultralytics_custom-8.0.112/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/autobackend.py` & `ultralytics_custom-8.0.112/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/autoshape.py` & `ultralytics_custom-8.0.112/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/modules/__init__.py` & `ultralytics_custom-8.0.112/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/modules/block.py` & `ultralytics_custom-8.0.112/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/modules/conv.py` & `ultralytics_custom-8.0.112/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/modules/head.py` & `ultralytics_custom-8.0.112/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/modules/transformer.py` & `ultralytics_custom-8.0.112/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/modules/utils.py` & `ultralytics_custom-8.0.112/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/nn/tasks.py` & `ultralytics_custom-8.0.112/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/tracker/cfg/botsort.yaml` & `ultralytics_custom-8.0.112/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/tracker/cfg/bytetrack.yaml` & `ultralytics_custom-8.0.112/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/tracker/track.py` & `ultralytics_custom-8.0.112/ultralytics/tracker/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/tracker/trackers/basetrack.py` & `ultralytics_custom-8.0.112/ultralytics/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/tracker/trackers/bot_sort.py` & `ultralytics_custom-8.0.112/ultralytics/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/tracker/trackers/byte_tracker.py` & `ultralytics_custom-8.0.112/ultralytics/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/tracker/utils/gmc.py` & `ultralytics_custom-8.0.112/ultralytics/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/tracker/utils/kalman_filter.py` & `ultralytics_custom-8.0.112/ultralytics/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/tracker/utils/matching.py` & `ultralytics_custom-8.0.112/ultralytics/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/rtdetr/model.py` & `ultralytics_custom-8.0.112/ultralytics/vit/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/rtdetr/predict.py` & `ultralytics_custom-8.0.112/ultralytics/vit/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/rtdetr/val.py` & `ultralytics_custom-8.0.112/ultralytics/vit/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/amg.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/autosize.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/autosize.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/build.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/model.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/decoders.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/encoders.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/mask_generator.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/mask_generator.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/prompt_predictor.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/prompt_predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/sam.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/modules/transformer.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/vit/sam/predict.py` & `ultralytics_custom-8.0.112/ultralytics/vit/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/cfg/__init__.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/cfg/default.yaml` & `ultralytics_custom-8.0.112/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/annotator.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/augment.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/base.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/build.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/converter.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/dataloaders/v5loader.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/dataset.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/dataset_wrappers.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/data/utils.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/engine/exporter.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/engine/model.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/engine/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         """
         Initializes the YOLO model.
 
         Args:
             model (Union[str, Path], optional): Path or name of the model to load or create. Defaults to 'yolov8n.pt'.
             task (Any, optional): Task type for the YOLO model. Defaults to None.
         """
-        print('🧊🧊custom yolov8🧊🧊')
+        print("custom yolov8🧊🧊🧊")
         self.callbacks = callbacks.get_default_callbacks()
         self.predictor = None  # reuse predictor
         self.model = None  # model object
         self.trainer = None  # trainer object
         self.task = None  # task type
         self.ckpt = None  # if loaded from *.pt
         self.cfg = None  # if loaded from *.yaml
```

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/engine/predictor.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/engine/results.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/engine/trainer.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/engine/validator.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/__init__.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/autobatch.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/benchmarks.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/base.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/clearml.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/comet.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/hub.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/mlflow.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/neptune.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/raytune.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/tensorboard.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/callbacks/wb.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/checks.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/dist.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/downloads.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/files.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/instance.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/loss.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 
 from ultralytics.yolo.utils.metrics import OKS_SIGMA
 from ultralytics.yolo.utils.ops import crop_mask, xywh2xyxy, xyxy2xywh
 from ultralytics.yolo.utils.tal import TaskAlignedAssigner, dist2bbox, make_anchors
 
-from .metrics import bbox_iou
+from .metrics import bbox_iou,bbox_iou_for_nms
 from .tal import bbox2dist
 
 
 class VarifocalLoss(nn.Module):
     """Varifocal loss by Zhang et al. https://arxiv.org/abs/2008.13367."""
 
     def __init__(self):
@@ -35,17 +35,21 @@
         super().__init__()
         self.reg_max = reg_max
         self.use_dfl = use_dfl
 
     def forward(self, pred_dist, pred_bboxes, anchor_points, target_bboxes, target_scores, target_scores_sum, fg_mask):
         """IoU loss."""
         weight = target_scores.sum(-1)[fg_mask].unsqueeze(-1)
-        iou = bbox_iou(pred_bboxes[fg_mask], target_bboxes[fg_mask], xywh=False, CIoU=True)
+        # # WIoU
+        iou = bbox_iou_for_nms(pred_bboxes[fg_mask], target_bboxes[fg_mask], xywh=False, WIoU=True,scale=True)
         if type(iou) is tuple:
-            loss_iou = ((1.0 - iou[0]) * iou[1].detach() * weight).sum() / target_scores_sum
+            if len(iou) == 2:
+                loss_iou = ((1.0 - iou[0]) * iou[1].detach() * weight).sum() / target_scores_sum
+            else:
+                loss_iou = (iou[0] * iou[1] * weight).sum() / target_scores_sum
         else:
             loss_iou = ((1.0 - iou) * weight).sum() / target_scores_sum
 
         # DFL loss
         if self.use_dfl:
             target_ltrb = bbox2dist(anchor_points, target_bboxes, self.reg_max)
             loss_dfl = self._df_loss(pred_dist[fg_mask].view(-1, self.reg_max + 1), target_ltrb[fg_mask]) * weight
```

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/metrics.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,65 +69,191 @@
     (a1, a2), (b1, b2) = box1.unsqueeze(1).chunk(2, 2), box2.unsqueeze(0).chunk(2, 2)
     inter = (torch.min(a2, b2) - torch.max(a1, b1)).clamp_(0).prod(2)
 
     # IoU = inter / (area1 + area2 - inter)
     return inter / ((a2 - a1).prod(2) + (b2 - b1).prod(2) - inter + eps)
 
 
-def bbox_iou(box1, box2, xywh=True, GIoU=False, DIoU=False, CIoU=False, SIoU=False, EIoU=False, Focal=False, alpha=1, gamma=0.5, eps=1e-7):
+class WIoU_Scale:
+    ''' monotonous: {
+            None: origin v1
+            True: monotonic FM v2
+            False: non-monotonic FM v3
+        }
+        momentum: The momentum of running mean'''
+    
+    iou_mean = 1.
+    monotonous = False
+    _momentum = 1 - 0.5 ** (1 / 7000)
+    _is_train = True
+ 
+    def __init__(self, iou):
+        self.iou = iou
+        self._update(self)
+    
+    @classmethod
+    def _update(cls, self):
+        if cls._is_train: cls.iou_mean = (1 - cls._momentum) * cls.iou_mean + \
+                                         cls._momentum * self.iou.detach().mean().item()
+    
+    @classmethod
+    def _scaled_loss(cls, self, gamma=1.9, delta=3):
+        if isinstance(self.monotonous, bool):
+            if self.monotonous:
+                return (self.iou.detach() / self.iou_mean).sqrt()
+            else:
+                beta = self.iou.detach() / self.iou_mean
+                alpha = delta * torch.pow(gamma, beta - delta)
+                return beta / alpha
+        return 1
+    
+ 
+def bbox_iou(box1, box2, xywh=True, GIoU=False, DIoU=False, CIoU=False, SIoU=False, EIoU=False, WIoU=False, Focal=False, alpha=1, gamma=0.5, scale=False, eps=1e-7):
     # Returns Intersection over Union (IoU) of box1(1,4) to box2(n,4)
-
+ 
     # Get the coordinates of bounding boxes
     if xywh:  # transform from xywh to xyxy
         (x1, y1, w1, h1), (x2, y2, w2, h2) = box1.chunk(4, -1), box2.chunk(4, -1)
         w1_, h1_, w2_, h2_ = w1 / 2, h1 / 2, w2 / 2, h2 / 2
         b1_x1, b1_x2, b1_y1, b1_y2 = x1 - w1_, x1 + w1_, y1 - h1_, y1 + h1_
         b2_x1, b2_x2, b2_y1, b2_y2 = x2 - w2_, x2 + w2_, y2 - h2_, y2 + h2_
     else:  # x1, y1, x2, y2 = box1
         b1_x1, b1_y1, b1_x2, b1_y2 = box1.chunk(4, -1)
         b2_x1, b2_y1, b2_x2, b2_y2 = box2.chunk(4, -1)
         w1, h1 = b1_x2 - b1_x1, (b1_y2 - b1_y1).clamp(eps)
         w2, h2 = b2_x2 - b2_x1, (b2_y2 - b2_y1).clamp(eps)
-
+ 
     # Intersection area
     inter = (b1_x2.minimum(b2_x2) - b1_x1.maximum(b2_x1)).clamp(0) * \
             (b1_y2.minimum(b2_y2) - b1_y1.maximum(b2_y1)).clamp(0)
-
+ 
     # Union Area
     union = w1 * h1 + w2 * h2 - inter + eps
-
+    if scale:
+        self = WIoU_Scale(1 - (inter / union))
+ 
+    # IoU
+    # iou = inter / union # ori iou
+    iou = torch.pow(inter/(union + eps), alpha) # alpha iou
+    if CIoU or DIoU or GIoU or EIoU or SIoU or WIoU:
+        cw = b1_x2.maximum(b2_x2) - b1_x1.minimum(b2_x1)  # convex (smallest enclosing box) width
+        ch = b1_y2.maximum(b2_y2) - b1_y1.minimum(b2_y1)  # convex height
+        if CIoU or DIoU or EIoU or SIoU or WIoU:  # Distance or Complete IoU https://arxiv.org/abs/1911.08287v1
+            c2 = (cw ** 2 + ch ** 2) ** alpha + eps  # convex diagonal squared
+            rho2 = (((b2_x1 + b2_x2 - b1_x1 - b1_x2) ** 2 + (b2_y1 + b2_y2 - b1_y1 - b1_y2) ** 2) / 4) ** alpha  # center dist ** 2
+            if CIoU:  # https://github.com/Zzh-tju/DIoU-SSD-pytorch/blob/master/utils/box/box_utils.py#L47
+                v = (4 / math.pi ** 2) * (torch.atan(w2 / h2) - torch.atan(w1 / h1)).pow(2)
+                with torch.no_grad():
+                    alpha_ciou = v / (v - iou + (1 + eps))
+                if Focal:
+                    return iou - (rho2 / c2 + torch.pow(v * alpha_ciou + eps, alpha)), torch.pow(inter/(union + eps), gamma)  # Focal_CIoU
+                else:
+                    return iou - (rho2 / c2 + torch.pow(v * alpha_ciou + eps, alpha))  # CIoU
+            elif EIoU:
+                rho_w2 = ((b2_x2 - b2_x1) - (b1_x2 - b1_x1)) ** 2
+                rho_h2 = ((b2_y2 - b2_y1) - (b1_y2 - b1_y1)) ** 2
+                cw2 = torch.pow(cw ** 2 + eps, alpha)
+                ch2 = torch.pow(ch ** 2 + eps, alpha)
+                if Focal:
+                    return iou - (rho2 / c2 + rho_w2 / cw2 + rho_h2 / ch2), torch.pow(inter/(union + eps), gamma) # Focal_EIou
+                else:
+                    return iou - (rho2 / c2 + rho_w2 / cw2 + rho_h2 / ch2) # EIou
+            elif SIoU:
+                # SIoU Loss https://arxiv.org/pdf/2205.12740.pdf
+                s_cw = (b2_x1 + b2_x2 - b1_x1 - b1_x2) * 0.5 + eps
+                s_ch = (b2_y1 + b2_y2 - b1_y1 - b1_y2) * 0.5 + eps
+                sigma = torch.pow(s_cw ** 2 + s_ch ** 2, 0.5)
+                sin_alpha_1 = torch.abs(s_cw) / sigma
+                sin_alpha_2 = torch.abs(s_ch) / sigma
+                threshold = pow(2, 0.5) / 2
+                sin_alpha = torch.where(sin_alpha_1 > threshold, sin_alpha_2, sin_alpha_1)
+                angle_cost = torch.cos(torch.arcsin(sin_alpha) * 2 - math.pi / 2)
+                rho_x = (s_cw / cw) ** 2
+                rho_y = (s_ch / ch) ** 2
+                gamma = angle_cost - 2
+                distance_cost = 2 - torch.exp(gamma * rho_x) - torch.exp(gamma * rho_y)
+                omiga_w = torch.abs(w1 - w2) / torch.max(w1, w2)
+                omiga_h = torch.abs(h1 - h2) / torch.max(h1, h2)
+                shape_cost = torch.pow(1 - torch.exp(-1 * omiga_w), 4) + torch.pow(1 - torch.exp(-1 * omiga_h), 4)
+                if Focal:
+                    return iou - torch.pow(0.5 * (distance_cost + shape_cost) + eps, alpha), torch.pow(inter/(union + eps), gamma) # Focal_SIou
+                else:
+                    return iou - torch.pow(0.5 * (distance_cost + shape_cost) + eps, alpha) # SIou
+            elif WIoU:
+                if Focal:
+                    raise RuntimeError("WIoU do not support Focal.")
+                elif scale:
+                    return getattr(WIoU_Scale, '_scaled_loss')(self), (1 - iou) * torch.exp((rho2 / c2)), iou # WIoU https://arxiv.org/abs/2301.10051
+                else:
+                    return iou, torch.exp((rho2 / c2)) # WIoU v1
+            if Focal:
+                return iou - rho2 / c2, torch.pow(inter/(union + eps), gamma)  # Focal_DIoU
+            else:
+                return iou - rho2 / c2  # DIoU
+        c_area = cw * ch + eps  # convex area
+        if Focal:
+            return iou - torch.pow((c_area - union) / c_area + eps, alpha), torch.pow(inter/(union + eps), gamma)  # Focal_GIoU https://arxiv.org/pdf/1902.09630.pdf
+        else:
+            return iou - torch.pow((c_area - union) / c_area + eps, alpha)  # GIoU https://arxiv.org/pdf/1902.09630.pdf
+    if Focal:
+        return iou, torch.pow(inter/(union + eps), gamma)  # Focal_IoU
+    else:
+        return iou  # IoU
+    
+    
+def bbox_iou_for_nms(box1, box2, xywh=True, GIoU=False, DIoU=False, CIoU=False, SIoU=False, EIoU=False, WIoU=False, Focal=False, alpha=1, gamma=0.5, scale=False, eps=1e-7):
+    # Returns Intersection over Union (IoU) of box1(1,4) to box2(n,4)
+ 
+    # Get the coordinates of bounding boxes
+    if xywh:  # transform from xywh to xyxy
+        (x1, y1, w1, h1), (x2, y2, w2, h2) = box1.chunk(4, -1), box2.chunk(4, -1)
+        w1_, h1_, w2_, h2_ = w1 / 2, h1 / 2, w2 / 2, h2 / 2
+        b1_x1, b1_x2, b1_y1, b1_y2 = x1 - w1_, x1 + w1_, y1 - h1_, y1 + h1_
+        b2_x1, b2_x2, b2_y1, b2_y2 = x2 - w2_, x2 + w2_, y2 - h2_, y2 + h2_
+    else:  # x1, y1, x2, y2 = box1
+        b1_x1, b1_y1, b1_x2, b1_y2 = box1.chunk(4, -1)
+        b2_x1, b2_y1, b2_x2, b2_y2 = box2.chunk(4, -1)
+        w1, h1 = b1_x2 - b1_x1, (b1_y2 - b1_y1).clamp(eps)
+        w2, h2 = b2_x2 - b2_x1, (b2_y2 - b2_y1).clamp(eps)
+ 
+    # Intersection area
+    inter = (b1_x2.minimum(b2_x2) - b1_x1.maximum(b2_x1)).clamp(0) * \
+            (b1_y2.minimum(b2_y2) - b1_y1.maximum(b2_y1)).clamp(0)
+ 
+    # Union Area
+    union = w1 * h1 + w2 * h2 - inter + eps
+    if scale:
+        self = WIoU_Scale(1 - (inter / union))
+ 
     # IoU
     # iou = inter / union # ori iou
-    iou = torch.pow(inter / (union + eps), alpha)  # alpha iou
-    if CIoU or DIoU or GIoU or EIoU or SIoU:
+    iou = torch.pow(inter/(union + eps), alpha) # alpha iou
+    if CIoU or DIoU or GIoU or EIoU or SIoU or WIoU:
         cw = b1_x2.maximum(b2_x2) - b1_x1.minimum(b2_x1)  # convex (smallest enclosing box) width
         ch = b1_y2.maximum(b2_y2) - b1_y1.minimum(b2_y1)  # convex height
-        if CIoU or DIoU or EIoU or SIoU:  # Distance or Complete IoU https://arxiv.org/abs/1911.08287v1
+        if CIoU or DIoU or EIoU or SIoU or WIoU:  # Distance or Complete IoU https://arxiv.org/abs/1911.08287v1
             c2 = (cw ** 2 + ch ** 2) ** alpha + eps  # convex diagonal squared
-            rho2 = (((b2_x1 + b2_x2 - b1_x1 - b1_x2) ** 2 + (b2_y1 + b2_y2 -
-                    b1_y1 - b1_y2) ** 2) / 4) ** alpha  # center dist ** 2
+            rho2 = (((b2_x1 + b2_x2 - b1_x1 - b1_x2) ** 2 + (b2_y1 + b2_y2 - b1_y1 - b1_y2) ** 2) / 4) ** alpha  # center dist ** 2
             if CIoU:  # https://github.com/Zzh-tju/DIoU-SSD-pytorch/blob/master/utils/box/box_utils.py#L47
                 v = (4 / math.pi ** 2) * (torch.atan(w2 / h2) - torch.atan(w1 / h1)).pow(2)
                 with torch.no_grad():
                     alpha_ciou = v / (v - iou + (1 + eps))
                 if Focal:
-                    # Focal_CIoU
-                    return iou - (rho2 / c2 + torch.pow(v * alpha_ciou + eps, alpha)), torch.pow(inter / (union + eps), gamma)
+                    return iou - (rho2 / c2 + torch.pow(v * alpha_ciou + eps, alpha)), torch.pow(inter/(union + eps), gamma)  # Focal_CIoU
                 else:
                     return iou - (rho2 / c2 + torch.pow(v * alpha_ciou + eps, alpha))  # CIoU
             elif EIoU:
                 rho_w2 = ((b2_x2 - b2_x1) - (b1_x2 - b1_x1)) ** 2
                 rho_h2 = ((b2_y2 - b2_y1) - (b1_y2 - b1_y1)) ** 2
                 cw2 = torch.pow(cw ** 2 + eps, alpha)
                 ch2 = torch.pow(ch ** 2 + eps, alpha)
                 if Focal:
-                    # Focal_EIou
-                    return iou - (rho2 / c2 + rho_w2 / cw2 + rho_h2 / ch2), torch.pow(inter / (union + eps), gamma)
+                    return iou - (rho2 / c2 + rho_w2 / cw2 + rho_h2 / ch2), torch.pow(inter/(union + eps), gamma) # Focal_EIou
                 else:
-                    return iou - (rho2 / c2 + rho_w2 / cw2 + rho_h2 / ch2)  # EIou
+                    return iou - (rho2 / c2 + rho_w2 / cw2 + rho_h2 / ch2) # EIou
             elif SIoU:
                 # SIoU Loss https://arxiv.org/pdf/2205.12740.pdf
                 s_cw = (b2_x1 + b2_x2 - b1_x1 - b1_x2) * 0.5 + eps
                 s_ch = (b2_y1 + b2_y2 - b1_y1 - b1_y2) * 0.5 + eps
                 sigma = torch.pow(s_cw ** 2 + s_ch ** 2, 0.5)
                 sin_alpha_1 = torch.abs(s_cw) / sigma
                 sin_alpha_2 = torch.abs(s_ch) / sigma
@@ -138,32 +264,69 @@
                 rho_y = (s_ch / ch) ** 2
                 gamma = angle_cost - 2
                 distance_cost = 2 - torch.exp(gamma * rho_x) - torch.exp(gamma * rho_y)
                 omiga_w = torch.abs(w1 - w2) / torch.max(w1, w2)
                 omiga_h = torch.abs(h1 - h2) / torch.max(h1, h2)
                 shape_cost = torch.pow(1 - torch.exp(-1 * omiga_w), 4) + torch.pow(1 - torch.exp(-1 * omiga_h), 4)
                 if Focal:
-                    # Focal_SIou
-                    return iou - torch.pow(0.5 * (distance_cost + shape_cost) + eps, alpha), torch.pow(inter / (union + eps), gamma)
+                    return iou - torch.pow(0.5 * (distance_cost + shape_cost) + eps, alpha), torch.pow(inter/(union + eps), gamma) # Focal_SIou
                 else:
-                    return iou - torch.pow(0.5 * (distance_cost + shape_cost) + eps, alpha)  # SIou
+                    return iou - torch.pow(0.5 * (distance_cost + shape_cost) + eps, alpha) # SIou
+            elif WIoU:
+                if Focal:
+                    raise RuntimeError("WIoU do not support Focal.")
+                elif scale:
+                    return getattr(WIoU_Scale, '_scaled_loss')(self), (1 - iou) * torch.exp((rho2 / c2)), iou # WIoU https://arxiv.org/abs/2301.10051
+                else:
+                    return iou, torch.exp((rho2 / c2)) # WIoU v1
             if Focal:
-                return iou - rho2 / c2, torch.pow(inter / (union + eps), gamma)  # Focal_DIoU
+                return iou - rho2 / c2, torch.pow(inter/(union + eps), gamma)  # Focal_DIoU
             else:
                 return iou - rho2 / c2  # DIoU
         c_area = cw * ch + eps  # convex area
         if Focal:
-            # Focal_GIoU https://arxiv.org/pdf/1902.09630.pdf
-            return iou - torch.pow((c_area - union) / c_area + eps, alpha), torch.pow(inter / (union + eps), gamma)
+            return iou - torch.pow((c_area - union) / c_area + eps, alpha), torch.pow(inter/(union + eps), gamma)  # Focal_GIoU https://arxiv.org/pdf/1902.09630.pdf
         else:
             return iou - torch.pow((c_area - union) / c_area + eps, alpha)  # GIoU https://arxiv.org/pdf/1902.09630.pdf
     if Focal:
-        return iou, torch.pow(inter / (union + eps), gamma)  # Focal_IoU
+        return iou, torch.pow(inter/(union + eps), gamma)  # Focal_IoU
     else:
         return iou  # IoU
+ 
+ 
+def soft_nms(bboxes, scores, iou_thresh=0.5,sigma=0.5,score_threshold=0.25):
+    order = torch.arange(0, scores.size(0)).to(bboxes.device)
+    keep = []
+    
+    while order.numel() > 1:
+        if order.numel() == 1:
+            keep.append(order[0])
+            break
+        else:
+            i = order[0]
+            keep.append(i)
+        
+        iou = bbox_iou_for_nms(bboxes[i], bboxes[order[1:]], EIoU=True).squeeze()
+        
+        idx = (iou > iou_thresh).nonzero().squeeze()
+        if idx.numel() > 0: 
+            iou = iou[idx] 
+            newScores = torch.exp(-torch.pow(iou,2)/sigma)
+            scores[order[idx+1]] *= newScores
+        
+        newOrder = (scores[order[1:]] > score_threshold).nonzero().squeeze() 
+        if newOrder.numel() == 0: 
+            break
+        else:
+            maxScoreIndex = torch.argmax(scores[order[newOrder+1]]) 
+            if maxScoreIndex != 0: 
+                newOrder[[0,maxScoreIndex],] = newOrder[[maxScoreIndex,0],]
+            order = order[newOrder+1]
+    
+    return torch.LongTensor(keep)
 
 
 def mask_iou(mask1, mask2, eps=1e-7):
     """
     Calculate masks IoU.
 
     Args:
@@ -460,18 +623,29 @@
     mrec = np.concatenate(([0.0], recall, [1.0]))
     mpre = np.concatenate(([1.0], precision, [0.0]))
 
     # Compute the precision envelope
     mpre = np.flip(np.maximum.accumulate(np.flip(mpre)))
 
     # Integrate area under curve
-    method = 'interp'  # methods: 'continuous', 'interp'
+    method = 'searchsorted'  # methods: 'continuous','searchsorted','interp'
     if method == 'interp':
         x = np.linspace(0, 1, 101)  # 101-point interp (COCO)
         ap = np.trapz(np.interp(x, mrec, mpre), x)  # integrate
+    elif method == 'searchsorted':
+        q = np.zeros((101,))
+        x = np.linspace(0, 1, 101)
+        inds = np.searchsorted(recall, x, side='left')
+        try:
+            for ri,pi in enumerate(inds):
+                q[ri] = precision[pi]
+        except:
+            pass
+        q_array = np.array(q)
+        ap = np.mean(q_array[q_array > -1])
     else:  # 'continuous'
         i = np.where(mrec[1:] != mrec[:-1])[0]  # points where x-axis (recall) changes
         ap = np.sum((mrec[i + 1] - mrec[i]) * mpre[i + 1])  # area under curve
 
     return ap, mpre, mrec
```

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/ops.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import torch
 import torch.nn.functional as F
 import torchvision
 
 from ultralytics.yolo.utils import LOGGER
 
-from .metrics import box_iou
+from .metrics import box_iou,soft_nms
 
 
 class Profile(contextlib.ContextDecorator):
     """
     YOLOv8 Profile class.
     Usage: as a decorator with @Profile() or as a context manager with 'with Profile():'
     """
@@ -242,15 +242,15 @@
         if not n:  # no boxes
             continue
         x = x[x[:, 4].argsort(descending=True)[:max_nms]]  # sort by confidence and remove excess boxes
 
         # Batched NMS
         c = x[:, 5:6] * (0 if agnostic else max_wh)  # classes
         boxes, scores = x[:, :4] + c, x[:, 4]  # boxes (offset by class), scores
-        i = torchvision.ops.nms(boxes, scores, iou_thres)  # NMS
+        i = soft_nms(boxes, scores, iou_thres)  # NMS
         i = i[:max_det]  # limit detections
         if merge and (1 < n < 3E3):  # Merge NMS (boxes merged using weighted mean)
             # Update boxes as boxes(i,4) = weights(i,n) * boxes(n,4)
             iou = box_iou(boxes[i], boxes) > iou_thres  # iou matrix
             weights = iou * scores[None]  # box weights
             x[i, :4] = torch.mm(weights, x[:, :4]).float() / weights.sum(1, keepdim=True)  # merged boxes
             if redundant:
```

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/patches.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/plotting.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/tal.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/torch_utils.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/utils/tuner.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/classify/predict.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/classify/train.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/classify/val.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/detect/predict.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/detect/train.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/detect/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,8 +136,9 @@
         YOLO(model).train(**args)
     else:
         trainer = DetectionTrainer(overrides=args)
         trainer.train()
 
 
 if __name__ == '__main__':
+    print('this is custom yolov8 🧊🧊🧊')
     train()
```

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/detect/val.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/pose/predict.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/pose/train.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/pose/val.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/segment/predict.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/segment/train.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics/yolo/v8/segment/val.py` & `ultralytics_custom-8.0.112/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics_custom-0.0.0/ultralytics_custom.egg-info/PKG-INFO` & `ultralytics_custom-8.0.112/ultralytics_custom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics-custom
-Version: 0.0.0
+Version: 8.0.112
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics-custom Version: 0.0.0 Summary:
+Metadata-Version: 2.1 Name: ultralytics-custom Version: 8.0.112 Summary:
 Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance
 segmentation, pose estimation and image classification. Home-page: https://
 github.com/ultralytics/ultralytics Author: Ultralytics Author-email:
 hello@ultralytics.com License: AGPL-3.0 Project-URL: Bug Reports, https://
 github.com/ultralytics/ultralytics/issues Project-URL: Funding, https://
 ultralytics.com Project-URL: Source, https://github.com/ultralytics/ultralytics
 Keywords: machine-learning,deep-
```

### Comparing `ultralytics_custom-0.0.0/ultralytics_custom.egg-info/SOURCES.txt` & `ultralytics_custom-8.0.112/ultralytics_custom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

