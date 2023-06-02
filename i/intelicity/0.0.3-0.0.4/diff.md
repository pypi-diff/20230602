# Comparing `tmp/intelicity-0.0.3-py3-none-any.whl.zip` & `tmp/intelicity-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 19074 bytes, number of entries: 23
+Zip file size: 19177 bytes, number of entries: 23
 -rw-rw-r--  2.0 unx      170 b- defN 23-Jun-02 14:49 intelicity/__init__.py
 -rw-rw-r--  2.0 unx     2425 b- defN 23-Jun-01 15:15 intelicity/ai_object.py
 -rw-rw-r--  2.0 unx     6322 b- defN 23-May-31 16:18 intelicity/bound_box.py
--rw-rw-r--  2.0 unx     3335 b- defN 23-Jun-02 13:23 intelicity/containers.py
--rw-rw-r--  2.0 unx     6699 b- defN 23-Jun-02 13:23 intelicity/contents.py
--rw-rw-r--  2.0 unx     1171 b- defN 23-Jun-02 13:24 intelicity/file_header.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-02 15:34 intelicity/containers.py
+-rw-rw-r--  2.0 unx     6687 b- defN 23-Jun-02 15:35 intelicity/contents.py
+-rw-rw-r--  2.0 unx     1163 b- defN 23-Jun-02 15:35 intelicity/file_header.py
 -rw-rw-r--  2.0 unx     2656 b- defN 23-Jun-01 14:37 intelicity/geo_location.py
 -rw-rw-r--  2.0 unx     1471 b- defN 23-Jun-01 15:59 intelicity/image.py
 -rw-rw-r--  2.0 unx     4411 b- defN 23-May-24 20:18 intelicity/main.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-02 13:45 src/__init__.py
 -rw-rw-r--  2.0 unx     2425 b- defN 23-Jun-01 15:15 src/ai_object.py
 -rw-rw-r--  2.0 unx     6322 b- defN 23-May-31 16:18 src/bound_box.py
 -rw-rw-r--  2.0 unx     3335 b- defN 23-Jun-02 13:23 src/containers.py
 -rw-rw-r--  2.0 unx     6699 b- defN 23-Jun-02 13:23 src/contents.py
 -rw-rw-r--  2.0 unx     1171 b- defN 23-Jun-02 13:24 src/file_header.py
 -rw-rw-r--  2.0 unx     2656 b- defN 23-Jun-01 14:37 src/geo_location.py
 -rw-rw-r--  2.0 unx     1471 b- defN 23-Jun-01 15:59 src/image.py
 -rw-rw-r--  2.0 unx     4411 b- defN 23-May-24 20:18 src/main.py
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-02 14:55 intelicity-0.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      643 b- defN 23-Jun-02 14:55 intelicity-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 14:55 intelicity-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-02 14:55 intelicity-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1763 b- defN 23-Jun-02 14:55 intelicity-0.0.3.dist-info/RECORD
-23 files, 60733 bytes uncompressed, 16274 bytes compressed:  73.2%
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-02 15:36 intelicity-0.0.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-02 15:36 intelicity-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 15:36 intelicity-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-02 15:36 intelicity-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1763 b- defN 23-Jun-02 15:36 intelicity-0.0.4.dist-info/RECORD
+23 files, 60709 bytes uncompressed, 16377 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: src/image.py
 Comment: 
 
 Filename: src/main.py
 Comment: 
 
-Filename: intelicity-0.0.3.dist-info/LICENSE
+Filename: intelicity-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: intelicity-0.0.3.dist-info/METADATA
+Filename: intelicity-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: intelicity-0.0.3.dist-info/WHEEL
+Filename: intelicity-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: intelicity-0.0.3.dist-info/top_level.txt
+Filename: intelicity-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: intelicity-0.0.3.dist-info/RECORD
+Filename: intelicity-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## intelicity/containers.py

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from src.contents import *
+from contents import *
 
 
 class Container:
 
     def __init__(self, contents: list[FileContent]):
         self.contents = contents
         pass
```

## intelicity/contents.py

```diff
@@ -1,10 +1,10 @@
-from src.ai_object import AiObject
-from src.bound_box import BoundBox
-from src.geo_location import GeoLocation
+from ai_object import AiObject
+from bound_box import BoundBox
+from geo_location import GeoLocation
 
 
 class FileContent:
     pass
 
 
 class DatabaseContent(FileContent):
```

## intelicity/file_header.py

```diff
@@ -1,9 +1,9 @@
-from src.containers import *
-from src.image import Image
+from containers import *
+from image import Image
 from pathlib import Path
 
 
 class FileHeader:
 
     def __init__(self, path: Path):
         self.path = path
```

## Comparing `intelicity-0.0.3.dist-info/LICENSE` & `intelicity-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intelicity-0.0.3.dist-info/METADATA` & `intelicity-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelicity
-Version: 0.0.3
+Version: 0.0.4
 Summary: a library for reading and managing data from the Intelicity server
 Author: Me
 Author-email: Felipe Rodrigues Peixoto da Silva <frps2003@gmail.com>
 License: MIT
 Project-URL: Homepage, https://inteli.city/
 Project-URL: project, https://github.com/Comunalti/Intelicity_Library
 Classifier: Programming Language :: Python :: 3
```

## Comparing `intelicity-0.0.3.dist-info/RECORD` & `intelicity-0.0.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 intelicity/__init__.py,sha256=bvhCTQCs-BWIPXNx3u1kV_l3FumakhfBSO7zMhWv1gk,170
 intelicity/ai_object.py,sha256=3o5XYoWvj3v0onvcF0gVkmYmXb-YM3BKSDB-vMPovNc,2425
 intelicity/bound_box.py,sha256=XvsWJz0R_dq3Mf8BdZc6mAARlOUgagbm3ZsiVFHW_sE,6322
-intelicity/containers.py,sha256=lmFi2ycZdA2iwqrY0vWsZG89QY81kEdsoVlP0IWJwRY,3335
-intelicity/contents.py,sha256=8OQTCisgAt7W8kV0Kbz5Qeo7PhtwobRM4Ssmw1vFAY0,6699
-intelicity/file_header.py,sha256=PpvZii5xMJhZMlVOlg2vmKHApM8kQvFB-ck-dV3j-bk,1171
+intelicity/containers.py,sha256=ss14h_IsxZWXSzg3P5aZdLt0x6EJU1MdeKOAzYrm1qc,3331
+intelicity/contents.py,sha256=hX77T0-fF1NwFZFWJZe1Z-xsaSAjAZ-A3X2d_gWecOM,6687
+intelicity/file_header.py,sha256=NIZw404s4bSiDmovRPi_s0b-E2orBQYOC7-uiWldK3M,1163
 intelicity/geo_location.py,sha256=r7oxnWKtIYavuGAySgQhhYpKNB3o-bs7-NnPq_ykvqY,2656
 intelicity/image.py,sha256=F8s6myDP8KlWPgRfW9PObH-mFqUjxPMSrW7e6W3MQPg,1471
 intelicity/main.py,sha256=lWFAod5cs5XuGfR63v-81omq_dzKtghlisJRf6DDrF8,4411
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/ai_object.py,sha256=3o5XYoWvj3v0onvcF0gVkmYmXb-YM3BKSDB-vMPovNc,2425
 src/bound_box.py,sha256=XvsWJz0R_dq3Mf8BdZc6mAARlOUgagbm3ZsiVFHW_sE,6322
 src/containers.py,sha256=lmFi2ycZdA2iwqrY0vWsZG89QY81kEdsoVlP0IWJwRY,3335
 src/contents.py,sha256=8OQTCisgAt7W8kV0Kbz5Qeo7PhtwobRM4Ssmw1vFAY0,6699
 src/file_header.py,sha256=PpvZii5xMJhZMlVOlg2vmKHApM8kQvFB-ck-dV3j-bk,1171
 src/geo_location.py,sha256=r7oxnWKtIYavuGAySgQhhYpKNB3o-bs7-NnPq_ykvqY,2656
 src/image.py,sha256=F8s6myDP8KlWPgRfW9PObH-mFqUjxPMSrW7e6W3MQPg,1471
 src/main.py,sha256=lWFAod5cs5XuGfR63v-81omq_dzKtghlisJRf6DDrF8,4411
-intelicity-0.0.3.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-intelicity-0.0.3.dist-info/METADATA,sha256=I-G4QsQUIDj2NRlShKXJdeB62UZPmFSsIUNFNS42qqk,643
-intelicity-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-intelicity-0.0.3.dist-info/top_level.txt,sha256=xHp1PhuI3caIPBFop84FTTiU1c_X4APlwoYvQkmTBcw,11
-intelicity-0.0.3.dist-info/RECORD,,
+intelicity-0.0.4.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+intelicity-0.0.4.dist-info/METADATA,sha256=7T0D-L-e1GeNPrucdts8gmlr4w0BH7JLgwhGd9Zyzw0,643
+intelicity-0.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+intelicity-0.0.4.dist-info/top_level.txt,sha256=xHp1PhuI3caIPBFop84FTTiU1c_X4APlwoYvQkmTBcw,11
+intelicity-0.0.4.dist-info/RECORD,,
```

