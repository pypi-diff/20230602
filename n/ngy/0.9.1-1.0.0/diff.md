# Comparing `tmp/ngy-0.9.1.tar.gz` & `tmp/ngy-1.0.0.tar.gz`

## Comparing `ngy-0.9.1.tar` & `ngy-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 ngy-0.9.1/examples/request_exemple.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Magic_Request.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Magic_Request_sav.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Map_func.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Request.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Tiles.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/__init__.py
--rw-r--r--   0        0        0  2564345 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/data/wmts.xml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ngy-0.9.1/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ngy-0.9.1/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ngy-0.9.1/README.md
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ngy-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ngy-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 ngy-1.0.0/examples/request_exemple.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 ngy-1.0.0/src/ngy/Magic_Request.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ngy-1.0.0/src/ngy/Magic_Request_sav.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 ngy-1.0.0/src/ngy/Map_func.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 ngy-1.0.0/src/ngy/Request.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ngy-1.0.0/src/ngy/Tiles.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 ngy-1.0.0/src/ngy/Tools.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ngy-1.0.0/src/ngy/__init__.py
+-rw-r--r--   0        0        0  2564345 2020-02-02 00:00:00.000000 ngy-1.0.0/src/ngy/data/wmts.xml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ngy-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ngy-1.0.0/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 ngy-1.0.0/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 ngy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 ngy-1.0.0/PKG-INFO
```

### Comparing `ngy-0.9.1/src/ngy/Magic_Request.py` & `ngy-1.0.0/src/ngy/Magic_Request.py`

 * *Files identical despite different names*

### Comparing `ngy-0.9.1/src/ngy/Magic_Request_sav.py` & `ngy-1.0.0/src/ngy/Magic_Request_sav.py`

 * *Files identical despite different names*

### Comparing `ngy-0.9.1/src/ngy/Map_func.py` & `ngy-1.0.0/src/ngy/Map_func.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,21 +41,25 @@
 # Get all information about tile sets
 MATRIX_SET_DATA = get_scale_denom_info(WMTS_FILE_PATH)
 
 def convert_coord(long_lat, matrix_data, zoom, projection):
     """convert decimals coords into Web Mercator coords into tile coords"""
     # See https://geoservices.ign.fr/documentation/geoservices/wmts.html
 
-    long_lat_ref = pyproj.Proj(init='epsg:4326')
+    #proj_4326 = pyproj.Proj(init='epsg:4326')
 
-    final_proj = pyproj.Proj(init=matrix_data[projection]['supportedcrs'])
+    #final_proj = pyproj.Proj(init=matrix_data[projection]['supportedcrs'])
+
+    transformer = pyproj.Transformer.from_crs('EPSG:4326', matrix_data[projection]['supportedcrs'])
     tile_res = matrix_data[projection][str(zoom)] * 256  # 256 pixel per tile
 
     # Web Mercator
-    (x, y) = pyproj.transform(long_lat_ref, final_proj, long_lat[0], long_lat[1])
+    #(x, y) = pyproj.transform(proj_4326, final_proj, long_lat[0], long_lat[1])
+    (x, y) = transformer.transform( long_lat[1], long_lat[0])
+
 
     # Get the top left corner
     (x0, y0) = (matrix_data[projection]['X_ref'], matrix_data[projection]['Y_ref'])
 
     # Tile coords depending on matrix_data (see get_scale_denom_info function)
     (xf, yf) = (int((x - x0) / tile_res), int((y0 - y) / tile_res))
     # ("Zoom: " + str(zoom) + " Tile Rez: " + str(tile_res) + " X,Y: " + str(xf) + "," + str(yf))
```

### Comparing `ngy-0.9.1/src/ngy/Request.py` & `ngy-1.0.0/src/ngy/Request.py`

 * *Files identical despite different names*

### Comparing `ngy-0.9.1/src/ngy/Tiles.py` & `ngy-1.0.0/src/ngy/Tiles.py`

 * *Files identical despite different names*

### Comparing `ngy-0.9.1/src/ngy/data/wmts.xml` & `ngy-1.0.0/src/ngy/data/wmts.xml`

 * *Files identical despite different names*

### Comparing `ngy-0.9.1/LICENSE` & `ngy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ngy-0.9.1/pyproject.toml` & `ngy-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 [project]
 name = "ngy"
-version = "0.9.1"
+version = "1.0.0"
 authors = [
   { name="Sébastien LAUTIER", email="sebastien.lautier@gmail.com" },
 ]
 description = "Create MBTiles from IGN maps"
 readme = "README.md"
 requires-python = ">=3.10.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "aiohttp>=3.8.4",
-    "aiosignal>=1.3.1",
-    "async-timeout>=4.0.2",
-    "attrs>=23.1.0",
-    "certifi>=2023.5.7",
-    "charset-normalizer>=3.1.0",
-    "colorama>=0.4.6",
-    "frozenlist>=1.3.3",
-    "idna>=3.4",
     "lxml>=4.9.2",
-    "multidict>=6.0.4",
     "pyproj>=3.5.0",
     "tqdm>=4.65.0",
-    "yarl>=1.9.2"
+    "fire>=0.5.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sebastien17/ngy"
 "Bug Tracker" = "https://github.com/sebastien17/ngy/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[project.scripts]
+locus = "ngy.Tools:__execute_locus"
+
 [tool.hatch.build]
 include = [
 ]
 exclude = [
   "requirements.txt"
 ]
```

