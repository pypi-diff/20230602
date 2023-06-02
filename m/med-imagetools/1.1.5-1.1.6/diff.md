# Comparing `tmp/med-imagetools-1.1.5.tar.gz` & `tmp/med-imagetools-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "med-imagetools-1.1.5.tar", last modified: Tue May  9 19:17:04 2023, max compression
+gzip compressed data, was "med-imagetools-1.1.6.tar", last modified: Fri Jun  2 19:06:27 2023, max compression
```

## Comparing `med-imagetools-1.1.5.tar` & `med-imagetools-1.1.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.709253 med-imagetools-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-09 19:17:04.705253 med-imagetools-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.693253 med-imagetools-1.1.5/imgtools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41500 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/autopipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.693253 med-imagetools-1.1.5/imgtools/io/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.697253 med-imagetools-1.1.5/imgtools/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28509 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/datagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/dose.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/pet.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/sparsemask.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/structureset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.697253 med-imagetools-1.1.5/imgtools/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22695 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/ops/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    63999 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/ops/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.701253 med-imagetools-1.1.5/imgtools/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/transforms/intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/transforms/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.705253 med-imagetools-1.1.5/imgtools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/arrayutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/autopipeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/dicomutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/nnunet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.705253 med-imagetools-1.1.5/med_imagetools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:17:04.709253 med-imagetools-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:06:27.277792 med-imagetools-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-02 19:06:27.277792 med-imagetools-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:06:27.273792 med-imagetools-1.1.6/imgtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41500 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/autopipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:06:27.273792 med-imagetools-1.1.6/imgtools/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/io/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/io/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/io/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:06:27.277792 med-imagetools-1.1.6/imgtools/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28548 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/modules/datagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/modules/dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/modules/pet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/modules/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/modules/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/modules/sparsemask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/modules/structureset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:06:27.277792 med-imagetools-1.1.6/imgtools/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22695 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/ops/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63999 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/ops/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:06:27.277792 med-imagetools-1.1.6/imgtools/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/transforms/intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/transforms/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:06:27.277792 med-imagetools-1.1.6/imgtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/utils/arrayutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/utils/autopipeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/utils/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/utils/dicomutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/utils/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/imgtools/utils/nnunet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:06:27.277792 med-imagetools-1.1.6/med_imagetools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-02 19:06:27.000000 med-imagetools-1.1.6/med_imagetools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 19:06:27.000000 med-imagetools-1.1.6/med_imagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:06:27.000000 med-imagetools-1.1.6/med_imagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 19:06:27.000000 med-imagetools-1.1.6/med_imagetools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-02 19:06:27.000000 med-imagetools-1.1.6/med_imagetools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 19:06:27.000000 med-imagetools-1.1.6/med_imagetools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 19:06:27.277792 med-imagetools-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-02 19:04:00.000000 med-imagetools-1.1.6/setup.py
```

### Comparing `med-imagetools-1.1.5/LICENSE` & `med-imagetools-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/PKG-INFO` & `med-imagetools-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: med-imagetools
-Version: 1.1.5
+Version: 1.1.6
 Summary: Transparent and reproducible image processing pipelines in Python.
 Home-page: https://github.com/bhklab/med-imagetools
 Author: Sejin Kim, Michal Kazmierski, Kevin Qu, Vishwesh Ramanathan, Benjamin Haibe-Kains
 Author-email: benjamin.haibe.kains@utoronto.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `med-imagetools-1.1.5/README.md` & `med-imagetools-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/autopipeline.py` & `med-imagetools-1.1.6/imgtools/autopipeline.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/image.py` & `med-imagetools-1.1.6/imgtools/image.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/io/common.py` & `med-imagetools-1.1.6/imgtools/io/common.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/io/dataset.py` & `med-imagetools-1.1.6/imgtools/io/dataset.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/io/loaders.py` & `med-imagetools-1.1.6/imgtools/io/loaders.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/io/writers.py` & `med-imagetools-1.1.6/imgtools/io/writers.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/modules/datagraph.py` & `med-imagetools-1.1.6/imgtools/modules/datagraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         Forms edge table based on the crawled data
         '''
         # enforce string type to all columns to prevent dtype merge errors for empty columns
         for col in self.df:
             self.df[col] = self.df[col].astype(str)
         
         #Get reference_rs information from RTDOSE-RTPLAN connections    
-        df_filter = pd.merge(self.df, self.df[["instance_uid","reference_rs"]], 
+        df_filter = pd.merge(self.df, self.df[["instance_uid","reference_rs"]].apply(lambda x: x.astype(str), axis=1), 
                              left_on="reference_pl", 
                              right_on="instance_uid", 
                              how="left")
         
         df_filter.loc[(df_filter.reference_rs_x.isna()) & (~df_filter.reference_rs_y.isna()),"reference_rs_x"] = df_filter.loc[(df_filter.reference_rs_x.isna()) & (~df_filter.reference_rs_y.isna()),"reference_rs_y"].values
         df_filter.drop(columns=["reference_rs_y", "instance_uid_y"], inplace=True)
         df_filter.rename(columns={"reference_rs_x":"reference_rs", "instance_uid_x":"instance_uid"}, inplace=True)
```

### Comparing `med-imagetools-1.1.5/imgtools/modules/dose.py` & `med-imagetools-1.1.6/imgtools/modules/dose.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/modules/pet.py` & `med-imagetools-1.1.6/imgtools/modules/pet.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/modules/segmentation.py` & `med-imagetools-1.1.6/imgtools/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/modules/structureset.py` & `med-imagetools-1.1.6/imgtools/modules/structureset.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/ops/functional.py` & `med-imagetools-1.1.6/imgtools/ops/functional.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/ops/ops.py` & `med-imagetools-1.1.6/imgtools/ops/ops.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/pipeline.py` & `med-imagetools-1.1.6/imgtools/pipeline.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/transforms/spatial.py` & `med-imagetools-1.1.6/imgtools/transforms/spatial.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/utils/args.py` & `med-imagetools-1.1.6/imgtools/utils/args.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/utils/arrayutils.py` & `med-imagetools-1.1.6/imgtools/utils/arrayutils.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/utils/autopipeutils.py` & `med-imagetools-1.1.6/imgtools/utils/autopipeutils.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/utils/crawl.py` & `med-imagetools-1.1.6/imgtools/utils/crawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             try:
                 dcm_path  = pathlib.Path(dcm)
                 # parent    = dcm_path.parent#.as_posix()
                 fname     = dcm_path.name
                 rel_path  = dcm_path.relative_to(folder_path.parent.parent)                                        # rel_path of dicom from folder
                 rel_posix = rel_path.parent.as_posix()     # folder name + until parent folder of dicom
 
-                meta      = dcmread(dcm, force=True)
+                meta      = dcmread(dcm, force=True, stop_before_pixels=True)
                 patient   = str(meta.PatientID)
                 study     = str(meta.StudyInstanceUID)
                 series    = str(meta.SeriesInstanceUID)
                 instance  = str(meta.SOPInstanceUID)
 
                 reference_ct, reference_rs, reference_pl,  = "", "", ""
                 tr, te, tesla, scan_seq, elem = "", "", "", "", ""
```

### Comparing `med-imagetools-1.1.5/imgtools/utils/dicomutils.py` & `med-imagetools-1.1.6/imgtools/utils/dicomutils.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/utils/imageutils.py` & `med-imagetools-1.1.6/imgtools/utils/imageutils.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/imgtools/utils/nnunet.py` & `med-imagetools-1.1.6/imgtools/utils/nnunet.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/med_imagetools.egg-info/PKG-INFO` & `med-imagetools-1.1.6/med_imagetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: med-imagetools
-Version: 1.1.5
+Version: 1.1.6
 Summary: Transparent and reproducible image processing pipelines in Python.
 Home-page: https://github.com/bhklab/med-imagetools
 Author: Sejin Kim, Michal Kazmierski, Kevin Qu, Vishwesh Ramanathan, Benjamin Haibe-Kains
 Author-email: benjamin.haibe.kains@utoronto.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `med-imagetools-1.1.5/med_imagetools.egg-info/SOURCES.txt` & `med-imagetools-1.1.6/med_imagetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.5/setup.py` & `med-imagetools-1.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     reqs = fh.read()
     
 setup(
     name="med-imagetools",
-    version="1.1.5",
+    version="1.1.6",
     author="Sejin Kim, Michal Kazmierski, Kevin Qu, Vishwesh Ramanathan, Benjamin Haibe-Kains",
     author_email="benjamin.haibe.kains@utoronto.ca",
     description="Transparent and reproducible image processing pipelines in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bhklab/med-imagetools",
     install_requires=reqs,
```

