# Comparing `tmp/seagal-2.3.tar.gz` & `tmp/seagal-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagal-2.3.tar", last modified: Fri Jun  2 16:13:08 2023, max compression
+gzip compressed data, was "seagal-2.4.tar", last modified: Fri Jun  2 16:17:08 2023, max compression
```

## Comparing `seagal-2.3.tar` & `seagal-2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:13:08.534849 seagal-2.3/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     1068 2023-02-11 05:25:59.000000 seagal-2.3/LICENSE
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-06-02 16:13:08.534849 seagal-2.3/PKG-INFO
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3231 2023-02-11 05:37:25.000000 seagal-2.3/README.md
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:13:08.526849 seagal-2.3/seagal/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.3/seagal/__init__.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3089 2023-02-11 05:26:14.000000 seagal-2.3/seagal/_gmod.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     4508 2023-06-02 15:57:57.000000 seagal-2.3/seagal/_plotting.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)    14996 2023-06-02 16:03:58.000000 seagal-2.3/seagal/_utils.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)    11622 2023-06-02 15:57:57.000000 seagal-2.3/seagal/lee_vec.py
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:13:08.530849 seagal-2.3/seagal/modules/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.3/seagal/modules/__init__.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3113 2023-02-11 05:26:14.000000 seagal-2.3/seagal/modules/gmod.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)      978 2023-02-11 05:26:14.000000 seagal-2.3/seagal/seagal.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     7473 2023-06-02 15:57:57.000000 seagal-2.3/seagal/spatial_measure.py
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:13:08.530849 seagal-2.3/seagal.egg-info/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/PKG-INFO
--rw-rw-r--   0 linhua    (1008) linhua    (1010)      387 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/SOURCES.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/dependency_links.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-02-11 05:26:14.000000 seagal-2.3/seagal.egg-info/not-zip-safe
--rw-rw-r--   0 linhua    (1008) linhua    (1010)       98 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/requires.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        7 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/top_level.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)       38 2023-06-02 16:13:08.534849 seagal-2.3/setup.cfg
--rw-rw-r--   0 linhua    (1008) linhua    (1010)      824 2023-06-02 16:11:56.000000 seagal-2.3/setup.py
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:17:08.896855 seagal-2.4/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     1068 2023-02-11 05:25:59.000000 seagal-2.4/LICENSE
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-06-02 16:17:08.892856 seagal-2.4/PKG-INFO
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3231 2023-02-11 05:37:25.000000 seagal-2.4/README.md
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:17:08.892856 seagal-2.4/seagal/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.4/seagal/__init__.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3089 2023-02-11 05:26:14.000000 seagal-2.4/seagal/_gmod.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     4508 2023-06-02 15:57:57.000000 seagal-2.4/seagal/_plotting.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)    15041 2023-06-02 16:16:42.000000 seagal-2.4/seagal/_utils.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)    11622 2023-06-02 15:57:57.000000 seagal-2.4/seagal/lee_vec.py
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:17:08.892856 seagal-2.4/seagal/modules/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.4/seagal/modules/__init__.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3113 2023-02-11 05:26:14.000000 seagal-2.4/seagal/modules/gmod.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)      978 2023-02-11 05:26:14.000000 seagal-2.4/seagal/seagal.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     7473 2023-06-02 15:57:57.000000 seagal-2.4/seagal/spatial_measure.py
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:17:08.892856 seagal-2.4/seagal.egg-info/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-06-02 16:17:08.000000 seagal-2.4/seagal.egg-info/PKG-INFO
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)      387 2023-06-02 16:17:08.000000 seagal-2.4/seagal.egg-info/SOURCES.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-06-02 16:17:08.000000 seagal-2.4/seagal.egg-info/dependency_links.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-02-11 05:26:14.000000 seagal-2.4/seagal.egg-info/not-zip-safe
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)       98 2023-06-02 16:17:08.000000 seagal-2.4/seagal.egg-info/requires.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        7 2023-06-02 16:17:08.000000 seagal-2.4/seagal.egg-info/top_level.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)       38 2023-06-02 16:17:08.896855 seagal-2.4/setup.cfg
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)      824 2023-06-02 16:16:47.000000 seagal-2.4/setup.py
```

### Comparing `seagal-2.3/LICENSE` & `seagal-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seagal-2.3/PKG-INFO` & `seagal-2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagal
-Version: 2.3
+Version: 2.4
 Summary: Spatial Enrichment Analysis of Gene Association using L-index
 Home-page: https://github.com/linhuawang/SEAGAL
 Author: Linhua Wang
 Author-email: linhuaw@bcm.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seagal-2.3/README.md` & `seagal-2.4/README.md`

 * *Files identical despite different names*

### Comparing `seagal-2.3/seagal/_gmod.py` & `seagal-2.4/seagal/_gmod.py`

 * *Files identical despite different names*

### Comparing `seagal-2.3/seagal/_plotting.py` & `seagal-2.4/seagal/_plotting.py`

 * *Files identical despite different names*

### Comparing `seagal-2.3/seagal/_utils.py` & `seagal-2.4/seagal/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     df["Association"] = "NS"
     df.loc[(df['L.FDR'] <= FDR_cutoff) & (df['L'] >= L_cutoff), "Association"] = "SigPos"
     df.loc[(df['L.FDR'] <= FDR_cutoff) & (df['L'] <= -L_cutoff), "Association"] = "SigNeg"
     self.co_expression = df
 
 def group_adata_by_genes(self, ct_dict = None, inplace=True, reference='hpca'):
     ## Overwrite self.co_expression_grouped object if existed.
-    MARKER_KNOWLEDGBASE = {'hpca':{'B cells': ['POU2AF1', 'MS4A1', 'JCHAIN', 'VPREB3', 'IGLL3P', 'IGHM',
+    MARKER_KNOWLEDGBASE = {'hpca': {'B cells': ['POU2AF1', 'MS4A1', 'JCHAIN', 'VPREB3', 'IGLL3P', 'IGHM',
                                          'TCL1A', 'STAP1', 'BLNK', 'TNFRSF17', 'CD19', 'CR2', 'CD79A', 
                                          'HLA-DOB', 'IGKC', 'FCRLA', 'P2RX5', 'GUSBP11', 'CD79B', 'RGS13'],
                          'Endothelial cells': ['GJA1', 'CTGF', 'EFEMP1', 'PLS3', 'CAV1', 'CDH5', 'ESM1',
                                          'ARHGAP29', 'ADGRL4', 'FSTL1', 'MMP1', 'SRPX', 'CYR61', 'CAV2', 'LAMB1',
                                           'TM4SF1', 'MMRN1', 'NNMT', 'HHIP', 'GNG11'], 
                         'Macrophages': ['GPNMB', 'MRC1', 'CHI3L1', 'SPP1', 'PLA2G7', 'APOC1', 
                                         'LPL', 'APOE', 'ADAMDEC1', 'CCL18', 'C1QA', 'C15orf48',
@@ -167,15 +167,16 @@
                                          'CD14', 'S100A9', 'LILRB2', 'RGS18', 'TYROBP', 'MNDA', 'CPVL',
                                           'APOBEC3A', 'HCK', 'CFP', 'NCF2', 'FCER1G'],
                         'Neutrophils': ['PI3', 'CXCR2', 'FCGR3B', 'STEAP4', 'PROK2', 'MGAM', 'IL1R2',
                                         'TNFAIP6', 'S100P', 'S100A12', 'CLC', 'KCNJ15', 'G0S2', 'KRT23',
                                          'PTGS2', 'P2RY14', 'CXCL1', 'TREM1', 'FFAR2', 'OSM'], 
                         'T cells': ['ITK', 'CD3D', 'TRBC1', 'TRAT1', 'TRAC', 'CD3G', 'CD2',
                                          'LCK', 'NELL2', 'NLRC3', 'GPR171', 'THEMIS', 'CD69',
-                                          'KLRB1', 'RASGRP1', 'BCL11B', 'GZMK', 'GZMA', 'TC2N', 'ITM2A']}
+                                          'KLRB1', 'RASGRP1', 'BCL11B', 'GZMK', 'GZMA', 'TC2N', 'ITM2A']},
+                                          
                 'mouse_immune': {'B cells': ['IGKC', 'EBF1', 'BANK1', 'CD79A', 'IGHD',
                                 'BACH2', 'IGHM', 'FCHSD2', 'LY6D', 'PAX5', 
                                 'RALGPS2', 'IGLC2', 'AFF3', 'MAN1A', 'BTLA',
                                   'MEF2C', 'CD79B', 'MS4A1', 'FOXP1', 'CD55'],
                     'Endothelial': ['WFDC18', 'CSN3', 'LCN2', 'PHLDA1','KRT18',
                                     'MAP1LC3A', 'HRAS', 'AQP5', 'KRT8', 'CRIP2',
                                     'CDKN1A', 'DBI', 'PGP', 'RPS27L', '1110008P14RIK',
```

### Comparing `seagal-2.3/seagal/lee_vec.py` & `seagal-2.4/seagal/lee_vec.py`

 * *Files identical despite different names*

### Comparing `seagal-2.3/seagal/modules/gmod.py` & `seagal-2.4/seagal/modules/gmod.py`

 * *Files identical despite different names*

### Comparing `seagal-2.3/seagal/seagal.py` & `seagal-2.4/seagal/seagal.py`

 * *Files identical despite different names*

### Comparing `seagal-2.3/seagal/spatial_measure.py` & `seagal-2.4/seagal/spatial_measure.py`

 * *Files identical despite different names*

### Comparing `seagal-2.3/seagal.egg-info/PKG-INFO` & `seagal-2.4/seagal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagal
-Version: 2.3
+Version: 2.4
 Summary: Spatial Enrichment Analysis of Gene Association using L-index
 Home-page: https://github.com/linhuawang/SEAGAL
 Author: Linhua Wang
 Author-email: linhuaw@bcm.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seagal-2.3/setup.py` & `seagal-2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='seagal',
-    version='2.3',
+    version='2.4',
     description='Spatial Enrichment Analysis of Gene Association using L-index',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/linhuawang/SEAGAL',
     author='Linhua Wang',
     author_email='linhuaw@bcm.edu',
     license='MIT',
```

