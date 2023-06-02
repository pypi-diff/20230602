# Comparing `tmp/pyrsig-0.4.0.tar.gz` & `tmp/pyrsig-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrsig-0.4.0.tar", last modified: Wed May 31 14:53:41 2023, max compression
+gzip compressed data, was "dist/pyrsig-0.4.1.tar", last modified: Fri Jun  2 18:50:23 2023, max compression
```

## Comparing `pyrsig-0.4.0.tar` & `pyrsig-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-31 14:53:41.000000 pyrsig-0.4.0/
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.0/setup.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-05-31 14:53:41.000000 pyrsig-0.4.0/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.0/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-31 14:53:41.000000 pyrsig-0.4.0/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/requires.txt
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-31 14:53:41.000000 pyrsig-0.4.0/pyrsig/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-31 14:53:41.000000 pyrsig-0.4.0/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.0/pyrsig/tests/test_api.py
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.0/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2058 2023-03-29 20:31:50.000000 pyrsig-0.4.0/pyrsig/tests/test_ioapi.py
--rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.0/pyrsig/tests/test_misc.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.4.0/pyrsig/tests/test_dataframes.py
--rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.0/pyrsig/tests/test_coards.py
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.0/pyrsig/tests/test_gui.py
--rw-r--r--   0 bhenders (83225) romo       (131)    46992 2023-05-31 14:29:01.000000 pyrsig-0.4.0/pyrsig/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-05-31 14:53:41.000000 pyrsig-0.4.0/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.0/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 18:50:23.000000 pyrsig-0.4.1/
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.1/setup.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-02 18:50:23.000000 pyrsig-0.4.1/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.1/LICENSE
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/requires.txt
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig/
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.1/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.1/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2058 2023-03-29 20:31:50.000000 pyrsig-0.4.1/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.1/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.4.1/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.1/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.1/pyrsig/tests/test_gui.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    47800 2023-06-02 18:49:39.000000 pyrsig-0.4.1/pyrsig/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-06-02 18:50:23.000000 pyrsig-0.4.1/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.1/README.md
```

### Comparing `pyrsig-0.4.0/setup.py` & `pyrsig-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.0/PKG-INFO` & `pyrsig-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.0/LICENSE` & `pyrsig-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.0/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.4.1/pyrsig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.0/pyrsig/tests/test_api.py` & `pyrsig-0.4.1/pyrsig/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.0/pyrsig/tests/test_ioapi.py` & `pyrsig-0.4.1/pyrsig/tests/test_ioapi.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.0/pyrsig/tests/test_dataframes.py` & `pyrsig-0.4.1/pyrsig/tests/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.0/pyrsig/tests/test_coards.py` & `pyrsig-0.4.1/pyrsig/tests/test_coards.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.0/pyrsig/tests/test_gui.py` & `pyrsig-0.4.1/pyrsig/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.0/pyrsig/__init__.py` & `pyrsig-0.4.1/pyrsig/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = ['RsigApi', 'RsigGui', 'open_ioapi']
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 
 import pandas as pd
 
 
 _def_grid_kw = {
     '12US1': dict(
         GDNAM='12US1', GDTYP=2, NCOLS=459, NROWS=299,
@@ -338,17 +338,23 @@
         projstr = (
             '+proj=lcc +lat_1={P_ALP} +lat_2={P_BET} +lat_0={YCENT}'
             ' +lon_0={XCENT} +R={earth_radius} +x_0={x_0} +y_0={y_0}'
             ' +to_meter={XCELL} +no_defs'
         ).format(**props)
     elif props['GDTYP'] == 6:
         projstr = (
-            '+proj=stere +lat_0={P_ALP * 90} +lat_ts={P_BET} +lon_0={XCENT} '
-            + '+x_0={x_0} +y_0={y_0} +R={earth_radius} +to_meter={XCELL} '
-            + '+no_defs'
+            '+proj=stere +lat_0={lat_0} +lat_ts={P_BET} +lon_0={XCENT}'
+            + ' +x_0={x_0} +y_0={y_0} +R={earth_radius} +to_meter={XCELL}'
+            + ' +no_defs'
+        ).format(lat_0=props['P_ALP'] * 90, **props)
+    elif props['GDTYP'] == 7:
+        projstr = (
+            '+proj=merc +R={earth_radius} +lat_ts=0 +lon_0={XORIG}'
+            + ' +x_0={x_0} +y_0={y_0} +to_meter={XCELL}'
+            + ' +no_defs'
         ).format(**props)
     else:
         raise ValueError('GDTYPE {GDTYP} not implemented'.format(**props))
 
     return projstr
 
 
@@ -559,15 +565,15 @@
 
         if bbox is None:
             self.bbox = (-126, 24, -66, 50)
         else:
             self.bbox = bbox
         if bdate is None:
             bdate = (
-                pd.to_datetime('now') - pd.to_timedelta('1day')
+                pd.to_datetime('now', utc=True) - pd.to_timedelta('1day')
             ).replace(hour=0, minute=0, second=0, microsecond=0, nanosecond=0)
 
         self.bdate = pd.to_datetime(bdate)
         if edate is None:
             self.edate = edate
         else:
             self.edate = pd.to_datetime(edate)
@@ -601,14 +607,31 @@
                 'out_in_flag': 0, 'freq': 'hourly',
                 'maximum_difference': 5, 'maximum_ratio': 0.70,
                 'agg_pct': 75, 'api_key': '<your key here>'
             }
 
         self.purpleair_kw = purpleair_kw
 
+    def resize_grid(self, clip=True):
+        """
+        Update grid_kw property so that it only covers the bbox by adjusting
+        the XORIG, YORIG, NCOLS and NROWS. If clip is True, this has the affect
+        of reducing the number of rows and columns. This is useful when the
+        area of interest is much smaller than the grid defined in grid_kw.
+
+        Arguments
+        ---------
+        clip : bool
+
+        Returns
+        -------
+        None
+        """
+        self.grid_kw = customize_grid(self.grid_kw, self.bbox, clip=clip)
+
     def describe(self, key, as_dataframe=True, raw=False):
         """
         describe returns details about the coverage specified by key. Details
         include spatial bounding box, time coverage, time resolution, variable
         label, and a short description.
 
         DescribeCoverage with a COVERAGE should be faster than descriptions
@@ -636,14 +659,15 @@
             print(df.to_csv())
             # ,name,label,description,bbox_str,beginPosition,timeResolution
             # 0,no2,no2(ppb),UTC hourly mean surface measured nitrogen ...,
             # ... -157 21 -51 64,2003-01-02T00:00:00Z,PT1H
         """
         import requests
         import warnings
+
         if key not in self._description:
             r = requests.get(
                 f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
                 f'1.0.0&REQUEST=DescribeCoverage&COVERAGE={key}&compress=1'
             )
             self._description[key] = r.text
```

### Comparing `pyrsig-0.4.0/README.md` & `pyrsig-0.4.1/README.md`

 * *Files identical despite different names*

