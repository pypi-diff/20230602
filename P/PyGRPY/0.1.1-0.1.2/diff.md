# Comparing `tmp/PyGRPY-0.1.1.tar.gz` & `tmp/PyGRPY-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGRPY-0.1.1.tar", last modified: Mon Sep 26 17:42:42 2022, max compression
+gzip compressed data, was "PyGRPY-0.1.2.tar", last modified: Fri Jun  2 10:27:38 2023, max compression
```

## Comparing `PyGRPY-0.1.1.tar` & `PyGRPY-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 radost    (1000) radost    (1000)        0 2022-09-26 17:42:42.937025 PyGRPY-0.1.1/
--rw-r--r--   0 radost    (1000) radost    (1000)    35149 2021-05-20 17:25:05.000000 PyGRPY-0.1.1/LICENSE
--rw-rw-r--   0 radost    (1000) radost    (1000)     1001 2022-09-26 17:42:42.937025 PyGRPY-0.1.1/PKG-INFO
-drwxrwxr-x   0 radost    (1000) radost    (1000)        0 2022-09-26 17:42:42.937025 PyGRPY-0.1.1/PyGRPY.egg-info/
--rw-r--r--   0 radost    (1000) radost    (1000)     1001 2022-09-26 17:42:42.000000 PyGRPY-0.1.1/PyGRPY.egg-info/PKG-INFO
--rw-r--r--   0 radost    (1000) radost    (1000)      289 2022-09-26 17:42:42.000000 PyGRPY-0.1.1/PyGRPY.egg-info/SOURCES.txt
--rw-r--r--   0 radost    (1000) radost    (1000)        1 2022-09-26 17:42:42.000000 PyGRPY-0.1.1/PyGRPY.egg-info/dependency_links.txt
--rw-r--r--   0 radost    (1000) radost    (1000)        1 2021-05-21 07:21:34.000000 PyGRPY-0.1.1/PyGRPY.egg-info/not-zip-safe
--rw-r--r--   0 radost    (1000) radost    (1000)        7 2022-09-26 17:42:42.000000 PyGRPY-0.1.1/PyGRPY.egg-info/top_level.txt
--rw-rw-r--   0 radost    (1000) radost    (1000)      573 2022-09-26 17:33:48.000000 PyGRPY-0.1.1/README.md
-drwxrwxr-x   0 radost    (1000) radost    (1000)        0 2022-09-26 17:42:42.937025 PyGRPY-0.1.1/pygrpy/
--rw-r--r--   0 radost    (1000) radost    (1000)       45 2021-05-23 15:59:52.000000 PyGRPY-0.1.1/pygrpy/__init__.py
--rw-rw-r--   0 radost    (1000) radost    (1000)     2175 2022-09-26 17:40:56.000000 PyGRPY-0.1.1/pygrpy/grpy.py
--rw-r--r--   0 radost    (1000) radost    (1000)    13148 2022-02-02 14:57:04.000000 PyGRPY-0.1.1/pygrpy/grpy_tensors.py
--rw-rw-r--   0 radost    (1000) radost    (1000)     9106 2022-02-02 14:44:16.000000 PyGRPY-0.1.1/pygrpy/jax_grpy_tensors.py
--rw-rw-r--   0 radost    (1000) radost    (1000)       38 2022-09-26 17:42:42.937025 PyGRPY-0.1.1/setup.cfg
--rw-rw-r--   0 radost    (1000) radost    (1000)      689 2022-09-26 17:33:40.000000 PyGRPY-0.1.1/setup.py
-drwxrwxr-x   0 radost    (1000) radost    (1000)        0 2022-09-26 17:42:42.937025 PyGRPY-0.1.1/test/
--rw-r--r--   0 radost    (1000) radost    (1000)    10560 2021-05-23 16:05:07.000000 PyGRPY-0.1.1/test/test.py
--rw-r--r--   0 radost    (1000) radost    (1000)     9912 2021-05-31 11:26:51.000000 PyGRPY-0.1.1/test/test_jax.py
+drwxrwxr-x   0 radost    (1000) radost    (1000)        0 2023-06-02 10:27:38.874615 PyGRPY-0.1.2/
+-rw-r--r--   0 radost    (1000) radost    (1000)    35149 2021-05-20 17:25:05.000000 PyGRPY-0.1.2/LICENSE
+-rw-rw-r--   0 radost    (1000) radost    (1000)     1248 2023-06-02 10:27:38.874615 PyGRPY-0.1.2/PKG-INFO
+drwxrwxr-x   0 radost    (1000) radost    (1000)        0 2023-06-02 10:27:38.874615 PyGRPY-0.1.2/PyGRPY.egg-info/
+-rw-r--r--   0 radost    (1000) radost    (1000)     1248 2023-06-02 10:27:38.000000 PyGRPY-0.1.2/PyGRPY.egg-info/PKG-INFO
+-rw-r--r--   0 radost    (1000) radost    (1000)      299 2023-06-02 10:27:38.000000 PyGRPY-0.1.2/PyGRPY.egg-info/SOURCES.txt
+-rw-r--r--   0 radost    (1000) radost    (1000)        1 2023-06-02 10:27:38.000000 PyGRPY-0.1.2/PyGRPY.egg-info/dependency_links.txt
+-rw-r--r--   0 radost    (1000) radost    (1000)        1 2021-05-21 07:21:34.000000 PyGRPY-0.1.2/PyGRPY.egg-info/not-zip-safe
+-rw-r--r--   0 radost    (1000) radost    (1000)        7 2023-06-02 10:27:38.000000 PyGRPY-0.1.2/PyGRPY.egg-info/top_level.txt
+-rw-rw-r--   0 radost    (1000) radost    (1000)      820 2022-09-27 19:26:16.000000 PyGRPY-0.1.2/README.md
+drwxrwxr-x   0 radost    (1000) radost    (1000)        0 2023-06-02 10:27:38.874615 PyGRPY-0.1.2/pygrpy/
+-rw-r--r--   0 radost    (1000) radost    (1000)       45 2021-05-23 15:59:52.000000 PyGRPY-0.1.2/pygrpy/__init__.py
+-rw-rw-r--   0 radost    (1000) radost    (1000)     2175 2022-09-26 17:40:56.000000 PyGRPY-0.1.2/pygrpy/grpy.py
+-rw-r--r--   0 radost    (1000) radost    (1000)    15769 2023-06-02 10:20:48.000000 PyGRPY-0.1.2/pygrpy/grpy_tensors.py
+-rw-rw-r--   0 radost    (1000) radost    (1000)     9106 2022-02-02 14:44:16.000000 PyGRPY-0.1.2/pygrpy/jax_grpy_tensors.py
+-rw-rw-r--   0 radost    (1000) radost    (1000)       38 2023-06-02 10:27:38.874615 PyGRPY-0.1.2/setup.cfg
+-rw-rw-r--   0 radost    (1000) radost    (1000)      689 2023-06-02 10:24:10.000000 PyGRPY-0.1.2/setup.py
+drwxrwxr-x   0 radost    (1000) radost    (1000)        0 2023-06-02 10:27:38.874615 PyGRPY-0.1.2/tests/
+-rw-r--r--   0 radost    (1000) radost    (1000)     9912 2021-05-31 11:26:51.000000 PyGRPY-0.1.2/tests/test_jax.py
+-rw-r--r--   0 radost    (1000) radost    (1000)    10857 2023-06-02 10:17:09.000000 PyGRPY-0.1.2/tests/test_tensors.py
```

### Comparing `PyGRPY-0.1.1/LICENSE` & `PyGRPY-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGRPY-0.1.1/PKG-INFO` & `PyGRPY-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: PyGRPY
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python port of Generalized Rotne Prager Yakamava tensors
 Home-page: https://github.com/RadostW/PyGRPY/
 Author: Radost Waszkiewicz
 Author-email: radost.waszkiewicz@gmail.com
 License: GNU GPLv3
 Project-URL: Documentation, https://pygrpy.readthedocs.io
 Project-URL: Source, https://github.com/RadostW/PyGRPY/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Tests](https://github.com/RadostW/PyGRPY/actions/workflows/tests.yml/badge.svg)
+
 # PyGRPY
 
 Python port of Generalized Rotne Prager Yakamawa hydrodynamic tensors.
 
 Now also supports jax, and jax.grad.
 
 
@@ -29,9 +31,12 @@
 
 Copyright (c) Pawel Jan Zuk (2017) - unported code.
 
 Copyright (c) Radost Waszkiewicz (2021) - python port.
 
 # How to cite
 
+Waszkiewicz, R., Bartczak M., Kolasa K. and Lisicki M. *Pychastic: Precise Brownian Dynamics using 
+Taylor-Ito integrators in Python*; Sci-Post (submitted) (2022)
+
 Zuk, P. J., B. Cichocki, and P. Szymczak *GRPY - an accurate bead method for calculation of hydrodynamic
 properties of rigid biomacromolecules*; Biophys. J. (submitted) (2017)
```

### Comparing `PyGRPY-0.1.1/PyGRPY.egg-info/PKG-INFO` & `PyGRPY-0.1.2/PyGRPY.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: PyGRPY
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python port of Generalized Rotne Prager Yakamava tensors
 Home-page: https://github.com/RadostW/PyGRPY/
 Author: Radost Waszkiewicz
 Author-email: radost.waszkiewicz@gmail.com
 License: GNU GPLv3
 Project-URL: Documentation, https://pygrpy.readthedocs.io
 Project-URL: Source, https://github.com/RadostW/PyGRPY/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Tests](https://github.com/RadostW/PyGRPY/actions/workflows/tests.yml/badge.svg)
+
 # PyGRPY
 
 Python port of Generalized Rotne Prager Yakamawa hydrodynamic tensors.
 
 Now also supports jax, and jax.grad.
 
 
@@ -29,9 +31,12 @@
 
 Copyright (c) Pawel Jan Zuk (2017) - unported code.
 
 Copyright (c) Radost Waszkiewicz (2021) - python port.
 
 # How to cite
 
+Waszkiewicz, R., Bartczak M., Kolasa K. and Lisicki M. *Pychastic: Precise Brownian Dynamics using 
+Taylor-Ito integrators in Python*; Sci-Post (submitted) (2022)
+
 Zuk, P. J., B. Cichocki, and P. Szymczak *GRPY - an accurate bead method for calculation of hydrodynamic
 properties of rigid biomacromolecules*; Biophys. J. (submitted) (2017)
```

### Comparing `PyGRPY-0.1.1/README.md` & `PyGRPY-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![Tests](https://github.com/RadostW/PyGRPY/actions/workflows/tests.yml/badge.svg)
+
 # PyGRPY
 
 Python port of Generalized Rotne Prager Yakamawa hydrodynamic tensors.
 
 Now also supports jax, and jax.grad.
 
 
@@ -16,9 +18,12 @@
 
 Copyright (c) Pawel Jan Zuk (2017) - unported code.
 
 Copyright (c) Radost Waszkiewicz (2021) - python port.
 
 # How to cite
 
+Waszkiewicz, R., Bartczak M., Kolasa K. and Lisicki M. *Pychastic: Precise Brownian Dynamics using 
+Taylor-Ito integrators in Python*; Sci-Post (submitted) (2022)
+
 Zuk, P. J., B. Cichocki, and P. Szymczak *GRPY - an accurate bead method for calculation of hydrodynamic
 properties of rigid biomacromolecules*; Biophys. J. (submitted) (2017)
```

### Comparing `PyGRPY-0.1.1/pygrpy/grpy.py` & `PyGRPY-0.1.2/pygrpy/grpy.py`

 * *Files identical despite different names*

### Comparing `PyGRPY-0.1.1/pygrpy/grpy_tensors.py` & `PyGRPY-0.1.2/pygrpy/grpy_tensors.py`

 * *Files 15% similar despite different names*

```diff
@@ -271,15 +271,80 @@
     # construct large matricies
     muTT = (
                 muTTidentityScale[:,:,np.newaxis,np.newaxis] * np.identity(3)[np.newaxis,np.newaxis,:,:] 
                 + muTTrHatScale[:,:,np.newaxis,np.newaxis] * rHatMatrix[:,:,np.newaxis,:] * rHatMatrix[:,:,:,np.newaxis]
            )
     # flatten (n,n,3,3) tensor in the correct order
     return muTT
-        
+
+def muTT_trace(centres,radii):
+    """
+    Returns beadwise trace of grand mobility matrix in RPY approximation.
+
+    Parameters
+    ----------
+    centers: np.array
+        An ``N`` by 3 array describing locations of centres of ``N`` beads.
+    radii: np.array
+        An array of length ``N`` describing sizes of ``N`` beads.
+
+    Returns
+    -------
+    np.array
+        A ``N`` by ``N`` array containing traces of translational mobility coefficients
+        of the beads.
+    """
+
+    # number of beads
+    n = len(radii)
+
+    displacements = centres[:, np.newaxis, :] - centres[np.newaxis, :, :]
+    distances = np.sqrt(np.sum(displacements ** 2, axis=-1)) 
+
+    # shorthand for radii, consistent with publication of Zuk et al
+    a = radii 
+    
+    ai = a[:,np.newaxis]
+    aj = a[np.newaxis,:]
+    
+    dist = distances + np.identity(n) # add identity to allow division
+
+    # prefactors of matricies for each bead pair
+    # matricies are {identity, r^hat r^hat, \\epsilon_ijk r^hat_k}
+    # these are grouped by interaction type {TT,TR,RR}
+    # and by solution branch {diagonal, close, far} for Rotne-Prager and Yakamava parts
+    # numpy magic does all operations componentwise
+
+    # ### translational matricies
+    muTTidentityScaleDiag   = 1.0 / (6 * math.pi * ai)
+
+    muTTidentityScaleFar    = (1.0 / (8.0 * math.pi * dist)) * (1.0 + (ai ** 2 + aj ** 2) / (3 * (dist ** 2)))
+    muTTrHatScaleFar        = (1.0 / (8.0 * math.pi * dist)) * (1.0 - (ai ** 2 + aj ** 2) / (dist ** 2))
+
+    muTTidentityScaleClose  = (1.0 / (6.0 * math.pi * ai * aj)) * ( ( 16.0 * (dist ** 3) * (ai + aj) - ((ai - aj) ** 2 + 3 * (dist ** 2)) ** 2 ) / (32.0 * (dist ** 3)))
+    muTTrHatScaleClose      = (1.0 / (6.0 * math.pi * ai * aj)) * ( 3.0 * ((ai - aj) ** 2 - dist ** 2) ** 2 / (32.0 * (dist ** 3)))
+
+    muTTidentityScaleInside = (1.0 / (6.0 * math.pi * np.maximum(ai,aj)))
+
+    # solution branch indicators
+    isFar = 1.0*(dist > ai + aj)
+    isOutside = 1.0*(dist > np.maximum(ai,aj) - np.minimum(ai,aj))
+    isDiag = 1.0*(np.identity(n))
+
+    # combine scale factors from branches
+    muTTidentityScale = isDiag * muTTidentityScaleDiag + (1.0 - isDiag) * (isOutside * (isFar * muTTidentityScaleFar + (1.0 - isFar) * muTTidentityScaleClose) + (1.0-isOutside) * muTTidentityScaleInside)
+    muTTrHatScale = isOutside * ((1.0 - isDiag) * (isFar * muTTrHatScaleFar + (1.0-isFar) * muTTrHatScaleClose))
+
+    # construct large matricies
+    ret_muTT_trace = (
+                3 *muTTidentityScale[:,:] 
+                + muTTrHatScale[:,:]
+           )
+    # flatten (n,n,3,3) tensor in the correct order
+    return ret_muTT_trace
 
 def conglomerateMobilityMatrix(centres,radii):
     '''
     Returns mobility matrix centred at `[0,0,0]` of bead conglomerate specified 
     by `centres` and `radii`. Treats conglomerate as rigid body.
```

### Comparing `PyGRPY-0.1.1/pygrpy/jax_grpy_tensors.py` & `PyGRPY-0.1.2/pygrpy/jax_grpy_tensors.py`

 * *Files identical despite different names*

### Comparing `PyGRPY-0.1.1/setup.py` & `PyGRPY-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='PyGRPY',
-      version='0.1.1',
+      version='0.1.2',
       description='Python port of Generalized Rotne Prager Yakamava tensors',
       url='https://github.com/RadostW/PyGRPY/',
       author='Radost Waszkiewicz',
       author_email='radost.waszkiewicz@gmail.com',
       long_description=long_description,
       long_description_content_type='text/markdown',  # This is important!
       project_urls = {
```

### Comparing `PyGRPY-0.1.1/test/test.py` & `PyGRPY-0.1.2/tests/test_tensors.py`

 * *Files 7% similar despite different names*

```diff
@@ -133,12 +133,19 @@
     assert type(testmob) == np.ndarray
     assert np.allclose(testmob, mob_four)
 
 def test_hydrosize():
     testsize = pygrpy.grpy.stokesRadius(centres_four,sizes_four)
     assert np.allclose(testsize, 1.5409546371938094)
 
+def test_fast_trace():
+    slow_mu = pygrpy.grpy_tensors.muTT(centres_four,sizes_four)
+    slow_trace_mu = np.trace(slow_mu, axis1=-2, axis2=-1)
+    fast_trace_mu = pygrpy.grpy_tensors.muTT_trace(centres_four,sizes_four)
+    assert np.allclose(slow_trace_mu, fast_trace_mu)
+
 if __name__ == "__main__":
     test_mobility_single_bead()
     test_mobility_two_beads()
     test_mobility_four_beads()  
     test_projection_four_beads()  
+    test_fast_trace()
```

### Comparing `PyGRPY-0.1.1/test/test_jax.py` & `PyGRPY-0.1.2/tests/test_jax.py`

 * *Files identical despite different names*

