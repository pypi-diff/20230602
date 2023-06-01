# Comparing `tmp/traker-0.1.3.tar.gz` & `tmp/traker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traker-0.1.3.tar", last modified: Wed Apr 19 18:30:35 2023, max compression
+gzip compressed data, was "traker-0.2.0.tar", last modified: Thu Jun  1 22:52:49 2023, max compression
```

## Comparing `traker-0.1.3.tar` & `traker-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-19 18:30:35.829877 traker-0.1.3/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-04-19 18:30:35.825877 traker-0.1.3/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3338 2023-04-19 18:30:13.000000 traker-0.1.3/README.md
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-04-19 18:30:35.833877 traker-0.1.3/setup.cfg
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      756 2023-04-19 18:30:13.000000 traker-0.1.3/setup.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-19 18:30:35.649875 traker-0.1.3/tests/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     5575 2023-04-12 13:40:47.000000 traker-0.1.3/tests/test_accuracy.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     2989 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_cifar_accuracy.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4143 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_class.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4571 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_integration_cifar.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1545 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_integration_clip.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    10812 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_jl.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4065 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_parallel.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3116 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_rademacher.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-19 18:30:35.749876 traker-0.1.3/trak/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       72 2023-04-19 18:30:13.000000 traker-0.1.3/trak/__init__.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     8766 2023-04-18 20:47:31.000000 traker-0.1.3/trak/gradient_computers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    20281 2023-04-18 20:47:31.000000 traker-0.1.3/trak/modelout_functions.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11180 2023-04-18 20:47:31.000000 traker-0.1.3/trak/projectors.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    12660 2023-04-18 20:47:31.000000 traker-0.1.3/trak/savers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3499 2023-04-18 20:47:31.000000 traker-0.1.3/trak/score_computers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    18787 2023-04-19 18:30:13.000000 traker-0.1.3/trak/traker.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1527 2023-04-18 20:47:31.000000 traker-0.1.3/trak/utils.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-19 18:30:35.809877 traker-0.1.3/traker.egg-info/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      525 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/SOURCES.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/dependency_links.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       96 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/requires.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        5 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/top_level.txt
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-01 22:52:49.283594 traker-0.2.0/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-06-01 22:52:49.275594 traker-0.2.0/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3338 2023-04-19 18:30:13.000000 traker-0.2.0/README.md
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-06-01 22:52:49.283594 traker-0.2.0/setup.cfg
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      757 2023-06-01 22:51:27.000000 traker-0.2.0/setup.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-01 22:52:49.107592 traker-0.2.0/tests/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4681 2023-06-01 22:51:27.000000 traker-0.2.0/tests/test_cifar10_accuracy.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3344 2023-06-01 22:51:27.000000 traker-0.2.0/tests/test_cifar2_accuracy.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11693 2023-06-01 22:51:28.000000 traker-0.2.0/tests/test_class.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1898 2023-06-01 22:51:28.000000 traker-0.2.0/tests/test_integration_cifar.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1540 2023-06-01 22:51:28.000000 traker-0.2.0/tests/test_integration_clip.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    10812 2023-04-18 20:47:31.000000 traker-0.2.0/tests/test_jl.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11501 2023-06-01 22:51:28.000000 traker-0.2.0/tests/test_parallel.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3116 2023-04-18 20:47:31.000000 traker-0.2.0/tests/test_rademacher.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-01 22:52:49.207593 traker-0.2.0/trak/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      105 2023-06-01 22:51:28.000000 traker-0.2.0/trak/__init__.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     8187 2023-06-01 22:51:28.000000 traker-0.2.0/trak/gradient_computers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    16829 2023-06-01 22:51:28.000000 traker-0.2.0/trak/modelout_functions.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    12251 2023-06-01 22:51:28.000000 traker-0.2.0/trak/projectors.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    15993 2023-06-01 22:51:29.000000 traker-0.2.0/trak/savers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3880 2023-06-01 22:51:29.000000 traker-0.2.0/trak/score_computers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    21812 2023-06-01 22:51:29.000000 traker-0.2.0/trak/traker.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3019 2023-06-01 22:51:29.000000 traker-0.2.0/trak/utils.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-01 22:52:49.263594 traker-0.2.0/traker.egg-info/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      534 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/SOURCES.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/dependency_links.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       97 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/requires.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        5 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/top_level.txt
```

### Comparing `traker-0.1.3/README.md` & `traker-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `traker-0.1.3/setup.py` & `traker-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(name="traker",
-      version="0.1.3",
+      version="0.2.0",
       description="TRAK: Attributing Model Behavior at Scale",
       long_description="Check https://trak.csail.mit.edu/ to learn more about TRAK",
       author="MadryLab",
       author_email='trak@mit.edu',
       license_files=('LICENSE.txt', ),
       packages=['trak'],
       install_requires=[
-       "torch>=1.13",
+       "torch>=2.0.0",
        "numpy",
        "tqdm",
        ],
       extras_require={
           'tests':
               ["assertpy",
                "torchvision",
```

### Comparing `traker-0.1.3/tests/test_accuracy.py` & `traker-0.2.0/tests/test_cifar10_accuracy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from tqdm import tqdm
 from pathlib import Path
 from itertools import product
-from scipy.stats import spearmanr
+import logging
 import pytest
 import torch
 import torchvision
-import numpy as np
 
 from trak import TRAKer
 from trak.projectors import BasicProjector
 
-from .utils import construct_rn9
+from .utils import construct_rn9, download_cifar_checkpoints, eval_correlations
 
 
 ch = torch
 
 
 def get_dataloader(batch_size=256, num_workers=8, split='train', shuffle=False, augment=True):
     if augment:
@@ -40,108 +39,82 @@
                                          shuffle=shuffle,
                                          batch_size=batch_size,
                                          num_workers=num_workers)
 
     return loader
 
 
-def eval_correlations(infls, tmp_path):
-
-    masks_path = Path('/mnt/cfs/projects/better_tracin/eval_margins/CIFAR10/50pct/mask.npy')
-    # num masks, num train samples
-    masks = ch.as_tensor(np.load(masks_path, mmap_mode='r')).float()
-
-    margins_path = Path('/mnt/cfs/projects/better_tracin/eval_margins/CIFAR10/50pct/val_margins.npy')
-    # num , num val samples
-    margins = ch.as_tensor(np.load(margins_path, mmap_mode='r'))
-
-    val_inds = np.arange(2000)
-    preds = masks @ infls
-    rs = []
-    ps = []
-    for ind, j in tqdm(enumerate(val_inds)):
-        r, p = spearmanr(preds[:, ind], margins[:, j])
-        rs.append(r)
-        ps.append(p)
-    rs, ps = np.array(rs), np.array(ps)
-    print(f'Correlation: {rs.mean()} (avg p value {ps.mean()})')
-    return rs.mean()
-
-
 def get_projector(use_cuda_projector, dtype):
     if use_cuda_projector:
         return None
-    return BasicProjector(grad_dim=2274880, proj_dim=4096,
+    return BasicProjector(grad_dim=2274880, proj_dim=2048,
                           seed=0, proj_type='normal', block_size=400,
                           dtype=dtype, device='cuda:0')
 
 
-PARAM = list(product([True],  # serialize
+# reduce the number of tests for CIFAR-10
+PARAM = list(product([False],  # serialize
                      [True],  # basic / cuda projector
                      [ch.float16],  # projection dtype
-                     [100],  # batch size
+                     [128],  # batch size
                      ))
 
 
 @pytest.mark.parametrize("serialize, use_cuda_projector, dtype, batch_size", PARAM)
 @pytest.mark.cuda
 def test_cifar_acc(serialize, use_cuda_projector, dtype, batch_size, tmp_path):
     device = 'cuda:0'
     projector = get_projector(use_cuda_projector, dtype)
     model = construct_rn9(10).to(memory_format=ch.channels_last).to(device)
     model = model.eval()
 
     loader_train = get_dataloader(batch_size=batch_size, split='train', augment=False)
     loader_val = get_dataloader(batch_size=batch_size, split='val', augment=False)
 
-    #  = Path(tmp_path).joinpath('cifar_ckpts')
-    # ckpt_files = download_cifar_checkpoints(CKPT_PATH)
-
-    # ckpt_files = sorted(list(Path('/mnt/xfs/home/krisgrg/projects/trak/examples/checkpoints_1').rglob('*.pt')))
-    ckpt_files = sorted(list(Path('/mnt/xfs/home/krisgrg/projects/trak/examples/checkpoints').rglob('*.pt')))
+    CKPT_PATH = Path(tmp_path).joinpath('cifar_ckpts')
+    ckpt_files = download_cifar_checkpoints(CKPT_PATH)
 
     ckpts = [ch.load(ckpt, map_location='cpu') for ckpt in ckpt_files]
 
     traker = TRAKer(model=model,
                     task='image_classification',
                     projector=projector,
-                    proj_dim=4096,
                     train_set_size=50_000,
                     save_dir=tmp_path,
+                    logging_level=logging.DEBUG,
                     device=device)
 
-    print('GRAD DIM:', traker.projector.grad_dim)
-    # print('jl matrix:', traker.projector.proj_matrix)
-
     for model_id, ckpt in enumerate(ckpts):
         traker.load_checkpoint(checkpoint=ckpt, model_id=model_id)
         for batch in tqdm(loader_train, desc='Computing TRAK embeddings...'):
             batch = [x.cuda() for x in batch]
             traker.featurize(batch=batch, num_samples=len(batch[0]))
 
     traker.finalize_features()
 
-    # print('jl matrix:', traker.projector.proj_matrix)
-
     if serialize:
         del traker
         traker = TRAKer(model=model,
                         task='image_classification',
                         projector=projector,
-                        proj_dim=4096,
                         train_set_size=50_000,
                         save_dir=tmp_path,
+                        logging_level=logging.DEBUG,
                         device=device)
 
     for model_id, ckpt in enumerate(ckpts):
-        traker.start_scoring_checkpoint(ckpt, model_id, num_targets=10_000)
+        traker.start_scoring_checkpoint(exp_name='test_experiment',
+                                        checkpoint=ckpt,
+                                        model_id=model_id,
+                                        num_targets=10_000)
         for batch in tqdm(loader_val, desc='Scoring...'):
             batch = [x.cuda() for x in batch]
             traker.score(batch=batch, num_samples=len(batch[0]))
 
-    scores = traker.finalize_scores().cpu()
+    print(traker.saver.experiments)
 
-    avg_corr = eval_correlations(infls=scores, tmp_path=tmp_path)
-    assert avg_corr > 0.062, 'correlation with 3 CIFAR-2 models should be >= 0.062'
+    scores = traker.finalize_scores(exp_name='test_experiment')
+    print(scores)
+    print(scores.shape)
 
-    # self.scores = (_scores / _num_models_used)
-    # print('NO OUT-TO-LOSS GRADS')
+    avg_corr = eval_correlations(infls=scores, tmp_path=tmp_path)
+    assert avg_corr > 0.05, 'correlation with the above 3 CIFAR-10 checkpoints should be >= 0.05'
```

### Comparing `traker-0.1.3/tests/test_cifar_accuracy.py` & `traker-0.2.0/tests/test_cifar2_accuracy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from tqdm import tqdm
 from pathlib import Path
 from itertools import product
+import logging
 import pytest
 import torch as ch
 
 from trak import TRAKer
 from trak.projectors import BasicProjector
 
 from .utils import construct_rn9, get_dataloader, eval_correlations
@@ -26,35 +27,41 @@
                      ))
 
 
 @pytest.mark.parametrize("serialize, use_cuda_projector, dtype, batch_size", PARAM)
 @pytest.mark.cuda
 def test_cifar_acc(serialize, use_cuda_projector, dtype, batch_size, tmp_path):
     device = 'cuda:0'
+    exp_name = 'test_experimet'
+
     projector = get_projector(use_cuda_projector, dtype)
     model = construct_rn9().to(memory_format=ch.channels_last).to(device)
     model = model.eval()
 
     BETONS_PATH = Path(tmp_path).joinpath('cifar_betons')
     BETONS = download_cifar_betons(BETONS_PATH)
 
     loader_train = get_dataloader(BETONS, batch_size=batch_size, split='train')
     loader_val = get_dataloader(BETONS, batch_size=batch_size, split='val')
 
     CKPT_PATH = Path(tmp_path).joinpath('cifar_ckpts')
-    ckpt_files = download_cifar_checkpoints(CKPT_PATH)
+    ckpt_files = download_cifar_checkpoints(CKPT_PATH, 'cifar2')
     ckpts = [ch.load(ckpt, map_location='cpu') for ckpt in ckpt_files]
 
+    use_half_precision = (dtype == ch.float16)
+
     traker = TRAKer(model=model,
                     task='image_classification',
                     projector=projector,
                     proj_dim=1024,
                     train_set_size=10_000,
                     save_dir=tmp_path,
-                    device=device)
+                    device=device,
+                    logging_level=logging.DEBUG,
+                    use_half_precision=use_half_precision)
 
     for model_id, ckpt in enumerate(ckpts):
         traker.load_checkpoint(checkpoint=ckpt, model_id=model_id)
         for batch in tqdm(loader_train, desc='Computing TRAK embeddings...'):
             traker.featurize(batch=batch, num_samples=len(batch[0]))
 
     traker.finalize_features()
@@ -63,18 +70,20 @@
         del traker
         traker = TRAKer(model=model,
                         task='image_classification',
                         projector=projector,
                         proj_dim=1024,
                         train_set_size=10_000,
                         save_dir=tmp_path,
-                        device=device)
+                        device=device,
+                        logging_level=logging.DEBUG,
+                        use_half_precision=use_half_precision)
 
     for model_id, ckpt in enumerate(ckpts):
-        traker.start_scoring_checkpoint(ckpt, model_id, num_targets=2_000)
+        traker.start_scoring_checkpoint(exp_name, ckpt, model_id, num_targets=2_000)
         for batch in tqdm(loader_val, desc='Scoring...'):
             traker.score(batch=batch, num_samples=len(batch[0]))
 
-    scores = traker.finalize_scores().cpu()
+    scores = traker.finalize_scores(exp_name)
 
-    avg_corr = eval_correlations(infls=scores, tmp_path=tmp_path)
+    avg_corr = eval_correlations(infls=scores, tmp_path=tmp_path, ds='cifar2')
     assert avg_corr > 0.062, 'correlation with 3 CIFAR-2 models should be >= 0.062'
```

### Comparing `traker-0.1.3/tests/test_integration_clip.py` & `traker-0.2.0/tests/test_integration_clip.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-import pytest
 from tqdm import tqdm
 from torchvision import datasets
-import open_clip
-
 from trak import TRAKer
-# from trak.gradient_computers import IterativeGradientComputer
+import logging
+import pytest
+import open_clip
 
 
 @pytest.mark.cuda
 def test_mscoco(tmp_path, device='cuda:0'):
     model, _, preprocess = open_clip.create_model_and_transforms('RN50')
     model = model.to(device)
     model.eval()
 
     tokenizer = open_clip.get_tokenizer('RN50')
 
-    ds_train = datasets.CocoCaptions(root='/path/to/coco_csv/train2014',
-                                     annFile='/path/to/coco_csv/coco_train_karpathy.json'
+    ds_train = datasets.CocoCaptions(root='/path/to/coco2014/images/train2014',
+                                     annFile='/path/to/coco2014/annotations/annotations/captions_train2014.json'
                                      )
 
     traker = TRAKer(model=model,
                     task='clip',
                     save_dir=tmp_path,
                     train_set_size=len(ds_train),
                     device=device,
                     proj_dim=512,
+                    logging_level=logging.DEBUG
                     )
 
-    traker.modelout_fn.get_embeddings(model, ds_train, batch_size=1, size=600,
-                                      preprocess_fn_img=lambda x: preprocess(x).to(device).unsqueeze(0),
-                                      preprocess_fn_txt=lambda x: tokenizer(x[0]).to(device))
+    traker.task.get_embeddings(model, ds_train, batch_size=1, size=600, embedding_dim=1024,
+                               preprocess_fn_img=lambda x: preprocess(x).to(device).unsqueeze(0),
+                               preprocess_fn_txt=lambda x: tokenizer(x[0]).to(device))
 
     traker.load_checkpoint(model.state_dict(), model_id=0)
     for bind, (img, captions) in enumerate(tqdm(ds_train)):
         x = preprocess(img).to(device).unsqueeze(0)
         # selecting (wlog) the first out of 5 captions
         y = tokenizer(captions[0]).to(device)
 
         traker.featurize(batch=(x, y), num_samples=x.shape[0])
         if bind == 2:
             break
-
-    traker.finalize_features()
```

### Comparing `traker-0.1.3/tests/test_jl.py` & `traker-0.2.0/tests/test_jl.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.3/tests/test_rademacher.py` & `traker-0.2.0/tests/test_rademacher.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.3/trak/gradient_computers.py` & `traker-0.2.0/trak/gradient_computers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Iterable, Optional
 from torch import Tensor
-from .utils import parameters_to_vector, vectorize_and_ignore_buffers, get_params_dict
+from .utils import vectorize, get_num_params, parameters_to_vector
 from .modelout_functions import AbstractModelOutput
 import torch
 ch = torch
-try:
-    from functorch import grad, vmap, make_functional_with_buffers
-except ImportError:
-    print('Cannot import `functorch`. Functional mode cannot be used.')
 
 
 class AbstractGradientComputer(ABC):
     """ Implementations of the GradientComputer class should allow for
     per-sample gradients.  This is behavior is enabled with three methods:
 
     - the :meth:`.load_model_params` method, well, loads model parameters. It can
@@ -21,108 +17,108 @@
     - the :meth:`.compute_per_sample_grad` method computes per-sample gradients
       of the chosen model output function with respect to the model's parameters.
 
     - the :meth:`.compute_loss_grad` method computes the gradients of the loss
       function with respect to the model output (which should be a scalar) for
       every sample.
 
-    The class attribute :code:`is_functional` is used to determine what
-    implementation of ModelOutput to use, i.e. whether it should use
-    :code:`functorch`'s functional models.
     """
-    is_functional = True
 
     @abstractmethod
     def __init__(self,
                  model: torch.nn.Module,
-                 modelout_fn: AbstractModelOutput,
+                 task: AbstractModelOutput,
                  grad_dim: Optional[int] = None,
                  ) -> None:
         """ Initializes attributes, nothing too interesting happening.
 
         Args:
             model (torch.nn.Module):
                 model
-            modelout_fn (AbstractModelOutput):
-                model output function
+            task (AbstractModelOutput):
+                task (model output function)
             grad_dim (int, optional):
                 Size of the gradients (number of model parameters). Defaults to
                 None.
 
         """
         self.model = model
-        self.modelout_fn = modelout_fn()
+        self.modelout_fn = task
         self.grad_dim = grad_dim
 
     @abstractmethod
     def load_model_params(self, model) -> None:
         ...
 
     @abstractmethod
-    def compute_per_sample_grad(self, batch: Iterable[Tensor], batch_size: int) -> Tensor:
+    def compute_per_sample_grad(self, batch: Iterable[Tensor]) -> Tensor:
         ...
 
     @abstractmethod
     def compute_loss_grad(self, batch: Iterable[Tensor], batch_size: int) -> Tensor:
         ...
 
 
 class FunctionalGradientComputer(AbstractGradientComputer):
     def __init__(self,
                  model: torch.nn.Module,
-                 modelout_fn: AbstractModelOutput,
+                 task: AbstractModelOutput,
                  grad_dim: int) -> None:
-        super().__init__(model, modelout_fn, grad_dim)
+        super().__init__(model, task, grad_dim)
+        self.model = model
+        self.num_params = get_num_params(self.model)
         self.load_model_params(model)
 
     def load_model_params(self, model) -> None:
-        """ Given a a torch.nn.Module model, inits/updates the func_model, along
-        with its weights and buffers. See
-        https://pytorch.org/functorch/stable/generated/functorch.make_functional_with_buffers.html#functorch-make-functional-with-buffers
-        for more details on `functorch`'s functional models.
+        """ Given a a torch.nn.Module model, inits/updates the (functional)
+        weights and buffers. See https://pytorch.org/docs/stable/func.html
+        for more details on :code:`torch.func`'s functional models.
 
         Args:
             model (torch.nn.Module):
                 model to load
 
         """
-        self.func_model, self.func_weights, self.func_buffers = make_functional_with_buffers(model)
-        self.params_dict = get_params_dict(model)
+        self.func_weights = dict(model.named_parameters())
+        self.func_buffers = dict(model.named_buffers())
 
-    def compute_per_sample_grad(self,
-                                batch: Iterable[Tensor],
-                                batch_size: Optional[int] = None,
-                                ) -> Tensor:
+    def compute_per_sample_grad(self, batch: Iterable[Tensor]) -> Tensor:
         """ Uses functorch's :code:`vmap` (see
         https://pytorch.org/functorch/stable/generated/functorch.vmap.html#functorch.vmap
         for more details) to vectorize the computations of per-sample gradients.
 
         Doesn't use :code:`batch_size`; only added to follow the abstract method
         signature.
 
         Args:
             batch (Iterable[Tensor]):
                 batch of data
-            batch_size (int, optional):
-                Defaults to None.
 
         Returns:
             Tensor:
                 gradients of the model output function of each sample in the
                 batch with respect to the model's parameters.
 
         """
         # taking the gradient wrt weights (second argument of get_output, hence argnums=1)
-        grads_loss = grad(self.modelout_fn.get_output, has_aux=False, argnums=1)
+        grads_loss = torch.func.grad(self.modelout_fn.get_output, has_aux=False, argnums=1)
         # map over batch dimensions (hence 0 for each batch dimension, and None for model params)
-        grads = vmap(grads_loss,
-                     in_dims=(None, None, None, *([0] * len(batch))),
-                     randomness='different')(self.func_model, self.func_weights,
-                                             self.func_buffers, *batch)
-        return vectorize_and_ignore_buffers(grads, self.params_dict)
+        grads = torch.empty(size=(batch[0].shape[0], self.num_params),
+                            dtype=batch[0].dtype,
+                            device=batch[0].device)
+
+        vectorize(torch.func.vmap(grads_loss,
+                                  in_dims=(None, None, None, *([0] * len(batch))),
+                                  randomness='different')(self.model,
+                                                          self.func_weights,
+                                                          self.func_buffers,
+                                                          *batch),
+                  grads)
+
+        return grads
 
     def compute_loss_grad(self, batch: Iterable[Tensor]) -> Tensor:
         """Computes the gradient of the loss with respect to the model output
 
         .. math::
 
             \\partial \\ell / \\partial \\text{(model output)}
@@ -141,85 +137,69 @@
             ...
 
         Args:
             batch (Iterable[Tensor]):
                 batch of data
 
         """
-        return self.modelout_fn.get_out_to_loss_grad(self.func_model,
+        return self.modelout_fn.get_out_to_loss_grad(self.model,
                                                      self.func_weights,
                                                      self.func_buffers,
                                                      batch)
 
 
 class IterativeGradientComputer(AbstractGradientComputer):
-    is_functional = False
-
     def __init__(self,
                  model,
-                 modelout_fn: AbstractModelOutput,
+                 task: AbstractModelOutput,
                  grad_dim: int) -> None:
-        super().__init__(model, modelout_fn, grad_dim)
+        super().__init__(model, task, grad_dim)
         self.load_model_params(model)
 
     def load_model_params(self, model) -> Tensor:
         self.model = model
         self.model_params = list(self.model.parameters())
 
-    def compute_per_sample_grad(self,
-                                batch: Iterable[Tensor],
-                                batch_size: int,
-                                ) -> Tensor:
+    def compute_per_sample_grad(self, batch: Iterable[Tensor]) -> Tensor:
         """ Computes per-sample gradients of the model output function This
         method does not leverage vectorization (and is hence much slower than
         its equivalent in :class:`.FunctionalGradientComputer`). We recommend
-        that you use this only if :code:`functorch` is not available to you,
-        e.g. you have a (very) old version of pytorch.
-
+        that you use this only if :code:`torch.func` is not available to you,
+        e.g. if you have a (very) old version of pytorch.
         Args:
             batch (Iterable[Tensor]):
                 batch of data
-            batch_size (int, optional):
-                Defaults to None.
-
         Returns:
             Tensor:
                 gradients of the model output function of each sample in the
                 batch with respect to the model's parameters.
-
         """
+        batch_size = batch[0].shape[0]
         grads = ch.zeros(batch_size, self.grad_dim).to(batch[0].device)
 
         margin = self.modelout_fn.get_output(self.model, *batch)
         for ind in range(batch_size):
             grads[ind] = parameters_to_vector(ch.autograd.grad(margin[ind],
                                                                self.model_params,
                                                                retain_graph=True))
         return grads
 
     def compute_loss_grad(self, batch: Iterable[Tensor]) -> Tensor:
         """Computes the gradient of the loss with respect to the model output
-
         .. math::
-
             \\partial \\ell / \\partial \\text{(model output)}
-
         Note: For all applications we considered, we analytically derived the
         out-to-loss gradient, thus avoiding the need to do any backward passes
         (let alone per-sample grads). If for your application this is not feasible,
         you'll need to subclass this and modify this method to have a structure
         similar to the one of :meth:`.IterativeGradientComputer.get_output`,
         i.e. something like:
-
         .. code-block:: python
-
             out_to_loss = self.model_out_to_loss(...)
             for ind in range(batch_size):
                 grads[ind] = torch.autograd.grad(out_to_loss[ind], ...)
             ...
-
         Args:
             batch (Iterable[Tensor]):
                 batch of data
-
         """
         return self.modelout_fn.get_out_to_loss_grad(self.model, batch)
```

### Comparing `traker-0.1.3/trak/modelout_functions.py` & `traker-0.2.0/trak/modelout_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
-Here we provide an abstract "model output" class AbstractModelOutput, together with a number
-of subclasses for particular applications (vision, language, etc):
+Here we provide an abstract "model output" class AbstractModelOutput, together
+with a number of subclasses for particular applications (vision, language, etc):
 
 - :class:`.ImageClassificationModelOutput`
-- :class:`.IterImageClassificationModelOutput`
 - :class:`.CLIPModelOutput`
 - :class:`.TextClassificationModelOutput`
 
-These classes implement methods that transform input batches to the desired model output
-(e.g. logits, loss, etc).
-See Sections 2 & 3 of `our paper <https://arxiv.org/abs/2303.14186>`_ for more
-details on what model output functions are in the context of TRAK and how to use
-& design them.
-
-See, e.g. `this tutorial <https://trak.readthedocs.io/en/latest/clip.html>`_ for an
-example on how to subclass :code:`AbstractModelOutput` for a task of your
-choice.
+These classes implement methods that transform input batches to the desired
+model output (e.g. logits, loss, etc).  See Sections 2 & 3 of `our paper
+<https://arxiv.org/abs/2303.14186>`_ for more details on what model output
+functions are in the context of TRAK and how to use & design them.
+
+See, e.g. `this tutorial
+<https://trak.readthedocs.io/en/latest/modeloutput.html>`_ for an example on how
+to subclass :code:`AbstractModelOutput` for a task of your choice.
 """
 from abc import ABC, abstractmethod
 from typing import Iterable
 from torch import Tensor
 from torch.nn import Module
 import torch as ch
 
@@ -98,190 +96,91 @@
             softmax for the out-to-loss function. Defaults to 1.
         """
         super().__init__()
         self.softmax = ch.nn.Softmax(-1)
         self.loss_temperature = temperature
 
     @staticmethod
-    def get_output(func_model,
+    def get_output(model: Module,
                    weights: Iterable[Tensor],
                    buffers: Iterable[Tensor],
                    image: Tensor,
                    label: Tensor) -> Tensor:
         """ For a given input :math:`z=(x, y)` and model parameters :math:`\\theta`,
         let :math:`p(z, \\theta)` be the softmax probability of the correct class.
         This method implements the model output function
 
         .. math::
 
             \\log(\\frac{p(z, \\theta)}{1 - p(z, \\theta)}).
 
-        It uses functorch's functional models to make the per-sample gradient computations faster.
-        For more details on what func_model, weights & buffers are, and how to use them, please
-        refer to https://pytorch.org/functorch/stable/ and
+        It uses functional models from torch.func (previously functorch) to make
+        the per-sample gradient computations (much) faster. For more details on
+        what functional models are, and how to use them, please refer to
+        https://pytorch.org/docs/stable/func.html and
         https://pytorch.org/functorch/stable/notebooks/per_sample_grads.html.
 
-        Note: this method slightly breaks abstraction since it has a different
-        signature from the abstract :code:`get_output`. It's only used
-        internally by :func:`GradientComputer` so it shouldn't be a big problem.
-        If you're reading this and feel strongly about it, feel free to make a
-        PR with a fix.
-
         Args:
-            func_model (func):
-                functorch functional model
+            model (torch.nn.Module):
+                torch model
             weights (Iterable[Tensor]):
                 functorch model weights
             buffers (Iterable[Tensor]):
                 functorch model buffers
             image (Tensor):
                 input image, should not have batch dimension
             label (Tensor):
                 input label, should not have batch dimension
 
         Returns:
             Tensor:
                 model output for the given image-label pair :math:`z` and
                 weights & buffers :math:`\\theta`.
         """
-        logits = func_model(weights, buffers, image.unsqueeze(0))
+        logits = ch.func.functional_call(model, (weights, buffers), image.unsqueeze(0))
         bindex = ch.arange(logits.shape[0]).to(logits.device, non_blocking=False)
         logits_correct = logits[bindex, label.unsqueeze(0)]
 
         cloned_logits = logits.clone()
-        # a hacky way to remove the logits of the correct labels from the sum
+        # remove the logits of the correct labels from the sum
         # in logsumexp by setting to -ch.inf
-        cloned_logits[bindex, label.unsqueeze(0)] = ch.tensor(-ch.inf).to(logits.device)
+        cloned_logits[bindex, label.unsqueeze(0)] = ch.tensor(-ch.inf, device=logits.device, dtype=logits.dtype)
 
         margins = logits_correct - cloned_logits.logsumexp(dim=-1)
         return margins.sum()
 
-    def forward(self, model: Module, batch: Iterable[Tensor]) -> Tensor:
-        """ Utility method to make forward passes compatible across different models,
-        e.g. image classification models take in only the images in the batch,
-        but CLIP takes in both the images and captions --- using this method,
-        the TRAKer class does not need to be modified when we have a new model
-        that uses different parts of the input batch.
-
-        Args:
-            model (Module):
-                model
-            batch (Iterable[Tensor]):
-                input batch
-
-        Returns:
-            Tensor:
-                model output (not to be confused with the model output function)
-        """
-        images, _ = batch
-        return model(images)
-
-    def get_out_to_loss_grad(self, func_model, weights, buffers, batch: Iterable[Tensor]) -> Tensor:
+    def get_out_to_loss_grad(self, model, weights, buffers, batch: Iterable[Tensor]) -> Tensor:
         """ Computes the (reweighting term Q in the paper)
 
         Args:
-            func_model (func):
-                functorch functional model
+            model (torch.nn.Module):
+                torch model
             weights (Iterable[Tensor]):
                 functorch model weights
             buffers (Iterable[Tensor]):
                 functorch model buffers
             batch (Iterable[Tensor]):
                 input batch
 
         Returns:
             Tensor:
                 out-to-loss (reweighting term) for the input batch
         """
         images, labels = batch
-        logits = func_model(weights, buffers, images)
-        # here we are directly implementing the gradient instead of relying on autodiff to do
-        # that for us
-        ps = self.softmax(logits / self.loss_temperature)[ch.arange(logits.size(0)), labels]
-        return (1 - ps).clone().detach().unsqueeze(-1)
-
-
-class IterImageClassificationModelOutput(AbstractModelOutput):
-    """
-    Margin for (multiclass) image classification. See Section 3.3 of `our paper
-    <https://arxiv.org/abs/2303.14186>`_ for more details.
-    """
-
-    def __init__(self, temperature=1.) -> None:
-        """
-        Args:
-            temperature (float, optional):
-                Temperature to use inside the softmax for the out-to-loss
-                function. Defaults to 1.
-        """
-        super().__init__()
-        self.softmax = ch.nn.Softmax(-1)
-        self.loss_temperature = temperature
-
-    def get_output(self,
-                   model: Module,
-                   images: Tensor,
-                   labels: Tensor) -> Tensor:
-        """ For a given input :math:`z=(x, y)` and model parameters :math:`\\theta`,
-        let :math:`p(z, \\theta)` be the softmax probability of the correct class.
-        This method implements the model output function
-
-        .. math::
-
-            \\log(\\frac{p(z, \\theta)}{1 - p(z, \\theta)}).
-
-        Args:
-            model (torch.nn.Module):
-                model
-            images (Tensor):
-                input images
-            labels (Tensor):
-                input labels
-
-        Returns:
-            Tensor:
-                model output for the given image-label pair :math:`z` and model
-                parameters :math:`\\theta`.
-        """
-        logits = model(images)
-        bindex = ch.arange(logits.shape[0]).to(logits.device, non_blocking=False)
-        logits_correct = logits[bindex, labels]
-
-        cloned_logits = logits.clone()
-        # a hacky way to remove the logits of the correct labels from the sum
-        # in logsumexp by setting to -ch.inf
-        cloned_logits[bindex, labels] = ch.tensor(-ch.inf).to(logits.device)
-
-        margins = logits_correct - cloned_logits.logsumexp(dim=-1)
-        return margins
-
-    def get_out_to_loss_grad(self, model: Module, batch: Iterable[Tensor]) -> Tensor:
-        """ Computes the (reweighting term Q in the paper)
-
-        Args:
-            model (torch.nn.Module)
-                model
-            batch (Iterable[Tensor]):
-                input batch
-
-        Returns:
-            Tensor:
-                out-to-loss (reweighting term) for the input batch
-        """
-        images, labels = batch
-        logits = model(images)
+        logits = ch.func.functional_call(model, (weights, buffers), images)
         # here we are directly implementing the gradient instead of relying on autodiff to do
         # that for us
         ps = self.softmax(logits / self.loss_temperature)[ch.arange(logits.size(0)), labels]
         return (1 - ps).clone().detach().unsqueeze(-1)
 
 
 class CLIPModelOutput(AbstractModelOutput):
     """ Margin for multimodal contrastive learning (CLIP). See Section 5.1 of
     `our paper <https://arxiv.org/abs/2303.14186>`_ for more details.
+    Compatible with the open_clip implementation of CLIP.
 
     Raises:
         AssertionError: this model output function requires using additional
         CLIP embeddings, which are computed using the :func:`get_embeddings`
         method. This method should be invoked before featurizing.
     """
     num_computed_embeddings = 0
@@ -303,25 +202,28 @@
                 Defaults to 300.
 
         """
         super().__init__()
         self.softmax = ch.nn.Softmax(-1)
         self.temperature = temperature
 
+        ch.backends.cuda.enable_mem_efficient_sdp(False)
+
         self.sim_batch_size = simulated_batch_size
         CLIPModelOutput.sim_batch_size = simulated_batch_size
 
     @staticmethod
     def get_embeddings(model,
                        loader,
                        batch_size: int,
+                       embedding_dim: int,
                        size: int = 50_000,
-                       embedding_dim: int = 1024,
                        preprocess_fn_img=None,
-                       preprocess_fn_txt=None) -> None:
+                       preprocess_fn_txt=None,
+                       ) -> None:
         """ Computes (image and text) embeddings and saves them in the class
         attributes :code:`image_embeddings` and :code:`text_embeddings`.
 
         Args:
             model (torch.nn.Module):
                 model
             loader ():
@@ -360,15 +262,15 @@
                     break
 
         CLIPModelOutput.image_embeddings = img_embs
         CLIPModelOutput.text_embeddings = txt_embs
         CLIPModelOutput.num_computed_embeddings = size
 
     @staticmethod
-    def get_output(func_model,
+    def get_output(model: Module,
                    weights: Iterable[Tensor],
                    buffers: Iterable[Tensor],
                    image: Tensor,
                    label: Tensor) -> Tensor:
         """ For a given input :math:`z=(x, y)` and model parameters
         :math:`\\theta`, let :math:`\\phi(x, \\theta)` be the CLIP image
         embedding and :math:`\\psi(y, \\theta)` be the CLIP text embedding.
@@ -378,29 +280,23 @@
         .. math::
 
             -\\log(\\frac{\\phi(x)\\cdot \\psi(y)}{\\sum_{(x', y')\\in B}
             \\phi(x)\\cdot \\psi(y')})
             -\\log(\\frac{\\phi(x)\\cdot \\psi(y)}{\\sum_{(x', y')\\in B}
             \\phi(x')\\cdot \\psi(y)})
 
-        It uses functorch's functional models to make the per-sample gradient
-        computations faster.  For more details on what func_model, weights &
-        buffers are, and how to use them, please refer to
-        https://pytorch.org/functorch/stable/ and
+        It uses functional models from torch.func (previously functorch) to make
+        the per-sample gradient computations (much) faster. For more details on
+        what functional models are, and how to use them, please refer to
+        https://pytorch.org/docs/stable/func.html and
         https://pytorch.org/functorch/stable/notebooks/per_sample_grads.html.
 
-        Note: this method slightly breaks abstraction since it has a different
-        signature from the abstract :code:`get_output`. It's only used
-        internally by :func:`GradientComputer` so it shouldn't be a big problem.
-        If you're reading this and feel strongly about it, feel free to make a
-        PR with a fix.
-
         Args:
-            func_model (func):
-                functorch functional model
+            model (torch.nn.Module):
+                torch model
             weights (Iterable[Tensor]):
                 functorch model weights
             buffers (Iterable[Tensor]):
                 functorch model buffers
             image (Tensor):
                 input image, should not have batch dimension
             label (Tensor):
@@ -413,48 +309,56 @@
         """
         all_im_embs = CLIPModelOutput.image_embeddings
         all_txt_embs = CLIPModelOutput.text_embeddings
         N = CLIPModelOutput.num_computed_embeddings
         sim_bs = CLIPModelOutput.sim_batch_size
 
         if all_im_embs is None:
-            raise AssertionError('Run traker.modelout_fn.get_embeddings first before featurizing!')
+            raise AssertionError('Run traker.task.get_embeddings first before featurizing!')
 
-        image_embeddings, text_embeddings, _ = func_model(weights,
-                                                          buffers,
-                                                          image.unsqueeze(0),
-                                                          label.unsqueeze(0))
+        # tailored for open_clip
+        # https://github.com/mlfoundations/open_clip/blob/fb72f4db1b17133befd6c67c9cf32a533b85a321/src/open_clip/model.py#L242-L245
+        clip_inputs = {'image': image.unsqueeze(0), 'text': label.unsqueeze(0)}
+        image_embeddings, text_embeddings, _ = ch.func.functional_call(model,
+                                                                       (weights, buffers),
+                                                                       args=(),
+                                                                       kwargs=clip_inputs)
 
         ii = ch.multinomial(input=ch.arange(N).float(),
                             num_samples=sim_bs,
                             replacement=False)
 
         result = -ch.logsumexp(-image_embeddings @ (text_embeddings - all_txt_embs[ii]).T, dim=1) +\
                  -ch.logsumexp(-text_embeddings @ (image_embeddings - all_im_embs[ii]).T, dim=1)
         return result.sum()  # shape of result should be [1]
 
-    def get_out_to_loss_grad(self, func_model, weights, buffers, batch: Iterable[Tensor]) -> Tensor:
+    def get_out_to_loss_grad(self, model, weights, buffers, batch: Iterable[Tensor]) -> Tensor:
         """ Computes the (reweighting term Q in the paper)
 
         Args:
-            func_model (func):
-                functorch functional model
+            model (torch.nn.Module):
+                torch model
             weights (Iterable[Tensor]):
                 functorch model weights
             buffers (Iterable[Tensor]):
                 functorch model buffers
             batch (Iterable[Tensor]):
                 input batch
 
         Returns:
             Tensor:
                 out-to-loss (reweighting term) for the input batch
 
         """
-        image_embeddings, text_embeddings, temp = func_model(weights, buffers, *batch)
+        image, label = batch
+        clip_inputs = {'image': image, 'text': label}
+        image_embeddings, text_embeddings, temp = ch.func.functional_call(model,
+                                                                          (weights, buffers),
+                                                                          args=(),
+                                                                          kwargs=clip_inputs)
         if self.temperature is None:
             self.temperature = temp
         res = self.temperature * image_embeddings @ text_embeddings.T
         ps = (self.softmax(res) + self.softmax(res.T)).diag() / 2.
         return (1 - ps).clone().detach()
 
 
@@ -471,46 +375,41 @@
 
     def __init__(self, temperature=1.) -> None:
         super().__init__()
         self.softmax = ch.nn.Softmax(-1)
         self.loss_temperature = temperature
 
     @staticmethod
-    def get_output(func_model,
+    def get_output(model,
                    weights: Iterable[Tensor],
                    buffers: Iterable[Tensor],
                    input_id: Tensor,
                    token_type_id: Tensor,
                    attention_mask: Tensor,
                    label: Tensor,
                    ) -> Tensor:
-        logits = func_model(weights, buffers, input_id.unsqueeze(0),
-                            token_type_id.unsqueeze(0),
-                            attention_mask.unsqueeze(0))
+        logits = ch.func.functional_call(model,
+                                         (weights, buffers),
+                                         input_id.unsqueeze(0),
+                                         token_type_id.unsqueeze(0),
+                                         attention_mask.unsqueeze(0))
         bindex = ch.arange(logits.shape[0]).to(logits.device, non_blocking=False)
         logits_correct = logits[bindex, label.unsqueeze(0)]
 
         cloned_logits = logits.clone()
-        cloned_logits[bindex, label.unsqueeze(0)] = ch.tensor(-ch.inf).to(logits.device)
+        cloned_logits[bindex, label.unsqueeze(0)] = ch.tensor(-ch.inf, device=logits.device, dtype=logits.dtype)
 
         margins = logits_correct - cloned_logits.logsumexp(dim=-1)
         return margins.sum()
 
-    def forward(self, model: Module, batch: Iterable[Tensor]) -> Tensor:
-        input_ids, token_type_ids, attention_mask, _ = batch
-        return model(input_ids=input_ids,
-                     token_type_ids=token_type_ids,
-                     attention_mask=attention_mask)
-
-    def get_out_to_loss_grad(self, func_model, weights, buffers, batch: Iterable[Tensor]) -> Tensor:
+    def get_out_to_loss_grad(self, model, weights, buffers, batch: Iterable[Tensor]) -> Tensor:
         input_ids, token_type_ids, attention_mask, labels = batch
-        logits = func_model(weights, buffers, input_ids, token_type_ids, attention_mask)
+        logits = ch.func.functional_call(model, (weights, buffers), input_ids, token_type_ids, attention_mask)
         ps = self.softmax(logits / self.loss_temperature)[ch.arange(logits.size(0)), labels]
         return (1 - ps).clone().detach().unsqueeze(-1)
 
 
 TASK_TO_MODELOUT = {
-    ('image_classification', True): ImageClassificationModelOutput,
-    ('image_classification', False): IterImageClassificationModelOutput,
-    ('text_classification', True): TextClassificationModelOutput,
-    ('clip', True): CLIPModelOutput,
+    'image_classification': ImageClassificationModelOutput,
+    'clip': CLIPModelOutput,
+    'text_classification': TextClassificationModelOutput,
 }
```

### Comparing `traker-0.1.3/trak/projectors.py` & `traker-0.2.0/trak/projectors.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,40 +63,69 @@
 
         Returns:
             Tensor: the projected gradients
         """
         ...
 
 
+class NoOpProjector(AbstractProjector):
+    """
+    A projector that returns the gradients as they are, i.e., implements
+    :code:`projector.project(grad) = grad`.
+    """
+    def __init__(self,
+                 grad_dim: int = 0,
+                 proj_dim: int = 0,
+                 seed: int = 0,
+                 proj_type: Union[str, ProjectionType] = 'na',
+                 device: Union[str, torch.device] = 'na',
+                 *args,
+                 **kwargs) -> None:
+        super().__init__(grad_dim, proj_dim, seed, proj_type, device)
+
+    def project(self, grads: Tensor, model_id: int) -> Tensor:
+        """ A no-op method.
+
+        Args:
+            grads (Tensor): a batch of gradients to be projected
+            model_id (int): a unique ID for a checkpoint
+
+        Returns:
+            Tensor: the (non-)projected gradients
+        """
+        return grads
+
+
 class BasicSingleBlockProjector(AbstractProjector):
     """
     A bare-bones, inefficient implementation of the projection, which simply
     calls torch's matmul for the projection step.
 
     Note: for most model sizes (e.g. even for ResNet18), and small projection
     dimensions (e.g. anything > 100) this method will OOM on an A100.
 
     Unless you have a good reason to use this class (I cannot think of one, I
     added this only for testing purposes), use instead the CudaProjector or
     BasicProjector.
     """
     def __init__(self, grad_dim: int, proj_dim: int, seed: int, proj_type:
-                 ProjectionType, device, dtype=ch.float16, model_id=0) -> None:
+                 ProjectionType, device, dtype=ch.float32, model_id=0,
+                 *args, **kwargs) -> None:
         super().__init__(grad_dim, proj_dim, seed, proj_type, device)
 
         self.model_id = model_id
         self.proj_type = proj_type
         self.generator = ch.Generator(device=self.device)
         self.generator = self.generator.manual_seed(self.seed + int(1e4) * self.model_id)
         self.dtype = dtype
 
-        self.proj_matrix = ch.ones(self.grad_dim,
-                                   self.proj_dim,
-                                   dtype=self.dtype,
-                                   device=self.device)
+        self.proj_matrix = ch.empty(self.grad_dim,
+                                    self.proj_dim,
+                                    dtype=self.dtype,
+                                    device=self.device)
 
         self.generate_sketch_matrix()  # updates self.proj_matrix
 
     def generate_sketch_matrix(self):
         if self.proj_type == ProjectionType.normal or self.proj_type == 'normal':
             self.proj_matrix.normal_(generator=self.generator)
         elif self.proj_type == ProjectionType.rademacher or self.proj_type == 'rademacher':
@@ -104,14 +133,15 @@
             # going from Bernoulli {0, 1} to Rademacher {-1, 1}
             self.proj_matrix *= 2.
             self.proj_matrix -= 1.
         else:
             raise KeyError(f'Projection type {self.proj_type} not recognized.')
 
     def project(self, grads: Tensor, model_id: int) -> Tensor:
+        grads = grads.to(dtype=self.dtype)
         if model_id != self.model_id:
             self.model_id = model_id
             self.generator = self.generator.manual_seed(self.seed + int(1e4) * self.model_id)
             self.generate_sketch_matrix()  # updates self.proj_matrix
 
         return grads @ self.proj_matrix
 
@@ -126,24 +156,25 @@
     footprint than the CudaProjector. It is recommended that you use this method
     only if the CudaProjector is not available to you -- e.g. if you don't have
     a CUDA-enabled device with compute capability >=7.0 (see
     https://developer.nvidia.com/cuda-gpus).
     """
     def __init__(self, grad_dim: int, proj_dim: int, seed: int, proj_type:
                  ProjectionType, device, block_size: int = 200, dtype=ch.float32,
-                 model_id=0) -> None:
+                 model_id=0, *args, **kwargs) -> None:
         super().__init__(grad_dim, proj_dim, seed, proj_type, device)
 
         self.block_size = min(self.proj_dim, block_size)
         self.num_blocks = math.ceil(self.proj_dim / self.block_size)
         self.dtype = dtype
         self.proj_type = proj_type
         self.model_id = model_id
 
-        self.proj_matrix = ch.empty(self.grad_dim, self.block_size,
+        self.proj_matrix = ch.empty(self.grad_dim,
+                                    self.block_size,
                                     dtype=self.dtype,
                                     device=self.device)
 
         self.generator = ch.Generator(device=self.device)
 
         self.get_generator_states()
         self.generate_sketch_matrix(self.generator_states[0])
@@ -167,14 +198,15 @@
             self.proj_matrix.bernoulli_(p=0.5, generator=self.generator)
             self.proj_matrix *= 2.
             self.proj_matrix -= 1.
         else:
             raise KeyError(f'Projection type {self.proj_type} not recognized.')
 
     def project(self, grads: Tensor, model_id: int) -> Tensor:
+        grads = grads.to(dtype=self.dtype)
         sketch = ch.zeros(size=(grads.size(0), self.proj_dim),
                           dtype=self.dtype, device=self.device)
 
         if model_id != self.model_id:
             self.model_id = model_id
             self.get_generator_states()  # regenerate random seeds for new model_id
             if self.num_blocks == 1:
@@ -194,15 +226,15 @@
 
 class CudaProjector(AbstractProjector):
     """
     A performant implementation of the projection for CUDA with compute
     capability >= 7.0.
     """
     def __init__(self, grad_dim: int, proj_dim: int, seed: int, proj_type:
-                 ProjectionType, device, max_batch_size: int = 32, *args, **kwargs) -> None:
+                 ProjectionType, device, max_batch_size: int, *args, **kwargs) -> None:
         """
 
         Args:
             grad_dim (int):
                 Number of parameters
             proj_dim (int):
                 Dimension we project *to* during the projection step
@@ -260,14 +292,14 @@
         function_name = f"project_{self.proj_type.value}_{effective_batch_size}"
         import fast_jl
         fn = getattr(fast_jl, function_name)
 
         try:
             result = fn(grads, self.proj_dim, self.seed + int(1e4) * model_id, self.num_sms)
         except RuntimeError as e:
-            if str(e) == 'CUDA error: too many resources requested for launch\nCUDA kernel errors might be asynchronously reported at some other API call, so the stacktrace below might be incorrect.\nFor debugging consider passing CUDA_LAUNCH_BLOCKING=1.\nCompile with `TORCH_USE_CUDA_DSA` to enable device-side assertions.\n':
+            if str(e) == 'CUDA error: too many resources requested for launch\nCUDA kernel errors might be asynchronously reported at some other API call, so the stacktrace below might be incorrect.\nFor debugging consider passing CUDA_LAUNCH_BLOCKING=1.\nCompile with `TORCH_USE_CUDA_DSA` to enable device-side assertions.\n':  # noqa: E501
                 # provide a more helpful error message
-                raise RuntimeError(f'The batch size of the CudaProjector is too large for your GPU. Reduce it by using the max_batch_size argument of the CudaProjector.\nOriginal error: {str(e)}')
+                raise RuntimeError('The batch size of the CudaProjector is too large for your GPU. Reduce it by using the proj_max_batch_size argument of the TRAKer.\nOriginal error.')  # noqa: E501
             else:
                 raise e
 
         return result
```

### Comparing `traker-0.1.3/trak/score_computers.py` & `traker-0.2.0/trak/score_computers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     The :code:`ScoreComputer` class
     Implementations of the ScoreComputer class must implement three methods:
     - :code:`get_xtx`
     - :code:`get_x_xtx_inv`
     - :code:`get_scores`
     """
     @abstractmethod
-    def __init__(self, device) -> None:
+    def __init__(self, dtype, device) -> None:
+        self.dtype = dtype
         self.device = device
 
     @abstractmethod
     def get_xtx(self, grads: Tensor) -> Tensor:
         ...
 
     @abstractmethod
@@ -30,70 +31,76 @@
 
 class BasicSingleBlockScoreComputer(AbstractScoreComputer):
     """ A bare-bones implementation of :code:`ScoreComputer` that will likely
     OOM for almost all applications. Here for testing purposes only. Unless you
     have a good reason not to, you should use :func:`BasicScoreComputer`
     instead.
     """
-    def __init__(self, device) -> None:
-        super().__init__(device)
+    def __init__(self, dtype, device) -> None:
+        super().__init__(dtype, device)
 
     def get_xtx(self, grads: Tensor) -> Tensor:
         return grads.T @ grads
 
     def get_x_xtx_inv(self, grads: Tensor, xtx: Tensor) -> Tensor:
-        return grads @ ch.linalg.inv(xtx)
+        # torch.linalg.inv does not support float16
+        return grads @ ch.linalg.inv(xtx.float()).to(self.dtype)
 
     def get_scores(self, features: Tensor, target_grads: Tensor) -> Tensor:
         return features @ target_grads.T
 
 
 class BasicScoreComputer(AbstractScoreComputer):
     """ An implementation of :code:`ScoreComputer` that computes matmuls in a
     block-wise manner.
     """
-    def __init__(self, device, CUDA_MAX_DIM_SIZE: int = 100_000) -> None:
+    def __init__(self, dtype, device, CUDA_MAX_DIM_SIZE: int = 100_000) -> None:
         """
         Args:
             device (Union[str, torch.device]): torch device to do matmuls on
             CUDA_MAX_DIM_SIZE (int, optional): Size of block for block-wise
             matmuls. Defaults to 100_000.
         """
-        super().__init__(device)
+        super().__init__(dtype, device)
         self.CUDA_MAX_DIM_SIZE = CUDA_MAX_DIM_SIZE
 
     def get_xtx(self, grads: Tensor) -> Tensor:
         self.proj_dim = grads.shape[1]
-        result = ch.zeros(self.proj_dim, self.proj_dim).to(self.device)
+        result = ch.zeros(self.proj_dim, self.proj_dim, dtype=self.dtype, device=self.device)
         blocks = ch.split(grads, split_size_or_sections=self.CUDA_MAX_DIM_SIZE, dim=0)
 
         for block in blocks:
             result += block.T.to(self.device) @ block.to(self.device)
 
         return result
 
     def get_x_xtx_inv(self, grads: Tensor, xtx: Tensor) -> Tensor:
         blocks = ch.split(grads, split_size_or_sections=self.CUDA_MAX_DIM_SIZE, dim=0)
-        xtx_inv = ch.linalg.inv(xtx)
+        xtx_inv = ch.linalg.inv(xtx.to(ch.float32))
 
-        result = ch.empty(grads.shape[0], xtx_inv.shape[1], device=self.device)
+        # center X^TX inverse a bit to avoid numerical issues when going to float16
+        xtx_inv /= xtx_inv.abs().mean()
+
+        xtx_inv = xtx_inv.to(self.dtype)
+
+        result = ch.empty(grads.shape[0], xtx_inv.shape[1], dtype=self.dtype, device=self.device)
         for i, block in enumerate(blocks):
             start = i * self.CUDA_MAX_DIM_SIZE
             end = min(grads.shape[0], (i + 1) * self.CUDA_MAX_DIM_SIZE)
             result[start: end] = (block.to(self.device) @ xtx_inv)
         return result
 
     def get_scores(self, features: Tensor, target_grads: Tensor) -> Tensor:
         train_dim = features.shape[0]
         target_dim = target_grads.shape[0]
 
         if target_dim < self.CUDA_MAX_DIM_SIZE:
             return features @ target_grads.T
 
-        result = ch.empty(train_dim, target_dim).to(self.device)
+        result = ch.empty(train_dim, target_dim, dtype=self.dtype, device=self.device)
         blocks = ch.split(target_grads, split_size_or_sections=self.CUDA_MAX_DIM_SIZE, dim=0)
 
         for i, block in enumerate(blocks):
             start = i * self.CUDA_MAX_DIM_SIZE
             end = min(target_grads.shape[0], (i + 1) * self.CUDA_MAX_DIM_SIZE)
             result[:, start: end] = features @ block.T
```

### Comparing `traker-0.1.3/trak/traker.py` & `traker-0.2.0/trak/traker.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .utils import get_num_params
 
 from typing import Iterable, Optional, Union
 from pathlib import Path
 from tqdm import tqdm
 from torch import Tensor
 
+import logging
 import numpy as np
 import torch
 ch = torch
 
 
 class TRAKer():
     """ The main front-facing class for TRAK. See the `README
@@ -30,27 +31,31 @@
                  load_from_save_dir: bool = True,
                  device: Union[str, torch.device] = 'cuda',
                  gradient_computer: AbstractGradientComputer = FunctionalGradientComputer,
                  projector: Optional[AbstractProjector] = None,
                  saver: Optional[AbstractSaver] = None,
                  score_computer: Optional[AbstractScoreComputer] = None,
                  proj_dim: int = 2048,
+                 logging_level=logging.INFO,
+                 use_half_precision: bool = True,
+                 proj_max_batch_size: int = 32,
                  ) -> None:
         """
 
         Args:
             model (torch.nn.Module):
                 model to use for TRAK
             task (Union[AbstractModelOutput, str]):
                 Type of model that TRAK will be ran on. Accepts either one of
                 the following strings:
                 - :code:`image_classification`
                 - :code:`text_classification`
                 - :code:`clip`
-                or an implementation of :class:`.AbstractModelOutput`.
+                or an instance of some implementation of the abstract class
+                :class:`.AbstractModelOutput`.
             train_set_size (int):
                 Size of the train set that TRAK is featurizing
             save_dir (str, optional):
                 Directory to save final TRAK scores, intermediate results, and
                 metadata. Defaults to :code:'./trak_results'.
             load_from_save_dir (bool, optional):
                 If True, the :class`.TRAKer` instance will attempt to load
@@ -75,88 +80,117 @@
             score_computer (Optional[AbstractScoreComputer], optional):
                 Class to use for computing the final TRAK scores. If None, the
                 :class:`.BasicScoreComputer` will be used. Defaults to None.
             proj_dim (int, optional):
                 Dimension of the projected TRAK features. See Section 4.3 of
                 `our paper <https://arxiv.org/abs/2303.14186>`_ for more
                 details. Defaults to 2048.
+            logging_level (int, optional):
+                Logging level for TRAK loggers. Defaults to logging.INFO.
+            use_half_precision (bool, optional):
+                If True, TRAK will use half precision (float16) for all
+                computations and arrays will be stored in float16. Otherwise, it
+                will use float32. Defaults to True.
 
         """
 
         self.model = model
         self.task = task
         self.train_set_size = train_set_size
         self.device = device
+        self.dtype = ch.float16 if use_half_precision else ch.float32
+
+        logging.basicConfig()
+        self.logger = logging.getLogger('TRAK')
+        self.logger.setLevel(logging_level)
+        self.logger.warning('TRAK is still in an early 0.x.x version.\n\
+                             Report any issues at https://github.com/MadryLab/trak/issues')
 
         self.num_params = get_num_params(self.model)
-        self.init_projector(projector, proj_dim)  # inits self.projector
+        # inits self.projector
+        self.init_projector(projector, proj_dim, proj_max_batch_size)
+
+        # normalize to make X^TX numerically stable
+        # doing this instead of normalizing the projector matrix
+        self.normalize_factor = ch.sqrt(ch.tensor(self.num_params, dtype=ch.float32))
 
         self.save_dir = Path(save_dir).resolve()
         self.load_from_save_dir = load_from_save_dir
 
         if type(self.task) is str:
-            self.task = TASK_TO_MODELOUT[(self.task, gradient_computer.is_functional)]
+            self.task = TASK_TO_MODELOUT[self.task]()
 
         self.gradient_computer = gradient_computer(model=self.model,
-                                                   modelout_fn=self.task,
+                                                   task=self.task,
                                                    grad_dim=self.num_params)
 
         if score_computer is None:
             score_computer = BasicScoreComputer
-        self.score_computer = score_computer(device=self.device)
+        self.score_computer = score_computer(dtype=self.dtype,
+                                             device=self.device)
 
         metadata = {
-            'JL dimension': self.projector.proj_dim,
+            'JL dimension': self.proj_dim,
             'JL matrix type': self.projector.proj_type,
+            'train set size': self.train_set_size,
         }
 
         if saver is None:
             saver = MmapSaver
         self.saver = saver(save_dir=self.save_dir,
                            metadata=metadata,
                            train_set_size=self.train_set_size,
                            proj_dim=self.proj_dim,
-                           load_from_save_dir=self.load_from_save_dir)
+                           load_from_save_dir=self.load_from_save_dir,
+                           logging_level=logging_level,
+                           use_half_precision=use_half_precision)
 
-    def init_projector(self, projector, proj_dim) -> None:
+        self.ckpt_loaded = 'no ckpt loaded'
+
+    def init_projector(self, projector, proj_dim, proj_max_batch_size) -> None:
         """ Initialize the projector for a traker class
 
         Args:
             projector (AbstractProjector):
                 JL projector
 
         """
 
         self.projector = projector
         if projector is not None:
             self.proj_dim = self.projector.proj_dim
+            if self.proj_dim == 0:  # using NoOpProjector
+                self.proj_dim = self.num_params
+
         else:
             self.proj_dim = proj_dim
             try:
                 import fast_jl
                 test_gradient = ch.ones(1, self.num_params).cuda()
                 num_sms = ch.cuda.get_device_properties('cuda').multi_processor_count
                 fast_jl.project_rademacher_8(test_gradient, self.proj_dim, 0, num_sms)
                 projector = CudaProjector
 
             except (ImportError, RuntimeError, AttributeError) as e:
-                print(f'Could not use CudaProjector.\nReason: {str(e)}')
-                print('Defaulting to BasicProjector.')
+                self.logger.error(f'Could not use CudaProjector.\nReason: {str(e)}')
+                self.logger.error('Defaulting to BasicProjector.')
                 projector = BasicProjector
 
             self.projector = projector(grad_dim=self.num_params,
                                        proj_dim=self.proj_dim,
                                        seed=0,
                                        proj_type=ProjectionType.rademacher,
+                                       max_batch_size=proj_max_batch_size,
+                                       dtype=self.dtype,
                                        device=self.device)
 
     def load_checkpoint(self,
                         checkpoint: Iterable[Tensor],
                         model_id: int,
-                        _allow_featurizing_already_registered=None) -> None:
+                        _allow_featurizing_already_registered=False) -> None:
         """ Loads state dictionary for the given checkpoint; initializes arrays
         to store TRAK features for that checkpoint, tied to the model ID.
 
         Args:
             checkpoint (Iterable[Tensor]):
                 state_dict to load
             model_id (int):
@@ -167,23 +201,23 @@
                 Defaults to None.
 
         """
         if self.saver.model_ids.get(model_id) is None:
             self.saver.register_model_id(model_id,
                                          _allow_featurizing_already_registered)
         else:
-            self.saver.load_store(model_id)
+            self.saver.load_current_store(model_id)
 
         self.model.load_state_dict(checkpoint)
         self.model.eval()
 
         self.gradient_computer.load_model_params(self.model)
 
         self._last_ind = 0
-        self._num_featurized = 0
+        self.ckpt_loaded = model_id
 
     def featurize(self,
                   batch: Iterable[Tensor],
                   inds: Optional[Iterable[int]] = None,
                   num_samples: Optional[int] = None
                   ) -> None:
         """ Creates TRAK features for the given batch by computing the gradient
@@ -204,39 +238,44 @@
                 input batch
             inds (Optional[Iterable[int]], optional):
                 Indices of the batch samples in the train set. Defaults to None.
             num_samples (Optional[int], optional):
                 Number of samples in the batch. Defaults to None.
 
         """
+        assert self.ckpt_loaded == self.saver.current_model_id,\
+            "Load a checkpoint using traker.load_checkpoint before featurizing"
         assert (inds is None) or (num_samples is None),\
             "Exactly one of num_samples and inds should be specified"
         assert (inds is not None) or (num_samples is not None),\
             "Exactly one of num_samples and inds should be specified"
 
         if num_samples is not None:
             inds = np.arange(self._last_ind, self._last_ind + num_samples)
             self._last_ind += num_samples
         else:
             num_samples = inds.reshape(-1).shape[0]
-        self._num_featurized += num_samples
 
-        grads = self.gradient_computer.compute_per_sample_grad(batch=batch,
-                                                               batch_size=num_samples)
+        # handle re-starting featurizing from a partially featurized model (some inds already featurized)
+        _already_done = (self.saver.current_store['is_featurized'][inds] == 1).reshape(-1)
+        inds = inds[~_already_done]
+        if len(inds) == 0:
+            self.logger.debug('All samples in batch already featurized.')
+            return 0
+
+        grads = self.gradient_computer.compute_per_sample_grad(batch=batch)
         grads = self.projector.project(grads, model_id=self.saver.current_model_id)
-        self.saver.current_grads[inds] = grads.cpu().clone().detach()
+        grads /= self.normalize_factor
+        self.saver.current_store['grads'][inds] = grads.to(self.dtype).cpu().clone().detach()
 
         loss_grads = self.gradient_computer.compute_loss_grad(batch)
-        self.saver.current_out_to_loss[inds] = loss_grads.cpu().clone().detach()
+        self.saver.current_store['out_to_loss'][inds] = loss_grads.to(self.dtype).cpu().clone().detach()
 
-        if self._num_featurized == self.train_set_size:
-            # TODO: currently this is breaking abstraction -- either define dict
-            # items in abstract __init__, or don't access them here
-            self.saver.model_ids[self.saver.current_model_id]['featurized'] = 1
-            self.saver.serialize_model_id_metadata(self.saver.current_model_id)
+        self.saver.current_store['is_featurized'][inds] = 1
+        self.saver.serialize_current_model_id_metadata()
 
     def finalize_features(self,
                           model_ids: Iterable[int] = None,
                           del_grads: bool = False) -> None:
         """ For a set of checkpoints :math:`C` (specified by model IDs), and
         gradients :math:`\\{ \\Phi_c \\}_{c\\in C}`, this method computes
         :math:`\\Phi_c (\\Phi_c^\\top\\Phi_c)^{-1}` for all :math:`c\\in C`
@@ -254,53 +293,67 @@
             model_ids = list(self.saver.model_ids.keys())
 
         self._last_ind = 0
 
         for model_id in tqdm(model_ids, desc='Finalizing features for all model IDs..'):
             if self.saver.model_ids.get(model_id) is None:
                 raise ModelIDException(f'Model ID {model_id} not registered, not ready for finalizing.')
-            elif self.saver.model_ids[model_id]['finalized'] == 1:
-                print(f'Model ID {model_id} already finalized, skipping .finalize_features for it.')
+            elif self.saver.model_ids[model_id]['is_featurized'] == 0:
+                raise ModelIDException(f'Model ID {model_id} not fully featurized, not ready for finalizing.')
+            elif self.saver.model_ids[model_id]['is_finalized'] == 1:
+                self.logger.warning(f'Model ID {model_id} already finalized, skipping .finalize_features for it.')
                 continue
 
-            self.saver.load_store(model_id)
+            self.saver.load_current_store(model_id)
 
-            g = ch.as_tensor(self.saver.current_grads)
+            g = ch.as_tensor(self.saver.current_store['grads'])
             xtx = self.score_computer.get_xtx(g)
+            self.logger.debug(f'XTX is {xtx}')
 
-            self.saver.current_features[:] = self.score_computer.get_x_xtx_inv(g, xtx).cpu()
+            features = self.score_computer.get_x_xtx_inv(g, xtx)
+            self.logger.debug(f'Features are {features}')
+            self.saver.current_store['features'][:] = features.to(self.dtype).cpu()
             if del_grads:
                 self.saver.del_grads(model_id)
 
-            self.saver.model_ids[self.saver.current_model_id]['finalized'] = 1
-            self.saver.serialize_model_id_metadata(self.saver.current_model_id)
+            self.saver.model_ids[self.saver.current_model_id]['is_finalized'] = 1
+            self.saver.serialize_current_model_id_metadata()
 
     def start_scoring_checkpoint(self,
+                                 exp_name: str,
                                  checkpoint: Iterable[Tensor],
                                  model_id: int,
                                  num_targets: int,
                                  ) -> None:
         """ This method prepares the internal store of the :class:`.TRAKer` class
         to start computing scores for a set of targets.
 
         Args:
+            exp_name (str):
+                Experiment name. Each experiment should have a unique name, and
+                it corresponds to a set of targets being scored. The experiment
+                name is used as the name for saving the target features, as well
+                as scores produced by this method in the :code:`save_dir` of the
+                :class:`.TRAKer` class.
             checkpoint (Iterable[Tensor]):
                 model checkpoint (state dict)
             model_id (int):
                 a unique ID for a checkpoint
             num_targets (int):
                 number of targets to score
 
         """
-        self.saver.load_target_store(model_id, num_targets, mode='w+')
+        self.saver.init_experiment(exp_name, num_targets, model_id)
 
         self.model.load_state_dict(checkpoint)
         self.model.eval()
         self.gradient_computer.load_model_params(self.model)
 
+        # TODO: make this exp_name-dependent
+        # e.g. make it a value in self.saver.experiments[exp_name]
         self._last_ind_target = 0
 
     def score(self,
               batch: Iterable[Tensor],
               inds: Optional[Iterable[int]] = None,
               num_samples: Optional[int] = None,
               ) -> None:
@@ -322,103 +375,109 @@
 
         """
         assert (inds is None) or (num_samples is None),\
             "Exactly one of num_samples and inds should be specified"
         assert (inds is not None) or (num_samples is not None),\
             "Exactly one of num_samples and inds should be specified"
 
-        # TODO: currently this is breaking abstraction -- either define dict
-        # items in abstract __init__, or don't access them here
-        if self.saver.model_ids[self.saver.current_model_id]['finalized'] == 0:
-            print(f'Model ID {self.saver.current_model_id} not finalized, cannot score')
+        if self.saver.model_ids[self.saver.current_model_id]['is_finalized'] == 0:
+            self.logger.error(f'Model ID {self.saver.current_model_id} not finalized, cannot score')
             return None
 
         if num_samples is not None:
             inds = np.arange(self._last_ind_target, self._last_ind_target + num_samples)
             self._last_ind_target += num_samples
         else:
             num_samples = inds.reshape(-1).shape[0]
 
-        grads = self.gradient_computer.compute_per_sample_grad(batch=batch,
-                                                               batch_size=num_samples)
+        grads = self.gradient_computer.compute_per_sample_grad(batch=batch)
 
         grads = self.projector.project(grads, model_id=self.saver.current_model_id)
+        grads /= self.normalize_factor
 
-        self.saver.current_target_grads[inds] = grads.cpu().clone().detach()
+        exp_name = self.saver.current_experiment_name
+        self.saver.current_store[f'{exp_name}_grads'][inds] = grads.to(self.dtype).cpu().clone().detach()
 
     def finalize_scores(self,
+                        exp_name: str,
                         model_ids: Iterable[int] = None,
-                        del_grads: bool = False,
                         allow_skip: bool = False,
-                        exp_name: str = None) -> Tensor:
+                        ) -> Tensor:
         """ This method computes the final TRAK scores for the given targets,
         train samples, and model checkpoints (specified by model IDs).
 
         Args:
+            exp_name (str):
+                Experiment name. Each experiment should have a unique name, and
+                it corresponds to a set of targets being scored. The experiment
+                name is used as the name for saving the target features, as well
+                as scores produced by this method in the :code:`save_dir` of the
+                :class:`.TRAKer` class.
             model_ids (Iterable[int], optional):
                 A list of model IDs for which
                 scores should be finalized. If None, scores are computed
                 for all model IDs in the :code:`save_dir` of the :class:`.TRAKer`
                 class. Defaults to None.
-            del_grads (bool, optional):
-                If True, the target gradients (intermediate results) are deleted
-                from the internal store of the :class:`.TRAKer` class.  Defaults
-                to False.
             allow_skip (bool, optional):
                 If True, raises only a warning, instead of an error, when target
                 gradients are not computed for a given model ID. Defaults to
                 False.
-            exp_name (str, optional):
-                Used to name the scores :code:`.npy` array produced by this
-                method in the :code:`save_dir` of the :class:`.TRAKer` class. If
-                None, a random uuid is generated.  Defaults to None.
 
         Returns:
             Tensor: TRAK scores
 
         """
         # reset counter for inds used for scoring
         self._last_ind_target = 0
 
         if model_ids is None:
             model_ids = self.saver.model_ids
+        else:
+            model_ids = {model_id: self.saver.model_ids[model_id] for model_id in model_ids}
+        assert len(model_ids) > 0, 'No model IDs to finalize scores for'
+
+        if self.saver.experiments.get(exp_name) is None:
+            raise ValueError(f'Experiment {exp_name} does not exist. Create it\n\
+                              and compute scores first before finalizing.')
 
+        num_targets = self.saver.experiments[exp_name]['num_targets']
         _completed = [False] * len(model_ids)
-        _scores = ch.zeros(self.train_set_size,
-                           self.saver.num_targets,
-                           device=self.device)
-        _avg_out_to_losses = ch.zeros(self.saver.train_set_size, 1, device=self.device)
+
+        self.saver.load_current_store(list(model_ids.keys())[0], exp_name, num_targets)
+        _scores = self.saver.current_store[f'{exp_name}_scores']
+        _scores[:] = 0.
+
+        _avg_out_to_losses = np.zeros((self.saver.train_set_size, 1),
+                                      dtype=np.float16 if self.dtype == ch.float16 else np.float32)
 
         for j, model_id in enumerate(tqdm(model_ids, desc='Finalizing scores for all model IDs..')):
-            self.saver.load_store(model_id)
+            self.saver.load_current_store(model_id)
             try:
-                self.saver.load_target_store(model_id, self.saver.num_targets)
+                self.saver.load_current_store(model_id, exp_name, num_targets)
             except OSError as e:
                 if allow_skip:
-                    print(f'Could not read target gradients for model ID {model_id}. Skipping.')
+                    self.logger.warning(f'Could not read target gradients for model ID {model_id}. Skipping.')
                     continue
                 else:
                     raise e
 
-            # TODO: currently this is breaking abstraction -- either define dict
-            # items in abstract __init__, or don't access them here
-            if self.saver.model_ids[self.saver.current_model_id]['finalized'] == 0:
-                print(f'Model ID {self.saver.current_model_id} not finalized, cannot score')
+            if self.saver.model_ids[self.saver.current_model_id]['is_finalized'] == 0:
+                self.logger.warning(f'Model ID {self.saver.current_model_id} not finalized, cannot score')
                 continue
 
-            g = ch.as_tensor(self.saver.current_features, device=self.device)
-            g_target = ch.as_tensor(self.saver.current_target_grads, device=self.device)
+            g = ch.as_tensor(self.saver.current_store['features'], device=self.device)
+            g_target = ch.as_tensor(self.saver.current_store[f'{exp_name}_grads'],
+                                    device=self.device)
 
-            _scores += self.score_computer.get_scores(g, g_target)
-            _avg_out_to_losses += ch.as_tensor(self.saver.current_out_to_loss, device=self.device)
-            _completed[j] = True
+            _scores += self.score_computer.get_scores(g, g_target).cpu().clone().detach().numpy()
 
-            if del_grads:
-                self.saver.del_grads(model_id, target=True)
-            else:
-                self.saver.clear_target_grad_count(model_id)
+            _avg_out_to_losses += self.saver.current_store['out_to_loss']
+            _completed[j] = True
 
         _num_models_used = float(sum(_completed))
-        self.scores = (_scores / _num_models_used) * (_avg_out_to_losses / _num_models_used)
-        self.saver.save_scores(self.scores.cpu().numpy(), exp_name)
+        _scores = (_scores / _num_models_used) * (_avg_out_to_losses / _num_models_used)
+
+        self.logger.debug(f'Scores dtype is {_scores.dtype}')
+        self.saver.save_scores(exp_name)
+        self.scores = _scores
 
         return self.scores
```

### Comparing `traker-0.1.3/traker.egg-info/SOURCES.txt` & `traker-0.2.0/traker.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 README.md
 setup.py
-tests/test_accuracy.py
-tests/test_cifar_accuracy.py
+tests/test_cifar10_accuracy.py
+tests/test_cifar2_accuracy.py
 tests/test_class.py
 tests/test_integration_cifar.py
 tests/test_integration_clip.py
 tests/test_jl.py
 tests/test_parallel.py
 tests/test_rademacher.py
 trak/__init__.py
```

