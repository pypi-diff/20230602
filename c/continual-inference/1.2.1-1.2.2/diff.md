# Comparing `tmp/continual-inference-1.2.1.tar.gz` & `tmp/continual-inference-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/continual-inference-1.2.1.tar", last modified: Fri Mar 24 08:54:02 2023, max compression
+gzip compressed data, was "continual-inference-1.2.2.tar", last modified: Fri Jun  2 15:30:11 2023, max compression
```

## Comparing `continual-inference-1.2.1.tar` & `continual-inference-1.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 08:54:02.000000 continual-inference-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (116)    36011 2023-03-24 08:54:02.000000 continual-inference-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    30378 2023-03-24 08:52:35.000000 continual-inference-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 08:54:02.000000 continual-inference-1.2.1/continual/
--rw-r--r--   0 runner    (1001) docker     (116)      359 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/__about__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1492 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6550 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/closure.py
--rw-r--r--   0 runner    (1001) docker     (116)    35637 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/container.py
--rw-r--r--   0 runner    (1001) docker     (116)    24313 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/conv.py
--rw-r--r--   0 runner    (1001) docker     (116)     7742 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/convert.py
--rw-r--r--   0 runner    (1001) docker     (116)     4803 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/delay.py
--rw-r--r--   0 runner    (1001) docker     (116)     4293 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/linear.py
--rw-r--r--   0 runner    (1001) docker     (116)     1135 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/logging.py
--rw-r--r--   0 runner    (1001) docker     (116)    14683 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/module.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 08:54:02.000000 continual-inference-1.2.1/continual/multihead_attention/
--rw-r--r--   0 runner    (1001) docker     (116)      149 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/multihead_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    24049 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/multihead_attention/mha_base.py
--rw-r--r--   0 runner    (1001) docker     (116)    14015 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/multihead_attention/retroactive_mha.py
--rw-r--r--   0 runner    (1001) docker     (116)    15027 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/multihead_attention/single_output_mha.py
--rw-r--r--   0 runner    (1001) docker     (116)    15136 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/onnx.py
--rw-r--r--   0 runner    (1001) docker     (116)    46663 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/pooling.py
--rw-r--r--   0 runner    (1001) docker     (116)     7056 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     2657 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/ptflops.py
--rw-r--r--   0 runner    (1001) docker     (116)    28266 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/rnn.py
--rw-r--r--   0 runner    (1001) docker     (116)     1813 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/shape.py
--rw-r--r--   0 runner    (1001) docker     (116)     1604 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/skip.py
--rw-r--r--   0 runner    (1001) docker     (116)    22363 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/transformer.py
--rw-r--r--   0 runner    (1001) docker     (116)     7059 2023-03-24 08:52:35.000000 continual-inference-1.2.1/continual/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 08:54:02.000000 continual-inference-1.2.1/continual_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    36011 2023-03-24 08:54:02.000000 continual-inference-1.2.1/continual_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      815 2023-03-24 08:54:02.000000 continual-inference-1.2.1/continual_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-24 08:54:02.000000 continual-inference-1.2.1/continual_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      345 2023-03-24 08:54:02.000000 continual-inference-1.2.1/continual_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2023-03-24 08:54:02.000000 continual-inference-1.2.1/continual_inference.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-24 08:54:02.000000 continual-inference-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2938 2023-03-24 08:52:35.000000 continual-inference-1.2.1/setup.py
+drwxr-xr-x   0 au478108 (794351465) 357318537        0 2023-06-02 15:30:11.422211 continual-inference-1.2.2/
+-rw-r--r--   0 au478108 (794351465) 357318537    36011 2023-06-02 15:30:11.421918 continual-inference-1.2.2/PKG-INFO
+-rw-r--r--   0 au478108 (794351465) 357318537    30378 2023-05-24 13:22:59.000000 continual-inference-1.2.2/README.md
+drwxr-xr-x   0 au478108 (794351465) 357318537        0 2023-06-02 15:30:11.416265 continual-inference-1.2.2/continual/
+-rw-r--r--   0 au478108 (794351465) 357318537      359 2023-06-02 07:52:08.000000 continual-inference-1.2.2/continual/__about__.py
+-rw-r--r--   0 au478108 (794351465) 357318537     1492 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/__init__.py
+-rw-r--r--   0 au478108 (794351465) 357318537     6550 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/closure.py
+-rw-r--r--   0 au478108 (794351465) 357318537    35637 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/container.py
+-rw-r--r--   0 au478108 (794351465) 357318537    24313 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/conv.py
+-rw-r--r--   0 au478108 (794351465) 357318537     7742 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/convert.py
+-rw-r--r--   0 au478108 (794351465) 357318537     4803 2023-03-24 09:21:27.000000 continual-inference-1.2.2/continual/delay.py
+-rw-r--r--   0 au478108 (794351465) 357318537     4293 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/linear.py
+-rw-r--r--   0 au478108 (794351465) 357318537     1135 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/logging.py
+-rw-r--r--   0 au478108 (794351465) 357318537    14683 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/module.py
+drwxr-xr-x   0 au478108 (794351465) 357318537        0 2023-06-02 15:30:11.419000 continual-inference-1.2.2/continual/multihead_attention/
+-rw-r--r--   0 au478108 (794351465) 357318537      149 2022-07-04 15:01:36.000000 continual-inference-1.2.2/continual/multihead_attention/__init__.py
+-rw-r--r--   0 au478108 (794351465) 357318537    24049 2022-12-02 09:07:24.000000 continual-inference-1.2.2/continual/multihead_attention/mha_base.py
+-rw-r--r--   0 au478108 (794351465) 357318537    14015 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/multihead_attention/retroactive_mha.py
+-rw-r--r--   0 au478108 (794351465) 357318537    15027 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/multihead_attention/single_output_mha.py
+-rw-r--r--   0 au478108 (794351465) 357318537    15136 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/onnx.py
+-rw-r--r--   0 au478108 (794351465) 357318537    46663 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/pooling.py
+-rw-r--r--   0 au478108 (794351465) 357318537     7056 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/positional_encoding.py
+-rw-r--r--   0 au478108 (794351465) 357318537     2657 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/ptflops.py
+-rw-r--r--   0 au478108 (794351465) 357318537    28266 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/rnn.py
+-rw-r--r--   0 au478108 (794351465) 357318537     1813 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/shape.py
+-rw-r--r--   0 au478108 (794351465) 357318537     1604 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/skip.py
+-rw-r--r--   0 au478108 (794351465) 357318537    22532 2023-06-02 07:52:08.000000 continual-inference-1.2.2/continual/transformer.py
+-rw-r--r--   0 au478108 (794351465) 357318537     7059 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/utils.py
+drwxr-xr-x   0 au478108 (794351465) 357318537        0 2023-06-02 15:30:11.421240 continual-inference-1.2.2/continual_inference.egg-info/
+-rw-r--r--   0 au478108 (794351465) 357318537    36011 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/PKG-INFO
+-rw-r--r--   0 au478108 (794351465) 357318537      815 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 au478108 (794351465) 357318537        1 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 au478108 (794351465) 357318537      345 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/requires.txt
+-rw-r--r--   0 au478108 (794351465) 357318537       10 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/top_level.txt
+-rw-r--r--   0 au478108 (794351465) 357318537       38 2023-06-02 15:30:11.422336 continual-inference-1.2.2/setup.cfg
+-rw-r--r--   0 au478108 (794351465) 357318537     2938 2022-12-21 08:00:31.000000 continual-inference-1.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `continual-inference-1.2.1/PKG-INFO` & `continual-inference-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continual-inference
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python library for Continual Inference Networks in PyTorch
 Home-page: https://github.com/lukashedegaard/continual-inference
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Description: <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/logo_name.svg" style="width: 400px;">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: continual-inference Version: 1.2.1 Summary: A
+Metadata-Version: 2.1 Name: continual-inference Version: 1.2.2 Summary: A
 Python library for Continual Inference Networks in PyTorch Home-page: https://
 github.com/lukashedegaard/continual-inference Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Description: [https://
 raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/
 logo_name.svg] __A Python library for Continual Inference Networks in PyTorch__
 [Quick-start](https://continual-inference.readthedocs.io/en/latest/generated/
 README.html#quick-start) â¢ [Docs](https://continual-inference.readthedocs.io/
```

### Comparing `continual-inference-1.2.1/README.md` & `continual-inference-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/__init__.py` & `continual-inference-1.2.2/continual/__init__.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/closure.py` & `continual-inference-1.2.2/continual/closure.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/container.py` & `continual-inference-1.2.2/continual/container.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/conv.py` & `continual-inference-1.2.2/continual/conv.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/convert.py` & `continual-inference-1.2.2/continual/convert.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/delay.py` & `continual-inference-1.2.2/continual/delay.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/linear.py` & `continual-inference-1.2.2/continual/linear.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/logging.py` & `continual-inference-1.2.2/continual/logging.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/module.py` & `continual-inference-1.2.2/continual/module.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/multihead_attention/mha_base.py` & `continual-inference-1.2.2/continual/multihead_attention/mha_base.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/multihead_attention/retroactive_mha.py` & `continual-inference-1.2.2/continual/multihead_attention/retroactive_mha.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/multihead_attention/single_output_mha.py` & `continual-inference-1.2.2/continual/multihead_attention/single_output_mha.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/onnx.py` & `continual-inference-1.2.2/continual/onnx.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/pooling.py` & `continual-inference-1.2.2/continual/pooling.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/positional_encoding.py` & `continual-inference-1.2.2/continual/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/ptflops.py` & `continual-inference-1.2.2/continual/ptflops.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/rnn.py` & `continual-inference-1.2.2/continual/rnn.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/shape.py` & `continual-inference-1.2.2/continual/shape.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/skip.py` & `continual-inference-1.2.2/continual/skip.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual/transformer.py` & `continual-inference-1.2.2/continual/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,15 +424,15 @@
 
 
 def TransformerEncoderLayerFactory(
     d_model: int,
     nhead: int,
     dim_feedforward: int = 2048,
     dropout: float = 0.1,
-    activation: Union[nn.Module, Callable[[Tensor], Tensor]] = nn.functional.relu,
+    activation: Union[nn.Module, Callable[[Tensor], Tensor], str] = nn.functional.relu,
     layer_norm_eps: float = 1e-5,
     # batch_first: bool = True,
     # norm_first: bool = False,
     device=None,
     dtype=None,
     sequence_len: int = None,
 ) -> Callable[[MhaType], Sequential]:
@@ -465,14 +465,19 @@
     Examples::
 
         encoder_layer = co.TransformerEncoderLayerFactory(d_model=512, nhead=8, sequence_len=32)
         transformer_encoder = co.TransformerEncoder(encoder_layer, num_layers=2)
         src = torch.rand(10, 512, 32)
         out = transformer_encoder(src)
     """
+    if activation in {"relu", "gelu"}:
+        activation = {
+            "relu": nn.functional.relu,
+            "gelu": nn.functional.relu,
+        }[activation]
 
     def TransformerEncoderLayer(mha_type: MhaType):
         factory_fn = {
             MhaType.RETROACTIVE: RetroactiveTransformerEncoderLayer,
             MhaType.SINGLE_OUTPUT: SingleOutputTransformerEncoderLayer,
             MhaType.SINGLE_OUTPUT_FORWARD: partial(
                 SingleOutputTransformerEncoderLayer, single_output_forward=True
```

### Comparing `continual-inference-1.2.1/continual/utils.py` & `continual-inference-1.2.2/continual/utils.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/continual_inference.egg-info/PKG-INFO` & `continual-inference-1.2.2/continual_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continual-inference
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python library for Continual Inference Networks in PyTorch
 Home-page: https://github.com/lukashedegaard/continual-inference
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Description: <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/logo_name.svg" style="width: 400px;">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: continual-inference Version: 1.2.1 Summary: A
+Metadata-Version: 2.1 Name: continual-inference Version: 1.2.2 Summary: A
 Python library for Continual Inference Networks in PyTorch Home-page: https://
 github.com/lukashedegaard/continual-inference Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Description: [https://
 raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/
 logo_name.svg] __A Python library for Continual Inference Networks in PyTorch__
 [Quick-start](https://continual-inference.readthedocs.io/en/latest/generated/
 README.html#quick-start) â¢ [Docs](https://continual-inference.readthedocs.io/
```

### Comparing `continual-inference-1.2.1/continual_inference.egg-info/SOURCES.txt` & `continual-inference-1.2.2/continual_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.1/setup.py` & `continual-inference-1.2.2/setup.py`

 * *Files identical despite different names*

