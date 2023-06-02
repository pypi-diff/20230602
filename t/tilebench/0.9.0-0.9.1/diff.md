# Comparing `tmp/tilebench-0.9.0.tar.gz` & `tmp/tilebench-0.9.1.tar.gz`

## Comparing `tilebench-0.9.0.tar` & `tilebench-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 tilebench-0.9.0/CHANGES.md
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 tilebench-0.9.0/README.md
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 tilebench-0.9.0/tilebench/__init__.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 tilebench-0.9.0/tilebench/middleware.py
--rw-r--r--   0        0        0    10773 2020-02-02 00:00:00.000000 tilebench-0.9.0/tilebench/viz.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tilebench-0.9.0/tilebench/resources/__init__.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 tilebench-0.9.0/tilebench/resources/responses.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tilebench-0.9.0/tilebench/scripts/__init__.py
--rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 tilebench-0.9.0/tilebench/scripts/cli.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 tilebench-0.9.0/tilebench/static/spherical-mercator.js
--rw-r--r--   0        0        0    16549 2020-02-02 00:00:00.000000 tilebench-0.9.0/tilebench/templates/index.html
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 tilebench-0.9.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tilebench-0.9.0/LICENSE
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 tilebench-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 tilebench-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 tilebench-0.9.1/CHANGES.md
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 tilebench-0.9.1/README.md
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 tilebench-0.9.1/tilebench/__init__.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 tilebench-0.9.1/tilebench/middleware.py
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 tilebench-0.9.1/tilebench/viz.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tilebench-0.9.1/tilebench/resources/__init__.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 tilebench-0.9.1/tilebench/resources/responses.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tilebench-0.9.1/tilebench/scripts/__init__.py
+-rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 tilebench-0.9.1/tilebench/scripts/cli.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 tilebench-0.9.1/tilebench/static/spherical-mercator.js
+-rw-r--r--   0        0        0    18115 2020-02-02 00:00:00.000000 tilebench-0.9.1/tilebench/templates/index.html
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 tilebench-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tilebench-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 tilebench-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    11882 2020-02-02 00:00:00.000000 tilebench-0.9.1/PKG-INFO
```

### Comparing `tilebench-0.9.0/CHANGES.md` & `tilebench-0.9.1/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 
+## 0.9.1 (2023-03-24)
+
+* handle dateline crossing dataset and remove pydantic serialization
+
 ## 0.9.0 (2023-03-14)
 
 * update pre-commit and fix issue with starlette>=0.26
 * re-write `NoCacheMiddleware` as pure ASGI middleware
 * rename `analyse_logs` to `parse_logs`
 * add python 3.11 support
```

### Comparing `tilebench-0.9.0/README.md` & `tilebench-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tilebench-0.9.0/tilebench/__init__.py` & `tilebench-0.9.1/tilebench/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tilebench."""
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 import cProfile
 import json
 import logging
 import pstats
 import sys
 import time
```

### Comparing `tilebench-0.9.0/tilebench/middleware.py` & `tilebench-0.9.1/tilebench/middleware.py`

 * *Files identical despite different names*

### Comparing `tilebench-0.9.0/tilebench/viz.py` & `tilebench-0.9.1/tilebench/viz.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 import attr
 import morecantile
 import numpy
 import rasterio
 import uvicorn
 from fastapi import APIRouter, FastAPI, Query
 from fastapi.staticfiles import StaticFiles
-from geojson_pydantic.features import Feature, FeatureCollection
 from rasterio import windows
 from rasterio._path import _parse_path as parse_path
 from rasterio.crs import CRS
-from rasterio.vrt import WarpedVRT
 from rasterio.warp import calculate_default_transform, transform_geom
 from rio_tiler.io import BaseReader, Reader
 from rio_tiler.utils import render
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, Response
 from starlette.templating import Jinja2Templates
 
@@ -35,34 +33,76 @@
 tms = morecantile.tms.get("WebMercatorQuad")
 WGS84_CRS = CRS.from_epsg(4326)
 
 
 def bbox_to_feature(
     bbox: Tuple[float, float, float, float],
     properties: Optional[Dict] = None,
-) -> Feature:
+) -> Dict:
     """Create a GeoJSON feature polygon from a bounding box."""
-    return Feature(
-        **{
-            "geometry": {
-                "type": "Polygon",
-                "coordinates": [
-                    [
-                        [bbox[0], bbox[3]],
-                        [bbox[0], bbox[1]],
-                        [bbox[2], bbox[1]],
-                        [bbox[2], bbox[3]],
-                        [bbox[0], bbox[3]],
-                    ]
-                ],
+    # Dateline crossing dataset
+    if bbox[0] > bbox[2]:
+        bounds_left = [-180, bbox[1], bbox[2], bbox[3]]
+        bounds_right = [bbox[0], bbox[1], 180, bbox[3]]
+
+        features = [
+            {
+                "geometry": {
+                    "type": "Polygon",
+                    "coordinates": [
+                        [
+                            [bounds_left[0], bounds_left[3]],
+                            [bounds_left[0], bounds_left[1]],
+                            [bounds_left[2], bounds_left[1]],
+                            [bounds_left[2], bounds_left[3]],
+                            [bounds_left[0], bounds_left[3]],
+                        ]
+                    ],
+                },
+                "properties": properties or {},
+                "type": "Feature",
             },
-            "properties": {} or properties,
-            "type": "Feature",
-        }
-    )
+            {
+                "geometry": {
+                    "type": "Polygon",
+                    "coordinates": [
+                        [
+                            [bounds_right[0], bounds_right[3]],
+                            [bounds_right[0], bounds_right[1]],
+                            [bounds_right[2], bounds_right[1]],
+                            [bounds_right[2], bounds_right[3]],
+                            [bounds_right[0], bounds_right[3]],
+                        ]
+                    ],
+                },
+                "properties": properties or {},
+                "type": "Feature",
+            },
+        ]
+    else:
+        features = [
+            {
+                "geometry": {
+                    "type": "Polygon",
+                    "coordinates": [
+                        [
+                            [bbox[0], bbox[3]],
+                            [bbox[0], bbox[1]],
+                            [bbox[2], bbox[1]],
+                            [bbox[2], bbox[3]],
+                            [bbox[0], bbox[3]],
+                        ]
+                    ],
+                },
+                "properties": properties or {},
+                "type": "Feature",
+            },
+        ]
+
+    return {"type": "FeatureCollection", "features": features}
 
 
 def dims(total: int, chop: int):
     """Given a total number of pixels, chop into equal chunks.
 
     yeilds (offset, size) tuples
     >>> list(dims(512, 256))
@@ -153,53 +193,49 @@
             response.headers[
                 "server-timing"
             ] = f"dataread; dur={round(t.elapsed * 1000, 2)}"
             return "OK"
 
         @self.router.get(
             r"/info.geojson",
-            response_model=Feature,
             response_model_exclude_none=True,
             response_class=GeoJSONResponse,
         )
         def info():
             """Return a geojson."""
-            with rasterio.open(self.src_path) as src_dst:
-                width, height = src_dst.width, src_dst.height
+            with Reader(self.src_path) as src_dst:
+                width, height = src_dst.dataset.width, src_dst.dataset.height
 
                 info = {
                     "width": width,
                     "height": height,
                 }
+                info["bounds"] = src_dst.geographic_bounds
 
-                with WarpedVRT(src_dst, crs="epsg:4326") as vrt:
-                    geographic_bounds = list(vrt.bounds)
-
-                info["bounds"] = geographic_bounds
+                info["crs"] = src_dst.dataset.crs.to_epsg()
 
-                info["crs"] = src_dst.crs.to_epsg()
-                ovr = src_dst.overviews(1)
+                ovr = src_dst.dataset.overviews(1)
                 info["overviews"] = len(ovr)
                 dst_affine, _, _ = calculate_default_transform(
-                    src_dst.crs,
+                    src_dst.dataset.crs,
                     tms.crs,
                     width,
                     height,
-                    *src_dst.bounds,
+                    *src_dst.dataset.bounds,
                 )
                 resolution = max(abs(dst_affine[0]), abs(dst_affine[4]))
                 zoom = tms.zoom_for_res(resolution)
                 info["maxzoom"] = zoom
 
                 ifd = [
                     {
                         "Level": 0,
                         "Width": width,
                         "Height": height,
-                        "Blocksize": src_dst.block_shapes[0],
+                        "Blocksize": src_dst.dataset.block_shapes[0],
                         "Decimation": 0,
                         "MercatorZoom": zoom,
                         "MercatorResolution": resolution,
                     }
                 ]
 
             for ix, decim in enumerate(ovr):
@@ -229,15 +265,14 @@
             info["ifd"] = ifd
             info["minzoom"] = zoom  # either the same has maxzoom or last IFD
 
             return bbox_to_feature(info["bounds"], properties=info)
 
         @self.router.get(
             r"/tiles.geojson",
-            response_model=FeatureCollection,
             response_model_exclude_none=True,
             response_class=GeoJSONResponse,
         )
         def grid(ovr_level: int = Query(...)):
             """return geojson."""
             options = {"OVERVIEW_LEVEL": ovr_level - 1} if ovr_level else {}
             with rasterio.open(self.src_path, **options) as src_dst:
@@ -245,28 +280,26 @@
                 blockxsize, blockysize = src_dst.block_shapes[0]
                 winds = (
                     windows.Window(col_off=col_off, row_off=row_off, width=w, height=h)
                     for row_off, h in dims(src_dst.height, blockysize)
                     for col_off, w in dims(src_dst.width, blockxsize)
                 )
                 for window in winds:
-                    geom = bbox_to_feature(
-                        windows.bounds(window, src_dst.transform)
-                    ).geometry.dict()
-                    geom = transform_geom(src_dst.crs, WGS84_CRS, geom)
-                    feats.append(
-                        {
-                            "type": "Feature",
-                            "geometry": geom,
-                            "properties": {"window": str(window)},
-                        }
-                    )
+                    fc = bbox_to_feature(windows.bounds(window, src_dst.transform))
+                    for feat in fc.get("features", []):
+                        geom = transform_geom(src_dst.crs, WGS84_CRS, feat["geometry"])
+                        feats.append(
+                            {
+                                "type": "Feature",
+                                "geometry": geom,
+                                "properties": {"window": str(window)},
+                            }
+                        )
 
-            grids = {"type": "FeatureCollection", "features": feats}
-            return grids
+            return {"type": "FeatureCollection", "features": feats}
 
         @self.router.get(
             "/",
             responses={200: {"description": "Simple COG viewer."}},
             response_class=HTMLResponse,
         )
         async def viewer(request: Request):
```

### Comparing `tilebench-0.9.0/tilebench/scripts/cli.py` & `tilebench-0.9.1/tilebench/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `tilebench-0.9.0/tilebench/static/spherical-mercator.js` & `tilebench-0.9.1/tilebench/static/spherical-mercator.js`

 * *Files identical despite different names*

### Comparing `tilebench-0.9.0/tilebench/templates/index.html` & `tilebench-0.9.1/tilebench/templates/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -104,15 +104,15 @@
           </div>
         </div>
       </div>
       <div class="zoom-info"><span id="zoom"></span></div>
     </div>
 
     <script>
-    const scope = {data: undefined}
+    const scope = {metadata: undefined}
     const merc = new SphericalMercator({ size: 256 });
 
     const info_endpoint = '{{ geojson_endpoint }}'
     const grid_endpoint = '{{ grid_endpoint }}'
     const image_endpoint = '{{ image_endpoint }}'
 
     var map = new maplibregl.Map({
@@ -168,15 +168,19 @@
             index += b.toString();
         }
         return index;
     }
 
     // return a geojson of Mercator Tiles for a bbox and zoom
     var mercator_grid = (zoom) => {
-        const extrema = merc.xyz(scope.data.properties.bounds, zoom);
+        let bounds = scope.metadata.bounds
+        if (bounds[0] > bounds[2]) {
+            bounds[0] = bounds[0] - 360
+        }
+        const extrema = merc.xyz(bounds, zoom);
 
         const featCollection = {
             'type': 'FeatureCollection',
             'features': [],
         }
 
         for (var x = extrema.minX, maxX = extrema.maxX + 1; x < maxX; x++) {
@@ -236,15 +240,15 @@
 
         fetch(info_endpoint)
             .then(res => {
                 if (res.ok) return res.json()
                 throw new Error('Network response was not ok.');
             })
             .then(data => {
-                scope.data = data
+                scope.metadata = data.features[0].properties
 
                 map.addSource('aoi', {
                     'type': 'geojson',
                     'data': data
                 })
                 map.addLayer({
                     id: 'aoi-polygon',
@@ -257,43 +261,75 @@
                     paint: {
                         'line-color': '#000000',
                         'line-dasharray': [3, 3],
                         'line-width': 1
                     }
                 })
 
-                const bounds = data.properties.bounds
-                const ll = truncate_lnglat(bounds[0], bounds[1])
-                const ur = truncate_lnglat(bounds[2], bounds[3])
-                map.fitBounds([ll, ur])
+                let crossing_dateline = false
+                let bounds = [...scope.metadata.bounds]
+                // Bounds crossing dateline
+                if (bounds[0] > bounds[2]) {
+                    crossing_dateline = true
+                    bounds[0] = bounds[0] - 360
+                }
+                map.fitBounds(
+                    [[bounds[0], bounds[1]], [bounds[2], bounds[3]]]
+                )
+
+                if (crossing_dateline) {
+                    // 2 sources and 2 layers
+                    // left
+                    map.addSource('raster-l', {
+                    type: 'raster',
+                    bounds: [-180, bounds[1], bounds[2], bounds[3]],
+                    minzoom: scope.metadata.minzoom,
+                    maxzoom: scope.metadata.minzoom,
+                    tiles: [image_endpoint],
+                    tileSize: 256 // This might be false but it's not in TileJSON
+                    })
+                    map.addLayer({id: 'raster-l', type: 'raster', source: 'raster-l', paint: {'raster-opacity': 0.6}})
 
-                map.addSource('raster', {
+                    //right
+                    map.addSource('raster-r', {
                     type: 'raster',
+                    bounds: [bounds[0], bounds[1], 180, bounds[3]],
+                    minzoom: scope.metadata.minzoom,
+                    maxzoom: scope.metadata.minzoom,
                     tiles: [image_endpoint],
-                    tileSize: 256,
-                    bounds: data.properties.bounds,
-                    minzoom: data.properties.minzoom,
-                    maxzoom: data.properties.minzoom  // THIS IS ON PURPOSE, We don't really need high resolution tiles
-                })
-                map.addLayer({id: 'raster', type: 'raster', source: 'raster', paint: {'raster-opacity': 0.6}})
+                    tileSize: 256 // This might be false but it's not in TileJSON
+                    })
+                    map.addLayer({id: 'raster-r', type: 'raster', source: 'raster-r', paint: {'raster-opacity': 0.6}})
+
+                } else {
+                    map.addSource('raster', {
+                    type: 'raster',
+                    bounds: bounds,
+                    minzoom: scope.metadata.minzoom,
+                    maxzoom: scope.metadata.minzoom, // THIS IS ON PURPOSE, We don't really need high resolution tiles
+                    tiles: [image_endpoint],
+                    tileSize: 256 // This might be false but it's not in TileJSON
+                    })
+                    map.addLayer({id: 'raster', type: 'raster', source: 'raster', paint: {'raster-opacity': 0.6}})
+                }
 
                 const sel = document.getElementById('ovr-selector')
-                const novr = data.properties.ifd.length
+                const novr = scope.metadata.ifd.length
 
                 for (var i = 0; i < novr; i++) {
                     let l = document.createElement('option')
-                    ifd = data.properties.ifd[i]
+                    ifd = scope.metadata.ifd[i]
                     l.setAttribute('level', ifd.Level)
                     l.setAttribute('zoom', ifd.MercatorZoom)
                     l.text = `Level: ${ifd.Level} (Zoom ${ifd.MercatorZoom})`
                     sel.appendChild(l)
                     if (i === novr - 1) l.selected = "selected"
                 }
-                document.getElementById('raster-crs').innerText = `CRS: epsg:${scope.data.properties["crs"]}`
-                document.getElementById('raster-size').innerText = `Size: ${scope.data.properties["height"]}x${scope.data.properties["width"]}`
+                document.getElementById('raster-crs').innerText = `CRS: epsg:${scope.metadata.crs}`
+                document.getElementById('raster-size').innerText = `Size: ${scope.metadata.height}x${scope.metadata.width}`
 
                 return update_viz()
             })
             .catch(err => {
                 console.warn(err)
             })
             .then(() => {
@@ -368,18 +404,18 @@
                     console.warn(err)
                 })
         }
 
         const update_viz = () => {
             const level = parseInt(document.getElementById('ovr-selector').selectedOptions[0].getAttribute("level"))
             const zoom = parseInt(document.getElementById('ovr-selector').selectedOptions[0].getAttribute("zoom"))
-            add_mercator_grid(scope.data.properties.ifd[level])
-            add_tile_grid(scope.data.properties.ifd[level])
+            add_mercator_grid(scope.metadata.ifd[level])
+            add_tile_grid(scope.metadata.ifd[level])
             document.getElementById('res-gmaps').innerText = ((2 * merc.MAXEXTENT) / merc.Ac[zoom]).toFixed(4)
-            document.getElementById('res-merc').innerText = scope.data.properties.ifd[level]["MercatorResolution"].toFixed(4)
+            document.getElementById('res-merc').innerText = scope.metadata.ifd[level]["MercatorResolution"].toFixed(4)
         }
 
         document.getElementById('ovr-selector').addEventListener('change', (e) => {
             update_viz()
         })
 
         map.on('mousemove', (e) => {
```

### Comparing `tilebench-0.9.0/.gitignore` & `tilebench-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tilebench-0.9.0/LICENSE` & `tilebench-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tilebench-0.9.0/pyproject.toml` & `tilebench-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tilebench-0.9.0/PKG-INFO` & `tilebench-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilebench
-Version: 0.9.0
+Version: 0.9.1
 Summary: Inspect HEAD/LIST/GET requests withing Rasterio
 Project-URL: Homepage, https://github.com/developmentseed/tilebench
 Project-URL: Issues, https://github.com/developmentseed/tilebench/issues
 Project-URL: Source, https://github.com/developmentseed/tilebench
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -305,14 +305,18 @@
 ## Changes
 
 See [CHANGES.md](https://github.com/developmentseed/tilebench/blob/main/CHANGES.md).
 
 ## Changelog
 
 
+## 0.9.1 (2023-03-24)
+
+* handle dateline crossing dataset and remove pydantic serialization
+
 ## 0.9.0 (2023-03-14)
 
 * update pre-commit and fix issue with starlette>=0.26
 * re-write `NoCacheMiddleware` as pure ASGI middleware
 * rename `analyse_logs` to `parse_logs`
 * add python 3.11 support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tilebench Version: 0.9.0 Summary: Inspect HEAD/
+Metadata-Version: 2.1 Name: tilebench Version: 0.9.1 Summary: Inspect HEAD/
 LIST/GET requests withing Rasterio Project-URL: Homepage, https://github.com/
 developmentseed/tilebench Project-URL: Issues, https://github.com/
 developmentseed/tilebench/issues Project-URL: Source, https://github.com/
 developmentseed/tilebench Author-email: Vincent Sarago
 developmentseed.com> License-Expression: MIT License-File: LICENSE Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -106,34 +106,35 @@
 Verifying PEP257 Compliance..............................................Passed
 mypy.....................................................................Passed
 $ git push origin ``` ## License See [LICENSE](https://github.com//
 developmentseed/tilebench/blob/main/LICENSE) ## Authors See [contributors]
 (https://github.com/developmentseed/tilebench/graphs/contributors) for a
 listing of individual contributors. ## Changes See [CHANGES.md](https://
 github.com/developmentseed/tilebench/blob/main/CHANGES.md). ## Changelog ##
-0.9.0 (2023-03-14) * update pre-commit and fix issue with starlette>=0.26 * re-
-write `NoCacheMiddleware` as pure ASGI middleware * rename `analyse_logs` to
-`parse_logs` * add python 3.11 support ## 0.8.2 (2022-11-21) * update hatch
-config ## 0.8.1 (2022-10-31) * fix issue with min/max zoom when there is no
-overviews * calculate windows from block_shapes ## 0.8.0 (2022-10-25) * update
-rio-tiler/rasterio dependencies * remove python 3.7 support * add python 3.10
-support * add image endpoint to show the data footprint * switch from mapbox to
-maplibre ## 0.7.0 (2022-06-14) * add `cProfile` stats ## 0.6.1 (2022-04-19) *
-Remove usage of `VSIStatsMiddleware` in `tilebench viz` ## 0.6.0 (2022-04-19) *
-switch to pyproject.toml ## 0.5.1 (2022-03-04) * make sure we don't cache
-previous request when using `tilebench profile` without `--tile` option ##
-0.5.0 (2022-02-28) * update rio-tiler requirement * add `reader` option ##
-0.4.1 (2022-02-14) * update Fastapi requirement * use WarpedVRT to get dataset
-bounds in epsg:4326 ## 0.4.0 (2021-12-13) * update rio-tiler's version
-requirement * add more information about the raster in the Viz web page (author
-[@drnextgis](https://github.com/drnextgis), https://github.com/developmentseed/
-tilebench/pull/14) * fix bug for latest GDAL/rasterio version * add default
-STAMEN basemap in *viz* and remove mapbox token/style options. * update fastapi
-requirement ## 0.3.0 (2021-03-05) * add `exclude_paths` options in
-`VSIStatsMiddleware` to exclude some endpoints (author [@drnextgis](https://
+0.9.1 (2023-03-24) * handle dateline crossing dataset and remove pydantic
+serialization ## 0.9.0 (2023-03-14) * update pre-commit and fix issue with
+starlette>=0.26 * re-write `NoCacheMiddleware` as pure ASGI middleware * rename
+`analyse_logs` to `parse_logs` * add python 3.11 support ## 0.8.2 (2022-11-21)
+* update hatch config ## 0.8.1 (2022-10-31) * fix issue with min/max zoom when
+there is no overviews * calculate windows from block_shapes ## 0.8.0 (2022-10-
+25) * update rio-tiler/rasterio dependencies * remove python 3.7 support * add
+python 3.10 support * add image endpoint to show the data footprint * switch
+from mapbox to maplibre ## 0.7.0 (2022-06-14) * add `cProfile` stats ## 0.6.1
+(2022-04-19) * Remove usage of `VSIStatsMiddleware` in `tilebench viz` ## 0.6.0
+(2022-04-19) * switch to pyproject.toml ## 0.5.1 (2022-03-04) * make sure we
+don't cache previous request when using `tilebench profile` without `--tile`
+option ## 0.5.0 (2022-02-28) * update rio-tiler requirement * add `reader`
+option ## 0.4.1 (2022-02-14) * update Fastapi requirement * use WarpedVRT to
+get dataset bounds in epsg:4326 ## 0.4.0 (2021-12-13) * update rio-tiler's
+version requirement * add more information about the raster in the Viz web page
+(author [@drnextgis](https://github.com/drnextgis), https://github.com/
+developmentseed/tilebench/pull/14) * fix bug for latest GDAL/rasterio version *
+add default STAMEN basemap in *viz* and remove mapbox token/style options. *
+update fastapi requirement ## 0.3.0 (2021-03-05) * add `exclude_paths` options
+in `VSIStatsMiddleware` to exclude some endpoints (author [@drnextgis](https://
 github.com/drnextgis), https://github.com/developmentseed/tilebench/pull/10) *
 renamed `ressources` to `resources` ## 0.2.1 (2021-02-19) * fix typo in UI ##
 0.2.0 (2021-01-28) * add warp-kernels in output in `profile` CLI * add
 rasterio/curl stdout in output * add dataread time in Viz ## 0.1.1 (2021-01-27)
 * update requirements ## 0.1.0 (2021-01-04) * add web UI for VSI stats
 visualization * add starlette middleware ## 0.0.2 (2020-12-15) * Update for
 rio-tiler==2.0.0rc3 ## 0.1.0 (2020-07-13) * Initial release
```

