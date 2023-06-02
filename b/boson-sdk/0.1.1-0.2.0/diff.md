# Comparing `tmp/boson_sdk-0.1.1-py3-none-any.whl.zip` & `tmp/boson_sdk-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 20577 bytes, number of entries: 15
--rw-r--r--  2.0 unx      749 b- defN 23-Jun-02 01:49 boson/__init__.py
--rw-r--r--  2.0 unx     4209 b- defN 23-Jun-02 01:49 boson/base.py
--rw-r--r--  2.0 unx     5320 b- defN 23-Jun-02 01:49 boson/boson_v1_pb2.py
--rw-r--r--  2.0 unx     3576 b- defN 23-Jun-02 01:49 boson/conversion.py
--rw-r--r--  2.0 unx     8496 b- defN 23-Jun-02 01:49 boson/features_pb2.py
--rw-r--r--  2.0 unx       57 b- defN 23-Jun-02 01:49 boson/grpc/__init__.py
--rw-r--r--  2.0 unx     5518 b- defN 23-Jun-02 01:49 boson/grpc/boson_v1_pb2_grpc.py
--rw-r--r--  2.0 unx     2159 b- defN 23-Jun-02 01:49 boson/grpc/server.py
--rw-r--r--  2.0 unx       57 b- defN 23-Jun-02 01:49 boson/http/__init__.py
--rw-r--r--  2.0 unx     2568 b- defN 23-Jun-02 01:49 boson/http/server.py
--rw-r--r--  2.0 unx    11356 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    14911 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1168 b- defN 23-Jun-02 01:49 boson_sdk-0.1.1.dist-info/RECORD
-15 files, 60242 bytes uncompressed, 18665 bytes compressed:  69.0%
+Zip file size: 20531 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      749 b- defN 23-Jun-02 17:56 boson/__init__.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-Jun-02 17:56 boson/base.py
+-rw-r--r--  2.0 unx     5320 b- defN 23-Jun-02 17:56 boson/boson_v1_pb2.py
+-rw-r--r--  2.0 unx     3684 b- defN 23-Jun-02 17:56 boson/conversion.py
+-rw-r--r--  2.0 unx     7772 b- defN 23-Jun-02 17:56 boson/features_pb2.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-02 17:56 boson/grpc/__init__.py
+-rw-r--r--  2.0 unx     5518 b- defN 23-Jun-02 17:56 boson/grpc/boson_v1_pb2_grpc.py
+-rw-r--r--  2.0 unx     2159 b- defN 23-Jun-02 17:56 boson/grpc/server.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-02 17:56 boson/http/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-Jun-02 17:56 boson/http/server.py
+-rw-r--r--  2.0 unx    11356 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14911 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1168 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/RECORD
+15 files, 59626 bytes uncompressed, 18619 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: boson/http/__init__.py
 Comment: 
 
 Filename: boson/http/server.py
 Comment: 
 
-Filename: boson_sdk-0.1.1.dist-info/LICENSE
+Filename: boson_sdk-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: boson_sdk-0.1.1.dist-info/METADATA
+Filename: boson_sdk-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: boson_sdk-0.1.1.dist-info/WHEEL
+Filename: boson_sdk-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: boson_sdk-0.1.1.dist-info/top_level.txt
+Filename: boson_sdk-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: boson_sdk-0.1.1.dist-info/RECORD
+Filename: boson_sdk-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## boson/conversion.py

```diff
@@ -1,13 +1,14 @@
 import uuid
 
 from typing import Union
 import numpy as np
 import geodesic
 import shapely.wkb as wkb
+from google.protobuf.struct_pb2 import Struct
 from boson.boson_v1_pb2 import RasterResponse, WarpRequest, BandID, SearchRequest
 from boson.features_pb2 import FeatureMsg, FeatureCollectionMsg, LinkMsg, AssetMsg
 
 
 def feature_collection_to_proto(fc: geodesic.FeatureCollection) -> FeatureCollectionMsg:
     features = []
     for feature in fc.features:
@@ -35,18 +36,22 @@
                 href=asset.href,
                 roles=asset.roles,
             )
     else:
         assetsMsg = None
 
     fid = feature.get("id", str(uuid.uuid4()))
+
+    properties = Struct()
+    properties.update(feature.properties)
+
     return FeatureMsg(
         id=fid,
         geometry=geom_wkb,
-        properties=feature.properties,
+        properties=properties,
         links=feature.links,
         assets=assetsMsg,
     )
 
 
 def link_to_proto(link: dict) -> LinkMsg:
     return LinkMsg(
```

## boson/features_pb2.py

```diff
@@ -11,68 +11,60 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x66\x65\x61tures.proto\x12\x04gogc\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xea\x03\n\rCollectionMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\t\x12\x0f\n\x07license\x18\x05 \x01(\t\x12\x1f\n\x06\x65xtent\x18\x06 \x01(\x0b\x32\x0f.gogc.ExtentMsg\x12\x1c\n\x05links\x18\x07 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x08 \x01(\t\x12\x12\n\nextensions\x18\t \x03(\t\x12$\n\tproviders\x18\n \x03(\x0b\x32\x11.gogc.ProviderMsg\x12\x35\n\tsummaries\x18\x0b \x03(\x0b\x32\".gogc.CollectionMsg.SummariesEntry\x12\x38\n\x0bitem_assets\x18\x0c \x03(\x0b\x32#.gogc.CollectionMsg.ItemAssetsEntry\x1aH\n\x0eSummariesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value:\x02\x38\x01\x1a\x41\n\x0fItemAssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xb8\x01\n\x14\x46\x65\x61tureCollectionMsg\x12\"\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x10.gogc.FeatureMsg\x12\x1c\n\x05links\x18\x02 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x16\n\x0enumber_matched\x18\x03 \x01(\x03\x12\x17\n\x0fnumber_returned\x18\x04 \x01(\x03\x12-\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xfd\x02\n\nFeatureMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08geometry\x18\x02 \x01(\x0c\x12\x0c\n\x04\x62\x62ox\x18\x03 \x03(\x01\x12\x34\n\nproperties\x18\x04 \x03(\x0b\x32 .gogc.FeatureMsg.PropertiesEntry\x12\x1c\n\x05links\x18\x05 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x12\n\nextensions\x18\x07 \x03(\t\x12,\n\x06\x61ssets\x18\x08 \x03(\x0b\x32\x1c.gogc.FeatureMsg.AssetsEntry\x12\x12\n\ncollection\x18\t \x01(\t\x1aI\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value:\x02\x38\x01\x1a=\n\x0b\x41ssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xbe\x02\n\x08\x41ssetMsg\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04href\x18\x04 \x01(\t\x12\r\n\x05roles\x18\x05 \x03(\t\x12!\n\x08\x65o_bands\x18\x06 \x03(\x0b\x32\x0f.gogc.EOBandMsg\x12)\n\x0craster_bands\x18\x07 \x03(\x0b\x32\x13.gogc.RasterBandMsg\x12!\n\x07storage\x18\t \x01(\x0b\x32\x10.gogc.StorageMsg\x12\x30\n\talternate\x18\n \x03(\x0b\x32\x1d.gogc.AssetMsg.AlternateEntry\x1a@\n\x0e\x41lternateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"T\n\nStorageMsg\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x16\n\x0erequester_pays\x18\x03 \x01(\x08\x12\x0c\n\x04tier\x18\x04 \x01(\t\"\xa4\x01\n\tEOBandMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x63ommon_name\x18\x02 \x01(\t\x12\x0b\n\x03gsd\x18\x03 \x01(\x01\x12\x19\n\x11\x63\x65nter_wavelength\x18\x04 \x01(\x01\x12\x1b\n\x13\x66ull_width_half_max\x18\x05 \x01(\x01\x12\x1a\n\x12solar_illumination\x18\x06 \x01(\x01\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\"\x9b\x02\n\rRasterBandMsg\x12\'\n\x07no_data\x18\x01 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x10\n\x08sampling\x18\x02 \x01(\t\x12\x11\n\tdata_type\x18\x03 \x01(\t\x12\x17\n\x0f\x62its_per_sample\x18\x04 \x01(\x05\x12\x1a\n\x12spatial_resolution\x18\x05 \x01(\x01\x12-\n\nstatistics\x18\x06 \x01(\x0b\x32\x19.gogc.RasterStatisticsMsg\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\r\n\x05scale\x18\x08 \x01(\x01\x12\x0e\n\x06offset\x18\t \x01(\x01\x12+\n\thistogram\x18\n \x01(\x0b\x32\x18.gogc.RasterHistogramMsg\"l\n\x13RasterStatisticsMsg\x12\x0c\n\x04mean\x18\x01 \x01(\x01\x12\x0f\n\x07minimum\x18\x02 \x01(\x01\x12\x0f\n\x07maximum\x18\x03 \x01(\x01\x12\x0e\n\x06stddev\x18\x04 \x01(\x01\x12\x15\n\rvalid_percent\x18\x05 \x01(\x01\"N\n\x12RasterHistogramMsg\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x0f\n\x07\x62uckets\x18\x04 \x03(\x04\"_\n\tExtentMsg\x12\'\n\x07spatial\x18\x01 \x03(\x0b\x32\x16.gogc.SpatialExtentMsg\x12)\n\x08temporal\x18\x02 \x03(\x0b\x32\x17.gogc.TemporalExtentMsg\" \n\x10SpatialExtentMsg\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\"A\n\x11TemporalExtentMsg\x12,\n\x08interval\x18\x01 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x02\n\x07LinkMsg\x12\x0c\n\x04href\x18\x01 \x01(\t\x12\x0b\n\x03rel\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08hreflang\x18\x04 \x01(\t\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06length\x18\x06 \x01(\x03\x12\x0e\n\x06method\x18\x07 \x01(\t\x12+\n\x07headers\x18\x08 \x03(\x0b\x32\x1a.gogc.LinkMsg.HeadersEntry\x12%\n\x04\x62ody\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05merge\x18\n \x01(\x08\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"L\n\x0bProviderMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\t\x12\x0b\n\x03url\x18\x04 \x01(\tB!Z\x1fgithub.com/seerai/gogc/featuresb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x66\x65\x61tures.proto\x12\x04gogc\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x95\x03\n\rCollectionMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\t\x12\x0f\n\x07license\x18\x05 \x01(\t\x12\x1f\n\x06\x65xtent\x18\x06 \x01(\x0b\x32\x0f.gogc.ExtentMsg\x12\x1c\n\x05links\x18\x07 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x08 \x01(\t\x12\x12\n\nextensions\x18\t \x03(\t\x12$\n\tproviders\x18\n \x03(\x0b\x32\x11.gogc.ProviderMsg\x12*\n\tsummaries\x18\x0b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x38\n\x0bitem_assets\x18\x0c \x03(\x0b\x32#.gogc.CollectionMsg.ItemAssetsEntry\x1a\x41\n\x0fItemAssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xb8\x01\n\x14\x46\x65\x61tureCollectionMsg\x12\"\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x10.gogc.FeatureMsg\x12\x1c\n\x05links\x18\x02 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x16\n\x0enumber_matched\x18\x03 \x01(\x03\x12\x17\n\x0fnumber_returned\x18\x04 \x01(\x03\x12-\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa9\x02\n\nFeatureMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08geometry\x18\x02 \x01(\x0c\x12\x0c\n\x04\x62\x62ox\x18\x03 \x03(\x01\x12+\n\nproperties\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1c\n\x05links\x18\x05 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x12\n\nextensions\x18\x07 \x03(\t\x12,\n\x06\x61ssets\x18\x08 \x03(\x0b\x32\x1c.gogc.FeatureMsg.AssetsEntry\x12\x12\n\ncollection\x18\t \x01(\t\x1a=\n\x0b\x41ssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xbe\x02\n\x08\x41ssetMsg\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04href\x18\x04 \x01(\t\x12\r\n\x05roles\x18\x05 \x03(\t\x12!\n\x08\x65o_bands\x18\x06 \x03(\x0b\x32\x0f.gogc.EOBandMsg\x12)\n\x0craster_bands\x18\x07 \x03(\x0b\x32\x13.gogc.RasterBandMsg\x12!\n\x07storage\x18\t \x01(\x0b\x32\x10.gogc.StorageMsg\x12\x30\n\talternate\x18\n \x03(\x0b\x32\x1d.gogc.AssetMsg.AlternateEntry\x1a@\n\x0e\x41lternateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"T\n\nStorageMsg\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x16\n\x0erequester_pays\x18\x03 \x01(\x08\x12\x0c\n\x04tier\x18\x04 \x01(\t\"\xa4\x01\n\tEOBandMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x63ommon_name\x18\x02 \x01(\t\x12\x0b\n\x03gsd\x18\x03 \x01(\x01\x12\x19\n\x11\x63\x65nter_wavelength\x18\x04 \x01(\x01\x12\x1b\n\x13\x66ull_width_half_max\x18\x05 \x01(\x01\x12\x1a\n\x12solar_illumination\x18\x06 \x01(\x01\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\"\x9b\x02\n\rRasterBandMsg\x12\'\n\x07no_data\x18\x01 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x10\n\x08sampling\x18\x02 \x01(\t\x12\x11\n\tdata_type\x18\x03 \x01(\t\x12\x17\n\x0f\x62its_per_sample\x18\x04 \x01(\x05\x12\x1a\n\x12spatial_resolution\x18\x05 \x01(\x01\x12-\n\nstatistics\x18\x06 \x01(\x0b\x32\x19.gogc.RasterStatisticsMsg\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\r\n\x05scale\x18\x08 \x01(\x01\x12\x0e\n\x06offset\x18\t \x01(\x01\x12+\n\thistogram\x18\n \x01(\x0b\x32\x18.gogc.RasterHistogramMsg\"l\n\x13RasterStatisticsMsg\x12\x0c\n\x04mean\x18\x01 \x01(\x01\x12\x0f\n\x07minimum\x18\x02 \x01(\x01\x12\x0f\n\x07maximum\x18\x03 \x01(\x01\x12\x0e\n\x06stddev\x18\x04 \x01(\x01\x12\x15\n\rvalid_percent\x18\x05 \x01(\x01\"N\n\x12RasterHistogramMsg\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x0f\n\x07\x62uckets\x18\x04 \x03(\x04\"_\n\tExtentMsg\x12\'\n\x07spatial\x18\x01 \x03(\x0b\x32\x16.gogc.SpatialExtentMsg\x12)\n\x08temporal\x18\x02 \x03(\x0b\x32\x17.gogc.TemporalExtentMsg\" \n\x10SpatialExtentMsg\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\"A\n\x11TemporalExtentMsg\x12,\n\x08interval\x18\x01 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x02\n\x07LinkMsg\x12\x0c\n\x04href\x18\x01 \x01(\t\x12\x0b\n\x03rel\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08hreflang\x18\x04 \x01(\t\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06length\x18\x06 \x01(\x03\x12\x0e\n\x06method\x18\x07 \x01(\t\x12+\n\x07headers\x18\x08 \x03(\x0b\x32\x1a.gogc.LinkMsg.HeadersEntry\x12%\n\x04\x62ody\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05merge\x18\n \x01(\x08\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"L\n\x0bProviderMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\t\x12\x0b\n\x03url\x18\x04 \x01(\tB!Z\x1fgithub.com/seerai/gogc/featuresb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'features_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\037github.com/seerai/gogc/features'
-  _COLLECTIONMSG_SUMMARIESENTRY._options = None
-  _COLLECTIONMSG_SUMMARIESENTRY._serialized_options = b'8\001'
   _COLLECTIONMSG_ITEMASSETSENTRY._options = None
   _COLLECTIONMSG_ITEMASSETSENTRY._serialized_options = b'8\001'
-  _FEATUREMSG_PROPERTIESENTRY._options = None
-  _FEATUREMSG_PROPERTIESENTRY._serialized_options = b'8\001'
   _FEATUREMSG_ASSETSENTRY._options = None
   _FEATUREMSG_ASSETSENTRY._serialized_options = b'8\001'
   _ASSETMSG_ALTERNATEENTRY._options = None
   _ASSETMSG_ALTERNATEENTRY._serialized_options = b'8\001'
   _LINKMSG_HEADERSENTRY._options = None
   _LINKMSG_HEADERSENTRY._serialized_options = b'8\001'
   _COLLECTIONMSG._serialized_start=88
-  _COLLECTIONMSG._serialized_end=578
-  _COLLECTIONMSG_SUMMARIESENTRY._serialized_start=439
-  _COLLECTIONMSG_SUMMARIESENTRY._serialized_end=511
-  _COLLECTIONMSG_ITEMASSETSENTRY._serialized_start=513
-  _COLLECTIONMSG_ITEMASSETSENTRY._serialized_end=578
-  _FEATURECOLLECTIONMSG._serialized_start=581
-  _FEATURECOLLECTIONMSG._serialized_end=765
-  _FEATUREMSG._serialized_start=768
-  _FEATUREMSG._serialized_end=1149
-  _FEATUREMSG_PROPERTIESENTRY._serialized_start=1013
-  _FEATUREMSG_PROPERTIESENTRY._serialized_end=1086
-  _FEATUREMSG_ASSETSENTRY._serialized_start=1088
-  _FEATUREMSG_ASSETSENTRY._serialized_end=1149
-  _ASSETMSG._serialized_start=1152
-  _ASSETMSG._serialized_end=1470
-  _ASSETMSG_ALTERNATEENTRY._serialized_start=1406
-  _ASSETMSG_ALTERNATEENTRY._serialized_end=1470
-  _STORAGEMSG._serialized_start=1472
-  _STORAGEMSG._serialized_end=1556
-  _EOBANDMSG._serialized_start=1559
-  _EOBANDMSG._serialized_end=1723
-  _RASTERBANDMSG._serialized_start=1726
-  _RASTERBANDMSG._serialized_end=2009
-  _RASTERSTATISTICSMSG._serialized_start=2011
-  _RASTERSTATISTICSMSG._serialized_end=2119
-  _RASTERHISTOGRAMMSG._serialized_start=2121
-  _RASTERHISTOGRAMMSG._serialized_end=2199
-  _EXTENTMSG._serialized_start=2201
-  _EXTENTMSG._serialized_end=2296
-  _SPATIALEXTENTMSG._serialized_start=2298
-  _SPATIALEXTENTMSG._serialized_end=2330
-  _TEMPORALEXTENTMSG._serialized_start=2332
-  _TEMPORALEXTENTMSG._serialized_end=2397
-  _LINKMSG._serialized_start=2400
-  _LINKMSG._serialized_end=2662
-  _LINKMSG_HEADERSENTRY._serialized_start=2616
-  _LINKMSG_HEADERSENTRY._serialized_end=2662
-  _PROVIDERMSG._serialized_start=2664
-  _PROVIDERMSG._serialized_end=2740
+  _COLLECTIONMSG._serialized_end=493
+  _COLLECTIONMSG_ITEMASSETSENTRY._serialized_start=428
+  _COLLECTIONMSG_ITEMASSETSENTRY._serialized_end=493
+  _FEATURECOLLECTIONMSG._serialized_start=496
+  _FEATURECOLLECTIONMSG._serialized_end=680
+  _FEATUREMSG._serialized_start=683
+  _FEATUREMSG._serialized_end=980
+  _FEATUREMSG_ASSETSENTRY._serialized_start=919
+  _FEATUREMSG_ASSETSENTRY._serialized_end=980
+  _ASSETMSG._serialized_start=983
+  _ASSETMSG._serialized_end=1301
+  _ASSETMSG_ALTERNATEENTRY._serialized_start=1237
+  _ASSETMSG_ALTERNATEENTRY._serialized_end=1301
+  _STORAGEMSG._serialized_start=1303
+  _STORAGEMSG._serialized_end=1387
+  _EOBANDMSG._serialized_start=1390
+  _EOBANDMSG._serialized_end=1554
+  _RASTERBANDMSG._serialized_start=1557
+  _RASTERBANDMSG._serialized_end=1840
+  _RASTERSTATISTICSMSG._serialized_start=1842
+  _RASTERSTATISTICSMSG._serialized_end=1950
+  _RASTERHISTOGRAMMSG._serialized_start=1952
+  _RASTERHISTOGRAMMSG._serialized_end=2030
+  _EXTENTMSG._serialized_start=2032
+  _EXTENTMSG._serialized_end=2127
+  _SPATIALEXTENTMSG._serialized_start=2129
+  _SPATIALEXTENTMSG._serialized_end=2161
+  _TEMPORALEXTENTMSG._serialized_start=2163
+  _TEMPORALEXTENTMSG._serialized_end=2228
+  _LINKMSG._serialized_start=2231
+  _LINKMSG._serialized_end=2493
+  _LINKMSG_HEADERSENTRY._serialized_start=2447
+  _LINKMSG_HEADERSENTRY._serialized_end=2493
+  _PROVIDERMSG._serialized_start=2495
+  _PROVIDERMSG._serialized_end=2571
 # @@protoc_insertion_point(module_scope)
```

## Comparing `boson_sdk-0.1.1.dist-info/LICENSE` & `boson_sdk-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `boson_sdk-0.1.1.dist-info/METADATA` & `boson_sdk-0.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boson-sdk
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python SDK for Boson Geospatial Service Mesh Providers
 Author-email: The SeerAI Team <contact@seer.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

