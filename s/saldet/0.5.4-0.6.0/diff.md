# Comparing `tmp/saldet-0.5.4.tar.gz` & `tmp/saldet-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saldet-0.5.4.tar", max compression
+gzip compressed data, was "saldet-0.6.0.tar", max compression
```

## Comparing `saldet-0.5.4.tar` & `saldet-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.5.4/LICENSE
--rw-r--r--   0        0        0     4452 2023-05-17 17:43:12.582735 saldet-0.5.4/README.md
--rw-r--r--   0        0        0      917 2023-05-17 17:43:28.129429 saldet-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       68 2023-05-17 17:40:46.932866 saldet-0.5.4/saldet/__init__.py
--rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.5.4/saldet/dataset/__init__.py
--rw-r--r--   0        0        0     2564 2023-05-11 09:06:14.061164 saldet-0.5.4/saldet/dataset/inference.py
--rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.5.4/saldet/dataset/saliency.py
--rw-r--r--   0        0        0       58 2023-05-11 09:06:14.061366 saldet-0.5.4/saldet/experiment/__init__.py
--rw-r--r--   0        0        0     2780 2023-05-17 16:13:05.313542 saldet-0.5.4/saldet/experiment/inference.py
--rw-r--r--   0        0        0     2312 2023-05-17 16:10:40.783399 saldet-0.5.4/saldet/experiment/train.py
--rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.5.4/saldet/io/__init__.py
--rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.5.4/saldet/io/config.py
--rw-r--r--   0        0        0     1873 2023-05-11 09:06:14.061761 saldet-0.5.4/saldet/io/image.py
--rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.5.4/saldet/loss/__init__.py
--rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.5.4/saldet/loss/_factory.py
--rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.5.4/saldet/loss/attn_guided.py
--rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.5.4/saldet/loss/bce_iou_loss.py
--rw-r--r--   0        0        0     1130 2023-05-17 16:56:43.163212 saldet-0.5.4/saldet/loss/multi_bce.py
--rw-r--r--   0        0        0      858 2023-05-17 16:57:23.426213 saldet-0.5.4/saldet/loss/pg.py
--rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.5.4/saldet/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.5.4/saldet/lr_scheduler/lr_scheduler.py
--rw-r--r--   0        0        0       65 2023-05-17 17:43:09.823099 saldet-0.5.4/saldet/model/__init__.py
--rw-r--r--   0        0        0     2424 2023-05-17 17:43:09.733847 saldet-0.5.4/saldet/model/_factory.py
--rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.5.4/saldet/model/models/__init__.py
--rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.5.4/saldet/model/models/pgnet.py
--rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.5.4/saldet/model/models/resnet.py
--rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.5.4/saldet/model/models/swin.py
--rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.5.4/saldet/model/models/u2net.py
--rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.5.4/saldet/ops/__init__.py
--rw-r--r--   0        0        0      930 2023-05-17 15:23:24.394224 saldet-0.5.4/saldet/ops/tensor.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.5.4/saldet/optimizer/__init__.py
--rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.5.4/saldet/optimizer/optimizer.py
--rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.5.4/saldet/pl/__init__.py
--rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.5.4/saldet/pl/data.py
--rw-r--r--   0        0        0     2370 2023-05-16 13:40:17.705235 saldet-0.5.4/saldet/pl/model.py
--rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.5.4/saldet/plot/__init__.py
--rw-r--r--   0        0        0     2597 2023-05-17 16:46:33.116615 saldet-0.5.4/saldet/plot/plot.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.5.4/saldet/trainer/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.5.4/saldet/trainer/callbacks.py
--rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.5.4/saldet/transform/__init__.py
--rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.5.4/saldet/transform/transform.py
--rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.5.4/saldet/utils/__init__.py
--rw-r--r--   0        0        0      225 2023-05-11 09:34:56.451378 saldet-0.5.4/saldet/utils/device.py
--rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.5.4/saldet/utils/time.py
--rw-r--r--   0        0        0     5530 1970-01-01 00:00:00.000000 saldet-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4916 2023-06-02 19:04:58.286355 saldet-0.6.0/README.md
+-rw-r--r--   0        0        0      917 2023-06-02 19:12:28.397873 saldet-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-02 18:45:06.967477 saldet-0.6.0/saldet/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.6.0/saldet/dataset/__init__.py
+-rw-r--r--   0        0        0     2564 2023-05-26 21:45:23.381327 saldet-0.6.0/saldet/dataset/inference.py
+-rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.6.0/saldet/dataset/saliency.py
+-rw-r--r--   0        0        0       58 2023-06-02 18:30:19.301072 saldet-0.6.0/saldet/experiment/__init__.py
+-rw-r--r--   0        0        0     2920 2023-06-02 18:45:34.745533 saldet-0.6.0/saldet/experiment/inference.py
+-rw-r--r--   0        0        0     2312 2023-06-02 17:51:09.638468 saldet-0.6.0/saldet/experiment/train.py
+-rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.6.0/saldet/io/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.6.0/saldet/io/config.py
+-rw-r--r--   0        0        0     1873 2023-05-26 21:46:31.461577 saldet-0.6.0/saldet/io/image.py
+-rw-r--r--   0        0        0      147 2023-06-02 18:45:03.905231 saldet-0.6.0/saldet/loss/__init__.py
+-rw-r--r--   0        0        0      415 2023-06-02 18:45:03.910327 saldet-0.6.0/saldet/loss/_factory.py
+-rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.6.0/saldet/loss/attn_guided.py
+-rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.6.0/saldet/loss/bce_iou_loss.py
+-rw-r--r--   0        0        0     1635 2023-06-02 18:45:03.825497 saldet-0.6.0/saldet/loss/edge_saliency_loss.py
+-rw-r--r--   0        0        0     1130 2023-05-17 16:56:43.163212 saldet-0.6.0/saldet/loss/multi_bce.py
+-rw-r--r--   0        0        0      858 2023-05-17 16:57:23.426213 saldet-0.6.0/saldet/loss/pg.py
+-rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.6.0/saldet/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.6.0/saldet/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0        0        0       65 2023-05-17 17:43:09.823099 saldet-0.6.0/saldet/models/__init__.py
+-rw-r--r--   0        0        0     2457 2023-06-02 18:43:03.889178 saldet-0.6.0/saldet/models/_factory.py
+-rw-r--r--   0        0        0       90 2023-06-02 18:43:55.413439 saldet-0.6.0/saldet/models/models/__init__.py
+-rw-r--r--   0        0        0     9456 2023-06-02 18:44:33.695473 saldet-0.6.0/saldet/models/models/pfan.py
+-rw-r--r--   0        0        0    10194 2023-06-02 18:39:22.910063 saldet-0.6.0/saldet/models/models/pgnet.py
+-rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.6.0/saldet/models/models/resnet.py
+-rw-r--r--   0        0        0    25344 2023-05-26 21:47:34.742688 saldet-0.6.0/saldet/models/models/swin.py
+-rw-r--r--   0        0        0     6809 2023-06-02 18:49:54.482272 saldet-0.6.0/saldet/models/models/u2net.py
+-rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.6.0/saldet/ops/__init__.py
+-rw-r--r--   0        0        0      930 2023-06-02 19:00:54.443854 saldet-0.6.0/saldet/ops/tensor.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.6.0/saldet/optimizer/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.6.0/saldet/optimizer/optimizer.py
+-rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.6.0/saldet/pl/__init__.py
+-rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.6.0/saldet/pl/data.py
+-rw-r--r--   0        0        0     2370 2023-06-02 17:51:50.370703 saldet-0.6.0/saldet/pl/model.py
+-rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.6.0/saldet/plot/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-26 21:47:47.719210 saldet-0.6.0/saldet/plot/plot.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.6.0/saldet/trainer/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-26 21:44:58.032894 saldet-0.6.0/saldet/trainer/callbacks.py
+-rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.6.0/saldet/transform/__init__.py
+-rw-r--r--   0        0        0     3419 2023-05-27 08:17:01.712509 saldet-0.6.0/saldet/transform/transform.py
+-rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.6.0/saldet/utils/__init__.py
+-rw-r--r--   0        0        0      225 2023-06-02 17:43:40.303851 saldet-0.6.0/saldet/utils/device.py
+-rw-r--r--   0        0        0      330 2023-05-26 21:42:57.941431 saldet-0.6.0/saldet/utils/time.py
+-rw-r--r--   0        0        0     5994 1970-01-01 00:00:00.000000 saldet-0.6.0/PKG-INFO
```

### Comparing `saldet-0.5.4/LICENSE` & `saldet-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/README.md` & `saldet-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 # saldet
 > **Sal**iency **Det**ection (*saldet*) is a collection of models and tools to perform Saliency Detection with PyTorch (cuda, mps, etc.).
 
-[![PyPI Version][pypi-image]][pypi-url]
-[![Build Status][build-image]][build-url]
-[![Code Coverage][coverage-image]][coverage-url]
-
-<!-- Badges: -->
-
-[pypi-image]: https://img.shields.io/pypi/v/saldet
-[pypi-url]: https://pypi.org/project/saldet/
-[build-image]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml/badge.svg
-[build-url]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml
-[coverage-image]: https://codecov.io/gh/riccardomusmeci/saldet/branch/main/graph/badge.svg
-[coverage-url]: https://codecov.io/gh/riccardomusmeci/saldet/
+[![PyPI Version](https://img.shields.io/pypi/v/saldet)](https://pypi.org/project/saldet/)
+[![Build Status](https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml/badge.svg)](https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml)
+[![Code Coverage](https://codecov.io/gh/riccardomusmeci/saldet/branch/main/graph/badge.svg)](https://codecov.io/gh/riccardomusmeci/saldet/)
+<!-- [![Documentation Status](https://readthedocs.org/projects/saldet/badge/?version=latest)](https://saldet.readthedocs.io/en/latest/?badge=latest) -->
+
 
 ## **Models**
 List of saliency detection models supported by saldet:
-
 * U2Net - https://arxiv.org/abs/2005.09007v3 ([U2Net repo](https://github.com/xuebinqin/U-2-Net))
 * PGNet - https://arxiv.org/abs/2204.05041 (follow training instructions from [PGNet repo](https://github.com/iCVTEAM/PGNet))
+* PFAN - https://arxiv.org/pdf/1903.00179v2.pdf ([PFAN repo](https://github.com/sairajk/PyTorch-Pyramid-Feature-Attention-Network-for-Saliency-Detection))
 
 ### **Weights**
-* PGNet -> weights from [PGNet's repo](https://github.com/iCVTEAM/PGNet) converted to saldet version from [here](https://drive.google.com/file/d/1gr0lWZoCIucrV5-Z_QV23tUNd8826EjN/view?usp=share_link)
+* PGNet -> weights from [PGNet repo](https://github.com/iCVTEAM/PGNet) converted to saldet version from [here](https://drive.google.com/file/d/1gr0lWZoCIucrV5-Z_QV23tUNd8826EjN/view?usp=share_link)
 * U2Net Lite -> weights from [here](https://drive.google.com/file/d/1rbSTGKAE-MTxBYHd-51l2hMOQPT_7EPy/view?usp=sharing) (U2Net repository)
 * U2Net Full -> weights from [here](https://drive.google.com/file/d/1ao1ovG1Qtx4b7EoskHXmi2E9rp5CHLcZ/view?usp=sharing) (U2Net repository)
 * U2Net Full - Portrait -> weights for portrait images from [here](https://drive.google.com/file/d/1IG3HdpcRiDoWNookbncQjeaPN28t90yW/view) (U2Net repository)
 * U2Net Full - Human Segmentation -> weights for segmenting humans from [here](https://drive.google.com/file/d/1-Yg0cxgrNhHP-016FPdp902BR-kSsA4P/view) (U2Net repository)
+* PFAN -> weights from [PFAN repo](https://github.com/sairajk/PyTorch-Pyramid-Feature-Attention-Network-for-Saliency-Detection) converted to saldet version from [here](https://drive.google.com/file/d/1z6KdZh6arQOE6R30_AxNLvCOLe00dnez/view?usp=share_link)
+
 
 To load pre-trained weights:
 ```python
 from saldet import create_model
-model = create_model("pgnet", checkpoint_path=".../pgnet.pth")
+model = create_model("pgnet", checkpoint_path="PATH/TO/pgnet.pth")
 ```
 
 ## **Train**
 
 ### **Easy Mode**
 The library comes with easy access to train models thanks to the amazing PyTorch Lightning support. 
 
@@ -72,15 +67,16 @@
 ```
 
 ### **PyTorch Lighting Mode**
 The library provides utils for model and data PyTorch Lightning Modules.
 ```python
 import pytorch_lightning as pl
 from saldet import create_model
-from saldet.pl import SaliencyPLDataModule, SaliencyPLModel
+from saldet.pl import
+ SaliencyPLDataModule, SaliencyPLModel
 from saldet.transform import SaliencyTransform
 
 # datamodule
 datamodule = SaliencyPLDataModule(
     root_dir=data_dir,
     train_transform=SaliencyTransform(train=True, **config["transform"]),
     val_transform=SaliencyTransform(train=False, **config["transform"]),
@@ -113,15 +109,16 @@
 from saldet.experiment import inference
 
 inference(
     images_dir=...,
     ckpt=..., # path to ckpt/pth model file
     config_path=..., # path to configuration file from saldet train
     output_dir=..., # where to save saliency maps
+    sigmoid=..., # whether to apply sigmoid to predicted masks
 )
 ```
 
 ## **To-Dos**
 
 [ ] Improve code coverage
 
-[ ] Add new models
+[ ] ReadTheDocs documentation
```

### Comparing `saldet-0.5.4/pyproject.toml` & `saldet-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saldet"
-version = "0.5.4"
+version = "0.6.0"
 description = "Saliency Detection library (models, loss, utils) with PyTorch"
 authors = ["Riccardo Musmeci"]
 repository = "https://github.com/riccardomusmeci/saldet"
 license = "MIT"
 readme = "README.md"
 keywords = ["computer vision", "saliency detection"]
```

### Comparing `saldet-0.5.4/saldet/dataset/inference.py` & `saldet-0.6.0/saldet/dataset/inference.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/dataset/saliency.py` & `saldet-0.6.0/saldet/dataset/saliency.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/experiment/inference.py` & `saldet-0.6.0/saldet/experiment/inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,36 @@
 from PIL import Image
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from saldet import ops
 from saldet.dataset import InferenceDataset
 from saldet.io import load_config
-from saldet.model import load_checkpoint
+from saldet.models import load_checkpoint
 from saldet.transform import SaliencyTransform
 from saldet.utils import device
 
 
 def inference(
     images_dir: Path,
     config_path: Path,
     ckpt: Path,
     output_dir: Path,
+    sigmoid: bool,
     resize_to_original: bool = True,
     threshold: float = None,
 ):
     """Inference entry point - create saliency maps and save them all in an output dir
 
     Args:
         images_dir (Path): path to folder with images
         config_path (Path): path to saldet configuration file
         ckpt (Path): path to model ckpt (.pth or .ckpt from pytorch_lightning)
         output_dir (Path): path to output dir where saliency maps will be saved
+        sigmoid (bool): if True, applies sigmoid to predicted mask.
         resize_to_original (bool, optional): if True, resize_to_original saliency maps. Defaults to True.
         threshold (float, optional): if True, applies a threshold to saliency maps to generate binary saliency maps. Defaults to None.
     """
     config = load_config(path=config_path)
 
     model = load_checkpoint(ckpt=ckpt, model_name=config["model"]["model_name"])
 
@@ -51,24 +53,24 @@
     with torch.no_grad():
         for _, batch in tqdm(
             enumerate(data_loader), total=len(data_loader), desc="Inference"
         ):
             x, image_path = batch
             x = x.to(device())
             preds = model(x)
-            if hasattr(preds, "__iter__"):
+            if isinstance(preds, tuple) or isinstance(preds, list):
                 preds = preds[0]
-            preds = torch.sigmoid(preds)
+            if sigmoid:
+                preds = torch.sigmoid(preds)
             if resize_to_original:
                 w, h = Image.open(image_path[0]).size
                 preds = F.interpolate(preds, size=(h, w), mode="bilinear")
             for pred, image_path in zip(preds, image_path):
                 image_name = os.path.basename(image_path).split(".")[0]
                 file_path = os.path.join(output_dir, f"{image_name}.png")
-
                 if threshold is not None:
                     pred[pred >= threshold] = 255
                     pred[pred < threshold] = 0
                 else:
                     pred *= 255
 
                 pred = pred.squeeze().cpu().numpy()
```

### Comparing `saldet-0.5.4/saldet/experiment/train.py` & `saldet-0.6.0/saldet/experiment/train.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/io/image.py` & `saldet-0.6.0/saldet/io/image.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/loss/attn_guided.py` & `saldet-0.6.0/saldet/loss/attn_guided.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/loss/bce_iou_loss.py` & `saldet-0.6.0/saldet/loss/bce_iou_loss.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/loss/multi_bce.py` & `saldet-0.6.0/saldet/loss/multi_bce.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/loss/pg.py` & `saldet-0.6.0/saldet/loss/pg.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/lr_scheduler/lr_scheduler.py` & `saldet-0.6.0/saldet/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/model/_factory.py` & `saldet-0.6.0/saldet/models/_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 from saldet.pl import SaliencyPLModel
 from saldet.utils import device
 
 from .models import *
 
 __all__ = ["create_model", "load_checkpoint"]
 
-FACTORY = {"u2net_lite": U2NET_lite, "u2net_full": U2NET_full, "pgnet": PGNet}
+FACTORY = {
+    "u2net_lite": U2NET_lite,
+    "u2net_full": U2NET_full,
+    "pgnet": PGNet,
+    "pfan": PFAN,
+}
 
 
 def create_model(model_name: str, checkpoint_path: str = None, **kwargs) -> nn.Module:
     """Create a saliency model
 
     Args:
         model_name (str): model name
```

### Comparing `saldet-0.5.4/saldet/model/models/pgnet.py` & `saldet-0.6.0/saldet/models/models/pgnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/model/models/resnet.py` & `saldet-0.6.0/saldet/models/models/resnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/model/models/swin.py` & `saldet-0.6.0/saldet/models/models/swin.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/model/models/u2net.py` & `saldet-0.6.0/saldet/models/models/u2net.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/ops/tensor.py` & `saldet-0.6.0/saldet/ops/tensor.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/optimizer/optimizer.py` & `saldet-0.6.0/saldet/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/pl/data.py` & `saldet-0.6.0/saldet/pl/data.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/pl/model.py` & `saldet-0.6.0/saldet/pl/model.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/plot/plot.py` & `saldet-0.6.0/saldet/plot/plot.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/trainer/callbacks.py` & `saldet-0.6.0/saldet/trainer/callbacks.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.4/saldet/transform/transform.py` & `saldet-0.6.0/saldet/transform/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 
         if isinstance(mask, Image.Image):
             image = np.array(image)
 
         if mask is not None:
             sample = self.transform(image=image, mask=mask)
             image, mask = sample["image"], sample["mask"]
-
         else:
             image = self.transform(image=image)["image"]
             mask = None
 
         image = torch.from_numpy(image.transpose(2, 0, 1))
         if mask is not None:
             mask = torch.from_numpy(mask).long()
```

### Comparing `saldet-0.5.4/PKG-INFO` & `saldet-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saldet
-Version: 0.5.4
+Version: 0.6.0
 Summary: Saliency Detection library (models, loss, utils) with PyTorch
 Home-page: https://github.com/riccardomusmeci/saldet
 License: MIT
 Keywords: computer vision,saliency detection
 Author: Riccardo Musmeci
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -24,44 +24,39 @@
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/riccardomusmeci/saldet
 Description-Content-Type: text/markdown
 
 # saldet
 > **Sal**iency **Det**ection (*saldet*) is a collection of models and tools to perform Saliency Detection with PyTorch (cuda, mps, etc.).
 
-[![PyPI Version][pypi-image]][pypi-url]
-[![Build Status][build-image]][build-url]
-[![Code Coverage][coverage-image]][coverage-url]
-
-<!-- Badges: -->
-
-[pypi-image]: https://img.shields.io/pypi/v/saldet
-[pypi-url]: https://pypi.org/project/saldet/
-[build-image]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml/badge.svg
-[build-url]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml
-[coverage-image]: https://codecov.io/gh/riccardomusmeci/saldet/branch/main/graph/badge.svg
-[coverage-url]: https://codecov.io/gh/riccardomusmeci/saldet/
+[![PyPI Version](https://img.shields.io/pypi/v/saldet)](https://pypi.org/project/saldet/)
+[![Build Status](https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml/badge.svg)](https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml)
+[![Code Coverage](https://codecov.io/gh/riccardomusmeci/saldet/branch/main/graph/badge.svg)](https://codecov.io/gh/riccardomusmeci/saldet/)
+<!-- [![Documentation Status](https://readthedocs.org/projects/saldet/badge/?version=latest)](https://saldet.readthedocs.io/en/latest/?badge=latest) -->
+
 
 ## **Models**
 List of saliency detection models supported by saldet:
-
 * U2Net - https://arxiv.org/abs/2005.09007v3 ([U2Net repo](https://github.com/xuebinqin/U-2-Net))
 * PGNet - https://arxiv.org/abs/2204.05041 (follow training instructions from [PGNet repo](https://github.com/iCVTEAM/PGNet))
+* PFAN - https://arxiv.org/pdf/1903.00179v2.pdf ([PFAN repo](https://github.com/sairajk/PyTorch-Pyramid-Feature-Attention-Network-for-Saliency-Detection))
 
 ### **Weights**
-* PGNet -> weights from [PGNet's repo](https://github.com/iCVTEAM/PGNet) converted to saldet version from [here](https://drive.google.com/file/d/1gr0lWZoCIucrV5-Z_QV23tUNd8826EjN/view?usp=share_link)
+* PGNet -> weights from [PGNet repo](https://github.com/iCVTEAM/PGNet) converted to saldet version from [here](https://drive.google.com/file/d/1gr0lWZoCIucrV5-Z_QV23tUNd8826EjN/view?usp=share_link)
 * U2Net Lite -> weights from [here](https://drive.google.com/file/d/1rbSTGKAE-MTxBYHd-51l2hMOQPT_7EPy/view?usp=sharing) (U2Net repository)
 * U2Net Full -> weights from [here](https://drive.google.com/file/d/1ao1ovG1Qtx4b7EoskHXmi2E9rp5CHLcZ/view?usp=sharing) (U2Net repository)
 * U2Net Full - Portrait -> weights for portrait images from [here](https://drive.google.com/file/d/1IG3HdpcRiDoWNookbncQjeaPN28t90yW/view) (U2Net repository)
 * U2Net Full - Human Segmentation -> weights for segmenting humans from [here](https://drive.google.com/file/d/1-Yg0cxgrNhHP-016FPdp902BR-kSsA4P/view) (U2Net repository)
+* PFAN -> weights from [PFAN repo](https://github.com/sairajk/PyTorch-Pyramid-Feature-Attention-Network-for-Saliency-Detection) converted to saldet version from [here](https://drive.google.com/file/d/1z6KdZh6arQOE6R30_AxNLvCOLe00dnez/view?usp=share_link)
+
 
 To load pre-trained weights:
 ```python
 from saldet import create_model
-model = create_model("pgnet", checkpoint_path=".../pgnet.pth")
+model = create_model("pgnet", checkpoint_path="PATH/TO/pgnet.pth")
 ```
 
 ## **Train**
 
 ### **Easy Mode**
 The library comes with easy access to train models thanks to the amazing PyTorch Lightning support. 
 
@@ -99,15 +94,16 @@
 ```
 
 ### **PyTorch Lighting Mode**
 The library provides utils for model and data PyTorch Lightning Modules.
 ```python
 import pytorch_lightning as pl
 from saldet import create_model
-from saldet.pl import SaliencyPLDataModule, SaliencyPLModel
+from saldet.pl import
+ SaliencyPLDataModule, SaliencyPLModel
 from saldet.transform import SaliencyTransform
 
 # datamodule
 datamodule = SaliencyPLDataModule(
     root_dir=data_dir,
     train_transform=SaliencyTransform(train=True, **config["transform"]),
     val_transform=SaliencyTransform(train=False, **config["transform"]),
@@ -140,16 +136,17 @@
 from saldet.experiment import inference
 
 inference(
     images_dir=...,
     ckpt=..., # path to ckpt/pth model file
     config_path=..., # path to configuration file from saldet train
     output_dir=..., # where to save saliency maps
+    sigmoid=..., # whether to apply sigmoid to predicted masks
 )
 ```
 
 ## **To-Dos**
 
 [ ] Improve code coverage
 
-[ ] Add new models
+[ ] ReadTheDocs documentation
```

