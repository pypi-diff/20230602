# Comparing `tmp/skysurvey-0.4.3.tar.gz` & `tmp/skysurvey-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey-0.4.3.tar", last modified: Wed May 31 11:53:31 2023, max compression
+gzip compressed data, was "skysurvey-0.5.1.tar", last modified: Fri Jun  2 10:05:29 2023, max compression
```

## Comparing `skysurvey-0.4.3.tar` & `skysurvey-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.032300 skysurvey-0.4.3/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.4.3/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-05-31 11:53:31.032169 skysurvey-0.4.3/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.4.3/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-31 11:53:31.032341 skysurvey-0.4.3/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)      632 2023-05-31 11:53:04.000000 skysurvey-0.4.3/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.030015 skysurvey-0.4.3/skysurvey/
--rw-r--r--   0 rigault   (2358) staff       (20)       92 2023-05-31 11:52:58.000000 skysurvey-0.4.3/skysurvey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.4.3/skysurvey/config.py
--rw-r--r--   0 rigault   (2358) staff       (20)    14150 2023-05-31 11:50:29.000000 skysurvey-0.4.3/skysurvey/dag.py
--rw-r--r--   0 rigault   (2358) staff       (20)    26322 2023-05-10 13:33:52.000000 skysurvey-0.4.3/skysurvey/dataset.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.031025 skysurvey-0.4.3/skysurvey/survey/
--rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.4.3/skysurvey/survey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8645 2023-05-02 20:15:06.000000 skysurvey-0.4.3/skysurvey/survey/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10973 2023-01-04 15:12:21.000000 skysurvey-0.4.3/skysurvey/survey/healpix.py
--rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.4.3/skysurvey/survey/polygon.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.4.3/skysurvey/survey/ztf.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.032016 skysurvey-0.4.3/skysurvey/target/
--rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.4.3/skysurvey/target/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.4.3/skysurvey/target/collection.py
--rw-r--r--   0 rigault   (2358) staff       (20)    31337 2023-05-31 08:44:18.000000 skysurvey-0.4.3/skysurvey/target/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.4.3/skysurvey/target/environments.py
--rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.4.3/skysurvey/target/kilonova.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2342 2023-05-07 10:18:11.000000 skysurvey-0.4.3/skysurvey/target/sncc.py
--rw-r--r--   0 rigault   (2358) staff       (20)     9879 2023-02-08 13:19:45.000000 skysurvey-0.4.3/skysurvey/target/snia.py
--rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-05-10 14:57:36.000000 skysurvey-0.4.3/skysurvey/target/stars.py
--rw-r--r--   0 rigault   (2358) staff       (20)     6216 2023-05-04 16:01:10.000000 skysurvey-0.4.3/skysurvey/target/timeserie.py
--rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.4.3/skysurvey/template.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.030476 skysurvey-0.4.3/skysurvey.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-05-31 11:53:30.000000 skysurvey-0.4.3/skysurvey.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      647 2023-05-31 11:53:31.000000 skysurvey-0.4.3/skysurvey.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 11:53:30.000000 skysurvey-0.4.3/skysurvey.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-05-31 11:53:30.000000 skysurvey-0.4.3/skysurvey.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 10:05:29.986789 skysurvey-0.5.1/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.5.1/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-06-02 10:05:29.986652 skysurvey-0.5.1/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.5.1/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-06-02 10:05:29.986830 skysurvey-0.5.1/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)      560 2023-06-02 10:04:59.000000 skysurvey-0.5.1/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 10:05:29.984206 skysurvey-0.5.1/skysurvey/
+-rw-r--r--   0 rigault   (2358) staff       (20)       92 2023-06-02 10:04:54.000000 skysurvey-0.5.1/skysurvey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.5.1/skysurvey/config.py
+-rw-r--r--   0 rigault   (2358) staff       (20)        0 2023-06-02 08:51:15.000000 skysurvey-0.5.1/skysurvey/dag.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    26322 2023-05-10 13:33:52.000000 skysurvey-0.5.1/skysurvey/dataset.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 10:05:29.985394 skysurvey-0.5.1/skysurvey/survey/
+-rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.5.1/skysurvey/survey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8645 2023-05-02 20:15:06.000000 skysurvey-0.5.1/skysurvey/survey/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10970 2023-06-02 10:03:36.000000 skysurvey-0.5.1/skysurvey/survey/healpix.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.5.1/skysurvey/survey/polygon.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.5.1/skysurvey/survey/ztf.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 10:05:29.986490 skysurvey-0.5.1/skysurvey/target/
+-rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.5.1/skysurvey/target/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.5.1/skysurvey/target/collection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    31327 2023-06-02 09:43:01.000000 skysurvey-0.5.1/skysurvey/target/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.5.1/skysurvey/target/environments.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.5.1/skysurvey/target/kilonova.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2342 2023-05-07 10:18:11.000000 skysurvey-0.5.1/skysurvey/target/sncc.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10070 2023-06-02 09:06:49.000000 skysurvey-0.5.1/skysurvey/target/snia.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.5.1/skysurvey/target/stars.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     6386 2023-06-02 09:51:33.000000 skysurvey-0.5.1/skysurvey/target/timeserie.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.5.1/skysurvey/template.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 10:05:29.984759 skysurvey-0.5.1/skysurvey.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-06-02 10:05:29.000000 skysurvey-0.5.1/skysurvey.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      647 2023-06-02 10:05:29.000000 skysurvey-0.5.1/skysurvey.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-02 10:05:29.000000 skysurvey-0.5.1/skysurvey.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-06-02 10:05:29.000000 skysurvey-0.5.1/skysurvey.egg-info/top_level.txt
```

### Comparing `skysurvey-0.4.3/LICENSE` & `skysurvey-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.3/README.md` & `skysurvey-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.3/skysurvey/dataset.py` & `skysurvey-0.5.1/skysurvey/dataset.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.3/skysurvey/survey/core.py` & `skysurvey-0.5.1/skysurvey/survey/core.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.3/skysurvey/survey/healpix.py` & `skysurvey-0.5.1/skysurvey/survey/healpix.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,17 +135,17 @@
     # ------- #
     def radec_to_fieldid(self, radec):
         """ get the fieldid of the given (list of) coordinates """
         if type(radec) is pandas.DataFrame:
             ra = np.asarray(radec["ra"].values, dtype="float")
             dec = np.asarray(radec["dec"].values, dtype="float")
         else:
-            ra, dec = np.asarray(radec).T
+            ra, dec = np.asarray(radec)
             
-        return hp.ang2pix(self.nside, dec * np.pi/180,  (90 - ra) * np.pi/180)
+        return hp.ang2pix(self.nside, (90 - ra) * np.pi/180, dec * np.pi/180)
 
     # ------- #
     #  draw   #
     # ------- #    
     def draw_random(self, size, 
                     bands, mjd_range, skynoise_range,
                     gain_range=1, zp_range=25,
```

### Comparing `skysurvey-0.4.3/skysurvey/survey/polygon.py` & `skysurvey-0.5.1/skysurvey/survey/polygon.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.3/skysurvey/survey/ztf.py` & `skysurvey-0.5.1/skysurvey/survey/ztf.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.3/skysurvey/target/collection.py` & `skysurvey-0.5.1/skysurvey/target/collection.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.3/skysurvey/target/core.py` & `skysurvey-0.5.1/skysurvey/target/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         See also
         --------
         from_draw: load the instance by a random draw generation.
         from_setting: loads an instance given model parameters
         """
         import sncosmo
         if type(template) is sncosmo.models.Model: # you provided a sncosmo.model.
-            template = Template.from_sncosmo_model(template) # let's build a skysurvey.Template
+            template = Template.from_sncosmo(template) # let's build a skysurvey.Template
         elif sncosmo.Source in template.__class__.__mro__ or type(template) is str: # you provided a source
             template = Template.from_sncosmo(template) # let's build a skysurvey.Template
         else:
             pass # assume it's a template.
             
         self._template = template
         
@@ -409,15 +409,15 @@
         Say you want to affect 'magobs' with a random gaussian noise of 
         1 +/- 0.1.
         ```
         error_model = {'magobs': {"model": np.random.normal, "param": {'loc':1, 'scale':0.1}}}
         ```
         With that, the 'magobs' columns with be changed and a magobs_err created. 
         """
-        from ..dag import ModelDAG
+        from modeldag import ModelDAG
         if type(error_model) is dict: # assumed to be a model's input
             error_model = ModelDAG(error_model).draw( len(self.data) )
         elif type(error_model) is ModelDAG: # assumed to be a model
             error_model = error_model.draw( len(self.data) )
         # else: dataframe
         
         data_ = self.data.copy()
@@ -545,23 +545,21 @@
         None
 
         See also
         --------
         from_setting: loads an instance given model parameters (dict)
         from_draw: loads and draw random data.
         """
-        from ..dag import ModelDAG
+        from modeldag import ModelDAG
         if type( model ) is dict:
             from copy import deepcopy
             model = ModelDAG(deepcopy(model), self)
             
-        
         self._model = model
 
-
     def set_data(self, data, incl_template=True):
         """ attach data  to this instance. 
 
         Parameters
         ----------
         data: pandas.DataFrame
             dataframe containing (at least) the template
```

### Comparing `skysurvey-0.4.3/skysurvey/target/sncc.py` & `skysurvey-0.5.1/skysurvey/target/sncc.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.3/skysurvey/target/snia.py` & `skysurvey-0.5.1/skysurvey/target/snia.py`

 * *Files 10% similar despite different names*

```diff
@@ -243,73 +243,77 @@
 class SNeIa( Transient ):
 
     _KIND = "SNIa"
     _TEMPLATE = "salt2"
     _RATE = 2.35 * 10**4 # Perley 2020
 
     # {'model': func, 'prop': dict, 'input':, 'as':}
-    _MODEL = dict( redshift = {"param":{"zmax":0.2}, "as":"z"},
+    _MODEL = dict( redshift = {"kwargs": {"zmax":0.2}, "as":"z"},
                               
-                   x1 = {"model": SNeIaStretch.nicolas2021}, 
+                   x1 = {"func": SNeIaStretch.nicolas2021}, 
                    
-                   c = {"model": SNeIaColor.intrinsic_and_dust},
+                   c = {"func": SNeIaColor.intrinsic_and_dust},
 
-                   t0 = {"model": np.random.uniform, 
-                         "param": {"low":56000, "high":57000} },
+                   t0 = {"func": np.random.uniform, 
+                         "kwargs": {"low":56000, "high":57000} },
                        
-                   magabs = {"model": SNeIaMagnitude.tripp1998,
-                             "input": ["x1","c"],
-                             "param": {"mabs":-19.3, "sigmaint":0.10}
+                   magabs = {"func": SNeIaMagnitude.tripp1998,
+                             "kwargs": {"x1": "@x1", "c": "@c",
+                                        "mabs":-19.3, "sigmaint":0.10}
                             },
                            
-                   magobs = {"model": "magabs_to_magobs", # defined in Target (mother of Transients)
-                             "input": ["z", "magabs"]},
+                   magobs = {"func": "magabs_to_magobs", # defined in Target (mother of Transients)
+                             "kwargs": {"z":"@z", "magabs":"@magabs"},
+                            },
 
-                   x0 = {"model": "magobs_to_amplitude", # defined in Transients
-                         "input": ["magobs"],
-                         "param": {"param_name": "x0"}}, #because it needs to call sncosmo_model.get(param_name)
+                   x0 = {"func": "magobs_to_amplitude", # defined in Transients
+                         "kwargs": {"magobs":"@magobs", "param_name": "x0"},
+                        }, #because it needs to call sncosmo_model.get(param_name)
                        
-                   radec = {"model": "random",
-                            "param": dict(ra_range=[0, 360], dec_range=[-30, 90]),
-                            "as": ["ra","dec"]}
+                   radec = {"func": "random",
+                            "kwargs": {"ra_range":[0, 360], "dec_range":[-30, 90]},
+                            "as": ["ra","dec"]
+                           }
                     )
 
 
 class SNeIaHostMass( Transient ):
     
     _KIND = "SNIa"
     _TEMPLATE = "salt2"
     _RATE = 2.35 * 10**4 # Perley 2020
 
-    # {'model': func, 'prop': dict, 'input':, 'as':}
-    _MODEL = dict( redshift = {"param":{"zmax":0.2}, "as":"z"},
+    # {'func': func, 'prop': dict, 'input':, 'as':}
+    _MODEL = dict( redshift = {"param":{"zmax":0.2},
+                                  "as":"z"},
                               
-                   x1 = {"model": SNeIaStretch.nicolas2021}, 
+                   x1 = {"func": SNeIaStretch.nicolas2021}, 
                    
-                   c = {"model": SNeIaColor.intrinsic_and_dust},
+                   c = {"func": SNeIaColor.intrinsic_and_dust},
 
-                   hostmass = {"model": getpdf_asymetric_gaussian},
+                   hostmass = {"func": getpdf_asymetric_gaussian},
 
-                   t0 = {"model": np.random.uniform, 
-                         "param": {"low":56000, "high":57000} },
+                   t0 = {"func": np.random.uniform, 
+                         "kwargs": {"low":56000, "high":57000} },
                        
-                   magabs = {"model": SNeIaMagnitude.tripp_and_massstep,
-                             "input": ["x1","c", "hostmass"],
-                             "param": {"mabs":-19.3, "sigmaint":0.10, "split":10}
+                   magabs = {"func": SNeIaMagnitude.tripp_and_massstep,
+                             "kwargs": { "x1": "@x1", "c": "@c", "hostmass": "@hostmass",
+                                        "mabs":-19.3, "sigmaint":0.10, "split":10}
                             },
                            
-                   magobs = {"model": "magabs_to_magobs", # defined in Target (mother of Transients)
-                             "input": ["z", "magabs"]},
-
-                   x0 = {"model": "magobs_to_amplitude", # defined in Transients
-                         "input": ["magobs"],
-                         "param": {"param_name":"x0"}}, #because it needs to call sncosmo_model.get(param_name)
+                   magobs = {"func": "magabs_to_magobs", # defined in Target (mother of Transients)
+                             "kwargs": {"z":"@z", "magabs":"@magabs"},
+                             },
+
+                   x0 = {"func": "magobs_to_amplitude", # defined in Transients
+                         "kwargs": {"magobs": "@magobs", "param_name":"x0"}
+                        }, #because it needs to call sncosmo_model.get(param_name)
                        
-                   radec = {"model": "random",
-                            "param": dict(ra_range=[0, 360], dec_range=[-30, 90]),
+                   radec = {"func": "random",
+                            "kwargs": dict(ra_range=[0, 360], dec_range=[-30, 90]),
                             "as": ["ra","dec"]}
                     )
```

### Comparing `skysurvey-0.4.3/skysurvey/target/stars.py` & `skysurvey-0.5.1/skysurvey/target/stars.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 
 
 
 class StableTarget( Target ):
     
     _KIND = "stable"
-    _MODEL = dict( radec = {"model":"random",
-                                "param":dict(ra_range=[0, 360], dec_range=[-30, 90]),
+    _MODEL = dict( radec = {"func":"random",
+                                "kwargs":dict(ra_range=[0, 360], dec_range=[-30, 90]),
                                 "as":["ra","dec"]},
-                    magobs = {"model": "random_magobs",
-                                "param": dict(zpmax=22.5)},
+                    magobs = {"func": "random_magobs",
+                                "kwargs": dict(zpmax=22.5)},
                    )
     
     @staticmethod
     def random_magobs(size=None, zpmax=22.5, scale=3):
         """ """
         exp_decay = np.random.exponential(scale=scale, size=size)
         return zpmax-exp_decay
```

### Comparing `skysurvey-0.4.3/skysurvey/target/timeserie.py` & `skysurvey-0.5.1/skysurvey/target/timeserie.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,30 +12,35 @@
 
     Example
     -------
     >>> snii = TSTransient.from_draw("snana-2004fe", 4000)
     >>> _ = snii.show_lightcurve(["ztfg","ztfr"], index=10, in_mag=True)
     """
     
-    _MODEL = dict( redshift = {"param": {"zmax": 0.05}, 
+    _MODEL = dict( redshift = {"kwargs": {"zmax": 0.05}, 
                                "as": "z"},
-                   t0 = {"model": np.random.uniform,
-                         "param": {"low": 56000, "high": 56000+4*365}},
+                   t0 = {"func": np.random.uniform,
+                         "kwargs": {"low": 56000, "high": 56000+4*365}
+                        },
                          
-                   magabs = {"model": np.random.normal,
-                             "param": {"loc": -18, "scale": 1}},
+                   magabs = {"func": np.random.normal,
+                             "kwargs": {"loc": -18, "scale": 1}
+                            },
                              
-                   magobs = {"model": "magabs_to_magobs",
-                               "input": ["z", "magabs"]},
+                   magobs = {"func": "magabs_to_magobs",
+                             "kwargs": {"z":"@z", "magabs": "@magabs"}
+                            },
                                
-                   amplitude = {"model": "magobs_to_amplitude",
-                                "input": ["magobs"]},
+                   amplitude = {"func": "magobs_to_amplitude",
+                                "kwargs": {"magobs": "@magobs"}
+                            },
                    # This you need to match with the survey
-                   radec={"model": "random",
-                          "as": ["ra","dec"]}
+                   radec = {"func": "random",
+                            "as": ["ra","dec"]
+                            }
                  )
     
     @classmethod
     def from_sncosmo(cls, source, rate=1e3, model=None,
                                 magabs=None, magscatter=None):
         """ loads an instance from a sncosmo TimeSeriesSource source
         (see https://sncosmo.readthedocs.io/en/stable/source-list.html#list-of-built-in-sources)
```

### Comparing `skysurvey-0.4.3/skysurvey/template.py` & `skysurvey-0.5.1/skysurvey/template.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.3/skysurvey.egg-info/SOURCES.txt` & `skysurvey-0.5.1/skysurvey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

