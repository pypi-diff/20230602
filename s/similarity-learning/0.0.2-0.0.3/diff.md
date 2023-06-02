# Comparing `tmp/similarity-learning-0.0.2.tar.gz` & `tmp/similarity-learning-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarity-learning-0.0.2.tar", last modified: Sat May 20 11:12:58 2023, max compression
+gzip compressed data, was "similarity-learning-0.0.3.tar", last modified: Fri Jun  2 13:42:28 2023, max compression
```

## Comparing `similarity-learning-0.0.2.tar` & `similarity-learning-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:12:58.404034 similarity-learning-0.0.2/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-18 07:33:16.000000 similarity-learning-0.0.2/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-01-20 02:50:04.000000 similarity-learning-0.0.2/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4124 2023-05-20 11:12:58.404034 similarity-learning-0.0.2/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2434 2023-05-20 11:12:23.000000 similarity-learning-0.0.2/README.md
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1026 2023-05-20 11:11:56.000000 similarity-learning-0.0.2/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-20 11:12:58.404034 similarity-learning-0.0.2/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-01-20 02:50:04.000000 similarity-learning-0.0.2/setup.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:12:58.400035 similarity-learning-0.0.2/similarity_learning/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    10970 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       72 2023-04-18 22:10:56.000000 similarity-learning-0.0.2/similarity_learning/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1064 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/facenet.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1255 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/feature_space_plotting.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1492 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/pair_matching.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2408 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/siamese.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5459 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/utils.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:12:58.404034 similarity-learning-0.0.2/similarity_learning.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4124 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      617 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       81 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-18 07:42:39.000000 similarity-learning-0.0.2/similarity_learning.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       64 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       20 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/top_level.txt
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-18 07:33:16.000000 similarity-learning-0.0.3/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-01-20 02:50:04.000000 similarity-learning-0.0.3/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3444 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1898 2023-05-20 12:47:49.000000 similarity-learning-0.0.3/README.md
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1026 2023-06-02 13:41:48.000000 similarity-learning-0.0.3/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-01-20 02:50:04.000000 similarity-learning-0.0.3/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/similarity_learning/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    11103 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      133 2023-05-23 07:24:39.000000 similarity-learning-0.0.3/similarity_learning/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1064 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/facenet.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1255 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/feature_space_plotting.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1505 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/pair_matching.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2594 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/siamese.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5486 2023-06-02 13:42:16.000000 similarity-learning-0.0.3/similarity_learning/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-02 13:42:28.727179 similarity-learning-0.0.3/similarity_learning.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3444 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      617 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       81 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-18 07:42:39.000000 similarity-learning-0.0.3/similarity_learning.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       64 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       20 2023-06-02 13:42:28.000000 similarity-learning-0.0.3/similarity_learning.egg-info/top_level.txt
```

### Comparing `similarity-learning-0.0.2/LICENSE` & `similarity-learning-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.2/PKG-INFO` & `similarity-learning-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-learning
-Version: 0.0.2
+Version: 0.0.3
 Summary: A fastai based framework for similarity learning
 Home-page: https://github.com/Irad-Zehavi/similarity-learning
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: similarity-learning
         ================
@@ -41,80 +41,62 @@
         
         ``` python
         pairs = Pairs(Imagenette(160), .1)
         dls = pairs.dls(after_item=Resize(128),
                         after_batch=Normalize.from_stats(*imagenet_stats))
         ```
         
-            <div>
-              <progress value='196' class='' max='196' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [196/196 00:00&lt;00:00]
-            </div>
-            
-        
         To get quick results, we can use the body of a pretrained model as a
         backbone for our Siamese neural network:
         
         ``` python
         classifier = resnet34(weights=ResNet34_Weights.DEFAULT)
         siamese = ThresholdSiamese(create_body(model=classifier, cut=-1)).to(dls.device)
         siamese.fit_threshold(dls.train)
         ```
         
-            <div>
-              <progress value='14' class='' max='14' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [14/14 00:05&lt;00:00]
-            </div>
-            
-        
-            (1.0299999713897705, 0.8895089626312256)
+            (1.0399999618530273, 0.8839285969734192)
         
         Let’s see how good it is:
         
         ``` python
         learn = Learner(dls, siamese, metrics=accuracy)
         learn.validate()
         ```
         
-            (#2) [0.541471004486084,0.9005101919174194]
+            (#2) [0.5608958601951599,0.8239796161651611]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         Not bad, but we can do better with finetuning:
         
         ``` python
         learn.fit(5, 1e-4)
         learn.validate()
         ```
         
-            (#2) [0.2768465280532837,0.9464285969734192]
+            (#2) [0.2924809157848358,0.9387755393981934]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-9-output-2.png)
         
         We can also consider the distribution of feature-space distances
         compared to the decision threshold:
         
         ``` python
         siamese.plot_distance_histogram(dls.valid)
         ```
         
-            <div>
-              <progress value='7' class='' max='7' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [7/7 00:02&lt;00:00]
-            </div>
-            
-        
         ![](index_files/figure-commonmark/cell-10-output-2.png)
         
         See the rest of the docs for more examples, including more
         visualizations, comparison of loss functions, and facial recognition.
         
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `similarity-learning-0.0.2/README.md` & `similarity-learning-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -33,77 +33,59 @@
 
 ``` python
 pairs = Pairs(Imagenette(160), .1)
 dls = pairs.dls(after_item=Resize(128),
                 after_batch=Normalize.from_stats(*imagenet_stats))
 ```
 
-    <div>
-      <progress value='196' class='' max='196' style='width:300px; height:20px; vertical-align: middle;'></progress>
-      100.00% [196/196 00:00&lt;00:00]
-    </div>
-    
-
 To get quick results, we can use the body of a pretrained model as a
 backbone for our Siamese neural network:
 
 ``` python
 classifier = resnet34(weights=ResNet34_Weights.DEFAULT)
 siamese = ThresholdSiamese(create_body(model=classifier, cut=-1)).to(dls.device)
 siamese.fit_threshold(dls.train)
 ```
 
-    <div>
-      <progress value='14' class='' max='14' style='width:300px; height:20px; vertical-align: middle;'></progress>
-      100.00% [14/14 00:05&lt;00:00]
-    </div>
-    
-
-    (1.0299999713897705, 0.8895089626312256)
+    (1.0399999618530273, 0.8839285969734192)
 
 Let’s see how good it is:
 
 ``` python
 learn = Learner(dls, siamese, metrics=accuracy)
 learn.validate()
 ```
 
-    (#2) [0.541471004486084,0.9005101919174194]
+    (#2) [0.5608958601951599,0.8239796161651611]
 
 ``` python
 learn.show_results()
 ```
 
 ![](index_files/figure-commonmark/cell-7-output-2.png)
 
 Not bad, but we can do better with finetuning:
 
 ``` python
 learn.fit(5, 1e-4)
 learn.validate()
 ```
 
-    (#2) [0.2768465280532837,0.9464285969734192]
+    (#2) [0.2924809157848358,0.9387755393981934]
 
 ``` python
 learn.show_results()
 ```
 
 ![](index_files/figure-commonmark/cell-9-output-2.png)
 
 We can also consider the distribution of feature-space distances
 compared to the decision threshold:
 
 ``` python
 siamese.plot_distance_histogram(dls.valid)
 ```
 
-    <div>
-      <progress value='7' class='' max='7' style='width:300px; height:20px; vertical-align: middle;'></progress>
-      100.00% [7/7 00:02&lt;00:00]
-    </div>
-    
-
 ![](index_files/figure-commonmark/cell-10-output-2.png)
 
 See the rest of the docs for more examples, including more
 visualizations, comparison of loss functions, and facial recognition.
```

### Comparing `similarity-learning-0.0.2/settings.ini` & `similarity-learning-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = similarity-learning
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = similarity_learning
```

### Comparing `similarity-learning-0.0.2/setup.py` & `similarity-learning-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.2/similarity_learning/_modidx.py` & `similarity-learning-0.0.3/similarity_learning/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,20 @@
                                                                                                        'similarity_learning/siamese.py'),
                                              'similarity_learning.siamese.ContrastiveLoss.__init__': ( 'siamese.html#contrastiveloss.__init__',
                                                                                                        'similarity_learning/siamese.py'),
                                              'similarity_learning.siamese.DistanceSiamese': ( 'siamese.html#distancesiamese',
                                                                                               'similarity_learning/siamese.py'),
                                              'similarity_learning.siamese.DistanceSiamese.__init__': ( 'siamese.html#distancesiamese.__init__',
                                                                                                        'similarity_learning/siamese.py'),
+                                             'similarity_learning.siamese.DistanceSiamese._hist': ( 'siamese.html#distancesiamese._hist',
+                                                                                                    'similarity_learning/siamese.py'),
                                              'similarity_learning.siamese.DistanceSiamese.forward': ( 'siamese.html#distancesiamese.forward',
                                                                                                       'similarity_learning/siamese.py'),
                                              'similarity_learning.siamese.DistanceSiamese.plot_distance_histogram': ( 'siamese.html#distancesiamese.plot_distance_histogram',
                                                                                                                       'similarity_learning/siamese.py'),
-                                             'similarity_learning.siamese._hist': ('siamese.html#_hist', 'similarity_learning/siamese.py'),
                                              'similarity_learning.siamese.normalized_squared_euclidean_distance': ( 'siamese.html#normalized_squared_euclidean_distance',
                                                                                                                     'similarity_learning/siamese.py')},
             'similarity_learning.utils': { 'similarity_learning.utils.ExperimentalResults': ( 'utils.html#experimentalresults',
                                                                                               'similarity_learning/utils.py'),
                                            'similarity_learning.utils.ExperimentalResults.collated_stats': ( 'utils.html#experimentalresults.collated_stats',
                                                                                                              'similarity_learning/utils.py'),
                                            'similarity_learning.utils.ExperimentalResults.plot_stats': ( 'utils.html#experimentalresults.plot_stats',
```

### Comparing `similarity-learning-0.0.2/similarity_learning/facenet.py` & `similarity-learning-0.0.3/similarity_learning/facenet.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.2/similarity_learning/feature_space_plotting.py` & `similarity-learning-0.0.3/similarity_learning/feature_space_plotting.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.2/similarity_learning/pair_matching.py` & `similarity-learning-0.0.3/similarity_learning/pair_matching.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,11 +32,11 @@
 
 # %% ../nbs/pair_matching.ipynb 10
 @patch
 def fit_threshold(self: ThresholdSiamese, train_dl: DataLoader):
     """Picks a threshold that maximizes the accuracy on a dataloader"""
     self.eval().to(train_dl.device)
     with torch.no_grad():
-        distances, targets = zip(*((self.distance(x), y) for x, y in progress_bar(train_dl)))
+        distances, targets = zip(*((self.distance(x), y) for x, y in progress_bar(train_dl, leave=False)))
         distances, targets = torch.cat(distances).as_subclass(Tensor), torch.cat(targets).as_subclass(Tensor)
 
         return self.threshold.fit(distances, targets)
```

### Comparing `similarity-learning-0.0.2/similarity_learning/siamese.py` & `similarity-learning-0.0.3/similarity_learning/siamese.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,25 +47,33 @@
 
 # %% ../nbs/siamese.ipynb 4
 from matplotlib.ticker import PercentFormatter
 from fastprogress.fastprogress import *
 import numpy as np
 
 @patch
-def plot_distance_histogram(self: DistanceSiamese, pairs_dl: TfmdDL, label='Distance'):
-    """Plots a histogram of intra-class and inter-class distances"""
-    self.eval().to(pairs_dl.device)
-    
-    with torch.no_grad():
-        processed_batches = [(self(x), y) for x, y in progress_bar(pairs_dl)]
-        distances, targets = [torch.cat(o).cpu().numpy() for o in zip(*processed_batches)]
+def plot_distance_histogram(self: DistanceSiamese, pairs_dls: Union[TfmdDL, Dict[str, TfmdDL]], label='Distance'):
+    """Plots a histogram of intra-class and inter-class distances"""    
+    if isinstance(pairs_dls, DataLoader):
+        pairs_dls = {
+            'Intra-Class': pairs_dls.by_target['Same'],
+            'Inter-Class': pairs_dls.by_target['Not Same']
+        }
+
+    self.eval()
 
-    _hist(distances[targets==1], 'Intra-Class')
-    _hist(distances[targets==0], 'Inter-Class')
+    with torch.no_grad():
+        for label, dl in pairs_dls.items():
+            self._hist(dl, label)
     
     plt.legend()
     plt.xlabel(label)
 
-def _hist(distances, label=None):
+
+@patch
+def _hist(self: DistanceSiamese, dl, label):
+    self.to(dl.device)
+    processed_batches = [self(x) for x, _ in progress_bar(dl, leave=False)]
+    distances = torch.cat(processed_batches).cpu().numpy()
     weights = np.ones_like(distances) / len(distances)  # normalization for percentage ticks
     plt.hist(distances, label=label, alpha=.5, edgecolor='black', lw=1, weights=weights)
     plt.gca().yaxis.set_major_formatter(PercentFormatter(1))
```

### Comparing `similarity-learning-0.0.2/similarity_learning/utils.py` & `similarity-learning-0.0.3/similarity_learning/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 
     @property
     def collated_stats(self):
         return {k: v.numpy() for k, v in default_collate(self.stats).items()}
 
     def plot_stats(self):
         fig, axs = plt.subplots(len(self.collated_stats), sharex=True)
+        fig.tight_layout()
         for ax, (stat_name, stat_values) in zip(axs, self.collated_stats.items()):
             ax.set_title(stat_name)
 
             min_val, max_val = min(stat_values), max(stat_values)
             val_range = max_val - min_val
             ax.set_ylim(min_val - .1*val_range, max_val + .1*val_range)
```

### Comparing `similarity-learning-0.0.2/similarity_learning.egg-info/PKG-INFO` & `similarity-learning-0.0.3/similarity_learning.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-learning
-Version: 0.0.2
+Version: 0.0.3
 Summary: A fastai based framework for similarity learning
 Home-page: https://github.com/Irad-Zehavi/similarity-learning
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: similarity-learning
         ================
@@ -41,80 +41,62 @@
         
         ``` python
         pairs = Pairs(Imagenette(160), .1)
         dls = pairs.dls(after_item=Resize(128),
                         after_batch=Normalize.from_stats(*imagenet_stats))
         ```
         
-            <div>
-              <progress value='196' class='' max='196' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [196/196 00:00&lt;00:00]
-            </div>
-            
-        
         To get quick results, we can use the body of a pretrained model as a
         backbone for our Siamese neural network:
         
         ``` python
         classifier = resnet34(weights=ResNet34_Weights.DEFAULT)
         siamese = ThresholdSiamese(create_body(model=classifier, cut=-1)).to(dls.device)
         siamese.fit_threshold(dls.train)
         ```
         
-            <div>
-              <progress value='14' class='' max='14' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [14/14 00:05&lt;00:00]
-            </div>
-            
-        
-            (1.0299999713897705, 0.8895089626312256)
+            (1.0399999618530273, 0.8839285969734192)
         
         Let’s see how good it is:
         
         ``` python
         learn = Learner(dls, siamese, metrics=accuracy)
         learn.validate()
         ```
         
-            (#2) [0.541471004486084,0.9005101919174194]
+            (#2) [0.5608958601951599,0.8239796161651611]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         Not bad, but we can do better with finetuning:
         
         ``` python
         learn.fit(5, 1e-4)
         learn.validate()
         ```
         
-            (#2) [0.2768465280532837,0.9464285969734192]
+            (#2) [0.2924809157848358,0.9387755393981934]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-9-output-2.png)
         
         We can also consider the distribution of feature-space distances
         compared to the decision threshold:
         
         ``` python
         siamese.plot_distance_histogram(dls.valid)
         ```
         
-            <div>
-              <progress value='7' class='' max='7' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [7/7 00:02&lt;00:00]
-            </div>
-            
-        
         ![](index_files/figure-commonmark/cell-10-output-2.png)
         
         See the rest of the docs for more examples, including more
         visualizations, comparison of loss functions, and facial recognition.
         
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `similarity-learning-0.0.2/similarity_learning.egg-info/SOURCES.txt` & `similarity-learning-0.0.3/similarity_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

