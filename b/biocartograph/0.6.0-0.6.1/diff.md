# Comparing `tmp/biocartograph-0.6.0.tar.gz` & `tmp/biocartograph-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocartograph-0.6.0.tar", last modified: Thu Jun  1 15:38:04 2023, max compression
+gzip compressed data, was "biocartograph-0.6.1.tar", last modified: Fri Jun  2 09:32:44 2023, max compression
```

## Comparing `biocartograph-0.6.0.tar` & `biocartograph-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-01 15:38:04.872826 biocartograph-0.6.0/
--rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-06-01 15:35:36.000000 biocartograph-0.6.0/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-01 15:38:04.872826 biocartograph-0.6.0/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-06-01 15:35:36.000000 biocartograph-0.6.0/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-01 15:38:04.872826 biocartograph-0.6.0/biocartograph.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-01 15:38:04.000000 biocartograph-0.6.0/biocartograph.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)      334 2023-06-01 15:38:04.000000 biocartograph-0.6.0/biocartograph.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-06-01 15:38:04.000000 biocartograph-0.6.0/biocartograph.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-06-01 15:38:04.000000 biocartograph-0.6.0/biocartograph.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-06-01 15:38:04.872826 biocartograph-0.6.0/setup.cfg
--rw-r--r--   0 rictjo    (1000) users      (100)      955 2023-06-01 15:35:36.000000 biocartograph-0.6.0/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-01 15:38:04.871826 biocartograph-0.6.0/src/
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-01 15:38:04.872826 biocartograph-0.6.0/src/biocartograph/
--rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/__init__.py
--rw-r--r--   0 rictjo    (1000) users      (100)     3334 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/composition.py
--rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/enrichment.py
--rw-r--r--   0 rictjo    (1000) users      (100)    22401 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (100)    26154 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/special.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-02 09:32:44.406843 biocartograph-0.6.1/
+-rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-06-01 15:35:36.000000 biocartograph-0.6.1/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-02 09:32:44.406843 biocartograph-0.6.1/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-06-01 15:35:36.000000 biocartograph-0.6.1/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-02 09:32:44.405843 biocartograph-0.6.1/biocartograph.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-02 09:32:44.000000 biocartograph-0.6.1/biocartograph.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)      334 2023-06-02 09:32:44.000000 biocartograph-0.6.1/biocartograph.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-06-02 09:32:44.000000 biocartograph-0.6.1/biocartograph.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-06-02 09:32:44.000000 biocartograph-0.6.1/biocartograph.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-06-02 09:32:44.406843 biocartograph-0.6.1/setup.cfg
+-rw-r--r--   0 rictjo    (1000) users      (100)      955 2023-06-02 09:32:03.000000 biocartograph-0.6.1/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-02 09:32:44.405843 biocartograph-0.6.1/src/
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-02 09:32:44.406843 biocartograph-0.6.1/src/biocartograph/
+-rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-06-01 15:35:36.000000 biocartograph-0.6.1/src/biocartograph/__init__.py
+-rw-r--r--   0 rictjo    (1000) users      (100)     3334 2023-06-01 15:35:36.000000 biocartograph-0.6.1/src/biocartograph/composition.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    16747 2023-06-02 09:32:03.000000 biocartograph-0.6.1/src/biocartograph/enrichment.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    22401 2023-06-01 15:35:36.000000 biocartograph-0.6.1/src/biocartograph/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    26154 2023-06-01 15:35:36.000000 biocartograph-0.6.1/src/biocartograph/special.py
```

### Comparing `biocartograph-0.6.0/LICENSE` & `biocartograph-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.0/PKG-INFO` & `biocartograph-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.6.0
+Version: 0.6.1
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.6.0/README.md` & `biocartograph-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.0/biocartograph.egg-info/PKG-INFO` & `biocartograph-0.6.1/biocartograph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.6.0
+Version: 0.6.1
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.6.0/setup.py` & `biocartograph-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name         = "biocartograph",
-    version      = "0.6.0",
+    version      = "0.6.1",
     author       = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description  = "Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/rictjo/biocarta",
     packages = setuptools.find_packages('src'),
```

### Comparing `biocartograph-0.6.0/src/biocartograph/composition.py` & `biocartograph-0.6.1/src/biocartograph/composition.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.0/src/biocartograph/enrichment.py` & `biocartograph-0.6.1/src/biocartograph/enrichment.py`

 * *Files 12% similar despite different names*

```diff
@@ -147,14 +147,56 @@
     )
     fig.update_traces(root_color="lightgrey")
     fig.update_layout(margin = dict(t=50, l=25, r=25, b=25))
     fig.show()
     """
     return ( dag_maps )
 
+import pandas as pd
+import numpy  as np
+
+from biocartograph.composition import composition_leading_label_and_metric
+
+def auto_annotate_clusters (	header_str:str = '../results/DMHMSY_Fri_Jun__2_09_15_35_2023_'	,
+				alignment_information:str       	= "pcas_df.tsv"		,
+				cluster_information:str         	= "resdf_f.tsv"		,
+				final_cluster_label:str         	= "cids.max"		,
+				enrichment_results_file_pattern:str 	= "(HEADER)treemap_c(CLUSTID).tsv" ) -> pd.DataFrame :
+    #
+    df_pca =        pd.read_csv( header_str + alignment_information , sep='\t', index_col=0 )
+    df_clu =        pd.read_csv( header_str + cluster_information   , sep='\t', index_col=0 )
+    #
+    merged_info = pd.concat ( [	df_clu .loc[:,[final_cluster_label]].T	,
+				df_pca .loc[:,[ c for c in df_pca.columns if 'Owner' in c ]].T,
+			 ]).T.rename( columns = { final_cluster_label:'cluster' } )
+    merged_info.columns	= [ v.replace('Owner','PCA.owner') for v in  merged_info.columns.values ]
+    consolidate		= [ c for c in merged_info.columns if 'owner' in c ]
+    #
+    from collections import Counter
+    # AUTO ANNOTATIONS
+    if len( consolidate ) > 1 :
+        auto_annotated_df = merged_info.groupby('cluster').apply(lambda x: pd.Series( [ len(x) ,
+		*[ v for v in composition_leading_label_and_metric(Counter(x.loc[ :, consolidate[0] ].values)).values() ]   ,
+		*[ v for v in composition_leading_label_and_metric(Counter(x.loc[ :, consolidate[1] ].values)).values() ] ] ,
+			index = [ 'N' , 'Reliability-Spec,Tau' , 'Specificity' ,
+					'Reliability-Aux,Tau'  , 'Auxiliary Annotation' ] ) )
+    else :
+        auto_annotated_df = merged_info.groupby('cluster').apply(lambda x: pd.Series( [ len(x) ,
+                *[ v for v in composition_leading_label_and_metric(Counter(x.loc[ :, consolidate[0] ].values)).values() ] ] ,
+                        index = [ 'N' , 'Reliability-Spec,Tau' , 'Specificity' ] ) )
+    #
+    # ADD IN TOP ENRICHMENT
+    function = []
+    for cid in auto_annotated_df .index.values.tolist() :
+        filename	= enrichment_results_file_pattern.replace('(HEADER)',header_str).replace('(CLUSTID)',str(cid))
+        df		= pd.read_csv(filename,sep='\t',index_col=0)
+        function .append( df.iloc[ np.argmin( df.loc[:,'p-value'].values ) , : ].loc['description'] )
+    auto_annotated_df.loc[:,'Function'] = function
+    return ( auto_annotated_df )
+
 
 def benchmark_group_expression_with_univariate_foldchange ( group_df:pd.DataFrame , journal_df:pd.DataFrame ,
                         major_group_label:str = None , what_thing:str = None , bRanked:bool=False ,
 			nsamples:int = None, bVerbose:bool = False , bgname:str = 'Background' ,
 			clean_label = lambda x : x.replace(' ','_').replace('/','Or').replace('\\','').replace('-','') ) -> pd.DataFrame :
 
     from biocartograph.special import calculate_volcano_df
```

### Comparing `biocartograph-0.6.0/src/biocartograph/quantification.py` & `biocartograph-0.6.1/src/biocartograph/quantification.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.6.0/src/biocartograph/special.py` & `biocartograph-0.6.1/src/biocartograph/special.py`

 * *Files identical despite different names*

