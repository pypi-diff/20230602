# Comparing `tmp/flaxsr-0.0.4.tar.gz` & `tmp/flaxsr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaxsr-0.0.4.tar", last modified: Thu Jun  1 08:20:35 2023, max compression
+gzip compressed data, was "flaxsr-0.0.5.tar", last modified: Fri Jun  2 13:53:12 2023, max compression
```

## Comparing `flaxsr-0.0.4.tar` & `flaxsr-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)    11313 2023-05-12 09:22:40.000000 flaxsr-0.0.4/LICENSE
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2807 2023-06-01 08:20:35.954687 flaxsr-0.0.4/PKG-INFO
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2183 2023-06-01 08:16:14.000000 flaxsr-0.0.4/README.md
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      111 2023-05-17 15:18:45.000000 flaxsr-0.0.4/flaxsr/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      661 2023-05-12 10:02:07.000000 flaxsr-0.0.4/flaxsr/_utils.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/layers/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      179 2023-05-12 09:22:40.000000 flaxsr-0.0.4/flaxsr/layers/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1651 2023-05-16 13:28:13.000000 flaxsr-0.0.4/flaxsr/layers/stochastic.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1673 2023-05-16 13:28:27.000000 flaxsr-0.0.4/flaxsr/layers/upscale.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/losses/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      921 2023-06-01 00:47:20.000000 flaxsr-0.0.4/flaxsr/losses/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4441 2023-05-31 15:44:50.000000 flaxsr-0.0.4/flaxsr/losses/adversarial_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2295 2023-05-31 15:35:59.000000 flaxsr-0.0.4/flaxsr/losses/perceptual_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1664 2023-05-31 15:35:14.000000 flaxsr-0.0.4/flaxsr/losses/pixel_wise_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4390 2023-06-01 00:50:10.000000 flaxsr-0.0.4/flaxsr/losses/utils.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/models/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      355 2023-05-12 09:22:40.000000 flaxsr-0.0.4/flaxsr/models/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3749 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/edsr.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      922 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/espcn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1138 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/fsrcnn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     6677 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/nafssr.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      994 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/ncnet.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1078 2023-05-12 09:49:43.000000 flaxsr-0.0.4/flaxsr/models/srcnn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4129 2023-05-30 16:42:22.000000 flaxsr-0.0.4/flaxsr/models/srgan.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      954 2023-05-12 09:50:48.000000 flaxsr-0.0.4/flaxsr/models/vdsr.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/training/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      149 2023-06-01 05:21:42.000000 flaxsr-0.0.4/flaxsr/training/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      503 2023-06-01 00:48:20.000000 flaxsr-0.0.4/flaxsr/training/train_states.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1345 2023-06-01 05:25:08.000000 flaxsr-0.0.4/flaxsr/training/train_step.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr.egg-info/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2807 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/PKG-INFO
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      745 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/SOURCES.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        1 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/dependency_links.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       46 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/requires.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        7 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/top_level.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       38 2023-06-01 08:20:35.954687 flaxsr-0.0.4/setup.cfg
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      961 2023-06-01 08:15:31.000000 flaxsr-0.0.4/setup.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)    11313 2023-05-12 09:22:40.000000 flaxsr-0.0.5/LICENSE
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1948 2023-06-02 13:53:12.175251 flaxsr-0.0.5/PKG-INFO
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1324 2023-06-02 13:51:10.000000 flaxsr-0.0.5/README.md
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      111 2023-05-17 15:18:45.000000 flaxsr-0.0.5/flaxsr/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      661 2023-05-12 10:02:07.000000 flaxsr-0.0.5/flaxsr/_utils.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/layers/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      179 2023-05-12 09:22:40.000000 flaxsr-0.0.5/flaxsr/layers/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1651 2023-05-16 13:28:13.000000 flaxsr-0.0.5/flaxsr/layers/stochastic.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1673 2023-05-16 13:28:27.000000 flaxsr-0.0.5/flaxsr/layers/upscale.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/losses/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1384 2023-06-02 13:50:17.000000 flaxsr-0.0.5/flaxsr/losses/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4806 2023-06-02 13:04:49.000000 flaxsr-0.0.5/flaxsr/losses/adversarial_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2495 2023-06-02 12:29:07.000000 flaxsr-0.0.5/flaxsr/losses/perceptual_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2229 2023-06-02 12:17:52.000000 flaxsr-0.0.5/flaxsr/losses/pixel_wise_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3190 2023-06-02 13:06:59.000000 flaxsr-0.0.5/flaxsr/losses/utils.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/models/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      392 2023-06-02 11:31:44.000000 flaxsr-0.0.5/flaxsr/models/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3749 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/edsr.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      922 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/espcn.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1138 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/fsrcnn.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     6677 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/nafssr.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      994 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/ncnet.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1078 2023-05-12 09:49:43.000000 flaxsr-0.0.5/flaxsr/models/srcnn.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4161 2023-06-02 11:35:45.000000 flaxsr-0.0.5/flaxsr/models/srgan.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      954 2023-05-12 09:50:48.000000 flaxsr-0.0.5/flaxsr/models/vdsr.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/training/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      149 2023-06-01 05:21:42.000000 flaxsr-0.0.5/flaxsr/training/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      503 2023-06-01 00:48:20.000000 flaxsr-0.0.5/flaxsr/training/train_states.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1345 2023-06-01 05:25:08.000000 flaxsr-0.0.5/flaxsr/training/train_step.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr.egg-info/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1948 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/PKG-INFO
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      745 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        1 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       46 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/requires.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        7 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/top_level.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       38 2023-06-02 13:53:12.175251 flaxsr-0.0.5/setup.cfg
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      961 2023-06-02 13:52:56.000000 flaxsr-0.0.5/setup.py
```

### Comparing `flaxsr-0.0.4/LICENSE` & `flaxsr-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/PKG-INFO` & `flaxsr-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaxsr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Super Resolution models with Jax/Flax
 Home-page: https://github.com/dslisleedh/FlaxSR
 Author: dslisleedh
 Author-email: dslisleedh@gmail.com
 Project-URL: Bug Tracker, https://github.com/dslisleedh/FlaxSR/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,74 +23,33 @@
 
 ### Install
 ```shell
 pip install flaxsr
 ```
 
 ### Usage
- - Models
-```python
-import flaxsr
-from flaxsr.models import VDSR
-import jax
-import jax.numpy as jnp
-import numpy as np
-
-inputs = jnp.ones((16, 256, 256, 3))
-key = jax.random.PRNGKey(42)
-model = VDSR(n_filters=64, n_blocks=20, scale=4)
-params = model.init(key, inputs)
-outputs = model.apply(params, inputs)
-print(outputs.shape)
-
-# Or you can use flaxsr.get function
-model_get = flaxsr.get("models", "vdsr", n_filters=64, n_blocks=20, scale=4)
-params_get = model_get.init(key, inputs)
-outputs_get = model_get.apply(params_get, inputs)
-print(outputs_get.shape)
-
-np.allclose(outputs, outputs_get)
-```
-
- - Losses
-```python
-import flaxsr
-import jax
-import jax.numpy as jnp
-import numpy as np
-
-hr = jnp.asarray(np.random.normal((16, 256, 256, 3)))
-sr = jnp.asarray(np.random.normal((16, 256, 256, 3)))
-
-loss = flaxsr.losses.l1_loss(hr, sr, "mean")
-
-# Or you can use flaxsr.get function
-metric = flaxsr.get("losses", "l1", "mean")
-loss_get = metric(hr, sr)
-
-np.allclose(loss, loss_get)
-```
-
 <b> You can easily load model/losses and train model using custom train_states. </b>
 
  - Train example
 ```python
 import flaxsr
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 
 model_kwargs = {
     'n_filters': 64, 'n_blocks': 8, 'scale': 4
 }
-model = flaxsr.get("models", "vdsr", **model_kwargs)
-losses = flaxsr.losses.LossWrapper(
-    losses=['l1', 'l2'], weights=[1.0, 1.0]
-)
+model = flaxsr.get("models", "vdsr", **model_kwargs)  # This equals flaxsr.models.VDSR(**model_kwargs)
+losses = [
+    flaxsr.losses.L1Loss(reduce='sum'),
+    flaxsr.get('losses', 'vgg', feats_from=(6, 8, 14,), before_act=False, reduce='mean')
+]
+loss_weights = (.1, 1.)
 params = model.init(jax.random.PRNGKey(0), jnp.ones((1, 8, 8, 3), dtype=jnp.float32))
 tx = optax.adam(1e-3)
 
 state = flaxsr.training.TrainState.create(
     apply_fn=model.apply, params=params, tx=tx, losses=losses
 )
 
@@ -109,8 +68,7 @@
  - SRCNN
  - FSRCNN
  - ESPCN
  - VDSR
  - EDSR, MDSR,
  - NCNet
  - SRResNet(SRGAN will be implemented in future)
- - NAFSSR
```

### Comparing `flaxsr-0.0.4/README.md` & `flaxsr-0.0.5/flaxsr.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,55 @@
+Metadata-Version: 2.1
+Name: flaxsr
+Version: 0.0.5
+Summary: Super Resolution models with Jax/Flax
+Home-page: https://github.com/dslisleedh/FlaxSR
+Author: dslisleedh
+Author-email: dslisleedh@gmail.com
+Project-URL: Bug Tracker, https://github.com/dslisleedh/FlaxSR/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # FlaxSR
 
 Super Resolution models with Jax/Flax
 
 ## HOW TO USE
 
 ### Install
 ```shell
 pip install flaxsr
 ```
 
 ### Usage
- - Models
-```python
-import flaxsr
-from flaxsr.models import VDSR
-import jax
-import jax.numpy as jnp
-import numpy as np
-
-inputs = jnp.ones((16, 256, 256, 3))
-key = jax.random.PRNGKey(42)
-model = VDSR(n_filters=64, n_blocks=20, scale=4)
-params = model.init(key, inputs)
-outputs = model.apply(params, inputs)
-print(outputs.shape)
-
-# Or you can use flaxsr.get function
-model_get = flaxsr.get("models", "vdsr", n_filters=64, n_blocks=20, scale=4)
-params_get = model_get.init(key, inputs)
-outputs_get = model_get.apply(params_get, inputs)
-print(outputs_get.shape)
-
-np.allclose(outputs, outputs_get)
-```
-
- - Losses
-```python
-import flaxsr
-import jax
-import jax.numpy as jnp
-import numpy as np
-
-hr = jnp.asarray(np.random.normal((16, 256, 256, 3)))
-sr = jnp.asarray(np.random.normal((16, 256, 256, 3)))
-
-loss = flaxsr.losses.l1_loss(hr, sr, "mean")
-
-# Or you can use flaxsr.get function
-metric = flaxsr.get("losses", "l1", "mean")
-loss_get = metric(hr, sr)
-
-np.allclose(loss, loss_get)
-```
-
 <b> You can easily load model/losses and train model using custom train_states. </b>
 
  - Train example
 ```python
 import flaxsr
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 
 model_kwargs = {
     'n_filters': 64, 'n_blocks': 8, 'scale': 4
 }
-model = flaxsr.get("models", "vdsr", **model_kwargs)
-losses = flaxsr.losses.LossWrapper(
-    losses=['l1', 'l2'], weights=[1.0, 1.0]
-)
+model = flaxsr.get("models", "vdsr", **model_kwargs)  # This equals flaxsr.models.VDSR(**model_kwargs)
+losses = [
+    flaxsr.losses.L1Loss(reduce='sum'),
+    flaxsr.get('losses', 'vgg', feats_from=(6, 8, 14,), before_act=False, reduce='mean')
+]
+loss_weights = (.1, 1.)
 params = model.init(jax.random.PRNGKey(0), jnp.ones((1, 8, 8, 3), dtype=jnp.float32))
 tx = optax.adam(1e-3)
 
 state = flaxsr.training.TrainState.create(
     apply_fn=model.apply, params=params, tx=tx, losses=losses
 )
 
@@ -92,8 +68,7 @@
  - SRCNN
  - FSRCNN
  - ESPCN
  - VDSR
  - EDSR, MDSR,
  - NCNet
  - SRResNet(SRGAN will be implemented in future)
- - NAFSSR
```

### Comparing `flaxsr-0.0.4/flaxsr/_utils.py` & `flaxsr-0.0.5/flaxsr/_utils.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/layers/stochastic.py` & `flaxsr-0.0.5/flaxsr/layers/stochastic.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/layers/upscale.py` & `flaxsr-0.0.5/flaxsr/layers/upscale.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/losses/__init__.py` & `flaxsr-0.0.5/flaxsr/losses/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 from .pixel_wise_losses import (
     l1_loss as l1_loss,
+    L1Loss as L1Loss,
     l2_loss as l2_loss,
+    L2Loss as L2Loss,
     charbonnier_loss as charbonnier_loss,
+    CharbonnierLoss as CharbonnierLoss,
 )
 from .perceptual_losses import (
     vgg_loss as vgg_loss,
+    VGGLoss as VGGLoss,
 )
 from .adversarial_losses import (
     minmax_discriminator_loss as minmax_discriminator_loss,
     minmax_generator_loss as minmax_generator_loss,
+    MinmaxDiscriminatorLoss as MinmaxDiscriminatorLoss,
+    MinmaxGeneratorLoss as MinmaxGeneratorLoss,
     least_square_discriminator_loss as least_square_discriminator_loss,
     least_square_generator_loss as least_square_generator_loss,
+    LeastSquareDiscriminatorLoss as LeastSquareDiscriminatorLoss,
+    LeastSquareGeneratorLoss as LeastSquareGeneratorLoss,
     relativistic_discriminator_loss as relativistic_discriminator_loss,
     relativistic_generator_loss as relativistic_generator_loss,
+    RelativisticDiscriminatorLoss as RelativisticDiscriminatorLoss,
+    RelativisticGeneratorLoss as RelativisticGeneratorLoss,
 )
 from .utils import (
     check_vgg_params_exists as check_vgg_params_exists,
     load_vgg19_params as load_vgg19_params,
     # get_loss_wrapper as get_loss_wrapper,
     # compute_loss as compute_loss,
-    Reduces as Reduces,
+    Reduce as Reduces,
     LossWrapper as LossWrapper,
 )
 
 
 check_vgg_params_exists()
 del check_vgg_params_exists
```

### Comparing `flaxsr-0.0.4/flaxsr/losses/perceptual_losses.py` & `flaxsr-0.0.5/flaxsr/losses/perceptual_losses.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import flax
 import flax.linen as nn
 
 import numpy as np
 import einops
 
 from functools import partial
-from typing import Sequence, Literal
+from typing import Sequence, Literal, Optional
 
-from flaxsr.losses.utils import reduce_fn, Reduces
+from flaxsr.losses.utils import reduce_fn, Reduce, Loss, load_vgg19_params, apply_mask
 from flaxsr._utils import register
 
 
 Pytree = any
 
 
 def _conv(x: jnp.ndarray, weights: jnp.ndarray, bias: jnp.ndarray):
@@ -45,40 +45,42 @@
             x = nn.max_pool(x, (2, 2), (2, 2), 'SAME')
         else:
             x = x  # for jax.jit
     outputs.append(x)
     return outputs
 
 
-@partial(jax.jit, static_argnums=(3, 4, 5,))
+@partial(jax.jit, static_argnums=(3, 5, 6,))
 def vgg_loss(
-        hr: jnp.ndarray, sr: jnp.ndarray, vgg_params: Pytree,
-        feats_from: Sequence[int], before_act: bool = False, reduces: str | Reduces = 'mean'
+        hr: jnp.ndarray, sr: jnp.ndarray, vgg_params: Pytree, feats_from: Sequence[int],
+        mask: Optional[jnp.ndarray] = None, before_act: bool = False, reduce: str | Reduce = 'mean'
 ) -> jnp.ndarray:
+    hr, sr = apply_mask(hr, sr, mask=mask)
     hr_feats = _get_feats_from_vgg19(hr, vgg_params, before_act)
     sr_feats = _get_feats_from_vgg19(sr, vgg_params, before_act)
 
     loss = 0.
     for i, (hr_feats, sr_feats) in enumerate(zip(hr_feats, sr_feats)):
         if i in feats_from:
             loss += jnp.mean((hr_feats - sr_feats) ** 2, axis=(1, 2, 3))
-    return reduce_fn(loss, reduces)
+    return reduce_fn(loss, reduce)
 
 
 @register('losses', 'vgg')
-class VGGLoss:
+class VGGLoss(Loss):
     def __init__(
-            self, feats_from: Sequence[int], before_act: bool = False, reduces: str | Reduces = 'mean'
+            self, feats_from: Sequence[int], before_act: bool = False, reduce: str | Reduce = 'mean'
     ):
+        super().__init__(reduce)
         self.feats_from = feats_from
         self.before_act = before_act
-        self.reduces = reduces
+        self.vgg_params = load_vgg19_params()
 
-    def __call__(self, hr: jnp.ndarray, sr: jnp.ndarray, vgg_params: Pytree) -> jnp.ndarray:
-        return vgg_loss(hr, sr, vgg_params, self.feats_from, self.before_act, self.reduces)
+    def __call__(self, hr: jnp.ndarray, sr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
+        return vgg_loss(hr, sr, self.vgg_params, self.feats_from, mask, self.before_act, self.reduce)
 
 
 """
 Maybe Implement Style Loss in the future?
 1. _gram_matrix
 2. style_loss
 3. StyleLoss
```

### Comparing `flaxsr-0.0.4/flaxsr/models/edsr.py` & `flaxsr-0.0.5/flaxsr/models/edsr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/models/espcn.py` & `flaxsr-0.0.5/flaxsr/models/espcn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/models/fsrcnn.py` & `flaxsr-0.0.5/flaxsr/models/fsrcnn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/models/nafssr.py` & `flaxsr-0.0.5/flaxsr/models/nafssr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/models/ncnet.py` & `flaxsr-0.0.5/flaxsr/models/ncnet.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/models/srcnn.py` & `flaxsr-0.0.5/flaxsr/models/srcnn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/models/srgan.py` & `flaxsr-0.0.5/flaxsr/models/srgan.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 
 """
 Implemented SRResNet only.
 SRGAN will be implemented later.
 """
 
 
-ml_config = any
-
-
 class ResBlock(nn.Module):
 
     @nn.compact
     def __call__(self, inputs: jnp.ndarray, training: bool = False, **kwargs) -> jnp.ndarray:
         shape = inputs.shape
         residual = nn.Conv(shape[-1], (3, 3), padding='SAME')(inputs)
         residual = nn.BatchNorm()(residual, use_running_average=not training)
@@ -97,24 +94,25 @@
         x = DiscriminatorBlock(self.n_filters * 2, 3, 1)(x, training=training)
         x = DiscriminatorBlock(self.n_filters * 2, 3, 2)(x, training=training)
         x = DiscriminatorBlock(self.n_filters * 4, 3, 1)(x, training=training)
         x = DiscriminatorBlock(self.n_filters * 4, 3, 2)(x, training=training)
         x = DiscriminatorBlock(self.n_filters * 8, 3, 1)(x, training=training)
         x = DiscriminatorBlock(self.n_filters * 8, 3, 2)(x, training=training)
 
+        x = einops.rearrange(x, '... h w c -> ... (h w c)')
         x = nn.Dense(1024)(x)
         x = nn.activation.leaky_relu(x, negative_slope=0.2)
         x = nn.Dense(1)(x)
         return x
 
 
 @register('models', 'srgan')
 class SRGAN(nn.Module):
-    generator_spec: ml_config
-    discriminator_spec: ml_config
+    generator_spec: dict
+    discriminator_spec: dict
 
     def setup(self) -> None:
         self.generator = SRResNet(**self.generator_spec)
         self.discriminator = Discriminator(**self.discriminator_spec)
 
     def __call__(self, x: jnp.ndarray, training: bool = False) -> jnp.ndarray:
         return self.generator(x, training=training)
```

### Comparing `flaxsr-0.0.4/flaxsr/models/vdsr.py` & `flaxsr-0.0.5/flaxsr/models/vdsr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr/training/train_step.py` & `flaxsr-0.0.5/flaxsr/training/train_step.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/flaxsr.egg-info/SOURCES.txt` & `flaxsr-0.0.5/flaxsr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.4/setup.py` & `flaxsr-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="flaxsr",
-    version="0.0.4",
+    version="0.0.5",
     author="dslisleedh",
     author_email="dslisleedh@gmail.com",
     description="Super Resolution models with Jax/Flax",
     long_description=open('README.md', 'rt').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/dslisleedh/FlaxSR",
     project_urls={
```

