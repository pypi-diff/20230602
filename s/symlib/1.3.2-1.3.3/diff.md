# Comparing `tmp/symlib-1.3.2.tar.gz` & `tmp/symlib-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.3.2.tar", last modified: Thu May 25 11:21:37 2023, max compression
+gzip compressed data, was "symlib-1.3.3.tar", last modified: Fri Jun  2 20:23:33 2023, max compression
```

## Comparing `symlib-1.3.2.tar` & `symlib-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-25 11:21:37.328703 symlib-1.3.2/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.2/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-25 11:21:37.328568 symlib-1.3.2/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.2/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.2/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-05-25 11:21:37.328759 symlib-1.3.2/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-05-25 11:19:28.000000 symlib-1.3.2/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-25 11:21:37.327366 symlib-1.3.2/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1658 2023-05-25 11:19:28.000000 symlib-1.3.2/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.2/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    52489 2023-05-25 11:19:28.000000 symlib-1.3.2/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)    35330 2023-04-11 22:48:38.000000 symlib-1.3.2/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     8508 2023-05-06 00:43:01.000000 symlib-1.3.2/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-25 11:21:37.328357 symlib-1.3.2/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      287 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 20:23:33.481546 symlib-1.3.3/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.3/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-02 20:23:33.481428 symlib-1.3.3/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.3/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.3/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-02 20:23:33.481578 symlib-1.3.3/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-02 20:23:27.000000 symlib-1.3.3/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 20:23:33.480599 symlib-1.3.3/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1658 2023-05-25 11:19:28.000000 symlib-1.3.3/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.3/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    52489 2023-05-25 11:19:28.000000 symlib-1.3.3/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)    36176 2023-06-02 20:23:27.000000 symlib-1.3.3/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     8508 2023-05-06 00:43:01.000000 symlib-1.3.3/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 20:23:33.481284 symlib-1.3.3/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      287 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.3.2/LICENSE` & `symlib-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.3.2/PKG-INFO` & `symlib-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.2
+Version: 1.3.3
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.3.2/setup.py` & `symlib-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.3.2"
+version = "1.3.3"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.3.2/symlib/__init__.py` & `symlib-1.3.3/symlib/__init__.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.2/symlib/file_management.py` & `symlib-1.3.3/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.2/symlib/lib.py` & `symlib-1.3.3/symlib/lib.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.2/symlib/star_tagging.py` & `symlib-1.3.3/symlib/star_tagging.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,31 +41,44 @@
 class ProfileModel(abc.ABC):
     """ AbstractProfile is an abstract base class for galaxy profile models. It
     allows you to convert a half-light radius into an enclosed stellar mass
     profile.
     """
     
     @abc.abstractmethod
-    def m_enc(self, m_star, r_half, r):
+    def m_enc(self, m_star, r_half, r, **kwargs):
         """ m_enc returns the enclosed mass profile as a function of 3D radius,
         r. m_star is the asymptotic stellar mass of the galaxy, r_half is the 2D
         half-light radius of the galaxy. Returned masses will be in the same
         units as m_star.
         """
         pass
 
     @abc.abstractmethod
-    def density(self, m_star, r_half, r):
+    def density(self, m_star, r_half, r, **kwargs):
         """ density returns the local density as a function of 3D radius, r.
         m_star is the asymptotic stellas mass of the galaxy, r_hald is the 2D
         half-light radius of the galaxy. Returned masses will be in the same
         units of m_star.
         """
         pass
 
+    @abc.abstractmethod
+    def var_names(self):
+        """ var_names returns the names of the variables this model requires.
+        """
+        pass
+
+    def trim_kwargs(self, kwargs):
+        out = {}
+        for key in self.var_names():
+            out[key] = kwargs[key]
+        return out
+
+
 class RHalfModel(abc.ABC):
     """ RHalfModel is an abstract base class for models of galaxy half-mass
     radii. 
     """
     
     @abc.abstractmethod
     def r_half(self, **kwargs):
@@ -192,22 +205,25 @@
         load_particles() first with a non-None argument for v.
         """
         if self.v is None: raise ValueError("v not set")
         
         core = self.v[np.searchsorted(self.idx, self.core_idx)]
         return np.median(core, axis=0)
         
-    def set_mp_star(self, rvir, profile_model, r_half, m_star,
+    def set_mp_star(self, kwargs, profile_model, r_half, m_star,
                     r_bins=DEFAULT_R_BINS):
+        rvir = kwargs["rvir"]
+
         r = np.sqrt(np.sum(self.x**2, axis=1))/rvir
         M = ranked_np_profile_matrix(self.ranks, self.idx, r, r_bins)
         n = M.shape[1]
 
+        profile_kwargs = profile_model.trim_kwargs(kwargs)
         m_star_enc_target = profile_model.m_enc(
-            m_star, r_half, r_bins[1:]*rvir)
+            m_star, r_half, r_bins[1:]*rvir, **profile_kwargs)
         
         dm_star_enc_target = np.zeros(len(m_star_enc_target))
         dm_star_enc_target[1:] = m_star_enc_target[1:] - m_star_enc_target[:-1]
         dm_star_enc_target[0] = m_star_enc_target[0]
 
         res = optimize.lsq_linear(
             M, dm_star_enc_target, bounds=(np.zeros(n), np.inf*np.ones(n))
@@ -275,32 +291,35 @@
 # Specific Model Implementations #
 ##################################
 
     
 class PlummerProfile(ProfileModel):
     """ PlummerProfile models a galaxy's mass distribution as a Plummer sphere.
     """
-    def m_enc(self, m_star, r_half, r):
+    def m_enc(self, m_star, r_half, r, **kwargs):
         """ m_enc returns the enclosed mass profile as a function of 3D radius,
         r. m_star is the asymptotic stellar mass of the galaxy, r_half is the 2D
         half-light radius of the galaxy. Returned masses will be in the same
         units as m_star.
         """
         a = r_half
         return m_star*r**3 /(r**2 + a**2)**1.5
     
-    def density(self, m_star, r_half, r):
+    def density(self, m_star, r_half, r, **kwargs):
         """ density returns the local density as a function of 3D radius, r.
         m_star is the asymptotic stellas mass of the galaxy, r_hald is the 2D
         half-light radius of the galaxy. Returned masses will be in the same
         units of m_star.
         """
         a = r_half
         return 3*m_star/(4*np.pi*a**3) * (1 + r**2/a**2)**(-5/2)
     
+    def var_names(self):
+        return []
+
 class Nadler2020RHalf(RHalfModel):
     """ Nadler20202RHalf models galaxies according to the z=0 size-mass relation
     in Nadler et al. 2020. (https://arxiv.org/abs/1912.03303)
 
     This is calibrated by fitting a galaxy-halo model to Milky Way satellites.
     """
     
@@ -398,28 +417,30 @@
         self.sigma_log_R = sigma_log_R
         self.a = a
         self.b = b
     
     def r_half(self, rvir=None, cvir=None, z=None, no_scatter=False):
         """ r_half returns the half-mass radius of a a galaxy in physical kpc.
         Required keyword arguments:
-         - mstar
+         - rvir
+         - cvir
+         - z
         """
         R = 10**(self.a + self.b*np.log10(0.247))
         log_scatter = self.sigma_log_R*random.normal(0, 1, size=np.shape(rvir))
         if not no_scatter:
             return 10**(np.log10(R) + log_scatter)
         else:
             return R
 
 
     def var_names(self):
         """ var_names returns the names of the variables this model requires.
         """
-        return ["mstar"]
+        return ["rvir", "cvir", "z"]
 
 class Kirby2013Metallicity(MetallicityModel):
     """ Kirby2013Metallicity models galaxy metallicity according to the
     z-agnostic fit in Kirby et al. 2013 (https://arxiv.org/pdf/1310.0814.pdf;
     Equation 4).
     """
     def __init__(self, sigma_Fe_H=0.17, Fe_H_dist_width=0.3):
@@ -449,16 +470,15 @@
         """
         return ["mstar"]
     
 class UniverseMachineMStarFit(MStarModel):
     def m_star(self, mpeak=None, z=None, no_scatter=False):
         """
          Required keyword arguments:
-         - rvir
-         - cvir
+         - mpeak
          - z
         """
 
         if mpeak is None: raise ValueError("mpeak not supplied")
         if z is None: raise ValueError("z not supplied")
         
         mpeak = mpeak
@@ -517,15 +537,15 @@
         return Ms
     
     def var_names(self):
         """ var_names returns the names of the variables this model requires.
         """
         return ["mpeak", "z"]
     
-    
+
 class RadialEnergyRanking(AbstractRanking):
     def __init__(self, params, x, v, idx, n_max,
                  core_particles=DEFAULT_CORE_PARTICLES,
                  quantile_edges=DEFAULT_QUANTILE_EDGES):
         """ Takes mp (Msun; may be a scalar), x (pkpc), v (pkm/s), idx (the
         index into the full particle array), and n_max (the number of particles
         in the full particle arrays).
@@ -788,15 +808,15 @@
 
         if r_half is None:
             check_var_names(kwargs, self.r_half_model)
             r_half = self.r_half_model.r_half(
                 no_scatter=self.no_scatter,
                 **self.r_half_model.trim_kwargs(kwargs))
             
-        mp_star = ranks.set_mp_star(kwargs["rvir"], self.profile_model,
+        mp_star = ranks.set_mp_star(kwargs, self.profile_model,
                                     r_half, m_star)
 
 
         if Fe_H is None:
             check_var_names(kwargs, self.metal_model)
             Fe_H = self.metal_model.Fe_H(
                 len(mp_star), no_scatter=self.no_scatter,
@@ -805,20 +825,26 @@
         return mp_star, m_star, r_half, Fe_H
     
     def var_names(self):
         """ var_names returns the names of the variables this model requires.
         """
         r_half_names = self.r_half_model.var_names()
         m_star_names = self.m_star_model.var_names()
-        
+        metal_names = self.metal_model.var_names()
+        profile_names = self.profile_model.var_names()
+
         out_dict = { }
         for i in range(len(r_half_names)):
             out_dict[r_half_names[i]] = None
         for i in range(len(m_star_names)):
             out_dict[m_star_names[i]] = None
+        for i in range(len(metal_names)):
+            out_dict[metal_names[i]] = None
+        for i in range(len(profile_names)):
+            out_dict[profile_names[i]] = None
 
         if "rvir" not in out_dict: out_dict["rvir"] = None
             
         return sorted(list(out_dict.keys()))
 
     def get_kwargs(self, params, scale, halo, snap):
         """ get_kwargs creates the kwargs that that are needed for a call to
@@ -835,14 +861,16 @@
         for i in range(len(var_names)):
             if var_names[i] == "z":
                 kwargs["z"] = z
                 continue
 
             if var_names[i] == "mpeak":
                 x = np.max(halo["mvir"][:snap+1])
+            elif var_names[i] == "mstar":
+                continue
             else:
                 x = halo[snap][var_names[i]]
             
             kwargs[var_names[i]] = x
 
         return kwargs
```

### Comparing `symlib-1.3.2/symlib/util.py` & `symlib-1.3.3/symlib/util.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.2/symlib.egg-info/PKG-INFO` & `symlib-1.3.3/symlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.2
+Version: 1.3.3
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

