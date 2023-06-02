# Comparing `tmp/kaparoo_lightning_package-0.2.0.tar.gz` & `tmp/kaparoo_lightning_package-0.2.1.tar.gz`

## Comparing `kaparoo_lightning_package-0.2.0.tar` & `kaparoo_lightning_package-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/common/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/common/types.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/__init__.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/constants.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/datamodules.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/datasets.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/utils.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/nn/__init__.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/nn/gan.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/LICENSE
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/README.md
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/common/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/common/types.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/data/__init__.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/data/constants.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/data/datamodules.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/data/datasets.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/data/utils.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/nn/__init__.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/kaparoo_lightning/nn/gan.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/README.md
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.1/PKG-INFO
```

### Comparing `kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/__init__.py` & `kaparoo_lightning_package-0.2.1/kaparoo_lightning/data/__init__.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/datamodules.py` & `kaparoo_lightning_package-0.2.1/kaparoo_lightning/data/datamodules.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/datasets.py` & `kaparoo_lightning_package-0.2.1/kaparoo_lightning/data/datasets.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/utils.py` & `kaparoo_lightning_package-0.2.1/kaparoo_lightning/data/utils.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.2.0/kaparoo_lightning/nn/gan.py` & `kaparoo_lightning_package-0.2.1/kaparoo_lightning/nn/gan.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,13 +15,15 @@
 
 
 class GAN(LightningModule):
     def __init__(self) -> None:
         super().__init__()
         self.automatic_optimization = False
 
-    def get_labels(self, preds: Tensor, as_real: bool = True) -> Tensor:
+    @classmethod
+    def get_labels(cls, preds: Tensor, as_real: bool = True) -> Tensor:
         return torch.ones_like(preds) if as_real else torch.zeros_like(preds)
 
-    def adversarial_loss(self, preds: Tensor, as_real: bool = True) -> Tensor:
-        labels = self.get_labels(preds, as_real)
+    @classmethod
+    def adversarial_loss(cls, preds: Tensor, as_real: bool = True) -> Tensor:
+        labels = cls.get_labels(preds, as_real)
         return F.binary_cross_entropy(preds, labels)
```

### Comparing `kaparoo_lightning_package-0.2.0/.gitignore` & `kaparoo_lightning_package-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.2.0/LICENSE` & `kaparoo_lightning_package-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.2.0/README.md` & `kaparoo_lightning_package-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.2.0/pyproject.toml` & `kaparoo_lightning_package-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.2.0/PKG-INFO` & `kaparoo_lightning_package-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-lightning-package
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package for (personally) common and useful features for PyTorch Lightning.
 Project-URL: GitHub, https://www.github.com/kaparoo/lightning-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
```

