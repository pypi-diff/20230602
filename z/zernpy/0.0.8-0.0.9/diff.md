# Comparing `tmp/zernpy-0.0.8.tar.gz` & `tmp/zernpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zernpy-0.0.8.tar", last modified: Tue Feb 28 16:00:52 2023, max compression
+gzip compressed data, was "zernpy-0.0.9.tar", last modified: Thu Mar  2 11:17:41 2023, max compression
```

## Comparing `zernpy-0.0.8.tar` & `zernpy-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.146130 zernpy-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-02-02 11:40:00.000000 zernpy-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       40 2023-02-02 12:31:23.000000 zernpy-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7593 2023-02-28 16:00:52.145133 zernpy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6826 2023-02-28 15:30:01.000000 zernpy-0.0.8/README.md
--rw-rw-rw-   0        0        0     1442 2023-02-28 14:54:59.000000 zernpy-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-28 16:00:52.146130 zernpy-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.045071 zernpy-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.072148 zernpy-0.0.8/src/zernpy/
--rw-rw-rw-   0        0        0      962 2023-02-02 14:34:04.000000 zernpy-0.0.8/src/zernpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.108054 zernpy-0.0.8/src/zernpy/calculations/
--rw-rw-rw-   0        0        0       72 2023-02-28 13:25:13.000000 zernpy-0.0.8/src/zernpy/calculations/__init__.py
--rw-rw-rw-   0        0        0    33600 2023-02-28 15:45:39.000000 zernpy-0.0.8/src/zernpy/calculations/calc_zernike_pol.py
--rw-rw-rw-   0        0        0    23546 2023-02-28 14:47:06.000000 zernpy-0.0.8/src/zernpy/calculations/find_pols_coeffs.py
--rw-rw-rw-   0        0        0    13057 2023-02-02 10:08:32.000000 zernpy-0.0.8/src/zernpy/calculations/fit_zernike_pols.py
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.119025 zernpy-0.0.8/src/zernpy/plotting/
--rw-rw-rw-   0        0        0       26 2022-12-05 11:57:03.000000 zernpy-0.0.8/src/zernpy/plotting/__init__.py
--rw-rw-rw-   0        0        0     3840 2023-01-31 13:29:52.000000 zernpy-0.0.8/src/zernpy/plotting/plot_zerns.py
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.122018 zernpy-0.0.8/src/zernpy/props/
--rw-rw-rw-   0        0        0       26 2023-02-24 13:23:33.000000 zernpy-0.0.8/src/zernpy/props/__init__.py
--rw-rw-rw-   0        0        0     2809 2023-02-24 14:03:28.000000 zernpy-0.0.8/src/zernpy/props/properties.py
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.124012 zernpy-0.0.8/src/zernpy/readme_images/
--rw-rw-rw-   0        0        0    59513 2023-02-02 11:26:55.000000 zernpy-0.0.8/src/zernpy/readme_images/Fitted_Profile.png
--rw-rw-rw-   0        0        0    60427 2023-02-02 11:26:36.000000 zernpy-0.0.8/src/zernpy/readme_images/Random_Profile.png
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.137977 zernpy-0.0.8/src/zernpy/tests/
--rw-rw-rw-   0        0        0      207 2023-01-05 13:32:53.000000 zernpy-0.0.8/src/zernpy/tests/__init__.py
--rw-rw-rw-   0        0        0     5758 2023-02-28 14:47:06.000000 zernpy-0.0.8/src/zernpy/tests/test_calculations.py
--rw-rw-rw-   0        0        0     5113 2023-02-28 15:51:31.000000 zernpy-0.0.8/src/zernpy/tests/test_fitting.py
--rw-rw-rw-   0        0        0     6422 2023-02-24 14:15:36.000000 zernpy-0.0.8/src/zernpy/tests/test_polynomials_initialization.py
--rw-rw-rw-   0        0        0    62325 2023-02-28 15:40:24.000000 zernpy-0.0.8/src/zernpy/zernikepol.py
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.091099 zernpy-0.0.8/src/zernpy.egg-info/
--rw-rw-rw-   0        0        0     7593 2023-02-28 16:00:52.000000 zernpy-0.0.8/src/zernpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2023-02-28 16:00:52.000000 zernpy-0.0.8/src/zernpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 16:00:52.000000 zernpy-0.0.8/src/zernpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-02-28 16:00:52.000000 zernpy-0.0.8/src/zernpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-28 16:00:52.000000 zernpy-0.0.8/src/zernpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-28 16:00:52.144133 zernpy-0.0.8/tests/
--rw-rw-rw-   0        0        0      728 2023-01-05 15:08:56.000000 zernpy-0.0.8/tests/test_package_import.py
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.577547 zernpy-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-02-02 11:40:00.000000 zernpy-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-02-02 12:31:23.000000 zernpy-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7842 2023-03-02 11:17:41.577547 zernpy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7075 2023-03-02 10:58:21.000000 zernpy-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1442 2023-03-02 11:00:07.000000 zernpy-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-02 11:17:41.577547 zernpy-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.514422 zernpy-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.537235 zernpy-0.0.9/src/zernpy/
+-rw-rw-rw-   0        0        0      962 2023-02-02 14:34:04.000000 zernpy-0.0.9/src/zernpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.561591 zernpy-0.0.9/src/zernpy/calculations/
+-rw-rw-rw-   0        0        0       72 2023-02-28 13:25:13.000000 zernpy-0.0.9/src/zernpy/calculations/__init__.py
+-rw-rw-rw-   0        0        0    38523 2023-03-02 10:39:50.000000 zernpy-0.0.9/src/zernpy/calculations/calc_zernike_pol.py
+-rw-rw-rw-   0        0        0    23546 2023-02-28 14:47:06.000000 zernpy-0.0.9/src/zernpy/calculations/find_pols_coeffs.py
+-rw-rw-rw-   0        0        0    13057 2023-02-02 10:08:32.000000 zernpy-0.0.9/src/zernpy/calculations/fit_zernike_pols.py
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.563585 zernpy-0.0.9/src/zernpy/plotting/
+-rw-rw-rw-   0        0        0       26 2022-12-05 11:57:03.000000 zernpy-0.0.9/src/zernpy/plotting/__init__.py
+-rw-rw-rw-   0        0        0     3840 2023-01-31 13:29:52.000000 zernpy-0.0.9/src/zernpy/plotting/plot_zerns.py
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.565581 zernpy-0.0.9/src/zernpy/props/
+-rw-rw-rw-   0        0        0       26 2023-02-24 13:23:33.000000 zernpy-0.0.9/src/zernpy/props/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-03-02 10:56:13.000000 zernpy-0.0.9/src/zernpy/props/properties.py
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.567575 zernpy-0.0.9/src/zernpy/readme_images/
+-rw-rw-rw-   0        0        0    59513 2023-02-02 11:26:55.000000 zernpy-0.0.9/src/zernpy/readme_images/Fitted_Profile.png
+-rw-rw-rw-   0        0        0    60427 2023-02-02 11:26:36.000000 zernpy-0.0.9/src/zernpy/readme_images/Random_Profile.png
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.571563 zernpy-0.0.9/src/zernpy/tests/
+-rw-rw-rw-   0        0        0      207 2023-01-05 13:32:53.000000 zernpy-0.0.9/src/zernpy/tests/__init__.py
+-rw-rw-rw-   0        0        0     5872 2023-03-02 10:07:20.000000 zernpy-0.0.9/src/zernpy/tests/test_calculations.py
+-rw-rw-rw-   0        0        0     5113 2023-03-02 10:44:56.000000 zernpy-0.0.9/src/zernpy/tests/test_fitting.py
+-rw-rw-rw-   0        0        0     6427 2023-03-02 10:56:13.000000 zernpy-0.0.9/src/zernpy/tests/test_polynomials_initialization.py
+-rw-rw-rw-   0        0        0    68960 2023-03-02 11:09:54.000000 zernpy-0.0.9/src/zernpy/zernikepol.py
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.557634 zernpy-0.0.9/src/zernpy.egg-info/
+-rw-rw-rw-   0        0        0     7842 2023-03-02 11:17:41.000000 zernpy-0.0.9/src/zernpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2023-03-02 11:17:41.000000 zernpy-0.0.9/src/zernpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-02 11:17:41.000000 zernpy-0.0.9/src/zernpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-03-02 11:17:41.000000 zernpy-0.0.9/src/zernpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-03-02 11:17:41.000000 zernpy-0.0.9/src/zernpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-02 11:17:41.577547 zernpy-0.0.9/tests/
+-rw-rw-rw-   0        0        0      728 2023-01-05 15:08:56.000000 zernpy-0.0.9/tests/test_package_import.py
```

### Comparing `zernpy-0.0.8/LICENSE` & `zernpy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zernpy-0.0.8/PKG-INFO` & `zernpy-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zernpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Calculation of Zernike polynomial value, their sums and basic plotting of their values in polar coordinates
 Author: Sergei Klykov
 Author-email: sergej.klykow@gmail.com
 License: MIT
 Project-URL: Homepage, https://pypi.org/project/zernpy/
 Project-URL: Repository, https://github.com/sklykov/zernpy/
 Project-URL: Bug Tracker, https://github.com/sklykov/zernpy/issues/
@@ -15,20 +15,22 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### zernpy - package for calculation Zernike polynomials
 
-This project is intended for calculation of Zernike polynomials parameters / values / properties using tabular and recursive equations, 
+This project is intended for calculation of Zernike polynomials parameters / values / properties using exact (analytical) and recursive equations, 
 the last ones were supposed to be the faster way to calculate values of high order polynomials in comparison to usage of their exact 
 definition (that used the sum of factorials, see the [Wiki article](https://en.wikipedia.org/wiki/Zernike_polynomials) for details).     
 However, it's turned out that usage of sum of factorials (calculated from *math.factorial* method) even for high orders provides
-sufficiently fast calculation of radial polynomials. Nevertheless, I hope that usage of recurrence equation might be advantageous (along
-with found way to speed up them by storing the coefficients for each radial order instead of using direct equation from the article).      
+sufficiently fast calculation of radial polynomials. On other hand, I found that for polynomials with radial orders higher than 46th order
+the exact equation with factorials starts providing ambiguous results due to high integers produced by factorials. Thus, it turns out that
+only possible stable way to get polynomial value for high orders is to use the recursive equations for retain stability of calculation along
+with the drawback of fast decreasing the performance with increasing of the radial order.    
 Also, I hope that someone also would find useful some of developed methods for usage in any further project.     
 The recursive and tabular equations are taken from the articles: [[1]](https://doi.org/10.1364/OL.38.002487), 
 [[2]](https://doi.org/10.1080/09500340.2011.554896) and [[3]](https://doi.org/10.1364/OE.26.018878).    
 Several useful transformations (e.g., from OSA / ANSI index to Noll one) are implemented as the methods of the main class.
 
 ### Setup instructions
```

### Comparing `zernpy-0.0.8/README.md` & `zernpy-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 ### zernpy - package for calculation Zernike polynomials
 
-This project is intended for calculation of Zernike polynomials parameters / values / properties using tabular and recursive equations, 
+This project is intended for calculation of Zernike polynomials parameters / values / properties using exact (analytical) and recursive equations, 
 the last ones were supposed to be the faster way to calculate values of high order polynomials in comparison to usage of their exact 
 definition (that used the sum of factorials, see the [Wiki article](https://en.wikipedia.org/wiki/Zernike_polynomials) for details).     
 However, it's turned out that usage of sum of factorials (calculated from *math.factorial* method) even for high orders provides
-sufficiently fast calculation of radial polynomials. Nevertheless, I hope that usage of recurrence equation might be advantageous (along
-with found way to speed up them by storing the coefficients for each radial order instead of using direct equation from the article).      
+sufficiently fast calculation of radial polynomials. On other hand, I found that for polynomials with radial orders higher than 46th order
+the exact equation with factorials starts providing ambiguous results due to high integers produced by factorials. Thus, it turns out that
+only possible stable way to get polynomial value for high orders is to use the recursive equations for retain stability of calculation along
+with the drawback of fast decreasing the performance with increasing of the radial order.    
 Also, I hope that someone also would find useful some of developed methods for usage in any further project.     
 The recursive and tabular equations are taken from the articles: [[1]](https://doi.org/10.1364/OL.38.002487), 
 [[2]](https://doi.org/10.1080/09500340.2011.554896) and [[3]](https://doi.org/10.1364/OE.26.018878).    
 Several useful transformations (e.g., from OSA / ANSI index to Noll one) are implemented as the methods of the main class.
 
 ### Setup instructions
```

### Comparing `zernpy-0.0.8/pyproject.toml` & `zernpy-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zernpy"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     {name = "Sergei Klykov"},
     {email = "sergej.klykow@gmail.com"}
 ]
 description = "Calculation of Zernike polynomial value, their sums and basic plotting of their values in polar coordinates"
 readme = "README.md"
 # license = {file = "LICENSE"}  # includes the whole text in METADATA, maybe not so convienient
```

### Comparing `zernpy-0.0.8/src/zernpy/__init__.py` & `zernpy-0.0.9/src/zernpy/__init__.py`

 * *Files identical despite different names*

### Comparing `zernpy-0.0.8/src/zernpy/calculations/calc_zernike_pol.py` & `zernpy-0.0.9/src/zernpy/calculations/calc_zernike_pol.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,23 +7,30 @@
 
 """
 # %% Global imports
 import numpy as np
 import math
 import time
 from pathlib import Path
+# from decimal import Decimal
 
 # %% Local (package-scoped) imports
 if __name__ == "__main__" or __name__ == Path(__file__).stem or __name__ == "__mp_main__":
     from find_pols_coeffs import find_coeffs_orders, find_coeffs_orders_dr
 else:
     from .find_pols_coeffs import find_coeffs_orders, find_coeffs_orders_dr
 
 # %% Module parameters
 __docformat__ = "numpydoc"
+# Below - empirically found max radial order allowing stable calculation using recursive coefficients defining
+# or using exact equation involving factorials calculation. Approximately, from 46th order the exact equation start
+# to violate condition that max of radial polynomial <= 1.0. From 40th order the difference between recurrence eq.
+# the exact one start to be too significant
+MAX_RADIAL_ORDER_COEFFS = 40
+MAX_RADIAL_ORDER_COEFFS_dR = 38
 
 
 # %% Calc. functions
 def define_orders(zernike_pol) -> tuple:
     """
     Return orders as tuple (m, n) for using in the functions below.
 
@@ -446,14 +453,17 @@
         return -m*np.cos(m*theta)
 
 
 def radial_polynomial_coeffs(zernike_pol, r):
     """
     Calculate radial polynomial using recursive finding algorithm of each coefficient for radial component (e.g. R^6).
 
+    After 40 order, this function again uses the recursive equation, because the finding the coefficients becomes
+    unstable.
+
     Parameters
     ----------
     zernike_pol : ZernPol or tuple with orders (m, n)
         ZernPol - class instance of the calling class (module zernikepol) or tuple with azimuthal and radial orders.
     r : float or numpy.ndarray
         Radius from the unit circle, float or array of values on which the Zernike polynomial is calculated.
 
@@ -463,24 +473,40 @@
 
     Returns
     -------
     r_sum : float or numpy.ndarray
         Depending on the type of theta, return float or np.ndarray with calculated values of radial polynomial.
 
     """
-    pols_coeffs = find_coeffs_orders(define_orders(zernike_pol))
+    m, n = define_orders(zernike_pol)
+    if n <= MAX_RADIAL_ORDER_COEFFS:
+        pols_coeffs = find_coeffs_orders((m, n))
     # Initial value for sum calculation
     if isinstance(r, float):
         r_sum = 0.0
     elif isinstance(r, np.ndarray):
         r_sum = np.zeros(shape=r.shape)
-    # Calculation of sum of orders
-    for key, value in pols_coeffs.items():
-        if abs(value) > 0:
-            r_sum += value*np.power(r, key)
+    # Calculation of sum of orders for not super high orders
+    if n <= MAX_RADIAL_ORDER_COEFFS:
+        for key, value in pols_coeffs.items():
+            if abs(value) > 0:
+                r_sum += value*np.power(r, key)
+    # Special case - for really high orders
+    else:
+        # Recurrence equations - stable way to refer previously stably calculated values
+        # Simple check that values stably calculated - radial polynomial values shouldn't exceed 1.0
+        if abs(m) == n:  # derivative from the simplified recurrence formula from [3]
+            r_sum = np.power(r, n)
+        elif m == 0:  # simplified recurrence formula from [3]
+            r_sum = 2.0*r*radial_polynomial_coeffs((1, n-1), r) - radial_polynomial_coeffs((0, n-2), r)
+        elif abs(m) == n-2:  # my guess about overall equation
+            r_sum = float(n)*np.power(r, n) - float(n-1)*np.power(r, n-2)
+        else:
+            r_sum = (r*(radial_polynomial_coeffs((abs(m-1), n-1), r) + radial_polynomial_coeffs((m+1, n-1), r))
+                     - radial_polynomial_coeffs((m, n-2), r))  # general recurrence formula from [1]
     return r_sum
 
 
 def radial_polynomial_coeffs_dr(zernike_pol, r):
     """
     Calculate radial polynomial derivative using recursive finding algorithm of each coefficient for radial component.
 
@@ -497,24 +523,43 @@
 
     Returns
     -------
     r_sum : float or numpy.ndarray
         Depending on the type of theta, return float or np.ndarray with calculated values of radial polynomial derivative.
 
     """
-    pols_coeffs = find_coeffs_orders_dr(define_orders(zernike_pol))
+    m, n = define_orders(zernike_pol)
+    if n <= MAX_RADIAL_ORDER_COEFFS_dR:
+        pols_coeffs = find_coeffs_orders_dr((m, n))
     # Initial value for sum calculation
     if isinstance(r, float):
         r_sum = 0.0
     elif isinstance(r, np.ndarray):
         r_sum = np.zeros(shape=r.shape)
-    # Calculation of sum of orders
-    for key, value in pols_coeffs.items():
-        if abs(value) > 0:
-            r_sum += value*np.power(r, key)
+    # Calculation of sum of orders for not super high orders
+    if n <= MAX_RADIAL_ORDER_COEFFS_dR:
+        for key, value in pols_coeffs.items():
+            if abs(value) > 0:
+                r_sum += value*np.power(r, key)
+    # Special case - for really high orders
+    else:
+        # Recurrence equations - stable way to refer previously stably calculated values
+        # Simple check that values stably calculated - radial polynomial values shouldn't exceed 1.0
+        if abs(m) == n:  # simplified recurrence formula from [3]
+            r_sum = float(n)*np.power(r, n-1)
+        elif m == 0:  # derivative from the simplified recurrence formula from [3]
+            r_sum = (2.0*(radial_polynomial_coeffs_dr((1, n-1), r) + r*radial_polynomial_coeffs_dr((1, n-1), r))
+                     - radial_polynomial_coeffs_dr((0, n-2), r))
+        elif abs(m) == n-2:  # derivative from my guess about overall equation
+            r_sum = float(n)*float(n)*np.power(r, n-1) - float(n-1)*float(n-2)*np.power(r, n-3)
+        else:
+            # derivative from the general recurrence formula from [1]
+            r_sum = ((radial_polynomial_coeffs((abs(m-1), n-1), r) + radial_polynomial_coeffs((m+1, n-1), r))
+                     + r*(radial_polynomial_coeffs_dr((abs(m-1), n-1), r) + radial_polynomial_coeffs_dr((m+1, n-1), r))
+                     - radial_polynomial_coeffs_dr((m, n-2), r))
     return r_sum
 
 
 # %% Test functions
 def compare_radial_calculations(max_order: int) -> np.ndarray:
     """
     Test difference between tabular/recursive and exact equation implementations of radial Zernike polynomials.
@@ -543,21 +588,20 @@
     for order in range(1, max_order):
         m = -order; n = order
         orders_list.append((m, n))
         for n_azimuthals in range(0, order):
             m += 2
             orders_list.append((m, n))
 
-    # Generation numpy array with radiuses
+    # Generation numpy array with radii
     n_points = 21
     test_r = np.zeros(shape=(n_points, ))
     for i in range(n_points):
         test_r[i] = i/(n_points-1)
     test_r = np.round(test_r, 4)
-
     # Testing that exact calculation and implementation of tabular / recursive are the same
     diff = np.ones(shape=(len(orders_list), n_points))
     for i, order in enumerate(orders_list):
         diff[i, :] = radial_polynomial(order, test_r) - radial_polynomial_eq(order, test_r)
     diff = np.round(diff, 9)
     assert np.max(np.abs(diff)) < 1E-9, (f"Order {order} has inconsistency between tabular/recursion"
                                          + f" and exact implementations, diff: {np.max(np.abs(diff))}")
@@ -593,21 +637,20 @@
     for order in range(1, max_order):
         m = -order; n = order
         orders_list.append((m, n))
         for n_azimuthals in range(0, order):
             m += 2
             orders_list.append((m, n))
 
-    # Generation numpy array with radiuses
+    # Generation numpy array with radii
     n_points = 21
     test_r = np.zeros(shape=(n_points, ))
     for i in range(n_points):
         test_r[i] = i/(n_points-1)
     test_r = np.round(test_r, 4)
-
     # Testing that exact calculation and implementation of tabular / recursive are the same
     diff = np.ones(shape=(len(orders_list), n_points))
     for i, order in enumerate(orders_list):
         diff[i, :] = radial_derivative(order, test_r) - radial_derivative_eq(order, test_r)
     diff = np.round(diff, 9)
     assert np.max(np.abs(diff)) < 1E-9, (f"Order {order} has inconsistency between tabular/recursion"
                                          + f" and exact implementations, diff: {np.max(np.abs(diff))}")
@@ -615,124 +658,166 @@
     return diff
 
 
 def compare_recursive_coeffs_radials() -> np.ndarray:
     """
     Test difference between exact radials and finding pols. coeffs. implementations of radial Zernike polynomials.
 
+    Comparison performed between orders 15 and 41 (more than MAX_RADIAL_ORDER_COEFFS).
+
     Returns
     -------
     diff : numpy.ndarray
-        Size corresponds to number of tested orders (m, n) calculated for the input and 21 radiuses between [0, 1].
-        Note that the checked precision difference is 1E-6 and thus the returned matrix also rounded to 9 numbers after
+        Size corresponds to number of tested orders (m, n) calculated for the input and 101 radii between [0, 1].
+        Note that the checked precision difference is 2E-2 and thus the returned matrix also rounded to 9 numbers after
         floating point.
 
     """
     # Generating Zernike orders in OSA/ANSI indexing scheme
     orders_list = []
-    for order in range(12, 26):
+    for order in range(15, MAX_RADIAL_ORDER_COEFFS+2):
         m = -order; n = order
         orders_list.append((m, n))
         for n_azimuthals in range(0, order):
             m += 2
             orders_list.append((m, n))
-    # Generation numpy array with radiuses
-    n_points = 21
+    # Generation numpy array with radii
+    n_points = 101
     test_r = np.zeros(shape=(n_points, ))
     for i in range(n_points):
         test_r[i] = i/(n_points-1)
     test_r = np.round(test_r, 4)
-
     # Testing that exact calculation and implementation of tabular / recursive are the same
     diff = np.ones(shape=(len(orders_list), n_points))
     for i, order in enumerate(orders_list):
         diff[i, :] = radial_polynomial_eq(order, test_r) - radial_polynomial_coeffs(order, test_r)
+        # diff[i, :] = radial_polynomial_coeffs(order, test_r)
+        # diff[i, :] = radial_polynomial_eq(order, test_r)
+        # if np.max(np.abs(diff)) > 1.0:
+        #     print(order, np.max(np.abs(diff)))
     diff = np.round(diff, 9)
-    assert np.max(np.abs(diff)) < 1E-6, (f"Order {order} has inconsistency between tabular/recursion"
+    assert np.max(np.abs(diff)) < 2E-2, (f"Order {order} has inconsistency between tabular/recursion"
                                          + f" and exact implementations, diff: {np.max(np.abs(diff))}")
     print("Difference between exact equation and pols. coeffs. finding algorithm is negligible, test passed")
     return diff
 
 
 def compare_recursive_coeffs_radials_dr() -> np.ndarray:
     """
     Test difference between exact radials and finding pols. coeffs. implementations of radial Zernike polynomials derivatives.
 
+    Comparison performed between orders 15 and 41 (more than MAX_RADIAL_ORDER_COEFFS).
+
     Returns
     -------
     diff : numpy.ndarray
         Size corresponds to number of tested orders (m, n) calculated for the input and 21 radiuses between [0, 1].
-        Note that the checked precision difference is 1E-6 and thus the returned matrix also rounded to 9 numbers after
+        Note that the checked precision difference is 5E-2 and thus the returned matrix also rounded to 9 numbers after
         floating point.
 
     """
     # Generating Zernike orders in OSA/ANSI indexing scheme
     orders_list = []
-    for order in range(12, 26):
+    for order in range(15, MAX_RADIAL_ORDER_COEFFS_dR+2):
         m = -order; n = order
         orders_list.append((m, n))
         for n_azimuthals in range(0, order):
             m += 2
             orders_list.append((m, n))
-    # Generation numpy array with radiuses
-    n_points = 21
+    # Generation numpy array with radii
+    n_points = 101
     test_r = np.zeros(shape=(n_points, ))
     for i in range(n_points):
         test_r[i] = i/(n_points-1)
     test_r = np.round(test_r, 4)
-
     # Testing that exact calculation and implementation of tabular / recursive are the same
     diff = np.ones(shape=(len(orders_list), n_points))
     for i, order in enumerate(orders_list):
         diff[i, :] = radial_derivative_eq(order, test_r) - radial_polynomial_coeffs_dr(order, test_r)
+        # if np.max(np.abs(diff)) > 1.0:
+        #     print(order, np.max(np.abs(diff)))
     diff = np.round(diff, 9)
-    assert np.max(np.abs(diff)) < 1E-6, (f"Order {order} has inconsistency between tabular/recursion"
+    assert np.max(np.abs(diff)) < 5E-2, (f"Order {order} has inconsistency between tabular/recursion"
                                          + f" and exact implementations, diff: {np.max(np.abs(diff))}")
     print("Difference between exact equation and pols. coeffs. finding algorithm is negligible, test passed")
     return diff
 
 
+def check_high_orders_recursion() -> np.ndarray:
+    """
+    Test max of abs value of calculated recursively radial polynomials for orders [41, 45].
+
+    Returns
+    -------
+    diff : numpy.ndarray.
+        Composed radial polynomials values for 51 radii.
+
+    """
+    # Generating Zernike orders in OSA/ANSI indexing scheme
+    orders_list = []
+    for order in range(MAX_RADIAL_ORDER_COEFFS+1, MAX_RADIAL_ORDER_COEFFS+6):
+        m = -order; n = order
+        orders_list.append((m, n))
+        for n_azimuthals in range(0, order):
+            m += 2
+            orders_list.append((m, n))
+    # Generation numpy array with radii
+    n_points = 51
+    test_r = np.zeros(shape=(n_points, ))
+    for i in range(n_points):
+        test_r[i] = i/(n_points-1)
+    test_r = np.round(test_r, 4)
+    # Testing that exact calculation and implementation of tabular / recursive are the same
+    diff = np.ones(shape=(len(orders_list), n_points))
+    for i, order in enumerate(orders_list):
+        diff[i, :] = radial_polynomial_coeffs(order, test_r)
+    diff = np.round(diff, 6)
+    assert np.max(np.abs(diff)) <= 1.0, f"Order {order} has inconsistency in max abs value: {np.max(np.abs(diff))}"
+    print("Abs max in calculated recursively radial polynomials <= 1.0, test passed")
+    return diff
+
+
 def time_radial_pols():
     """
     Measure in the simple way the required time for calculation of radial polynomials with high orders.
 
     Returns
     -------
     None.
 
     """
     calc_times_ms = []  # for storing calculation times
     zp1 = (2, 16); zp2 = (0, 18); zp3 = (-2, 20); zp4 = (6, 22); zp5 = (-4, 24); zp6 = (-3, 25); r = 0.425
-    zpols = [zp1, zp2, zp3, zp4, zp5, zp6]
+    zpols = [zp1, zp2, zp3, zp4, zp5]
     for zp in zpols:
         t1 = time.perf_counter()
         radial_polynomial(zp, r)
         t2 = time.perf_counter()
         calc_times_ms.append(int(round(1000*(t2-t1), 0)))
     print("Timed calc. recursive rad. pol.", zpols, ":", calc_times_ms)
     calc_times_ms = []  # refresh stored values
     for zp in zpols:
         t1 = time.perf_counter()
         radial_polynomial_coeffs(zp, r)
         t2 = time.perf_counter()
-        calc_times_ms.append(int(round(1000*(t2-t1), 0)))
+        calc_times_ms.append(round(1000*(t2-t1), 3))
     print("Timed calc. using finding coeffs. rad. pol.", calc_times_ms)
     calc_times_ms = []  # refresh stored values
     for zp in zpols:
         t1 = time.perf_counter()
         radial_polynomial_eq(zp, r)
         t2 = time.perf_counter()
-        calc_times_ms.append(int(round(1000*(t2-t1), 0)))
+        calc_times_ms.append(round(1000*(t2-t1), 3))
     print("Timed calc. using exact equation rad. pol.", calc_times_ms)
     calc_times_ms = []  # refresh stored values
     for zp in zpols:
         t1 = time.perf_counter()
         radial_polynomial_coeffs_dr(zp, r)
         t2 = time.perf_counter()
-        calc_times_ms.append(int(round(1000*(t2-t1), 0)))
+        calc_times_ms.append(round(1000*(t2-t1), 3))
     print("Timed calc. using finding coeffs. deriv. rad. pol.", calc_times_ms)
     # Separate test of exact equation performance
     zp1 = (-14, 18); zp2 = (0, 26); zp3 = (3, 29); zp4 = (0, 31); zp5 = (-2, 36); zp6 = (1, 39); r = 0.425
     zpols = [zp1, zp2, zp3, zp4, zp5, zp6]
     calc_times_ms = []  # refresh stored values
     for zp in zpols:
         t1 = time.perf_counter()
@@ -748,10 +833,12 @@
     Theta = [i*np.pi/3 for i in range(6)]; Theta = np.asarray(Theta)
     orders = (-2, 2); r = 0.5
     ZR = radial_polynomial(orders, R); ZR1 = radial_polynomial(orders, r)
     TR = triangular_function(orders, Theta)
     diff = compare_radial_calculations(max_order=20)
     diff_deriv = compare_radial_derivatives(max_order=18)
     # Test specific implementations
-    orders = (-7, 11); r = 0.55; val = radial_polynomial(orders, r)
-    time_radial_pols(); diff_coeffs = compare_recursive_coeffs_radials()
+    orders = (-8, 52); r = 0.95; val = radial_polynomial_coeffs(orders, r)
+    time_radial_pols()  # initial estimation of performance of calculations
+    diff_coeffs = compare_recursive_coeffs_radials()
     diff_deriv_coeffs = compare_recursive_coeffs_radials_dr()
+    high_R = check_high_orders_recursion()
```

### Comparing `zernpy-0.0.8/src/zernpy/calculations/find_pols_coeffs.py` & `zernpy-0.0.9/src/zernpy/calculations/find_pols_coeffs.py`

 * *Files identical despite different names*

### Comparing `zernpy-0.0.8/src/zernpy/calculations/fit_zernike_pols.py` & `zernpy-0.0.9/src/zernpy/calculations/fit_zernike_pols.py`

 * *Files identical despite different names*

### Comparing `zernpy-0.0.8/src/zernpy/plotting/plot_zerns.py` & `zernpy-0.0.9/src/zernpy/plotting/plot_zerns.py`

 * *Files identical despite different names*

### Comparing `zernpy-0.0.8/src/zernpy/readme_images/Fitted_Profile.png` & `zernpy-0.0.9/src/zernpy/readme_images/Fitted_Profile.png`

 * *Files identical despite different names*

### Comparing `zernpy-0.0.8/src/zernpy/readme_images/Random_Profile.png` & `zernpy-0.0.9/src/zernpy/readme_images/Random_Profile.png`

 * *Files identical despite different names*

### Comparing `zernpy-0.0.8/src/zernpy/tests/test_calculations.py` & `zernpy-0.0.9/src/zernpy/tests/test_calculations.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,31 @@
 """
 import math
 import numpy as np
 
 # Importing the written in the modules test functions for letting pytest library their automatic exploration
 if __name__ != "__main__":
     from ..calculations.calc_zernike_pol import (compare_radial_calculations, compare_radial_derivatives,
-                                                 compare_recursive_coeffs_radials, compare_recursive_coeffs_radials_dr)
+                                                 compare_recursive_coeffs_radials, compare_recursive_coeffs_radials_dr,
+                                                 check_high_orders_recursion)
     from ..zernikepol import ZernPol
 
 
 # Testing implemented equations for tabular R(m, n) from References by comparing with the exact ones (with factorials)
 def test_tabular_orders():
     compare_radial_calculations(max_order=10)
 
 
 # Testing implemented tabular and recursive equations for R(m, n) by comparing with the exact ones (with factorials)
 # Also, testing implemented recursive scheme for finding the polynomials coefficients for each order and comparison
 # with the exact equations (with factorials)
 def test_recursive_orders():
     compare_radial_calculations(max_order=17)
     compare_recursive_coeffs_radials()
+    check_high_orders_recursion()
 
 
 # Testing derived equations for derivatives dR(m, n)/dr by comparing with the exact ones (with factorials)
 def test_tabular_derivatives():
     compare_radial_derivatives(max_order=10)
```

### Comparing `zernpy-0.0.8/src/zernpy/tests/test_fitting.py` & `zernpy-0.0.9/src/zernpy/tests/test_fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 height = 127; width = 127; crop_r = 1.0; strict_border = False; mdp = 15.0; stop_warns = False
             elif i == 5:
                 height = 140; width = 140; crop_r = 0.98; strict_border = False; mdp = 25.0; stop_warns = True
             elif i == 6:
                 height = 201; width = 204; crop_r = 0.94; strict_border = True; mdp = 20.0; stop_warns = True
             elif i == 7:
                 # The allowed percentage below is huge because the cropping radius is equal to 80% of image size
-                height = 200; width = 200; strict_border = False; crop_r = 0.8; mdp = 33.0; stop_warns = True
+                height = 150; width = 150; strict_border = False; crop_r = 0.8; mdp = 33.0; stop_warns = True
             random_phases_image, random_amplitudes, polynomials_tuple = generate_random_phases(max_order=i, img_height=height,
                                                                                                img_width=width)
             fitted_amplitudes, _ = fit_polynomials(random_phases_image, polynomials_tuple, suppress_warnings=stop_warns,
                                                    crop_radius=crop_r, strict_circle_border=strict_border)
             abs_diff_amplitudes = np.abs(fitted_amplitudes - random_amplitudes)
             max_abs_diff = round(np.max(abs_diff_amplitudes), 6); max_src_ampl = round(np.max(np.abs(random_amplitudes)), 6)
             # max_ampl = max(np.max(np.abs(random_amplitudes)), np.max(np.abs(fitted_amplitudes)))  # max abs amplitude
```

### Comparing `zernpy-0.0.8/src/zernpy/tests/test_polynomials_initialization.py` & `zernpy-0.0.9/src/zernpy/tests/test_polynomials_initialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # Testing initialization of Zernike polynomials, for details, see the zernikepol module
 def test_polynomials_initialization():
     check_conformity()
 
 
 # Explicit testing initialization of Zernike polynomials
 def test_explicit_initialization():
-    # Testing the ordinar, normal initialization of polynomials
+    # Testing the ordinary, normal initialization of polynomials
     m = 0; n = 2; zp = ZernPol(l=m, n=n)
     assert abs(zp.radial_dr(0.25) - 1.0) < 1E-9, f"Radial derivative calculated with error for Z{(m, n)}"
     m = 0; n = 6; zp = ZernPol(n=n, l=m)
     assert abs(zp.triangular_dtheta(math.pi)) < 1E-9, f"Triangular derivative calculated with error for Z{(m, n)}"
     m = -1; n = 1; zp = ZernPol(azimuthal_order=m, radial_order=n)
     assert abs(zp.polynomial_value(0.5, math.pi/2) - 1.0) < 1E-9, f"Pol. value Z{(m, n)} for r=0.5, theta=pi/2 calculated with error"
     m = 2; n = 2; zp = ZernPol(azimuthal_order=m, radial_order=n)
@@ -47,15 +47,15 @@
     zernpol = ZernPol(osa=9); m, n = zernpol.get_mn_orders()
     assert zernpol.get_polynomial_name() == "Oblique trefoil", f"Returned wrong name for Z{(m, n)}"
     zernpol = ZernPol(noll=15); m, n = zernpol.get_mn_orders()
     assert zernpol.get_polynomial_name(True) == "Obliq. 4foil", f"Returned wrong short name for Z{(m, n)}"
     zernpol = ZernPol(fringe=60); m, n = zernpol.get_mn_orders()
     assert len(zernpol.get_polynomial_name()) == 0, f"Returned some name for Z{(m, n)}, but it's not defined"
 
-    # Testing wrong initialization parameters - for checking that they not passed through
+    # Testing wrong initialization parameters - for checking that they are not passed through
     # OSA
     try:
         ZernPol(osa=-1); assert_flag = False
     except ValueError:
         assert_flag = True
     assert assert_flag, "Wrong initialization parameter passed: ZernPol(osa=-1)"
```

### Comparing `zernpy-0.0.8/src/zernpy/zernikepol.py` & `zernpy-0.0.9/src/zernpy/zernikepol.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,32 +12,35 @@
 import numpy as np
 from pathlib import Path
 import warnings
 import math
 from collections import namedtuple
 import matplotlib.pyplot as plt
 import random
+import time
 
 # %% Local (package-scoped) imports
 if __name__ == "__main__" or __name__ == Path(__file__).stem or __name__ == "__mp_main__":
     from calculations.calc_zernike_pol import (normalization_factor, radial_polynomial, triangular_function,
                                                triangular_derivative, radial_derivative,
                                                radial_polynomial_eq, radial_derivative_eq,
-                                               radial_polynomial_coeffs, radial_polynomial_coeffs_dr)
+                                               radial_polynomial_coeffs, radial_polynomial_coeffs_dr,
+                                               MAX_RADIAL_ORDER_COEFFS, MAX_RADIAL_ORDER_COEFFS_dR)
     from plotting.plot_zerns import plot_sum_fig, subplot_sum_on_fig
     from calculations.fit_zernike_pols import crop_phases_img, fit_zernikes
-    from props.properties import polynomial_names, short_polynomial_names
+    from props.properties import polynomial_names, short_polynomial_names, warn_mess_r_long, warn_mess_dr_long
 else:
     from .calculations.calc_zernike_pol import (normalization_factor, radial_polynomial, triangular_function,
                                                 triangular_derivative, radial_derivative,
                                                 radial_polynomial_eq, radial_derivative_eq,
-                                                radial_polynomial_coeffs, radial_polynomial_coeffs_dr)
+                                                radial_polynomial_coeffs, radial_polynomial_coeffs_dr,
+                                                MAX_RADIAL_ORDER_COEFFS, MAX_RADIAL_ORDER_COEFFS_dR)
     from .plotting.plot_zerns import plot_sum_fig, subplot_sum_on_fig
     from .calculations.fit_zernike_pols import crop_phases_img, fit_zernikes
-    from .props.properties import polynomial_names, short_polynomial_names
+    from .props.properties import polynomial_names, short_polynomial_names, warn_mess_r_long, warn_mess_dr_long
 
 # %% Module parameters
 __docformat__ = "numpydoc"
 polar_vectors = namedtuple("PolarVectors", "R Theta")  # re-used below as the return type
 zernikes_surface = namedtuple("ZernikesSurface", "ZernSurf R Theta")  # used as input type
 
 
@@ -51,16 +54,16 @@
 
     def __init__(self, **kwargs):
         """
         Initialize of the class for Zernike polynomial definition as the object.
 
         Parameters
         ----------
-        **kwargs : orders or index for Zernike polynomial initialization. \n
-            Acceptable variants for key word arguments: \n
+        **kwargs : orders or index for Zernike polynomial initialization expected as key=value pairs \n
+            Acceptable variants for key=value pairs arguments: \n
             1) n=int, m=int with alternatives: "radial_order" for n; "l", "azimuthal_order", "angular_frequency" for m; \n
             2) osa_index=int with alternatives: "osa", "ansi_index", "ansi"; \n
             3) noll_index=int with alternative "noll"; \n
             4) fringe_index=int with alternative "fringe" \n
 
         Raises
         ------
@@ -193,14 +196,23 @@
                     else:
                         raise ValueError("Fringe index provided not as an integer")
         else:
             raise ValueError("Length of provided key arguments are not equal 1 (OSA/Fringe/Noll index) or 2 (m, n orders)")
         # Also raise the ValueError if the ZernPol hasn't been initialized by orders / indices
         if not self.__initialized:
             raise ValueError("The initialization parameters for Zernike polynomial hasn't been parsed / recognized")
+        # Generate warning messages for possible re-usage
+        if self.__n > MAX_RADIAL_ORDER_COEFFS:
+            self.__warn_mes_r = f"Call for radial order {self.__n} is higher than {MAX_RADIAL_ORDER_COEFFS}"
+        else:
+            self.warn_mes_r = ""
+        if self.__n > MAX_RADIAL_ORDER_COEFFS_dR:
+            self.__warn_mes_dr = f"Call for derivative of radial order {self.__n} is > than {MAX_RADIAL_ORDER_COEFFS_dR}"
+        else:
+            self.warn_mes_dr = ""
 
     def get_indices(self):
         """
         Return the tuple with following orders: ((m, n), OSA index, Noll index, Fringe index).
 
         Returns
         -------
@@ -254,17 +266,23 @@
 
     # %% Calculations
     def polynomial_value(self, r, theta, use_exact_eq: bool = False):
         """
         Calculate Zernike polynomial value(-s) within the unit circle.
 
         Calculation up to 10th order of Zernike function performed by exact equations from Ref.[2],
-        after - using the recurrence equations taken from the Ref.[1]. \n
+        after - using the recurrence equations taken from the Ref.[1], using shortcut of storing
+        coefficients for each power of radius (coefficient*R^n) \n
         Surprisingly, the exact equation for polynomials are just pretty fast to use them directly, without
-        any need to use the recurrence equations. It can be used by providing the flag as the input parameter.
+        any need to use the recurrence equations. It can be used by providing the flag as the input parameter. \n
+        However, after ~ the 46th radial order due to the high integer values involved in the exact equation
+        (factorials) producing ambiguous results (failed simple check that radial polynomial <= 1.0),
+        only iterative equations (which along with increasing order become time-consuming and slow)
+        could be used. The 40th radial order as the limit for usage of the exact equation is selected due to
+        found increasing after this order discrepancy between results of recursive and factorial formulas.
 
         References
         ----------
         [1] Shakibaei B.H., Paramesran R. "Recursive formula to compute Zernike radial polynomials" (2013) \n
         [2] Lakshminarayanan V., Fleck A. "Zernike polynomials: a guide" (2011) \n
         [3] Andersen T. B. "Efficient and robust recurrence relations for the Zernike
         circle polynomials and their derivatives in Cartesian coordinates" (2018) \n
@@ -274,16 +292,15 @@
         r : float or numpy.ndarray
             Radius (radii) from unit circle or the range [0.0, 1.0], float / array, for which the polynomial is calculated.
         theta : float or numpy.ndarray
             Theta - angle in radians from the range [0, 2*pi], float or array, for which the polynomial is calculated.
             Note that the theta counting is counterclockwise, as it is default for the matplotlib library.
         use_exact_eq : bool, optional
             Flag for using the exact equation with factorials. The default is False.
-            Surprisingly, but even factorials for high numbers are calculated actually pretty fast, so the radial
-            polynomials could be calculated without using any recursion.
+            Note about the limit for usage of the exact equation - up to 40th radial order (n).
 
         Raises
         ------
         ValueError
             Check the Error stack trace for reasons of raising, most probably input parameters aren't acceptable.
         Warning
             If the theta angles lie outside the range [0, 2*pi] (entire period).
@@ -300,46 +317,59 @@
         # Checking that angles lie in the range [0, 2*pi] and their type
         theta = ZernPol._check_angles(theta)
         # Checking coincidence of shapes if theta and r are arrays
         if isinstance(r, np.ndarray) and isinstance(theta, np.ndarray):
             if r.shape != theta.shape:
                 raise ValueError("Shape of input arrays r and theta is not equal")
         # Calculation using imported function from submodule depending on radial order, use different eq.
-        if self.__n <= 15:  # after, the direct recursive eq. becomes ineffective
-            return normalization_factor(self)*radial_polynomial(self, r)*triangular_function(self, theta)
+        nTr = normalization_factor(self)*triangular_function(self, theta)
+        if not use_exact_eq:
+            if self.__n <= 12:  # condition to switch from direct recurrence equation to finding of coeffs. algorithm
+                return nTr*radial_polynomial(self, r)
+            else:
+                return nTr*radial_polynomial_coeffs(self, r)
         else:
-            if not use_exact_eq:
-                return normalization_factor(self)*radial_polynomial_coeffs(self, r)*triangular_function(self, theta)
+            if self.__n > MAX_RADIAL_ORDER_COEFFS:
+                warnings.warn(self.__warn_mes_r + warn_mess_r_long)
+                if isinstance(r, float):
+                    return 0.0
+                elif isinstance(r, np.ndarray):
+                    return np.zeros(shape=r.shape)
             else:
-                return normalization_factor(self)*radial_polynomial_eq(self, r)*triangular_function(self, theta)
+                return nTr*radial_polynomial_eq(self, r)
 
     def radial(self, r, use_exact_eq: bool = False):
         """
         Calculate R(m, n) - radial Zernike function value(-s) within the unit circle.
 
         Calculation up to 10th order of Zernike function performed by exact equations from Ref.[2],
-        after - using the recurrence equations taken from the Ref.[1]. \n
+        after - using the recurrence equations taken from the Ref.[1], using shortcut of storing
+        coefficients for each power of radius (coefficient*R^n) \n
         Surprisingly, the exact equation for polynomials are just pretty fast to use them directly, without
-        any need to use the recurrence equations. It can be used by providing the flag as the input parameter.
+        any need to use the recurrence equations. It can be used by providing the flag as the input parameter. \n
+        However, after ~ the 46th radial order due to the high integer values involved in the exact equation
+        (factorials) producing ambiguous results (failed simple check that radial polynomial <= 1.0),
+        only iterative equations (which along with increasing order become time-consuming and slow)
+        could be used. The 40th radial order as the limit for usage of the exact equation is selected due to
+        found increasing after this order discrepancy between results of recursive and factorial formulas.
 
         References
         ----------
         [1] Shakibaei B.H., Paramesran R. "Recursive formula to compute Zernike radial polynomials" (2013) \n
         [2] Lakshminarayanan V., Fleck A. "Zernike polynomials: a guide" (2011) \n
         [3] Andersen T. B. "Efficient and robust recurrence relations for the Zernike
         circle polynomials and their derivatives in Cartesian coordinates" (2018) \n
 
         Parameters
         ----------
         r : float or numpy.ndarray
             Radius (radii) from unit circle or the range [0.0, 1.0], float / array, for which the function is calculated.
         use_exact_eq : bool, optional
             Flag for using the exact equation with factorials. The default is False.
-            Surprisingly, but even factorials for high numbers are calculated actually pretty fast, so the radial
-            polynomials could be calculated without using any recursion.
+            Note about the limit for usage of the exact equation - up to 40th radial order (n).
 
         Raises
         ------
         ValueError
             The probable reasons: radius (radii) doesn't belong to a unit circle, input type isn't acceptable.
 
         Returns
@@ -347,19 +377,26 @@
         float or numpy.ndarray
             Calculated Zernike radial function value(-s) on provided float values / arrays of radiuses.
 
         """
         # Check radii type and that they are not lying outside range [0.0, 1.0] - unit circle
         r = ZernPol._check_radii(r)
         # Calculation using imported function from submodule depending on radial order, use different eq.
-        if self.__n <= 15:  # after, the direct recursive eq. becomes ineffective
-            return radial_polynomial(self, r)
-        else:
-            if not use_exact_eq:
+        if not use_exact_eq:
+            if self.__n <= 12:  # condition to switch from direct recurrence equation to finding of coeffs. algorithm
+                return radial_polynomial(self, r)
+            else:
                 return radial_polynomial_coeffs(self, r)
+        else:
+            if self.__n > MAX_RADIAL_ORDER_COEFFS:
+                warnings.warn(self.__warn_mes_r + warn_mess_r_long)
+                if isinstance(r, float):
+                    return 0.0
+                elif isinstance(r, np.ndarray):
+                    return np.zeros(shape=r.shape)
             else:
                 return radial_polynomial_eq(self, r)
 
     def triangular(self, theta):
         """
         Calculate triangular Zernike function value(-s) within the unit circle.
 
@@ -389,28 +426,36 @@
         return triangular_function(self, theta)
 
     def radial_dr(self, r, use_exact_eq: bool = False):
         """
         Calculate derivative of radial Zernike polynomial value(-s) within the unit circle.
 
         Calculation up to 10th order of Zernike polynomials performed by exact equations,
-        after - using the recurrence equations.
+        after - using the recurrence equations, using shortcut of storing
+        coefficients for each power of radius (coefficient*R^n) \n
+        The input flag use_exact_eq allows using the exact equation with factorials.
+        But note that after 38th radial order the usage of the exact equation is forbidden, because
+        after ~ the 44th radial order due to the high integer values associated with factorials and power
+        values produced by derivatives leading to ambiguous results, only iterative equations
+        (which along with increasing order become time-consuming and slow) could be used. The 38th radial order
+        as the limit for usage of the exact equation is selected due to found increasing after this order
+        discrepancy between results of recursive and factorial formulas.
+
 
         References
         ----------
         Same as for the method "radial" or "polynomial value"
 
         Parameters
         ----------
         r : float or numpy.ndarray
             Radius (radii) from unit circle or the range [0.0, 1.0], float / array, for which the polynomial is calculated.
         use_exact_eq : bool, optional
             Flag for using the exact equation with factorials. The default is False.
-            Surprisingly, but even factorials for high numbers are calculated actually pretty fast, so the radial
-            polynomials could be calculated without using any recursion.
+            Note about the limit for usage of the exact equation - up to 38th radial order (n).
 
         Raises
         ------
         ValueError
             The probable reasons: radius (radii) doesn't belong to a unit circle, input type isn't acceptable.
 
         Returns
@@ -418,19 +463,26 @@
         float or numpy.ndarray
             Calculated derivative of Zernike radial function value(-s) on provided float values / arrays of radiuses.
 
         """
         # Checking input parameters for avoiding errors and unexpectable values
         r = ZernPol._check_radii(r)
         # Calculation using imported function from submodule depending on radial order, use different eq.
-        if self.__n <= 15:  # after, the direct recursive eq. becomes ineffective
-            return radial_derivative(self, r)
-        else:
-            if not use_exact_eq:
+        if not use_exact_eq:
+            if self.__n <= 12:  # condition to switch from direct recurrence equation to finding of coeffs. algorithm
+                return radial_derivative(self, r)
+            else:
                 return radial_polynomial_coeffs_dr(self, r)
+        else:
+            if self.__n > MAX_RADIAL_ORDER_COEFFS_dR:
+                warnings.warn(self.__warn_mes_dr + warn_mess_dr_long)
+                if isinstance(r, float):
+                    return 0.0
+                elif isinstance(r, np.ndarray):
+                    return np.zeros(shape=r.shape)
             else:
                 return radial_derivative_eq(self, r)
 
     def triangular_dtheta(self, theta):
         """
         Calculate derivative from triangular function on angle theta.
 
@@ -1196,14 +1248,83 @@
     zernike_coefficients = np.round(zernike_coefficients, round_digits)
     if return_cropped_image:
         return zernike_coefficients, cropped_image
     else:
         return zernike_coefficients, None
 
 
+def compare_performances(min_order: int, max_order: int) -> tuple:
+    """
+    Compare performances of radial polynomials calculation by using recursive and exact equations.
+
+    Comparison achieved by simple measuring of time in msec needed for calculation of all radial
+    polynomials from minimal radial order up to maximum radial order returned as tuple.
+
+    Parameters
+    ----------
+    min_order : int
+        Minimum radial order of used polynomials (n).
+    max_order : int
+        Maximum radial order of used polynomials (n).
+
+    Returns
+    -------
+    tuple
+        Composed by time for recursive calculation and time for exact calculation.
+
+    """
+    # Generation of orders in OSA/ANSI indexing scheme for initializing Zernike polynomials
+    zernpols = []
+    for order in range(min_order, max_order+1):
+        m = -order; n = order
+        zernpols.append(ZernPol(m=m, n=n))
+        for n_azimuthals in range(0, order):
+            m += 2
+            zernpols.append(ZernPol(m=m, n=n))
+    # Generation numpy array with radii
+    n_points = 251
+    test_r = np.zeros(shape=(n_points, ))
+    for i in range(n_points):
+        test_r[i] = i/(n_points-1)
+    test_r = np.round(test_r, 6)
+    # Measuring performance of radial polynomials calculations using recursive implementation
+    t1 = time.perf_counter()
+    for i, polynomial in enumerate(zernpols):
+        polynomial.radial(test_r)  # calculate radial polynomials over vector of radii
+    t2 = time.perf_counter()
+    t_recursive_ms = round(1000*(t2-t1), 3)
+    # Measuring performance of radial polynomials calculations using exact implementation
+    t1 = time.perf_counter()
+    for i, polynomial in enumerate(zernpols):
+        polynomial.radial(test_r, use_exact_eq=True)  # calculate radial polynomials over vector of radii
+    t2 = time.perf_counter()
+    t_exact_ms = round(1000*(t2-t1), 3)
+    return (t_recursive_ms, t_exact_ms, f"Used polynomials: {i}", f"Radii: {n_points}")
+
+
+def _estimate_high_order_calc_times():
+    """
+    Estimate slowing down of radial polynomial calculation with increasing of radial order.
+
+    Returns
+    -------
+    None.
+
+    """
+    r = 0.55
+    high_order_pols = [ZernPol(m=-2, n=46), ZernPol(m=1, n=47), ZernPol(m=2, n=48), ZernPol(m=-1, n=49),
+                       ZernPol(m=2, n=50), ZernPol(m=1, n=51), ZernPol(m=-2, n=52)]
+    times = []
+    for pol in high_order_pols:
+        # calculate radial polynomials over vector of radii
+        t1 = time.perf_counter(); pol.radial(r); t2 = time.perf_counter()
+        times.append(f"{pol.get_mn_orders()}: {int(round(1000*(t2-t1), 0))} ms")
+    print(times)
+
+
 # %% Test functions for the external call
 def check_conformity():
     """
     Test initialization parameters and transform between indices consistency.
 
     Returns
     -------
@@ -1282,15 +1403,16 @@
         zp = ZernPol(m=-10, n=30); ZernPol.plot_zernike_polynomial(zp, color_map="jet", show_title=False)  # high order plot
         # ZernPol._plot_zernikes_half_pyramid()
         fig3 = plt.figure(figsize=(2, 2)); zp3 = ZernPol(osa=58); polynomials = [zp3]; coefficients = [1.0]
         fig3 = ZernPol.plot_sum_zernikes_on_fig(coefficients, polynomials, fig3, show_range=False, color_map="turbo")
         fig3.subplots_adjust(0, 0, 1, 1)
         # Tests with generation / restoring Zernike profiles (phases images)
         phases_image, polynomials_ampls, polynomials = generate_random_phases(img_height=301, img_width=301)
-        plt.figure(); plt.axis("off"); plt.imshow(phases_image, cmap="jet"); plt.tight_layout(); plt.subplots_adjust(0, 0, 1, 1)
+        plt.figure(); plt.axis("off"); plt.imshow(phases_image, cmap="jet"); plt.tight_layout()
+        plt.subplots_adjust(0, 0, 1, 1)
         polynomials_amplitudes, cropped_img = fit_polynomials(phases_image, polynomials, return_cropped_image=True,
                                                               strict_circle_border=False, crop_radius=1.0)
         plt.figure(); plt.axis("off"); plt.imshow(cropped_img, cmap="jet"); plt.tight_layout(); plt.subplots_adjust(0, 0, 1, 1)
         plt.show()  # show all images created by plt.figure() calls
     # Simple test of two concepts of calculations - exact and recursive equations
     z = ZernPol(n=30, m=-2); print("Diff. between recursive and exact equations:",
                                    round(z.radial(0.85) - z.radial(0.85, use_exact_eq=True), 9))
@@ -1299,7 +1421,13 @@
     r = -0.955; theta = np.pi/8; z = ZernPol(osa=55)
     print("Diff. between recursive and exact equations:",
           round(z.polynomial_value(r, theta) - z.polynomial_value(r, theta, use_exact_eq=True), 9))
     z = ZernPol(n=35, l=-1); print("Diff. between recursive & exact eq-s for derivatives:",
                                    round(z.radial_dr(0.78) - z.radial_dr(0.78, use_exact_eq=True), 9))
     z = ZernPol(n=38, m=-2); print("Diff. between recursive & exact eq-s for derivatives:",
                                    round(z.radial_dr(0.9) - z.radial_dr(0.9, use_exact_eq=True), 9))
+    # Compare performances
+    print("Tabular (10th order) / exact calc. times:", compare_performances(1, 10))
+    print("Recursive / exact calc. times for high orders:", compare_performances(12, 40))
+    # Statement below producing expected warnings
+    # print("Slow Recursive / exact calc. times for high orders:", compare_performances(41, 42))
+    _estimate_high_order_calc_times()
```

### Comparing `zernpy-0.0.8/src/zernpy.egg-info/PKG-INFO` & `zernpy-0.0.9/src/zernpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zernpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Calculation of Zernike polynomial value, their sums and basic plotting of their values in polar coordinates
 Author: Sergei Klykov
 Author-email: sergej.klykow@gmail.com
 License: MIT
 Project-URL: Homepage, https://pypi.org/project/zernpy/
 Project-URL: Repository, https://github.com/sklykov/zernpy/
 Project-URL: Bug Tracker, https://github.com/sklykov/zernpy/issues/
@@ -15,20 +15,22 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### zernpy - package for calculation Zernike polynomials
 
-This project is intended for calculation of Zernike polynomials parameters / values / properties using tabular and recursive equations, 
+This project is intended for calculation of Zernike polynomials parameters / values / properties using exact (analytical) and recursive equations, 
 the last ones were supposed to be the faster way to calculate values of high order polynomials in comparison to usage of their exact 
 definition (that used the sum of factorials, see the [Wiki article](https://en.wikipedia.org/wiki/Zernike_polynomials) for details).     
 However, it's turned out that usage of sum of factorials (calculated from *math.factorial* method) even for high orders provides
-sufficiently fast calculation of radial polynomials. Nevertheless, I hope that usage of recurrence equation might be advantageous (along
-with found way to speed up them by storing the coefficients for each radial order instead of using direct equation from the article).      
+sufficiently fast calculation of radial polynomials. On other hand, I found that for polynomials with radial orders higher than 46th order
+the exact equation with factorials starts providing ambiguous results due to high integers produced by factorials. Thus, it turns out that
+only possible stable way to get polynomial value for high orders is to use the recursive equations for retain stability of calculation along
+with the drawback of fast decreasing the performance with increasing of the radial order.    
 Also, I hope that someone also would find useful some of developed methods for usage in any further project.     
 The recursive and tabular equations are taken from the articles: [[1]](https://doi.org/10.1364/OL.38.002487), 
 [[2]](https://doi.org/10.1080/09500340.2011.554896) and [[3]](https://doi.org/10.1364/OE.26.018878).    
 Several useful transformations (e.g., from OSA / ANSI index to Noll one) are implemented as the methods of the main class.
 
 ### Setup instructions
```

### Comparing `zernpy-0.0.8/src/zernpy.egg-info/SOURCES.txt` & `zernpy-0.0.9/src/zernpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zernpy-0.0.8/tests/test_package_import.py` & `zernpy-0.0.9/tests/test_package_import.py`

 * *Files identical despite different names*

