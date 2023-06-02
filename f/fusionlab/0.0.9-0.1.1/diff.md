# Comparing `tmp/fusionlab-0.0.9.tar.gz` & `tmp/fusionlab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fusionlab-0.0.9.tar", last modified: Sat Dec 17 03:09:18 2022, max compression
+gzip compressed data, was "fusionlab-0.1.1.tar", last modified: Fri Jun  2 07:18:07 2023, max compression
```

## Comparing `fusionlab-0.0.9.tar` & `fusionlab-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,101 @@
-drwxr-xr-x   0 SheepLi    (502) staff       (20)        0 2022-12-17 03:09:18.000000 fusionlab-0.0.9/
--rw-r--r--   0 SheepLi    (502) staff       (20)      510 2022-12-17 03:09:18.000000 fusionlab-0.0.9/PKG-INFO
--rw-r--r--   0 SheepLi    (502) staff       (20)     1060 2022-12-10 09:38:45.000000 fusionlab-0.0.9/LICENSE
-drwxr-xr-x   0 SheepLi    (502) staff       (20)        0 2022-12-17 03:09:18.000000 fusionlab-0.0.9/fusionlab.egg-info/
--rw-r--r--   0 SheepLi    (502) staff       (20)      510 2022-12-17 03:09:18.000000 fusionlab-0.0.9/fusionlab.egg-info/PKG-INFO
--rw-r--r--   0 SheepLi    (502) staff       (20)      327 2022-12-17 03:09:18.000000 fusionlab-0.0.9/fusionlab.egg-info/SOURCES.txt
--rw-r--r--   0 SheepLi    (502) staff       (20)      119 2022-12-17 03:09:18.000000 fusionlab-0.0.9/fusionlab.egg-info/requires.txt
--rw-r--r--   0 SheepLi    (502) staff       (20)       10 2022-12-17 03:09:18.000000 fusionlab-0.0.9/fusionlab.egg-info/top_level.txt
--rw-r--r--   0 SheepLi    (502) staff       (20)        1 2022-12-17 03:09:18.000000 fusionlab-0.0.9/fusionlab.egg-info/dependency_links.txt
--rw-r--r--   0 SheepLi    (502) staff       (20)       27 2022-12-10 09:38:45.000000 fusionlab-0.0.9/README.md
--rw-r--r--   0 SheepLi    (502) staff       (20)     3944 2022-12-11 14:01:12.000000 fusionlab-0.0.9/setup.py
-drwxr-xr-x   0 SheepLi    (502) staff       (20)        0 2022-12-17 03:09:18.000000 fusionlab-0.0.9/fusionlab/
-drwxr-xr-x   0 SheepLi    (502) staff       (20)        0 2022-12-17 03:09:18.000000 fusionlab-0.0.9/fusionlab/layers/
--rw-r--r--   0 SheepLi    (502) staff       (20)        0 2022-12-16 09:07:14.000000 fusionlab-0.0.9/fusionlab/layers/__init__.py
--rw-r--r--   0 SheepLi    (502) staff       (20)      128 2022-12-16 09:33:52.000000 fusionlab-0.0.9/fusionlab/__init__.py
--rw-r--r--   0 SheepLi    (502) staff       (20)       63 2022-12-17 03:08:48.000000 fusionlab-0.0.9/fusionlab/__version__.py
-drwxr-xr-x   0 SheepLi    (502) staff       (20)        0 2022-12-17 03:09:18.000000 fusionlab-0.0.9/fusionlab/encoders/
--rw-r--r--   0 SheepLi    (502) staff       (20)       22 2022-12-16 09:29:29.000000 fusionlab-0.0.9/fusionlab/encoders/__init__.py
--rw-r--r--   0 SheepLi    (502) staff       (20)     2321 2022-12-17 03:08:27.000000 fusionlab-0.0.9/fusionlab/encoders/alexnet.py
--rw-r--r--   0 SheepLi    (502) staff       (20)       38 2022-12-17 03:09:18.000000 fusionlab-0.0.9/setup.cfg
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.208282 fusionlab-0.1.1/
+-rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.1/LICENSE
+-rw-r--r--   0 cyli       (502) staff       (20)     3337 2023-06-02 07:18:07.208100 fusionlab-0.1.1/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     2874 2023-06-02 07:07:59.000000 fusionlab-0.1.1/README.md
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.195335 fusionlab-0.1.1/fusionlab/
+-rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)       63 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/__version__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.196865 fusionlab-0.1.1/fusionlab/classification/
+-rw-r--r--   0 cyli       (502) staff       (20)      310 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/classification/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      924 2023-05-21 15:35:40.000000 fusionlab-0.1.1/fusionlab/classification/base.py
+-rw-r--r--   0 cyli       (502) staff       (20)      701 2023-05-21 15:35:40.000000 fusionlab-0.1.1/fusionlab/classification/lstm.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1368 2023-05-21 15:39:08.000000 fusionlab-0.1.1/fusionlab/classification/vgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/configs.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.198377 fusionlab-0.1.1/fusionlab/datasets/
+-rw-r--r--   0 cyli       (502) staff       (20)      422 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/datasets/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/datasets/a12lead.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/datasets/cinc2017.py
+-rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/datasets/csvread.py
+-rw-r--r--   0 cyli       (502) staff       (20)     7788 2023-06-02 07:08:22.000000 fusionlab-0.1.1/fusionlab/datasets/ludb.py
+-rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/datasets/muse.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1506 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/datasets/utils.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.198519 fusionlab-0.1.1/fusionlab/encoders/
+-rw-r--r--   0 cyli       (502) staff       (20)      507 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.199114 fusionlab-0.1.1/fusionlab/encoders/alexnet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/alexnet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-05-22 15:23:04.000000 fusionlab-0.1.1/fusionlab/encoders/alexnet/alexnet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.1/fusionlab/encoders/alexnet/tfalexnet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.199662 fusionlab-0.1.1/fusionlab/encoders/inceptionv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/inceptionv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-05-22 15:20:40.000000 fusionlab-0.1.1/fusionlab/encoders/inceptionv1/inceptionv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.1/fusionlab/encoders/inceptionv1/tfinceptionv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.200218 fusionlab-0.1.1/fusionlab/encoders/resnetv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/resnetv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-05-22 15:21:31.000000 fusionlab-0.1.1/fusionlab/encoders/resnetv1/resnetv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.1/fusionlab/encoders/resnetv1/tfresnetv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.200808 fusionlab-0.1.1/fusionlab/encoders/vgg/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/encoders/vgg/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.1/fusionlab/encoders/vgg/tfvgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4751 2023-05-22 15:25:07.000000 fusionlab-0.1.1/fusionlab/encoders/vgg/vgg.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.201878 fusionlab-0.1.1/fusionlab/functional/
+-rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/tfdice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/functional/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.202151 fusionlab-0.1.1/fusionlab/layers/
+-rw-r--r--   0 cyli       (502) staff       (20)      255 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/layers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)    15525 2023-05-30 12:59:43.000000 fusionlab-0.1.1/fusionlab/layers/factories.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.202642 fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1045 2023-05-20 16:17:48.000000 fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/se.py
+-rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.1/fusionlab/layers/squeeze_excitation/tfse.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.202869 fusionlab-0.1.1/fusionlab/losses/
+-rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/losses/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.203320 fusionlab-0.1.1/fusionlab/losses/diceloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/losses/diceloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/losses/diceloss/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.1/fusionlab/losses/diceloss/tfdice.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.203881 fusionlab-0.1.1/fusionlab/losses/iouloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/losses/iouloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/losses/iouloss/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.1/fusionlab/losses/iouloss/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.204593 fusionlab-0.1.1/fusionlab/losses/tversky/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.1/fusionlab/losses/tversky/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.1/fusionlab/losses/tversky/tftversky.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.1/fusionlab/losses/tversky/tversky.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.204872 fusionlab-0.1.1/fusionlab/metrics/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.1/fusionlab/metrics/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.205249 fusionlab-0.1.1/fusionlab/segmentation/
+-rw-r--r--   0 cyli       (502) staff       (20)      378 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      388 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/base.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.205824 fusionlab-0.1.1/fusionlab/segmentation/resunet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.1/fusionlab/segmentation/resunet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5240 2023-06-02 02:24:31.000000 fusionlab-0.1.1/fusionlab/segmentation/resunet/resunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/resunet/tfresunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/tfbase.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.206282 fusionlab-0.1.1/fusionlab/segmentation/unet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.1/fusionlab/segmentation/unet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/unet/tfunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5383 2023-05-21 15:35:40.000000 fusionlab-0.1.1/fusionlab/segmentation/unet/unet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.206693 fusionlab-0.1.1/fusionlab/segmentation/unet2plus/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.1/fusionlab/segmentation/unet2plus/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/segmentation/unet2plus/tfunet2plus.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5631 2023-05-21 15:35:40.000000 fusionlab-0.1.1/fusionlab/segmentation/unet2plus/unet2plus.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.207366 fusionlab-0.1.1/fusionlab/trainers/
+-rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.1/fusionlab/trainers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/trainers/dcgan.py
+-rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.1/fusionlab/trainers/test.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/trainers/trainer.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.207877 fusionlab-0.1.1/fusionlab/utils/
+-rw-r--r--   0 cyli       (502) staff       (20)       60 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/utils/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      218 2022-12-31 04:40:09.000000 fusionlab-0.1.1/fusionlab/utils/basic.py
+-rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 07:07:59.000000 fusionlab-0.1.1/fusionlab/utils/trace.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:18:07.196141 fusionlab-0.1.1/fusionlab.egg-info/
+-rw-r--r--   0 cyli       (502) staff       (20)     3337 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     2501 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/SOURCES.txt
+-rw-r--r--   0 cyli       (502) staff       (20)        1 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/dependency_links.txt
+-rw-r--r--   0 cyli       (502) staff       (20)      191 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/requires.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       10 2023-06-02 07:18:07.000000 fusionlab-0.1.1/fusionlab.egg-info/top_level.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       38 2023-06-02 07:18:07.208332 fusionlab-0.1.1/setup.cfg
+-rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fusionlab-0.0.9/LICENSE` & `fusionlab-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fusionlab-0.0.9/setup.py` & `fusionlab-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     "test": [
         "pytest",
         "mock",
         "pre-commit",
         "black==22.3.0",
         "flake8==4.0.1",
         "flake8-docstrings==1.6.0",
+        "torchvision",
+        "tensorflow",
     ],
 }
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
     with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
```

