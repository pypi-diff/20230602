# Comparing `tmp/ngy-0.9.0.tar.gz` & `tmp/ngy-0.9.1.tar.gz`

## Comparing `ngy-0.9.0.tar` & `ngy-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 ngy-0.9.0/examples/request_exemple.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 ngy-0.9.0/src/NGY/Magic_Request.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ngy-0.9.0/src/NGY/Magic_Request_sav.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 ngy-0.9.0/src/NGY/Map_func.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 ngy-0.9.0/src/NGY/Request.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ngy-0.9.0/src/NGY/Tiles.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ngy-0.9.0/src/NGY/__init__.py
--rw-r--r--   0        0        0  2564345 2020-02-02 00:00:00.000000 ngy-0.9.0/src/NGY/data/wmts.xml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ngy-0.9.0/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ngy-0.9.0/LICENSE
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ngy-0.9.0/README.md
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ngy-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 ngy-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 ngy-0.9.1/examples/request_exemple.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Magic_Request.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Magic_Request_sav.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Map_func.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Request.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/Tiles.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/__init__.py
+-rw-r--r--   0        0        0  2564345 2020-02-02 00:00:00.000000 ngy-0.9.1/src/ngy/data/wmts.xml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ngy-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ngy-0.9.1/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ngy-0.9.1/README.md
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ngy-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ngy-0.9.1/PKG-INFO
```

### Comparing `ngy-0.9.0/src/NGY/Magic_Request.py` & `ngy-0.9.1/src/ngy/Magic_Request.py`

 * *Files identical despite different names*

### Comparing `ngy-0.9.0/src/NGY/Magic_Request_sav.py` & `ngy-0.9.1/src/ngy/Magic_Request_sav.py`

 * *Files identical despite different names*

### Comparing `ngy-0.9.0/src/NGY/Map_func.py` & `ngy-0.9.1/src/ngy/Map_func.py`

 * *Files identical despite different names*

### Comparing `ngy-0.9.0/src/NGY/Request.py` & `ngy-0.9.1/src/ngy/Request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-import NGY.Map_func
-import NGY.Magic_Request
-import NGY.Tiles
+import ngy.Map_func
+import ngy.Magic_Request
+import ngy.Tiles
 from urllib.parse import urlencode
 import sqlite3
 import os
 
 
 class Request:
 
@@ -49,21 +49,21 @@
             'Service': 'WMTS',
             'Request': 'GetTile',
             'Version': '1.0.0',
             'Format': 'image/' + self.format
         }
 
         for k in self.zoom_list:
-            top_left_corner = NGY.Map_func.Coord._make(
-                NGY.Map_func.convert_coord((min(self.bounds[0], self.bounds[2]), max(self.bounds[1], self.bounds[3])),
-                                           NGY.Map_func.MATRIX_SET_DATA, k, self.projection))
-
-            bot_right_corner = NGY.Map_func.Coord._make(
-                NGY.Map_func.convert_coord((max(self.bounds[0], self.bounds[2]), min(self.bounds[1], self.bounds[3])),
-                                           NGY.Map_func.MATRIX_SET_DATA, k, self.projection))
+            top_left_corner = ngy.Map_func.Coord._make(
+                ngy.Map_func.convert_coord((min(self.bounds[0], self.bounds[2]), max(self.bounds[1], self.bounds[3])),
+                                           ngy.Map_func.MATRIX_SET_DATA, k, self.projection))
+
+            bot_right_corner = ngy.Map_func.Coord._make(
+                ngy.Map_func.convert_coord((max(self.bounds[0], self.bounds[2]), min(self.bounds[1], self.bounds[3])),
+                                           ngy.Map_func.MATRIX_SET_DATA, k, self.projection))
 
             def url_build(i, j, zoom):
                 _values = _default_value
                 _values['TileCol'] = i
                 _values['TileRow'] = j
                 _values['TileMatrix'] = zoom
                 return self._base_url + '?' + urlencode(_values)
@@ -71,19 +71,19 @@
             for j in range(top_left_corner.lat, bot_right_corner.lat + 1):
                 for i in range(top_left_corner.lon, bot_right_corner.lon + 1):
                     self._request_list.append({'x': i, 'y': j, 'z': k, 'url': url_build(i, j, k)})
 
     def fetch_data(self):
         if not self._request_list:
             self._build_request_list()
-        _data = NGY.Magic_Request.async_req([_item['url'] for _item in self._request_list], headers=self._headers)
+        _data = ngy.Magic_Request.async_req([_item['url'] for _item in self._request_list], headers=self._headers)
         # TODO : To optimize
         _temp = list(zip(self._request_list, _data))
-        _temp2 = [NGY.Tiles.Tile(_item[0]['x'], _item[0]['y'], _item[0]['z'], _item[1], format=self.format) for _item in _temp]
-        self._tile_set = NGY.Tiles.Tileset(_temp2)
+        _temp2 = [ngy.Tiles.Tile(_item[0]['x'], _item[0]['y'], _item[0]['z'], _item[1], format=self.format) for _item in _temp]
+        self._tile_set = ngy.Tiles.Tileset(_temp2)
 
     def save(self, file, name, meta=None ):
         # See https://github.com/mapbox/mbtiles-spec/blob/master/1.3/spec.md
         _format_trans = dict(jpeg="jpg", png="png", pbf="pbf", webp="webp")
         _meta = dict(name=name,
                      format=_format_trans[self.format],
                      bounds=", ".join(str(v) for v in self.bounds),
```

### Comparing `ngy-0.9.0/src/NGY/Tiles.py` & `ngy-0.9.1/src/ngy/Tiles.py`

 * *Files identical despite different names*

### Comparing `ngy-0.9.0/src/NGY/data/wmts.xml` & `ngy-0.9.1/src/ngy/data/wmts.xml`

 * *Files identical despite different names*

### Comparing `ngy-0.9.0/LICENSE` & `ngy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ngy-0.9.0/pyproject.toml` & `ngy-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ngy"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
   { name="Sébastien LAUTIER", email="sebastien.lautier@gmail.com" },
 ]
 description = "Create MBTiles from IGN maps"
 readme = "README.md"
 requires-python = ">=3.10.11"
 classifiers = [
```

### Comparing `ngy-0.9.0/PKG-INFO` & `ngy-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Create MBTiles from IGN maps
 Project-URL: Homepage, https://github.com/sebastien17/ngy
 Project-URL: Bug Tracker, https://github.com/sebastien17/ngy/issues
 Author-email: Sébastien LAUTIER <sebastien.lautier@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Requires-Dist: multidict>=6.0.4
 Requires-Dist: pyproj>=3.5.0
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: yarl>=1.9.2
 Description-Content-Type: text/markdown
 
 # ngy
-Create MBTiles  from IGN maps
+Create MBTiles from IGN maps
 
 ## Installation
 Compatible with Python 3.10 +
 
 pip install ngy
 
 ## Usage
```

