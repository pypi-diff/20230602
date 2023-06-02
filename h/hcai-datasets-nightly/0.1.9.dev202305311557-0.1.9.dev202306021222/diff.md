# Comparing `tmp/hcai-datasets-nightly-0.1.9.dev202305311557.tar.gz` & `tmp/hcai-datasets-nightly-0.1.9.dev202306021222.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-nightly-0.1.9.dev202305311557.tar", last modified: Wed May 31 15:57:56 2023, max compression
+gzip compressed data, was "hcai-datasets-nightly-0.1.9.dev202306021222.tar", last modified: Fri Jun  2 12:22:11 2023, max compression
```

## Comparing `hcai-datasets-nightly-0.1.9.dev202305311557.tar` & `hcai-datasets-nightly-0.1.9.dev202306021222.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.234508 hcai-datasets-nightly-0.1.9.dev202305311557/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-31 15:57:56.234508 hcai-datasets-nightly-0.1.9.dev202305311557/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.230508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.230508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.230508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.230508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.230508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.230508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.230508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.234508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.234508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.234508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22444 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)    25026 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.234508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12724 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    19619 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:57:56.234508 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-31 15:57:56.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-05-31 15:57:56.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 15:57:56.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-31 15:57:56.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-31 15:57:56.000000 hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 15:57:56.234508 hcai-datasets-nightly-0.1.9.dev202305311557/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-05-31 15:57:43.000000 hcai-datasets-nightly-0.1.9.dev202305311557/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.675143 hcai-datasets-nightly-0.1.9.dev202306021222/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-06-02 12:22:11.675143 hcai-datasets-nightly-0.1.9.dev202306021222/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.667143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.667143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.667143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.671143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.671143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.671143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.675143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.675143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.675143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.675143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22809 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25026 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.675143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12724 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19619 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:22:11.675143 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-06-02 12:22:11.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-06-02 12:22:11.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 12:22:11.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-02 12:22:11.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-02 12:22:11.000000 hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 12:22:11.675143 hcai-datasets-nightly-0.1.9.dev202306021222/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-06-02 12:21:57.000000 hcai-datasets-nightly-0.1.9.dev202306021222/setup.py
```

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/PKG-INFO` & `hcai-datasets-nightly-0.1.9.dev202306021222/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.9.dev202305311557
+Version: 0.1.9.dev202306021222
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/README.md` & `hcai-datasets-nightly-0.1.9.dev202306021222/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/import_validator.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_dataset_utils/statistics.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/__init__.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         sessions=None,
         annotator=None,
         schemes=None,
         roles=None,
         data_streams=None,
         start=None,
         end=None,
-        left_context="0s",
-        right_context="0s",
+        left_context=None,
+        right_context=None,
         frame_size=None,
         stride=None,
         add_rest_class=True,
         flatten_samples=False,
         supervised_keys=None,
         lazy_loading=False,
         fake_missing_data=True,
@@ -76,17 +76,19 @@
         self.sessions = sessions
         self.roles = roles
         self.schemes = schemes
         self.data_streams = data_streams
         self.annotator = annotator
 
         # Sliding window parameters for the main stream
-        self.left_context, self.left_context_unit = ndu.parse_time_str(left_context)
-        self.right_context, self.right_context_unit = ndu.parse_time_str(right_context)
+        self.left_context, self.left_context_unit = ndu.parse_time_str(left_context if left_context else '0')
+        self.right_context, self.right_context_unit = ndu.parse_time_str(right_context if right_context else '0')
         self.frame_size, self.frame_size_unit = ndu.parse_time_str(frame_size)
+
+        # Framesize 0 or None indicates that the whole session should be returned as one sample
         if self.frame_size == 0:
             print(
                 "WARNING: Frame size 0 is invalid. Returning whole session as sample."
             )
             self.frame_size = None
         self.stride, self.stride_unit = ndu.parse_time_str(stride) if stride else self.frame_size, self.frame_size_unit
 
@@ -377,17 +379,22 @@
                     raise fnf
 
     def _build_sample_dict(self, labels_for_frame, data_for_frame):
         sample_dict = {}
 
         garbage_detected = False
         for label_id, label_value in labels_for_frame:
-            # check for nan
-            if label_value != label_value:
-                garbage_detected = True
+            # if value is not list type check for nan
+            if (
+                    type(label_value) != list
+                    and type(label_value) != str
+                    and type(label_value) != np.ndarray
+            ):
+                if label_value != label_value:
+                    garbage_detected = True
 
             sample_dict.update({label_id: label_value})
 
         # If at least one label is a garbage label we skip this iteration
         if garbage_detected:
             return None
```

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets_nightly.egg-info/PKG-INFO` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.9.dev202305311557
+Version: 0.1.9.dev202306021222
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/hcai_datasets_nightly.egg-info/SOURCES.txt` & `hcai-datasets-nightly-0.1.9.dev202306021222/hcai_datasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.9.dev202305311557/setup.py` & `hcai-datasets-nightly-0.1.9.dev202306021222/setup.py`

 * *Files identical despite different names*

