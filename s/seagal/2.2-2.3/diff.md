# Comparing `tmp/seagal-2.2.tar.gz` & `tmp/seagal-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagal-2.2.tar", last modified: Fri Apr 14 14:13:57 2023, max compression
+gzip compressed data, was "seagal-2.3.tar", last modified: Fri Jun  2 16:13:08 2023, max compression
```

## Comparing `seagal-2.2.tar` & `seagal-2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-14 14:13:57.214665 seagal-2.2/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     1068 2023-02-11 05:25:59.000000 seagal-2.2/LICENSE
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-04-14 14:13:57.214665 seagal-2.2/PKG-INFO
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3231 2023-02-11 05:37:25.000000 seagal-2.2/README.md
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-14 14:13:57.214665 seagal-2.2/seagal/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.2/seagal/__init__.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3089 2023-02-11 05:26:14.000000 seagal-2.2/seagal/_gmod.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     4228 2023-04-05 19:57:00.000000 seagal-2.2/seagal/_plotting.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)    15595 2023-04-10 19:15:59.000000 seagal-2.2/seagal/_utils.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)    11553 2023-02-11 05:26:14.000000 seagal-2.2/seagal/lee_vec.py
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-14 14:13:57.214665 seagal-2.2/seagal/modules/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.2/seagal/modules/__init__.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3113 2023-02-11 05:26:14.000000 seagal-2.2/seagal/modules/gmod.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)      978 2023-02-11 05:26:14.000000 seagal-2.2/seagal/seagal.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     6633 2023-04-10 19:11:32.000000 seagal-2.2/seagal/spatial_measure.py
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-14 14:13:57.214665 seagal-2.2/seagal.egg-info/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/PKG-INFO
--rw-rw-r--   0 linhua    (1008) linhua    (1010)      387 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/SOURCES.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/dependency_links.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-02-11 05:26:14.000000 seagal-2.2/seagal.egg-info/not-zip-safe
--rw-rw-r--   0 linhua    (1008) linhua    (1010)       98 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/requires.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        7 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/top_level.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)       38 2023-04-14 14:13:57.214665 seagal-2.2/setup.cfg
--rw-rw-r--   0 linhua    (1008) linhua    (1010)      824 2023-04-10 21:45:04.000000 seagal-2.2/setup.py
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:13:08.534849 seagal-2.3/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     1068 2023-02-11 05:25:59.000000 seagal-2.3/LICENSE
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-06-02 16:13:08.534849 seagal-2.3/PKG-INFO
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3231 2023-02-11 05:37:25.000000 seagal-2.3/README.md
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:13:08.526849 seagal-2.3/seagal/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.3/seagal/__init__.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3089 2023-02-11 05:26:14.000000 seagal-2.3/seagal/_gmod.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     4508 2023-06-02 15:57:57.000000 seagal-2.3/seagal/_plotting.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)    14996 2023-06-02 16:03:58.000000 seagal-2.3/seagal/_utils.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)    11622 2023-06-02 15:57:57.000000 seagal-2.3/seagal/lee_vec.py
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:13:08.530849 seagal-2.3/seagal/modules/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.3/seagal/modules/__init__.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3113 2023-02-11 05:26:14.000000 seagal-2.3/seagal/modules/gmod.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)      978 2023-02-11 05:26:14.000000 seagal-2.3/seagal/seagal.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     7473 2023-06-02 15:57:57.000000 seagal-2.3/seagal/spatial_measure.py
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-06-02 16:13:08.530849 seagal-2.3/seagal.egg-info/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/PKG-INFO
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)      387 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/SOURCES.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/dependency_links.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-02-11 05:26:14.000000 seagal-2.3/seagal.egg-info/not-zip-safe
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)       98 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/requires.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        7 2023-06-02 16:13:08.000000 seagal-2.3/seagal.egg-info/top_level.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)       38 2023-06-02 16:13:08.534849 seagal-2.3/setup.cfg
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)      824 2023-06-02 16:11:56.000000 seagal-2.3/setup.py
```

### Comparing `seagal-2.2/LICENSE` & `seagal-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seagal-2.2/PKG-INFO` & `seagal-2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagal
-Version: 2.2
+Version: 2.3
 Summary: Spatial Enrichment Analysis of Gene Association using L-index
 Home-page: https://github.com/linhuawang/SEAGAL
 Author: Linhua Wang
 Author-email: linhuaw@bcm.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seagal-2.2/README.md` & `seagal-2.3/README.md`

 * *Files identical despite different names*

### Comparing `seagal-2.2/seagal/_gmod.py` & `seagal-2.3/seagal/_gmod.py`

 * *Files identical despite different names*

### Comparing `seagal-2.2/seagal/_plotting.py` & `seagal-2.3/seagal/_plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,20 @@
         adata.X = adata.X.toarray()
     except:
         pass
 
     if var_1 not in adata.var_names or var_2 not in adata.var_names:
         print("One of the queried features is not in the adata. Check if the correct `use_grouped` parameter is used, or typos in the names.")
         return
-
-    adata1 = Local_L(adata, var_1, var_2, dropout_rm=dropout_rm, max_RAM=32)
-    adata.obs[f'{var_1} & {var_2}'] = adata1.uns['Local_L'].ravel()
+    if f'{var_1}_{var_2}' not in adata.uns.get('Local_L_names',[]):
+        adata1 = Local_L(adata, [var_1], [var_2], dropout_rm=dropout_rm, max_RAM=32)
+        adata.obs[f'{var_1} & {var_2}'] = adata1.uns['Local_L'][:,adata1.uns['Local_L_names']==f'{var_1}_{var_2}'][:,0].ravel()
+    else:
+        adata.obs[f'{var_1} & {var_2}'] = adata.uns['Local_L'][:,adata.uns['Local_L_names']==f'{var_1}_{var_2}'][:,0].ravel()
+        
     f, ax = plt.subplots(1,1, figsize=(5,4))
     if self.data_type == 'visium':
         sc.pl.spatial(adata, color=f'{var_1} & {var_2}', ax=ax, cmap=cmap, alpha_img=alpha_img, vmin=vmin, vmax=vmax)
     else:
         vals = np.ravel(adata.obs[f'{var_1} & {var_2}'].to_numpy())
         vals[vals < vmin] = vmin
         vals[vals > vmax] = vmax
```

### Comparing `seagal-2.2/seagal/_utils.py` & `seagal-2.3/seagal/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -148,25 +148,35 @@
         df['-log10(FDR)'] = -2
         
     df["Association"] = "NS"
     df.loc[(df['L.FDR'] <= FDR_cutoff) & (df['L'] >= L_cutoff), "Association"] = "SigPos"
     df.loc[(df['L.FDR'] <= FDR_cutoff) & (df['L'] <= -L_cutoff), "Association"] = "SigNeg"
     self.co_expression = df
 
-def group_adata_by_genes(self, ct_dict = None, inplace=True):
+def group_adata_by_genes(self, ct_dict = None, inplace=True, reference='hpca'):
     ## Overwrite self.co_expression_grouped object if existed.
-    if self.co_expression_grouped is not None:
-        self.co_expression_grouped = None
-
-    data = self.raw_adata.copy()
-    sc.pp.normalize_total(data, target_sum=10**6)
-    pool_genes = data.var_names.tolist()
-
-    if ct_dict is None:
-        ct_dict = {'B cells': ['IGKC', 'EBF1', 'BANK1', 'CD79A', 'IGHD',
+    MARKER_KNOWLEDGBASE = {'hpca':{'B cells': ['POU2AF1', 'MS4A1', 'JCHAIN', 'VPREB3', 'IGLL3P', 'IGHM',
+                                         'TCL1A', 'STAP1', 'BLNK', 'TNFRSF17', 'CD19', 'CR2', 'CD79A', 
+                                         'HLA-DOB', 'IGKC', 'FCRLA', 'P2RX5', 'GUSBP11', 'CD79B', 'RGS13'],
+                         'Endothelial cells': ['GJA1', 'CTGF', 'EFEMP1', 'PLS3', 'CAV1', 'CDH5', 'ESM1',
+                                         'ARHGAP29', 'ADGRL4', 'FSTL1', 'MMP1', 'SRPX', 'CYR61', 'CAV2', 'LAMB1',
+                                          'TM4SF1', 'MMRN1', 'NNMT', 'HHIP', 'GNG11'], 
+                        'Macrophages': ['GPNMB', 'MRC1', 'CHI3L1', 'SPP1', 'PLA2G7', 'APOC1', 
+                                        'LPL', 'APOE', 'ADAMDEC1', 'CCL18', 'C1QA', 'C15orf48',
+                                         'DCSTAMP', 'FBP1', 'C1QC', 'C1QB', 'NR1H3', 'CYP1B1', 'MMP9', 'A2M'],
+                        'Monocytes': ['FCN1', 'VCAN', 'S100A12', 'S100A8', 'CSTA', 'CX3CR1', 'LYZ', 'MPEG1',
+                                         'CD14', 'S100A9', 'LILRB2', 'RGS18', 'TYROBP', 'MNDA', 'CPVL',
+                                          'APOBEC3A', 'HCK', 'CFP', 'NCF2', 'FCER1G'],
+                        'Neutrophils': ['PI3', 'CXCR2', 'FCGR3B', 'STEAP4', 'PROK2', 'MGAM', 'IL1R2',
+                                        'TNFAIP6', 'S100P', 'S100A12', 'CLC', 'KCNJ15', 'G0S2', 'KRT23',
+                                         'PTGS2', 'P2RY14', 'CXCL1', 'TREM1', 'FFAR2', 'OSM'], 
+                        'T cells': ['ITK', 'CD3D', 'TRBC1', 'TRAT1', 'TRAC', 'CD3G', 'CD2',
+                                         'LCK', 'NELL2', 'NLRC3', 'GPR171', 'THEMIS', 'CD69',
+                                          'KLRB1', 'RASGRP1', 'BCL11B', 'GZMK', 'GZMA', 'TC2N', 'ITM2A']}
+                'mouse_immune': {'B cells': ['IGKC', 'EBF1', 'BANK1', 'CD79A', 'IGHD',
                                 'BACH2', 'IGHM', 'FCHSD2', 'LY6D', 'PAX5', 
                                 'RALGPS2', 'IGLC2', 'AFF3', 'MAN1A', 'BTLA',
                                   'MEF2C', 'CD79B', 'MS4A1', 'FOXP1', 'CD55'],
                     'Endothelial': ['WFDC18', 'CSN3', 'LCN2', 'PHLDA1','KRT18',
                                     'MAP1LC3A', 'HRAS', 'AQP5', 'KRT8', 'CRIP2',
                                     'CDKN1A', 'DBI', 'PGP', 'RPS27L', '1110008P14RIK', 
                                     'SPINT2', 'MRPS6', 'DSTN', 'HMGN1', 'XBP1'],
@@ -187,49 +197,26 @@
                                     'MXD1', 'GDA', 'SORL1', 'CLEC4D', 'WFDC21', 
                                     'S100A11', 'IL1R2', 'CD44', 'PGLYRP1'], 
                     'T cells': ['GM2682', 'LEF1', 'SKAP1', 'CD3E', 'MS4A4B', 
                                 'ITK', 'CD3G', 'CD3D', 'INPP4B', 'LAT', 'SATB1', 
                                 'PRKCQ', 'THY1', 'CD247', 'TRBC2', 'BCL11B', 
                                 'NKG7', 'GRAP2', 'TCF7', 'BCL2']}
 
-        # ct_dict = {'B cells': ['IGKC', 'EBF1', 'BANK1', 'CD79A',
-        #                      'IGHD', 'IGHM', 'PAX5', 'IGLC2',
-        #                      'FCHSD2', 'CD79B', 'RALGPS2', 'LY6D',
-        #                       'MS4A1', 'MEF2C', 'IGLC3', 'BACH2', 'MAN1A',
-        #                        'CD55', 'BTLA', 'AFF3'],
-        #             'DC': ['CD209A', 'CRIP1', 'CST3', 'CBFA2T3', 
-        #                     'TCF4', 'VIM', 'PID1', 'IRF8', 'FLT3',
-        #                      'TAGLN2', 'AHNAK', 'S100A4', 'IFI30',
-        #                       'LGALS1', 'CCND1', 'SYNGR2', 'H2AFY', 
-        #                       'BST2', 'LY6C2', 'CCDC88A'],
-        #             'Macrophages': ['APOE', 'C1QB', 'C1QC', 'C1QA', 
-        #                             'CCL4', 'RGS1', 'CD81', 'MS4A7',
-        #                              'CTSB', 'LGMN', 'CTSS', 'SELENOP', 
-        #                              'CD63', 'CD72', 'CCL3', 'CTSC', 
-        #                              'TMEM176B', 'FTL1', 'ACP5', 'AIF1'], 
-        #             'Monocytes': ['PLAC8', 'SLC8A1', 'FN1', 'S100A4', 
-        #                             'LYZ2', 'LY6C2', 'F13A1', 'IFITM3', 
-        #                             'CCR2', 'ADGRE4', 'CYBB', 'CRIP1',
-        #                              'LDLRAD3', 'PID1', 'GPR141', 'LRP1',
-        #                               'CCL9', 'ZEB2', 'AHNAK', 'IFITM6'], 
-        #             'Neutrophils': ['S100A8', 'S100A9', 'RETNLG', 'CSF3R',
-        #                              'IFITM1', 'SLPI', 'HDC', 'MMP9', 
-        #                              'CXCR2', 'PBX1', 'WFDC21', 'MXD1', 
-        #                              'CLEC4D', 'GDA', 'SLFN4', 'GSR',
-        #                               'S100A11', 'IL1B', 'GCNT2', 'MSRB1'],
-        #             'NK cells': ['GZMA', 'GZMB', 'CD7', 'CCL5', 
-        #                             'NKG7', 'AW112010', 'IL2RB', 'KLRB1C', 
-        #                             'KLRE1', 'KLRK1', 'CTSW', 'KLRA7', 
-        #                             'KLRD1', 'NCR1', 'PRF1', 'ARSB', 
-        #                             'LGALS1', 'ID2', 'CST7', 'CAR2'],
-        #             'T cells': ['GM2682', 'LEF1', 'SKAP1', 'THEMIS',
-        #                          'IL7R', 'ITK', 'PRKCQ', 'BCL11B',
-        #                           'MS4A4B', 'CD247', 'TCF7', 'CD3E',
-        #                            'CD3D', 'TRBC2', 'INPP4B', 'CD3G',
-        #                             'GRAP2', 'CAMK4', 'SATB1', 'SIDT1']}
+    }
+
+    if self.co_expression_grouped is not None:
+        self.co_expression_grouped = None
+
+    data = self.raw_adata.copy()
+    sc.pp.normalize_total(data, target_sum=10**6)
+    pool_genes = data.var_names.tolist()
+
+    if ct_dict is None:
+        ct_dict = MARKER_KNOWLEDGBASE[reference]
+
     cts = list(ct_dict.keys())
     if len(cts) < 2:
         print("Please include at list 2 groups to compare against each other and call the function again.")
         return
     for key in ct_dict.keys():
         vals = [v.upper() for v in ct_dict[key] if v.upper() in pool_genes]
         ct_dict[key] = vals
```

### Comparing `seagal-2.2/seagal/lee_vec.py` & `seagal-2.3/seagal/lee_vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         self.association_ = self._statistic(X, Y, self.ctc, self.denom, max_RAM)
 
 
         if self.permutations is None:
             return self
         elif self.permutations < 1:
             return self
-
+        
         if self.permutations:
             self.reference_distribution_ = numpy.zeros((self.permutations, X.shape[1]))
 
             for i in range(self.permutations):
                 itp = numpy.random.choice(numpy.arange(X.shape[0]), int(X.shape[0]*percent), replace=False)
                 rnd_index = numpy.arange(X.shape[0])
                 rnd_index[itp] = numpy.random.permutation(itp)
@@ -118,14 +118,15 @@
             self.z_sim = (self.association_ - numpy.mean(self.reference_distribution_, axis=0)) / numpy.std(self.reference_distribution_, axis=0)
 
             #above = self.reference_distribution_ >= numpy.repeat(self.association_[numpy.newaxis,:],self.permutations,axis=0)  #self.association_
             #larger = above.sum(axis=0)
             #extreme = numpy.minimum(self.permutations - larger, larger)
             #self.significance_ = (extreme + 1.0) / (self.permutations + 1.0)
             self.significance_ = scipy.stats.norm.sf(numpy.abs(self.z_sim))
+           
         return self
 
     @staticmethod
     def _statistic(X, Y, ctc, denom, max_RAM):
 
         '''
         Memory taken (Mb): 0.000008 * (2 * p * n + p)
@@ -258,27 +259,28 @@
             for i in range(X.shape[1]):
                 perm_X = numpy.empty((self.permutations, X.shape[0]))
                 perm_Y = numpy.empty((self.permutations, Y.shape[0]))
                 for j in range(self.permutations):
                     rnd_index = numpy.random.permutation(numpy.arange(X.shape[0]))
                     perm_X[j] = X[rnd_index,i]
                     perm_Y[j] = Y[rnd_index,i]
+                
 
                 reference_distribution = numpy.transpose(
-                    (numpy.transpose(perm_Y[:,:,numpy.newaxis], (0,2,1)) @ self.standard_connectivity.T), (0, 2, 1)
-                    ) * (self.standard_connectivity @ perm_X[:,:,numpy.newaxis])
+                    (numpy.transpose(perm_Y[:,:,numpy.newaxis], (0,2,1)) @ self.standard_connectivity.T.toarray()), (0, 2, 1)
+                    ) * (self.standard_connectivity.toarray() @ perm_X[:,:,numpy.newaxis])
 
                 above = reference_distribution.squeeze(-1) >= numpy.repeat(self.associations_[:,i][numpy.newaxis,:],self.permutations,axis=0)
                 larger = above.sum(axis=0)
                 extreme = numpy.minimum(larger, self.permutations - larger)
                 self.significance_[:,i] = (extreme + 1.0) / (self.permutations + 1.0)
 
-
         else:
             self.reference_distribution_ = None
+            
         return self
 
     @staticmethod
     def _statistic(X, Y, W, max_RAM):
 
         '''
         Memory taken (Mb): 0.000008 * (3 * p * n)
```

### Comparing `seagal-2.2/seagal/modules/gmod.py` & `seagal-2.3/seagal/modules/gmod.py`

 * *Files identical despite different names*

### Comparing `seagal-2.2/seagal/seagal.py` & `seagal-2.3/seagal/seagal.py`

 * *Files identical despite different names*

### Comparing `seagal-2.2/seagal/spatial_measure.py` & `seagal-2.3/seagal/spatial_measure.py`

 * *Files 18% similar despite different names*

```diff
@@ -81,69 +81,76 @@
     
     return anndat_sp
 
 
 
 
 def Local_L(anndat_sp,
-            var_1, var_2,
+            vars_1, vars_2,
             dropout_rm=True,
             permutations=0, seed=1, max_RAM=32):
     random.seed(seed)
     np.random.seed(seed)
     start = time.time()
 
     print("Calculating local spatial correlation value...")
     
         
-    L_mtx, L_mtx_names = _calculate_LL(anndat_sp, var_1, var_2,
-                                       permutations=permutations, seed=seed, max_RAM=max_RAM)
+    L_mtx, L_mtx_names, local_p_df = _calculate_LL(anndat_sp, vars_1, vars_2,
+                                                   permutations=permutations, seed=seed, max_RAM=max_RAM)
 
     if dropout_rm:
         # print("Set L to 0 for cells with no expression on either feature of a certain pair...")
         GP_names = L_mtx_names
         Dropout_mtx = dropout_filter(anndat_sp, GP_names)
         L_mtx = L_mtx * Dropout_mtx
-
-    anndat_sp.uns['Local_L'] = L_mtx
-    anndat_sp.uns['Local_L_names'] = L_mtx_names
+    
+    if 'Local_L' in anndat_sp.uns.keys():
+        anndat_sp.uns['Local_L'] = np.concatenate((anndat_sp.uns['Local_L'], L_mtx), axis=1)
+        anndat_sp.uns['Local_L_names'] = np.concatenate((anndat_sp.uns['Local_L_names'], L_mtx_names), axis=None) #L_mtx_names
+        # remove duplicates
+        anndat_sp.uns['Local_L'] = anndat_sp.uns['Local_L'][:,(~(pd.Series(anndat_sp.uns['Local_L_names']).duplicated())).to_numpy()]
+        anndat_sp.uns['Local_L_names'] = anndat_sp.uns['Local_L_names'][(~(pd.Series(anndat_sp.uns['Local_L_names']).duplicated())).to_numpy()]
+    else:
+        anndat_sp.uns['Local_L'] = L_mtx
+        anndat_sp.uns['Local_L_names'] = L_mtx_names
+    
+    if permutations:
+        if 'Local_pval' in anndat_sp.uns.keys():
+            anndat_sp.uns['Local_pval'] = pd.concat([anndat_sp.uns['Local_pval'], local_p_df], axis=1)
+            anndat_sp.uns['Local_pval'] = anndat_sp.uns['Local_pval'].loc[:,~(anndat_sp.uns['Local_pval'].columns.duplicated())]
+        else:
+            anndat_sp.uns['Local_pval'] = local_p_df
 
     #anndat_sp.uns['peaks_nearby'] = peaks_nearby_orig.copy()
     # print("Following changes made to the AnnData object:")
     # print("\tSpatial Pearson Correlation results saved in uns['Local_L']")
     # print("\tuns['co_expression']['Local_L'] added indicates feature selected for local L calculation or not.")
 
     print("Local L elapsed time: %.3fs"%(time.time()-start))
     return anndat_sp
 
 
 
 def _calculate_LL(anndat_sp,
-                  var_1, var_2,
+                  vars_1, vars_2,
                   permutations=0, seed=1, max_RAM=16):
     random.seed(seed)
     np.random.seed(seed)
 
     #anndat_sp.var['index'] = np.arange(anndat_sp.n_vars)
     
     index_df = pd.DataFrame({'index':np.arange(anndat_sp.n_vars)})
     index_df.index = anndat_sp.var.index
     
     #if features is None:
     #    features = anndat_sp.var_names.to_numpy()
-    features_1 = [var_1]
-    features_2 = [var_2]
-    pair_names = [str(var_1) + '_' + str(var_2)]
-    '''
-    for i in range(len(features)):
-        for j in range(i+1, len(features)):
-            features_1.append(str(features[i]))
-            features_2.append(str(features[j]))
-            pair_names.append(str(features[i]) + '_' + str(features[j]))
-    '''
+    features_1 = vars_1 #[var_1]
+    features_2 = vars_2 #[var_2]
+    pair_names = [str(vars_1[i]) + '_' + str(vars_2[i]) for i in range(len(vars_1))]
 
     features_1 = np.array(features_1)
     features_2 = np.array(features_2)
 
     features_1_index = index_df.loc[features_1,'index'].to_numpy()
     features_2_index = index_df.loc[features_2,'index'].to_numpy()
 
@@ -156,18 +163,20 @@
     eSP2 = eSP2.fit(features_1_X, features_2_X, seed=seed, max_RAM=max_RAM)
     local_L_df = pd.DataFrame(eSP2.associations_)
     local_L_df.columns = pair_names
 
     if permutations:
         local_p_df = pd.DataFrame(eSP2.significance_)
         local_p_df.columns = pair_names
+    else:
+        local_p_df = pd.DataFrame()
 
     L_mtx = local_L_df.to_numpy()
 
-    return L_mtx, local_L_df.columns.to_numpy()
+    return L_mtx, local_L_df.columns.to_numpy(), local_p_df
 
 
 
 def dropout_filter(anndat_sp, GP_names):
     index_df = pd.DataFrame({'index':np.arange(len(anndat_sp.var_names))})
     index_df.index = anndat_sp.var_names
     GP_G = [gp.split('_')[0] for gp in GP_names]
```

### Comparing `seagal-2.2/seagal.egg-info/PKG-INFO` & `seagal-2.3/seagal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagal
-Version: 2.2
+Version: 2.3
 Summary: Spatial Enrichment Analysis of Gene Association using L-index
 Home-page: https://github.com/linhuawang/SEAGAL
 Author: Linhua Wang
 Author-email: linhuaw@bcm.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seagal-2.2/setup.py` & `seagal-2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='seagal',
-    version='2.2',
+    version='2.3',
     description='Spatial Enrichment Analysis of Gene Association using L-index',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/linhuawang/SEAGAL',
     author='Linhua Wang',
     author_email='linhuaw@bcm.edu',
     license='MIT',
```

