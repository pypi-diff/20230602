# Comparing `tmp/clarifai-9.5.1.tar.gz` & `tmp/clarifai-9.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.5.1.tar", last modified: Fri Jun  2 14:49:32 2023, max compression
+gzip compressed data, was "clarifai-9.5.2.tar", last modified: Fri Jun  2 20:19:37 2023, max compression
```

## Comparing `clarifai-9.5.1.tar` & `clarifai-9.5.2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.590064 clarifai-9.5.1/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      555 2023-06-01 21:00:24.000000 clarifai-9.5.1/LICENSE
--rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-06-01 21:00:24.000000 clarifai-9.5.1/MANIFEST.in
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-06-02 14:49:32.589928 clarifai-9.5.1/PKG-INFO
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2347 2023-06-01 21:00:24.000000 clarifai-9.5.1/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.576762 clarifai-9.5.1/clarifai/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.577631 clarifai-9.5.1/clarifai/auth/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/auth/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    12239 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/auth/helper.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.578318 clarifai-9.5.1/clarifai/client/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/client/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/client/abc.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/client/stub.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.578703 clarifai-9.5.1/clarifai/data_upload/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.579518 clarifai-9.5.1/clarifai/data_upload/datasets/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    10349 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.580371 clarifai-9.5.1/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1414 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.574378 clarifai-9.5.1/clarifai/data_upload/examples/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.580509 clarifai-9.5.1/clarifai/data_upload/examples/image_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.580699 clarifai-9.5.1/clarifai/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.580931 clarifai-9.5.1/clarifai/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.581119 clarifai-9.5.1/clarifai/data_upload/examples/text_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.581313 clarifai-9.5.1/clarifai/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/examples.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    13040 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/data_upload/upload.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.581571 clarifai-9.5.1/clarifai/dataset_export/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     5130 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.583140 clarifai-9.5.1/clarifai/listing/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/listing/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/listing/concepts.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/listing/datasets.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/listing/inputs.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/listing/lister.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/listing/models.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/listing/module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/listing/modules.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.583518 clarifai-9.5.1/clarifai/modules/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/modules/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/modules/css.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/modules/pages.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.583653 clarifai-9.5.1/clarifai/urls/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3172 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai/urls/helper.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.577417 clarifai-9.5.1/clarifai.egg-info/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-06-02 14:49:32.000000 clarifai-9.5.1/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4038 2023-06-02 14:49:32.000000 clarifai-9.5.1/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)        1 2023-06-02 14:49:32.000000 clarifai-9.5.1/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-06-02 14:49:32.000000 clarifai-9.5.1/clarifai.egg-info/requires.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       24 2023-06-02 14:49:32.000000 clarifai-9.5.1/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.583815 clarifai-9.5.1/clarifai_utils/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.584004 clarifai-9.5.1/clarifai_utils/auth/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/auth/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    12239 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.584390 clarifai-9.5.1/clarifai_utils/client/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/client/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/client/abc.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/client/stub.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.584732 clarifai-9.5.1/clarifai_utils/data_upload/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.585331 clarifai-9.5.1/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    10349 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.586090 clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1414 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.575458 clarifai-9.5.1/clarifai_utils/data_upload/examples/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.586233 clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.586428 clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.586650 clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.586781 clarifai-9.5.1/clarifai_utils/data_upload/examples/text_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.586986 clarifai-9.5.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    13040 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.587121 clarifai-9.5.1/clarifai_utils/dataset_export/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     5130 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.588260 clarifai-9.5.1/clarifai_utils/listing/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/listing/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/listing/concepts.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/listing/datasets.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/listing/inputs.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/listing/lister.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/listing/models.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.588826 clarifai-9.5.1/clarifai_utils/modules/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/modules/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/modules/css.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/modules/pages.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     5230 2023-06-02 14:43:49.000000 clarifai-9.5.1/clarifai_utils/modules/style.css
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.589066 clarifai-9.5.1/clarifai_utils/urls/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3172 2023-06-01 21:00:24.000000 clarifai-9.5.1/clarifai_utils/urls/helper.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)       38 2023-06-02 14:49:32.590134 clarifai-9.5.1/setup.cfg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      897 2023-06-02 14:46:52.000000 clarifai-9.5.1/setup.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 14:49:32.589670 clarifai-9.5.1/tests/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2265 2023-06-01 21:00:24.000000 clarifai-9.5.1/tests/test_auth.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3865 2023-06-01 21:00:24.000000 clarifai-9.5.1/tests/test_modules.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3716 2023-06-01 21:00:24.000000 clarifai-9.5.1/tests/test_stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.650743 clarifai-9.5.2/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      555 2023-06-01 21:00:24.000000 clarifai-9.5.2/LICENSE
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-06-01 21:00:24.000000 clarifai-9.5.2/MANIFEST.in
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-06-02 20:19:37.650604 clarifai-9.5.2/PKG-INFO
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2347 2023-06-01 21:00:24.000000 clarifai-9.5.2/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.637220 clarifai-9.5.2/clarifai/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.638024 clarifai-9.5.2/clarifai/auth/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/auth/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    12239 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/auth/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.638769 clarifai-9.5.2/clarifai/client/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/client/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/client/abc.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/client/stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.639203 clarifai-9.5.2/clarifai/data_upload/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.640025 clarifai-9.5.2/clarifai/data_upload/datasets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    10349 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.640946 clarifai-9.5.2/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1414 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.634865 clarifai-9.5.2/clarifai/data_upload/examples/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.641109 clarifai-9.5.2/clarifai/data_upload/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.641363 clarifai-9.5.2/clarifai/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.641641 clarifai-9.5.2/clarifai/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.641786 clarifai-9.5.2/clarifai/data_upload/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.642002 clarifai-9.5.2/clarifai/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/examples.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    13040 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/data_upload/upload.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.642262 clarifai-9.5.2/clarifai/dataset_export/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     5130 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.643662 clarifai-9.5.2/clarifai/listing/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/listing/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/listing/concepts.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/listing/datasets.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/listing/inputs.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/listing/lister.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/listing/models.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/listing/module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/listing/modules.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.644091 clarifai-9.5.2/clarifai/modules/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/modules/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/modules/css.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/modules/pages.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.644242 clarifai-9.5.2/clarifai/urls/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3172 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai/urls/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.637816 clarifai-9.5.2/clarifai.egg-info/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-06-02 20:19:37.000000 clarifai-9.5.2/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4038 2023-06-02 20:19:37.000000 clarifai-9.5.2/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        1 2023-06-02 20:19:37.000000 clarifai-9.5.2/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-06-02 20:19:37.000000 clarifai-9.5.2/clarifai.egg-info/requires.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       24 2023-06-02 20:19:37.000000 clarifai-9.5.2/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.644403 clarifai-9.5.2/clarifai_utils/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.644650 clarifai-9.5.2/clarifai_utils/auth/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    12239 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.645061 clarifai-9.5.2/clarifai_utils/client/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/client/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/client/abc.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/client/stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.645438 clarifai-9.5.2/clarifai_utils/data_upload/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.646076 clarifai-9.5.2/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    10349 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.646947 clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1414 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.635920 clarifai-9.5.2/clarifai_utils/data_upload/examples/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.647105 clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.647387 clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.647658 clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.647826 clarifai-9.5.2/clarifai_utils/data_upload/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.648034 clarifai-9.5.2/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    13040 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.648221 clarifai-9.5.2/clarifai_utils/dataset_export/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     5130 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.649253 clarifai-9.5.2/clarifai_utils/listing/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/listing/lister.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/listing/models.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.649721 clarifai-9.5.2/clarifai_utils/modules/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/modules/css.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/modules/pages.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6003 2023-06-02 20:18:09.000000 clarifai-9.5.2/clarifai_utils/modules/style.css
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.649953 clarifai-9.5.2/clarifai_utils/urls/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3172 2023-06-01 21:00:24.000000 clarifai-9.5.2/clarifai_utils/urls/helper.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       38 2023-06-02 20:19:37.650781 clarifai-9.5.2/setup.cfg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      897 2023-06-02 20:18:09.000000 clarifai-9.5.2/setup.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-02 20:19:37.650373 clarifai-9.5.2/tests/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2265 2023-06-01 21:00:24.000000 clarifai-9.5.2/tests/test_auth.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3865 2023-06-01 21:00:24.000000 clarifai-9.5.2/tests/test_modules.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3716 2023-06-01 21:00:24.000000 clarifai-9.5.2/tests/test_stub.py
```

### Comparing `clarifai-9.5.1/LICENSE` & `clarifai-9.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/PKG-INFO` & `clarifai-9.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.5.1
+Version: 9.5.2
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.5.1/README.md` & `clarifai-9.5.2/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/auth/helper.py` & `clarifai-9.5.2/clarifai/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/client/abc.py` & `clarifai-9.5.2/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/client/stub.py` & `clarifai-9.5.2/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/datasets/base.py` & `clarifai-9.5.2/clarifai/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/datasets/features.py` & `clarifai-9.5.2/clarifai/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/datasets/image.py` & `clarifai-9.5.2/clarifai/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/datasets/text.py` & `clarifai-9.5.2/clarifai/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.5.2/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.5.2/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.5.2/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.5.2/clarifai/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.5.2/clarifai/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.5.2/clarifai/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.5.2/clarifai/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.5.2/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/examples.py` & `clarifai-9.5.2/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/data_upload/upload.py` & `clarifai-9.5.2/clarifai/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/dataset_export/dataset_export_inputs.py` & `clarifai-9.5.2/clarifai/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/listing/concepts.py` & `clarifai-9.5.2/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/listing/datasets.py` & `clarifai-9.5.2/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/listing/inputs.py` & `clarifai-9.5.2/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/listing/installed_module_versions.py` & `clarifai-9.5.2/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/listing/lister.py` & `clarifai-9.5.2/clarifai/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/listing/models.py` & `clarifai-9.5.2/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/listing/module_versions.py` & `clarifai-9.5.2/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/listing/modules.py` & `clarifai-9.5.2/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/modules/css.py` & `clarifai-9.5.2/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/modules/pages.py` & `clarifai-9.5.2/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai/urls/helper.py` & `clarifai-9.5.2/clarifai/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai.egg-info/PKG-INFO` & `clarifai-9.5.2/clarifai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.5.1
+Version: 9.5.2
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.5.1/clarifai.egg-info/SOURCES.txt` & `clarifai-9.5.2/clarifai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/auth/helper.py` & `clarifai-9.5.2/clarifai_utils/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/client/abc.py` & `clarifai-9.5.2/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/client/stub.py` & `clarifai-9.5.2/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/datasets/base.py` & `clarifai-9.5.2/clarifai_utils/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/datasets/features.py` & `clarifai-9.5.2/clarifai_utils/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.5.2/clarifai_utils/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.5.2/clarifai_utils/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.5.2/clarifai_utils/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.5.2/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.5.2/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/examples.py` & `clarifai-9.5.2/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/data_upload/upload.py` & `clarifai-9.5.2/clarifai_utils/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/dataset_export/dataset_export_inputs.py` & `clarifai-9.5.2/clarifai_utils/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/listing/concepts.py` & `clarifai-9.5.2/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/listing/datasets.py` & `clarifai-9.5.2/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/listing/inputs.py` & `clarifai-9.5.2/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.5.2/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/listing/lister.py` & `clarifai-9.5.2/clarifai_utils/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/listing/models.py` & `clarifai-9.5.2/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/listing/module_versions.py` & `clarifai-9.5.2/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/listing/modules.py` & `clarifai-9.5.2/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/modules/css.py` & `clarifai-9.5.2/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/modules/pages.py` & `clarifai-9.5.2/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/clarifai_utils/urls/helper.py` & `clarifai-9.5.2/clarifai_utils/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/setup.py` & `clarifai-9.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_namespace_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.5.1",
+    version="9.5.2",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
```

### Comparing `clarifai-9.5.1/tests/test_auth.py` & `clarifai-9.5.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/tests/test_modules.py` & `clarifai-9.5.2/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.1/tests/test_stub.py` & `clarifai-9.5.2/tests/test_stub.py`

 * *Files identical despite different names*

