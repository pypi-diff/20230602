# Comparing `tmp/psdist-0.1.4.tar.gz` & `tmp/psdist-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdist-0.1.4.tar", last modified: Wed May 24 17:51:17 2023, max compression
+gzip compressed data, was "psdist-0.1.5.tar", last modified: Fri Jun  2 17:04:59 2023, max compression
```

## Comparing `psdist-0.1.4.tar` & `psdist-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-05-24 17:51:17.387772 psdist-0.1.4/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.4/LICENSE
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1160 2023-05-24 17:51:17.387656 psdist-0.1.4/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      702 2023-03-07 19:34:27.000000 psdist-0.1.4/README.md
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-05-24 17:51:17.385944 psdist-0.1.4/psdist/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.4/psdist/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.4/psdist/ap.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    12828 2023-05-24 15:50:44.000000 psdist-0.1.4/psdist/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.4/psdist/data.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    17668 2023-05-24 15:50:44.000000 psdist-0.1.4/psdist/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       53 2023-05-24 15:51:53.000000 psdist-0.1.4/psdist/sampling.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1344 2023-03-02 16:46:32.000000 psdist-0.1.4/psdist/utils.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-05-24 17:51:17.387468 psdist-0.1.4/psdist/visualization/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.4/psdist/visualization/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    14912 2023-05-24 17:16:25.000000 psdist-0.1.4/psdist/visualization/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    36316 2023-05-24 15:50:44.000000 psdist-0.1.4/psdist/visualization/grid.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22492 2023-05-24 15:50:44.000000 psdist-0.1.4/psdist/visualization/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.4/psdist/visualization/visualization.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-05-24 17:51:17.386656 psdist-0.1.4/psdist.egg-info/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1160 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      455 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/SOURCES.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/dependency_links.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/requires.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/top_level.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-05-24 17:50:13.000000 psdist-0.1.4/pyproject.toml
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-05-24 17:51:17.387809 psdist-0.1.4/setup.cfg
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-02 17:04:59.648864 psdist-0.1.5/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.5/LICENSE
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1245 2023-06-02 17:04:59.648720 psdist-0.1.5/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      787 2023-06-02 12:53:27.000000 psdist-0.1.5/README.md
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-02 17:04:59.646177 psdist-0.1.5/psdist/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.5/psdist/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.5/psdist/ap.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    12828 2023-06-02 13:20:42.000000 psdist-0.1.5/psdist/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.5/psdist/data.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    18125 2023-06-02 16:02:32.000000 psdist-0.1.5/psdist/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       53 2023-05-24 15:51:53.000000 psdist-0.1.5/psdist/sampling.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1344 2023-03-02 16:46:32.000000 psdist-0.1.5/psdist/utils.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-02 17:04:59.648361 psdist-0.1.5/psdist/visualization/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.5/psdist/visualization/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    16217 2023-06-02 16:55:39.000000 psdist-0.1.5/psdist/visualization/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    36316 2023-05-24 15:50:44.000000 psdist-0.1.5/psdist/visualization/grid.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22591 2023-06-02 17:03:58.000000 psdist-0.1.5/psdist/visualization/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.5/psdist/visualization/visualization.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-02 17:04:59.647091 psdist-0.1.5/psdist.egg-info/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1245 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      455 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/SOURCES.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/dependency_links.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/requires.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/top_level.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-06-02 17:03:41.000000 psdist-0.1.5/pyproject.toml
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-06-02 17:04:59.648914 psdist-0.1.5/setup.cfg
```

### Comparing `psdist-0.1.4/LICENSE` & `psdist-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psdist-0.1.4/PKG-INFO` & `psdist-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: psdist
-Version: 0.1.4
+Version: 0.1.5
 Summary: Analysis/visualization of phase space distributions
 Author-email: Austin Hoover <ahoover1218@gmail.com>
 Project-URL: homepage, https://github.com/austin-hoover/psdist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psdist
 
-This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions.
+This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions. Most of the methods should work for point-cloud or image data of any dimensionality.
 
 
 ## Installation
 
 https://pypi.org/project/psdist/
```

### Comparing `psdist-0.1.4/README.md` & `psdist-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # psdist
 
-This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions.
+This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions. Most of the methods should work for point-cloud or image data of any dimensionality.
 
 
 ## Installation
 
 https://pypi.org/project/psdist/
```

### Comparing `psdist-0.1.4/psdist/ap.py` & `psdist-0.1.5/psdist/ap.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.4/psdist/cloud.py` & `psdist-0.1.5/psdist/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
             center = np.full(d, center)
         if not array_like(width):
             width = np.full(d, width)
         center = np.array(center)
         width = np.array(width)
         limits = list(zip(center - 0.5 * width, center + 0.5 * width))  
     limits = np.array(limits)
-    if limits.ndim == 0:
+    if limits.ndim == 1:
         limits = limits[None, :]
     conditions = []
     for j, (umin, umax) in zip(axis, limits):
         conditions.append(X[:, j] > umin)
         conditions.append(X[:, j] < umax)
     idx = np.logical_and.reduce(conditions)
     return X[idx, :]
```

### Comparing `psdist-0.1.4/psdist/data.py` & `psdist-0.1.5/psdist/data.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.4/psdist/image.py` & `psdist-0.1.5/psdist/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,59 +455,76 @@
         if copy:
             return np.broadcast_to(f, new_shape).copy()
         else:
             return np.broadcast_to(f, new_shape)
     return None
 
 
-def _normalize(f, norm="volume", pixel_volume=1.0):
+# Processing
+
+def blur(f, sigma):
+    """Simple Gaussian blur."""
+    return ndimage.gaussian_filter(f, sigma)
+
+
+def clip(f, lmin=None, lmax=None, frac=False):
+    """Clip between lmin and lmax, can be fractions or absolute values."""
+    if not (lmin or lmax):
+        return f
+    if frac:
+        f_max = np.max(f)
+        if lmin:
+            lmin = f_max * lmin
+        if lmax:
+            lmax = f_max * lmax
+    return np.clip(f, lmin, lmax)
+
+
+def fill(f, fill_value=None):
+    """Fill masked values."""
+    return np.ma.filled(f, fill_value=fill_value)
+
+
+def normalize(f, norm="volume", pixel_volume=1.0):
+    """Scale to unit volume or unit maximum."""
     factor = 1.0
     if norm == "volume":
         factor = np.sum(f) * pixel_volume
     elif norm == "max":
         factor = np.max(f)
     if factor == 0.0:
         return f
     return f / factor
 
 
-def _threshold(f, lmin=None, frac=False):
+def threshold(f, lmin=None, frac=False):
+    """Set pixels less than lmin to zero."""
     if lmin:
         if frac:
             f_max = np.max(f)
             lmin = lmin * f_max
         f[f < lmin] = 0.0
     return f
 
 
-def _clip(f, lmin=None, lmax=None, frac=False):
-    if not (lmin or lmax):
-        return f
-    if frac:
-        f_max = np.max(f)
-        if lmin:
-            lmin = f_max * lmin
-        if lmax:
-            lmax = f_max * lmax
-    return np.clip(f, lmin, lmax)
-
-
 def process(
     f,
     fill_value=None,
     thresh=None,
     thresh_type="abs",
     clip=None,
     clip_type="abs",
     norm=None,
     pixel_volume=1.0,
-    blur=0.0,
+    blur_sigma=None,
 ):
     """Return processed image.
 
+    This is a convenience function mostly for plotting routines.
+
     Parameters
     ----------
     f : ndarray
         A two-dimensional image.
     fill_value : float
         Fill masked elements of `f` with this value.
     mask_nonpositive : bool
@@ -519,27 +536,27 @@
     thresh_type, clip_type : {'abs', 'frac'}
         Whether `thresh` and `clip` refer to absolute values or fractions
         of the maximum element of `f`.
     norm : {None, 'max', 'volume'}
         Whether to normalize the image by its volume or maximum element.
     pixel_volume : float
         Needed if normalizing by volume.
-    blur : float
+    blur_sigma : float
         Sigma for Gaussian filter.
     """
     if fill_value is not None:
-        f = np.ma.filled(f, fill_value=fill_value)
+        f = fill(f, fill_value=None)
     if thresh is not None:
-        f = _threshold(f, thresh, frac=(thresh_type == "frac"))
+        f = threshold(f, thresh, frac=(thresh_type == "frac"))
     if clip is not None:
-        f = _clip(f, clip[0], clip[1], frac=(clip_type == "frac"))
-    if blur:
-        f = ndimage.gaussian_filter(f, blur)
+        f = clip(f, clip[0], clip[1], frac=(clip_type == "frac"))
+    if blur_sigma is not None:
+        f = blur(f, blur_sigma)
     if norm:
-        f = _normalize(f, norm=norm, pixel_volume=pixel_volume)
+        f = normalize(f, norm=norm, pixel_volume=pixel_volume)
     return f
 
 
 # Sampling
 # ------------------------------------------------------------------------------
```

### Comparing `psdist-0.1.4/psdist/utils.py` & `psdist-0.1.5/psdist/utils.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.4/psdist/visualization/cloud.py` & `psdist-0.1.5/psdist/visualization/cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Plotting routines for point clouds."""
+"""Plotting routines for point data."""
 from ipywidgets import interactive
 from ipywidgets import widgets
 from matplotlib import pyplot as plt
 import numpy as np
 import proplot as pplt
 
 import psdist.cloud
@@ -284,178 +284,213 @@
         diag_kws=diag_kws,
         **kws,
     )
     return grid
 
 
 def proj2d_interactive_slice(
-    X,
+    data=None,
     limits=None,
-    nbins=30,
     default_ind=(0, 1),
     slice_type="int",
     dims=None,
     units=None,
+    autolim_kws=None,
+    fig_kws=None,
     **plot_kws,
 ):
-    """2D partial projection of bunch with interactive slicing.
+    """2D partial projection with interactive slicing.
 
     Parameters
     ----------
-    X : ndarray, shape (n, d)
-        Coordinates of n points in d-dimensional space.
+    data : ndarray, shape (n, d) or list[ndarray, shape (n, d)]
+        Coordinates of n points in d-dimensional space. Alternatively, a list of k 
+        data sets can be provided. This will generate k figures, allowing side-by-side
+        comparision. There is no limit on the number of figures!
     limits : list[(min, max)]
         Limits along each axis.
-    nbins : int
-        Default number of bins for slicing/viewing. Both can be changed with
-        sliders.
     default_ind : (i, j)
         Default view axis.
     slice_type : {'int', 'range'}
         Whether to slice one index along the axis or a range of indices.
     dims, units : list[str], shape (n,)
         Dimension names and units.
+    autolim_kws : dict
+        Key word arguments passed to `auto_limits`.
+    fig_kws : dict
+        Key word arguments passed to `proplot.subplots`.
     **plot_kws
         Key word arguments passed to `plot2d`.
     """
-    plot_kws.setdefault("kind", "hist")
+    if np.ndim(data) == 2:
+        data = [data]
+    n_data = len(data)
+    n_dims = data[0].shape[1]
+    for i in range(1, n_data):
+        if data[i].shape[1] != n_dims:
+            raise ValueError("data must have the same number of dimensions.")
+
+    if fig_kws is None:
+        fig_kws = dict()
+    plot_kws.setdefault("kind", "hist")    
+
     if limits is None:
-        limits = [(np.min(X[:, i]), np.max(X[:, i])) for i in range(X.shape[1])]
+        if autolim_kws is None:
+            autolim_kws = dict()
+        limits_list = np.array([auto_limits(X, **autolim_kws) for X in data])
+        mins = np.min(limits_list[:, :, 0], axis=0)   
+        maxs = np.max(limits_list[:, :, 1], axis=0)
+        # mins = np.min([np.min(X, axis=0) for X in data], axis=0)
+        # maxs = np.max([np.max(X, axis=0) for X in data], axis=0)
+        limits = [(mins[i], maxs[i]) for i in range(n_dims)]
     if dims is None:
-        dims = [f"x{i + 1}" for i in range(X.shape[1])]
+        dims = [f"x{i + 1}" for i in range(n_dims)]
     if units is None:
-        units = X.shape[1] * [""]
+        units = n_dims * [""]
     dims_units = []
     for dim, unit in zip(dims, units):
         dims_units.append(f"{dim}" + f" [{unit}]" if unit != "" else dim)
 
     # Widgets
-    nbins_default = nbins
     dim1 = widgets.Dropdown(options=dims, index=default_ind[0], description="dim 1")
     dim2 = widgets.Dropdown(options=dims, index=default_ind[1], description="dim 2")
-    nbins = widgets.IntSlider(
-        min=2, max=100, value=nbins_default, description="grid res"
-    )
-    nbins_plot = widgets.IntSlider(
-        min=2, max=200, value=nbins_default, description="plot res"
-    )
+    n_bins = widgets.BoundedIntText(
+        value=32,
+        min=2,
+        max=150,
+        step=1,
+        description="slice res",
+    )    
+    n_bins_plot = widgets.BoundedIntText(
+        value=50,
+        min=2,
+        max=250,
+        step=1,
+        description="plot res",
+    )    
     autobin = widgets.Checkbox(description="auto plot res", value=False)
     log = widgets.Checkbox(description="log", value=False)
     sliders, checks = [], []
-    for k in range(X.shape[1]):
+    for k in range(n_dims):
         if slice_type == "int":
             slider = widgets.IntSlider(
                 min=0,
-                max=100,
-                value=0,
+                max=(n_bins.value - 1),
+                value=int(n_bins.value / 2),
                 description=dims[k],
                 continuous_update=True,
             )
         elif slice_type == "range":
             slider = widgets.IntRangeSlider(
-                value=(0, 100),
                 min=0,
-                max=100,
+                max=(n_bins.value - 1),
+                value=(0, n_bins.value - 1),
                 description=dims[k],
                 continuous_update=True,
             )
         else:
             raise ValueError("Invalid `slice_type`.")
         slider.layout.display = "none"
         sliders.append(slider)
         checks.append(widgets.Checkbox(description=f"slice {dims[k]}"))
 
     def hide(button):
         """Hide inactive sliders."""
-        for k in range(X.shape[1]):
+        for k in range(n_dims):
             # Hide elements for dimensions being plotted.
             valid = dims[k] not in (dim1.value, dim2.value)
             disp = None if valid else "none"
             for element in [sliders[k], checks[k]]:
                 element.layout.display = disp
             # Uncheck boxes for dimensions being plotted.
             if not valid and checks[k].value:
                 checks[k].value = False
             # Make sliders respond to check boxes.
             if not checks[k].value:
                 sliders[k].layout.display = "none"
-            nbins_plot.layout.display = "none" if autobin.value else None
+            n_bins_plot.layout.display = "none" if autobin.value else None
 
     # Make slider visiblity depend on checkmarks.
     for element in (dim1, dim2, *checks, autobin):
         element.observe(hide, names="value")
 
     # Initial hide
-    nbins_plot.layout.display = "none"
-    for k in range(X.shape[1]):
+    for k in range(n_dims):
         if k in default_ind:
             checks[k].layout.display = "none"
             sliders[k].layout.display = "none"
 
     def update(**kws):
         dim1 = kws["dim1"]
         dim2 = kws["dim2"]
-        nbins = kws["nbins"]
-        nbins_plot = kws["nbins_plot"]
+        n_bins = kws["n_bins"]
+        n_bins_plot = kws["n_bins_plot"]
         autobin = kws["autobin"]
+
+        # Update the slider ranges based on n_bins.
+        for slider in sliders:
+            slider.max = n_bins - 1
+
+        # Collect slice indices.
         ind, checks = [], []
-        for i in range(100):
+        for i in range(1, n_dims + 1):
             if f"check{i}" in kws:
                 checks.append(kws[f"check{i}"])
             if f"slider{i}" in kws:
                 _ind = kws[f"slider{i}"]
                 if type(_ind) is int:
                     _ind = (_ind, _ind + 1)
                 ind.append(_ind)
 
         # Exit if input does not make sense.
         for dim, check in zip(dims, checks):
             if check and dim in (dim1, dim2):
                 return
         if dim1 == dim2:
-            return
+            return     
 
-        # Slice the distribution
+        # Slice the distributions.
         axis_view = [dims.index(dim) for dim in (dim1, dim2)]
         axis_slice = [dims.index(dim) for dim, check in zip(dims, checks) if check]
-        edges = [np.linspace(umin, umax, nbins + 1) for (umin, umax) in limits]
-        if axis_slice:
-            center, width = [], []
+        edges = [np.linspace(limits[i][0], limits[i][1], n_bins + 1) for i in range(n_dims)]        
+        _data = []
+        if not axis_slice:
+            _data = data
+        else:
+            slice_limits = []
             for k in axis_slice:
                 imin, imax = ind[k]
                 if imax > len(edges[k]) - 1:
                     print(f"{dims[k]} out of range.")
                     return
-                width.append(edges[k][imax] - edges[k][imin])
-                center.append(0.5 * (edges[k][imax] + edges[k][imin]))
-            _X = psdist.cloud.slice_planar(
-                X, axis=axis_slice, center=center, width=width
-            )
-        else:
-            _X = X[:, :]
-        if _X.shape[0] == 0:
-            return
+                slice_limits.append((edges[k][imin], edges[k][imax]))
+            _data = [psdist.cloud.slice_planar(X, axis=axis_slice, limits=slice_limits) for X in data]
+        for _X in _data:
+            if _X.shape[0] == 0:
+                return
 
         # Update plotting key word arguments.
         if plot_kws["kind"] != "scatter":
-            plot_kws["bins"] = "auto" if autobin else nbins_plot
+            plot_kws["bins"] = "auto" if autobin else n_bins_plot
             plot_kws["limits"] = [limits[axis_view[0]], limits[axis_view[1]]]
             plot_kws["norm"] = "log" if kws["log"] else None
 
         # Plot the selected points.
-        fig, ax = pplt.subplots()
-        plot2d(_X[:, axis_view], ax=ax, **plot_kws)
-        ax.format(xlabel=dims_units[axis_view[0]], ylabel=dims_units[axis_view[1]])
+        fig, axs = pplt.subplots(ncols=n_data, **fig_kws)
+        for ax, _X in zip(axs, _data):
+            plot2d(_X[:, axis_view], ax=ax, **plot_kws)
+        axs.format(xlabel=dims_units[axis_view[0]], ylabel=dims_units[axis_view[1]])
         plt.show()
 
+    # Pass key word arguments to `ipywidgets.interactive`.
     kws = dict()
     kws["log"] = log
     kws["autobin"] = autobin
+    kws["n_bins"] = n_bins
+    kws["n_bins_plot"] = n_bins_plot
     kws["dim1"] = dim1
     kws["dim2"] = dim2
     for i, check in enumerate(checks, start=1):
         kws[f"check{i}"] = check
     for i, slider in enumerate(sliders, start=1):
         kws[f"slider{i}"] = slider
-    kws["nbins"] = nbins
-    kws["nbins_plot"] = nbins_plot
     return interactive(update, **kws)
```

### Comparing `psdist-0.1.4/psdist/visualization/grid.py` & `psdist-0.1.5/psdist/visualization/grid.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.4/psdist/visualization/image.py` & `psdist-0.1.5/psdist/visualization/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,40 +494,44 @@
         dim1, dim2 = kws["dim1"], kws["dim2"]
         ind, checks = [], []
         for i in range(100):
             if f"check{i}" in kws:
                 checks.append(kws[f"check{i}"])
             if f"slider{i}" in kws:
                 ind.append(kws[f"slider{i}"])
+                
         # Return nothing if input does not make sense.
         for dim, check in zip(dims, checks):
             if check and dim in (dim1, dim2):
                 return
         if dim1 == dim2:
             return
+            
         # Slice and project the distribution.
         axis_view = [dims.index(dim) for dim in (dim1, dim2)]
         axis_slice = [dims.index(dim) for dim, check in zip(dims, checks) if check]
         for k in range(f.ndim):
             if type(ind[k]) is int:
                 ind[k] = (ind[k], ind[k] + 1)
         ind = [ind[k] for k in axis_slice]
         idx = psdist.image.slice_idx(f.ndim, axis_slice, ind)
         _f = psdist.image.project(f[idx], axis_view)
+        
         # Update plotting key word arguments.
         if "cmap" in kws:
             plot_kws["cmap"] = kws["cmap"]
         if "profiles_checkbox" in kws:
             plot_kws["profx"] = plot_kws["profy"] = kws["profiles_checkbox"]
         plot_kws["norm"] = "log" if kws["log"] else None
         plot_kws["process_kws"]["fill_value"] = 0
         if "thresh_slider" in kws:
             plot_kws["process_kws"]["thresh"] = 10.0 ** kws["thresh_slider"]
         else:
             plot_kws["process_kws"]["thresh"] = None
+            
         # Plot the projection onto the specified axes.
         fig, ax = pplt.subplots()
         ax = plot2d(
             _f, coords=[coords[axis_view[0]], coords[axis_view[1]]], ax=ax, **plot_kws
         )
         ax.format(xlabel=dims_units[axis_view[0]], ylabel=dims_units[axis_view[1]])
         plt.show()
@@ -658,29 +662,32 @@
         dim1 = kws["dim1"]
         ind, checks = [], []
         for i in range(100):
             if f"check{i}" in kws:
                 checks.append(kws[f"check{i}"])
             if f"slider{i}" in kws:
                 ind.append(kws[f"slider{i}"])
+                
         # Return nothing if input does not make sense.
         for dim, check in zip(dims, checks):
             if check and dim == dim1:
                 return
+                
         # Slice, then project onto the specified axis.
         axis_view = dims.index(dim1)
         axis_slice = [dims.index(dim) for dim, check in zip(dims, checks) if check]
         for k in range(f.ndim):
             if type(ind[k]) is int:
                 ind[k] = (ind[k], ind[k] + 1)
         ind = [ind[k] for k in axis_slice]
         idx = psdist.image.slice_idx(f.ndim, axis_slice, ind)
         profile = psdist.image.project(f[idx], axis_view)
         if np.max(profile) > 0:
             profile = profile / np.sum(profile)
+            
         # Plot the projection.
         fig, ax = pplt.subplots(**fig_kws)
         ax.format(xlabel=dims_units[axis_view])
         vis.plot1d(coords[axis_view], profile, ax=ax, **plot_kws)
         plt.show()
 
     kws = {"dim1": dim1}
```

### Comparing `psdist-0.1.4/psdist/visualization/visualization.py` & `psdist-0.1.5/psdist/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.4/psdist.egg-info/PKG-INFO` & `psdist-0.1.5/psdist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: psdist
-Version: 0.1.4
+Version: 0.1.5
 Summary: Analysis/visualization of phase space distributions
 Author-email: Austin Hoover <ahoover1218@gmail.com>
 Project-URL: homepage, https://github.com/austin-hoover/psdist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psdist
 
-This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions.
+This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions. Most of the methods should work for point-cloud or image data of any dimensionality.
 
 
 ## Installation
 
 https://pypi.org/project/psdist/
```

### Comparing `psdist-0.1.4/pyproject.toml` & `psdist-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psdist"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Austin Hoover", email="ahoover1218@gmail.com" },
 ]
 description = "Analysis/visualization of phase space distributions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

