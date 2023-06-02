# Comparing `tmp/tacv-1.1.5.tar.gz` & `tmp/tacv-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tacv-1.1.5.tar", last modified: Fri Apr 21 03:50:37 2023, max compression
+gzip compressed data, was "tacv-1.1.6.tar", last modified: Fri Jun  2 03:26:12 2023, max compression
```

## Comparing `tacv-1.1.5.tar` & `tacv-1.1.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/
--rw-rw-r--   0 tu        (1000) tu        (1000)     1065 2022-07-26 16:30:33.000000 tacv-1.1.5/LICENSE
--rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2023-04-21 03:50:37.357515 tacv-1.1.5/PKG-INFO
--rw-rw-r--   0 tu        (1000) tu        (1000)     6908 2022-07-29 02:23:53.000000 tacv-1.1.5/README.md
--rw-rw-r--   0 tu        (1000) tu        (1000)      105 2022-07-26 16:30:33.000000 tacv-1.1.5/pyproject.toml
--rw-rw-r--   0 tu        (1000) tu        (1000)       32 2022-07-26 16:30:33.000000 tacv-1.1.5/requirements.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)      200 2023-04-21 03:50:37.357515 tacv-1.1.5/setup.cfg
--rw-rw-r--   0 tu        (1000) tu        (1000)     1838 2023-04-21 03:50:30.000000 tacv-1.1.5/setup.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.353515 tacv-1.1.5/tacv/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/cli/
--rw-rw-r--   0 tu        (1000) tu        (1000)       63 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/cli/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      206 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/cli/cli.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/
--rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-28 14:56:31.000000 tacv-1.1.5/tacv/detection/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/
--rw-rw-r--   0 tu        (1000) tu        (1000)     9698 2022-07-29 02:23:53.000000 tacv-1.1.5/tacv/detection/centernet/CenterNet.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     4429 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/Trainer.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      130 2022-07-28 14:56:31.000000 tacv-1.1.5/tacv/detection/centernet/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/backbones/
--rw-rw-r--   0 tu        (1000) tu        (1000)      100 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/backbones/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)    10067 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/backbones/resnet.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/heads/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/heads/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/losses/
--rw-rw-r--   0 tu        (1000) tu        (1000)       35 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/losses/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     1363 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/losses/losses.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/utils/
--rw-rw-r--   0 tu        (1000) tu        (1000)       90 2022-07-28 14:56:31.000000 tacv-1.1.5/tacv/detection/centernet/utils/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      261 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/common.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     2448 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/data_utils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     3031 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/geometry_utils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     2345 2022-07-29 02:21:21.000000 tacv-1.1.5/tacv/detection/centernet/utils/infer.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      189 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/lightning_utils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/pytorch_model_utils.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/fileUtils/
--rw-rw-r--   0 tu        (1000) tu        (1000)       72 2023-04-21 02:49:52.000000 tacv-1.1.5/tacv/fileUtils/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     1577 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/fileUtils/fileutils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     5615 2023-04-21 03:48:04.000000 tacv-1.1.5/tacv/fileUtils/thread_downloader.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/geometry/
--rw-rw-r--   0 tu        (1000) tu        (1000)       18 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/geometry/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      782 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/geometry/iou.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/resources/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/resources/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/torch/
--rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/torch/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     1046 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/torch/model_utils.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/video/
--rw-rw-r--   0 tu        (1000) tu        (1000)       25 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/video/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     2710 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/video/video_proc.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/visual/
--rw-rw-r--   0 tu        (1000) tu        (1000)       21 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/visual/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      558 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/visual/draw2d.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv.egg-info/
--rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/PKG-INFO
--rw-rw-r--   0 tu        (1000) tu        (1000)     1281 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/SOURCES.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)        1 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/dependency_links.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)       92 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/entry_points.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)       33 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/requires.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)        5 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/top_level.txt
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.551066 tacv-1.1.6/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1065 2022-07-26 16:30:33.000000 tacv-1.1.6/LICENSE
+-rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2023-06-02 03:26:12.551066 tacv-1.1.6/PKG-INFO
+-rw-rw-r--   0 tu        (1000) tu        (1000)     6908 2022-07-29 02:23:53.000000 tacv-1.1.6/README.md
+-rw-rw-r--   0 tu        (1000) tu        (1000)      105 2022-07-26 16:30:33.000000 tacv-1.1.6/pyproject.toml
+-rw-rw-r--   0 tu        (1000) tu        (1000)       32 2022-07-26 16:30:33.000000 tacv-1.1.6/requirements.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)      200 2023-06-02 03:26:12.551066 tacv-1.1.6/setup.cfg
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1838 2023-06-02 03:25:44.000000 tacv-1.1.6/setup.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/cli/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       63 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/cli/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      206 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/cli/cli.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-28 14:56:31.000000 tacv-1.1.6/tacv/detection/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     9698 2022-07-29 02:23:53.000000 tacv-1.1.6/tacv/detection/centernet/CenterNet.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     4429 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/Trainer.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      130 2022-07-28 14:56:31.000000 tacv-1.1.6/tacv/detection/centernet/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/backbones/
+-rw-rw-r--   0 tu        (1000) tu        (1000)      100 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/backbones/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)    10067 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/backbones/resnet.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/heads/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/heads/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/losses/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       35 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/losses/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1363 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/losses/losses.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/utils/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       90 2022-07-28 14:56:31.000000 tacv-1.1.6/tacv/detection/centernet/utils/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      261 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/common.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2448 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/data_utils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     3031 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/geometry_utils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2345 2022-07-29 02:21:21.000000 tacv-1.1.6/tacv/detection/centernet/utils/infer.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      189 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/lightning_utils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/pytorch_model_utils.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/fileUtils/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       72 2023-04-21 02:49:52.000000 tacv-1.1.6/tacv/fileUtils/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1577 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/fileUtils/fileutils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     5573 2023-06-02 03:21:52.000000 tacv-1.1.6/tacv/fileUtils/thread_downloader.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/geometry/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       18 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/geometry/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      782 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/geometry/iou.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/resources/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/resources/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.551066 tacv-1.1.6/tacv/torch/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/torch/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1046 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/torch/model_utils.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.551066 tacv-1.1.6/tacv/video/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       25 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/video/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2710 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/video/video_proc.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.551066 tacv-1.1.6/tacv/visual/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       21 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/visual/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      558 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/visual/draw2d.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv.egg-info/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/PKG-INFO
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1281 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/SOURCES.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)        1 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/dependency_links.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)       92 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/entry_points.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)       33 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/requires.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)        5 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/top_level.txt
```

### Comparing `tacv-1.1.5/LICENSE` & `tacv-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/PKG-INFO` & `tacv-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tacv
-Version: 1.1.5
+Version: 1.1.6
 Summary: A mini package for daily tasks
 Home-page: https://github.com/TaQuangTu/TaCV
 Author: TaQuangTu
 Author-email: taquangtu132@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tacv-1.1.5/README.md` & `tacv-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/setup.py` & `tacv-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r") as f:
     lines = f.readlines()
     required_pkgs = [item.strip() for item in lines]
 
 # version_file = "tacv/resources/version.txt"
-new_ver = "1.1.5"  # increase_version_by_one(version_file)
+new_ver = "1.1.6"  # increase_version_by_one(version_file)
 print(f"Building {new_ver}")
 setup(
     name='tacv',
     version=new_ver,
     packages=setuptools.find_packages(where="."),
     url='https://github.com/TaQuangTu/TaCV',
     license='LICENSE',
```

### Comparing `tacv-1.1.5/tacv/detection/centernet/CenterNet.py` & `tacv-1.1.6/tacv/detection/centernet/CenterNet.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/detection/centernet/Trainer.py` & `tacv-1.1.6/tacv/detection/centernet/Trainer.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/detection/centernet/backbones/resnet.py` & `tacv-1.1.6/tacv/detection/centernet/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/detection/centernet/losses/losses.py` & `tacv-1.1.6/tacv/detection/centernet/losses/losses.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/detection/centernet/utils/data_utils.py` & `tacv-1.1.6/tacv/detection/centernet/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/detection/centernet/utils/geometry_utils.py` & `tacv-1.1.6/tacv/detection/centernet/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/detection/centernet/utils/infer.py` & `tacv-1.1.6/tacv/detection/centernet/utils/infer.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/fileUtils/fileutils.py` & `tacv-1.1.6/tacv/fileUtils/fileutils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/fileUtils/thread_downloader.py` & `tacv-1.1.6/tacv/fileUtils/thread_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import threading
 import sys, os, re
 import time
 from queue import Queue
 from urllib.request import urlopen
 
-from attr.validators import instance_of
-
 
 class ThreadedDownload(object):
     REGEX = {
         'hostname_strip': re.compile('.*\..*?/', re.I)
     }
 
     class MissingDirectoryException(Exception):
@@ -119,15 +117,15 @@
         elif self.directory_structure == True:
             # Strip off hostname, keep all other directories
             file_destination = '%s%s' % (self.destination, ThreadedDownload.REGEX['hostname_strip'].sub('', url))
 
         elif hasattr(self.directory_structure, '__len__') and len(self.directory_structure) == 2:
             # User supplied a custom regex replace
             regex = self.directory_structure[0]
-            if instance_of(regex, str):
+            if isinstance(regex, str):
                 regex = re.compile(str)
             replace = self.directory_structure[1]
             file_destination = '%s%s' % (self.destination, regex.sub(replace, url))
 
         else:
             # No idea what's wanted
             file_destination = None
```

### Comparing `tacv-1.1.5/tacv/geometry/iou.py` & `tacv-1.1.6/tacv/geometry/iou.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/torch/model_utils.py` & `tacv-1.1.6/tacv/torch/model_utils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/video/video_proc.py` & `tacv-1.1.6/tacv/video/video_proc.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv/visual/draw2d.py` & `tacv-1.1.6/tacv/visual/draw2d.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.5/tacv.egg-info/PKG-INFO` & `tacv-1.1.6/tacv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tacv
-Version: 1.1.5
+Version: 1.1.6
 Summary: A mini package for daily tasks
 Home-page: https://github.com/TaQuangTu/TaCV
 Author: TaQuangTu
 Author-email: taquangtu132@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tacv-1.1.5/tacv.egg-info/SOURCES.txt` & `tacv-1.1.6/tacv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

