# Comparing `tmp/traker-0.2.0.tar.gz` & `tmp/traker-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traker-0.2.0.tar", last modified: Thu Jun  1 22:52:49 2023, max compression
+gzip compressed data, was "traker-0.2.1.tar", last modified: Fri Jun  2 15:53:31 2023, max compression
```

## Comparing `traker-0.2.0.tar` & `traker-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-01 22:52:49.283594 traker-0.2.0/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-06-01 22:52:49.275594 traker-0.2.0/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3338 2023-04-19 18:30:13.000000 traker-0.2.0/README.md
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-06-01 22:52:49.283594 traker-0.2.0/setup.cfg
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      757 2023-06-01 22:51:27.000000 traker-0.2.0/setup.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-01 22:52:49.107592 traker-0.2.0/tests/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4681 2023-06-01 22:51:27.000000 traker-0.2.0/tests/test_cifar10_accuracy.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3344 2023-06-01 22:51:27.000000 traker-0.2.0/tests/test_cifar2_accuracy.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11693 2023-06-01 22:51:28.000000 traker-0.2.0/tests/test_class.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1898 2023-06-01 22:51:28.000000 traker-0.2.0/tests/test_integration_cifar.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1540 2023-06-01 22:51:28.000000 traker-0.2.0/tests/test_integration_clip.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    10812 2023-04-18 20:47:31.000000 traker-0.2.0/tests/test_jl.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11501 2023-06-01 22:51:28.000000 traker-0.2.0/tests/test_parallel.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3116 2023-04-18 20:47:31.000000 traker-0.2.0/tests/test_rademacher.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-01 22:52:49.207593 traker-0.2.0/trak/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      105 2023-06-01 22:51:28.000000 traker-0.2.0/trak/__init__.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     8187 2023-06-01 22:51:28.000000 traker-0.2.0/trak/gradient_computers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    16829 2023-06-01 22:51:28.000000 traker-0.2.0/trak/modelout_functions.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    12251 2023-06-01 22:51:28.000000 traker-0.2.0/trak/projectors.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    15993 2023-06-01 22:51:29.000000 traker-0.2.0/trak/savers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3880 2023-06-01 22:51:29.000000 traker-0.2.0/trak/score_computers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    21812 2023-06-01 22:51:29.000000 traker-0.2.0/trak/traker.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3019 2023-06-01 22:51:29.000000 traker-0.2.0/trak/utils.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-01 22:52:49.263594 traker-0.2.0/traker.egg-info/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      534 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/SOURCES.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/dependency_links.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       97 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/requires.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        5 2023-06-01 22:52:48.000000 traker-0.2.0/traker.egg-info/top_level.txt
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-02 15:53:31.577504 traker-0.2.1/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-06-02 15:53:31.577504 traker-0.2.1/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3807 2023-06-02 15:02:15.000000 traker-0.2.1/README.md
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-06-02 15:53:31.585504 traker-0.2.1/setup.cfg
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      757 2023-06-02 15:52:25.000000 traker-0.2.1/setup.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-02 15:53:31.369500 traker-0.2.1/tests/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4681 2023-06-02 15:02:16.000000 traker-0.2.1/tests/test_cifar10_accuracy.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3344 2023-06-02 15:02:16.000000 traker-0.2.1/tests/test_cifar2_accuracy.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11693 2023-06-02 15:02:16.000000 traker-0.2.1/tests/test_class.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1898 2023-06-02 15:02:16.000000 traker-0.2.1/tests/test_integration_cifar.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1540 2023-06-02 15:02:16.000000 traker-0.2.1/tests/test_integration_clip.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    10812 2023-06-02 15:02:16.000000 traker-0.2.1/tests/test_jl.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11501 2023-06-02 15:02:16.000000 traker-0.2.1/tests/test_parallel.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3116 2023-06-02 15:02:16.000000 traker-0.2.1/tests/test_rademacher.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-02 15:53:31.473502 traker-0.2.1/trak/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      105 2023-06-02 15:52:40.000000 traker-0.2.1/trak/__init__.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     8187 2023-06-02 15:02:16.000000 traker-0.2.1/trak/gradient_computers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    16848 2023-06-02 15:51:59.000000 traker-0.2.1/trak/modelout_functions.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    12251 2023-06-02 15:02:16.000000 traker-0.2.1/trak/projectors.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    15986 2023-06-02 15:51:59.000000 traker-0.2.1/trak/savers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3880 2023-06-02 15:02:17.000000 traker-0.2.1/trak/score_computers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    21818 2023-06-02 15:51:59.000000 traker-0.2.1/trak/traker.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3019 2023-06-02 15:02:17.000000 traker-0.2.1/trak/utils.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-06-02 15:53:31.549503 traker-0.2.1/traker.egg-info/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-06-02 15:53:31.000000 traker-0.2.1/traker.egg-info/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      534 2023-06-02 15:53:31.000000 traker-0.2.1/traker.egg-info/SOURCES.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-06-02 15:53:31.000000 traker-0.2.1/traker.egg-info/dependency_links.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       97 2023-06-02 15:53:31.000000 traker-0.2.1/traker.egg-info/requires.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        5 2023-06-02 15:53:31.000000 traker-0.2.1/traker.egg-info/top_level.txt
```

### Comparing `traker-0.2.0/README.md` & `traker-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![arXiv](https://img.shields.io/badge/arXiv-2303.14186-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2303.14186)
 [![PyPI version](https://badge.fury.io/py/traker.svg)](https://badge.fury.io/py/traker)
+[![Documentation Status](https://readthedocs.org/projects/trak/badge/?version=latest)](https://trak.readthedocs.io/en/latest/?badge=latest)
 
 # TRAK: Attributing Model Behavior at Scale
 
 [[docs & tutorials]](https://trak.readthedocs.io/en/latest/)
 [[blog post]](https://gradientscience.org/trak/)
 [[website]](https://trak.csail.mit.edu)
 
@@ -14,16 +15,16 @@
 Computing  data attribution with  TRAK is 2-3 orders of magnitude cheaper than
 comparably effective methods, e.g., see our evaluation on:
 
 ![Main figure](/docs/assets/main_figure.png)
 
 ## Usage
 
-[[quickstart]](https://trak.readthedocs.io/en/latest/quickstart.html)
-[[pre-computed TRAK scores for CIFAR-10]](https://colab.research.google.com/drive/1Mlpzno97qpI3UC1jpOATXEHPD-lzn9Wg?usp=sharing)
+- [quickstart (tutorial & notebook)](https://trak.readthedocs.io/en/latest/quickstart.html)
+- [pre-computed TRAK scores for CIFAR-10 (Google Colab notebook)](https://colab.research.google.com/drive/1Mlpzno97qpI3UC1jpOATXEHPD-lzn9Wg?usp=sharing)
 
 Check [our docs](https://trak.readthedocs.io/en/latest/) for more detailed examples and
 tutorials on how to use `TRAK`.  Below, we provide a brief blueprint of using `TRAK`'s API to compute attribution scores.
 
 ### Make a `TRAKer` instance
 
 ```python
@@ -48,31 +49,36 @@
 
 ### Compute `TRAK` scores for target examples
 
 ```python
 targets_loader = ...
 
 for model_id, checkpoint in enumerate(checkpoints):
-  traker.start_scoring_checkpoint(ckeckpoint, model_id=model_id, num_targets=...)
+  traker.start_scoring_checkpoint(ckeckpoint,
+                                  model_id=model_id,
+                                  exp_name='test',
+                                  num_targets=...)
   for batch in targets_loader:
     traker.score(batch=batch, ...)
 
-scores = traker.finalize_scores()
+scores = traker.finalize_scores(exp_name='test')
 ```
+Check out the [quickstart](https://trak.readthedocs.io/en/latest/quickstart.html) for a complete ready-to-run example notebook.
+
 
 ## Examples
 You can find several end-to-end examples in the `examples/` directory.
 
 ## Citation
 If you use this code in your work, please cite using the following BibTeX entry:
 ```
 @inproceedings{park2023trak,
   title = {TRAK: Attributing Model Behavior at Scale},
   author = {Sung Min Park and Kristian Georgiev and Andrew Ilyas and Guillaume Leclerc and Aleksander Madry},
-  booktitle = {Arxiv preprint arXiv:2303.14186},
+  booktitle = {International Conference on Machine Learning (ICML)},
   year = {2023}
 }
 ```
 
 ## Installation
 
 To install the version of our package which contains a fast, custom `CUDA`
```

### Comparing `traker-0.2.0/setup.py` & `traker-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(name="traker",
-      version="0.2.0",
+      version="0.2.1",
       description="TRAK: Attributing Model Behavior at Scale",
       long_description="Check https://trak.csail.mit.edu/ to learn more about TRAK",
       author="MadryLab",
       author_email='trak@mit.edu',
       license_files=('LICENSE.txt', ),
       packages=['trak'],
       install_requires=[
```

### Comparing `traker-0.2.0/tests/test_cifar10_accuracy.py` & `traker-0.2.1/tests/test_cifar10_accuracy.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/tests/test_cifar2_accuracy.py` & `traker-0.2.1/tests/test_cifar2_accuracy.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/tests/test_class.py` & `traker-0.2.1/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/tests/test_integration_cifar.py` & `traker-0.2.1/tests/test_integration_cifar.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/tests/test_integration_clip.py` & `traker-0.2.1/tests/test_integration_clip.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/tests/test_jl.py` & `traker-0.2.1/tests/test_jl.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/tests/test_parallel.py` & `traker-0.2.1/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/tests/test_rademacher.py` & `traker-0.2.1/tests/test_rademacher.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/trak/gradient_computers.py` & `traker-0.2.1/trak/gradient_computers.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/trak/modelout_functions.py` & `traker-0.2.1/trak/modelout_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,17 +385,17 @@
                    input_id: Tensor,
                    token_type_id: Tensor,
                    attention_mask: Tensor,
                    label: Tensor,
                    ) -> Tensor:
         logits = ch.func.functional_call(model,
                                          (weights, buffers),
-                                         input_id.unsqueeze(0),
-                                         token_type_id.unsqueeze(0),
-                                         attention_mask.unsqueeze(0))
+                                         args=(input_id.unsqueeze(0),
+                                               token_type_id.unsqueeze(0),
+                                               attention_mask.unsqueeze(0)))
         bindex = ch.arange(logits.shape[0]).to(logits.device, non_blocking=False)
         logits_correct = logits[bindex, label.unsqueeze(0)]
 
         cloned_logits = logits.clone()
         cloned_logits[bindex, label.unsqueeze(0)] = ch.tensor(-ch.inf, device=logits.device, dtype=logits.dtype)
 
         margins = logits_correct - cloned_logits.logsumexp(dim=-1)
```

### Comparing `traker-0.2.0/trak/projectors.py` & `traker-0.2.1/trak/projectors.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/trak/savers.py` & `traker-0.2.1/trak/savers.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
         for name, (path, shape, dtype) in to_load.items():
             self.current_store[name] = self._load(path, shape, mode, dtype)
 
     def save_scores(self, exp_name):
         assert self.current_experiment_name == exp_name
         prefix = self.save_dir.joinpath('scores')
-        self.logger.info(f'Saving scores in {prefix}/scores/{exp_name}.mmap')
+        self.logger.info(f'Saving scores in {prefix}/{exp_name}.mmap')
         self.current_store[f'{exp_name}_scores'].flush()
         self.experiments[exp_name]['scores_finalized'] = True
 
     def del_grads(self, model_id):
         grads_file = self.save_dir.joinpath(str(model_id)).joinpath('grads.mmap')
 
         # delete grads memmap
```

### Comparing `traker-0.2.0/trak/score_computers.py` & `traker-0.2.1/trak/score_computers.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/trak/traker.py` & `traker-0.2.1/trak/traker.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,20 +464,20 @@
                 self.logger.warning(f'Model ID {self.saver.current_model_id} not finalized, cannot score')
                 continue
 
             g = ch.as_tensor(self.saver.current_store['features'], device=self.device)
             g_target = ch.as_tensor(self.saver.current_store[f'{exp_name}_grads'],
                                     device=self.device)
 
-            _scores += self.score_computer.get_scores(g, g_target).cpu().clone().detach().numpy()
+            _scores[:] += self.score_computer.get_scores(g, g_target).cpu().clone().detach().numpy()
 
             _avg_out_to_losses += self.saver.current_store['out_to_loss']
             _completed[j] = True
 
         _num_models_used = float(sum(_completed))
-        _scores = (_scores / _num_models_used) * (_avg_out_to_losses / _num_models_used)
+        _scores[:] = (_scores / _num_models_used) * (_avg_out_to_losses / _num_models_used)
 
         self.logger.debug(f'Scores dtype is {_scores.dtype}')
         self.saver.save_scores(exp_name)
         self.scores = _scores
 
         return self.scores
```

### Comparing `traker-0.2.0/trak/utils.py` & `traker-0.2.1/trak/utils.py`

 * *Files identical despite different names*

### Comparing `traker-0.2.0/traker.egg-info/SOURCES.txt` & `traker-0.2.1/traker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

