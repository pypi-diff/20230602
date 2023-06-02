# Comparing `tmp/netspresso-0.1.2-py3-none-any.whl.zip` & `tmp/netspresso-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 18464 bytes, number of entries: 21
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-02 01:16 netspresso/__init__.py
+Zip file size: 18978 bytes, number of entries: 23
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-02 01:20 netspresso/__init__.py
 -rw-r--r--  2.0 unx    19641 b- defN 23-Jun-01 18:22 netspresso/compressor/__init__.py
 -rw-r--r--  2.0 unx     8237 b- defN 23-Jun-01 17:47 netspresso/compressor/client/__init__.py
 -rw-r--r--  2.0 unx      517 b- defN 23-Jun-01 17:47 netspresso/compressor/client/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 17:47 netspresso/compressor/client/schemas/__init__.py
 -rw-r--r--  2.0 unx     2584 b- defN 23-Jun-01 17:47 netspresso/compressor/client/schemas/auth.py
 -rw-r--r--  2.0 unx      466 b- defN 23-Jun-01 17:47 netspresso/compressor/client/schemas/common.py
 -rw-r--r--  2.0 unx     4042 b- defN 23-Jun-01 17:47 netspresso/compressor/client/schemas/compression.py
@@ -11,13 +11,15 @@
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 17:47 netspresso/compressor/client/utils/__init__.py
 -rw-r--r--  2.0 unx      465 b- defN 23-Jun-01 17:47 netspresso/compressor/client/utils/common.py
 -rw-r--r--  2.0 unx      694 b- defN 23-Jun-01 17:47 netspresso/compressor/client/utils/enum.py
 -rw-r--r--  2.0 unx     3735 b- defN 23-Jun-01 17:47 netspresso/compressor/client/utils/validator.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 17:47 netspresso/compressor/core/__init__.py
 -rw-r--r--  2.0 unx      551 b- defN 23-Jun-01 17:47 netspresso/compressor/core/compression.py
 -rw-r--r--  2.0 unx      507 b- defN 23-Jun-01 17:47 netspresso/compressor/core/model.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-02 01:17 netspresso-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3794 b- defN 23-Jun-02 01:17 netspresso-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 01:17 netspresso-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-02 01:17 netspresso-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-02 01:17 netspresso-0.1.2.dist-info/RECORD
-21 files, 62916 bytes uncompressed, 15178 bytes compressed:  75.9%
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 01:20 netspresso/compressor/utils/__init__.py
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-01 17:47 netspresso/compressor/utils/token.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-02 01:20 netspresso-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3794 b- defN 23-Jun-02 01:20 netspresso-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 01:20 netspresso-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-02 01:20 netspresso-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2143 b- defN 23-Jun-02 01:20 netspresso-0.1.3.dist-info/RECORD
+23 files, 63329 bytes uncompressed, 15390 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -42,23 +42,29 @@
 
 Filename: netspresso/compressor/core/compression.py
 Comment: 
 
 Filename: netspresso/compressor/core/model.py
 Comment: 
 
-Filename: netspresso-0.1.2.dist-info/LICENSE
+Filename: netspresso/compressor/utils/__init__.py
 Comment: 
 
-Filename: netspresso-0.1.2.dist-info/METADATA
+Filename: netspresso/compressor/utils/token.py
 Comment: 
 
-Filename: netspresso-0.1.2.dist-info/WHEEL
+Filename: netspresso-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: netspresso-0.1.2.dist-info/top_level.txt
+Filename: netspresso-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: netspresso-0.1.2.dist-info/RECORD
+Filename: netspresso-0.1.3.dist-info/WHEEL
+Comment: 
+
+Filename: netspresso-0.1.3.dist-info/top_level.txt
+Comment: 
+
+Filename: netspresso-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netspresso/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `netspresso-0.1.2.dist-info/LICENSE` & `netspresso-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netspresso-0.1.2.dist-info/METADATA` & `netspresso-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netspresso
-Version: 0.1.2
+Version: 0.1.3
 Summary: python client for the NetsPresso
 Home-page: https://github.com/nota-github/netspresso-python
 Author: NetsPresso
 Author-email: bmlee@nota.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `netspresso-0.1.2.dist-info/RECORD` & `netspresso-0.1.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-netspresso/__init__.py,sha256=YvuYzWnKtqBb-IqG8HAu-nhIYAsgj9Vmc_b9o7vO-js,22
+netspresso/__init__.py,sha256=XEqb2aiIn8fzGE68Mph4ck1FtQqsR_am0wRWvrYPffQ,22
 netspresso/compressor/__init__.py,sha256=JBF9PJJbadvVaDKB-YG8KBLsfxzJgoO8zB_rBYng6EY,19641
 netspresso/compressor/client/__init__.py,sha256=EQ6bIJ3MrdXImw3GLj6HE6FKe1AyeLwWfT8aG8jwY1E,8237
 netspresso/compressor/client/config.py,sha256=LRYWzn_wFLixxexrCbQ3XTk1lU9HaFbEfGmKehruQYE,517
 netspresso/compressor/client/schemas/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/client/schemas/auth.py,sha256=6s3owU388I7u0XSMx1quwuHA3a534Z2EqiP1_Y_893k,2584
 netspresso/compressor/client/schemas/common.py,sha256=d6J6A40pqFncvRZtEY_3y49sMbcnNvCCBbWy9lV72gI,466
 netspresso/compressor/client/schemas/compression.py,sha256=Bzm8vHHsPQfT1Q4qugavYHeeCsmUsK7WhO1Vjq7BR20,4042
@@ -10,12 +10,14 @@
 netspresso/compressor/client/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/client/utils/common.py,sha256=JLxIRbkOwEjQQ1utVN8jNBBPp9rEch0l08-toHceYQk,465
 netspresso/compressor/client/utils/enum.py,sha256=ak9nJYKipWAMr0wCsR4xv6J8om7DTPc1ToUKU18YETE,694
 netspresso/compressor/client/utils/validator.py,sha256=H9eLujAKAJx-ZNs9JXpOWkOf6U_t-51zzsEqIWme29Y,3735
 netspresso/compressor/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/core/compression.py,sha256=dlF0_tB1HjBEI7d2NQfNqnqdVMw5BIlxSjgdEQqmdjE,551
 netspresso/compressor/core/model.py,sha256=h69FnQeh-dgxxG-fmOFl045l-C5usRjZzK_3e7gAxPI,507
-netspresso-0.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-netspresso-0.1.2.dist-info/METADATA,sha256=6EvoJmj2rqD0bLlSKFRYPHPdNBA_Sh5LVu3nUXSUafU,3794
-netspresso-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-netspresso-0.1.2.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
-netspresso-0.1.2.dist-info/RECORD,,
+netspresso/compressor/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+netspresso/compressor/utils/token.py,sha256=Zqnmc9RK5s_AIrP3z0aAPE7dlO5OmD1xz6AAZ63woCc,228
+netspresso-0.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+netspresso-0.1.3.dist-info/METADATA,sha256=oX3h_dZ11tERYYaAoB9FDW6rcD9_65O6StH1AO-hJTA,3794
+netspresso-0.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+netspresso-0.1.3.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
+netspresso-0.1.3.dist-info/RECORD,,
```

