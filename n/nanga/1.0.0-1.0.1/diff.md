# Comparing `tmp/nanga-1.0.0-py3-none-any.whl.zip` & `tmp/nanga-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -32,12 +32,12 @@
 -rw-rw-r--  2.0 unx     7312 b- defN 22-Jul-19 14:16 nanga/summarization/core/extractive/extractive_summarizer.py
 -rw-rw-r--  2.0 unx       46 b- defN 22-Jul-18 13:51 nanga/summarization/core/texts/__init__.py
 -rw-rw-r--  2.0 unx     2419 b- defN 22-Jul-19 06:48 nanga/summarization/core/texts/sentence_handler.py
 -rw-rw-r--  2.0 unx       39 b- defN 22-Jul-18 12:36 nanga/summarization/models/__init__.py
 -rw-rw-r--  2.0 unx     6866 b- defN 22-Jul-19 07:08 nanga/summarization/models/bert_models.py
 -rw-rw-r--  2.0 unx       24 b- defN 22-Jul-27 07:46 nanga/utils/__init__.py
 -rw-rw-r--  2.0 unx     1259 b- defN 22-Jul-27 07:13 nanga/utils/log.py
--rw-rw-r--  2.0 unx      798 b- defN 23-Jun-01 15:49 nanga-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-01 15:49 nanga-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Jun-01 15:49 nanga-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3615 b- defN 23-Jun-01 15:49 nanga-1.0.0.dist-info/RECORD
+-rw-rw-r--  2.0 unx      798 b- defN 23-Jun-02 09:06 nanga-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 09:06 nanga-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-02 09:06 nanga-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3615 b- defN 23-Jun-02 09:06 nanga-1.0.1.dist-info/RECORD
 41 files, 138451 bytes uncompressed, 39463 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -105,20 +105,20 @@
 
 Filename: nanga/utils/__init__.py
 Comment: 
 
 Filename: nanga/utils/log.py
 Comment: 
 
-Filename: nanga-1.0.0.dist-info/METADATA
+Filename: nanga-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: nanga-1.0.0.dist-info/WHEEL
+Filename: nanga-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: nanga-1.0.0.dist-info/top_level.txt
+Filename: nanga-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nanga-1.0.0.dist-info/RECORD
+Filename: nanga-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nanga-1.0.0.dist-info/METADATA` & `nanga-1.0.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanga
-Version: 1.0.0
+Version: 1.0.1
 Summary: NLP tasks
 Home-page: UNKNOWN
 Author: Fréjus A.A. Laleye
 Author-email: frejus.laleye@gmail.com
 Maintainer: Fréjus A. A. Laleye
 Maintainer-email: frejus.laleye@gmail.com
 License: UNKNOWN
@@ -12,16 +12,16 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: transformers (==4.25.1)
+Requires-Dist: transformers (>=4.20.1)
 Requires-Dist: joblib (==1.1.0)
-Requires-Dist: torch (==2.0.1)
+Requires-Dist: torch (>=2.0.1)
 Requires-Dist: spacy (==3.4.4)
 Requires-Dist: scikit-learn (==1.1.1)
-Requires-Dist: torchtext (==0.15.2)
+Requires-Dist: torchtext (>=0.15.2)
 
 # nanga
```

## Comparing `nanga-1.0.0.dist-info/RECORD` & `nanga-1.0.1.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -31,11 +31,11 @@
 nanga/summarization/core/extractive/extractive_summarizer.py,sha256=QWWm_86OsOknMND1Y5NnQsL_FIxKqBYPGzCNDAatHLQ,7312
 nanga/summarization/core/texts/__init__.py,sha256=_XP6TFhcMluovJLjud3WH7SlfjcFc3WiKfG4h64sWuQ,46
 nanga/summarization/core/texts/sentence_handler.py,sha256=s9FQWDWt6Fdri4NdGledpqfYNag3fl5re7-s7F74T-Q,2419
 nanga/summarization/models/__init__.py,sha256=tHYHy53-xNOHX3O-5WKpahUPXKM21uIJ2r6gF_UM9hM,39
 nanga/summarization/models/bert_models.py,sha256=iEwliMraaCJD41ichDlhyEClNO2ixYOBoqvZxTUW_W4,6866
 nanga/utils/__init__.py,sha256=BGNIj7InL5EAbQjIcaalzvkQCSy3-ykPi3e_g0kMZzQ,24
 nanga/utils/log.py,sha256=zU8C1_mnXV4z14Ilao78sUotVrurcO6ymNsQa5p5ZCY,1259
-nanga-1.0.0.dist-info/METADATA,sha256=ifHtcrT3PhvUscdPQXGZSgmrAC7OHcn5hEI5ko0ZVCg,798
-nanga-1.0.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-nanga-1.0.0.dist-info/top_level.txt,sha256=ZXWTSEH_GkKdJBBOBDRvP3gQAHrd4na5av9FCPXn85s,6
-nanga-1.0.0.dist-info/RECORD,,
+nanga-1.0.1.dist-info/METADATA,sha256=czZpusoJyhAbgNCT5xYMaerp_7IPkin4-jRTR7bH7S8,798
+nanga-1.0.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+nanga-1.0.1.dist-info/top_level.txt,sha256=ZXWTSEH_GkKdJBBOBDRvP3gQAHrd4na5av9FCPXn85s,6
+nanga-1.0.1.dist-info/RECORD,,
```

