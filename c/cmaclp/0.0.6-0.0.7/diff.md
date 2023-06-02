# Comparing `tmp/cmaclp-0.0.6-py3-none-any.whl.zip` & `tmp/cmaclp-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10321 bytes, number of entries: 9
--rw-rw-r--  2.0 unx    12776 b- defN 23-Jun-01 11:41 cmaclp/SVM_prediction.py
--rw-rw-r--  2.0 unx       21 b- defN 23-Jun-01 13:25 cmaclp/__init__.py
--rw-rw-r--  2.0 unx     1108 b- defN 23-Jun-01 11:41 cmaclp/tests/cmaclp_test.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-01 13:31 cmaclp-0.0.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx      755 b- defN 23-Jun-01 13:31 cmaclp-0.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-01 13:31 cmaclp-0.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       62 b- defN 23-Jun-01 13:31 cmaclp-0.0.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-01 13:31 cmaclp-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      713 b- defN 23-Jun-01 13:31 cmaclp-0.0.6.dist-info/RECORD
-9 files, 26891 bytes uncompressed, 9091 bytes compressed:  66.2%
+Zip file size: 10320 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    12776 b- defN 23-Jun-02 17:29 cmaclp/SVM_prediction.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-02 17:29 cmaclp/__init__.py
+-rw-r--r--  2.0 unx     1108 b- defN 23-Jun-02 17:29 cmaclp/tests/cmaclp_test.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-02 17:31 cmaclp-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      755 b- defN 23-Jun-02 17:31 cmaclp-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 17:31 cmaclp-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-02 17:31 cmaclp-0.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-02 17:31 cmaclp-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      713 b- defN 23-Jun-02 17:31 cmaclp-0.0.7.dist-info/RECORD
+9 files, 26891 bytes uncompressed, 9090 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: cmaclp/__init__.py
 Comment: 
 
 Filename: cmaclp/tests/cmaclp_test.py
 Comment: 
 
-Filename: cmaclp-0.0.6.dist-info/LICENSE
+Filename: cmaclp-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: cmaclp-0.0.6.dist-info/METADATA
+Filename: cmaclp-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: cmaclp-0.0.6.dist-info/WHEEL
+Filename: cmaclp-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: cmaclp-0.0.6.dist-info/entry_points.txt
+Filename: cmaclp-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmaclp-0.0.6.dist-info/top_level.txt
+Filename: cmaclp-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: cmaclp-0.0.6.dist-info/RECORD
+Filename: cmaclp-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmaclp/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.6"
+__version__ = "0.0.7"
```

## Comparing `cmaclp-0.0.6.dist-info/LICENSE` & `cmaclp-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cmaclp-0.0.6.dist-info/METADATA` & `cmaclp-0.0.7.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmaclp
-Version: 0.0.6
+Version: 0.0.7
 Summary: Corneal meta-atlas command line predictor
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools (<=57.5.0)
 Requires-Dist: wheel
 Requires-Dist: python-build
 Requires-Dist: pytest-cov
```

## Comparing `cmaclp-0.0.6.dist-info/RECORD` & `cmaclp-0.0.7.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmaclp/SVM_prediction.py,sha256=9Ydy_aEb2EDTLnlVEjy6fN1EBsOHHRKTCprq-l_etzc,12776
-cmaclp/__init__.py,sha256=CzcXzRPJNqTNVzWp48bKd5k9CaHSjpVkLYKkiQcGpAY,21
+cmaclp/__init__.py,sha256=D0UVD6fSKhTEm2bcEShuydq4MtAQfmIq3CLzUVZH53I,21
 cmaclp/tests/cmaclp_test.py,sha256=Qq8FYvzrnfVwNsaknF_RxBEuZV79w7EGA9z-mg9Fc3A,1108
-cmaclp-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cmaclp-0.0.6.dist-info/METADATA,sha256=cOzQ_OIp6msxv0ZO8W5CM7uB6JM79MFQIsKlWJMcbSk,755
-cmaclp-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cmaclp-0.0.6.dist-info/entry_points.txt,sha256=yc4QzRXLMSJ3eu6IwPrSMsaTxxv0ONJ2nhS9c8n7HzY,62
-cmaclp-0.0.6.dist-info/top_level.txt,sha256=aDpLhklg1da22MWr2NS6Do368bNv2rlOX_pk5T57tS4,7
-cmaclp-0.0.6.dist-info/RECORD,,
+cmaclp-0.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cmaclp-0.0.7.dist-info/METADATA,sha256=iY7TBXRSMRDUFBw-p1sNDaWOYT2fJniVmN8EPnaGpVc,755
+cmaclp-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cmaclp-0.0.7.dist-info/entry_points.txt,sha256=yc4QzRXLMSJ3eu6IwPrSMsaTxxv0ONJ2nhS9c8n7HzY,62
+cmaclp-0.0.7.dist-info/top_level.txt,sha256=aDpLhklg1da22MWr2NS6Do368bNv2rlOX_pk5T57tS4,7
+cmaclp-0.0.7.dist-info/RECORD,,
```

