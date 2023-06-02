# Comparing `tmp/boson_sdk-0.1.0-py3-none-any.whl.zip` & `tmp/boson_sdk-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 20274 bytes, number of entries: 15
--rw-r--r--  2.0 unx      749 b- defN 23-Jun-01 20:32 boson/__init__.py
--rw-r--r--  2.0 unx     3157 b- defN 23-Jun-01 20:32 boson/base.py
--rw-r--r--  2.0 unx     5320 b- defN 23-Jun-01 20:32 boson/boson_v1_pb2.py
--rw-r--r--  2.0 unx     3714 b- defN 23-Jun-01 20:32 boson/conversion.py
--rw-r--r--  2.0 unx     8496 b- defN 23-Jun-01 20:32 boson/features_pb2.py
--rw-r--r--  2.0 unx       57 b- defN 23-Jun-01 20:32 boson/grpc/__init__.py
--rw-r--r--  2.0 unx     5518 b- defN 23-Jun-01 20:32 boson/grpc/boson_v1_pb2_grpc.py
--rw-r--r--  2.0 unx     2159 b- defN 23-Jun-01 20:32 boson/grpc/server.py
--rw-r--r--  2.0 unx       57 b- defN 23-Jun-01 20:32 boson/http/__init__.py
--rw-r--r--  2.0 unx     2568 b- defN 23-Jun-01 20:32 boson/http/server.py
--rw-r--r--  2.0 unx    11356 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    14911 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1168 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/RECORD
-15 files, 59328 bytes uncompressed, 18362 bytes compressed:  69.1%
+Zip file size: 20577 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      749 b- defN 23-Jun-02 01:49 boson/__init__.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-Jun-02 01:49 boson/base.py
+-rw-r--r--  2.0 unx     5320 b- defN 23-Jun-02 01:49 boson/boson_v1_pb2.py
+-rw-r--r--  2.0 unx     3576 b- defN 23-Jun-02 01:49 boson/conversion.py
+-rw-r--r--  2.0 unx     8496 b- defN 23-Jun-02 01:49 boson/features_pb2.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-02 01:49 boson/grpc/__init__.py
+-rw-r--r--  2.0 unx     5518 b- defN 23-Jun-02 01:49 boson/grpc/boson_v1_pb2_grpc.py
+-rw-r--r--  2.0 unx     2159 b- defN 23-Jun-02 01:49 boson/grpc/server.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-02 01:49 boson/http/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-Jun-02 01:49 boson/http/server.py
+-rw-r--r--  2.0 unx    11356 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14911 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1168 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/RECORD
+15 files, 60242 bytes uncompressed, 18665 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: boson/http/__init__.py
 Comment: 
 
 Filename: boson/http/server.py
 Comment: 
 
-Filename: boson_sdk-0.1.0.dist-info/LICENSE
+Filename: boson_sdk-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: boson_sdk-0.1.0.dist-info/METADATA
+Filename: boson_sdk-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: boson_sdk-0.1.0.dist-info/WHEEL
+Filename: boson_sdk-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: boson_sdk-0.1.0.dist-info/top_level.txt
+Filename: boson_sdk-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: boson_sdk-0.1.0.dist-info/RECORD
+Filename: boson_sdk-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## boson/base.py

```diff
@@ -1,19 +1,21 @@
 from types import FunctionType
-from typing import Optional
+from typing import Optional, List
+import datetime
 
 from boson.boson_v1_pb2 import (
     DatasetInfoRequest,
     DatasetInfoResponse,
     WarpRequest,
     RasterResponse,
     SearchRequest,
     SearchResponse,
 )
-from boson.features_pb2 import CollectionMsg
+from google.protobuf.timestamp_pb2 import Timestamp
+from boson.features_pb2 import CollectionMsg, ExtentMsg, SpatialExtentMsg, TemporalExtentMsg
 from boson.conversion import (
     search_request_to_kwargs,
     warp_request_to_kwargs,
     feature_collection_to_proto,
     numpy_to_raster_response,
 )
 
@@ -60,39 +62,64 @@
                 "https://api.stacspec.org/v1.0.0/item-search",
                 "https://api.stacspec.org/v1.0.0/ogcapi-features",
                 "https://api.stacspec.org/v1.0.0/collections",
                 "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/core",
                 "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/oas30",
                 "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/geojson",
             ],
-            collections=CollectionMsg(**self._collection),
+            collections=[CollectionMsg(**self._collection())],
         )
 
+    def _parse_interval(self, interval) -> List[Timestamp]:
+        timestamps = []
+        for x in interval:
+            if x is None:
+                timestamps.append(Timestamp())
+            elif isinstance(x, datetime.datetime):
+                t = Timestamp()
+                t.FromDatetime(x)
+                timestamps.append(t)
+            else:
+                timestamps.append(x)
+
+        return timestamps
+
+    def _extent_msg(self) -> ExtentMsg:
+        bboxes = self.extent.get("bbox", [[-180, -90, 180, 90]])
+        intervals = self.extent.get("interval", [[None, None]])
+
+        bbox_msgs = [SpatialExtentMsg(bbox=bbox) for bbox in bboxes]
+        interval_msgs = [
+            TemporalExtentMsg(interval=self._parse_interval(interval)) for interval in intervals
+        ]
+
+        return ExtentMsg(spatial=bbox_msgs, temporal=interval_msgs)
+
     def _collection(self) -> dict:
         return {
             "version": "v1.0.0",
             "id": self.name,
             "title": self.alias,
             "description": self.description,
             "license": self.license,
+            "extent": self._extent_msg(),
         }
 
     def warp(self, request: WarpRequest) -> RasterResponse:
         warp_kwargs = warp_request_to_kwargs(request)
 
         x = self.warp_func(**warp_kwargs)
 
         return numpy_to_raster_response(x)
 
     def search(self, request: SearchRequest) -> SearchResponse:
         search_kwargs = search_request_to_kwargs(request)
-
         res = self.search_func(**search_kwargs)
         token = ""
-        if len(res) == 2:
-            fc, token = res
-        else:
+
+        if isinstance(res, dict):
             fc = res
+        elif len(res) == 2:
+            fc, token = res
 
         fc_proto = feature_collection_to_proto(fc)
-
         return SearchResponse(feature_collection=fc_proto, token=token)
```

## boson/conversion.py

```diff
@@ -13,126 +13,113 @@
     for feature in fc.features:
         features.append(feature_to_proto(feature))
 
     links = []
     for link in fc.links:
         links.append(link_to_proto(link))
 
-    return FeatureCollectionMsg(
-        features=features,
-        links=links
-    )
+    return FeatureCollectionMsg(features=features, links=links)
 
 
 def feature_to_proto(feature: geodesic.Feature) -> FeatureMsg:
     geom_wkb = feature.geometry.wkb
 
-    assets = feature.get('assets')
+    assets = feature.get("assets")
 
     if assets is not None:
         assetsMsg = {}
         for asset_name, asset in assets.items():
             assetsMsg[asset_name] = AssetMsg(
                 title=asset.title,
                 description=asset.description,
                 type=asset.type,
                 href=asset.href,
-                roles=asset.roles
+                roles=asset.roles,
             )
     else:
         assetsMsg = None
 
-    fid = feature.get('id', str(uuid.uuid4()))
+    fid = feature.get("id", str(uuid.uuid4()))
     return FeatureMsg(
         id=fid,
         geometry=geom_wkb,
         properties=feature.properties,
         links=feature.links,
-        assets=assetsMsg
+        assets=assetsMsg,
     )
 
 
 def link_to_proto(link: dict) -> LinkMsg:
     return LinkMsg(
-        href=link.get('href'),
-        rel=link.get('rel'),
-        type=link.get('type'),
-        title=link.get('title')
+        href=link.get("href"), rel=link.get("rel"), type=link.get("type"), title=link.get("title")
     )
 
 
 def search_request_to_kwargs(request: SearchRequest) -> dict:
     bbox = request.bbox
     datetime = request.datetime
     filter = request.filter
     collections = request.collections
     feature_ids = request.feature_ids
     fields = None
     if request.fields is not None:
         fields = {
-            'include': request.fields.include,
-            'exclude': request.fields.exclude,
+            "include": request.fields.include,
+            "exclude": request.fields.exclude,
         }
 
     intersects = None
-    if request.intersects is not None:
+    if request.intersects:
         intersects = wkb.loads(request.intersects)
 
     return {
-        'bbox': tuple(bbox) if bbox is not None else None,
-        'datetime': datetime,
-        'filter': filter,
-        'collections': collections,
-        'feature_ids': feature_ids,
-        'fields': fields,
-        'intersects': intersects,
-        'limit': request.limit,
-        'page': request.page,
-        'token': request.token
+        "bbox": tuple(bbox) if bbox else None,
+        "datetime": datetime,
+        "filter": filter,
+        "collections": collections,
+        "feature_ids": feature_ids,
+        "fields": fields,
+        "intersects": intersects,
+        "limit": request.limit,
+        "page": request.page,
+        "token": request.token,
     }
 
 
 def numpy_to_raster_response(x: np.ndarray) -> RasterResponse:
     _, descr = x.dtype.descr[0]
 
-    return RasterResponse(
-        data=x.tobytes(),
-        content_type='raw',
-        pixel_type=descr,
-        shape=x.shape
-    )
+    return RasterResponse(data=x.tobytes(), content_type="raw", pixel_type=descr, shape=x.shape)
 
 
 def warp_request_to_kwargs(request: WarpRequest) -> dict:
     bbox = request.output_extent
     bbox84 = request.output_extent_wgs84
     pixel_size = request.output_pixel_size
     shape = request.output_shape
 
     asset_bands = []
     if request.asset_bands is not None:
         asset_bands = [
-            {
-                'asset': ab.asset,
-                'bands': tuple([convert_band_id(band_id) for band_id in ab.bands])
-            } for ab in request.asset_bands
+            {"asset": ab.asset, "bands": tuple([convert_band_id(band_id) for band_id in ab.bands])}
+            for ab in request.asset_bands
         ]
 
     return dict(
         bbox=bbox,
         bbox84=bbox84,
         pixel_size=tuple(pixel_size),
         shape=tuple(shape),
         output_srs=request.output_spatial_reference,
         bbox_srs=request.output_extent_spatial_reference,
         time_instant=request.time_instant,
         time_range=request.time_range,
         asset_bands=asset_bands,
         input_filepaths=request.input_filepaths,
-        filter=request.filter
+        filter=request.filter,
     )
 
 
 def convert_band_id(band_id: BandID) -> Union[str, int]:
     if band_id.name is not None:
         return band_id.name
     return band_id.id
```

## Comparing `boson_sdk-0.1.0.dist-info/LICENSE` & `boson_sdk-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `boson_sdk-0.1.0.dist-info/METADATA` & `boson_sdk-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boson-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK for Boson Geospatial Service Mesh Providers
 Author-email: The SeerAI Team <contact@seer.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

## Comparing `boson_sdk-0.1.0.dist-info/RECORD` & `boson_sdk-0.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 boson/__init__.py,sha256=Xnoa1_beJWNJ7vMFMhJdJM3cMKOQzvK0cwnlh7GsprA,749
-boson/base.py,sha256=8wEWKFirWB4I46hOFslUFd6Le9YwmCwrXVbw83WbQ6k,3157
+boson/base.py,sha256=-HsRg75UFtc2V66HaT7-5ENJraDbfT8pPNh2JPskai0,4209
 boson/boson_v1_pb2.py,sha256=3SDZu0ktfhwRGkjrXDliI_uOQIYgZnqvGSTnF3Z7SEE,5320
-boson/conversion.py,sha256=WxminEDzcwj0o3txCi10bNc87d3GSH17htTXtVtevF4,3714
+boson/conversion.py,sha256=kWZU7XlE7PzvSi6HcQFzAXWScz1oy9vB2lBMbp8z960,3576
 boson/features_pb2.py,sha256=VFTKLcXxvSfqnuW_-Sj1qR6FiXrG33PzssSOAdx6Ads,8496
 boson/grpc/__init__.py,sha256=Z1VcMBg4TgrsHfO7jI7pyAZ0jKzJ1ya4gn5gwJkYGp8,57
 boson/grpc/boson_v1_pb2_grpc.py,sha256=aL02_ezWzSWJIDy5n2mxCswmGA4bMyXbGkU6FURivGo,5518
 boson/grpc/server.py,sha256=XBMosGe56I827E00QGUsIngyZiWUyfAo0hbDNFamYLA,2159
 boson/http/__init__.py,sha256=1J3MipaATnk1VFxmMV0uXeW7DWrD9t6vfcDlHOEjyrA,57
 boson/http/server.py,sha256=Q2gKtPCyXenaxNRUNkZF28FvuzcqRmtDLICA-Wrbx6k,2568
-boson_sdk-0.1.0.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-boson_sdk-0.1.0.dist-info/METADATA,sha256=E7ReiCEYNZS_ZKFGqEJQoM63OzBWxfoj9pHTwyTWCKo,14911
-boson_sdk-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-boson_sdk-0.1.0.dist-info/top_level.txt,sha256=a05hL1bKBp1M9A2czOQcnAZrKe63bhOjgjTAf4ri-4c,6
-boson_sdk-0.1.0.dist-info/RECORD,,
+boson_sdk-0.1.1.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+boson_sdk-0.1.1.dist-info/METADATA,sha256=DVbY4DYhtQ73w2wBES-NwinS6G21YWCcNlL5Mx6I1BU,14911
+boson_sdk-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+boson_sdk-0.1.1.dist-info/top_level.txt,sha256=a05hL1bKBp1M9A2czOQcnAZrKe63bhOjgjTAf4ri-4c,6
+boson_sdk-0.1.1.dist-info/RECORD,,
```

