# Comparing `tmp/waffle_hub-0.2.1.tar.gz` & `tmp/waffle_hub-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.2.1.tar", last modified: Thu May 25 07:08:05 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.2.tar", last modified: Fri Jun  2 11:05:31 2023, max compression
```

## Comparing `waffle_hub-0.2.1.tar` & `waffle_hub-0.2.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.2.1/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.2.1/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      881 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      398 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2670 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6092 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/tests/test_cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8248 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/tests/test_dataset.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10344 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3810 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/dataset/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/dataset/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      168 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/dataset/adapter/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3037 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/dataset/adapter/coco.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4836 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/dataset/adapter/huggingface.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7268 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/dataset/adapter/yolo.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    40910 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/experimental/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/experimental/auto_label/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/experimental/auto_label/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2406 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10318 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8490 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/train_input_helper.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2439 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/config.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3203 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8515 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4252 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    12302 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    37106 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/base_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    12854 2023-05-25 07:04:29.000000 waffle_hub-0.2.1/waffle_hub/hub/model/wrapper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10134 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/schema/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      304 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/schema/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-04-25 04:16:04.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    15506 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/schema/fields/image.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/schema/result.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.1/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-05-25 07:06:29.000000 waffle_hub-0.2.1/waffle_hub/utils/conversion.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-04-25 08:43:33.000000 waffle_hub-0.2.1/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3218 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/utils/draw.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3706 2023-05-03 03:24:46.000000 waffle_hub-0.2.1/waffle_hub/utils/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-25 07:08:05.343711 waffle_hub-0.2.1/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2070 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       68 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      319 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-05-25 07:08:05.000000 waffle_hub-0.2.1/waffle_hub.egg-info/top_level.txt
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/
+-rw-r--r--   0 zero      (1000) zero      (1000)    35149 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/LICENSE
+-rw-r--r--   0 zero      (1000) zero      (1000)      138 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/MANIFEST.in
+-rw-r--r--   0 zero      (1000) zero      (1000)     1962 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/PKG-INFO
+-rw-r--r--   0 zero      (1000) zero      (1000)      881 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/README.md
+-rw-r--r--   0 zero      (1000) zero      (1000)      385 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/requirements.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)       38 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/setup.cfg
+-rw-r--r--   0 zero      (1000) zero      (1000)     2670 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/setup.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.875476 waffle_hub-0.2.2/tests/
+-rw-r--r--   0 zero      (1000) zero      (1000)     8047 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/tests/test_cli.py
+-rw-r--r--   0 zero      (1000) zero      (1000)    12185 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/tests/test_dataset.py
+-rw-r--r--   0 zero      (1000) zero      (1000)    10733 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/tests/test_hub.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.875476 waffle_hub-0.2.2/waffle_hub/
+-rw-r--r--   0 zero      (1000) zero      (1000)     3723 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/__init__.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.875476 waffle_hub-0.2.2/waffle_hub/dataset/
+-rw-r--r--   0 zero      (1000) zero      (1000)       53 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/__init__.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/dataset/adapter/
+-rw-r--r--   0 zero      (1000) zero      (1000)      168 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/adapter/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     2992 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/adapter/coco.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     4780 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/adapter/huggingface.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     7223 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/adapter/yolo.py
+-rw-r--r--   0 zero      (1000) zero      (1000)    51612 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/dataset.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/experimental/
+-rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/experimental/__init__.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/experimental/auto_label/
+-rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/experimental/auto_label/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     7920 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     2986 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/experimental/serve.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/
+-rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/__init__.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/
+-rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/__init__.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/
+-rw-r--r--   0 zero      (1000) zero      (1000)       75 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     9319 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     2409 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/config.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/
+-rw-r--r--   0 zero      (1000) zero      (1000)      129 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     1913 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     3660 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/
+-rw-r--r--   0 zero      (1000) zero      (1000)       75 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     2406 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/config.py
+-rw-r--r--   0 zero      (1000) zero      (1000)    10318 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     8490 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/train_input_helper.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/
+-rw-r--r--   0 zero      (1000) zero      (1000)       74 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     4252 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/config.py
+-rw-r--r--   0 zero      (1000) zero      (1000)    12302 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-r--r--   0 zero      (1000) zero      (1000)    37067 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/base_hub.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/model/
+-rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/model/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)    12854 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/model/wrapper.py
+-rw-r--r--   0 zero      (1000) zero      (1000)    12811 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/run.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/schema/
+-rw-r--r--   0 zero      (1000) zero      (1000)      345 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     1169 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/base_schema.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     1699 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/configs.py
+-rw-r--r--   0 zero      (1000) zero      (1000)      785 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/data.py
+-rw-r--r--   0 zero      (1000) zero      (1000)      304 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/evaluate.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/schema/fields/
+-rw-r--r--   0 zero      (1000) zero      (1000)      138 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)    17217 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/annotation.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     1455 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/base_field.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     7241 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/category.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     2599 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/image.py
+-rw-r--r--   0 zero      (1000) zero      (1000)      496 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/result.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/utils/
+-rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     3694 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/callback.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     1686 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/conversion.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     5650 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/data.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     3218 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/draw.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     3706 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/evaluate.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.875476 waffle_hub-0.2.2/waffle_hub.egg-info/
+-rw-r--r--   0 zero      (1000) zero      (1000)     1962 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/PKG-INFO
+-rw-r--r--   0 zero      (1000) zero      (1000)     2098 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)        1 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)       68 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/entry_points.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)      302 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/requires.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)       11 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.2.1/LICENSE` & `waffle_hub-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/PKG-INFO` & `waffle_hub-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.2.1
+Version: 0.2.2
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.1 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.2 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.1/README.md` & `waffle_hub-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/setup.py` & `waffle_hub-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/tests/test_cli.py` & `waffle_hub-0.2.2/tests/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -115,14 +115,83 @@
         --root-dir {test_dir / 'datasets'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "clone").exists()
 
 
+def test_dataset_delete(test_dir: Path):
+    cmd = f"python -m waffle_hub.run dataset delete \
+        --name clone \
+        --root-dir {test_dir / 'datasets'} \
+    "
+    ret = run_cli(cmd)
+    assert ret.returncode == 0
+    assert not (test_dir / "datasets" / "clone").exists()
+
+
+def test_dataset_get_split_ids(test_dir: Path):
+    cmd = f"python -m waffle_hub.run dataset get_split_ids \
+        --name from_coco \
+        --root-dir {test_dir / 'datasets'} \
+    "
+    ret = run_cli(cmd)
+    assert ret.returncode == 0
+
+
+def test_dataset_merge(test_dir: Path):
+    cmd = f"python -m waffle_hub.run dataset merge \
+        --name merge \
+        --root-dir {test_dir / 'datasets'} \
+        --src-names from_coco --src-names from_hf \
+        --src-root-dirs {test_dir / 'datasets'} --src-root-dirs {test_dir / 'datasets'} \
+        --task classification \
+    "
+    ret = run_cli(cmd)
+    assert ret.returncode == 0
+    assert (test_dir / "datasets" / "merge").exists()
+
+
+def test_dataset_sample(test_dir: Path):
+    cmd = f"python -m waffle_hub.run dataset sample \
+        --name sample \
+        --root-dir {test_dir / 'datasets'} \
+        --task object_detection \
+    "
+    ret = run_cli(cmd)
+    assert ret.returncode == 0
+    assert (test_dir / "datasets" / "sample").exists()
+
+
+def test_dataset_get_fields(test_dir: Path):
+    # image
+    cmd = f"python -m waffle_hub.run dataset get_images \
+        --name sample \
+        --root-dir {test_dir / 'datasets'} \
+    "
+    ret = run_cli(cmd)
+    assert ret.returncode == 0
+
+    # annotation
+    cmd = f"python -m waffle_hub.run dataset get_annotations \
+        --name sample \
+        --root-dir {test_dir / 'datasets'} \
+    "
+    ret = run_cli(cmd)
+    assert ret.returncode == 0
+
+    # category
+    cmd = f"python -m waffle_hub.run dataset get_categories \
+        --name sample \
+        --root-dir {test_dir / 'datasets'} \
+    "
+    ret = run_cli(cmd)
+    assert ret.returncode == 0
+
+
 def test_hub_new(test_dir: Path):
     cmd = f'python -m waffle_hub.run hub new \
         --backend ultralytics \
         --root-dir {test_dir / "hubs"} \
         --name test \
         --task classification \
         --model-type yolov8 \
```

### Comparing `waffle_hub-0.2.1/tests/test_dataset.py` & `waffle_hub-0.2.2/tests/test_dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from collections import Counter
 from pathlib import Path
 
 import pytest
+from waffle_utils.file.io import load_json, save_json
 
 from waffle_hub import TaskType
 from waffle_hub.dataset import Dataset
 from waffle_hub.schema.fields import Annotation, Category, Image
 from waffle_hub.utils.data import ImageDataset, LabeledDataset
 
 
@@ -20,14 +22,22 @@
         image_id=1,
         category_id=1,
         bbox=bbox,
         area=10000,
     )
     assert not a.is_prediction()
 
+    a = Annotation.object_detection(
+        annotation_id=1,
+        image_id=1,
+        category_id=1,
+        bbox=bbox,
+    )
+    assert a.area == 10000
+
     a.score = 0.4
     assert a.is_prediction()
 
     d = a.to_dict()
     a = Annotation.from_dict(d)
 
     # classification
@@ -42,14 +52,24 @@
         annotation_id=1,
         image_id=1,
         category_id=1,
         segmentation=segmentation,
         area=10000,
     )
     assert a.bbox == [110, 110, 20, 20]
+    assert a.area == 10000
+
+    a = Annotation.instance_segmentation(
+        annotation_id=1,
+        image_id=1,
+        category_id=1,
+        segmentation=segmentation,
+    )
+    assert a.bbox == [110, 110, 20, 20]
+    assert a.area == 200
 
     # keypoint detection
     a = Annotation.keypoint_detection(
         annotation_id=1,
         image_id=1,
         category_id=1,
         keypoints=keypoints,
@@ -141,38 +161,72 @@
 
     dataset.split(0.4, 0.4, 0.2)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) + len(val_ids) + len(test_ids) == len(dataset.images)
 
     dataset.split(0.99999999999999, 0.0)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
-    assert len(train_ids) == 99 and len(val_ids) == 1 and len(test_ids) == 1
+    assert len(dataset.categories) == len(val_ids) == len(test_ids)
 
     dataset.split(0.00000000000001, 0.0)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
-    assert len(train_ids) == 1 and len(val_ids) == 99 and len(test_ids) == 99
+    assert len(dataset.categories) == len(train_ids)
 
     with pytest.raises(ValueError):
         dataset.split(0.0, 0.2)
 
     with pytest.raises(ValueError):
         dataset.split(0.9, 0.2)
 
 
 def _export(dataset_name, task: TaskType, root_dir):
     dataset = Dataset.load(dataset_name, root_dir=root_dir)
+    dataset.split(0.05)
 
     if task in [TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION, TaskType.CLASSIFICATION]:
         dataset.export("coco")
     if task in [TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION, TaskType.CLASSIFICATION]:
         dataset.export("yolo")
     if task in [TaskType.OBJECT_DETECTION, TaskType.CLASSIFICATION]:
         dataset.export("huggingface")
 
 
+# test dummy
+def _dummy(dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir):
+    dataset = Dataset.dummy(
+        name=dataset_name,
+        task=task,
+        image_num=image_num,
+        category_num=category_num,
+        unlabeld_image_num=unlabeled_image_num,
+        root_dir=root_dir,
+    )
+    assert len(dataset.images) == image_num
+    assert len(dataset.categories) == category_num
+    assert len(dataset.unlabeled_images) == unlabeled_image_num
+
+
+def _total_dummy(
+    dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir
+):
+    _dummy(dataset_name, task, image_num, category_num, unlabeled_image_num, root_dir)
+    _load(dataset_name, root_dir)
+    _clone(dataset_name, root_dir)
+    _split(dataset_name, root_dir)
+    _export(dataset_name, task, root_dir)
+
+
+def test_dummy(tmpdir):
+    for task in [TaskType.CLASSIFICATION, TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION]:
+        _total_dummy(f"dummy_{task}", task, 100, 5, 10, tmpdir)
+
+    with pytest.raises(ValueError):
+        _total_dummy("dummy", TaskType.CLASSIFICATION, 3, 3, 0, tmpdir)
+
+
 # test coco
 def _from_coco(dataset_name, task: TaskType, coco_path, root_dir):
     dataset = Dataset.from_coco(
         name=dataset_name,
         task=task,
         coco_file=coco_path / "coco.json",
         coco_root_dir=coco_path / "images",
@@ -277,11 +331,89 @@
     labeled_dataset = LabeledDataset(ds, 224)
     assert len(labeled_dataset) == 100
     labeled_dataloader = labeled_dataset.get_dataloader(batch_size=32, num_workers=0)
     assert len(labeled_dataloader) == 4
 
     ds.split(0.8)
     labeled_dataset = LabeledDataset(ds, 224, set_name="train")
-    assert len(labeled_dataset) == 80
-
     image, image_info, annotations = labeled_dataset[0]
     assert hasattr(annotations[0], "bbox")
+
+
+# etc
+def test_sample(tmpdir):
+    for task_type in TaskType:
+        try:
+            Dataset.sample(
+                name=f"sample_{task_type}",
+                root_dir=tmpdir,
+                task=task_type,
+            )
+        except NotImplementedError:
+            continue
+
+        assert (tmpdir / f"sample_{task_type}").exists()
+
+
+def test_merge(coco_path, tmpdir):
+    ds1 = Dataset.from_coco(
+        name="ds1",
+        task=TaskType.OBJECT_DETECTION,
+        coco_file=coco_path / "coco.json",
+        coco_root_dir=coco_path / "images",
+        root_dir=tmpdir,
+    )
+    ds2 = Dataset.from_coco(
+        name="ds2",
+        task=TaskType.OBJECT_DETECTION,
+        coco_file=coco_path / "coco.json",
+        coco_root_dir=coco_path / "images",
+        root_dir=tmpdir,
+    )
+
+    cateids_of_ann = [annotation.category_id for annotation in ds1.annotations.values()]
+    category_counts = Counter(cateids_of_ann)
+
+    category_1_num = category_counts[1]
+    category_2_num = category_counts[2]
+
+    ds = Dataset.merge(
+        name="merge",
+        src_names=["ds1", "ds2"],
+        src_root_dirs=[tmpdir, tmpdir],
+        root_dir=tmpdir,
+        task=TaskType.OBJECT_DETECTION,
+    )
+
+    cateids_of_ann = [annotation.category_id for annotation in ds.annotations.values()]
+    category_counts = Counter(cateids_of_ann)
+
+    assert (ds.raw_image_dir).exists()
+    assert len(ds.images) == 100
+    assert len(ds.annotations) == 100
+    assert len(ds.categories) == 2
+    assert category_counts[1] == category_1_num
+    assert category_counts[2] == category_2_num
+
+    # test merge with different category name
+    category = load_json(ds1.category_dir / "1.json")
+    category["name"] = "one"
+    save_json(category, ds1.category_dir / "1.json")
+
+    ds = Dataset.merge(
+        name="merge2",
+        src_names=["ds1", "ds2"],
+        src_root_dirs=[tmpdir, tmpdir],
+        root_dir=tmpdir,
+        task=TaskType.OBJECT_DETECTION,
+    )
+
+    cateids_of_ann = [annotation.category_id for annotation in ds.annotations.values()]
+    category_counts = Counter(cateids_of_ann)
+
+    assert len(ds.images) == 100
+    assert len(ds.annotations) == 100 + category_1_num
+    assert len(ds.categories) == 3
+
+    assert category_counts[1] == category_1_num
+    assert category_counts[2] == category_2_num
+    assert category_counts[3] == category_1_num
```

### Comparing `waffle_hub-0.2.1/tests/test_hub.py` & `waffle_hub-0.2.2/tests/test_hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,63 +2,63 @@
 from pathlib import Path
 
 import pytest
 import torch
 
 from waffle_hub import TaskType
 from waffle_hub.dataset import Dataset
+from waffle_hub.hub.adapter.autocare_dlt import AutocareDLTHub
 from waffle_hub.hub.adapter.hugging_face import HuggingFaceHub
 from waffle_hub.hub.adapter.ultralytics import UltralyticsHub
 from waffle_hub.schema.result import (
     EvaluateResult,
     ExportResult,
     InferenceResult,
     TrainResult,
 )
 
 
-# from waffle_hub.hub.adapter.tx_model import TxModelHub
 @pytest.fixture
 def instance_segmentation_dataset(coco_path: Path, tmpdir: Path):
     dataset: Dataset = Dataset.from_coco(
         name="seg",
         task=TaskType.INSTANCE_SEGMENTATION,
         coco_file=coco_path / "coco.json",
         coco_root_dir=coco_path / "images",
         root_dir=tmpdir,
     )
-    dataset.split(0.8)
+    dataset.split(0.2, 0.2, 0.6)
 
     return dataset
 
 
 @pytest.fixture
 def object_detection_dataset(coco_path: Path, tmpdir: Path):
     dataset: Dataset = Dataset.from_coco(
         name="od",
         task=TaskType.OBJECT_DETECTION,
         coco_file=coco_path / "coco.json",
         coco_root_dir=coco_path / "images",
         root_dir=tmpdir,
     )
-    dataset.split(0.1, 0.1, 0.8)
+    dataset.split(0.2, 0.2, 0.6)
 
     return dataset
 
 
 @pytest.fixture
 def classification_dataset(coco_path: Path, tmpdir: Path):
     dataset: Dataset = Dataset.from_coco(
         name="cls",
         task=TaskType.CLASSIFICATION,
         coco_file=coco_path / "coco.json",
         coco_root_dir=coco_path / "images",
         root_dir=tmpdir,
     )
-    dataset.split(0.8)
+    dataset.split(0.2, 0.2, 0.6)
 
     return dataset
 
 
 def _train(hub, dataset: Dataset, image_size: int, hold: bool = True):
     result: TrainResult = hub.train(
         dataset_path=dataset.export(hub.backend),
@@ -321,57 +321,65 @@
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size, hold=False)
 
 
-# def test_tx_model_object_detection(
-#     object_detection_dataset: Dataset, tmpdir: Path
-# ):
-#     image_size = 32
-#     dataset = object_detection_dataset
-
-#     # test hub
-#     name = "test_det"
-#     hub = TxModelHub.new(
-#         name=name,
-#         task=TaskType.OBJECT_DETECTION,
-#         model_type="YOLOv5",
-#         model_size="s",
-#         categories=object_detection_dataset.category_names,
-#         root_dir=tmpdir,
-#     )
-#     hub = TxModelHub.load(name=name, root_dir=tmpdir)
-#     hub: TxModelHub = TxModelHub.from_model_config(
-#         name=name,
-#         model_config_file=tmpdir / name / TxModelHub.MODEL_CONFIG_FILE,
-#         root_dir=tmpdir,
-#     )
-
-#     _total(hub, dataset, image_size)
-
-
-# def test_tx_model_classification(
-#     classification_dataset: Dataset, tmpdir: Path
-# ):
-#     image_size = 32
-#     dataset = classification_dataset
-
-#     # test hub
-#     name = "test_cls"
-#     hub = TxModelHub.new(
-#         name=name,
-#         task=TaskType.CLASSIFICATION,
-#         model_type="Classifier",
-#         model_size="s",
-#         categories=classification_dataset.category_names,
-#         root_dir=tmpdir,
-#     )
-#     hub = TxModelHub.load(name=name, root_dir=tmpdir)
-#     hub: TxModelHub = TxModelHub.from_model_config(
-#         name=name,
-#         model_config_file=tmpdir / name / TxModelHub.MODEL_CONFIG_FILE,
-#         root_dir=tmpdir,
-#     )
+def test_autocare_dlt_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
+    image_size = 32
+    dataset = object_detection_dataset
+
+    # test hub
+    name = "test_det"
+    hub = AutocareDLTHub.new(
+        name=name,
+        task=TaskType.OBJECT_DETECTION,
+        model_type="YOLOv5",
+        model_size="s",
+        categories=object_detection_dataset.category_names,
+        root_dir=tmpdir,
+    )
+    hub = AutocareDLTHub.load(name=name, root_dir=tmpdir)
+    hub: AutocareDLTHub = AutocareDLTHub.from_model_config(
+        name=name,
+        model_config_file=tmpdir / name / AutocareDLTHub.MODEL_CONFIG_FILE,
+        root_dir=tmpdir,
+    )
+
+    _total(hub, dataset, image_size)
+
 
-#     _total(hub, dataset, image_size)
+def test_autocare_dlt_classification(classification_dataset: Dataset, tmpdir: Path):
+    image_size = 32
+    dataset = classification_dataset
+
+    # temporal solution
+    super_cat = [[c.supercategory, c.name] for c in dataset.categories.values()]
+    super_cat_dict = {}
+    for super_cat, cat in super_cat:
+        if super_cat not in super_cat_dict:
+            super_cat_dict[super_cat] = []
+        super_cat_dict[super_cat].append(cat)
+    super_cat_dict_list = []
+
+    for super_cat, cat in super_cat_dict.items():
+        super_cat_dict_list.append({super_cat: cat})
+
+    # test hub
+    name = "test_cls"
+    hub = AutocareDLTHub.new(
+        name=name,
+        task=TaskType.CLASSIFICATION,
+        model_type="Classifier",
+        model_size="s",
+        categories=super_cat_dict_list,
+        root_dir=tmpdir,
+    )
+    hub = AutocareDLTHub.load(name=name, root_dir=tmpdir)
+    hub: AutocareDLTHub = AutocareDLTHub.from_model_config(
+        name=name,
+        model_config_file=tmpdir / name / AutocareDLTHub.MODEL_CONFIG_FILE,
+        root_dir=tmpdir,
+    )
+
+    _total(hub, dataset, image_size)
```

### Comparing `waffle_hub-0.2.1/waffle_hub/__init__.py` & `waffle_hub-0.2.2/waffle_hub/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 import enum
 import importlib
 import warnings
 from collections import OrderedDict
 
 from tabulate import tabulate
 
 # pytorch install check (necessary installation)
-pytorch_versions = ["1.13.1"]
+pytorch_version = "1.13.1"
 try:
     import torch
 
-    if torch.__version__ not in pytorch_versions:
+    if pytorch_version not in torch.__version__:
         warnings.warn(
             f"""
             torch {torch.__version__} has not been tested.
-            We recommend you to use one of {pytorch_versions}
+            We recommend you to use {pytorch_version}
             """
         )
 except ModuleNotFoundError as e:
-    # TODO: Generalize install strings
     strings = []
 
     e.msg = "Need to install torch\n" + "\n".join(strings)
     raise e
 
 # backend supports
 _backends = OrderedDict(
     {
-        "ultralytics": ["8.0.87"],
-        "autocare_tx_model": ["0.2.0"],
-        "transformers": ["4.27.4"],
+        "ultralytics": ["8.0.112"],
+        "autocare_dlt": ["0.2.3"],
+        "transformers": ["4.28.1"],
     }
 )
 
 
 def get_backends() -> dict:
     return _backends
 
@@ -137,16 +136,15 @@
 class DataType(BaseEnum):
     # TODO: map to same value
 
     YOLO = enum.auto()
     ULTRALYTICS = enum.auto()
 
     COCO = enum.auto()
-    TX_MODEL = enum.auto()
-    AUTOCARE_TX_MODEL = enum.auto()
+    AUTOCARE_DLT = enum.auto()
 
     HUGGINGFACE = enum.auto()
     TRANSFORMERS = enum.auto()
 
 
 class TaskType(BaseEnum):
     CLASSIFICATION = enum.auto()
```

### Comparing `waffle_hub-0.2.1/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.2.2/waffle_hub/dataset/adapter/coco.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,19 +77,19 @@
         export_dir (str): Path to export directory
 
     Returns:
         str: Path to export directory
     """
     export_dir = Path(export_dir)
 
-    train_ids, val_ids, test_ids, unlabeled_ids = self.get_split_ids()
+    train_ids, val_ids, test_ids, _ = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
-        _export_coco(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
+        _export_coco(self, export_dir, train_ids, val_ids, test_ids, [])
     elif self.task == TaskType.OBJECT_DETECTION:
-        _export_coco(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
+        _export_coco(self, export_dir, train_ids, val_ids, test_ids, [])
     elif self.task == TaskType.INSTANCE_SEGMENTATION:
-        _export_coco(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
+        _export_coco(self, export_dir, train_ids, val_ids, test_ids, [])
     else:
         raise ValueError(f"Unsupported task type: {self.task}")
 
     return str(export_dir)
```

### Comparing `waffle_hub-0.2.1/waffle_hub/dataset/adapter/huggingface.py` & `waffle_hub-0.2.2/waffle_hub/dataset/adapter/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,19 +148,17 @@
         export_dir (str): Path to export directory
 
     Returns:
         str: Path to export directory
     """
     export_dir = Path(export_dir)
 
-    train_ids, val_ids, test_ids, unlabeled_ids = self.get_split_ids()
+    train_ids, val_ids, test_ids, _ = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
-        _export_huggingface_classification(
-            self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids
-        )
+        _export_huggingface_classification(self, export_dir, train_ids, val_ids, test_ids, [])
     elif self.task == TaskType.OBJECT_DETECTION:
-        _export_huggingface_detection(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
+        _export_huggingface_detection(self, export_dir, train_ids, val_ids, test_ids, [])
     else:
         raise ValueError(f"Unsupported task type: {self.task}")
 
     return str(export_dir)
```

### Comparing `waffle_hub-0.2.1/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.2/waffle_hub/dataset/adapter/yolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,22 +196,22 @@
     Returns:
         str: Path to export directory
     """
     _check_valid_file_paths(self.images)
 
     export_dir = Path(export_dir)
 
-    train_ids, val_ids, test_ids, unlabeled_ids = self.get_split_ids()
+    train_ids, val_ids, test_ids, _ = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
-        _export_yolo_classification(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
+        _export_yolo_classification(self, export_dir, train_ids, val_ids, test_ids, [])
     elif self.task == TaskType.OBJECT_DETECTION:
-        _export_yolo_detection(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
+        _export_yolo_detection(self, export_dir, train_ids, val_ids, test_ids, [])
     elif self.task == TaskType.INSTANCE_SEGMENTATION:
-        _export_yolo_segmentation(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
+        _export_yolo_segmentation(self, export_dir, train_ids, val_ids, test_ids, [])
     else:
         raise ValueError(f"Unsupported task type: {self.task}")
 
     io.save_yaml(
         {
             "path": str(export_dir.absolute()),
             "train": "train",
```

### Comparing `waffle_hub-0.2.1/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.2/waffle_hub/dataset/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import copy
 import logging
 import random
+import shutil
 import warnings
-from collections import OrderedDict, defaultdict
+from collections import Counter, OrderedDict, defaultdict
 from functools import cached_property
-from itertools import combinations
-from math import ceil, floor
 from pathlib import Path
+from tempfile import mkdtemp
 from typing import Union
 
 import cv2
 import PIL.Image
 import tqdm
 from pycocotools.coco import COCO
-from waffle_utils.file import io
+from waffle_utils.file import io, network
 from waffle_utils.file.search import get_files, get_image_files
 from waffle_utils.log import datetime_now
 from waffle_utils.utils import type_validator
 
 from datasets import Dataset as HFDataset
 from datasets import DatasetDict, load_from_disk
 from waffle_hub import DataType, SplitMethod, TaskType
@@ -43,14 +44,16 @@
     SET_DIR = Path("sets")
 
     TRAIN_SET_FILE_NAME = Path("train.json")
     VAL_SET_FILE_NAME = Path("val.json")
     TEST_SET_FILE_NAME = Path("test.json")
     UNLABELED_SET_FILE_NAME = Path("unlabeled.json")
 
+    MINIMUM_TRAINABLE_IMAGE_NUM_PER_CATEGORY = 3
+
     def __init__(
         self,
         name: str,
         task: Union[str, TaskType],
         created: str = None,
         root_dir: str = None,
     ):
@@ -195,14 +198,54 @@
             for annotation in tqdm.tqdm(
                 self.annotations.values(), desc="Building image to annotation index"
             ):
                 image_to_annotations[annotation.image_id].append(annotation)
             self._image_to_annotations = dict(image_to_annotations)
         return self._image_to_annotations
 
+    @cached_property
+    def category_to_annotations(self) -> dict[int, list[Annotation]]:
+        if not hasattr(self, "_category_to_annotations"):
+            category_to_annotations = defaultdict(list)
+            for annotation in tqdm.tqdm(
+                self.annotations.values(), desc="Building category to annotation index"
+            ):
+                category_to_annotations[annotation.category_id].append(annotation)
+            self._category_to_annotations = dict(category_to_annotations)
+        return self._category_to_annotations
+
+    @cached_property
+    def category_to_images(self) -> dict[int, list[Image]]:
+        if not hasattr(self, "_category_to_images"):
+            category_to_images = {category_id: [] for category_id in self.categories.keys()}
+            for image_id, annotations in tqdm.tqdm(
+                self.image_to_annotations.items(), desc="Building category to image index"
+            ):
+                category_count = Counter(map(lambda a: a.category_id, annotations))
+                category_to_images[category_count.most_common(1)[0][0]].append(self.images[image_id])
+            self._category_to_images = dict(category_to_images)
+        return self._category_to_images
+
+    @cached_property
+    def num_images_per_category(self) -> dict[int, int]:
+        if not hasattr(self, "_num_images_per_category"):
+            self._num_images_per_category = {
+                category_id: len(images) for category_id, images in self.category_to_images.items()
+            }
+        return self._num_images_per_category
+
+    @cached_property
+    def num_annotations_per_category(self) -> dict[int, int]:
+        if not hasattr(self, "_num_annotations_per_category"):
+            self._num_annotations_per_category = {
+                category_id: len(annotations)
+                for category_id, annotations in self.category_to_annotations.items()
+            }
+        return self._num_annotations_per_category
+
     # factories
     @classmethod
     def new(cls, name: str, task: str, root_dir: str = None) -> "Dataset":
         """
         Create New Dataset.
         This method creates a new dataset directory and initialize dataset info file.
         If you have other types of data, you can use from_* methods to create a dataset.
@@ -274,14 +317,134 @@
         ds = Dataset.new(name, src_ds.task, root_dir)
         io.copy_files_to_directory(src_ds.dataset_dir, ds.dataset_dir, create_directory=True)
         ds.initialize()
 
         return ds
 
     @classmethod
+    def dummy(
+        cls,
+        name: str,
+        task: str,
+        image_num: int = 100,
+        category_num: int = 10,
+        unlabeld_image_num: int = 0,
+        root_dir: str = None,
+    ) -> "Dataset":
+        """
+        Create Dummy Dataset (for debugging).
+
+        Args:
+            name (str): Dataset name
+            task (str): Dataset task
+            image_num (int, optional): Number of images. Defaults to 100.
+            category_num (int, optional): Number of categories. Defaults to 10.
+            unlabeld_image_num (int, optional): Number of unlabeled images. Defaults to 0.
+            root_dir (str, optional): Dataset root directory. Defaults to None.
+
+        Raises:
+            FileExistsError: if dataset name already exists
+
+        Examples:
+            >>> ds = Dataset.dummy("my_dataset", "CLASSIFICATION", image_num=100, category_num=10)
+            >>> len(ds.images)
+            100
+            >>> len(ds.categories)
+            10
+        """
+        ds = Dataset.new(name, task, root_dir)
+
+        try:
+            for category_id in range(1, category_num + 1):
+
+                if task == TaskType.CLASSIFICATION:
+                    category = Category.classification(
+                        category_id=category_id,
+                        name=f"category_{category_id}",
+                        supercategory="object",
+                    )
+                elif task == TaskType.OBJECT_DETECTION:
+                    category = Category.object_detection(
+                        category_id=category_id,
+                        name=f"category_{category_id}",
+                        supercategory="object",
+                    )
+                elif task == TaskType.INSTANCE_SEGMENTATION:
+                    category = Category.instance_segmentation(
+                        category_id=category_id,
+                        name=f"category_{category_id}",
+                        supercategory="object",
+                    )
+
+                ds.add_categories([category])
+
+            annotation_id = 1
+            for image_id in range(1, image_num + 1):
+                file_name = f"image_{image_id}.jpg"
+                ds.add_images([Image(image_id=image_id, file_name=file_name, width=100, height=100)])
+                PIL.Image.new("RGB", (100, 100)).save(ds.raw_image_dir / file_name)
+
+                if task == TaskType.CLASSIFICATION:
+                    annotations = [
+                        Annotation.classification(
+                            annotation_id=annotation_id,
+                            image_id=image_id,
+                            category_id=random.randint(1, category_num),
+                        )
+                    ]
+                elif task == TaskType.OBJECT_DETECTION:
+                    annotations = [
+                        Annotation.object_detection(
+                            annotation_id=annotation_id + i,
+                            image_id=image_id,
+                            category_id=random.randint(1, category_num),
+                            bbox=[
+                                random.randint(0, 100),
+                                random.randint(0, 100),
+                                random.randint(0, 100),
+                                random.randint(0, 100),
+                            ],
+                        )
+                        for i in range(random.randint(1, 5))
+                    ]
+                elif task == TaskType.INSTANCE_SEGMENTATION:
+                    annotations = [
+                        Annotation.instance_segmentation(
+                            annotation_id=annotation_id + i,
+                            image_id=image_id,
+                            category_id=random.randint(1, category_num),
+                            bbox=[
+                                random.randint(0, 100),
+                                random.randint(0, 100),
+                                random.randint(0, 100),
+                                random.randint(0, 100),
+                            ],
+                            segmentation=[[random.randint(0, 100) for _ in range(10)]],
+                        )
+                        for i in range(random.randint(1, 5))
+                    ]
+
+                ds.add_annotations(annotations)
+                annotation_id += len(annotations)
+
+            if unlabeld_image_num > 0:
+                for image_id in range(image_num + 1, image_num + unlabeld_image_num + 1):
+                    file_name = f"image_{image_id}.jpg"
+                    ds.add_images(
+                        [Image(image_id=image_id, file_name=file_name, width=100, height=100)]
+                    )
+                    PIL.Image.new("RGB", (100, 100)).save(ds.raw_image_dir / file_name)
+
+        except Exception as e:
+            ds.delete()
+            raise e
+
+        return ds
+
+    @classmethod
     def load(cls, name: str, root_dir: str = None) -> "Dataset":
         """
         Load Dataset.
         This method loads an existing dataset.
 
         Args:
             name (str): Dataset name that Waffle Created
@@ -302,14 +465,125 @@
         dataset_info_file = root_dir / name / Dataset.DATASET_INFO_FILE_NAME
         if not dataset_info_file.exists():
             raise FileNotFoundError(f"{dataset_info_file} has not been created.")
         dataset_info = DatasetInfo.load(dataset_info_file)
         return cls(**dataset_info.to_dict(), root_dir=root_dir)
 
     @classmethod
+    def merge(
+        cls,
+        name: str,
+        root_dir: str,
+        src_names: list[str],
+        src_root_dirs: Union[str, list[str]],
+        task: str,
+    ) -> "Dataset":
+        """
+        Merge Datasets.
+        This method merges multiple datasets into one dataset.
+
+        Args:
+            name (str): New Dataset name
+            root_dir (str): New Dataset root directory
+            src_names (list[str]): Source Dataset names
+            src_root_dirs (Union[str, list[str]]): Source Dataset root directories
+            task (str): Dataset task
+
+        Returns:
+            Dataset: Dataset Class
+
+        """
+        if isinstance(src_root_dirs, str):
+            src_root_dirs = [src_root_dirs] * len(src_names)
+        if len(src_names) != len(src_root_dirs):
+            raise ValueError("Length of src_names and src_root_dirs should be same.")
+        if isinstance(task, str):
+            task = task.upper()
+        if task not in [k for k in TaskType]:
+            raise ValueError(f"task should be one of {[k for k in TaskType]}")
+
+        merged_ds = Dataset.new(
+            name=name,
+            root_dir=root_dir,
+            task=task,
+        )
+
+        categoryname2id = {}
+        filename2id = {}
+        new_annotation_id = 1
+
+        try:
+            for src_name, src_root_dir in zip(src_names, src_root_dirs):
+                src_ds = Dataset.load(src_name, src_root_dir)
+
+                if src_ds.task != task:
+                    raise ValueError(f"Task of {src_ds.name} is {src_ds.task}. It should be {task}.")
+
+                # merge - raw images
+                io.copy_files_to_directory(
+                    src_ds.raw_image_dir, merged_ds.raw_image_dir, create_directory=True
+                )
+
+                # merge - categories
+                for category in src_ds.categories.values():
+                    if category.name not in categoryname2id:
+                        new_category_id = len(categoryname2id) + 1
+                        categoryname2id[category.name] = new_category_id
+
+                        new_category = copy.deepcopy(category)
+                        new_category.category_id = new_category_id
+                        merged_ds.add_categories([new_category])
+
+                for image_id, annotations in src_ds.image_to_annotations.items():
+                    image = src_ds.images[image_id]
+
+                    # merge - images
+                    is_new_image = False
+                    if image.file_name not in filename2id:
+                        is_new_image = True
+
+                        new_image_id = len(filename2id) + 1
+                        filename2id[image.file_name] = new_image_id
+
+                        new_image = copy.deepcopy(image)
+                        new_image.image_id = new_image_id
+                        merged_ds.add_images([new_image])
+
+                    new_image_id = filename2id[image.file_name]
+
+                    # merge - annotations
+                    for annotation in annotations:
+                        new_annotation = copy.deepcopy(annotation)
+                        new_annotation.category_id = categoryname2id[
+                            src_ds.categories[annotation.category_id].name
+                        ]
+
+                        # check if new annotation
+                        is_new_annotation = True
+                        if not is_new_image:
+                            for merged_ann in merged_ds.image_to_annotations[new_image_id]:
+                                if new_annotation == merged_ann:
+                                    is_new_annotation = False
+                                    break
+
+                        # merge
+                        if is_new_annotation:
+                            new_annotation.image_id = filename2id[image.file_name]
+                            new_annotation.annotation_id = new_annotation_id
+                            new_annotation_id += 1
+                            merged_ds.add_annotations([new_annotation])
+
+        except Exception as e:
+            if merged_ds.dataset_dir.exists():
+                io.remove_directory(merged_ds.dataset_dir)
+            raise e
+
+        return Dataset.load(name, root_dir)
+
+    @classmethod
     def from_coco(
         cls,
         name: str,
         task: str,
         coco_file: Union[str, list[str]],
         coco_root_dir: Union[str, list[str]],
         root_dir: str = None,
@@ -749,14 +1023,54 @@
             _import(dataset, task, image_ids)
 
         # TODO: add unlabeled set
         io.save_json([], ds.unlabeled_set_file, create_directory=True)
 
         return ds
 
+    @classmethod
+    def sample(cls, name: str, task: str, root_dir: str = None) -> "Dataset":
+        """
+        Import sample Dataset.
+
+        Args:
+            name (str): Dataset name.
+            task (str): Task name.
+            root_dir (str, optional): Dataset root directory. Defaults to None.
+
+        Returns:
+            Dataset: Dataset Class
+        """
+        if task not in [
+            TaskType.CLASSIFICATION,
+            TaskType.OBJECT_DETECTION,
+            TaskType.INSTANCE_SEGMENTATION,
+        ]:
+            raise NotImplementedError(f"not supported task: {task}")
+
+        try:
+            url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist.zip"
+            temp_dir = Path(mkdtemp())
+            network.get_file_from_url(url, temp_dir / "mnist.zip")
+            io.unzip(temp_dir / "mnist.zip", temp_dir)
+
+            ds = Dataset.from_coco(
+                name=name,
+                root_dir=root_dir,
+                task=task,
+                coco_file=str(temp_dir / "coco.json"),
+                coco_root_dir=str(temp_dir / "images"),
+            )
+        except Exception as e:
+            raise e
+        finally:
+            shutil.rmtree(temp_dir)
+
+        return ds
+
     def initialize(self):
         """Initialize Dataset.
         It creates necessary directories under {dataset_root_dir}/{dataset_name}.
         """
         io.make_directory(self.raw_image_dir)
         io.make_directory(self.image_dir)
         io.make_directory(self.annotation_dir)
@@ -774,14 +1088,49 @@
         Returns:
             bool:
                 initialized -> True
                 not initialized -> False
         """
         return self.dataset_info_file.exists()
 
+    def trainable(self) -> bool:
+        """Check if Dataset is trainable or not.
+
+        Returns:
+            bool:
+                trainable -> True
+                not trainable -> False
+        """
+        category_to_images: dict[int, list[Image]] = self.category_to_images
+        for _, images in category_to_images.items():
+            image_num = len(images)
+            if image_num < Dataset.MINIMUM_TRAINABLE_IMAGE_NUM_PER_CATEGORY:
+                return False
+        return True
+
+    def check_trainable(self):
+        """
+        Check if Dataset is trainable or not.
+
+        Raises:
+            ValueError: if dataset has not enough annotations.
+        """
+        if not self.trainable():
+            raise ValueError(
+                "Dataset is not trainable\n"
+                + f"Please check if the MINIMUM_TRAINABLE_IMAGE_NUM_PER_CATEGORY={Dataset.MINIMUM_TRAINABLE_IMAGE_NUM_PER_CATEGORY} is satisfied\n"
+                + "Your dataset is consisted of\n"
+                + "\n".join(
+                    [
+                        f"  - {category.name}: {self.num_images_per_category[category_id]} images"
+                        for category_id, category in self.categories.items()
+                    ]
+                )
+            )
+
     # get
     def get_images(self, image_ids: list[int] = None, labeled: bool = True) -> list[Image]:
         """Get "Image"s.
 
         Args:
             image_ids (list[int], optional): id list. None for all "Image"s. Defaults to None.
             labeled (bool, optional): get labeled images. False for unlabeled images. Defaults to True.
@@ -930,114 +1279,55 @@
         Examples:
             >>> dataset = Dataset.load("some_dataset")
             >>> dataset.split(train_ratio=0.8, val_ratio=0.1, test_ratio=0.1)
             >>> dataset.get_split_ids()
             [[1, 2, 3, 4, 5, 6, 7, 8], [9], [10], []]  # train, val, test, unlabeled image ids
         """
 
+        self.check_trainable()
+
         if train_ratio <= 0.0 or train_ratio >= 1.0:
             raise ValueError(
                 "train_ratio must be between 0.0 and 1.0\n" f"given train_ratio: {train_ratio}"
             )
 
         if val_ratio == 0.0 and test_ratio == 0.0:
             val_ratio = 1 - train_ratio
 
         if train_ratio + val_ratio + test_ratio != 1.0:
             raise ValueError(
                 "train_ratio + val_ratio + test_ratio must be 1.0\n"
                 f"given train_ratio: {train_ratio}, val_ratio: {val_ratio}, test_ratio: {test_ratio}"
             )
 
-        image_ids = list(self.images.keys())
-        image_num = len(image_ids)
-        if image_num <= 2:
-            raise ValueError("image_num must be greater than 2\n" f"given image_num: {image_num}")
-
         if method == SplitMethod.RANDOM:
-            train_num = max(int(image_num * train_ratio), 1)
-            val_num = max(int(image_num * val_ratio), 1)
-
             random.seed(seed)
-            random.shuffle(image_ids)
 
-            if test_ratio == 0.0:
-                train_ids = image_ids[:train_num]
-                val_ids = image_ids[train_num:]
-                test_ids = val_ids
-            else:
-                train_ids = image_ids[:train_num]
-                val_ids = image_ids[train_num : train_num + val_num]
-                test_ids = image_ids[train_num + val_num :]
-
-        elif method == SplitMethod.STRATIFIED:
-            # """
-            # Given a dataset of image annotations, find the set of categories associated with each image and stratify them by categories.
-            # For example, if the dataset has annotations with the following image and category IDs:
-
-            # datasets: [
-            #     {"annotation_id": 1, "image_id": 1, "category_id": 1},
-            #     {"annotation_id": 2, "image_id": 1, "category_id": 2},
-            #     {"annotation_id": 3, "image_id": 2, "category_id": 1},
-            #     {"annotation_id": 4, "image_id": 2, "category_id": 2},
-            #     {"annotation_id": 5, "image_id": 3, "category_id": 1},
-            #     {"annotation_id": 6, "image_id": 4, "category_id": 1},
-            #     {"annotation_id": 7, "image_id": 5, "category_id": 2},
-            #     {"annotation_id": 8, "image_id": 6, "category_id": 2},
-            # ],
-
-            # the output should be stratified by categories:
-
-            # Categories 1 and 2 are associated with images 1, 2, 3, and 4.
-            # Category 1 is associated with images 3 and 4.
-            # Category 2 is associated with images 5 and 6.
-            # If the train_ratio : val_ratio is 0.5 : 0.5, a valid output would be:
-
-            # The training set consists of images 1, 3, and 5.
-            # The test set consists of images 2, 4, and 6.
-            # """
-
-            # train_ids = []
-            # val_ids = []
-            # test_ids = []
-
-            # # find set of categories
-            # num_category = len(self.categories)
-            # category_combinations = []
-            # for comb in [combinations(self.categories, num) for num in range(1, num_category + 1)]:
-            #     category_combinations.extend(comb)
-
-            # # for round error handling
-            # train_round_method = floor
-            # val_round_method = ceil
-
-            # # split by categories
-            # for comb in category_combinations:
-            #     image_ids_by_categories = list(
-            #         filter(
-            #             lambda image_id: set(comb)
-            #             == {ann.category_id for ann in self.image_to_annotations[image_id]},
-            #             image_ids,
-            #         )
-            #     )
-
-            #     num_images = len(image_ids_by_categories)
-            #     train_num = train_round_method(num_images * train_ratio)
-            #     val_num = val_round_method(num_images * val_ratio)
-            #     train_round_method, val_round_method = val_round_method, train_round_method
-
-            #     if test_ratio == 0.0:
-            #         train_ids += image_ids_by_categories[:train_num]
-            #         val_ids += image_ids_by_categories[train_num:]
-            #         test_ids += image_ids_by_categories[train_num:]
-            #     else:
-            #         train_ids += image_ids_by_categories[:train_num]
-            #         val_ids += image_ids_by_categories[train_num : train_num + val_num]
-            #         test_ids += image_ids_by_categories[train_num + val_num :]
-            raise NotImplementedError("(TODO) This feature will be updated soon.")
+            train_ids = []
+            val_ids = []
+            test_ids = []
+
+            for category_id, images in self.category_to_images.items():
+
+                image_num = len(images)
+                image_ids = list(map(lambda x: x.image_id, images))
+                random.shuffle(image_ids)
+
+                # flatten images to one list [cat]
+                train_num = max(int(image_num * train_ratio), 1)
+                val_num = max(int(image_num * val_ratio), 1)
+
+                if test_ratio == 0.0:
+                    train_ids.extend(image_ids[:train_num])
+                    val_ids.extend(image_ids[train_num:])
+                    test_ids = val_ids
+                else:
+                    train_ids.extend(image_ids[:train_num])
+                    val_ids.extend(image_ids[train_num : train_num + val_num])
+                    test_ids.extend(image_ids[train_num + val_num :])
 
         else:
             raise ValueError(f"Unknown split method: {method}")
 
         logger.info(
             f"train num: {len(train_ids)}  val num: {len(val_ids)}  test num: {len(test_ids)}"
         )
@@ -1102,21 +1392,22 @@
             # You can train with exported dataset
             >>> hub.train("path/to/dataset_dir/exports/yolo", ...)
 
         Returns:
             str: exported dataset directory
         """
 
+        self.check_trainable()
+
         if data_type in [DataType.YOLO, DataType.ULTRALYTICS]:
             export_dir: Path = self.export_dir / str(DataType.YOLO)
             export_function = export_yolo
         elif data_type in [
             DataType.COCO,
-            DataType.TX_MODEL,
-            DataType.AUTOCARE_TX_MODEL,
+            DataType.AUTOCARE_DLT,
         ]:
             export_dir: Path = self.export_dir / str(DataType.COCO)
             export_function = export_coco
         elif data_type in [DataType.HUGGINGFACE, DataType.TRANSFORMERS]:
             export_dir: Path = self.export_dir / str(DataType.HUGGINGFACE)
             export_function = export_huggingface
         else:
```

### Comparing `waffle_hub-0.2.1/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.2/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.2/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/config.py` & `waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py` & `waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/adapter/hugging_face/train_input_helper.py` & `waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/train_input_helper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/config.py` & `waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     "object_detection": "COCODetectionDataset",
     "classification": "COCOClassificationDataset",
 }
 
 WEIGHT_PATH = {
     "object_detection": {
         "YOLOv5": {
-            "s": "temp/autocare_tx_model/detectors/small/model.pth",
-            "m": "temp/autocare_tx_model/detectors/medium/model.pth",
-            "l": "temp/autocare_tx_model/detectors/large/model.pth",
+            "s": "temp/autocare_dlt/detectors/small/model.pth",
+            "m": "temp/autocare_dlt/detectors/medium/model.pth",
+            "l": "temp/autocare_dlt/detectors/large/model.pth",
         }
     },
     "classification": {
         "Classifier": {
-            "s": "temp/autocare_tx_model/classifiers/small/model.pth",
-            "m": "temp/autocare_tx_model/classifiers/medium/model.pth",
-            "l": "temp/autocare_tx_model/classifiers/large/model.pth",
+            "s": "temp/autocare_dlt/classifiers/small/model.pth",
+            "m": "temp/autocare_dlt/classifiers/medium/model.pth",
+            "l": "temp/autocare_dlt/classifiers/large/model.pth",
         }
     },
 }
 
 DEFAULT_PARAMAS = {
     "object_detection": {
         "YOLOv5": {
```

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py` & `waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py` & `waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py`

 * *Files 22% similar despite different names*

```diff
@@ -92,10 +92,25 @@
                 "momentum": 0.9,
                 "weight_decay": 0.0001,
             },
             "lr_cfg": {"type": "cosine"},
             "use_model_ema": True,
             "max_epoch": epochs,
             "seed": seed,
-            "classes": [{"none": categories}],
+            "classes": get_multi_task_categories(categories),
             "num_classes": len(categories),
         }
+
+
+def get_multi_task_categories(categories: list[dict]):
+    multi_task_categories = []
+    cat_dict = {}
+    for category in categories:
+        sup = category["supercategory"]
+        name = category["name"]
+        if sup not in cat_dict:
+            cat_dict[sup] = [name]
+        else:
+            cat_dict[sup].append(name)
+    for k, v in cat_dict.items():
+        multi_task_categories.append({k: v})
+    return multi_task_categories
```

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/adapter/tx_model/tx_model_hub.py` & `waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """
 Tx Model Hub
 See BaseHub documentation for more details about usage.
 """
 
 from waffle_hub import get_installed_backend_version
 
-BACKEND_NAME = "autocare_tx_model"
+BACKEND_NAME = "autocare_dlt"
 BACKEND_VERSION = get_installed_backend_version(BACKEND_NAME)
 
 import warnings
 from pathlib import Path
 from typing import Union
 
 import tbparse
 import torch
-from attrdict import AttrDict
-from autocare_tx_model.core.model import build_model
-from autocare_tx_model.tools import train
+from autocare_dlt.core.model import build_model
+from autocare_dlt.tools import train
+from box import Box
 from torchvision import transforms as T
 from waffle_utils.file import io
+from waffle_utils.utils import type_validator
 
 from waffle_hub import TaskType
-from waffle_hub.hub.adapter.tx_model.configs import (
+from waffle_hub.hub.adapter.autocare_dlt.configs import (
     get_data_config,
     get_model_config,
 )
 from waffle_hub.hub.base_hub import BaseHub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
 from .config import DATA_TYPE_MAP, DEFAULT_PARAMAS, MODEL_TYPES, WEIGHT_PATH
 
 
-class TxModelHub(BaseHub):
+class AutocareDLTHub(BaseHub):
     MODEL_TYPES = MODEL_TYPES
     DATA_TYPE_MAP = DATA_TYPE_MAP
     WEIGHT_PATH = WEIGHT_PATH
     DEFAULT_PARAMAS = DEFAULT_PARAMAS
 
     def __init__(
         self,
@@ -46,15 +47,15 @@
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
         backend: str = None,
         version: str = None,
     ):
-        """Create Tx Model Hub Class. Do not use this class directly. Use TxModelHub.new() instead."""
+        """Create Tx Model Hub Class. Do not use this class directly. Use AutocareDLTHub.new() instead."""
 
         if backend is not None and backend != BACKEND_NAME:
             raise ValueError(f"you've loaded {backend}. backend must be {BACKEND_NAME}")
 
         if version is not None and version != BACKEND_VERSION:
             warnings.warn(
                 f"you've loaded a {BACKEND_NAME}=={version} version while {BACKEND_NAME}=={BACKEND_VERSION} version is installed."
@@ -97,14 +98,32 @@
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
+    @property
+    def categories(self) -> list[dict]:
+        return self.__categories
+
+    @categories.setter
+    @type_validator(list)
+    def categories(self, v):
+        if isinstance(v[0], str):
+            v = [{"supercategory": "object", "name": n} for n in v]
+        elif isinstance(v[0], dict) and "supercategory" not in v[0]:
+            # TODO: Temporal solution for DLT classification: Not supported multi-task yet.
+            v_ = []
+            for k, cls in v[0].items():
+                for c in cls:
+                    v_.append({"supercategory": k, "name": c})
+            v = v_
+        self.__categories = v
+
     # Hub Utils
     def get_preprocess(self, *args, **kwargs):
 
         if self.task == TaskType.OBJECT_DETECTION:
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
@@ -180,19 +199,24 @@
             str(cfg.dataset_path / "images"),
             str(cfg.dataset_path / "test.json"),
             str(cfg.dataset_path / "images"),
         )
 
         cfg.data_config = self.artifact_dir / "data.json"
         io.save_json(data_config, cfg.data_config, create_directory=True)
+        categories = (
+            self.categories
+            if self._BaseHub__task == "classification"
+            else [x["name"] for x in self.categories]
+        )
 
         model_config = get_model_config(
             self.model_type,
             self.model_size,
-            [x["name"] for x in self.categories],
+            categories,
             cfg.seed,
             cfg.learning_rate,
             cfg.letter_box,
             cfg.epochs,
         )
 
         cfg.model_config = self.artifact_dir / "model.json"
@@ -251,15 +275,15 @@
 
         # get model
         categories = [x["name"] for x in self.categories]
         cfg = io.load_json(self.artifact_dir / "model.json")
         cfg["ckpt"] = str(self.best_ckpt_file)
         cfg["model"]["head"]["num_classes"] = len(categories)
         cfg["num_classes"] = len(categories)
-        model, categories = build_model(AttrDict(cfg), strict=True)
+        model, categories = build_model(Box(cfg), strict=True)
 
         model = ModelWrapper(
             model=model.eval(),
             preprocess=preprocess,
             postprocess=postprocess,
         )
```

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/config.py` & `waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/base_hub.py` & `waffle_hub-0.2.2/waffle_hub/hub/base_hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,38 +13,37 @@
 import warnings
 from functools import cached_property
 from pathlib import Path
 from typing import Union
 
 import cpuinfo
 import cv2
+import numpy as np
 import torch
 import tqdm
-import numpy as np
-
 from waffle_utils.file import io
 from waffle_utils.utils import type_validator
 
 from waffle_hub import TaskType
 from waffle_hub.dataset import Dataset
 from waffle_hub.hub.model.wrapper import get_parser
 from waffle_hub.schema.configs import (
     EvaluateConfig,
     ExportConfig,
     InferenceConfig,
     ModelConfig,
     TrainConfig,
 )
+from waffle_hub.schema.data import ImageInfo
 from waffle_hub.schema.result import (
     EvaluateResult,
     ExportResult,
     InferenceResult,
     TrainResult,
 )
-from waffle_hub.schema.data import ImageInfo
 from waffle_hub.utils.callback import (
     EvaluateCallback,
     ExportCallback,
     InferenceCallback,
     TrainCallback,
 )
 from waffle_hub.utils.data import ImageDataset, LabeledDataset, get_image_transform
@@ -436,41 +435,43 @@
 
         Returns:
             list[dict]: inference result
         """
         if not self.inference_file.exists():
             return []
         return io.load_json(self.inference_file)
-    
+
     # Hub Utils
     def get_image_loader(self) -> tuple[torch.Tensor, ImageInfo]:
         """Get image loader function.
 
         Returns:
             tuple[torch.Tensor, ImageInfo]: input transform function
-        
+
         Example:
             >>> transform = hub.get_image_loader()
             >>> image, image_info = transform("path/to/image.jpg")
             >>> model = hub.get_model()
             >>> output = model(image.unsqueeze(0))
         """
         train_config: TrainConfig = self.get_train_config()
         transform = get_image_transform(train_config.image_size, train_config.letter_box)
+
         def inner(x: Union[np.ndarray, str]):
             """Input Transform Function
-            
+
             Args:
                 x (Union[np.ndarray, str]): opencv image or image path
-                
+
             Returns:
                 tuple[torch.Tensor, ImageInfo]: image and image info
             """
             image, image_info = transform(x)
             return image, image_info
+
         return inner
 
     # Train Hook
     def before_train(self, cfg: TrainConfig):
         pass
 
     def on_train_start(self, cfg: TrainConfig):
```

### Comparing `waffle_hub-0.2.1/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.2.2/waffle_hub/hub/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/run.py` & `waffle_hub-0.2.2/waffle_hub/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from typing import List
 
 import typer
 from rich import print
 
 from waffle_hub.dataset.dataset import Dataset
+from waffle_hub.hub.adapter.autocare_dlt import AutocareDLTHub
 from waffle_hub.hub.adapter.hugging_face import HuggingFaceHub
 from waffle_hub.hub.adapter.ultralytics import UltralyticsHub
 
-# from waffle_hub.hub.adapter.tx_model import TxModelHub
-
 dataset = typer.Typer(name="dataset")
 hub = typer.Typer(name="hub")
 app = typer.Typer()
 app.add_typer(dataset)
 app.add_typer(hub)
 
 BACKEND_MAP = {
     "ultralytics": UltralyticsHub,
     "huggingface": HuggingFaceHub,
-    # "tx_model": TxModelHub,
+    "autocare_dlt": AutocareDLTHub,
 }
 
 EXPORT_MAP = {
     "ultralytics": "YOLO",
     "huggingface": "HUGGINGFACE",
-    # "tx_model": "TX_MODEL",
+    "autocare_dlt": "AutocareDLT",
 }
 
 
 @hub.command(name="new")
 def _new_hub(
     backend: str = typer.Option(..., help="Backend to use"),
     name: str = typer.Option(..., help="Name of the hub"),
@@ -312,9 +311,114 @@
         name=name,
         root_dir=root_dir,
     )
 
     ds.export(data_type)
 
 
+@dataset.command(name="delete")
+def _delete_dataset(
+    name: str = typer.Option(..., help="Name of the dataset"),
+    root_dir: str = typer.Option(..., help="Root directory"),
+):
+    ds = Dataset.load(
+        name=name,
+        root_dir=root_dir,
+    )
+
+    ds.delete()
+
+
+@dataset.command(name="get_split_ids")
+def _get_split_ids(
+    name: str = typer.Option(..., help="Name of the dataset"),
+    root_dir: str = typer.Option(..., help="Root directory"),
+):
+    ds = Dataset.load(
+        name=name,
+        root_dir=root_dir,
+    )
+
+    for set_name, set_ids in zip(["train", "val", "test", "unlabeled"], ds.get_split_ids()):
+        print(f"{set_name}: {set_ids}")
+
+
+@dataset.command(name="merge")
+def _merge_dataset(
+    name: str = typer.Option(..., help="Name of the dataset"),
+    root_dir: str = typer.Option(..., help="Root directory"),
+    src_names: list[str] = typer.Option(..., help="Source name of the dataset"),
+    src_root_dirs: list[str] = typer.Option(..., help="Source root directory"),
+    task: str = typer.Option(..., help="Task"),
+):
+    Dataset.merge(
+        name=name,
+        root_dir=root_dir,
+        src_names=src_names,
+        src_root_dirs=src_root_dirs,
+        task=task,
+    )
+
+
+@dataset.command(name="sample")
+def _sample_dataset(
+    name: str = typer.Option(..., help="Name of the dataset"),
+    root_dir: str = typer.Option(..., help="Root directory"),
+    task: str = typer.Option(..., help="Task"),
+):
+    Dataset.sample(
+        name=name,
+        root_dir=root_dir,
+        task=task,
+    )
+
+
+@dataset.command(name="get_images")
+def _get_images_dataset(
+    name: str = typer.Option(..., help="Name of the dataset"),
+    root_dir: str = typer.Option(..., help="Root directory"),
+):
+    ds = Dataset.load(
+        name=name,
+        root_dir=root_dir,
+    )
+
+    images = ds.get_images()
+
+    for image in images:
+        print(image.to_dict())
+
+
+@dataset.command(name="get_annotations")
+def _get_annotations_dataset(
+    name: str = typer.Option(..., help="Name of the dataset"),
+    root_dir: str = typer.Option(..., help="Root directory"),
+):
+    ds = Dataset.load(
+        name=name,
+        root_dir=root_dir,
+    )
+
+    annotations = ds.get_annotations()
+
+    for annotation in annotations:
+        print(annotation.to_dict())
+
+
+@dataset.command(name="get_categories")
+def _get_categories_dataset(
+    name: str = typer.Option(..., help="Name of the dataset"),
+    root_dir: str = typer.Option(..., help="Root directory"),
+):
+    ds = Dataset.load(
+        name=name,
+        root_dir=root_dir,
+    )
+
+    categories = ds.get_categories()
+
+    for category in categories:
+        print(category.to_dict())
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `waffle_hub-0.2.1/waffle_hub/schema/base_schema.py` & `waffle_hub-0.2.2/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/schema/configs.py` & `waffle_hub-0.2.2/waffle_hub/schema/configs.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/schema/data.py` & `waffle_hub-0.2.2/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.2/waffle_hub/schema/fields/annotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Union
 
+from shapely import Polygon
 from waffle_utils.utils import type_validator
 
 from waffle_hub import TaskType
 from waffle_hub.utils.conversion import convert_rle_to_polygon
 
 from .base_field import BaseField
 
@@ -91,32 +92,20 @@
         self.__bbox = v
 
     @property
     def segmentation(self):
         return self.__segmentation
 
     @segmentation.setter
-    # XXX: dict->rle, list->polygon
     def segmentation(self, v):
-        if isinstance(v, dict):
-            v: list = convert_rle_to_polygon(v)
         if v:
             for segment in v:
                 if len(segment) % 2 != 0:
                     raise ValueError("the length of segmentation should be divisible by 2.")
 
-            if self.bbox is None:
-                xs = [x for segment in v for x in segment[::2]]
-                ys = [y for segment in v for y in segment[1::2]]
-                x1 = min(xs)
-                y1 = min(ys)
-                w = max(xs) - x1
-                h = max(ys) - y1
-                self.bbox = [x1, y1, w, h]
-
         self.__segmentation = v
 
     @property
     def area(self):
         return self.__area
 
     @area.setter
@@ -186,14 +175,38 @@
 
     @task.setter
     def task(self, v):
         if v is not None and v not in TaskType:
             raise ValueError(f"Invalid task type: {v}" f"Available task types: {list(TaskType)}")
         self.__task = str(v).upper()
 
+    def __eq__(self, other):
+        if not isinstance(other, Annotation):
+            return False
+
+        if self.task == TaskType.CLASSIFICATION:
+            return self.category_id == other.category_id
+
+        elif self.task == TaskType.OBJECT_DETECTION:
+            return (
+                self.category_id == other.category_id
+                and self.bbox == other.bbox
+                and self.iscrowd == other.iscrowd
+            )
+
+        elif self.task == TaskType.INSTANCE_SEGMENTATION:
+            return (
+                self.category_id == other.category_id
+                and self.segmentation == other.segmentation
+                and self.iscrowd == other.iscrowd
+            )
+
+        else:
+            raise NotImplementedError(f"Task type {self.task} is not supported.")
+
     # factories
     @classmethod
     def new(
         cls,
         annotation_id: int = None,
         image_id: int = None,
         category_id: int = None,
@@ -297,14 +310,18 @@
             area (int): bbox area.
             iscrowd (int, optional): is crowd or not. Default to 0.
             score (float, optional): prediction score. Default to None.
 
         Returns:
             Annotation: annotation class
         """
+
+        if area is None:
+            area = bbox[2] * bbox[3]
+
         return cls(
             annotation_id,
             image_id,
             category_id=category_id,
             bbox=bbox,
             area=area,
             iscrowd=iscrowd,
@@ -315,35 +332,53 @@
     @classmethod
     def semantic_segmentation(
         cls,
         annotation_id: int = None,
         image_id: int = None,
         category_id: int = None,
         bbox: list[float] = None,
-        segmentation: list[list[float]] = None,
+        segmentation: Union[list[list[float]], dict] = None,
         area: int = None,
         iscrowd: int = 0,
         score: float = None,
         **kwargs,
     ) -> "Annotation":
         """Segmentation Annotation Format
 
         Args:
             annotation_id (int): annotaion id. natural number.
             image_id (int): image id. natural number.
             category_id (int): category id. natural number.
             bbox (list[float]): [x1, y1, w, h].
-            segmentation (list[list[float]]): [[x1, y1, x2, y2, x3, y3, ...], [polygon]].
+            segmentation (Union[list[list[float]], dict]): [[x1, y1, x2, y2, x3, y3, ...], [polygon]] or RLE.
             area (int): segmentation segmentation area.
             iscrowd (int, optional): is crowd or not. Default to 0.
             score (float, optional): prediction score. Default to None.
 
         Returns:
             Annotation: annotation class
         """
+
+        if isinstance(segmentation, dict):
+            segmentation = convert_rle_to_polygon(segmentation)
+
+        if bbox is None:
+            xs = [x for polygon in segmentation for x in polygon[::2]]
+            ys = [y for polygon in segmentation for y in polygon[1::2]]
+            x1 = min(xs)
+            y1 = min(ys)
+            w = max(xs) - x1
+            h = max(ys) - y1
+            bbox = [x1, y1, w, h]
+
+        if area is None:
+            area = 0
+            for polygon in segmentation:
+                area += Polygon([(x, y) for x, y in zip(polygon[::2], polygon[1::2])]).area
+
         return cls(
             annotation_id,
             image_id,
             category_id=category_id,
             bbox=bbox,
             segmentation=segmentation,
             area=area,
@@ -355,35 +390,53 @@
     @classmethod
     def instance_segmentation(
         cls,
         annotation_id: int = None,
         image_id: int = None,
         category_id: int = None,
         bbox: list[float] = None,
-        segmentation: list[list[float]] = None,
+        segmentation: Union[list[list[float]], dict] = None,
         area: int = None,
         iscrowd: int = 0,
         score: float = None,
         **kwargs,
     ) -> "Annotation":
         """Instance Annotation Format
 
         Args:
             annotation_id (int): annotaion id. natural number.
             image_id (int): image id. natural number.
             category_id (int): category id. natural number.
             bbox (list[float]): [x1, y1, w, h].
-            segmentation (list[list[float]]): [[x1, y1, x2, y2, x3, y3, ...], [polygon]].
+            segmentation (Union[list[list[float]], dict]): [[x1, y1, x2, y2, x3, y3, ...], [polygon]] or RLE.
             area (int): segmentation segmentation area.
             iscrowd (int, optional): is crowd or not. Default to 0.
             score (float, optional): prediction score. Default to None.
 
         Returns:
             Annotation: annotation class
         """
+
+        if isinstance(segmentation, dict):
+            segmentation = convert_rle_to_polygon(segmentation)
+
+        if bbox is None:
+            xs = [x for polygon in segmentation for x in polygon[::2]]
+            ys = [y for polygon in segmentation for y in polygon[1::2]]
+            x1 = min(xs)
+            y1 = min(ys)
+            w = max(xs) - x1
+            h = max(ys) - y1
+            bbox = [x1, y1, w, h]
+
+        if area is None:
+            area = 0
+            for polygon in segmentation:
+                area += Polygon([(x, y) for x, y in zip(polygon[::2], polygon[1::2])]).area
+
         return cls(
             annotation_id,
             image_id,
             category_id=category_id,
             bbox=bbox,
             segmentation=segmentation,
             area=area,
```

### Comparing `waffle_hub-0.2.1/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.2/waffle_hub/schema/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.2/waffle_hub/schema/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.2/waffle_hub/schema/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/utils/callback.py` & `waffle_hub-0.2.2/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/utils/conversion.py` & `waffle_hub-0.2.2/waffle_hub/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/utils/data.py` & `waffle_hub-0.2.2/waffle_hub/utils/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/utils/draw.py` & `waffle_hub-0.2.2/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.2/waffle_hub/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.1/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.2.2/waffle_hub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.2.1
+Version: 0.2.2
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.1 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.2 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.1/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.2/waffle_hub.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 waffle_hub/experimental/__init__.py
 waffle_hub/experimental/serve.py
 waffle_hub/experimental/auto_label/__init__.py
 waffle_hub/experimental/auto_label/grounding_dino.py
 waffle_hub/hub/__init__.py
 waffle_hub/hub/base_hub.py
 waffle_hub/hub/adapter/__init__.py
+waffle_hub/hub/adapter/autocare_dlt/__init__.py
+waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
+waffle_hub/hub/adapter/autocare_dlt/config.py
+waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
+waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
+waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
 waffle_hub/hub/adapter/hugging_face/__init__.py
 waffle_hub/hub/adapter/hugging_face/config.py
 waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
 waffle_hub/hub/adapter/hugging_face/train_input_helper.py
-waffle_hub/hub/adapter/tx_model/__init__.py
-waffle_hub/hub/adapter/tx_model/config.py
-waffle_hub/hub/adapter/tx_model/tx_model_hub.py
-waffle_hub/hub/adapter/tx_model/configs/__init__.py
-waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
-waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
 waffle_hub/hub/adapter/ultralytics/__init__.py
 waffle_hub/hub/adapter/ultralytics/config.py
 waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
 waffle_hub/hub/model/__init__.py
 waffle_hub/hub/model/wrapper.py
 waffle_hub/schema/__init__.py
 waffle_hub/schema/base_schema.py
```

