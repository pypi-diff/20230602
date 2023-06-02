# Comparing `tmp/fusionlab-0.1.1.tar.gz` & `tmp/fusionlab-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusionlab-0.1.1.tar", last modified: Fri Jun  2 07:18:07 2023, max compression
+gzip compressed data, was "fusionlab-0.1.2.tar", last modified: Fri Jun  2 07:56:10 2023, max compression
```

## Comparing `fusionlab-0.1.1.tar` & `fusionlab-0.1.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.208282 fusionlab-0.1.1/
--rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.1/LICENSE
--rw-r--r--   0 cyli       (502) staff       (20)     3337 2023-06-02 07:18:07.208100 fusionlab-0.1.1/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     2874 2023-06-02 07:07:59.000000 fusionlab-0.1.1/README.md
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.195335 fusionlab-0.1.1/fusionlab/
--rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)       63 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/__version__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.196865 fusionlab-0.1.1/fusionlab/classification/
--rw-r--r--   0 cyli       (502) staff       (20)      310 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/classification/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      924 2023-05-21 15:35:40.000000 fusionlab-0.1.1/fusionlab/classification/base.py
--rw-r--r--   0 cyli       (502) staff       (20)      701 2023-05-21 15:35:40.000000 fusionlab-0.1.1/fusionlab/classification/lstm.py
--rw-r--r--   0 cyli       (502) staff       (20)     1368 2023-05-21 15:39:08.000000 fusionlab-0.1.1/fusionlab/classification/vgg.py
--rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/configs.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.198377 fusionlab-0.1.1/fusionlab/datasets/
--rw-r--r--   0 cyli       (502) staff       (20)      422 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/datasets/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/datasets/a12lead.py
--rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/datasets/cinc2017.py
--rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/datasets/csvread.py
--rw-r--r--   0 cyli       (502) staff       (20)     7788 2023-06-02 07:08:22.000000 fusionlab-0.1.1/fusionlab/datasets/ludb.py
--rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/datasets/muse.py
--rw-r--r--   0 cyli       (502) staff       (20)     1506 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/datasets/utils.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.198519 fusionlab-0.1.1/fusionlab/encoders/
--rw-r--r--   0 cyli       (502) staff       (20)      507 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.199114 fusionlab-0.1.1/fusionlab/encoders/alexnet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/alexnet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-05-22 15:23:04.000000 fusionlab-0.1.1/fusionlab/encoders/alexnet/alexnet.py
--rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.1/fusionlab/encoders/alexnet/tfalexnet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.199662 fusionlab-0.1.1/fusionlab/encoders/inceptionv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/inceptionv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-05-22 15:20:40.000000 fusionlab-0.1.1/fusionlab/encoders/inceptionv1/inceptionv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.1/fusionlab/encoders/inceptionv1/tfinceptionv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.200218 fusionlab-0.1.1/fusionlab/encoders/resnetv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/resnetv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-05-22 15:21:31.000000 fusionlab-0.1.1/fusionlab/encoders/resnetv1/resnetv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.1/fusionlab/encoders/resnetv1/tfresnetv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.200808 fusionlab-0.1.1/fusionlab/encoders/vgg/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/vgg/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.1/fusionlab/encoders/vgg/tfvgg.py
--rw-r--r--   0 cyli       (502) staff       (20)     4751 2023-05-22 15:25:07.000000 fusionlab-0.1.1/fusionlab/encoders/vgg/vgg.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.201878 fusionlab-0.1.1/fusionlab/functional/
--rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/tfdice.py
--rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.202151 fusionlab-0.1.1/fusionlab/layers/
--rw-r--r--   0 cyli       (502) staff       (20)      255 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/layers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)    15525 2023-05-30 12:59:43.000000 fusionlab-0.1.1/fusionlab/layers/factories.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.202642 fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1045 2023-05-20 16:17:48.000000 fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/se.py
--rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/tfse.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.202869 fusionlab-0.1.1/fusionlab/losses/
--rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/losses/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.203320 fusionlab-0.1.1/fusionlab/losses/diceloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/losses/diceloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/losses/diceloss/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.1/fusionlab/losses/diceloss/tfdice.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.203881 fusionlab-0.1.1/fusionlab/losses/iouloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/losses/iouloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/losses/iouloss/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.1/fusionlab/losses/iouloss/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.204593 fusionlab-0.1.1/fusionlab/losses/tversky/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.1/fusionlab/losses/tversky/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.1/fusionlab/losses/tversky/tftversky.py
--rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.1/fusionlab/losses/tversky/tversky.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.204872 fusionlab-0.1.1/fusionlab/metrics/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/metrics/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.205249 fusionlab-0.1.1/fusionlab/segmentation/
--rw-r--r--   0 cyli       (502) staff       (20)      378 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      388 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/base.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.205824 fusionlab-0.1.1/fusionlab/segmentation/resunet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.1/fusionlab/segmentation/resunet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     5240 2023-06-02 02:24:31.000000 fusionlab-0.1.1/fusionlab/segmentation/resunet/resunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/resunet/tfresunet.py
--rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/tfbase.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.206282 fusionlab-0.1.1/fusionlab/segmentation/unet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.1/fusionlab/segmentation/unet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/unet/tfunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     5383 2023-05-21 15:35:40.000000 fusionlab-0.1.1/fusionlab/segmentation/unet/unet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.206693 fusionlab-0.1.1/fusionlab/segmentation/unet2plus/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.1/fusionlab/segmentation/unet2plus/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/unet2plus/tfunet2plus.py
--rw-r--r--   0 cyli       (502) staff       (20)     5631 2023-05-21 15:35:40.000000 fusionlab-0.1.1/fusionlab/segmentation/unet2plus/unet2plus.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.207366 fusionlab-0.1.1/fusionlab/trainers/
--rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/trainers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/trainers/dcgan.py
--rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.1/fusionlab/trainers/test.py
--rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/trainers/trainer.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.207877 fusionlab-0.1.1/fusionlab/utils/
--rw-r--r--   0 cyli       (502) staff       (20)       60 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/utils/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      218 2022-12-31 04:40:09.000000 fusionlab-0.1.1/fusionlab/utils/basic.py
--rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/utils/trace.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.196141 fusionlab-0.1.1/fusionlab.egg-info/
--rw-r--r--   0 cyli       (502) staff       (20)     3337 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     2501 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/SOURCES.txt
--rw-r--r--   0 cyli       (502) staff       (20)        1 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/dependency_links.txt
--rw-r--r--   0 cyli       (502) staff       (20)      191 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/requires.txt
--rw-r--r--   0 cyli       (502) staff       (20)       10 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/top_level.txt
--rw-r--r--   0 cyli       (502) staff       (20)       38 2023-06-02 07:18:07.208332 fusionlab-0.1.1/setup.cfg
--rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.1/setup.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.659056 fusionlab-0.1.2/
+-rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.2/LICENSE
+-rw-r--r--   0 cyli       (502) staff       (20)     3337 2023-06-02 07:56:10.658918 fusionlab-0.1.2/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     2874 2023-06-02 07:07:59.000000 fusionlab-0.1.2/README.md
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.645246 fusionlab-0.1.2/fusionlab/
+-rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)       63 2023-06-02 07:55:20.000000 fusionlab-0.1.2/fusionlab/__version__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.646571 fusionlab-0.1.2/fusionlab/classification/
+-rw-r--r--   0 cyli       (502) staff       (20)      310 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/classification/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      924 2023-05-21 15:35:40.000000 fusionlab-0.1.2/fusionlab/classification/base.py
+-rw-r--r--   0 cyli       (502) staff       (20)      701 2023-05-21 15:35:40.000000 fusionlab-0.1.2/fusionlab/classification/lstm.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1368 2023-05-21 15:39:08.000000 fusionlab-0.1.2/fusionlab/classification/vgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/configs.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.648114 fusionlab-0.1.2/fusionlab/datasets/
+-rw-r--r--   0 cyli       (502) staff       (20)      486 2023-06-02 07:24:15.000000 fusionlab-0.1.2/fusionlab/datasets/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/datasets/a12lead.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/datasets/cinc2017.py
+-rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/datasets/csvread.py
+-rw-r--r--   0 cyli       (502) staff       (20)     9199 2023-06-02 07:54:07.000000 fusionlab-0.1.2/fusionlab/datasets/ludb.py
+-rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/datasets/muse.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1506 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/datasets/utils.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.648238 fusionlab-0.1.2/fusionlab/encoders/
+-rw-r--r--   0 cyli       (502) staff       (20)      507 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.648800 fusionlab-0.1.2/fusionlab/encoders/alexnet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/alexnet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-05-22 15:23:04.000000 fusionlab-0.1.2/fusionlab/encoders/alexnet/alexnet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.2/fusionlab/encoders/alexnet/tfalexnet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.649319 fusionlab-0.1.2/fusionlab/encoders/inceptionv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/inceptionv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-05-22 15:20:40.000000 fusionlab-0.1.2/fusionlab/encoders/inceptionv1/inceptionv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.2/fusionlab/encoders/inceptionv1/tfinceptionv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.649879 fusionlab-0.1.2/fusionlab/encoders/resnetv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/resnetv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-05-22 15:21:31.000000 fusionlab-0.1.2/fusionlab/encoders/resnetv1/resnetv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.2/fusionlab/encoders/resnetv1/tfresnetv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.650424 fusionlab-0.1.2/fusionlab/encoders/vgg/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/vgg/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.2/fusionlab/encoders/vgg/tfvgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4751 2023-05-22 15:25:07.000000 fusionlab-0.1.2/fusionlab/encoders/vgg/vgg.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.651158 fusionlab-0.1.2/fusionlab/functional/
+-rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/tfdice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.651413 fusionlab-0.1.2/fusionlab/layers/
+-rw-r--r--   0 cyli       (502) staff       (20)      255 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/layers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)    15525 2023-05-30 12:59:43.000000 fusionlab-0.1.2/fusionlab/layers/factories.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.653071 fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1045 2023-05-20 16:17:48.000000 fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/se.py
+-rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/tfse.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.653777 fusionlab-0.1.2/fusionlab/losses/
+-rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/losses/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.654234 fusionlab-0.1.2/fusionlab/losses/diceloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/losses/diceloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/losses/diceloss/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.2/fusionlab/losses/diceloss/tfdice.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.654773 fusionlab-0.1.2/fusionlab/losses/iouloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/losses/iouloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/losses/iouloss/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.2/fusionlab/losses/iouloss/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.655331 fusionlab-0.1.2/fusionlab/losses/tversky/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.2/fusionlab/losses/tversky/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.2/fusionlab/losses/tversky/tftversky.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.2/fusionlab/losses/tversky/tversky.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.655580 fusionlab-0.1.2/fusionlab/metrics/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/metrics/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.655923 fusionlab-0.1.2/fusionlab/segmentation/
+-rw-r--r--   0 cyli       (502) staff       (20)      378 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      388 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/base.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.656396 fusionlab-0.1.2/fusionlab/segmentation/resunet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.2/fusionlab/segmentation/resunet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5240 2023-06-02 02:24:31.000000 fusionlab-0.1.2/fusionlab/segmentation/resunet/resunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/resunet/tfresunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/tfbase.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.656758 fusionlab-0.1.2/fusionlab/segmentation/unet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.2/fusionlab/segmentation/unet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/unet/tfunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5383 2023-05-21 15:35:40.000000 fusionlab-0.1.2/fusionlab/segmentation/unet/unet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.657107 fusionlab-0.1.2/fusionlab/segmentation/unet2plus/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.2/fusionlab/segmentation/unet2plus/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/unet2plus/tfunet2plus.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5631 2023-05-21 15:35:40.000000 fusionlab-0.1.2/fusionlab/segmentation/unet2plus/unet2plus.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.657849 fusionlab-0.1.2/fusionlab/trainers/
+-rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/trainers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/trainers/dcgan.py
+-rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.2/fusionlab/trainers/test.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/trainers/trainer.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.658556 fusionlab-0.1.2/fusionlab/utils/
+-rw-r--r--   0 cyli       (502) staff       (20)       60 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/utils/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      218 2022-12-31 04:40:09.000000 fusionlab-0.1.2/fusionlab/utils/basic.py
+-rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/utils/trace.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.645914 fusionlab-0.1.2/fusionlab.egg-info/
+-rw-r--r--   0 cyli       (502) staff       (20)     3337 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     2501 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/SOURCES.txt
+-rw-r--r--   0 cyli       (502) staff       (20)        1 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/dependency_links.txt
+-rw-r--r--   0 cyli       (502) staff       (20)      191 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/requires.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       10 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/top_level.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       38 2023-06-02 07:56:10.659100 fusionlab-0.1.2/setup.cfg
+-rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.2/setup.py
```

### Comparing `fusionlab-0.1.1/LICENSE` & `fusionlab-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/PKG-INFO` & `fusionlab-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.1
+Version: 0.1.2
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fusionlab-0.1.1/README.md` & `fusionlab-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/__init__.py` & `fusionlab-0.1.2/fusionlab/__init__.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/classification/base.py` & `fusionlab-0.1.2/fusionlab/classification/base.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/classification/lstm.py` & `fusionlab-0.1.2/fusionlab/classification/lstm.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/classification/vgg.py` & `fusionlab-0.1.2/fusionlab/classification/vgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/datasets/a12lead.py` & `fusionlab-0.1.2/fusionlab/datasets/a12lead.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/datasets/cinc2017.py` & `fusionlab-0.1.2/fusionlab/datasets/cinc2017.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/datasets/ludb.py` & `fusionlab-0.1.2/fusionlab/datasets/ludb.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,27 +42,41 @@
 PAT_ID_LIST = list(range(1, 201))
 CLS_COLOR = {
     1: 'red', # p
     2: 'blue', # qrs
     3: 'green', # t
 }
 
-# plot signal with annotation
 def plot(signal, label_seq):
+    """plot signal with annotation"""
     import matplotlib.pyplot as plt
     plt.plot(signal[:, 0].numpy())
     # fill range with matplotlib axvspan
     for i in range(len(label_seq)):
         if label_seq[i] != 0:
-            plt.axvspan(i, i+1, color=CLS_COLOR[label_seq[i].item()], alpha=0.5, 
-                        linewidth=0,
-                        )
+            plt.axvspan(i, i+1, 
+                        color=CLS_COLOR[label_seq[i].item()], 
+                        alpha=0.5, 
+                        linewidth=0)
     plt.show()
 
 class LUDBDataset(torch.utils.data.Dataset):
+    """
+    Args:
+        data_dir (str): path to the dataset folder
+        annotation_path (str): path to the annotation json file
+        transform (callable, optional): Optional transform to be applied on a sample.
+        start_idx (int): start index of the signal
+        end_idx (int): end index of the signal
+
+    Returns:
+        signal: (channels, sequence lenth)
+        label_seq: (sequence lenth,)
+
+    """
     def __init__(self, data_dir, annotation_path, transform=None, start_idx=641, end_idx=3996):
         # validate raw files
         try:
             self.validate_files(data_dir)
         except Exception as e:
             print(e)
             print(f"Start downloading the dataset from {DATASET_URL} to {os.path.join(data_dir, TARGET_FILENAME)}")
@@ -95,25 +109,42 @@
         signal, label_seq = self.extract_signal_label(signal, label_seq)
 
         if self.transform:
             signal = self.transform(signal)
 
         signal = torch.tensor(signal, dtype=torch.float)
         label_seq = torch.tensor(label_seq, dtype=torch.long)
+        signal = signal.permute(1, 0) # (C, L)
         return signal, label_seq
 
     def __len__(self):
         return len(self.file_ids)
     
     def extract_signal_label(self, signal, label):
-        # extract signal and label with respect to start and end index
+        """
+        extract signal and label with respect to start and end index
+
+        Args:
+            signal (np.array): (signal length, 12)
+            label (np.array): (signal length,)
+        """
         return signal[self.start_idx:self.end_idx, :], label[self.start_idx:self.end_idx]
     
     # validate number of files and file types
     def validate_files(self, data_dir):
+        """
+        validate number of files and file types
+        1. check if files exist
+        2. check if file types are valid
+        3. check if number of files are valid
+
+        Args:
+            data_dir (str): path to the dataset folder
+
+        """
         assert os.path.exists(data_dir)
         paths = glob(os.path.join(data_dir, DIR_NAME, "data", "*"))
         if len(paths) == 0:
             raise Exception(f"No files found in the dataset folder: {data_dir}")
         
         extension_count = {}
         for p in paths:
@@ -123,38 +154,62 @@
         keys = list(extension_count.keys())
         counts = list(extension_count.values())
         if sorted(keys) != sorted(['dat', 'hea'] + LEAD_NAMES):
             raise Exception(f"Invalid file types: {keys}")
         if len(set(counts)) > 1:
             raise Exception(f"Different number of files for each file type: {extension_count}")
     
-    # process annotation file and save to json
     def process_annotation(self, export_path):
+        """ 
+        process annotation file and save to json
+
+        Args:
+            export_path (str): path to save the annotation json file
+
+        """
         label_list = []
         # extract symbols' index range
         for pat_id in tqdm(PAT_ID_LIST):
             label_dict = self.get_segment_annotation(pat_id)
             label_list.append(label_dict)
 
         # save label list to json
         with open(export_path, "w") as f:
             json.dump(label_list, f)
 
-    # map json annotation to label sequence
     def map_annotaion_to_label_seq(self, annotation, sig_len):
+        """
+        Args:
+            annotation (dict): annotation dict
+            sig_len (int): signal length
+        
+        Returns:
+            label_seq (np.array): label sequence with integer class index
+            
+        """
         label_seq = np.zeros(sig_len, dtype=int)
         for segment in annotation["label"]:
             start = segment["start"]
             end = segment["end"]
             segment_class = segment["timeserieslabels"][0]
             segment_class_idx = CLS_MAP[segment_class]
             label_seq[start:end] = segment_class_idx
         return label_seq
     
     def get_signal(self, DATA_FOLDER, index: int):
+        """
+        
+        Args:
+            DATA_FOLDER (str): path to the data folder
+            index (int): patient id
+
+        Returns:
+            signal (np.array): (signal length, 12)
+
+        """
         record = wfdb.rdrecord(DATA_FOLDER + "/" + str(index))
         assert type(record) is wfdb.Record
         return record.p_signal
 
 
     # get annotations given the ecg lead
     def get_annotation(self, DATA_FOLDER, index: int, lead_name: str):
```

### Comparing `fusionlab-0.1.1/fusionlab/datasets/muse.py` & `fusionlab-0.1.2/fusionlab/datasets/muse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/datasets/utils.py` & `fusionlab-0.1.2/fusionlab/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/encoders/alexnet/alexnet.py` & `fusionlab-0.1.2/fusionlab/encoders/alexnet/alexnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/encoders/alexnet/tfalexnet.py` & `fusionlab-0.1.2/fusionlab/encoders/alexnet/tfalexnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/encoders/inceptionv1/inceptionv1.py` & `fusionlab-0.1.2/fusionlab/encoders/inceptionv1/inceptionv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/encoders/inceptionv1/tfinceptionv1.py` & `fusionlab-0.1.2/fusionlab/encoders/inceptionv1/tfinceptionv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/encoders/resnetv1/resnetv1.py` & `fusionlab-0.1.2/fusionlab/encoders/resnetv1/resnetv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/encoders/resnetv1/tfresnetv1.py` & `fusionlab-0.1.2/fusionlab/encoders/resnetv1/tfresnetv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/encoders/vgg/tfvgg.py` & `fusionlab-0.1.2/fusionlab/encoders/vgg/tfvgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/encoders/vgg/vgg.py` & `fusionlab-0.1.2/fusionlab/encoders/vgg/vgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/functional/tfdice.py` & `fusionlab-0.1.2/fusionlab/functional/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/functional/tfiou.py` & `fusionlab-0.1.2/fusionlab/functional/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/layers/factories.py` & `fusionlab-0.1.2/fusionlab/layers/factories.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/se.py` & `fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/se.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/tfse.py` & `fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/tfse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/losses/diceloss/dice.py` & `fusionlab-0.1.2/fusionlab/losses/diceloss/dice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/losses/diceloss/tfdice.py` & `fusionlab-0.1.2/fusionlab/losses/diceloss/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/losses/iouloss/iou.py` & `fusionlab-0.1.2/fusionlab/losses/iouloss/iou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/losses/iouloss/tfiou.py` & `fusionlab-0.1.2/fusionlab/losses/iouloss/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/losses/tversky/tftversky.py` & `fusionlab-0.1.2/fusionlab/losses/tversky/tftversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/losses/tversky/tversky.py` & `fusionlab-0.1.2/fusionlab/losses/tversky/tversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/segmentation/resunet/resunet.py` & `fusionlab-0.1.2/fusionlab/segmentation/resunet/resunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/segmentation/resunet/tfresunet.py` & `fusionlab-0.1.2/fusionlab/segmentation/resunet/tfresunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/segmentation/tfbase.py` & `fusionlab-0.1.2/fusionlab/segmentation/tfbase.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/segmentation/unet/tfunet.py` & `fusionlab-0.1.2/fusionlab/segmentation/unet/tfunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/segmentation/unet/unet.py` & `fusionlab-0.1.2/fusionlab/segmentation/unet/unet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/segmentation/unet2plus/tfunet2plus.py` & `fusionlab-0.1.2/fusionlab/segmentation/unet2plus/tfunet2plus.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/segmentation/unet2plus/unet2plus.py` & `fusionlab-0.1.2/fusionlab/segmentation/unet2plus/unet2plus.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/trainers/dcgan.py` & `fusionlab-0.1.2/fusionlab/trainers/dcgan.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/trainers/trainer.py` & `fusionlab-0.1.2/fusionlab/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab/utils/trace.py` & `fusionlab-0.1.2/fusionlab/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/fusionlab.egg-info/PKG-INFO` & `fusionlab-0.1.2/fusionlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.1
+Version: 0.1.2
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fusionlab-0.1.1/fusionlab.egg-info/SOURCES.txt` & `fusionlab-0.1.2/fusionlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.1/setup.py` & `fusionlab-0.1.2/setup.py`

 * *Files identical despite different names*

