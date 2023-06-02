# Comparing `tmp/liqa-1.1.8.tar.gz` & `tmp/liqa-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/liqa-1.1.8.tar", last modified: Fri Jan 22 03:11:23 2021, max compression
+gzip compressed data, was "liqa-1.2.tar", last modified: Fri Jun  2 15:39:43 2023, max compression
```

## Comparing `liqa-1.1.8.tar` & `liqa-1.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-sr-x   0 huy4     (995663) wang_lab_hpc (85000781)        0 2021-01-22 03:11:23.000000 liqa-1.1.8/
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)     1048 2021-01-19 23:02:49.000000 liqa-1.1.8/LICENSE
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)       25 2021-01-19 23:02:54.000000 liqa-1.1.8/MANIFEST.in
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)     2125 2021-01-22 03:11:23.000000 liqa-1.1.8/PKG-INFO
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)     1472 2021-01-20 19:48:26.000000 liqa-1.1.8/README.md
-drwxr-sr-x   0 huy4     (995663) wang_lab_hpc (85000781)        0 2021-01-22 03:11:23.000000 liqa-1.1.8/liqa.egg-info/
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)     2125 2021-01-22 03:11:19.000000 liqa-1.1.8/liqa.egg-info/PKG-INFO
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)      289 2021-01-22 03:11:20.000000 liqa-1.1.8/liqa.egg-info/SOURCES.txt
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)        1 2021-01-22 03:11:19.000000 liqa-1.1.8/liqa.egg-info/dependency_links.txt
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)       45 2021-01-22 03:11:19.000000 liqa-1.1.8/liqa.egg-info/entry_points.txt
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)       16 2021-01-22 03:11:19.000000 liqa-1.1.8/liqa.egg-info/requires.txt
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)       18 2021-01-22 03:11:19.000000 liqa-1.1.8/liqa.egg-info/top_level.txt
-drwxr-sr-x   0 huy4     (995663) wang_lab_hpc (85000781)        0 2021-01-22 03:11:23.000000 liqa-1.1.8/liqa_src/
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)     2707 2021-01-22 03:09:30.000000 liqa-1.1.8/liqa_src/liqa.py
-drwxr-sr-x   0 huy4     (995663) wang_lab_hpc (85000781)        0 2021-01-22 03:11:23.000000 liqa-1.1.8/liqa_src/liqa_bin/
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)     2949 2020-12-07 20:53:20.000000 liqa-1.1.8/liqa_src/liqa_bin/my_functions.py
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)    25717 2020-12-20 22:16:23.000000 liqa-1.1.8/liqa_src/liqa_bin/quantify.py
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)       38 2021-01-22 03:11:23.000000 liqa-1.1.8/setup.cfg
--rw-r--r--   0 huy4     (995663) wang_lab_hpc (85000781)      965 2021-01-22 03:10:46.000000 liqa-1.1.8/setup.py
+drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-06-02 15:39:43.529716 liqa-1.2/
+-rw-r--r--   0 wenli      (501) staff       (20)      693 2023-06-02 14:46:22.000000 liqa-1.2/LICENSE
+-rw-r--r--   0 wenli      (501) staff       (20)       25 2023-06-02 14:46:22.000000 liqa-1.2/MANIFEST.in
+-rw-r--r--   0 wenli      (501) staff       (20)     2193 2023-06-02 15:39:43.529585 liqa-1.2/PKG-INFO
+-rw-r--r--   0 wenli      (501) staff       (20)     1743 2023-06-02 14:46:22.000000 liqa-1.2/README.md
+drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-06-02 15:39:43.523308 liqa-1.2/liqa.egg-info/
+-rw-r--r--   0 wenli      (501) staff       (20)     2193 2023-06-02 15:39:43.000000 liqa-1.2/liqa.egg-info/PKG-INFO
+-rw-r--r--   0 wenli      (501) staff       (20)      366 2023-06-02 15:39:43.000000 liqa-1.2/liqa.egg-info/SOURCES.txt
+-rw-r--r--   0 wenli      (501) staff       (20)        1 2023-06-02 15:39:43.000000 liqa-1.2/liqa.egg-info/dependency_links.txt
+-rw-r--r--   0 wenli      (501) staff       (20)       44 2023-06-02 15:39:43.000000 liqa-1.2/liqa.egg-info/entry_points.txt
+-rw-r--r--   0 wenli      (501) staff       (20)       16 2023-06-02 15:39:43.000000 liqa-1.2/liqa.egg-info/requires.txt
+-rw-r--r--   0 wenli      (501) staff       (20)        9 2023-06-02 15:39:43.000000 liqa-1.2/liqa.egg-info/top_level.txt
+drwxr-xr-x   0 wenli      (501) staff       (20)        0 2023-06-02 15:39:43.528860 liqa-1.2/liqa_src/
+-rw-r--r--   0 wenli      (501) staff       (20)     5381 2023-06-02 14:46:22.000000 liqa-1.2/liqa_src/PreProcess.pl
+-rw-r--r--   0 wenli      (501) staff       (20)     6619 2023-06-02 14:46:22.000000 liqa-1.2/liqa_src/PreProcess_gtf.pl
+-rw-r--r--   0 wenli      (501) staff       (20)     2302 2023-06-02 14:46:22.000000 liqa-1.2/liqa_src/group_process.pl
+-rw-r--r--   0 wenli      (501) staff       (20)     4087 2023-06-02 14:46:22.000000 liqa-1.2/liqa_src/liqa.py
+-rw-r--r--   0 wenli      (501) staff       (20)     2949 2023-06-02 14:46:22.000000 liqa-1.2/liqa_src/my_functions.py
+-rw-r--r--   0 wenli      (501) staff       (20)    26418 2023-06-02 14:46:22.000000 liqa-1.2/liqa_src/quantify.py
+-rw-r--r--   0 wenli      (501) staff       (20)     5750 2023-06-02 14:46:22.000000 liqa-1.2/liqa_src/testDAS.R
+-rw-r--r--   0 wenli      (501) staff       (20)       38 2023-06-02 15:39:43.529754 liqa-1.2/setup.cfg
+-rw-r--r--   0 wenli      (501) staff       (20)     1153 2023-06-02 15:39:02.000000 liqa-1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `liqa-1.1.8/PKG-INFO` & `liqa-1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 Metadata-Version: 2.1
 Name: liqa
-Version: 1.1.8
+Version: 1.2
 Summary: A statistical tool to quantify isoform-specific expression using long-read RNA-seq
 Home-page: https://github.com/WGLab/LIQA
 Author: Yu Hu
 Author-email: huyu999999@gmail.com
 License: MIT
-Description: # Long-read Isoform Quantification and Analysis
-        LIQA (Long-read Isoform Quantification and Analysis) is an Expectation-Maximization based statistical method to quantify isoform expression and detect differential alternative splicing (DAS) events using long-read RNA-seq data. LIQA incorporates base-pair quality score and isoform-specific read length information to assign different weights across reads instead of summarizing isoform-specific read counts directly. Moreover, LIQA can detect DAS events between conditions using isoform usage estimates.
-        
-        ## Computational pipeline of LIQA
-        <p align="center">
-          <img width="575" height="406" src="doc/liqa_flowchart.png">
-        </p>
-        
-        ## Inputs of LIQA
-        The input of LIQA is long-read RNA-seq read data in BAM format together with a refrence isoform annotation file.
-        
-        ## Installation
-        Please refer to [Installation](https://github.com/WGLab/LIQA/blob/master/doc/Install.md) for how to install LIQA.
-        
-        ## Usage
-        Please refere to [Usage](https://github.com/WGLab/LIQA/blob/master/doc/Usage.md) for how to use LIQA.
-        
-        ## Contact
-        
-        If you have any questions/issues/bugs, please post them on [GitHub](https://github.com/WGLab/LIQA/issues). They would also be helpful to other users. 
-        
-        ## Citation
-        
-        Yu Hu, Li Fang, Xuelian Chen, Jiang F. Zhong, Mingyao Li, Kai Wang. LIQA: Long-read Isoform Quantification and Analysis. 2020. bioRxiv doi: [https://doi.org/10.1101/2020.09.09.289793](https://www.biorxiv.org/content/10.1101/2020.09.09.289793v1)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Long-read Isoform Quantification and Analysis
+
+[![DOI](https://zenodo.org/badge/257630000.svg)](https://zenodo.org/badge/latestdoi/257630000)
+
+LIQA (Long-read Isoform Quantification and Analysis) is an Expectation-Maximization based statistical method to quantify isoform expression and detect differential alternative splicing (DAS) events using long-read RNA-seq data. LIQA incorporates base-pair quality score and isoform-specific read length information to assign different weights across reads instead of summarizing isoform-specific read counts directly. Moreover, LIQA can detect DAS events between conditions using isoform usage estimates.
+
+## Computational pipeline of LIQA
+<p align="center">
+  <img width="575" height="406" src="doc/liqa_flowchart.png">
+</p>
+
+## Inputs of LIQA
+The input of LIQA is long-read RNA-seq read data in BAM format together with a refrence isoform annotation file.
+
+## Installation
+Please refer to [Installation](https://github.com/WGLab/LIQA/blob/master/doc/Install.md) for how to install LIQA.
+
+## Usage
+Please refere to [Usage](https://github.com/WGLab/LIQA/blob/master/doc/Usage.md) for how to use LIQA.
+
+## Examples of isoform analysis using LIQA.
+
+Please refer to [Demo and Examples](https://github.com/WGLab/LIQA/blob/master/doc/Examples.md) for examples of how to use LIQA.
+
+## Contact
+
+If you have any questions/issues/bugs, please post them on [GitHub](https://github.com/WGLab/LIQA/issues). They would also be helpful to other users. 
+
+## Citation
+
+Yu Hu, Li Fang, Xuelian Chen, Jiang F. Zhong, Mingyao Li, Kai Wang. LIQA: Long-read Isoform Quantification and Analysis. 2020. bioRxiv doi: [https://doi.org/10.1101/2020.09.09.289793](https://www.biorxiv.org/content/10.1101/2020.09.09.289793v1)
```

### Comparing `liqa-1.1.8/README.md` & `liqa-1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # Long-read Isoform Quantification and Analysis
+
+[![DOI](https://zenodo.org/badge/257630000.svg)](https://zenodo.org/badge/latestdoi/257630000)
+
 LIQA (Long-read Isoform Quantification and Analysis) is an Expectation-Maximization based statistical method to quantify isoform expression and detect differential alternative splicing (DAS) events using long-read RNA-seq data. LIQA incorporates base-pair quality score and isoform-specific read length information to assign different weights across reads instead of summarizing isoform-specific read counts directly. Moreover, LIQA can detect DAS events between conditions using isoform usage estimates.
 
 ## Computational pipeline of LIQA
 <p align="center">
   <img width="575" height="406" src="doc/liqa_flowchart.png">
 </p>
 
@@ -11,14 +14,18 @@
 
 ## Installation
 Please refer to [Installation](https://github.com/WGLab/LIQA/blob/master/doc/Install.md) for how to install LIQA.
 
 ## Usage
 Please refere to [Usage](https://github.com/WGLab/LIQA/blob/master/doc/Usage.md) for how to use LIQA.
 
+## Examples of isoform analysis using LIQA.
+
+Please refer to [Demo and Examples](https://github.com/WGLab/LIQA/blob/master/doc/Examples.md) for examples of how to use LIQA.
+
 ## Contact
 
 If you have any questions/issues/bugs, please post them on [GitHub](https://github.com/WGLab/LIQA/issues). They would also be helpful to other users. 
 
 ## Citation
 
 Yu Hu, Li Fang, Xuelian Chen, Jiang F. Zhong, Mingyao Li, Kai Wang. LIQA: Long-read Isoform Quantification and Analysis. 2020. bioRxiv doi: [https://doi.org/10.1101/2020.09.09.289793](https://www.biorxiv.org/content/10.1101/2020.09.09.289793v1)
```

### Comparing `liqa-1.1.8/liqa.egg-info/PKG-INFO` & `liqa-1.2/liqa.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 Metadata-Version: 2.1
 Name: liqa
-Version: 1.1.8
+Version: 1.2
 Summary: A statistical tool to quantify isoform-specific expression using long-read RNA-seq
 Home-page: https://github.com/WGLab/LIQA
 Author: Yu Hu
 Author-email: huyu999999@gmail.com
 License: MIT
-Description: # Long-read Isoform Quantification and Analysis
-        LIQA (Long-read Isoform Quantification and Analysis) is an Expectation-Maximization based statistical method to quantify isoform expression and detect differential alternative splicing (DAS) events using long-read RNA-seq data. LIQA incorporates base-pair quality score and isoform-specific read length information to assign different weights across reads instead of summarizing isoform-specific read counts directly. Moreover, LIQA can detect DAS events between conditions using isoform usage estimates.
-        
-        ## Computational pipeline of LIQA
-        <p align="center">
-          <img width="575" height="406" src="doc/liqa_flowchart.png">
-        </p>
-        
-        ## Inputs of LIQA
-        The input of LIQA is long-read RNA-seq read data in BAM format together with a refrence isoform annotation file.
-        
-        ## Installation
-        Please refer to [Installation](https://github.com/WGLab/LIQA/blob/master/doc/Install.md) for how to install LIQA.
-        
-        ## Usage
-        Please refere to [Usage](https://github.com/WGLab/LIQA/blob/master/doc/Usage.md) for how to use LIQA.
-        
-        ## Contact
-        
-        If you have any questions/issues/bugs, please post them on [GitHub](https://github.com/WGLab/LIQA/issues). They would also be helpful to other users. 
-        
-        ## Citation
-        
-        Yu Hu, Li Fang, Xuelian Chen, Jiang F. Zhong, Mingyao Li, Kai Wang. LIQA: Long-read Isoform Quantification and Analysis. 2020. bioRxiv doi: [https://doi.org/10.1101/2020.09.09.289793](https://www.biorxiv.org/content/10.1101/2020.09.09.289793v1)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Long-read Isoform Quantification and Analysis
+
+[![DOI](https://zenodo.org/badge/257630000.svg)](https://zenodo.org/badge/latestdoi/257630000)
+
+LIQA (Long-read Isoform Quantification and Analysis) is an Expectation-Maximization based statistical method to quantify isoform expression and detect differential alternative splicing (DAS) events using long-read RNA-seq data. LIQA incorporates base-pair quality score and isoform-specific read length information to assign different weights across reads instead of summarizing isoform-specific read counts directly. Moreover, LIQA can detect DAS events between conditions using isoform usage estimates.
+
+## Computational pipeline of LIQA
+<p align="center">
+  <img width="575" height="406" src="doc/liqa_flowchart.png">
+</p>
+
+## Inputs of LIQA
+The input of LIQA is long-read RNA-seq read data in BAM format together with a refrence isoform annotation file.
+
+## Installation
+Please refer to [Installation](https://github.com/WGLab/LIQA/blob/master/doc/Install.md) for how to install LIQA.
+
+## Usage
+Please refere to [Usage](https://github.com/WGLab/LIQA/blob/master/doc/Usage.md) for how to use LIQA.
+
+## Examples of isoform analysis using LIQA.
+
+Please refer to [Demo and Examples](https://github.com/WGLab/LIQA/blob/master/doc/Examples.md) for examples of how to use LIQA.
+
+## Contact
+
+If you have any questions/issues/bugs, please post them on [GitHub](https://github.com/WGLab/LIQA/issues). They would also be helpful to other users. 
+
+## Citation
+
+Yu Hu, Li Fang, Xuelian Chen, Jiang F. Zhong, Mingyao Li, Kai Wang. LIQA: Long-read Isoform Quantification and Analysis. 2020. bioRxiv doi: [https://doi.org/10.1101/2020.09.09.289793](https://www.biorxiv.org/content/10.1101/2020.09.09.289793v1)
```

### Comparing `liqa-1.1.8/liqa_src/liqa_bin/my_functions.py` & `liqa-1.2/liqa_src/my_functions.py`

 * *Files identical despite different names*

### Comparing `liqa-1.1.8/liqa_src/liqa_bin/quantify.py` & `liqa-1.2/liqa_src/quantify.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,17 @@
         if not bool(geneStructureInformation[gene]):
             geneLineCount[gene] = 0
             geneStructureInformation[gene][geneLineCount[gene]] = line
         else:
             geneLineCount[gene] += 1
             geneStructureInformation[gene][geneLineCount[gene]] = line
 
+#if weightF <= 1:
+    #weightF = 0
+infthreshold = float(weightF)/10.0
 
 #####################################
 ## Using pysam to read in bam file !!
 #####################################
 bamFilePysam = pysam.Samfile(bamFile,"rb")
 
 
@@ -104,15 +107,15 @@
 ##########################################################################################################################
 
 geneCount = 0
 
 startTime = time.time()
 
 #OUT.write("GeneName\tIsoformName\tNumberOfReads\tRelativeAbundance\n") ## Header of Results
-OUT.write("GeneName\tIsoformName\tRelativeAbundance\tReadPerGene_corrected\n")
+OUT.write("GeneName\tIsoformName\tReadPerGene_corrected\tRelativeAbundance\tinfor_ratio\n")
 
 for gene in geneStructureInformation:
 
     geneCount += 1
     tmpTime = (time.time() - startTime)/60.0
     
     
@@ -137,15 +140,15 @@
             tmpisolength[iii] = (int(tmpisolength[iii]) - geneStart)
             if tmpisolength[iii] == 666:
                 tmpisolength[iii] = 0
             else:
                 tmpisolength[iii] = tmpisolength[iii]/2566
             #print(gene+"\t"+str(tmpisolength[iii]))
     else:
-        genelength = 1
+        genelength = 100
         tmpisolength = tmpisoinf[0].split(",")
         for iii in range(len(tmpisolength)-1):
             tmpisolength[iii] = 0
 
     ## load all reads information which were mapped to the specific gene within this loop using pysam
     for read in bamFilePysam.fetch(geneChr, geneStart, geneEnd):
         line = str(read)
@@ -212,31 +215,35 @@
                     lociIndicators[isoformNames[i]][k] = 1
 
     #########################################################################################################################################
     ## START TO ANALYZE EACH READ 
     ##################################################################################################################################################
 
     qualifiedRead = auto_dict()
+    prereadCount = 0
     readCount = 0
+    readCount1iso = 0
     fragmentStart = auto_dict()
     fragmentEnd = auto_dict()
     CompatibleMatrix = auto_dict()
     tmpCompatibleMatrix = auto_dict()
+    qualitycheck = auto_dict()
     
     for readName in sameReadCount:
-
+        
         # load CIGAR information
         cigarNumberRead1 = auto_dict()
         cigarNumberRead2 = auto_dict()
         cigarMatchRead1 = auto_dict()
         cigarMatchRead2 = auto_dict()
         cigarInfCountRead1 = 0
         cigarInfCountRead2 = 0
         cigarInfCountRead1tmp = 0
         cigarInfCountRead2tmp = 0
+        qualitycheck[readName] = 0
         
         tmp1 = re.split("([A-Z])",readCigar[readName][1])
         for i in range(len(tmp1)-1):
             if tmp1[i].isalpha():
                 cigarMatchRead1[cigarInfCountRead1] = tmp1[i]
                 cigarInfCountRead1 += 1
             else:
@@ -359,27 +366,33 @@
                             if tmpcount2 > 1 and tmpcount22 >= 1 and tmpcount22 < tmpcount2: ## confirm the exon i is skipped by read!!
                                 for j in range(len(isoformNames)):
                                     if exonIndicators[isoformNames[j]][i] == 1: compatibleVector[j] = 0
                                                                 
                 ##################################################################################################################################################
                 ## fill in compatible matrix ##
                 if tmpcount1 > 0 or (tmpcount2 > 0 and sameReadCount[readName] == 2):
-                    readCount += 1
-                    qualifiedRead[readName] = 1
+                    prereadCount += 1
                     for i in range(len(isoformNames)):
                         CompatibleMatrix[readName][isoformNames[i]] = compatibleVector[i]
                         tmpCompatibleMatrix[readName][isoformNames[i]] = compatibleVector[i]
-                
-
+                        qualitycheck[readName] += compatibleVector[i]
+                    if qualitycheck[readName] > 0:
+                        qualifiedRead[readName] = 1
+                        #readCount += 1
+                    if qualitycheck[readName] == 1:
+                        readCount1iso += 1
+                    readCount += 1
 
     ### COMPATIBLE MATRIX OBTAINED !!!
     ###############################################################################################################
     
     if readCount == 0: continue
-    print(gene+"\t"+str(readCount)+" reads detected...")
+    fisherinf = readCount1iso/float(prereadCount)
+    if fisherinf < infthreshold: continue
+    print(gene+"\tprocessing...")
     
     ##############################################################################################################
     ### ANALYZE EMPIRICAL READS DISTRIBUTION BASED ON NON-PARAMATRIC METHOD
     ##############################################################################################################
 
     positionsFragmentCovered = auto_dict()
     readsDistributionIsoform = auto_dict()
@@ -445,22 +458,22 @@
         for j in range(len(exonStarts)):
             if exonIndicators[isoformNames[i]][j] == 1:
                 if not bool(isoformLength[isoformNames[i]]): isoformLength[isoformNames[i]] = exonEnds[j] - exonStarts[j] + 1
                 else: isoformLength[isoformNames[i]] += exonEnds[j] - exonStarts[j] + 1  ## calculate isoform length
 
     ########################################################################################################            
     ## UPDATE empirical probability of read mapped to the specific position
-
+ 
     Hfunction = auto_dict()
     numerator = auto_dict()
     numeratorKnown = auto_dict()
     for i in range(len(isoformNames)):
         if not bool(isoformLength[isoformNames[i]]): isoformLength[isoformNames[i]] = 0
         for readName in qualifiedRead:
-            if isoformLength[isoformNames[i]] > 0: Hfunction[readName][isoformNames[i]] = float(1) / isoformLength[isoformNames[i]]
+            if isoformLength[isoformNames[i]] > 0: Hfunction[readName][isoformNames[i]] = float(1)
             else: Hfunction[readName][isoformNames[i]] = 0
 
     #########################################################################################################
     ## iteration begins        
             
     diff = 1.0
     iterCount = 0
@@ -517,26 +530,29 @@
     for i in range(len(Alpha)):
         Alpha[i] = Alpha[i] / sumAlpha
 
     isoformRelativeAbundances = [None] * len(isoformNames)
     sumTheta = 0.0
     for i in range(len(Alpha)):
         #sumTheta += Alpha[i] / isoformLength[isoformNames[i]] + weightF * tmpisolength[i]
-        sumTheta += Alpha[i] + weightF * tmpisolength[i]
+        sumTheta += Alpha[i] #+ weightF * tmpisolength[i]
 
     print(gene+"\t"+str(iterCount)+" iterations\tDone!")
-
-    rpg_lengthcorrected = readCount/genelength*100
+    
+    #rpg_lengthcorrected = readCount/genelength*100
     for i in range(len(Alpha)):
         #isoformRelativeAbundances[i] = (Alpha[i]/isoformLength[isoformNames[i]]+tmpisolength[i]*weightF) /(sumTheta)
-        isoformRelativeAbundances[i] = (Alpha[i] + tmpisolength[i]*weightF) /(sumTheta)
+        #isoformRelativeAbundances[i] = (Alpha[i] + tmpisolength[i]*weightF) /(sumTheta)
+        isoformRelativeAbundances[i] = (Alpha[i]) /(sumTheta)
         #print(gene+"\t"+str(geneCount)+"\t"+str(iterCount)+"\t"+isoformNames[i]+"\t"+str(isoformRelativeAbundances[i])+"\t"+str(tmpTime))
+        
+        rpg_lengthcorrected = readCount/genelength*100*isoformRelativeAbundances[i]
 
         #OUT.write(gene+"\t"+isoformNames[i]+"\t"+str(readCount)+"\t"+str(isoformRelativeAbundances[i])+"\t"+str(rpg_lengthcorrected)+"\n") ## write results into specified file
-        OUT.write(gene+"\t"+isoformNames[i]+"\t"+str(isoformRelativeAbundances[i])+"\t"+str(rpg_lengthcorrected)+"\n")
+        OUT.write(gene+"\t"+isoformNames[i]+"\t"+str(rpg_lengthcorrected)+"\t"+str(isoformRelativeAbundances[i])+"\t"+str(fisherinf)+"\n")
 
 OUT.close()
```

### Comparing `liqa-1.1.8/setup.py` & `liqa-1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="liqa",
-    version="1.1.8",
+    version="1.2",
     author="Yu Hu",
     author_email="huyu999999@gmail.com",
     description="A statistical tool to quantify isoform-specific expression using long-read RNA-seq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WGLab/LIQA",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["pysam", "lifelines"],
     #python_requires='>=3.6',
-    packages=["liqa_src","liqa_bin"],
-    package_dir={"liqa_src":"liqa_src","liqa_bin":"liqa_src/liqa_bin"},
+    #packages=["liqa_src","liqa_bin"],
+    #package_dir={"liqa_src":"liqa_src","liqa_bin":"liqa_src/liqa_bin"},
+    packages=["liqa_src"],
+    package_dir={"liqa_src":"liqa_src"},
+    scripts=["liqa_src/group_process.pl","liqa_src/testDAS.R", "liqa_src/PreProcess.pl", "liqa_src/PreProcess_gtf.pl"],
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "liqa=liqa_src.liqa:main",
         ]
     },
 )
```

