# Comparing `tmp/magnify-0.2.2.tar.gz` & `tmp/magnify-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.2.2.tar", max compression
+gzip compressed data, was "magnify-0.3.0.tar", max compression
```

## Comparing `magnify-0.2.2.tar` & `magnify-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.2.2/README.md
--rw-r--r--   0        0        0     1601 2023-05-11 17:10:32.989687 magnify-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      222 2023-05-11 17:10:39.829824 magnify-0.2.2/src/magnify/__init__.py
--rw-r--r--   0        0        0     4586 2023-04-19 17:49:40.798430 magnify-0.2.2/src/magnify/filter.py
--rw-r--r--   0        0        0    26017 2023-04-20 23:51:46.110906 magnify-0.2.2/src/magnify/find.py
--rw-r--r--   0        0        0     1406 2023-04-14 21:30:07.711891 magnify-0.2.2/src/magnify/pipeline.py
--rw-r--r--   0        0        0      291 2023-04-14 03:25:12.785396 magnify-0.2.2/src/magnify/plot/__init__.py
--rw-r--r--   0        0        0     2348 2023-05-09 14:34:10.399616 magnify-0.2.2/src/magnify/plot/image.py
--rw-r--r--   0        0        0     1855 2023-05-11 01:21:29.027397 magnify-0.2.2/src/magnify/plot/ndplot.py
--rw-r--r--   0        0        0     2488 2023-05-11 02:09:19.162200 magnify-0.2.2/src/magnify/plot/relation.py
--rw-r--r--   0        0        0      650 2023-05-11 02:30:53.591879 magnify-0.2.2/src/magnify/plot/style.py
--rw-r--r--   0        0        0     1033 2023-04-20 23:51:45.846900 magnify-0.2.2/src/magnify/postprocess.py
--rw-r--r--   0        0        0     1736 2023-04-14 21:30:15.276066 magnify-0.2.2/src/magnify/preprocess.py
--rw-r--r--   0        0        0    14065 2023-04-19 01:42:37.155610 magnify-0.2.2/src/magnify/reader.py
--rw-r--r--   0        0        0     3374 2023-04-19 18:59:40.761736 magnify-0.2.2/src/magnify/registry.py
--rw-r--r--   0        0        0     1121 2023-04-07 21:54:06.746151 magnify-0.2.2/src/magnify/stitch.py
--rw-r--r--   0        0        0     2644 2023-04-21 02:34:29.243260 magnify-0.2.2/src/magnify/utils.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 magnify-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.3.0/README.md
+-rw-r--r--   0        0        0     1649 2023-06-02 00:28:59.358390 magnify-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-02 00:26:47.659424 magnify-0.3.0/src/magnify/__init__.py
+-rw-r--r--   0        0        0     4571 2023-06-02 00:21:13.635636 magnify-0.3.0/src/magnify/filter.py
+-rw-r--r--   0        0        0    26578 2023-06-02 00:21:04.883425 magnify-0.3.0/src/magnify/find.py
+-rw-r--r--   0        0        0     3573 2023-06-02 00:26:38.835224 magnify-0.3.0/src/magnify/identify.py
+-rw-r--r--   0        0        0     1406 2023-04-14 21:30:07.711891 magnify-0.3.0/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      317 2023-05-31 18:04:36.204183 magnify-0.3.0/src/magnify/plot/__init__.py
+-rw-r--r--   0        0        0     2339 2023-06-02 00:19:24.832979 magnify-0.3.0/src/magnify/plot/image.py
+-rw-r--r--   0        0        0     1855 2023-05-11 01:21:29.027397 magnify-0.3.0/src/magnify/plot/ndplot.py
+-rw-r--r--   0        0        0     2483 2023-05-31 18:00:09.258919 magnify-0.3.0/src/magnify/plot/relation.py
+-rw-r--r--   0        0        0      650 2023-05-11 02:30:53.591879 magnify-0.3.0/src/magnify/plot/style.py
+-rw-r--r--   0        0        0     1017 2023-06-02 00:16:42.972866 magnify-0.3.0/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1736 2023-04-14 21:30:15.276066 magnify-0.3.0/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    15093 2023-05-31 01:36:36.512603 magnify-0.3.0/src/magnify/reader.py
+-rw-r--r--   0        0        0     3339 2023-06-02 00:16:33.476618 magnify-0.3.0/src/magnify/registry.py
+-rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.3.0/src/magnify/stitch.py
+-rw-r--r--   0        0        0     2639 2023-06-02 00:20:14.442200 magnify-0.3.0/src/magnify/utils.py
+-rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 magnify-0.3.0/PKG-INFO
```

### Comparing `magnify-0.2.2/pyproject.toml` & `magnify-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.2.2"
+version = "0.3.0"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 opencv-python = [
@@ -20,14 +20,16 @@
 types-tqdm = "^4.64"
 xarray = {extras = ["complete"], version = ">=2023.01.0"}
 dask = {extras = ["complete"], version = ">=2022.02.0"}
 catalogue = "^2.0.8"
 beautifulsoup4 = "^4.10.0"
 lxml = "^4.6.0"
 confection = "^0.0.4"
+scikit-learn = "^1.2.0"
+scikit-image = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.6.0"
 mypy = "^1.0.1"
 pytest = ">=7.1.2"
 ruff = ">=0.0.249"
 sphinx = "^5.0.2"
```

### Comparing `magnify-0.2.2/src/magnify/filter.py` & `magnify-0.3.0/src/magnify/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
         # Find markers where the fg - bg is below 5 sigma of the mean difference.
         upper_bound = 5 * diffs.std()
         fg = subassay.roi.where(subassay.fg).median(dim=["roi_x", "roi_y"]).compute()
         empty = fg - bg < upper_bound
         for i in range(assay.sizes["mark_row"]):
             for j in range(assay.sizes["mark_col"]):
-                if subassay.mark_tag[i, j] == "":
+                if subassay.tag[i, j] == "":
                     continue
-                if i > 0 and subassay.mark_tag[i - 1, j] == "":
+                if i > 0 and subassay.tag[i - 1, j] == "":
                     assay.valid[i, j] &= empty[i - 1, j]
-                if i < assay.sizes["mark_row"] - 1 and subassay.mark_tag[i + 1, j] == "":
+                if i < assay.sizes["mark_row"] - 1 and subassay.tag[i + 1, j] == "":
                     assay.valid[i, j] &= empty[i + 1, j]
 
     return assay
```

### Comparing `magnify-0.2.2/src/magnify/find.py` & `magnify-0.3.0/src/magnify/find.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 import math
 import logging
 
 from numpy.typing import ArrayLike
 import cv2 as cv
 import dask.array as da
+import numba
 import numpy as np
 import scipy
+import skimage
 import tqdm
 import xarray as xr
 
 from magnify import utils
 import magnify.registry as registry
 
 logger = logging.getLogger(__name__)
@@ -40,15 +42,15 @@
         self.search_timesteps = utils.to_list(search_timestep)
         if search_channel == "all":
             self.search_channels = assay.channel
         else:
             self.search_channels = utils.to_list(search_channel)
 
     def __call__(self, assay: xr.Dataset) -> xr.Dataset:
-        num_rows, num_cols = assay.mark_tag.shape
+        num_rows, num_cols = assay.tag.shape
 
         # Store all channels and timesteps for each marker in one chunk and set marker row/col
         # sizes so each chunk ends up being at least 10MB.
         chunk_bytes = 1e7
         # Don't take into account dtype size since fg/bg bool arrays should also be 10MB.
         mark_bytes = assay.dims["channel"] * assay.dims["time"] * self.roi_length**2
         # Prioritize larger row chunks since we're more likely to want whole columns than rows.
@@ -126,15 +128,15 @@
             # Compute the roi, foreground and background masks for all buttons.
             assay.roi[:, :, :, t], assay.fg[:, :, :, t], assay.bg[:, :, :, t] = self.find_rois(
                 images, t, do_search, assay
             )
         # assay = assay.stack(mark=("mark_row", "mark_col"), create_index=True).transpose(
         #     "mark", ...
         # )
-        # assay = assay.set_xindex("mark_tag")
+        # assay = assay.set_xindex("tag")
 
         return assay
 
     def find_centers(self, images: xr.DataArray, assay: xr.Dataset):
         points = np.empty((0, 2))
         min_button_dist = round(min(self.row_dist, self.col_dist) / 2)
         if min_button_dist % 2 == 0:
@@ -179,16 +181,16 @@
             points = np.concatenate([points, new_points])
 
         # Split the points into x and y components.
         x = points[:, 0]
         y = points[:, 1]
 
         # Step 3: Cluster the points into distinct rows and columns.
-        points_per_row = (assay.mark_tag != "").sum(dim="mark_col")
-        points_per_col = (assay.mark_tag != "").sum(dim="mark_row")
+        points_per_row = (assay.tag != "").sum(dim="mark_col")
+        points_per_col = (assay.tag != "").sum(dim="mark_row")
         num_rows, num_cols = assay.sizes["mark_row"], assay.sizes["mark_col"]
         row_labels = cluster_1d(
             y,
             total_length=image.shape[0],
             num_clusters=num_rows,
             cluster_length=self.row_dist,
             ideal_num_points=points_per_row,
@@ -238,16 +240,16 @@
         # Initialize the roi images.
         for i in range(num_rows):
             for j in range(num_cols):
                 top, bottom, left, right = utils.bounding_box(
                     round(float(assay.x[i, j, t])),
                     round(float(assay.y[i, j, t])),
                     self.roi_length,
-                    assay.sizes["im_y"],
                     assay.sizes["im_x"],
+                    assay.sizes["im_y"],
                 )
                 roi[i, j] = images[..., top:bottom, left:right]
                 offsets[i, j] = left, top
 
         if not do_search:
             # If we're not searching just use the previous background/foreground masks.
             return roi, assay.fg[:, :, :, t - 1].compute(), assay.bg[:, :, :, t - 1].compute()
@@ -257,15 +259,15 @@
         for i in range(num_rows):
             for j in range(num_cols):
                 # TODO: This step should occur over multiple channels.
                 subimage = utils.to_uint8(roi[i, j].sel(channel=self.search_channels[0]).to_numpy())
 
                 # Find circles to refine our button estimate unless we have a blank chamber.
                 circles = None
-                if assay.mark_tag[i, j] != "":
+                if assay.tag[i, j] != "":
                     # Filter the subimage to smooth edges and remove noise.
                     filtered = cv.bilateralFilter(
                         subimage,
                         d=9,
                         sigmaColor=75,
                         sigmaSpace=75,
                         borderType=cv.BORDER_DEFAULT,
@@ -295,16 +297,16 @@
                     closest_idx = np.argmin(np.linalg.norm(circles - point, axis=1))
                     assay.x[i, j, t], assay.y[i, j, t] = circles[closest_idx]
                     # Move the roi bounding box to the center the new x, y values.
                     top, bottom, left, right = utils.bounding_box(
                         round(float(assay.x[i, j, t])),
                         round(float(assay.y[i, j, t])),
                         self.roi_length,
-                        assay.sizes["im_y"],
                         assay.sizes["im_x"],
+                        assay.sizes["im_y"],
                     )
                     roi[i, j] = images[..., top:bottom, left:right]
                     # TODO: This step should occur over multiple channels.
                     subimage = utils.to_uint8(
                         roi[i, j].sel(channel=self.search_channels[0]).to_numpy()
                     )
 
@@ -376,186 +378,162 @@
             search_channel=search_channel,
         )
 
 
 class BeadFinder:
     def __init__(
         self,
-        min_bead_radius: int = 10,
-        max_bead_radius: int = 30,
+        min_bead_radius: int = 5,
+        max_bead_radius: int = 25,
         roi_length: int = 61,
-        param1: int = 50,
-        param2: int = 30,
     ):
         self.min_bead_radius = min_bead_radius
         self.max_bead_radius = max_bead_radius
         self.roi_length = roi_length
-        self.param1 = param1
-        self.param2 = param2
 
     def __call__(self, assay: xr.Dataset) -> xr.Dataset:
         if isinstance(assay.search_channel, str):
             if assay.search_channel in assay.channel:
                 search_channels = [assay.search_channel]
             elif assay.search_channel == "all":
                 search_channels = assay.channel
             else:
                 raise ValueError(f"{assay.search_channel} is not a channel name.")
         else:
             # We're searching across multiple channels.
             search_channels = assay.search_channel
 
         centers = np.empty((0, 2))
-        radii = np.empty((0))
+        labels = np.zeros((assay.sizes["im_y"], assay.sizes["im_x"]), dtype=int)
         for t in assay.time:
             for search_channel in search_channels:
                 image = utils.to_uint8(assay.image.sel(channel=search_channel, time=t).to_numpy())
-                # Filter the subimage to smooth edges and remove noise.
-                filtered = cv.bilateralFilter(
+                # Find a mask of all bright spots.
+                mask = cv.adaptiveThreshold(
                     image,
-                    d=9,
-                    sigmaColor=75,
-                    sigmaSpace=75,
-                    borderType=cv.BORDER_DEFAULT,
+                    maxValue=255,
+                    adaptiveMethod=cv.ADAPTIVE_THRESH_GAUSSIAN_C,
+                    thresholdType=cv.THRESH_BINARY,
+                    blockSize=2 * self.max_bead_radius + 1,
+                    C=-5,
                 )
-
-                # Find any circles in the image.
-                circles = cv.HoughCircles(
-                    filtered,
-                    method=cv.HOUGH_GRADIENT,
-                    dp=1,
-                    minDist=2 * self.min_bead_radius,
-                    param1=self.param1,
-                    param2=self.param2,
-                    minRadius=self.min_bead_radius,
-                    maxRadius=self.max_bead_radius,
+                # Find points far away from any dim spots.
+                dist = scipy.ndimage.distance_transform_edt(mask)
+                local_max = skimage.feature.peak_local_max(
+                    dist,
+                    min_distance=self.min_bead_radius,
+                    threshold_rel=self.min_bead_radius / self.max_bead_radius,
+                    labels=mask,
+                    footprint=np.ones((3, 3)),
                 )
+                max_mask = np.zeros(dist.shape, dtype=bool)
+                max_mask[tuple(local_max.T)] = True
 
-                if circles is not None:
-                    circles = circles[0]
-                    # Save circle center locations.
-                    c = circles[:, :2]
-                    if len(centers) > 0:
-                        # Remove centers too close to those we already found in another channel or time.
-                        dist_matrix = np.linalg.norm(c[np.newaxis] - centers[:, np.newaxis], axis=2)
-                        valid = np.min(dist_matrix, axis=0) > self.min_bead_radius
-                    else:
-                        valid = np.ones(len(circles), dtype=bool)
-
-                    centers = np.concatenate([centers, c[valid]])
-                    radii = np.concatenate([radii, circles[valid, 2]])
+                # Use watershed to separate touching beads.
+                markers = scipy.ndimage.label(max_mask)[0]
+                l = skimage.segmentation.watershed(-dist, markers, mask=mask)
+
+                # Exclude beads that we've already seen or that don't fit size criteria.
+                c = exclude_beads(l, labels, centers, self.min_bead_radius, self.max_bead_radius)
+                if len(c) > 0:
+                    centers = np.concatenate([centers, c])
 
         # Update the assay object with the beads we found.
-        if len(centers) > 0:
-            num_beads = len(centers)
-            # Create the array of subimage regions.
-            assay = assay.assign(
-                roi=(
-                    ("mark", "channel", "time", "roi_y", "roi_x"),
-                    np.empty(
-                        (
-                            num_beads,
-                            assay.dims["channel"],
-                            assay.dims["time"],
-                            self.roi_length,
-                            self.roi_length,
-                        ),
-                        dtype=assay.image.dtype,
+        num_beads = len(centers)
+        # Create the array of subimage regions.
+        assay = assay.assign(
+            roi=(
+                ("mark", "channel", "time", "roi_y", "roi_x"),
+                np.empty(
+                    (
+                        num_beads,
+                        assay.dims["channel"],
+                        assay.dims["time"],
+                        self.roi_length,
+                        self.roi_length,
                     ),
+                    dtype=assay.image.dtype,
                 ),
-                fg=(
-                    ("mark", "channel", "time", "roi_y", "roi_x"),
-                    np.empty(
-                        (
-                            num_beads,
-                            assay.dims["channel"],
-                            assay.dims["time"],
-                            self.roi_length,
-                            self.roi_length,
-                        ),
-                        dtype=bool,
+            ),
+            fg=(
+                ("mark", "channel", "time", "roi_y", "roi_x"),
+                np.empty(
+                    (
+                        num_beads,
+                        assay.dims["channel"],
+                        assay.dims["time"],
+                        self.roi_length,
+                        self.roi_length,
                     ),
+                    dtype=bool,
                 ),
-                bg=(
-                    ("mark", "channel", "time", "roi_y", "roi_x"),
-                    np.empty(
-                        (
-                            num_beads,
-                            assay.dims["channel"],
-                            assay.dims["time"],
-                            self.roi_length,
-                            self.roi_length,
-                        ),
-                        dtype=bool,
+            ),
+            bg=(
+                ("mark", "channel", "time", "roi_y", "roi_x"),
+                np.empty(
+                    (
+                        num_beads,
+                        assay.dims["channel"],
+                        assay.dims["time"],
+                        self.roi_length,
+                        self.roi_length,
                     ),
+                    dtype=bool,
                 ),
-            )
-            assay = assay.assign(
-                x=(
-                    ["mark", "time"],
-                    np.repeat(centers[:, np.newaxis, 0], assay.dims["time"], axis=1),
-                ),
-                y=(
-                    ["mark", "time"],
-                    np.repeat(centers[:, np.newaxis, 1], assay.dims["time"], axis=1),
-                ),
-            )
+            ),
+        )
+        assay = assay.assign(
+            x=(
+                ["mark", "time"],
+                np.repeat(centers[:, np.newaxis, 0], assay.dims["time"], axis=1),
+            ),
+            y=(
+                ["mark", "time"],
+                np.repeat(centers[:, np.newaxis, 1], assay.dims["time"], axis=1),
+            ),
+        )
 
-            rois = np.empty(assay.roi.shape, dtype=assay.roi.dtype)
-            fgs = np.empty(assay.roi.shape, dtype=bool)
-            bgs = np.empty(assay.roi.shape, dtype=bool)
-            image = assay.image.to_numpy()
-            # Compute the foreground and background masks for all buttons.
-            for i in range(num_beads):
-                # Set the subimage region for this bead.
-                top, bottom, left, right = utils.bounding_box(
-                    round(float(assay.x[i, 0])),
-                    round(float(assay.y[i, 0])),
-                    self.roi_length,
-                    image.shape[-2],
-                    image.shape[-1],
-                )
-                rois[i] = image[..., top:bottom, left:right]
+        rois = np.empty(assay.roi.shape, dtype=assay.roi.dtype)
+        fgs = np.empty(assay.roi.shape, dtype=bool)
+        bgs = np.empty(assay.roi.shape, dtype=bool)
+        image = assay.image.to_numpy()
+        # Compute the foreground and background masks for all buttons.
+        for i in range(num_beads):
+            # Set the subimage region for this bead.
+            top, bottom, left, right = utils.bounding_box(
+                round(float(assay.x[i, 0])),
+                round(float(assay.y[i, 0])),
+                self.roi_length,
+                assay.sizes["im_x"],
+                assay.sizes["im_y"],
+            )
+            rois[i] = image[..., top:bottom, left:right]
 
-                # Set the foreground of the bead to be the circle we found.
-                fg_mask = utils.circle(
-                    self.roi_length,
-                    row=round(float(assay.y[i, 0] - top)),
-                    col=round(float(assay.x[i, 0] - left)),
-                    radius=round(radii[i]),
-                    value=True,
-                )
+            # Set the foreground of the bead.
+            fgs[i] = labels[top:bottom, left:right] == i + 1
 
-                # Set the background to be everything else in the region,
-                # which could include other beads.
-                bg_mask = ~fg_mask
-
-                # Set the masked arrays with our computed masks.
-                fgs[i] = fg_mask
-                bgs[i] = bg_mask
+            # Set the background to be everything else in the region,
+            # which could include other beads.
+            bgs[i] = ~fgs[i]
 
         assay.fg[:] = fgs
         assay.bg[:] = bgs
         assay.roi[:] = rois
         return assay
 
     @registry.components.register("find_beads")
     def make(
-        min_bead_radius: int = 10,
-        max_bead_radius: int = 30,
+        min_bead_radius: int = 5,
+        max_bead_radius: int = 25,
         roi_length: int = 61,
-        param1: int = 50,
-        param2: int = 30,
     ):
         return BeadFinder(
             min_bead_radius=min_bead_radius,
             max_bead_radius=max_bead_radius,
             roi_length=roi_length,
-            param1=param1,
-            param2=param2,
         )
 
 
 def cluster_1d(
     points: np.ndarray,
     total_length: int,
     num_clusters: int,
@@ -642,7 +620,52 @@
             weight = min(len(x), ideal_num_points[i]) / ideal_num_points[i]
             intercepts[i] = weight * intercepts[i] + (1 - weight) * (intercept_m * i + intercept_b)
         else:
             # Just use our global estimate when we have an empty cluster.
             intercepts[i] = intercept_m * i + intercept_b
 
     return slope, intercepts
+
+
+@numba.jit(nopython=True)
+def exclude_beads(new_labels, labels, centers, min_bead_radius, max_bead_radius):
+    # Compute the area of each bead and their centers.
+    num_labels = new_labels.max()
+    pts = np.zeros((num_labels, 2))
+    areas = np.zeros(num_labels)
+    for i in range(new_labels.shape[0]):
+        for j in range(new_labels.shape[1]):
+            k = new_labels[i, j]
+            areas[k - 1] += 1
+            pts[k - 1, 0] += j
+            pts[k - 1, 1] += i
+    pts /= np.expand_dims(areas, axis=1)
+
+    # Mark valid beads.
+    old_max_label = labels.max()
+    curr_label = old_max_label + 1
+    label_idxs = np.zeros(num_labels)
+    new_centers = []
+    for i in range(num_labels):
+        if (areas[i] < np.pi * min_bead_radius**2) or (areas[i] > np.pi * max_bead_radius**2):
+            # Ignore incorrectly sized beads
+            continue
+        elif (
+            len(centers) > 0
+            and np.min(np.sqrt(np.sum((pts[i] - centers) ** 2, axis=1))) < 2 * min_bead_radius
+        ):
+            # Ignore beads we've already seen.
+            continue
+        else:
+            new_centers.append(pts[i])
+            label_idxs[i] = curr_label
+            curr_label += 1
+
+    # Update the global labels array.
+    for i in range(new_labels.shape[0]):
+        for j in range(new_labels.shape[1]):
+            k = new_labels[i, j]
+            if k != 0 and label_idxs[k - 1] != 0:
+                l = label_idxs[k - 1]
+                labels[i, j] = l
+
+    return new_centers
```

### Comparing `magnify-0.2.2/src/magnify/pipeline.py` & `magnify-0.3.0/src/magnify/pipeline.py`

 * *Files identical despite different names*

### Comparing `magnify-0.2.2/src/magnify/plot/image.py` & `magnify-0.3.0/src/magnify/plot/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from holoviews import opts
 import holoviews as hv
 import holoviews.operation.datashader as ds
 import xarray as xr
 
-from magnify.magniplot.ndplot import ndplot
+from magnify.plot.ndplot import ndplot
 
 
 def roishow(assay: xr.Dataset, grid=None, slider=None, rasterize=True, **kwargs):
     if grid is None and slider is None:
         slider = ["channel", "time"]
         grid = ["mark"]
 
     def imfunc(assay: xr.Dataset, **kwargs):
         img = hv.Image((assay.roi_x, assay.roi_y, assay.roi)).opts(**kwargs)
         return img
 
     plot = ndplot(assay, imfunc, grid=grid, slider=slider, **kwargs)
     plot = plot.opts(opts.Image(tools=["hover"]))
-    return ds.rasterize(plot) if rasterize else img
+    return ds.rasterize(plot) if rasterize else plot
 
 
 def imshow(assay: xr.Dataset, grid=None, slider=None, rasterize=True, compression_ratio=1, **kwargs):
     if grid is None and slider is None:
         slider = ["channel", "time"]
 
     def imfunc(assay: xr.Dataset, **kwargs):
@@ -35,15 +35,15 @@
             x = m.x.item()
             y = m.y.item()
             bounds.append(
                 hv.Bounds((m.x - len_x / 2, m.y + len_y / 2, m.x + len_x / 2, m.y - len_y / 2))
             )
 
             # Get the label for the bounding box.
-            tag = m.mark_tag.item()
+            tag = m.tag.item()
             row = m.mark_row.item()
             col = m.mark_col.item()
             labels.append((x, y - 0.55 * len_y, f"{tag} ({row}, {col})"))
 
         valid = assay.valid.to_numpy().flatten()
         img = assay.image[..., ::compression_ratio, ::compression_ratio]
         # Overlay image, bounding boxes, and labels.
```

### Comparing `magnify-0.2.2/src/magnify/plot/ndplot.py` & `magnify-0.3.0/src/magnify/plot/ndplot.py`

 * *Files identical despite different names*

### Comparing `magnify-0.2.2/src/magnify/plot/relation.py` & `magnify-0.3.0/src/magnify/plot/relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import holoviews as hv
 import numpy as np
 import plotly.express as px
 import scipy.stats
 import xarray as xr
 
 from magnify import utils
-from magnify.magniplot.ndplot import ndplot
+from magnify.plot.ndplot import ndplot
 
 
 def relplot(
     assay: xr.Dataset,
     x="time.seconds",
     y="tag_intensity",
     fit_method="linear",
```

### Comparing `magnify-0.2.2/src/magnify/plot/style.py` & `magnify-0.3.0/src/magnify/plot/style.py`

 * *Files identical despite different names*

### Comparing `magnify-0.2.2/src/magnify/postprocess.py` & `magnify-0.3.0/src/magnify/postprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,20 @@
     return assay.squeeze(drop=True)
 
 
 @registry.component("summarize_sum")
 def summarize_sum(assay: xr.Dataset):
     fg_area = assay.fg.sum(dim=["roi_x", "roi_y"]).compute()
     fg = assay.roi.where(assay.fg).sum(dim=["roi_x", "roi_y"]).compute()
-    bg = (assay.roi.where(assay.bg).isel(time=0).median(dim=["roi_x", "roi_y"]) * fg_area).compute()
+    bg = (assay.roi.where(assay.bg).median(dim=["roi_x", "roi_y"]) * fg_area).compute()
     assay["mark_intensity"] = fg - bg
 
     shape = (len(assay.tag),) + assay.image.shape[:2]
     tag_intensity = xr.DataArray(data=np.empty(shape), dims=("tag", "channel", "time"))
     for i, tag in enumerate(assay.tag):
-        subintensity = utils.sel_tag(fg, tag)  # - utils.sel_tag(bg, tag)
+        subintensity = utils.sel_tag(fg, tag) - utils.sel_tag(bg, tag)
         if tag != "":
             subintensity = subintensity.where(utils.sel_tag(assay.valid, tag))
         tag_intensity[i] = subintensity.mean(dim="mark")
 
     assay["tag_intensity"] = tag_intensity
     return assay
```

### Comparing `magnify-0.2.2/src/magnify/preprocess.py` & `magnify-0.3.0/src/magnify/preprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.2.2/src/magnify/reader.py` & `magnify-0.3.0/src/magnify/reader.py`

 * *Files 27% similar despite different names*

```diff
@@ -34,21 +34,31 @@
         times: Sequence[int] | None = None,
         channels: Sequence[str] | None = None,
     ) -> Iterator[xr.Dataset]:
         if isinstance(data, str):
             data = [data]
 
         for d in data:
-            path_dict, info_dict = extract_paths(d)
+            path_dict, meta_dict = extract_paths(
+                d, assay="str", channel="str", time="time", row="int", col="int"
+            )
             if len(path_dict) == 0:
                 raise FileNotFoundError(f"The pattern {d} did not lead to any files.")
 
-            for assay_name, assay_dict in sorted(
-                path_dict.items(), key=lambda x: utils.natural_sort_key(x[0])
-            ):
+            # None assay names should just mean a nameless assay.
+            path_dict = {("",) + k[1:] if k[0] is None else k: v for k, v in path_dict.items()}
+            assay_names = set(list(zip(*path_dict.keys()))[0])
+
+            for assay_name in sorted(assay_names, key=utils.natural_sort_key):
+                # Extract the paths for this assay and turn all Nones into -1 so sorting works.
+                assay_dict = {
+                    tuple(-1 if x is None else x for x in k[1:]): v
+                    for k, v in path_dict.items()
+                    if k[0] == assay_name
+                }
                 # Use these variables within the loop so we don't affect other assays.
                 channel_coords = channels
                 time_coords = times
 
                 # Get the indices specified in the path each in sorted order.
                 channel_idxs, time_idxs, row_idxs, col_idxs = (
                     sorted(set(idx)) for idx in zip(*assay_dict.keys())
@@ -184,25 +194,18 @@
 
                 coords = {}
                 # Set named coordinates for channels and times if they're available.
                 if channel_coords is not None:
                     coords["channel"] = channel_coords
                 if time_coords is not None:
                     coords["time"] = time_coords
-                # Get the indices specified in the info dict each in sorted order.
-                assay_info = info_dict[assay_name]
-                if assay_info:
-                    info_idxs, time_idxs = (sorted(set(idx)) for idx in zip(*assay_info.keys()))
-                    for info_idx in info_idxs:
-                        info_vals = [assay_info[(info_idx, time_idx)] for time_idx in time_idxs]
-                        coords[info_idx] = ("time", info_vals)
-
-                if "time" in coords:
-                    coords["time"] = pd.to_datetime(coords["time"])
-                    coords["time"] -= coords["time"][0]
+
+                # if "time" in coords:
+                #     coords["time"] = pd.to_datetime(coords["time"])
+                #     coords["time"] -= coords["time"][0]
 
                 # Put all our data into an xarray dataset.
                 assay = xr.Dataset(
                     {"tile": (dims_in_path + dims_in_file, tiles)},
                     coords=coords,
                     attrs={
                         "name": assay_name,
@@ -220,110 +223,109 @@
                 desired_order = ["channel", "time", "tile_row", "tile_col", "tile_y", "tile_x"]
                 for dim in desired_order:
                     if dim not in assay.tile.dims:
                         assay["tile"] = assay.tile.expand_dims(dim)
 
                 assay = assay.transpose(*desired_order)
 
+                # Add any metadata coodinates specified by the user.
+                for (meta_name, dim), meta_idxs_dict in meta_dict.items():
+                    if dim == "time":
+                        # Make sure we're indexing using datetimes.
+                        dim_idxs = assay[dim] = pd.to_datetime(assay[dim])
+                    else:
+                        dim_idxs = assay[dim].values
+
+                    meta_idxs = [meta_idxs_dict[dim_idx] for dim_idx in dim_idxs]
+                    assay = assay.assign_coords({meta_name: (dim, meta_idxs)})
+
+                # Make sure the time dimension starts at 0 seconds.
+                assay = assay.assign_coords(time=assay.time - assay.time[0])
+
                 yield assay
 
     @registry.readers.register("read")
     def make():
         return Reader()
 
 
-@registry.component("read_pinlist")
-def read_pinlist(assay, pinlist, blank=None):
-    if blank is None:
-        blank = ["", "blank", "BLANK"]
-
-    df = pd.read_csv(pinlist)
-    df["Indices"] = df["Indices"].apply(
-        lambda s: [int(x) for x in re.sub(r"[\(\)]", "", s).split(",")]
-    )
-    # Replace blanks with the empty string.
-    df["MutantID"] = df["MutantID"].replace(blank, "")
-    # Zero-index the indices.
-    cols, rows = np.array(df["Indices"].to_list()).T - 1
-    names = df["MutantID"].to_numpy(dtype=str, na_value="")
-    names_array = np.empty((max(rows) + 1, max(cols) + 1), dtype=names.dtype)
-    names_array[rows, cols] = names
-    assay = assay.assign_coords(tag=np.unique(names_array))
-    assay = assay.assign_coords(mark_tag=(("mark_row", "mark_col"), names_array))
-    assay["valid"] = (
-        ("mark_row", "mark_col", "time"),
-        np.ones(
-            (assay.sizes["mark_row"], assay.sizes["mark_col"], assay.sizes["time"]), dtype=bool
-        ),
-    )
-    return assay
-
+def extract_paths(pattern, **kwargs) -> dict[tuple[int, str, int, int], str]:
+    default_formatters = {
+        "": lambda x, y: x,
+        "str": lambda x, y: x,
+        "time": lambda x, y: datetime.datetime.strptime(x, y if y else "%Y%m%d-%H%M%S"),
+        "int": lambda x, y: int(x),
+        "float": lambda x, y: float(x),
+    }
+
+    keys = kwargs
+    # Make sure keys is always a dict whose values are formatting functions.
+    if not isinstance(keys, dict):
+        keys = {key: "str" for key in keys}
+    keys = {k: f if callable(f) else default_formatters[f] for k, f in keys.items()}
+    all_keys = list(keys)
 
-def extract_paths(pattern) -> dict[tuple[int, str, int, int], str]:
+    # Format the pattern so we can do a glob search and so we can use it to extract
+    # filename metadata using regexes.
     pattern = os.path.expanduser(pattern)
+    meta = collections.defaultdict(dict)
+    glob_path = pattern
+    regex_path = fnmatch.translate(pattern)
+    for key, formatter in list(keys.items()):
+        # For globs replace all named search patterns e.g.: (time|%S) with the wildcard *.
+        glob_path = re.sub(rf"\({key}.*?\)", "*", glob_path)
+        glob_path = re.sub(rf"\(.*?_{key}.*?\)", "*", glob_path)
+        # For regexes replace all named search patterns with named wildcard groups.
+        regex_path = re.sub(rf"\\\({key}.*?\\\)", rf"(?P<{key}>.*?)", regex_path)
+        regex_path = re.sub(rf"\\\((.*?)_{key}.*?\\\)", r"(?P<\1>.*?)", regex_path)
+
+        # Get any associated formatting information in the named search pattern.
+        key_search = re.search(rf"\({key}(?:\s*\|\s*(.*?))?\)", pattern)
+        if key_search:
+            format_str = key_search.group(1)
+            # Rebind the function, we need to set default argument values because of closure rules.
+            keys[key] = lambda x, y=format_str, f=formatter: f(x, y)
+        else:
+            # Remove keys that weren't specified in the pattern.
+            del keys[key]
 
-    # Filter out special signifiers used for pattern matching.
-    glob_path = pattern.replace("(assay)", "*")
-    glob_path = glob_path.replace("(channel)", "*")
-    glob_path = re.sub(r"\(time\s*\|?.*?\)", "*", glob_path)
-    glob_path = glob_path.replace("(row)", "*")
-    glob_path = glob_path.replace("(col)", "*")
-    glob_path = re.sub(r"\(info\s*=\s*.*?\)", "*", glob_path)
+        # Get meta information that provides alternate value mappings for a given key
+        # along with any formatting information e.g. (concentration_time|float).
+        meta_search = re.findall(rf"\((.*?)_{key}(?:\s*\|\s*(.*?))?(?:\s*\|\s*(.*?))?\)", pattern)
+        for name, formatter_str, format_str in meta_search:
+            meta_formatter = default_formatters[formatter_str]
+            # Once again we need to set default arguments because of closure rules in Python.
+            meta_formatter = lambda x, y=format_str, f=meta_formatter: f(x, y)
+            meta[key][name] = meta_formatter
 
+    regex_path = re.compile(regex_path, re.IGNORECASE)
     # Search for files matching the pattern.
     paths = glob.glob(glob_path, recursive=True)
 
-    regex_path = fnmatch.translate(pattern)
-    regex_path = regex_path.replace("\\(assay\\)", "(?P<assay>.*?)")
-    regex_path = regex_path.replace("\\(channel\\)", "(?P<channel>.*?)")
-    regex_path = re.sub(r"\\\(time\s*\|?.*?\\\)", r"(?P<time>.*?)", regex_path)
-    regex_path = regex_path.replace("\\(row\\)", "(?P<row>.*?)")
-    regex_path = regex_path.replace("\\(col\\)", "(?P<col>.*?)")
-    regex_path = re.sub(r"\\\(info\s*=\s*(.*?)\\\)", r"(?P<\1>.*?)", regex_path)
-    regex_path = re.compile(regex_path, re.IGNORECASE)
-
-    path_dict = collections.defaultdict(dict)
-    info_dict = collections.defaultdict(dict)
+    path_dict = {}
+    meta_dict = collections.defaultdict(dict)
     for path in paths:
         match = regex_path.fullmatch(path)
-        if "(assay)" in pattern:
-            assay = match.group("assay")
+        idxs = []
+        for key in all_keys:
+            if key in keys:
+                # First get the value for the given key for the current path.
+                idx = match.group(key)
+                formatter = keys[key]
+                idx = formatter(idx)
+                idxs.append(idx)
+                # Then get all the associated metadata for that key.
+                for name, formatter in meta[key].items():
+                    meta_idx = match.group(name)
+                    meta_dict[name, key][idx] = formatter(meta_idx)
+            else:
+                # If the key wasn't specified in the pattern we still include it in the idxs.
+                idxs.append(None)
+
+        # Keep track of which indices correspond to which paths.
+        idxs = tuple(idxs)
+        if idxs not in path_dict:
+            path_dict[idxs] = os.path.abspath(path)
         else:
-            assay = ""
-
-        if "(channel)" in pattern:
-            channel = match.group("channel")
-        else:
-            channel = -1
-
-        time_search = re.search(r"\(time\s*\|?\s*(.*?)\)", pattern)
-        if time_search:
-            format_str = time_search.group(1)
-            if not format_str:
-                format_str = "%Y%m%d-%H%M%S"
-            time_str = match.group("time")
-            time = datetime.datetime.strptime(time_str, format_str)
-        else:
-            time = -1
-
-        if "(row)" in pattern:
-            row = int(match.group("row"))
-        else:
-            row = -1
-
-        if "(col)" in pattern:
-            col = int(match.group("col"))
-        else:
-            col = -1
-
-        idx = (channel, time, row, col)
-        if idx not in path_dict[assay]:
-            path_dict[assay][idx] = os.path.abspath(path)
-        else:
-            raise ValueError(f"{path} and {path_dict[assay][idx]} map to the same index.")
-
-        info_search = re.search(r"\(info\s*=\s*(.*?)\)", pattern)
-        if info_search:
-            for info in info_search.groups():
-                info_dict[assay][info, time] = match.group(info)
+            raise ValueError(f"{path} and {path_dict[idxs]} map to the same index.")
 
-    return path_dict, info_dict
+    return path_dict, meta_dict
```

### Comparing `magnify-0.2.2/src/magnify/registry.py` & `magnify-0.3.0/src/magnify/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,58 +46,57 @@
 
 def ps_chip_pipeline(**kwargs):
     # Button centers are apart 375um vertically and 655um horizontally.
     # Assuming a 4x objective and 2x2 binning each pixel is 3.22um.
     defaults = confection.Config(dict(row_dist=375 / 3.22, col_dist=655 / 3.22))
     config = defaults.merge(confection.Config(kwargs))
     pipe = Pipeline("read", config=config)
-    pipe.add_pipe("read_pinlist")
-    # pipe.add_pipe("preprocessor")
+    pipe.add_pipe("identify_buttons")
     pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("find_buttons")
-    # pipe.add_pipe("background_filter")
     pipe.add_pipe("filter_expression")
     pipe.add_pipe("filter_nonround")
     pipe.add_pipe("filter_leaky")
-    pipe.add_pipe("summarize_sum")
+    # pipe.add_pipe("summarize_sum")
     pipe.add_pipe("squeeze")
 
     return pipe
 
 
 def pc_chip_pipeline(**kwargs):
     # Button centers are apart 412um vertically and 760um horizontally.
     # Assuming a 4x objective and 2x2 binning each pixel is 3.22um.
     defaults = confection.Config(dict(row_dist=412 / 3.22, col_dist=760 / 3.22))
     config = defaults.merge(confection.Config(kwargs))
     pipe = Pipeline("read", config=config)
-    pipe.add_pipe("read_pinlist")
-    # pipe.add_pipe("preprocessor")
+    pipe.add_pipe("identify_buttons")
     pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("find_buttons")
-    # pipe.add_pipe("background_filter")
     pipe.add_pipe("filter_expression")
     pipe.add_pipe("filter_nonround")
     pipe.add_pipe("filter_leaky")
-    pipe.add_pipe("summarize_sum")
+    # pipe.add_pipe("summarize_sum")
     pipe.add_pipe("squeeze")
 
     return pipe
 
 
 def mrbles_pipeline(**kwargs):
     pipe = Pipeline("read", config=kwargs)
     pipe.add_pipe("flatfield_correct")
+    # pipe.add_pipe("horizontal_flip")
+    pipe.add_pipe("vertical_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("find_beads")
-    # pipe.add_pipe("background_filter")
+    pipe.add_pipe("identify_mrbles")
+    # pipe.add_pipe("summarize_sum")
     pipe.add_pipe("squeeze")
 
     return pipe
 
 
 def imread_pipeline(**kwargs):
     pipe = Pipeline("read", config=kwargs)
```

### Comparing `magnify-0.2.2/src/magnify/stitch.py` & `magnify-0.3.0/src/magnify/stitch.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from magnify.registry import components
 
 
 class Stitcher:
     def __init__(self, overlap: int = 102):
         self.overlap = overlap
 
-    def __call__(self, assay: xr.Dataset, overlap=102) -> xr.Dataset:
-        self.overlap = overlap
+    def __call__(self, assay: xr.Dataset) -> xr.Dataset:
         tiles = assay.tile[..., : -self.overlap, : -self.overlap]
         # Move the time and channel axes last so we can focus on joining images.
         tiles = tiles.transpose("tile_row", "tile_col", "tile_y", "tile_x", "channel", "time")
         tiles = xr.concat(tiles, dim="tile_y")
         images = xr.concat(tiles, dim="tile_x")
         # Change the x and y dimension names to be about the images.
         images = images.rename(tile_y="im_y", tile_x="im_x")
```

### Comparing `magnify-0.2.2/src/magnify/utils.py` & `magnify-0.3.0/src/magnify/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import xarray as xr
 
 
 def sel_tag(assay: xr.Dataset, tag: str):
     if "mark_row" in assay.dims:
         assay = assay.stack(mark=("mark_row", "mark_col"))
         assay = assay.transpose("mark", ...)
-    idxs = np.where(assay.mark_tag == tag)
+    idxs = np.where(assay.tag == tag)
     return assay.isel(mark=idxs[0])
 
 
 def to_uint8(arr: np.ndarray) -> np.ndarray:
     arr = arr.astype(float)
     arr = 255 * arr / np.max(arr)
     return arr.astype(np.uint8)
```

### Comparing `magnify-0.2.2/PKG-INFO` & `magnify-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnify
-Version: 0.2.2
+Version: 0.3.0
 Summary: A microscopy image processing toolkit.
 Author: Karl Krauth
 Author-email: karl.krauth@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,16 @@
 Requires-Dist: confection (>=0.0.4,<0.0.5)
 Requires-Dist: dask[complete] (>=2022.02.0)
 Requires-Dist: lxml (>=4.6.0,<5.0.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: opencv-python (>=4.0) ; sys_platform != "darwin"
 Requires-Dist: opencv-python (>=4.0,!=4.7.0.68) ; sys_platform == "darwin"
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
+Requires-Dist: scikit-image (>=0.2.0,<0.3.0)
+Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Requires-Dist: tifffile (>=2021.11.2)
 Requires-Dist: tqdm (>=4.64,<5.0)
 Requires-Dist: types-tqdm (>=4.64,<5.0)
 Requires-Dist: xarray[complete] (>=2023.01.0)
 Description-Content-Type: text/markdown
```

