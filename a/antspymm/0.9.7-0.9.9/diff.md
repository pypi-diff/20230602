# Comparing `tmp/antspymm-0.9.7.tar.gz` & `tmp/antspymm-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspymm-0.9.7.tar", last modified: Tue May  9 17:59:31 2023, max compression
+gzip compressed data, was "antspymm-0.9.9.tar", last modified: Fri Jun  2 00:52:02 2023, max compression
```

## Comparing `antspymm-0.9.7.tar` & `antspymm-0.9.9.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 17:59:31.621544 antspymm-0.9.7/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.7/LICENSE
--rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.7/MANIFEST.in
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-09 17:59:31.621389 antspymm-0.9.7/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.7/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 17:59:31.611384 antspymm-0.9.7/antspymm/
--rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.7/antspymm/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)   285326 2023-05-09 17:48:01.000000 antspymm-0.9.7/antspymm/mm.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 17:59:31.612267 antspymm-0.9.7/antspymm.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-09 17:59:31.000000 antspymm-0.9.7/antspymm.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      789 2023-05-09 17:59:31.000000 antspymm-0.9.7/antspymm.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-09 17:59:31.000000 antspymm-0.9.7/antspymm.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-09 17:59:31.000000 antspymm-0.9.7/antspymm.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)      112 2023-05-09 17:59:31.000000 antspymm-0.9.7/antspymm.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)        9 2023-05-09 17:59:31.000000 antspymm-0.9.7/antspymm.egg-info/top_level.txt
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 17:59:31.617100 antspymm-0.9.7/docs/
--rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.7/docs/antspymm_data_dictionary.csv
--rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.7/docs/bids_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.7/docs/example_run_from_directory.py
--rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.7/docs/make_dict_table.Rmd
--rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.7/docs/nrg_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.7/docs/outlierness.py
--rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.7/docs/ukbb_to_nrg_processing.py
--rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.7/docs/ukbb_to_nrg_processing2.py
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-05-09 17:59:31.621599 antspymm-0.9.7/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      681 2023-05-09 17:58:14.000000 antspymm-0.9.7/setup.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 17:59:31.620984 antspymm-0.9.7/tests/
--rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.7/tests/mm.py
--rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.7/tests/mm_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.7/tests/test_bids_2_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.7/tests/test_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1500 2023-05-01 14:47:40.000000 antspymm-0.9.7/tests/test_dti_reg.py
--rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.7/tests/test_dwi_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.7/tests/test_flair_run.py
--rw-r--r--   0 stnava     (501) staff       (20)     3368 2023-05-02 12:19:49.000000 antspymm-0.9.7/tests/test_joint_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.7/tests/test_mm_csv.py
--rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.7/tests/test_rsfmri_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      762 2023-05-05 18:29:30.000000 antspymm-0.9.7/tests/test_ukbb_rsfmri.py
--rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.7/tests/testsr.py
--rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.7/tests/visualize_tractogram.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-02 00:52:02.054420 antspymm-0.9.9/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.9/LICENSE
+-rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.9/MANIFEST.in
+-rw-r--r--   0 stnava     (501) staff       (20)    10425 2023-06-02 00:52:02.054019 antspymm-0.9.9/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)    10068 2023-05-16 19:58:13.000000 antspymm-0.9.9/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-02 00:52:02.035562 antspymm-0.9.9/antspymm/
+-rw-r--r--   0 stnava     (501) staff       (20)     2792 2023-05-17 13:39:41.000000 antspymm-0.9.9/antspymm/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)   295165 2023-06-02 00:48:21.000000 antspymm-0.9.9/antspymm/mm.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-02 00:52:02.037620 antspymm-0.9.9/antspymm.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)    10425 2023-06-02 00:52:01.000000 antspymm-0.9.9/antspymm.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      854 2023-06-02 00:52:01.000000 antspymm-0.9.9/antspymm.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-06-02 00:52:01.000000 antspymm-0.9.9/antspymm.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-06-02 00:52:01.000000 antspymm-0.9.9/antspymm.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)      112 2023-06-02 00:52:01.000000 antspymm-0.9.9/antspymm.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        9 2023-06-02 00:52:01.000000 antspymm-0.9.9/antspymm.egg-info/top_level.txt
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-02 00:52:02.045762 antspymm-0.9.9/docs/
+-rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.9/docs/antspymm_data_dictionary.csv
+-rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.9/docs/bids_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.9/docs/example_run_from_directory.py
+-rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.9/docs/make_dict_table.Rmd
+-rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.9/docs/nrg_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.9/docs/outlierness.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.9/docs/ukbb_to_nrg_processing.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.9/docs/ukbb_to_nrg_processing2.py
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2023-06-02 00:52:02.054500 antspymm-0.9.9/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)      681 2023-05-16 19:39:19.000000 antspymm-0.9.9/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-06-02 00:52:02.053265 antspymm-0.9.9/tests/
+-rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.9/tests/mm.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.9/tests/mm_nrg.py
+-rw-rw-r--   0 stnava     (501) staff       (20)     1050 2023-05-16 18:55:19.000000 antspymm-0.9.9/tests/outlierness.py
+-rw-rw-r--   0 stnava     (501) staff       (20)      830 2023-05-19 09:24:27.000000 antspymm-0.9.9/tests/parallel_study_aggregation_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.9/tests/test_bids_2_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.9/tests/test_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1500 2023-05-01 14:47:40.000000 antspymm-0.9.9/tests/test_dti_reg.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.9/tests/test_dwi_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.9/tests/test_flair_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3368 2023-05-02 12:19:49.000000 antspymm-0.9.9/tests/test_joint_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.9/tests/test_mm_csv.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.9/tests/test_rsfmri_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      762 2023-05-05 18:29:30.000000 antspymm-0.9.9/tests/test_ukbb_rsfmri.py
+-rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.9/tests/testsr.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.9/tests/visualize_tractogram.py
```

### Comparing `antspymm-0.9.7/LICENSE` & `antspymm-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/PKG-INFO` & `antspymm-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.7
+Version: 0.9.9
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
@@ -76,14 +76,25 @@
 * T1w: voxel-based cortical thickness (DiReCT) 10.1016/j.neuroimage.2008.12.016
 
 Results of these processes are plentiful; processing for a single subject
 will all modalities will take around 2 hours on an average laptop.
 
 documentation of functions [here](http://htmlpreview.github.io/?https://github.com/stnava/ANTsPyMM/blob/main/docs/antspymm/mm.html).
 
+
+achieved through four steps (recommended approach):
+
+1. organize data in NRG format
+
+2. perform blind QC
+
+3. compute outlierness per modality and select optimally matched modalities ( steps 3.1 and 3.2 )
+
+4. run the main antspymm function
+
 # first time setup
 
 ```python
 import antspyt1w
 import antspymm
 antspyt1w.get_data(force_download=True)
 antspymm.get_data(force_download=True)
```

### Comparing `antspymm-0.9.7/README.md` & `antspymm-0.9.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,25 @@
 * T1w: voxel-based cortical thickness (DiReCT) 10.1016/j.neuroimage.2008.12.016
 
 Results of these processes are plentiful; processing for a single subject
 will all modalities will take around 2 hours on an average laptop.
 
 documentation of functions [here](http://htmlpreview.github.io/?https://github.com/stnava/ANTsPyMM/blob/main/docs/antspymm/mm.html).
 
+
+achieved through four steps (recommended approach):
+
+1. organize data in NRG format
+
+2. perform blind QC
+
+3. compute outlierness per modality and select optimally matched modalities ( steps 3.1 and 3.2 )
+
+4. run the main antspymm function
+
 # first time setup
 
 ```python
 import antspyt1w
 import antspymm
 antspyt1w.get_data(force_download=True)
 antspymm.get_data(force_download=True)
```

### Comparing `antspymm-0.9.7/antspymm/__init__.py` & `antspymm-0.9.9/antspymm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,7 +80,9 @@
 from .mm import novelty_detection_svm
 from .mm import novelty_detection_lof
 from .mm import novelty_detection_loop
 from .mm import novelty_detection_quantile
 from .mm import generate_mm_dataframe
 from .mm import collect_blind_qc_by_modality
 from .mm import get_valid_modalities
+from .mm import study_dataframe_from_matched_dataframe
+from .mm import merge_wides_to_study_dataframe
```

### Comparing `antspymm-0.9.7/antspymm/mm.py` & `antspymm-0.9.9/antspymm/mm.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,16 @@
     'parse_nrg_filename',
     'novelty_detection_svm',
     'novelty_detection_ee',
     'novelty_detection_lof',
     'novelty_detection_loop',
     'novelty_detection_quantile',
     'generate_mm_dataframe',
+    'study_dataframe_from_matched_dataframe',
+    'merge_wides_to_study_dataframe',
     'wmh']
 
 from pathlib import Path
 from pathlib import PurePath
 import os
 import pandas as pd
 import math
@@ -490,14 +492,106 @@
     the path where one would write the image on disk
 
     """
     thedirectory = os.path.join( str(projectID), str(subjectID), str(date), str(modality), str(imageID) )
     thefilename = str(projectID) + separator + str(subjectID) + separator + str(date) + separator + str(modality) + separator + str(imageID)
     return os.path.join( thedirectory, thefilename )
 
+
+def study_dataframe_from_matched_dataframe( matched_dataframe, rootdir, outputdir, verbose=False ):
+    """
+    converts the output of antspymm.match_modalities dataframe (one row) to that needed for a study-driving dataframe for input to mm_csv
+
+    matched_dataframe : output of antspymm.match_modalities
+
+    rootdir : location for the input data root folder (in e.g. NRG format)
+
+    outputdir : location for the output data
+
+    verbose : boolean
+    """
+    iext='.nii.gz'
+    from os.path import exists
+    musthavecols = ['projectID', 'subjectID','date','imageID','fn']
+    for k in range(len(musthavecols)):
+        if not musthavecols[k] in matched_dataframe.keys():
+            raise ValueError('matched_dataframe is missing column ' +musthavecols[k] + ' in study_dataframe_from_qc_dataframe' )
+    csvrow=matched_dataframe.dropna(axis=1)
+    pid=str(csvrow['projectID'].iloc[0] )
+    sid=str(csvrow['subjectID'].iloc[0] )
+    dt=str(csvrow['date'].iloc[0])
+    iid=str(csvrow['imageID'].iloc[0])
+    nrgt1fn=os.path.join( rootdir, pid, sid, dt, 'T1w', iid, str(csvrow['fn'].iloc[0]+iext) )
+    if not exists( nrgt1fn ):
+        raise ValueError("T1 " + nrgt1fn + " does not exist in study_dataframe_from_qc_dataframe")
+    flList=[]
+    dtList=[]
+    rsfList=[]
+    nmList=[]
+    if 'flairfn' in csvrow.keys():
+        flid=str(int(csvrow['flairid'].iloc[0]))
+        nrgt2fn=os.path.join( rootdir, pid, sid, dt, 'T2Flair', flid, str(csvrow['flairfn'].iloc[0]+iext) )
+        if exists( nrgt2fn ):
+            flList.append( nrgt2fn )
+    if 'dtfn1' in csvrow.keys():
+        dtid=str(int(csvrow['dtid1'].iloc[0]))
+        dtfn1=glob.glob(os.path.join( rootdir, pid, sid, dt, 'DTI*', dtid, str(csvrow['dtfn1'].iloc[0]+iext) ))[0]
+        if exists( dtfn1 ):
+            dtList.append( dtfn1 )
+    if 'dtfn2' in csvrow.keys():
+        dtid=str(int(csvrow['dtid2'].iloc[0]))
+        dtfn2=glob.glob(os.path.join(rootdir, pid, sid, dt, 'DTI*', dtid, str(csvrow['dtfn2'].iloc[0]+iext) ))[0]
+        if exists( dtfn2 ):
+            dtList.append( dtfn2 )
+    if 'rsffn1' in csvrow.keys():
+        rsid=str(int(csvrow['rsfid1'].iloc[0]))
+        rsfn1=glob.glob(os.path.join( rootdir, pid, sid, dt, 'rsfMRI*', rsid, str(csvrow['rsffn1'].iloc[0]+iext) ))[0]
+        if exists( rsfn1 ):
+            rsfList.append( rsfn1 )
+    if 'rsffn2' in csvrow.keys():
+        rsid=str(int(csvrow['rsfid2'].iloc[0]))
+        rsfn2=glob.glob(os.path.join( rootdir, pid, sid, dt, 'rsfMRI*', rsid, str(csvrow['rsffn2'].iloc[0]+iext) ))[0]
+        if exists( rsfn2 ):
+            rsfList.append( rsfn2 )
+    for j in range(11):
+        keyname="nmfn"+str(j)
+        keynameid="nmid"+str(j)
+        if keyname in csvrow.keys() and keynameid in csvrow.keys():
+            nmid=str(int(csvrow[keynameid].iloc[0]))
+            nmsearchpath=os.path.join( rootdir, pid, sid, dt, 'NM2DMT', nmid, "*"+nmid+iext)
+            nmfn=glob.glob( nmsearchpath )
+            nmfn=nmfn[0]
+            if exists( nmfn ):
+                nmList.append( nmfn )
+    if verbose:
+        print("assembled the image lists mapping to ....")
+        print(nrgt1fn)
+        print("NM")
+        print(nmList)
+        print("FLAIR")
+        print(flList)
+        print("DTI")
+        print(dtList)
+        print("rsfMRI")
+        print(rsfList)
+    studycsv = generate_mm_dataframe(
+        pid,
+        sid,
+        dt,
+        iid, # the T1 id
+        'T1w',
+        rootdir,
+        outputdir,
+        t1_filename=nrgt1fn,
+        flair_filename=flList,
+        dti_filenames=dtList,
+        rsf_filenames=rsfList,
+        nm_filenames=nmList)
+    return studycsv.dropna(axis=1)
+
 def highest_quality_repeat(mxdfin, idvar, visitvar, qualityvar):
     """
     This function returns a subset of the input dataframe that retains only the rows
     that correspond to the highest quality observation for each combination of ID and visit.
 
     Parameters:
     ----------
@@ -2312,15 +2406,18 @@
         RGB = ants.from_numpy( RGB.astype(np.float32) )
         RGB0 = ants.copy_image_info( b0, ants.slice_image( RGB, axis=3, idx=0 ) )
         RGB1 = ants.copy_image_info( b0, ants.slice_image( RGB, axis=3, idx=1 ) )
         RGB2 = ants.copy_image_info( b0, ants.slice_image( RGB, axis=3, idx=2 ) )
         RGB = ants.merge_channels( [RGB0,RGB1,RGB2] )
         return tenfit, FA, MD1, RGB
 
-    gtab = gradient_table(bvals, bvecs)
+    import numpy as np
+    if abs(np.linalg.norm(bvecs)-1) > 0.009 and False:
+        bvecs=bvecs/np.linalg.norm(bvecs, axis=1)  
+    gtab = gradient_table(bvals, bvecs, atol=0.1 )
     tenfit, FA, MD1, RGB = justthefit( gtab, fit_method, image, maskdil )
     if verbose:
         print("recon dti.TensorModel done",flush=True)
 
     # change the brain mask based on high FA values
     if trim_the_mask > 0 and fit_method is not None:
         mask = trim_dti_mask( FA, mask, trim_the_mask )
@@ -2479,19 +2576,19 @@
             imgout = ants.from_numpy( img[:,:,:,0:bvecs.shape[0]] )
             imgout = ants.copy_image_info( img, imgout )
             return( imgout )
         else:
             return( img )
 
     img_LR = fix_dwi_shape( img_LR, bval_LR, bvec_LR )
-    if denoise and srmodel is None:
+    if denoise :
         img_LR = mc_denoise( img_LR )
     if img_RL is not None:
         img_RL = fix_dwi_shape( img_RL, bval_RL, bvec_RL )
-        if denoise and srmodel is None:
+        if denoise :
             img_RL = mc_denoise( img_RL )
 
     if brain_mask is not None:
         maskInRightSpace = ants.image_physical_space_consistency( brain_mask, reference_B0 )
         if not maskInRightSpace :
             raise ValueError('not maskInRightSpace ... provided brain mask should be in reference_B0 space')
 
@@ -2846,15 +2943,18 @@
     from dipy.tracking.utils import path_length
     if verbose:
         print("begin tracking",flush=True)
     dwi_img = dwi.to_nibabel()
     affine = dwi_img.affine
     if isinstance( bvals, str ) or isinstance( bvecs, str ):
         bvals, bvecs = read_bvals_bvecs(bvals, bvecs)
-    gtab = gradient_table(bvals, bvecs)
+    import numpy as np
+    if abs(np.linalg.norm(bvecs)-1) > 0.009 and False:
+        bvecs=bvecs/np.linalg.norm(bvecs, axis=1 )  
+    gtab = gradient_table(bvals, bvecs, atol=0.1 )
     if mask is None:
         mask = ants.threshold_image( fa, fa_thresh, 2.0 ).iMath("GetLargestComponent")
     dwi_data = dwi_img.get_fdata()
     dwi_mask = mask.numpy() == 1
     dti_model = dti.TensorModel(gtab,fit_method=fit_method)
     if verbose:
         print("begin tracking fit",flush=True)
@@ -3014,15 +3114,18 @@
 
     if verbose:
         print("begin tracking",flush=True)
     dwi_img = dwi.to_nibabel()
     affine = dwi_img.affine
     if isinstance( bvals, str ) or isinstance( bvecs, str ):
         bvals, bvecs = read_bvals_bvecs(bvals, bvecs)
-    gtab = gradient_table(bvals, bvecs)
+    import numpy as np
+    if abs(np.linalg.norm(bvecs)-1) > 0.009 and False:
+        bvecs=bvecs/np.linalg.norm(bvecs, axis=1)  
+    gtab = gradient_table(bvals, bvecs, atol=0.1 )
     if mask is None:
         mask = ants.threshold_image( fa, fa_thresh, 2.0 ).iMath("GetLargestComponent")
     dwi_data = dwi_img.get_fdata()
     dwi_mask = mask.numpy() == 1
 
 
     response, ratio = auto_response_ssst(gtab, dwi_data, roi_radii=10, fa_thr=0.7)
@@ -3999,23 +4102,26 @@
   ct = 0
   numofnets = [3,5,6,7,8,9,10,11,13]
   for mynet in numofnets:
     netname = re.sub( " ", "", networks[mynet] )
     netname = re.sub( "-", "", netname )
     ww = np.where( powers_areal_mni_itk['SystemName'] == networks[mynet] )[0]
     dfnImg = ants.make_points_image(pts2bold.iloc[ww,:3].values, bmask, radius=1).threshold_image( 1, 1e9 )
-    dfnmat = ants.timeseries_to_matrix( simg, ants.threshold_image( dfnImg, 1, dfnImg.max() ) )
-    dfnmat = ants.bandpass_filter_matrix( dfnmat, tr = tr, lowf=f[0], highf=f[1]  )
-    dfnmat = ants.regress_components( dfnmat, nuisance )
-    dfnsignal = dfnmat.mean( axis = 1 )
-    gmmatDFNCorr = np.zeros( gmmat.shape[1] )
-    for k in range( gmmat.shape[1] ):
-      gmmatDFNCorr[ k ] = pearsonr( dfnsignal, gmmat[:,k] )[0]
-    corrImg = ants.make_image( gmseg, gmmatDFNCorr  )
-    outdict[ netname ] = corrImg
+    if dfnImg.max() >= 1:
+        dfnmat = ants.timeseries_to_matrix( simg, ants.threshold_image( dfnImg, 1, dfnImg.max() ) )
+        dfnmat = ants.bandpass_filter_matrix( dfnmat, tr = tr, lowf=f[0], highf=f[1]  )
+        dfnmat = ants.regress_components( dfnmat, nuisance )
+        dfnsignal = dfnmat.mean( axis = 1 )
+        gmmatDFNCorr = np.zeros( gmmat.shape[1] )
+        for k in range( gmmat.shape[1] ):
+            gmmatDFNCorr[ k ] = pearsonr( dfnsignal, gmmat[:,k] )[0]
+        corrImg = ants.make_image( gmseg, gmmatDFNCorr  )
+        outdict[ netname ] = corrImg
+    else:
+        outdict[ netname ] = None
     ct = ct + 1
 
   A = np.zeros( ( len( numofnets ) , len( numofnets ) ) )
   A_wide = np.zeros( ( 1, len( numofnets ) * len( numofnets ) ) )
   newnames=[]
   newnames_wide=[]
   ct = 0
@@ -5154,16 +5260,16 @@
 
 def mm_csv(
     studycsv,   # pandas data frame
     mysep = '-', # or "_" for BIDS
     srmodel_T1 = False, # optional - will add a great deal of time
     srmodel_NM = False, # optional - will add a great deal of time
     srmodel_DTI = False, # optional - will add a great deal of time
-    dti_motion_correct = 'Rigid',
-    dti_denoise = False,
+    dti_motion_correct = 'SyN',
+    dti_denoise = True,
     nrg_modality_list = None
 ):
     """
     too dangerous to document ... use with care.
 
     processes multiple modality MRI specifically:
 
@@ -5334,15 +5440,15 @@
         print( "REGISTRATION EXISTENCE: " +
             str(exists( templateTx['fwdtransforms'][0])) + " " +
             str(exists( templateTx['fwdtransforms'][1])) + " " +
             str(exists( templateTx['invtransforms'][0])) + " " +
             str(exists( templateTx['invtransforms'][1])) )
     if verbose:
         print( hierfntest )
-    hierexists = exists( hierfntest ) # FIXME should test this explicitly but we assume it here
+    hierexists = exists( hierfntest ) and exists( templateTx['fwdtransforms'][0]) and exists( templateTx['fwdtransforms'][1]) and exists( templateTx['invtransforms'][0]) and exists( templateTx['invtransforms'][1])
     hier = None
     if not hierexists and not testloop:
         subjectpropath = os.path.dirname( hierfn )
         if verbose:
             print( subjectpropath )
         os.makedirs( subjectpropath, exist_ok=True  )
         hier = antspyt1w.hierarchical( t1, hierfn, labels_to_register=None )
@@ -5567,66 +5673,70 @@
                                     ants.plot( tabPro['rsf']['meanBold'], ants.iMath(tabPro['rsf']['falff'],"Normalize"),
                                         axis=2, nslices=maxslice, ncol=7, crop=True, title='fALFF', filename=mymm+mysep+"boldfALFF.png" )
                                     ants.plot( tabPro['rsf']['meanBold'], tabPro['rsf']['DefaultMode'],
                                         axis=2, nslices=maxslice, ncol=7, crop=True, title='DefaultMode', filename=mymm+mysep+"boldDefaultMode.png" )
                                     ants.plot( tabPro['rsf']['meanBold'], tabPro['rsf']['FrontoparietalTaskControl'],
                                         axis=2, nslices=maxslice, ncol=7, crop=True, title='FrontoparietalTaskControl', filename=mymm+mysep+"boldFrontoparietalTaskControl.png"  )
                             if ( mymod == 'DTI_LR' or mymod == 'DTI_RL' or mymod == 'DTI' ) and ishapelen == 4:
-                                dowrite=True
                                 bvalfn = re.sub( '.nii.gz', '.bval' , myimg )
                                 bvecfn = re.sub( '.nii.gz', '.bvec' , myimg )
                                 imgList = [ img ]
                                 bvalfnList = [ bvalfn ]
                                 bvecfnList = [ bvecfn ]
+                                missing_dti_data=False # bval, bvec or images
                                 if len( myimgsr ) > 1:  # find DTI_RL
                                     dtilrfn = myimgsr[myimgcount+1]
                                     if exists( dtilrfn ):
                                         bvalfnRL = re.sub( '.nii.gz', '.bval' , dtilrfn )
                                         bvecfnRL = re.sub( '.nii.gz', '.bvec' , dtilrfn )
                                         imgRL = ants.image_read( dtilrfn )
                                         imgList.append( imgRL )
                                         bvalfnList.append( bvalfnRL )
                                         bvecfnList.append( bvecfnRL )
                                 # check existence of all files expected ...
                                 for dtiex in bvalfnList+bvecfnList+myimgsr:
                                     if not exists(dtiex):
-                                        raise ValueError('mm_csv dti data ' + dtiex )
-                                srmodel_DTI_mdl=None
-                                if srmodel_DTI is not False:
-                                    temp = ants.get_spacing(img)
-                                    dtspc=[temp[0],temp[1],temp[2]]
-                                    bestup = siq.optimize_upsampling_shape( dtspc, modality='DTI' )
-                                    mdlfn = ex_pathmm + "siq_default_sisr_" + bestup + "_1chan_featvggL6_best_mdl.h5"
-                                    if isinstance( srmodel_DTI, str ):
-                                        srmodel_DTI = re.sub( "bestup", bestup, srmodel_DTI )
-                                        mdlfn = os.path.join( ex_pathmm, srmodel_DTI )
-                                    if exists( mdlfn ):
-                                        if verbose:
-                                            print(mdlfn)
-                                        srmodel_DTI_mdl = tf.keras.models.load_model( mdlfn, compile=False )
-                                    else:
-                                        print(mdlfn + " does not exist - wont use SR")
-                                tabPro, normPro = mm( t1, hier,
-                                    dw_image=imgList,
-                                    bvals = bvalfnList,
-                                    bvecs = bvecfnList,
-                                    srmodel=srmodel_DTI_mdl,
-                                    do_tractography=not test_run,
-                                    do_kk=False,
-                                    do_normalization=templateTx,
-                                    dti_motion_correct = dti_motion_correct,
-                                    dti_denoise = dti_denoise,
-                                    test_run=test_run,
-                                    verbose=True )
-                                mydti = tabPro['DTI']
-                                if visualize:
-                                    maxslice = np.min( [21, mydti['recon_fa'] ] )
-                                    ants.plot( mydti['recon_fa'],  axis=2, nslices=maxslice, ncol=7, crop=True, title='FA (supposed to be better)', filename=mymm+mysep+"FAbetter.png"  )
-                                    ants.plot( mydti['recon_fa'], mydti['jhu_labels'], axis=2, nslices=maxslice, ncol=7, crop=True, title='FA + JHU', filename=mymm+mysep+"FAJHU.png"  )
-                                    ants.plot( mydti['recon_md'],  axis=2, nslices=maxslice, ncol=7, crop=True, title='MD', filename=mymm+mysep+"MD.png"  )
+                                        print('mm_csv: missing dti data ' + dtiex )
+                                        missing_dti_data=True
+                                        dowrite=False
+                                if not missing_dti_data:
+                                    dowrite=True
+                                    srmodel_DTI_mdl=None
+                                    if srmodel_DTI is not False:
+                                        temp = ants.get_spacing(img)
+                                        dtspc=[temp[0],temp[1],temp[2]]
+                                        bestup = siq.optimize_upsampling_shape( dtspc, modality='DTI' )
+                                        mdlfn = ex_pathmm + "siq_default_sisr_" + bestup + "_1chan_featvggL6_best_mdl.h5"
+                                        if isinstance( srmodel_DTI, str ):
+                                            srmodel_DTI = re.sub( "bestup", bestup, srmodel_DTI )
+                                            mdlfn = os.path.join( ex_pathmm, srmodel_DTI )
+                                        if exists( mdlfn ):
+                                            if verbose:
+                                                print(mdlfn)
+                                            srmodel_DTI_mdl = tf.keras.models.load_model( mdlfn, compile=False )
+                                        else:
+                                            print(mdlfn + " does not exist - wont use SR")
+                                    tabPro, normPro = mm( t1, hier,
+                                        dw_image=imgList,
+                                        bvals = bvalfnList,
+                                        bvecs = bvecfnList,
+                                        srmodel=srmodel_DTI_mdl,
+                                        do_tractography=not test_run,
+                                        do_kk=False,
+                                        do_normalization=templateTx,
+                                        dti_motion_correct = dti_motion_correct,
+                                        dti_denoise = dti_denoise,
+                                        test_run=test_run,
+                                        verbose=True )
+                                    mydti = tabPro['DTI']
+                                    if visualize:
+                                        maxslice = np.min( [21, mydti['recon_fa'] ] )
+                                        ants.plot( mydti['recon_fa'],  axis=2, nslices=maxslice, ncol=7, crop=True, title='FA (supposed to be better)', filename=mymm+mysep+"FAbetter.png"  )
+                                        ants.plot( mydti['recon_fa'], mydti['jhu_labels'], axis=2, nslices=maxslice, ncol=7, crop=True, title='FA + JHU', filename=mymm+mysep+"FAJHU.png"  )
+                                        ants.plot( mydti['recon_md'],  axis=2, nslices=maxslice, ncol=7, crop=True, title='MD', filename=mymm+mysep+"MD.png"  )
                             if dowrite:
                                 write_mm( output_prefix=mymm, mm=tabPro, mm_norm=normPro, t1wide=t1wide, separator=mysep )
                                 for mykey in normPro.keys():
                                     if normPro[mykey] is not None:
                                         if visualize:
                                             ants.plot( template, normPro[mykey], axis=2, nslices=21, ncol=7, crop=True, title=mykey, filename=mymm+mysep+mykey+".png"   )
         if overmodX == nrg_modality_list[ len( nrg_modality_list ) - 1 ]:
@@ -6026,14 +6136,118 @@
             xdf = pd.DataFrame(ddnum, columns=xdfcols )
     if xdf.shape[1] == 0:
         return None
     if colprefix is not None:
         xdf.columns=colprefix + xdf.columns
     return pd.concat( [df,xdf], axis=1 )
 
+def merge_wides_to_study_dataframe( sdf, processing_dir, separator='-', sid_is_int=True, id_is_int=True, date_is_int=True, report_missing=False,
+progress=False, verbose=False ):
+    """
+    extend a study data frame with wide outputs
+
+    sdf : the input study dataframe
+
+    processing_dir:  the directory location of the processed data 
+
+    separator : string usually '-' or '_'
+
+    sid_is_int : boolean set to True to cast unique subject ids to int; can be useful if they are inadvertently stored as float by pandas
+
+    date_is_int : boolean set to True to cast date to int; can be useful if they are inadvertently stored as float by pandas
+
+    id_is_int : boolean set to True to cast unique image ids to int; can be useful if they are inadvertently stored as float by pandas
+
+    report_missing : boolean combined with verbose will report missing modalities
+
+    progress : integer reports percent progress modulo progress value 
+
+    verbose : boolean
+    """
+    from os.path import exists
+    musthavecols = ['projectID', 'subjectID','date','imageID','fn']
+    for k in range(len(musthavecols)):
+        if not musthavecols[k] in sdf.keys():
+            raise ValueError('sdf is missing column ' +musthavecols[k] + ' in merge_wides_to_study_dataframe' )
+    possible_iids = [ 'imageID', 'imageID', 'imageID', 'flairid', 'dtid1', 'dtid2', 'rsfid1', 'rsfid2', 'nmid1', 'nmid2', 'nmid3', 'nmid4', 'nmid5', 'nmid6', 'nmid7', 'nmid8', 'nmid9', 'nmid10' ]
+    modality_ids = [ 'T1wHierarchical', 'T1wHierarchicalSR', 'T1w', 'T2Flair', 'DTI', 'DTI', 'rsfMRI', 'rsfMRI', 'NM2DMT', 'NM2DMT', 'NM2DMT', 'NM2DMT', 'NM2DMT', 'NM2DMT', 'NM2DMT', 'NM2DMT', 'NM2DMT', 'NM2DMT']
+    alldf=pd.DataFrame()
+    for myk in sdf.index:
+        if progress > 0 and int(myk) % int(progress) == 0:
+            print( str( round( myk/sdf.shape[0]*100.0)) + "%...", end='', flush=True)
+        if verbose:
+            print( "DOROW " + str(myk) + ' of ' + str( sdf.shape[0] ) )
+        csvrow = sdf.loc[sdf.index == myk].dropna(axis=1)
+        ct=-1
+        for iidkey in possible_iids:
+            ct=ct+1
+            mod_name = modality_ids[ct]
+            if iidkey in csvrow.keys():
+                if id_is_int:
+                    iid = str( int( csvrow[iidkey].iloc[0] ) )
+                else:
+                    iid = str( csvrow[iidkey].iloc[0] )
+                if verbose:
+                    print( "iidkey " + iidkey + " modality " + mod_name + ' iid '+ iid )
+                pid=str(csvrow['projectID'].iloc[0] )
+                if sid_is_int:
+                    sid=str(int(csvrow['subjectID'].iloc[0] ))
+                else:
+                    sid=str(csvrow['subjectID'].iloc[0] )
+                if date_is_int:
+                    dt=str(int(csvrow['date'].iloc[0]))
+                else:
+                    dt=str(csvrow['date'].iloc[0])
+                if id_is_int:
+                    t1iid=str(int(csvrow['imageID'].iloc[0]))
+                else:
+                    t1iid=str(csvrow['imageID'].iloc[0])
+                if t1iid != iid:
+                    iidj=iid+"_"+t1iid
+                else:
+                    iidj=iid
+                rootid = pid +separator+ sid +separator+dt+separator+mod_name+separator+iidj
+                myext = rootid +separator+'mmwide.csv'
+                nrgwidefn=os.path.join( processing_dir, pid, sid, dt, mod_name, iid, myext )
+                moddersub = mod_name
+                is_t1=False
+                if mod_name == 'T1wHierarchical':
+                    is_t1=True
+                    moddersub='T1Hier'
+                elif mod_name == 'T1wHierarchicalSR':
+                    is_t1=True
+                    moddersub='T1HSR'
+                if exists( nrgwidefn ):
+                    if verbose:
+                        print( nrgwidefn + " exists")
+                    mm=read_mm_csv( nrgwidefn, colprefix=moddersub+'_', is_t1=is_t1, separator=separator, verbose=verbose )
+                    if mm is not None:
+                        if mod_name == 'T1wHierarchical':
+                            a=list( csvrow.keys() )
+                            b=list( mm.keys() )
+                            abintersect=list(set(b).intersection( set(a) ) )
+                            if len( abintersect  ) > 0 :
+                                for qq in abintersect:
+                                    mm.pop( qq )
+                        mm.index=csvrow.index
+                        uidname = mod_name + '_mmwide_filename'
+                        mm[ uidname ] = rootid
+                        csvrow=pd.concat( [csvrow,mm], axis=1 )
+                else:
+                    if verbose and report_missing:
+                        print( nrgwidefn + " absent")
+        if alldf.shape[0] == 0:
+            alldf = csvrow.copy()
+            alldf = alldf.loc[:,~alldf.columns.duplicated()]
+        else:
+            csvrow=csvrow.loc[:,~csvrow.columns.duplicated()]
+            alldf = alldf.loc[:,~alldf.columns.duplicated()]
+            alldf = pd.concat( [alldf, csvrow], axis=0, ignore_index=True)
+    return alldf
+
 def assemble_modality_specific_dataframes( mm_wide_csvs, hierdfin, nrg_modality, separator='-', progress=None, verbose=False ):
     moddersub = re.sub( "[*]","",nrg_modality)
     nmdf=pd.DataFrame()
     for k in range( hierdfin.shape[0] ):
         if progress is not None:
             if k % progress == 0:
                 progger = str( np.round( k / hierdfin.shape[0] * 100 ) )
@@ -6132,15 +6346,15 @@
     wmh_sum_aug = 0
     wmh_sum_prior_aug = 0
     augprob = flair * 0.0
     augprob_prior = None
     if prior_probability is not None:
         augprob_prior = flair * 0.0
     for n in range(n_simulations):
-        augflair, tx, itx = augment_image( flair, 5 )
+        augflair, tx, itx = augment_image( ants.iMath(flair,"Normalize"), 5, 0.01 )
         locwmh = wmh( augflair, t1, t1seg, mmfromconvexhull = mmfromconvexhull,
             strict=strict, probability_mask=None, prior_probability=prior_probability )
         if verbose:
             print( "flair sim: " + str(n) + " vol: " + str( locwmh['wmh_mass'] )+ " vol-prior: " + str( locwmh['wmh_mass_prior'] )+ " snr: " + str( locwmh['wmh_SNR'] ) )
         wmh_sum_aug = wmh_sum_aug + locwmh['wmh_mass']
         wmh_sum_prior_aug = wmh_sum_prior_aug + locwmh['wmh_mass_prior']
         temp = locwmh['WMH_probability_map']
@@ -6790,17 +7004,15 @@
     modalities = modalities[modalities != 'unknown']
     # Get modalities to select
     m0sel = qc_full['modality'].isin(modalities)
     # Get unique ids
     uid = qc_full['fn'] + "_" + qc_full['modality'].astype(str)
     to_average = uid.unique()
     # Define column indices
-    contcols = ['noise', 'snr', 'cnr', 'psnr', 'ssim', 'mi',
-       'reflection_err', 'EVR', 'msk_vol', 'spc0', 'spc1', 'spc2', 'dimx',
-       'dimy', 'dimz', 'slice']
+    contcols = ['noise', 'snr', 'cnr', 'psnr', 'ssim', 'mi','reflection_err', 'EVR', 'msk_vol', 'spc0', 'spc1', 'spc2', 'org0','org1','org2', 'dimx', 'dimy', 'dimz', 'slice']
     ocols = ['fn','modality', 'mriseries', 'mrimfg', 'mrimodel']
     # restrict to columns we "know"
     qc_full = qc_full[ocols+contcols]
     # Create empty meta dataframe
     meta = pd.DataFrame(columns=ocols+contcols)
     # Process each unique id
     n = len(to_average)
```

### Comparing `antspymm-0.9.7/antspymm.egg-info/PKG-INFO` & `antspymm-0.9.9/antspymm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.7
+Version: 0.9.9
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
@@ -76,14 +76,25 @@
 * T1w: voxel-based cortical thickness (DiReCT) 10.1016/j.neuroimage.2008.12.016
 
 Results of these processes are plentiful; processing for a single subject
 will all modalities will take around 2 hours on an average laptop.
 
 documentation of functions [here](http://htmlpreview.github.io/?https://github.com/stnava/ANTsPyMM/blob/main/docs/antspymm/mm.html).
 
+
+achieved through four steps (recommended approach):
+
+1. organize data in NRG format
+
+2. perform blind QC
+
+3. compute outlierness per modality and select optimally matched modalities ( steps 3.1 and 3.2 )
+
+4. run the main antspymm function
+
 # first time setup
 
 ```python
 import antspyt1w
 import antspymm
 antspyt1w.get_data(force_download=True)
 antspymm.get_data(force_download=True)
```

### Comparing `antspymm-0.9.7/antspymm.egg-info/SOURCES.txt` & `antspymm-0.9.9/antspymm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 docs/make_dict_table.Rmd
 docs/nrg_cohort_example.py
 docs/outlierness.py
 docs/ukbb_to_nrg_processing.py
 docs/ukbb_to_nrg_processing2.py
 tests/mm.py
 tests/mm_nrg.py
+tests/outlierness.py
+tests/parallel_study_aggregation_example.py
 tests/test_bids_2_nrg.py
 tests/test_dti_recon.py
 tests/test_dti_reg.py
 tests/test_dwi_run.py
 tests/test_flair_run.py
 tests/test_joint_dti_recon.py
 tests/test_mm_csv.py
```

### Comparing `antspymm-0.9.7/docs/antspymm_data_dictionary.csv` & `antspymm-0.9.9/docs/antspymm_data_dictionary.csv`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/docs/bids_cohort_example.py` & `antspymm-0.9.9/docs/bids_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/docs/example_run_from_directory.py` & `antspymm-0.9.9/docs/example_run_from_directory.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/docs/nrg_cohort_example.py` & `antspymm-0.9.9/docs/nrg_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/docs/outlierness.py` & `antspymm-0.9.9/docs/outlierness.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/docs/ukbb_to_nrg_processing.py` & `antspymm-0.9.9/docs/ukbb_to_nrg_processing.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/docs/ukbb_to_nrg_processing2.py` & `antspymm-0.9.9/docs/ukbb_to_nrg_processing2.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/setup.py` & `antspymm-0.9.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = open("README.md").read()
 
 with open("./requirements.txt") as f:
       requirements = f.read().splitlines()
 
 setup(name='antspymm',
-      version='0.9.7',
+      version='0.9.9',
       description='multi-channel/time-series medical image processing with antspyx',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/stnava/ANTsPyMM',
       author='Avants, Gosselin, Tustison, Reardon',
       author_email='stnava@gmail.com',
       license='Apache 2.0',
```

### Comparing `antspymm-0.9.7/tests/mm.py` & `antspymm-0.9.9/tests/mm.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/tests/mm_nrg.py` & `antspymm-0.9.9/tests/mm_nrg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/tests/test_dti_reg.py` & `antspymm-0.9.9/tests/test_dti_reg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/tests/test_dwi_run.py` & `antspymm-0.9.9/tests/test_dwi_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/tests/test_joint_dti_recon.py` & `antspymm-0.9.9/tests/test_joint_dti_recon.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/tests/test_mm_csv.py` & `antspymm-0.9.9/tests/test_mm_csv.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/tests/test_rsfmri_run.py` & `antspymm-0.9.9/tests/test_rsfmri_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/tests/test_ukbb_rsfmri.py` & `antspymm-0.9.9/tests/test_ukbb_rsfmri.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/tests/testsr.py` & `antspymm-0.9.9/tests/testsr.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.7/tests/visualize_tractogram.py` & `antspymm-0.9.9/tests/visualize_tractogram.py`

 * *Files identical despite different names*

