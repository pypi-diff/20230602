# Comparing `tmp/fastai-datasets-0.0.6.tar.gz` & `tmp/fastai-datasets-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastai-datasets-0.0.6.tar", last modified: Sat May 20 11:11:38 2023, max compression
+gzip compressed data, was "fastai-datasets-0.0.7.tar", last modified: Fri Jun  2 13:39:58 2023, max compression
```

## Comparing `fastai-datasets-0.0.6.tar` & `fastai-datasets-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:11:38.643440 fastai-datasets-0.0.6/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.6/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.6/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5419 2023-05-20 11:11:38.643440 fastai-datasets-0.0.6/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3821 2023-05-20 11:10:54.000000 fastai-datasets-0.0.6/README.md
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:11:38.639440 fastai-datasets-0.0.6/fastai_datasets/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12255 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.6/fastai_datasets/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/cifar10.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      947 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/imagenette.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/lfw.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      882 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/mnist.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3761 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/pairs.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5827 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/patches.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/pfr.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1877 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/utils.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:11:38.639440 fastai-datasets-0.0.6/fastai_datasets.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5419 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/top_level.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-05-20 11:10:39.000000 fastai-datasets-0.0.6/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-20 11:11:38.643440 fastai-datasets-0.0.6/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.6/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:39:58.189643 fastai-datasets-0.0.7/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.7/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.7/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4738 2023-06-02 13:39:58.185643 fastai-datasets-0.0.7/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3284 2023-05-20 11:36:01.000000 fastai-datasets-0.0.7/README.md
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:39:58.177643 fastai-datasets-0.0.7/fastai_datasets/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    13272 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.7/fastai_datasets/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/cifar10.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      947 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/imagenette.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/lfw.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      882 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/mnist.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3800 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/pairs.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     6947 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/patches.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/pfr.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1877 2023-06-02 13:39:43.000000 fastai-datasets-0.0.7/fastai_datasets/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:39:58.185643 fastai-datasets-0.0.7/fastai_datasets.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4738 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-06-02 13:39:58.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-06-02 13:39:57.000000 fastai-datasets-0.0.7/fastai_datasets.egg-info/top_level.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-06-02 13:38:51.000000 fastai-datasets-0.0.7/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-06-02 13:39:58.189643 fastai-datasets-0.0.7/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.7/setup.py
```

### Comparing `fastai-datasets-0.0.6/LICENSE` & `fastai-datasets-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.6/PKG-INFO` & `fastai-datasets-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.6
+Version: 0.0.7
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: fastai-datasets
         ================
@@ -43,20 +43,14 @@
         
         ### Show the class distribution
         
         ``` python
         mnist.plot_class_distribution()
         ```
         
-            <div>
-              <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [10/10 00:00&lt;00:00]
-            </div>
-            
-        
         ![](index_files/figure-commonmark/cell-4-output-2.png)
         
         ### Sample a subset
         
         Whole datasets:
         
         ``` python
@@ -68,45 +62,33 @@
         
         Subset:
         
         ``` python
         mnist.random_sub_dsets(1000)
         ```
         
-            [(#881) [(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(4)),(PILImageBW mode=L size=28x28, TensorCategory(7)),(PILImageBW mode=L size=28x28, TensorCategory(2)),(PILImageBW mode=L size=28x28, TensorCategory(9)),(PILImageBW mode=L size=28x28, TensorCategory(0)),(PILImageBW mode=L size=28x28, TensorCategory(9)),(PILImageBW mode=L size=28x28, TensorCategory(8)),(PILImageBW mode=L size=28x28, TensorCategory(4))...]
-            (#119) [(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(4)),(PILImageBW mode=L size=28x28, TensorCategory(2)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(0)),(PILImageBW mode=L size=28x28, TensorCategory(9)),(PILImageBW mode=L size=28x28, TensorCategory(8)),(PILImageBW mode=L size=28x28, TensorCategory(7)),(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(9))...]]
+            [(#861) [(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(6)),(PILImageBW mode=L size=28x28, TensorCategory(7)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(4)),(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(5)),(PILImageBW mode=L size=28x28, TensorCategory(1))...]
+            (#139) [(PILImageBW mode=L size=28x28, TensorCategory(0)),(PILImageBW mode=L size=28x28, TensorCategory(0)),(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(2)),(PILImageBW mode=L size=28x28, TensorCategory(8)),(PILImageBW mode=L size=28x28, TensorCategory(4)),(PILImageBW mode=L size=28x28, TensorCategory(2)),(PILImageBW mode=L size=28x28, TensorCategory(8)),(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(9))...]]
         
         ### Construct a subset based on classes
         
         ``` python
         cifar10 = CIFAR10()
         dig_frog_bird = cifar10.by_target['dog'] + cifar10.by_target['frog'] + cifar10.by_target['bird']
         dig_frog_bird.dls().show_batch()
         ```
         
-            <div>
-              <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [10/10 00:00&lt;00:00]
-            </div>
-            
-        
         ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         ### Construct a dataset of similarity pairs
         
         ``` python
         Pairs(cifar10, .01).dls().show_batch()
         ```
         
-            <div>
-              <progress value='50' class='' max='50' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [50/50 00:00&lt;00:00]
-            </div>
-            
-        
         ![](index_files/figure-commonmark/cell-8-output-2.png)
         
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `fastai-datasets-0.0.6/fastai_datasets/_modidx.py` & `fastai-datasets-0.0.7/fastai_datasets/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,23 @@
                                                                                     'fastai_datasets/pairs.py'),
                                        'fastai_datasets.pairs.Sameness.encodes': ( 'pairs.html#sameness.encodes',
                                                                                    'fastai_datasets/pairs.py'),
                                        'fastai_datasets.pairs._pairs_for_split': ( 'pairs.html#_pairs_for_split',
                                                                                    'fastai_datasets/pairs.py'),
                                        'fastai_datasets.pairs.show_batch': ('pairs.html#show_batch', 'fastai_datasets/pairs.py'),
                                        'fastai_datasets.pairs.show_results': ('pairs.html#show_results', 'fastai_datasets/pairs.py')},
-            'fastai_datasets.patches': { 'fastai_datasets.patches.Datasets.__add__': ( 'Core/patches.html#datasets.__add__',
+            'fastai_datasets.patches': { 'fastai_datasets.patches.DataLoader.__add__': ( 'Core/patches.html#dataloader.__add__',
+                                                                                         'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.DataLoader.by_target': ( 'Core/patches.html#dataloader.by_target',
+                                                                                           'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.DataLoader.random_sub_dl': ( 'Core/patches.html#dataloader.random_sub_dl',
+                                                                                               'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.DataLoader.sub_dl': ( 'Core/patches.html#dataloader.sub_dl',
+                                                                                        'fastai_datasets/patches.py'),
+                                         'fastai_datasets.patches.Datasets.__add__': ( 'Core/patches.html#datasets.__add__',
                                                                                        'fastai_datasets/patches.py'),
                                          'fastai_datasets.patches.Datasets.__repr__': ( 'Core/patches.html#datasets.__repr__',
                                                                                         'fastai_datasets/patches.py'),
                                          'fastai_datasets.patches.Datasets.__sub__': ( 'Core/patches.html#datasets.__sub__',
                                                                                        'fastai_datasets/patches.py'),
                                          'fastai_datasets.patches.Datasets.by_target': ( 'Core/patches.html#datasets.by_target',
                                                                                          'fastai_datasets/patches.py'),
```

### Comparing `fastai-datasets-0.0.6/fastai_datasets/imagenette.py` & `fastai-datasets-0.0.7/fastai_datasets/imagenette.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.6/fastai_datasets/lfw.py` & `fastai-datasets-0.0.7/fastai_datasets/lfw.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.6/fastai_datasets/mnist.py` & `fastai-datasets-0.0.7/fastai_datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.6/fastai_datasets/pairs.py` & `fastai-datasets-0.0.7/fastai_datasets/pairs.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,27 +52,27 @@
 def _pairs_for_split(singles: DataLoaders, split_idx: int, factor: int):
     assert singles.n_inp == 1
 
     indices = L(range_of(singles))[singles.splits[split_idx]]
     num = int(len(indices) * factor)
 
     class_map = defaultdict(list)
-    for i, c in progress_bar(indices.zipwith(singles.i2t.subset(split_idx))):
+    for i, c in progress_bar(indices.zipwith(singles.i2t.subset(split_idx)), leave=False):
         class_map[singles.vocab[c]].append(i)
 
     @return_list
     def _positive_pairs():
         multi_item_class_map = {k: v for k, v in class_map.items() if len(v)>1}
-        for _ in progress_bar(range(num//2)):
+        for _ in progress_bar(range(num//2), leave=False):
             c, idxs = random.choice(list(multi_item_class_map.items()))
             yield tuple(random.sample(idxs, 2))
 
     @return_list
     def _negative_pairs():
-        for _ in progress_bar(range(num//2)):
+        for _ in progress_bar(range(num//2), leave=False):
             (c1, idxs1), (c2, idxs2) = random.sample(list(class_map.items()), 2)
             yield (random.choice(idxs1), random.choice(idxs2))
 
     return _positive_pairs() + _negative_pairs()
 
 
 def Pairs(singles: Datasets,  # Used to construct pairs
```

### Comparing `fastai-datasets-0.0.6/fastai_datasets/patches.py` & `fastai-datasets-0.0.7/fastai_datasets/patches.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,25 +30,36 @@
 # %% ../nbs/Core/patches.ipynb 9
 @patch
 def sub_dsets(self: Datasets, indices: Iterable[int]):
     return Datasets(tls=[t.sublist(indices) for t in self.tls])
 
 # %% ../nbs/Core/patches.ipynb 13
 @patch
+def sub_dl(self:DataLoader, indices: Iterable[int]):
+    return self.new(self.dataset.sub_dsets(indices))
+
+# %% ../nbs/Core/patches.ipynb 18
+@patch
 def random_sub_dsets(self: Datasets, size, with_replacement=False, less_ok=False) -> Datasets:
     if size == 0:
         return self.subset([])
     if len(self) < size:
         assert less_ok
         size = len(self)
     sampler = random.choices if with_replacement else random.sample
     indices = sampler(range(len(self)),  k=size)
     return self.sub_dsets(indices)
 
-# %% ../nbs/Core/patches.ipynb 18
+# %% ../nbs/Core/patches.ipynb 21
+@patch
+@delegates(Datasets.random_sub_dsets)
+def random_sub_dl(self: DataLoader, *args, **kwargs):
+    return self.new(self.dataset.random_sub_dsets(*args, **kwargs))
+
+# %% ../nbs/Core/patches.ipynb 25
 @patch
 def subset(self: TfmdLists, i):
     s = self._new(self._get(self.splits[i]), split_idx=i)
     s.splits = [slice(None), []]  # fastai bugfix
     return s
 
 @patch
@@ -71,62 +82,83 @@
         [[i, item] for i, l in enumerate([l1, l2]) for item in l.items],
         tfms=[lambda o: [tfms1, tfms2][o[0]](o[1]), *merged_tfms],
         splits=[L(range_of(l1))[s1] + [i+len(l1) for i in L(range_of(l2))[s2]]
                 for s1, s2 in zip_longest(l1.splits, l2.splits, fillvalue=[])],
         do_setup=False
     )
 
-# %% ../nbs/Core/patches.ipynb 25
+# %% ../nbs/Core/patches.ipynb 32
 @patch
 def __add__(self: Datasets, other: Datasets):
     assert len(self.tls) == len(other.tls)
     return Datasets(tls=[t1 + t2 for t1, t2 in zip(self.tls, other.tls)])
 
-# %% ../nbs/Core/patches.ipynb 30
+# %% ../nbs/Core/patches.ipynb 37
 @patch
 def __sub__(self: Datasets, other: Datasets):
     assert self.tfms == other.tfms
-    assert set(other.items).issubset(self.items)
-    return self.sub_dsets([i for i, o in enumerate(self.items) if o not in set(other.items)])
+    other_items = set(other.items)
+    assert other_items.issubset(self.items)
+    return self.sub_dsets([i for i, o in enumerate(progress_bar(self.items, leave=False)) if o not in other_items])
+
+# %% ../nbs/Core/patches.ipynb 40
+from types import MethodType
+
+@patch
+def __add__(self: DataLoader, other: DataLoader):
+    for k in list(self.__stored_args__.keys()) + self._methods:
+        if k in {'dataset', 'n'}:
+            continue
+        v1 = getattr(self, k)
+        v2 = getattr(other, k)
+        if isinstance(v1, MethodType) and isinstance(v2, MethodType):
+            continue
+        assert v1 == v2, f"Property {k} mismatch: {v1} != {v2}"
+    return self.new(self.dataset + other.dataset)
 
-# %% ../nbs/Core/patches.ipynb 33
+# %% ../nbs/Core/patches.ipynb 45
 @patch(as_prop=True)
 def i2t(self: Datasets):
     assert self.n_inp == len(self.tls) - 1
     return self.tls[-1]
 
-# %% ../nbs/Core/patches.ipynb 35
+# %% ../nbs/Core/patches.ipynb 47
 @patch(as_prop=True)
 def by_target(self: Datasets) -> Dict[int, Datasets]:
     if not hasattr(self, '_by_target'):
-        targets = [int(t) for t in progress_bar(self.i2t)]
+        targets = [int(t) for t in progress_bar(self.i2t, leave=False)]
         class_map = groupby(enumerate(targets), key=1, val=0)
         self._by_target = {self.vocab[c]: self.sub_dsets(indices)
-                           for c, indices in progress_bar(class_map.items())}
+                           for c, indices in progress_bar(class_map.items(), leave=False)}
     return self._by_target
 
-# %% ../nbs/Core/patches.ipynb 37
+# %% ../nbs/Core/patches.ipynb 50
+@patch(as_prop=True)
+def by_target(self: DataLoader) -> Dict[int, DataLoader]:
+    return {k: self.new(v) for k, v in self.dataset.by_target.items()}
+
+# %% ../nbs/Core/patches.ipynb 52
 import matplotlib.pyplot as plt
 
 @patch()
 def plot_class_distribution(self: Datasets):
     for split in self.subsets:
         plt.bar(self.vocab, [len(split.by_target[c]) for c in self.vocab])
 
-# %% ../nbs/Core/patches.ipynb 41
+# %% ../nbs/Core/patches.ipynb 56
 class ListToTuple(Transform):
     """Transforms lists to tuples, useful for fixing a bug in pytorch (pin_memory turns inner tuples into lists)"""
     def encodes(self, o:list):
         return tuple(o)
 
-# %% ../nbs/Core/patches.ipynb 42
+# %% ../nbs/Core/patches.ipynb 57
 dl_defaults = {'pin_memory': default_device() != torch.device('cpu'), 'device': default_device(),
                'after_item': [ToTensor], 'after_batch': [ListToTuple, IntToFloatTensor]}
 
-# %% ../nbs/Core/patches.ipynb 44
+# %% ../nbs/Core/patches.ipynb 59
 def _dl_args(**kwargs):
     kwargs = deepcopy(kwargs)
     args = deepcopy(dl_defaults)
     for event in ['after_item', 'after_batch']:
         if event in kwargs:
             tfms = kwargs.pop(event)
             args[event] += tfms if isinstance(tfms, Sequence) else [tfms]
@@ -139,33 +171,33 @@
     return self.dataloaders(**_dl_args(**kwargs))
 
 @patch
 def dl(self: Datasets, **kwargs) -> DataLoader:
     """Creates a `DataLoader` (ignoring splits) with defaults from `dl_defaults`"""
     return self._dl_type(self, **_dl_args(**kwargs))
 
-# %% ../nbs/Core/patches.ipynb 46
+# %% ../nbs/Core/patches.ipynb 61
 @patch
 def load(self: Datasets, **kwargs):
     return first(self.dl(bs=len(self), **kwargs))
 
-# %% ../nbs/Core/patches.ipynb 49
+# %% ../nbs/Core/patches.ipynb 64
 @patch(as_prop=True)
 def subsets(self: Datasets) -> TfmdLists:
     """Lazy list of a `Datasets`'s subsets"""
     return TfmdLists(range(self.n_subsets), self.subset)
 
-# %% ../nbs/Core/patches.ipynb 51
+# %% ../nbs/Core/patches.ipynb 66
 @patch
 def resplit(self: Datasets,
             splits: Union[Callable, List[List[int]]]  # a splitter function or a list of splits
             ):
     """Sets the splits of a `Datasets`"""
     if isinstance(splits, Callable):
         splits = splits(self)
     for t in self.tls:
         t.splits = splits
 
-# %% ../nbs/Core/patches.ipynb 54
+# %% ../nbs/Core/patches.ipynb 69
 @patch()
 def __repr__(self: Datasets):
     return '['+'\n'.join(repr(s) for s in self.subsets)+']' if self.split_idx is None else coll_repr(self)
```

### Comparing `fastai-datasets-0.0.6/fastai_datasets/pfr.py` & `fastai-datasets-0.0.7/fastai_datasets/pfr.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.6/fastai_datasets/utils.py` & `fastai-datasets-0.0.7/fastai_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.6/fastai_datasets.egg-info/PKG-INFO` & `fastai-datasets-0.0.7/fastai_datasets.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.6
+Version: 0.0.7
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: fastai-datasets
         ================
@@ -43,20 +43,14 @@
         
         ### Show the class distribution
         
         ``` python
         mnist.plot_class_distribution()
         ```
         
-            <div>
-              <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [10/10 00:00&lt;00:00]
-            </div>
-            
-        
         ![](index_files/figure-commonmark/cell-4-output-2.png)
         
         ### Sample a subset
         
         Whole datasets:
         
         ``` python
@@ -68,45 +62,33 @@
         
         Subset:
         
         ``` python
         mnist.random_sub_dsets(1000)
         ```
         
-            [(#881) [(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(4)),(PILImageBW mode=L size=28x28, TensorCategory(7)),(PILImageBW mode=L size=28x28, TensorCategory(2)),(PILImageBW mode=L size=28x28, TensorCategory(9)),(PILImageBW mode=L size=28x28, TensorCategory(0)),(PILImageBW mode=L size=28x28, TensorCategory(9)),(PILImageBW mode=L size=28x28, TensorCategory(8)),(PILImageBW mode=L size=28x28, TensorCategory(4))...]
-            (#119) [(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(4)),(PILImageBW mode=L size=28x28, TensorCategory(2)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(0)),(PILImageBW mode=L size=28x28, TensorCategory(9)),(PILImageBW mode=L size=28x28, TensorCategory(8)),(PILImageBW mode=L size=28x28, TensorCategory(7)),(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(9))...]]
+            [(#861) [(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(6)),(PILImageBW mode=L size=28x28, TensorCategory(7)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(3)),(PILImageBW mode=L size=28x28, TensorCategory(4)),(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(5)),(PILImageBW mode=L size=28x28, TensorCategory(1))...]
+            (#139) [(PILImageBW mode=L size=28x28, TensorCategory(0)),(PILImageBW mode=L size=28x28, TensorCategory(0)),(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(2)),(PILImageBW mode=L size=28x28, TensorCategory(8)),(PILImageBW mode=L size=28x28, TensorCategory(4)),(PILImageBW mode=L size=28x28, TensorCategory(2)),(PILImageBW mode=L size=28x28, TensorCategory(8)),(PILImageBW mode=L size=28x28, TensorCategory(1)),(PILImageBW mode=L size=28x28, TensorCategory(9))...]]
         
         ### Construct a subset based on classes
         
         ``` python
         cifar10 = CIFAR10()
         dig_frog_bird = cifar10.by_target['dog'] + cifar10.by_target['frog'] + cifar10.by_target['bird']
         dig_frog_bird.dls().show_batch()
         ```
         
-            <div>
-              <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [10/10 00:00&lt;00:00]
-            </div>
-            
-        
         ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         ### Construct a dataset of similarity pairs
         
         ``` python
         Pairs(cifar10, .01).dls().show_batch()
         ```
         
-            <div>
-              <progress value='50' class='' max='50' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [50/50 00:00&lt;00:00]
-            </div>
-            
-        
         ![](index_files/figure-commonmark/cell-8-output-2.png)
         
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `fastai-datasets-0.0.6/fastai_datasets.egg-info/SOURCES.txt` & `fastai-datasets-0.0.7/fastai_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.6/settings.ini` & `fastai-datasets-0.0.7/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastai-datasets
 lib_name = %(repo)s
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastai_datasets
```

### Comparing `fastai-datasets-0.0.6/setup.py` & `fastai-datasets-0.0.7/setup.py`

 * *Files identical despite different names*

