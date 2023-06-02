# Comparing `tmp/torchility-0.7.2.tar.gz` & `tmp/torchility-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.7.2.tar", last modified: Sat May 27 15:22:26 2023, max compression
+gzip compressed data, was "torchility-0.7.3.tar", last modified: Fri Jun  2 07:24:35 2023, max compression
```

## Comparing `torchility-0.7.2.tar` & `torchility-0.7.3.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.484918 torchility-0.7.2/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.2/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2119 2023-05-27 15:22:26.483681 torchility-0.7.2/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1640 2023-05-27 07:50:27.000000 torchility-0.7.2/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.434146 torchility-0.7.2/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1872 2023-05-27 07:45:07.000000 torchility-0.7.2/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.2/examples/10-model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.2/examples/11-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2073 2023-05-27 07:49:20.000000 torchility-0.7.2/examples/2-metrics_basic.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.2/examples/3-metrics_more.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.2/examples/4-callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.2/examples/5-lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.2/examples/6-optimizer.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.2/examples/7-interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.2/examples/8-multi_dataloaders.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.2/examples/9-reset_train_dataloader.py
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-27 15:22:26.485550 torchility-0.7.2/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.2/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.442169 torchility-0.7.2/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-27 15:22:03.000000 torchility-0.7.2/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.467400 torchility-0.7.2/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.2/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.2/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.2/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.2/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)     9796 2023-05-27 15:05:14.000000 torchility-0.7.2/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.2/torchility/datamodule.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.2/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.2/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6693 2023-05-27 15:21:51.000000 torchility-0.7.2/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5695 2023-05-23 02:30:35.000000 torchility-0.7.2/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 15:21:26.000000 torchility-0.7.2/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.479521 torchility-0.7.2/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       96 2023-05-15 04:51:01.000000 torchility-0.7.2/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2647 2023-05-21 03:41:57.000000 torchility-0.7.2/torchility/utils/metric_utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.2/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.2/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.7.2/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.450385 torchility-0.7.2/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2119 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      979 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.732027 torchility-0.7.3/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.3/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2215 2023-06-02 07:24:35.731440 torchility-0.7.3/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1736 2023-05-28 14:40:21.000000 torchility-0.7.3/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.707110 torchility-0.7.3/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1873 2023-05-28 13:25:54.000000 torchility-0.7.3/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.3/examples/10-model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.3/examples/11-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2625 2023-05-28 13:29:46.000000 torchility-0.7.3/examples/2-metrics_basic.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.3/examples/3-metrics_more.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.3/examples/4-callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.3/examples/5-lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.3/examples/6-optimizer.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.3/examples/7-interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.3/examples/8-multi_dataloaders.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.3/examples/9-reset_train_dataloader.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.708698 torchility-0.7.3/imgs/
+-rw-r--r--   0 liuchen    (501) staff       (20)   119040 2023-05-28 14:38:16.000000 torchility-0.7.3/imgs/data_flow.png
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-06-02 07:24:35.732350 torchility-0.7.3/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.3/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.717083 torchility-0.7.3/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-06-02 07:24:15.000000 torchility-0.7.3/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.727469 torchility-0.7.3/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.3/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.3/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.3/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.3/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     9796 2023-05-27 15:05:14.000000 torchility-0.7.3/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.3/torchility/datamodule.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.3/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.3/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6732 2023-06-02 07:24:04.000000 torchility-0.7.3/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5695 2023-05-23 02:30:35.000000 torchility-0.7.3/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 15:21:26.000000 torchility-0.7.3/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.730782 torchility-0.7.3/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)       97 2023-05-28 01:59:22.000000 torchility-0.7.3/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2647 2023-05-21 03:41:57.000000 torchility-0.7.3/torchility/utils/metric_utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.3/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.3/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.7.3/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.723794 torchility-0.7.3/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2215 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)      998 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.7.2/LICENSE` & `torchility-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/PKG-INFO` & `torchility-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.2
+Version: 0.7.3
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -28,14 +28,22 @@
 - torchmetrics>=0.11,<0.12
 - matplotlib>=3.3
 - pyyaml>=5.4
 - tensorboardX>=2.6
 
 ## Usage
 
+### Data Flow
+
+<center>
+    <img src="imgs/data_flow.png" width="60%"/>
+</center>
+
+### Example
+
 - MNIST
 
 ```python
 from torchility import Trainer
 import torch
 from torch import nn
 from torch.nn import functional as F
```

### Comparing `torchility-0.7.2/README.md` & `torchility-0.7.3/examples/5-lr_find.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,46 @@
-# torchility
-
-A tool for training pytorch deep learning model more simply which is based on Pytorch-lightning.
-
-## Install
-
-- `pip install torchility`
-### Dependency
-- pytorch>=2.0
-- pytorch-lightning>=2.0,<2.1
-- torchmetrics>=0.11,<0.12
-- matplotlib>=3.3
-- pyyaml>=5.4
-- tensorboardX>=2.6
-
-## Usage
-
-- MNIST
-
-```python
-from torchility import Trainer
 import torch
 from torch import nn
 from torch.nn import functional as F
 from torchvision.datasets import MNIST
 from torchvision import transforms
 from torch.utils.data import DataLoader, random_split
+from torchility import Trainer
+from torchility.callbacks import LRFinder
+import matplotlib.pyplot as plt
 import warnings
-warnings.simplefilter("ignore")  # ignore annoying warnings
+warnings.simplefilter("ignore")
+
 
-# datasets
+# 1. --- 数据
 data_dir = './datasets'
 transform = transforms.Compose([transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))])
 mnist_full = MNIST(data_dir, train=True, transform=transform, download=True)
 train_ds, val_ds = random_split(mnist_full, [55000, 5000])
 test_ds = MNIST(data_dir, train=False, transform=transform, download=True)
-
-# dataloaders
 train_dl = DataLoader(train_ds, batch_size=32)
 val_dl = DataLoader(val_ds, batch_size=32)
 test_dl = DataLoader(test_ds, batch_size=32)
 
-# pytorch model
+
+# 2. --- 模型
 channels, width, height = (1, 28, 28)
 model = nn.Sequential(
     nn.Flatten(),
     nn.Linear(channels * width * height, 64),
     nn.ReLU(),
     nn.Dropout(0.1),
     nn.Linear(64, 64),
     nn.ReLU(),
     nn.Dropout(0.1),
     nn.Linear(64, 10)
 )
 
-# optimizer
+
+# 3. --- 优化器
 opt = torch.optim.Adam(model.parameters(), lr=2e-4)
-# trainer
-trainer = Trainer(model, F.cross_entropy, opt, epochs=2)
-# train and validate
-trainer.fit(train_dl, val_dl)
-# test
-trainer.test(test_dl)
-```
 
-- See the `examples` for more examples 
+
+# 4. --- 训练
+trainer = Trainer(model, F.cross_entropy, opt,          # 训练器，使用LRFinder
+                  epochs=2, callbacks=[LRFinder(max_batch=100)])  
+trainer.fit(train_dl)                                   # 训练、验证
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchility-0.7.2/examples/1-mnist.py` & `torchility-0.7.3/examples/1-mnist.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # 1. --- 数据
 data_dir = './datasets'
 transform = transforms.Compose([transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))])
 mnist_full = MNIST(data_dir, train=True, transform=transform, download=True)
 train_ds, val_ds = random_split(mnist_full, [55000, 5000])
 test_ds = MNIST(data_dir, train=False, transform=transform, download=True)
+
 train_dl = DataLoader(train_ds, batch_size=32)
 val_dl = DataLoader(val_ds, batch_size=32)
 test_dl = DataLoader(test_ds, batch_size=32)
 
 # 2. --- 模型
 channels, width, height = (1, 28, 28)
 model = nn.Sequential(
```

### Comparing `torchility-0.7.2/examples/10-model_analysis.py` & `torchility-0.7.3/examples/10-model_analysis.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/examples/11-graph_node_clasification_DGL.py` & `torchility-0.7.3/examples/11-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/examples/2-metrics_basic.py` & `torchility-0.7.3/examples/4-callbacks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,24 @@
+from pytorch_lightning.callbacks import ModelCheckpoint, EarlyStopping
 from torchility import Trainer
 from torch.utils.data import DataLoader, random_split
 from torchvision import transforms
 from torchvision.datasets import MNIST
 from torch.nn import functional as F
-from torchmetrics import Accuracy
 from torch import nn
 import torch
 import warnings
 
 warnings.simplefilter("ignore")
 
 # 1. --- 数据
 data_dir = './datasets'
 transform = transforms.Compose([transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))])
 mnist_full = MNIST(data_dir, train=True, transform=transform, download=True)
-# train_ds, val_ds = random_split(mnist_full, [55000, 5000])
-train_ds, val_ds, _ = random_split(mnist_full, [5000, 5000, 50000])
-
+train_ds, val_ds = random_split(mnist_full, [55000, 5000])
 test_ds = MNIST(data_dir, train=False, transform=transform, download=True)
 train_dl = DataLoader(train_ds, batch_size=32)
 val_dl = DataLoader(val_ds, batch_size=32)
 test_dl = DataLoader(test_ds, batch_size=32)
 
 
 # 2. --- 模型
@@ -38,28 +36,22 @@
 
 
 # 3. --- 优化器
 opt = torch.optim.Adam(model.parameters(), lr=2e-4)
 
 
 # 4. --- 训练
-acc = 'acc', Accuracy(task='multiclass', num_classes=10)
-acc1 = 'acc1', Accuracy(task='multiclass', average='macro', num_classes=10)
-
-def acc2(preds, targets):
-    preds = preds.argmax(1)
-    return (preds == targets).float().mean()
-
-def acc3(preds, targets):
-    """同时计算多个指标"""
-    preds = preds.argmax(1)
-    return {'a':(preds == targets).float().mean(), 'b':(preds == targets).float().mean()}
-
-trainer = Trainer(model, F.cross_entropy, opt, epochs=10,
-                  metrics=[acc, acc1, acc2, acc3],    # 指定计算指标，默认在train、val和test中都会计算
-                  val_frac=2                          # 每2个epoch做一次验证
-                  )
-progress = trainer.fit(train_dl, val_dl)              # 训练、验证
 
-trainer.test(test_dl)                                 # 测试
+# 早停callback
+early_stop_cbk = EarlyStopping(monitor='val_loss', min_delta=0.00, patience=3, verbose=False, mode='min')
+# 模型checkpoint callback
+model_cbk = ModelCheckpoint(save_top_k=1, monitor='val_loss', mode='min')
+
+# 训练器，使用新的进度条，以及其他callbacks
+trainer = Trainer(model, F.cross_entropy, opt, epochs=2,
+                  callbacks=[
+                                model_cbk,
+                                early_stop_cbk
+                            ])
+trainer.fit(train_dl, val_dl)
 
-print(progress)
+trainer.test(test_dl)
```

### Comparing `torchility-0.7.2/examples/3-metrics_more.py` & `torchility-0.7.3/examples/3-metrics_more.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/examples/4-callbacks.py` & `torchility-0.7.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,74 @@
-from pytorch_lightning.callbacks import ModelCheckpoint, EarlyStopping
+# torchility
+
+A tool for training pytorch deep learning model more simply which is based on Pytorch-lightning.
+
+## Install
+
+- `pip install torchility`
+### Dependency
+- pytorch>=2.0
+- pytorch-lightning>=2.0,<2.1
+- torchmetrics>=0.11,<0.12
+- matplotlib>=3.3
+- pyyaml>=5.4
+- tensorboardX>=2.6
+
+## Usage
+
+### Data Flow
+
+<center>
+    <img src="imgs/data_flow.png" width="60%"/>
+</center>
+
+### Example
+
+- MNIST
+
+```python
 from torchility import Trainer
-from torch.utils.data import DataLoader, random_split
-from torchvision import transforms
-from torchvision.datasets import MNIST
-from torch.nn import functional as F
-from torch import nn
 import torch
+from torch import nn
+from torch.nn import functional as F
+from torchvision.datasets import MNIST
+from torchvision import transforms
+from torch.utils.data import DataLoader, random_split
 import warnings
+warnings.simplefilter("ignore")  # ignore annoying warnings
 
-warnings.simplefilter("ignore")
-
-# 1. --- 数据
+# datasets
 data_dir = './datasets'
 transform = transforms.Compose([transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))])
 mnist_full = MNIST(data_dir, train=True, transform=transform, download=True)
 train_ds, val_ds = random_split(mnist_full, [55000, 5000])
 test_ds = MNIST(data_dir, train=False, transform=transform, download=True)
+
+# dataloaders
 train_dl = DataLoader(train_ds, batch_size=32)
 val_dl = DataLoader(val_ds, batch_size=32)
 test_dl = DataLoader(test_ds, batch_size=32)
 
-
-# 2. --- 模型
+# pytorch model
 channels, width, height = (1, 28, 28)
 model = nn.Sequential(
     nn.Flatten(),
     nn.Linear(channels * width * height, 64),
     nn.ReLU(),
     nn.Dropout(0.1),
     nn.Linear(64, 64),
     nn.ReLU(),
     nn.Dropout(0.1),
     nn.Linear(64, 10)
 )
 
-
-# 3. --- 优化器
+# optimizer
 opt = torch.optim.Adam(model.parameters(), lr=2e-4)
-
-
-# 4. --- 训练
-
-# 早停callback
-early_stop_cbk = EarlyStopping(monitor='val_loss', min_delta=0.00, patience=3, verbose=False, mode='min')
-# 模型checkpoint callback
-model_cbk = ModelCheckpoint(save_top_k=1, monitor='val_loss', mode='min')
-
-# 训练器，使用新的进度条，以及其他callbacks
-trainer = Trainer(model, F.cross_entropy, opt, epochs=2,
-                  callbacks=[
-                                model_cbk,
-                                early_stop_cbk
-                            ])
+# trainer
+trainer = Trainer(model, F.cross_entropy, opt, epochs=2)
+# train and validate
 trainer.fit(train_dl, val_dl)
-
+# test
 trainer.test(test_dl)
+```
+
+- See the `examples` for more examples
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `torchility-0.7.2/examples/5-lr_find.py` & `torchility-0.7.3/examples/6-optimizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import torch
-from torch import nn
-from torch.nn import functional as F
-from torchvision.datasets import MNIST
-from torchvision import transforms
-from torch.utils.data import DataLoader, random_split
 from torchility import Trainer
-from torchility.callbacks import LRFinder
-import matplotlib.pyplot as plt
+from torch.utils.data import DataLoader, random_split
+from torchvision import transforms
+from torchvision.datasets import MNIST
+from torch.nn import functional as F
+from torch import nn
+import torch
 import warnings
-warnings.simplefilter("ignore")
 
+warnings.simplefilter("ignore")
 
 # 1. --- 数据
 data_dir = './datasets'
 transform = transforms.Compose([transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))])
 mnist_full = MNIST(data_dir, train=True, transform=transform, download=True)
 train_ds, val_ds = random_split(mnist_full, [55000, 5000])
 test_ds = MNIST(data_dir, train=False, transform=transform, download=True)
@@ -34,13 +32,24 @@
     nn.Dropout(0.1),
     nn.Linear(64, 10)
 )
 
 
 # 3. --- 优化器
 opt = torch.optim.Adam(model.parameters(), lr=2e-4)
+scheduler = torch.optim.lr_scheduler.StepLR(opt, 8, gamma=0.1, last_epoch=-1)
+
+opt_tuple = (opt, scheduler)
 
+opt_dict = {
+        'optimizer': opt,
+        'lr_scheduler': scheduler
+      }
 
 # 4. --- 训练
-trainer = Trainer(model, F.cross_entropy, opt,          # 训练器，使用LRFinder
-                  epochs=2, callbacks=[LRFinder(max_batch=100)])  
-trainer.fit(train_dl)                                   # 训练、验证
+trainer = Trainer(model, F.cross_entropy, opt_tuple, epochs=10)
+# 或者
+# trainer = Trainer(model, F.cross_entropy, opt_dict, epochs=10)
+trainer.fit(train_dl, val_dl)               # 训练、验证
+
+
+trainer.test(test_dl)                       # 测试
```

### Comparing `torchility-0.7.2/examples/7-interpreter.py` & `torchility-0.7.3/examples/7-interpreter.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/examples/8-multi_dataloaders.py` & `torchility-0.7.3/examples/8-multi_dataloaders.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/examples/9-reset_train_dataloader.py` & `torchility-0.7.3/examples/9-reset_train_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/setup.py` & `torchility-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/callbacks/common.py` & `torchility-0.7.3/torchility/callbacks/common.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/callbacks/interpreters.py` & `torchility-0.7.3/torchility/callbacks/interpreters.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/callbacks/performances.py` & `torchility-0.7.3/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/callbacks/progress.py` & `torchility-0.7.3/torchility/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/datamodule.py` & `torchility-0.7.3/torchility/datamodule.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/hooks.py` & `torchility-0.7.3/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/losses.py` & `torchility-0.7.3/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/metrics.py` & `torchility-0.7.3/torchility/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import torch
 from .utils import rename, concat, get_batch_size
 import torch.nn.functional as F
 import numpy as np
 from copy import deepcopy
 
 
+class MetricNotUpdated(Exception):
+    pass
+
+
 class MetricBase:
     """
     torchility评价指标的使用方式有如下三种：
     （1）torchmetrics.Metric的子类，包括torchmetrics中提供的各种指标。
         如果模型输出结果比较复杂，可重写forward方法，先预处理再调用父类forward方法。
     （2）自定义指标。继承MetricBase，指标的计算方法可以以metric_fn参数传入，或者重写forward方法。
         如果模型输出结果比较复杂，可重写prepare方法预处理。
@@ -76,17 +80,17 @@
     def reset(self):
         self.pred_batchs = []
         self.target_batchs = []
         self.cumulate_size = 0
         self.cumulate_value = None
 
     def compute(self):
-        if self.cumulate_size == 0 or self.cumulate_value is None:
-            raise Exception("This metric have not updated!") # pylint: disable=W0719
         if self.simple_cumulate:
+            if self.cumulate_size == 0 or self.cumulate_value is None:
+                raise MetricNotUpdated("The metric have not been updated!")
             if isinstance(self.cumulate_value, dict):
                 return {k: v/self.cumulate_size for k, v in self.cumulate_value.items()}
             else:
                 return self.cumulate_value / self.cumulate_size
         else:
             if len(self.pred_batchs) == 0 and len(self.pred_batchs) == 0:
                 return 0.0000
@@ -94,16 +98,14 @@
             target_epoch = concat(self.target_batchs)
             return self.metric_fn(pred_epoch, target_epoch)
 
     def clone(self):
         return deepcopy(self)
 
 
-
-
 @rename('acc')
 def accuracy(out, yb):
     return (torch.argmax(out, dim=1) == yb).float().mean()
 
 
 @rename('acc')
 def masked_accuracy(preds, targets):
```

### Comparing `torchility-0.7.2/torchility/tasks.py` & `torchility-0.7.3/torchility/tasks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/trainer.py` & `torchility-0.7.3/torchility/trainer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/utils/metric_utils.py` & `torchility-0.7.3/torchility/utils/metric_utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/utils/plots.py` & `torchility-0.7.3/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/utils/utils.py` & `torchility-0.7.3/torchility/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility/utils/yaml_config.py` & `torchility-0.7.3/torchility/utils/yaml_config.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.2/torchility.egg-info/PKG-INFO` & `torchility-0.7.3/torchility.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.2
+Version: 0.7.3
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -28,14 +28,22 @@
 - torchmetrics>=0.11,<0.12
 - matplotlib>=3.3
 - pyyaml>=5.4
 - tensorboardX>=2.6
 
 ## Usage
 
+### Data Flow
+
+<center>
+    <img src="imgs/data_flow.png" width="60%"/>
+</center>
+
+### Example
+
 - MNIST
 
 ```python
 from torchility import Trainer
 import torch
 from torch import nn
 from torch.nn import functional as F
```

### Comparing `torchility-0.7.2/torchility.egg-info/SOURCES.txt` & `torchility-0.7.3/torchility.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 examples/3-metrics_more.py
 examples/4-callbacks.py
 examples/5-lr_find.py
 examples/6-optimizer.py
 examples/7-interpreter.py
 examples/8-multi_dataloaders.py
 examples/9-reset_train_dataloader.py
+imgs/data_flow.png
 torchility/__init__.py
 torchility/datamodule.py
 torchility/hooks.py
 torchility/losses.py
 torchility/metrics.py
 torchility/tasks.py
 torchility/trainer.py
```

