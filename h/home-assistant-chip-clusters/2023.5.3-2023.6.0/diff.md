# Comparing `tmp/home_assistant_chip_clusters-2023.5.3-py3-none-any.whl.zip` & `tmp/home_assistant_chip_clusters-2023.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 103841 bytes, number of entries: 13
--rw-r--r--  2.0 unx     2154 b- defN 23-May-26 08:51 chip/ChipUtility.py
--rw-r--r--  2.0 unx   314619 b- defN 23-May-26 08:51 chip/clusters/CHIPClusters.py
--rw-r--r--  2.0 unx    12945 b- defN 23-May-26 08:51 chip/clusters/ClusterObjects.py
--rw-r--r--  2.0 unx  1296745 b- defN 23-May-26 08:51 chip/clusters/Objects.py
--rw-r--r--  2.0 unx     1947 b- defN 23-May-26 08:51 chip/clusters/TestObjects.py
--rw-r--r--  2.0 unx     1014 b- defN 23-May-26 08:51 chip/clusters/Types.py
--rw-r--r--  2.0 unx     2404 b- defN 23-May-26 08:51 chip/clusters/enum.py
--rw-r--r--  2.0 unx    28802 b- defN 23-May-26 08:51 chip/tlv/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-26 08:51 home_assistant_chip_clusters-2023.5.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      548 b- defN 23-May-26 08:51 home_assistant_chip_clusters-2023.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 08:51 home_assistant_chip_clusters-2023.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-26 08:51 home_assistant_chip_clusters-2023.5.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1162 b- defN 23-May-26 08:51 home_assistant_chip_clusters-2023.5.3.dist-info/RECORD
-13 files, 1673794 bytes uncompressed, 101885 bytes compressed:  93.9%
+Zip file size: 103843 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     2154 b- defN 23-Jun-02 10:25 chip/ChipUtility.py
+-rw-r--r--  2.0 unx   314619 b- defN 23-Jun-02 10:25 chip/clusters/CHIPClusters.py
+-rw-r--r--  2.0 unx    12945 b- defN 23-Jun-02 10:25 chip/clusters/ClusterObjects.py
+-rw-r--r--  2.0 unx  1296745 b- defN 23-Jun-02 10:25 chip/clusters/Objects.py
+-rw-r--r--  2.0 unx     1947 b- defN 23-Jun-02 10:25 chip/clusters/TestObjects.py
+-rw-r--r--  2.0 unx     1014 b- defN 23-Jun-02 10:25 chip/clusters/Types.py
+-rw-r--r--  2.0 unx     2404 b- defN 23-Jun-02 10:25 chip/clusters/enum.py
+-rw-r--r--  2.0 unx    28802 b- defN 23-Jun-02 10:25 chip/tlv/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-02 10:25 home_assistant_chip_clusters-2023.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      548 b- defN 23-Jun-02 10:25 home_assistant_chip_clusters-2023.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 10:25 home_assistant_chip_clusters-2023.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-02 10:25 home_assistant_chip_clusters-2023.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1162 b- defN 23-Jun-02 10:25 home_assistant_chip_clusters-2023.6.0.dist-info/RECORD
+13 files, 1673794 bytes uncompressed, 101887 bytes compressed:  93.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: chip/clusters/enum.py
 Comment: 
 
 Filename: chip/tlv/__init__.py
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.3.dist-info/LICENSE
+Filename: home_assistant_chip_clusters-2023.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.3.dist-info/METADATA
+Filename: home_assistant_chip_clusters-2023.6.0.dist-info/METADATA
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.3.dist-info/WHEEL
+Filename: home_assistant_chip_clusters-2023.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.3.dist-info/top_level.txt
+Filename: home_assistant_chip_clusters-2023.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.3.dist-info/RECORD
+Filename: home_assistant_chip_clusters-2023.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `home_assistant_chip_clusters-2023.5.3.dist-info/LICENSE` & `home_assistant_chip_clusters-2023.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `home_assistant_chip_clusters-2023.5.3.dist-info/METADATA` & `home_assistant_chip_clusters-2023.6.0.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-chip-clusters
-Version: 2023.5.3
+Version: 2023.6.0
 Summary: Python-base APIs and tools for CHIP.
 Home-page: https://github.com/project-chip/connectedhomeip
 License: Apache
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `home_assistant_chip_clusters-2023.5.3.dist-info/RECORD` & `home_assistant_chip_clusters-2023.6.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 chip/clusters/CHIPClusters.py,sha256=rEIS3hnjd9nT3c_M3UGibQy_XnWIgI1F0XAz0_NSLW4,314619
 chip/clusters/ClusterObjects.py,sha256=S2Bc0oUe6Wo4OYnlFfT6BB3GaZculvTGVUxkJqq7JAc,12945
 chip/clusters/Objects.py,sha256=yYKeyip-F-PcJUjAaOB41Co2yAtvG9NWr2ik3akFIbM,1296745
 chip/clusters/TestObjects.py,sha256=Az2iQd-H0sN9tXOjLQkzd8nMA5STRFTMButw-8ro5GQ,1947
 chip/clusters/Types.py,sha256=sRRy-_Bec3EaXIs1XNXr6qFRqXckn2YAgwvoD4ISjC4,1014
 chip/clusters/enum.py,sha256=zw06GH82ONj3CIHKNI4sr7QnBXEr7vBB6zQnYFVAvYg,2404
 chip/tlv/__init__.py,sha256=SeIN82CcAqgyte0dcbNQwqUJULlUHRmqRMG_0HYowc0,28802
-home_assistant_chip_clusters-2023.5.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-home_assistant_chip_clusters-2023.5.3.dist-info/METADATA,sha256=IsSe_YU_Exv1_bqEWFbGYeLwnQo-bQf9QTnwTee27Vg,548
-home_assistant_chip_clusters-2023.5.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-home_assistant_chip_clusters-2023.5.3.dist-info/top_level.txt,sha256=5pBsfKK6BMqu66YKYb0-uQqOgrqirLFfcBFAxXDNme0,5
-home_assistant_chip_clusters-2023.5.3.dist-info/RECORD,,
+home_assistant_chip_clusters-2023.6.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+home_assistant_chip_clusters-2023.6.0.dist-info/METADATA,sha256=tgl18MAhOaUlm0cbuzWztGb6zrdjchWRqW6lqwMua3A,548
+home_assistant_chip_clusters-2023.6.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+home_assistant_chip_clusters-2023.6.0.dist-info/top_level.txt,sha256=5pBsfKK6BMqu66YKYb0-uQqOgrqirLFfcBFAxXDNme0,5
+home_assistant_chip_clusters-2023.6.0.dist-info/RECORD,,
```

