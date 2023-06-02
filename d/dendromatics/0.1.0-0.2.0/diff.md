# Comparing `tmp/dendromatics-0.1.0.tar.gz` & `tmp/dendromatics-0.2.0.tar.gz`

## Comparing `dendromatics-0.1.0.tar` & `dendromatics-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 dendromatics-0.1.0/TODO.txt
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dendromatics-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 dendromatics-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/algorithm.rst
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/cc_plugin.rst
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/dendromatics.rst
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/examples.rst
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/executable.rst
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/installation.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/make.bat
--rw-r--r--   0        0        0    56840 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/_static/3dfin_2_png.png
--rw-r--r--   0        0        0    22215 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/_static/dendromatics_logo.png
--rw-r--r--   0        0        0   113056 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/_static/height-normalization.jpg
--rw-r--r--   0        0        0    45823 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/_static/individualized_trees.jpg
--rw-r--r--   0        0        0   109342 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/_static/sections_and_axes.jpg
--rw-r--r--   0        0        0   210688 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/_static/stripe_and_groups.jpg
--rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 dendromatics-0.1.0/docs/_static/tree_height.jpg
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 dendromatics-0.1.0/examples/example.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dendromatics-0.1.0/src/dendromatics/__about__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 dendromatics-0.1.0/src/dendromatics/__init__.py
--rw-r--r--   0        0        0    13688 2020-02-02 00:00:00.000000 dendromatics-0.1.0/src/dendromatics/draw.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 dendromatics-0.1.0/src/dendromatics/ground.py
--rw-r--r--   0        0        0    18201 2020-02-02 00:00:00.000000 dendromatics-0.1.0/src/dendromatics/individualize.py
--rw-r--r--   0        0        0    42691 2020-02-02 00:00:00.000000 dendromatics-0.1.0/src/dendromatics/sections.py
--rw-r--r--   0        0        0     8424 2020-02-02 00:00:00.000000 dendromatics-0.1.0/src/dendromatics/stripe.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dendromatics-0.1.0/src/dendromatics/voxel/__init__.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 dendromatics-0.1.0/src/dendromatics/voxel/voxel.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 dendromatics-0.1.0/tests/test_ground.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 dendromatics-0.1.0/tests/test_voxel.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 dendromatics-0.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 dendromatics-0.1.0/LICENSE
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 dendromatics-0.1.0/README.rst
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dendromatics-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 dendromatics-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 dendromatics-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dendromatics-0.2.0/readthedocs.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dendromatics-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 dendromatics-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/algorithm.rst
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/cc_plugin.rst
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/dendromatics.rst
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/examples.rst
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/executable.rst
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/installation.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0   252269 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/3dfin_logo.png
+-rw-r--r--   0        0        0   270012 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/dendromatics_logo.png
+-rw-r--r--   0        0        0   113056 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/height-normalization.jpg
+-rw-r--r--   0        0        0    45823 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/individualized_trees.jpg
+-rw-r--r--   0        0        0   109342 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/sections_and_axes.jpg
+-rw-r--r--   0        0        0   210688 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/stripe_and_groups.jpg
+-rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/tree_height.jpg
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 dendromatics-0.2.0/examples/example.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/__about__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/__init__.py
+-rw-r--r--   0        0        0    13686 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/draw.py
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/ground.py
+-rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/individualize.py
+-rw-r--r--   0        0        0    42900 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/sections.py
+-rw-r--r--   0        0        0     8424 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/stripe.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/voxel/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/voxel/voxel.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 dendromatics-0.2.0/tests/test_ground.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 dendromatics-0.2.0/tests/test_voxel.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 dendromatics-0.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 dendromatics-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 dendromatics-0.2.0/README.rst
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 dendromatics-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 dendromatics-0.2.0/PKG-INFO
```

### Comparing `dendromatics-0.1.0/.github/workflows/build.yml` & `dendromatics-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/.github/workflows/test.yml` & `dendromatics-0.2.0/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Test dendromatics
+name: Tests
 
 # we only want to trigger this on main branch for PR and all branch for Push.
 on:
   push:
   pull_request:
     branches:
       - main
```

### Comparing `dendromatics-0.1.0/docs/Makefile` & `dendromatics-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/docs/algorithm.rst` & `dendromatics-0.2.0/docs/algorithm.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Algorithm
 =========
 
 The package functionalities are based on an updated version of the algorithm presented in [CABO2018]_. What follows is a description of the main steps of the algorithm.
 
 
-0. Height-normalization of the point cloud (pre-requisite)
+0. Height-normalization of the point cloud
 ----------------------------------------------------------------
 
-The algorithm requires a height-normalized point cloud as input, as in Figure 1. 
+The algorithm starts with a height-normalized point cloud as input, as in Figure 1. Functionality to compute normalized heights is provided in ground module.
 
 .. image:: _static/height-normalization.jpg
   :width: 670
   :align: center
 
-*Figure 1. The algorithm requires height-normalized point clouds. A) Original point cloud. B) Height-normalized point cloud. From* [CABO2018]_.
+*Figure 1. The algorithm uses normalized heights, which can be computed using dendromatics functionalities. A) Original point cloud. B) Height-normalized point cloud. From* [CABO2018]_.
 
 To achieve this, a digital terrain model (DTM) is generated and the normalized heights for each point in the cloud are obtained as the difference between their (z) value and the (z) value of the DTM points that are below. 
 
 To generate the DTM itself, a cloth-simulation filter (CSF) as described in [ZHAN2016]_ is applied to the point cloud. To obtain the DTM points that are below a certain cloud point, a cKDtree is generated and the 3 closest DTM points are identified. Then, a weighted average of the (z) value based on the distance to the cloud point is obtained, and the normalized height value is computed as the difference between the (z) value of the cloud point and the weighted average (z) value of the DTM points.
 
 
 1. Identification of stems among user-provided horizontal stripe
```

### Comparing `dendromatics-0.1.0/docs/conf.py` & `dendromatics-0.2.0/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,48 +24,48 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx.ext.napoleon",
-    "sphinx_reference_rename",
+    #   "sphinx_reference_rename",
     "sphinx.ext.intersphinx",
 ]
 
 napoleon_google_docstring = False
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 
 # Modifying qualified names
 
-sphinx_reference_rename_mapping = {
-    "dendromatics.voxel.voxel.voxelate": "voxelate",
-    "dendromatics.ground.clean_cloth": "clean_cloth",
-    "dendromatics.ground.clean_ground": "clean_ground",
-    "dendromatics.ground.generate_dtm": "generate_dtm",
-    "dendromatics.ground.normalize_heights": "normalize_heights",
-    "dendromatics.stripe.verticality_clustering": "verticality_clustering",
-    "dendromatics.stripe.verticality_clustering_iteration": "verticality_clustering_iteration",
-    "dendromatics.individualize.compute_axes": "compute_axes",
-    "dendromatics.individualize.compute_heights": "compute_heights",
-    "dendromatics.individualize.individualize_trees": "individualize_trees",
-    "dendromatics.sections.compute_sections": "compute_sections",
-    "dendromatics.sections.fit_circle": "fit_circle",
-    "dendromatics.sections.fit_circle_check": "fit_circle_check",
-    "dendromatics.sections.inner_circle": "inner_circle",
-    "dendromatics.sections.point_clustering": "point_clustering",
-    "dendromatics.sections.sector_occupancy": "sector_occupancy",
-    "dendromatics.sections.tilt_detection": "tilt_detection",
-    "dendromatics.sections.tree_locator": "tree_locator",
-    "dendromatics.draw.draw_axes": "draw_axes",
-    "dendromatics.draw.draw_circles": "draw_circles",
-}
+# sphinx_reference_rename_mapping = {
+#     "dendromatics.voxel.voxel.voxelate": "voxelate",
+#     "dendromatics.ground.clean_cloth": "clean_cloth",
+#     "dendromatics.ground.clean_ground": "clean_ground",
+#     "dendromatics.ground.generate_dtm": "generate_dtm",
+#     "dendromatics.ground.normalize_heights": "normalize_heights",
+#     "dendromatics.stripe.verticality_clustering": "verticality_clustering",
+#     "dendromatics.stripe.verticality_clustering_iteration": "verticality_clustering_iteration",
+#     "dendromatics.individualize.compute_axes": "compute_axes",
+#     "dendromatics.individualize.compute_heights": "compute_heights",
+#     "dendromatics.individualize.individualize_trees": "individualize_trees",
+#     "dendromatics.sections.compute_sections": "compute_sections",
+#     "dendromatics.sections.fit_circle": "fit_circle",
+#     "dendromatics.sections.fit_circle_check": "fit_circle_check",
+#     "dendromatics.sections.inner_circle": "inner_circle",
+#     "dendromatics.sections.point_clustering": "point_clustering",
+#     "dendromatics.sections.sector_occupancy": "sector_occupancy",
+#     "dendromatics.sections.tilt_detection": "tilt_detection",
+#     "dendromatics.sections.tree_locator": "tree_locator",
+#     "dendromatics.draw.draw_axes": "draw_axes",
+#     "dendromatics.draw.draw_circles": "draw_circles",
+# }
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
```

### Comparing `dendromatics-0.1.0/docs/dendromatics.rst` & `dendromatics-0.2.0/docs/dendromatics.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/docs/examples.rst` & `dendromatics-0.2.0/docs/examples.rst`

 * *Files 1% similar despite different names*

```diff
@@ -76,12 +76,12 @@
 tilt_detection() computes an 'outlier probability' for each section based on its tilting relative to neighbour sections and the relative to the tree axis::
     
     outlier_prob = dm.tilt_detection(X_c, Y_c, R, sections)
 
 
 For further examples and more thorough explanations, please check *example.py* script in */examples* folder in the official GitHub repository:
 
-https://github.com/3DFIN/dendromatics
+https://github.com/3DFin/dendromatics
```

### Comparing `dendromatics-0.1.0/docs/index.rst` & `dendromatics-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/docs/make.bat` & `dendromatics-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/docs/_static/height-normalization.jpg` & `dendromatics-0.2.0/docs/_static/height-normalization.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/docs/_static/individualized_trees.jpg` & `dendromatics-0.2.0/docs/_static/individualized_trees.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/docs/_static/sections_and_axes.jpg` & `dendromatics-0.2.0/docs/_static/sections_and_axes.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/docs/_static/stripe_and_groups.jpg` & `dendromatics-0.2.0/docs/_static/stripe_and_groups.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/docs/_static/tree_height.jpg` & `dendromatics-0.2.0/docs/_static/tree_height.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/examples/example.py` & `dendromatics-0.2.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/src/dendromatics/draw.py` & `dendromatics-0.2.0/src/dendromatics/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,19 +291,18 @@
     stripe_lower_limit : float
         Lower (vertical) limit of the stripe (units is meters). Defaults to 0.7.
     stripe_upper_limit : float
         Upper (vertical) limit of the stripe (units is meters). Defaults to 3.5.
     point_interval : float
         Step value used to draw points (unit is meters). Defaults to 0.01.
 
-    Returns:
+    Returns
     --------
     axes_point : numpy.ndarray
         Matrix that describes the point cloud of the axes
-
     tilt : numpy.ndarray
         Matrix that describes the tilt of each axes
     """
     stripe_centroid = (stripe_lower_limit + stripe_upper_limit) / 2
     mean_descend = stripe_centroid + line_downstep
     mean_rise = line_upstep - stripe_centroid
```

### Comparing `dendromatics-0.1.0/src/dendromatics/ground.py` & `dendromatics-0.2.0/src/dendromatics/ground.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #### IMPORTS ####
 import CSF
 import numpy as np
+from scipy.interpolate import griddata
 from scipy.spatial import cKDTree
 from sklearn.cluster import DBSCAN
 
 from .voxel.voxel import *
 
 # -----------------------------------------------------------------------------
 # clean_ground
@@ -145,14 +146,56 @@
     mads = np.median(abs_devs)
     clean_points = dtm_points[abs_devs < 2 * mads]
 
     return clean_points
 
 
 # -----------------------------------------------------------------------------
+# complete_dtm
+# -----------------------------------------------------------------------------
+
+
+def complete_dtm(dtm_points):
+    """This function uses scipy.interpolate.griddata to interpolate the missing
+    values in a Digital Terrain Model (DTM).
+
+    Parameters
+    ----------
+    dtm_points : numpy array
+        Matrix containing (x, y, z) coordinates of the DTM points.
+
+    Returns
+    -------
+    completed_dtm : numpy.ndarray
+        Matrix containing (x, y, z) coordinates of the completed DTM points.
+    """
+
+    # Separate x, y, z coordinates
+    x = dtm_points[:, 0]
+    y = dtm_points[:, 1]
+    z = dtm_points[:, 2]
+
+    # Generate a grid of points based on min x, y values
+    xi = np.linspace(min(x), max(x), 100)
+    yi = np.linspace(min(y), max(y), 100)
+    xi, yi = np.meshgrid(xi, yi)
+
+    # Interpolate missing values using griddata
+    zi = griddata((x, y), z, (xi, yi), method="cubic")
+
+    # Combine interpolated points with existing points
+    completed_dtm = np.hstack((xi.reshape(-1, 1), yi.reshape(-1, 1), zi.reshape(-1, 1)))
+
+    # Remove nan values which may arise from interpolation
+    completed_dtm = completed_dtm[~np.isnan(completed_dtm).any(axis=1)]
+
+    return completed_dtm
+
+
+# -----------------------------------------------------------------------------
 # normalize_heights
 # -----------------------------------------------------------------------------
 
 
 def normalize_heights(cloud, dtm_points):
     """This function takes a point cloud and a Digital Terrain Model (DTM) and
     normalizes the heights of the first based on the second.
```

### Comparing `dendromatics-0.1.0/src/dendromatics/individualize.py` & `dendromatics-0.2.0/src/dendromatics/individualize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #### IMPORTS ####
-import sys
 
 import numpy as np
 from sklearn.cluster import DBSCAN
 from sklearn.decomposition import PCA
 
 from .voxel.voxel import *
 
@@ -21,14 +20,15 @@
     min_points,
     d_max,
     X_field,
     Y_field,
     Z_field,
     Z0_field,
     tree_id_field,
+    progress_hook=None,
 ):
     """Function used inside individualize_trees during tree individualization
     process. It identifies tree axes. It expects a voxelated version of the
     point cloud and a filtered (based on the verticality clustering process)
     stripe as input, so that it only contains (hopefully) stems. Those stems
     are isolated and enumerated, and then, their axes are identified using PCA
     (PCA1 direction). This allows to group points based on their distance to
@@ -61,14 +61,17 @@
         Index at which (y) coordinates are stored.
     Z_field : int
         Index at which (z) coordinates are stored.
     Z0_field : int
         Index at which (z0) coordinates are stored.
     tree_id_field : int
         Index at which cluster ID is stored.
+    progress_hook : callable, optional
+        A hook that take two int, the first is the current number of iteration
+        and the second is the targetted number iteration. Defaults to None.
 
     Returns
     -------
     detected_trees : numpy.ndarray
         Matrix with as many rows as trees, containing a description of each
         individualized tree. It stores the following values: tree ID, PCA1 X
         value, PCA1 Y value, PCA1 Z value, stem centroid X value, stem centroid
@@ -108,14 +111,17 @@
     ind = 0
 
     # Height range (actual value, not the %) that points should extend throughout
     h_range_value = (stripe_upper_limit - stripe_lower_limit) * h_range
 
     # First loop: It goes over each tree (still stems) except for the first entry,
     # which maps to noise (this entry is generated by DBSCAN during clustering).
+
+    if progress_hook is not None:
+        progress_hook(0, n_values)
     for i in filt_unique_values:
         # Isolation of stems: stem_i only contains points associated to 1 tree.
         stem_i = clust_stripe[clust_stripe[:, tree_id_field] == i][
             :, [X_field, Y_field, Z_field]
         ]
 
         # Z and Z0 mean heights of points in a given tree
@@ -148,18 +154,17 @@
                 np.arctan(
                     np.sqrt(detected_trees[ind, 1] ** 2 + detected_trees[ind, 2] ** 2)
                     / detected_trees[ind, 3]
                 )
                 * 180
                 / np.pi
             )
-
             ind = ind + 1
-            sys.stdout.write("\r%d%%" % np.float64((n_values - ind) * 100 / n_values))
-            sys.stdout.flush()
+            if progress_hook is not None:
+                progress_hook(ind, n_values)
 
             # Coordinate transformation from original to PCA. Done for EVERY
             # point of the original cloud from the PCA of a SINGLE stem.
             cloud_pca_coords = pca_out.transform(
                 voxelated_cloud[:, [X_field, Y_field, Z_field]]
             )
 
@@ -170,15 +175,14 @@
             # Points that are closer than d_max to an axis are assigned to that axis.
             # Also, if a point is closer to an axis than it was to previous axes, accounting for points
             # that were previously assigned to some other axis in previous iterations, it is assigned
             # to the new, closer axis. Distance to the axis is stored as well.
             valid_points = (axis_dist < d_max) & ((axis_dist - dist_to_axis) < 0)
             tree_id_vector[valid_points] = i
             dist_to_axis[valid_points] = axis_dist[valid_points]
-
     # This deletes the trailing rows that only contains zeros
     detected_trees = detected_trees[~np.all(detected_trees == 0, axis=1)]
     return (detected_trees, dist_to_axis, tree_id_vector)
 
 
 # -----------------------------------------------------------------------------
 # compute_heights
@@ -334,14 +338,15 @@
     resolution_heights=0.3,
     n_digits=5,
     X_field=0,
     Y_field=1,
     Z_field=2,
     Z0_field=3,
     tree_id_field=-1,
+    progress_hook=None,
 ):
     """This function expects a filtered (based on the clustering process)
     stripe as input, so that it only contains (hopefully) stems. Those stems
     are voxelated and enumerated, and then, their axes are identified using PCA
     (PCA1 direction). This allows to group points based on their distance to
     those axes, thus assigning each point to a tree. This last step is applied
     to the WHOLE original cloud. It also measures tree heights.
@@ -393,14 +398,17 @@
         Index at which (y) coordinate is stored. Defaults to 1.
     Z_field : int
         Index at which (z) coordinate is stored. Defaults to 2.
     Z0_field : int
         Index at which (z0) coordinate is stored. Defaults to 3.
     tree_id_field : int
         Index at which cluster ID is stored. Defaults to -1.
+    progress_hook : callable, optional
+        A hook that take two int, the first is the current number of iteration
+        and the second is the targetted number iteration. Defaults to None.
 
     Returns
     -------
     assigned_cloud : numpy.ndarray
         Point cloud containing individualized trees. It consists of
         (x), (y), (z) and (z0) coordinates, a 5th column containing tree ID
         that each point belongs to and a 6th column containing point distance
@@ -441,14 +449,15 @@
         min_points,
         d_max,
         X_field,
         Y_field,
         Z_field,
         Z0_field,
         tree_id_field,
+        progress_hook,
     )
 
     # Call to compute_heights
     tree_heights = compute_heights(
         voxelated_cloud,
         detected_trees,
         dist_to_axis,
```

### Comparing `dendromatics-0.1.0/src/dendromatics/sections.py` & `dendromatics-0.2.0/src/dendromatics/sections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #### IMPORTS ####
-import sys
 
 import numpy as np
 from scipy import optimize as opt
 from scipy.cluster import hierarchy as sch
 from scipy.spatial import distance_matrix
 
 from .voxel.voxel import *
@@ -444,14 +443,15 @@
     n_sectors=16,
     min_n_sectors=9,
     width=2,
     X_field=0,
     Y_field=1,
     Z0_field=3,
     tree_id_field=4,
+    progress_hook=None,
 ):
     """This function calls fit_circle_check() to compute stem diameter at
     given sections.
 
     Parameters
     ----------
     stems : numpy.ndarray
@@ -485,14 +485,17 @@
         Index at which (x) coordinate is stored. Defaults to 0.
     Y_field : int
         Index at which (y) coordinate is stored. Defaults to 1.
     Z0_field : int
         Index at which (z0) coordinate is stored. Defaults to 3.
     tree_id_field : int
         Index at which cluster ID is stored. Defaults to 4.
+    progress_hook : callable, optional
+        A hook that take two int, the first is the current number of iteration
+        and the second is the targetted number iteration. Defaults to None.
 
     Returns
     -------
     X_c : numpy.ndarray
         Matrix containing (x) coordinates of the center of the best-fit circles.
     Y_c : numpy.ndarray
         Matrix containing (y) coordinates of the center of the best-fit circles.
@@ -525,26 +528,23 @@
         (n_trees, n_sections), dtype=float
     )  # Empty array to store inner points data
 
     # Filling previous empty arrays
 
     # Auxiliar index for first loop
     tree = -1  # Loop will start at -1
-
+    if progress_hook is not None:
+        progress_hook(0, n_trees)
     # First loop: iterates over each tree
     for tr in trees:
         # Tree ID is used to iterate over trees
         tree_i = stems[stems[:, tree_id_field] == tr, :]
         tree = tree + 1
-
-        sys.stdout.write(
-            "\r%d%%" % np.float64((trees.shape[0] - tree) * 100 / trees.shape[0])
-        )
-        sys.stdout.flush()
-
+        if progress_hook is not None:
+            progress_hook(tree + 1, n_trees)
         # Auxiliar index for second loop
         section = 0
 
         # Second loop: iterates over each section
         for b in sections:
             # Selecting (x, y) coordinates of points within the section
             X = tree_i[
@@ -587,15 +587,14 @@
             R[tree, section] = R_fill
             check_circle[tree, section] = check_circle_fill
             second_time[tree, section] = second_time_fill
             sector_perct[tree, section] = sector_perct_fill
             n_points_in[tree, section] = n_points_in_fill
 
             section = section + 1
-
     return (X_c, Y_c, R, check_circle, second_time, sector_perct, n_points_in)
 
 
 # -----------------------------------------------------------------------------
 # tilt_detection
 # -----------------------------------------------------------------------------
```

### Comparing `dendromatics-0.1.0/src/dendromatics/stripe.py` & `dendromatics-0.2.0/src/dendromatics/stripe.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/src/dendromatics/voxel/voxel.py` & `dendromatics-0.2.0/src/dendromatics/voxel/voxel.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/tests/test_ground.py` & `dendromatics-0.2.0/tests/test_ground.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/tests/test_voxel.py` & `dendromatics-0.2.0/tests/test_voxel.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/.gitignore` & `dendromatics-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/LICENSE` & `dendromatics-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dendromatics-0.1.0/README.rst` & `dendromatics-0.2.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,55 @@
+.. image:: https://github.com/3DFin/dendromatics/blob/main/docs/_static/dendromatics_logo.png
+  :width: 300
+  :align: center
+
+Dendromatics
+============
+
+|docs| |pypi| |tests|
+
+.. |docs| image:: https://readthedocs.org/projects/dendromatics/badge/?version=latest
+    :alt: Documentation Status
+    :scale: 100%
+    :target: https://dendromatics.readthedocs.io/en/latest/?badge=latest
+
+.. |pypi| image:: https://badge.fury.io/py/dendromatics.svg
+    :alt: PyPI status
+    :scale: 100%
+    :target: https://badge.fury.io/py/dendromatics
+
+.. |tests| image:: https://github.com/3DFin/dendromatics/actions/workflows/test.yml/badge.svg
+    :alt: Tests status
+    :scale: 100%
+    :target:  https://github.com/3DFin/dendromatics/actions
+
+
 Description
 ===========
 
-The `src` folder contains functionalities to detect the trees present in a terrestrial 3D point cloud from a forest plot, and compute individual tree parameters: tree height, tree location, diameters along the stem (including DBH), and stem axis. These are based on an updated version of the algorithm proposed by (Cabo et al., 2018).
+The *src* folder contains functionalities to detect the trees present in a terrestrial 3D point cloud from a forest plot, and compute individual tree parameters: tree height, tree location, diameters along the stem (including DBH), and stem axis. These are based on an updated version of the algorithm proposed by (Cabo et al., 2018).
 
 The functionalities may be divided in four main steps:
 
-0. Height-normalization of the point cloud (pre-requisite). 
+0. Height-normalization of the point cloud. 
 1. Identification of stems among user-provided stripe.
 2. Tree individualization based on point-to-stems distances.
 3. Robust computation of stems diameter at different section heights.
 
 Although individual, somewhat independent functions are provided, they are designed to be used in a script that calls one after the other following the algorithm structure. An example script can be found in `example` folder.
 
 
 Examples
 ========
 
 
 Height-normalization
 --------------------
 
-Almost all functions in the module expect a height-normalized point cloud to work as intended. If your point cloud is not height-normalized, you can do it in a simple way using some of the module functions.
+Almost all functions in the module expect a height-normalized point cloud to work as intended. If your point cloud is not height-normalized, you can do it in a simple way using some of the module functions. I'ts based on 'Cloth simulation Filter' (Zhang et al., 2016).
 
 .. code-block:: python
     
     import laspy
     import numpy as np
     import dendromatics as dm
 
@@ -110,24 +135,28 @@
 
 References
 ==========
 
 Cabo, C., Ordóñez, C., López-Sánchez, C. A., & Armesto, J. (2018). Automatic dendrometry: Tree detection, tree height and diameter estimation using terrestrial laser scanning. International Journal of Applied Earth Observation and Geoinformation, 69, 164–174. https://doi.org/10.1016/j.jag.2018.01.011
 
 
-Ester, M., Kriegel, H.-P., Sander, J., & Xu, X. (1996). A Density-Based Algorithm for Discovering Clusters in Large Spatial Databases with Noise. www.aaai.org
+Prendes, C., Cabo, C., Ordoñez, C., Majada, J., & Canga, E. (2021). An algorithm for the automatic parametrization of wood volume equations from Terrestrial Laser Scanning point clouds: application in Pinus pinaster. GIScience and Remote Sensing, 58(7), 1130–1150. https://doi.org/10.1080/15481603.2021.1972712 
 
 
-Prendes, C., Cabo, C., Ordoñez, C., Majada, J., & Canga, E. (2021). An algorithm for the automatic parametrization of wood volume equations from Terrestrial Laser Scanning point clouds: application in Pinus pinaster. GIScience and Remote Sensing, 58(7), 1130–1150. https://doi.org/10.1080/15481603.2021.1972712 
+Zhang, W., Qi, J., Wan, P., Wang, H., Xie, D., Wang, X., & Yan, G. (2016). An easy-to-use airborne LiDAR data filtering method based on cloth simulation. Remote Sensing, 8(6). https://doi.org/10.3390/rs8060501
 
 
 Install
 =======
 
-*dendromatics* is available on `PyPI <TODO PyPi link>`_ and the full documentation can be consulted on `TBD <TODO doc link>`_
+*dendromatics* is available on `PyPI <https://pypi.org/project/dendromatics/>`_ and the full documentation can be consulted on `ReadTheDocs.io <https://dendromatics.readthedocs.io/en/latest/>`_
+
+.. code-block:: console
+    
+    python -m pip install dendromatics
 
 The list of dependencies is available in the *pyproject.toml* file.
 
 *dendromatics* relies on `hatch <https://github.com/pypa/hatch>`_
 
 Depending on your version of Python and your OS, you might also need a C/C++ compiler to compile some of the mandatory dependencies (CSF and jakteristics). 
 But in any case you would not have to run the compiler by yourself, the build system will manage dependencies and compilation for you.
```

### Comparing `dendromatics-0.1.0/pyproject.toml` & `dendromatics-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -33,18 +33,17 @@
     "scipy>=1.10.0",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project.urls]
-Source = "https://github.com/3DFIN/dendromatics"
-# TODO: to be changed once sphinx documentation is deployed
-Documentation = "https://github.com/3DFIN/3DFIN#README.md"
-Issues = "https://github.com/3DFIN/dendromatics/issues"
+Source = "https://github.com/3DFin/dendromatics"
+Documentation = "https://dendromatics.readthedocs.io/en/latest/"
+Issues = "https://github.com/3DFin/dendromatics/issues"
 
 [tool.hatch.version]
 path = "src/dendromatics/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
```

### Comparing `dendromatics-0.1.0/PKG-INFO` & `dendromatics-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dendromatics
-Version: 0.1.0
+Version: 0.2.0
 Summary: Automatic dendrometry and forest inventory for terrestrial point clouds
-Project-URL: Source, https://github.com/3DFIN/dendromatics
-Project-URL: Documentation, https://github.com/3DFIN/3DFIN#README.md
-Project-URL: Issues, https://github.com/3DFIN/dendromatics/issues
+Project-URL: Source, https://github.com/3DFin/dendromatics
+Project-URL: Documentation, https://dendromatics.readthedocs.io/en/latest/
+Project-URL: Issues, https://github.com/3DFin/dendromatics/issues
 Author-email: Carlos Cabo <carloscabo@uniovi.es>, Diego Laino <diegolainor@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: forestry,lidar,tls
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
@@ -18,37 +18,62 @@
 Requires-Dist: jakteristics>=0.5.1
 Requires-Dist: laspy>=2.4.0
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: scikit-learn>=1.2.0
 Requires-Dist: scipy>=1.10.0
 Description-Content-Type: text/x-rst
 
+.. image:: https://github.com/3DFin/dendromatics/blob/main/docs/_static/dendromatics_logo.png
+  :width: 300
+  :align: center
+
+Dendromatics
+============
+
+|docs| |pypi| |tests|
+
+.. |docs| image:: https://readthedocs.org/projects/dendromatics/badge/?version=latest
+    :alt: Documentation Status
+    :scale: 100%
+    :target: https://dendromatics.readthedocs.io/en/latest/?badge=latest
+
+.. |pypi| image:: https://badge.fury.io/py/dendromatics.svg
+    :alt: PyPI status
+    :scale: 100%
+    :target: https://badge.fury.io/py/dendromatics
+
+.. |tests| image:: https://github.com/3DFin/dendromatics/actions/workflows/test.yml/badge.svg
+    :alt: Tests status
+    :scale: 100%
+    :target:  https://github.com/3DFin/dendromatics/actions
+
+
 Description
 ===========
 
-The `src` folder contains functionalities to detect the trees present in a terrestrial 3D point cloud from a forest plot, and compute individual tree parameters: tree height, tree location, diameters along the stem (including DBH), and stem axis. These are based on an updated version of the algorithm proposed by (Cabo et al., 2018).
+The *src* folder contains functionalities to detect the trees present in a terrestrial 3D point cloud from a forest plot, and compute individual tree parameters: tree height, tree location, diameters along the stem (including DBH), and stem axis. These are based on an updated version of the algorithm proposed by (Cabo et al., 2018).
 
 The functionalities may be divided in four main steps:
 
-0. Height-normalization of the point cloud (pre-requisite). 
+0. Height-normalization of the point cloud. 
 1. Identification of stems among user-provided stripe.
 2. Tree individualization based on point-to-stems distances.
 3. Robust computation of stems diameter at different section heights.
 
 Although individual, somewhat independent functions are provided, they are designed to be used in a script that calls one after the other following the algorithm structure. An example script can be found in `example` folder.
 
 
 Examples
 ========
 
 
 Height-normalization
 --------------------
 
-Almost all functions in the module expect a height-normalized point cloud to work as intended. If your point cloud is not height-normalized, you can do it in a simple way using some of the module functions.
+Almost all functions in the module expect a height-normalized point cloud to work as intended. If your point cloud is not height-normalized, you can do it in a simple way using some of the module functions. I'ts based on 'Cloth simulation Filter' (Zhang et al., 2016).
 
 .. code-block:: python
     
     import laspy
     import numpy as np
     import dendromatics as dm
 
@@ -134,24 +159,28 @@
 
 References
 ==========
 
 Cabo, C., Ordóñez, C., López-Sánchez, C. A., & Armesto, J. (2018). Automatic dendrometry: Tree detection, tree height and diameter estimation using terrestrial laser scanning. International Journal of Applied Earth Observation and Geoinformation, 69, 164–174. https://doi.org/10.1016/j.jag.2018.01.011
 
 
-Ester, M., Kriegel, H.-P., Sander, J., & Xu, X. (1996). A Density-Based Algorithm for Discovering Clusters in Large Spatial Databases with Noise. www.aaai.org
+Prendes, C., Cabo, C., Ordoñez, C., Majada, J., & Canga, E. (2021). An algorithm for the automatic parametrization of wood volume equations from Terrestrial Laser Scanning point clouds: application in Pinus pinaster. GIScience and Remote Sensing, 58(7), 1130–1150. https://doi.org/10.1080/15481603.2021.1972712 
 
 
-Prendes, C., Cabo, C., Ordoñez, C., Majada, J., & Canga, E. (2021). An algorithm for the automatic parametrization of wood volume equations from Terrestrial Laser Scanning point clouds: application in Pinus pinaster. GIScience and Remote Sensing, 58(7), 1130–1150. https://doi.org/10.1080/15481603.2021.1972712 
+Zhang, W., Qi, J., Wan, P., Wang, H., Xie, D., Wang, X., & Yan, G. (2016). An easy-to-use airborne LiDAR data filtering method based on cloth simulation. Remote Sensing, 8(6). https://doi.org/10.3390/rs8060501
 
 
 Install
 =======
 
-*dendromatics* is available on `PyPI <TODO PyPi link>`_ and the full documentation can be consulted on `TBD <TODO doc link>`_
+*dendromatics* is available on `PyPI <https://pypi.org/project/dendromatics/>`_ and the full documentation can be consulted on `ReadTheDocs.io <https://dendromatics.readthedocs.io/en/latest/>`_
+
+.. code-block:: console
+    
+    python -m pip install dendromatics
 
 The list of dependencies is available in the *pyproject.toml* file.
 
 *dendromatics* relies on `hatch <https://github.com/pypa/hatch>`_
 
 Depending on your version of Python and your OS, you might also need a C/C++ compiler to compile some of the mandatory dependencies (CSF and jakteristics). 
 But in any case you would not have to run the compiler by yourself, the build system will manage dependencies and compilation for you.
```

