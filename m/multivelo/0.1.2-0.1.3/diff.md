# Comparing `tmp/multivelo-0.1.2.tar.gz` & `tmp/multivelo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multivelo-0.1.2.tar", last modified: Tue Jun 28 17:28:58 2022, max compression
+gzip compressed data, was "multivelo-0.1.3.tar", last modified: Fri Jun  2 20:54:03 2023, max compression
```

## Comparing `multivelo-0.1.2.tar` & `multivelo-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 chen      (1000) users      (985)        0 2022-06-28 17:28:58.282802 multivelo-0.1.2/
--rw-r--r--   0 chen      (1000) users      (985)     1509 2021-08-30 21:11:19.000000 multivelo-0.1.2/LICENSE
--rw-r--r--   0 chen      (1000) users      (985)     3680 2022-06-28 17:28:58.282802 multivelo-0.1.2/PKG-INFO
--rw-r--r--   0 chen      (1000) users      (985)     2619 2022-06-13 16:44:26.000000 multivelo-0.1.2/README.rst
--rw-r--r--   0 chen      (1000) users      (985)      273 2021-12-14 02:33:43.000000 multivelo-0.1.2/pyproject.toml
--rw-r--r--   0 chen      (1000) users      (985)     1372 2022-06-28 17:28:58.282802 multivelo-0.1.2/setup.cfg
-drwxr-xr-x   0 chen      (1000) users      (985)        0 2022-06-28 17:28:58.279469 multivelo-0.1.2/src/
-drwxr-xr-x   0 chen      (1000) users      (985)        0 2022-06-28 17:28:58.279469 multivelo-0.1.2/src/multivelo/
--rw-r--r--   0 chen      (1000) users      (985)      637 2022-05-09 00:13:15.000000 multivelo-0.1.2/src/multivelo/__init__.py
--rw-r--r--   0 chen      (1000) users      (985)    31745 2022-06-22 21:39:05.000000 multivelo-0.1.2/src/multivelo/auxiliary.py
--rw-r--r--   0 chen      (1000) users      (985)   192358 2022-06-28 17:25:38.000000 multivelo-0.1.2/src/multivelo/dynamical_chrom_func.py
--rw-r--r--   0 chen      (1000) users      (985)    24829 2022-05-05 20:25:45.000000 multivelo-0.1.2/src/multivelo/steady_chrom_func.py
-drwxr-xr-x   0 chen      (1000) users      (985)        0 2022-06-28 17:28:58.282802 multivelo-0.1.2/src/multivelo.egg-info/
--rw-r--r--   0 chen      (1000) users      (985)     3680 2022-06-28 17:28:57.000000 multivelo-0.1.2/src/multivelo.egg-info/PKG-INFO
--rw-r--r--   0 chen      (1000) users      (985)      353 2022-06-28 17:28:58.000000 multivelo-0.1.2/src/multivelo.egg-info/SOURCES.txt
--rw-r--r--   0 chen      (1000) users      (985)        1 2022-06-28 17:28:57.000000 multivelo-0.1.2/src/multivelo.egg-info/dependency_links.txt
--rw-r--r--   0 chen      (1000) users      (985)      218 2022-06-28 17:28:58.000000 multivelo-0.1.2/src/multivelo.egg-info/requires.txt
--rw-r--r--   0 chen      (1000) users      (985)       10 2022-06-28 17:28:58.000000 multivelo-0.1.2/src/multivelo.egg-info/top_level.txt
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-06-02 20:54:03.709785 multivelo-0.1.3/
+-rw-r--r--   0 jake       (501) staff       (20)     1509 2023-06-02 20:40:10.000000 multivelo-0.1.3/LICENSE
+-rw-r--r--   0 jake       (501) staff       (20)     4291 2023-06-02 20:54:03.709856 multivelo-0.1.3/PKG-INFO
+-rw-r--r--   0 jake       (501) staff       (20)     3230 2023-06-02 20:40:10.000000 multivelo-0.1.3/README.rst
+-rw-r--r--   0 jake       (501) staff       (20)      273 2023-06-02 20:40:10.000000 multivelo-0.1.3/pyproject.toml
+-rw-r--r--   0 jake       (501) staff       (20)     1379 2023-06-02 20:54:03.710237 multivelo-0.1.3/setup.cfg
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-06-02 20:54:03.706149 multivelo-0.1.3/src/
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-06-02 20:54:03.708799 multivelo-0.1.3/src/multivelo/
+-rw-r--r--   0 jake       (501) staff       (20)      676 2023-06-02 20:40:10.000000 multivelo-0.1.3/src/multivelo/__init__.py
+-rw-r--r--   0 jake       (501) staff       (20)    37763 2023-06-02 20:40:10.000000 multivelo-0.1.3/src/multivelo/auxiliary.py
+-rw-r--r--   0 jake       (501) staff       (20)   206606 2023-06-02 20:40:10.000000 multivelo-0.1.3/src/multivelo/dynamical_chrom_func.py
+-rw-r--r--   0 jake       (501) staff       (20)     9484 2023-06-02 20:40:10.000000 multivelo-0.1.3/src/multivelo/pyWNN.py
+-rw-r--r--   0 jake       (501) staff       (20)    25200 2023-06-02 20:40:10.000000 multivelo-0.1.3/src/multivelo/steady_chrom_func.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-06-02 20:54:03.709659 multivelo-0.1.3/src/multivelo.egg-info/
+-rw-r--r--   0 jake       (501) staff       (20)     4291 2023-06-02 20:54:03.000000 multivelo-0.1.3/src/multivelo.egg-info/PKG-INFO
+-rw-r--r--   0 jake       (501) staff       (20)      376 2023-06-02 20:54:03.000000 multivelo-0.1.3/src/multivelo.egg-info/SOURCES.txt
+-rw-r--r--   0 jake       (501) staff       (20)        1 2023-06-02 20:54:03.000000 multivelo-0.1.3/src/multivelo.egg-info/dependency_links.txt
+-rw-r--r--   0 jake       (501) staff       (20)      225 2023-06-02 20:54:03.000000 multivelo-0.1.3/src/multivelo.egg-info/requires.txt
+-rw-r--r--   0 jake       (501) staff       (20)       10 2023-06-02 20:54:03.000000 multivelo-0.1.3/src/multivelo.egg-info/top_level.txt
```

### Comparing `multivelo-0.1.2/LICENSE` & `multivelo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multivelo-0.1.2/PKG-INFO` & `multivelo-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multivelo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Multi-omic extension of single-cell RNA velocity
 Home-page: https://github.com/welch-lab/MultiVelo
 Author: Chen Li
 Author-email: chlseven@umich.edu
 License: BSD 3-Clause License
 Keywords: RNA velocity,single-cell,transcriptomics,chromatin,epigenetic,epigenomic,gene regulation,multi-omic,dynamical
 Classifier: Development Status :: 4 - Beta
@@ -35,26 +35,47 @@
 MultiVelo uses a probabilistic latent variable model to estimate the switch time and rate 
 parameters of gene regulation, providing a quantitative summary of the temporal relationship 
 between epigenomic and transcriptomic changes. Fitting MultiVelo on single-cell multi-omic 
 datasets revealed two distinct mechanisms of regulation by chromatin accessibility, quantified 
 the degree of concordance or discordance between transcriptomic and epigenomic states within 
 each cell, and inferred the lengths of time lags between transcriptomic and epigenomic changes.
 
-Install through PyPI: **pip install multivelo**
+Installation
+------------
 
-**New**: `ReadTheDocs <https://multivelo.readthedocs.io/en/latest/>`_ page is up. You can find detailed parameter descriptions and tutorials on the website.
+Install through PyPI: 
 
-A tutorial showing how to run MultiVelo can be found in `multivelo_demo <https://github.com/welch-lab/MultiVelo/tree/main/multivelo_demo>`_.
+``pip install multivelo``
 
-We use the embryonic E18 mouse brain from 10X Multiome as an example (`jupyter notebook <https://github.com/welch-lab/MultiVelo/tree/main/multivelo_demo/MultiVelo_Demo.ipynb>`_).
+The package is also available on Bioconda. Install with:
 
+``conda install -c bioconda multivelo`` or ``mamba install -c bioconda multivelo``
+
+Documentation
+-------------
+
+We have a `ReadTheDocs <https://multivelo.readthedocs.io/en/latest/>`_ page.
+
+Tutorial
+--------
+
+*New*: we have added Jupyter notebooks showing how to reproduce the main figure panels, along with all required processed data files. These can be found under the `Examples <https://github.com/welch-lab/MultiVelo/tree/main/Examples>`_ folder in this repository or on our `ReadTheDocs <https://multivelo.readthedocs.io/en/latest/>`_ page.
+
+A tutorial showing how to run MultiVelo can be found here: (`jupyter notebook <https://github.com/welch-lab/MultiVelo/blob/main/Examples/MultiVelo_Demo.ipynb>`_)
+
+The tutorial uses the embryonic E18 mouse brain from 10X Multiome as an example.
 CellRanger output files can be downloaded from 
 `10X website <https://www.10xgenomics.com/resources/datasets/fresh-embryonic-e-18-mouse-brain-5-k-1-standard-1-0-0>`_. 
 Crucially, the filtered feature barcode matrix folder, ATAC peak annotations TSV, and the feature 
 linkage BEDPE file in the secondary analysis outputs folder will be needed in this demo.
 
 You can download the processed data that we used for this analysis if you want to run the example yourself. 
 Unspliced and spliced counts, as well as cell type annotations can be downloaded from the MultiVelo GitHub page. 
 We provide the cell annotations for this dataset in "cell_annotations.tsv". 
 We also provide the nearest neighbor graph used to smooth chromatin accessibility values in the GitHub folder "seurat_wnn", 
 which contains a zip file of three files: "nn_cells.txt", "nn_dist.txt", and "nn_idx.txt". Please unzip the archive after downloading. 
 The R script used to generate these files can also be found in the same folder.
+
+Citation
+--------
+
+| Li, C., Virgilio, M.C., Collins, K.L. & Welch J.D. Multi-omic single-cell velocity models epigenome–transcriptome interactions and improves cell fate prediction. *Nat Biotechnol* (2022).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `multivelo-0.1.2/README.rst` & `multivelo-0.1.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,26 +10,47 @@
 MultiVelo uses a probabilistic latent variable model to estimate the switch time and rate 
 parameters of gene regulation, providing a quantitative summary of the temporal relationship 
 between epigenomic and transcriptomic changes. Fitting MultiVelo on single-cell multi-omic 
 datasets revealed two distinct mechanisms of regulation by chromatin accessibility, quantified 
 the degree of concordance or discordance between transcriptomic and epigenomic states within 
 each cell, and inferred the lengths of time lags between transcriptomic and epigenomic changes.
 
-Install through PyPI: **pip install multivelo**
+Installation
+------------
 
-**New**: `ReadTheDocs <https://multivelo.readthedocs.io/en/latest/>`_ page is up. You can find detailed parameter descriptions and tutorials on the website.
+Install through PyPI: 
 
-A tutorial showing how to run MultiVelo can be found in `multivelo_demo <https://github.com/welch-lab/MultiVelo/tree/main/multivelo_demo>`_.
+``pip install multivelo``
 
-We use the embryonic E18 mouse brain from 10X Multiome as an example (`jupyter notebook <https://github.com/welch-lab/MultiVelo/tree/main/multivelo_demo/MultiVelo_Demo.ipynb>`_).
+The package is also available on Bioconda. Install with:
 
+``conda install -c bioconda multivelo`` or ``mamba install -c bioconda multivelo``
+
+Documentation
+-------------
+
+We have a `ReadTheDocs <https://multivelo.readthedocs.io/en/latest/>`_ page.
+
+Tutorial
+--------
+
+*New*: we have added Jupyter notebooks showing how to reproduce the main figure panels, along with all required processed data files. These can be found under the `Examples <https://github.com/welch-lab/MultiVelo/tree/main/Examples>`_ folder in this repository or on our `ReadTheDocs <https://multivelo.readthedocs.io/en/latest/>`_ page.
+
+A tutorial showing how to run MultiVelo can be found here: (`jupyter notebook <https://github.com/welch-lab/MultiVelo/blob/main/Examples/MultiVelo_Demo.ipynb>`_)
+
+The tutorial uses the embryonic E18 mouse brain from 10X Multiome as an example.
 CellRanger output files can be downloaded from 
 `10X website <https://www.10xgenomics.com/resources/datasets/fresh-embryonic-e-18-mouse-brain-5-k-1-standard-1-0-0>`_. 
 Crucially, the filtered feature barcode matrix folder, ATAC peak annotations TSV, and the feature 
 linkage BEDPE file in the secondary analysis outputs folder will be needed in this demo.
 
 You can download the processed data that we used for this analysis if you want to run the example yourself. 
 Unspliced and spliced counts, as well as cell type annotations can be downloaded from the MultiVelo GitHub page. 
 We provide the cell annotations for this dataset in "cell_annotations.tsv". 
 We also provide the nearest neighbor graph used to smooth chromatin accessibility values in the GitHub folder "seurat_wnn", 
 which contains a zip file of three files: "nn_cells.txt", "nn_dist.txt", and "nn_idx.txt". Please unzip the archive after downloading. 
 The R script used to generate these files can also be found in the same folder.
+
+Citation
+--------
+
+| Li, C., Virgilio, M.C., Collins, K.L. & Welch J.D. Multi-omic single-cell velocity models epigenome–transcriptome interactions and improves cell fate prediction. *Nat Biotechnol* (2022).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `multivelo-0.1.2/setup.cfg` & `multivelo-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multivelo
-version = 0.1.2
+version = 0.1.3
 author = Chen Li
 author_email = chlseven@umich.edu
 description = Multi-omic extension of single-cell RNA velocity
 long_description = file: README.rst
 url = https://github.com/welch-lab/MultiVelo
 keywords = 
 	RNA velocity
@@ -49,15 +49,15 @@
 	scipy>=1.4.1
 	pandas>=0.23
 	scikit-learn>=0.23.0
 	matplotlib>=3.3.0
 	seaborn>=0.11.0
 	tqdm
 	joblib
-	ipywidgets
+	ipywidgets<=7.7.1
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 	multivelo_demo
 	docs
```

### Comparing `multivelo-0.1.2/src/multivelo/auxiliary.py` & `multivelo-0.1.3/src/multivelo/auxiliary.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,30 +3,42 @@
 from scipy.sparse import coo_matrix, csr_matrix, diags
 from umap.umap_ import fuzzy_simplicial_set
 from anndata import AnnData
 import scanpy as sc
 import scvelo as scv
 import pandas as pd
 from tqdm.auto import tqdm
-import ipywidgets
+import scipy
+import os
+import sys
+
+current_path = os.path.dirname(__file__)
+
+sys.path.append(current_path)
+
+from pyWNN import pyWNN
+
+def aggregate_peaks_10x(adata_atac, peak_annot_file, linkage_file,
+                        peak_dist=10000, min_corr=0.5, gene_body=False,
+                        return_dict=False, verbose=False):
 
-def aggregate_peaks_10x(adata_atac, peak_annot_file, linkage_file, peak_dist=10000, min_corr=0.5, gene_body=False, return_dict=False, verbose=False):
     """Peak to gene aggregation.
 
-    This function aggregates promoter and enhancer peaks to genes based on the 10X linkage file.
+    This function aggregates promoter and enhancer peaks to genes based on the
+    10X linkage file.
 
     Parameters
     ----------
     adata_atac: :class:`~anndata.AnnData`
         ATAC anndata object which stores raw peak counts.
     peak_annot_file: `str`
         Peak annotation file from 10X CellRanger ARC.
     linkage_file: `str`
-        Peak-gene linkage file from 10X CellRanger ARC. This file stores highly correlated peak-peak
-        and peak-gene pair information.
+        Peak-gene linkage file from 10X CellRanger ARC. This file stores highly
+        correlated peak-peak and peak-gene pair information.
     peak_dist: `int` (default: 10000)
         Maximum distance for peaks to be included for a gene.
     min_corr: `float` (default: 0.5)
         Minimum correlation for a peak to be considered as enhancer.
     gene_body: `bool` (default: `False`)
         Whether to add gene body peaks to the associated promoters.
     return_dict: `bool` (default: `False`)
@@ -51,27 +63,29 @@
         header = next(f)
         tmp = header.split('\t')
         if len(tmp) == 4:
             cellranger_version = 1
         elif len(tmp) == 6:
             cellranger_version = 2
         else:
-            raise ValueError('Peak annotation file should contain 4 columns (CellRanger ARC 1.0.0) or 5 columns (CellRanger ARC 2.0.0)')
+            raise ValueError('Peak annotation file should contain 4 columns '
+                             '(CellRanger ARC 1.0.0) or 5 columns (CellRanger '
+                             'ARC 2.0.0)')
         if verbose:
             print(f'CellRanger ARC identified as {cellranger_version}.0.0')
         if cellranger_version == 1:
             for line in f:
                 tmp = line.rstrip().split('\t')
                 tmp1 = tmp[0].split('_')
                 peak = f'{tmp1[0]}:{tmp1[1]}-{tmp1[2]}'
                 if tmp[1] != '':
                     genes = tmp[1].split(';')
                     dists = tmp[2].split(';')
                     types = tmp[3].split(';')
-                    for i,gene in enumerate(genes):
+                    for i, gene in enumerate(genes):
                         dist = dists[i]
                         annot = types[i]
                         if annot == 'promoter':
                             if gene not in promoter_dict:
                                 promoter_dict[gene] = [peak]
                             else:
                                 promoter_dict[gene].append(peak)
@@ -120,84 +134,126 @@
                 tmp2 = tmp[6].split('><')[0][1:].split(';')
                 tmp3 = tmp[6].split('><')[1][:-1].split(';')
                 corr = float(tmp[7])
                 for t2 in tmp2:
                     gene1 = t2.split('_')
                     for t3 in tmp3:
                         gene2 = t3.split('_')
-                        # one of the peaks is in promoter, peaks belong to the same gene or are close in distance
-                        if ((gene1[1] == "promoter") != (gene2[1] == "promoter")) and ((gene1[0] == gene2[0]) or (float(tmp[11]) < peak_dist)):
+                        # one of the peaks is in promoter, peaks belong to the
+                        # same gene or are close in distance
+                        if (((gene1[1] == "promoter") !=
+                            (gene2[1] == "promoter")) and
+                            ((gene1[0] == gene2[0]) or
+                             (float(tmp[11]) < peak_dist))):
+
                             if gene1[1] == "promoter":
                                 gene = gene1[0]
                             else:
                                 gene = gene2[0]
                             if gene in corr_dict:
-                                # peak 1 is in promoter, peak 2 is not in gene body -> peak 2 is added to gene 1
-                                if peak2 not in corr_dict[gene] and gene1[1] == "promoter" and (gene2[0] not in gene_body_dict or peak2 not in gene_body_dict[gene2[0]]):
+                                # peak 1 is in promoter, peak 2 is not in gene
+                                # body -> peak 2 is added to gene 1
+                                if (peak2 not in corr_dict[gene] and
+                                    gene1[1] == "promoter" and
+                                    (gene2[0] not in gene_body_dict or
+                                     peak2 not in gene_body_dict[gene2[0]])):
+
                                     corr_dict[gene][0].append(peak2)
                                     corr_dict[gene][1].append(corr)
-                                # peak 2 is in promoter, peak 1 is not in gene body -> peak 1 is added to gene 2
-                                if peak1 not in corr_dict[gene] and gene2[1] == "promoter" and (gene1[0] not in gene_body_dict or peak1 not in gene_body_dict[gene1[0]]):
+                                # peak 2 is in promoter, peak 1 is not in gene
+                                # body -> peak 1 is added to gene 2
+                                if (peak1 not in corr_dict[gene] and
+                                    gene2[1] == "promoter" and
+                                    (gene1[0] not in gene_body_dict or
+                                     peak1 not in gene_body_dict[gene1[0]])):
+
                                     corr_dict[gene][0].append(peak1)
                                     corr_dict[gene][1].append(corr)
                             else:
-                                # peak 1 is in promoter, peak 2 is not in gene body -> peak 2 is added to gene 1
-                                if gene1[1] == "promoter" and (gene2[0] not in gene_body_dict or peak2 not in gene_body_dict[gene2[0]]):
+                                # peak 1 is in promoter, peak 2 is not in gene
+                                # body -> peak 2 is added to gene 1
+                                if (gene1[1] == "promoter" and
+                                    (gene2[0] not in
+                                     gene_body_dict
+                                     or peak2 not in
+                                     gene_body_dict[gene2[0]])):
+
                                     corr_dict[gene] = [[peak2], [corr]]
-                                # peak 2 is in promoter, peak 1 is not in gene body -> peak 1 is added to gene 2
-                                if gene2[1] == "promoter" and (gene1[0] not in gene_body_dict or peak1 not in gene_body_dict[gene1[0]]):
+                                # peak 2 is in promoter, peak 1 is not in gene
+                                # body -> peak 1 is added to gene 2
+                                if (gene2[1] == "promoter" and
+                                    (gene1[0] not in
+                                     gene_body_dict
+                                     or peak1 not in
+                                     gene_body_dict[gene1[0]])):
+
                                     corr_dict[gene] = [[peak1], [corr]]
             elif tmp[12] == "peak-gene":
                 peak1 = f'{tmp[0]}:{tmp[1]}-{tmp[2]}'
                 tmp2 = tmp[6].split('><')[0][1:].split(';')
                 gene2 = tmp[6].split('><')[1][:-1]
                 corr = float(tmp[7])
                 for t2 in tmp2:
                     gene1 = t2.split('_')
-                    # peak 1 belongs to gene 2 or are close in distance -> peak 1 is added to gene 2
+                    # peak 1 belongs to gene 2 or are close in distance
+                    # -> peak 1 is added to gene 2
                     if ((gene1[0] == gene2) or (float(tmp[11]) < peak_dist)):
                         gene = gene1[0]
                         if gene in corr_dict:
-                            if peak1 not in corr_dict[gene] and gene1[1] != "promoter" and (gene1[0] not in gene_body_dict or peak1 not in gene_body_dict[gene1[0]]):
+                            if (peak1 not in corr_dict[gene] and
+                                gene1[1] != "promoter" and
+                                (gene1[0] not in gene_body_dict or
+                                 peak1 not in gene_body_dict[gene1[0]])):
+
                                 corr_dict[gene][0].append(peak1)
                                 corr_dict[gene][1].append(corr)
                         else:
-                            if gene1[1] != "promoter" and (gene1[0] not in gene_body_dict or peak1 not in gene_body_dict[gene1[0]]):
+                            if (gene1[1] != "promoter" and
+                                (gene1[0] not in gene_body_dict or
+                                 peak1 not in gene_body_dict[gene1[0]])):
                                 corr_dict[gene] = [[peak1], [corr]]
             elif tmp[12] == "gene-peak":
                 peak2 = f'{tmp[3]}:{tmp[4]}-{tmp[5]}'
                 gene1 = tmp[6].split('><')[0][1:]
                 tmp3 = tmp[6].split('><')[1][:-1].split(';')
                 corr = float(tmp[7])
                 for t3 in tmp3:
                     gene2 = t3.split('_')
-                    # peak 2 belongs to gene 1 or are close in distance -> peak 2 is added to gene 1
+                    # peak 2 belongs to gene 1 or are close in distance
+                    # -> peak 2 is added to gene 1
                     if ((gene1 == gene2[0]) or (float(tmp[11]) < peak_dist)):
                         gene = gene1
                         if gene in corr_dict:
-                            if peak2 not in corr_dict[gene] and gene2[1] != "promoter" and (gene2[0] not in gene_body_dict or peak2 not in gene_body_dict[gene2[0]]):
+                            if (peak2 not in corr_dict[gene] and
+                                gene2[1] != "promoter" and
+                                (gene2[0] not in gene_body_dict or
+                                 peak2 not in gene_body_dict[gene2[0]])):
+
                                 corr_dict[gene][0].append(peak2)
                                 corr_dict[gene][1].append(corr)
                         else:
-                            if gene2[1] != "promoter" and (gene2[0] not in gene_body_dict or peak2 not in gene_body_dict[gene2[0]]):
+                            if (gene2[1] != "promoter" and
+                                (gene2[0] not in gene_body_dict or
+                                 peak2 not in gene_body_dict[gene2[0]])):
+
                                 corr_dict[gene] = [[peak2], [corr]]
 
     gene_dict = promoter_dict
     enhancer_dict = {}
     promoter_genes = list(promoter_dict.keys())
     if verbose:
         print(f'Found {len(promoter_genes)} genes with promoter peaks')
     for gene in promoter_genes:
-        if gene_body: # add gene-body peaks
+        if gene_body:  # add gene-body peaks
             if gene in gene_body_dict:
                 for peak in gene_body_dict[gene]:
                     if peak not in gene_dict[gene]:
                         gene_dict[gene].append(peak)
         enhancer_dict[gene] = []
-        if gene in corr_dict: # add enhancer peaks
+        if gene in corr_dict:  # add enhancer peaks
             for j, peak in enumerate(corr_dict[gene][0]):
                 corr = corr_dict[gene][1][j]
                 if corr > min_corr:
                     if peak not in gene_dict[gene]:
                         gene_dict[gene].append(peak)
                         enhancer_dict[gene].append(peak)
 
@@ -206,20 +262,20 @@
     gene_mat = np.zeros((adata_atac.shape[0], len(promoter_genes)))
     var_names = adata_atac.var_names.to_numpy()
     for i, gene in tqdm(enumerate(promoter_genes), total=len(promoter_genes)):
         peaks = gene_dict[gene]
         for peak in peaks:
             if peak in var_names:
                 peak_index = np.where(var_names == peak)[0][0]
-                gene_mat[:,i] += adata_atac_X_copy[:,peak_index]
+                gene_mat[:, i] += adata_atac_X_copy[:, peak_index]
     gene_mat[gene_mat < 0] = 0
     gene_mat = AnnData(X=csr_matrix(gene_mat))
     gene_mat.obs_names = pd.Index(list(adata_atac.obs_names))
     gene_mat.var_names = pd.Index(promoter_genes)
-    gene_mat = gene_mat[:,gene_mat.X.sum(0) > 0]
+    gene_mat = gene_mat[:, gene_mat.X.sum(0) > 0]
     if return_dict:
         return gene_mat, promoter_dict, enhancer_dict
     else:
         return gene_mat
 
 
 def tfidf_norm(adata_atac, scale_factor=1e4, copy=False):
@@ -234,29 +290,114 @@
     scale_factor: `float` (default: 1e4)
         Value to be multiplied after normalization.
     copy: `bool` (default: `False`)
         Whether to return a copy or modify `.X` directly.
 
     Returns
     -------
-    If `copy==True`, a new ATAC anndata object which stores normalized counts in `.X`.
+    If `copy==True`, a new ATAC anndata object which stores normalized counts
+    in `.X`.
     """
     npeaks = adata_atac.X.sum(1)
     npeaks_inv = csr_matrix(1.0/npeaks)
     tf = adata_atac.X.multiply(npeaks_inv)
     idf = diags(np.ravel(adata_atac.X.shape[0] / adata_atac.X.sum(0))).log1p()
     if copy:
         adata_atac_copy = adata_atac.copy()
         adata_atac_copy.X = tf.dot(idf) * scale_factor
         return adata_atac_copy
     else:
         adata_atac.X = tf.dot(idf) * scale_factor
 
 
-def knn_smooth_chrom(adata_atac, nn_idx=None, nn_dist=None, conn=None, n_neighbors=None):
+def gen_wnn(adata_rna, adata_adt, dims, nn):
+    """Computes inputs for KNN smoothing.
+
+    This function calculates the nn_idx and nn_dist matrices needed
+    to run knn_smooth_chrom().
+
+    Parameters
+    ----------
+    adata_rna: :class:`~anndata.AnnData`
+        RNA anndata object.
+    adata_atac: :class:`~anndata.AnnData`
+        ATAC anndata object.
+    dims: `List[int]`
+        Dimensions of data for RNA (index=0) and ATAC (index=1)
+    nn: `int` (default: `None`)
+        Top N neighbors to extract for each cell in the connectivities matrix.
+
+    Returns
+    -------
+    nn_idx: `np.darray` (default: `None`)
+        KNN index matrix of size (cells, k).
+    nn_dist: `np.darray` (default: `None`)
+        KNN distance matrix of size (cells, k).
+    """
+
+    # make a copy of the original adata objects so as to keep them unchanged
+    rna_copy = adata_rna.copy()
+    adt_copy = adata_adt.copy()
+
+    sc.tl.pca(rna_copy,
+              n_comps=dims[0],
+              random_state=np.random.RandomState(seed=42),
+              use_highly_variable=True)  # run PCA on RNA
+
+    lsi = scipy.sparse.linalg.svds(adt_copy.X, k=dims[1])  # run SVD on ADT
+
+    # get the lsi result
+    adt_copy.obsm['X_lsi'] = lsi[0]
+
+    # add the PCA from adt to rna
+    rna_copy.obsm['X_rna_pca'] = rna_copy.obsm.pop('X_pca')
+    rna_copy.obsm['X_adt_lsi'] = adt_copy.obsm['X_lsi']
+
+    # run WNN
+    WNNobj = pyWNN(rna_copy,
+                      reps=['X_rna_pca', 'X_adt_lsi'],
+                      npcs=dims,
+                      n_neighbors=nn,
+                      seed=42)
+
+    adata_seurat = WNNobj.compute_wnn(rna_copy)
+
+    # get the matrix storing the distances between each cell and its neighbors
+    cx = scipy.sparse.coo_matrix(adata_seurat.obsp["WNN_distance"])
+
+    # the number of cells
+    cells = adata_seurat.obsp['WNN_distance'].shape[0]
+
+    # define the shape of our final results
+    # and make the arrays that will hold the results
+    new_shape = (cells, nn)
+    nn_dist = np.zeros(shape=new_shape)
+    nn_idx = np.zeros(shape=new_shape)
+
+    # new_col defines what column we store data in
+    # our result arrays
+    new_col = 0
+
+    # loop through the distance matrices
+    for i, j, v in zip(cx.row, cx.col, cx.data):
+
+        # store the distances between neighbor cells
+        nn_dist[i][new_col % nn] = v
+
+        # for each cell's row, store the row numbers of its neighbor cells
+        # (1-indexing instead of 0- is a holdover from R multimodalneighbors())
+        nn_idx[i][new_col % nn] = int(j) + 1
+
+        new_col += 1
+
+    return nn_idx, nn_dist
+
+
+def knn_smooth_chrom(adata_atac, nn_idx=None, nn_dist=None, conn=None,
+                     n_neighbors=None):
     """KNN smoothing.
 
     This function smooth (impute) the count matrix with k nearest neighbors.
     The inputs can be either KNN index and distance matrices or a pre-computed
     connectivities matrix (for example in adata_rna object).
 
     Parameters
@@ -274,96 +415,117 @@
 
     Returns
     -------
     `.layers['Mc']` stores imputed values.
     """
     if nn_idx is not None and nn_dist is not None:
         if nn_idx.shape[0] != adata_atac.shape[0]:
-            raise ValueError('Number of rows of KNN indices does not equal to number of observations.')
+            raise ValueError('Number of rows of KNN indices does not equal to '
+                             'number of observations.')
         if nn_dist.shape[0] != adata_atac.shape[0]:
-            raise ValueError('Number of rows of KNN distances does not equal to number of observations.')
+            raise ValueError('Number of rows of KNN distances does not equal '
+                             'to number of observations.')
         X = coo_matrix(([], ([], [])), shape=(nn_idx.shape[0], 1))
-        conn, sigma, rho, dists = fuzzy_simplicial_set(X, nn_idx.shape[1], None, None, knn_indices=nn_idx-1, knn_dists=nn_dist, return_dists=True)
+        conn, sigma, rho, dists = fuzzy_simplicial_set(X, nn_idx.shape[1],
+                                                       None, None,
+                                                       knn_indices=nn_idx-1,
+                                                       knn_dists=nn_dist,
+                                                       return_dists=True)
     elif conn is not None:
         pass
     else:
-        raise ValueError('Please input nearest neighbor indices and distances, or a connectivities matrix of size n x n, with columns being neighbors.' + 
-                         ' For example, RNA connectivities can usually be found in adata.obsp.')
+        raise ValueError('Please input nearest neighbor indices and distances,'
+                         ' or a connectivities matrix of size n x n, with '
+                         'columns being neighbors.'
+                         ' For example, RNA connectivities can usually be '
+                         'found in adata.obsp.')
+
     conn = conn.tocsr().copy()
     n_counts = (conn > 0).sum(1).A1
     if n_neighbors is not None and n_neighbors < n_counts.min():
         conn = top_n_sparse(conn, n_neighbors)
     conn.setdiag(1)
     conn_norm = conn.multiply(1.0 / conn.sum(1)).tocsr()
     adata_atac.layers['Mc'] = csr_matrix.dot(conn_norm, adata_atac.X)
     adata_atac.obsp['connectivities'] = conn
 
 
 def calculate_qc_metrics(adata, **kwargs):
     """Basic QC metrics.
 
-    This function calculate basic QC metrics with `scanpy.pp.calculate_qc_metrics`.
-    Additionally, total counts and the ratio of unspliced and spliced matrices, as well as
-    the cell cycle scores (with `scvelo.tl.score_genes_cell_cycle`) will be computed. 
+    This function calculate basic QC metrics with
+    `scanpy.pp.calculate_qc_metrics`.
+    Additionally, total counts and the ratio of unspliced and spliced matrices,
+    as well as the cell cycle scores (with `scvelo.tl.score_genes_cell_cycle`)
+    will be computed.
 
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         RNA anndata object. Required fields: `unspliced` and `spliced`.
     Additional parameters passed to `scanpy.pp.calculate_qc_metrics`.
 
     Returns
     -------
-    Outputs of `scanpy.pp.calculate_qc_metrics` and `scvelo.tl.score_genes_cell_cycle`.
-    total_unspliced, total_spliced: `.var`
+    Outputs of `scanpy.pp.calculate_qc_metrics` and
+    `scvelo.tl.score_genes_cell_cycle`. total_unspliced, total_spliced: `.var`
         total counts of unspliced and spliced matrices.
     unspliced_ratio: `.var`
         ratio of unspliced counts vs (unspliced + spliced counts).
     cell_cycle_score: `.var`
         cell cycle score difference between G2M_score and S_score.
     """
+    print("Running from here!")
     sc.pp.calculate_qc_metrics(adata, **kwargs)
     if 'spliced' not in adata.layers:
         raise ValueError('Spliced matrix not found in adata.layers')
     if 'unspliced' not in adata.layers:
         raise ValueError('Unspliced matrix not found in adata.layers')
-    total_s = np.nansum(adata.layers['spliced'], axis=1)
-    total_u = np.nansum(adata.layers['unspliced'], axis=1)
-    adata.var['total_unspliced'] = total_u
-    adata.var['total_spliced'] = total_s
-    adata.var['unspliced_ratio'] = total_u / (total_s + total_u)
+    print(adata.layers['spliced'].shape)
+    total_s = np.nansum(adata.layers['spliced'].toarray(), axis=1)
+    total_u = np.nansum(adata.layers['unspliced'].toarray(), axis=1)
+    print(total_u.shape)
+    adata.obs['total_unspliced'] = total_u
+    adata.obs['total_spliced'] = total_s
+    adata.obs['unspliced_ratio'] = total_u / (total_s + total_u)
     scv.tl.score_genes_cell_cycle(adata)
-    adata.obs['cell_cycle_score'] = adata.obs['G2M_score'] - adata.obs['S_score']
+    adata.obs['cell_cycle_score'] = (adata.obs['G2M_score']
+                                     - adata.obs['S_score'])
 
 
-def ellipse_fit(adata, 
-                genes, 
-                color_by='quantile', 
-                n_cols=8, 
-                title=None, 
-                figsize=None, 
+def ellipse_fit(adata,
+                genes,
+                color_by='quantile',
+                n_cols=8,
+                title=None,
+                figsize=None,
                 axis_on=False,
-                pointsize=2, 
+                pointsize=2,
                 linewidth=2
                 ):
     """Fit ellipses to unspliced and spliced phase portraits.
 
-    This function plots the ellipse fits on the unspliced-spliced phase portraits.
+    This function plots the ellipse fits on the unspliced-spliced phase
+    portraits.
 
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         RNA anndata object. Required fields: `Mu` and `Ms`.
     genes: `str`,  list of `str`
         List of genes to plot.
     color_by: `str` (default: `quantile`)
-        Color by the four quantiles based on ellipse fit if `quantile`. Other common values are leiden, louvain, celltype, etc.
-        If not `quantile`, the color field must be present in `.uns`, which can be pre-computed with `scanpy.pl.scatter`.
-        For `quantile`, red, orange, green, and blue represent quantile left, top, right, and bottom, respectively.
-        If `quantile_scores`, `multivelo.compute_quantile_scores` function must have been run.
+        Color by the four quantiles based on ellipse fit if `quantile`. Other
+        common values are leiden, louvain, celltype, etc.
+        If not `quantile`, the color field must be present in `.uns`, which
+        can be pre-computed with `scanpy.pl.scatter`.
+        For `quantile`, red, orange, green, and blue represent quantile left,
+        top, right, and bottom, respectively.
+        If `quantile_scores`, `multivelo.compute_quantile_scores` function
+        must have been run.
     n_cols: `int` (default: 8)
         Number of columns to plot on each row.
     figsize: `tuple` (default: `None`)
         Total figure size.
     title: `tuple` (default: `None`)
         Title of the figure. Default is `Ellipse Fit`.
     axis_on: `bool` (default: `False`)
@@ -377,51 +539,56 @@
     by_quantile_score = color_by == 'quantile_scores'
     if not by_quantile and not by_quantile_score:
         types = adata.obs[color_by].cat.categories
         colors = adata.uns[f'{color_by}_colors']
     gn = len(genes)
     if gn < n_cols:
         n_cols = gn
-    fig, axs = plt.subplots(-(-gn // n_cols), n_cols, figsize=(2 * n_cols, 2.4 * (-(-gn // n_cols))) if figsize is None else figsize)
+    fig, axs = plt.subplots(-(-gn // n_cols), n_cols, figsize=(2 * n_cols,
+                            2.4 * (-(-gn // n_cols)))
+                            if figsize is None else figsize)
     count = 0
     for gene in genes:
-        u = np.array(adata[:,gene].layers['Mu'])
-        s = np.array(adata[:,gene].layers['Ms'])
+        u = np.array(adata[:, gene].layers['Mu'])
+        s = np.array(adata[:, gene].layers['Ms'])
         row = count // n_cols
         col = count % n_cols
-        non_zero = (u>0) & (s>0)
+        non_zero = (u > 0) & (s > 0)
         if np.sum(non_zero) < 10:
             count += 1
             fig.delaxes(axs[row, col])
             continue
 
         mean_u, mean_s = np.mean(u[non_zero]), np.mean(s[non_zero])
         std_u, std_s = np.std(u[non_zero]), np.std(s[non_zero])
         u_ = (u - mean_u)/std_u
         s_ = (s - mean_s)/std_s
-        X = np.reshape(s_[non_zero], (-1,1))
-        Y = np.reshape(u_[non_zero], (-1,1))
+        X = np.reshape(s_[non_zero], (-1, 1))
+        Y = np.reshape(u_[non_zero], (-1, 1))
 
         # Ax^2 + Bxy + Cy^2 + Dx + Ey + 1 = 0
         A = np.hstack([X**2, X * Y, Y**2, X, Y])
         b = -np.ones_like(X)
-        x,res,_,_ = np.linalg.lstsq(A, b)
+        x, res, _, _ = np.linalg.lstsq(A, b)
         x = x.squeeze()
-        A,B,C,D,E = x
+        A, B, C, D, E = x
         good_fit = B**2 - 4*A*C < 0
-        theta = np.arctan(B/(A - C))/2 if x[0] > x[2] else np.pi/2 + np.arctan(B/(A - C))/2
+        theta = np.arctan(B/(A - C))/2 \
+            if x[0] > x[2] \
+            else np.pi/2 + np.arctan(B/(A - C))/2
         good_fit = good_fit & (theta < np.pi/2) & (theta > 0)
         if not good_fit:
             count += 1
             fig.delaxes(axs[row, col])
             continue
         x_coord = np.linspace((-mean_s)/std_s, (np.max(s)-mean_s)/std_s, 500)
         y_coord = np.linspace((-mean_u)/std_u, (np.max(u)-mean_u)/std_u, 500)
         X_coord, Y_coord = np.meshgrid(x_coord, y_coord)
-        Z_coord = A * X_coord**2 + B * X_coord * Y_coord + C * Y_coord**2 + D * X_coord + E * Y_coord + 1
+        Z_coord = (A * X_coord**2 + B * X_coord * Y_coord + C * Y_coord**2 +
+                   D * X_coord + E * Y_coord + 1)
 
         M0 = np.array([
              A, B/2, D/2,
              B/2, C, E/2,
              D/2, E/2, 1,
         ]).reshape(3, 3)
         M = np.array([
@@ -441,47 +608,62 @@
         xbot = xc - a*np.cos(theta)
         ybot = yc - a*np.sin(theta)
         xtop2 = xc + b*np.cos(theta2)
         ytop2 = yc + b*np.sin(theta2)
         xbot2 = xc - b*np.cos(theta2)
         ybot2 = yc - b*np.sin(theta2)
         mse = res[0] / np.sum(non_zero)
-        major = lambda x,y : (y - yc) - (slope_major * (x - xc))
-        minor = lambda x,y : (y - yc) - (slope_minor * (x - xc))
-        quant1 = (major(s_,u_) > 0) & (minor(s_,u_) < 0)
-        quant2 = (major(s_,u_) > 0) & (minor(s_,u_) > 0)
-        quant3 = (major(s_,u_) < 0) & (minor(s_,u_) > 0)
-        quant4 = (major(s_,u_) < 0) & (minor(s_,u_) < 0)
+        major = lambda x, y: (y - yc) - (slope_major * (x - xc))
+        minor = lambda x, y: (y - yc) - (slope_minor * (x - xc))
+        quant1 = (major(s_, u_) > 0) & (minor(s_, u_) < 0)
+        quant2 = (major(s_, u_) > 0) & (minor(s_, u_) > 0)
+        quant3 = (major(s_, u_) < 0) & (minor(s_, u_) > 0)
+        quant4 = (major(s_, u_) < 0) & (minor(s_, u_) < 0)
         if (np.sum(quant1 | quant4) < 10) or (np.sum(quant2 | quant3) < 10):
             count += 1
             continue
 
         if by_quantile:
-            axs[row, col].scatter(s_[quant1], u_[quant1], s=pointsize, c='tab:red', alpha=0.6)
-            axs[row, col].scatter(s_[quant2], u_[quant2], s=pointsize, c='tab:orange', alpha=0.6)
-            axs[row, col].scatter(s_[quant3], u_[quant3], s=pointsize, c='tab:green', alpha=0.6)
-            axs[row, col].scatter(s_[quant4], u_[quant4], s=pointsize, c='tab:blue', alpha=0.6)
+            axs[row, col].scatter(s_[quant1], u_[quant1], s=pointsize,
+                                  c='tab:red', alpha=0.6)
+            axs[row, col].scatter(s_[quant2], u_[quant2], s=pointsize,
+                                  c='tab:orange', alpha=0.6)
+            axs[row, col].scatter(s_[quant3], u_[quant3], s=pointsize,
+                                  c='tab:green', alpha=0.6)
+            axs[row, col].scatter(s_[quant4], u_[quant4], s=pointsize,
+                                  c='tab:blue', alpha=0.6)
         elif by_quantile_score:
             if 'quantile_scores' not in adata.layers:
-                raise ValueError('Please run multivelo.compute_quantile_scores first to compute quantile scores.')
-            axs[row, col].scatter(s_, u_, s=pointsize, c=adata[:,gene].layers['quantile_scores'], cmap='RdBu_r', alpha=0.7)
+                raise ValueError('Please run multivelo.compute_quantile_scores'
+                                 ' first to compute quantile scores.')
+            axs[row, col].scatter(s_, u_, s=pointsize,
+                                  c=adata[:, gene].layers['quantile_scores'],
+                                  cmap='RdBu_r', alpha=0.7)
         else:
             for i in range(len(types)):
                 filt = adata.obs[color_by] == types[i]
-                axs[row, col].scatter(s_[filt], u_[filt], s=pointsize, c=colors[i], alpha=0.7)
-        axs[row, col].contour(X_coord, Y_coord, Z_coord, levels=[0], colors=('r'), linewidths=linewidth, alpha=0.7)
+                axs[row, col].scatter(s_[filt], u_[filt], s=pointsize,
+                                      c=colors[i], alpha=0.7)
+        axs[row, col].contour(X_coord, Y_coord, Z_coord, levels=[0],
+                              colors=('r'), linewidths=linewidth, alpha=0.7)
         axs[row, col].scatter([xc], [yc], c='black', s=5, zorder=2)
         axs[row, col].scatter([0], [0], c='black', s=5, zorder=2)
-        axs[row, col].plot([xtop, xbot], [ytop, ybot], color='b', linestyle='dashed', linewidth=linewidth, alpha=0.7)
-        axs[row, col].plot([xtop2, xbot2], [ytop2, ybot2], color='g', linestyle='dashed', linewidth=linewidth, alpha=0.7)
+        axs[row, col].plot([xtop, xbot], [ytop, ybot], color='b',
+                           linestyle='dashed', linewidth=linewidth, alpha=0.7)
+        axs[row, col].plot([xtop2, xbot2], [ytop2, ybot2], color='g',
+                           linestyle='dashed', linewidth=linewidth, alpha=0.7)
 
         axs[row, col].set_title(f'{gene} {mse:.3g}')
         axs[row, col].set_xlabel('s')
         axs[row, col].set_ylabel('u')
-        common_range = [np.min([(-mean_s)/std_s, (-mean_u)/std_u])-(0.05*np.max(s)/std_s), np.max([(np.max(s)-mean_s)/std_s, (np.max(u)-mean_u)/std_u])+(0.05*np.max(s)/std_s)]
+        common_range = [(np.min([(-mean_s)/std_s, (-mean_u)/std_u])
+                        - (0.05*np.max(s)/std_s)),
+                        (np.max([(np.max(s)-mean_s)/std_s,
+                                 (np.max(u)-mean_u)/std_u])
+                        + (0.05*np.max(s)/std_s))]
         axs[row, col].set_xlim(common_range)
         axs[row, col].set_ylim(common_range)
         if not axis_on:
             axs[row, col].xaxis.set_ticks_position('none')
             axs[row, col].yaxis.set_ticks_position('none')
             axs[row, col].get_xaxis().set_visible(False)
             axs[row, col].get_yaxis().set_visible(False)
@@ -495,30 +677,32 @@
     if title is not None:
         fig.suptitle(title, fontsize=15)
     else:
         fig.suptitle('Ellipse Fit', fontsize=15)
     fig.tight_layout(rect=[0, 0.1, 1, 0.98])
 
 
-def compute_quantile_scores(adata, 
-                            verbose=True, 
-                            n_pcs=30, 
+def compute_quantile_scores(adata,
+                            verbose=True,
+                            n_pcs=30,
                             n_neighbors=30
                             ):
-    """Fit ellipses to unspliced and spliced phase portraits and compute quantile scores.
+    """Fit ellipses to unspliced and spliced phase portraits and compute
+        quantile scores.
 
-    This function fit ellipses to unspliced-spliced phase portraits. The cells are split into
-    four groups (quantiles) based on the axes of the ellipse. Then the function assigns each 
-    quantile a score: -3 for left, -1 for top, 1 for right, and 3 for bottom. These gene-specific
-    values are smoothed with a connectivities matirx. This is similar to the RNA velocity
-    gene time assignment.
-
-    In addition, a 2-bit tuple is assigned to each of the four quantiles, (0,0) for left,
-    (1,0) for top, (1,1) for right, and (0,1) for bottom. This is to mimic the distance 
-    relationship between quantiles.
+    This function fit ellipses to unspliced-spliced phase portraits. The cells
+    are split into four groups (quantiles) based on the axes of the ellipse.
+    Then the function assigns each quantile a score: -3 for left, -1 for top, 1
+    for right, and 3 for bottom. These gene-specific values are smoothed with a
+    connectivities matrix. This is similar to the RNA velocity gene time
+    assignment.
+
+    In addition, a 2-bit tuple is assigned to each of the four quantiles, (0,0)
+    for left, (1,0) for top, (1,1) for right, and (0,1) for bottom. This is to
+    mimic the distance relationship between quantiles.
 
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         RNA anndata object. Required fields: `Mu` and `Ms`.
     verbose: `bool` (default: `True`)
         Print the number of good ellipse fit based on some criteria.
@@ -544,145 +728,167 @@
     conn.setdiag(1)
     conn_norm = conn.multiply(1.0 / conn.sum(1)).tocsr()
 
     quantile_scores = np.zeros(adata.shape)
     quantile_scores_2bit = np.zeros((adata.shape[0], adata.shape[1], 2))
     quantile_gene = np.full(adata.n_vars, False)
     quality_gene_idx = []
-    for idx,gene in enumerate(adata.var_names):
-        u = np.array(adata[:,gene].layers['Mu'])
-        s = np.array(adata[:,gene].layers['Ms'])
-        non_zero = (u>0) & (s>0)
+    for idx, gene in enumerate(adata.var_names):
+        u = np.array(adata[:, gene].layers['Mu'])
+        s = np.array(adata[:, gene].layers['Ms'])
+        non_zero = (u > 0) & (s > 0)
         if np.sum(non_zero) < 10:
             continue
 
         mean_u, mean_s = np.mean(u[non_zero]), np.mean(s[non_zero])
         std_u, std_s = np.std(u[non_zero]), np.std(s[non_zero])
         u_ = (u - mean_u)/std_u
         s_ = (s - mean_s)/std_s
-        X = np.reshape(s_[non_zero], (-1,1))
-        Y = np.reshape(u_[non_zero], (-1,1))
+        X = np.reshape(s_[non_zero], (-1, 1))
+        Y = np.reshape(u_[non_zero], (-1, 1))
 
         # Ax^2 + Bxy + Cy^2 + Dx + Ey + 1 = 0
         A = np.hstack([X**2, X * Y, Y**2, X, Y])
         b = -np.ones_like(X)
-        x,res,_,_ = np.linalg.lstsq(A, b)
+        x, res, _, _ = np.linalg.lstsq(A, b)
         x = x.squeeze()
-        A,B,C,D,E = x
+        A, B, C, D, E = x
         good_fit = B**2 - 4*A*C < 0
-        theta = np.arctan(B/(A - C))/2 if x[0] > x[2] else np.pi/2 + np.arctan(B/(A - C))/2
+        theta = np.arctan(B/(A - C))/2 \
+            if x[0] > x[2] \
+            else np.pi/2 + np.arctan(B/(A - C))/2
         good_fit = good_fit & (theta < np.pi/2) & (theta > 0)
         if not good_fit:
             continue
 
         x_coord = np.linspace((-mean_s)/std_s, (np.max(s)-mean_s)/std_s, 500)
         y_coord = np.linspace((-mean_u)/std_u, (np.max(u)-mean_u)/std_u, 500)
         X_coord, Y_coord = np.meshgrid(x_coord, y_coord)
-        Z_coord = A * X_coord**2 + B * X_coord * Y_coord + C * Y_coord**2 + D * X_coord + E * Y_coord + 1
-        M0 = np.array([
-             A, B/2, D/2,
-             B/2, C, E/2,
-             D/2, E/2, 1,
-        ]).reshape(3, 3)
         M = np.array([
             A, B/2,
             B/2, C,
         ]).reshape(2, 2)
         l1, l2 = np.sort(np.linalg.eigvals(M))
         xc = (B*E - 2*C*D)/(4*A*C - B**2)
         yc = (B*D - 2*A*E)/(4*A*C - B**2)
         slope_major = np.tan(theta)
         theta2 = np.pi/2 + theta
         slope_minor = np.tan(theta2)
-        major = lambda x,y : (y - yc) - (slope_major * (x - xc))
-        minor = lambda x,y : (y - yc) - (slope_minor * (x - xc))
+        major = lambda x, y: (y - yc) - (slope_major * (x - xc))
+        minor = lambda x, y: (y - yc) - (slope_minor * (x - xc))
 
-        quant1 = (major(s_,u_) > 0) & (minor(s_,u_) < 0)
-        quant2 = (major(s_,u_) > 0) & (minor(s_,u_) > 0)
-        quant3 = (major(s_,u_) < 0) & (minor(s_,u_) > 0)
-        quant4 = (major(s_,u_) < 0) & (minor(s_,u_) < 0)
+        quant1 = (major(s_, u_) > 0) & (minor(s_, u_) < 0)
+        quant2 = (major(s_, u_) > 0) & (minor(s_, u_) > 0)
+        quant3 = (major(s_, u_) < 0) & (minor(s_, u_) > 0)
+        quant4 = (major(s_, u_) < 0) & (minor(s_, u_) < 0)
         if (np.sum(quant1 | quant4) < 10) or (np.sum(quant2 | quant3) < 10):
             continue
 
-        quantile_scores[:,idx:idx+1] = (-3.) * quant1 + (-1.) * quant2 + 1. * quant3 + 3. * quant4
-        quantile_scores_2bit[:,idx:idx+1,0] = 1. * (quant1 | quant2)
-        quantile_scores_2bit[:,idx:idx+1,1] = 1. * (quant2 | quant3)
+        quantile_scores[:, idx:idx+1] = ((-3.) * quant1 + (-1.) * quant2 + 1.
+                                         * quant3 + 3. * quant4)
+        quantile_scores_2bit[:, idx:idx+1, 0] = 1. * (quant1 | quant2)
+        quantile_scores_2bit[:, idx:idx+1, 1] = 1. * (quant2 | quant3)
         quality_gene_idx.append(idx)
 
     quantile_scores = csr_matrix.dot(conn_norm, quantile_scores)
-    quantile_scores_2bit[:,:,0] = csr_matrix.dot(conn_norm, quantile_scores_2bit[:,:,0])
-    quantile_scores_2bit[:,:,1] = csr_matrix.dot(conn_norm, quantile_scores_2bit[:,:,1])
+    quantile_scores_2bit[:, :, 0] = csr_matrix.dot(conn_norm,
+                                                   quantile_scores_2bit[:,
+                                                                        :, 0])
+    quantile_scores_2bit[:, :, 1] = csr_matrix.dot(conn_norm,
+                                                   quantile_scores_2bit[:,
+                                                                        :, 1])
     adata.layers['quantile_scores'] = quantile_scores
-    adata.layers['quantile_scores_1st_bit'] = quantile_scores_2bit[:,:,0]
-    adata.layers['quantile_scores_2nd_bit'] = quantile_scores_2bit[:,:,1]
+    adata.layers['quantile_scores_1st_bit'] = quantile_scores_2bit[:, :, 0]
+    adata.layers['quantile_scores_2nd_bit'] = quantile_scores_2bit[:, :, 1]
     quantile_gene[quality_gene_idx] = True
 
     if verbose:
         perc_good = np.sum(quantile_gene) / adata.n_vars * 100
-        print(f'{np.sum(quantile_gene)}/{adata.n_vars} - {perc_good:.3g}% genes have good ellipse fits')
+        print(f'{np.sum(quantile_gene)}/{adata.n_vars} - {perc_good:.3g}%'
+              'genes have good ellipse fits')
 
-    adata.obs['quantile_score_sum'] = np.sum(adata[:,quantile_gene].layers['quantile_scores'], axis=1)
+    adata.obs['quantile_score_sum'] = \
+        np.sum(adata[:, quantile_gene].layers['quantile_scores'], axis=1)
     adata.var['quantile_genes'] = quantile_gene
 
 
-def cluster_by_quantile(adata, 
-                        plot=False, 
-                        n_clusters=None, 
-                        affinity='euclidean', 
+def cluster_by_quantile(adata,
+                        plot=False,
+                        n_clusters=None,
+                        affinity='euclidean',
                         linkage='ward'
                         ):
     """Cluster genes based on 2-bit quantile scores.
 
-    This function cluster similar genes based on their 2-bit quantile score assignments from ellipse fit.
+    This function cluster similar genes based on their 2-bit quantile score
+    assignments from ellipse fit.
     Hierarchical cluster is done with `sklean.cluster.AgglomerativeClustering`.
 
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         RNA anndata object. Required fields: `Mu` and `Ms`.
     plot: `bool` (default: `False`)
         Plot the hierarchical clusters.
     n_clusters: `int` (default: None)
         The number of clusters to keep.
     affinity: `str` (default: `euclidean`)
-        Metric used to compute linkage. Passed to `sklean.cluster.AgglomerativeClustering`.
+        Metric used to compute linkage. Passed to
+        `sklean.cluster.AgglomerativeClustering`.
     linkage: `str` (default: `ward`)
-        Linkage criterion to use. Passed to `sklean.cluster.AgglomerativeClustering`.
+        Linkage criterion to use. Passed to
+        `sklean.cluster.AgglomerativeClustering`.
 
     Returns
     -------
     quantile_cluster: `.var`
         cluster assignments of genes based on quantiles
     """
     from sklearn.cluster import AgglomerativeClustering
     if 'quantile_scores_1st_bit' not in adata.layers.keys():
-        raise ValueError("Quantile scores not found. Please run compute_quantile_scores function first.")
+        raise ValueError("Quantile scores not found. Please run "
+                         "compute_quantile_scores function first.")
     quantile_gene = adata.var['quantile_genes']
     if plot or n_clusters is None:
-        cluster = AgglomerativeClustering(distance_threshold=0, n_clusters=None, affinity=affinity, linkage=linkage)
-        cluster = cluster.fit(np.vstack((adata[:,quantile_gene].layers['quantile_scores_1st_bit'], adata[:,quantile_gene].layers['quantile_scores_2nd_bit'])).transpose())
+        cluster = AgglomerativeClustering(distance_threshold=0,
+                                          n_clusters=None,
+                                          affinity=affinity,
+                                          linkage=linkage)
+        cluster = cluster.fit(np.vstack((adata[:, quantile_gene]
+                                         .layers['quantile_scores_1st_bit'],
+                                         adata[:, quantile_gene]
+                                         .layers['quantile_scores_2nd_bit']))
+                                .transpose())
 
         # https://scikit-learn.org/stable/auto_examples/cluster/plot_agglomerative_dendrogram.html
         def plot_dendrogram(model, **kwargs):
             from scipy.cluster.hierarchy import dendrogram
             counts = np.zeros(model.children_.shape[0])
             n_samples = len(model.labels_)
             for i, merge in enumerate(model.children_):
                 current_count = 0
                 for child_idx in merge:
                     if child_idx < n_samples:
                         current_count += 1
                     else:
                         current_count += counts[child_idx - n_samples]
                 counts[i] = current_count
-            linkage_matrix = np.column_stack([model.children_, model.distances_, counts]).astype(float)
+            linkage_matrix = np.column_stack([model.children_,
+                                              model.distances_,
+                                              counts]).astype(float)
             dendrogram(linkage_matrix, **kwargs)
 
         plot_dendrogram(cluster, truncate_mode='level', p=5, no_labels=True)
 
     if n_clusters is not None:
         n_clusters = int(n_clusters)
-        cluster = AgglomerativeClustering(n_clusters=n_clusters, affinity=affinity, linkage=linkage)
-        cluster = cluster.fit_predict(np.vstack((adata[:,quantile_gene].layers['quantile_scores_1st_bit'], adata[:,quantile_gene].layers['quantile_scores_2nd_bit'])).transpose())
+        cluster = AgglomerativeClustering(n_clusters=n_clusters,
+                                          affinity=affinity,
+                                          linkage=linkage)
+        cluster = cluster.fit_predict(np.vstack((adata[:, quantile_gene].layers
+                                                 ['quantile_scores_1st_bit'],
+                                                 adata[:, quantile_gene].layers
+                                                 ['quantile_scores_2nd_bit']))
+                                        .transpose())
         quantile_cluster = np.full(adata.n_vars, -1)
         quantile_cluster[quantile_gene] = cluster
         adata.var['quantile_cluster'] = quantile_cluster
```

### Comparing `multivelo-0.1.2/src/multivelo/dynamical_chrom_func.py` & `multivelo-0.1.3/src/multivelo/dynamical_chrom_func.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,247 +1,384 @@
 import os
 import numpy as np
 from numpy.linalg import norm
 import matplotlib.pyplot as plt
 from scipy import sparse
-from scipy.sparse import coo_matrix, csr_matrix, diags
+from scipy.sparse import coo_matrix
 from scipy.optimize import minimize
 from scipy.spatial import KDTree
 from sklearn.metrics import pairwise_distances
 from sklearn.mixture import GaussianMixture
-from anndata import AnnData
-import scanpy as sc
 from scanpy import Neighbors
 import scvelo as scv
 import pandas as pd
 import seaborn as sns
 from numba import jit
 from numba.typed import List
 from tqdm.auto import tqdm
-import ipywidgets
 from joblib import Parallel, delayed
 
+
 @jit(nopython=True, fastmath=True)
-def predict_exp(tau, 
-                c0, 
-                u0, 
-                s0, 
-                alpha_c, 
-                alpha, 
-                beta, 
-                gamma, 
-                scale_cc=1, 
-                pred_r=True, 
-                chrom_open=True, 
-                backward=False, 
+def predict_exp(tau,
+                c0,
+                u0,
+                s0,
+                alpha_c,
+                alpha,
+                beta,
+                gamma,
+                scale_cc=1,
+                pred_r=True,
+                chrom_open=True,
+                backward=False,
                 rna_only=False):
 
     if len(tau) == 0:
-        return np.empty((0,3))
+        return np.empty((0, 3))
     if backward:
         tau = -tau
-    res = np.empty((len(tau),3))
+    res = np.empty((len(tau), 3))
     eat = np.exp(-alpha_c * tau)
     ebt = np.exp(-beta * tau)
     egt = np.exp(-gamma * tau)
     if rna_only:
         kc = 1
         c0 = 1
     else:
         if chrom_open:
             kc = 1
         else:
             kc = 0
             alpha_c *= scale_cc
     const = (kc - c0) * alpha / (beta - alpha_c)
-    res[:,0] = kc - (kc - c0) * eat
+    res[:, 0] = kc - (kc - c0) * eat
     if pred_r:
-        res[:,1] = u0 * ebt + (alpha * kc / beta) * (1 - ebt)
-        res[:,1] += const * (ebt - eat)
+        res[:, 1] = u0 * ebt + (alpha * kc / beta) * (1 - ebt)
+        res[:, 1] += const * (ebt - eat)
 
-        res[:,2] = s0 * egt + (alpha * kc / gamma) * (1 - egt)
-        res[:,2] += (beta / (gamma - beta)) * ((alpha * kc / beta) - u0 - const) * (egt - ebt)
-        res[:,2] += (beta / (gamma - alpha_c)) * const * (egt - eat)
+        res[:, 2] = s0 * egt + (alpha * kc / gamma) * (1 - egt)
+        res[:, 2] += ((beta / (gamma - beta)) *
+                      ((alpha * kc / beta) - u0 - const) * (egt - ebt))
+        res[:, 2] += (beta / (gamma - alpha_c)) * const * (egt - eat)
     else:
-        res[:,1] = np.zeros(len(tau))
-        res[:,2] = np.zeros(len(tau))
+        res[:, 1] = np.zeros(len(tau))
+        res[:, 2] = np.zeros(len(tau))
     return res
 
 
 @jit(nopython=True, fastmath=True)
-def generate_exp(tau_list, 
-                 t_sw_array, 
-                 alpha_c, 
-                 alpha, 
-                 beta, 
-                 gamma, 
-                 scale_cc=1, 
-                 model=1, 
+def generate_exp(tau_list,
+                 t_sw_array,
+                 alpha_c,
+                 alpha,
+                 beta,
+                 gamma,
+                 scale_cc=1,
+                 model=1,
                  rna_only=False):
 
     if beta == alpha_c:
         beta += 1e-3
     if gamma == beta or gamma == alpha_c:
         gamma += 1e-3
     switch = len(t_sw_array)
     if switch >= 1:
         tau_sw1 = np.array([t_sw_array[0]])
         if switch >= 2:
             tau_sw2 = np.array([t_sw_array[1] - t_sw_array[0]])
             if switch == 3:
                 tau_sw3 = np.array([t_sw_array[2] - t_sw_array[1]])
-    exp_sw1, exp_sw2, exp_sw3 = np.empty((0,3)), np.empty((0,3)), np.empty((0,3))
+    exp_sw1, exp_sw2, exp_sw3 = (np.empty((0, 3)),
+                                 np.empty((0, 3)),
+                                 np.empty((0, 3)))
     if tau_list is None:
         if model == 0:
             if switch >= 1:
-                exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta, gamma, pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
+                exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta,
+                                      gamma, pred_r=False, scale_cc=scale_cc,
+                                      rna_only=rna_only)
                 if switch >= 2:
-                    exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, pred_r=False, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+                    exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0],
+                                          exp_sw1[0, 1], exp_sw1[0, 2],
+                                          alpha_c, alpha, beta, gamma,
+                                          pred_r=False, chrom_open=False,
+                                          scale_cc=scale_cc, rna_only=rna_only)
                     if switch >= 3:
-                        exp_sw3 = predict_exp(tau_sw3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, alpha, beta, gamma, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+                        exp_sw3 = predict_exp(tau_sw3, exp_sw2[0, 0],
+                                              exp_sw2[0, 1], exp_sw2[0, 2],
+                                              alpha_c, alpha, beta, gamma,
+                                              chrom_open=False,
+                                              scale_cc=scale_cc,
+                                              rna_only=rna_only)
         elif model == 1:
             if switch >= 1:
-                exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta, gamma, pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
+                exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta,
+                                      gamma, pred_r=False, scale_cc=scale_cc,
+                                      rna_only=rna_only)
                 if switch >= 2:
-                    exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, rna_only=rna_only)
+                    exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0],
+                                          exp_sw1[0, 1], exp_sw1[0, 2],
+                                          alpha_c, alpha, beta, gamma,
+                                          scale_cc=scale_cc, rna_only=rna_only)
                     if switch >= 3:
-                        exp_sw3 = predict_exp(tau_sw3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, alpha, beta, gamma, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+                        exp_sw3 = predict_exp(tau_sw3, exp_sw2[0, 0],
+                                              exp_sw2[0, 1], exp_sw2[0, 2],
+                                              alpha_c, alpha, beta, gamma,
+                                              chrom_open=False,
+                                              scale_cc=scale_cc,
+                                              rna_only=rna_only)
         elif model == 2:
             if switch >= 1:
-                exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta, gamma, pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
+                exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta,
+                                      gamma, pred_r=False, scale_cc=scale_cc,
+                                      rna_only=rna_only)
                 if switch >= 2:
-                    exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, rna_only=rna_only)
+                    exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0],
+                                          exp_sw1[0, 1], exp_sw1[0, 2],
+                                          alpha_c, alpha, beta, gamma,
+                                          scale_cc=scale_cc, rna_only=rna_only)
                     if switch >= 3:
-                        exp_sw3 = predict_exp(tau_sw3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, 0, beta, gamma, scale_cc=scale_cc, rna_only=rna_only)
-        return (np.empty((0,3)), np.empty((0,3)), np.empty((0,3)), np.empty((0,3))), (exp_sw1, exp_sw2, exp_sw3)
+                        exp_sw3 = predict_exp(tau_sw3, exp_sw2[0, 0],
+                                              exp_sw2[0, 1], exp_sw2[0, 2],
+                                              alpha_c, 0, beta, gamma,
+                                              scale_cc=scale_cc,
+                                              rna_only=rna_only)
+
+        return (np.empty((0, 3)), np.empty((0, 3)), np.empty((0, 3)),
+                np.empty((0, 3))), (exp_sw1, exp_sw2, exp_sw3)
 
     tau1 = tau_list[0]
     if switch >= 1:
         tau2 = tau_list[1]
         if switch >= 2:
             tau3 = tau_list[2]
             if switch == 3:
                 tau4 = tau_list[3]
-    exp1, exp2, exp3, exp4 = np.empty((0,3)), np.empty((0,3)), np.empty((0,3)), np.empty((0,3))
+    exp1, exp2, exp3, exp4 = (np.empty((0, 3)), np.empty((0, 3)),
+                              np.empty((0, 3)), np.empty((0, 3)))
     if model == 0:
-        exp1 = predict_exp(tau1, 0, 0, 0, alpha_c, alpha, beta, gamma, pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
+        exp1 = predict_exp(tau1, 0, 0, 0, alpha_c, alpha, beta, gamma,
+                           pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
         if switch >= 1:
-            exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta, gamma, pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
-            exp2 = predict_exp(tau2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, pred_r=False, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+            exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta,
+                                  gamma, pred_r=False, scale_cc=scale_cc,
+                                  rna_only=rna_only)
+            exp2 = predict_exp(tau2, exp_sw1[0, 0], exp_sw1[0, 1],
+                               exp_sw1[0, 2], alpha_c, alpha, beta, gamma,
+                               pred_r=False, chrom_open=False,
+                               scale_cc=scale_cc, rna_only=rna_only)
             if switch >= 2:
-                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, pred_r=False, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
-                exp3 = predict_exp(tau3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, alpha, beta, gamma, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                      exp_sw1[0, 2], alpha_c, alpha, beta,
+                                      gamma, pred_r=False, chrom_open=False,
+                                      scale_cc=scale_cc, rna_only=rna_only)
+                exp3 = predict_exp(tau3, exp_sw2[0, 0], exp_sw2[0, 1],
+                                   exp_sw2[0, 2], alpha_c, alpha, beta, gamma,
+                                   chrom_open=False, scale_cc=scale_cc,
+                                   rna_only=rna_only)
                 if switch == 3:
-                    exp_sw3 = predict_exp(tau_sw3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, alpha, beta, gamma, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
-                    exp4 = predict_exp(tau4, exp_sw3[0,0], exp_sw3[0,1], exp_sw3[0,2], alpha_c, 0, beta, gamma, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+                    exp_sw3 = predict_exp(tau_sw3, exp_sw2[0, 0],
+                                          exp_sw2[0, 1], exp_sw2[0, 2],
+                                          alpha_c, alpha, beta, gamma,
+                                          chrom_open=False, scale_cc=scale_cc,
+                                          rna_only=rna_only)
+                    exp4 = predict_exp(tau4, exp_sw3[0, 0], exp_sw3[0, 1],
+                                       exp_sw3[0, 2], alpha_c, 0, beta, gamma,
+                                       chrom_open=False, scale_cc=scale_cc,
+                                       rna_only=rna_only)
     elif model == 1:
-        exp1 = predict_exp(tau1, 0, 0, 0, alpha_c, alpha, beta, gamma, pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
+        exp1 = predict_exp(tau1, 0, 0, 0, alpha_c, alpha, beta, gamma,
+                           pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
         if switch >= 1:
-            exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta, gamma, pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
-            exp2 = predict_exp(tau2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, rna_only=rna_only)
+            exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta,
+                                  gamma, pred_r=False, scale_cc=scale_cc,
+                                  rna_only=rna_only)
+            exp2 = predict_exp(tau2, exp_sw1[0, 0], exp_sw1[0, 1],
+                               exp_sw1[0, 2], alpha_c, alpha, beta, gamma,
+                               scale_cc=scale_cc, rna_only=rna_only)
             if switch >= 2:
-                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, rna_only=rna_only)
-                exp3 = predict_exp(tau3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, alpha, beta, gamma, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                      exp_sw1[0, 2], alpha_c, alpha, beta,
+                                      gamma, scale_cc=scale_cc,
+                                      rna_only=rna_only)
+                exp3 = predict_exp(tau3, exp_sw2[0, 0], exp_sw2[0, 1],
+                                   exp_sw2[0, 2], alpha_c, alpha, beta, gamma,
+                                   chrom_open=False, scale_cc=scale_cc,
+                                   rna_only=rna_only)
                 if switch == 3:
-                    exp_sw3 = predict_exp(tau_sw3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, alpha, beta, gamma, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
-                    exp4 = predict_exp(tau4, exp_sw3[0,0], exp_sw3[0,1], exp_sw3[0,2], alpha_c, 0, beta, gamma, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+                    exp_sw3 = predict_exp(tau_sw3, exp_sw2[0, 0],
+                                          exp_sw2[0, 1], exp_sw2[0, 2],
+                                          alpha_c, alpha, beta, gamma,
+                                          chrom_open=False, scale_cc=scale_cc,
+                                          rna_only=rna_only)
+                    exp4 = predict_exp(tau4, exp_sw3[0, 0], exp_sw3[0, 1],
+                                       exp_sw3[0, 2], alpha_c, 0, beta, gamma,
+                                       chrom_open=False, scale_cc=scale_cc,
+                                       rna_only=rna_only)
     elif model == 2:
-        exp1 = predict_exp(tau1, 0, 0, 0, alpha_c, alpha, beta, gamma, pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
+        exp1 = predict_exp(tau1, 0, 0, 0, alpha_c, alpha, beta, gamma,
+                           pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
         if switch >= 1:
-            exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta, gamma, pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
-            exp2 = predict_exp(tau2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, rna_only=rna_only)
+            exp_sw1 = predict_exp(tau_sw1, 0, 0, 0, alpha_c, alpha, beta,
+                                  gamma, pred_r=False, scale_cc=scale_cc,
+                                  rna_only=rna_only)
+            exp2 = predict_exp(tau2, exp_sw1[0, 0], exp_sw1[0, 1],
+                               exp_sw1[0, 2], alpha_c, alpha, beta, gamma,
+                               scale_cc=scale_cc, rna_only=rna_only)
             if switch >= 2:
-                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, rna_only=rna_only)
-                exp3 = predict_exp(tau3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, 0, beta, gamma, scale_cc=scale_cc, rna_only=rna_only)
+                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                      exp_sw1[0, 2], alpha_c, alpha, beta,
+                                      gamma, scale_cc=scale_cc,
+                                      rna_only=rna_only)
+                exp3 = predict_exp(tau3, exp_sw2[0, 0], exp_sw2[0, 1],
+                                   exp_sw2[0, 2], alpha_c, 0, beta, gamma,
+                                   scale_cc=scale_cc, rna_only=rna_only)
                 if switch == 3:
-                    exp_sw3 = predict_exp(tau_sw3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, 0, beta, gamma, scale_cc=scale_cc, rna_only=rna_only)
-                    exp4 = predict_exp(tau4, exp_sw3[0,0], exp_sw3[0,1], exp_sw3[0,2], alpha_c, 0, beta, gamma, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+                    exp_sw3 = predict_exp(tau_sw3, exp_sw2[0, 0],
+                                          exp_sw2[0, 1], exp_sw2[0, 2],
+                                          alpha_c, 0, beta, gamma,
+                                          scale_cc=scale_cc, rna_only=rna_only)
+                    exp4 = predict_exp(tau4, exp_sw3[0, 0], exp_sw3[0, 1],
+                                       exp_sw3[0, 2], alpha_c, 0, beta, gamma,
+                                       chrom_open=False, scale_cc=scale_cc,
+                                       rna_only=rna_only)
     return (exp1, exp2, exp3, exp4), (exp_sw1, exp_sw2, exp_sw3)
 
 
 @jit(nopython=True, fastmath=True)
-def generate_exp_backward(tau_list, t_sw_array, alpha_c, alpha, beta, gamma, scale_cc=1, model=1):
+def generate_exp_backward(tau_list, t_sw_array, alpha_c, alpha, beta, gamma,
+                          scale_cc=1, model=1):
     if beta == alpha_c:
         beta += 1e-3
     if gamma == beta or gamma == alpha_c:
         gamma += 1e-3
     switch = len(t_sw_array)
     if switch >= 1:
         tau_sw1 = np.array([t_sw_array[0]])
         if switch >= 2:
             tau_sw2 = np.array([t_sw_array[1] - t_sw_array[0]])
     if t is None:
         if model == 0:
-            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
-            exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
+            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta,
+                                  gamma, scale_cc=scale_cc, chrom_open=False,
+                                  backward=True)
+            exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                  exp_sw1[0, 2], alpha_c, alpha, beta, gamma,
+                                  scale_cc=scale_cc, chrom_open=False,
+                                  backward=True)
         elif model == 1:
-            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
-            exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
+            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta,
+                                  gamma, scale_cc=scale_cc, chrom_open=False,
+                                  backward=True)
+            exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                  exp_sw1[0, 2], alpha_c, alpha, beta, gamma,
+                                  scale_cc=scale_cc, chrom_open=False,
+                                  backward=True)
         elif model == 2:
-            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
-            exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, 0, beta, gamma, scale_cc=scale_cc, backward=True)
-        return (np.empty((0,0)), np.empty((0,0)), np.empty((0,0))), (exp_sw1, exp_sw2)
+            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta,
+                                  gamma, scale_cc=scale_cc, chrom_open=False,
+                                  backward=True)
+            exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                  exp_sw1[0, 2], alpha_c, 0, beta, gamma,
+                                  scale_cc=scale_cc, backward=True)
+        return (np.empty((0, 0)),
+                np.empty((0, 0)),
+                np.empty((0, 0))), (exp_sw1, exp_sw2)
 
     tau1 = tau_list[0]
     if switch >= 1:
         tau2 = tau_list[1]
         if switch >= 2:
             tau3 = tau_list[2]
 
-    exp1, exp2, exp3 = np.empty((0,3)), np.empty((0,3)), np.empty((0,3))
+    exp1, exp2, exp3 = np.empty((0, 3)), np.empty((0, 3)), np.empty((0, 3))
     if model == 0:
-        exp1 = predict_exp(tau1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
+        exp1 = predict_exp(tau1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma,
+                           scale_cc=scale_cc, chrom_open=False, backward=True)
         if switch >= 1:
-            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
-            exp2 = predict_exp(tau2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
+            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta,
+                                  gamma, scale_cc=scale_cc, chrom_open=False,
+                                  backward=True)
+            exp2 = predict_exp(tau2, exp_sw1[0, 0], exp_sw1[0, 1],
+                               exp_sw1[0, 2], alpha_c, alpha, beta, gamma,
+                               scale_cc=scale_cc, chrom_open=False,
+                               backward=True)
             if switch >= 2:
-                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
-                exp3 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
+                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                      exp_sw1[0, 2], alpha_c, alpha, beta,
+                                      gamma, scale_cc=scale_cc,
+                                      chrom_open=False, backward=True)
+                exp3 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                   exp_sw1[0, 2], alpha_c, alpha, beta, gamma,
+                                   scale_cc=scale_cc, chrom_open=False,
+                                   backward=True)
     elif model == 1:
-        exp1 = predict_exp(tau1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
+        exp1 = predict_exp(tau1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma,
+                           scale_cc=scale_cc, chrom_open=False, backward=True)
         if switch >= 1:
-            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
-            exp2 = predict_exp(tau2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
+            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta,
+                                  gamma, scale_cc=scale_cc, chrom_open=False,
+                                  backward=True)
+            exp2 = predict_exp(tau2, exp_sw1[0, 0], exp_sw1[0, 1],
+                               exp_sw1[0, 2], alpha_c, alpha, beta, gamma,
+                               scale_cc=scale_cc, chrom_open=False,
+                               backward=True)
             if switch >= 2:
-                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
-                exp3 = predict_exp(tau3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, backward=True)
+                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                      exp_sw1[0, 2], alpha_c, alpha, beta,
+                                      gamma, scale_cc=scale_cc,
+                                      chrom_open=False, backward=True)
+                exp3 = predict_exp(tau3, exp_sw2[0, 0], exp_sw2[0, 1],
+                                   exp_sw2[0, 2], alpha_c, alpha, beta, gamma,
+                                   scale_cc=scale_cc, backward=True)
     elif model == 2:
-        exp1 = predict_exp(tau1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
+        exp1 = predict_exp(tau1, 1e-3, 1e-3, 1e-3, alpha_c, 0, beta, gamma,
+                           scale_cc=scale_cc, chrom_open=False, backward=True)
         if switch >= 1:
-            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, alpha, beta, gamma, scale_cc=scale_cc, chrom_open=False, backward=True)
-            exp2 = predict_exp(tau2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, 0, beta, gamma, scale_cc=scale_cc, backward=True)
+            exp_sw1 = predict_exp(tau_sw1, 1e-3, 1e-3, 1e-3, alpha_c, alpha,
+                                  beta, gamma, scale_cc=scale_cc,
+                                  chrom_open=False, backward=True)
+            exp2 = predict_exp(tau2, exp_sw1[0, 0], exp_sw1[0, 1],
+                               exp_sw1[0, 2], alpha_c, 0, beta, gamma,
+                               scale_cc=scale_cc, backward=True)
             if switch >= 2:
-                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0,0], exp_sw1[0,1], exp_sw1[0,2], alpha_c, 0, beta, gamma, scale_cc=scale_cc, backward=True)
-                exp3 = predict_exp(tau3, exp_sw2[0,0], exp_sw2[0,1], exp_sw2[0,2], alpha_c, alpha, beta, gamma, scale_cc=scale_cc, backward=True)
+                exp_sw2 = predict_exp(tau_sw2, exp_sw1[0, 0], exp_sw1[0, 1],
+                                      exp_sw1[0, 2], alpha_c, 0, beta, gamma,
+                                      scale_cc=scale_cc, backward=True)
+                exp3 = predict_exp(tau3, exp_sw2[0, 0], exp_sw2[0, 1],
+                                   exp_sw2[0, 2], alpha_c, alpha, beta, gamma,
+                                   scale_cc=scale_cc, backward=True)
     return (exp1, exp2, exp3), (exp_sw1, exp_sw2)
 
 
 @jit(nopython=True, fastmath=True)
 def ss_exp(alpha_c, alpha, beta, gamma, pred_r=True, chrom_open=True):
-    res = np.empty((1,3))
+    res = np.empty((1, 3))
     if not chrom_open:
-        res[0,0] = 0
-        res[0,1] = 0
-        res[0,2] = 0
+        res[0, 0] = 0
+        res[0, 1] = 0
+        res[0, 2] = 0
     else:
-        res[0,0] = 1
+        res[0, 0] = 1
         if pred_r:
-            res[0,1] = alpha / beta
-            res[0,2] = alpha / gamma
+            res[0, 1] = alpha / beta
+            res[0, 2] = alpha / gamma
         else:
-            res[0,1] = 0
-            res[0,2] = 0
+            res[0, 1] = 0
+            res[0, 2] = 0
     return res
 
 
 @jit(nopython=True, fastmath=True)
 def compute_ss_exp(alpha_c, alpha, beta, gamma, model=0):
     if model == 0:
         ss1 = ss_exp(alpha_c, alpha, beta, gamma, pred_r=False)
-        ss2 = ss_exp(alpha_c, alpha, beta, gamma, pred_r=False, chrom_open=False)
+        ss2 = ss_exp(alpha_c, alpha, beta, gamma, pred_r=False,
+                     chrom_open=False)
         ss3 = ss_exp(alpha_c, alpha, beta, gamma, chrom_open=False)
         ss4 = ss_exp(alpha_c, 0, beta, gamma, chrom_open=False)
     elif model == 1:
         ss1 = ss_exp(alpha_c, alpha, beta, gamma, pred_r=False)
         ss2 = ss_exp(alpha_c, alpha, beta, gamma)
         ss3 = ss_exp(alpha_c, alpha, beta, gamma, chrom_open=False)
         ss4 = ss_exp(alpha_c, 0, beta, gamma, chrom_open=False)
@@ -250,138 +387,154 @@
         ss2 = ss_exp(alpha_c, alpha, beta, gamma)
         ss3 = ss_exp(alpha_c, 0, beta, gamma)
         ss4 = ss_exp(alpha_c, 0, beta, gamma, chrom_open=False)
     return np.vstack((ss1, ss2, ss3, ss4))
 
 
 @jit(nopython=True, fastmath=True)
-def velocity_equations(c, u, s, alpha_c, alpha, beta, gamma, scale_cc=1, pred_r=True, chrom_open=True, rna_only=False):
+def velocity_equations(c, u, s, alpha_c, alpha, beta, gamma, scale_cc=1,
+                       pred_r=True, chrom_open=True, rna_only=False):
     if rna_only:
         c = np.full(len(u), 1.0)
     if not chrom_open:
         alpha_c *= scale_cc
         if pred_r:
             return -alpha_c * c, alpha * c - beta * u, beta * u - gamma * s
         else:
             return -alpha_c * c, np.zeros(len(u)), np.zeros(len(u))
     else:
         if pred_r:
-            return alpha_c - alpha_c * c, alpha * c - beta * u, beta * u - gamma * s
+            return (alpha_c - alpha_c * c), (alpha * c - beta * u), (beta * u
+                                                                     - gamma
+                                                                     * s)
         else:
             return alpha_c - alpha_c * c, np.zeros(len(u)), np.zeros(len(u))
 
 
 @jit(nopython=True, fastmath=True)
-def compute_velocity(t, 
-                     t_sw_array, 
-                     state, 
-                     alpha_c, 
-                     alpha, 
-                     beta, 
-                     gamma, 
-                     rescale_c, 
-                     rescale_u, 
-                     scale_cc=1, 
-                     model=1, 
-                     total_h=20, 
+def compute_velocity(t,
+                     t_sw_array,
+                     state,
+                     alpha_c,
+                     alpha,
+                     beta,
+                     gamma,
+                     rescale_c,
+                     rescale_u,
+                     scale_cc=1,
+                     model=1,
+                     total_h=20,
                      rna_only=False):
 
     if state is None:
-        state0 = t<=t_sw_array[0]
-        state1 = (t_sw_array[0]<t) & (t<=t_sw_array[1])
-        state2 = (t_sw_array[1]<t) & (t<=t_sw_array[2])
-        state3 = t_sw_array[2]<t
+        state0 = t <= t_sw_array[0]
+        state1 = (t_sw_array[0] < t) & (t <= t_sw_array[1])
+        state2 = (t_sw_array[1] < t) & (t <= t_sw_array[2])
+        state3 = t_sw_array[2] < t
     else:
         state0 = np.equal(state, 0)
         state1 = np.equal(state, 1)
         state2 = np.equal(state, 2)
         state3 = np.equal(state, 3)
 
     tau1 = t[state0]
     tau2 = t[state1] - t_sw_array[0]
     tau3 = t[state2] - t_sw_array[1]
     tau4 = t[state3] - t_sw_array[2]
     tau_list = [tau1, tau2, tau3, tau4]
     switch = np.sum(t_sw_array < total_h)
     typed_tau_list = List()
     [typed_tau_list.append(x) for x in tau_list]
-    exp_list, exp_sw_list = generate_exp(typed_tau_list, 
-                                         t_sw_array[:switch], 
-                                         alpha_c, 
-                                         alpha, 
-                                         beta, 
-                                         gamma, 
-                                         model=model, 
-                                         scale_cc=scale_cc, 
+    exp_list, exp_sw_list = generate_exp(typed_tau_list,
+                                         t_sw_array[:switch],
+                                         alpha_c,
+                                         alpha,
+                                         beta,
+                                         gamma,
+                                         model=model,
+                                         scale_cc=scale_cc,
                                          rna_only=rna_only)
 
     c = np.empty(len(t))
     u = np.empty(len(t))
     s = np.empty(len(t))
-    for i,ii in enumerate([state0, state1, state2, state3]):
+    for i, ii in enumerate([state0, state1, state2, state3]):
         if np.any(ii):
-            c[ii] = exp_list[i][:,0]
-            u[ii] = exp_list[i][:,1]
-            s[ii] = exp_list[i][:,2]
+            c[ii] = exp_list[i][:, 0]
+            u[ii] = exp_list[i][:, 1]
+            s[ii] = exp_list[i][:, 2]
 
     vc_vec = np.zeros(len(u))
     vu_vec = np.zeros(len(u))
     vs_vec = np.zeros(len(u))
 
     if model == 0:
         if np.any(state0):
-            vc_vec[state0], vu_vec[state0], vs_vec[state0] = velocity_equations(c[state0], u[state0], s[state0], 
-                                                                                alpha_c, alpha, beta, gamma, 
-                                                                                pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state0], vu_vec[state0], vs_vec[state0] = \
+                velocity_equations(c[state0], u[state0], s[state0], alpha_c,
+                                   alpha, beta, gamma, pred_r=False,
+                                   scale_cc=scale_cc, rna_only=rna_only)
         if np.any(state1):
-            vc_vec[state1], vu_vec[state1], vs_vec[state1] = velocity_equations(c[state1], u[state1], s[state1], 
-                                                                                alpha_c, alpha, beta, gamma, 
-                                                                                pred_r=False, chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state1], vu_vec[state1], vs_vec[state1] = \
+                velocity_equations(c[state1], u[state1], s[state1], alpha_c,
+                                   alpha, beta, gamma, pred_r=False,
+                                   chrom_open=False, scale_cc=scale_cc,
+                                   rna_only=rna_only)
         if np.any(state2):
-            vc_vec[state2], vu_vec[state2], vs_vec[state2] = velocity_equations(c[state2], u[state2], s[state2], 
-                                                                                alpha_c, alpha, beta, gamma, 
-                                                                                chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state2], vu_vec[state2], vs_vec[state2] = \
+                velocity_equations(c[state2], u[state2], s[state2], alpha_c,
+                                   alpha, beta, gamma, chrom_open=False,
+                                   scale_cc=scale_cc, rna_only=rna_only)
         if np.any(state3):
-            vc_vec[state3], vu_vec[state3], vs_vec[state3] = velocity_equations(c[state3], u[state3], s[state3], 
-                                                                                alpha_c, 0, beta, gamma, 
-                                                                                chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state3], vu_vec[state3], vs_vec[state3] = \
+                velocity_equations(c[state3], u[state3], s[state3], alpha_c, 0,
+                                   beta, gamma, chrom_open=False,
+                                   scale_cc=scale_cc, rna_only=rna_only)
     elif model == 1:
         if np.any(state0):
-            vc_vec[state0], vu_vec[state0], vs_vec[state0] = velocity_equations(c[state0], u[state0], s[state0], 
-                                                                                alpha_c, alpha, beta, gamma, 
-                                                                                pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state0], vu_vec[state0], vs_vec[state0] = \
+                velocity_equations(c[state0], u[state0], s[state0], alpha_c,
+                                   alpha, beta, gamma, pred_r=False,
+                                   scale_cc=scale_cc, rna_only=rna_only)
         if np.any(state1):
-            vc_vec[state1], vu_vec[state1], vs_vec[state1] = velocity_equations(c[state1], u[state1], s[state1], 
-                                                                                alpha_c, alpha, beta, gamma, 
-                                                                                scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state1], vu_vec[state1], vs_vec[state1] = \
+                velocity_equations(c[state1], u[state1], s[state1], alpha_c,
+                                   alpha, beta, gamma, scale_cc=scale_cc,
+                                   rna_only=rna_only)
         if np.any(state2):
-            vc_vec[state2], vu_vec[state2], vs_vec[state2] = velocity_equations(c[state2], u[state2], s[state2], 
-                                                                                alpha_c, alpha, beta, gamma, 
-                                                                                chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state2], vu_vec[state2], vs_vec[state2] = \
+                velocity_equations(c[state2], u[state2], s[state2], alpha_c,
+                                   alpha, beta, gamma, chrom_open=False,
+                                   scale_cc=scale_cc, rna_only=rna_only)
         if np.any(state3):
-            vc_vec[state3], vu_vec[state3], vs_vec[state3] = velocity_equations(c[state3], u[state3], s[state3], 
-                                                                                alpha_c, 0, beta, gamma, 
-                                                                                chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state3], vu_vec[state3], vs_vec[state3] = \
+                velocity_equations(c[state3], u[state3], s[state3], alpha_c, 0,
+                                   beta, gamma, chrom_open=False,
+                                   scale_cc=scale_cc, rna_only=rna_only)
     elif model == 2:
         if np.any(state0):
-            vc_vec[state0], vu_vec[state0], vs_vec[state0] = velocity_equations(c[state0], u[state0], s[state0], 
-                                                                                alpha_c, alpha, beta, gamma, 
-                                                                                pred_r=False, scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state0], vu_vec[state0], vs_vec[state0] = \
+                velocity_equations(c[state0], u[state0], s[state0], alpha_c,
+                                   alpha, beta, gamma, pred_r=False,
+                                   scale_cc=scale_cc, rna_only=rna_only)
         if np.any(state1):
-            vc_vec[state1], vu_vec[state1], vs_vec[state1] = velocity_equations(c[state1], u[state1], s[state1], 
-                                                                                alpha_c, alpha, beta, gamma, 
-                                                                                scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state1], vu_vec[state1], vs_vec[state1] = \
+                velocity_equations(c[state1], u[state1], s[state1], alpha_c,
+                                   alpha, beta, gamma, scale_cc=scale_cc,
+                                   rna_only=rna_only)
         if np.any(state2):
-            vc_vec[state2], vu_vec[state2], vs_vec[state2] = velocity_equations(c[state2], u[state2], s[state2], 
-                                                                                alpha_c, 0, beta, gamma, 
-                                                                                scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state2], vu_vec[state2], vs_vec[state2] = \
+                velocity_equations(c[state2], u[state2], s[state2], alpha_c,
+                                   0, beta, gamma, scale_cc=scale_cc,
+                                   rna_only=rna_only)
         if np.any(state3):
-            vc_vec[state3], vu_vec[state3], vs_vec[state3] = velocity_equations(c[state3], u[state3], s[state3], 
-                                                                                alpha_c, 0, beta, gamma, 
-                                                                                chrom_open=False, scale_cc=scale_cc, rna_only=rna_only)
+            vc_vec[state3], vu_vec[state3], vs_vec[state3] = \
+                velocity_equations(c[state3], u[state3], s[state3], alpha_c, 0,
+                                   beta, gamma, chrom_open=False,
+                                   scale_cc=scale_cc, rna_only=rna_only)
     return vc_vec * rescale_c, vu_vec * rescale_u, vs_vec
 
 
 def log_valid(x):
     return np.log(np.clip(x, 1e-3, 1 - 1e-3))
 
 
@@ -391,26 +544,28 @@
     u_inf = alpha / beta
     if beta > gamma:
         b_new = beta / (gamma - beta)
         s_inf = alpha / gamma
         s_inf_new = s_inf - b_new * u_inf
         s_new = s - b_new * u
         s0_new = s0 - b_new * u0
-        tau = -1.0 / gamma * log_valid((s_new - s_inf_new) / (s0_new - s_inf_new))
+        tau = -1.0 / gamma * log_valid((s_new - s_inf_new) /
+                                       (s0_new - s_inf_new))
     else:
         tau = -1.0 / beta * log_valid((u - u_inf) / (u0 - u_inf))
     return tau
 
 
-def anchor_points(t_sw_array, total_h=20, t=1000, mode='uniform', return_time=False):
+def anchor_points(t_sw_array, total_h=20, t=1000, mode='uniform',
+                  return_time=False):
     t_ = np.linspace(0, total_h, t)
-    tau1 = t_[t_<=t_sw_array[0]]
-    tau2 = t_[(t_sw_array[0]<t_) & (t_<=t_sw_array[1])] - t_sw_array[0]
-    tau3 = t_[(t_sw_array[1]<t_) & (t_<=t_sw_array[2])] - t_sw_array[1]
-    tau4 = t_[t_sw_array[2]<t_] - t_sw_array[2]
+    tau1 = t_[t_ <= t_sw_array[0]]
+    tau2 = t_[(t_sw_array[0] < t_) & (t_ <= t_sw_array[1])] - t_sw_array[0]
+    tau3 = t_[(t_sw_array[1] < t_) & (t_ <= t_sw_array[2])] - t_sw_array[1]
+    tau4 = t_[t_sw_array[2] < t_] - t_sw_array[2]
 
     if mode == 'log':
         if len(tau1) > 0:
             tau1 = np.expm1(tau1)
             tau1 = tau1 / np.max(tau1) * (t_sw_array[0])
         if len(tau2) > 0:
             tau2 = np.expm1(tau2)
@@ -438,118 +593,126 @@
             for i in range(X.shape[1]):
                 tmp = X[a, i] - Y[b, i]
                 val += tmp**2
             res[a, b] = val
     return res
 
 
-def calculate_dist_and_time(c, u, s, 
-                            t_sw_array, 
-                            alpha_c, alpha, beta, gamma, 
-                            rescale_c, rescale_u, 
-                            scale_cc=1, 
-                            scale_factor=None, 
-                            model=1, 
-                            conn=None, 
-                            t=1000, k=1, 
-                            direction='complete', 
-                            total_h=20, 
+def calculate_dist_and_time(c, u, s,
+                            t_sw_array,
+                            alpha_c, alpha, beta, gamma,
+                            rescale_c, rescale_u,
+                            scale_cc=1,
+                            scale_factor=None,
+                            model=1,
+                            conn=None,
+                            t=1000, k=1,
+                            direction='complete',
+                            total_h=20,
                             rna_only=False,
                             penalize_gap=True,
                             all_cells=True):
 
     n = len(u)
     if scale_factor is None:
         scale_factor = np.array([np.std(c), np.std(u), np.std(s)])
     tau_list = anchor_points(t_sw_array, total_h, t)
     switch = np.sum(t_sw_array < total_h)
     typed_tau_list = List()
     [typed_tau_list.append(x) for x in tau_list]
-    exp_list, exp_sw_list = generate_exp(typed_tau_list, 
-                                         t_sw_array[:switch], 
-                                         alpha_c, 
-                                         alpha, 
-                                         beta, 
-                                         gamma, 
-                                         model=model, 
-                                         scale_cc=scale_cc, 
+    exp_list, exp_sw_list = generate_exp(typed_tau_list,
+                                         t_sw_array[:switch],
+                                         alpha_c,
+                                         alpha,
+                                         beta,
+                                         gamma,
+                                         model=model,
+                                         scale_cc=scale_cc,
                                          rna_only=rna_only)
     rescale_factor = np.array([rescale_c, rescale_u, 1.0])
     exp_list = [x*rescale_factor for x in exp_list]
     exp_sw_list = [x*rescale_factor for x in exp_sw_list]
     max_c = 0
     max_u = 0
     max_s = 0
     if rna_only:
-        exp_mat = np.hstack((np.reshape(u, (-1,1)), np.reshape(s, (-1,1)))) / scale_factor[1:]
+        exp_mat = (np.hstack((np.reshape(u, (-1, 1)), np.reshape(s, (-1, 1))))
+                   / scale_factor[1:])
     else:
-        exp_mat = np.hstack((np.reshape(c, (-1,1)), np.reshape(u, (-1,1)), np.reshape(s, (-1,1)))) / scale_factor
+        exp_mat = np.hstack((np.reshape(c, (-1, 1)), np.reshape(u, (-1, 1)),
+                             np.reshape(s, (-1, 1)))) / scale_factor
 
     dists = np.full((n, 4), np.inf)
     taus = np.zeros((n, 4), dtype=u.dtype)
     ts = np.zeros((n, 4), dtype=u.dtype)
     anchor_exp, anchor_t = None, None
 
     for i in range(switch+1):
         if not all_cells:
-            max_ci = np.max(exp_list[i][:,0]) if exp_list[i].shape[0] > 0 else 0
+            max_ci = (np.max(exp_list[i][:, 0]) if exp_list[i].shape[0] > 0
+                      else 0)
             max_c = max_ci if max_ci > max_c else max_c
-        max_ui = np.max(exp_list[i][:,1]) if exp_list[i].shape[0] > 0 else 0
+        max_ui = np.max(exp_list[i][:, 1]) if exp_list[i].shape[0] > 0 else 0
         max_u = max_ui if max_ui > max_u else max_u
-        max_si = np.max(exp_list[i][:,2]) if exp_list[i].shape[0] > 0 else 0
+        max_si = np.max(exp_list[i][:, 2]) if exp_list[i].shape[0] > 0 else 0
         max_s = max_si if max_si > max_s else max_s
 
         skip_phase = False
         if direction == 'off':
-            if (model in [1,2]) and (i < 2):
+            if (model in [1, 2]) and (i < 2):
                 skip_phase = True
         elif direction == 'on':
-            if (model in [1,2]) and (i >= 2):
+            if (model in [1, 2]) and (i >= 2):
                 skip_phase = True
         if rna_only and i == 0:
             skip_phase = True
 
         if not skip_phase:
             if rna_only:
-                tmp = exp_list[i][:,1:] / scale_factor[1:]
+                tmp = exp_list[i][:, 1:] / scale_factor[1:]
             else:
                 tmp = exp_list[i] / scale_factor
             if anchor_exp is None:
                 anchor_exp = exp_list[i]
-                anchor_t = tau_list[i] + t_sw_array[i-1] if i >= 1 else tau_list[i]
+                anchor_t = (tau_list[i] + t_sw_array[i-1] if i >= 1
+                            else tau_list[i])
             else:
                 anchor_exp = np.vstack((anchor_exp, exp_list[i]))
-                anchor_t = np.hstack((anchor_t, tau_list[i] + t_sw_array[i-1] if i >= 1 else tau_list[i]))
+                anchor_t = np.hstack((anchor_t, tau_list[i] + t_sw_array[i-1]
+                                      if i >= 1 else tau_list[i]))
 
             if not all_cells:
-                anchor_dist = np.diff(tmp, axis=0, prepend=np.zeros((1,2)) if rna_only else np.zeros((1,3)))
+                anchor_dist = np.diff(tmp, axis=0, prepend=np.zeros((1, 2))
+                                      if rna_only else np.zeros((1, 3)))
                 anchor_dist = np.sqrt((anchor_dist**2).sum(axis=1))
-                remove_cand = anchor_dist < (0.01*np.max(exp_mat[1]) if rna_only else 0.01*np.max(exp_mat[2]))
-                step_idx = np.arange(0,len(anchor_dist),1) % 3 > 0
+                remove_cand = anchor_dist < (0.01*np.max(exp_mat[1])
+                                             if rna_only
+                                             else 0.01*np.max(exp_mat[2]))
+                step_idx = np.arange(0, len(anchor_dist), 1) % 3 > 0
                 remove_cand &= step_idx
                 keep_idx = np.where(~remove_cand)[0]
-                tmp = tmp[keep_idx,:]
+                tmp = tmp[keep_idx, :]
 
             tree = KDTree(tmp)
             dd, ii = tree.query(exp_mat, k=k)
             dd = dd**2
             if k > 1:
                 dd = np.mean(dd, axis=1)
             if conn is not None:
                 dd = conn.dot(dd)
-            dists[:,i] = dd
+            dists[:, i] = dd
 
             if not all_cells:
                 ii = keep_idx[ii]
             if k == 1:
-                taus[:,i] = tau_list[i][ii]
+                taus[:, i] = tau_list[i][ii]
             else:
                 for j in range(n):
-                    taus[j,i] = tau_list[i][ii[j,:]]
-            ts[:,i] = taus[:,i] + t_sw_array[i-1] if i >= 1 else taus[:,i]
+                    taus[j, i] = tau_list[i][ii[j, :]]
+            ts[:, i] = taus[:, i] + t_sw_array[i-1] if i >= 1 else taus[:, i]
 
     min_dist = np.min(dists, axis=1)
     state_pred = np.argmin(dists, axis=1)
     t_pred = ts[np.arange(n), state_pred]
 
     anchor_t1_list = []
     anchor_t2_list = []
@@ -559,75 +722,82 @@
         t_sorted = np.sort(t_pred)
         dt = np.diff(t_sorted, prepend=0)
         gap_thresh = 3*np.percentile(dt, 99)
         idx = np.where(dt > gap_thresh)[0]
         for i in idx:
             t1 = t_sorted[i-1] if i > 0 else 0
             t2 = t_sorted[i]
-            anchor_t1 = anchor_exp[np.argmin(np.abs(anchor_t - t1)),:]
-            anchor_t2 = anchor_exp[np.argmin(np.abs(anchor_t - t2)),:]
+            anchor_t1 = anchor_exp[np.argmin(np.abs(anchor_t - t1)), :]
+            anchor_t2 = anchor_exp[np.argmin(np.abs(anchor_t - t2)), :]
             if all_cells:
                 anchor_t1_list.append(np.ravel(anchor_t1))
                 anchor_t2_list.append(np.ravel(anchor_t2))
             if not all_cells:
                 for j in range(1, switch):
-                    crit1 = (t1 > t_sw_array[j-1]) and (t2 > t_sw_array[j-1]) and (t1 <= t_sw_array[j]) and (t2 <= t_sw_array[j])
-                    crit2 = (np.abs(anchor_t1[2] - exp_sw_list[j][0,2]) < 0.02 * max_s) and (np.abs(anchor_t2[2] - exp_sw_list[j][0,2]) < 0.01 * max_s)
-                    crit3 = (np.abs(anchor_t1[1] - exp_sw_list[j][0,1]) < 0.02 * max_u) and (np.abs(anchor_t2[1] - exp_sw_list[j][0,1]) < 0.01 * max_u)
-                    crit4 = (np.abs(anchor_t1[0] - exp_sw_list[j][0,0]) < 0.02 * max_c) and (np.abs(anchor_t2[0] - exp_sw_list[j][0,0]) < 0.01 * max_c)
+                    crit1 = ((t1 > t_sw_array[j-1]) and (t2 > t_sw_array[j-1])
+                             and (t1 <= t_sw_array[j])
+                             and (t2 <= t_sw_array[j]))
+                    crit2 = ((np.abs(anchor_t1[2] - exp_sw_list[j][0, 2])
+                             < 0.02 * max_s) and
+                             (np.abs(anchor_t2[2] - exp_sw_list[j][0, 2])
+                             < 0.01 * max_s))
+                    crit3 = ((np.abs(anchor_t1[1] - exp_sw_list[j][0, 1])
+                             < 0.02 * max_u) and
+                             (np.abs(anchor_t2[1] - exp_sw_list[j][0, 1])
+                             < 0.01 * max_u))
+                    crit4 = ((np.abs(anchor_t1[0] - exp_sw_list[j][0, 0])
+                             < 0.02 * max_c) and
+                             (np.abs(anchor_t2[0] - exp_sw_list[j][0, 0])
+                             < 0.01 * max_c))
                     if crit1 and crit2 and crit3 and crit4:
                         t_sw_adjust[j] += t2 - t1
             if penalize_gap:
-                dist_gap = np.sum(((anchor_t1[1:] - anchor_t2[1:]) / scale_factor[1:])**2)
+                dist_gap = np.sum(((anchor_t1[1:] - anchor_t2[1:]) /
+                                   scale_factor[1:])**2)
                 idx_to_adjust = t_pred >= t2
                 t_sw_array_ = np.append(t_sw_array, total_h)
                 state_to_adjust = np.where(t_sw_array_ > t2)[0]
                 dists[np.ix_(idx_to_adjust, state_to_adjust)] += dist_gap
         min_dist = np.min(dists, axis=1)
         state_pred = np.argmin(dists, axis=1)
         if all_cells:
             t_pred = ts[np.arange(n), state_pred]
 
-    #state23 = np.equal(state_pred, 2) | np.equal(state_pred, 3)
-    #if np.any(state23) and (np.sum(dists[state23, 1]) + np.sum(min_dist[~state23]) < 1.1 * np.sum(min_dist)):
-        #state_pred[state23] = 1
-        #min_dist[state23] = dists[state23, 1]
-        #if all_cells:
-            #t_pred = ts[np.arange(n), state_pred]
-
     if all_cells:
         exp_ss_mat = compute_ss_exp(alpha_c, alpha, beta, gamma, model=model)
         if rna_only:
-            exp_ss_mat[:,0] = 1
-        dists_ss = pairwise_distance_square(exp_mat, exp_ss_mat * rescale_factor / scale_factor)
+            exp_ss_mat[:, 0] = 1
+        dists_ss = pairwise_distance_square(exp_mat, exp_ss_mat *
+                                            rescale_factor / scale_factor)
 
-        reach_ss = np.full((n,4), False)
+        reach_ss = np.full((n, 4), False)
         for i in range(n):
             for j in range(4):
-                if min_dist[i] > dists_ss[i,j]:
-                    reach_ss[i,j] = True
+                if min_dist[i] > dists_ss[i, j]:
+                    reach_ss[i, j] = True
         late_phase = np.full(n, -1)
         for i in range(3):
             late_phase[np.abs(t_pred - t_sw_array[i]) < 0.1] = i
-        return min_dist, t_pred, state_pred, reach_ss, late_phase, max_u, max_s, anchor_t1_list, anchor_t2_list
+        return min_dist, t_pred, state_pred, reach_ss, late_phase, max_u, \
+            max_s, anchor_t1_list, anchor_t2_list
     else:
         return min_dist, state_pred, max_u, max_s, t_sw_adjust
 
 
-#@jit(nopython=True, fastmath=True)
-def compute_likelihood(c, u, s, 
-                       t_sw_array, 
-                       alpha_c, alpha, beta, gamma, 
-                       rescale_c, rescale_u, 
-                       t_pred, 
-                       state_pred, 
-                       scale_cc=1, 
-                       scale_factor=None, 
-                       model=1, 
-                       weight=None, 
+# @jit(nopython=True, fastmath=True)
+def compute_likelihood(c, u, s,
+                       t_sw_array,
+                       alpha_c, alpha, beta, gamma,
+                       rescale_c, rescale_u,
+                       t_pred,
+                       state_pred,
+                       scale_cc=1,
+                       scale_factor=None,
+                       model=1,
+                       weight=None,
                        total_h=20,
                        rna_only=False):
 
     if weight is None:
         weight = np.full(c.shape, True)
     c_ = c[weight]
     u_ = u[weight]
@@ -642,96 +812,92 @@
     tau2 = t_pred_[state_pred_ == 1] - t_sw_array[0]
     tau3 = t_pred_[state_pred_ == 2] - t_sw_array[1]
     tau4 = t_pred_[state_pred_ == 3] - t_sw_array[2]
     tau_list = [tau1, tau2, tau3, tau4]
     switch = np.sum(t_sw_array < total_h)
     typed_tau_list = List()
     [typed_tau_list.append(x) for x in tau_list]
-    exp_list, _ = generate_exp(typed_tau_list, 
-                               t_sw_array[:switch], 
-                               alpha_c, 
-                               alpha, 
-                               beta, 
-                               gamma, 
-                               model=model, 
-                               scale_cc=scale_cc, 
+    exp_list, _ = generate_exp(typed_tau_list,
+                               t_sw_array[:switch],
+                               alpha_c,
+                               alpha,
+                               beta,
+                               gamma,
+                               model=model,
+                               scale_cc=scale_cc,
                                rna_only=rna_only)
     rescale_factor = np.array([rescale_c, rescale_u, 1.0])
     exp_list = [x*rescale_factor*scale_factor for x in exp_list]
-    exp_mat = np.hstack((np.reshape(c_, (-1,1)), np.reshape(u_, (-1,1)), np.reshape(s_, (-1,1)))) * scale_factor
-    diffs = np.empty((n,3), dtype=u.dtype)
+    exp_mat = np.hstack((np.reshape(c_, (-1, 1)), np.reshape(u_, (-1, 1)),
+                         np.reshape(s_, (-1, 1)))) * scale_factor
+    diffs = np.empty((n, 3), dtype=u.dtype)
     likelihood_c = 0
     likelihood_u = 0
     likelihood_s = 0
     ssd_c, var_c = 0, 0
     for i in range(switch+1):
         index = state_pred_ == i
         if np.sum(index) > 0:
-            diff = exp_mat[index,:] - exp_list[i]
+            diff = exp_mat[index, :] - exp_list[i]
             diffs[index, :] = diff
     if rna_only:
-        diff_u = np.ravel(diffs[:,0])
-        diff_s = np.ravel(diffs[:,1])
+        diff_u = np.ravel(diffs[:, 0])
+        diff_s = np.ravel(diffs[:, 1])
         dist_us = diff_u ** 2 + diff_s ** 2
         var_us = np.var(np.sign(diff_s) * np.sqrt(dist_us))
-        nll = 0.5 * np.log(2 * np.pi * var_us) + 0.5 / n / var_us * np.sum(dist_us)
+        nll = (0.5 * np.log(2 * np.pi * var_us) + 0.5 / n /
+               var_us * np.sum(dist_us))
     else:
-        diff_c = np.ravel(diffs[:,0])
-        diff_u = np.ravel(diffs[:,1])
-        diff_s = np.ravel(diffs[:,2])
-        #dist_cu = diff_c ** 2 + diff_u ** 2
-        #dist_us = diff_u ** 2 + diff_s ** 2
-        #dist_cs = diff_c ** 2 + diff_s ** 2
-        #var_cu = 0.5 * np.var(np.sign(diff_u) * np.sqrt(dist_cu))
-        #var_us = 0.5 * np.var(np.sign(diff_s) * np.sqrt(dist_us))
-        #var_cs = 0.5 * np.var(np.sign(diff_c) * np.sqrt(dist_cs))
-        #nll = 0.5 * np.log(2 * np.pi * var_cu) + 0.25 / n / var_cu * np.sum(dist_cu)
-        #nll += 0.5 * np.log(2 * np.pi * var_us) + 0.25 / n / var_us * np.sum(dist_us)
-        #nll += 0.5 * np.log(2 * np.pi * var_cs) + 0.25 / n / var_cs * np.sum(dist_cs)
+        diff_c = np.ravel(diffs[:, 0])
+        diff_u = np.ravel(diffs[:, 1])
+        diff_s = np.ravel(diffs[:, 2])
         dist_c = diff_c ** 2
         dist_u = diff_u ** 2
         dist_s = diff_s ** 2
         var_c = np.var(diff_c)
         var_u = np.var(diff_u)
         var_s = np.var(diff_s)
         ssd_c = np.sum(dist_c)
-        nll_c = 0.5 * np.log(2 * np.pi * var_c) + 0.5 / n / var_c * np.sum(dist_c)
-        nll_u = 0.5 * np.log(2 * np.pi * var_u) + 0.5 / n / var_u * np.sum(dist_u)
-        nll_s = 0.5 * np.log(2 * np.pi * var_s) + 0.5 / n / var_s * np.sum(dist_s)
+        nll_c = (0.5 * np.log(2 * np.pi * var_c) + 0.5 / n /
+                 var_c * np.sum(dist_c))
+        nll_u = (0.5 * np.log(2 * np.pi * var_u) + 0.5 / n /
+                 var_u * np.sum(dist_u))
+        nll_s = (0.5 * np.log(2 * np.pi * var_s) + 0.5 / n /
+                 var_s * np.sum(dist_s))
         nll = nll_c + nll_u + nll_s
         likelihood_c = np.exp(-nll_c)
         likelihood_u = np.exp(-nll_u)
         likelihood_s = np.exp(-nll_s)
     likelihood = np.exp(-nll)
     return likelihood, likelihood_c, ssd_c, var_c, likelihood_u, likelihood_s
 
 
 class ChromatinDynamical:
-    def __init__(self, c, u, s, 
-                 gene=None, 
-                 model=None, 
-                 max_iter=10, 
-                 init_mode="grid", 
-                 local_std=None, 
-                 embed_coord=None, 
-                 connectivities=None, 
-                 verbose=False, 
-                 plot=False, 
-                 save_plot=False, 
-                 plot_dir=None, 
-                 fit_args=None, 
-                 partial=None, 
-                 direction=None, 
-                 rna_only=False, 
-                 fit_decoupling=True, 
-                 extra_color=None, 
-                 rescale_u=None, 
-                 alpha=None, 
-                 beta=None, 
-                 gamma=None, 
+    def __init__(self, c, u, s,
+                 gene=None,
+                 model=None,
+                 max_iter=10,
+                 init_mode="grid",
+                 local_std=None,
+                 embed_coord=None,
+                 connectivities=None,
+                 verbose=False,
+                 plot=False,
+                 save_plot=False,
+                 plot_dir=None,
+                 fit_args=None,
+                 partial=None,
+                 direction=None,
+                 rna_only=False,
+                 fit_decoupling=True,
+                 extra_color=None,
+                 rescale_u=None,
+                 alpha=None,
+                 beta=None,
+                 gamma=None,
                  t_=None
                  ):
 
         self.gene = gene
         self.local_std = local_std
         self.conn = connectivities
         self.verbose = verbose
@@ -748,16 +914,16 @@
         self.outlier = np.clip(fit_args['outlier'], 80, 100)
         self.model = int(model) if isinstance(model, float) else model
         self.model_ = None
         if self.model == 0 and self.init_mode == 'invert':
             self.init_mode = 'grid'
 
         # plot parameters
-        self.plot= plot
-        self.save_plot=save_plot
+        self.plot = plot
+        self.save_plot = save_plot
         self.extra_color = extra_color
         self.fig_size = fit_args['fig_size']
         self.point_size = fit_args['point_size']
         if plot_dir is None:
             self.plot_path = 'rna_plots' if self.rna_only else 'plots'
         else:
             self.plot_path = plot_dir
@@ -774,52 +940,68 @@
         if sparse.issparse(s):
             s = s.A
         self.c_all = np.ravel(np.array(c, dtype=np.float64))
         self.u_all = np.ravel(np.array(u, dtype=np.float64))
         self.s_all = np.ravel(np.array(s, dtype=np.float64))
 
         # adjust offset
-        self.offset_c, self.offset_u, self.offset_s = np.min(self.c_all), np.min(self.u_all), np.min(self.s_all)
+        self.offset_c, self.offset_u, self.offset_s = np.min(self.c_all), \
+            np.min(self.u_all), np.min(self.s_all)
         self.offset_c = 0 if self.rna_only else self.offset_c
         self.c_all -= self.offset_c
         self.u_all -= self.offset_u
         self.s_all -= self.offset_s
         # remove zero counts
-        self.non_zero = np.ravel(self.c_all > 0) | np.ravel(self.u_all > 0) | np.ravel(self.s_all > 0)
+        self.non_zero = (np.ravel(self.c_all > 0) | np.ravel(self.u_all > 0) |
+                         np.ravel(self.s_all > 0))
         # remove outliers
-        self.non_outlier = np.ravel(self.c_all <= np.percentile(self.c_all, self.outlier))
-        self.non_outlier &= np.ravel(self.u_all <= np.percentile(self.u_all, self.outlier))
-        self.non_outlier &= np.ravel(self.s_all <= np.percentile(self.s_all, self.outlier))
+        self.non_outlier = np.ravel(self.c_all <= np.percentile(self.c_all,
+                                                                self.outlier))
+        self.non_outlier &= np.ravel(self.u_all <= np.percentile(self.u_all,
+                                                                 self.outlier))
+        self.non_outlier &= np.ravel(self.s_all <= np.percentile(self.s_all,
+                                                                 self.outlier))
         self.c = self.c_all[self.non_zero & self.non_outlier]
         self.u = self.u_all[self.non_zero & self.non_outlier]
         self.s = self.s_all[self.non_zero & self.non_outlier]
         self.low_quality = len(self.u) < 10
         # scale modalities
-        self.std_c, self.std_u, self.std_s = np.std(self.c_all) if not self.rna_only else 1.0, np.std(self.u_all), np.std(self.s_all)
+        self.std_c, self.std_u, self.std_s = (np.std(self.c_all)
+                                              if not self.rna_only
+                                              else 1.0, np.std(self.u_all),
+                                              np.std(self.s_all))
         if self.std_u == 0 or self.std_s == 0:
             self.low_quality = True
-        self.scale_c, self.scale_u, self.scale_s = np.max(self.c_all) if not self.rna_only else 1.0, self.std_u/self.std_s, 1.0
+        self.scale_c, self.scale_u, self.scale_s = np.max(self.c_all) \
+            if not self.rna_only else 1.0, self.std_u/self.std_s, 1.0
         self.c_all /= self.scale_c
         self.u_all /= self.scale_u
         self.s_all /= self.scale_s
         self.c /= self.scale_c
         self.u /= self.scale_u
         self.s /= self.scale_s
-        self.scale_factor = np.array([np.std(self.c_all)/self.std_s/self.weight_c, 1.0, 1.0])
+        self.scale_factor = np.array([np.std(self.c_all) / self.std_s /
+                                      self.weight_c, 1.0, 1.0])
         self.scale_factor[0] = 1 if self.rna_only else self.scale_factor[0]
         self.max_u, self.max_s = np.max(self.u), np.max(self.s)
         if self.conn is not None:
-            self.conn_sub = self.conn[np.ix_(self.non_zero & self.non_outlier, self.non_zero & self.non_outlier)]
+            self.conn_sub = self.conn[np.ix_(self.non_zero & self.non_outlier,
+                                             self.non_zero & self.non_outlier)]
         else:
             self.conn_sub = None
         if self.verbose >= 2:
-            print(f'{len(self.u)} cells passed filter and will be used to compute trajectories.')
-        self.known_pars = True if None not in [rescale_u, alpha, beta, gamma, t_] else False
+            print(f'{len(self.u)} cells passed filter and will be used to '
+                  'compute trajectories.')
+        self.known_pars = (True
+                           if None not in [rescale_u, alpha, beta, gamma, t_]
+                           else False)
         if self.known_pars and self.verbose >= 1:
-            print(f'known parameters for gene {self.gene} are scaling={rescale_u}, alpha={alpha}, beta={beta}, gamma={gamma}, t_={t_}.')
+            print(f'known parameters for gene {self.gene} are '
+                  'scaling={rescale_u}, alpha={alpha}, beta={beta},'
+                  ' gamma={gamma}, t_={t_}.')
 
         # 4 rate parameters
         self.alpha_c = 0.1
         self.alpha = alpha if alpha is not None else 0.0
         self.beta = beta if beta is not None else 0.0
         self.gamma = gamma if gamma is not None else 0.0
         # 3 possible switch time points
@@ -827,15 +1009,15 @@
         self.t_sw_2 = t_+0.1 if t_ is not None else 0.0
         self.t_sw_3 = 20.0 if t_ is not None else 0.0
         # 2 rescale factors
         self.rescale_c = 1.0
         self.rescale_u = rescale_u if rescale_u is not None else 1.0
         self.rates = None
         self.t_sw_array = None
-        self.fit_rescale = True if rescale_u == None else False
+        self.fit_rescale = True if rescale_u is None else False
         self.params = None
 
         # other parameters or results
         self.t = None
         self.state = None
         self.loss = [np.inf]
         self.likelihood = -1.0
@@ -843,15 +1025,16 @@
         self.ssd_c, self.var_c = 0, 0
         self.scale_cc = 1.0
         self.fitting_flag_ = 0
         self.velocity = None
         self.anchor_t1_list, self.anchor_t2_list = None, None
         self.anchor_exp = None
         self.anchor_exp_sw = None
-        self.anchor_min_idx, self.anchor_max_idx, self.anchor_velo_min_idx, self.anchor_velo_max_idx = None, None, None, None
+        self.anchor_min_idx, self.anchor_max_idx, self.anchor_velo_min_idx, \
+            self.anchor_velo_max_idx = None, None, None, None
         self.anchor_velo = None
         self.c0 = self.u0 = self.s0 = 0.0
         self.realign_ratio = 1.0
         self.partial = False
         self.direction = 'complete'
         self.steady_state_func = None
 
@@ -861,156 +1044,168 @@
         self.cur_state_pred = None
         self.cur_t_sw_adjust = None
 
         # partial checking and model examination
         determine_model = model is None
         if partial is None and direction is None:
             if embed_coord is not None:
-                self.embed_coord = embed_coord[self.non_zero & self.non_outlier]
+                self.embed_coord = embed_coord[self.non_zero &
+                                               self.non_outlier]
             else:
                 self.embed_coord = None
             self.check_partial_trajectory(determine_model=determine_model)
         elif direction is not None:
             self.direction = direction
             if direction in ['on', 'off']:
                 self.partial = True
             else:
                 self.partial = False
-            self.check_partial_trajectory(fit_gmm=False, fit_slope=False, determine_model=determine_model)
+            self.check_partial_trajectory(fit_gmm=False, fit_slope=False,
+                                          determine_model=determine_model)
         elif partial is not None:
             self.partial = partial
-            self.check_partial_trajectory(fit_gmm=False, determine_model=determine_model)
+            self.check_partial_trajectory(fit_gmm=False,
+                                          determine_model=determine_model)
         else:
-            self.check_partial_trajectory(fit_gmm=False, fit_slope=False, determine_model=determine_model)
+            self.check_partial_trajectory(fit_gmm=False, fit_slope=False,
+                                          determine_model=determine_model)
 
         # intialize steady state parameters
         if not self.known_pars and not self.low_quality:
-            self.initialize_steady_state_params(model_mismatch=self.model != self.model_)
+            self.initialize_steady_state_params(model_mismatch=self.model
+                                                != self.model_)
         if self.known_pars:
-            self.params = np.array([self.t_sw_1, 
-                                    self.t_sw_2-self.t_sw_1, 
-                                    self.t_sw_3-self.t_sw_2, 
-                                    self.alpha_c, 
-                                    self.alpha, 
-                                    self.beta, 
-                                    self.gamma, 
-                                    self.scale_cc, 
-                                    self.rescale_c, 
+            self.params = np.array([self.t_sw_1,
+                                    self.t_sw_2-self.t_sw_1,
+                                    self.t_sw_3-self.t_sw_2,
+                                    self.alpha_c,
+                                    self.alpha,
+                                    self.beta,
+                                    self.gamma,
+                                    self.scale_cc,
+                                    self.rescale_c,
                                     self.rescale_u])
 
-
-    def check_partial_trajectory(self, fit_gmm=True, fit_slope=True, determine_model=True):
-        w_non_zero = (self.c >= 0.1 * np.max(self.c)) & (self.u >= 0.1 * np.max(self.u)) & (self.s >= 0.1 * np.max(self.s))
+    def check_partial_trajectory(self, fit_gmm=True, fit_slope=True,
+                                 determine_model=True):
+        w_non_zero = ((self.c >= 0.1 * np.max(self.c)) &
+                      (self.u >= 0.1 * np.max(self.u)) &
+                      (self.s >= 0.1 * np.max(self.s)))
         u_non_zero = self.u[w_non_zero]
         s_non_zero = self.s[w_non_zero]
         if len(u_non_zero) < 10:
             self.low_quality = True
             return
 
         # GMM
-        w_low = (np.percentile(s_non_zero, 30) <= s_non_zero) & (s_non_zero <= np.percentile(s_non_zero, 40))
+        w_low = ((np.percentile(s_non_zero, 30) <= s_non_zero) &
+                 (s_non_zero <= np.percentile(s_non_zero, 40)))
         if np.sum(w_low) < 10:
             fit_gmm = False
             self.partial = True
         if self.verbose >= 2:
             if self.local_std is None:
-                print('Warning: local standard deviation not provided. Skipping GMM..')
+                print('Warning: local standard deviation not provided. '
+                      'Skipping GMM..')
             if self.embed_coord is None:
-                print('Warning: embedded coordinates not provided. Skipping GMM..')
-        if fit_gmm and self.local_std is not None and self.embed_coord is not None:
-            pdist = pairwise_distances(self.embed_coord[w_non_zero,:][w_low,:])
-            dists = np.ravel(pdist[np.triu_indices_from(pdist, k=1)]).reshape(-1, 1)
-            model = GaussianMixture(n_components=2, covariance_type='tied', random_state=2021).fit(dists)
+                print('Warning: embedded coordinates not provided. '
+                      'Skipping GMM..')
+        if (fit_gmm and self.local_std is not None and self.embed_coord
+                is not None):
+
+            pdist = pairwise_distances(
+                self.embed_coord[w_non_zero, :][w_low, :])
+            dists = (np.ravel(pdist[np.triu_indices_from(pdist, k=1)])
+                     .reshape(-1, 1))
+            model = GaussianMixture(n_components=2, covariance_type='tied',
+                                    random_state=2021).fit(dists)
             mean_diff = np.abs(model.means_[1][0] - model.means_[0][0])
             criterion1 = mean_diff > self.local_std / self.tm
             if self.verbose >= 2:
-                print(f'GMM: difference between means = {mean_diff}, threshold = {self.local_std / self.tm}.')
+                print(f'GMM: difference between means = {mean_diff}, '
+                      'threshold = {self.local_std / self.tm}.')
             criterion2 = np.all(model.weights_[1] > 0.2 / self.tm)
             if self.verbose >= 2:
-                print(f'GMM: weight of the second Gaussian = {model.weights_[1]}.')
+                print('GMM: weight of the second Gaussian ='
+                      f' {model.weights_[1]}.')
             if criterion1 and criterion2:
                 self.partial = False
             else:
                 self.partial = True
             if self.verbose >= 2:
                 print(f'GMM decides {"" if self.partial else "not "}partial.')
 
         # steady-state slope
         wu = self.u >= np.percentile(u_non_zero, 95)
         ws = self.s >= np.percentile(s_non_zero, 95)
         ss_u = self.u[wu | ws]
         ss_s = self.s[wu | ws]
-        if np.all(ss_u==0) or np.all(ss_s==0):
+        if np.all(ss_u == 0) or np.all(ss_s == 0):
             self.low_quality = True
             return
         gamma = np.dot(ss_u, ss_s) / np.dot(ss_s, ss_s)
         self.steady_state_func = lambda x: gamma*x
 
         # thickness of phase portrait
         u_norm = u_non_zero / np.max(self.u)
         s_norm = s_non_zero / np.max(self.s)
-        exp = np.hstack((np.reshape(u_norm, (-1,1)), np.reshape(s_norm, (-1,1))))
+        exp = np.hstack((np.reshape(u_norm, (-1, 1)),
+                         np.reshape(s_norm, (-1, 1))))
         U, S, Vh = np.linalg.svd(exp)
         self.thickness = S[1]
 
         # slope-based direction decision
-        with np.errstate(divide='ignore',invalid='ignore'):
+        with np.errstate(divide='ignore', invalid='ignore'):
             slope = self.u / self.s
         non_nan = ~np.isnan(slope)
         slope = slope[non_nan]
         on = slope >= gamma
         off = slope < gamma
         if len(ss_u) < 10 or len(u_non_zero) < 10:
             fit_slope = False
             self.direction = 'complete'
         if fit_slope:
-            #on_ratio = np.sum(on) / len(slope)
-            #off_ratio = np.sum(off) / len(slope)
-            #on_dist = np.sum((slope[on] - gamma)**2)
-            #off_dist = np.sum((gamma - slope[off])**2)
-            #if on_ratio > 0.7:
-                #self.direction = 'on'
-                #self.partial = True
-            #elif off_ratio > 0.7:
-                #self.direction = 'off'
-                #self.partial = True
             slope_ = u_non_zero / s_non_zero
             on_ = slope_ >= gamma
             off_ = slope_ < gamma
             on_dist = np.sum((u_non_zero[on_] - gamma * s_non_zero[on_])**2)
             off_dist = np.sum((gamma * s_non_zero[off_] - u_non_zero[off_])**2)
             if self.verbose >= 2:
-                print(f'Slope: SSE on induction phase = {on_dist}, SSE on repression phase = {off_dist}.')
+                print(f'Slope: SSE on induction phase = {on_dist},'
+                      f' SSE on repression phase = {off_dist}.')
             if self.thickness < 1.5 / np.sqrt(self.tm):
                 narrow = True
             else:
                 narrow = False
             if self.verbose >= 2:
-                print(f'Thickness of trajectory = {self.thickness}. Trajectory is {"narrow" if narrow else "normal"}.')
+                print(f'Thickness of trajectory = {self.thickness}. '
+                      'Trajectory is {"narrow" if narrow else "normal"}.')
             if on_dist > 10 * self.tm**2 * off_dist:
                 self.direction = 'on'
                 self.partial = True
             elif off_dist > 10 * self.tm**2 * on_dist:
                 self.direction = 'off'
                 self.partial = True
             else:
-                if self.partial == True:
+                if self.partial is True:
                     if on_dist > 3 * self.tm * off_dist:
                         self.direction = 'on'
                     elif off_dist > 3 * self.tm * on_dist:
                         self.direction = 'off'
                     else:
                         if narrow:
                             self.direction = 'on'
                         else:
                             self.direction = 'complete'
                             self.partial = False
                 else:
                     if narrow:
-                        self.direction = 'off' if off_dist > 2 * self.tm * on_dist else 'on'
+                        self.direction = ('off'
+                                          if off_dist > 2 * self.tm * on_dist
+                                          else 'on')
                         self.partial = True
                     else:
                         self.direction = 'complete'
 
         # model pre-determination
         if self.direction == 'on':
             self.model_ = 1
@@ -1021,15 +1216,15 @@
             c_high = c_high[non_nan]
             if np.sum(c_high) < 10:
                 c_high = self.c >= np.mean(self.c) + np.std(self.c)
                 c_high = c_high[non_nan]
             if np.sum(c_high) < 10:
                 c_high = self.c >= np.percentile(self.c, 90)
                 c_high = c_high[non_nan]
-            if np.sum(self.c[non_nan][c_high]==0) > 0.5*np.sum(c_high):
+            if np.sum(self.c[non_nan][c_high] == 0) > 0.5*np.sum(c_high):
                 self.low_quality = True
                 return
             c_high_on = np.sum(c_high & on)
             c_high_off = np.sum(c_high & off)
             if c_high_on > c_high_off:
                 self.model_ = 1
             else:
@@ -1040,25 +1235,24 @@
         if self.verbose >= 1 and not self.known_pars:
             if fit_gmm or fit_slope:
                 print(f'predicted partial trajectory: {self.partial}')
                 print(f'predicted trajectory direction: {self.direction}')
             if determine_model:
                 print(f'predicted model: {self.model}')
 
-
     def initialize_steady_state_params(self, model_mismatch=False):
         self.scale_cc = 1.0
         self.rescale_c = 1.0
         # estimate rescale factor for u
         s_norm = self.s / self.max_s
         u_mid = (self.u >= 0.4 * self.max_u) & (self.u <= 0.6 * self.max_u)
         if np.sum(u_mid) < 10:
             self.rescale_u = self.thickness / 5
         else:
-            s_low, s_high = np.percentile(s_norm[u_mid], [2,98])
+            s_low, s_high = np.percentile(s_norm[u_mid], [2, 98])
             s_dist = s_high - s_low
             self.rescale_u = s_dist
         if self.rescale_u == 0:
             self.low_quality = True
             return
 
         c = self.c / self.rescale_c
@@ -1068,175 +1262,192 @@
         # some extreme values
         wu = u >= np.percentile(u, 97)
         ws = s >= np.percentile(s, 97)
         ss_u = u[wu | ws]
         ss_s = s[wu | ws]
         c_upper = np.mean(c[wu | ws])
 
-        c_high = c >= np.mean(c)# + np.std(c)
+        c_high = c >= np.mean(c)
         # _r stands for repressed state
         c0_r = np.mean(c[c_high])
         u0_r = np.mean(ss_u)
         s0_r = np.mean(ss_s)
         if c0_r < c_upper:
             c0_r = c_upper + 0.1
 
         # adjust chromatin level for reasonable initialization
-        if model_mismatch or not self.fit_decoupling: 
+        if model_mismatch or not self.fit_decoupling:
             c_indu = np.mean(c[self.u > self.steady_state_func(self.s)])
             c_repr = np.mean(c[self.u < self.steady_state_func(self.s)])
             if c_indu == np.nan or c_repr == np.nan:
                 self.low_quality = True
                 return
             c0_r = np.mean(c[c >= np.min([c_indu, c_repr])])
 
         # initialize rates
         self.alpha_c = 0.1
         self.beta = 1.0
         self.gamma = np.dot(ss_u, ss_s) / np.dot(ss_s, ss_s)
         alpha = u0_r
         self.alpha = u0_r
-        self.rates = np.array([self.alpha_c, self.alpha, self.beta, self.gamma])
+        self.rates = np.array([self.alpha_c, self.alpha, self.beta,
+                               self.gamma])
 
         # RNA-only
         if self.rna_only:
             t_sw_1 = 0.1
             t_sw_3 = 20.0
             if self.init_mode == 'grid':
-                for t_sw_2 in np.arange(2, 20, 4, dtype=np.float64): # 2,6,10,14,18
-                    self.update(params, initialize=True, adjust_time=False, plot=False)
+                # arange returns sequence [2,6,10,14,18]
+                for t_sw_2 in np.arange(2, 20, 4, dtype=np.float64):
+                    self.update(params, initialize=True, adjust_time=False,
+                                plot=False)
 
             elif self.init_mode == 'simple':
                 t_sw_2 = 10
-                self.params = np.array([t_sw_1, 
-                                        t_sw_2-t_sw_1, 
-                                        t_sw_3-t_sw_2, 
-                                        self.alpha_c, 
-                                        self.alpha, 
-                                        self.beta, 
-                                        self.gamma, 
-                                        self.scale_cc, 
+                self.params = np.array([t_sw_1,
+                                        t_sw_2-t_sw_1,
+                                        t_sw_3-t_sw_2,
+                                        self.alpha_c,
+                                        self.alpha,
+                                        self.beta,
+                                        self.gamma,
+                                        self.scale_cc,
                                         self.rescale_c,
                                         self.rescale_u])
 
             elif self.init_mode == 'invert':
-                t_sw_2 = approx_tau(u0_r, s0_r, 0, 0, alpha, self.beta, self.gamma)
+                t_sw_2 = approx_tau(u0_r, s0_r, 0, 0, alpha, self.beta,
+                                    self.gamma)
                 if t_sw_2 <= 0.2:
                     t_sw_2 = 1.0
                 elif t_sw_2 >= 19.9:
                     t_sw_2 = 19.0
-                self.params = np.array([t_sw_1, 
-                                        t_sw_2-t_sw_1, 
-                                        t_sw_3-t_sw_2, 
-                                        self.alpha_c, 
-                                        self.alpha, 
-                                        self.beta, 
-                                        self.gamma, 
-                                        self.scale_cc, 
-                                        self.rescale_c, 
+                self.params = np.array([t_sw_1,
+                                        t_sw_2-t_sw_1,
+                                        t_sw_3-t_sw_2,
+                                        self.alpha_c,
+                                        self.alpha,
+                                        self.beta,
+                                        self.gamma,
+                                        self.scale_cc,
+                                        self.rescale_c,
                                         self.rescale_u])
 
         # chromatin-RNA
         else:
             if self.init_mode == 'grid':
-                for t_sw_1 in np.arange(1, 18, 4, dtype=np.float64): # 1,5,9,13,17
-                    for t_sw_2 in np.arange(t_sw_1+1, 19, 4, dtype=np.float64): # 2,6,10,14,18
-                        for t_sw_3 in np.arange(t_sw_2+1, 20, 4, dtype=np.float64): # 3,7,11,15,19
+                # arange returns sequence [1,5,9,13,17]
+                for t_sw_1 in np.arange(1, 18, 4, dtype=np.float64):
+                    # arange returns sequence 2,6,10,14,18
+                    for t_sw_2 in np.arange(t_sw_1+1, 19, 4, dtype=np.float64):
+                        # arange returns sequence [3,7,11,15,19]
+                        for t_sw_3 in np.arange(t_sw_2+1, 20, 4,
+                                                dtype=np.float64):
                             if not self.fit_decoupling:
                                 t_sw_3 = t_sw_2 + 30 / self.n_anchors
-                            params = np.array([t_sw_1, 
-                                               t_sw_2-t_sw_1, 
-                                               t_sw_3-t_sw_2, 
-                                               self.alpha_c, 
-                                               self.alpha, 
-                                               self.beta, 
-                                               self.gamma, 
-                                               self.scale_cc, 
+                            params = np.array([t_sw_1,
+                                               t_sw_2-t_sw_1,
+                                               t_sw_3-t_sw_2,
+                                               self.alpha_c,
+                                               self.alpha,
+                                               self.beta,
+                                               self.gamma,
+                                               self.scale_cc,
                                                self.rescale_c,
                                                self.rescale_u])
-                            self.update(params, initialize=True, adjust_time=False, plot=False)
+                            self.update(params, initialize=True,
+                                        adjust_time=False, plot=False)
                             if not self.fit_decoupling:
                                 break
 
             elif self.init_mode == 'simple':
-                t_sw_1, t_sw_2, t_sw_3 = 5, 10, 15 if not self.fit_decoupling else 10.1
-                self.params = np.array([t_sw_1, 
-                                        t_sw_2-t_sw_1, 
-                                        t_sw_3-t_sw_2, 
-                                        self.alpha_c, 
-                                        self.alpha, 
-                                        self.beta, 
-                                        self.gamma, 
-                                        self.scale_cc, 
-                                        self.rescale_c, 
+                t_sw_1, t_sw_2, t_sw_3 = 5, 10, 15 \
+                    if not self.fit_decoupling \
+                    else 10.1
+                self.params = np.array([t_sw_1,
+                                        t_sw_2-t_sw_1,
+                                        t_sw_3-t_sw_2,
+                                        self.alpha_c,
+                                        self.alpha,
+                                        self.beta,
+                                        self.gamma,
+                                        self.scale_cc,
+                                        self.rescale_c,
                                         self.rescale_u])
 
             elif self.init_mode == 'invert':
                 self.alpha = u0_r / c_upper
                 if model_mismatch or not self.fit_decoupling:
                     self.alpha = u0_r / c0_r
-                rna_interval = approx_tau(u0_r, s0_r, 0, 0, alpha, self.beta, self.gamma)
+                rna_interval = approx_tau(u0_r, s0_r, 0, 0, alpha, self.beta,
+                                          self.gamma)
                 rna_interval = np.clip(rna_interval, 3, 12)
                 if self.model == 1:
-                    for t_sw_1 in np.arange(1, rna_interval-1, 2, dtype=np.float64):
+                    for t_sw_1 in np.arange(1, rna_interval-1, 2,
+                                            dtype=np.float64):
                         t_sw_3 = rna_interval + t_sw_1
-                        for t_sw_2 in np.arange(t_sw_1+1, rna_interval, 2, dtype=np.float64):
+                        for t_sw_2 in np.arange(t_sw_1+1, rna_interval, 2,
+                                                dtype=np.float64):
                             if not self.fit_decoupling:
                                 t_sw_2 = t_sw_3 - 30 / self.n_anchors
-                                #c0_r = c_upper
 
                             alpha_c = -np.log(1 - c0_r) / t_sw_2
-                            params = np.array([t_sw_1, 
-                                               t_sw_2-t_sw_1, 
-                                               t_sw_3-t_sw_2, 
-                                               alpha_c, 
-                                               self.alpha, 
-                                               self.beta, 
-                                               self.gamma, 
-                                               self.scale_cc, 
-                                               self.rescale_c, 
+                            params = np.array([t_sw_1,
+                                               t_sw_2-t_sw_1,
+                                               t_sw_3-t_sw_2,
+                                               alpha_c,
+                                               self.alpha,
+                                               self.beta,
+                                               self.gamma,
+                                               self.scale_cc,
+                                               self.rescale_c,
                                                self.rescale_u])
-                            self.update(params, initialize=True, adjust_time=False, plot=False)
+                            self.update(params, initialize=True,
+                                        adjust_time=False, plot=False)
                             if not self.fit_decoupling:
                                 break
 
                 elif self.model == 2:
-                    for t_sw_1 in np.arange(1, rna_interval, 2, dtype=np.float64):
+                    for t_sw_1 in np.arange(1, rna_interval, 2,
+                                            dtype=np.float64):
                         t_sw_2 = rna_interval + t_sw_1
-                        for t_sw_3 in np.arange(t_sw_2+1, t_sw_2+6, 2, dtype=np.float64):
+                        for t_sw_3 in np.arange(t_sw_2+1, t_sw_2+6, 2,
+                                                dtype=np.float64):
                             if not self.fit_decoupling:
                                 t_sw_3 = t_sw_2 + 30 / self.n_anchors
-                                #c0_r = c_upper
 
                             alpha_c = -np.log(1 - c0_r) / t_sw_3
-                            params = np.array([t_sw_1, 
-                                               t_sw_2-t_sw_1, 
-                                               t_sw_3-t_sw_2, 
-                                               alpha_c, 
-                                               self.alpha, 
-                                               self.beta, 
-                                               self.gamma, 
-                                               self.scale_cc, 
-                                               self.rescale_c, 
+                            params = np.array([t_sw_1,
+                                               t_sw_2-t_sw_1,
+                                               t_sw_3-t_sw_2,
+                                               alpha_c,
+                                               self.alpha,
+                                               self.beta,
+                                               self.gamma,
+                                               self.scale_cc,
+                                               self.rescale_c,
                                                self.rescale_u])
-                            self.update(params, initialize=True, adjust_time=False, plot=False)
+                            self.update(params, initialize=True,
+                                        adjust_time=False, plot=False)
                             if not self.fit_decoupling:
                                 break
 
         self.loss = [self.mse(self.params)]
-        self.t_sw_array = np.array([self.params[0], 
-                                    self.params[0]+self.params[1], 
-                                    self.params[0]+self.params[1]+self.params[2]])
+        self.t_sw_array = np.array([self.params[0],
+                                    self.params[0]+self.params[1],
+                                    self.params[0]+self.params[1]
+                                    + self.params[2]])
         self.t_sw_1, self.t_sw_2, self.t_sw_3 = self.t_sw_array
 
         if self.verbose >= 1:
-            print(f'initial params: {self.t_sw_array} {self.rates} {self.rescale_c} {self.rescale_u}')
+            print(f'initial params: {self.t_sw_array} {self.rates} '
+                  '{self.rescale_c} {self.rescale_u}')
             print(f'initial loss: {self.loss[-1]}')
 
-
     def fit(self):
         if self.low_quality:
             return self.loss
 
         if self.plot:
             plt.ion()
             self.fig = plt.figure(figsize=self.fig_size)
@@ -1244,15 +1455,16 @@
                 self.ax = self.fig.add_subplot(111)
             else:
                 self.ax = self.fig.add_subplot(111, projection='3d')
 
         if not self.known_pars:
             self.fit_dyn()
 
-        self.update(self.params, perform_update=True, fit_outlier=True, plot=True)
+        self.update(self.params, perform_update=True, fit_outlier=True,
+                    plot=True)
 
         # remove long gaps in the last observed state
         t_sorted = np.sort(self.t)
         dt = np.diff(t_sorted, prepend=0)
         mean_dt = np.mean(dt)
         std_dt = np.std(dt)
         gap_thresh = np.clip(mean_dt+3*std_dt, 3*20/self.n_anchors, None)
@@ -1270,333 +1482,420 @@
             realign_ratio = np.clip(20/(20 - gap_sum), None, 20/last_t_sw)
             if self.verbose >= 1:
                 print(f'removing gaps and realigning by {realign_ratio}..')
             self.rates /= realign_ratio
             self.alpha_c, self.alpha, self.beta, self.gamma = self.rates
             self.params[:3] *= realign_ratio
             self.params[3:7] = self.rates
-            self.t_sw_array = np.array([self.params[0], self.params[0]+self.params[1], self.params[0]+self.params[1]+self.params[2]])
+            self.t_sw_array = np.array([self.params[0],
+                                        self.params[0]+self.params[1],
+                                        self.params[0]+self.params[1]
+                                        + self.params[2]])
             self.t_sw_1, self.t_sw_2, self.t_sw_3 = self.t_sw_array
-            self.update(self.params, perform_update=True, fit_outlier=True, plot=True)
+            self.update(self.params, perform_update=True, fit_outlier=True,
+                        plot=True)
 
         if self.plot:
             plt.ioff()
             plt.show(block=True)
 
         # likelihood
         if self.verbose >= 1:
             print('computing likelihood..')
-        keep = self.non_zero & self.non_outlier & (self.u_all > 0.2 * np.percentile(self.u_all, 99.5)) & (self.s_all > 0.2 * np.percentile(self.s_all, 99.5))
-        scale_factor = np.array([self.scale_c / self.std_c, self.scale_u / self.std_u, self.scale_s / self.std_s])
+        keep = self.non_zero & self.non_outlier & \
+            (self.u_all > 0.2 * np.percentile(self.u_all, 99.5)) & \
+            (self.s_all > 0.2 * np.percentile(self.s_all, 99.5))
+        scale_factor = np.array([self.scale_c / self.std_c,
+                                 self.scale_u / self.std_u,
+                                 self.scale_s / self.std_s])
         if np.sum(keep) >= 10:
-            self.likelihood, self.l_c, self.ssd_c, self.var_c, l_u, l_s = compute_likelihood(self.c_all, 
-                                                                                             self.u_all, 
-                                                                                             self.s_all, 
-                                                                                             self.t_sw_array, 
-                                                                                             self.alpha_c, 
-                                                                                             self.alpha, 
-                                                                                             self.beta, 
-                                                                                             self.gamma, 
-                                                                                             self.rescale_c,
-                                                                                             self.rescale_u,
-                                                                                             self.t, 
-                                                                                             self.state, 
-                                                                                             scale_cc=self.scale_cc, 
-                                                                                             scale_factor=scale_factor, 
-                                                                                             model=self.model, 
-                                                                                             weight=keep, 
-                                                                                             rna_only=self.rna_only)
+            self.likelihood, self.l_c, self.ssd_c, self.var_c, l_u, l_s = \
+                compute_likelihood(self.c_all,
+                                   self.u_all,
+                                   self.s_all,
+                                   self.t_sw_array,
+                                   self.alpha_c,
+                                   self.alpha,
+                                   self.beta,
+                                   self.gamma,
+                                   self.rescale_c,
+                                   self.rescale_u,
+                                   self.t,
+                                   self.state,
+                                   scale_cc=self.scale_cc,
+                                   scale_factor=scale_factor,
+                                   model=self.model,
+                                   weight=keep,
+                                   rna_only=self.rna_only)
         else:
-            self.likelihood, self.l_c, self.ssd_c, self.var_c, l_u, l_s = 0, 0, 0, 0, 0, 0
+            self.likelihood, self.l_c, self.ssd_c, self.var_c, l_u = \
+                0, 0, 0, 0, 0
 
         if not self.rna_only and self.verbose >= 1:
-            print(f'likelihood of c: {self.l_c}, likelihood of u: {l_u}, likelihood of s: {l_s}')
+            print(f'likelihood of c: {self.l_c}, likelihood of u: {l_u}, '
+                  'likelihood of s: {l_s}')
 
         # velocity
         if self.verbose >= 1:
             print('computing velocities..')
         self.velocity = np.empty((len(self.u_all), 3))
         if self.conn is not None:
             new_time = self.conn.dot(self.t)
             new_time[new_time > 20] = 20
             new_state = self.state.copy()
             new_state[new_time <= self.t_sw_1] = 0
             new_state[(self.t_sw_1 < new_time) & (new_time <= self.t_sw_2)] = 1
             new_state[(self.t_sw_2 < new_time) & (new_time <= self.t_sw_3)] = 2
             new_state[self.t_sw_3 < new_time] = 3
-            #self.t = new_time
-            #self.state = new_state
+
         else:
             new_time = self.t
             new_state = self.state
 
-        vc, vu, vs = compute_velocity(new_time, 
-                                      self.t_sw_array, 
-                                      new_state, 
-                                      self.alpha_c, 
-                                      self.alpha, 
-                                      self.beta, 
-                                      self.gamma, 
+        vc, vu, vs = compute_velocity(new_time,
+                                      self.t_sw_array,
+                                      new_state,
+                                      self.alpha_c,
+                                      self.alpha,
+                                      self.beta,
+                                      self.gamma,
                                       self.rescale_c,
                                       self.rescale_u,
-                                      scale_cc=self.scale_cc, 
-                                      model=self.model, 
+                                      scale_cc=self.scale_cc,
+                                      model=self.model,
                                       rna_only=self.rna_only)
 
-        self.velocity[:,0] = vc * self.scale_c
-        self.velocity[:,1] = vu * self.scale_u
-        self.velocity[:,2] = vs * self.scale_s
+        self.velocity[:, 0] = vc * self.scale_c
+        self.velocity[:, 1] = vu * self.scale_u
+        self.velocity[:, 2] = vs * self.scale_s
 
         # anchor expression and velocity
-        anchor_time, tau_list = anchor_points(self.t_sw_array, 20, self.n_anchors, return_time=True)
+        anchor_time, tau_list = anchor_points(self.t_sw_array, 20,
+                                              self.n_anchors, return_time=True)
         switch = np.sum(self.t_sw_array < 20)
         typed_tau_list = List()
         [typed_tau_list.append(x) for x in tau_list]
-        exp_list, exp_sw_list = generate_exp(typed_tau_list, 
-                                             self.t_sw_array[:switch], 
-                                             self.alpha_c, 
-                                             self.alpha, 
-                                             self.beta, 
-                                             self.gamma, 
-                                             scale_cc=self.scale_cc, 
-                                             model=self.model, 
+        exp_list, exp_sw_list = generate_exp(typed_tau_list,
+                                             self.t_sw_array[:switch],
+                                             self.alpha_c,
+                                             self.alpha,
+                                             self.beta,
+                                             self.gamma,
+                                             scale_cc=self.scale_cc,
+                                             model=self.model,
                                              rna_only=self.rna_only)
         rescale_factor = np.array([self.rescale_c, self.rescale_u, 1.0])
         exp_list = [x*rescale_factor for x in exp_list]
         exp_sw_list = [x*rescale_factor for x in exp_sw_list]
-        c = np.ravel(np.concatenate([exp_list[x][:,0] for x in range(switch+1)]))
-        u = np.ravel(np.concatenate([exp_list[x][:,1] for x in range(switch+1)]))
-        s = np.ravel(np.concatenate([exp_list[x][:,2] for x in range(switch+1)]))
-        c_sw = np.ravel(np.concatenate([exp_sw_list[x][:,0] for x in range(switch)]))
-        u_sw = np.ravel(np.concatenate([exp_sw_list[x][:,1] for x in range(switch)]))
-        s_sw = np.ravel(np.concatenate([exp_sw_list[x][:,2] for x in range(switch)]))
-        vc, vu, vs = compute_velocity(anchor_time, 
-                                      self.t_sw_array, 
-                                      None, 
-                                      self.alpha_c, 
-                                      self.alpha, 
-                                      self.beta, 
-                                      self.gamma, 
+        c = np.ravel(np.concatenate([exp_list[x][:, 0]
+                                     for x in range(switch+1)]))
+        u = np.ravel(np.concatenate([exp_list[x][:, 1]
+                                     for x in range(switch+1)]))
+        s = np.ravel(np.concatenate([exp_list[x][:, 2]
+                                     for x in range(switch+1)]))
+        c_sw = np.ravel(np.concatenate([exp_sw_list[x][:, 0]
+                                        for x in range(switch)]))
+        u_sw = np.ravel(np.concatenate([exp_sw_list[x][:, 1]
+                                        for x in range(switch)]))
+        s_sw = np.ravel(np.concatenate([exp_sw_list[x][:, 2]
+                                        for x in range(switch)]))
+        vc, vu, vs = compute_velocity(anchor_time,
+                                      self.t_sw_array,
+                                      None,
+                                      self.alpha_c,
+                                      self.alpha,
+                                      self.beta,
+                                      self.gamma,
                                       self.rescale_c,
                                       self.rescale_u,
-                                      scale_cc=self.scale_cc, 
-                                      model=self.model, 
+                                      scale_cc=self.scale_cc,
+                                      model=self.model,
                                       rna_only=self.rna_only)
 
         # scale and shift back to original scale
         c_ = c * self.scale_c + self.offset_c
         u_ = u * self.scale_u + self.offset_u
         s_ = s * self.scale_s + self.offset_s
         c_sw_ = c_sw * self.scale_c + self.offset_c
         u_sw_ = u_sw * self.scale_u + self.offset_u
         s_sw_ = s_sw * self.scale_s + self.offset_s
         vc = vc * self.scale_c
         vu = vu * self.scale_u
         vs = vs * self.scale_s
 
         self.anchor_exp = np.empty((len(u_), 3))
-        self.anchor_exp[:,0], self.anchor_exp[:,1], self.anchor_exp[:,2] = c_, u_, s_
+        self.anchor_exp[:, 0], self.anchor_exp[:, 1], self.anchor_exp[:, 2] = \
+            c_, u_, s_
         self.anchor_exp_sw = np.empty((len(u_sw_), 3))
-        self.anchor_exp_sw[:,0], self.anchor_exp_sw[:,1], self.anchor_exp_sw[:,2] = c_sw_, u_sw_, s_sw_
+        self.anchor_exp_sw[:, 0], self.anchor_exp_sw[:, 1], \
+            self.anchor_exp_sw[:, 2] = c_sw_, u_sw_, s_sw_
         self.anchor_velo = np.empty((len(u_), 3))
-        self.anchor_velo[:,0] = vc
-        self.anchor_velo[:,1] = vu
-        self.anchor_velo[:,2] = vs
+        self.anchor_velo[:, 0] = vc
+        self.anchor_velo[:, 1] = vu
+        self.anchor_velo[:, 2] = vs
         self.anchor_velo_min_idx = np.sum(anchor_time < np.min(new_time))
         self.anchor_velo_max_idx = np.sum(anchor_time < np.max(new_time)) - 1
 
         if self.save_plot:
             if self.verbose >= 1:
                 print('saving plots..')
             self.save_dyn_plot(c_, u_, s_, c_sw_, u_sw_, s_sw_, tau_list)
 
         self.realign_time_and_velocity(c, u, s, anchor_time)
 
         if self.verbose >= 1:
-            print(f'final params: {self.t_sw_array} {self.rates} {self.scale_cc} {self.rescale_c} {self.rescale_u}')
+            print(f'final params: {self.t_sw_array} {self.rates} '
+                  '{self.scale_cc} {self.rescale_c} {self.rescale_u}')
             print(f'final loss: {self.loss[-1]}')
             print(f'final likelihood: {self.likelihood}')
 
         return self.loss
 
-
     def fit_dyn(self):
 
         while self.cur_iter < self.max_iter:
             self.cur_iter += 1
 
             # RNA-only
             if self.rna_only:
-                #self.update(self.params, perform_update=True)
                 if self.verbose >= 2:
                     print('Nelder Mead on t_sw_2 and alpha..')
                 self.fitting_flag_ = 0
                 if self.cur_iter == 1:
-                    var_test = self.alpha + np.array([-2,-1,-0.5,0.5,1,2]) * 0.1 * self.alpha
+                    var_test = (self.alpha +
+                                np.array([-2, -1, -0.5, 0.5, 1, 2]) * 0.1
+                                * self.alpha)
                     new_params = self.params.copy()
                     for var in var_test:
                         new_params[4] = var
-                        self.update(new_params, adjust_time=False, penalize_gap=False)
-                res = minimize(self.mse, x0=[self.params[1], self.params[4]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':3})
+                        self.update(new_params, adjust_time=False,
+                                    penalize_gap=False)
+                res = minimize(self.mse, x0=[self.params[1], self.params[4]],
+                               method='Nelder-Mead', tol=1e-2,
+                               callback=self.update, options={'maxiter': 3})
 
                 if self.fit_rescale:
                     if self.verbose >= 2:
                         print('Nelder Mead on t_sw_2, beta, and rescale u..')
-                    res = minimize(self.mse, x0=[self.params[1], self.params[5], self.params[9]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':5})
+                    res = minimize(self.mse, x0=[self.params[1],
+                                                 self.params[5],
+                                                 self.params[9]],
+                                   method='Nelder-Mead', tol=1e-2,
+                                   callback=self.update,
+                                   options={'maxiter': 5})
 
                 if self.verbose >= 2:
                     print('Nelder Mead on alpha and gamma..')
                 self.fitting_flag_ = 1
-                res = minimize(self.mse, x0=[self.params[4], self.params[6]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':3})
+                res = minimize(self.mse, x0=[self.params[4], self.params[6]],
+                               method='Nelder-Mead', tol=1e-2,
+                               callback=self.update, options={'maxiter': 3})
 
                 if self.verbose >= 2:
                     print('Nelder Mead on t_sw_2..')
-                res = minimize(self.mse, x0=[self.params[1]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':2})
+                res = minimize(self.mse, x0=[self.params[1]],
+                               method='Nelder-Mead', tol=1e-2,
+                               callback=self.update, options={'maxiter': 2})
 
                 if self.verbose >= 2:
                     print('Full Nelder Mead..')
-                res = minimize(self.mse, x0=[self.params[1], self.params[4], self.params[5], self.params[6]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':5})
+                res = minimize(self.mse, x0=[self.params[1], self.params[4],
+                                             self.params[5], self.params[6]],
+                               method='Nelder-Mead', tol=1e-2,
+                               callback=self.update, options={'maxiter': 5})
 
             # chromatin-RNA
             else:
-                #self.update(self.params, perform_update=True)
                 if self.verbose >= 2:
-                    print('Nelder Mead on t_sw_1, chromatin switch time, and alpha_c..')
+                    print('Nelder Mead on t_sw_1, chromatin switch time, and '
+                          'alpha_c..')
                 self.fitting_flag_ = 1
                 if self.cur_iter == 1:
-                    var_test = self.gamma + np.array([-1,-0.5,0.5,1]) * 0.1 * self.gamma
+                    var_test = (self.gamma + np.array([-1, -0.5, 0.5, 1])
+                                * 0.1 * self.gamma)
                     new_params = self.params.copy()
                     for var in var_test:
                         new_params[6] = var
                         self.update(new_params, adjust_time=False)
                 if self.model == 0 or self.model == 1:
-                    res = minimize(self.mse, x0=[self.params[0], self.params[1], self.params[3]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':20})
+                    res = minimize(self.mse, x0=[self.params[0],
+                                                 self.params[1],
+                                                 self.params[3]],
+                                   method='Nelder-Mead', tol=1e-2,
+                                   callback=self.update,
+                                   options={'maxiter': 20})
                 elif self.model == 2:
-                    res = minimize(self.mse, x0=[self.params[0], self.params[2], self.params[3]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':20})
+                    res = minimize(self.mse, x0=[self.params[0],
+                                                 self.params[2],
+                                                 self.params[3]],
+                                   method='Nelder-Mead', tol=1e-2,
+                                   callback=self.update,
+                                   options={'maxiter': 20})
 
                 if self.verbose >= 2:
-                    print('Nelder Mead on chromatin switch time, chromatin closing rate scaling, and rescale c..')
+                    print('Nelder Mead on chromatin switch time, chromatin '
+                          'closing rate scaling, and rescale c..')
                 self.fitting_flag_ = 2
                 if self.model == 0 or self.model == 1:
-                    res = minimize(self.mse, x0=[self.params[1], self.params[7], self.params[8]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':20})
+                    res = minimize(self.mse, x0=[self.params[1],
+                                                 self.params[7],
+                                                 self.params[8]],
+                                   method='Nelder-Mead', tol=1e-2,
+                                   callback=self.update,
+                                   options={'maxiter': 20})
                 elif self.model == 2:
-                    res = minimize(self.mse, x0=[self.params[2], self.params[7], self.params[8]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':20})
+                    res = minimize(self.mse, x0=[self.params[2],
+                                                 self.params[7],
+                                                 self.params[8]],
+                                   method='Nelder-Mead', tol=1e-2,
+                                   callback=self.update,
+                                   options={'maxiter': 20})
 
                 if self.verbose >= 2:
                     print('Nelder Mead on rna switch time and alpha..')
                 self.fitting_flag_ = 1
                 if self.model == 0 or self.model == 1:
-                    res = minimize(self.mse, x0=[self.params[2], self.params[4]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':10})
+                    res = minimize(self.mse, x0=[self.params[2],
+                                                 self.params[4]],
+                                   method='Nelder-Mead', tol=1e-2,
+                                   callback=self.update,
+                                   options={'maxiter': 10})
                 elif self.model == 2:
-                    res = minimize(self.mse, x0=[self.params[1], self.params[4]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':10})
+                    res = minimize(self.mse, x0=[self.params[1],
+                                                 self.params[4]],
+                                   method='Nelder-Mead', tol=1e-2,
+                                   callback=self.update,
+                                   options={'maxiter': 10})
 
                 if self.verbose >= 2:
-                    print('Nelder Mead on rna switch time, beta, and rescale u..')
+                    print('Nelder Mead on rna switch time, beta, and '
+                          'rescale u..')
                 self.fitting_flag_ = 3
                 if self.model == 0 or self.model == 1:
-                    res = minimize(self.mse, x0=[self.params[2], self.params[5], self.params[9]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':20})
+                    res = minimize(self.mse, x0=[self.params[2],
+                                                 self.params[5],
+                                                 self.params[9]],
+                                   method='Nelder-Mead', tol=1e-2,
+                                   callback=self.update,
+                                   options={'maxiter': 20})
                 elif self.model == 2:
-                    res = minimize(self.mse, x0=[self.params[1], self.params[5], self.params[9]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':20})
+                    res = minimize(self.mse, x0=[self.params[1],
+                                                 self.params[5],
+                                                 self.params[9]],
+                                   method='Nelder-Mead', tol=1e-2,
+                                   callback=self.update,
+                                   options={'maxiter': 20})
 
                 if self.verbose >= 2:
                     print('Nelder Mead on alpha and gamma..')
                 self.fitting_flag_ = 2
-                res = minimize(self.mse, x0=[self.params[4], self.params[6]], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':10})
+                res = minimize(self.mse, x0=[self.params[4], self.params[6]],
+                               method='Nelder-Mead', tol=1e-2,
+                               callback=self.update, options={'maxiter': 10})
 
                 if self.verbose >= 2:
                     print('Nelder Mead on t_sw..')
                 self.fitting_flag_ = 4
-                res = minimize(self.mse, x0=self.params[:3], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':20})
-
-                #if self.verbose >= 2:
-                    #print('full Nelder Mead')
-                #res = minimize(self.mse, x0=self.params[:7], method='Nelder-Mead', tol=1e-2, callback=self.update, options={'maxiter':20})
+                res = minimize(self.mse, x0=self.params[:3],
+                               method='Nelder-Mead', tol=1e-2,
+                               callback=self.update, options={'maxiter': 20})
 
             if self.verbose >= 2:
                 print(f'iteration {self.cur_iter} finished')
 
-
     def _variables(self, x):
         scale_cc = self.scale_cc
         rescale_c = self.rescale_c
         rescale_u = self.rescale_u
 
         # RNA-only
         if self.rna_only:
-            if len(x) == 1: # fit t_sw_2
-                t3 = np.array([self.t_sw_1, x[0], self.t_sw_3 - self.t_sw_1 - x[0]])
+            if len(x) == 1:  # fit t_sw_2
+                t3 = np.array([self.t_sw_1, x[0],
+                               self.t_sw_3 - self.t_sw_1 - x[0]])
                 r4 = self.rates
 
-            elif len(x) == 2: 
-                if self.fitting_flag_: # fit alpha and gamma
+            elif len(x) == 2:
+                if self.fitting_flag_:  # fit alpha and gamma
                     t3 = self.params[:3]
                     r4 = np.array([self.alpha_c, x[0], self.beta, x[1]])
-                else: # fit t_sw_2 and alpha
-                    t3 = np.array([self.t_sw_1, x[0], self.t_sw_3 - self.t_sw_1 - x[0]])
+                else:  # fit t_sw_2 and alpha
+                    t3 = np.array([self.t_sw_1, x[0],
+                                   self.t_sw_3 - self.t_sw_1 - x[0]])
                     r4 = np.array([self.alpha_c, x[1], self.beta, self.gamma])
 
-            elif len(x) == 3: # fit t_sw_2, beta, and rescale u
-                t3 = np.array([self.t_sw_1, x[0], self.t_sw_3 - self.t_sw_1 - x[0]])
+            elif len(x) == 3:  # fit t_sw_2, beta, and rescale u
+                t3 = np.array([self.t_sw_1,
+                               x[0], self.t_sw_3 - self.t_sw_1 - x[0]])
                 r4 = np.array([self.alpha_c, self.alpha, x[1], self.gamma])
                 rescale_u = x[2]
 
-            elif len(x) == 4: # fit all
-                t3 = np.array([self.t_sw_1, x[0], self.t_sw_3 - self.t_sw_1 - x[0]])
+            elif len(x) == 4:  # fit all
+                t3 = np.array([self.t_sw_1, x[0], self.t_sw_3 - self.t_sw_1
+                               - x[0]])
                 r4 = np.array([self.alpha_c, x[1], x[2], x[3]])
 
-            elif len(x) == 10: # all available
+            elif len(x) == 10:  # all available
                 t3 = x[:3]
                 r4 = x[3:7]
                 scale_cc = x[7]
                 rescale_c = x[8]
                 rescale_u = x[9]
 
             else:
                 return
 
         # chromatin-RNA
         else:
-            if len(x) == 2: 
-                if self.fitting_flag_ == 1: # fit rna switch time and alpha
+            if len(x) == 2:
+                if self.fitting_flag_ == 1:  # fit rna switch time and alpha
                     if self.model == 0 or self.model == 1:
                         t3 = np.array([self.t_sw_1, self.params[1], x[0]])
                     elif self.model == 2:
-                        t3 = np.array([self.t_sw_1, x[0], self.t_sw_3 - self.t_sw_1 - x[0]])
+                        t3 = np.array([self.t_sw_1, x[0],
+                                       self.t_sw_3 - self.t_sw_1 - x[0]])
                     r4 = np.array([self.alpha_c, x[1], self.beta, self.gamma])
-                elif self.fitting_flag_ == 2: # fit alpha and gamma
+                elif self.fitting_flag_ == 2:  # fit alpha and gamma
                     t3 = self.params[:3]
                     r4 = np.array([self.alpha_c, x[0], self.beta, x[1]])
 
-            elif len(x) == 3: 
-                if self.fitting_flag_ == 1: # fit t_sw_1, chromatin switch time, and alpha_c
+            elif len(x) == 3:
+                # fit t_sw_1, chromatin switch time, and alpha_c
+                if self.fitting_flag_ == 1:
                     if self.model == 0 or self.model == 1:
                         t3 = np.array([x[0], x[1], self.t_sw_3 - x[0] - x[1]])
                     elif self.model == 2:
                         t3 = np.array([x[0], self.t_sw_2 - x[0], x[1]])
                     r4 = np.array([x[2], self.alpha, self.beta, self.gamma])
-                elif self.fitting_flag_ == 2: # fit chromatin switch time, chromatin closing rate scaling, and rescale c
+                # fit chromatin switch time, chromatin closing rate scaling,
+                # and rescale c
+                elif self.fitting_flag_ == 2:
                     if self.model == 0 or self.model == 1:
-                        t3 = np.array([self.t_sw_1, x[0], self.t_sw_3 - self.t_sw_1 - x[0]])
+                        t3 = np.array([self.t_sw_1, x[0],
+                                       self.t_sw_3 - self.t_sw_1 - x[0]])
                     elif self.model == 2:
                         t3 = np.array([self.t_sw_1, self.params[1], x[0]])
                     r4 = self.rates
                     scale_cc = x[1]
                     rescale_c = x[2]
-                elif self.fitting_flag_ == 3: # fit rna switch time, beta, and rescale u
+                # fit rna switch time, beta, and rescale u
+                elif self.fitting_flag_ == 3:
                     if self.model == 0 or self.model == 1:
                         t3 = np.array([self.t_sw_1, self.params[1], x[0]])
                     elif self.model == 2:
-                        t3 = np.array([self.t_sw_1, x[0], self.t_sw_3 - self.t_sw_1 - x[0]])
+                        t3 = np.array([self.t_sw_1, x[0],
+                                       self.t_sw_3 - self.t_sw_1 - x[0]])
                     r4 = np.array([self.alpha_c, self.alpha, x[1], self.gamma])
                     rescale_u = x[2]
-                elif self.fitting_flag_ == 4: # fit three switch times
+                # fit three switch times
+                elif self.fitting_flag_ == 4:
                     t3 = x
                     r4 = self.rates
 
-            elif len(x) == 7: 
+            elif len(x) == 7:
                 t3 = x[:3]
                 r4 = x[3:]
 
             elif len(x) == 10:
                 t3 = x[:3]
                 r4 = x[3:7]
                 scale_cc = x[7]
@@ -1604,109 +1903,112 @@
                 rescale_u = x[9]
 
             else:
                 return
 
         # clip to meaningful values
         if self.fitting_flag_:
-            scale_cc = np.clip(scale_cc, np.max([0.5*self.scale_cc, 0.25]), np.min([2*self.scale_cc, 4]))
+            scale_cc = np.clip(scale_cc,
+                               np.max([0.5*self.scale_cc, 0.25]),
+                               np.min([2*self.scale_cc, 4]))
 
         if not self.known_pars:
             if self.fit_decoupling:
                 t3 = np.clip(t3, 0.1, None)
             else:
                 t3[2] = 30 / self.n_anchors
                 t3[:2] = np.clip(t3[:2], 0.1, None)
             r4 = np.clip(r4, 0.001, 1000)
             rescale_c = np.clip(rescale_c, 0.75, 1.5)
             rescale_u = np.clip(rescale_u, 0.2, 3)
 
         return t3, r4, scale_cc, rescale_c, rescale_u
 
-
     def mse(self, x, fit_outlier=False, penalize_gap=True):
         x = np.array(x)
-        n = len(self.u)
 
         t3, r4, scale_cc, rescale_c, rescale_u = self._variables(x)
 
         t_sw_array = np.array([t3[0], t3[0]+t3[1], t3[0]+t3[1]+t3[2]])
         if self.rna_only:
             t_sw_array[2] = 20
 
         # conditions for minimum switch time and rate params
         penalty = 0
         if any(t3 < 0.2) or any(r4 < 0.005):
-            penalty = np.sum(0.2 - t3[t3 < 0.2]) if self.fit_decoupling else np.sum(0.2 - t3[:2][t3[:2] < 0.2])
+            penalty = (np.sum(0.2 - t3[t3 < 0.2]) if self.fit_decoupling
+                       else np.sum(0.2 - t3[:2][t3[:2] < 0.2]))
             penalty += np.sum(0.005 - r4[r4 < 0.005]) * 1e2
 
-        #condition for all params
+        # condition for all params
         if any(x > 500):
             penalty = np.sum(x[x > 500] - 500) * 1e-2
 
         c_array = self.c_all if fit_outlier else self.c
         u_array = self.u_all if fit_outlier else self.u
         s_array = self.s_all if fit_outlier else self.s
 
         # distances and time assignments
-        res = calculate_dist_and_time(c_array, 
-                                      u_array, 
-                                      s_array, 
-                                      t_sw_array, 
-                                      r4[0], 
-                                      r4[1], 
-                                      r4[2], 
-                                      r4[3], 
-                                      rescale_c, 
-                                      rescale_u, 
-                                      scale_cc=scale_cc, 
-                                      scale_factor=self.scale_factor, 
-                                      model=self.model, 
-                                      direction=self.direction, 
-                                      conn=self.conn if fit_outlier else self.conn_sub, 
-                                      k=self.k_dist, 
-                                      t=self.n_anchors, 
+        res = calculate_dist_and_time(c_array,
+                                      u_array,
+                                      s_array,
+                                      t_sw_array,
+                                      r4[0],
+                                      r4[1],
+                                      r4[2],
+                                      r4[3],
+                                      rescale_c,
+                                      rescale_u,
+                                      scale_cc=scale_cc,
+                                      scale_factor=self.scale_factor,
+                                      model=self.model,
+                                      direction=self.direction,
+                                      conn=self.conn if fit_outlier
+                                      else self.conn_sub,
+                                      k=self.k_dist,
+                                      t=self.n_anchors,
                                       rna_only=self.rna_only,
                                       penalize_gap=penalize_gap,
                                       all_cells=fit_outlier)
 
         if fit_outlier:
-            min_dist, t_pred, state_pred, reach_ss, late_phase, max_u, max_s, self.anchor_t1_list, self.anchor_t2_list = res
+            min_dist, t_pred, state_pred, reach_ss, late_phase, max_u, max_s, \
+                self.anchor_t1_list, self.anchor_t2_list = res
         else:
             min_dist, state_pred, max_u, max_s, t_sw_adjust = res
 
-
         loss = np.mean(min_dist)
 
         # avoid exceeding maximum expressions
         reg = np.max([0, max_s - self.max_s]) + np.max([0, max_u - self.max_u])
-        #reg = np.abs(max_s - np.percentile(s_array, 99)) + np.abs(max_u - np.percentile(u_array, 99))
         loss += reg
 
         loss += 1e-1 * penalty
         self.cur_loss = loss
         self.cur_state_pred = state_pred
 
         if fit_outlier:
             return loss, t_pred
         else:
             self.cur_t_sw_adjust = t_sw_adjust
 
         return loss
 
-
-    def update(self, x, perform_update=False, initialize=False, fit_outlier=False, adjust_time=True, penalize_gap=True, plot=True):
+    def update(self, x, perform_update=False, initialize=False,
+               fit_outlier=False, adjust_time=True, penalize_gap=True,
+               plot=True):
         t3, r4, scale_cc, rescale_c, rescale_u = self._variables(x)
         t_sw_array = np.array([t3[0], t3[0]+t3[1], t3[0]+t3[1]+t3[2]])
 
         # read results
         if initialize:
             new_loss = self.mse(x, penalize_gap=penalize_gap)
         elif fit_outlier:
-            new_loss, t_pred = self.mse(x, fit_outlier=True, penalize_gap=penalize_gap)
+            new_loss, t_pred = self.mse(x, fit_outlier=True,
+                                        penalize_gap=penalize_gap)
         else:
             new_loss = self.cur_loss
             t_sw_adjust = self.cur_t_sw_adjust
         state_pred = self.cur_state_pred
 
         if new_loss < self.loss[-1] or perform_update:
             perform_update = True
@@ -1722,103 +2024,124 @@
             if not fit_outlier and adjust_time:
                 t_sw_array -= np.cumsum(t_sw_adjust)
                 if self.rna_only:
                     t_sw_array[2] = 20
 
             self.t_sw_1, self.t_sw_2, self.t_sw_3 = t_sw_array
             self.t_sw_array = t_sw_array
-            self.params = np.array([self.t_sw_1, 
-                                    self.t_sw_2-self.t_sw_1, 
-                                    self.t_sw_3-self.t_sw_2, 
-                                    self.alpha_c, 
-                                    self.alpha, 
-                                    self.beta, 
-                                    self.gamma, 
-                                    self.scale_cc, 
-                                    self.rescale_c, 
+            self.params = np.array([self.t_sw_1,
+                                    self.t_sw_2-self.t_sw_1,
+                                    self.t_sw_3-self.t_sw_2,
+                                    self.alpha_c,
+                                    self.alpha,
+                                    self.beta,
+                                    self.gamma,
+                                    self.scale_cc,
+                                    self.rescale_c,
                                     self.rescale_u])
             if not initialize:
                 self.state = state_pred
             if fit_outlier:
                 self.t = t_pred
 
             if self.verbose >= 2:
-                print(f'params updated as: {self.t_sw_array} {self.rates} {self.scale_cc} {self.rescale_c} {self.rescale_u}')
+                print(f'params updated as: {self.t_sw_array} {self.rates} '
+                      '{self.scale_cc} {self.rescale_c} {self.rescale_u}')
                 print(f'current loss: {self.loss[-1]}')
 
             # interactive plot
             if self.plot and plot:
                 tau_list = anchor_points(self.t_sw_array, 20, self.n_anchors)
                 switch = np.sum(self.t_sw_array < 20)
                 typed_tau_list = List()
                 [typed_tau_list.append(x) for x in tau_list]
-                exp_list, exp_sw_list = generate_exp(typed_tau_list, 
-                                                     self.t_sw_array[:switch], 
-                                                     self.alpha_c, 
-                                                     self.alpha, 
-                                                     self.beta, 
-                                                     self.gamma, 
-                                                     scale_cc=self.scale_cc, 
-                                                     model=self.model, 
+                exp_list, exp_sw_list = generate_exp(typed_tau_list,
+                                                     self.t_sw_array[:switch],
+                                                     self.alpha_c,
+                                                     self.alpha,
+                                                     self.beta,
+                                                     self.gamma,
+                                                     scale_cc=self.scale_cc,
+                                                     model=self.model,
                                                      rna_only=self.rna_only)
-                rescale_factor = np.array([self.rescale_c, self.rescale_u, 1.0])
+                rescale_factor = np.array([self.rescale_c,
+                                           self.rescale_u,
+                                           1.0])
                 exp_list = [x*rescale_factor for x in exp_list]
                 exp_sw_list = [x*rescale_factor for x in exp_sw_list]
-                c = np.ravel(np.concatenate([exp_list[x][:,0] for x in range(switch+1)]))
-                u = np.ravel(np.concatenate([exp_list[x][:,1] for x in range(switch+1)]))
-                s = np.ravel(np.concatenate([exp_list[x][:,2] for x in range(switch+1)]))
+                c = np.ravel(np.concatenate([exp_list[x][:, 0] for x in
+                                             range(switch+1)]))
+                u = np.ravel(np.concatenate([exp_list[x][:, 1] for x in
+                                             range(switch+1)]))
+                s = np.ravel(np.concatenate([exp_list[x][:, 2] for x in
+                                             range(switch+1)]))
                 c_ = self.c_all if fit_outlier else self.c
                 u_ = self.u_all if fit_outlier else self.u
                 s_ = self.s_all if fit_outlier else self.s
                 self.ax.clear()
                 plt.pause(0.1)
                 if self.rna_only:
-                    self.ax.scatter(s, u, s=self.point_size*1.5, c='black', alpha=0.6, zorder=2)
+                    self.ax.scatter(s, u, s=self.point_size*1.5, c='black',
+                                    alpha=0.6, zorder=2)
                     if switch >= 1:
                         c_sw1, u_sw1, s_sw1 = exp_sw_list[0][0]
-                        self.ax.plot([s_sw1], [u_sw1], "om", markersize=self.point_size, zorder=5)
+                        self.ax.plot([s_sw1], [u_sw1], "om",
+                                     markersize=self.point_size, zorder=5)
                     if switch >= 2:
                         c_sw2, u_sw2, s_sw2 = exp_sw_list[1][0]
-                        self.ax.plot([s_sw2], [u_sw2], "Xm", markersize=self.point_size, zorder=5)
+                        self.ax.plot([s_sw2], [u_sw2], "Xm",
+                                     markersize=self.point_size, zorder=5)
                     if switch == 3:
                         c_sw3, u_sw3, s_sw3 = exp_sw_list[2][0]
-                        self.ax.plot([s_sw3], [u_sw3], "Dm", markersize=self.point_size, zorder=5)
+                        self.ax.plot([s_sw3], [u_sw3], "Dm",
+                                     markersize=self.point_size, zorder=5)
                     if np.max(self.t) == 20:
-                        self.ax.plot([s[-1]], [u[-1]], "*m", markersize=self.point_size, zorder=5)
+                        self.ax.plot([s[-1]], [u[-1]], "*m",
+                                     markersize=self.point_size, zorder=5)
                     for i in range(4):
                         if any(self.state == i):
-                            self.ax.scatter(s_[(self.state == i)], u_[(self.state == i)], s=self.point_size, c=self.color[i])
+                            self.ax.scatter(s_[(self.state == i)],
+                                            u_[(self.state == i)],
+                                            s=self.point_size, c=self.color[i])
                     self.ax.set_xlabel('s')
                     self.ax.set_ylabel('u')
 
                 else:
-                    self.ax.scatter(s, u, c, s=self.point_size*1.5, c='black', alpha=0.6, zorder=2)
+                    self.ax.scatter(s, u, c, s=self.point_size*1.5,
+                                    c='black', alpha=0.6, zorder=2)
                     if switch >= 1:
                         c_sw1, u_sw1, s_sw1 = exp_sw_list[0][0]
-                        self.ax.plot([s_sw1], [u_sw1], [c_sw1], "om", markersize=self.point_size, zorder=5)
+                        self.ax.plot([s_sw1], [u_sw1], [c_sw1], "om",
+                                     markersize=self.point_size, zorder=5)
                     if switch >= 2:
                         c_sw2, u_sw2, s_sw2 = exp_sw_list[1][0]
-                        self.ax.plot([s_sw2], [u_sw2], [c_sw2], "Xm", markersize=self.point_size, zorder=5)
+                        self.ax.plot([s_sw2], [u_sw2], [c_sw2], "Xm",
+                                     markersize=self.point_size, zorder=5)
                     if switch == 3:
                         c_sw3, u_sw3, s_sw3 = exp_sw_list[2][0]
-                        self.ax.plot([s_sw3], [u_sw3], [c_sw3], "Dm", markersize=self.point_size, zorder=5)
+                        self.ax.plot([s_sw3], [u_sw3], [c_sw3], "Dm",
+                                     markersize=self.point_size, zorder=5)
                     if np.max(self.t) == 20:
-                        self.ax.plot([s[-1]], [u[-1]], [c[-1]], "*m", markersize=self.point_size, zorder=5)
+                        self.ax.plot([s[-1]], [u[-1]], [c[-1]], "*m",
+                                     markersize=self.point_size, zorder=5)
                     for i in range(4):
                         if any(self.state == i):
-                            self.ax.scatter(s_[(self.state == i)], u_[(self.state == i)], c_[(self.state == i)], s=self.point_size, c=self.color[i])
+                            self.ax.scatter(s_[(self.state == i)],
+                                            u_[(self.state == i)],
+                                            c_[(self.state == i)],
+                                            s=self.point_size, c=self.color[i])
                     self.ax.set_xlabel('s')
                     self.ax.set_ylabel('u')
                     self.ax.set_zlabel('c')
                 self.fig.canvas.draw()
                 plt.pause(0.1)
         return perform_update
 
-
-    def save_dyn_plot(self, c, u, s, c_sw, u_sw, s_sw, tau_list, show_all=False):
+    def save_dyn_plot(self, c, u, s, c_sw, u_sw, s_sw, tau_list,
+                      show_all=False):
         if not os.path.exists(self.plot_path):
             os.makedirs(self.plot_path)
             if self.verbose >= 2:
                 print(f'{self.plot_path} directory created.')
 
         switch = np.sum(self.t_sw_array < 20)
         scale_back = np.array([self.scale_c, self.scale_u, self.scale_s])
@@ -1830,15 +2153,17 @@
         if switch == 3:
             c_sw3, u_sw3, s_sw3 = c_sw[2], u_sw[2], s_sw[2]
 
         if not show_all:
             n_anchors = len(u)
             t_lower = np.min(self.t)
             t_upper = np.max(self.t)
-            t_ = np.concatenate((tau_list[0], tau_list[1] + self.t_sw_array[0], tau_list[2] + self.t_sw_array[1], tau_list[3] + self.t_sw_array[2]))
+            t_ = np.concatenate((tau_list[0], tau_list[1] + self.t_sw_array[0],
+                                 tau_list[2] + self.t_sw_array[1],
+                                 tau_list[3] + self.t_sw_array[2]))
             c_pre = c[t_[:n_anchors] <= t_lower]
             u_pre = u[t_[:n_anchors] <= t_lower]
             s_pre = s[t_[:n_anchors] <= t_lower]
             c = c[(t_lower < t_[:n_anchors]) & (t_[:n_anchors] < t_upper)]
             u = u[(t_lower < t_[:n_anchors]) & (t_[:n_anchors] < t_upper)]
             s = s[(t_lower < t_[:n_anchors]) & (t_[:n_anchors] < t_upper)]
 
@@ -1846,308 +2171,405 @@
         u_all = self.u_all * self.scale_u + self.offset_u
         s_all = self.s_all * self.scale_s + self.offset_s
 
         fig = plt.figure(figsize=self.fig_size)
         fig.patch.set_facecolor('white')
         ax = fig.add_subplot(111, facecolor='white')
         if not show_all and len(u_pre) > 0:
-            ax.scatter(s_pre, u_pre, s=self.point_size/2, c='black', alpha=0.4, zorder=2)
+            ax.scatter(s_pre, u_pre, s=self.point_size/2, c='black',
+                       alpha=0.4, zorder=2)
         ax.scatter(s, u, s=self.point_size*1.5, c='black', alpha=0.6, zorder=2)
         for i in range(4):
             if any(self.state == i):
-                ax.scatter(s_all[(self.state == i) & (self.non_outlier)], u_all[(self.state == i) & (self.non_outlier)], s=self.point_size, c=self.color[i])
-        ax.scatter(s_all[~self.non_outlier], u_all[~self.non_outlier], s=self.point_size/2, c='grey')
+                ax.scatter(s_all[(self.state == i) & (self.non_outlier)],
+                           u_all[(self.state == i) & (self.non_outlier)],
+                           s=self.point_size, c=self.color[i])
+        ax.scatter(s_all[~self.non_outlier], u_all[~self.non_outlier],
+                   s=self.point_size/2, c='grey')
         if show_all or t_lower <= self.t_sw_array[0]:
-            ax.plot([s_sw1], [u_sw1], "om", markersize=self.point_size, zorder=5)
-        if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and t_upper >= self.t_sw_array[1])):
-            ax.plot([s_sw2], [u_sw2], "Xm", markersize=self.point_size, zorder=5)
-        if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and t_upper >= self.t_sw_array[2])):
-            ax.plot([s_sw3], [u_sw3], "Dm", markersize=self.point_size, zorder=5)
+            ax.plot([s_sw1], [u_sw1], "om", markersize=self.point_size,
+                    zorder=5)
+        if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and
+                                         t_upper >= self.t_sw_array[1])):
+            ax.plot([s_sw2], [u_sw2], "Xm", markersize=self.point_size,
+                    zorder=5)
+        if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and
+                                         t_upper >= self.t_sw_array[2])):
+            ax.plot([s_sw3], [u_sw3], "Dm", markersize=self.point_size,
+                    zorder=5)
         if np.max(self.t) == 20:
-            ax.plot([s[-1]], [u[-1]], "*m", markersize=self.point_size, zorder=5)
-        if self.anchor_t1_list is not None and len(self.anchor_t1_list) > 0 and show_all:
+            ax.plot([s[-1]], [u[-1]], "*m", markersize=self.point_size,
+                    zorder=5)
+        if (self.anchor_t1_list is not None and len(self.anchor_t1_list) > 0
+                and show_all):
             for i in range(len(self.anchor_t1_list)):
                 exp_t1 = self.anchor_t1_list[i] * scale_back + shift_back
                 exp_t2 = self.anchor_t2_list[i] * scale_back + shift_back
-                ax.plot([exp_t1[2]], [exp_t1[1]], "|y", markersize=self.point_size*1.5)
-                ax.plot([exp_t2[2]], [exp_t2[1]], "|c", markersize=self.point_size*1.5)
-        ax.plot(s_all, self.steady_state_func(self.s_all) * self.scale_u + self.offset_u, c='grey', ls=':', lw=self.point_size/4, alpha=0.7)
+                ax.plot([exp_t1[2]], [exp_t1[1]], "|y",
+                        markersize=self.point_size*1.5)
+                ax.plot([exp_t2[2]], [exp_t2[1]], "|c",
+                        markersize=self.point_size*1.5)
+        ax.plot(s_all,
+                self.steady_state_func(self.s_all) * self.scale_u
+                + self.offset_u, c='grey', ls=':', lw=self.point_size/4,
+                alpha=0.7)
         ax.set_xlabel('s')
         ax.set_ylabel('u')
         ax.set_title(f'{self.gene}-{self.model}')
         plt.tight_layout()
-        fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-us.png', dpi=fig.dpi, facecolor=fig.get_facecolor(), transparent=False, edgecolor='none')
+        fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-us.png',
+                    dpi=fig.dpi, facecolor=fig.get_facecolor(),
+                    transparent=False, edgecolor='none')
         plt.close(fig)
         plt.pause(0.2)
 
         if self.extra_color is not None:
             fig = plt.figure(figsize=self.fig_size)
             fig.patch.set_facecolor('white')
             ax = fig.add_subplot(111, facecolor='white')
             if not show_all and len(u_pre) > 0:
-                ax.scatter(s_pre, u_pre, s=self.point_size/2, c='black', alpha=0.4, zorder=2)
-            ax.scatter(s, u, s=self.point_size*1.5, c='black', alpha=0.6, zorder=2)
+                ax.scatter(s_pre, u_pre, s=self.point_size/2, c='black',
+                           alpha=0.4, zorder=2)
+            ax.scatter(s, u, s=self.point_size*1.5, c='black', alpha=0.6,
+                       zorder=2)
             ax.scatter(s_all, u_all, s=self.point_size, c=self.extra_color)
             if show_all or t_lower <= self.t_sw_array[0]:
-                ax.plot([s_sw1], [u_sw1], "om", markersize=self.point_size, zorder=5)
-            if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and t_upper >= self.t_sw_array[1])):
-                ax.plot([s_sw2], [u_sw2], "Xm", markersize=self.point_size, zorder=5)
-            if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and t_upper >= self.t_sw_array[2])):
-                ax.plot([s_sw3], [u_sw3], "Dm", markersize=self.point_size, zorder=5)
+                ax.plot([s_sw1], [u_sw1], "om", markersize=self.point_size,
+                        zorder=5)
+            if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and
+                                             t_upper >= self.t_sw_array[1])):
+                ax.plot([s_sw2], [u_sw2], "Xm", markersize=self.point_size,
+                        zorder=5)
+            if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and
+                                             t_upper >= self.t_sw_array[2])):
+                ax.plot([s_sw3], [u_sw3], "Dm", markersize=self.point_size,
+                        zorder=5)
             if np.max(self.t) == 20:
-                ax.plot([s[-1]], [u[-1]], "*m", markersize=self.point_size, zorder=5)
-            if self.anchor_t1_list is not None and len(self.anchor_t1_list) > 0 and show_all:
+                ax.plot([s[-1]], [u[-1]], "*m", markersize=self.point_size,
+                        zorder=5)
+            if (self.anchor_t1_list is not None and
+                    len(self.anchor_t1_list) > 0 and show_all):
                 for i in range(len(self.anchor_t1_list)):
                     exp_t1 = self.anchor_t1_list[i] * scale_back + shift_back
                     exp_t2 = self.anchor_t2_list[i] * scale_back + shift_back
-                    ax.plot([exp_t1[2]], [exp_t1[1]], "|y", markersize=self.point_size*1.5)
-                    ax.plot([exp_t2[2]], [exp_t2[1]], "|c", markersize=self.point_size*1.5)
-            ax.plot(s_all, self.steady_state_func(self.s_all) * self.scale_u + self.offset_u, c='grey', ls=':', lw=self.point_size/4, alpha=0.7)
+                    ax.plot([exp_t1[2]], [exp_t1[1]], "|y",
+                            markersize=self.point_size*1.5)
+                    ax.plot([exp_t2[2]], [exp_t2[1]], "|c",
+                            markersize=self.point_size*1.5)
+            ax.plot(s_all, self.steady_state_func(self.s_all) * self.scale_u
+                    + self.offset_u, c='grey', ls=':', lw=self.point_size/4,
+                    alpha=0.7)
             ax.set_xlabel('s')
             ax.set_ylabel('u')
             ax.set_title(f'{self.gene}-{self.model}')
             plt.tight_layout()
-            fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-us_colorby_extra.png', dpi=fig.dpi, facecolor=fig.get_facecolor(), transparent=False, edgecolor='none')
+            fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-'
+                        'us_colorby_extra.png', dpi=fig.dpi,
+                        facecolor=fig.get_facecolor(), transparent=False,
+                        edgecolor='none')
             plt.close(fig)
             plt.pause(0.2)
 
             if not self.rna_only:
                 fig = plt.figure(figsize=self.fig_size)
                 fig.patch.set_facecolor('white')
                 ax = fig.add_subplot(111, facecolor='white')
                 if not show_all and len(u_pre) > 0:
-                    ax.scatter(u_pre, c_pre, s=self.point_size/2, c='black', alpha=0.4, zorder=2)
-                ax.scatter(u, c, s=self.point_size*1.5, c='black', alpha=0.6, zorder=2)
+                    ax.scatter(u_pre, c_pre, s=self.point_size/2, c='black',
+                               alpha=0.4, zorder=2)
+                ax.scatter(u, c, s=self.point_size*1.5, c='black', alpha=0.6,
+                           zorder=2)
                 ax.scatter(u_all, c_all, s=self.point_size, c=self.extra_color)
                 if show_all or t_lower <= self.t_sw_array[0]:
-                    ax.plot([u_sw1], [c_sw1], "om", markersize=self.point_size, zorder=5)
-                if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and t_upper >= self.t_sw_array[1])):
-                    ax.plot([u_sw2], [c_sw2], "Xm", markersize=self.point_size, zorder=5)
-                if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and t_upper >= self.t_sw_array[2])):
-                    ax.plot([u_sw3], [c_sw3], "Dm", markersize=self.point_size, zorder=5)
+                    ax.plot([u_sw1], [c_sw1], "om", markersize=self.point_size,
+                            zorder=5)
+                if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1]
+                                                 and t_upper >=
+                                                 self.t_sw_array[1])):
+                    ax.plot([u_sw2], [c_sw2], "Xm", markersize=self.point_size,
+                            zorder=5)
+                if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2]
+                                                 and t_upper >=
+                                                 self.t_sw_array[2])):
+                    ax.plot([u_sw3], [c_sw3], "Dm", markersize=self.point_size,
+                            zorder=5)
                 if np.max(self.t) == 20:
-                    ax.plot([u[-1]], [c[-1]], "*m", markersize=self.point_size, zorder=5)
+                    ax.plot([u[-1]], [c[-1]], "*m", markersize=self.point_size,
+                            zorder=5)
                 ax.set_xlabel('u')
                 ax.set_ylabel('c')
                 ax.set_title(f'{self.gene}-{self.model}')
                 plt.tight_layout()
-                fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-cu_colorby_extra.png', dpi=fig.dpi, facecolor=fig.get_facecolor(), transparent=False, edgecolor='none')
+                fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-'
+                            'cu_colorby_extra.png', dpi=fig.dpi,
+                            facecolor=fig.get_facecolor(), transparent=False,
+                            edgecolor='none')
                 plt.close(fig)
                 plt.pause(0.2)
 
         if not self.rna_only:
             fig = plt.figure(figsize=self.fig_size)
             fig.patch.set_facecolor('white')
             ax = fig.add_subplot(111, projection='3d', facecolor='white')
             if not show_all and len(u_pre) > 0:
-                ax.scatter(s_pre, u_pre, c_pre, s=self.point_size/2, c='black', alpha=0.4, zorder=2)
-            ax.scatter(s, u, c, s=self.point_size*1.5, c='black', alpha=0.6, zorder=2)
+                ax.scatter(s_pre, u_pre, c_pre, s=self.point_size/2, c='black',
+                           alpha=0.4, zorder=2)
+            ax.scatter(s, u, c, s=self.point_size*1.5, c='black', alpha=0.6,
+                       zorder=2)
             for i in range(4):
                 if any(self.state == i):
-                    ax.scatter(s_all[(self.state == i) & (self.non_outlier)], 
-                               u_all[(self.state == i) & (self.non_outlier)], 
-                               c_all[(self.state == i) & (self.non_outlier)], 
+                    ax.scatter(s_all[(self.state == i) & (self.non_outlier)],
+                               u_all[(self.state == i) & (self.non_outlier)],
+                               c_all[(self.state == i) & (self.non_outlier)],
                                s=self.point_size, c=self.color[i])
-            ax.scatter(s_all[~self.non_outlier], u_all[~self.non_outlier], c_all[~self.non_outlier], s=self.point_size/2, c='grey')
+            ax.scatter(s_all[~self.non_outlier], u_all[~self.non_outlier],
+                       c_all[~self.non_outlier], s=self.point_size/2, c='grey')
             if show_all or t_lower <= self.t_sw_array[0]:
-                ax.plot([s_sw1], [u_sw1], [c_sw1], "om", markersize=self.point_size, zorder=5)
-            if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and t_upper >= self.t_sw_array[1])):
-                ax.plot([s_sw2], [u_sw2], [c_sw2], "Xm", markersize=self.point_size, zorder=5)
-            if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and t_upper >= self.t_sw_array[2])):
-                ax.plot([s_sw3], [u_sw3], [c_sw3], "Dm", markersize=self.point_size, zorder=5)
+                ax.plot([s_sw1], [u_sw1], [c_sw1], "om",
+                        markersize=self.point_size, zorder=5)
+            if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and
+                                             t_upper >= self.t_sw_array[1])):
+                ax.plot([s_sw2], [u_sw2], [c_sw2], "Xm",
+                        markersize=self.point_size, zorder=5)
+            if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and
+                                             t_upper >= self.t_sw_array[2])):
+                ax.plot([s_sw3], [u_sw3], [c_sw3], "Dm",
+                        markersize=self.point_size, zorder=5)
             if np.max(self.t) == 20:
-                ax.plot([s[-1]], [u[-1]], [c[-1]], "*m", markersize=self.point_size, zorder=5)
+                ax.plot([s[-1]], [u[-1]], [c[-1]], "*m",
+                        markersize=self.point_size, zorder=5)
             ax.set_xlabel('s')
             ax.set_ylabel('u')
             ax.set_zlabel('c')
             ax.set_title(f'{self.gene}-{self.model}')
             plt.tight_layout()
-            fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-cus.png', dpi=fig.dpi, facecolor=fig.get_facecolor(), transparent=False, edgecolor='none')
+            fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-cus.png',
+                        dpi=fig.dpi, facecolor=fig.get_facecolor(),
+                        transparent=False, edgecolor='none')
             plt.close(fig)
             plt.pause(0.2)
 
             fig = plt.figure(figsize=self.fig_size)
             fig.patch.set_facecolor('white')
             ax = fig.add_subplot(111, facecolor='white')
             if not show_all and len(u_pre) > 0:
-                ax.scatter(s_pre, u_pre, s=self.point_size/2, c='black', alpha=0.4, zorder=2)
-            ax.scatter(s, u, s=self.point_size*1.5, c='black', alpha=0.6, zorder=2)
-            ax.scatter(s_all, u_all, s=self.point_size, c=np.log1p(self.c_all), cmap='coolwarm')
+                ax.scatter(s_pre, u_pre, s=self.point_size/2, c='black',
+                           alpha=0.4, zorder=2)
+            ax.scatter(s, u, s=self.point_size*1.5, c='black', alpha=0.6,
+                       zorder=2)
+            ax.scatter(s_all, u_all, s=self.point_size, c=np.log1p(self.c_all),
+                       cmap='coolwarm')
             if show_all or t_lower <= self.t_sw_array[0]:
-                ax.plot([s_sw1], [u_sw1], "om", markersize=self.point_size, zorder=5)
-            if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and t_upper >= self.t_sw_array[1])):
-                ax.plot([s_sw2], [u_sw2], "Xm", markersize=self.point_size, zorder=5)
-            if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and t_upper >= self.t_sw_array[2])):
-                ax.plot([s_sw3], [u_sw3], "Dm", markersize=self.point_size, zorder=5)
+                ax.plot([s_sw1], [u_sw1], "om", markersize=self.point_size,
+                        zorder=5)
+            if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and
+                                             t_upper >= self.t_sw_array[1])):
+                ax.plot([s_sw2], [u_sw2], "Xm", markersize=self.point_size,
+                        zorder=5)
+            if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and
+                                             t_upper >= self.t_sw_array[2])):
+                ax.plot([s_sw3], [u_sw3], "Dm", markersize=self.point_size,
+                        zorder=5)
             if np.max(self.t) == 20:
-                ax.plot([s[-1]], [u[-1]], "*m", markersize=self.point_size, zorder=5)
-            ax.plot(s_all, self.steady_state_func(self.s_all) * self.scale_u + self.offset_u, c='grey', ls=':', lw=self.point_size/4, alpha=0.7)
+                ax.plot([s[-1]], [u[-1]], "*m", markersize=self.point_size,
+                        zorder=5)
+            ax.plot(s_all, self.steady_state_func(self.s_all) * self.scale_u +
+                    self.offset_u, c='grey', ls=':', lw=self.point_size/4,
+                    alpha=0.7)
             ax.set_xlabel('s')
             ax.set_ylabel('u')
             ax.set_title(f'{self.gene}-{self.model}')
             plt.tight_layout()
-            fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-us_colorby_c.png', dpi=fig.dpi, facecolor=fig.get_facecolor(), transparent=False, edgecolor='none')
+            fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-'
+                        'us_colorby_c.png', dpi=fig.dpi,
+                        facecolor=fig.get_facecolor(), transparent=False,
+                        edgecolor='none')
             plt.close(fig)
             plt.pause(0.2)
 
             fig = plt.figure(figsize=self.fig_size)
             fig.patch.set_facecolor('white')
             ax = fig.add_subplot(111, facecolor='white')
             if not show_all and len(u_pre) > 0:
-                ax.scatter(u_pre, c_pre, s=self.point_size/2, c='black', alpha=0.4, zorder=2)
-            ax.scatter(u, c, s=self.point_size*1.5, c='black', alpha=0.6, zorder=2)
+                ax.scatter(u_pre, c_pre, s=self.point_size/2, c='black',
+                           alpha=0.4, zorder=2)
+            ax.scatter(u, c, s=self.point_size*1.5, c='black', alpha=0.6,
+                       zorder=2)
             for i in range(4):
                 if any(self.state == i):
-                    ax.scatter(u_all[(self.state == i) & (self.non_outlier)], c_all[(self.state == i) & (self.non_outlier)], s=self.point_size, c=self.color[i])
-            ax.scatter(u_all[~self.non_outlier], c_all[~self.non_outlier], s=self.point_size/2, c='grey')
+                    ax.scatter(u_all[(self.state == i) & (self.non_outlier)],
+                               c_all[(self.state == i) & (self.non_outlier)],
+                               s=self.point_size, c=self.color[i])
+            ax.scatter(u_all[~self.non_outlier], c_all[~self.non_outlier],
+                       s=self.point_size/2, c='grey')
             if show_all or t_lower <= self.t_sw_array[0]:
-                ax.plot([u_sw1], [c_sw1], "om", markersize=self.point_size, zorder=5)
-            if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and t_upper >= self.t_sw_array[1])):
-                ax.plot([u_sw2], [c_sw2], "Xm", markersize=self.point_size, zorder=5)
-            if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and t_upper >= self.t_sw_array[2])):
-                ax.plot([u_sw3], [c_sw3], "Dm", markersize=self.point_size, zorder=5)
+                ax.plot([u_sw1], [c_sw1], "om", markersize=self.point_size,
+                        zorder=5)
+            if switch >= 2 and (show_all or (t_lower <= self.t_sw_array[1] and
+                                             t_upper >= self.t_sw_array[1])):
+                ax.plot([u_sw2], [c_sw2], "Xm", markersize=self.point_size,
+                        zorder=5)
+            if switch >= 3 and (show_all or (t_lower <= self.t_sw_array[2] and
+                                             t_upper >= self.t_sw_array[2])):
+                ax.plot([u_sw3], [c_sw3], "Dm", markersize=self.point_size,
+                        zorder=5)
             if np.max(self.t) == 20:
-                ax.plot([u[-1]], [c[-1]], "*m", markersize=self.point_size, zorder=5)
+                ax.plot([u[-1]], [c[-1]], "*m", markersize=self.point_size,
+                        zorder=5)
             ax.set_xlabel('u')
             ax.set_ylabel('c')
             ax.set_title(f'{self.gene}-{self.model}')
             plt.tight_layout()
-            fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-cu.png', dpi=fig.dpi, facecolor=fig.get_facecolor(), transparent=False, edgecolor='none')
+            fig.savefig(f'{self.plot_path}/{self.gene}-{self.model}-cu.png',
+                        dpi=fig.dpi, facecolor=fig.get_facecolor(),
+                        transparent=False, edgecolor='none')
             plt.close(fig)
             plt.pause(0.2)
 
-
     def get_loss(self):
         return self.loss
 
-
     def get_model(self):
         return self.model
 
-
     def get_params(self):
-        return self.t_sw_array, self.rates, self.scale_cc, self.rescale_c, self.rescale_u, self.realign_ratio
-
+        return self.t_sw_array, self.rates, self.scale_cc, self.rescale_c, \
+            self.rescale_u, self.realign_ratio
 
     def is_partial(self):
         return self.partial
 
-
     def get_direction(self):
         return self.direction
 
-
     def realign_time_and_velocity(self, c, u, s, anchor_time):
         # realign time to range (0,20)
         self.anchor_min_idx = np.sum(anchor_time < (np.min(self.t)-1e-5))
-        self.anchor_max_idx = np.sum(anchor_time < (np.max(self.t)-1e-5))# - 1
+        self.anchor_max_idx = np.sum(anchor_time < (np.max(self.t)-1e-5))
         self.c0 = c[self.anchor_min_idx]
         self.u0 = u[self.anchor_min_idx]
         self.s0 = s[self.anchor_min_idx]
         self.realign_ratio = 20 / (np.max(self.t) - np.min(self.t))
         if self.verbose >= 1:
-            print(f'fitted params: {self.t_sw_array} {self.rates} {self.scale_cc} {self.rescale_c} {self.rescale_u}')
+            print(f'fitted params: {self.t_sw_array} {self.rates} '
+                  '{self.scale_cc} {self.rescale_c} {self.rescale_u}')
             print(f'aligning to range (0,20) by {self.realign_ratio}..')
         self.rates /= self.realign_ratio
         self.alpha_c, self.alpha, self.beta, self.gamma = self.rates
         self.params[3:7] = self.rates
-        self.t_sw_array = (self.t_sw_array - np.min(self.t)) * self.realign_ratio
+        self.t_sw_array = ((self.t_sw_array - np.min(self.t))
+                           * self.realign_ratio)
         self.t_sw_1, self.t_sw_2, self.t_sw_3 = self.t_sw_array
-        self.params[:3] = np.array([self.t_sw_1, self.t_sw_2 - self.t_sw_1, self.t_sw_3 - self.t_sw_2])
+        self.params[:3] = np.array([self.t_sw_1, self.t_sw_2 - self.t_sw_1,
+                                    self.t_sw_3 - self.t_sw_2])
         self.t -= np.min(self.t)
         self.t = self.t * 20 / np.max(self.t)
         self.velocity /= self.realign_ratio
-        self.velocity[:,0] = np.clip(self.velocity[:,0], -self.c_all * self.scale_c, None)
-        self.velocity[:,1] = np.clip(self.velocity[:,1], -self.u_all * self.scale_u, None)
-        self.velocity[:,2] = np.clip(self.velocity[:,2], -self.s_all * self.scale_s, None)
+        self.velocity[:, 0] = np.clip(self.velocity[:, 0], -self.c_all
+                                      * self.scale_c, None)
+        self.velocity[:, 1] = np.clip(self.velocity[:, 1], -self.u_all
+                                      * self.scale_u, None)
+        self.velocity[:, 2] = np.clip(self.velocity[:, 2], -self.s_all
+                                      * self.scale_s, None)
         self.anchor_velo /= self.realign_ratio
-        self.anchor_velo[:,0] = np.clip(self.anchor_velo[:,0], -np.max(self.c_all * self.scale_c), None)
-        self.anchor_velo[:,1] = np.clip(self.anchor_velo[:,1], -np.max(self.u_all * self.scale_u), None)
-        self.anchor_velo[:,2] = np.clip(self.anchor_velo[:,2], -np.max(self.s_all * self.scale_s), None)
-
+        self.anchor_velo[:, 0] = np.clip(self.anchor_velo[:, 0],
+                                         -np.max(self.c_all * self.scale_c),
+                                         None)
+        self.anchor_velo[:, 1] = np.clip(self.anchor_velo[:, 1],
+                                         -np.max(self.u_all * self.scale_u),
+                                         None)
+        self.anchor_velo[:, 2] = np.clip(self.anchor_velo[:, 2],
+                                         -np.max(self.s_all * self.scale_s),
+                                         None)
 
     def get_initial_exp(self):
         return np.array([self.c0, self.u0, self.s0])
 
-
     def get_time_assignment(self):
         if self.low_quality:
             return np.zeros(len(self.u_all))
         return self.t
 
-
     def get_state_assignment(self):
         if self.low_quality:
             return np.zeros(len(self.u_all))
         return self.state
 
-
     def get_velocity(self):
         if self.low_quality:
             return np.zeros((len(self.u_all), 3))
         return self.velocity
 
-
     def get_likelihood(self):
         return self.likelihood, self.l_c, self.ssd_c, self.var_c
 
-
     def get_anchors(self):
         if self.low_quality:
-            return (np.zeros((1, 3)), np.zeros((1, 3)), np.zeros((1, 3)), 0, 0, 0, 0)
-        return self.anchor_exp, self.anchor_exp_sw, self.anchor_velo, self.anchor_min_idx, self.anchor_max_idx, self.anchor_velo_min_idx, self.anchor_velo_max_idx
+            return (np.zeros((1, 3)), np.zeros((1, 3)), np.zeros((1, 3)),
+                    0, 0, 0, 0)
+        return self.anchor_exp, self.anchor_exp_sw, self.anchor_velo, \
+            self.anchor_min_idx, self.anchor_max_idx, \
+            self.anchor_velo_min_idx, self.anchor_velo_max_idx
+
 
+def regress_func(c, u, s, m, mi, im, gpdist, embed, conn, v, pl, sp, pdir, fa,
+                 gene, pa, di, ro, fit, fd, extra, ru, alpha, beta, gamma, t_):
 
-def regress_func(c,u,s,m,mi,im,gpdist,embed,conn,v,pl,sp,pdir,fa,gene,pa,di,ro,fit,fd,extra,ru,alpha,beta,gamma,t_):
     if v >= 1 and m is not None:
-        print('###############################################################################################')
+        print('###############################################################'
+              '################################')
         print(f'testing model {m}')
 
     c_90 = np.percentile(c, 90)
     u_90 = np.percentile(u, 90)
     s_90 = np.percentile(s, 90)
-    low_quality = (u_90 == 0 or s_90 == 0) if ro else (c_90 == 0 or u_90 == 0 or s_90 == 0)
+    low_quality = (u_90 == 0 or s_90 == 0) if ro else (c_90 == 0 or u_90 == 0
+                                                       or s_90 == 0)
     if low_quality:
         if v >= 1:
             print(f'low quality gene {gene}, skipping')
-        return (np.inf, np.nan, '', (np.zeros(3), np.zeros(4), 0, 0, 0, 0), np.zeros(3), np.zeros(len(u)), np.zeros(len(u)), 
-                np.zeros((len(u), 3)), (-1.0, 0, 0, 0), (np.zeros((1, 3)), np.zeros((1, 3)), np.zeros((1, 3)), 0, 0, 0, 0))
+        return (np.inf, np.nan, '', (np.zeros(3), np.zeros(4), 0, 0, 0, 0),
+                np.zeros(3), np.zeros(len(u)), np.zeros(len(u)),
+                np.zeros((len(u), 3)), (-1.0, 0, 0, 0),
+                (np.zeros((1, 3)), np.zeros((1, 3)), np.zeros((1, 3)), 0, 0,
+                 0, 0))
 
     if gpdist is not None:
         subset_cells = s > 0.1 * np.percentile(s, 99)
         subset_cells = np.where(subset_cells)[0]
         if len(subset_cells) > 3000:
             rng = np.random.default_rng(2021)
             subset_cells = rng.choice(subset_cells, 3000, replace=False)
         local_pdist = gpdist[np.ix_(subset_cells, subset_cells)]
-        dists = np.ravel(local_pdist[np.triu_indices_from(local_pdist, k=1)]).reshape(-1, 1)
+        dists = (np.ravel(local_pdist[np.triu_indices_from(local_pdist, k=1)])
+                 .reshape(-1, 1))
         local_std = np.std(dists)
     else:
         local_std = None
 
-    cdc = ChromatinDynamical(c, 
-                             u, 
-                             s, 
-                             model=m, 
-                             max_iter=mi, 
-                             init_mode=im, 
-                             local_std=local_std, 
-                             embed_coord=embed, 
-                             connectivities=conn, 
-                             verbose=v, 
-                             plot=pl, 
-                             save_plot=sp, 
-                             plot_dir=pdir, 
-                             fit_args=fa, 
-                             gene=gene, 
-                             partial=pa, 
-                             direction=di, 
-                             rna_only=ro, 
-                             fit_decoupling=fd, 
-                             extra_color=extra, 
+    cdc = ChromatinDynamical(c,
+                             u,
+                             s,
+                             model=m,
+                             max_iter=mi,
+                             init_mode=im,
+                             local_std=local_std,
+                             embed_coord=embed,
+                             connectivities=conn,
+                             verbose=v,
+                             plot=pl,
+                             save_plot=sp,
+                             plot_dir=pdir,
+                             fit_args=fa,
+                             gene=gene,
+                             partial=pa,
+                             direction=di,
+                             rna_only=ro,
+                             fit_decoupling=fd,
+                             extra_color=extra,
                              rescale_u=ru,
                              alpha=alpha,
                              beta=beta,
                              gamma=gamma,
                              t_=t_)
     if fit:
         loss = cdc.fit()
@@ -2159,74 +2581,55 @@
     parameters = cdc.get_params()
     initial_exp = cdc.get_initial_exp()
     velocity = cdc.get_velocity()
     likelihood = cdc.get_likelihood()
     time = cdc.get_time_assignment()
     state = cdc.get_state_assignment()
     anchors = cdc.get_anchors()
-    return loss[-1], model, direction, parameters, initial_exp, time, state, velocity, likelihood, anchors
+    return loss[-1], model, direction, parameters, initial_exp, time, state, \
+        velocity, likelihood, anchors
 
 
-def multimodel_helper(c, u, s, 
-                      model_to_run, 
-                      max_iter, 
-                      init_mode, 
-                      global_pdist, 
-                      embed_coord, 
-                      conn, 
-                      verbose, 
-                      plot, 
-                      save_plot, 
-                      plot_dir, 
-                      fit_args, 
-                      gene, 
-                      partial, 
-                      direction, 
-                      rna_only, 
-                      fit, 
-                      fit_decoupling, 
-                      extra_color, 
-                      rescale_u, 
-                      alpha, 
-                      beta, 
-                      gamma, 
+def multimodel_helper(c, u, s,
+                      model_to_run,
+                      max_iter,
+                      init_mode,
+                      global_pdist,
+                      embed_coord,
+                      conn,
+                      verbose,
+                      plot,
+                      save_plot,
+                      plot_dir,
+                      fit_args,
+                      gene,
+                      partial,
+                      direction,
+                      rna_only,
+                      fit,
+                      fit_decoupling,
+                      extra_color,
+                      rescale_u,
+                      alpha,
+                      beta,
+                      gamma,
                       t_
                       ):
 
     loss, param_cand, initial_cand, time_cand = [], [], [], []
     state_cand, velo_cand, likelihood_cand, anch_cand = [], [], [], []
 
     for model in model_to_run:
-        (loss_m, _, direction_, parameters, initial_exp, 
-         time, state, velocity, likelihood, anchors) = regress_func(c, 
-                                                                    u, 
-                                                                    s, 
-                                                                    model, 
-                                                                    max_iter, 
-                                                                    init_mode, 
-                                                                    global_pdist, 
-                                                                    embed_coord, 
-                                                                    conn, 
-                                                                    verbose, 
-                                                                    plot, 
-                                                                    save_plot, 
-                                                                    plot_dir, 
-                                                                    fit_args, 
-                                                                    gene, 
-                                                                    partial, 
-                                                                    direction, 
-                                                                    rna_only, 
-                                                                    fit, 
-                                                                    fit_decoupling, 
-                                                                    extra_color, 
-                                                                    rescale_u,
-                                                                    alpha,
-                                                                    beta,
-                                                                    gamma,
-                                                                    t_)
+        (loss_m, _, direction_, parameters, initial_exp,
+         time, state, velocity, likelihood, anchors) = \
+         regress_func(c, u, s, model, max_iter, init_mode, global_pdist,
+                      embed_coord, conn, verbose, plot, save_plot, plot_dir,
+                      fit_args, gene, partial, direction, rna_only, fit,
+                      fit_decoupling, extra_color, rescale_u, alpha, beta,
+                      gamma, t_)
         loss.append(loss_m)
         param_cand.append(parameters)
         initial_cand.append(initial_exp)
         time_cand.append(time)
         state_cand.append(state)
         velo_cand.append(velocity)
         likelihood_cand.append(likelihood)
@@ -2237,149 +2640,170 @@
     parameters = param_cand[best_model]
     initial_exp = initial_cand[best_model]
     time = time_cand[best_model]
     state = state_cand[best_model]
     velocity = velo_cand[best_model]
     likelihood = likelihood_cand[best_model]
     anchors = anch_cand[best_model]
-    return loss, model, direction_, parameters, initial_exp, time, state, velocity, likelihood, anchors
+    return loss, model, direction_, parameters, initial_exp, time, state,\
+        velocity, likelihood, anchors
 
 
-def recover_dynamics_chrom(adata_rna, 
-                           adata_atac=None, 
-                           gene_list=None, 
-                           max_iter=5, 
-                           init_mode='invert', 
-                           model_to_run=None, 
-                           verbose=False, 
-                           plot=False, 
-                           parallel=True, 
-                           n_jobs=None, 
-                           save_plot=False, 
+def recover_dynamics_chrom(adata_rna,
+                           adata_atac=None,
+                           gene_list=None,
+                           max_iter=5,
+                           init_mode='invert',
+                           model_to_run=None,
+                           verbose=False,
+                           plot=False,
+                           parallel=True,
+                           n_jobs=None,
+                           save_plot=False,
                            plot_dir=None,
-                           rna_only=False, 
-                           fit=True, 
-                           fit_decoupling=True, 
-                           extra_color_key=None, 
-                           embedding='X_umap', 
-                           n_anchors=500, 
-                           k_dist=1, 
-                           thresh_multiplier=1.0, 
-                           weight_c=0.6, 
-                           outlier=99.8, 
-                           n_pcs=30, 
-                           n_neighbors=30, 
-                           fig_size=(8,6), 
-                           point_size=7, 
-                           partial=None, 
-                           direction=None, 
-                           rescale_u=None, 
-                           alpha=None, 
-                           beta=None, 
-                           gamma=None, 
+                           rna_only=False,
+                           fit=True,
+                           fit_decoupling=True,
+                           extra_color_key=None,
+                           embedding='X_umap',
+                           n_anchors=500,
+                           k_dist=1,
+                           thresh_multiplier=1.0,
+                           weight_c=0.6,
+                           outlier=99.8,
+                           n_pcs=30,
+                           n_neighbors=30,
+                           fig_size=(8, 6),
+                           point_size=7,
+                           partial=None,
+                           direction=None,
+                           rescale_u=None,
+                           alpha=None,
+                           beta=None,
+                           gamma=None,
                            t_sw=None
                            ):
 
     """Multi-omic dynamics recovery.
 
-    This function optimizes the joint chromatin and RNA model parameters in ODE solutions.
+    This function optimizes the joint chromatin and RNA model parameters in
+    ODE solutions.
 
     Parameters
     ----------
     adata_rna: :class:`~anndata.AnnData`
         RNA anndata object. Required fields: `Mu`, `Ms`, and `connectivities`.
     adata_atac: :class:`~anndata.AnnData` (default: `None`)
         ATAC anndata object. Required fields: `Mc`.
     gene_list: `str`,  list of `str` (default: highly variable genes)
         Genes to use for model fitting.
     max_iter: `int` (default: `5`)
         Iterations to run for parameter optimization.
     init_mode: `str` (default: `'invert'`)
         Initialization method for switch times.
-        `'invert'`: initial RNA switch time will be computed with scVelo time inversion method.
+        `'invert'`: initial RNA switch time will be computed with scVelo time
+        inversion method.
         `'grid'`: grid search the best set of switch times.
         `'simple'`: simply initialize switch times to be 5, 10, and 15.
     model_to_run: `int` or list of `int` (default: `None`)
-        User specified models for each genes. Possible values are 1 are 2. If `None`, the model 
-        for each gene will be inferred based on expression patterns. If more than one value is given, 
+        User specified models for each genes. Possible values are 1 are 2. If
+        `None`, the model
+        for each gene will be inferred based on expression patterns. If more
+        than one value is given,
         the best model will be decided based on loss of fit.
     verbose: `int` or `bool` (default: `False`)
-        Level of fitting detail to output. Possible values: `False`, 0, 1, 2, or any number above 2.
+        Level of fitting detail to output. Possible values: `False`, 0, 1, 2,
+        or any number above 2.
     plot: `bool` or `None` (default: `False`)
-        Whether to interactively plot the 3D gene portraits. Ignored if parallel is True.
+        Whether to interactively plot the 3D gene portraits. Ignored if
+        parallel is True.
     parallel: `bool` (default: `True`)
         Whether to fit genes in a parallel fashion (recommended).
     n_jobs: `int` (default: available threads)
         Number of parallel jobs.
     save_plot: `bool` (default: `False`)
-        Whether to save the fitted gene portrait figures as files. This will take some disk space.
-    plot_dir: `str` (default: `plots` for multiome and `rna_plots` for RNA-only)
+        Whether to save the fitted gene portrait figures as files. This will
+        take some disk space.
+    plot_dir: `str` (default: `plots` for multiome and `rna_plots` for
+    RNA-only)
         Directory to save the plots.
     rna_only: `bool` (default: `False`)
         Whether to only use RNA for fitting (RNA velocity).
     fit: `bool` (default: `True`)
-        Whether to fit the models. If False, only pre-determination and initialization will be run.
+        Whether to fit the models. If False, only pre-determination and
+        initialization will be run.
     fit_decoupling: `bool` (default: `True`)
         Whether to fit decoupling phase (Model 1 vs Model 2 distinction).
     n_anchors: `int` (default: 500)
-        Number of anchor time-points to generate as a representation of the trajectory.
+        Number of anchor time-points to generate as a representation of the
+        trajectory.
     k_dist: `int` (default: 1)
-        Number of anchors to use to determine a cell's gene time. If more than 1, time will be averaged.
+        Number of anchors to use to determine a cell's gene time. If more than
+        1, time will be averaged.
     thresh_multiplier: `float` (default: 1.0)
-        Multiplier for the heuristic threshold of partial versus complete trajectory pre-determination.
+        Multiplier for the heuristic threshold of partial versus complete
+        trajectory pre-determination.
     weight_c: `float` (default: 0.6)
-        Weighting of scaled chromatin distances when performing 3D residual calculation.
+        Weighting of scaled chromatin distances when performing 3D residual
+        calculation.
     outlier: `float` (default: 99.8)
-        The percentile to mark as outlier that will be excluded when fitting the model.
+        The percentile to mark as outlier that will be excluded when fitting
+        the model.
     n_pcs: `int` (default: 30)
-        Number of principal components to compute distance smoothing neighbors. 
+        Number of principal components to compute distance smoothing neighbors.
         This can be different from the one used for expression smoothing.
     n_neighbors: `int` (default: 30)
-        Number of nearest neighbors for distance smoothing. 
+        Number of nearest neighbors for distance smoothing.
         This can be different from the one used for expression smoothing.
     fig_size: `tuple` (default: (8,6))
         Size of each figure when saved.
     point_size: `float` (default: 7)
         Marker point size for plotting.
     extra_color_key: `str` (default: `None`)
-        Extra color key used for plotting. Common choices are `leiden`, `celltype`, etc. 
-        The colors for each category must be present in one of anndatas, which can be pre-computed 
+        Extra color key used for plotting. Common choices are `leiden`,
+        `celltype`, etc.
+        The colors for each category must be present in one of anndatas, which
+        can be pre-computed
         with `scanpy.pl.scatter` function.
     embedding: `str` (default: `X_umap`)
         2D coordinates of the low-dimensional embedding of cells.
     partial: `bool` or list of `bool` (default: `None`)
         User specified trajectory completeness for each gene.
     direction: `str` or list of `str` (default: `None`)
         User specified trajectory directionality for each gene.
     rescale_u: `float` or list of `float` (default: `None`)
-        Known scaling factors for unspliced. Can be computed from scVelo `fit_scaling` values 
+        Known scaling factors for unspliced. Can be computed from scVelo
+        `fit_scaling` values
         as `rescale_u = fit_scaling / std(u) * std(s)`.
     alpha: `float` or list of `float` (default: `None`)
-        Known trascription rates. Can be computed from scVelo `fit_alpha` values 
+        Known trascription rates. Can be computed from scVelo `fit_alpha`
+        values
         as `alpha = fit_alpha * fit_alignment_scaling`.
     beta: `float` or list of `float` (default: `None`)
-        Known splicing rates. Can be computed from scVelo `fit_alpha` values 
+        Known splicing rates. Can be computed from scVelo `fit_alpha` values
         as `beta = fit_beta * fit_alignment_scaling`.
     gamma: `float` or list of `float` (default: `None`)
-        Known degradation rates. Can be computed from scVelo `fit_gamma` values 
+        Known degradation rates. Can be computed from scVelo `fit_gamma` values
         as `gamma = fit_gamma * fit_alignment_scaling`.
     t_sw: `float` or list of `float` (default: `None`)
-        Known RNA switch time. Can be computed from scVelo `fit_t_` values 
+        Known RNA switch time. Can be computed from scVelo `fit_t_` values
         as `t_sw = fit_t_ / fit_alignment_scaling`.
 
     Returns
     -------
     fit_alpha_c, fit_alpha, fit_beta, fit_gamma: `.var`
-        inferred chromatin opening, transcription, splicing, and degradation (nuclear export) rates
+        inferred chromatin opening, transcription, splicing, and degradation
+        (nuclear export) rates
     fit_t_sw1, fit_t_sw2, fit_t_sw3: `.var`
         inferred switching time points
     fit_rescale_c, fit_rescale_u: `.var`
         inferred scaling factor for chromatin and unspliced counts
     fit_scale_cc: `.var`
-        inferred scaling value for chromatin closing rate compared to opening rate
+        inferred scaling value for chromatin closing rate compared to opening
+        rate
     fit_alignment_scaling: `.var`
         ratio used to realign observed time range to 0-20
     fit_c0, fit_u0, fit_s0: `.var`
         initial expression values at earliest observed time
     fit_model: `.var`
         inferred gene model
     fit_direction: `.var`
@@ -2432,75 +2856,91 @@
     fit_args['n_neighbors'] = n_neighbors
     fit_args['fig_size'] = list(fig_size)
     fit_args['point_size'] = point_size
 
     all_genes = adata_rna.var_names
     if adata_atac is None:
         import anndata as ad
-        from scipy.sparse import diags
         rna_only = True
-        adata_atac = ad.AnnData(X=np.ones(adata_rna.shape), obs=adata_rna.obs, var=adata_rna.var)
+        adata_atac = ad.AnnData(X=np.ones(adata_rna.shape), obs=adata_rna.obs,
+                                var=adata_rna.var)
         adata_atac.layers['Mc'] = np.ones(adata_rna.shape)
     if adata_rna.shape != adata_atac.shape:
-        raise ValueError(f'Shape of RNA and ATAC adata objects do not match: {adata_rna.shape} {adata_atac.shape}')
+        raise ValueError('Shape of RNA and ATAC adata objects do not match: '
+                         f'{adata_rna.shape} {adata_atac.shape}')
     if not np.all(adata_rna.obs_names == adata_atac.obs_names):
-        raise ValueError('obs_names of RNA and ATAC adata objects do not match, please check if they are consistent')
+        raise ValueError('obs_names of RNA and ATAC adata objects do not '
+                         'match, please check if they are consistent')
     if not np.all(all_genes == adata_atac.var_names):
-        raise ValueError('var_names of RNA and ATAC adata objects do not match, please check if they are consistent')
+        raise ValueError('var_names of RNA and ATAC adata objects do not '
+                         'match, please check if they are consistent')
     if 'connectivities' not in adata_rna.obsp.keys():
         raise ValueError('Missing connectivities entry in RNA adata object')
     if extra_color_key is None:
         extra_color = None
-    elif isinstance(extra_color_key, str) and extra_color_key in adata_rna.obs and adata_rna.obs[extra_color_key].dtype.name == 'category':
+    elif (isinstance(extra_color_key, str) and extra_color_key in adata_rna.obs
+            and adata_rna.obs[extra_color_key].dtype.name == 'category'):
         ngroups = len(adata_rna.obs[extra_color_key].cat.categories)
-        extra_color = adata_rna.obs[extra_color_key].cat.rename_categories(adata_rna.uns[extra_color_key+'_colors'][:ngroups]).to_numpy()
-    elif isinstance(extra_color_key, str) and extra_color_key in adata_atac.obs and adata_rna.obs[extra_color_key].dtype.name == 'category':
+        extra_color = adata_rna.obs[extra_color_key].cat.rename_categories(
+            adata_rna.uns[extra_color_key+'_colors'][:ngroups]).to_numpy()
+    elif (isinstance(extra_color_key, str) and extra_color_key in
+          adata_atac.obs and
+          adata_rna.obs[extra_color_key].dtype.name == 'category'):
         ngroups = len(adata_atac.obs[extra_color_key].cat.categories)
-        extra_color = adata_atac.obs[extra_color_key].cat.rename_categories(adata_atac.uns[extra_color_key+'_colors'][:ngroups]).to_numpy()
+        extra_color = adata_atac.obs[extra_color_key].cat.rename_categories(
+            adata_atac.uns[extra_color_key+'_colors'][:ngroups]).to_numpy()
     else:
-        raise ValueError('Currently, extra_color_key must be a single string of categories and available in adata obs, and its colors can be found in adata uns')
-    if 'connectivities' not in adata_rna.obsp.keys() or (adata_rna.obsp['connectivities'] > 0).sum(1).min() > (n_neighbors-1):
+        raise ValueError('Currently, extra_color_key must be a single string '
+                         'of categories and available in adata obs, and its '
+                         'colors can be found in adata uns')
+    if ('connectivities' not in adata_rna.obsp.keys() or
+            (adata_rna.obsp['connectivities'] > 0).sum(1).min()
+            > (n_neighbors-1)):
         neighbors = Neighbors(adata_rna)
-        neighbors.compute_neighbors(n_neighbors=n_neighbors, knn=True, n_pcs=n_pcs)
+        neighbors.compute_neighbors(n_neighbors=n_neighbors, knn=True,
+                                    n_pcs=n_pcs)
         rna_conn = neighbors.connectivities
     else:
         rna_conn = adata_rna.obsp['connectivities'].copy()
-    #rna_conn = top_n_sparse(rna_conn, n_neighbors)
     rna_conn.setdiag(1)
     rna_conn = rna_conn.multiply(1.0 / rna_conn.sum(1)).tocsr()
-    #integ_conn = None
     if not rna_only:
         if 'connectivities' not in adata_atac.obsp.keys():
-            print('Missing connectivities in ATAC adata object, using RNA connectivities instead')
+            print('Missing connectivities in ATAC adata object, using RNA'
+                  ' connectivities instead')
             atac_conn = rna_conn
         else:
             atac_conn = adata_atac.obsp['connectivities'].copy()
             atac_conn.setdiag(1)
         atac_conn = atac_conn.multiply(1.0 / atac_conn.sum(1)).tocsr()
-        #integ_conn = rna_conn + atac_conn
-        #integ_conn = integ_conn.multiply(1.0 / integ_conn.sum(1)).tocsr()
     if gene_list is None:
         if 'highly_variable' in adata_rna.var:
-            gene_list = adata_rna.var_names[adata_rna.var['highly_variable']].values
+            gene_list = adata_rna.var_names[adata_rna.var['highly_variable']]\
+                .values
         else:
-            gene_list = adata_rna.var_names.values[(~np.isnan(np.asarray(adata_rna.layers['Mu'].sum(0)).reshape(-1) 
-                                                                if sparse.issparse(adata_rna.layers['Mu']) 
-                                                                else np.sum(adata_rna.layers['Mu'], axis=0)))
-                                                   & (~np.isnan(np.asarray(adata_rna.layers['Ms'].sum(0)).reshape(-1) 
-                                                                if sparse.issparse(adata_rna.layers['Ms']) 
-                                                                else np.sum(adata_rna.layers['Ms'], axis=0)))
-                                                   & (~np.isnan(np.asarray(adata_atac.layers['Mc'].sum(0)).reshape(-1) 
-                                                                if sparse.issparse(adata_atac.layers['Mc']) 
-                                                                else np.sum(adata_atac.layers['Mc'], axis=0)))]
-    elif isinstance(gene_list,(list, np.ndarray, pd.Index, pd.Series)):
+            gene_list = adata_rna.var_names.values[
+                (~np.isnan(np.asarray(adata_rna.layers['Mu'].sum(0))
+                             .reshape(-1)
+                           if sparse.issparse(adata_rna.layers['Mu'])
+                           else np.sum(adata_rna.layers['Mu'], axis=0)))
+                & (~np.isnan(np.asarray(adata_rna.layers['Ms'].sum(0))
+                             .reshape(-1)
+                             if sparse.issparse(adata_rna.layers['Ms'])
+                             else np.sum(adata_rna.layers['Ms'], axis=0)))
+                & (~np.isnan(np.asarray(adata_atac.layers['Mc'].sum(0))
+                             .reshape(-1)
+                             if sparse.issparse(adata_atac.layers['Mc'])
+                             else np.sum(adata_atac.layers['Mc'], axis=0)))]
+    elif isinstance(gene_list, (list, np.ndarray, pd.Index, pd.Series)):
         gene_list = np.array([x for x in gene_list if x in all_genes])
     elif isinstance(gene_list, str):
         gene_list = np.array([gene_list]) if gene_list in all_genes else []
     else:
-        raise ValueError('Invalid gene list, must be one of (str, np.ndarray, pd.Index, pd.Series)')
+        raise ValueError('Invalid gene list, must be one of (str, np.ndarray,'
+                         'pd.Index, pd.Series)')
     gn = len(gene_list)
     if gn == 0:
         raise ValueError('None of the genes specified are in the adata object')
     if verbose is True:
         verbose = 1
     if verbose >= 1:
         print(f'{gn} genes will be fitted')
@@ -2541,93 +2981,113 @@
     if rna_only:
         model_to_run = [2]
         if verbose >= 1:
             print('Skipping model checking for RNA-only, running model 2')
 
     m_per_g = False
     if model_to_run is not None:
-        if isinstance(model_to_run,(list, np.ndarray, pd.Index, pd.Series)):
+        if isinstance(model_to_run, (list, np.ndarray, pd.Index, pd.Series)):
             model_to_run = [int(x) for x in model_to_run]
-            if np.any(~np.isin(model_to_run, [0,1,2])):
-                raise ValueError('Invalid model number (must be values in [0,1,2])')
+            if np.any(~np.isin(model_to_run, [0, 1, 2])):
+                raise ValueError('Invalid model number (must be values in'
+                                 ' [0,1,2])')
             if len(model_to_run) == gn:
                 losses = np.zeros((gn, 1))
                 m_per_g = True
                 func_to_call = regress_func
             else:
                 losses = np.zeros((gn, len(model_to_run)))
                 func_to_call = multimodel_helper
         elif isinstance(model_to_run, (int, float)):
             model_to_run = int(model_to_run)
-            if not np.isin(model_to_run, [0,1,2]):
-                raise ValueError('Invalid model number (must be values in [0,1,2])')
+            if not np.isin(model_to_run, [0, 1, 2]):
+                raise ValueError('Invalid model number (must be values in '
+                                 '[0,1,2])')
             model_to_run = [model_to_run]
             losses = np.zeros((gn, 1))
             func_to_call = multimodel_helper
         else:
-            raise ValueError('Invalid model number (must be values in [0,1,2])')
+            raise ValueError('Invalid model number (must be values in '
+                             '[0,1,2])')
     else:
         losses = np.zeros((gn, 1))
         func_to_call = regress_func
 
     p_per_g = False
     if partial is not None:
-        if isinstance(partial,(list, np.ndarray, pd.Index, pd.Series)):
+        if isinstance(partial, (list, np.ndarray, pd.Index, pd.Series)):
             if np.any(~np.isin(partial, [True, False])):
-                raise ValueError('Invalid partial argument (must be values in [True,False])')
+                raise ValueError('Invalid partial argument (must be values in'
+                                 ' [True,False])')
             if len(partial) == gn:
                 p_per_g = True
             else:
                 raise ValueError('Incorrect partial argument length')
         elif isinstance(partial, bool):
-            if not np.isin(partial, [True,False]):
-                raise ValueError('Invalid partial argument (must be values in [True,False])')
+            if not np.isin(partial, [True, False]):
+                raise ValueError('Invalid partial argument (must be values in'
+                                 ' [True,False])')
         else:
-            raise ValueError('Invalid partial argument (must be values in [True,False])')
+            raise ValueError('Invalid partial argument (must be values in'
+                             ' [True,False])')
 
     d_per_g = False
     if direction is not None:
-        if isinstance(direction,(list, np.ndarray, pd.Index, pd.Series)):
+        if isinstance(direction, (list, np.ndarray, pd.Index, pd.Series)):
             if np.any(~np.isin(direction, ['on', 'off', 'complete'])):
-                raise ValueError('Invalid direction argument (must be values in ["on","off","complete"])')
+                raise ValueError('Invalid direction argument (must be values'
+                                 ' in ["on","off","complete"])')
             if len(direction) == gn:
                 d_per_g = True
             else:
                 raise ValueError('Incorrect direction argument length')
         elif isinstance(direction, str):
             if not np.isin(direction, ['on', 'off', 'complete']):
-                raise ValueError('Invalid direction argument (must be values in ["on","off","complete"])')
+                raise ValueError('Invalid direction argument (must be values'
+                                 ' in ["on","off","complete"])')
         else:
-            raise ValueError('Invalid direction argument (must be values in ["on","off","complete"])')
+            raise ValueError('Invalid direction argument (must be values in'
+                             ' ["on","off","complete"])')
 
     known_pars = [rescale_u, alpha, beta, gamma, t_sw]
     for x in known_pars:
         if x is not None:
             if isinstance(x, (list, np.ndarray)):
                 if np.sum(np.isnan(x)) + np.sum(np.isinf(x)) > 0:
-                    raise ValueError('Known parameters cannot contain NaN or Inf')
+                    raise ValueError('Known parameters cannot contain NaN or'
+                                     ' Inf')
             elif isinstance(x, (int, float)):
                 if x == np.nan or x == np.inf:
-                    raise ValueError('Known parameters cannot contain NaN or Inf')
+                    raise ValueError('Known parameters cannot contain NaN or'
+                                     ' Inf')
             else:
                 raise ValueError('Invalid known parameters type')
 
-    if (embedding not in adata_rna.obsm) and (embedding not in adata_atac.obsm):
+    if ((embedding not in adata_rna.obsm) and
+            (embedding not in adata_atac.obsm)):
         raise ValueError(f'{embedding} is not found in obsm')
-    embed_coord = adata_rna.obsm[embedding] if embedding in adata_rna.obsm else adata_atac.obsm[embedding]
+    embed_coord = adata_rna.obsm[embedding] if embedding in adata_rna.obsm \
+        else adata_atac.obsm[embedding]
     global_pdist = pairwise_distances(embed_coord)
 
-    u_mat = adata_rna[:,gene_list].layers['Mu'].A if sparse.issparse(adata_rna.layers['Mu']) else adata_rna[:,gene_list].layers['Mu']
-    s_mat = adata_rna[:,gene_list].layers['Ms'].A if sparse.issparse(adata_rna.layers['Ms']) else adata_rna[:,gene_list].layers['Ms']
-    c_mat = adata_atac[:,gene_list].layers['Mc'].A if sparse.issparse(adata_atac.layers['Mc']) else adata_atac[:,gene_list].layers['Mc']
+    u_mat = adata_rna[:, gene_list].layers['Mu'].A \
+        if sparse.issparse(adata_rna.layers['Mu']) \
+        else adata_rna[:, gene_list].layers['Mu']
+    s_mat = adata_rna[:, gene_list].layers['Ms'].A \
+        if sparse.issparse(adata_rna.layers['Ms']) \
+        else adata_rna[:, gene_list].layers['Ms']
+    c_mat = adata_atac[:, gene_list].layers['Mc'].A \
+        if sparse.issparse(adata_atac.layers['Mc']) \
+        else adata_atac[:, gene_list].layers['Mc']
 
     ru = rescale_u if rescale_u is not None else None
 
     if parallel:
-        if n_jobs is None or not isinstance(n_jobs, int) or n_jobs < 0 or n_jobs > os.cpu_count():
+        if (n_jobs is None or not isinstance(n_jobs, int) or n_jobs < 0 or
+                n_jobs > os.cpu_count()):
             n_jobs = os.cpu_count()
         if n_jobs > gn:
             n_jobs = gn
         batches = -(-gn // n_jobs)
         if n_jobs > 1 and verbose >= 1:
             print(f'running {n_jobs} jobs in parallel')
     else:
@@ -2642,213 +3102,213 @@
         if parallel:
             verb = 5 if verbose >= 2 else 0
             verbose = False
             plot = False
 
             res = Parallel(n_jobs=n_jobs, backend='loky', verbose=verb)(
                 delayed(func_to_call)(
-                    c_mat[:,i], 
-                    u_mat[:,i], 
-                    s_mat[:,i], 
-                    model_to_run[i] if m_per_g else model_to_run, 
-                    max_iter, 
-                    init_mode, 
-                    global_pdist, 
-                    embed_coord, 
-                    rna_conn, 
-                    verbose, 
-                    plot, 
-                    save_plot, 
-                    plot_dir, 
-                    fit_args, 
-                    gene_list[i], 
-                    partial[i] if p_per_g else partial, 
-                    direction[i] if d_per_g else direction, 
-                    rna_only, 
-                    fit, 
-                    fit_decoupling, 
-                    extra_color, 
+                    c_mat[:, i],
+                    u_mat[:, i],
+                    s_mat[:, i],
+                    model_to_run[i] if m_per_g else model_to_run,
+                    max_iter,
+                    init_mode,
+                    global_pdist,
+                    embed_coord,
+                    rna_conn,
+                    verbose,
+                    plot,
+                    save_plot,
+                    plot_dir,
+                    fit_args,
+                    gene_list[i],
+                    partial[i] if p_per_g else partial,
+                    direction[i] if d_per_g else direction,
+                    rna_only,
+                    fit,
+                    fit_decoupling,
+                    extra_color,
                     ru[i] if isinstance(ru, (list, np.ndarray)) else ru,
-                    alpha[i] if isinstance(alpha, (list, np.ndarray)) else alpha,
-                    beta[i] if isinstance(beta, (list, np.ndarray)) else beta,
-                    gamma[i] if isinstance(gamma, (list, np.ndarray)) else gamma,
-                    t_sw[i] if isinstance(t_sw, (list, np.ndarray)) else t_sw) 
+                    alpha[i] if isinstance(alpha, (list, np.ndarray))
+                    else alpha,
+                    beta[i] if isinstance(beta, (list, np.ndarray))
+                    else beta,
+                    gamma[i] if isinstance(gamma, (list, np.ndarray))
+                    else gamma,
+                    t_sw[i] if isinstance(t_sw, (list, np.ndarray)) else t_sw)
                 for i in gene_indices)
 
-            for i,r in zip(gene_indices, res):
-                (loss, model, direct_out, parameters, initial_exp, 
+            for i, r in zip(gene_indices, res):
+                (loss, model, direct_out, parameters, initial_exp,
                  time, state, velocity, likelihood, anchors) = r
-                switch, rate, scale_cc, rescale_c, rescale_u, realign_ratio = parameters
+                switch, rate, scale_cc, rescale_c, rescale_u, realign_ratio = \
+                    parameters
                 likelihood, l_c, ssd_c, var_c = likelihood
-                losses[i,:] = loss
+                losses[i, :] = loss
                 models[i] = model
                 directions.append(direct_out)
-                t_sws[i,:] = switch
-                rates[i,:] = rate
+                t_sws[i, :] = switch
+                rates[i, :] = rate
                 scale_ccs[i] = scale_cc
                 rescale_cs[i] = rescale_c
                 rescale_us[i] = rescale_u
                 realign_ratios[i] = realign_ratio
                 likelihoods[i] = likelihood
                 l_cs[i] = l_c
                 ssd_cs[i] = ssd_c
                 var_cs[i] = var_c
                 if fit:
-                    initial_exps[i,:] = initial_exp
-                    times[:,i] = time
-                    states[:,i] = state
+                    initial_exps[i, :] = initial_exp
+                    times[:, i] = time
+                    states[:, i] = state
                     n_anchors_ = anchors[0].shape[0]
                     n_switch = anchors[1].shape[0]
                     if not rna_only:
-                        velo_c[:,i] = smooth_scale(atac_conn, velocity[:,0])
-                        #velo_c[:,i] = velocity[:,0]
-                        anchor_c[:n_anchors_,i] = anchors[0][:,0]
-                        anchor_c_sw[:n_switch,i] = anchors[1][:,0]
-                        anchor_vc[:n_anchors_,i] = anchors[2][:,0]
-                    velo_u[:,i] = smooth_scale(rna_conn, velocity[:,1])
-                    #velo_u[:,i] = velocity[:,1]
-                    velo_s[:,i] = smooth_scale(rna_conn, velocity[:,2])
-                    #velo_s[:,i] = velocity[:,2]
-                    anchor_u[:n_anchors_,i] = anchors[0][:,1]
-                    anchor_s[:n_anchors_,i] = anchors[0][:,2]
-                    anchor_u_sw[:n_switch,i] = anchors[1][:,1]
-                    anchor_s_sw[:n_switch,i] = anchors[1][:,2]
-                    anchor_vu[:n_anchors_,i] = anchors[2][:,1]
-                    anchor_vs[:n_anchors_,i] = anchors[2][:,2]
+                        velo_c[:, i] = smooth_scale(atac_conn, velocity[:, 0])
+                        anchor_c[:n_anchors_, i] = anchors[0][:, 0]
+                        anchor_c_sw[:n_switch, i] = anchors[1][:, 0]
+                        anchor_vc[:n_anchors_, i] = anchors[2][:, 0]
+                    velo_u[:, i] = smooth_scale(rna_conn, velocity[:, 1])
+                    velo_s[:, i] = smooth_scale(rna_conn, velocity[:, 2])
+                    anchor_u[:n_anchors_, i] = anchors[0][:, 1]
+                    anchor_s[:n_anchors_, i] = anchors[0][:, 2]
+                    anchor_u_sw[:n_switch, i] = anchors[1][:, 1]
+                    anchor_s_sw[:n_switch, i] = anchors[1][:, 2]
+                    anchor_vu[:n_anchors_, i] = anchors[2][:, 1]
+                    anchor_vs[:n_anchors_, i] = anchors[2][:, 2]
                     anchor_min_idx[i] = anchors[3]
                     anchor_max_idx[i] = anchors[4]
                     anchor_velo_min_idx[i] = anchors[5]
                     anchor_velo_max_idx[i] = anchors[6]
         else:
             i = group
             gene = gene_list[i]
             if verbose >= 1:
                 print(f'@@@@@fitting {gene}')
-            (loss, model, direct_out, parameters, initial_exp, 
-             time, state, velocity, likelihood, anchors) = func_to_call(c_mat[:,i], 
-                                                                        u_mat[:,i], 
-                                                                        s_mat[:,i], 
-                                                                        model_to_run[i] if m_per_g else model_to_run, 
-                                                                        max_iter, 
-                                                                        init_mode, 
-                                                                        global_pdist, 
-                                                                        embed_coord, 
-                                                                        rna_conn, 
-                                                                        verbose, 
-                                                                        plot, 
-                                                                        save_plot, 
-                                                                        plot_dir, 
-                                                                        fit_args, 
-                                                                        gene, 
-                                                                        partial[i] if p_per_g else partial, 
-                                                                        direction[i] if d_per_g else direction, 
-                                                                        rna_only, 
-                                                                        fit, 
-                                                                        fit_decoupling, 
-                                                                        extra_color, 
-                                                                        ru[i] if isinstance(ru, (list, np.ndarray)) else ru,
-                                                                        alpha[i] if isinstance(alpha, (list, np.ndarray)) else alpha,
-                                                                        beta[i] if isinstance(beta, (list, np.ndarray)) else beta,
-                                                                        gamma[i] if isinstance(gamma, (list, np.ndarray)) else gamma,
-                                                                        t_sw[i] if isinstance(t_sw, (list, np.ndarray)) else t_sw)
-            switch, rate, scale_cc, rescale_c, rescale_u, realign_ratio = parameters
+            (loss, model, direct_out,
+             parameters, initial_exp,
+             time, state, velocity,
+             likelihood, anchors) = \
+                func_to_call(c_mat[:, i], u_mat[:, i], s_mat[:, i],
+                             model_to_run[i] if m_per_g else model_to_run,
+                             max_iter, init_mode, global_pdist, embed_coord,
+                             rna_conn, verbose, plot, save_plot, plot_dir,
+                             fit_args, gene,
+                             partial[i] if p_per_g else partial,
+                             direction[i] if d_per_g else direction,
+                             rna_only, fit, fit_decoupling, extra_color,
+                             ru[i] if isinstance(ru, (list, np.ndarray))
+                             else ru,
+                             alpha[i] if isinstance(alpha, (list, np.ndarray))
+                             else alpha,
+                             beta[i] if isinstance(beta, (list, np.ndarray))
+                             else beta,
+                             gamma[i] if isinstance(gamma, (list, np.ndarray))
+                             else gamma,
+                             t_sw[i] if isinstance(t_sw, (list, np.ndarray))
+                             else t_sw)
+            switch, rate, scale_cc, rescale_c, rescale_u, realign_ratio = \
+                parameters
             likelihood, l_c, ssd_c, var_c = likelihood
-            losses[i,:] = loss
+            losses[i, :] = loss
             models[i] = model
             directions.append(direct_out)
-            t_sws[i,:] = switch
-            rates[i,:] = rate
+            t_sws[i, :] = switch
+            rates[i, :] = rate
             scale_ccs[i] = scale_cc
             rescale_cs[i] = rescale_c
             rescale_us[i] = rescale_u
             realign_ratios[i] = realign_ratio
             likelihoods[i] = likelihood
             l_cs[i] = l_c
             ssd_cs[i] = ssd_c
             var_cs[i] = var_c
             if fit:
-                initial_exps[i,:] = initial_exp
-                times[:,i] = time
-                states[:,i] = state
+                initial_exps[i, :] = initial_exp
+                times[:, i] = time
+                states[:, i] = state
                 n_anchors_ = anchors[0].shape[0]
                 n_switch = anchors[1].shape[0]
                 if not rna_only:
-                    velo_c[:,i] = smooth_scale(atac_conn, velocity[:,0])
-                    anchor_c[:n_anchors_,i] = anchors[0][:,0]
-                    anchor_c_sw[:n_switch,i] = anchors[1][:,0]
-                    anchor_vc[:n_anchors_,i] = anchors[2][:,0]
-                velo_u[:,i] = smooth_scale(rna_conn, velocity[:,1])
-                velo_s[:,i] = smooth_scale(rna_conn, velocity[:,2])
-                anchor_u[:n_anchors_,i] = anchors[0][:,1]
-                anchor_s[:n_anchors_,i] = anchors[0][:,2]
-                anchor_u_sw[:n_switch,i] = anchors[1][:,1]
-                anchor_s_sw[:n_switch,i] = anchors[1][:,2]
-                anchor_vu[:n_anchors_,i] = anchors[2][:,1]
-                anchor_vs[:n_anchors_,i] = anchors[2][:,2]
+                    velo_c[:, i] = smooth_scale(atac_conn, velocity[:, 0])
+                    anchor_c[:n_anchors_, i] = anchors[0][:, 0]
+                    anchor_c_sw[:n_switch, i] = anchors[1][:, 0]
+                    anchor_vc[:n_anchors_, i] = anchors[2][:, 0]
+                velo_u[:, i] = smooth_scale(rna_conn, velocity[:, 1])
+                velo_s[:, i] = smooth_scale(rna_conn, velocity[:, 2])
+                anchor_u[:n_anchors_, i] = anchors[0][:, 1]
+                anchor_s[:n_anchors_, i] = anchors[0][:, 2]
+                anchor_u_sw[:n_switch, i] = anchors[1][:, 1]
+                anchor_s_sw[:n_switch, i] = anchors[1][:, 2]
+                anchor_vu[:n_anchors_, i] = anchors[2][:, 1]
+                anchor_vs[:n_anchors_, i] = anchors[2][:, 2]
                 anchor_min_idx[i] = anchors[3]
                 anchor_max_idx[i] = anchors[4]
                 anchor_velo_min_idx[i] = anchors[5]
                 anchor_velo_max_idx[i] = anchors[6]
         pbar.update(len(gene_indices))
     pbar.close()
     directions = np.array(directions)
 
     filt = np.sum(losses != np.inf, 1) >= 1
     if np.sum(filt) == 0:
-        raise ValueError('None of the genes were fitted due to low quality, not returning')
-    adata_copy = adata_rna[:,gene_list[filt]].copy()
-    adata_copy.layers['ATAC'] = c_mat[:,filt]
-    adata_copy.var['fit_alpha_c'] = rates[filt,0]
-    adata_copy.var['fit_alpha'] = rates[filt,1]
-    adata_copy.var['fit_beta'] = rates[filt,2]
-    adata_copy.var['fit_gamma'] = rates[filt,3]
-    adata_copy.var['fit_t_sw1'] = t_sws[filt,0]
-    adata_copy.var['fit_t_sw2'] = t_sws[filt,1]
-    adata_copy.var['fit_t_sw3'] = t_sws[filt,2]
+        raise ValueError('None of the genes were fitted due to low quality,'
+                         ' not returning')
+    adata_copy = adata_rna[:, gene_list[filt]].copy()
+    adata_copy.layers['ATAC'] = c_mat[:, filt]
+    adata_copy.var['fit_alpha_c'] = rates[filt, 0]
+    adata_copy.var['fit_alpha'] = rates[filt, 1]
+    adata_copy.var['fit_beta'] = rates[filt, 2]
+    adata_copy.var['fit_gamma'] = rates[filt, 3]
+    adata_copy.var['fit_t_sw1'] = t_sws[filt, 0]
+    adata_copy.var['fit_t_sw2'] = t_sws[filt, 1]
+    adata_copy.var['fit_t_sw3'] = t_sws[filt, 2]
     adata_copy.var['fit_scale_cc'] = scale_ccs[filt]
     adata_copy.var['fit_rescale_c'] = rescale_cs[filt]
     adata_copy.var['fit_rescale_u'] = rescale_us[filt]
     adata_copy.var['fit_alignment_scaling'] = realign_ratios[filt]
     adata_copy.var['fit_model'] = models[filt]
     adata_copy.var['fit_direction'] = directions[filt]
     if model_to_run is not None and not m_per_g and not rna_only:
-        for i,m in enumerate(model_to_run):
-            adata_copy.var[f'fit_loss_M{m}'] = losses[filt,i]
+        for i, m in enumerate(model_to_run):
+            adata_copy.var[f'fit_loss_M{m}'] = losses[filt, i]
     else:
-        adata_copy.var['fit_loss'] = losses[filt,0]
+        adata_copy.var['fit_loss'] = losses[filt, 0]
     adata_copy.var['fit_likelihood'] = likelihoods[filt]
     adata_copy.var['fit_likelihood_c'] = l_cs[filt]
     adata_copy.var['fit_ssd_c'] = ssd_cs[filt]
     adata_copy.var['fit_var_c'] = var_cs[filt]
     if fit:
-        adata_copy.layers['fit_t'] = times[:,filt]
-        adata_copy.layers['fit_state'] = states[:,filt]
-        adata_copy.layers['velo_s'] = velo_s[:,filt]
-        adata_copy.layers['velo_u'] = velo_u[:,filt]
+        adata_copy.layers['fit_t'] = times[:, filt]
+        adata_copy.layers['fit_state'] = states[:, filt]
+        adata_copy.layers['velo_s'] = velo_s[:, filt]
+        adata_copy.layers['velo_u'] = velo_u[:, filt]
         if not rna_only:
-            adata_copy.layers['velo_chrom'] = velo_c[:,filt]
-        adata_copy.var['fit_c0'] = initial_exps[filt,0]
-        adata_copy.var['fit_u0'] = initial_exps[filt,1]
-        adata_copy.var['fit_s0'] = initial_exps[filt,2]
+            adata_copy.layers['velo_chrom'] = velo_c[:, filt]
+        adata_copy.var['fit_c0'] = initial_exps[filt, 0]
+        adata_copy.var['fit_u0'] = initial_exps[filt, 1]
+        adata_copy.var['fit_s0'] = initial_exps[filt, 2]
         adata_copy.var['fit_anchor_min_idx'] = anchor_min_idx[filt]
         adata_copy.var['fit_anchor_max_idx'] = anchor_max_idx[filt]
         adata_copy.var['fit_anchor_velo_min_idx'] = anchor_velo_min_idx[filt]
         adata_copy.var['fit_anchor_velo_max_idx'] = anchor_velo_max_idx[filt]
-        adata_copy.varm['fit_anchor_c'] = np.transpose(anchor_c[:,filt])
-        adata_copy.varm['fit_anchor_u'] = np.transpose(anchor_u[:,filt])
-        adata_copy.varm['fit_anchor_s'] = np.transpose(anchor_s[:,filt])
-        adata_copy.varm['fit_anchor_c_sw'] = np.transpose(anchor_c_sw[:,filt])
-        adata_copy.varm['fit_anchor_u_sw'] = np.transpose(anchor_u_sw[:,filt])
-        adata_copy.varm['fit_anchor_s_sw'] = np.transpose(anchor_s_sw[:,filt])
-        adata_copy.varm['fit_anchor_c_velo'] = np.transpose(anchor_vc[:,filt])
-        adata_copy.varm['fit_anchor_u_velo'] = np.transpose(anchor_vu[:,filt])
-        adata_copy.varm['fit_anchor_s_velo'] = np.transpose(anchor_vs[:,filt])
+        adata_copy.varm['fit_anchor_c'] = np.transpose(anchor_c[:, filt])
+        adata_copy.varm['fit_anchor_u'] = np.transpose(anchor_u[:, filt])
+        adata_copy.varm['fit_anchor_s'] = np.transpose(anchor_s[:, filt])
+        adata_copy.varm['fit_anchor_c_sw'] = np.transpose(anchor_c_sw[:, filt])
+        adata_copy.varm['fit_anchor_u_sw'] = np.transpose(anchor_u_sw[:, filt])
+        adata_copy.varm['fit_anchor_s_sw'] = np.transpose(anchor_s_sw[:, filt])
+        adata_copy.varm['fit_anchor_c_velo'] = np.transpose(anchor_vc[:, filt])
+        adata_copy.varm['fit_anchor_u_velo'] = np.transpose(anchor_vu[:, filt])
+        adata_copy.varm['fit_anchor_s_velo'] = np.transpose(anchor_vs[:, filt])
     v_genes = adata_copy.var['fit_likelihood'] >= 0.05
-    adata_copy.var['velo_s_genes'] = adata_copy.var['velo_u_genes'] = adata_copy.var['velo_chrom_genes'] = v_genes
-    adata_copy.uns['velo_s_params'] = adata_copy.uns['velo_u_params'] = adata_copy.uns['velo_chrom_params'] = {'mode': 'dynamical'}
+    adata_copy.var['velo_s_genes'] = adata_copy.var['velo_u_genes'] = \
+        adata_copy.var['velo_chrom_genes'] = v_genes
+    adata_copy.uns['velo_s_params'] = adata_copy.uns['velo_u_params'] = \
+        adata_copy.uns['velo_chrom_params'] = {'mode': 'dynamical'}
     adata_copy.uns['velo_s_params'].update(fit_args)
     adata_copy.uns['velo_u_params'].update(fit_args)
     adata_copy.uns['velo_chrom_params'].update(fit_args)
     adata_copy.obsp['_RNA_conn'] = rna_conn
     if not rna_only:
         adata_copy.obsp['_ATAC_conn'] = atac_conn
     return adata_copy
@@ -2881,33 +3341,33 @@
     conn[idx1] = 0.25
     conn[idx2] = 0.5
     conn[idx3] = 1
     conn.eliminate_zeros()
     return conn
 
 
-def set_velocity_genes(adata, 
-                       likelihood_lower=0.05, 
-                       rescale_u_upper=None, 
-                       rescale_u_lower=None, 
-                       rescale_c_upper=None, 
-                       rescale_c_lower=None, 
-                       primed_upper=None, 
-                       primed_lower=None, 
-                       decoupled_upper=None, 
-                       decoupled_lower=None, 
-                       alpha_c_upper=None, 
-                       alpha_c_lower=None, 
-                       alpha_upper=None, 
-                       alpha_lower=None, 
-                       beta_upper=None, 
-                       beta_lower=None, 
-                       gamma_upper=None, 
-                       gamma_lower=None, 
-                       scale_cc_upper=None, 
+def set_velocity_genes(adata,
+                       likelihood_lower=0.05,
+                       rescale_u_upper=None,
+                       rescale_u_lower=None,
+                       rescale_c_upper=None,
+                       rescale_c_lower=None,
+                       primed_upper=None,
+                       primed_lower=None,
+                       decoupled_upper=None,
+                       decoupled_lower=None,
+                       alpha_c_upper=None,
+                       alpha_c_lower=None,
+                       alpha_upper=None,
+                       alpha_lower=None,
+                       beta_upper=None,
+                       beta_lower=None,
+                       gamma_upper=None,
+                       gamma_lower=None,
+                       scale_cc_upper=None,
                        scale_cc_lower=None,
                        verbose=False
                        ):
     """Reset velocity genes.
 
     This function resets velocity genes based on criteria of variables.
 
@@ -2916,47 +3376,47 @@
     adata: :class:`~anndata.AnnData`
         Anndata result from dynamics recovery.
     likelihood_lower: `float` (default: 0.05)
         Minimum ikelihood.
     rescale_u_upper: `float` (default: `None`)
         Maximum rescale_u.
     rescale_u_lower: `float` (default: `None`)
-        Maximum rescale_u.
+        Minimum rescale_u.
     rescale_c_upper: `float` (default: `None`)
         Maximum rescale_c.
     rescale_c_lower: `float` (default: `None`)
-        Maximum rescale_c.
+        Minimum rescale_c.
     primed_upper: `float` (default: `None`)
         Maximum primed interval.
     primed_lower: `float` (default: `None`)
-        Maximum primed interval.
+        Minimum primed interval.
     decoupled_upper: `float` (default: `None`)
         Maximum decoupled interval.
     decoupled_lower: `float` (default: `None`)
-        Maximum decoupled interval.
+        Minimum decoupled interval.
     alpha_c_upper: `float` (default: `None`)
         Maximum alpha_c.
     alpha_c_lower: `float` (default: `None`)
-        Maximum alpha_c.
+        Minimum alpha_c.
     alpha_upper: `float` (default: `None`)
         Maximum alpha.
     alpha_lower: `float` (default: `None`)
-        Maximum alpha.
+        Minimum alpha.
     beta_upper: `float` (default: `None`)
         Maximum beta.
     beta_lower: `float` (default: `None`)
-        Maximum beta.
+        Minimum beta.
     gamma_upper: `float` (default: `None`)
         Maximum gamma.
     gamma_lower: `float` (default: `None`)
-        Maximum gamma.
+        Minimum gamma.
     scale_cc_upper: `float` (default: `None`)
         Maximum scale_cc.
     scale_cc_lower: `float` (default: `None`)
-        Maximum scale_cc.
+        Minimum scale_cc.
     verbose: `bool` (default: `False`)
         Whether to print the number of velocity genes.
 
     Returns
     -------
     velo_s_genes, velo_u_genes, velo_chrom_genes: `.var`
         new velocity genes for each modalities.
@@ -2967,15 +3427,16 @@
         v_genes &= adata.var['fit_rescale_u'] <= rescale_u_upper
     if rescale_u_lower is not None:
         v_genes &= adata.var['fit_rescale_u'] >= rescale_u_lower
     if rescale_c_upper is not None:
         v_genes &= adata.var['fit_rescale_c'] <= rescale_c_upper
     if rescale_c_lower is not None:
         v_genes &= adata.var['fit_rescale_c'] >= rescale_c_lower
-    t_sw1 = adata.var['fit_t_sw1'] + 20 / adata.uns['velo_s_params']['t'] * adata.var['fit_anchor_min_idx'] *  adata.var['fit_alignment_scaling']
+    t_sw1 = adata.var['fit_t_sw1'] + 20 / adata.uns['velo_s_params']['t'] * \
+        adata.var['fit_anchor_min_idx'] * adata.var['fit_alignment_scaling']
     if primed_upper is not None:
         v_genes &= t_sw1 <= primed_upper
     if primed_lower is not None:
         v_genes &= t_sw1 >= primed_lower
     t_sw2 = np.clip(adata.var['fit_t_sw2'], None, 20)
     t_sw3 = np.clip(adata.var['fit_t_sw3'], None, 20)
     t_interval3 = t_sw3 - t_sw2
@@ -3001,21 +3462,23 @@
         v_genes &= adata.var['fit_gamma'] >= gamma_lower
     if scale_cc_upper is not None:
         v_genes &= adata.var['fit_scale_cc'] <= scale_cc_upper
     if scale_cc_lower is not None:
         v_genes &= adata.var['fit_scale_cc'] >= scale_cc_lower
     if verbose:
         print(f'{np.sum(v_genes)} velocity genes were selected')
-    adata.var['velo_s_genes'] = adata.var['velo_u_genes'] = adata.var['velo_chrom_genes'] = v_genes
+    adata.var['velo_s_genes'] = adata.var['velo_u_genes'] = \
+        adata.var['velo_chrom_genes'] = v_genes
 
 
 def velocity_graph(adata, vkey='velo_s', xkey='Ms', **kwargs):
     """Computes velocity graph.
 
-    This function normalizes the velocity matrix and computes velocity graph with `scvelo.tl.velocity_graph`.
+    This function normalizes the velocity matrix and computes velocity graph
+    with `scvelo.tl.velocity_graph`.
 
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         Anndata result from dynamics recovery.
     vkey: `str` (default: `velo_s`)
         Default to use spliced velocities.
@@ -3025,28 +3488,31 @@
 
     Returns
     -------
     Normalized velocity matrix and associated velocity genes and params.
     Outputs of `scvelo.tl.velocity_graph`.
     """
     if vkey not in adata.layers.keys():
-        raise ValueError('Velocity matrix is not found. Please run multivelo.recover_dynamics_chrom function first.')
+        raise ValueError('Velocity matrix is not found. Please run multivelo'
+                         '.recover_dynamics_chrom function first.')
     if vkey+'_norm' not in adata.layers.keys():
-        adata.layers[vkey+'_norm'] = adata.layers[vkey] / np.sum(np.abs(adata.layers[vkey]), 0)
+        adata.layers[vkey+'_norm'] = adata.layers[vkey] / np.sum(
+            np.abs(adata.layers[vkey]), 0)
         adata.layers[vkey+'_norm'] /= np.mean(adata.layers[vkey+'_norm'])
         adata.uns[vkey+'_norm_params'] = adata.uns[vkey+'_params']
     if vkey+'_norm_genes' not in adata.var.columns:
         adata.var[vkey+'_norm_genes'] = adata.var[vkey+'_genes']
     scv.tl.velocity_graph(adata, vkey=vkey+'_norm', xkey=xkey, **kwargs)
 
 
 def velocity_embedding_stream(adata, vkey='velo_s', show=True, **kwargs):
     """Plots velocity stream.
 
-    This function plots velocity streamplot with `scvelo.pl.velocity_embedding_stream`.
+    This function plots velocity streamplot with
+    `scvelo.pl.velocity_embedding_stream`.
 
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         Anndata result from dynamics recovery.
     vkey: `str` (default: `velo_s`)
         Default to use spliced velocities. The normalized matrix will be used.
@@ -3055,23 +3521,26 @@
     Additional parameters passed to `scvelo.tl.velocity_graph`.
 
     Returns
     -------
     If `show==False`, a matplotlib axis object.
     """
     if vkey not in adata.layers:
-        raise ValueError('Velocity matrix is not found. Please run multivelo.recover_dynamics_chrom function first.')
+        raise ValueError('Velocity matrix is not found. Please run multivelo.'
+                         'recover_dynamics_chrom function first.')
     if vkey+'_norm' not in adata.layers.keys():
-        adata.layers[vkey+'_norm'] = adata.layers[vkey] / np.sum(np.abs(adata.layers[vkey]), 0)
+        adata.layers[vkey+'_norm'] = adata.layers[vkey] / np.sum(
+            np.abs(adata.layers[vkey]), 0)
         adata.uns[vkey+'_norm_params'] = adata.uns[vkey+'_params']
     if vkey+'_norm_genes' not in adata.var.columns:
         adata.var[vkey+'_norm_genes'] = adata.var[vkey+'_genes']
     if vkey+'_norm_graph' not in adata.uns.keys():
         velocity_graph(adata, vkey=vkey, **kwargs)
-    out = scv.pl.velocity_embedding_stream(adata, vkey=vkey+'_norm', **kwargs)
+    out = scv.pl.velocity_embedding_stream(adata, vkey=vkey+'_norm', show=show,
+                                           **kwargs)
     if not show:
         return out
 
 
 def latent_time(adata, vkey='velo_s', **kwargs):
     """Computes latent time.
 
@@ -3086,26 +3555,29 @@
     Additional parameters passed to `scvelo.tl.velocity_graph`.
 
     Returns
     -------
     Outputs of `scvelo.tl.latent_time`.
     """
     if vkey not in adata.layers.keys() or 'fit_t' not in adata.layers.keys():
-        raise ValueError('Velocity or time matrix is not found. Please run multivelo.recover_dynamics_chrom function first.')
+        raise ValueError('Velocity or time matrix is not found. Please run '
+                         'multivelo.recover_dynamics_chrom function first.')
     if vkey+'_norm' not in adata.layers.keys():
-        raise ValueError('Normalized velocity matrix is not found. Please multivelo.run velocity_graph function first.')
+        raise ValueError('Normalized velocity matrix is not found. Please '
+                         'run multivelo.velocity_graph function first.')
     if vkey+'_norm_graph' not in adata.uns.keys():
         velocity_graph(adata, vkey=vkey, **kwargs)
     scv.tl.latent_time(adata, vkey=vkey+'_norm', **kwargs)
 
 
 def LRT_decoupling(adata_rna, adata_atac, **kwargs):
     """Computes likelihood ratio test for decoupling state.
 
-    This function computes whether keeping decoupling state improves fit Likelihood.
+    This function computes whether keeping decoupling state improves fit
+    Likelihood.
 
     Parameters
     ----------
     adata_rna: :class:`~anndata.AnnData`
         RNA anndata object
     adata_atac: :class:`~anndata.AnnData`
         ATAC anndata object.
@@ -3118,110 +3590,118 @@
     adata_result_w_decoupled: class:`~anndata.AnnData`
         fit result without decoupling state
     res: `pandas.DataFrame`
         LRT statistics
     """
     from scipy.stats.distributions import chi2
     print('fitting models with decoupling intervals')
-    adata_result_w_decoupled = recover_dynamics_chrom(adata_rna, adata_atac, fit_decoupling=True, **kwargs)
+    adata_result_w_decoupled = recover_dynamics_chrom(adata_rna, adata_atac,
+                                                      fit_decoupling=True,
+                                                      **kwargs)
     print('fitting models without decoupling intervals')
-    adata_result_wo_decoupled = recover_dynamics_chrom(adata_rna, adata_atac, fit_decoupling=False, **kwargs)
+    adata_result_wo_decoupled = recover_dynamics_chrom(adata_rna, adata_atac,
+                                                       fit_decoupling=False,
+                                                       **kwargs)
     print('testing likelihood ratio')
-    shared_genes = pd.Index(np.intersect1d(adata_result_w_decoupled.var_names, adata_result_wo_decoupled.var_names))
-    l_c_w_decoupled = adata_result_w_decoupled[:,shared_genes].var['fit_likelihood_c'].values
-    l_c_wo_decoupled = adata_result_wo_decoupled[:,shared_genes].var['fit_likelihood_c'].values
+    shared_genes = pd.Index(np.intersect1d(adata_result_w_decoupled.var_names,
+                                           adata_result_wo_decoupled.var_names)
+                            )
+    l_c_w_decoupled = adata_result_w_decoupled[:, shared_genes].\
+        var['fit_likelihood_c'].values
+    l_c_wo_decoupled = adata_result_wo_decoupled[:, shared_genes].\
+        var['fit_likelihood_c'].values
     n_obs = adata_rna.n_obs
     LRT_c = -2 * n_obs * (np.log(l_c_wo_decoupled) - np.log(l_c_w_decoupled))
     p_c = chi2.sf(LRT_c, 1)
-    l_w_decoupled = adata_result_w_decoupled[:,shared_genes].var['fit_likelihood'].values
-    l_wo_decoupled = adata_result_wo_decoupled[:,shared_genes].var['fit_likelihood'].values
+    l_w_decoupled = adata_result_w_decoupled[:, shared_genes].\
+        var['fit_likelihood'].values
+    l_wo_decoupled = adata_result_wo_decoupled[:, shared_genes].\
+        var['fit_likelihood'].values
     LRT = -2 * n_obs * (np.log(l_wo_decoupled) - np.log(l_w_decoupled))
     p = chi2.sf(LRT, 1)
-    res = pd.DataFrame({'likelihood_c_w_decoupled':l_c_w_decoupled, 
-                        'likelihood_c_wo_decoupled':l_c_wo_decoupled, 
-                        'LRT_c': LRT_c, 
-                        'pval_c': p_c, 
-                        'likelihood_w_decoupled':l_w_decoupled, 
-                        'likelihood_wo_decoupled':l_wo_decoupled, 
-                        'LRT': LRT, 
-                        'pval': p, 
+    res = pd.DataFrame({'likelihood_c_w_decoupled': l_c_w_decoupled,
+                        'likelihood_c_wo_decoupled': l_c_wo_decoupled,
+                        'LRT_c': LRT_c,
+                        'pval_c': p_c,
+                        'likelihood_w_decoupled': l_w_decoupled,
+                        'likelihood_wo_decoupled': l_wo_decoupled,
+                        'LRT': LRT,
+                        'pval': p,
                         }, index=shared_genes)
     return adata_result_w_decoupled, adata_result_wo_decoupled, res
 
 
 def transition_matrix_s(s_mat, velo_s, knn):
     knn = knn.astype(int)
     tm_val, tm_col, tm_row = [], [], []
     for i in range(knn.shape[0]):
-        two_step_knn = knn[i,:]
-        for j in knn[i,:]:
-            two_step_knn = np.append(two_step_knn, knn[j,:])
+        two_step_knn = knn[i, :]
+        for j in knn[i, :]:
+            two_step_knn = np.append(two_step_knn, knn[j, :])
         two_step_knn = np.unique(two_step_knn)
         for j in two_step_knn:
-            s = s_mat[i,:]
-            sn = s_mat[j,:]
+            s = s_mat[i, :]
+            sn = s_mat[j, :]
             ds = s - sn
-            #ds = ds - np.mean(ds)
             dx = np.ravel(ds.A)
-            velo = velo_s[i,:]
+            velo = velo_s[i, :]
             cos_sim = np.dot(dx, velo)/(norm(dx)*norm(velo))
             tm_val.append(cos_sim)
             tm_col.append(j)
             tm_row.append(i)
-    tm = coo_matrix((tm_val, (tm_row, tm_col)), shape = (s_mat.shape[0], s_mat.shape[0])).tocsr()
+    tm = coo_matrix((tm_val, (tm_row, tm_col)), shape=(s_mat.shape[0],
+                    s_mat.shape[0])).tocsr()
     tm.setdiag(0)
     tm_neg = tm.copy()
     tm.data = np.clip(tm.data, 0, 1)
     tm_neg.data = np.clip(tm_neg.data, -1, 0)
     tm.eliminate_zeros()
     tm_neg.eliminate_zeros()
     return tm, tm_neg
 
 
 def transition_matrix_chrom(c_mat, u_mat, s_mat, velo_c, velo_u, velo_s, knn):
     knn = knn.astype(int)
     tm_val, tm_col, tm_row = [], [], []
     for i in range(knn.shape[0]):
-        two_step_knn = knn[i,:]
-        for j in knn[i,:]:
-            two_step_knn = np.append(two_step_knn, knn[j,:])
+        two_step_knn = knn[i, :]
+        for j in knn[i, :]:
+            two_step_knn = np.append(two_step_knn, knn[j, :])
         two_step_knn = np.unique(two_step_knn)
         for j in two_step_knn:
-            u = u_mat[i,:].A
-            s = s_mat[i,:].A
-            c = c_mat[i,:].A
-            un = u_mat[j,:]
-            sn = s_mat[j,:]
-            cn = c_mat[j,:]
+            u = u_mat[i, :].A
+            s = s_mat[i, :].A
+            c = c_mat[i, :].A
+            un = u_mat[j, :]
+            sn = s_mat[j, :]
+            cn = c_mat[j, :]
             dc = (c - cn) / np.std(c)
             du = (u - un) / np.std(u)
             ds = (s - sn) / np.std(s)
-            #dc = dc - np.mean(dc)
-            #du = du - np.mean(du)
-            #ds = ds - np.mean(ds)
             dx = np.ravel(np.hstack((dc.A, du.A, ds.A)))
-            velo = np.hstack((velo_c[i,:], velo_u[i,:], velo_s[i,:]))
+            velo = np.hstack((velo_c[i, :], velo_u[i, :], velo_s[i, :]))
             cos_sim = np.dot(dx, velo)/(norm(dx)*norm(velo))
             tm_val.append(cos_sim)
             tm_col.append(j)
             tm_row.append(i)
-    tm = coo_matrix((tm_val, (tm_row, tm_col)), shape = (c_mat.shape[0], c_mat.shape[0])).tocsr()
+    tm = coo_matrix((tm_val, (tm_row, tm_col)), shape=(c_mat.shape[0],
+                    c_mat.shape[0])).tocsr()
     tm.setdiag(0)
     tm_neg = tm.copy()
     tm.data = np.clip(tm.data, 0, 1)
     tm_neg.data = np.clip(tm_neg.data, -1, 0)
     tm.eliminate_zeros()
     tm_neg.eliminate_zeros()
     return tm, tm_neg
 
 
-def likelihood_plot(adata, 
-                    genes=None, 
-                    figsize=(14,10), 
-                    bins=50, 
+def likelihood_plot(adata,
+                    genes=None,
+                    figsize=(14, 10),
+                    bins=50,
                     pointsize=4
                     ):
     """Likelihood plots.
 
     This function plots likelihood and variable distributions.
 
     Parameters
@@ -3237,106 +3717,111 @@
     pointsize: `float` (default: 4)
         Point size for scatter plots.
     """
     if genes is None:
         var = adata.var
     else:
         genes = np.array(genes)
-        var = adata[:,genes].var
+        var = adata[:, genes].var
     likelihood = var[['fit_likelihood']].values
     rescale_u = var[['fit_rescale_u']].values
     rescale_c = var[['fit_rescale_c']].values
-    t_interval1 = var['fit_t_sw1'] + 20 / adata.uns['velo_s_params']['t'] * var['fit_anchor_min_idx'] * var['fit_alignment_scaling']
+    t_interval1 = var['fit_t_sw1'] + 20 / adata.uns['velo_s_params']['t'] \
+        * var['fit_anchor_min_idx'] * var['fit_alignment_scaling']
     t_sw2 = np.clip(var['fit_t_sw2'], None, 20)
     t_sw3 = np.clip(var['fit_t_sw3'], None, 20)
     t_interval3 = t_sw3 - t_sw2
     log_s = np.log1p(np.sum(adata.layers['Ms'], axis=0))
     alpha_c = var[['fit_alpha_c']].values
     alpha = var[['fit_alpha']].values
     beta = var[['fit_beta']].values
     gamma = var[['fit_gamma']].values
     scale_cc = var[['fit_scale_cc']].values
 
     fig, axes = plt.subplots(4, 5, figsize=figsize)
-    axes[0,0].hist(likelihood, bins=bins);
-    axes[0,0].set_title('likelihood');
-    axes[0,1].hist(rescale_u, bins=bins);
-    axes[0,1].set_title('rescale u');
-    axes[0,2].hist(rescale_c, bins=bins);
-    axes[0,2].set_title('rescale c');
-    axes[0,3].hist(t_interval1.values, bins=bins);
-    axes[0,3].set_title('primed interval');
-    axes[0,4].hist(t_interval3, bins=bins);
-    axes[0,4].set_title('decoupled interval');
-
-    axes[1,0].scatter(log_s, likelihood, s=pointsize);
-    axes[1,0].set_xlabel('log spliced');
-    axes[1,0].set_ylabel('likelihood');
-    axes[1,1].scatter(rescale_u, likelihood, s=pointsize);
-    axes[1,1].set_xlabel('rescale u');
-    axes[1,2].scatter(rescale_c, likelihood, s=pointsize);
-    axes[1,2].set_xlabel('rescale c');
-    axes[1,3].scatter(t_interval1.values, likelihood, s=pointsize);
-    axes[1,3].set_xlabel('primed interval');
-    axes[1,4].scatter(t_interval3, likelihood, s=pointsize);
-    axes[1,4].set_xlabel('decoupled interval');
-
-    axes[2,0].hist(alpha_c, bins=bins);
-    axes[2,0].set_title('alpha c');
-    axes[2,1].hist(alpha, bins=bins);
-    axes[2,1].set_title('alpha');
-    axes[2,2].hist(beta, bins=bins);
-    axes[2,2].set_title('beta');
-    axes[2,3].hist(gamma, bins=bins);
-    axes[2,3].set_title('gamma');
-    axes[2,4].hist(scale_cc, bins=bins);
-    axes[2,4].set_title('scale cc');
-
-    axes[3,0].scatter(alpha_c, likelihood, s=pointsize);
-    axes[3,0].set_xlabel('alpha c');
-    axes[3,0].set_ylabel('likelihood');
-    axes[3,1].scatter(alpha, likelihood, s=pointsize);
-    axes[3,1].set_xlabel('alpha');
-    axes[3,2].scatter(beta, likelihood, s=pointsize);
-    axes[3,2].set_xlabel('beta');
-    axes[3,3].scatter(gamma, likelihood, s=pointsize);
-    axes[3,3].set_xlabel('gamma');
-    axes[3,4].scatter(scale_cc, likelihood, s=pointsize);
-    axes[3,4].set_xlabel('scale cc');
+    axes[0, 0].hist(likelihood, bins=bins)
+    axes[0, 0].set_title('likelihood')
+    axes[0, 1].hist(rescale_u, bins=bins)
+    axes[0, 1].set_title('rescale u')
+    axes[0, 2].hist(rescale_c, bins=bins)
+    axes[0, 2].set_title('rescale c')
+    axes[0, 3].hist(t_interval1.values, bins=bins)
+    axes[0, 3].set_title('primed interval')
+    axes[0, 4].hist(t_interval3, bins=bins)
+    axes[0, 4].set_title('decoupled interval')
+
+    axes[1, 0].scatter(log_s, likelihood, s=pointsize)
+    axes[1, 0].set_xlabel('log spliced')
+    axes[1, 0].set_ylabel('likelihood')
+    axes[1, 1].scatter(rescale_u, likelihood, s=pointsize)
+    axes[1, 1].set_xlabel('rescale u')
+    axes[1, 2].scatter(rescale_c, likelihood, s=pointsize)
+    axes[1, 2].set_xlabel('rescale c')
+    axes[1, 3].scatter(t_interval1.values, likelihood, s=pointsize)
+    axes[1, 3].set_xlabel('primed interval')
+    axes[1, 4].scatter(t_interval3, likelihood, s=pointsize)
+    axes[1, 4].set_xlabel('decoupled interval')
+
+    axes[2, 0].hist(alpha_c, bins=bins)
+    axes[2, 0].set_title('alpha c')
+    axes[2, 1].hist(alpha, bins=bins)
+    axes[2, 1].set_title('alpha')
+    axes[2, 2].hist(beta, bins=bins)
+    axes[2, 2].set_title('beta')
+    axes[2, 3].hist(gamma, bins=bins)
+    axes[2, 3].set_title('gamma')
+    axes[2, 4].hist(scale_cc, bins=bins)
+    axes[2, 4].set_title('scale cc')
+
+    axes[3, 0].scatter(alpha_c, likelihood, s=pointsize)
+    axes[3, 0].set_xlabel('alpha c')
+    axes[3, 0].set_ylabel('likelihood')
+    axes[3, 1].scatter(alpha, likelihood, s=pointsize)
+    axes[3, 1].set_xlabel('alpha')
+    axes[3, 2].scatter(beta, likelihood, s=pointsize)
+    axes[3, 2].set_xlabel('beta')
+    axes[3, 3].scatter(gamma, likelihood, s=pointsize)
+    axes[3, 3].set_xlabel('gamma')
+    axes[3, 4].scatter(scale_cc, likelihood, s=pointsize)
+    axes[3, 4].set_xlabel('scale cc')
     fig.tight_layout()
 
 
 def pie_summary(adata, genes=None):
     """Summary of directions and models.
 
-    This function plots a pie chart for (pre-determined or specified) directions and models.
+    This function plots a pie chart for (pre-determined or specified)
+    directions and models.
     `induction`: induction-only genes.
     `repression`: repression-only genes.
     `Model 1`: model 1 complete genes.
     `Model 2`: model 2 complete genes.
 
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         Anndata result from dynamics recovery.
     genes: `str`,  list of `str` (default: `None`)
         If `None`, will use all fitted genes.
     """
     if genes is None:
         genes = adata.var_names
-    fit_model = adata[:,(adata.var['fit_direction']=='complete') & np.isin(adata.var_names, genes)].var['fit_model'].values
-    fit_direction = adata[:,genes].var['fit_direction'].values
-    data = [np.sum(fit_direction == 'on'), np.sum(fit_direction == 'off'), np.sum(fit_model == 1), np.sum(fit_model == 2)]
+    fit_model = adata[:, (adata.var['fit_direction'] == 'complete') &
+                      np.isin(adata.var_names, genes)].var['fit_model'].values
+    fit_direction = adata[:, genes].var['fit_direction'].values
+    data = [np.sum(fit_direction == 'on'), np.sum(fit_direction == 'off'),
+            np.sum(fit_model == 1), np.sum(fit_model == 2)]
     index = ['induction', 'repression', 'Model 1', 'Model 2']
-    index = [x for i,x in enumerate(index) if data[i] > 0]
+    index = [x for i, x in enumerate(index) if data[i] > 0]
     data = [x for x in data if x > 0]
-    df = pd.DataFrame({'data':data}, index=index)
-    df.plot.pie(y='data', autopct='%1.1f%%', legend=False, startangle=30, ylabel='')
-    circle = plt.Circle((0,0),0.8,fc='white')
-    fig=plt.gcf()
+    df = pd.DataFrame({'data': data}, index=index)
+    df.plot.pie(y='data', autopct='%1.1f%%', legend=False, startangle=30,
+                ylabel='')
+    circle = plt.Circle((0, 0), 0.8, fc='white')
+    fig = plt.gcf()
     fig.gca().add_artist(circle)
 
 
 def switch_time_summary(adata, genes=None):
     """Summary of switch times.
 
     This function plots a box plot for observed switch times.
@@ -3348,79 +3833,92 @@
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         Anndata result from dynamics recovery.
     genes: `str`,  list of `str` (default: `None`)
         If `None`, will use velocity genes.
     """
-    t_sw = adata[:,adata.var['velo_s_genes'] if genes is None else genes].var[['fit_t_sw1', 'fit_t_sw2', 'fit_t_sw3']].copy()
+    t_sw = adata[:, adata.var['velo_s_genes']
+                 if genes is None
+                 else genes] \
+        .var[['fit_t_sw1', 'fit_t_sw2', 'fit_t_sw3']].copy()
     t_sw = t_sw.mask(t_sw > 20, 20)
     t_sw = t_sw.mask(t_sw < 0)
     t_sw['interval 1'] = t_sw['fit_t_sw1']
     t_sw['t_sw2 - t_sw1'] = t_sw['fit_t_sw2'] - t_sw['fit_t_sw1']
     t_sw['t_sw3 - t_sw2'] = t_sw['fit_t_sw3'] - t_sw['fit_t_sw2']
     t_sw['20 - t_sw3'] = 20 - t_sw['fit_t_sw3']
     t_sw = t_sw.mask(t_sw <= 0)
     t_sw = t_sw.mask(t_sw > 20)
-    t_sw.columns = pd.Index(['time 1', 'time 2', 'time 3', 'primed', 'coupled-on', 'decoupled', 'coupled-off'])
+    t_sw.columns = pd.Index(['time 1', 'time 2', 'time 3', 'primed',
+                             'coupled-on', 'decoupled', 'coupled-off'])
     t_sw = t_sw[['primed', 'coupled-on', 'decoupled', 'coupled-off']]
     t_sw = t_sw / 20
     fig, ax = plt.subplots(figsize=(4, 5))
     ax = sns.boxplot(data=t_sw, width=0.5, palette='Set2', ax=ax)
     ax.set_yticks(np.linspace(0, 1, 5))
     ax.set_title('Switch Intervals')
 
 
-def dynamic_plot(adata, 
-                 genes, 
-                 by='expression', 
-                 color_by='state', 
-                 gene_time=True, 
-                 axis_on=True, 
-                 frame_on=True, 
-                 show_anchors=True, 
-                 show_switches=True, 
-                 downsample=1, 
-                 full_range=False, 
-                 figsize=None, 
-                 pointsize=2, 
-                 linewidth=1.5, 
+def dynamic_plot(adata,
+                 genes,
+                 by='expression',
+                 color_by='state',
+                 gene_time=True,
+                 axis_on=True,
+                 frame_on=True,
+                 show_anchors=True,
+                 show_switches=True,
+                 downsample=1,
+                 full_range=False,
+                 figsize=None,
+                 pointsize=2,
+                 linewidth=1.5,
                  cmap='coolwarm'
                  ):
     """Gene dynamics plot.
 
     This function plots accessibility, expression, or velocity by time.
 
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         Anndata result from dynamics recovery.
     genes: `str`,  list of `str`
         List of genes to plot.
     by: `str` (default: `expression`)
-        Plot accessibilities and expressions if `expression`. Plot velocities if `velocity`.
+        Plot accessibilities and expressions if `expression`. Plot velocities
+        if `velocity`.
     color_by: `str` (default: `state`)
-        Color by the four potential states if `state`. Other common values are leiden, louvain, celltype, etc.
-        If not `state`, the color field must be present in `.uns`, which can be pre-computed with `scanpy.pl.scatter`.
-        For `state`, red, orange, green, and blue represent state 1, 2, 3, and 4, respectively.
+        Color by the four potential states if `state`. Other common values are
+        leiden, louvain, celltype, etc.
+        If not `state`, the color field must be present in `.uns`, which can
+        be pre-computed with `scanpy.pl.scatter`.
+        For `state`, red, orange, green, and blue represent state 1, 2, 3, and
+        4, respectively.
     gene_time: `bool` (default: `True`)
-        Whether to use individual gene fitted time, or shared global latent time.
-        Mean values of 20 equal sized windows will be connected and shown if `gene_time==False`.
+        Whether to use individual gene fitted time, or shared global latent
+        time.
+        Mean values of 20 equal sized windows will be connected and shown if
+        `gene_time==False`.
     axis_on: `bool` (default: `True`)
         Whether to show axis labels.
     frame_on: `bool` (default: `True`)
         Whether to show plot frames.
     show_anchors: `bool` (default: `True`)
         Whether to display anchors.
     show_switches: `bool` (default: `True`)
-        Whether to show switch times. The switch times are indicated by vertical dotted line.
+        Whether to show switch times. The switch times are indicated by
+        vertical dotted line.
     downsample: `int` (default: 1)
-        How much to downsample the cells. The remaining number will be `1/downsample` of original.
+        How much to downsample the cells. The remaining number will be
+        `1/downsample` of original.
     full_range: `bool` (default: `False`)
-        Whether to show the full time range of velocities before smoothing or subset to only smoothed range.
+        Whether to show the full time range of velocities before smoothing or
+        subset to only smoothed range.
     figsize: `tuple` (default: `None`)
         Total figure size.
     pointsize: `float` (default: 2)
         Point size for scatter plots.
     linewidth: `float` (default: 1.5)
         Line width for anchor line or mean line.
     cmap: `str` (default: `coolwarm`)
@@ -3428,24 +3926,28 @@
     """
     from pandas.api.types import is_numeric_dtype, is_categorical_dtype
     if by not in ['expression', 'velocity']:
         raise ValueError('"by" must be either "expression" or "velocity".')
     if by == 'velocity':
         show_switches = False
     if color_by == 'state':
-        types = [0,1,2,3]
+        types = [0, 1, 2, 3]
         colors = ['tab:red', 'tab:orange', 'tab:green', 'tab:blue']
     elif color_by in adata.obs and is_numeric_dtype(adata.obs[color_by]):
         types = None
         colors = adata.obs[color_by].values
-    elif color_by in adata.obs and is_categorical_dtype(adata.obs[color_by]) and color_by+'_colors' in adata.uns.keys():
+    elif color_by in adata.obs and is_categorical_dtype(adata.obs[color_by]) \
+            and color_by+'_colors' in adata.uns.keys():
         types = adata.obs[color_by].cat.categories
         colors = adata.uns[f'{color_by}_colors']
     else:
-        raise ValueError('Currently, color key must be a single string of either numerical or categorical available in adata obs, and the colors of categories can be found in adata uns.')
+        raise ValueError('Currently, color key must be a single string of '
+                         'either numerical or categorical available in adata '
+                         'obs, and the colors of categories can be found in '
+                         'adata uns.')
 
     downsample = np.clip(int(downsample), 1, 10)
     genes = np.array(genes)
     missing_genes = genes[~np.isin(genes, adata.var_names)]
     if len(missing_genes) > 0:
         print(f'{missing_genes} not found')
     genes = genes[np.isin(genes, adata.var_names)]
@@ -3453,116 +3955,160 @@
     if gn == 0:
         return
     if not gene_time:
         show_anchors = False
         latent_time = np.array(adata.obs['latent_time'])
         time_window = latent_time // 0.05
         time_window = time_window.astype(int)
-        time_window[time_window==20] = 19
-    if 'velo_s_params' in adata.uns.keys() and 'outlier' in adata.uns['velo_s_params']:
+        time_window[time_window == 20] = 19
+    if 'velo_s_params' in adata.uns.keys() and 'outlier' \
+            in adata.uns['velo_s_params']:
         outlier = adata.uns['velo_s_params']['outlier']
     else:
         outlier = 99
 
-    fig, axs = plt.subplots(gn, 3, squeeze=False, figsize=(10, 2.3*gn) if figsize is None else figsize)
+    fig, axs = plt.subplots(gn, 3, squeeze=False, figsize=(10, 2.3*gn)
+                            if figsize is None else figsize)
     fig.patch.set_facecolor('white')
     for row, gene in enumerate(genes):
-        u = adata[:,gene].layers['Mu' if by == 'expression' else 'velo_u']
-        s = adata[:,gene].layers['Ms' if by == 'expression' else 'velo_s']
-        c = adata[:,gene].layers['ATAC' if by == 'expression' else 'velo_chrom']
+        u = adata[:, gene].layers['Mu' if by == 'expression' else 'velo_u']
+        s = adata[:, gene].layers['Ms' if by == 'expression' else 'velo_s']
+        c = adata[:, gene].layers['ATAC' if by == 'expression'
+                                  else 'velo_chrom']
         c = c.A if sparse.issparse(c) else c
         u = u.A if sparse.issparse(u) else u
         s = s.A if sparse.issparse(s) else s
         c, u, s = np.ravel(c), np.ravel(u), np.ravel(s)
         non_outlier = c <= np.percentile(c, outlier)
         non_outlier &= u <= np.percentile(u, outlier)
         non_outlier &= s <= np.percentile(s, outlier)
         c, u, s = c[non_outlier], u[non_outlier], s[non_outlier]
-        time = np.array(adata[:,gene].layers['fit_t'] if gene_time else latent_time)
+        time = np.array(adata[:, gene].layers['fit_t'] if gene_time
+                        else latent_time)
         if by == 'velocity':
-            time = np.reshape(time, (-1,1))
+            time = np.reshape(time, (-1, 1))
             time = np.ravel(adata.obsp['_RNA_conn'].dot(time))
         time = time[non_outlier]
         if types is not None:
             for i in range(len(types)):
                 if color_by == 'state':
-                    filt = adata[non_outlier,gene].layers['fit_state'] == types[i]
+                    filt = adata[non_outlier, gene].layers['fit_state'] \
+                           == types[i]
                 else:
-                    filt = adata[non_outlier,:].obs[color_by] == types[i]
+                    filt = adata[non_outlier, :].obs[color_by] == types[i]
                 filt = np.ravel(filt)
                 if np.sum(filt) > 0:
-                    axs[row, 0].scatter(time[filt][::downsample], c[filt][::downsample], s=pointsize, c=colors[i], alpha=0.6)
-                    axs[row, 1].scatter(time[filt][::downsample], u[filt][::downsample], s=pointsize, c=colors[i], alpha=0.6)
-                    axs[row, 2].scatter(time[filt][::downsample], s[filt][::downsample], s=pointsize, c=colors[i], alpha=0.6)
-        else:
-            axs[row, 0].scatter(time[::downsample], c[::downsample], s=pointsize, c=colors[non_outlier][::downsample], alpha=0.6, cmap=cmap)
-            axs[row, 1].scatter(time[::downsample], u[::downsample], s=pointsize, c=colors[non_outlier][::downsample], alpha=0.6, cmap=cmap)
-            axs[row, 2].scatter(time[::downsample], s[::downsample], s=pointsize, c=colors[non_outlier][::downsample], alpha=0.6, cmap=cmap)
+                    axs[row, 0].scatter(time[filt][::downsample],
+                                        c[filt][::downsample], s=pointsize,
+                                        c=colors[i], alpha=0.6)
+                    axs[row, 1].scatter(time[filt][::downsample],
+                                        u[filt][::downsample],
+                                        s=pointsize, c=colors[i], alpha=0.6)
+                    axs[row, 2].scatter(time[filt][::downsample],
+                                        s[filt][::downsample], s=pointsize,
+                                        c=colors[i], alpha=0.6)
+        else:
+            axs[row, 0].scatter(time[::downsample], c[::downsample],
+                                s=pointsize,
+                                c=colors[non_outlier][::downsample],
+                                alpha=0.6, cmap=cmap)
+            axs[row, 1].scatter(time[::downsample], u[::downsample],
+                                s=pointsize,
+                                c=colors[non_outlier][::downsample],
+                                alpha=0.6, cmap=cmap)
+            axs[row, 2].scatter(time[::downsample], s[::downsample],
+                                s=pointsize,
+                                c=colors[non_outlier][::downsample],
+                                alpha=0.6, cmap=cmap)
 
         if not gene_time:
             window_count = np.zeros(20)
             window_mean_c = np.zeros(20)
             window_mean_u = np.zeros(20)
             window_mean_s = np.zeros(20)
             for i in np.unique(time_window[non_outlier]):
                 idx = time_window[non_outlier] == i
                 window_count[i] = np.sum(idx)
                 window_mean_c[i] = np.mean(c[idx])
                 window_mean_u[i] = np.mean(u[idx])
                 window_mean_s[i] = np.mean(s[idx])
             window_idx = np.where(window_count > 20)[0]
-            axs[row, 0].plot(window_idx*0.05+0.025, window_mean_c[window_idx], linewidth=linewidth, color='black', alpha=0.5)
-            axs[row, 1].plot(window_idx*0.05+0.025, window_mean_u[window_idx], linewidth=linewidth, color='black', alpha=0.5)
-            axs[row, 2].plot(window_idx*0.05+0.025, window_mean_s[window_idx], linewidth=linewidth, color='black', alpha=0.5)
+            axs[row, 0].plot(window_idx*0.05+0.025, window_mean_c[window_idx],
+                             linewidth=linewidth, color='black', alpha=0.5)
+            axs[row, 1].plot(window_idx*0.05+0.025, window_mean_u[window_idx],
+                             linewidth=linewidth, color='black', alpha=0.5)
+            axs[row, 2].plot(window_idx*0.05+0.025, window_mean_s[window_idx],
+                             linewidth=linewidth, color='black', alpha=0.5)
 
         if show_anchors:
             n_anchors = adata.uns['velo_s_params']['t']
-            t_sw_array = np.array([adata[:,gene].var['fit_t_sw1'], adata[:,gene].var['fit_t_sw2'], adata[:,gene].var['fit_t_sw3']])
+            t_sw_array = np.array([adata[:, gene].var['fit_t_sw1'],
+                                   adata[:, gene].var['fit_t_sw2'],
+                                   adata[:, gene].var['fit_t_sw3']])
             t_sw_array = t_sw_array[t_sw_array < 20]
-            min_idx = int(adata[:,gene].var['fit_anchor_min_idx'])
-            max_idx = int(adata[:,gene].var['fit_anchor_max_idx'])
+            min_idx = int(adata[:, gene].var['fit_anchor_min_idx'])
+            max_idx = int(adata[:, gene].var['fit_anchor_max_idx'])
             old_t = np.linspace(0, 20, n_anchors)[min_idx:max_idx+1]
             new_t = old_t - np.min(old_t)
             new_t = new_t * 20 / np.max(new_t)
             if by == 'velocity' and not full_range:
                 anchor_interval = 20 / (max_idx + 1 - min_idx)
-                min_idx = int(adata[:,gene].var['fit_anchor_velo_min_idx'])
-                max_idx = int(adata[:,gene].var['fit_anchor_velo_max_idx'])
-                start = 0 + (min_idx - adata[:,gene].var['fit_anchor_min_idx']) * anchor_interval
-                end = 20 + (max_idx - adata[:,gene].var['fit_anchor_max_idx']) * anchor_interval
+                min_idx = int(adata[:, gene].var['fit_anchor_velo_min_idx'])
+                max_idx = int(adata[:, gene].var['fit_anchor_velo_max_idx'])
+                start = 0 + (min_idx -
+                             adata[:, gene].var['fit_anchor_min_idx']) \
+                    * anchor_interval
+                end = 20 + (max_idx -
+                            adata[:, gene].var['fit_anchor_max_idx']) \
+                    * anchor_interval
                 new_t = np.linspace(start, end, max_idx + 1 - min_idx)
             ax = axs[row, 0]
-            a_c = adata[:,gene].varm['fit_anchor_c' if by == 'expression' else 'fit_anchor_c_velo'].ravel()[min_idx:max_idx+1]
+            a_c = adata[:, gene].varm['fit_anchor_c' if by == 'expression'
+                                      else 'fit_anchor_c_velo']\
+                                .ravel()[min_idx:max_idx+1]
             if show_switches:
                 for t_sw in t_sw_array:
                     if t_sw > 0:
-                        ax.vlines(t_sw, np.min(c), np.max(c), colors='black', linestyles='dashed', alpha=0.5)
-            ax.plot(new_t[0:new_t.shape[0]], a_c, linewidth=linewidth, color='black', alpha=0.5)
+                        ax.vlines(t_sw, np.min(c), np.max(c), colors='black',
+                                  linestyles='dashed', alpha=0.5)
+            ax.plot(new_t[0:new_t.shape[0]], a_c, linewidth=linewidth,
+                    color='black', alpha=0.5)
             ax = axs[row, 1]
-            a_u = adata[:,gene].varm['fit_anchor_u' if by == 'expression' else 'fit_anchor_u_velo'].ravel()[min_idx:max_idx+1]
+            a_u = adata[:, gene].varm['fit_anchor_u' if by == 'expression'
+                                      else 'fit_anchor_u_velo']\
+                                .ravel()[min_idx:max_idx+1]
             if show_switches:
                 for t_sw in t_sw_array:
                     if t_sw > 0:
-                        ax.vlines(t_sw, np.min(u), np.max(u), colors='black', linestyles='dashed', alpha=0.5)
-            ax.plot(new_t[0:new_t.shape[0]], a_u, linewidth=linewidth, color='black', alpha=0.5)
+                        ax.vlines(t_sw, np.min(u), np.max(u), colors='black',
+                                  linestyles='dashed', alpha=0.5)
+            ax.plot(new_t[0:new_t.shape[0]], a_u, linewidth=linewidth,
+                    color='black', alpha=0.5)
             ax = axs[row, 2]
-            a_s = adata[:,gene].varm['fit_anchor_s' if by == 'expression' else 'fit_anchor_s_velo'].ravel()[min_idx:max_idx+1]
+            a_s = adata[:, gene].varm['fit_anchor_s' if by == 'expression'
+                                      else 'fit_anchor_s_velo']\
+                                .ravel()[min_idx:max_idx+1]
             if show_switches:
                 for t_sw in t_sw_array:
                     if t_sw > 0:
-                        ax.vlines(t_sw, np.min(s), np.max(s), colors='black', linestyles='dashed', alpha=0.5)
-            ax.plot(new_t[0:new_t.shape[0]], a_s, linewidth=linewidth, color='black', alpha=0.5)
+                        ax.vlines(t_sw, np.min(s), np.max(s), colors='black',
+                                  linestyles='dashed', alpha=0.5)
+            ax.plot(new_t[0:new_t.shape[0]], a_s, linewidth=linewidth,
+                    color='black', alpha=0.5)
 
-        axs[row, 0].set_title(f'{gene} ATAC' if by == 'expression' else f'{gene} chromatin velocity')
+        axs[row, 0].set_title(f'{gene} ATAC' if by == 'expression'
+                              else f'{gene} chromatin velocity')
         axs[row, 0].set_xlabel('t' if by == 'expression' else '~t')
         axs[row, 0].set_ylabel('c' if by == 'expression' else 'dc/dt')
-        axs[row, 1].set_title(f'{gene} unspliced' + ('' if by == 'expression' else ' velocity'))
+        axs[row, 1].set_title(f'{gene} unspliced' + ('' if by == 'expression'
+                              else ' velocity'))
         axs[row, 1].set_xlabel('t' if by == 'expression' else '~t')
         axs[row, 1].set_ylabel('u' if by == 'expression' else 'du/dt')
-        axs[row, 2].set_title(f'{gene} spliced' + ('' if by == 'expression' else ' velocity'))
+        axs[row, 2].set_title(f'{gene} spliced' + ('' if by == 'expression'
+                              else ' velocity'))
         axs[row, 2].set_xlabel('t' if by == 'expression' else '~t')
         axs[row, 2].set_ylabel('s' if by == 'expression' else 'ds/dt')
 
         for j in range(3):
             ax = axs[row, j]
             if not axis_on:
                 ax.xaxis.set_ticks_position('none')
@@ -3572,325 +4118,425 @@
             if not frame_on:
                 ax.xaxis.set_ticks_position('none')
                 ax.yaxis.set_ticks_position('none')
                 ax.set_frame_on(False)
     fig.tight_layout()
 
 
-def scatter_plot(adata, 
-                 genes, 
-                 by='us', 
-                 color_by='state', 
-                 n_cols=5, 
-                 axis_on=True, 
-                 frame_on=True, 
-                 show_anchors=True, 
-                 show_switches=True, 
-                 show_all_anchors=False, 
-                 title_more_info=False, 
-                 velocity_arrows=False, 
-                 downsample=1, 
-                 figsize=None, 
-                 pointsize=2, 
-                 markersize=5, 
-                 linewidth=2, 
-                 cmap='coolwarm', 
-                 view_3d_elev=None, 
-                 view_3d_azim=None, 
+def scatter_plot(adata,
+                 genes,
+                 by='us',
+                 color_by='state',
+                 n_cols=5,
+                 axis_on=True,
+                 frame_on=True,
+                 show_anchors=True,
+                 show_switches=True,
+                 show_all_anchors=False,
+                 title_more_info=False,
+                 velocity_arrows=False,
+                 downsample=1,
+                 figsize=None,
+                 pointsize=2,
+                 markersize=5,
+                 linewidth=2,
+                 cmap='coolwarm',
+                 view_3d_elev=None,
+                 view_3d_azim=None,
                  full_name=False
                  ):
     """Gene scatter plot.
 
     This function plots phase portraits of the specified plane.
 
     Parameters
     ----------
     adata: :class:`~anndata.AnnData`
         Anndata result from dynamics recovery.
     genes: `str`,  list of `str`
         List of genes to plot.
     by: `str` (default: `us`)
-        Plot unspliced-spliced plane if `us`. Plot chromatin-unspliced plane if `cu`.
+        Plot unspliced-spliced plane if `us`. Plot chromatin-unspliced plane
+        if `cu`.
         Plot 3D phase portraits if `cus`.
     color_by: `str` (default: `state`)
-        Color by the four potential states if `state`. Other common values are leiden, louvain, celltype, etc.
-        If not `state`, the color field must be present in `.uns`, which can be pre-computed with `scanpy.pl.scatter`.
-        For `state`, red, orange, green, and blue represent state 1, 2, 3, and 4, respectively.
-        When `by=='us'`, `color_by` can also be `c`, which displays the log accessibility on U-S phase portraits.
+        Color by the four potential states if `state`. Other common values are
+        leiden, louvain, celltype, etc.
+        If not `state`, the color field must be present in `.uns`, which can be
+        pre-computed with `scanpy.pl.scatter`.
+        For `state`, red, orange, green, and blue represent state 1, 2, 3, and
+        4, respectively.
+        When `by=='us'`, `color_by` can also be `c`, which displays the log
+        accessibility on U-S phase portraits.
     n_cols: `int` (default: 5)
         Number of columns to plot on each row.
     axis_on: `bool` (default: `True`)
         Whether to show axis labels.
     frame_on: `bool` (default: `True`)
         Whether to show plot frames.
     show_anchors: `bool` (default: `True`)
         Whether to display anchors.
     show_switches: `bool` (default: `True`)
-        Whether to show switch times. The three switch times and the end of trajectory are indicated by 
+        Whether to show switch times. The three switch times and the end of
+        trajectory are indicated by
         circle, cross, dismond, and star, respectively.
     show_all_anchors: `bool` (default: `False`)
-        Whether to display full range of (predicted) anchors even for repression-only genes.
+        Whether to display full range of (predicted) anchors even for
+        repression-only genes.
     title_more_info: `bool` (default: `False`)
-        Whether to display model, direction, and likelihood information for the gene in title.
+        Whether to display model, direction, and likelihood information for
+        the gene in title.
     velocity_arrows: `bool` (default: `False`)
         Whether to show velocity arrows of cells on the phase portraits.
     downsample: `int` (default: 1)
-        How much to downsample the cells. The remaining number will be `1/downsample` of original.
+        How much to downsample the cells. The remaining number will be
+        `1/downsample` of original.
     figsize: `tuple` (default: `None`)
         Total figure size.
     pointsize: `float` (default: 2)
         Point size for scatter plots.
     markersize: `float` (default: 5)
         Point size for switch time points.
     linewidth: `float` (default: 2)
         Line width for connected anchors.
     cmap: `str` (default: `coolwarm`)
-        Color map for log accessibilities or other continuous color keys when plotting on U-S plane.
+        Color map for log accessibilities or other continuous color keys when
+        plotting on U-S plane.
     view_3d_elev: `float` (default: `None`)
-        Matplotlib 3D plot `elev` argument. `elev=90` is the same as U-S plane, and `elev=0` is the same as C-U plane.
+        Matplotlib 3D plot `elev` argument. `elev=90` is the same as U-S plane,
+        and `elev=0` is the same as C-U plane.
     view_3d_azim: `float` (default: `None`)
-        Matplotlib 3D plot `azim` argument. `azim=270` is the same as U-S plane, and `azim=0` is the same as C-U plane.
+        Matplotlib 3D plot `azim` argument. `azim=270` is the same as U-S
+        plane, and `azim=0` is the same as C-U plane.
     full_name: `bool` (default: `False`)
-        Show full names for chromatin, unspliced, and spliced rather than using abbreviated terms c, u, and s.
+        Show full names for chromatin, unspliced, and spliced rather than
+        using abbreviated terms c, u, and s.
     """
     from pandas.api.types import is_numeric_dtype, is_categorical_dtype
     if by not in ['us', 'cu', 'cus']:
         raise ValueError("'by' argument must be one of ['us', 'cu', 'cus']")
     if color_by == 'state':
-        types = [0,1,2,3]
+        types = [0, 1, 2, 3]
         colors = ['tab:red', 'tab:orange', 'tab:green', 'tab:blue']
     elif by == 'us' and color_by == 'c':
         types = None
     elif color_by in adata.obs and is_numeric_dtype(adata.obs[color_by]):
         types = None
         colors = adata.obs[color_by].values
-    elif color_by in adata.obs and is_categorical_dtype(adata.obs[color_by]) and color_by+'_colors' in adata.uns.keys():
+    elif color_by in adata.obs and is_categorical_dtype(adata.obs[color_by]) \
+            and color_by+'_colors' in adata.uns.keys():
         types = adata.obs[color_by].cat.categories
         colors = adata.uns[f'{color_by}_colors']
     else:
-        raise ValueError('Currently, color key must be a single string of either numerical or categorical available in adata obs, and the colors of categories can be found in adata uns.')
+        raise ValueError('Currently, color key must be a single string of '
+                         'either numerical or categorical available in adata'
+                         ' obs, and the colors of categories can be found in'
+                         ' adata uns.')
 
-    if 'velo_s_params' not in adata.uns.keys() or 'fit_anchor_s' not in adata.varm.keys():
+    if 'velo_s_params' not in adata.uns.keys() \
+            or 'fit_anchor_s' not in adata.varm.keys():
         show_anchors = False
     if color_by == 'state' and 'fit_state' not in adata.layers.keys():
-        raise ValueError('fit_state is not found. Please run recover_dynamics_chrom function first or provide a valid color key.')
+        raise ValueError('fit_state is not found. Please run '
+                         'recover_dynamics_chrom function first or provide a '
+                         'valid color key.')
 
     downsample = np.clip(int(downsample), 1, 10)
     genes = np.array(genes)
     missing_genes = genes[~np.isin(genes, adata.var_names)]
     if len(missing_genes) > 0:
         print(f'{missing_genes} not found')
     genes = genes[np.isin(genes, adata.var_names)]
     gn = len(genes)
     if gn == 0:
         return
     if gn < n_cols:
         n_cols = gn
     if by == 'cus':
-        fig, axs = plt.subplots(-(-gn // n_cols), n_cols, squeeze=False, figsize=(3.2*n_cols, 2.7*(-(-gn // n_cols))) if figsize is None else figsize, subplot_kw={'projection':'3d'})
+        fig, axs = plt.subplots(-(-gn // n_cols), n_cols, squeeze=False,
+                                figsize=(3.2*n_cols, 2.7*(-(-gn // n_cols)))
+                                if figsize is None else figsize,
+                                subplot_kw={'projection': '3d'})
     else:
-        fig, axs = plt.subplots(-(-gn // n_cols), n_cols, squeeze=False, figsize=(2.7*n_cols, 2.4*(-(-gn // n_cols))) if figsize is None else figsize)
+        fig, axs = plt.subplots(-(-gn // n_cols), n_cols, squeeze=False,
+                                figsize=(2.7*n_cols, 2.4*(-(-gn // n_cols)))
+                                if figsize is None else figsize)
     fig.patch.set_facecolor('white')
     count = 0
     for gene in genes:
-        u = adata[:,gene].layers['Mu'].copy() if 'Mu' in adata.layers else adata[:,gene].layers['unspliced'].copy()
-        s = adata[:,gene].layers['Ms'].copy() if 'Ms' in adata.layers else adata[:,gene].layers['spliced'].copy()
+        u = adata[:, gene].layers['Mu'].copy() if 'Mu' in adata.layers \
+            else adata[:, gene].layers['unspliced'].copy()
+        s = adata[:, gene].layers['Ms'].copy() if 'Ms' in adata.layers \
+            else adata[:, gene].layers['spliced'].copy()
         u = u.A if sparse.issparse(u) else u
         s = s.A if sparse.issparse(s) else s
         u, s = np.ravel(u), np.ravel(s)
-        if 'ATAC' not in adata.layers.keys() and 'Mc' not in adata.layers.keys():
+        if 'ATAC' not in adata.layers.keys() and \
+                'Mc' not in adata.layers.keys():
             show_anchors = False
         elif 'ATAC' in adata.layers.keys():
-            c = adata[:,gene].layers['ATAC'].copy()
+            c = adata[:, gene].layers['ATAC'].copy()
             c = c.A if sparse.issparse(c) else c
             c = np.ravel(c)
         elif 'Mc' in adata.layers.keys():
-            c = adata[:,gene].layers['Mc'].copy()
+            c = adata[:, gene].layers['Mc'].copy()
             c = c.A if sparse.issparse(c) else c
             c = np.ravel(c)
 
         if velocity_arrows:
             if 'velo_u' in adata.layers.keys():
-                vu = adata[:,gene].layers['velo_u'].copy()
+                vu = adata[:, gene].layers['velo_u'].copy()
             elif 'velocity_u' in adata.layers.keys():
-                vu = adata[:,gene].layers['velocity_u'].copy()
+                vu = adata[:, gene].layers['velocity_u'].copy()
             else:
                 vu = np.zeros(adata.n_obs)
             max_u = np.max([np.max(u), 1e-6])
             u /= max_u
             vu = np.ravel(vu)
             vu /= np.max([np.max(np.abs(vu)), 1e-6])
             if 'velo_s' in adata.layers.keys():
-                vs = adata[:,gene].layers['velo_s'].copy()
+                vs = adata[:, gene].layers['velo_s'].copy()
             elif 'velocity' in adata.layers.keys():
-                vs = adata[:,gene].layers['velocity'].copy()
+                vs = adata[:, gene].layers['velocity'].copy()
             max_s = np.max([np.max(s), 1e-6])
             s /= max_s
             vs = np.ravel(vs)
             vs /= np.max([np.max(np.abs(vs)), 1e-6])
             if 'velo_chrom' in adata.layers.keys():
-                vc = adata[:,gene].layers['velo_chrom'].copy()
+                vc = adata[:, gene].layers['velo_chrom'].copy()
                 max_c = np.max([np.max(c), 1e-6])
                 c /= max_c
                 vc = np.ravel(vc)
                 vc /= np.max([np.max(np.abs(vc)), 1e-6])
 
         row = count // n_cols
         col = count % n_cols
         ax = axs[row, col]
         if types is not None:
             for i in range(len(types)):
                 if color_by == 'state':
-                    filt = adata[:,gene].layers['fit_state'] == types[i]
+                    filt = adata[:, gene].layers['fit_state'] == types[i]
                 else:
                     filt = adata.obs[color_by] == types[i]
                 filt = np.ravel(filt)
                 if by == 'us':
                     if velocity_arrows:
-                        ax.quiver(s[filt][::downsample], u[filt][::downsample], vs[filt][::downsample], vu[filt][::downsample], 
-                                  color=colors[i], alpha=0.5, scale_units='xy', scale=10, width=0.005, headwidth=4, headaxislength=5.5)
+                        ax.quiver(s[filt][::downsample], u[filt][::downsample],
+                                  vs[filt][::downsample],
+                                  vu[filt][::downsample], color=colors[i],
+                                  alpha=0.5, scale_units='xy', scale=10,
+                                  width=0.005, headwidth=4, headaxislength=5.5)
                     else:
-                        ax.scatter(s[filt][::downsample], u[filt][::downsample], s=pointsize, c=colors[i], alpha=0.7)
+                        ax.scatter(s[filt][::downsample],
+                                   u[filt][::downsample], s=pointsize,
+                                   c=colors[i], alpha=0.7)
                 elif by == 'cu':
                     if velocity_arrows:
-                        ax.quiver(u[filt][::downsample], c[filt][::downsample], vu[filt][::downsample], vc[filt][::downsample], 
-                                  color=colors[i], alpha=0.5, scale_units='xy', scale=10, width=0.005, headwidth=4, headaxislength=5.5)
+                        ax.quiver(u[filt][::downsample],
+                                  c[filt][::downsample],
+                                  vu[filt][::downsample],
+                                  vc[filt][::downsample], color=colors[i],
+                                  alpha=0.5, scale_units='xy', scale=10,
+                                  width=0.005, headwidth=4, headaxislength=5.5)
                     else:
-                        ax.scatter(u[filt][::downsample], c[filt][::downsample], s=pointsize, c=colors[i], alpha=0.7)
+                        ax.scatter(u[filt][::downsample],
+                                   c[filt][::downsample], s=pointsize,
+                                   c=colors[i], alpha=0.7)
                 else:
                     if velocity_arrows:
-                        ax.quiver(s[filt][::downsample], u[filt][::downsample], c[filt][::downsample], 
-                                  vs[filt][::downsample], vu[filt][::downsample], vc[filt][::downsample], 
-                                  color=colors[i], alpha=0.4, length=0.1, arrow_length_ratio=0.5, normalize=True)
+                        ax.quiver(s[filt][::downsample],
+                                  u[filt][::downsample], c[filt][::downsample],
+                                  vs[filt][::downsample],
+                                  vu[filt][::downsample],
+                                  vc[filt][::downsample],
+                                  color=colors[i], alpha=0.4, length=0.1,
+                                  arrow_length_ratio=0.5, normalize=True)
                     else:
-                        ax.scatter(s[filt][::downsample], u[filt][::downsample], c[filt][::downsample], s=pointsize, c=colors[i], alpha=0.7)
+                        ax.scatter(s[filt][::downsample],
+                                   u[filt][::downsample],
+                                   c[filt][::downsample], s=pointsize,
+                                   c=colors[i], alpha=0.7)
         elif color_by == 'c':
-            if 'velo_s_params' in adata.uns.keys() and 'outlier' in adata.uns['velo_s_params']:
+            if 'velo_s_params' in adata.uns.keys() and \
+                    'outlier' in adata.uns['velo_s_params']:
                 outlier = adata.uns['velo_s_params']['outlier']
             else:
                 outlier = 99.8
             non_zero = (u > 0) & (s > 0) & (c > 0)
             non_outlier = u < np.percentile(u, outlier)
             non_outlier &= s < np.percentile(s, outlier)
             non_outlier &= c < np.percentile(c, outlier)
             c -= np.min(c)
             c /= np.max(c)
             if velocity_arrows:
-                ax.quiver(s[non_zero & non_outlier][::downsample], u[non_zero & non_outlier][::downsample], 
-                          vs[non_zero & non_outlier][::downsample], vu[non_zero & non_outlier][::downsample], 
-                          np.log1p(c[non_zero & non_outlier][::downsample]), alpha=0.5, 
-                          scale_units='xy', scale=10, width=0.005, headwidth=4, headaxislength=5.5, cmap=cmap)
+                ax.quiver(s[non_zero & non_outlier][::downsample],
+                          u[non_zero & non_outlier][::downsample],
+                          vs[non_zero & non_outlier][::downsample],
+                          vu[non_zero & non_outlier][::downsample],
+                          np.log1p(c[non_zero & non_outlier][::downsample]),
+                          alpha=0.5,
+                          scale_units='xy', scale=10, width=0.005,
+                          headwidth=4, headaxislength=5.5, cmap=cmap)
             else:
-                ax.scatter(s[non_zero & non_outlier][::downsample], u[non_zero & non_outlier][::downsample], s=pointsize, 
-                           c=np.log1p(c[non_zero & non_outlier][::downsample]), alpha=0.8, cmap=cmap)
+                ax.scatter(s[non_zero & non_outlier][::downsample],
+                           u[non_zero & non_outlier][::downsample],
+                           s=pointsize,
+                           c=np.log1p(c[non_zero & non_outlier][::downsample]),
+                           alpha=0.8, cmap=cmap)
         else:
             if by == 'us':
                 if velocity_arrows:
-                    ax.quiver(s[::downsample], u[::downsample], vs[::downsample], vu[::downsample], 
-                              colors[::downsample], alpha=0.5, scale_units='xy', scale=10, width=0.005, headwidth=4, headaxislength=5.5, cmap=cmap)
+                    ax.quiver(s[::downsample], u[::downsample],
+                              vs[::downsample], vu[::downsample],
+                              colors[::downsample], alpha=0.5,
+                              scale_units='xy', scale=10, width=0.005,
+                              headwidth=4, headaxislength=5.5, cmap=cmap)
                 else:
-                    ax.scatter(s[::downsample], u[::downsample], s=pointsize, c=colors[::downsample], alpha=0.7, cmap=cmap)
+                    ax.scatter(s[::downsample], u[::downsample], s=pointsize,
+                               c=colors[::downsample], alpha=0.7, cmap=cmap)
             elif by == 'cu':
                 if velocity_arrows:
-                    ax.quiver(u[::downsample], c[::downsample], vu[::downsample], vc[::downsample], 
-                              colors[::downsample], alpha=0.5, scale_units='xy', scale=10, width=0.005, headwidth=4, headaxislength=5.5, cmap=cmap)
+                    ax.quiver(u[::downsample], c[::downsample],
+                              vu[::downsample], vc[::downsample],
+                              colors[::downsample], alpha=0.5,
+                              scale_units='xy', scale=10, width=0.005,
+                              headwidth=4, headaxislength=5.5, cmap=cmap)
                 else:
-                    ax.scatter(u[::downsample], c[::downsample], s=pointsize, c=colors[::downsample], alpha=0.7, cmap=cmap)
+                    ax.scatter(u[::downsample], c[::downsample], s=pointsize,
+                               c=colors[::downsample], alpha=0.7, cmap=cmap)
             else:
                 if velocity_arrows:
-                    ax.quiver(s[::downsample], u[::downsample], c[::downsample], 
-                              vs[::downsample], vu[::downsample], vc[::downsample], 
-                              colors[::downsample], alpha=0.4, length=0.1, arrow_length_ratio=0.5, normalize=True, cmap=cmap)
+                    ax.quiver(s[::downsample], u[::downsample],
+                              c[::downsample], vs[::downsample],
+                              vu[::downsample], vc[::downsample],
+                              colors[::downsample], alpha=0.4, length=0.1,
+                              arrow_length_ratio=0.5, normalize=True,
+                              cmap=cmap)
                 else:
-                    ax.scatter(s[::downsample], u[::downsample], c[::downsample], s=pointsize, c=colors[::downsample], alpha=0.7, cmap=cmap)
+                    ax.scatter(s[::downsample], u[::downsample],
+                               c[::downsample], s=pointsize,
+                               c=colors[::downsample], alpha=0.7, cmap=cmap)
 
         if show_anchors:
-            min_idx = int(adata[:,gene].var['fit_anchor_min_idx'])
-            max_idx = int(adata[:,gene].var['fit_anchor_max_idx'])
-            a_c = adata[:,gene].varm['fit_anchor_c'].ravel()[min_idx:max_idx+1].copy()
-            a_u = adata[:,gene].varm['fit_anchor_u'].ravel()[min_idx:max_idx+1].copy()
-            a_s = adata[:,gene].varm['fit_anchor_s'].ravel()[min_idx:max_idx+1].copy()
+            min_idx = int(adata[:, gene].var['fit_anchor_min_idx'])
+            max_idx = int(adata[:, gene].var['fit_anchor_max_idx'])
+            a_c = adata[:, gene].varm['fit_anchor_c']\
+                .ravel()[min_idx:max_idx+1].copy()
+            a_u = adata[:, gene].varm['fit_anchor_u']\
+                .ravel()[min_idx:max_idx+1].copy()
+            a_s = adata[:, gene].varm['fit_anchor_s']\
+                .ravel()[min_idx:max_idx+1].copy()
             if velocity_arrows:
                 a_c /= max_c
                 a_u /= max_u
                 a_s /= max_s
             if by == 'us':
-                ax.plot(a_s, a_u, linewidth=linewidth, color='black', alpha=0.7, zorder=1000)
+                ax.plot(a_s, a_u, linewidth=linewidth, color='black',
+                        alpha=0.7, zorder=1000)
             elif by == 'cu':
-                ax.plot(a_u, a_c, linewidth=linewidth, color='black', alpha=0.7, zorder=1000)
+                ax.plot(a_u, a_c, linewidth=linewidth, color='black',
+                        alpha=0.7, zorder=1000)
             else:
-                ax.plot(a_s, a_u, a_c, linewidth=linewidth, color='black', alpha=0.7, zorder=1000)
+                ax.plot(a_s, a_u, a_c, linewidth=linewidth, color='black',
+                        alpha=0.7, zorder=1000)
             if show_all_anchors:
-                a_c_pre = adata[:,gene].varm['fit_anchor_c'].ravel()[:min_idx].copy()
-                a_u_pre = adata[:,gene].varm['fit_anchor_u'].ravel()[:min_idx].copy()
-                a_s_pre = adata[:,gene].varm['fit_anchor_s'].ravel()[:min_idx].copy()
+                a_c_pre = adata[:, gene].varm['fit_anchor_c']\
+                    .ravel()[:min_idx].copy()
+                a_u_pre = adata[:, gene].varm['fit_anchor_u']\
+                    .ravel()[:min_idx].copy()
+                a_s_pre = adata[:, gene].varm['fit_anchor_s']\
+                    .ravel()[:min_idx].copy()
                 if velocity_arrows:
                     a_c_pre /= max_c
                     a_u_pre /= max_u
                     a_s_pre /= max_s
                 if len(a_c_pre) > 0:
                     if by == 'us':
-                        ax.plot(a_s_pre, a_u_pre, linewidth=linewidth/1.3, color='black', alpha=0.6, zorder=1000)
+                        ax.plot(a_s_pre, a_u_pre, linewidth=linewidth/1.3,
+                                color='black', alpha=0.6, zorder=1000)
                     elif by == 'cu':
-                        ax.plot(a_u_pre, a_c_pre, linewidth=linewidth/1.3, color='black', alpha=0.6, zorder=1000)
+                        ax.plot(a_u_pre, a_c_pre, linewidth=linewidth/1.3,
+                                color='black', alpha=0.6, zorder=1000)
                     else:
-                        ax.plot(a_s_pre, a_u_pre, a_c_pre, linewidth=linewidth/1.3, color='black', alpha=0.6, zorder=1000)
+                        ax.plot(a_s_pre, a_u_pre, a_c_pre,
+                                linewidth=linewidth/1.3, color='black',
+                                alpha=0.6, zorder=1000)
             if show_switches:
-                t_sw_array = np.array([adata[:,gene].var['fit_t_sw1'].values[0], adata[:,gene].var['fit_t_sw2'].values[0], adata[:,gene].var['fit_t_sw3'].values[0]])
+                t_sw_array = np.array([adata[:, gene].var['fit_t_sw1']
+                                      .values[0],
+                                      adata[:, gene].var['fit_t_sw2']
+                                      .values[0],
+                                      adata[:, gene].var['fit_t_sw3']
+                                      .values[0]])
                 in_range = (t_sw_array > 0) & (t_sw_array < 20)
-                a_c_sw = adata[:,gene].varm['fit_anchor_c_sw'].ravel().copy()
-                a_u_sw = adata[:,gene].varm['fit_anchor_u_sw'].ravel().copy()
-                a_s_sw = adata[:,gene].varm['fit_anchor_s_sw'].ravel().copy()
+                a_c_sw = adata[:, gene].varm['fit_anchor_c_sw'].ravel().copy()
+                a_u_sw = adata[:, gene].varm['fit_anchor_u_sw'].ravel().copy()
+                a_s_sw = adata[:, gene].varm['fit_anchor_s_sw'].ravel().copy()
                 if velocity_arrows:
                     a_c_sw /= max_c
                     a_u_sw /= max_u
                     a_s_sw /= max_s
                 if in_range[0]:
                     c_sw1, u_sw1, s_sw1 = a_c_sw[0], a_u_sw[0], a_s_sw[0]
                     if by == 'us':
-                        ax.plot([s_sw1], [u_sw1], "om", markersize=markersize, zorder=2000)
+                        ax.plot([s_sw1], [u_sw1], "om", markersize=markersize,
+                                zorder=2000)
                     elif by == 'cu':
-                        ax.plot([u_sw1], [c_sw1], "om", markersize=markersize, zorder=2000)
+                        ax.plot([u_sw1], [c_sw1], "om", markersize=markersize,
+                                zorder=2000)
                     else:
-                        ax.plot([s_sw1], [u_sw1], [c_sw1], "om", markersize=markersize, zorder=2000)
+                        ax.plot([s_sw1], [u_sw1], [c_sw1], "om",
+                                markersize=markersize, zorder=2000)
                 if in_range[1]:
                     c_sw2, u_sw2, s_sw2 = a_c_sw[1], a_u_sw[1], a_s_sw[1]
                     if by == 'us':
-                        ax.plot([s_sw2], [u_sw2], "Xm", markersize=markersize, zorder=2000)
+                        ax.plot([s_sw2], [u_sw2], "Xm", markersize=markersize,
+                                zorder=2000)
                     elif by == 'cu':
-                        ax.plot([u_sw2], [c_sw2], "Xm", markersize=markersize, zorder=2000)
+                        ax.plot([u_sw2], [c_sw2], "Xm", markersize=markersize,
+                                zorder=2000)
                     else:
-                        ax.plot([s_sw2], [u_sw2], [c_sw2], "Xm", markersize=markersize, zorder=2000)
+                        ax.plot([s_sw2], [u_sw2], [c_sw2], "Xm",
+                                markersize=markersize, zorder=2000)
                 if in_range[2]:
                     c_sw3, u_sw3, s_sw3 = a_c_sw[2], a_u_sw[2], a_s_sw[2]
                     if by == 'us':
-                        ax.plot([s_sw3], [u_sw3], "Dm", markersize=markersize, zorder=2000)
+                        ax.plot([s_sw3], [u_sw3], "Dm", markersize=markersize,
+                                zorder=2000)
                     elif by == 'cu':
-                        ax.plot([u_sw3], [c_sw3], "Dm", markersize=markersize, zorder=2000)
+                        ax.plot([u_sw3], [c_sw3], "Dm", markersize=markersize,
+                                zorder=2000)
                     else:
-                        ax.plot([s_sw3], [u_sw3], [c_sw3], "Dm", markersize=markersize, zorder=2000)
+                        ax.plot([s_sw3], [u_sw3], [c_sw3], "Dm",
+                                markersize=markersize, zorder=2000)
                 if max_idx > adata.uns['velo_s_params']['t'] - 4:
                     if by == 'us':
-                        ax.plot([a_s[-1]], [a_u[-1]], "*m", markersize=markersize, zorder=2000)
+                        ax.plot([a_s[-1]], [a_u[-1]], "*m",
+                                markersize=markersize, zorder=2000)
                     elif by == 'cu':
-                        ax.plot([a_u[-1]], [a_c[-1]], "*m", markersize=markersize, zorder=2000)
+                        ax.plot([a_u[-1]], [a_c[-1]], "*m",
+                                markersize=markersize, zorder=2000)
                     else:
-                        ax.plot([a_s[-1]], [a_u[-1]], [a_c[-1]], "*m", markersize=markersize, zorder=2000)
+                        ax.plot([a_s[-1]], [a_u[-1]], [a_c[-1]], "*m",
+                                markersize=markersize, zorder=2000)
 
-        if by == 'cus' and (view_3d_elev is not None or view_3d_azim is not None):
+        if by == 'cus' and \
+                (view_3d_elev is not None or view_3d_azim is not None):
             # US: elev=90, azim=270. CU: elev=0, azim=0.
             ax.view_init(elev=view_3d_elev, azim=view_3d_azim)
         title = gene
         if title_more_info:
             if 'fit_model' in adata.var:
                 title += f" M{int(adata[:,gene].var['fit_model'].values[0])}"
             if 'fit_direction' in adata.var:
                 title += f" {adata[:,gene].var['fit_direction'].values[0]}"
-            if 'fit_likelihood' in adata.var and not np.all(adata.var['fit_likelihood'].values==-1):
-                title += f" {adata[:,gene].var['fit_likelihood'].values[0]:.3g}"
+            if 'fit_likelihood' in adata.var \
+                    and not np.all(adata.var['fit_likelihood'].values == -1):
+                title += " "
+                f"{adata[:,gene].var['fit_likelihood'].values[0]:.3g}"
         ax.set_title(f'{title}', fontsize=11)
         if by == 'us':
             ax.set_xlabel('spliced' if full_name else 's')
             ax.set_ylabel('unspliced' if full_name else 'u')
         elif by == 'cu':
             ax.set_xlabel('unspliced' if full_name else 'u')
             ax.set_ylabel('chromatin' if full_name else 'c')
@@ -3913,17 +4559,17 @@
                 ax.set_xlabel('')
                 ax.set_ylabel('')
                 ax.set_zlabel('')
                 ax.xaxis.set_ticklabels([])
                 ax.yaxis.set_ticklabels([])
                 ax.zaxis.set_ticklabels([])
             if not frame_on:
-                ax.xaxis._axinfo['grid']['color'] =  (1,1,1,0)
-                ax.yaxis._axinfo['grid']['color'] =  (1,1,1,0)
-                ax.zaxis._axinfo['grid']['color'] =  (1,1,1,0)
+                ax.xaxis._axinfo['grid']['color'] = (1, 1, 1, 0)
+                ax.yaxis._axinfo['grid']['color'] = (1, 1, 1, 0)
+                ax.zaxis._axinfo['grid']['color'] = (1, 1, 1, 0)
                 ax.xaxis._axinfo['tick']['inward_factor'] = 0
                 ax.xaxis._axinfo['tick']['outward_factor'] = 0
                 ax.yaxis._axinfo['tick']['inward_factor'] = 0
                 ax.yaxis._axinfo['tick']['outward_factor'] = 0
                 ax.zaxis._axinfo['tick']['inward_factor'] = 0
                 ax.zaxis._axinfo['tick']['outward_factor'] = 0
         count += 1
```

### Comparing `multivelo-0.1.2/src/multivelo/steady_chrom_func.py` & `multivelo-0.1.3/src/multivelo/steady_chrom_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 import os
 import warnings
 import numpy as np
-from numpy.linalg import norm
-import matplotlib.pyplot as plt
 from scipy import sparse
-from scipy.sparse import csr_matrix, issparse, diags
-from anndata import AnnData
-import scanpy as sc
+from scipy.sparse import csr_matrix, issparse
 from scanpy import Neighbors
-import scvelo as scv
 import pandas as pd
-import seaborn as sns
 from tqdm.auto import tqdm
-import ipywidgets
 from joblib import Parallel, delayed
 
 
 class ChromatinVelocity:
-    def __init__(self, c, u, s, 
-                 ss, us, 
-                 gene=None, 
-                 verbose=False, 
-                 save_plot=False, 
-                 plot_dir=None, 
-                 fit_args=None, 
-                 rna_only=False, 
-                 extra_color=None, 
-                 r2_adjusted=True, 
+    def __init__(self, c, u, s,
+                 ss, us,
+                 gene=None,
+                 verbose=False,
+                 save_plot=False,
+                 plot_dir=None,
+                 fit_args=None,
+                 rna_only=False,
+                 extra_color=None,
+                 r2_adjusted=True,
                  ):
 
         self.gene = gene
         self.verbose = verbose
 
         # fitting arguments
         self.rna_only = rna_only
         self.outlier = np.clip(fit_args['outlier'], 80, 100)
         self.r2_adjusted = r2_adjusted
 
         # plot parameters
-        self.save_plot=save_plot
+        self.save_plot = save_plot
         self.extra_color = extra_color
         self.fig_size = fit_args['fig_size']
         self.point_size = fit_args['point_size']
         if plot_dir is None:
             self.plot_path = 'plots_steady_state'
         else:
             self.plot_path = plot_dir
@@ -64,33 +57,42 @@
         self.s_all = np.ravel(np.array(s, dtype=np.float64))
         if ss is not None:
             self.ss_all = np.ravel(np.array(ss, dtype=np.float64))
         if us is not None:
             self.us_all = np.ravel(np.array(us, dtype=np.float64))
 
         # adjust offset
-        self.offset_c, self.offset_u, self.offset_s = np.min(self.c_all), np.min(self.u_all), np.min(self.s_all)
+        self.offset_c, self.offset_u, self.offset_s = np.min(self.c_all), \
+            np.min(self.u_all), \
+            np.min(self.s_all)
         self.offset_c = 0 if self.rna_only else self.offset_c
         self.c_all -= self.offset_c
         self.u_all -= self.offset_u
         self.s_all -= self.offset_s
         # remove zero counts
-        self.non_zero = np.ravel(self.c_all > 0) | np.ravel(self.u_all > 0) | np.ravel(self.s_all > 0)
+        self.non_zero = np.ravel(self.c_all > 0) | np.ravel(self.u_all > 0) | \
+            np.ravel(self.s_all > 0)
         # remove outliers
-        self.non_outlier = np.ravel(self.c_all <= np.percentile(self.c_all, self.outlier))
-        self.non_outlier &= np.ravel(self.u_all <= np.percentile(self.u_all, self.outlier))
-        self.non_outlier &= np.ravel(self.s_all <= np.percentile(self.s_all, self.outlier))
+        self.non_outlier = np.ravel(self.c_all <=
+                                    np.percentile(self.c_all, self.outlier))
+        self.non_outlier &= np.ravel(self.u_all <=
+                                     np.percentile(self.u_all, self.outlier))
+        self.non_outlier &= np.ravel(self.s_all <=
+                                     np.percentile(self.s_all, self.outlier))
         self.c = self.c_all[self.non_zero & self.non_outlier]
         self.u = self.u_all[self.non_zero & self.non_outlier]
         self.s = self.s_all[self.non_zero & self.non_outlier]
-        self.ss = None if ss is None else self.ss_all[self.non_zero & self.non_outlier]
-        self.us = None if us is None else self.us_all[self.non_zero & self.non_outlier]
+        self.ss = (None if ss is None
+                   else self.ss_all[self.non_zero & self.non_outlier])
+        self.us = (None if us is None
+                   else self.us_all[self.non_zero & self.non_outlier])
         self.low_quality = len(self.u) < 10
         if self.verbose >= 2:
-            print(f'{len(self.u)} cells passed filter and will be used to fit regressions.')
+            print(f'{len(self.u)} cells passed filter and will be used to fit'
+                  ' regressions.')
 
         # 4 rate parameters
         self.alpha_c = 0.1
         self.alpha = 0.0
         self.beta = 0.0
         self.gamma = 0.0
 
@@ -98,18 +100,22 @@
         self.loss = np.inf
         self.r2 = 0
         self.residual = None
         self.residual2 = None
         self.steady_state_func = None
 
         # select cells for regression
-        w_sub = (self.c >= 0.1 * np.max(self.c)) & (self.u >= 0.1 * np.max(self.u)) & (self.s >= 0.1 * np.max(self.s))
+        w_sub = (self.c >= 0.1 * np.max(self.c)) & \
+                (self.u >= 0.1 * np.max(self.u)) & \
+                (self.s >= 0.1 * np.max(self.s))
         c_sub = self.c[w_sub]
         if not self.rna_only:
-            w_sub = (self.c >= np.mean(c_sub)+np.std(c_sub)) & (self.u >= 0.1 * np.max(self.u)) & (self.s >= 0.1 * np.max(self.s))
+            w_sub = (self.c >= np.mean(c_sub)+np.std(c_sub)) & \
+                    (self.u >= 0.1 * np.max(self.u)) & \
+                    (self.s >= 0.1 * np.max(self.s))
         self.w_sub = w_sub
         if np.sum(self.w_sub) < 10:
             self.low_quality = True
 
     def compute_deterministic(self):
         if self.rna_only:
             # steady-state slope
@@ -134,15 +140,14 @@
         if self.r2_adjusted:
             gamma = np.dot(self.u, self.s) / np.dot(self.s, self.s)
             residual = self.u_all - gamma * self.s_all
 
         total = self.u_all - np.mean(self.u_all)
         self.r2 = 1 - np.dot(residual, residual) / np.dot(total, total)
 
-
     def compute_stochastic(self):
         self.compute_deterministic()
 
         var_ss = 2 * self.ss - self.s
         cov_us = 2 * self.us + self.u
         s_all_ = 2 * self.s_all**2 - (2 * self.ss_all - self.s_all)
         u_all_ = (2 * self.us_all + self.u_all) - 2 * self.u_all*self.s_all
@@ -172,128 +177,134 @@
             b = np.hstack((ss_u / std_first, cov_us[self.w_sub] / std_second))
         gamma = np.dot(b, a) / np.dot(a, a)
         self.steady_state_func = lambda x: gamma*x
         self.residual = self.u_all - self.steady_state_func(self.s_all)
         self.residual2 = u_all_ - self.steady_state_func(s_all_)
         self.loss = np.dot(self.residual, self.residual) / len(self.u_all)
 
-
     def get_velocity(self):
         return self.residual
 
-
     def get_variance_velocity(self):
         return self.residual2
 
-
     def get_r2(self):
         return self.r2
 
-
     def get_loss(self):
         return self.loss
 
 
-def regress_func(c,u,s,ss,us,m,v,sp,pdir,fa,gene,ro,extra):
+def regress_func(c, u, s, ss, us, m, v, sp, pdir, fa, gene, ro, extra):
 
     c_90 = np.percentile(c, 90)
     u_90 = np.percentile(u, 90)
     s_90 = np.percentile(s, 90)
-    low_quality = (u_90 == 0 or s_90 == 0) if ro else (c_90 == 0 or u_90 == 0 or s_90 == 0)
+    low_quality = ((u_90 == 0 or s_90 == 0) if ro
+                   else (c_90 == 0 or u_90 == 0 or s_90 == 0))
     if low_quality:
         if v >= 1:
             print(f'low quality gene {gene}, skipping')
         return np.zeros(len(u)), np.zeros(len(u)), 0, np.inf
 
-    cvc = ChromatinVelocity(c, 
-                            u, 
-                            s, 
-                            ss, 
-                            us, 
-                            verbose=v, 
-                            save_plot=sp, 
-                            plot_dir=pdir, 
-                            fit_args=fa, 
-                            gene=gene, 
-                            rna_only=ro, 
+    cvc = ChromatinVelocity(c,
+                            u,
+                            s,
+                            ss,
+                            us,
+                            verbose=v,
+                            save_plot=sp,
+                            plot_dir=pdir,
+                            fit_args=fa,
+                            gene=gene,
+                            rna_only=ro,
                             extra_color=extra)
     if cvc.low_quality:
         return np.zeros(len(u)), np.zeros(len(u)), 0, np.inf
 
     if m == 'deterministic':
         cvc.compute_deterministic()
     elif m == 'stochastic':
         cvc.compute_stochastic()
     velocity = cvc.get_velocity()
     r2 = cvc.get_r2()
     loss = cvc.get_loss()
-    variance_velocity = None if m == 'deterministic' else cvc.get_variance_velocity()
+    variance_velocity = (None if m == 'deterministic'
+                         else cvc.get_variance_velocity())
     return velocity, variance_velocity, r2, loss
 
 
-def velocity_chrom(adata_rna, 
-                   adata_atac=None, 
-                   gene_list=None, 
-                   mode='stochastic', 
-                   verbose=False, 
-                   parallel=True, 
-                   n_jobs=None, 
-                   save_plot=False, 
+def velocity_chrom(adata_rna,
+                   adata_atac=None,
+                   gene_list=None,
+                   mode='stochastic',
+                   verbose=False,
+                   parallel=True,
+                   n_jobs=None,
+                   save_plot=False,
                    plot_dir=None,
-                   rna_only=False, 
-                   extra_color_key=None, 
-                   min_r2=1e-2, 
-                   outlier=99.8, 
-                   n_pcs=30, 
-                   n_neighbors=30, 
-                   fig_size=(8,6), 
+                   rna_only=False,
+                   extra_color_key=None,
+                   min_r2=1e-2,
+                   outlier=99.8,
+                   n_pcs=30,
+                   n_neighbors=30,
+                   fig_size=(8, 6),
                    point_size=7
                    ):
 
     """Multi-omic steady-state model.
 
-    This function incorporates chromatin accessibilities into RNA steady-state velocity.
+    This function incorporates chromatin accessibilities into RNA steady-state
+    velocity.
 
     Parameters
     ----------
     adata_rna: :class:`~anndata.AnnData`
         RNA anndata object. Required fields: `Mu`, `Ms`, and `connectivities`.
     adata_atac: :class:`~anndata.AnnData` (default: `None`)
         ATAC anndata object. Required fields: `Mc`.
     gene_list: `str`,  list of `str` (default: highly variable genes)
         Genes to use for model fitting.
     mode: `str` (default: `'stochastic'`)
-        Fitting method. 
-        `'stochastic'`: computing steady-state ratio with the first and second moments.
+        Fitting method.
+        `'stochastic'`: computing steady-state ratio with the first and second
+        moments.
         `'deterministic'`: computing steady-state ratio with the first moments.
     verbose: `int` or `bool` (default: `False`)
-        Level of fitting detail to output. Possible values: `False`, 0, 1, 2, or any number above 2.
+        Level of fitting detail to output. Possible values: `False`, 0, 1, 2,
+        or any number above 2.
     parallel: `bool` (default: `True`)
         Whether to fit genes in a parallel fashion (recommended).
     n_jobs: `int` (default: available threads)
         Number of parallel jobs.
     save_plot: `bool` (default: `False`)
-        Whether to save the fitted gene portrait figures as files. This will take some disk space.
-    plot_dir: `str` (default: `plots` for multiome and `rna_plots` for RNA-only)
+        Whether to save the fitted gene portrait figures as files. This will
+        take some disk space.
+    plot_dir: `str` (default: `plots` for multiome and `rna_plots` for
+    RNA-only)
         Directory to save the plots.
     rna_only: `bool` (default: `False`)
         Whether to only use RNA for fitting (RNA velocity).
     extra_color_key: `str` (default: `None`)
-        Extra color key used for plotting. Common choices are `leiden`, `celltype`, etc. 
-        The colors for each category must be present in one of anndatas, which can be pre-computed 
+        Extra color key used for plotting. Common choices are `leiden`,
+        `celltype`, etc.
+        The colors for each category must be present in one of anndatas, which
+        can be pre-computed.
         with `scanpy.pl.scatter` function.
     min_r2: `float` (default: 1e-2)
         Minimum R-squared value for selecting velocity genes.
     outlier: `float` (default: 99.8)
-        The percentile to mark as outlier that will be excluded when fitting the model.
+        The percentile to mark as outlier that will be excluded when fitting
+        the model.
     n_pcs: `int` (default: 30)
-        Number of principal components to compute distance smoothing neighbors. 
+        Number of principal components to compute distance smoothing neighbors.
         This can be different from the one used for expression smoothing.
     n_neighbors: `int` (default: 30)
-        Number of nearest neighbors for distance smoothing. 
+        Number of nearest neighbors for distance smoothing.
         This can be different from the one used for expression smoothing.
     fig_size: `tuple` (default: (8,6))
         Size of each figure when saved.
     point_size: `float` (default: 7)
         Marker point size for plotting.
 
     Returns
@@ -318,94 +329,122 @@
     fit_args['min_r2'] = min_r2
     fit_args['outlier'] = outlier
     fit_args['n_pcs'] = n_pcs
     fit_args['n_neighbors'] = n_neighbors
     fit_args['fig_size'] = list(fig_size)
     fit_args['point_size'] = point_size
     if mode == 'dynamical':
-        print('You do not need to run mv.velocity for chromatin dynamical model')
+        print('You do not need to run mv.velocity for chromatin dynamical '
+              'model')
         return
     elif mode == 'stochastic' or mode == 'deterministic':
         fit_args['mode'] = mode
     else:
-        raise ValueError('Unknown mode. Must be either stochastic or deterministic')
+        raise ValueError('Unknown mode. Must be either stochastic or '
+                         'deterministic')
 
     all_genes = adata_rna.var_names
     if adata_atac is None:
         import anndata as ad
-        from scipy.sparse import diags
         rna_only = True
-        adata_atac = ad.AnnData(X=np.ones(adata_rna.shape), obs=adata_rna.obs, var=adata_rna.var)
+        adata_atac = ad.AnnData(X=np.ones(adata_rna.shape), obs=adata_rna.obs,
+                                var=adata_rna.var)
         adata_atac.layers['Mc'] = np.ones(adata_rna.shape)
     if adata_rna.shape != adata_atac.shape:
-        raise ValueError(f'Shape of RNA and ATAC adata objects do not match: {adata_rna.shape} {adata_atac.shape}')
+        raise ValueError('Shape of RNA and ATAC adata objects do not match:'
+                         f'{adata_rna.shape} {adata_atac.shape}')
     if not np.all(adata_rna.obs_names == adata_atac.obs_names):
-        raise ValueError('obs_names of RNA and ATAC adata objects do not match, please check if they are consistent')
+        raise ValueError('obs_names of RNA and ATAC adata objects do not '
+                         'match, please check if they are consistent')
     if not np.all(all_genes == adata_atac.var_names):
-        raise ValueError('var_names of RNA and ATAC adata objects do not match, please check if they are consistent')
+        raise ValueError('var_names of RNA and ATAC adata objects do not '
+                         'match, please check if they are consistent')
     if extra_color_key is None:
         extra_color = None
-    elif isinstance(extra_color_key, str) and extra_color_key in adata_rna.obs and adata_rna.obs[extra_color_key].dtype.name == 'category':
+    elif (isinstance(extra_color_key, str) and extra_color_key in adata_rna.obs
+          and adata_rna.obs[extra_color_key].dtype.name == 'category'):
         ngroups = len(adata_rna.obs[extra_color_key].cat.categories)
-        extra_color = adata_rna.obs[extra_color_key].cat.rename_categories(adata_rna.uns[extra_color_key+'_colors'][:ngroups]).to_numpy()
-    elif isinstance(extra_color_key, str) and extra_color_key in adata_atac.obs and adata_rna.obs[extra_color_key].dtype.name == 'category':
+        extra_color = adata_rna.obs[extra_color_key].cat.rename_categories(
+            adata_rna.uns[extra_color_key+'_colors'][:ngroups]).to_numpy()
+    elif (isinstance(extra_color_key, str)
+          and extra_color_key in adata_atac.obs and
+          adata_rna.obs[extra_color_key].dtype.name == 'category'):
         ngroups = len(adata_atac.obs[extra_color_key].cat.categories)
-        extra_color = adata_atac.obs[extra_color_key].cat.rename_categories(adata_atac.uns[extra_color_key+'_colors'][:ngroups]).to_numpy()
+        extra_color = adata_atac.obs[extra_color_key].cat.rename_categories(
+            adata_atac.uns[extra_color_key+'_colors'][:ngroups]).to_numpy()
     else:
-        raise ValueError('Currently, extra_color_key must be a single string of categories and available in adata obs, and its colors can be found in adata uns')
-    if 'connectivities' not in adata_rna.obsp.keys() or (adata_rna.obsp['connectivities'] > 0).sum(1).min() > (n_neighbors-1):
+        raise ValueError('Currently, extra_color_key must be a single string '
+                         'of categories and available in adata obs, and its '
+                         'colors can be found in adata uns')
+    if ('connectivities' not in adata_rna.obsp.keys() or
+            (adata_rna.obsp['connectivities'] > 0).sum(1).min()
+            > (n_neighbors-1)):
         neighbors = Neighbors(adata_rna)
-        neighbors.compute_neighbors(n_neighbors=n_neighbors, knn=True, n_pcs=n_pcs)
+        neighbors.compute_neighbors(n_neighbors=n_neighbors,
+                                    knn=True, n_pcs=n_pcs)
         rna_conn = neighbors.connectivities
     else:
         rna_conn = adata_rna.obsp['connectivities'].copy()
     rna_conn.setdiag(1)
     rna_conn = rna_conn.multiply(1.0 / rna_conn.sum(1)).tocsr()
 
     Mss, Mus = None, None
     if mode == 'stochastic':
         Mss, Mus = second_order_moments(adata_rna)
 
     if gene_list is None:
         if 'highly_variable' in adata_rna.var:
-            gene_list = adata_rna.var_names[adata_rna.var['highly_variable']].values
+            gene_list = adata_rna.var_names[
+                adata_rna.var['highly_variable']].values
         else:
-            gene_list = adata_rna.var_names.values[(~np.isnan(np.asarray(adata_rna.layers['Mu'].sum(0)).reshape(-1) 
-                                                                if sparse.issparse(adata_rna.layers['Mu']) 
-                                                                else np.sum(adata_rna.layers['Mu'], axis=0)))
-                                                   & (~np.isnan(np.asarray(adata_rna.layers['Ms'].sum(0)).reshape(-1) 
-                                                                if sparse.issparse(adata_rna.layers['Ms']) 
-                                                                else np.sum(adata_rna.layers['Ms'], axis=0)))
-                                                   & (~np.isnan(np.asarray(adata_atac.layers['Mc'].sum(0)).reshape(-1) 
-                                                                if sparse.issparse(adata_atac.layers['Mc']) 
-                                                                else np.sum(adata_atac.layers['Mc'], axis=0)))]
-    elif isinstance(gene_list,(list, np.ndarray, pd.Index, pd.Series)):
+            gene_list = adata_rna.var_names.values[
+                (~np.isnan(np.asarray(adata_rna.layers['Mu'].sum(0))
+                           .reshape(-1)
+                           if sparse.issparse(adata_rna.layers['Mu'])
+                           else np.sum(adata_rna.layers['Mu'], axis=0)))
+                & (~np.isnan(np.asarray(adata_rna.layers['Ms'].sum(0))
+                             .reshape(-1)
+                             if sparse.issparse(adata_rna.layers['Ms'])
+                             else np.sum(adata_rna.layers['Ms'], axis=0)))
+                & (~np.isnan(np.asarray(adata_atac.layers['Mc'].sum(0))
+                             .reshape(-1)
+                             if sparse.issparse(adata_atac.layers['Mc'])
+                             else np.sum(adata_atac.layers['Mc'], axis=0)))]
+    elif isinstance(gene_list, (list, np.ndarray, pd.Index, pd.Series)):
         gene_list = np.array([x for x in gene_list if x in all_genes])
     elif isinstance(gene_list, str):
         gene_list = np.array([gene_list]) if gene_list in all_genes else []
     else:
-        raise ValueError('Invalid gene list, must be one of (str, np.ndarray, pd.Index, pd.Series)')
+        raise ValueError('Invalid gene list, must be one of (str, np.ndarray,'
+                         ' pd.Index, pd.Series)')
     gn = len(gene_list)
     if gn == 0:
         raise ValueError('None of the genes specified are in the adata object')
     if verbose is True:
         verbose = 1
     if verbose >= 1:
         print(f'{gn} genes will be fitted')
 
     velo_s = np.zeros((adata_rna.n_obs, gn))
     variance_velo_s = np.zeros((adata_rna.n_obs, gn))
     r2s = np.zeros(gn)
     losses = np.zeros(gn)
 
-    u_mat = adata_rna[:,gene_list].layers['Mu'].A if sparse.issparse(adata_rna.layers['Mu']) else adata_rna[:,gene_list].layers['Mu']
-    s_mat = adata_rna[:,gene_list].layers['Ms'].A if sparse.issparse(adata_rna.layers['Ms']) else adata_rna[:,gene_list].layers['Ms']
-    c_mat = adata_atac[:,gene_list].layers['Mc'].A if sparse.issparse(adata_atac.layers['Mc']) else adata_atac[:,gene_list].layers['Mc']
+    u_mat = (adata_rna[:, gene_list].layers['Mu'].A
+             if sparse.issparse(adata_rna.layers['Mu'])
+             else adata_rna[:, gene_list].layers['Mu'])
+    s_mat = (adata_rna[:, gene_list].layers['Ms'].A
+             if sparse.issparse(adata_rna.layers['Ms'])
+             else adata_rna[:, gene_list].layers['Ms'])
+    c_mat = (adata_atac[:, gene_list].layers['Mc'].A
+             if sparse.issparse(adata_atac.layers['Mc'])
+             else adata_atac[:, gene_list].layers['Mc'])
     if parallel:
-        if n_jobs is None or not isinstance(n_jobs, int) or n_jobs < 0 or n_jobs > os.cpu_count():
+        if (n_jobs is None or not isinstance(n_jobs, int) or
+                n_jobs < 0 or n_jobs > os.cpu_count()):
             n_jobs = os.cpu_count()
         if n_jobs > gn:
             n_jobs = gn
         batches = -(-gn // n_jobs)
         if n_jobs > 1 and verbose >= 1:
             print(f'running {n_jobs} jobs in parallel')
     else:
@@ -416,80 +455,85 @@
 
     pbar = tqdm(total=gn)
     for group in range(batches):
         gene_indices = range(group * n_jobs, np.min([gn, (group+1) * n_jobs]))
         if parallel:
             verb = 5 if verbose >= 2 else 0
             verbose = False
-            plot = False
 
             res = Parallel(n_jobs=n_jobs, backend='loky', verbose=verb)(
                 delayed(regress_func)(
-                    c_mat[:,i], 
-                    u_mat[:,i], 
-                    s_mat[:,i], 
-                    None if mode == 'deterministic' else Mss[:,i], 
-                    None if mode == 'deterministic' else Mus[:,i], 
-                    mode, 
-                    verbose, 
-                    save_plot, 
-                    plot_dir, 
-                    fit_args, 
-                    gene_list[i], 
-                    rna_only, 
-                    extra_color) 
+                    c_mat[:, i],
+                    u_mat[:, i],
+                    s_mat[:, i],
+                    None if mode == 'deterministic' else Mss[:, i],
+                    None if mode == 'deterministic' else Mus[:, i],
+                    mode,
+                    verbose,
+                    save_plot,
+                    plot_dir,
+                    fit_args,
+                    gene_list[i],
+                    rna_only,
+                    extra_color)
                 for i in gene_indices)
 
-            for i,r in zip(gene_indices, res):
+            for i, r in zip(gene_indices, res):
                 velocity, variance_velocity, r2, loss = r
                 r2s[i] = r2
                 losses[i] = loss
-                velo_s[:,i] = smooth_scale(rna_conn, velocity)
+                velo_s[:, i] = smooth_scale(rna_conn, velocity)
                 if mode == 'stochastic':
-                    variance_velo_s[:,i] = smooth_scale(rna_conn, variance_velocity)
+                    variance_velo_s[:, i] = smooth_scale(rna_conn,
+                                                         variance_velocity)
 
         else:
             i = group
             gene = gene_list[i]
             if verbose >= 1:
                 print(f'@@@@@fitting {gene}')
-            velocity, variance_velocity, r2, loss = regress_func(c_mat[:,i], 
-                                                                 u_mat[:,i], 
-                                                                 s_mat[:,i], 
-                                                                 None if mode == 'deterministic' else Mss[:,i], 
-                                                                 None if mode == 'deterministic' else Mus[:,i], 
-                                                                 mode, 
-                                                                 verbose, 
-                                                                 save_plot, 
-                                                                 plot_dir, 
-                                                                 fit_args, 
-                                                                 gene_list[i], 
-                                                                 rna_only, 
-                                                                 extra_color)
+            velocity, variance_velocity, r2, loss = \
+                regress_func(c_mat[:, i],
+                             u_mat[:, i],
+                             s_mat[:, i],
+                             None
+                             if mode == 'deterministic' else Mss[:, i],
+                             None if mode == 'deterministic' else Mus[:, i],
+                             mode,
+                             verbose,
+                             save_plot,
+                             plot_dir,
+                             fit_args,
+                             gene_list[i],
+                             rna_only,
+                             extra_color)
             r2s[i] = r2
             losses[i] = loss
-            velo_s[:,i] = smooth_scale(rna_conn, velocity)
+            velo_s[:, i] = smooth_scale(rna_conn, velocity)
             if mode == 'stochastic':
-                variance_velo_s[:,i] = smooth_scale(rna_conn, variance_velocity)
+                variance_velo_s[:, i] = smooth_scale(rna_conn,
+                                                     variance_velocity)
         pbar.update(len(gene_indices))
     pbar.close()
 
     filt = losses != np.inf
     if np.sum(filt) == 0:
-        raise ValueError('None of the genes were fitted due to low quality, not returning')
-    adata_copy = adata_rna[:,gene_list[filt]].copy()
-    adata_copy.layers['ATAC'] = c_mat[:,filt]
+        raise ValueError('None of the genes were fitted due to low quality, '
+                         'not returning')
+    adata_copy = adata_rna[:, gene_list[filt]].copy()
+    adata_copy.layers['ATAC'] = c_mat[:, filt]
     adata_copy.var['fit_loss'] = losses[filt]
     adata_copy.var['fit_r2'] = r2s[filt]
-    adata_copy.layers['velo_s'] = velo_s[:,filt]
+    adata_copy.layers['velo_s'] = velo_s[:, filt]
     if mode == 'stochastic':
-        adata_copy.layers['variance_velo_s'] = variance_velo_s[:,filt]
+        adata_copy.layers['variance_velo_s'] = variance_velo_s[:, filt]
     v_genes = adata_copy.var['fit_r2'] >= min_r2
     adata_copy.var['velo_s_genes'] = v_genes
-    adata_copy.uns['velo_s_params'] = {'mode': mode, 'fit_offset': False, 'perc': 95}
+    adata_copy.uns['velo_s_params'] = {'mode': mode, 'fit_offset': False,
+                                       'perc': 95}
     adata_copy.uns['velo_s_params'].update(fit_args)
     adata_copy.obsp['_RNA_conn'] = rna_conn
     return adata_copy
 
 
 def smooth_scale(conn, vector):
     max_to = np.max(vector)
@@ -497,23 +541,25 @@
     v = conn.dot(vector.T).T
     max_from = np.max(v)
     min_from = np.min(v)
     res = ((v - min_from) * (max_to - min_to) / (max_from - min_from)) + min_to
     return res
 
 
-##########################################################################################
-# The following functions are taken directly from scVelo preprocessing [Bergen et al., 2020] (https://github.com/theislab/scvelo)
-##########################################################################################
+###############################################################################
+# The following functions are taken directly from scVelo preprocessing
+# [Bergen et al., 2020] (https://github.com/theislab/scvelo)
+###############################################################################
 
 def select_connectivities(connectivities, n_neighbors=None):
     C = connectivities.copy()
     n_counts = (C > 0).sum(1).A1 if issparse(C) else (C > 0).sum(1)
     n_neighbors = (
-        n_counts.min() if n_neighbors is None else min(n_counts.min(), n_neighbors)
+        n_counts.min() if n_neighbors is None else min(n_counts.min(),
+                                                       n_neighbors)
     )
     rows = np.where(n_counts > n_neighbors)[0]
     cumsum_neighs = np.insert(n_counts.cumsum(), 0, 0)
     dat = C.data
 
     for row in rows:
         n0, n1 = cumsum_neighs[row], cumsum_neighs[row + 1]
@@ -529,33 +575,36 @@
     elif "neighbors" in adata.uns.keys() and mode in adata.uns["neighbors"]:
         return adata.uns["neighbors"][mode]
     else:
         raise ValueError("The selected mode is not valid.")
 
 
 def get_n_neighs(adata):
-    return adata.uns.get("neighbors", {}).get("params", {}).get("n_neighbors", 0)
+    return (adata.uns.get("neighbors", {}).get("params", {})
+            .get("n_neighbors", 0))
 
 
-def get_connectivities(adata, mode="connectivities", n_neighbors=None, recurse_neighbors=False):
+def get_connectivities(adata, mode="connectivities", n_neighbors=None,
+                       recurse_neighbors=False):
     if "neighbors" in adata.uns.keys():
         C = get_neighs(adata, mode)
         if n_neighbors is not None and n_neighbors < get_n_neighs(adata):
             if mode == "connectivities":
                 C = select_connectivities(C, n_neighbors)
             else:
                 C = select_distances(C, n_neighbors)
         connectivities = C > 0
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             connectivities.setdiag(1)
             if recurse_neighbors:
                 connectivities += connectivities.dot(connectivities * 0.5)
                 connectivities.data = np.clip(connectivities.data, 0, 1)
-            connectivities = connectivities.multiply(1.0 / connectivities.sum(1))
+            connectivities = connectivities.multiply(1.0 /
+                                                     connectivities.sum(1))
         return connectivities.tocsr().astype(np.float32)
     else:
         return None
 
 
 def second_order_moments(adata, adjusted=False):
     """Computes second order moments for stochastic velocity estimation.
@@ -567,19 +616,21 @@
     -------
     Mss: Second order moments for spliced abundances
     Mus: Second order moments for spliced with unspliced abundances
     """
 
     if "neighbors" not in adata.uns:
         raise ValueError(
-            "You need to run `pp.neighbors` first to compute a neighborhood graph."
+            "You need to run `pp.neighbors` first to compute a neighborhood "
+            "graph."
         )
 
     connectivities = get_connectivities(adata)
-    s, u = csr_matrix(adata.layers["spliced"]), csr_matrix(adata.layers["unspliced"])
+    s, u = csr_matrix(adata.layers["spliced"]), \
+        csr_matrix(adata.layers["unspliced"])
     if s.shape[0] == 1:
         s, u = s.T, u.T
     Mss = csr_matrix.dot(connectivities, s.multiply(s)).astype(np.float32).A
     Mus = csr_matrix.dot(connectivities, s.multiply(u)).astype(np.float32).A
     if adjusted:
         Mss = 2 * Mss - adata.layers["Ms"].reshape(Mss.shape)
         Mus = 2 * Mus - adata.layers["Mu"].reshape(Mus.shape)
```

### Comparing `multivelo-0.1.2/src/multivelo.egg-info/PKG-INFO` & `multivelo-0.1.3/src/multivelo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multivelo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Multi-omic extension of single-cell RNA velocity
 Home-page: https://github.com/welch-lab/MultiVelo
 Author: Chen Li
 Author-email: chlseven@umich.edu
 License: BSD 3-Clause License
 Keywords: RNA velocity,single-cell,transcriptomics,chromatin,epigenetic,epigenomic,gene regulation,multi-omic,dynamical
 Classifier: Development Status :: 4 - Beta
@@ -35,26 +35,47 @@
 MultiVelo uses a probabilistic latent variable model to estimate the switch time and rate 
 parameters of gene regulation, providing a quantitative summary of the temporal relationship 
 between epigenomic and transcriptomic changes. Fitting MultiVelo on single-cell multi-omic 
 datasets revealed two distinct mechanisms of regulation by chromatin accessibility, quantified 
 the degree of concordance or discordance between transcriptomic and epigenomic states within 
 each cell, and inferred the lengths of time lags between transcriptomic and epigenomic changes.
 
-Install through PyPI: **pip install multivelo**
+Installation
+------------
 
-**New**: `ReadTheDocs <https://multivelo.readthedocs.io/en/latest/>`_ page is up. You can find detailed parameter descriptions and tutorials on the website.
+Install through PyPI: 
 
-A tutorial showing how to run MultiVelo can be found in `multivelo_demo <https://github.com/welch-lab/MultiVelo/tree/main/multivelo_demo>`_.
+``pip install multivelo``
 
-We use the embryonic E18 mouse brain from 10X Multiome as an example (`jupyter notebook <https://github.com/welch-lab/MultiVelo/tree/main/multivelo_demo/MultiVelo_Demo.ipynb>`_).
+The package is also available on Bioconda. Install with:
 
+``conda install -c bioconda multivelo`` or ``mamba install -c bioconda multivelo``
+
+Documentation
+-------------
+
+We have a `ReadTheDocs <https://multivelo.readthedocs.io/en/latest/>`_ page.
+
+Tutorial
+--------
+
+*New*: we have added Jupyter notebooks showing how to reproduce the main figure panels, along with all required processed data files. These can be found under the `Examples <https://github.com/welch-lab/MultiVelo/tree/main/Examples>`_ folder in this repository or on our `ReadTheDocs <https://multivelo.readthedocs.io/en/latest/>`_ page.
+
+A tutorial showing how to run MultiVelo can be found here: (`jupyter notebook <https://github.com/welch-lab/MultiVelo/blob/main/Examples/MultiVelo_Demo.ipynb>`_)
+
+The tutorial uses the embryonic E18 mouse brain from 10X Multiome as an example.
 CellRanger output files can be downloaded from 
 `10X website <https://www.10xgenomics.com/resources/datasets/fresh-embryonic-e-18-mouse-brain-5-k-1-standard-1-0-0>`_. 
 Crucially, the filtered feature barcode matrix folder, ATAC peak annotations TSV, and the feature 
 linkage BEDPE file in the secondary analysis outputs folder will be needed in this demo.
 
 You can download the processed data that we used for this analysis if you want to run the example yourself. 
 Unspliced and spliced counts, as well as cell type annotations can be downloaded from the MultiVelo GitHub page. 
 We provide the cell annotations for this dataset in "cell_annotations.tsv". 
 We also provide the nearest neighbor graph used to smooth chromatin accessibility values in the GitHub folder "seurat_wnn", 
 which contains a zip file of three files: "nn_cells.txt", "nn_dist.txt", and "nn_idx.txt". Please unzip the archive after downloading. 
 The R script used to generate these files can also be found in the same folder.
+
+Citation
+--------
+
+| Li, C., Virgilio, M.C., Collins, K.L. & Welch J.D. Multi-omic single-cell velocity models epigenome–transcriptome interactions and improves cell fate prediction. *Nat Biotechnol* (2022).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

