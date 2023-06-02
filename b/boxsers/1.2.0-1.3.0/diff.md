# Comparing `tmp/boxsers-1.2.0.tar.gz` & `tmp/boxsers-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxsers-1.2.0.tar", last modified: Tue Apr  4 19:52:56 2023, max compression
+gzip compressed data, was "boxsers-1.3.0.tar", last modified: Fri Jun  2 18:23:38 2023, max compression
```

## Comparing `boxsers-1.2.0.tar` & `boxsers-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 19:52:56.802832 boxsers-1.2.0/
--rw-rw-rw-   0        0        0     1093 2021-08-13 16:59:11.000000 boxsers-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     8765 2023-04-04 19:52:56.802832 boxsers-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10872 2023-04-04 19:42:12.000000 boxsers-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 19:52:56.749464 boxsers-1.2.0/boxsers/
--rw-rw-rw-   0        0        0      673 2022-09-26 19:10:22.000000 boxsers-1.2.0/boxsers/__init__.py
--rw-rw-rw-   0        0        0      987 2022-07-15 15:44:15.000000 boxsers-1.2.0/boxsers/_boxsers_utils.py
--rw-rw-rw-   0        0        0    22039 2021-10-08 20:25:36.000000 boxsers-1.2.0/boxsers/data_augmentation.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:52:56.800826 boxsers-1.2.0/boxsers/machine_learning/
--rw-rw-rw-   0        0        0      380 2022-07-20 13:18:32.000000 boxsers-1.2.0/boxsers/machine_learning/__init__.py
--rw-rw-rw-   0        0        0    12773 2022-09-26 19:07:40.000000 boxsers-1.2.0/boxsers/machine_learning/classification.py
--rw-rw-rw-   0        0        0     7295 2022-07-13 19:35:31.000000 boxsers-1.2.0/boxsers/machine_learning/clustering.py
--rw-rw-rw-   0        0        0    24197 2023-04-04 19:42:12.000000 boxsers-1.2.0/boxsers/machine_learning/dimension_reduction.py
--rw-rw-rw-   0        0        0    35367 2023-04-04 19:42:12.000000 boxsers-1.2.0/boxsers/machine_learning/neural_networks.py
--rw-rw-rw-   0        0        0     7667 2022-07-20 19:26:31.000000 boxsers-1.2.0/boxsers/machine_learning/validation_metrics.py
--rw-rw-rw-   0        0        0     6667 2022-11-17 19:15:22.000000 boxsers-1.2.0/boxsers/misc_tools.py
--rw-rw-rw-   0        0        0    11083 2022-03-15 19:24:28.000000 boxsers-1.2.0/boxsers/preprocessing.py
--rw-rw-rw-   0        0        0    18237 2022-11-17 19:02:06.000000 boxsers-1.2.0/boxsers/visual_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:52:56.770842 boxsers-1.2.0/boxsers.egg-info/
--rw-rw-rw-   0        0        0     8765 2023-04-04 19:52:56.000000 boxsers-1.2.0/boxsers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-04-04 19:52:56.000000 boxsers-1.2.0/boxsers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 19:52:56.000000 boxsers-1.2.0/boxsers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-04 19:52:56.000000 boxsers-1.2.0/boxsers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-04 19:52:56.000000 boxsers-1.2.0/boxsers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 19:52:56.802832 boxsers-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-04-04 19:52:41.000000 boxsers-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:23:38.809660 boxsers-1.3.0/
+-rw-rw-rw-   0        0        0     1093 2021-08-13 16:59:11.000000 boxsers-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     8765 2023-06-02 18:23:38.808670 boxsers-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11114 2023-04-06 13:13:22.000000 boxsers-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 18:23:38.746309 boxsers-1.3.0/boxsers/
+-rw-rw-rw-   0        0        0      673 2022-09-26 19:10:22.000000 boxsers-1.3.0/boxsers/__init__.py
+-rw-rw-rw-   0        0        0      987 2022-07-15 15:44:15.000000 boxsers-1.3.0/boxsers/_boxsers_utils.py
+-rw-rw-rw-   0        0        0    27447 2023-05-31 17:04:22.000000 boxsers-1.3.0/boxsers/data_augmentation.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:23:38.807652 boxsers-1.3.0/boxsers/machine_learning/
+-rw-rw-rw-   0        0        0      380 2022-07-20 13:18:32.000000 boxsers-1.3.0/boxsers/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0    12773 2022-09-26 19:07:40.000000 boxsers-1.3.0/boxsers/machine_learning/classification.py
+-rw-rw-rw-   0        0        0     7295 2022-07-13 19:35:31.000000 boxsers-1.3.0/boxsers/machine_learning/clustering.py
+-rw-rw-rw-   0        0        0    24197 2023-04-06 13:16:16.000000 boxsers-1.3.0/boxsers/machine_learning/dimension_reduction.py
+-rw-rw-rw-   0        0        0    35367 2023-04-04 19:42:12.000000 boxsers-1.3.0/boxsers/machine_learning/neural_networks.py
+-rw-rw-rw-   0        0        0     7667 2022-07-20 19:26:31.000000 boxsers-1.3.0/boxsers/machine_learning/validation_metrics.py
+-rw-rw-rw-   0        0        0     7755 2023-05-31 17:28:13.000000 boxsers-1.3.0/boxsers/misc_tools.py
+-rw-rw-rw-   0        0        0    13083 2023-06-02 18:14:58.000000 boxsers-1.3.0/boxsers/preprocessing.py
+-rw-rw-rw-   0        0        0    18237 2022-11-17 19:02:06.000000 boxsers-1.3.0/boxsers/visual_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:23:38.762330 boxsers-1.3.0/boxsers.egg-info/
+-rw-rw-rw-   0        0        0     8765 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 18:23:38.000000 boxsers-1.3.0/boxsers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 18:23:38.809660 boxsers-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-05-31 17:28:54.000000 boxsers-1.3.0/setup.py
```

### Comparing `boxsers-1.2.0/LICENSE.txt` & `boxsers-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/PKG-INFO` & `boxsers-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsers
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package that provides a full range of functionality to process and analyze vibrational spectra (Raman, SERS, FTIR, etc.).
 Home-page: https://github.com/ALebrun-108/BoxSERS
 Author: Alexis Lebrun
 Author-email: alexis.lebrun.1@ulaval.ca
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boxsers-1.2.0/README.md` & `boxsers-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -246,15 +246,20 @@
 
 ### Module ``dimension_reduction``
 This module provides different techniques to perform dimensionality reduction of
 vibrational spectra.
 
 * **SpectroPCA** : Principal Component Analysis (PCA) model object.
 
-
+```python
+pca_model = SpectroPCA(n_comp=10)
+pca_model.fit_model(sp)
+pca_model.scatter_plot(sp, label, component_x=1, component_y=2, fontsize=13, class_names=['Mol. A', 'Mol. B', 'Mol. C']) 
+```
+![test image size](fig/PCA_scatterplot.png)
 ### Module ``clustering``
 This module provides unsupervised learning models for vibrational spectra cluster analysis.
 
 * **SpectroKmeans** : K-Means clustering model.
 
 
 * **SpectroGmixture** : Gaussian mixture probability distribution model.
```

### Comparing `boxsers-1.2.0/boxsers/__init__.py` & `boxsers-1.3.0/boxsers/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/boxsers/_boxsers_utils.py` & `boxsers-1.3.0/boxsers/_boxsers_utils.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/boxsers/data_augmentation.py` & `boxsers-1.3.0/boxsers/data_augmentation.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,21 +6,95 @@
 This module provides funtions to generate new spectra by adding different variations to
 existing spectra.
 """
 import numpy as np
 from sklearn.utils import shuffle
 
 
-def aug_mixup(sp, lab, n_spec=2, alpha=0.5, quantity=1, mode='default', shuffle_enabled=True):
+def _range_converter(param_range, multiplier_cond=False):
+    """
+    Returns superior and inferior bounds according to a given range.
+
+    Parameters:
+        param_range : float or integer, list or tuple
+            Range of possible values for a given value. These values can be specified as follows:
+                - param_range = (a, b) or [a, b] --> a is the left limit value and b is the right limit value.
+                - (multiplier_cond=False)
+                    - param_range = a --> -a is the left limit value and +a is the right limit value.
+                - (multiplier_cond=True)
+                    - param_range = a --> (1 - a) is the left limit value and (1 + a) is the right limit value.
+
+        multiplier_cond : boolean, default=False
+            See above for information
+
+    Returns:
+        (float, int) Inferior boudary value.
+
+        (float, int) Superior boundary value.
+    """
+    param_range_inf = 0.0
+    param_range_sup = 0.0
+
+    if isinstance(param_range, list):
+        param_range_inf = param_range[0]
+        param_range_sup = param_range[1]
+    elif isinstance(param_range, (float, int)) and not multiplier_cond:
+        param_range_inf = -param_range
+        param_range_sup = param_range
+    elif isinstance(param_range, (float, int)) and multiplier_cond:
+        param_range_inf = 1 - param_range
+        param_range_sup = 1 + param_range
+    return param_range_inf, param_range_sup
+
+
+def _xshift(sp, x_shft, fill_mode, fill_value):
+    """
+    Moves spectrum/spectra along the pixel axis. Uses the same parameters as the aug_xshift function.
+    """
+    # sp initialization, sp is forced to be a two-dimensional array
+    sp = np.array(sp, ndmin=2)
+
+    # initialization and space allocation for shft_sp and fill_value
+    shft_sp = np.zeros_like(sp)
+    fill_value_left = np.zeros_like(x_shft)
+    fill_value_right = np.zeros_like(x_shft)
+    # x_shft index splitting for positive and negative shifts
+    positives = np.argwhere(x_shft > 0)[:, 0]
+    negatives = np.argwhere(x_shft < 0)[:, 0]
+
+    if fill_mode == 'edge':
+        fill_value_left = sp[:, 0]
+        fill_value_right = sp[:, -1]
+    elif fill_mode == 'fixed':
+        fill_value_left[:] = fill_value
+        fill_value_right[:] = fill_value
+    else:
+        print('Invalid fill_mode: fill value(s) has been set to zero')
+
+    for p in positives:
+        shft_sp[p, :int(x_shft[p])] = fill_value_left[p]
+        shft_sp[p, int(x_shft[p]):] = sp[p, :-int(x_shft[p])]
+    for n in negatives:
+        shft_sp[n, int(x_shft[n]):] = fill_value_right[n]
+        shft_sp[n, :int(x_shft[n])] = sp[n, -int(x_shft[n]):]
+    return shft_sp
+
+
+def aug_mixup(sp, lab, n_spec=2, alpha=0.5, quantity=1, shuffle_enabled=True, return_infos=False):
     """
     Randomly generates new spectra by mixing together several spectra with
     a Dirichlet probability distribution.
 
     This function is inspired of the Mixeup method proposed by zang (Zhang, Hongyi, et al. 2017).
 
+    Notes:
+        Updated [2023-05-31]:
+            - parameter `mode` removed, use `return_infos` instead for parameters selection and validation.
+            - Computation time and memory consumption reduced !
+
     Parameters:
         sp : array
             Input Spectrum(s), array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
             for a single spectrum.
 
         lab : array
             Labels(must be binary) assigned the "sp" spectra, array shape = (n_spectra, n_classes).
@@ -31,168 +105,182 @@
         alpha : float
             Dirichlet distribution concentration parameter.
 
         quantity : integer, default=1
             Quantity of new spectra generated for one spectrum. If less than or equal to zero, no new
             spectrum is generated.
 
-        mode(str):{'default', 'review'}, default='default'
-            Function mode used.
-                -'default': Randomly generates new spectra. Used for data augmentation.
-                -'review': Generates spectra with the selected limit values. Used for
-                    parameters selection and validation.
-
         shuffle_enabled : boolean, default=True
             If True, shuffles the new spectra.
 
+        return_infos : boolean, default=False
+            If True, returns the indexes and the lambda values of the spectra mixed together
+
     Return:
         (array) New spectra generated.
 
         (array) New labels generated.
+
+        (array) Optional; Indexes of the spectra mixed together.
+
+        (array) Optional; Lambda values of the spectra mixed together.
     """
     # sp initialization, sp is forced to be a two-dimensional array
     sp = np.array(sp, ndmin=2)
     # lab initialization, lab is forced to be a two-dimensional array
     lab = np.array(lab, ndmin=2)
 
-    sp_len = sp.shape[1]  # spectrum length
+    n_spectra, sp_len = sp.shape  # number of spectra, spectrum length
     lab_len = lab.shape[1]  # label length
-    # defining empty arrays to contain the newly generated data
-    sp_aug = np.empty(shape=(1, sp_len))
-    lab_aug = np.empty(shape=(1, lab_len))
+
+    # array preallocation
+    sp_aug = np.zeros((quantity * n_spectra, sp_len))
+    lab_aug = np.zeros((quantity * n_spectra, lab_len))
 
     # initialization and space allocation
     alpha_array = np.ones(n_spec) * alpha
     # Lambda values generated with a dirichlet distribution
-    lam_s = np.random.dirichlet(alpha_array, sp.shape[0])
-    arr_review = []
-    lab_review = []
-    lam_review = []
+    lambda_values = np.random.dirichlet(alpha_array, quantity*n_spectra)
 
-    if mode == 'review':
-        # generation of new spectra
-        sp_sum = np.zeros(sp.shape)
-        lab_sum = np.zeros(lab.shape)
+    # random spectra index selection
+    random_indexes = np.random.choice(n_spectra, size=(quantity * n_spectra, n_spec), replace=True)
 
-        for n in range(0, n_spec):
-            arr_, lab_ = shuffle(sp, lab)
-            lam = np.array(lam_s[:, n], ndmin=2).transpose()
-            sp_sum = sp_sum + lam * arr_
-            lab_sum = lab_sum + lam * lab_
-            arr_review.append(arr_)
-            lab_review.append(lab_)
-            lam_review.append(lam)
-        sp_aug = sp_sum
-        lab_aug = lab_sum
-
-        arr_review.append(sp_aug)
-        lab_review.append(lab_aug)
-        return arr_review, lab_review, lam_review
-
-    elif mode == 'default':
-
-        for i in range(quantity):
-            sp_sum = np.zeros(sp.shape)
-            lab_sum = np.zeros(lab.shape)
-
-            for n in range(0, n_spec):
-                arr_, lab_ = shuffle(sp, lab)
-                lam = np.array(lam_s[:, n], ndmin=2).transpose()
-                sp_sum = sp_sum + lam * arr_
-                lab_sum = lab_sum + lam * lab_
-
-            sp_aug = np.vstack((sp_aug, sp_sum))
-            lab_aug = np.vstack((lab_aug, lab_sum))
-
-        # removal of the first empty sample
-        sp_aug = np.delete(sp_aug, 0, 0)
-        lab_aug = np.delete(lab_aug, 0, 0)
-
-        if shuffle_enabled:
-            # spectra and labels are randomly mixed
-            sp_aug, lab_aug = shuffle(sp_aug, lab_aug)
+    for i, (lam, index) in enumerate(zip(lambda_values, random_indexes)):
+        mixed_sp = lam[:, np.newaxis] * sp[index]
+        mixed_lab = lam[:, np.newaxis] * lab[index]
+        sp_aug[i] += np.sum(mixed_sp, axis=0)
+        lab_aug[i] += np.sum(mixed_lab, axis=0)
+
+    if shuffle_enabled:
+        # spectra, labels, indexes and lambda are randomly shuffled
+        sp_aug, lab_aug, random_indexes, lambda_values = shuffle(sp_aug, lab_aug, random_indexes, lambda_values)
+
+    if return_infos:
+        # returns the indexes for the spectra mixed together
+        return sp_aug, lab_aug, random_indexes, lambda_values
 
     return sp_aug, lab_aug
 
 
-def aug_multiplier(sp, lab, mult_range, quantity=1, shuffle_enabled=True):
+def aug_newband(sp, lab, inv_p=None, inv_p_degree=4, intensity_range=(0.05, 0.95), width_range=(2, 5),
+                quantity=1, shuffle_enabled=True, return_band=False):
     """
-    Randomly generates new spectra with multiplicative factors applied
+    Randomly generates new spectra with additionnal Gaussian peak added.
 
     Parameters:
         sp : array
             Input Spectrum(s), array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
             for a single spectrum.
 
         lab : array
             Labels assigned the "sp" spectra, array shape = (n_spectra,) for integer labels
             and (n_spectra, n_classes) for binary labels.
 
-        mult_range : integer, list or tuple
-            Values delimiting the range of possible values for random multiplier. These values can be
-            specified as follows:
-                - mult_range = (a, b) or [a, b] --> a is the left limit value and b is the right limit value.
-                - mult_range = a --> (1 - a) is the left limit value and (1 + a) is the right limit value.
+        inv_p: string, default=None,
+            Reference value for the inverse probability density function. If None, it is the input spectra
+            that will be used.
+
+        inv_p_degree : float, default=1
+            Determines where additional Raman bands will be more likely positioned on the spectrum according
+            to inv_p.
+                - > 0 : positioned at different locations than input spectrum bands.
+                - = 0 : randomly postioned.
+                - < 0 : positioned close to input spectrum bands.
+
+        intensity_range : float or integer, list or tuple, default = (0.02, 0.98)
+            Values delimiting the range of possible values for the Raman band intensity..
+
+        width_range : list or tuple, default = (1, 5)
+            Values delimiting the range of possible values for the Raman band width (in pixels).
 
         quantity : integer, default=1
             Quantity of new spectra generated for one spectrum. If less than or equal to zero, no new
             spectrum is generated.
 
         shuffle_enabled : boolean, default=True
             If True, shuffles the new spectra.
 
+        return_band : boolean, default=False
+            If True, returns the individual peak added.
+
     Return:
         (array) New spectra generated.
 
         (array) New labels generated.
+
+        (array) Optional; New Raman bands added.
     """
     # sp initialization, sp is forced to be a two-dimensional array
     sp = np.array(sp, ndmin=2)
     # lab initialization, lab is forced to be a two-dimensional array
     lab = np.array(lab, ndmin=2)
 
-    sp_len = sp.shape[1]  # spectrum length
-    lab_len = lab.shape[1]  # label length
-    # defining empty arrays to contain the newly generated data
-    sp_aug = np.empty(shape=(1, sp_len))
-    lab_aug = np.empty(shape=(1, lab_len))
-    mult_range_inf = 0
-    mult_range_sup = 0
-
-    if isinstance(mult_range, list):
-        mult_range_inf = mult_range[0]
-        mult_range_sup = mult_range[1]
-    elif isinstance(mult_range, (float, int)):
-        mult_range_inf = 1 - mult_range
-        mult_range_sup = 1 + mult_range
-
-    for i in range(quantity):
-        # random generation of multiplier(s) using uniform distribution
-        multiplier = np.random.uniform(mult_range_inf, mult_range_sup, (sp.shape[0], 1))
+    n_spectra, sp_len = sp.shape  # number of spectra, spectrum length
+
+    # array preallocation
+    sp_aug = np.empty((quantity * n_spectra, sp_len))
+    added_bands = np.empty((quantity * n_spectra, sp_len))
+    # as no changes are made to the labels, they are repeated to match the new spectra generated.
+    lab_aug = np.repeat(lab, quantity, axis=0)
+
+    if inv_p is None:
+        # spectra values are used as the input for the inverse probability density
+        inv_p = sp
+    else:
+        # inverse probability density function is given
+        inv_p = np.array(inv_p, ndmin=2)
+
+    # inverse density probabilities calculation
+    inv_density = 1.0 / (inv_p ** inv_p_degree)
+    # normalizing the probabilities to sum up to 1 for each row
+    inverse_density_norm = inv_density / inv_density.sum(axis=1, keepdims=1)
+    inverse_density_norm = np.repeat(inverse_density_norm, quantity, axis=0)
+
+    # upper and lower bounds are determined from the given range
+    intensity_range_inf, intensity_range_sup = _range_converter(intensity_range, multiplier_cond=True)
+
+    # upper and lower bounds are multiplied by the average intensity of each spectrum
+    intensity_inf = np.mean(sp, axis=1) * intensity_range_inf
+    intensity_sup = np.mean(sp, axis=1) * intensity_range_sup
+
+    # random band_intensities and band_widths generation using uniform distribution
+    band_intensities = np.random.uniform(intensity_inf.repeat(quantity), intensity_sup.repeat(quantity))
+    band_widths = np.random.uniform(width_range[0]/2, width_range[1]/2, size=(quantity * n_spectra))
+
+    indexes = np.arange(sp_len)
+    for i, (intensity, width) in enumerate(zip(band_intensities, band_widths)):
+        # choose a random index based on the inverse density probabilities
+        random_index = np.random.choice(sp_len, p=inverse_density_norm[i])
+        # generates a new Raman Gaussian band
+        new_band = intensity * np.exp(-0.5 * ((indexes - random_index) / width) ** 2)
         # generation of new spectra
-        sp_mult = sp*multiplier
-        # new spectra & labels are appended together
-        sp_aug = np.vstack((sp_aug, sp_mult))
-        lab_aug = np.vstack((lab_aug, lab))
-
-    # first empty sample(first row) is removed from spectra and label
-    sp_aug = np.delete(sp_aug, 0, 0)
-    lab_aug = np.delete(lab_aug, 0, 0)
+        sp_newband = sp[i // quantity] + new_band
+
+        # sp_aug and added band are filled progressively
+        sp_aug[i] = sp_newband
+        added_bands[i] = new_band
 
     if shuffle_enabled:
-        # spectra and labels are randomly mixed
-        sp_aug, lab_aug = shuffle(sp_aug, lab_aug)
+        # spectra, labels and new bands are randomly shuffled
+        sp_aug, lab_aug, added_bands = shuffle(sp_aug, lab_aug, added_bands)
 
+    if return_band:
+        # the new Raman peak is also returned
+        return sp_aug, lab_aug, added_bands
     return sp_aug, lab_aug
 
 
 def aug_noise(sp, lab, snr=10, quantity=1, noise_type='proportional', shuffle_enabled=True, return_noise=False):
     """
     Randomly generates new spectra with Gaussian noise added.
 
+    Notes:
+        Updated [2023-05-31]:
+            - Computation time and memory consumption reduced !
+
     Parameters:
         sp : array
             Input Spectrum(s), array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
             for a single spectrum.
 
         lab : array
             Labels assigned the "sp" spectra, array shape = (n_spectra,) for integer labels
@@ -219,96 +307,87 @@
             If True, returns the last generated noise signal
 
     Return:
         (array) New spectra generated.
 
         (array) New labels generated.
 
-        (array) Last noise signal.
+        (array) Optional; Noise generated.
     """
     # sp initialization, sp is forced to be a two-dimensional array
     sp = np.array(sp, ndmin=2)
     # lab initialization, lab is forced to be a two-dimensional array
     lab = np.array(lab, ndmin=2)
 
-    sp_len = sp.shape[1]  # spectrum length
-    lab_len = lab.shape[1]  # label length
-    # defining empty arrays to contain the newly generated data
-    sp_aug = np.empty(shape=(1, sp_len))
-    lab_aug = np.empty(shape=(1, lab_len))
-
-    # proportional noise varies with the intensity values of the spectra
-    sp_abs = abs(sp)
+    n_spectra, sp_len = sp.shape  # number of spectra, spectrum length
 
-    # uniform noise varies with the average intensity of the spectra
-    sp_avg = np.mean(sp, axis=1, keepdims=True)
+    # array preallocation
+    sp_aug = np.empty((quantity * n_spectra, sp_len))
+    # as no changes are made to the labels, they are repeated to match the new spectra generated.
+    lab_aug = np.repeat(lab, quantity, axis=0)
 
-    # print(f"{sp_abs=}")  # Debug lines
-    # print(f"{sp_avg=}")
+    if noise_type == 'proportional':
+        # proportional noise varies with the intensity values of the spectra
+        std_ref = abs(sp)  # shape = (n_spectra, sp_len)
+    elif noise_type == 'uniform':
+        # uniform noise varies with the average intensity of the spectra
+        std_ref = np.mean(sp, axis=1, keepdims=True)  # shape = (n_spectra, 1)
+    else:
+        std_ref = 0
 
     # Converts to dB
-    sp_avg_db = 10 * np.log10(sp_avg)
-    sp_abs_db = 10 * np.log10(sp_abs)
+    std_db = 10 * np.log10(std_ref)
 
     # Calculate noise in dB
-    noise_avg_db = sp_avg_db - snr
-    noise_abs_db = sp_abs_db - snr
+    noise_db = std_db - snr
 
     # Convert noise to spectra intensity values
-    noise_avg = 10 ** (noise_avg_db / 10)
-    noise_abs = 10 ** (noise_abs_db / 10)
+    noise_std = 10 ** (noise_db / 10)
+    noise_std = np.repeat(noise_std, quantity, axis=0)
 
-    if noise_type == 'proportional':
-        for i in range(quantity):
-            # generation of new spectra
-            noise = np.random.normal(0, noise_abs)
-            # new spectra & labels are appended together
-            sp_aug = np.vstack((sp_aug, sp+noise))
-            lab_aug = np.vstack((lab_aug, lab))
-    elif noise_type == 'uniform':
-        for i in range(quantity):
-            # generation of new spectra
-            noise = np.random.normal(0, noise_avg, size=sp.shape)
-            # new spectra & labels are appended together
-            sp_aug = np.vstack((sp_aug, sp+noise))
-            lab_aug = np.vstack((lab_aug, lab))
-
-    # removal of the first empty sample
-    sp_aug = np.delete(sp_aug, 0, 0)
-    lab_aug = np.delete(lab_aug, 0, 0)
+    noises = np.random.normal(0, noise_std, size=sp_aug.shape)
+
+    for i, noise in enumerate(noises):
+        # generation of new spectra
+        sp_noise = sp[i // quantity] + noise
+        # sp_aug is filled progressively
+        sp_aug[i] = sp_noise
 
     if shuffle_enabled:
-        # spectra and labels are randomly mixed
-        sp_aug, lab_aug = shuffle(sp_aug, lab_aug)
+        # spectra, labels and noise are randomly mixed
+        sp_aug, lab_aug, noises = shuffle(sp_aug, lab_aug, noises)
 
     if return_noise:
         # added noise is returned
-        return sp_aug, lab_aug, noise
-    else:
-        return sp_aug, lab_aug
+        return sp_aug, lab_aug, noises
+    return sp_aug, lab_aug
 
 
-def aug_offset(sp, lab, offset_range, quantity=1, shuffle_enabled=True):
+def aug_multiplier(sp, lab, mult_range, quantity=1, shuffle_enabled=True):
     """
-    Randomly generates new spectra shifted in intensity.
+    Randomly generates new spectra with multiplicative factors applied
+
+    Notes:
+        Updated [2023-05-31]:
+            - Computation time and memory consumption reduced !
 
     Parameters:
         sp : array
             Input Spectrum(s), array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
             for a single spectrum.
 
         lab : array
             Labels assigned the "sp" spectra, array shape = (n_spectra,) for integer labels
             and (n_spectra, n_classes) for binary labels.
 
-        offset_range : integer, list or tuple
-            Values delimiting the range of possible values for random intensity offset. These values can be
+        mult_range : float or integer, list or tuple
+            Values delimiting the range of possible values for random multiplier. These values can be
             specified as follows:
-                - offset_range = (a, b) or [a, b] --> a is the left limit value and b is the right limit value.
-                - offset_range = a --> -a is the left limit value and +a is the right limit value.
+                - mult_range = (a, b) or [a, b] --> a is the left limit value and b is the right limit value.
+                - mult_range = a --> (1 - a) is the left limit value and (1 + a) is the right limit value.
 
         quantity : integer, default=1
             Quantity of new spectra generated for one spectrum. If less than or equal to zero, no new
             spectrum is generated.
 
         shuffle_enabled : boolean, default=True
             If True, shuffles the new spectra.
@@ -319,187 +398,138 @@
         (array) New labels generated.
     """
     # sp initialization, sp is forced to be a two-dimensional array
     sp = np.array(sp, ndmin=2)
     # lab initialization, lab is forced to be a two-dimensional array
     lab = np.array(lab, ndmin=2)
 
-    sp_len = sp.shape[1]  # spectrum length
-    lab_len = lab.shape[1]  # label length
-    # defining empty arrays to contain the newly generated data
-    sp_aug = np.empty(shape=(1, sp_len))
-    lab_aug = np.empty(shape=(1, lab_len))
-    # average intensity is calculated for each spectra
-    sp_mean = np.mean(sp, axis=1, keepdims=True)
+    n_spectra, sp_len = sp.shape  # number of spectra, spectrum length
 
-    offset_range_inf = 0
-    offset_range_sup = 0
+    # array preallocation
+    sp_aug = np.empty((quantity * n_spectra, sp_len))
+    # as no changes are made to the labels, they are repeated to match the new spectra generated.
+    lab_aug = np.repeat(lab, quantity, axis=0)
 
-    if isinstance(offset_range, list):
-        offset_range_inf = offset_range[0]
-        offset_range_sup = offset_range[1]
-    elif isinstance(offset_range, (float, int)):
-        offset_range_inf = -offset_range
-        offset_range_sup = offset_range
-
-    for i in range(quantity):
-        # random generation of intensity offset(s) using uniform distribution
-        offset = np.random.uniform(offset_range_inf, offset_range_sup, (sp.shape[0], 1))
-        sp_offset = sp + offset*sp_mean
-        # new spectra & labels are appended together
-        sp_aug = np.vstack((sp_aug, sp_offset))
-        lab_aug = np.vstack((lab_aug, lab))
-
-    # first empty sample(first row) is removed from spectra and label
-    sp_aug = np.delete(sp_aug, 0, 0)
-    lab_aug = np.delete(lab_aug, 0, 0)
+    # upper and lower bounds are determined from the given range
+    mult_range_inf, mult_range_sup = _range_converter(mult_range, multiplier_cond=True)
+
+    # random generation of multiplier(s) using uniform distribution
+    multipliers = np.random.uniform(mult_range_inf, mult_range_sup, size=(n_spectra * quantity))
+
+    for i, multiplier in enumerate(multipliers):
+        # generation of new spectra
+        sp_mult = sp[i // quantity] * multiplier
+        # sp_aug is filled progressively
+        sp_aug[i] = sp_mult
 
     if shuffle_enabled:
-        # spectra and labels are randomly mixed(set False for review)
+        # spectra and labels are randomly mixed
         sp_aug, lab_aug = shuffle(sp_aug, lab_aug)
+
     return sp_aug, lab_aug
 
 
-def aug_xshift(sp, lab, xshift_range, quantity=1, fill_mode='edge', fill_value=0, shuffle_enabled=True):
+def aug_offset(sp, lab, offset_range, quantity=1, shuffle_enabled=True):
     """
-    Randomly generates new spectra shifted in wavelength.
+    Randomly generates new spectra shifted in intensity.
+
+    Notes:
+        Updated [2023-05-31]:
+            - Computation time and memory consumption reduced !
 
     Parameters:
         sp : array
             Input Spectrum(s), array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
             for a single spectrum.
 
         lab : array
             Labels assigned the "sp" spectra, array shape = (n_spectra,) for integer labels
             and (n_spectra, n_classes) for binary labels.
 
-        xshift_range : integer, list or tuple
-            Values delimiting the range of possible values for random pixel shift. These values can be
+        offset_range : float or integer, list or tuple
+            Values delimiting the range of possible values for random intensity offset. These values can be
             specified as follows:
-                - xshift_range = (a, b) or [a, b] --> a is the left limit value and b is the right limit value.
-                - xshift_range = a --> -a is the left limit value and +a is the right limit value.
+                - offset_range = (a, b) or [a, b] --> a is the left limit value and b is the right limit value.
+                - offset_range = a --> -a is the left limit value and +a is the right limit value.
 
         quantity : integer, default=1
             Quantity of new spectra generated for one spectrum. If less than or equal to zero, no new
             spectrum is generated.
 
-        fill_mode : {'edge', 'fixed'}, default='edge'
-            Fill mode used for new values created at the extremities of the spectra when they are shifted.
-                - 'edge': Edge values are used to fill new values.
-                - 'fixed': A fixed value(fixed_value) is used to fill new values.
-
-        fill_value : integer or float, default=0
-            Value used when "fill_mode" is 'fixed'.
-
         shuffle_enabled : boolean, default=True
             If True, shuffles the new spectra.
 
     Return:
         (array) New spectra generated.
 
         (array) New labels generated.
     """
     # sp initialization, sp is forced to be a two-dimensional array
     sp = np.array(sp, ndmin=2)
     # lab initialization, lab is forced to be a two-dimensional array
     lab = np.array(lab, ndmin=2)
 
-    # defining a first empty sample for the stacking of the newly generated data
-    sp_aug = np.empty(shape=(1, sp.shape[1]))
-    lab_aug = np.empty(shape=(1, lab.shape[1]))
-    xshift_range_inf = 0
-    xshift_range_sup = 0
-
-    if isinstance(xshift_range, (list, tuple)):  # xshift_range is a list or a tuple
-        xshift_range_inf = xshift_range[0]
-        xshift_range_sup = xshift_range[1]
-    elif isinstance(xshift_range, (float, int)):  # xshift_range is a float or a int value
-        xshift_range_inf = -xshift_range
-        xshift_range_sup = xshift_range
+    n_spectra, sp_len = sp.shape  # number of spectra, spectrum length
 
-    xshift_range = list(range(xshift_range_inf, xshift_range_sup + 1))
+    # array preallocation
+    sp_aug = np.empty((quantity * n_spectra, sp_len))
+    # as no changes are made to the labels, they are repeated to match the new spectra generated.
+    lab_aug = np.repeat(lab, quantity, axis=0)
 
-    # the null shift value is removed
-    if 0 in xshift_range:
-        xshift_range.remove(0)
+    # upper and lower bounds are determined from the given range
+    offset_range_inf, offset_range_sup = _range_converter(offset_range)
+
+    # upper and lower bounds are multiplied by the average intensity of each spectrum
+    offset_range_inf = offset_range_inf * np.mean(sp, axis=1)
+    offset_range_sup = offset_range_sup * np.mean(sp, axis=1)
 
-    for i in range(quantity):
-        # random shift(s) generation using an uniform random distribution
-        wshft = np.random.choice(xshift_range, (sp.shape[0], 1))
-        sp_wshft = _xshift(sp, wshft, fill_mode=fill_mode, fill_value=fill_value)
-        # new spectra & labels are appended together
-        sp_aug = np.vstack((sp_aug, sp_wshft))
-        lab_aug = np.vstack((lab_aug, lab))
-
-    # removal of the first empty sample
-    sp_aug = np.delete(sp_aug, 0, 0)
-    lab_aug = np.delete(lab_aug, 0, 0)
+    # random intensity offset(s) generation using uniform distribution
+    offsets = np.random.uniform(offset_range_inf.repeat(quantity), offset_range_sup.repeat(quantity))
+
+    for i, offset in enumerate(offsets):
+        # generation of new spectra
+        sp_offset = sp[i // quantity] + offset
+        # sp_aug is filled progressively
+        sp_aug[i] = sp_offset
 
     if shuffle_enabled:
-        # spectra and labels are randomly mixed
+        # spectra and labels are randomly mixed(set False for review)
         sp_aug, lab_aug = shuffle(sp_aug, lab_aug)
-
     return sp_aug, lab_aug
 
 
-def _xshift(sp, x_shft, fill_mode, fill_value):
-    """
-    Moves spectrum/spectra along the pixel axis. Uses the same parameters as the aug_xshift function.
-    """
-
-    # initialization and space allocation for shft_sp and fill_value
-    shft_sp = np.zeros_like(sp)
-    fill_value_left = np.zeros_like(x_shft)
-    fill_value_right = np.zeros_like(x_shft)
-    # x_shft index splitting for positive and negative shifts
-    positives = np.argwhere(x_shft > 0)[:, 0]
-    negatives = np.argwhere(x_shft < 0)[:, 0]
-
-    if fill_mode == 'edge':
-        fill_value_left = sp[:, 0]
-        fill_value_right = sp[:, -1]
-    elif fill_mode == 'fixed':
-        fill_value_left[:] = fill_value
-        fill_value_right[:] = fill_value
-    else:
-        print('Invalid fill_mode: fill value(s) has been set to zero')
-
-    for p in positives:
-        shft_sp[p, :int(x_shft[p])] = fill_value_left[p]
-        shft_sp[p, int(x_shft[p]):] = sp[p, :-int(x_shft[p])]
-    for n in negatives:
-        shft_sp[n, int(x_shft[n]):] = fill_value_right[n]
-        shft_sp[n, :int(x_shft[n])] = sp[n, -int(x_shft[n]):]
-    return shft_sp
-
-
 def aug_linslope(sp, lab, slope_range, xinter_range, yinter_range=0, quantity=1, shuffle_enabled=True):
     """
     Randomly generates new spectra with additional linear slopes.
 
+    Notes:
+        Updated [2023-05-31]:
+            - Computation time and memory consumption reduced !
+
     Parameters:
         sp : array
             Input Spectrum(s), array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
             for a single spectrum.
 
         lab : array
             Labels assigned the "sp" spectra, array shape = (n_spectra,) for integer labels
             and (n_spectra, n_classes) for binary labels.
 
-        slope_range : integer, list or tuple
+        slope_range : float or integer, list or tuple
             Values delimiting the range of possible values for random slope. These values can be
             specified as follows:
                 - slope_range = (a, b) or [a, b] --> a is the left limit value and b is the right limit value.
                 - slope_range = a --> -a is the left limit value and +a is the right limit value.
 
-        xinter_range : integer, list or tuple
+        xinter_range : float or integer, list or tuple
             Values delimiting the possible random values for the x-intersept. These values are specified the
-            same way as "slope_range".
+            same way as "slope_range". If = 0, the x-intercept will be at the left end of the spectrum, and
+            if =1 at the right end.
 
-        yinter_range : integer, list or tuple
+        yinter_range : float or integer, list or tuple
             Values delimiting the possible random values for the y-intersept. Same effect as adding an offset
             with the function "aug_ioffset". These values are specified the same way as "slope_range".
 
         quantity : integer, default=1
             Quantity of new spectra generated for one spectrum. If less than or equal to zero, no new
             spectrum is generated.
 
@@ -512,58 +542,128 @@
         (array) New labels generated.
     """
     # sp initialization, sp is forced to be a two-dimensional array
     sp = np.array(sp, ndmin=2)
     # lab initialization, lab is forced to be a two-dimensional array
     lab = np.array(lab, ndmin=2)
 
-    sp_len = sp.shape[1]   # spectrum length
-    lab_len = lab.shape[1]  # label length
-    # defining empty arrays to contain the newly generated data
-    sp_aug = np.empty(shape=(1, sp_len))
-    lab_aug = np.empty(shape=(1, lab_len))
-    pixels = np.arange(0, sp_len)
+    n_spectra, sp_len = sp.shape  # number of spectra, spectrum length
+
+    # array preallocation
+    sp_aug = np.empty((quantity * n_spectra, sp_len))
+    # as no changes are made to the labels, they are repeated to match the new spectra generated.
+    lab_aug = np.repeat(lab, quantity, axis=0)
+
     # average intensity is calculated for each spectra
-    sp_mean = np.mean(sp, axis=1, keepdims=True)
+    sp_mean = np.mean(sp, axis=1)
+
+    # upper and lower bounds are determined from the given range
+    slope_range_inf, slope_range_sup = _range_converter(slope_range)
+    xinter_range_inf, xinter_range_sup = _range_converter(xinter_range)
+    yinter_range_inf, yinter_range_sup = _range_converter(yinter_range)
+
+    # upper and lower bounds are multiplied by the average intensity of each spectrum (slope and y_intercept only)
+    slope_range_inf = slope_range_inf * sp_mean
+    slope_range_sup = slope_range_sup * sp_mean
+    yinter_range_inf = yinter_range_inf * sp_mean
+    yinter_range_sup = yinter_range_sup * sp_mean
+    # upper and lower bounds are multiplied by the spectrum lenght
+    xinter_range_inf = xinter_range_inf * sp_len
+    xinter_range_sup = xinter_range_sup * sp_len
+
+    # random slope(s) and intercept(s) generation using uniform distribution
+    slopes = np.random.uniform(slope_range_inf.repeat(quantity), slope_range_sup.repeat(quantity))
+    xinters = -1 * np.random.uniform(xinter_range_inf, xinter_range_sup, size=(quantity * n_spectra))
+    yinters = np.random.uniform(yinter_range_inf.repeat(quantity), yinter_range_sup.repeat(quantity))
+
+    indexes = np.arange(sp_len)
+    for i, (slope, xinter, yinter) in enumerate(zip(slopes, xinters, yinters)):
+        # generation of new spectra
+        sp_slope = sp[i // quantity] + ((indexes + xinter) * slope / sp_len + yinter)
+        # sp_aug is filled progressively
+        sp_aug[i] = sp_slope
+
+    if shuffle_enabled:
+        # spectra and labels are randomly mixed
+        sp_aug, lab_aug = shuffle(sp_aug, lab_aug)
+
+    return sp_aug, lab_aug
+
+
+def aug_xshift(sp, lab, xshift_range, quantity=1, fill_mode='edge', fill_value=0, shuffle_enabled=True):
+    """
+    Randomly generates new spectra shifted in wavelength.
+
+    Notes:
+        Updated [2023-05-31]:
+            - Computation time and memory consumption reduced !
+
+    Parameters:
+        sp : array
+            Input Spectrum(s), array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
+            for a single spectrum.
+
+        lab : array
+            Labels assigned the "sp" spectra, array shape = (n_spectra,) for integer labels
+            and (n_spectra, n_classes) for binary labels.
+
+        xshift_range : float or integer, list or tuple
+            Values delimiting the range of possible values for random pixel shift. These values can be
+            specified as follows:
+                - xshift_range = (a, b) or [a, b] --> a is the left limit value and b is the right limit value.
+                - xshift_range = a --> -a is the left limit value and +a is the right limit value.
+
+        quantity : integer, default=1
+            Quantity of new spectra generated for one spectrum. If less than or equal to zero, no new
+            spectrum is generated.
+
+        fill_mode : {'edge', 'fixed'}, default='edge'
+            Fill mode used for new values created at the extremities of the spectra when they are shifted.
+                - 'edge': Edge values are used to fill new values.
+                - 'fixed': A fixed value(fixed_value) is used to fill new values.
+
+        fill_value : integer or float, default=0
+            Value used when "fill_mode" is 'fixed'.
+
+        shuffle_enabled : boolean, default=True
+            If True, shuffles the new spectra.
+
+    Return:
+        (array) New spectra generated.
+
+        (array) New labels generated.
+    """
+    # sp initialization, sp is forced to be a two-dimensional array
+    sp = np.array(sp, ndmin=2)
+    # lab initialization, lab is forced to be a two-dimensional array
+    lab = np.array(lab, ndmin=2)
+
+    n_spectra, sp_len = sp.shape  # number of spectra, spectrum length
+
+    # array preallocation
+    sp_aug = np.empty((quantity * n_spectra, sp_len))
+    # as no changes are made to the labels, they are repeated to match the new spectra generated.
+    lab_aug = np.repeat(lab, quantity, axis=0)
+
+    # upper and lower bounds are determined from the given range
+    xshift_range_inf, xshift_range_sup = _range_converter(xshift_range)
+
+    # the null shift value is removed
+    xshift_range_cor = list(range(xshift_range_inf, xshift_range_sup + 1))
+    if 0 in xshift_range_cor:
+        xshift_range_cor.remove(0)
+
+    # random shift(s) generation using an uniform random distribution
+    xshifts = np.random.choice(xshift_range_cor, size=(quantity * n_spectra, 1), replace=True)
 
-    if isinstance(slope_range, list):
-        slope_range_inf = slope_range[0]
-        slope_range_sup = slope_range[1]
-    elif isinstance(slope_range, (float, int)):
-        slope_range_inf = -slope_range
-        slope_range_sup = slope_range
-
-    if isinstance(xinter_range, list):
-        xinter_range_inf = xinter_range[0]
-        xinter_range_sup = xinter_range[1]
-    elif isinstance(xinter_range, (float, int)):
-        xinter_range_inf = -xinter_range
-        xinter_range_sup = xinter_range
-
-    if isinstance(yinter_range, list):
-        yinter_range_inf = yinter_range[0]
-        yinter_range_sup = yinter_range[1]
-    elif isinstance(yinter_range, (float, int)):
-        yinter_range_inf = -yinter_range
-        yinter_range_sup = +yinter_range
-
-    for i in range(quantity):
-        # random slope and intercept(s) generation using uniform distribution
-        slope = np.random.uniform(slope_range_inf, slope_range_sup, (sp.shape[0], 1)) * sp_mean
-        xinter = -np.random.uniform(xinter_range_inf, xinter_range_sup, (sp.shape[0], 1)) * sp_len
-        yinter = np.random.uniform(yinter_range_inf, yinter_range_sup, (sp.shape[0], 1)) * sp_mean
+    for i, xshift in enumerate(xshifts):
         # generation of new spectra
-        sp_slope = sp + ((pixels+xinter)*slope/sp_len + yinter)
-        # new spectra & labels are appended together
-        sp_aug = np.vstack((sp_aug, sp_slope))
-        lab_aug = np.vstack((lab_aug, lab))
-
-    # removal of the first empty sample
-    sp_aug = np.delete(sp_aug, 0, 0)
-    lab_aug = np.delete(lab_aug, 0, 0)
+        sp_xshift = _xshift(sp[i//quantity], xshift, fill_mode=fill_mode, fill_value=fill_value)
+        # sp_aug is filled progressively
+        sp_aug[i] = sp_xshift
 
     if shuffle_enabled:
         # spectra and labels are randomly mixed
         sp_aug, lab_aug = shuffle(sp_aug, lab_aug)
 
     return sp_aug, lab_aug
```

### Comparing `boxsers-1.2.0/boxsers/machine_learning/classification.py` & `boxsers-1.3.0/boxsers/machine_learning/classification.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/boxsers/machine_learning/clustering.py` & `boxsers-1.3.0/boxsers/machine_learning/clustering.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/boxsers/machine_learning/dimension_reduction.py` & `boxsers-1.3.0/boxsers/machine_learning/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/boxsers/machine_learning/neural_networks.py` & `boxsers-1.3.0/boxsers/machine_learning/neural_networks.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/boxsers/machine_learning/validation_metrics.py` & `boxsers-1.3.0/boxsers/machine_learning/validation_metrics.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/boxsers/misc_tools.py` & `boxsers-1.3.0/boxsers/misc_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,29 +72,62 @@
         print("Subset A distribution  : ", distribution_a)
         print("\nSubset B shape :", sp_b.shape)
         print("Subset B distribution  : ", distribution_b, '\n')
 
     return sp_a, sp_b, lab_a, lab_b
 
 
+def spectro_subsampling(sp, lab=None, batch_size=0.5):
+    """
+    Subsamples a given fraction or number of spectra from an initial spectra array.
+
+    Parameters:
+        sp : array
+            Input spectra, array shape = (n_spectra, n_pixels)
+
+        lab : array, default=None
+            Labels assigned the "sp" spectra, array shape = (n_spectra,) for integer labels
+            and (n_spectra, n_classes) for binary labels.
+
+        batch_size : float or integer positive value, default=0.5
+             Fraction or number of spectra to sample from the initial spectra array.
+
+    Returns:
+        (array) Sampled subset of spectra.
+
+        (array) Sampled subset of labels.
+    """
+    if 0 < batch_size < 1:
+        batch_size = int(batch_size * sp.shape[0])
+    else:
+        batch_size = batch_size
+
+    random_row = np.random.choice(sp.shape[0], size=batch_size, replace=False)
+    sp_sample = sp[random_row, :]
+    if lab is not None:
+        lab_sample = lab[random_row, :]
+        return sp_sample, lab_sample
+    return sp_sample
+
+
 def load_rruff(directory):
     """
     Export a subset of Raman spectra from the RRUFF database in the form of three related lists
     containing Raman shifts, intensities and mineral names.
 
     Parameters:
         directory : String
             Online directory that leads to a zip file containing the desired set of RRUFF spectra. Here are
             the possible directories for RRUFF Raman spectra:
-                - 'http://rruff.info/zipped_data_files/raman/excellent_oriented.zip'
-                - 'http://rruff.info/zipped_data_files/raman/excellent_unoriented.zip'
-                - 'http://rruff.info/zipped_data_files/raman/fair_oriented.zip'
-                - 'http://rruff.info/zipped_data_files/raman/fair_unoriented.zip'
-                - 'http://rruff.info/zipped_data_files/raman/poor_oriented.zip'
-                - 'http://rruff.info/zipped_data_files/raman/poor_unoriented.zip'
+                - 'https://rruff.info/zipped_data_files/raman/excellent_oriented.zip'
+                - 'https://rruff.info/zipped_data_files/raman/excellent_unoriented.zip'
+                - 'https://rruff.info/zipped_data_files/raman/fair_oriented.zip'
+                - 'https://rruff.info/zipped_data_files/raman/fair_unoriented.zip'
+                - 'https://rruff.info/zipped_data_files/raman/poor_oriented.zip'
+                - 'https://rruff.info/zipped_data_files/raman/poor_unoriented.zip'
 
     Return:
         (List of numpy array) List that contains Raman shift arrays.
 
         (List of numpy array) List that contains intensity arrays.
 
         (List of string) List that contains RRUFF labels (mineral names).
```

### Comparing `boxsers-1.2.0/boxsers/preprocessing.py` & `boxsers-1.3.0/boxsers/preprocessing.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This module provides functions to preprocess vibrational spectra. These features
 improve spectrum quality and can improve performance for machine learning applications
 """
 import numpy as np
 from scipy import interpolate, sparse
 from scipy.sparse.linalg import spsolve
 from scipy.signal import savgol_filter, medfilt
+from scipy.spatial import ConvexHull
 from sklearn.preprocessing import normalize
 
 
 def als_baseline_cor(sp, lam=1e4, p=0.001, niter=10, return_baseline=False):
     """
     Subtracts the baseline signal from the spectrum(s) using Asymmetric Least Squares estimation.
     (Updated April 2020: improved computing speed)
@@ -57,18 +58,64 @@
             w_matrix.setdiag(w)
             z = w_matrix + diag
             baseline[n] = spsolve(z, w * sp[n])
             w = p * (sp[n] > baseline[n]) + (1 - p) * (sp[n] < baseline[n])  # w is updated according to baseline
 
     if return_baseline:
         return sp-baseline, baseline
-
     return sp-baseline
 
 
+def rubberband_baseline_cor(sp, return_baseline=False):
+    """
+    Notes:
+        - code mainly coming from:
+        https://dsp.stackexchange.com/questions/2725/how-to-perform-a-rubberband-correction-on-spectroscopic-data
+        - Compared with the als_baseline_cor method, this technique is faster
+          to run, but has no parameters to adjust to optimize the correction.
+
+    Parameters:
+        sp : array
+            Input Spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
+            for a single spectrum.
+
+        return_baseline : Boolean, default=False
+            If True, the function also returns the baseline array.
+
+    Returns:
+        (array) Baseline substracted spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra
+                and = (n_pixels,) for a single spectrum.
+
+        (array)(OPTIONAL) Baseline signal(s). Array shape = (n_spectra, n_pixels) for multiple spectra
+                and = (n_pixels,) for a single spectrum.
+    """
+    # sp is forced to be a two-dimensional array
+    sp = np.array(sp, ndmin=2)
+    n_spectra, sp_length = sp.shape  # number of spectra, spectrum length
+
+    # initialization and space allocation
+    baseline = np.zeros(sp.shape)  # baseline signal array
+    indexes = np.arange(sp_length)
+
+    for i in range(n_spectra):
+        # find the convex hull vertices
+        convex_v = ConvexHull(np.array(list(zip(indexes, sp[i])))).vertices
+        # rotate convex hull vertices until they start from the lowest one
+        convex_v = np.roll(convex_v, -convex_v.argmin())
+        # leave only the ascending part
+        convex_v = convex_v[:convex_v.argmax()]
+
+        # create baseline using linear interpolation between vertices
+        baseline[i] = np.interp(indexes, indexes[convex_v], sp[i, convex_v])
+
+    if return_baseline:
+        return sp - baseline, baseline
+    return sp - baseline
+
+
 def cosmic_filter(sp, ks=3):
     """
     Apply a median filter to the spectrum(s) to remove cosmic rays.
 
     Parameters:
         sp : array
             Input Spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
```

### Comparing `boxsers-1.2.0/boxsers/visual_tools.py` & `boxsers-1.3.0/boxsers/visual_tools.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/boxsers.egg-info/PKG-INFO` & `boxsers-1.3.0/boxsers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsers
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package that provides a full range of functionality to process and analyze vibrational spectra (Raman, SERS, FTIR, etc.).
 Home-page: https://github.com/ALebrun-108/BoxSERS
 Author: Alexis Lebrun
 Author-email: alexis.lebrun.1@ulaval.ca
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boxsers-1.2.0/boxsers.egg-info/SOURCES.txt` & `boxsers-1.3.0/boxsers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boxsers-1.2.0/setup.py` & `boxsers-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     author='Alexis Lebrun',
     author_email='alexis.lebrun.1@ulaval.ca',
     # dependencies
     install_requires=['numpy', 'pandas', 'matplotlib', 'seaborn', 'scipy', 'scikit-learn', 'tensorflow',
                       'tables'],
     python_requires='>=3.6',
     # *strongly* suggested for sharing
-    version='1.2.0',
+    version='1.3.0',
     # The license can be anything you like
     license='MIT',
     description='Python package that provides a full range of functionality to process and analyze vibrational'
                 ' spectra (Raman, SERS, FTIR, etc.).',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README_pypi.md').read(),
     long_description_content_type="text/markdown",
```

