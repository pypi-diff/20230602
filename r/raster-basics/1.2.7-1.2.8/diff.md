# Comparing `tmp/raster_basics-1.2.7.tar.gz` & `tmp/raster_basics-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_basics-1.2.7.tar", last modified: Fri Jun  2 17:24:20 2023, max compression
+gzip compressed data, was "raster_basics-1.2.8.tar", last modified: Fri Jun  2 17:27:47 2023, max compression
```

## Comparing `raster_basics-1.2.7.tar` & `raster_basics-1.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-02 17:24:20.629250 raster_basics-1.2.7/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-02 17:24:20.629320 raster_basics-1.2.7/PKG-INFO
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-02 17:24:20.628334 raster_basics-1.2.7/raster_basics/
--rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.2.7/raster_basics/BaseFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.2.7/raster_basics/DataPlots.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    17696 2023-06-02 17:21:57.000000 raster_basics-1.2.7/raster_basics/GlacierFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.2.7/raster_basics/RasterBasics.py
--rwxrwxrwx   0 albinwells   (501) staff       (20)    11730 2023-03-02 22:38:38.000000 raster_basics-1.2.7/raster_basics/SmoothingFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.2.7/raster_basics/__init__.py
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-02 17:24:20.629129 raster_basics-1.2.7/raster_basics.egg-info/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/PKG-INFO
--rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/SOURCES.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/dependency_links.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/not-zip-safe
--rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-02 17:24:20.000000 raster_basics-1.2.7/raster_basics.egg-info/top_level.txt
--rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-02 17:24:20.629607 raster_basics-1.2.7/setup.cfg
--rw-rw-r--   0 albinwells   (501) staff       (20)      400 2023-06-02 17:23:58.000000 raster_basics-1.2.7/setup.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-02 17:27:47.757835 raster_basics-1.2.8/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-02 17:27:47.757900 raster_basics-1.2.8/PKG-INFO
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-02 17:27:47.756567 raster_basics-1.2.8/raster_basics/
+-rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.2.8/raster_basics/BaseFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.2.8/raster_basics/DataPlots.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    17690 2023-06-02 17:27:11.000000 raster_basics-1.2.8/raster_basics/GlacierFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.2.8/raster_basics/RasterBasics.py
+-rwxrwxrwx   0 albinwells   (501) staff       (20)    11730 2023-03-02 22:38:38.000000 raster_basics-1.2.8/raster_basics/SmoothingFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.2.8/raster_basics/__init__.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-02 17:27:47.757703 raster_basics-1.2.8/raster_basics.egg-info/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-02 17:27:47.000000 raster_basics-1.2.8/raster_basics.egg-info/PKG-INFO
+-rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-02 17:27:47.000000 raster_basics-1.2.8/raster_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-02 17:27:47.000000 raster_basics-1.2.8/raster_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-02 17:27:47.000000 raster_basics-1.2.8/raster_basics.egg-info/not-zip-safe
+-rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-02 17:27:47.000000 raster_basics-1.2.8/raster_basics.egg-info/top_level.txt
+-rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-02 17:27:47.758187 raster_basics-1.2.8/setup.cfg
+-rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-02 17:27:22.000000 raster_basics-1.2.8/setup.py
```

### Comparing `raster_basics-1.2.7/raster_basics/BaseFunctions.py` & `raster_basics-1.2.8/raster_basics/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.7/raster_basics/DataPlots.py` & `raster_basics-1.2.8/raster_basics/DataPlots.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.7/raster_basics/GlacierFunctions.py` & `raster_basics-1.2.8/raster_basics/GlacierFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     # array: 2D numpy array, output aspect will be the same size
     # arr_extent: Array extent in shapely geometry coordinates (left, bottom, right, top)
     '''
     aspect_array = np.zeros_like(array)
     x, y = np.meshgrid(np.arange(arr_extent[0], arr_extent[2]+1), np.arange(arr_extent[1], arr_extent[3]+1))
     
     # iterate through velocity array
-    for i in tqdm(range(len(array))): 
+    for i in range(len(array)): 
         for j in range(len(array[0])):
             point = Point(x[i,j], y[i,j]) # find our point in json coordinates
             closest_point = linestring.interpolate(linestring.project(point)) # find the nearest point on linestring
             coords = np.array(linestring.coords)
             dists = np.linalg.norm(coords - closest_point.coords, axis=1)
             closest_idx = np.argmin(dists) # find the index of the closest point on the line
```

### Comparing `raster_basics-1.2.7/raster_basics/RasterBasics.py` & `raster_basics-1.2.8/raster_basics/RasterBasics.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.7/raster_basics/SmoothingFunctions.py` & `raster_basics-1.2.8/raster_basics/SmoothingFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.7/raster_basics/__init__.py` & `raster_basics-1.2.8/raster_basics/__init__.py`

 * *Files identical despite different names*

