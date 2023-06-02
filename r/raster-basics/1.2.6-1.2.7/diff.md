# Comparing `tmp/raster_basics-1.2.6.tar.gz` & `tmp/raster_basics-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_basics-1.2.6.tar", last modified: Thu Mar  2 22:40:01 2023, max compression
+gzip compressed data, was "raster_basics-1.2.7.tar", last modified: Fri Jun  2 17:24:20 2023, max compression
```

## Comparing `raster_basics-1.2.6.tar` & `raster_basics-1.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-03-02 22:40:01.567415 raster_basics-1.2.6/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-03-02 22:40:01.567485 raster_basics-1.2.6/PKG-INFO
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-03-02 22:40:01.566219 raster_basics-1.2.6/raster_basics/
--rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.2.6/raster_basics/BaseFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    42093 2023-02-28 15:52:24.000000 raster_basics-1.2.6/raster_basics/DataPlots.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    15302 2023-03-02 19:25:28.000000 raster_basics-1.2.6/raster_basics/GlacierFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    12176 2023-02-28 19:45:54.000000 raster_basics-1.2.6/raster_basics/RasterBasics.py
--rwxrwxrwx   0 albinwells   (501) staff       (20)    11730 2023-03-02 22:38:38.000000 raster_basics-1.2.6/raster_basics/SmoothingFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.2.6/raster_basics/__init__.py
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-03-02 22:40:01.567287 raster_basics-1.2.6/raster_basics.egg-info/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-03-02 22:40:01.000000 raster_basics-1.2.6/raster_basics.egg-info/PKG-INFO
--rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-03-02 22:40:01.000000 raster_basics-1.2.6/raster_basics.egg-info/SOURCES.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-03-02 22:40:01.000000 raster_basics-1.2.6/raster_basics.egg-info/dependency_links.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-03-02 22:40:01.000000 raster_basics-1.2.6/raster_basics.egg-info/not-zip-safe
--rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-03-02 22:40:01.000000 raster_basics-1.2.6/raster_basics.egg-info/top_level.txt
--rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-03-02 22:40:01.567836 raster_basics-1.2.6/setup.cfg
--rw-rw-r--   0 albinwells   (501) staff       (20)      376 2023-03-02 22:39:00.000000 raster_basics-1.2.6/setup.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-02 17:24:20.629250 raster_basics-1.2.7/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-02 17:24:20.629320 raster_basics-1.2.7/PKG-INFO
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-02 17:24:20.628334 raster_basics-1.2.7/raster_basics/
+-rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.2.7/raster_basics/BaseFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.2.7/raster_basics/DataPlots.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    17696 2023-06-02 17:21:57.000000 raster_basics-1.2.7/raster_basics/GlacierFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.2.7/raster_basics/RasterBasics.py
+-rwxrwxrwx   0 albinwells   (501) staff       (20)    11730 2023-03-02 22:38:38.000000 raster_basics-1.2.7/raster_basics/SmoothingFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.2.7/raster_basics/__init__.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-02 17:24:20.629129 raster_basics-1.2.7/raster_basics.egg-info/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/PKG-INFO
+-rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/not-zip-safe
+-rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/top_level.txt
+-rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-02 17:24:20.629607 raster_basics-1.2.7/setup.cfg
+-rw-rw-r--   0 albinwells   (501) staff       (20)      400 2023-06-02 17:23:58.000000 raster_basics-1.2.7/setup.py
```

### Comparing `raster_basics-1.2.6/raster_basics/BaseFunctions.py` & `raster_basics-1.2.7/raster_basics/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.6/raster_basics/DataPlots.py` & `raster_basics-1.2.7/raster_basics/DataPlots.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,26 +597,26 @@
     	plt.show(block=False)
     	figName = plotTitle.replace(' ', '_') + '.png'
     	fig.savefig(figName, dpi=250)
     	# Image.open(figName).show()
     else:
     	plt.show()
 
-def velPlot(vx, vy, v_tot, area, threshold):
+def velPlot(vx, vy, v_tot, pixel_size, threshold):
     '''
     Show velocity vector arrows
     :param vx1: x-direction velocity
     :param vy1: y-direction velocity
     :param v_tot: magnitude of velocity
     :param pixel_size: pixel size (for density of vectors)
     :param threshold: velocity magnitude threshold for showing arrows
     :return:
     '''
     # fig, ax = plt.subplots()                                  # uncomment lines to plot this graph separately
-    if area/1000000 > 10:
+    if pixel_size < 10:
         freq = 20
     else:
         freq = 10
     xx = np.arange(0, vx.shape[1], freq)                          # last number represents arrow frequency
     yy = np.arange(0, vy.shape[0], freq)
     points = np.ix_(yy, xx)
     px, py = np.meshgrid(xx, yy)
```

### Comparing `raster_basics-1.2.6/raster_basics/GlacierFunctions.py` & `raster_basics-1.2.7/raster_basics/GlacierFunctions.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import rasterio.mask
 import earthpy.spatial as es
 import richdem as rd
 import numpy as np
 import math
 import matplotlib.pyplot as plt
 from scipy import stats
-from raster_basics.SmoothingFunctions import dynamicSmoothing
+from shapely.geometry import Point
+from raster_basics.SmoothingFunctions import dynamicSmoothing, dynamicSmoothingExponential
 
 
 def glacierArea(outline, res):
     """
 	Area of a glacier
 		outline: glacier outline, binary array with 1 denoting on-glacier terrain and 0 denoting off-glacier terrain (array-like)
 		res: raster resolution (int or float)
@@ -50,33 +51,40 @@
 		res: pixel resolution (int or float)
 		vCol: vertical-average velocity scaling factor, typically 0.8 (int or float)
     """
     divQarray = ((np.gradient(vx, res)[1] * h) + (np.gradient(h, res)[1] * vx) +
                   (np.gradient(vy * -1, res)[0] * h) + (np.gradient(h * -1, res)[0] * vy)) * vCol
     return divQarray
     
-def flux_div_comps(vx, vy, h, res, vCol=0.8, filt=True, filter_factor=4):
+def flux_div_comps(vx, vy, h, res, vCol=0.8, filt=True, filter_type='Gauss', filter_factor=4):
     """
-	Flux divergence - return each component as well
-		vx, vy: x- and y-direction velocity, m/yr (array-like)
-		h: glacier thickness, m (array-like)
-		res: pixel resolution (int or float)
-		vCol: vertical-average velocity scaling factor, typically 0.8 (int or float)
-		filter: whether or not to smooth derivatives
-		filter_factor: smoothing factor for filtering
+    Flux divergence - return each component as well
+	vx, vy: x- and y-direction velocity, m/yr (array-like)
+	h: glacier thickness, m (array-like)
+	res: pixel resolution (int or float)
+	vCol: vertical-average velocity scaling factor, typically 0.8 (int or float)
+	filt: whether or not to smooth derivatives
+	filter_type: type of filter, either 'Gauss' or 'Exp'
+	filter_factor: smoothing factor for filtering
     """
     dvx = (np.gradient(vx, res)[1] * h) * vCol
     dvy = (np.gradient(vy * -1, res)[0] * h) * vCol
     dhx = (np.gradient(h, res)[1] * vx) * vCol
     dhy = (np.gradient(h * -1, res)[0] * vy) * vCol
     if filt == True:
-        dvx = dynamicSmoothing(dvx, h, res, filter_factor)
-        dvy = dynamicSmoothing(dvy, h, res, filter_factor)
-        dhx = dynamicSmoothing(dhx, h, res, filter_factor)
-        dhy = dynamicSmoothing(dhy, h, res, filter_factor)
+        if filter_type == 'Gauss':
+            dvx = dynamicSmoothing(dvx, h, res, filter_factor)
+            dvy = dynamicSmoothing(dvy, h, res, filter_factor)
+            dhx = dynamicSmoothing(dhx, h, res, filter_factor)
+            dhy = dynamicSmoothing(dhy, h, res, filter_factor)
+        elif filter_type == 'Exp':
+            dvx = dynamicSmoothingExponential(dvx, h, res, filter_factor)
+            dvy = dynamicSmoothingExponential(dvy, h, res, filter_factor)
+            dhx = dynamicSmoothingExponential(dhx, h, res, filter_factor)
+            dhy = dynamicSmoothingExponential(dhy, h, res, filter_factor)
     divQ = dvx + dvy + dhx + dhy
     return divQ, dvx, dvy, dhx, dhy
 
 
 def glacierAttributes(dem_rast, attrFormat):
     # return desired attribute (attrFormat is 'slope_degree' or 'slope_percentage', 'slope_riserun', 'aspect')
     # https://richdem.readthedocs.io/en/latest/python_api.html#richdem.rdarray
@@ -129,14 +137,49 @@
                 pixel_aspect = abs(pixel_deg) + 90
             elif pixel_deg > 90:
                 pixel_aspect = 450 - pixel_deg
             aspect_array[i][j] = pixel_aspect
     return aspect_array
 
 
+def velFlowlineAspect(linestring, array, arr_extent):
+    '''
+    Use flowline as velocity direction. Returns array of aspects, based on the flowline.
+    # linestring: center flowline json object. Type: shapely.geometry.linestring.LineString
+    # array: 2D numpy array, output aspect will be the same size
+    # arr_extent: Array extent in shapely geometry coordinates (left, bottom, right, top)
+    '''
+    aspect_array = np.zeros_like(array)
+    x, y = np.meshgrid(np.arange(arr_extent[0], arr_extent[2]+1), np.arange(arr_extent[1], arr_extent[3]+1))
+    
+    # iterate through velocity array
+    for i in tqdm(range(len(array))): 
+        for j in range(len(array[0])):
+            point = Point(x[i,j], y[i,j]) # find our point in json coordinates
+            closest_point = linestring.interpolate(linestring.project(point)) # find the nearest point on linestring
+            coords = np.array(linestring.coords)
+            dists = np.linalg.norm(coords - closest_point.coords, axis=1)
+            closest_idx = np.argmin(dists) # find the index of the closest point on the line
+
+            if closest_idx == 0: # check if nearest point is endpoint
+                prev_point = coords[closest_idx]
+                next_point = coords[closest_idx + 2]
+            elif closest_idx == len(np.array(linestring.coords)) - 1:
+                prev_point = coords[closest_idx - 2]
+                next_point = coords[closest_idx]
+            else:
+                prev_point = coords[closest_idx - 1]
+                next_point = coords[closest_idx + 1]
+
+            # angle of perpendicular line -- perpendicular line is -1/m, so we input (-x, y) instead of (y, x)
+            aspect_angle = np.rad2deg(np.arctan2(prev_point[0] - next_point[0], next_point[1] - prev_point[1]))
+            aspect_array[i][j] = aspect_angle # add to array of aspects
+    return aspect_array
+
+
 def velocityAspect(vel_x, vel_y):
     # gets the aspect of velocity vectors, given input x- and y-direction velocity arrays
     vel_aspect = np.zeros_like(vel_x)
     for i in range(len(vel_aspect)):
         for j in range(len(vel_aspect[0])):
             pixel_deg = math.atan2(vel_y[i][j], vel_x[i][j]) * 180 / math.pi
             if pixel_deg >= 0 and pixel_deg <= 90:
```

### Comparing `raster_basics-1.2.6/raster_basics/RasterBasics.py` & `raster_basics-1.2.7/raster_basics/RasterBasics.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     """
 	Clip a geotiff with a shapefile
 		geotiff: input raster to clip (str) (e.g. 'input.tif')
 		shapefile: shapefile used for clipping (str) (e.g. 'input_shape.shp')
 		destination: output clipped raster filename (str) (e.g. 'output.tif')
 		nan_val: NaN value (int or float)
 		fill: If True, the pixels outside the features will be set to nan_val. If False, the output array will contain the original pixel data, and only the mask will be based on shapes (boolean) 
-		pad_size: width of padding in pixels (int or float)    
+		pad_size: width of padding in pixels (int or float)
+		crop: whether to crop the raster to the extent of the shapes
     """
     
     with rasterio.open(geotiff) as src:
         # we need to make a temporary shapefile with the same crs as the geotiff 
         shpReprojection(shapefile, src.crs, dst='temp.shp')
         with fiona.open('temp.shp', 'r') as openshape:
             shapes = [feature['geometry'] for feature in openshape]
```

### Comparing `raster_basics-1.2.6/raster_basics/SmoothingFunctions.py` & `raster_basics-1.2.7/raster_basics/SmoothingFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.6/raster_basics/__init__.py` & `raster_basics-1.2.7/raster_basics/__init__.py`

 * *Files identical despite different names*

