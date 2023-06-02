# Comparing `tmp/databento_dbn-0.6.0-cp39-none-win_amd64.whl.zip` & `tmp/databento_dbn-0.6.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 544943 bytes, number of entries: 8
--rw-r--r--  4.6 unx     2966 b- defN 23-May-26 20:01 databento_dbn-0.6.0.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-May-26 20:01 databento_dbn-0.6.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     9868 b- defN 23-May-26 20:01 databento_dbn-0.6.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      135 b- defN 23-May-26 20:01 databento_dbn/__init__.py
--rw-r--r--  4.6 unx    37132 b- defN 23-May-26 20:01 databento_dbn/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-May-26 20:01 databento_dbn/py.typed
--rwxr-xr-x  4.6 unx  1555968 b- defN 23-May-26 20:01 databento_dbn/databento_dbn.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      679 b- defN 23-May-26 20:01 databento_dbn-0.6.0.dist-info/RECORD
-8 files, 1606843 bytes uncompressed, 543755 bytes compressed:  66.2%
+Zip file size: 544968 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2990 b- defN 23-Jun-02 19:02 databento_dbn-0.6.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jun-02 19:02 databento_dbn-0.6.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9868 b- defN 23-Jun-02 19:02 databento_dbn-0.6.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      135 b- defN 23-Jun-02 19:02 databento_dbn/__init__.py
+-rw-r--r--  4.6 unx    37132 b- defN 23-Jun-02 19:02 databento_dbn/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-02 19:02 databento_dbn/py.typed
+-rwxr-xr-x  4.6 unx  1553920 b- defN 23-Jun-02 19:02 databento_dbn/databento_dbn.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      679 b- defN 23-Jun-02 19:02 databento_dbn-0.6.1.dist-info/RECORD
+8 files, 1604818 bytes uncompressed, 543780 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: databento_dbn-0.6.0.dist-info/METADATA
+Filename: databento_dbn-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: databento_dbn-0.6.0.dist-info/WHEEL
+Filename: databento_dbn-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: databento_dbn-0.6.0.dist-info/license_files/LICENSE
+Filename: databento_dbn-0.6.1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: databento_dbn/__init__.py
 Comment: 
 
 Filename: databento_dbn/__init__.pyi
 Comment: 
 
 Filename: databento_dbn/py.typed
 Comment: 
 
 Filename: databento_dbn/databento_dbn.cp39-win_amd64.pyd
 Comment: 
 
-Filename: databento_dbn-0.6.0.dist-info/RECORD
+Filename: databento_dbn-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `databento_dbn-0.6.0.dist-info/METADATA` & `databento_dbn-0.6.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: databento-dbn
-Version: 0.6.0
+Version: 0.6.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
-Summary: Native Databento bindings based on dbn Rust crate
+Summary: Python bindings for encoding and decoding Databento Binary Encoding (DBN)
 Author: Databento <support@databento.com>
 Author-email: Databento <support@databento.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/databento/dbn
```

## Comparing `databento_dbn-0.6.0.dist-info/license_files/LICENSE` & `databento_dbn-0.6.1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `databento_dbn-0.6.0.dist-info/RECORD` & `databento_dbn-0.6.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-databento_dbn-0.6.0.dist-info/METADATA,sha256=64Ha0vD3yZXj960RsRRlHR3YPlEsKVjMpzeWWFLqZo4,2966
-databento_dbn-0.6.0.dist-info/WHEEL,sha256=an3xOxErGJeHkLgr587-bgaHQa25SvmEjtVGHxu1c38,95
-databento_dbn-0.6.0.dist-info/license_files/LICENSE,sha256=d69bve2VkRS216XupRiyvjZOBPT0qV-eh9mHDCdxPSQ,9868
+databento_dbn-0.6.1.dist-info/METADATA,sha256=XXLcUyVSDPajw7Rjfx1G3K13AJJY1hBAce3PDx1ruq4,2990
+databento_dbn-0.6.1.dist-info/WHEEL,sha256=uQ_TrbBhuFeDuk9Fdh4dzErtvHNb_ytk8sONwymU8b0,94
+databento_dbn-0.6.1.dist-info/license_files/LICENSE,sha256=d69bve2VkRS216XupRiyvjZOBPT0qV-eh9mHDCdxPSQ,9868
 databento_dbn/__init__.py,sha256=TeY-_YtACSjQLT3FBRPqxJrcYFf8yu_11WeB5LcyEKo,135
 databento_dbn/__init__.pyi,sha256=yp5BpGlaUsszqWG6DvCBT_Lle5cKRjZktvwazW0Ux4g,37132
 databento_dbn/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-databento_dbn/databento_dbn.cp39-win_amd64.pyd,sha256=KYWSs8liRClwREvl2A5x80Vc-9SETZDWkHfQcBInjk8,1555968
-databento_dbn-0.6.0.dist-info/RECORD,,
+databento_dbn/databento_dbn.cp39-win_amd64.pyd,sha256=KoxMq_1d0FgGo4J11ci9j8Tg9x83vA6IM9F0Szbx268,1553920
+databento_dbn-0.6.1.dist-info/RECORD,,
```

