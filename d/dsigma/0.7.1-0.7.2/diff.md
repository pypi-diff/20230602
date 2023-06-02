# Comparing `tmp/dsigma-0.7.1.tar.gz` & `tmp/dsigma-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsigma-0.7.1.tar", last modified: Wed Jan 18 14:05:07 2023, max compression
+gzip compressed data, was "dsigma-0.7.2.tar", last modified: Fri Jun  2 19:17:12 2023, max compression
```

## Comparing `dsigma-0.7.1.tar` & `dsigma-0.7.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-01-18 14:05:07.994606 dsigma-0.7.1/
--rw-r--r--   0 research  (1001) research  (1001)     1683 2023-01-18 13:59:53.000000 dsigma-0.7.1/CHANGELOG.md
--rw-r--r--   0 research  (1001) research  (1001)     1107 2022-10-07 17:36:19.000000 dsigma-0.7.1/LICENSE
--rw-r--r--   0 research  (1001) research  (1001)      115 2023-01-06 05:11:30.000000 dsigma-0.7.1/MANIFEST.in
--rw-r--r--   0 research  (1001) research  (1001)     3880 2023-01-18 14:05:07.994606 dsigma-0.7.1/PKG-INFO
--rw-r--r--   0 research  (1001) research  (1001)     2251 2023-01-06 05:11:30.000000 dsigma-0.7.1/README.md
-drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-01-18 14:05:07.993606 dsigma-0.7.1/dsigma/
--rw-r--r--   0 research  (1001) research  (1001)      366 2023-01-18 14:00:39.000000 dsigma-0.7.1/dsigma/__init__.py
--rw-r--r--   0 research  (1001) research  (1001)     7528 2022-10-07 18:40:55.000000 dsigma-0.7.1/dsigma/helpers.py
--rw-r--r--   0 research  (1001) research  (1001)     8724 2023-01-18 13:56:55.000000 dsigma-0.7.1/dsigma/jackknife.py
--rw-r--r--   0 research  (1001) research  (1001)    10075 2022-10-07 18:40:55.000000 dsigma-0.7.1/dsigma/physics.py
--rw-r--r--   0 research  (1001) research  (1001)    19625 2023-01-18 13:37:15.000000 dsigma-0.7.1/dsigma/precompute.py
--rw-r--r--   0 research  (1001) research  (1001)   967825 2023-01-18 14:05:07.000000 dsigma-0.7.1/dsigma/precompute_engine.c
--rw-r--r--   0 research  (1001) research  (1001)    10368 2023-01-06 05:11:30.000000 dsigma-0.7.1/dsigma/precompute_engine.pyx
--rw-r--r--   0 research  (1001) research  (1001)    18256 2023-01-06 05:11:30.000000 dsigma-0.7.1/dsigma/stacking.py
-drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-01-18 14:05:07.994606 dsigma-0.7.1/dsigma/surveys/
--rw-r--r--   0 research  (1001) research  (1001)       81 2022-10-07 17:36:19.000000 dsigma-0.7.1/dsigma/surveys/__init__.py
--rw-r--r--   0 research  (1001) research  (1001)      715 2022-10-07 18:40:55.000000 dsigma-0.7.1/dsigma/surveys/cfhtls.py
--rw-r--r--   0 research  (1001) research  (1001)     6238 2022-10-07 18:40:55.000000 dsigma-0.7.1/dsigma/surveys/des.py
--rw-r--r--   0 research  (1001) research  (1001)     4601 2022-10-07 18:40:55.000000 dsigma-0.7.1/dsigma/surveys/hsc.py
--rw-r--r--   0 research  (1001) research  (1001)     3745 2022-10-07 18:40:55.000000 dsigma-0.7.1/dsigma/surveys/kids.py
-drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-01-18 14:05:07.994606 dsigma-0.7.1/dsigma.egg-info/
--rw-r--r--   0 research  (1001) research  (1001)     3880 2023-01-18 14:05:07.000000 dsigma-0.7.1/dsigma.egg-info/PKG-INFO
--rw-r--r--   0 research  (1001) research  (1001)      505 2023-01-18 14:05:07.000000 dsigma-0.7.1/dsigma.egg-info/SOURCES.txt
--rw-r--r--   0 research  (1001) research  (1001)        1 2023-01-18 14:05:07.000000 dsigma-0.7.1/dsigma.egg-info/dependency_links.txt
--rw-r--r--   0 research  (1001) research  (1001)       54 2023-01-18 14:05:07.000000 dsigma-0.7.1/dsigma.egg-info/requires.txt
--rw-r--r--   0 research  (1001) research  (1001)        7 2023-01-18 14:05:07.000000 dsigma-0.7.1/dsigma.egg-info/top_level.txt
--rw-r--r--   0 research  (1001) research  (1001)      643 2023-01-18 13:30:05.000000 dsigma-0.7.1/pyproject.toml
--rw-r--r--   0 research  (1001) research  (1001)       38 2023-01-18 14:05:07.994606 dsigma-0.7.1/setup.cfg
--rw-r--r--   0 research  (1001) research  (1001)      248 2023-01-06 05:11:30.000000 dsigma-0.7.1/setup.py
+drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-06-02 19:17:12.957168 dsigma-0.7.2/
+-rw-r--r--   0 research  (1001) research  (1001)     2232 2023-06-02 18:56:14.000000 dsigma-0.7.2/CHANGELOG.md
+-rw-r--r--   0 research  (1001) research  (1001)     1107 2023-04-26 17:55:50.000000 dsigma-0.7.2/LICENSE
+-rw-r--r--   0 research  (1001) research  (1001)      115 2023-04-26 17:55:50.000000 dsigma-0.7.2/MANIFEST.in
+-rw-r--r--   0 research  (1001) research  (1001)     3880 2023-06-02 19:17:12.957168 dsigma-0.7.2/PKG-INFO
+-rw-r--r--   0 research  (1001) research  (1001)     2251 2023-04-26 17:55:50.000000 dsigma-0.7.2/README.md
+drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-06-02 19:17:12.955168 dsigma-0.7.2/dsigma/
+-rw-r--r--   0 research  (1001) research  (1001)      366 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/__init__.py
+-rw-r--r--   0 research  (1001) research  (1001)     7528 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/helpers.py
+-rw-r--r--   0 research  (1001) research  (1001)     8721 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/jackknife.py
+-rw-r--r--   0 research  (1001) research  (1001)    10075 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/physics.py
+-rw-r--r--   0 research  (1001) research  (1001)    20046 2023-04-28 20:13:07.000000 dsigma-0.7.2/dsigma/precompute.py
+-rw-r--r--   0 research  (1001) research  (1001)   968246 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma/precompute_engine.c
+-rw-r--r--   0 research  (1001) research  (1001)    10368 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/precompute_engine.pyx
+-rw-r--r--   0 research  (1001) research  (1001)    18468 2023-04-28 20:18:19.000000 dsigma-0.7.2/dsigma/stacking.py
+drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-06-02 19:17:12.956168 dsigma-0.7.2/dsigma/surveys/
+-rw-r--r--   0 research  (1001) research  (1001)       81 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/surveys/__init__.py
+-rw-r--r--   0 research  (1001) research  (1001)      715 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/surveys/cfhtls.py
+-rw-r--r--   0 research  (1001) research  (1001)     6238 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/surveys/des.py
+-rw-r--r--   0 research  (1001) research  (1001)     4601 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/surveys/hsc.py
+-rw-r--r--   0 research  (1001) research  (1001)     3783 2023-06-02 19:03:36.000000 dsigma-0.7.2/dsigma/surveys/kids.py
+drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-06-02 19:17:12.956168 dsigma-0.7.2/dsigma.egg-info/
+-rw-r--r--   0 research  (1001) research  (1001)     3880 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/PKG-INFO
+-rw-r--r--   0 research  (1001) research  (1001)      505 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/SOURCES.txt
+-rw-r--r--   0 research  (1001) research  (1001)        1 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/dependency_links.txt
+-rw-r--r--   0 research  (1001) research  (1001)       54 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/requires.txt
+-rw-r--r--   0 research  (1001) research  (1001)        7 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/top_level.txt
+-rw-r--r--   0 research  (1001) research  (1001)      643 2023-06-02 19:01:10.000000 dsigma-0.7.2/pyproject.toml
+-rw-r--r--   0 research  (1001) research  (1001)       38 2023-06-02 19:17:12.957168 dsigma-0.7.2/setup.cfg
+-rw-r--r--   0 research  (1001) research  (1001)      248 2023-04-26 17:55:50.000000 dsigma-0.7.2/setup.py
```

### Comparing `dsigma-0.7.1/CHANGELOG.md` & `dsigma-0.7.2/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,36 @@
 Notable changes to dsigma will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.7.2] - 2023-06-02
+
+### Changed
+
+- `dsigma.stacking.lens_magnification_bias` can now be used to compute the bias in the tangential shear
+- mean source redshift now takes into account n(z)'s passed to `dsigma.precompute.precompute`
+
+### Fixed
+
+- incompatibility with numpy 1.24
+- bug in `dsigma.stacking.tangential_shear` when `random_subtraction=True`
+- error in tomographic redshift bin assignment for KiDS, sources with photo-z's at the bin edges were assigned to the wrong tomographic bin, this biased KiDS lensing measurements by order 2%
+
 ## [0.7.1] - 2023-01-18
 
 ### Changed
 
-- `dsigma.jackknife.compress_jackknife_fields` now supresses `numpy` warnings if columns contain NaNs
+- `dsigma.jackknife.compress_jackknife_fields` now suppresses `numpy` warnings if columns contain NaNs
 
 ### Fixed
 
-- bug in the calcaluation of the photo-z dilution correction factor, led to percent-level biases in the total galaxy-galaxy lensing amplitude, did not affect DES and KiDS calculations since those are based on n(z)'s, bug was introduced in version 0.6
+- bug in the calculation of the photo-z dilution correction factor, led to percent-level biases in the total galaxy-galaxy lensing amplitude, did not affect DES and KiDS calculations since those are based on n(z)'s, bug was introduced in version 0.6
 
 ## [0.7.0] - 2023-01-06
 
 ### Changed
 
 - `dsigma.precompute.add_precompute_results` has been renamed to `dsigma.precompute.precompute`
 - `dsigma.precompute.add_maximum_lens_redshift` has been removed and the functionality integrated into `dsigma.precompute.precompute` using the `lens_source_cut` argument
```

### Comparing `dsigma-0.7.1/LICENSE` & `dsigma-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.1/PKG-INFO` & `dsigma-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsigma
-Version: 0.7.1
+Version: 0.7.2
 Author: Song Huang
 Author-email: "Johannes U. Lange" <julange.astro@pm.me>
 License: The MIT License (MIT)
         
         Copyright (c) 2017 - Present: Johannes Lange and Song Huang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dsigma-0.7.1/README.md` & `dsigma-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.1/dsigma/helpers.py` & `dsigma-0.7.2/dsigma/helpers.py`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.1/dsigma/jackknife.py` & `dsigma-0.7.2/dsigma/jackknife.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             "The number of jackknife regions cannot be smaller than the " +
             "number of continous fields. Try increasing `distance_threshold`" +
             " or decreasing `centers`.")
 
     # Assign the number of jackknife fields according to the total number of
     # objects in each field.
     n_jk_per_c = np.diff(np.rint(
-        np.cumsum(w_c) / np.sum(w_c) * n_jk).astype(np.int), prepend=0)
+        np.cumsum(w_c) / np.sum(w_c) * n_jk).astype(int), prepend=0)
 
     # It can happen that one field is assigned 0 jackknife fields. In this
     # case, we will assign 1.
     while np.any(w_c[n_jk_per_c == 0] > 0):
         n_jk_per_c[np.argmin(n_jk_per_c)] += 1
         n_jk_per_c[np.argmax(n_jk_per_c)] -= 1
```

### Comparing `dsigma-0.7.1/dsigma/physics.py` & `dsigma-0.7.2/dsigma/physics.py`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.1/dsigma/precompute.py` & `dsigma-0.7.2/dsigma/precompute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Module for pre-computing lensing results."""
 
-import numbers
-import warnings
 import multiprocessing as mp
+import numbers
+import numpy as np
 import queue as Queue
+import warnings
 
-import numpy as np
-from astropy_healpix import HEALPix
-from scipy.interpolate import interp1d
 
-from astropy.cosmology import FlatLambdaCDM
 from astropy import units as u
+from astropy.cosmology import FlatLambdaCDM
 from astropy.units import UnitConversionError
+from astropy_healpix import HEALPix
+from scipy.interpolate import interp1d
 
 from .physics import critical_surface_density
 from .physics import effective_critical_surface_density
 from .precompute_engine import precompute_engine
 
 
 __all__ = ["photo_z_dilution_factor", "mean_photo_z_offset", "precompute"]
@@ -343,14 +343,15 @@
             fill_value=(dz_s_interp[0], dz_s_interp[-1]))
         table_engine_l['delta z_s'] = np.ascontiguousarray(
             dz_s_interp(np.array(table_engine_l['z'])), dtype=np.float64)
 
     elif table_c is None and table_n is not None:
         n_bins = table_n['n'].data.shape[1]
         sigma_crit_eff = np.zeros(len(table_l) * n_bins, dtype=np.float64)
+        z_mean = np.zeros(n_bins, dtype=np.float64)
         for i in range(n_bins):
             z_min = np.amin(table_l['z'])
             z_max = min(np.amax(table_l['z']),
                         np.amax(table_n['z'][table_n['n'][:, i] > 0]))
             z_interp = np.linspace(
                 z_min, z_max, max(10, int((z_max - z_min) / 0.001)))
 
@@ -364,18 +365,25 @@
                             sigma_crit_eff_inv_interp[-1]))
             sigma_crit_eff_inv_interp = sigma_crit_eff_inv_interp(
                 np.array(table_engine_l['z']))
             sigma_crit_eff_interp = np.repeat(np.inf, len(table_l))
             mask = sigma_crit_eff_inv_interp == 0
             sigma_crit_eff_interp[~mask] = sigma_crit_eff_inv_interp[~mask]**-1
             sigma_crit_eff[i::n_bins] = sigma_crit_eff_interp
+            z_mean[i] = np.average(table_n['z'], weights=table_n['n'][:, i])
         table_engine_l['sigma_crit_eff'] = np.ascontiguousarray(
             sigma_crit_eff, dtype=np.float64)
         table_engine_s['z_bin'] = np.ascontiguousarray(
             table_s['z_bin'][argsort_pix_s], dtype=int)
+        # Overwrite the photometric redshifts in the source table. These
+        # redshifts will be used to compute the mean source redshifts for each
+        # lens.
+        table_engine_s['z'] = np.ascontiguousarray(
+            z_mean[table_s['z_bin']][argsort_pix_s], dtype=np.float64)
+
     elif table_c is not None and table_s is not None:
         raise ValueError('table_c and table_n cannot both be given.')
 
     # Create arrays that will hold the final results.
     table_engine_r = {}
     n_results = len(table_l) * (len(bins) - 1)
```

### Comparing `dsigma-0.7.1/dsigma/precompute_engine.c` & `dsigma-0.7.2/dsigma/precompute_engine.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-O3",
@@ -22,16 +22,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -91,16 +91,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -216,15 +220,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -255,15 +259,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -19115,15 +19119,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -19237,15 +19241,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -19501,15 +19505,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -19650,15 +19654,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -22351,28 +22355,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -24417,15 +24421,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24651,15 +24655,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24885,15 +24889,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `dsigma-0.7.1/dsigma/precompute_engine.pyx` & `dsigma-0.7.2/dsigma/precompute_engine.pyx`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.1/dsigma/stacking.py` & `dsigma-0.7.2/dsigma/stacking.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Module for stacking lensing results after pre-computation."""
 
 import numpy as np
+from astropy import units as u
 from astropy.table import Table
 from astropy.cosmology import FlatLambdaCDM
+from astropy.units import UnitConversionError
 from . import surveys
 from .physics import mpc_per_degree, lens_magnification_shear_bias
 from .physics import critical_surface_density
 
 __all__ = ['number_of_pairs', 'raw_tangential_shear',
            'raw_excess_surface_density', 'photo_z_dilution_factor',
            'boost_factor', 'scalar_shear_response_factor',
@@ -232,28 +234,32 @@
 
     return (
         np.sum(table_l[key_num] * table_l['w_sys'][:, None], axis=0) /
         np.sum(table_l['sum w_ls'] * table_l['w_sys'][:, None], axis=0))
 
 
 def lens_magnification_bias(table_l, alpha_l, camb_results,
-                            photo_z_correction=True):
+                            photo_z_correction=True, shear=False):
     """Estimate the additive lens magnification bias.
 
     Parameters
     ----------
     table_l : astropy.table.Table
         Precompute results for the lenses.
     alpha_l : float
-        TBD
+        The response of the lenses to magnification.
     camb_results : camb.results.CAMBdata
         CAMB results object that contains information on cosmology and the
         matter power spectrum.
     photo_z_correction : boolean, optional
-        Whether to correct for photo-z dilution and offsets.
+        Whether to correct for photo-z dilution and offsets. Default is True.
+    shear : boolean, optional
+        If True, return bias of the mean tangential shear. Otherwise, return
+        an estimate for the bias of the excess surface density. Default is
+        False.
 
     Returns
     -------
     ds_lm : numpy.ndarray
         The lens magnification bias in each radial bin.
 
     """
@@ -272,33 +278,30 @@
                 z_l, z_s_true, cosmology, comoving=table_l.meta['comoving'])
     else:
         sigma_crit = critical_surface_density(
             z_l, z_s, cosmology, comoving=table_l.meta['comoving'])
         z_s_true = z_s
 
     bins = table_l.meta['bins']
+    d = 2.0 / 3.0 * np.diff(bins**3) / np.diff(bins**2)
 
-    shear_mode = ('shear_mode' in table_l.meta.keys() and
-                  table_l.meta['shear_mode'])
-
-    if shear_mode:
-        theta = 2.0 / 3.0 * np.diff(bins**3) / np.diff(bins**2)
-    else:
-        rp = 2.0 / 3.0 * np.diff(bins**3) / np.diff(bins**2)
-        theta = np.deg2rad(rp / mpc_per_degree(
+    try:
+        theta = d.to(u.rad).value
+    except UnitConversionError:
+        theta = np.deg2rad(d.to(u.Mpc).value / mpc_per_degree(
             z_l, cosmology=cosmology, comoving=table_l.meta['comoving']))
 
-    gamma = np.array([lens_magnification_shear_bias(
+    gt = np.array([lens_magnification_shear_bias(
         theta[i], alpha_l, z_l[i], z_s_true[i], camb_results) for i in
         range(len(theta))])
 
-    if shear_mode:
-        return gamma
+    if shear:
+        return gt
     else:
-        return gamma * sigma_crit
+        return gt * sigma_crit
 
 
 def tangential_shear(table_l, table_r=None, boost_correction=False,
                      scalar_shear_response_correction=False,
                      matrix_shear_response_correction=False,
                      shear_responsivity_correction=False,
                      hsc_selection_bias_correction=False,
@@ -383,15 +386,15 @@
             table_l)
         result['et'] *= result['1+m_sel']
 
     if random_subtraction:
         if table_r is None:
             raise ValueError('Cannot subtract random results without ' +
                              'results from a random catalog.')
-        result['et_r'] = excess_surface_density(
+        result['et_r'] = tangential_shear(
             table_r, boost_correction=False,
             scalar_shear_response_correction=scalar_shear_response_correction,
             matrix_shear_response_correction=matrix_shear_response_correction,
             shear_responsivity_correction=shear_responsivity_correction,
             hsc_selection_bias_correction=hsc_selection_bias_correction,
             random_subtraction=False, return_table=False)
         result['et'] -= result['et_r']
```

### Comparing `dsigma-0.7.1/dsigma/surveys/cfhtls.py` & `dsigma-0.7.2/dsigma/surveys/cfhtls.py`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.1/dsigma/surveys/des.py` & `dsigma-0.7.2/dsigma/surveys/des.py`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.1/dsigma/surveys/hsc.py` & `dsigma-0.7.2/dsigma/surveys/hsc.py`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.1/dsigma/surveys/kids.py` & `dsigma-0.7.2/dsigma/surveys/kids.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,16 @@
     Returns
     -------
     z_bin : numpy.ndarray
         The tomographic redshift bin corresponding to each photometric
         redshift. Returns -1 in case a redshift does not fall into any bin.
 
     """
-    z_bin = np.digitize(z_s, [0.1, 0.3, 0.5, 0.7, 0.9, 1.2]) - 1
+    z_bin = np.digitize(z_s, np.array(
+        [0.1, 0.3, 0.5, 0.7, 0.9, 1.2]) + 1e-6, right=True) - 1
     z_bin = np.where((z_s < 0.1) | (z_s >= 1.2), -1, z_bin)
 
     return z_bin
 
 
 def multiplicative_shear_bias(z_bin, version=default_version):
     """Return the multiplicative shear bias.
```

### Comparing `dsigma-0.7.1/dsigma.egg-info/PKG-INFO` & `dsigma-0.7.2/dsigma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsigma
-Version: 0.7.1
+Version: 0.7.2
 Author: Song Huang
 Author-email: "Johannes U. Lange" <julange.astro@pm.me>
 License: The MIT License (MIT)
         
         Copyright (c) 2017 - Present: Johannes Lange and Song Huang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dsigma-0.7.1/pyproject.toml` & `dsigma-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dsigma"
-version = "0.7.1"
+version = "0.7.2"
 requires-python = ">=3.8"
 authors = [{name = "Johannes U. Lange", email = "julange.astro@pm.me"},
            {name = "Song Huang"}]
 readme = "README.md"
 keywords = ["astronomy", "weak-lensing"]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
```

