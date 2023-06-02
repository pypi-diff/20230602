# Comparing `tmp/pyrsig-0.4.1.tar.gz` & `tmp/pyrsig-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrsig-0.4.1.tar", last modified: Fri Jun  2 18:50:23 2023, max compression
+gzip compressed data, was "dist/pyrsig-0.4.2.tar", last modified: Fri Jun  2 19:11:47 2023, max compression
```

## Comparing `pyrsig-0.4.1.tar` & `pyrsig-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 18:50:23.000000 pyrsig-0.4.1/
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.1/setup.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-02 18:50:23.000000 pyrsig-0.4.1/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.1/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig.egg-info/requires.txt
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 18:50:23.000000 pyrsig-0.4.1/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.1/pyrsig/tests/test_api.py
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.1/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2058 2023-03-29 20:31:50.000000 pyrsig-0.4.1/pyrsig/tests/test_ioapi.py
--rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.1/pyrsig/tests/test_misc.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.4.1/pyrsig/tests/test_dataframes.py
--rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.1/pyrsig/tests/test_coards.py
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.1/pyrsig/tests/test_gui.py
--rw-r--r--   0 bhenders (83225) romo       (131)    47800 2023-06-02 18:49:39.000000 pyrsig-0.4.1/pyrsig/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-06-02 18:50:23.000000 pyrsig-0.4.1/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.1/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 19:11:47.000000 pyrsig-0.4.2/
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.2/setup.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-02 19:11:47.000000 pyrsig-0.4.2/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.2/LICENSE
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig.egg-info/requires.txt
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig/
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-02 19:11:47.000000 pyrsig-0.4.2/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.2/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.2/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2450 2023-06-02 19:05:44.000000 pyrsig-0.4.2/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.2/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.4.2/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.2/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.2/pyrsig/tests/test_gui.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    47853 2023-06-02 19:11:29.000000 pyrsig-0.4.2/pyrsig/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-06-02 19:11:47.000000 pyrsig-0.4.2/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.2/README.md
```

### Comparing `pyrsig-0.4.1/setup.py` & `pyrsig-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.1/PKG-INFO` & `pyrsig-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.1/LICENSE` & `pyrsig-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.1/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.4.2/pyrsig.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.1/pyrsig/tests/test_api.py` & `pyrsig-0.4.2/pyrsig/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.1/pyrsig/tests/test_ioapi.py` & `pyrsig-0.4.2/pyrsig/tests/test_ioapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,29 @@
         )
         ds = rsigapi.to_ioapi(
             'tropomi.offl.no2.nitrogendioxide_tropospheric_column'
         )
         print(ds.dims)
 
 
+def test_tropomi_stereo():
+    from .. import RsigApi
+    import tempfile
+
+    with tempfile.TemporaryDirectory() as td:
+        rsigapi = RsigApi(
+            bdate='2022-03-01', workdir=td,
+            bbox=(-97, 20, -65, 50), grid_kw='108NHEMI2'
+        )
+        ds = rsigapi.to_ioapi(
+            'tropomi.offl.no2.nitrogendioxide_tropospheric_column'
+        )
+        print(ds.dims)
+
+
 def test_tropomi_cache():
     from .. import RsigApi
     import tempfile
 
     with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
             bdate='2022-03-01', workdir=td,
```

### Comparing `pyrsig-0.4.1/pyrsig/tests/test_dataframes.py` & `pyrsig-0.4.2/pyrsig/tests/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.1/pyrsig/tests/test_coards.py` & `pyrsig-0.4.2/pyrsig/tests/test_coards.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.1/pyrsig/tests/test_gui.py` & `pyrsig-0.4.2/pyrsig/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.1/pyrsig/__init__.py` & `pyrsig-0.4.2/pyrsig/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = ['RsigApi', 'RsigGui', 'open_ioapi']
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 
 import pandas as pd
 
 
 _def_grid_kw = {
     '12US1': dict(
         GDNAM='12US1', GDTYP=2, NCOLS=459, NROWS=299,
@@ -1023,30 +1023,33 @@
 
     def _build_grid(self, grid_kw):
         """
         Build the regrid portion of the URL
 
         """
         grid_kw.setdefault('earth_radius', 6370000)
-        if grid_kw.get('GDTYP', 2) == 2:
-            gridstr = (
-                '&REGRID=weighted'
-                '&LAMBERT={P_ALP},{P_BET},{XCENT},{YCENT}'
-                '&ELLIPSOID={earth_radius},{earth_radius}'
-                '&GRID={NCOLS},{NROWS},{XORIG},{YORIG},{XCELL},{YCELL}'
-            ).format(**grid_kw)
-            if grid_kw.get('REGRID_AGGREGATE', 'None').strip() != 'None':
-                gridstr += (
-                    "&REGRID_AGGREGATE={REGRID_AGGREGATE}".format(**grid_kw)
-                )
-
-            return gridstr
+        GDTYP = grid_kw.get('GDTYP', 2)
+        if GDTYP == 2:
+            projstr = '&LAMBERT={P_ALP},{P_BET},{XCENT},{YCENT}'
+        elif GDTYP == 6:
+            projstr = '&STEREOGRAPHIC={XCENT},{YCENT},{P_BET}'
         else:
             raise KeyError('GDTYP only implemented for ')
 
+        gridstr = (
+            '&REGRID=weighted'
+            + projstr
+            + '&ELLIPSOID={earth_radius},{earth_radius}'
+            + '&GRID={NCOLS},{NROWS},{XORIG},{YORIG},{XCELL},{YCELL}'
+        )
+        if grid_kw.get('REGRID_AGGREGATE', 'None').strip() != 'None':
+            gridstr += "&REGRID_AGGREGATE={REGRID_AGGREGATE}"
+
+        return gridstr.format(**grid_kw)
+
     def to_dataframe(
         self, key=None, bdate=None, edate=None, bbox=None, unit_keys=True,
         parse_dates=False, withmeta=False, verbose=0
     ):
         """
         All arguments default to those provided during initialization.
```

### Comparing `pyrsig-0.4.1/README.md` & `pyrsig-0.4.2/README.md`

 * *Files identical despite different names*

