# Comparing `tmp/torchlie-0.0.1.dev4.tar.gz` & `tmp/torchlie-0.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlie-0.0.1.dev4.tar", last modified: Fri Jun  2 19:35:27 2023, max compression
+gzip compressed data, was "torchlie-0.0.1.dev5.tar", last modified: Fri Jun  2 21:06:38 2023, max compression
```

## Comparing `torchlie-0.0.1.dev4.tar` & `torchlie-0.0.1.dev5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 19:35:27.493326 torchlie-0.0.1.dev4/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-06-02 19:35:27.491773 torchlie-0.0.1.dev4/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/README.md
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 19:35:27.444626 torchlie-0.0.1.dev4/lie/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      561 2023-06-02 19:35:12.000000 torchlie-0.0.1.dev4/lie/__init__.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 19:35:27.472423 torchlie-0.0.1.dev4/lie/functional/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-06-02 17:13:39.000000 torchlie-0.0.1.dev4/lie/functional/__init__.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/functional/check_contexts.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      536 2023-06-02 16:51:55.000000 torchlie-0.0.1.dev4/lie/functional/constants.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10767 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/functional/lie_group.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32686 2023-06-02 17:57:25.000000 torchlie-0.0.1.dev4/lie/functional/se3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    35965 2023-06-02 17:31:58.000000 torchlie-0.0.1.dev4/lie/functional/so3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1259 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/functional/utils.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20259 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/lie_tensor.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1965 2023-06-02 16:51:55.000000 torchlie-0.0.1.dev4/lie/options.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3094 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/types.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-06-02 19:35:27.494307 torchlie-0.0.1.dev4/setup.cfg
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1184 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/setup.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 19:35:27.487278 torchlie-0.0.1.dev4/torchlie.egg-info/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-06-02 19:35:27.000000 torchlie-0.0.1.dev4/torchlie.egg-info/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      402 2023-06-02 19:35:27.000000 torchlie-0.0.1.dev4/torchlie.egg-info/SOURCES.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-06-02 19:35:27.000000 torchlie-0.0.1.dev4/torchlie.egg-info/dependency_links.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        4 2023-06-02 19:35:27.000000 torchlie-0.0.1.dev4/torchlie.egg-info/top_level.txt
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 21:06:38.101780 torchlie-0.0.1.dev5/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-06-02 21:06:38.100315 torchlie-0.0.1.dev5/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/README.md
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 21:06:38.048425 torchlie-0.0.1.dev5/lie/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      583 2023-06-02 20:20:32.000000 torchlie-0.0.1.dev5/lie/__init__.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 21:06:38.078567 torchlie-0.0.1.dev5/lie/functional/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-06-02 17:13:39.000000 torchlie-0.0.1.dev5/lie/functional/__init__.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/functional/check_contexts.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      536 2023-06-02 16:51:55.000000 torchlie-0.0.1.dev5/lie/functional/constants.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10767 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/functional/lie_group.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32686 2023-06-02 19:50:24.000000 torchlie-0.0.1.dev5/lie/functional/se3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    35973 2023-06-02 19:39:01.000000 torchlie-0.0.1.dev5/lie/functional/so3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1259 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/functional/utils.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20259 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/lie_tensor.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     2166 2023-06-02 20:21:09.000000 torchlie-0.0.1.dev5/lie/options.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3094 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/types.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-06-02 21:06:38.102854 torchlie-0.0.1.dev5/setup.cfg
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1184 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/setup.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 21:06:38.095300 torchlie-0.0.1.dev5/torchlie.egg-info/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-06-02 21:06:37.000000 torchlie-0.0.1.dev5/torchlie.egg-info/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      402 2023-06-02 21:06:37.000000 torchlie-0.0.1.dev5/torchlie.egg-info/SOURCES.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-06-02 21:06:37.000000 torchlie-0.0.1.dev5/torchlie.egg-info/dependency_links.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        4 2023-06-02 21:06:37.000000 torchlie-0.0.1.dev5/torchlie.egg-info/top_level.txt
```

### Comparing `torchlie-0.0.1.dev4/PKG-INFO` & `torchlie-0.0.1.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1.dev4
+Version: 0.0.1.dev5
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchlie-0.0.1.dev4/lie/__init__.py` & `torchlie-0.0.1.dev5/lie/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-__version__ = "0.0.1.dev4"
+__version__ = "0.0.1.dev5"
 
 from .types import ltype, SE3, SO3
 from .lie_tensor import (  # usort: skip
     LieTensor,
     adj,
     as_euclidean,
     as_lietensor,
@@ -20,8 +20,8 @@
     jtransform_from,
     left_act,
     left_project,
     local,
     log,
     transform_from,
 )
-from .options import set_global_options
+from .options import reset_global_options, set_global_options
```

### Comparing `torchlie-0.0.1.dev4/lie/functional/check_contexts.py` & `torchlie-0.0.1.dev5/lie/functional/check_contexts.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev4/lie/functional/constants.py` & `torchlie-0.0.1.dev5/lie/functional/constants.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev4/lie/functional/lie_group.py` & `torchlie-0.0.1.dev5/lie/functional/lie_group.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev4/lie/functional/se3_impl.py` & `torchlie-0.0.1.dev5/lie/functional/se3_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,15 @@
     check_group_tensor(group)
     size = get_group_size(group)
 
     # Compute the rotation
     ret_ang, (theta, sine, cosine) = SO3._log_impl_helper(group[..., :3])
 
     # Compute the translation
-    near_zero = theta < LIE_OPTS.get_eps("se3", "near_zero", group.dtype)
+    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", group.dtype)
     theta2 = theta**2
     sine_theta = sine * theta
     two_cosine_minus_two = 2 * cosine - 2
     two_cosine_minus_two_nz = torch.where(
         near_zero, constants._NON_ZERO, two_cosine_minus_two
     )
```

### Comparing `torchlie-0.0.1.dev4/lie/functional/so3_impl.py` & `torchlie-0.0.1.dev5/lie/functional/so3_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 _DIAG_3_IDX = [0, 1, 2]
 
 _module = get_module(__name__)
 
 
 def check_group_tensor(tensor: torch.Tensor):
     def _impl(t_):
-        MATRIX_EPS = constants._SO3_MATRIX_EPS[t_.dtype]
+        MATRIX_EPS = LIE_OPTS.get_eps("so3", "matrix", t_.dtype)
         if t_.dtype != torch.float64:
             t_ = t_.double()
 
         _check = (
             torch.matmul(t_, t_.transpose(-1, -2))
             - torch.eye(3, 3, dtype=t_.dtype, device=t_.device)
         ).abs().max().item() < MATRIX_EPS
```

### Comparing `torchlie-0.0.1.dev4/lie/functional/utils.py` & `torchlie-0.0.1.dev5/lie/functional/utils.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev4/lie/lie_tensor.py` & `torchlie-0.0.1.dev5/lie/lie_tensor.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev4/lie/types.py` & `torchlie-0.0.1.dev5/lie/types.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev4/setup.py` & `torchlie-0.0.1.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev4/torchlie.egg-info/PKG-INFO` & `torchlie-0.0.1.dev5/torchlie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1.dev4
+Version: 0.0.1.dev5
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

