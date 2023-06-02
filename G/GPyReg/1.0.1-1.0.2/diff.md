# Comparing `tmp/GPyReg-1.0.1.tar.gz` & `tmp/GPyReg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPyReg-1.0.1.tar", last modified: Wed Apr 12 20:22:10 2023, max compression
+gzip compressed data, was "GPyReg-1.0.2.tar", last modified: Fri Jun  2 14:31:07 2023, max compression
```

## Comparing `GPyReg-1.0.1.tar` & `GPyReg-1.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.716208 GPyReg-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.708208 GPyReg-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/merge-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/GPyReg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-12 20:22:00.000000 GPyReg-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 20:22:00.000000 GPyReg-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-12 20:22:10.712208 GPyReg-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-12 20:22:00.000000 GPyReg-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-12 20:22:00.000000 GPyReg-1.0.1/coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 20:22:00.000000 GPyReg-1.0.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 20:22:00.000000 GPyReg-1.0.1/environment_pure_conda.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-12 20:22:00.000000 GPyReg-1.0.1/examples/example_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-12 20:22:00.000000 GPyReg-1.0.1/examples/example_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/gpyreg/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/covariance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/f_min_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    92330 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/isotropic_covariance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/noise_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30718 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/slice_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/gpyreg/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_covariance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    35700 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    35420 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_gaussian_process_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_isotropic_covariance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_noise_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_slice_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_smoothbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_smoothbox_student_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    19388 2023-04-12 20:22:00.000000 GPyReg-1.0.1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-12 20:22:00.000000 GPyReg-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:22:10.716208 GPyReg-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 20:22:00.000000 GPyReg-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:31:07.215485 GPyReg-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-02 14:30:57.000000 GPyReg-1.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:31:07.211485 GPyReg-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:31:07.211485 GPyReg-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-02 14:30:57.000000 GPyReg-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 14:30:57.000000 GPyReg-1.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-02 14:30:57.000000 GPyReg-1.0.2/.github/workflows/merge-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-02 14:30:57.000000 GPyReg-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 14:30:57.000000 GPyReg-1.0.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-02 14:30:57.000000 GPyReg-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-02 14:30:57.000000 GPyReg-1.0.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:31:07.211485 GPyReg-1.0.2/GPyReg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-02 14:31:07.000000 GPyReg-1.0.2/GPyReg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-02 14:31:07.000000 GPyReg-1.0.2/GPyReg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:31:07.000000 GPyReg-1.0.2/GPyReg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-02 14:31:07.000000 GPyReg-1.0.2/GPyReg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 14:31:07.000000 GPyReg-1.0.2/GPyReg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-02 14:30:57.000000 GPyReg-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:30:57.000000 GPyReg-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-02 14:31:07.215485 GPyReg-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-02 14:30:57.000000 GPyReg-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-02 14:30:57.000000 GPyReg-1.0.2/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-02 14:30:57.000000 GPyReg-1.0.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 14:30:57.000000 GPyReg-1.0.2/environment_pure_conda.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:31:07.211485 GPyReg-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-02 14:30:57.000000 GPyReg-1.0.2/examples/example_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-02 14:30:57.000000 GPyReg-1.0.2/examples/example_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:31:07.215485 GPyReg-1.0.2/gpyreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/covariance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/f_min_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93944 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/isotropic_covariance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/mean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/noise_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30716 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/slice_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:31:07.215485 GPyReg-1.0.2/gpyreg/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/test_covariance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36735 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/test_gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35440 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/test_gaussian_process_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/test_isotropic_covariance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/test_mean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/test_noise_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/test_slice_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/test_smoothbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-02 14:30:57.000000 GPyReg-1.0.2/gpyreg/testing/test_smoothbox_student_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19388 2023-06-02 14:30:57.000000 GPyReg-1.0.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-02 14:30:57.000000 GPyReg-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:31:07.215485 GPyReg-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-02 14:30:57.000000 GPyReg-1.0.2/setup.py
```

### Comparing `GPyReg-1.0.1/.github/workflows/docs.yml` & `GPyReg-1.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/.github/workflows/merge-tests.yml` & `GPyReg-1.0.2/.github/workflows/merge-tests.yml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/.github/workflows/release.yml` & `GPyReg-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/.github/workflows/tests.yml` & `GPyReg-1.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/.gitignore` & `GPyReg-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/.pre-commit-config.yaml` & `GPyReg-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/GPyReg.egg-info/PKG-INFO` & `GPyReg-1.0.2/GPyReg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPyReg
-Version: 1.0.1
+Version: 1.0.2
 Summary: Lightweight package for Gaussian process regression.
 License: BSD 3-Clause License
         
         Copyright (c) 2021, GPyReg Developers and their Assignees
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `GPyReg-1.0.1/GPyReg.egg-info/SOURCES.txt` & `GPyReg-1.0.2/GPyReg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/LICENSE` & `GPyReg-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/PKG-INFO` & `GPyReg-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPyReg
-Version: 1.0.1
+Version: 1.0.2
 Summary: Lightweight package for Gaussian process regression.
 License: BSD 3-Clause License
         
         Copyright (c) 2021, GPyReg Developers and their Assignees
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `GPyReg-1.0.1/README.md` & `GPyReg-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/examples/example_1.py` & `GPyReg-1.0.2/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/examples/example_2.py` & `GPyReg-1.0.2/examples/example_2.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/gpyreg/covariance_functions.py` & `GPyReg-1.0.2/gpyreg/covariance_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,17 @@
         else:
             tmp = cdist(X / ell, X_star / ell, "sqeuclidean")
 
         K = sf2 * np.exp(-tmp / 2)
 
         if compute_grad:
             if X_star is not None:
-                raise ValueError("X_star should be None when compute_grad is True.")
+                raise ValueError(
+                    "X_star should be None when compute_grad is True."
+                )
             dK = np.zeros((cov_N, N, N))
             for i in range(0, D):
                 # Gradient of cov length scales
                 dK[i, :, :] = K * squareform(
                     pdist(np.reshape(X[:, i] / ell[i], (-1, 1)), "sqeuclidean")
                 )
             # Gradient of cov output scale.
@@ -254,15 +256,17 @@
             b = X_star @ np.diag(np.sqrt(self.degree) / ell)
             tmp = cdist(a, b)
 
         K = sf2 * self.f(tmp) * np.exp(-tmp)
 
         if compute_grad:
             if X_star is not None:
-                raise ValueError("X_star should be None when compute_grad is True.")
+                raise ValueError(
+                    "X_star should be None when compute_grad is True."
+                )
             dK = np.zeros((cov_N, N, N))
             for i in range(0, D):
                 Ki = squareform(
                     pdist(
                         np.reshape(
                             np.sqrt(self.degree) / ell[i] * X[:, i], (-1, 1)
                         ),
@@ -332,15 +336,17 @@
             tmp = cdist(a, b, "sqeuclidean")
 
         M = 1 + 0.5 * tmp / alpha
         K = sf2 * M ** (-alpha)
 
         if compute_grad:
             if X_star is not None:
-                raise ValueError("X_star should be None when compute_grad is True.")
+                raise ValueError(
+                    "X_star should be None when compute_grad is True."
+                )
             dK = np.zeros((cov_N, N, N))
 
             # Gradient respect of lenght scale.
             for i in range(0, D):
                 Ki = squareform(
                     pdist(
                         np.reshape(1.0 / ell[i] * X[:, i], (-1, 1)),
```

### Comparing `GPyReg-1.0.1/gpyreg/f_min_fill.py` & `GPyReg-1.0.2/gpyreg/f_min_fill.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/gpyreg/formatting.py` & `GPyReg-1.0.2/gpyreg/formatting.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/gpyreg/gaussian_process.py` & `GPyReg-1.0.2/gpyreg/gaussian_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module for Gaussian Processes."""
 
 import math
 import time
 import warnings
 from textwrap import indent
+from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy as sp
 
 import gpyreg.covariance_functions
 import gpyreg.mean_functions
@@ -716,23 +717,24 @@
 
         Raises
         =======
         LinAlgError
             Raised when the Cholesky decomposition failed multiple times even
             by adding numerical stability values to the matrix.
         """
-
+        X_new, y_new, s2_new = self._convert_shapes(X_new, y_new, s2_new)
         # Create local copies so we won't get trouble
         # with references later.
         if X_new is not None:
             X_new = X_new.copy()
         if y_new is not None:
             y_new = y_new.copy()
         if s2_new is not None:
             s2_new = s2_new.copy()
+
         if hyp is not None:
             hyp = hyp.copy()
 
         # Check whether to do a rank-1 update.
         rank_one_update = False
         if X_new is not None and y_new is not None and compute_posterior:
             if (
@@ -776,15 +778,15 @@
                 if L_chol:  # High-noise parametrization
                     new_L_column = sp.linalg.solve_triangular(
                         L, Ks, trans=1, check_finite=False
                     )
                     # If rank-1 update is not numerically stable, perform a
                     # full update for this posterior instead:
                     sqrt_arg = (
-                        sn2_eff ** 2
+                        sn2_eff**2
                         + K * sn2_eff
                         - np.dot(new_L_column.T, new_L_column)
                     )
                     if sqrt_arg <= 0.0:
                         full_update_s = (
                             True  #  Mark this posterior for full update
                         )
@@ -983,15 +985,15 @@
         ValueError
             Raised when the `sampler_name` is not slicesample.
         """
         ## Default options
         if options is None:
             options = {}
         opts_N = options.get("opts_N", 3)
-        init_N = options.get("init_N", 2 ** 10)
+        init_N = options.get("init_N", 2**10)
         init_method = options.get("init_method", "sobol")
         thin = options.get("thin", 5)
         df_base = options.get("df_base", 7)
         widths = options.get("widths", None)
         log_p = options.get("log_P", None)  # Not used since no slicelite
         outwarp_fun = options.get("outwarp_fun", None)  # Not used
         step_size = options.get("step_size", None)  # Not used since no MALA
@@ -999,14 +1001,15 @@
         tol_opt_mcmc = options.get("tol_opt_mcmc", 1e-3)
         sampler_name = options.get("sampler", "slicesample")
         s_N = options.get("n_samples", 10)
         burn_in = options.get("burn", thin * s_N)
         lower_bounds = options.get("lower_bounds", "current")
         upper_bounds = options.get("upper_bounds", "current")
 
+        X, y, s2 = self._convert_shapes(X, y, s2)
         # Initialize GP if requested.
         if X is not None:
             self.X = X
 
         if y is not None:
             self.y = y
 
@@ -1339,15 +1342,15 @@
             z2_tmp[sb_idx_a] = (
                 (hyp[sb_idx_a] - b[sb_idx_a]) / sigma[sb_idx_a]
             ) ** 2
 
             if np.any(sb_idx_b | sb_idx_a):
                 lp -= 0.5 * np.sum(
                     np.log(
-                        C ** 2 * 2 * np.pi * sigma[sb_idx_b | sb_idx_a] ** 2
+                        C**2 * 2 * np.pi * sigma[sb_idx_b | sb_idx_a] ** 2
                     )
                     + z2_tmp[sb_idx_b | sb_idx_a]
                 )
             if np.any(sb_idx_btw):
                 lp -= np.sum(
                     np.log(C * sigma[sb_idx_btw]) + np.log(np.sqrt(2 * np.pi))
                 )
@@ -1555,15 +1558,15 @@
 
         return nlZ
 
     def predict_full(
         self,
         x_star: np.ndarray,
         y_star: np.ndarray = None,
-        s2_star: np.ndarray = 0,
+        s2_star: np.ndarray = None,
         add_noise: bool = False,
     ):
         """
         Compute the GP posterior mean and full covariance matrix for each
         hyperparameter sample.
 
         Parameters
@@ -1581,15 +1584,15 @@
         =======
         mu : ndarray, shape (M, sample_N)
             Posterior mean at the requested points for each hyperparameter
             sample.
         cov : ndarray, shape (M, M, sample_N)
             Covariance matrix for each hyperparameter sample.
         """
-
+        x_star, y_star, s2_star = self._convert_shapes(x_star, y_star, s2_star)
         s_N = self.posteriors.size
         N_star, _ = x_star.shape
 
         cov_N = self.covariance.hyperparameter_count(self.D)
         mean_N = self.mean.hyperparameter_count(self.D)
         noise_N = self.noise.hyperparameter_count()
 
@@ -1657,15 +1660,15 @@
 
         return mu, cov.transpose(1, 2, 0)
 
     def predict(
         self,
         x_star: np.ndarray,
         y_star: np.ndarray = None,
-        s2_star: np.ndarray = 0,
+        s2_star: np.ndarray = None,
         add_noise: bool = False,
         separate_samples: bool = False,
         return_lpd: bool = False,
     ):
         """
         Compute the GP posterior mean and noise variance at given points.
 
@@ -1695,14 +1698,15 @@
             otherwise it is  ``(M,)``.
             sample.
         s2 : ndarray
             Noise variance at each point. If we requested
             separate samples the shape is ``(M, sample_N)`` while
             otherwise it is ``(M,)``.
         """
+        x_star, y_star, s2_star = self._convert_shapes(x_star, y_star, s2_star)
 
         s_N = self.posteriors.size
         N_star, D = x_star.shape
 
         # Preallocate space
         mu = np.zeros((N_star, s_N))
         s2 = np.zeros((N_star, s_N))
@@ -1914,15 +1918,15 @@
             L = self.posteriors[s].L
             L_chol = self.posteriors[s].L_chol
 
             sn2 = np.exp(2 * hyp[cov_N])
             sn2_eff = sn2 * self.posteriors[s].sn2_mult
 
             # Compute posterior mean of the integral
-            tau = np.sqrt(sigma ** 2 + ell ** 2)
+            tau = np.sqrt(sigma**2 + ell**2)
             lnnf = (
                 ln_sf2 + sum_lnell - np.sum(np.log(tau), 1)
             )  # Covariance normalization factor
             sum_delta2 = np.zeros((N_star, N))
 
             for i in range(0, D):
                 sum_delta2 += (
@@ -1931,23 +1935,23 @@
                 ) ** 2
             z = np.exp(np.reshape(lnnf, (-1, 1)) - 0.5 * sum_delta2)
             F[:, s : s + 1] = np.dot(z, alpha) + m0
 
             if quadratic_mean_fun:
                 nu_k = -0.5 * np.sum(
                     1
-                    / omega ** 2
-                    * (mu ** 2 + sigma ** 2 - 2 * mu * xm + xm ** 2),
+                    / omega**2
+                    * (mu**2 + sigma**2 - 2 * mu * xm + xm**2),
                     1,
                 )
                 F[:, s] += nu_k
 
             # Compute posterior variance of the integral
             if compute_var:
-                tau_kk = np.sqrt(2 * sigma ** 2 + ell ** 2)
+                tau_kk = np.sqrt(2 * sigma**2 + ell**2)
                 nf_kk = np.exp(ln_sf2 + sum_lnell - np.sum(np.log(tau_kk), 1))
                 if L_chol:
                     tmp_result = sp.linalg.solve_triangular(
                         L, z.T, trans=1, check_finite=False
                     )
                     invKzk = (
                         sp.linalg.solve_triangular(
@@ -2022,15 +2026,15 @@
 
         # Loop over hyperparameter samples.
         ell = np.zeros((self.D, s_N))
         for s in range(0, s_N):
             ell[:, s] = np.exp(
                 self.posteriors[s].hyp[0 : self.D]
             )  # Extract length scale from HYP
-        ellbar = np.sqrt(np.mean(ell ** 2, 1)).T
+        ellbar = np.sqrt(np.mean(ell**2, 1)).T
 
         if lb is None:
             if self.X is not None:
                 lb = np.min(self.X, axis=0) - ellbar
             else:
                 lb = -ellbar
         if ub is None:
@@ -2056,15 +2060,15 @@
         flo = fhi = None
         for i in range(0, self.D):
             ax[i, i].set_position(
                 self.__tight_subplot(self.D, self.D, i, i, gutter, margins)
             )
 
             xx_vec = np.reshape(
-                np.linspace(lb[i], ub[i], np.ceil(x_N ** 1.5).astype(int)),
+                np.linspace(lb[i], ub[i], np.ceil(x_N**1.5).astype(int)),
                 (-1, 1),
             )
             if self.D > 1:
                 if x0 is not None:
                     xx = np.tile(x0, (np.size(xx_vec), 1))
                 else:
                     xx = np.tile(np.full((self.D,), 0.0), (np.size(xx_vec), 1))
@@ -2089,15 +2093,15 @@
                     lb[i] = xx_vec[idx1] - 0.5 * dx
                     ub[i] = xx_vec[idx2] + 0.5 * dx
                 else:
                     lb[i] = x0[i] - 0.5 * dx
                     ub[i] = x0[i] + 0.5 * dx
 
                 xx_vec = np.reshape(
-                    np.linspace(lb[i], ub[i], np.ceil(x_N ** 1.5).astype(int)),
+                    np.linspace(lb[i], ub[i], np.ceil(x_N**1.5).astype(int)),
                     (-1, 1),
                 )
                 if self.D > 1:
                     xx = np.tile(x0, (np.size(xx_vec), 1))
                     xx[:, i : i + 1] = xx_vec
                 else:
                     xx = xx_vec
@@ -2145,17 +2149,17 @@
                 xx1_vec = np.reshape(np.linspace(lb[i], ub[i], x_N), (-1, 1)).T
                 xx2_vec = np.reshape(np.linspace(lb[j], ub[j], x_N), (-1, 1)).T
                 xx_vec = np.array(np.meshgrid(xx1_vec, xx2_vec)).T.reshape(
                     -1, 2
                 )
 
                 if x0 is not None:
-                    xx = np.tile(x0, (x_N ** 2, 1))
+                    xx = np.tile(x0, (x_N**2, 1))
                 else:
-                    xx = np.tile(np.full((self.D,), 0.0), (x_N ** 2, 1))
+                    xx = np.tile(np.full((self.D,), 0.0), (x_N**2, 1))
                 xx[:, i] = xx_vec[:, 0]
                 xx[:, j] = xx_vec[:, 1]
 
                 fmu, fs2 = self.predict(xx, add_noise=False)
 
                 for k in range(0, 2):
                     if k == 1:
@@ -2466,26 +2470,22 @@
                 np.dot((self.y - m).T, alpha / 2)
                 + np.sum(np.log(np.diag(L)))
                 + N * np.log(2 * np.pi * sl) / 2
             )
 
             if compute_nlZ_grad:
                 dnlZ = np.zeros(hyp.shape)
-                Q = (
+                Q = sp.linalg.solve_triangular(
+                    L,
                     sp.linalg.solve_triangular(
-                        L,
-                        sp.linalg.solve_triangular(
-                            L, np.eye(N), trans=1, check_finite=False
-                        ),
-                        trans=0,
-                        check_finite=False,
-                    )
-                    / sl
-                    - np.dot(alpha, alpha.T)
-                )
+                        L, np.eye(N), trans=1, check_finite=False
+                    ),
+                    trans=0,
+                    check_finite=False,
+                ) / sl - np.dot(alpha, alpha.T)
 
                 # Gradient of covariance hyperparameters.
                 for i in range(0, cov_N):
                     dnlZ[i] = np.sum(np.sum(Q * dK[:, :, i])) / 2
 
                 # Gradient of GP likelihood
                 if np.isscalar(sn2):
@@ -2514,14 +2514,58 @@
             alpha,
             np.ones((N, 1)) / np.sqrt(np.min(sn2) * sn2_mult),
             pL,
             sn2_mult,
             L_chol,
         )
 
+    def _convert_shapes(
+        self,
+        X: Union[np.ndarray, None],
+        y: Union[np.ndarray, None],
+        s2: Union[np.ndarray, float, int, None],
+    ):
+        """Convert input data to correct shapes."""
+        if X is None and y is None and s2 is None:
+            return X, y, s2
+
+        if X is not None:
+            if X.ndim == 1:
+                X = X[None, :]
+            if X.ndim != 2:
+                raise AssertionError("X need to be an array of shape (N, D)")
+            N, D = X.shape
+            if D != self.D:
+                raise AssertionError(
+                    f"The dimension of input data {D}"
+                    f"doesn't match GP's input dimension {self.D}."
+                )
+        else:
+            try:
+                N, D = self.X.shape
+            except AttributeError as e:
+                raise AttributeError(
+                    "self.X is not a numpy array, " f"self.X = {self.X}"
+                )
+
+        if y is not None:
+            y = y.reshape(N, 1)
+        if isinstance(s2, float) or isinstance(s2, int):
+            s2 = s2 * np.ones((N, 1))
+        elif isinstance(s2, np.ndarray):
+            s2 = s2.reshape(N, 1)
+        elif s2 is None:
+            s2 = None  # noiseless case
+        else:
+            raise TypeError(
+                "s2 type need to be \
+                            Union[np.ndarray, float, int, None]."
+            )
+        return X, y, s2
+
 
 class Posterior:
     """
     This object represents the posterior.
     """
 
     def __init__(self, hyp, alpha, sW, L, sn2_mult, Lchol):
```

### Comparing `GPyReg-1.0.1/gpyreg/isotropic_covariance_functions.py` & `GPyReg-1.0.2/gpyreg/isotropic_covariance_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from abc import ABC, abstractmethod
-
 import numpy as np
 from scipy.spatial.distance import cdist, pdist, squareform
 
 from .covariance_functions import AbstractKernel, Matern, SquaredExponential
 
+
 class AbstractIsotropicKernel(AbstractKernel):
     """Abstract base class for isotropic kernel functions.
 
     The two default hyperparameters are the log-lengthscale and
     log-outputscale.
     """
 
@@ -79,14 +78,15 @@
                     The plausible starting point.
 
             where ``cov_N`` is the number of hyperparameters.
         """
         cov_N = self.hyperparameter_count(X.shape[1])
         return _isotropic_bounds_info_helper(cov_N, X, y)
 
+
 class MaternIsotropic(AbstractIsotropicKernel, Matern):
     """
     Isotropic Matern kernel.
 
     Overrides `compute`. Inherits `hyperparameter_count` and
     `hyperparameter_info` from :class:`AbstractIsotropicKernel`. Inherits other
     methods from :class:`Matern`.
@@ -127,41 +127,44 @@
         ell = np.exp(hyp[0])
         sf2 = np.exp(2 * hyp[1])
 
         if X_star is None:
             if compute_diag:
                 tmp = np.zeros((N, 1))
             else:
-                tmp = squareform(
-                    pdist(X * np.sqrt(self.degree) / ell)
-                )
+                tmp = squareform(pdist(X * np.sqrt(self.degree) / ell))
         else:
             a = X * np.sqrt(self.degree) / ell
             b = X_star * np.sqrt(self.degree) / ell
             tmp = cdist(a, b)
 
         K = sf2 * self.f(tmp) * np.exp(-tmp)
 
         if compute_grad:
             if X_star is not None:
-                raise ValueError("X_star should be None when compute_grad is True.")
+                raise ValueError(
+                    "X_star should be None when compute_grad is True."
+                )
             dK = np.zeros((cov_N, N, N))
             # Gradient of cov length scale
-            K_ls = squareform(pdist(np.sqrt(self.degree) / ell * X, "sqeuclidean"))
+            K_ls = squareform(
+                pdist(np.sqrt(self.degree) / ell * X, "sqeuclidean")
+            )
             # With d=1 kernel there will be issues caused by zero
             # divisions. This is OK, the kernel is just not
             # differentiable there.
             with np.errstate(all="ignore"):
                 dK[0, :, :] = sf2 * (self.df(tmp) * np.exp(-tmp)) * K_ls
             # Gradient of cov output scale
             dK[1, :, :] = 2 * K
             return K, dK.transpose(1, 2, 0)
 
         return K
 
+
 class SquaredExponentialIsotropic(AbstractIsotropicKernel, SquaredExponential):
     """Isotropic squared exponential kernel.
 
     Overrides `compute`. Inherits `hyperparameter_count` and
     `hyperparameter_info` from :class:`AbstractIsotropicKernel`. Inherits other
     methods from :class:`SquaredExponential`.
     """
@@ -201,24 +204,27 @@
         else:
             tmp = cdist(X / ell, X_star / ell, "sqeuclidean")
 
         K = sf2 * np.exp(-tmp / 2)
 
         if compute_grad:
             if X_star is not None:
-                raise ValueError("X_star should be None when compute_grad is True.")
+                raise ValueError(
+                    "X_star should be None when compute_grad is True."
+                )
             dK = np.zeros((cov_N, N, N))
             # Gradient of cov length scale
             dK[0, :, :] = K * squareform(pdist(X / ell, "sqeuclidean"))
             # Gradient of cov output scale.
             dK[1, :, :] = 2 * K
             return K, dK.transpose(1, 2, 0)
 
         return K
 
+
 def _isotropic_bounds_info_helper(cov_N, X, y):
     _, D = X.shape
     tol = 1e-6
     lower_bounds = np.full((cov_N,), -np.inf)
     upper_bounds = np.full((cov_N,), np.inf)
     plausible_lower_bounds = np.full((cov_N,), -np.inf)
     plausible_upper_bounds = np.full((cov_N,), np.inf)
@@ -227,19 +233,21 @@
     width = np.mean(np.max(X, axis=0) - np.min(X, axis=0))
     min_width = np.min(width)
     max_width = np.max(width)
     if np.size(y) <= 1:
         y = np.array([0, 1])
     height = np.max(y) - np.min(y)
 
-    lower_bounds[0:cov_N - 1] = np.log(min_width) + np.log(tol)
-    upper_bounds[0:cov_N - 1] = np.log(max_width * 10)
-    plausible_lower_bounds[0:cov_N - 1] = np.log(min_width) + 0.5 * np.log(tol)
-    plausible_upper_bounds[0:cov_N - 1] = np.log(max_width)
-    plausible_x0[0:cov_N - 1] = np.log(np.std(X, ddof=1))
+    lower_bounds[0 : cov_N - 1] = np.log(min_width) + np.log(tol)
+    upper_bounds[0 : cov_N - 1] = np.log(max_width * 10)
+    plausible_lower_bounds[0 : cov_N - 1] = np.log(min_width) + 0.5 * np.log(
+        tol
+    )
+    plausible_upper_bounds[0 : cov_N - 1] = np.log(max_width)
+    plausible_x0[0 : cov_N - 1] = np.log(np.std(X, ddof=1))
 
     lower_bounds[cov_N - 1] = np.log(height) + np.log(tol)
     upper_bounds[cov_N - 1] = np.log(height * 10)
     plausible_lower_bounds[cov_N - 1] = np.log(height) + 0.5 * np.log(tol)
     plausible_upper_bounds[cov_N - 1] = np.log(height)
     plausible_x0[cov_N - 1] = np.log(np.std(y, ddof=1))
```

### Comparing `GPyReg-1.0.1/gpyreg/mean_functions.py` & `GPyReg-1.0.2/gpyreg/mean_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         omega = np.exp(hyp[(1 + D) : (1 + 2 * D)])
         z_2 = ((X - x_m) / omega) ** 2
         m = m_0 - 0.5 * np.sum(z_2, 1)
 
         if compute_grad:
             dm = np.zeros((N, mean_N))
             dm[:, 0] = np.ones((N,))
-            dm[:, 1 : D + 1] = (X - x_m) / omega ** 2
+            dm[:, 1 : D + 1] = (X - x_m) / omega**2
             dm[:, D + 1 :] = z_2
             return m, dm
 
         return m
 
 
 def _bounds_info_helper(mean_N, X, y, idx):
```

### Comparing `GPyReg-1.0.1/gpyreg/noise_functions.py` & `GPyReg-1.0.2/gpyreg/noise_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,31 +251,33 @@
             sn2 = np.spacing(1.0)
         else:
             sn2 = np.exp(2 * hyp[i])
             if compute_grad:
                 dsn2[:, i] = 2 * sn2
             i += 1
 
+        if s2 is None:
+            s2 = 0
         if self.parameters[1] == 1:
             sn2 += s2
         elif self.parameters[1] == 2:
             sn2 += np.exp(hyp[i]) * s2
             if compute_grad:
                 dsn2[:, i : i + 1] = np.exp(hyp[i]) * s2
             i += 1
 
         if self.parameters[2] == 1:
             if y is not None:
                 y_tresh = hyp[i]
                 w2 = np.exp(2 * hyp[i + 1])
                 zz = np.maximum(0, y_tresh - y)
 
-                sn2 += w2 * zz ** 2
+                sn2 += w2 * zz**2
                 if compute_grad:
                     dsn2[:, i : i + 1] = 2 * w2 * (y_tresh - y) * (zz > 0)
-                    dsn2[:, i + 1 : i + 2] = 2 * w2 * zz ** 2
+                    dsn2[:, i + 1 : i + 2] = 2 * w2 * zz**2
             i += 2
 
         if compute_grad:
             return sn2, dsn2
 
         return sn2
```

### Comparing `GPyReg-1.0.1/gpyreg/slice_sample.py` & `GPyReg-1.0.2/gpyreg/slice_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,15 +508,15 @@
                 samples[i_smpl, :] = xx
                 f_vals[i_smpl, :] = f_val
                 log_priors[i_smpl] = log_prior
 
             # Store summary statistics starting half.way into burn-in.
             if burn / 2 <= i < burn:
                 xx_sum += xx
-                xx_sq_sum += xx ** 2
+                xx_sq_sum += xx**2
 
                 # End of burn-in, update widths if using adaptive method.
                 if i == burn - 1 and self.adaptive:
                     burn_stored = np.floor(burn / 2)
                     # There can be numerical error here but then width
                     # has already shrunk to 0?
                     new_widths = np.fmin(
```

### Comparing `GPyReg-1.0.1/gpyreg/testing/test_covariance_functions.py` & `GPyReg-1.0.2/gpyreg/testing/test_covariance_functions.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/gpyreg/testing/test_gaussian_process.py` & `GPyReg-1.0.2/gpyreg/testing/test_gaussian_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -617,16 +617,16 @@
 
     pdf_tmp = np.reshape(scipy.stats.norm.pdf(x_star, scale=0.1), (-1, 1))
     tmp = np.dot(pdf_tmp, pdf_tmp.T)
     F_predict_var = np.sum(np.sum(f_cov[:, :, 0] * tmp)) * (30 / mu_N) ** 2
 
     F_bayes, F_bayes_var = gp.quad(0, 0.1, compute_var=True)
 
-    assert np.abs(F_bayes_var - F_predict_var) < 0.01
-    assert np.abs(F_bayes - F_predict) < 0.01
+    assert np.abs(F_bayes_var - F_predict_var) < 0.05
+    assert np.abs(F_bayes - F_predict) < 0.05
 
     def f(x):
         y = np.sin(x)
         if y < 0:
             return -np.abs(3 * y) ** 2
         return y
 
@@ -681,15 +681,15 @@
     # gp.plot()
 
 
 def test_setting_bounds():
     N = 20
     D = 2
     X = np.reshape(np.linspace(-10, 10, N), (-1, 2))
-    y = 1 + np.sin(X)
+    y = 1 + np.sum(np.sin(X), 1)
 
     gp = gpr.GP(
         D=D,
         covariance=gpr.covariance_functions.Matern(3),
         mean=gpr.mean_functions.ConstantMean(),
         noise=gpr.noise_functions.GaussianNoise(constant_add=True),
     )
@@ -828,15 +828,15 @@
     gp.fit(X=X, y=y, options=gp_train_5)
     gp.fit(X=X, y=y, options=gp_train_6)
     gp.fit(X=X, y=y, options=gp_train_7)
     gp.fit(X=X, y=y, options=gp_train_8)
 
 
 def test_fitting():
-    N = 1000
+    N = 500
     D = 1
     X = np.reshape(np.linspace(-10, 10, N), (-1, 1))
 
     gp = gpr.GP(
         D=D,
         covariance=gpr.covariance_functions.Matern(5),
         mean=gpr.mean_functions.ZeroMean(),
@@ -1054,15 +1054,15 @@
 
 
 def test__str__and__repr__():
     # 1-D:
     N = 20
     D = 1
     X = np.reshape(np.linspace(-10, 10, N), (-1, 1))
-    y = 1 + np.sin(X)
+    y = 1 + np.sum(np.sin(X), 1)
 
     gp = gpr.GP(
         D=D,
         covariance=gpr.covariance_functions.Matern(3),
         mean=gpr.mean_functions.ConstantMean(),
         noise=gpr.noise_functions.GaussianNoise(constant_add=True),
     )
@@ -1094,15 +1094,15 @@
     )
     assert "self.lower_bounds = [-10.8" in repr_
 
     # 2-D:
     N = 20
     D = 2
     X = np.reshape(np.linspace(-10, 10, N), (-1, 2))
-    y = 1 + np.sin(X)
+    y = 1 + np.sum(np.sin(X), 1)
 
     gp = gpr.GP(
         D=D,
         covariance=gpr.covariance_functions.Matern(3),
         mean=gpr.mean_functions.ConstantMean(),
         noise=gpr.noise_functions.GaussianNoise(constant_add=True),
     )
@@ -1129,7 +1129,40 @@
     assert "Covariance function: Matern" in str_
     repr_ = gp.__repr__()
     assert (
         "self.covariance = <gpyreg.covariance_functions.Matern object at "
         in repr_
     )
     assert "self.lower_bounds = [-10.8" in repr_
+
+
+def test_convert_shapes():
+    D = 3
+    gp = gpr.GP(
+        D=D,
+        covariance=gpr.covariance_functions.SquaredExponential(),
+        mean=gpr.mean_functions.NegativeQuadratic(),
+        noise=gpr.noise_functions.GaussianNoise(user_provided_add=True),
+    )
+    N = 10
+    X = np.ones((N, D))
+    y = np.ones(N)
+    s2 = np.ones(N)
+    X, y, s2 = gp._convert_shapes(X, y, s2)
+    assert X.shape == (N, D) and y.shape == (N, 1) and s2.shape == (N, 1)
+    s2 = None
+    X, y, s2 = gp._convert_shapes(X, y, s2)
+    assert X.shape == (N, D) and y.shape == (N, 1) and s2 is None
+    s2 = 1
+    X, y, s2 = gp._convert_shapes(X, y, s2)
+    assert (
+        X.shape == (N, D)
+        and y.shape == (N, 1)
+        and np.allclose(s2, np.ones((N, 1)))
+    )
+    with pytest.raises(AttributeError):
+        gp._convert_shapes(None, y, s2)
+    gp.X = X
+    y = np.ones(N)
+    s2 = np.ones(N)
+    X, y, s2 = gp._convert_shapes(None, y, s2)
+    assert X is None and y.shape == (N, 1) and s2.shape == (N, 1)
```

### Comparing `GPyReg-1.0.1/gpyreg/testing/test_gaussian_process_isotropic.py` & `GPyReg-1.0.2/gpyreg/testing/test_gaussian_process_isotropic.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 import numpy as np
 import pytest
 import scipy.stats
 from scipy.integrate import quad
 from scipy.misc import derivative
 
 import gpyreg as gpr
-from gpyreg.isotropic_covariance_functions import MaternIsotropic, SquaredExponentialIsotropic
+from gpyreg.isotropic_covariance_functions import (
+    MaternIsotropic,
+    SquaredExponentialIsotropic,
+)
 
 
 @pytest.mark.filterwarnings(
     """ignore:Matplotlib is currently using agg:UserWarning"""
 )
 def test_empty_gp():
     N = 20
@@ -201,17 +204,15 @@
         "noise_log_scale": (-np.inf, np.inf),
         "mean_const": (-np.inf, np.inf),
     }
 
     with pytest.raises(ValueError):
         gp.set_bounds(gp_bounds_mistaken)
 
-    hyp_arr = np.array(
-        [[-0.4630094, -0.2209450, -7.2947503, 0.03713608]]
-    )
+    hyp_arr = np.array([[-0.4630094, -0.2209450, -7.2947503, 0.03713608]])
     hyp = gp.hyperparameters_to_dict(hyp_arr)
     gp.set_hyperparameters(hyp)
     assert np.all(gp.get_hyperparameters(as_array=True) == hyp_arr)
 
     gp.set_hyperparameters(hyp_arr)
     assert np.all(gp.get_hyperparameters(as_array=True) == hyp_arr)
 
@@ -618,16 +619,16 @@
 
     pdf_tmp = np.reshape(scipy.stats.norm.pdf(x_star, scale=0.1), (-1, 1))
     tmp = np.dot(pdf_tmp, pdf_tmp.T)
     F_predict_var = np.sum(np.sum(f_cov[:, :, 0] * tmp)) * (30 / mu_N) ** 2
 
     F_bayes, F_bayes_var = gp.quad(0, 0.1, compute_var=True)
 
-    assert np.abs(F_bayes_var - F_predict_var) < 0.01
-    assert np.abs(F_bayes - F_predict) < 0.01
+    assert np.abs(F_bayes_var - F_predict_var) < 0.05
+    assert np.abs(F_bayes - F_predict) < 0.05
 
     def f(x):
         y = np.sin(x)
         if y < 0:
             return -np.abs(3 * y) ** 2
         return y
 
@@ -682,15 +683,15 @@
     # gp.plot()
 
 
 def test_setting_bounds():
     N = 20
     D = 2
     X = np.reshape(np.linspace(-10, 10, N), (-1, 2))
-    y = 1 + np.sin(X)
+    y = 1 + np.sum(np.sin(X), 1)
 
     gp = gpr.GP(
         D=D,
         covariance=MaternIsotropic(3),
         mean=gpr.mean_functions.ConstantMean(),
         noise=gpr.noise_functions.GaussianNoise(constant_add=True),
     )
@@ -829,15 +830,15 @@
     gp.fit(X=X, y=y, options=gp_train_5)
     gp.fit(X=X, y=y, options=gp_train_6)
     gp.fit(X=X, y=y, options=gp_train_7)
     gp.fit(X=X, y=y, options=gp_train_8)
 
 
 def test_fitting():
-    N = 1000
+    N = 500
     D = 1
     X = np.reshape(np.linspace(-10, 10, N), (-1, 1))
 
     gp = gpr.GP(
         D=D,
         covariance=MaternIsotropic(5),
         mean=gpr.mean_functions.ZeroMean(),
@@ -1095,15 +1096,15 @@
     )
     assert "self.lower_bounds = [-10.8" in repr_
 
     # 2-D:
     N = 20
     D = 2
     X = np.reshape(np.linspace(-10, 10, N), (-1, 2))
-    y = 1 + np.sin(X)
+    y = 1 + np.sum(np.sin(X), 1)
 
     gp = gpr.GP(
         D=D,
         covariance=MaternIsotropic(3),
         mean=gpr.mean_functions.ConstantMean(),
         noise=gpr.noise_functions.GaussianNoise(constant_add=True),
     )
```

### Comparing `GPyReg-1.0.1/gpyreg/testing/test_isotropic_covariance_functions.py` & `GPyReg-1.0.2/gpyreg/testing/test_isotropic_covariance_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import numpy as np
 import pytest
 
-from gpyreg.covariance_functions import AbstractKernel, Matern, SquaredExponential
+from gpyreg.covariance_functions import (
+    AbstractKernel,
+    Matern,
+    SquaredExponential,
+)
 from gpyreg.isotropic_covariance_functions import (
     AbstractIsotropicKernel,
     MaternIsotropic,
     SquaredExponentialIsotropic,
 )
 
 
@@ -99,14 +103,15 @@
     X = (np.random.multivariate_normal(np.zeros(N), diag_cov, D)).T
     hyp_D = 2
     diag_cov = np.eye(hyp_D) * (0.2)
     hyp = np.random.multivariate_normal(np.zeros(hyp_D), diag_cov)
 
     _test_kernel_gradient_(matern_fun, hyp, X)
 
+
 def _test_kernel_gradient_(
     kernel_fun: AbstractKernel,
     hyp,
     X: np.ndarray,
     X_star: np.ndarray = None,
     h=1e-5,
     eps=1e-4,
@@ -151,14 +156,15 @@
         f_neg_2h = kernel_fun.compute(hyp_new, X, X_star)
 
         finite_diff[:, :, idx] = -f_2h + 8.0 * f_h - 8.0 * f_neg_h + f_neg_2h
         finite_diff[:, :, idx] = finite_diff[:, :, idx] / (12 * h)
 
     assert np.all(np.abs(finite_diff - dK) <= eps)
 
+
 def test_matern_isotropic_against_anisotropic():
     N = 10
     M = 5
     for degree in [1, 3, 5]:
         D = np.random.randint(1, 11)
 
         # Isotropic kernel:
@@ -179,23 +185,26 @@
 
         K1_iso = matern_iso.compute(hyp_iso, X)
         K1 = matern.compute(hyp, X)
         assert np.allclose(K1_iso, K1), f"degree {degree}"
 
         K2_iso, dK2_iso = matern_iso.compute(hyp_iso, X, compute_grad=True)
         K2, dK2 = matern.compute(hyp, X, compute_grad=True)
-        dK2 = np.dstack([dK2[:, :, 0:-1].sum(axis=2, keepdims=True), dK2[:, :, [-1]]])
+        dK2 = np.dstack(
+            [dK2[:, :, 0:-1].sum(axis=2, keepdims=True), dK2[:, :, [-1]]]
+        )
         assert np.allclose(K2_iso, K2), f"degree {degree}"
         assert np.allclose(dK2_iso, dK2, equal_nan=True), f"degree {degree}"
         assert np.allclose(K2_iso, K1_iso), f"degree {degree}"
 
         K3_iso = matern_iso.compute(hyp_iso, X, X_star)
         K3 = matern.compute(hyp, X, X_star)
         assert np.allclose(K3_iso, K3), f"degree {degree}"
 
+
 def test_squared_exponential_isotropic_against_anisotropic():
     N = 10
     M = 5
     D = np.random.randint(1, 11)
 
     # Isotropic kernel:
     sqexp_iso = SquaredExponentialIsotropic()
@@ -215,16 +224,17 @@
 
     K1_iso = sqexp_iso.compute(hyp_iso, X)
     K1 = sqexp.compute(hyp, X)
     assert np.allclose(K1_iso, K1)
 
     K2_iso, dK2_iso = sqexp_iso.compute(hyp_iso, X, compute_grad=True)
     K2, dK2 = sqexp.compute(hyp, X, compute_grad=True)
-    dK2 = np.dstack([dK2[:, :, 0:-1].sum(axis=2, keepdims=True), dK2[:, :, [-1]]])
+    dK2 = np.dstack(
+        [dK2[:, :, 0:-1].sum(axis=2, keepdims=True), dK2[:, :, [-1]]]
+    )
     assert np.allclose(K2_iso, K2)
     assert np.allclose(dK2_iso, dK2)
     assert np.allclose(K2_iso, K1_iso)
 
     K3_iso = sqexp_iso.compute(hyp_iso, X, X_star)
     K3 = sqexp.compute(hyp, X, X_star)
     assert np.allclose(K3_iso, K3)
-
```

### Comparing `GPyReg-1.0.1/gpyreg/testing/test_mean_functions.py` & `GPyReg-1.0.2/gpyreg/testing/test_mean_functions.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/gpyreg/testing/test_noise_functions.py` & `GPyReg-1.0.2/gpyreg/testing/test_noise_functions.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/gpyreg/testing/test_slice_sample.py` & `GPyReg-1.0.2/gpyreg/testing/test_slice_sample.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/gpyreg/testing/test_smoothbox.py` & `GPyReg-1.0.2/gpyreg/testing/test_smoothbox.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/gpyreg/testing/test_smoothbox_student_t.py` & `GPyReg-1.0.2/gpyreg/testing/test_smoothbox_student_t.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/pylintrc` & `GPyReg-1.0.2/pylintrc`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.1/pyproject.toml` & `GPyReg-1.0.2/pyproject.toml`

 * *Files identical despite different names*

