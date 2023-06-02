# Comparing `tmp/intelicity-0.0.5-py3-none-any.whl.zip` & `tmp/intelicity-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 19200 bytes, number of entries: 23
+Zip file size: 19199 bytes, number of entries: 23
 -rw-rw-r--  2.0 unx      198 b- defN 23-Jun-02 15:43 intelicity/__init__.py
 -rw-rw-r--  2.0 unx     2425 b- defN 23-Jun-01 15:15 intelicity/ai_object.py
 -rw-rw-r--  2.0 unx     6322 b- defN 23-May-31 16:18 intelicity/bound_box.py
 -rw-rw-r--  2.0 unx     3342 b- defN 23-Jun-02 15:43 intelicity/containers.py
 -rw-rw-r--  2.0 unx     6720 b- defN 23-Jun-02 15:45 intelicity/contents.py
 -rw-rw-r--  2.0 unx     1181 b- defN 23-Jun-02 15:45 intelicity/file_header.py
 -rw-rw-r--  2.0 unx     2656 b- defN 23-Jun-01 14:37 intelicity/geo_location.py
@@ -13,13 +13,13 @@
 -rw-rw-r--  2.0 unx     6322 b- defN 23-May-31 16:18 src/bound_box.py
 -rw-rw-r--  2.0 unx     3335 b- defN 23-Jun-02 13:23 src/containers.py
 -rw-rw-r--  2.0 unx     6699 b- defN 23-Jun-02 13:23 src/contents.py
 -rw-rw-r--  2.0 unx     1171 b- defN 23-Jun-02 13:24 src/file_header.py
 -rw-rw-r--  2.0 unx     2656 b- defN 23-Jun-01 14:37 src/geo_location.py
 -rw-rw-r--  2.0 unx     1471 b- defN 23-Jun-01 15:59 src/image.py
 -rw-rw-r--  2.0 unx     4411 b- defN 23-May-24 20:18 src/main.py
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-02 15:46 intelicity-0.0.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx      643 b- defN 23-Jun-02 15:46 intelicity-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 15:46 intelicity-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-02 15:46 intelicity-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1763 b- defN 23-Jun-02 15:46 intelicity-0.0.5.dist-info/RECORD
-23 files, 60799 bytes uncompressed, 16400 bytes compressed:  73.0%
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-02 16:08 intelicity-0.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-02 16:08 intelicity-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 16:08 intelicity-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-02 16:08 intelicity-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1763 b- defN 23-Jun-02 16:08 intelicity-0.0.6.dist-info/RECORD
+23 files, 60799 bytes uncompressed, 16399 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: src/image.py
 Comment: 
 
 Filename: src/main.py
 Comment: 
 
-Filename: intelicity-0.0.5.dist-info/LICENSE
+Filename: intelicity-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: intelicity-0.0.5.dist-info/METADATA
+Filename: intelicity-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: intelicity-0.0.5.dist-info/WHEEL
+Filename: intelicity-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: intelicity-0.0.5.dist-info/top_level.txt
+Filename: intelicity-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: intelicity-0.0.5.dist-info/RECORD
+Filename: intelicity-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `intelicity-0.0.5.dist-info/LICENSE` & `intelicity-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intelicity-0.0.5.dist-info/METADATA` & `intelicity-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelicity
-Version: 0.0.5
+Version: 0.0.6
 Summary: a library for reading and managing data from the Intelicity server
 Author: Me
 Author-email: Felipe Rodrigues Peixoto da Silva <frps2003@gmail.com>
 License: MIT
 Project-URL: Homepage, https://inteli.city/
 Project-URL: project, https://github.com/Comunalti/Intelicity_Library
 Classifier: Programming Language :: Python :: 3
```

## Comparing `intelicity-0.0.5.dist-info/RECORD` & `intelicity-0.0.6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 src/bound_box.py,sha256=XvsWJz0R_dq3Mf8BdZc6mAARlOUgagbm3ZsiVFHW_sE,6322
 src/containers.py,sha256=lmFi2ycZdA2iwqrY0vWsZG89QY81kEdsoVlP0IWJwRY,3335
 src/contents.py,sha256=8OQTCisgAt7W8kV0Kbz5Qeo7PhtwobRM4Ssmw1vFAY0,6699
 src/file_header.py,sha256=PpvZii5xMJhZMlVOlg2vmKHApM8kQvFB-ck-dV3j-bk,1171
 src/geo_location.py,sha256=r7oxnWKtIYavuGAySgQhhYpKNB3o-bs7-NnPq_ykvqY,2656
 src/image.py,sha256=F8s6myDP8KlWPgRfW9PObH-mFqUjxPMSrW7e6W3MQPg,1471
 src/main.py,sha256=lWFAod5cs5XuGfR63v-81omq_dzKtghlisJRf6DDrF8,4411
-intelicity-0.0.5.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-intelicity-0.0.5.dist-info/METADATA,sha256=-uQNz5_XAILFktY9j48H0oIZOGhUv08vSZr0CqF3MGo,643
-intelicity-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-intelicity-0.0.5.dist-info/top_level.txt,sha256=xHp1PhuI3caIPBFop84FTTiU1c_X4APlwoYvQkmTBcw,11
-intelicity-0.0.5.dist-info/RECORD,,
+intelicity-0.0.6.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+intelicity-0.0.6.dist-info/METADATA,sha256=KrmyznNT9DjDl3PqqQu0lWYwljy0MFxna1uzyi7rD0c,643
+intelicity-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+intelicity-0.0.6.dist-info/top_level.txt,sha256=xHp1PhuI3caIPBFop84FTTiU1c_X4APlwoYvQkmTBcw,11
+intelicity-0.0.6.dist-info/RECORD,,
```

