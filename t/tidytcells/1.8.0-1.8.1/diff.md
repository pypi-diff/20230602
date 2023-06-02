# Comparing `tmp/tidytcells-1.8.0.tar.gz` & `tmp/tidytcells-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidytcells-1.8.0.tar", last modified: Tue May 23 16:25:09 2023, max compression
+gzip compressed data, was "tidytcells-1.8.1.tar", last modified: Fri Jun  2 16:52:54 2023, max compression
```

## Comparing `tidytcells-1.8.0.tar` & `tidytcells-1.8.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.854359 tidytcells-1.8.0/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-12-06 13:03:03.000000 tidytcells-1.8.0/LICENSE.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-12-06 13:03:03.000000 tidytcells-1.8.0/MANIFEST.in
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-05-23 16:25:09.854359 tidytcells-1.8.0/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1433 2023-05-23 15:08:38.000000 tidytcells-1.8.0/README.md
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-05-23 16:21:15.000000 tidytcells-1.8.0/VERSION.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-05-23 16:25:09.854359 tidytcells-1.8.0/setup.cfg
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1287 2023-05-23 16:19:34.000000 tidytcells-1.8.0/setup.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.845358 tidytcells-1.8.0/src/
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.846358 tidytcells-1.8.0/src/tidytcells/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/__init__.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.850358 tidytcells-1.8.0/src/tidytcells/_resources/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1283 2023-05-23 16:14:45.000000 tidytcells-1.8.0/src/tidytcells/_resources/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   611997 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-05-23 16:03:07.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-05-23 16:03:08.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-05-23 16:03:08.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_tcr.json
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.851359 tidytcells-1.8.0/src/tidytcells/_utils/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_utils/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4336 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/_utils/abstract_functions.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/_utils/gene_query_engines.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10869 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/_utils/gene_standardisers.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      553 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/_utils/warnings.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.852358 tidytcells-1.8.0/src/tidytcells/aa/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/aa/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/aa/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.852358 tidytcells-1.8.0/src/tidytcells/junction/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/junction/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/junction/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.852358 tidytcells-1.8.0/src/tidytcells/mhc/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      403 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/mhc/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9648 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/mhc/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.853358 tidytcells-1.8.0/src/tidytcells/tcr/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/tcr/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8425 2023-05-23 16:22:37.000000 tidytcells-1.8.0/src/tidytcells/tcr/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.847359 tidytcells-1.8.0/src/tidytcells.egg-info/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/SOURCES.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/dependency_links.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       89 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/requires.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/top_level.txt
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.853358 tidytcells-1.8.0/tests/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-05-23 15:08:38.000000 tidytcells-1.8.0/tests/test_aa.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-05-23 15:08:38.000000 tidytcells-1.8.0/tests/test_junction.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8969 2023-05-23 15:08:38.000000 tidytcells-1.8.0/tests/test_mhc.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8072 2023-05-23 16:10:54.000000 tidytcells-1.8.0/tests/test_tcr.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.677380 tidytcells-1.8.1/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-12-06 13:03:03.000000 tidytcells-1.8.1/LICENSE.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-12-06 13:03:03.000000 tidytcells-1.8.1/MANIFEST.in
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-06-02 16:52:54.677380 tidytcells-1.8.1/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1433 2023-06-02 16:02:49.000000 tidytcells-1.8.1/README.md
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-02 16:49:12.000000 tidytcells-1.8.1/VERSION.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-02 16:52:54.677380 tidytcells-1.8.1/setup.cfg
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1287 2023-06-02 16:02:49.000000 tidytcells-1.8.1/setup.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.660380 tidytcells-1.8.1/src/
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.662380 tidytcells-1.8.1/src/tidytcells/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-06-02 16:02:49.000000 tidytcells-1.8.1/src/tidytcells/__init__.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.675380 tidytcells-1.8.1/src/tidytcells/_resources/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1283 2023-06-02 16:02:49.000000 tidytcells-1.8.1/src/tidytcells/_resources/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   611997 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-05-23 16:03:07.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-02 16:02:49.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-05-23 16:03:08.000000 tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_tcr.json
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.676380 tidytcells-1.8.1/src/tidytcells/_utils/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-02 13:53:55.000000 tidytcells-1.8.1/src/tidytcells/_utils/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4225 2023-06-02 16:09:52.000000 tidytcells-1.8.1/src/tidytcells/_utils/abstract_functions.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-06-02 16:02:49.000000 tidytcells-1.8.1/src/tidytcells/_utils/gene_query_engines.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    11289 2023-06-02 16:08:36.000000 tidytcells-1.8.1/src/tidytcells/_utils/gene_standardizers.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-02 16:10:03.000000 tidytcells-1.8.1/src/tidytcells/_utils/warnings.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.676380 tidytcells-1.8.1/src/tidytcells/aa/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-02 16:10:51.000000 tidytcells-1.8.1/src/tidytcells/aa/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-06-02 16:10:30.000000 tidytcells-1.8.1/src/tidytcells/aa/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.676380 tidytcells-1.8.1/src/tidytcells/junction/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-02 16:11:27.000000 tidytcells-1.8.1/src/tidytcells/junction/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-06-02 16:11:13.000000 tidytcells-1.8.1/src/tidytcells/junction/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.676380 tidytcells-1.8.1/src/tidytcells/mhc/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-02 16:45:57.000000 tidytcells-1.8.1/src/tidytcells/mhc/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10302 2023-06-02 16:38:32.000000 tidytcells-1.8.1/src/tidytcells/mhc/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.677380 tidytcells-1.8.1/src/tidytcells/tcr/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-02 16:06:36.000000 tidytcells-1.8.1/src/tidytcells/tcr/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8597 2023-06-02 16:40:17.000000 tidytcells-1.8.1/src/tidytcells/tcr/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.662380 tidytcells-1.8.1/src/tidytcells.egg-info/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/SOURCES.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/dependency_links.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       89 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/requires.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-02 16:52:54.000000 tidytcells-1.8.1/src/tidytcells.egg-info/top_level.txt
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-02 16:52:54.677380 tidytcells-1.8.1/tests/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-06-02 16:02:49.000000 tidytcells-1.8.1/tests/test_aa.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-06-02 16:02:49.000000 tidytcells-1.8.1/tests/test_junction.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9153 2023-06-02 16:38:32.000000 tidytcells-1.8.1/tests/test_mhc.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8118 2023-06-02 16:39:27.000000 tidytcells-1.8.1/tests/test_tcr.py
```

### Comparing `tidytcells-1.8.0/LICENSE.txt` & `tidytcells-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/PKG-INFO` & `tidytcells-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.0
+Version: 1.8.1
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.0/README.md` & `tidytcells-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/setup.py` & `tidytcells-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_resources/__init__.py` & `tidytcells-1.8.1/src/tidytcells/_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_mhc.json` & `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json` & `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr.json` & `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json` & `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json` & `tidytcells-1.8.1/src/tidytcells/_resources/homosapiens_tcr_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_mhc.json` & `tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json` & `tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_tcr.json` & `tidytcells-1.8.1/src/tidytcells/_resources/musmusculus_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_utils/abstract_functions.py` & `tidytcells-1.8.1/src/tidytcells/_utils/abstract_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+from .gene_standardizers import GeneStandardizer
 import re
 from .._resources import AMINO_ACIDS
-from typing import FrozenSet, Optional
+from typing import Dict, FrozenSet, Optional
 from .warnings import *
 
 
-def standardise_template(
+def standardize_template(
     gene: str,
     gene_type: str,
     species: str,
     enforce_functional: bool,
     precision: str,
     suppress_warnings: bool,
-    standardiser_dict: dict,
+    standardizer_dict: Dict[str, GeneStandardizer],
     allowed_precision: set,
 ) -> str:
-    # Type checks
     if type(gene) != str:
         raise TypeError(f"gene_name must be type str, got {gene} ({type(gene)}).")
     if type(species) != str:
         raise TypeError(f"species must be type str, got {species} ({type(species)}).")
     if type(enforce_functional) != bool:
         raise TypeError(
             "enforce_functional must be type bool, got "
@@ -30,54 +30,54 @@
         )
     if type(suppress_warnings) != bool:
         raise TypeError(
             "suppress_warnings must be type bool, got "
             f"{suppress_warnings} ({type(suppress_warnings)})."
         )
 
-    # Allowed value checks
     if not precision in allowed_precision:
         raise ValueError(f"precision must be in {allowed_precision}, got {precision}.")
 
     # For backward compatibility, fix CamelCased species
     species = "".join(species.split()).lower()
 
-    # If the specified species is not supported, no-op (with warning)
-    if not species in standardiser_dict:
+    if not species in standardizer_dict:
         if not suppress_warnings:
             warn_unsupported_species(species, gene_type)
         return gene
 
-    # Take note of initial input for reference
     original_input = gene
 
-    # Clean whitespace, remove known pollutors, uppercase
     gene = "".join(gene.split())
     gene = gene.replace("&nbsp;", "")
     gene = gene.upper()
 
-    # Standardisation attempt
-    standardised = standardiser_dict[species](gene)
+    standardized = standardizer_dict[species](gene)
 
-    if not standardised.valid(enforce_functional):  # Standaridsation failure
+    invalid_reason = standardized.invalid(enforce_functional)
+    if invalid_reason:
         if not suppress_warnings:
-            warn_failure(original_input, standardised.compile("allele"), species)
+            warn_failure(
+                reason_for_failure=invalid_reason,
+                original_input=original_input,
+                attempted_fix=standardized.compile("allele"),
+                species=species,
+            )
         return None
 
-    return standardised.compile(precision)
+    return standardized.compile(precision)
 
 
 def query_template(
     species: str,
     precision: str,
     functionality: str,
     contains: Optional[str],
     query_engine_dict: dict,
 ) -> FrozenSet[str]:
-    # Type checks
     if type(species) != str:
         raise TypeError(f"species must be type str, got {species} ({type(species)}).")
     if type(functionality) != str:
         raise TypeError(
             f"functionality must be type str, got {functionality} ({type(functionality)})."
         )
     if type(precision) != str:
@@ -85,15 +85,14 @@
             f"precision must be type str, got {precision} ({type(precision)})."
         )
     if not (contains is None or type(contains) == str):
         raise TypeError(
             f"contains must be either None or type str, got {contains} ({type(contains)})."
         )
 
-    # Allowed value checks
     if not precision in {"allele", "gene"}:
         raise ValueError(
             f'precision must be either "allele" or "gene", got {precision}.'
         )
     if not functionality in {"any", "F", "NF", "P", "ORF"}:
         raise ValueError(
             f'functionality must be "any", "F", "NF", "P", or "ORF", got {functionality}.'
@@ -111,20 +110,18 @@
 
     if contains is None:
         return result
 
     return frozenset([i for i in result if re.search(contains, i)])
 
 
-def standardise_aa_template(seq: str, suppress_warnings: bool):
-    # type checks
+def standardize_aa_template(seq: str, suppress_warnings: bool):
     if type(seq) != str:
         raise TypeError(f"seq must be type str, got {seq} ({type(seq)}).")
 
-    # take note of original input
     original_input = seq
 
     seq = seq.upper()
 
     for char in seq:
         if not char in AMINO_ACIDS:
             if not suppress_warnings:
```

### Comparing `tidytcells-1.8.0/src/tidytcells/_utils/gene_query_engines.py` & `tidytcells-1.8.1/src/tidytcells/_utils/gene_query_engines.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/src/tidytcells/_utils/gene_standardisers.py` & `tidytcells-1.8.1/src/tidytcells/_utils/gene_standardizers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Gene standardiser classes
+Gene standardizer classes
 """
 
 
 from abc import ABC, abstractmethod
 from itertools import product
 import re
 from .._resources import *
@@ -13,49 +13,57 @@
 
 
 SUB_DV_RE = re.compile(r"(?<!TR)(?<!\/)DV")
 SUB_OR_RE = re.compile(r"(?<!\/)OR")
 SUB_ZERO_RE = re.compile(r"(?<!\d)0")
 
 
-# --- STANDARDISER CLASSES ---
+# --- STANDARDIZER CLASSES ---
 
 
-class GeneStandardiser(ABC):
+class GeneStandardizer(ABC):
     """
-    Abstract base standardiser class.
+    Abstract base standardizer class.
     """
 
     @abstractmethod
     def __init__(self, gene: str) -> None:
         """
-        Init method for the standardiser objects. Should expect a whitespace-
+        Init method for the standardizer objects. Should expect a whitespace-
         cleaned, uppercased string to be supplied to the 'gene' parameter.
         """
 
-    @abstractmethod
     def valid(self, enforce_functional: bool = False) -> bool:
         """
-        Returns True if the gene's name is a real, valid and existing one.
-        Else returns False. If enforce_functional, additionally verify that
-        the gene in question is functional.
+        Taking into account whether enforcing functionality or not, returns
+        True if the gene/allele is valid in its current state. Returns False
+        otherwise.
+        """
+        return self.invalid(enforce_functional) is None
+
+    @abstractmethod
+    def invalid(self, enforce_functional: bool = False) -> bool:
+        """
+        If the gene cannot be standardized (it is invalid), this method returns
+        a string outlining the reason why (nonexistent gene, not functional,
+        etc.). Returns None if standardisation was successful.
         """
 
     @abstractmethod
     def compile(self, precision: str = "allele") -> str:
         """
         Compile a complete string representation of the gene. The argument
         given to precision will determine the amount of specificity given
         in the compiled string.
         """
 
 
-class TCRStandardiser(GeneStandardiser):
+class TCRStandardizer(GeneStandardizer):
     """
-    TCR standardiser base class.
+    TCR standardizer base class.
     """
 
     ref_dict = None
     syn_dict = None
 
     def __init__(self, gene: str) -> None:
         self.parse_gene_str(gene)
@@ -108,58 +116,60 @@
         # Resolve AV designation from DV is necessary
         if self.gene.startswith("TRDV"):
             for valid_gene in self.ref_dict:
                 if re.match(rf"^TRAV\d+(-\d)?\/{self.gene[2:]}$", valid_gene):
                     self.gene = valid_gene
                     return
 
-    def valid(self, enforce_functional: bool = False) -> bool:
-        # Is the gene valid?
+    def invalid(self, enforce_functional: bool = False) -> bool:
         if not self.gene in self.ref_dict:
-            return False
+            return "unrecognised gene name"
 
-        # If the gene exists and an allele is specified, check if it exists
         if self.allele_designation:
             allele_valid = self.allele_designation in self.ref_dict[self.gene]
 
-            if not enforce_functional:
-                return allele_valid
+            if not allele_valid:
+                return "nonexistent allele for recognised gene"
+
+            if (
+                enforce_functional
+                and self.ref_dict[self.gene][self.allele_designation] != "F"
+            ):
+                return "nonfunctional allele"
 
-            return self.ref_dict[self.gene][self.allele_designation] == "F"
+            return None
 
-        # If enforce_functional, ensure there is at least one functional allele
-        if enforce_functional:
-            return "F" in self.ref_dict[self.gene].values()
+        if enforce_functional and not "F" in self.ref_dict[self.gene].values():
+            return "gene has no functional alleles"
 
-        # Otherwise gene is valid so return true
-        return True
+        return None
 
     def compile(self, precision: str = "allele") -> str:
         if precision == "allele" and self.allele_designation:
             return f"{self.gene}*{self.allele_designation}"
 
         return self.gene
 
 
-class HomoSapiensTCRStandardiser(TCRStandardiser):
+class HomoSapiensTCRStandardizer(TCRStandardizer):
     ref_dict = HOMOSAPIENS_TCR
     syn_dict = HOMOSAPIENS_TCR_SYNONYMS
 
     def resolve_errors(self) -> None:
         super().resolve_errors()
 
         # Fix common errors
         self.gene = re.sub(r"(?<!\/)OR", "/OR", self.gene)
 
 
-class MusMusculusTCRStandardiser(TCRStandardiser):
+class MusMusculusTCRStandardizer(TCRStandardizer):
     ref_dict = MUSMUSCULUS_TCR
 
 
-class HLAStandardiser(GeneStandardiser):
+class HLAStandardizer(GeneStandardizer):
     def __init__(self, gene: str) -> None:
         self.parse_gene(gene)
         self.resolve_errors()
 
     def parse_gene(self, gene: str) -> None:
         if gene == "B2M":
             self.gene = "B2M"
@@ -249,65 +259,62 @@
         ads = [int(ad) for ad in self.allele_designation[:2]]
         ads_reformatted = [[f"{ad:02}", f"{ad:03}"] for ad in ads]
         for new_ads in product(*ads_reformatted):
             self.allele_designation = list(new_ads) + self.allele_designation[2:]
             if self.valid():
                 return
 
-    def valid(self, enforce_functional: bool = False) -> bool:
-        # Is the gene B2M?
+    def invalid(self, enforce_functional: bool = False) -> bool:
         if self.gene == "B2M" and not self.allele_designation:
-            return True
+            return None
 
-        # Is the gene valid?
         if not self.gene in HOMOSAPIENS_MHC:
-            return False
+            return "unrecognised gene name"
 
         # Verify allele designators up to the level of the protein (or G/P)
         allele_designation = self.allele_designation.copy()
         if not self.is_group:
             allele_designation = allele_designation[:2]
         current_root = HOMOSAPIENS_MHC[self.gene]
 
         while len(allele_designation) > 0:
             try:
                 current_root = current_root[allele_designation.pop(0)]
             except KeyError:
-                return False
+                return "nonexistent allele for recognised gene"
 
         # If there are designator fields past the protein level, just make sure
         # they look like legitimate designator field values
         if not self.is_group and len(self.allele_designation) > 2:
             further_designators = self.allele_designation[2:]
 
             if len(further_designators) > 2:
-                return False
+                return "too many allele designators"
 
             for field in further_designators:
                 if not field.isdigit():
-                    return False
+                    return "non-numerical allele designators"
 
                 if len(field) < 2:
-                    return False
+                    return "non-2-digit allele designators"
 
-        # Valid gene with valid specifier fields, so valid!
-        return True
+        return None
 
     def compile(self, precision) -> str:
         if self.allele_designation:
             if precision == "allele":
                 return f'{self.gene}*{":".join(self.allele_designation)}'
 
             if precision == "protein":
                 return f'{self.gene}*{":".join(self.allele_designation[:2])}'
 
         return self.gene
 
 
-class MusMusculusMHCStandardiser(GeneStandardiser):
+class MusMusculusMHCStandardizer(GeneStandardizer):
     def __init__(self, gene: str) -> None:
         self.parse_gene(gene)
         self.resolve_errors()
 
     def parse_gene(self, gene: str) -> None:
         parse_attempt = re.match(r"^([A-Z0-9\-\.\(\)\/]+)(\*(\d+))?", gene)
 
@@ -329,15 +336,18 @@
 
         # If a synonym, correct to currently approved name
         if self.gene.replace("-", "") in MUSMUSCULUS_MHC_SYNONYMS:
             self.gene = MUSMUSCULUS_MHC_SYNONYMS[self.gene.replace("-", "")]
             if self.valid():
                 return
 
-    def valid(self, enforce_functional: bool = False) -> bool:
-        return self.gene in MUSMUSCULUS_MHC
+    def invalid(self, enforce_functional: bool = False) -> bool:
+        if not self.gene in MUSMUSCULUS_MHC:
+            return "unrecognised gene name"
+
+        return None
 
     def compile(self, precision: str = "allele") -> str:
         if precision == "allele" and self.allele_designation:
             return f"{self.gene}*{self.allele_designation}"
 
         return self.gene
```

### Comparing `tidytcells-1.8.0/src/tidytcells/aa/_main.py` & `tidytcells-1.8.1/src/tidytcells/aa/_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .._utils.abstract_functions import standardise_aa_template
+from .._utils.abstract_functions import standardize_aa_template
 
 
-def standardise(seq: str, suppress_warnings: bool = False):
+def standardize(seq: str, suppress_warnings: bool = False):
     """
     Ensures that a string value looks like a valid amino acid sequence.
 
     :param seq:
         String value representing an amino acid sequence.
     :type seq:
         ``str``
@@ -21,19 +21,19 @@
     :rtype:
         ``str`` or ``None``
 
     .. topic:: Example usage
 
         Strings that look like amino acid sequences will be accepted, and returned in capitalised form.
 
-        >>> tt.aa.standardise("sqllnakyl")
+        >>> tt.aa.standardize("sqllnakyl")
         'SQLLNAKYL'
 
         Any strings that contain characters that cannot be recognised as amino acids will be rejected, and the function will return ``None``.
 
-        >>> result = tt.aa.standardise("sqll?akyl")
+        >>> result = tt.aa.standardize("sqll?akyl")
         UserWarning: Input sqll?akyl was rejected as it is not a valid amino acid sequence.
         >>> print(result)
         None
     """
 
-    return standardise_aa_template(seq, suppress_warnings)
+    return standardize_aa_template(seq, suppress_warnings)
```

### Comparing `tidytcells-1.8.0/src/tidytcells/junction/_main.py` & `tidytcells-1.8.1/src/tidytcells/junction/_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
-from .._utils.abstract_functions import standardise_aa_template
+from .._utils.abstract_functions import standardize_aa_template
 from warnings import warn
 
 
-def standardise(seq: str, strict: bool = False, suppress_warnings: bool = False):
+def standardize(seq: str, strict: bool = False, suppress_warnings: bool = False):
     """
     Ensures that a string value looks like a valid junction (CDR3) amino acid sequence.
-    This function is a special variant of :py:func:`tidytcells.aa.standardise`.
+    This function is a special variant of :py:func:`tidytcells.aa.standardize`.
 
     A valid junction sequence must:
 
     1. Be a valid amino acid sequence
     2. Begin with a cysteine (C)
     3. End with a phenylalanine (F) or a tryptophan (W)
 
@@ -27,43 +27,43 @@
     :param suppress_warnings:
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
         ``bool``
 
     :return:
-        If possible, a standardised version of the input string is returned.
-        If the input string cannot be standardised, it is rejected and ``None`` is returned.
+        If possible, a standardized version of the input string is returned.
+        If the input string cannot be standardized, it is rejected and ``None`` is returned.
     :rtype:
         ``str`` or ``None``
 
     .. topic:: Example usage
 
         Strings that look like junction sequences will be accepted, and returned in capitalised form.
 
-        >>> tt.junction.standardise("csadaff")
+        >>> tt.junction.standardize("csadaff")
         'CSADAFF'
 
         Strings that are valid amino acid sequences but do not stard and end with the appropriate residues will have a C and an F appended to its beginning and end respectively.
 
-        >>> tt.junction.standardise("sadaf")
+        >>> tt.junction.standardize("sadaf")
         'CSADAFF'
 
         However, setting ``strict`` to ``True`` will cause these cases to be rejected.
 
-        >>> result = tt.junction.standardise("sadaf", strict=True)
+        >>> result = tt.junction.standardize("sadaf", strict=True)
         UserWarning: Input sadaf was rejected as it is not a valid junction sequence.
         >>> print(result)
         None
     """
 
     # take note of original input
     original_input = seq
 
-    seq = standardise_aa_template(seq, suppress_warnings)
+    seq = standardize_aa_template(seq, suppress_warnings)
 
     if seq is None:  # not a valid amino acid sequence
         return None
 
     if not re.match(f"^C[A-Z]*[FW]$", seq):
         if strict:
             if not suppress_warnings:
```

### Comparing `tidytcells-1.8.0/src/tidytcells/mhc/_main.py` & `tidytcells-1.8.1/src/tidytcells/mhc/_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,125 +2,129 @@
 Utility functions related to MHCs and MHC genes.
 """
 
 
 import re
 from .._resources import *
 from typing import Optional, FrozenSet
-from .._utils.abstract_functions import standardise_template, query_template
+from .._utils.abstract_functions import standardize_template, query_template
 from .._utils.gene_query_engines import HLAQueryEngine, MusMusculusMHCQueryEngine
-from .._utils.gene_standardisers import HLAStandardiser, MusMusculusMHCStandardiser
+from .._utils.gene_standardizers import HLAStandardizer, MusMusculusMHCStandardizer
 from .._utils.warnings import *
 
 
 # --- STATIC RESOURCES ---
 
 CHAIN_ALPHA_RE = re.compile(r"HLA-([ABCEFG]|D[PQR]A)")
 CHAIN_BETA_RE = re.compile(r"HLA-D[PQR]B|B2M")
 CLASS_1_RE = re.compile(r"HLA-[ABCEFG]|B2M")
 CLASS_2_RE = re.compile(r"HLA-D[PQR][AB]")
 
 
 # --- MAIN FUNCTIONS ---
 
-STANDARDISERS = {
-    "homosapiens": HLAStandardiser,
-    "musmusculus": MusMusculusMHCStandardiser,
+STANDARDIZERS = {
+    "homosapiens": HLAStandardizer,
+    "musmusculus": MusMusculusMHCStandardizer,
 }
 
 QUERY_ENGINES = {
     "homosapiens": HLAQueryEngine,
     "musmusculus": MusMusculusMHCQueryEngine,
 }
 
 
-def standardise(
+def standardize(
     gene: Optional[str] = None,
     species: str = "homosapiens",
     precision: str = "allele",
     suppress_warnings: bool = False,
     gene_name: Optional[str] = None,
 ) -> tuple:
     """
-    Attempt to standardise an MHC gene name to be IMGT-compliant.
+    Attempt to standardize an MHC gene name to be IMGT-compliant.
 
     .. topic:: Supported species
 
         - ``'homosapiens'``
         - ``'musmusculus'``
 
     .. note::
         This function will only verify the validity of an MHC gene/allele up to the level of the protein.
         Any further precise allele designations will not be verified, apart from the requirement that the format (colon-separated numbers) look valid.
         The reasons for this is firstly because new alleles at that level are added to the IMGT list quite often and so accurate verification is difficult, secondly because people rarely need verification to such a precise level, and finally because such verification costs more computational effort with diminishing returns.
 
     :param gene:
-        Potentially non-standardised MHC gene name.
+        Potentially non-standardized MHC gene name.
     :type gene:
         ``str``
     :param species:
         Species to which the MHC gene belongs (see above for supported species).
         Defaults to ``'homosapiens'``.
     :type species:
         ``str``
     :param precision:
-        The maximum level of precision to standardise to.
-        ``'allele'`` standardises to the maximum precision possible.
+        The maximum level of precision to standardize to.
+        ``'allele'`` standardizes to the maximum precision possible.
         ``'protein'`` keeps allele designators up to the level of the protein.
-        ``'gene'`` standardises only to the level of the gene.
+        ``'gene'`` standardizes only to the level of the gene.
         Defaults to ``'allele'``.
     :type precision:
         ``str``
     :param suppress_warnings:
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
         ``bool``
 
     :param gene_name:
-        Alias for the parameter ``gene``.
+        Alias for the parameter ``gene``. This will be deprecated soon.
     :type gene_name:
         ``str``
 
     :return:
-        If the specified ``species`` is supported, and ``gene`` could be standardised, then return the standardised gene name.
-        If ``species`` is unsupported, then the function does not attempt to standardise, and returns the unaltered ``gene`` string.
+        If the specified ``species`` is supported, and ``gene`` could be standardized, then return the standardized gene name.
+        If ``species`` is unsupported, then the function does not attempt to standardize, and returns the unaltered ``gene`` string.
         Else returns ``None``.
     :rtype:
         ``str`` or ``None``
 
     .. topic:: Example usage
 
         Input strings will intelligently be corrected to IMGT-compliant gene symbols.
 
-        >>> tt.mhc.standardise("A1")
+        >>> tt.mhc.standardize("A1")
         'HLA-A*01'
 
         The ``precision`` setting can truncate unnecessary information.
 
-        >>> tt.mhc.standardise("HLA-A*01", precision="gene")
+        >>> tt.mhc.standardize("HLA-A*01", precision="gene")
         'HLA-A'
 
         *Mus musculus* is a supported species.
 
-        >>> tt.mhc.standardise("CRW2", species="musmusculus")
+        >>> tt.mhc.standardize("CRW2", species="musmusculus")
         'MH1-M5'
     """
     # Alias resolution
-    if gene is None:
+    if gene is None and not gene_name is None:
+        warn(
+            'The parameter "gene_name" will be deprecated in the near future. Please switch to using "gene".',
+            FutureWarning,
+        )
         gene = gene_name
 
-    return standardise_template(
+    return standardize_template(
         gene=gene,
         gene_type="MHC",
         species=species,
         enforce_functional=True,
         precision=precision,
         suppress_warnings=suppress_warnings,
-        standardiser_dict=STANDARDISERS,
+        standardizer_dict=STANDARDIZERS,
         allowed_precision={"allele", "protein", "gene"},
     )
 
 
 def query(
     species: str = "homosapiens",
     precision: str = "allele",
@@ -188,32 +192,32 @@
 
 def get_chain(
     gene: Optional[str] = None,
     suppress_warnings: bool = False,
     gene_name: Optional[str] = None,
 ) -> str:
     """
-    Given a standardised MHC gene name, detect whether it codes for an alpha or a beta chain molecule.
+    Given a standardized MHC gene name, detect whether it codes for an alpha or a beta chain molecule.
 
     .. note::
 
         This function currently only recognises HLAs, and not MHCs from other species.
 
     :param gene:
-        Standardised MHC gene name
+        Standardized MHC gene name
     :type gene:
         ``str``
     :param suppress_warnings:
         Disable warnings that are usually emitted when chain classification fails.
         Defaults to ``False``.
     :type suppress_warnings:
         ``bool``
 
     :param gene_name:
-        Alias for the parameter ``gene``.
+        Alias for the parameter ``gene``. This will be deprecated soon.
     :type gene_name:
         ``str``
 
     :return:
         ``'alpha'`` or ``'beta'`` if ``gene`` is recognised and its chain is known, else ``None``.
     :rtype:
         ``str`` or ``None``
@@ -224,24 +228,28 @@
         'alpha'
         >>> tt.mhc.get_chain("HLA-DRB2")
         'beta'
         >>> tt.mhc.get_chain("B2M")
         'beta'
     """
     # Alias resolution
-    if gene is None:
+    if gene is None and not gene_name is None:
+        warn(
+            'The parameter "gene_name" will be deprecated in the near future. Please switch to using "gene".',
+            FutureWarning,
+        )
         gene = gene_name
 
     if type(gene) == str:
         # If we don't recognise the gene, return None with warning
         gene = gene.split("*")[0]
 
         if not gene in (*HOMOSAPIENS_MHC, "B2M"):
             if not suppress_warnings:
-                warn(f"Unrecognised gene {gene}. Is this standardised?")
+                warn(f"Unrecognised gene {gene}. Is this standardized?")
             return None
 
         if CHAIN_ALPHA_RE.match(gene):
             return "alpha"
 
         if CHAIN_BETA_RE.match(gene):
             return "beta"
@@ -255,33 +263,33 @@
 
 def get_class(
     gene: Optional[str] = None,
     suppress_warnings: bool = False,
     gene_name: Optional[str] = None,
 ) -> int:
     """
-    Given a standardised MHC gene name, detect whether it comprises a class I
+    Given a standardized MHC gene name, detect whether it comprises a class I
     or II MHC receptor complex.
 
     .. note::
 
         This function currently only recognises HLAs, and not MHCs from other species.
 
     :param gene:
-        Standardised MHC gene name
+        Standardized MHC gene name
     :type gene:
         ``str``
     :param suppress_warnings:
         Disable warnings that are usually emitted when classification fails.
         Defaults to ``False``.
     :type suppress_warnings:
         ``bool``
 
     :param gene_name:
-        Alias for the parameter ``gene``.
+        Alias for the parameter ``gene``. This will be deprecated soon.
     :type gene_name:
         ``str``
 
     :return:
         ``1`` or ``2`` if ``gene`` is recognised and its class is known, else ``None``.
     :rtype:
         ``int`` or ``None``
@@ -292,24 +300,28 @@
         1
         >>> tt.mhc.get_class("HLA-DRB2")
         2
         >>> tt.mhc.get_class("B2M")
         1
     """
     # Alias resolution
-    if gene is None:
+    if gene is None and not gene_name is None:
+        warn(
+            'The parameter "gene_name" will be deprecated in the near future. Please switch to using "gene".',
+            FutureWarning,
+        )
         gene = gene_name
 
     if type(gene) == str:
         # If we don't recognise the gene, return None with warning
         gene = gene.split("*")[0]
 
         if not gene in (*HOMOSAPIENS_MHC, "B2M"):
             if not suppress_warnings:
-                warn(f"Unrecognised gene {gene}. Is this standardised?")
+                warn(f"Unrecognised gene {gene}. Is this standardized?")
             return None
 
         if CLASS_1_RE.match(gene):
             return 1
 
         if CLASS_2_RE.match(gene):
             return 2
```

### Comparing `tidytcells-1.8.0/src/tidytcells/tcr/_main.py` & `tidytcells-1.8.1/src/tidytcells/tcr/_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,128 +1,132 @@
 """
 Utility functions related to TCRs and TCR genes.
 """
 
 
 from typing import Dict, FrozenSet, Optional
 from .._resources import HOMOSAPIENS_TCR_AA_SEQUENCES
-from .._utils.abstract_functions import standardise_template, query_template
+from .._utils.abstract_functions import standardize_template, query_template
 from .._utils.gene_query_engines import (
     HomoSapiensTCRQueryEngine,
     MusMusculusTCRQueryEngine,
 )
-from .._utils.gene_standardisers import (
-    HomoSapiensTCRStandardiser,
-    MusMusculusTCRStandardiser,
+from .._utils.gene_standardizers import (
+    HomoSapiensTCRStandardizer,
+    MusMusculusTCRStandardizer,
 )
 from .._utils.warnings import *
 
 
-STANDARDISERS = {
-    "homosapiens": HomoSapiensTCRStandardiser,
-    "musmusculus": MusMusculusTCRStandardiser,
+STANDARDIZERS = {
+    "homosapiens": HomoSapiensTCRStandardizer,
+    "musmusculus": MusMusculusTCRStandardizer,
 }
 
 QUERY_ENGINES = {
     "homosapiens": HomoSapiensTCRQueryEngine,
     "musmusculus": MusMusculusTCRQueryEngine,
 }
 
 
-def standardise(
+def standardize(
     gene: Optional[str] = None,
     species: str = "homosapiens",
     enforce_functional: bool = False,
     precision: str = "allele",
     suppress_warnings: bool = False,
     gene_name: Optional[str] = None,
 ) -> str:
     """
-    Attempt to standardise a TCR gene name to be IMGT-compliant.
+    Attempt to standardize a TCR gene name to be IMGT-compliant.
 
     .. topic:: Supported species
 
         - ``'homosapiens'``
         - ``'musmusculus'``
 
     :param gene:
-        Potentially non-standardised TCR gene name.
+        Potentially non-standardized TCR gene name.
     :type gene:
         ``str``
     :param species:
         Species to which the TCR gene belongs (see above for supported species).
         Defaults to ``'homosapiens'``.
     :type species:
         ``str``
     :param enforce_functional:
         If ``True``, disallows TCR genes that are recognised by IMGT but are marked as non-functional (ORF or pseudogene).
         Defaults to ``False``.
     :type enforce_functional:
         ``bool``
     :param precision:
-        The maximum level of precision to standardise to.
-        ``'allele'`` standardises to the maximum precision possible.
-        ``'gene'`` standardises only to the level of the gene.
+        The maximum level of precision to standardize to.
+        ``'allele'`` standardizes to the maximum precision possible.
+        ``'gene'`` standardizes only to the level of the gene.
         Defaults to ``'allele'``.
     :type precision:
         ``str``
     :param suppress_warnings:
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
         ``bool``
 
     :param gene_name:
-        Alias for the parameter ``gene``.
+        Alias for the parameter ``gene``. This will be deprecated soon.
     :type gene_name:
         ``str``
 
     :return:
-        If the specified ``species`` is supported, and ``gene`` could be standardised, then return the standardised gene name.
-        If ``species`` is unsupported, then the function does not attempt to standardise , and returns the unaltered ``gene`` string.
+        If the specified ``species`` is supported, and ``gene`` could be standardized, then return the standardized gene name.
+        If ``species`` is unsupported, then the function does not attempt to standardize , and returns the unaltered ``gene`` string.
         Else returns ``None``.
     :rtype:
         ``str`` or ``None``
 
     .. topic:: Example usage
 
         Input strings will intelligently be corrected to IMGT-compliant gene symbols.
 
-        >>> tt.tcr.standardise("aj1")
+        >>> tt.tcr.standardize("aj1")
         'TRAJ1'
 
         The ``precision`` setting can truncate unnecessary information.
 
-        >>> tt.tcr.standardise("TRBV6-4*01", precision="gene")
+        >>> tt.tcr.standardize("TRBV6-4*01", precision="gene")
         'TRBV6-4'
 
         The ``enforce_functional`` setting will cause non-functional genes or alleles to be rejected.
 
-        >>> result = tt.tcr.standardise("TRBV1", enforce_functional=True)
-        UserWarning: Failed to standardise: "TRBV1" for species homosapiens. Attempted fix "TRBV1" did not meet the standardised format requirements. Ignoring this gene name...
+        >>> result = tt.tcr.standardize("TRBV1", enforce_functional=True)
+        UserWarning: Failed to standardize "TRBV1" for species homosapiens: gene has no functional alleles. Attempted fix "TRBV1".
         >>> print(result)
         None
 
         *Mus musculus* is a supported species.
 
-        >>> tt.tcr.standardise("TCRBV22S1A2N1T", species="musmusculus")
+        >>> tt.tcr.standardize("TCRBV22S1A2N1T", species="musmusculus")
         'TRBV2'
     """
     # Alias resolution
-    if gene is None:
+    if gene is None and not gene_name is None:
+        warn(
+            'The parameter "gene_name" will be deprecated in the near future. Please switch to using "gene".',
+            FutureWarning,
+        )
         gene = gene_name
 
-    return standardise_template(
+    return standardize_template(
         gene=gene,
         gene_type="TCR",
         species=species,
         enforce_functional=enforce_functional,
         precision=precision,
         suppress_warnings=suppress_warnings,
-        standardiser_dict=STANDARDISERS,
+        standardizer_dict=STANDARDIZERS,
         allowed_precision={"allele", "gene"},
     )
 
 
 def query(
     species: str = "homosapiens",
     precision: str = "allele",
@@ -205,15 +209,15 @@
 
     .. note::
 
         This function currently only supports V genes.
         Support for J genes is planned for the future.
 
     :param gene:
-        Standardised gene name.
+        Standardized gene name.
         The gene must be specified to the level of the allele.
         Note that some genes, notably the non-functional ones, will not have resolvable amino acid sequences.
     :type gene:
         ``str``
     :param species:
         Species to which the TCR gene in question belongs (see above for supported species).
         Defaults to ``'homosapiens'``.
```

### Comparing `tidytcells-1.8.0/src/tidytcells.egg-info/PKG-INFO` & `tidytcells-1.8.1/src/tidytcells.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.0
+Version: 1.8.1
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.0/src/tidytcells.egg-info/SOURCES.txt` & `tidytcells-1.8.1/src/tidytcells.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 src/tidytcells/_resources/homosapiens_tcr_synonyms.json
 src/tidytcells/_resources/musmusculus_mhc.json
 src/tidytcells/_resources/musmusculus_mhc_synonyms.json
 src/tidytcells/_resources/musmusculus_tcr.json
 src/tidytcells/_utils/__init__.py
 src/tidytcells/_utils/abstract_functions.py
 src/tidytcells/_utils/gene_query_engines.py
-src/tidytcells/_utils/gene_standardisers.py
+src/tidytcells/_utils/gene_standardizers.py
 src/tidytcells/_utils/warnings.py
 src/tidytcells/aa/__init__.py
 src/tidytcells/aa/_main.py
 src/tidytcells/junction/__init__.py
 src/tidytcells/junction/_main.py
 src/tidytcells/mhc/__init__.py
 src/tidytcells/mhc/_main.py
```

### Comparing `tidytcells-1.8.0/tests/test_aa.py` & `tidytcells-1.8.1/tests/test_aa.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/tests/test_junction.py` & `tidytcells-1.8.1/tests/test_junction.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.0/tests/test_mhc.py` & `tidytcells-1.8.1/tests/test_mhc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,95 +1,96 @@
 import pytest
 from tidytcells import mhc
 from tidytcells._resources import *
 from typing import FrozenSet
 import warnings
 
 
-class TestStandardise:
+class TestStandardize:
     @pytest.mark.parametrize("species", ("foobar", "yoinkdoink", ""))
     def test_unsupported_species(self, species):
         with pytest.warns(UserWarning, match="Unsupported"):
-            result = mhc.standardise(gene="HLA-A*01:01:01:01", species=species)
+            result = mhc.standardize(gene="HLA-A*01:01:01:01", species=species)
 
         assert result == "HLA-A*01:01:01:01"
 
     @pytest.mark.parametrize("gene", (1234, None))
     def test_bad_type(self, gene):
         with pytest.raises(TypeError):
-            mhc.standardise(gene=gene)
+            mhc.standardize(gene=gene)
 
     def test_default_homosapiens(self):
-        result = mhc.standardise("HLA-B*07")
+        result = mhc.standardize("HLA-B*07")
 
         assert result == "HLA-B*07"
 
     @pytest.mark.parametrize(
         ("gene", "expected", "precision"),
         (
             ("HLA-DRB3*01:01:02:01", "HLA-DRB3*01:01:02:01", "allele"),
             ("HLA-DRB3*01:01:02:01", "HLA-DRB3*01:01", "protein"),
             ("HLA-DRB3*01:01:02:01", "HLA-DRB3", "gene"),
         ),
     )
     def test_precision(self, gene, expected, precision):
-        result = mhc.standardise(gene=gene, species="homosapiens", precision=precision)
+        result = mhc.standardize(gene=gene, species="homosapiens", precision=precision)
 
         assert result == expected
 
-    def test_standardize(self):
-        result = mhc.standardize("HLA-B*07")
+    def test_standardise(self):
+        result = mhc.standardise("HLA-B*07")
 
         assert result == "HLA-B*07"
 
     def test_gene_name(self):
-        result = mhc.standardise(gene_name="HLA-B*07")
+        with pytest.warns(FutureWarning):
+            result = mhc.standardize(gene_name="HLA-B*07")
 
         assert result == "HLA-B*07"
 
     def test_suppress_warnings(self):
         with warnings.catch_warnings():
             warnings.simplefilter("error")
-            mhc.standardise("foobarbaz", suppress_warnings=True)
+            mhc.standardize("foobarbaz", suppress_warnings=True)
 
 
-class TestStandardiseHomoSapiens:
+class TestStandardizeHomoSapiens:
     @pytest.mark.parametrize("gene", [*HOMOSAPIENS_MHC, "B2M"])
     def test_already_correctly_formatted(self, gene):
-        result = mhc.standardise(gene=gene, species="homosapiens")
+        result = mhc.standardize(gene=gene, species="homosapiens")
 
         assert result == gene
 
     @pytest.mark.parametrize(
         "gene", ("foobar", "yoinkdoink", "HLA-FOOBAR123456", "=======")
     )
     def test_invalid_mhc(self, gene):
-        with pytest.warns(UserWarning, match="Failed to standardise"):
-            result = mhc.standardise(gene=gene, species="homosapiens")
+        with pytest.warns(UserWarning, match="Failed to standardize"):
+            result = mhc.standardize(gene=gene, species="homosapiens")
 
         assert result == None
 
     @pytest.mark.parametrize("gene", ("HLA-A*01:01:1:1:1:1:1:1",))
     def test_bad_allele_designation(self, gene):
-        with pytest.warns(UserWarning, match="Failed to standardise"):
-            result = mhc.standardise(gene=gene, species="homosapiens")
+        with pytest.warns(UserWarning, match="Failed to standardize"):
+            result = mhc.standardize(gene=gene, species="homosapiens")
 
         assert result == None
 
     @pytest.mark.parametrize(
         ("gene", "expected"),
         (
             ("D6S204", "HLA-C"),
             ("HLA-DQA*01:01", "HLA-DQA1*01:01"),
             ("HLA-DQB*05:01", "HLA-DQB1*05:01"),
             ("HLA-DRA1*01:01", "HLA-DRA*01:01"),
         ),
     )
     def test_fix_deprecated_names(self, gene, expected):
-        result = mhc.standardise(gene=gene, species="homosapiens")
+        result = mhc.standardize(gene=gene, species="homosapiens")
 
         assert result == expected
 
     @pytest.mark.parametrize(
         "gene",
         (
             "HLA-A*01:01:01:01N",
@@ -97,15 +98,15 @@
             "HLA-A*01:01:01:01S",
             "HLA-A*01:01:01:01C",
             "HLA-A*01:01:01:01A",
             "HLA-A*01:01:01:01Q",
         ),
     )
     def test_remove_expression_qualifier(self, gene):
-        result = mhc.standardise(gene=gene, species="homosapiens")
+        result = mhc.standardize(gene=gene, species="homosapiens")
 
         assert result == "HLA-A*01:01:01:01"
 
     @pytest.mark.parametrize(
         ("gene", "expected"),
         (
             ("HLA-B8", "HLA-B*08"),
@@ -114,38 +115,38 @@
             ("HLA-B*5701", "HLA-B*57:01"),
             ("B35.3", "HLA-B*35:03"),
             ("HLA-DQB103:01", "HLA-DQB1*03:01"),
             ("HLA-A*01:01:1:1", "HLA-A*01:01:01:01"),
         ),
     )
     def test_various_typos(self, gene, expected):
-        result = mhc.standardise(gene=gene, species="homosapiens")
+        result = mhc.standardize(gene=gene, species="homosapiens")
 
         assert result == expected
 
 
-class TestStandardiseMusMusculus:
+class TestStandardizeMusMusculus:
     @pytest.mark.parametrize("gene", MUSMUSCULUS_MHC)
     def test_already_correctly_formatted(self, gene):
-        result = mhc.standardise(gene=gene, species="musmusculus")
+        result = mhc.standardize(gene=gene, species="musmusculus")
 
         assert result == gene
 
     @pytest.mark.parametrize("gene", ("foobar", "yoinkdoink", "MH1-ABC", "======="))
     def test_invalid_mhc(self, gene):
-        with pytest.warns(UserWarning, match="Failed to standardise"):
-            result = mhc.standardise(gene=gene, species="musmusculus")
+        with pytest.warns(UserWarning, match="Failed to standardize"):
+            result = mhc.standardize(gene=gene, species="musmusculus")
 
         assert result == None
 
     @pytest.mark.parametrize(
         ("gene", "expected"), (("H-2Eb1", "MH2-EB1"), ("H-2Aa", "MH2-AA"))
     )
     def test_fix_deprecated_names(self, gene, expected):
-        result = mhc.standardise(gene=gene, species="musmusculus")
+        result = mhc.standardize(gene=gene, species="musmusculus")
 
         assert result == expected
 
 
 class TestQuery:
     @pytest.mark.filterwarnings("ignore:tidytcells is not.+aware")
     @pytest.mark.parametrize(
@@ -224,15 +225,16 @@
 
     @pytest.mark.parametrize("gene", (1234, None))
     def test_bad_type(self, gene):
         with pytest.raises(TypeError):
             mhc.get_chain(gene)
 
     def test_gene_name(self):
-        result = mhc.get_chain(gene_name="HLA-A")
+        with pytest.warns(FutureWarning):
+            result = mhc.get_chain(gene_name="HLA-A")
 
         assert result == "alpha"
 
     def test_suppress_warnings(self):
         with warnings.catch_warnings():
             warnings.simplefilter("error")
             mhc.get_chain("foobarbaz", suppress_warnings=True)
@@ -271,20 +273,22 @@
 
     @pytest.mark.parametrize("gene", (1234, None))
     def test_bad_type(self, gene):
         with pytest.raises(TypeError):
             mhc.get_class(gene)
 
     def test_gene_name(self):
-        result = mhc.get_class(gene_name="HLA-A")
+        with pytest.warns(FutureWarning):
+            result = mhc.get_class(gene_name="HLA-A")
 
         assert result == 1
 
     def test_suppress_warnings(self):
         with warnings.catch_warnings():
             warnings.simplefilter("error")
             mhc.get_class("foobarbaz", suppress_warnings=True)
 
     def test_classify(self):
-        result = mhc.classify(gene="HLA-A")
+        with pytest.warns(FutureWarning):
+            result = mhc.classify(gene="HLA-A")
 
         assert result == 1
```

### Comparing `tidytcells-1.8.0/tests/test_tcr.py` & `tidytcells-1.8.1/tests/test_tcr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,111 +1,112 @@
 import pytest
 from tidytcells import tcr
 from tidytcells._resources import HOMOSAPIENS_TCR, MUSMUSCULUS_TCR
 import warnings
 
 
-class TestStandardise:
+class TestStandardize:
     @pytest.mark.parametrize("species", ("foobar", "yoinkdoink", ""))
     def test_unsupported_species(self, species):
         with pytest.warns(UserWarning, match="Unsupported"):
-            result = tcr.standardise(gene="foobarbaz", species=species)
+            result = tcr.standardize(gene="foobarbaz", species=species)
 
         assert result == "foobarbaz"
 
     @pytest.mark.parametrize("gene", (1234, None))
     def test_bad_type(self, gene):
         with pytest.raises(TypeError):
-            tcr.standardise(gene=gene)
+            tcr.standardize(gene=gene)
 
     def test_default_homosapiens(self):
-        result = tcr.standardise("TRBV20/OR9-2*01")
+        result = tcr.standardize("TRBV20/OR9-2*01")
 
         assert result == "TRBV20/OR9-2*01"
 
     @pytest.mark.parametrize(
         ("gene", "expected"),
         (("TRAV3*01&nbsp;", "TRAV3*01"), (" TRAV3 * 01 ", "TRAV3*01")),
     )
     def test_remove_pollutants(self, gene, expected):
-        result = tcr.standardise(gene=gene, species="homosapiens")
+        result = tcr.standardize(gene=gene, species="homosapiens")
 
         assert result == expected
 
-    @pytest.mark.filterwarnings("ignore:Failed to standardise")
+    @pytest.mark.filterwarnings("ignore:Failed to standardize")
     @pytest.mark.parametrize(
         ("gene", "expected", "enforce_functional"),
         (
             ("TRAV35*01", "TRAV35*01", True),
             ("TRAV35*03", None, True),
             ("TRAV35*03", "TRAV35*03", False),
             ("TRAV35", "TRAV35", True),
             ("TRAV8-7", None, True),
             ("TRAV8-7", "TRAV8-7", False),
         ),
     )
     def test_enforce_functional(self, gene, expected, enforce_functional):
-        result = tcr.standardise(
+        result = tcr.standardize(
             gene=gene, species="homosapiens", enforce_functional=enforce_functional
         )
 
         assert result == expected
 
     @pytest.mark.parametrize(
         ("gene", "expected", "precision"),
         (
             ("TRBV24/OR9-2*01", "TRBV24/OR9-2*01", "allele"),
             ("TRAV16*01", "TRAV16", "gene"),
         ),
     )
     def test_precision(self, gene, expected, precision):
-        result = tcr.standardise(gene=gene, species="homosapiens", precision=precision)
+        result = tcr.standardize(gene=gene, species="homosapiens", precision=precision)
 
         assert result == expected
 
-    def test_standardize(self):
-        result = tcr.standardize("TRBV20/OR9-2*01")
+    def test_standardise(self):
+        result = tcr.standardise("TRBV20/OR9-2*01")
 
         assert result == "TRBV20/OR9-2*01"
 
     def test_gene_name(self):
-        result = tcr.standardise(gene_name="TRBV20/OR9-2*01")
+        with pytest.warns(FutureWarning):
+            result = tcr.standardize(gene_name="TRBV20/OR9-2*01")
 
         assert result == "TRBV20/OR9-2*01"
 
     def test_suppress_warnings(self):
         with warnings.catch_warnings():
             warnings.simplefilter("error")
-            tcr.standardise("foobarbaz", suppress_warnings=True)
+            tcr.standardize("foobarbaz", suppress_warnings=True)
 
 
-class TestStandardiseHomoSapiens:
+class TestStandardizeHomoSapiens:
     @pytest.mark.parametrize("gene", HOMOSAPIENS_TCR)
     def test_already_correctly_formatted(self, gene):
-        result = tcr.standardise(gene=gene, species="homosapiens")
+        result = tcr.standardize(gene=gene, species="homosapiens")
 
         assert result == gene
 
     @pytest.mark.parametrize("gene", ("foobar", "TRAV3D-3*01"))
     def test_invalid_tcr(self, gene):
-        with pytest.warns(UserWarning, match="Failed to standardise"):
-            result = tcr.standardise(gene=gene, species="homosapiens")
+        with pytest.warns(UserWarning, match="Failed to standardize"):
+            result = tcr.standardize(gene=gene, species="homosapiens")
 
         assert result == None
 
     @pytest.mark.parametrize(
         ("gene", "expected"),
         (
             ("TCRAV32S1", "TRAV25"),
             ("TCRAV14S2", "TRAV38-1"),
             ("TCRBV21S1*01", "TRBV11-1*01"),
         ),
     )
     def test_resolve_alternate_tcr_names(self, gene, expected):
-        result = tcr.standardise(gene=gene, species="homosapiens")
+        result = tcr.standardize(gene=gene, species="homosapiens")
 
         assert result == expected
 
     @pytest.mark.parametrize(
         ("gene", "expected"),
         (
             ("TRAV14DV4", "TRAV14/DV4"),
@@ -113,30 +114,30 @@
             ("TRBV01", "TRBV1"),
             ("TCRBV1", "TRBV1"),
             ("TRAV14", "TRAV14/DV4"),
             ("TRDV4", "TRAV14/DV4"),
         ),
     )
     def test_various_typos(self, gene, expected):
-        result = tcr.standardise(gene=gene, species="homosapiens")
+        result = tcr.standardize(gene=gene, species="homosapiens")
 
         assert result == expected
 
 
-class TestStandardiseMusMusculus:
+class TestStandardizeMusMusculus:
     @pytest.mark.parametrize("gene", MUSMUSCULUS_TCR)
     def test_already_correctly_formatted(self, gene):
-        result = tcr.standardise(gene=gene, species="musmusculus")
+        result = tcr.standardize(gene=gene, species="musmusculus")
 
         assert result == gene
 
     @pytest.mark.parametrize("gene", ("foobar", "TRAV3*01"))
     def test_inivalid_tcr(self, gene):
-        with pytest.warns(UserWarning, match="Failed to standardise"):
-            result = tcr.standardise(gene=gene, species="musmusculus")
+        with pytest.warns(UserWarning, match="Failed to standardize"):
+            result = tcr.standardize(gene=gene, species="musmusculus")
 
         assert result == None
 
 
 class TestQuery:
     @pytest.mark.parametrize(
         ("species", "precision", "expected_len", "expected_in", "expected_not_in"),
```

