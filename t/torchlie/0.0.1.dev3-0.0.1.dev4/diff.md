# Comparing `tmp/torchlie-0.0.1.dev3.tar.gz` & `tmp/torchlie-0.0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlie-0.0.1.dev3.tar", last modified: Wed May 31 14:07:33 2023, max compression
+gzip compressed data, was "torchlie-0.0.1.dev4.tar", last modified: Fri Jun  2 19:35:27 2023, max compression
```

## Comparing `torchlie-0.0.1.dev3.tar` & `torchlie-0.0.1.dev4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:07:33.661072 torchlie-0.0.1.dev3/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-05-31 14:07:33.659020 torchlie-0.0.1.dev3/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-05-30 20:56:05.000000 torchlie-0.0.1.dev3/README.md
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:07:33.606418 torchlie-0.0.1.dev3/lie/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      521 2023-05-31 14:05:55.000000 torchlie-0.0.1.dev3/lie/__init__.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:07:33.637227 torchlie-0.0.1.dev3/lie/functional/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/__init__.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/check_contexts.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1818 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/constants.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10767 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/lie_group.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32596 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/se3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    35868 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/so3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1259 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/utils.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20259 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/lie_tensor.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3094 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/types.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-05-31 14:07:33.662222 torchlie-0.0.1.dev3/setup.cfg
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1184 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/setup.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:07:33.654709 torchlie-0.0.1.dev3/torchlie.egg-info/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-05-31 14:07:33.000000 torchlie-0.0.1.dev3/torchlie.egg-info/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      387 2023-05-31 14:07:33.000000 torchlie-0.0.1.dev3/torchlie.egg-info/SOURCES.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-05-31 14:07:33.000000 torchlie-0.0.1.dev3/torchlie.egg-info/dependency_links.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        4 2023-05-31 14:07:33.000000 torchlie-0.0.1.dev3/torchlie.egg-info/top_level.txt
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 19:35:27.493326 torchlie-0.0.1.dev4/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-06-02 19:35:27.491773 torchlie-0.0.1.dev4/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/README.md
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 19:35:27.444626 torchlie-0.0.1.dev4/lie/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      561 2023-06-02 19:35:12.000000 torchlie-0.0.1.dev4/lie/__init__.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 19:35:27.472423 torchlie-0.0.1.dev4/lie/functional/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-06-02 17:13:39.000000 torchlie-0.0.1.dev4/lie/functional/__init__.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/functional/check_contexts.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      536 2023-06-02 16:51:55.000000 torchlie-0.0.1.dev4/lie/functional/constants.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10767 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/functional/lie_group.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32686 2023-06-02 17:57:25.000000 torchlie-0.0.1.dev4/lie/functional/se3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    35965 2023-06-02 17:31:58.000000 torchlie-0.0.1.dev4/lie/functional/so3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1259 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/functional/utils.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20259 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/lie_tensor.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1965 2023-06-02 16:51:55.000000 torchlie-0.0.1.dev4/lie/options.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3094 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/lie/types.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-06-02 19:35:27.494307 torchlie-0.0.1.dev4/setup.cfg
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1184 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev4/setup.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 19:35:27.487278 torchlie-0.0.1.dev4/torchlie.egg-info/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-06-02 19:35:27.000000 torchlie-0.0.1.dev4/torchlie.egg-info/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      402 2023-06-02 19:35:27.000000 torchlie-0.0.1.dev4/torchlie.egg-info/SOURCES.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-06-02 19:35:27.000000 torchlie-0.0.1.dev4/torchlie.egg-info/dependency_links.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        4 2023-06-02 19:35:27.000000 torchlie-0.0.1.dev4/torchlie.egg-info/top_level.txt
```

### Comparing `torchlie-0.0.1.dev3/PKG-INFO` & `torchlie-0.0.1.dev4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchlie-0.0.1.dev3/lie/__init__.py` & `torchlie-0.0.1.dev4/lie/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-__version__ = "0.0.1.dev3"
+__version__ = "0.0.1.dev4"
 
 from .types import ltype, SE3, SO3
 from .lie_tensor import (  # usort: skip
     LieTensor,
     adj,
     as_euclidean,
     as_lietensor,
@@ -20,7 +20,8 @@
     jtransform_from,
     left_act,
     left_project,
     local,
     log,
     transform_from,
 )
+from .options import set_global_options
```

### Comparing `torchlie-0.0.1.dev3/lie/functional/check_contexts.py` & `torchlie-0.0.1.dev4/lie/functional/check_contexts.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev3/lie/functional/lie_group.py` & `torchlie-0.0.1.dev4/lie/functional/lie_group.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev3/lie/functional/se3_impl.py` & `torchlie-0.0.1.dev4/lie/functional/se3_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 from typing import cast, List, Tuple, Optional
 
-from . import constants
-from . import lie_group, so3_impl as SO3
+from lie.options import _TORCHLIE_GLOBAL_OPTIONS as LIE_OPTS
+from . import constants, lie_group, so3_impl as SO3
 from .check_contexts import checks_base
 from .utils import get_module, shape_err_msg
 
 
 NAME: str = "SE3"
 DIM: int = 6
 _DIAG_6_IDX = [0, 1, 2, 3, 4, 5]
@@ -44,15 +44,15 @@
                 tangent_vector.shape,
             )
         )
 
 
 def check_hat_tensor(tensor: torch.Tensor):
     def _impl(t_: torch.Tensor):
-        if t_[..., -1].abs().max() > constants._SE3_NEAR_ZERO_EPS[t_.dtype]:
+        if t_[..., -1].abs().max() > LIE_OPTS.get_eps("se3", "hat", t_.dtype):
             raise ValueError("The last row for hat tensors of SE3 must be zero")
 
         SO3.check_hat_tensor(t_[..., :3, :3])
 
     if tensor.shape[-2:] != (4, 4):
         raise ValueError(
             shape_err_msg("Hat tensors of SE3", "(..., 4, 4)", tensor.shape)
@@ -188,15 +188,15 @@
         sine_by_theta,
         one_minus_cosine_by_theta2,
     ) = SO3._exp_impl_helper(tangent_vector[..., 3:])
 
     # Compute the translation
     tangent_vector_lin = tangent_vector[..., :3].view(*size, 3, 1)
     tangent_vector_ang = tangent_vector[..., 3:].view(*size, 3, 1)
-    near_zero = theta < constants._SO3_NEAR_ZERO_EPS[tangent_vector.dtype]
+    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
     theta3_nz = theta_nz * theta2_nz
     theta_minus_sine_by_theta3_t = torch.where(
         near_zero, 1.0 / 6 - theta2 / 120, (theta - sine) / theta3_nz
     )
     ret[..., 3:] = sine_by_theta * tangent_vector_lin
     ret[..., 3:] += one_minus_cosine_by_theta2 * torch.cross(
         tangent_vector_ang, tangent_vector_lin, dim=-2
@@ -239,15 +239,15 @@
         sine_by_theta,
         one_minus_cosine_by_theta2,
         theta_minus_sine_by_theta3_rot,
     )
     jac[..., 3:, 3:] = jac[..., :3, :3]
 
     # compute translation jacobians
-    near_zero = theta < constants._SO3_NEAR_ZERO_EPS[tangent_vector.dtype]
+    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
     d_one_minus_cosine_by_theta2 = torch.where(
         near_zero,
         constants._NEAR_ZERO_D_ONE_MINUS_COSINE_BY_THETA2,
         (sine_by_theta - 2 * one_minus_cosine_by_theta2) / theta2_nz,
     )
     d_theta_minus_sine_by_theta3 = torch.where(
         near_zero,
@@ -286,15 +286,15 @@
     ret, (
         theta,
         theta2_nz,
         sine_by_theta,
         one_minus_cosine_by_theta2,
         theta_minus_sine_by_theta3_t,
     ) = _exp_impl_helper(tangent_vector)
-    near_zero = theta < constants._SO3_NEAR_ZERO_EPS[tangent_vector.dtype]
+    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
     theta_minus_sine_by_theta3_rot = torch.where(
         near_zero, torch.zeros_like(theta), theta_minus_sine_by_theta3_t
     )
     jac, _ = _jexp_impl_helper(
         tangent_vector,
         ret[..., :3],
         theta,
@@ -353,15 +353,15 @@
     check_group_tensor(group)
     size = get_group_size(group)
 
     # Compute the rotation
     ret_ang, (theta, sine, cosine) = SO3._log_impl_helper(group[..., :3])
 
     # Compute the translation
-    near_zero = theta < constants._SO3_NEAR_ZERO_EPS[group.dtype]
+    near_zero = theta < LIE_OPTS.get_eps("se3", "near_zero", group.dtype)
     theta2 = theta**2
     sine_theta = sine * theta
     two_cosine_minus_two = 2 * cosine - 2
     two_cosine_minus_two_nz = torch.where(
         near_zero, constants._NON_ZERO, two_cosine_minus_two
     )
 
@@ -410,15 +410,15 @@
     two_cosine_minus_two_nz: torch.Tensor,
     a: torch.Tensor,
     b: torch.Tensor,
 ):
     ret_lin = tangent_vector[..., :3]
     ret_ang = tangent_vector[..., 3:]
     size = get_tangent_vector_size(tangent_vector)
-    near_zero = theta < constants._SO3_NEAR_ZERO_EPS[tangent_vector.dtype]
+    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
     jac = tangent_vector.new_zeros(*size, 6, 6)
     jac[..., :3, :3], (b_ret_ang,) = SO3._jlog_impl_helper(ret_ang, theta, sine, cosine)
     jac[..., 3:, 3:] = jac[..., :3, :3]
 
     theta_nz = torch.where(near_zero, constants._NON_ZERO, theta)
     theta4_nz = theta2_nz**2
     c = torch.where(
```

### Comparing `torchlie-0.0.1.dev3/lie/functional/so3_impl.py` & `torchlie-0.0.1.dev4/lie/functional/so3_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 from typing import cast, List, Tuple, Optional
 
-from . import constants
-from . import lie_group
+from lie.options import _TORCHLIE_GLOBAL_OPTIONS as LIE_OPTS
+from . import constants, lie_group
 from .check_contexts import checks_base
 from .utils import (
     get_module,
     shape_err_msg,
     permute_op_dim,
     unpermute_op_dim,
     fill_dims,
@@ -62,17 +62,17 @@
                 tangent_vector.shape,
             )
         )
 
 
 def check_hat_tensor(tensor: torch.Tensor):
     def _impl(t_: torch.Tensor):
-        if (t_.transpose(-1, -2) + t_).abs().max().item() > constants._SO3_HAT_EPS[
-            t_.dtype
-        ]:
+        if (t_.transpose(-1, -2) + t_).abs().max().item() > LIE_OPTS.get_eps(
+            "so3", "hat", t_.dtype
+        ):
             raise ValueError("Hat tensors of SO3 can only be skew-symmetric.")
 
     if tensor.shape[-2:] != (3, 3):
         raise ValueError(
             shape_err_msg("Hat tensors of SO3", "(..., 3, 3)", tensor.shape)
         )
 
@@ -102,15 +102,15 @@
         raise ValueError(
             shape_err_msg("Projected tensors of SO3", "(..., 3, 3)", tensor.shape)
         )
 
 
 def check_unit_quaternion(quaternion: torch.Tensor):
     def _impl(t_: torch.Tensor):
-        QUANTERNION_EPS = constants._SO3_QUATERNION_EPS[t_.dtype]
+        QUANTERNION_EPS = LIE_OPTS.get_eps("so3", "quat", t_.dtype)
 
         if t_.dtype != torch.float64:
             t_ = t_.double()
 
         if (torch.linalg.norm(t_, dim=-1) - 1).abs().max().item() >= QUANTERNION_EPS:
             raise ValueError("Not unit quaternions.")
 
@@ -216,15 +216,15 @@
 # -----------------------------------------------------------------------------
 # Exponential Map
 # -----------------------------------------------------------------------------
 def _exp_impl_helper(tangent_vector: torch.Tensor):
     theta = torch.linalg.norm(tangent_vector, dim=-1, keepdim=True).unsqueeze(-1)
     theta2 = theta**2
     # Compute the approximations when theta ~ 0
-    near_zero = theta < constants._SO3_NEAR_ZERO_EPS[tangent_vector.dtype]
+    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
     theta_nz = torch.where(near_zero, constants._NON_ZERO, theta)
     theta2_nz = torch.where(near_zero, constants._NON_ZERO, theta2)
 
     cosine = torch.where(near_zero, 8 / (4 + theta2) - 1, theta.cos())
     sine = theta.sin()
     sine_by_theta = torch.where(near_zero, 0.5 * cosine + 0.5, sine / theta_nz)
     one_minus_cosine_by_theta2 = torch.where(
@@ -300,15 +300,15 @@
         theta2_nz,
         sine,
         _,
         sine_by_theta,
         one_minus_cosine_by_theta2,
     ) = _exp_impl_helper(tangent_vector)
 
-    near_zero = theta < constants._SO3_NEAR_ZERO_EPS[tangent_vector.dtype]
+    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
     theta3_nz = theta_nz * theta2_nz
     theta_minus_sine_by_theta3 = torch.where(
         near_zero, torch.zeros_like(theta), (theta - sine) / theta3_nz
     )
     jac, _ = _jexp_impl_helper(
         tangent_vector,
         sine_by_theta,
@@ -363,17 +363,16 @@
     sine_axis[..., 0] = 0.5 * (group[..., 2, 1] - group[..., 1, 2])
     sine_axis[..., 1] = 0.5 * (group[..., 0, 2] - group[..., 2, 0])
     sine_axis[..., 2] = 0.5 * (group[..., 1, 0] - group[..., 0, 1])
     cosine = 0.5 * (group.diagonal(dim1=-1, dim2=-2).sum(dim=-1) - 1)
     sine = sine_axis.norm(dim=-1)
     theta = torch.atan2(sine, cosine)
 
-    near_zero = theta < constants._SO3_NEAR_ZERO_EPS[group.dtype]
-
-    near_pi = 1 + cosine <= constants._SO3_NEAR_PI_EPS[group.dtype]
+    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", group.dtype)
+    near_pi = 1 + cosine <= LIE_OPTS.get_eps("so3", "near_pi", group.dtype)
     # theta != pi
     near_zero_or_near_pi = torch.logical_or(near_zero, near_pi)
     # Compute the approximation of theta / sin(theta) when theta is near to 0
     sine_nz = torch.where(near_zero_or_near_pi, constants._NON_ZERO, sine)
     scale = torch.where(
         near_zero_or_near_pi,
         1 + sine**2 / 6,
@@ -416,15 +415,15 @@
 def _jlog_impl_helper(
     tangent_vector: torch.Tensor,
     theta: torch.Tensor,
     sine: torch.Tensor,
     cosine: torch.Tensor,
 ):
     size = get_tangent_vector_size(tangent_vector)
-    near_zero = theta < constants._SO3_NEAR_ZERO_EPS[tangent_vector.dtype]
+    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
     theta2 = theta**2
     sine_theta = sine * theta
     two_cosine_minus_two = 2 * cosine - 2
     two_cosine_minus_two_nz = torch.where(
         near_zero, constants._NON_ZERO, two_cosine_minus_two
     )
     theta2_nz = torch.where(near_zero, constants._NON_ZERO, theta2)
```

### Comparing `torchlie-0.0.1.dev3/lie/functional/utils.py` & `torchlie-0.0.1.dev4/lie/functional/utils.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev3/lie/lie_tensor.py` & `torchlie-0.0.1.dev4/lie/lie_tensor.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev3/lie/types.py` & `torchlie-0.0.1.dev4/lie/types.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev3/setup.py` & `torchlie-0.0.1.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev3/torchlie.egg-info/PKG-INFO` & `torchlie-0.0.1.dev4/torchlie.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

