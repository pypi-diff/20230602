# Comparing `tmp/kaparoo_lightning_package-0.1.0.tar.gz` & `tmp/kaparoo_lightning_package-0.2.0.tar.gz`

## Comparing `kaparoo_lightning_package-0.1.0.tar` & `kaparoo_lightning_package-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/common/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/common/types.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/data/__init__.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/data/constants.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/data/datamodules.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/data/utils.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/models/__init__.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/kaparoo_lightning/models/gan.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/LICENSE
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/README.md
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/common/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/common/types.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/__init__.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/constants.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/datamodules.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/datasets.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/utils.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/nn/__init__.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/kaparoo_lightning/nn/gan.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/README.md
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 kaparoo_lightning_package-0.2.0/PKG-INFO
```

### Comparing `kaparoo_lightning_package-0.1.0/kaparoo_lightning/data/datamodules.py` & `kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/datamodules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 
 __all__ = ("DataModule",)
 
 from typing import Any, Generic
 
+from beartype import beartype
+from kaparoo.beartype import NonNegInt, PosInt
 from kaparoo.utils import unwrap_or_default
 from kaparoo.utils.types import T_co
 from lightning import LightningDataModule
 from torch.utils.data import DataLoader, Dataset
 from typing_extensions import LiteralString
 
 from kaparoo_lightning.data.constants import BATCH_SIZE, NUM_WORKERS
@@ -39,25 +41,26 @@
         return isinstance(self.dataset_pred, Dataset)
 
     def __str__(self) -> LiteralString:
         return self.__class__.__name__
 
 
 class DataModule(DataModuleBase[T_co]):
+    @beartype
     def __init__(
         self,
-        batch_size: int = BATCH_SIZE,
-        num_workers: int = NUM_WORKERS,
+        batch_size: PosInt = BATCH_SIZE,
+        num_workers: NonNegInt = NUM_WORKERS,
         shuffle: bool = True,
         *,
         # for `Dataset`
-        max_trains: int | None = None,
-        max_valids: int | None = None,
-        max_tests: int | None = None,
-        max_preds: int | None = None,
+        max_trains: NonNegInt | None = None,
+        max_valids: NonNegInt | None = None,
+        max_tests: NonNegInt | None = None,
+        max_preds: NonNegInt | None = None,
         # for `DataLoader`
         dataloader_spec: DataLoaderSpec | None = None,
         train_loader_spec: DataLoaderSpec | None = None,
         valid_loader_spec: DataLoaderSpec | None = None,
         test_loader_spec: DataLoaderSpec | None = None,
         pred_loader_spec: DataLoaderSpec | None = None,
     ) -> None:
```

### Comparing `kaparoo_lightning_package-0.1.0/kaparoo_lightning/data/utils.py` & `kaparoo_lightning_package-0.2.0/kaparoo_lightning/data/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 __all__ = ("DataLoaderSpec", "update_dataloader_spec")
 
 from collections.abc import Iterable, Sequence
 from typing import Any, TypedDict
 
+from beartype import beartype
 from kaparoo.utils import unwrap_or_default
 from torch.utils.data import Sampler
 from torch.utils.data.dataloader import _collate_fn_t, _worker_init_fn_t
 
 
 class DataLoaderSpec(TypedDict, total=False):
     batch_size: int
@@ -26,13 +27,14 @@
     multiprocessing_context: Any
     generator: Any
     prefetch_factor: int
     persistent_workers: bool
     pin_memory_device: str
 
 
+@beartype
 def update_dataloader_spec(
     default: DataLoaderSpec, optional: DataLoaderSpec | None
 ) -> DataLoaderSpec:
     optional = unwrap_or_default(optional, {})
     # false positive error by mypy (see issue #4122)
     return {**default, **optional}  # type: ignore[misc]
```

### Comparing `kaparoo_lightning_package-0.1.0/kaparoo_lightning/models/gan.py` & `kaparoo_lightning_package-0.2.0/kaparoo_lightning/nn/gan.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.1.0/.gitignore` & `kaparoo_lightning_package-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.1.0/LICENSE` & `kaparoo_lightning_package-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.1.0/README.md` & `kaparoo_lightning_package-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning_package-0.1.0/pyproject.toml` & `kaparoo_lightning_package-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Typing :: Typed",
 ]
 dependencies = [
     "lightning>=2.0",
-    "kaparoo-python-package>=0.2.3",
+    "kaparoo-python-package>=0.3.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "hatch>=1.7.0",
     "ruff>=0.0.270",
     "mypy>=1.3.0",
```

### Comparing `kaparoo_lightning_package-0.1.0/PKG-INFO` & `kaparoo_lightning_package-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-lightning-package
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package for (personally) common and useful features for PyTorch Lightning.
 Project-URL: GitHub, https://www.github.com/kaparoo/lightning-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
         
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
-Requires-Dist: kaparoo-python-package>=0.2.3
+Requires-Dist: kaparoo-python-package>=0.3.0
 Requires-Dist: lightning>=2.0
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: hatch>=1.7.0; extra == 'dev'
 Requires-Dist: mypy>=1.3.0; extra == 'dev'
 Requires-Dist: pytest>=7.3.1; extra == 'dev'
 Requires-Dist: ruff>=0.0.270; extra == 'dev'
```

