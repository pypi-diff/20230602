# Comparing `tmp/napatrackmater-3.5.7.tar.gz` & `tmp/napatrackmater-3.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-kyut1p9q/napatrackmater-3.5.7.tar", last modified: Mon May  8 17:47:56 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-ixpbdgwx/napatrackmater-3.5.8.tar", last modified: Fri Jun  2 15:35:04 2023, max compression
```

## Comparing `napatrackmater-3.5.7.tar` & `napatrackmater-3.5.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-08 17:47:56.980134 napatrackmater-3.5.7/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.5.7/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-08 17:47:56.973820 napatrackmater-3.5.7/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.5.7/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-08 17:47:56.726730 napatrackmater-3.5.7/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.5.7/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.5.7/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   109610 2023-05-08 17:47:12.000000 napatrackmater-3.5.7/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.5.7/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.5.7/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13523 2023-05-04 16:47:51.000000 napatrackmater-3.5.7/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.5.7/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.5.7/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.5.7/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-08 17:47:16.000000 napatrackmater-3.5.7/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-08 17:47:56.928113 napatrackmater-3.5.7/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-08 17:47:55.000000 napatrackmater-3.5.7/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-08 17:47:56.000000 napatrackmater-3.5.7/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-08 17:47:55.000000 napatrackmater-3.5.7/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-08 17:47:55.000000 napatrackmater-3.5.7/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-08 17:47:56.000000 napatrackmater-3.5.7/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-08 17:47:56.000000 napatrackmater-3.5.7/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-08 17:47:56.982142 napatrackmater-3.5.7/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.5.7/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 15:35:04.320238 napatrackmater-3.5.8/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.5.8/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-02 15:35:04.313760 napatrackmater-3.5.8/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.5.8/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 15:35:03.998386 napatrackmater-3.5.8/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.5.8/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.5.8/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110145 2023-06-02 11:26:18.000000 napatrackmater-3.5.8/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.5.8/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.5.8/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13533 2023-06-02 15:33:59.000000 napatrackmater-3.5.8/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.5.8/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.5.8/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.5.8/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-02 10:50:16.000000 napatrackmater-3.5.8/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-02 15:35:04.261403 napatrackmater-3.5.8/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-02 15:35:03.000000 napatrackmater-3.5.8/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-02 15:35:03.000000 napatrackmater-3.5.8/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-02 15:35:03.000000 napatrackmater-3.5.8/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-02 15:35:03.000000 napatrackmater-3.5.8/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-06-02 15:35:03.000000 napatrackmater-3.5.8/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-02 15:35:03.000000 napatrackmater-3.5.8/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-02 15:35:04.323603 napatrackmater-3.5.8/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-05-08 19:47:10.000000 napatrackmater-3.5.8/setup.py
```

### Comparing `napatrackmater-3.5.7/LICENSE` & `napatrackmater-3.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.7/PKG-INFO` & `napatrackmater-3.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.5.7
+Version: 3.5.8
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.5.7/README.md` & `napatrackmater-3.5.8/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.7/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.5.8/napatrackmater/CloudAutoEncoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from cellshape_cloud import CloudAutoEncoder
 import sys
+from kapoorlabs_lightning.pytorch_models import CloudAutoEncoder
 from .pretrained import get_autoencoder_instance, get_model_details, get_registered_models
 
 
 class CloudAutoEncoder(CloudAutoEncoder):
     def __init__(
         self,
         num_features,
```

### Comparing `napatrackmater-3.5.7/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.5.8/napatrackmater/DeepEmbeddedClustering.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cellshape_cluster import DeepEmbeddedClustering
+from kapoorlabs_lightning.pytorch_models import DeepEmbeddedClustering
 from .pretrained import get_cluster_instance, get_model_details, get_registered_models
 import sys
 
 class DeepEmbeddedClustering(DeepEmbeddedClustering):
     def __init__(self, autoencoder, num_clusters):
         super().__init__(autoencoder, num_clusters)
```

### Comparing `napatrackmater-3.5.7/napatrackmater/Trackmate.py` & `napatrackmater-3.5.8/napatrackmater/Trackmate.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,6812 +40,6846 @@
 00000270: 2c20 5472 6163 6b69 6442 6f78 2c20 6178  , TrackidBox, ax
 00000280: 6573 2c20 2070 726f 6772 6573 735f 6261  es,  progress_ba
 00000290: 7220 3d20 4e6f 6e65 2c20 0d0a 2020 2020  r = None, ..    
 000002a0: 2020 2020 2020 2020 2020 2020 206d 6173               mas
 000002b0: 7465 725f 786d 6c5f 7061 7468 3a20 5061  ter_xml_path: Pa
 000002c0: 7468 203d 204e 6f6e 652c 206d 6173 7465  th = None, maste
 000002d0: 725f 6578 7472 615f 6e61 6d65 203d 2027  r_extra_name = '
-000002e0: 272c 2073 6567 5f69 6d61 6765 203d 204e  ', seg_image = N
-000002f0: 6f6e 652c 2063 6861 6e6e 656c 5f73 6567  one, channel_seg
-00000300: 5f69 6d61 6765 203d 204e 6f6e 652c 2069  _image = None, i
-00000310: 6d61 6765 203d 204e 6f6e 652c 206d 6173  mage = None, mas
-00000320: 6b20 3d20 4e6f 6e65 2c20 666f 7572 6965  k = None, fourie
-00000330: 7220 3d20 5472 7565 2c20 636c 7573 7465  r = True, cluste
-00000340: 725f 6d6f 6465 6c20 3d20 4e6f 6e65 2c20  r_model = None, 
-00000350: 6e75 6d5f 706f 696e 7473 203d 2032 3034  num_points = 204
-00000360: 382c 2062 6174 6368 5f73 697a 6520 3d20  8, batch_size = 
-00000370: 3129 3a0d 0a20 2020 2020 2020 200d 0a20  1):..        .. 
-00000380: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000390: 2073 656c 662e 786d 6c5f 7061 7468 203d   self.xml_path =
-000003a0: 2078 6d6c 5f70 6174 680d 0a20 2020 2020   xml_path..     
-000003b0: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
-000003c0: 6d6c 5f70 6174 6820 3d20 6d61 7374 6572  ml_path = master
-000003d0: 5f78 6d6c 5f70 6174 680d 0a20 2020 2020  _xml_path..     
-000003e0: 2020 2073 656c 662e 7370 6f74 5f63 7376     self.spot_csv
-000003f0: 5f70 6174 6820 3d20 7370 6f74 5f63 7376  _path = spot_csv
-00000400: 5f70 6174 680d 0a20 2020 2020 2020 2073  _path..        s
-00000410: 656c 662e 7472 6163 6b5f 6373 765f 7061  elf.track_csv_pa
-00000420: 7468 203d 2074 7261 636b 5f63 7376 5f70  th = track_csv_p
-00000430: 6174 6820 0d0a 2020 2020 2020 2020 7365  ath ..        se
-00000440: 6c66 2e65 6467 6573 5f63 7376 5f70 6174  lf.edges_csv_pat
-00000450: 6820 3d20 6564 6765 735f 6373 765f 7061  h = edges_csv_pa
-00000460: 7468 0d0a 2020 2020 2020 2020 7365 6c66  th..        self
-00000470: 2e69 6d61 6765 203d 2069 6d61 6765 200d  .image = image .
-00000480: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
-00000490: 736b 203d 206d 6173 6b0d 0a20 2020 2020  sk = mask..     
-000004a0: 2020 2073 656c 662e 666f 7572 6965 7220     self.fourier 
-000004b0: 3d20 666f 7572 6965 720d 0a20 2020 2020  = fourier..     
-000004c0: 2020 2073 656c 662e 636c 7573 7465 725f     self.cluster_
-000004d0: 6d6f 6465 6c20 3d20 636c 7573 7465 725f  model = cluster_
-000004e0: 6d6f 6465 6c20 0d0a 2020 2020 2020 2020  model ..        
-000004f0: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
-00000500: 5f69 6d61 6765 203d 2063 6861 6e6e 656c  _image = channel
-00000510: 5f73 6567 5f69 6d61 6765 0d0a 2020 2020  _seg_image..    
-00000520: 2020 2020 7365 6c66 2e73 6567 5f69 6d61      self.seg_ima
-00000530: 6765 203d 2073 6567 5f69 6d61 6765 0d0a  ge = seg_image..
-00000540: 2020 2020 2020 2020 7365 6c66 2e41 7474          self.Att
-00000550: 7269 6275 7465 426f 786e 616d 6520 3d20  ributeBoxname = 
-00000560: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
-00000570: 0d0a 2020 2020 2020 2020 7365 6c66 2e54  ..        self.T
-00000580: 7261 636b 4174 7472 6962 7574 6542 6f78  rackAttributeBox
-00000590: 6e61 6d65 203d 2054 7261 636b 4174 7472  name = TrackAttr
-000005a0: 6962 7574 6542 6f78 6e61 6d65 0d0a 2020  ibuteBoxname..  
-000005b0: 2020 2020 2020 7365 6c66 2e54 7261 636b        self.Track
-000005c0: 6964 426f 7820 3d20 5472 6163 6b69 6442  idBox = TrackidB
-000005d0: 6f78 0d0a 2020 2020 2020 2020 7365 6c66  ox..        self
-000005e0: 2e6d 6173 7465 725f 6578 7472 615f 6e61  .master_extra_na
-000005f0: 6d65 203d 206d 6173 7465 725f 6578 7472  me = master_extr
-00000600: 615f 6e61 6d65 0d0a 2020 2020 2020 200d  a_name..       .
-00000610: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
-00000620: 2020 7365 6c66 2e6e 756d 5f70 6f69 6e74    self.num_point
-00000630: 7320 3d20 6e75 6d5f 706f 696e 7473 0d0a  s = num_points..
-00000640: 2020 2020 2020 2020 7365 6c66 2e73 706f          self.spo
-00000650: 745f 6461 7461 7365 742c 2073 656c 662e  t_dataset, self.
-00000660: 7370 6f74 5f64 6174 6173 6574 5f69 6e64  spot_dataset_ind
-00000670: 6578 203d 2067 6574 5f63 7376 5f64 6174  ex = get_csv_dat
-00000680: 6128 7365 6c66 2e73 706f 745f 6373 765f  a(self.spot_csv_
-00000690: 7061 7468 290d 0a20 2020 2020 2020 2073  path)..        s
-000006a0: 656c 662e 7472 6163 6b5f 6461 7461 7365  elf.track_datase
-000006b0: 742c 2073 656c 662e 7472 6163 6b5f 6461  t, self.track_da
-000006c0: 7461 7365 745f 696e 6465 7820 3d20 6765  taset_index = ge
-000006d0: 745f 6373 765f 6461 7461 2873 656c 662e  t_csv_data(self.
-000006e0: 7472 6163 6b5f 6373 765f 7061 7468 290d  track_csv_path).
-000006f0: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-00000700: 6765 735f 6461 7461 7365 742c 2073 656c  ges_dataset, sel
-00000710: 662e 6564 6765 735f 6461 7461 7365 745f  f.edges_dataset_
-00000720: 696e 6465 7820 3d20 6765 745f 6373 765f  index = get_csv_
-00000730: 6461 7461 2873 656c 662e 6564 6765 735f  data(self.edges_
-00000740: 6373 765f 7061 7468 290d 0a20 2020 2020  csv_path)..     
-00000750: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-00000760: 5f62 6172 203d 2070 726f 6772 6573 735f  _bar = progress_
-00000770: 6261 720d 0a20 2020 2020 2020 2073 656c  bar..        sel
-00000780: 662e 6178 6573 203d 2061 7865 7320 2020  f.axes = axes   
-00000790: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000007a0: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
-000007b0: 685f 7369 7a65 203d 2062 6174 6368 5f73  h_size = batch_s
-000007c0: 697a 6520 0d0a 2020 2020 2020 2020 0d0a  ize ..        ..
-000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007f0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00000800: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-00000810: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00000820: 6b65 7973 203d 2064 6963 7428 0d0a 2020  keys = dict(..  
-00000830: 2020 2020 2020 2020 2020 2020 2020 7370                sp
-00000840: 6f74 5f69 643d 2249 4422 2c0d 0a20 2020  ot_id="ID",..   
-00000850: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00000860: 636b 5f69 643d 2254 5241 434b 5f49 4422  ck_id="TRACK_ID"
-00000870: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000880: 2020 2071 7561 6c69 7479 3d22 5155 414c     quality="QUAL
-00000890: 4954 5922 2c0d 0a20 2020 2020 2020 2020  ITY",..         
-000008a0: 2020 2020 2020 2070 6f73 6978 3d22 504f         posix="PO
-000008b0: 5349 5449 4f4e 5f58 222c 0d0a 2020 2020  SITION_X",..    
-000008c0: 2020 2020 2020 2020 2020 2020 706f 7369              posi
-000008d0: 793d 2250 4f53 4954 494f 4e5f 5922 2c0d  y="POSITION_Y",.
-000008e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000008f0: 2070 6f73 697a 3d22 504f 5349 5449 4f4e   posiz="POSITION
-00000900: 5f5a 222c 0d0a 2020 2020 2020 2020 2020  _Z",..          
-00000910: 2020 2020 2020 706f 7369 743d 2250 4f53        posit="POS
-00000920: 4954 494f 4e5f 5422 2c0d 0a20 2020 2020  ITION_T",..     
-00000930: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
-00000940: 3d22 4652 414d 4522 2c0d 0a20 2020 2020  ="FRAME",..     
-00000950: 2020 2020 2020 2020 2020 2072 6164 6975             radiu
-00000960: 733d 2252 4144 4955 5322 2c0d 0a20 2020  s="RADIUS",..   
-00000970: 2020 2020 2020 2020 2020 2020 206d 6561               mea
-00000980: 6e5f 696e 7465 6e73 6974 795f 6368 313d  n_intensity_ch1=
-00000990: 224d 4541 4e5f 494e 5445 4e53 4954 595f  "MEAN_INTENSITY_
-000009a0: 4348 3122 2c0d 0a20 2020 2020 2020 2020  CH1",..         
-000009b0: 2020 2020 2020 2074 6f74 616c 5f69 6e74         total_int
-000009c0: 656e 7369 7479 5f63 6831 3d22 544f 5441  ensity_ch1="TOTA
-000009d0: 4c5f 494e 5445 4e53 4954 595f 4348 3122  L_INTENSITY_CH1"
-000009e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000009f0: 2020 206d 6561 6e5f 696e 7465 6e73 6974     mean_intensit
-00000a00: 795f 6368 323d 224d 4541 4e5f 494e 5445  y_ch2="MEAN_INTE
-00000a10: 4e53 4954 595f 4348 3222 2c0d 0a20 2020  NSITY_CH2",..   
-00000a20: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
-00000a30: 616c 5f69 6e74 656e 7369 7479 5f63 6832  al_intensity_ch2
-00000a40: 3d22 544f 5441 4c5f 494e 5445 4e53 4954  ="TOTAL_INTENSIT
-00000a50: 595f 4348 3222 2c0d 0a20 2020 2020 2020  Y_CH2",..       
-00000a60: 2020 2020 2020 2020 206d 6561 6e5f 696e           mean_in
-00000a70: 7465 6e73 6974 793d 224d 4541 4e5f 494e  tensity="MEAN_IN
-00000a80: 5445 4e53 4954 5922 2c0d 0a20 2020 2020  TENSITY",..     
-00000a90: 2020 2020 2020 2020 2020 2074 6f74 616c             total
-00000aa0: 5f69 6e74 656e 7369 7479 3d22 544f 5441  _intensity="TOTA
-00000ab0: 4c5f 494e 5445 4e53 4954 5922 0d0a 2020  L_INTENSITY"..  
-00000ac0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00000ad0: 2020 2020 2073 656c 662e 7472 6163 6b5f       self.track_
-00000ae0: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
-00000af0: 6579 7320 3d20 6469 6374 280d 0a20 2020  eys = dict(..   
-00000b00: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00000b10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000b20: 706f 745f 736f 7572 6365 5f69 643d 2253  pot_source_id="S
-00000b30: 504f 545f 534f 5552 4345 5f49 4422 2c0d  POT_SOURCE_ID",.
-00000b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b50: 2073 706f 745f 7461 7267 6574 5f69 643d   spot_target_id=
-00000b60: 2253 504f 545f 5441 5247 4554 5f49 4422  "SPOT_TARGET_ID"
-00000b70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000b80: 2020 2073 7065 6564 3d22 5350 4545 4422     speed="SPEED"
-00000b90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000ba0: 2020 2064 6973 706c 6163 656d 656e 743d     displacement=
-00000bb0: 2244 4953 504c 4143 454d 454e 5422 2c0d  "DISPLACEMENT",.
-00000bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000bd0: 2065 6467 655f 7469 6d65 3d22 4544 4745   edge_time="EDGE
-00000be0: 5f54 494d 4522 2c0d 0a20 2020 2020 2020  _TIME",..       
-00000bf0: 2020 2020 2020 2020 2065 6467 655f 785f           edge_x_
-00000c00: 6c6f 6361 7469 6f6e 3d22 4544 4745 5f58  location="EDGE_X
-00000c10: 5f4c 4f43 4154 494f 4e22 2c0d 0a20 2020  _LOCATION",..   
-00000c20: 2020 2020 2020 2020 2020 2020 2065 6467               edg
-00000c30: 655f 795f 6c6f 6361 7469 6f6e 3d22 4544  e_y_location="ED
-00000c40: 4745 5f59 5f4c 4f43 4154 494f 4e22 2c0d  GE_Y_LOCATION",.
-00000c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c60: 2065 6467 655f 7a5f 6c6f 6361 7469 6f6e   edge_z_location
-00000c70: 3d22 4544 4745 5f5a 5f4c 4f43 4154 494f  ="EDGE_Z_LOCATIO
-00000c80: 4e22 2c0d 0a20 2020 2020 2020 2020 2020  N",..           
-00000c90: 2029 0d0a 2020 2020 2020 2020 7365 6c66   )..        self
-00000ca0: 2e74 7261 636b 5f61 6e61 6c79 7369 735f  .track_analysis_
-00000cb0: 7472 6163 6b5f 6b65 7973 203d 2064 6963  track_keys = dic
-00000cc0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-00000cd0: 2020 2020 6e75 6d62 6572 5f73 706f 7473      number_spots
-00000ce0: 3d22 4e55 4d42 4552 5f53 504f 5453 222c  ="NUMBER_SPOTS",
-00000cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000d00: 2020 6e75 6d62 6572 5f67 6170 733d 224e    number_gaps="N
-00000d10: 554d 4245 525f 4741 5053 222c 0d0a 2020  UMBER_GAPS",..  
-00000d20: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00000d30: 6d62 6572 5f73 706c 6974 733d 224e 554d  mber_splits="NUM
-00000d40: 4245 525f 5350 4c49 5453 222c 0d0a 2020  BER_SPLITS",..  
-00000d50: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00000d60: 6d62 6572 5f6d 6572 6765 733d 224e 554d  mber_merges="NUM
-00000d70: 4245 525f 4d45 5247 4553 222c 0d0a 2020  BER_MERGES",..  
-00000d80: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00000d90: 6163 6b5f 6475 7261 7469 6f6e 3d22 5452  ack_duration="TR
-00000da0: 4143 4b5f 4455 5241 5449 4f4e 222c 0d0a  ACK_DURATION",..
-00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dc0: 7472 6163 6b5f 7374 6172 743d 2254 5241  track_start="TRA
-00000dd0: 434b 5f53 5441 5254 222c 0d0a 2020 2020  CK_START",..    
-00000de0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00000df0: 6b5f 7374 6f70 3d22 5452 4143 4b5f 5354  k_stop="TRACK_ST
-00000e00: 4f50 222c 0d0a 2020 2020 2020 2020 2020  OP",..          
-00000e10: 2020 2020 2020 7472 6163 6b5f 6469 7370        track_disp
-00000e20: 6c61 6365 6d65 6e74 3d22 5452 4143 4b5f  lacement="TRACK_
-00000e30: 4449 5350 4c41 4345 4d45 4e54 222c 0d0a  DISPLACEMENT",..
-00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e50: 7472 6163 6b5f 785f 6c6f 6361 7469 6f6e  track_x_location
-00000e60: 3d22 5452 4143 4b5f 585f 4c4f 4341 5449  ="TRACK_X_LOCATI
-00000e70: 4f4e 222c 0d0a 2020 2020 2020 2020 2020  ON",..          
-00000e80: 2020 2020 2020 7472 6163 6b5f 795f 6c6f        track_y_lo
-00000e90: 6361 7469 6f6e 3d22 5452 4143 4b5f 595f  cation="TRACK_Y_
-00000ea0: 4c4f 4341 5449 4f4e 222c 0d0a 2020 2020  LOCATION",..    
-00000eb0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00000ec0: 6b5f 7a5f 6c6f 6361 7469 6f6e 3d22 5452  k_z_location="TR
-00000ed0: 4143 4b5f 5a5f 4c4f 4341 5449 4f4e 222c  ACK_Z_LOCATION",
-00000ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000ef0: 2020 7472 6163 6b5f 6d65 616e 5f73 7065    track_mean_spe
-00000f00: 6564 3d22 5452 4143 4b5f 4d45 414e 5f53  ed="TRACK_MEAN_S
-00000f10: 5045 4544 222c 0d0a 2020 2020 2020 2020  PEED",..        
-00000f20: 2020 2020 2020 2020 7472 6163 6b5f 6d61          track_ma
-00000f30: 785f 7370 6565 643d 2254 5241 434b 5f4d  x_speed="TRACK_M
-00000f40: 4158 5f53 5045 4544 222c 0d0a 2020 2020  AX_SPEED",..    
-00000f50: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00000f60: 6b5f 6d69 6e5f 7370 6565 643d 2254 5241  k_min_speed="TRA
-00000f70: 434b 5f4d 494e 5f53 5045 4544 222c 0d0a  CK_MIN_SPEED",..
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 7472 6163 6b5f 6d65 6469 616e 5f73 7065  track_median_spe
-00000fa0: 6564 3d22 5452 4143 4b5f 4d45 4449 414e  ed="TRACK_MEDIAN
-00000fb0: 5f53 5045 4544 222c 0d0a 2020 2020 2020  _SPEED",..      
-00000fc0: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
-00000fd0: 7374 645f 7370 6565 643d 2254 5241 434b  std_speed="TRACK
-00000fe0: 5f53 5444 5f53 5045 4544 222c 0d0a 2020  _STD_SPEED",..  
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00001000: 6163 6b5f 6d65 616e 5f71 7561 6c69 7479  ack_mean_quality
-00001010: 3d22 5452 4143 4b5f 4d45 414e 5f51 5541  ="TRACK_MEAN_QUA
-00001020: 4c49 5459 222c 0d0a 2020 2020 2020 2020  LITY",..        
-00001030: 2020 2020 2020 2020 746f 7461 6c5f 7472          total_tr
-00001040: 6163 6b5f 6469 7374 616e 6365 3d22 544f  ack_distance="TO
-00001050: 5441 4c5f 4449 5354 414e 4345 5f54 5241  TAL_DISTANCE_TRA
-00001060: 5645 4c45 4422 2c0d 0a20 2020 2020 2020  VELED",..       
-00001070: 2020 2020 2020 2020 206d 6178 5f74 7261           max_tra
-00001080: 636b 5f64 6973 7461 6e63 653d 224d 4158  ck_distance="MAX
-00001090: 5f44 4953 5441 4e43 455f 5452 4156 454c  _DISTANCE_TRAVEL
-000010a0: 4544 222c 0d0a 2020 2020 2020 2020 2020  ED",..          
-000010b0: 2020 2020 2020 6d65 616e 5f73 7472 6169        mean_strai
-000010c0: 6768 745f 6c69 6e65 5f73 7065 6564 3d22  ght_line_speed="
-000010d0: 4d45 414e 5f53 5452 4149 4748 545f 4c49  MEAN_STRAIGHT_LI
-000010e0: 4e45 5f53 5045 4544 222c 0d0a 2020 2020  NE_SPEED",..    
-000010f0: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-00001100: 6172 6974 795f 666f 7277 6172 645f 7072  arity_forward_pr
-00001110: 6f67 7265 7373 696f 6e3d 224c 494e 4541  ogression="LINEA
-00001120: 5249 5459 5f4f 465f 464f 5257 4152 445f  RITY_OF_FORWARD_
-00001130: 5052 4f47 5245 5353 494f 4e22 0d0a 2020  PROGRESSION"..  
-00001140: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
-00001150: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
-00001160: 6569 645f 6b65 7920 3d20 7365 6c66 2e74  eid_key = self.t
-00001170: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00001180: 6f74 5f6b 6579 735b 2266 7261 6d65 225d  ot_keys["frame"]
-00001190: 0d0a 2020 2020 2020 2020 7365 6c66 2e7a  ..        self.z
-000011a0: 706f 7369 645f 6b65 7920 3d20 7365 6c66  posid_key = self
-000011b0: 2e74 7261 636b 5f61 6e61 6c79 7369 735f  .track_analysis_
-000011c0: 7370 6f74 5f6b 6579 735b 2270 6f73 697a  spot_keys["posiz
-000011d0: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
-000011e0: 2e79 706f 7369 645f 6b65 7920 3d20 7365  .yposid_key = se
-000011f0: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
-00001200: 735f 7370 6f74 5f6b 6579 735b 2270 6f73  s_spot_keys["pos
-00001210: 6979 225d 0d0a 2020 2020 2020 2020 7365  iy"]..        se
-00001220: 6c66 2e78 706f 7369 645f 6b65 7920 3d20  lf.xposid_key = 
-00001230: 7365 6c66 2e74 7261 636b 5f61 6e61 6c79  self.track_analy
-00001240: 7369 735f 7370 6f74 5f6b 6579 735b 2270  sis_spot_keys["p
-00001250: 6f73 6978 225d 0d0a 2020 2020 2020 2020  osix"]..        
-00001260: 7365 6c66 2e73 706f 7469 645f 6b65 7920  self.spotid_key 
-00001270: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
-00001280: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-00001290: 2273 706f 745f 6964 225d 0d0a 2020 2020  "spot_id"]..    
-000012a0: 2020 2020 7365 6c66 2e74 7261 636b 6964      self.trackid
-000012b0: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
-000012c0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-000012d0: 6b65 7973 5b22 7472 6163 6b5f 6964 225d  keys["track_id"]
-000012e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-000012f0: 6164 6975 735f 6b65 7920 3d20 7365 6c66  adius_key = self
-00001300: 2e74 7261 636b 5f61 6e61 6c79 7369 735f  .track_analysis_
-00001310: 7370 6f74 5f6b 6579 735b 2272 6164 6975  spot_keys["radiu
-00001320: 7322 5d0d 0a20 2020 2020 2020 2073 656c  s"]..        sel
-00001330: 662e 7175 616c 6974 795f 6b65 7920 3d20  f.quality_key = 
-00001340: 7365 6c66 2e74 7261 636b 5f61 6e61 6c79  self.track_analy
-00001350: 7369 735f 7370 6f74 5f6b 6579 735b 2271  sis_spot_keys["q
-00001360: 7561 6c69 7479 225d 0d0a 0d0a 2020 2020  uality"]....    
-00001370: 2020 2020 7365 6c66 2e67 656e 6572 6174      self.generat
-00001380: 696f 6e69 645f 6b65 7920 3d20 2767 656e  ionid_key = 'gen
-00001390: 6572 6174 696f 6e5f 6964 270d 0a20 2020  eration_id'..   
-000013a0: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
-000013b0: 6574 6964 5f6b 6579 203d 2027 7472 6163  etid_key = 'trac
-000013c0: 6b6c 6574 5f69 6427 0d0a 2020 2020 2020  klet_id'..      
-000013d0: 2020 7365 6c66 2e75 6e69 7175 6569 645f    self.uniqueid_
-000013e0: 6b65 7920 3d20 2775 6e69 7175 655f 6964  key = 'unique_id
-000013f0: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
-00001400: 6166 7465 7269 645f 6b65 7920 3d20 2761  afterid_key = 'a
-00001410: 6674 6572 5f69 6427 0d0a 2020 2020 2020  fter_id'..      
-00001420: 2020 7365 6c66 2e62 6566 6f72 6569 645f    self.beforeid_
-00001430: 6b65 7920 3d20 2762 6566 6f72 655f 6964  key = 'before_id
-00001440: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
-00001450: 6469 7669 6469 6e67 5f6b 6579 203d 2027  dividing_key = '
-00001460: 6469 7669 6469 6e67 5f6e 6f72 6d61 6c27  dividing_normal'
-00001470: 0d0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-00001480: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
-00001490: 6579 203d 2027 6e75 6d62 6572 5f64 6976  ey = 'number_div
-000014a0: 6964 696e 6727 0d0a 2020 2020 2020 2020  iding'..        
-000014b0: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-000014c0: 6c6c 5f6d 6173 6b5f 6b65 7920 3d20 2764  ll_mask_key = 'd
-000014d0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000014e0: 6b27 0d0a 2020 2020 2020 2020 7365 6c66  k'..        self
-000014f0: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
-00001500: 6b65 7920 3d20 276d 6173 6b63 656e 7472  key = 'maskcentr
-00001510: 6f69 645f 785f 6b65 7927 0d0a 2020 2020  oid_x_key'..    
-00001520: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
-00001530: 7472 6f69 645f 7a5f 6b65 7920 3d20 276d  troid_z_key = 'm
-00001540: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
-00001550: 7927 0d0a 2020 2020 2020 2020 7365 6c66  y'..        self
-00001560: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
-00001570: 6b65 7920 3d20 276d 6173 6b63 656e 7472  key = 'maskcentr
-00001580: 6f69 645f 795f 6b65 7927 0d0a 2020 2020  oid_y_key'..    
-00001590: 2020 2020 7365 6c66 2e63 656c 6c61 7869      self.cellaxi
-000015a0: 735f 6d61 736b 5f6b 6579 203d 2027 6365  s_mask_key = 'ce
-000015b0: 6c6c 6178 6973 5f6d 6173 6b5f 6b65 7927  llaxis_mask_key'
-000015c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-000015d0: 656c 6c69 645f 6b65 7920 3d20 2763 656c  ellid_key = 'cel
-000015e0: 6c5f 6964 270d 0a20 2020 2020 2020 2073  l_id'..        s
-000015f0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00001600: 5f6b 6579 203d 2027 6163 6365 6c65 7261  _key = 'accelera
-00001610: 7469 6f6e 270d 0a20 2020 2020 2020 2073  tion'..        s
-00001620: 656c 662e 6365 6e74 726f 6964 5f6b 6579  elf.centroid_key
-00001630: 203d 2027 6365 6e74 726f 6964 270d 0a20   = 'centroid'.. 
-00001640: 2020 2020 2020 2073 656c 662e 636c 7573         self.clus
-00001650: 7465 7263 6c61 7373 5f6b 6579 203d 2027  terclass_key = '
-00001660: 636c 7573 7465 725f 636c 6173 7327 0d0a  cluster_class'..
-00001670: 2020 2020 2020 2020 7365 6c66 2e63 6c75          self.clu
-00001680: 7374 6572 7363 6f72 655f 6b65 7920 3d20  sterscore_key = 
-00001690: 2763 6c75 7374 6572 5f73 636f 7265 270d  'cluster_score'.
-000016a0: 0a20 2020 2020 2020 2073 656c 662e 6563  .        self.ec
-000016b0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-000016c0: 6669 7273 746b 6579 203d 2027 636c 6f75  firstkey = 'clou
-000016d0: 645f 6563 6365 6e74 7269 6369 7479 5f63  d_eccentricity_c
-000016e0: 6f6d 705f 6669 7273 7427 0d0a 2020 2020  omp_first'..    
-000016f0: 2020 2020 7365 6c66 2e65 6363 656e 7472      self.eccentr
-00001700: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-00001710: 646b 6579 203d 2027 636c 6f75 645f 6563  dkey = 'cloud_ec
-00001720: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00001730: 7365 636f 6e64 270d 0a20 2020 2020 2020  second'..       
-00001740: 2073 656c 662e 7375 7266 6163 655f 6172   self.surface_ar
-00001750: 6561 5f6b 6579 203d 2027 636c 6f75 645f  ea_key = 'cloud_
-00001760: 7375 7266 6163 6561 7265 6127 0d0a 2020  surfacearea'..  
-00001770: 2020 2020 2020 7365 6c66 2e72 6164 6961        self.radia
-00001780: 6c5f 616e 676c 655f 6b65 7920 3d20 2772  l_angle_key = 'r
-00001790: 6164 6961 6c5f 616e 676c 655f 6b65 7927  adial_angle_key'
-000017a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-000017b0: 6f74 696f 6e5f 616e 676c 655f 6b65 7920  otion_angle_key 
-000017c0: 3d20 276d 6f74 696f 6e5f 616e 676c 6527  = 'motion_angle'
-000017d0: 200d 0a0d 0a20 2020 2020 2020 2073 656c   ....        sel
-000017e0: 662e 6d65 616e 5f69 6e74 656e 7369 7479  f.mean_intensity
-000017f0: 5f63 6831 5f6b 6579 203d 2073 656c 662e  _ch1_key = self.
-00001800: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-00001810: 706f 745f 6b65 7973 5b22 6d65 616e 5f69  pot_keys["mean_i
-00001820: 6e74 656e 7369 7479 5f63 6831 225d 0d0a  ntensity_ch1"]..
-00001830: 2020 2020 2020 2020 7365 6c66 2e6d 6561          self.mea
-00001840: 6e5f 696e 7465 6e73 6974 795f 6368 325f  n_intensity_ch2_
-00001850: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
-00001860: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00001870: 6579 735b 226d 6561 6e5f 696e 7465 6e73  eys["mean_intens
-00001880: 6974 795f 6368 3222 5d0d 0a20 2020 2020  ity_ch2"]..     
-00001890: 2020 2073 656c 662e 746f 7461 6c5f 696e     self.total_in
-000018a0: 7465 6e73 6974 795f 6368 315f 6b65 7920  tensity_ch1_key 
-000018b0: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
-000018c0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-000018d0: 2274 6f74 616c 5f69 6e74 656e 7369 7479  "total_intensity
-000018e0: 5f63 6831 225d 0d0a 2020 2020 2020 2020  _ch1"]..        
-000018f0: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-00001900: 7369 7479 5f63 6832 5f6b 6579 203d 2073  sity_ch2_key = s
-00001910: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001920: 6973 5f73 706f 745f 6b65 7973 5b22 746f  is_spot_keys["to
-00001930: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
-00001940: 3222 5d0d 0a0d 0a20 2020 2020 2020 2073  2"]....        s
-00001950: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-00001960: 7479 5f6b 6579 203d 2073 656c 662e 7472  ty_key = self.tr
-00001970: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00001980: 745f 6b65 7973 5b22 6d65 616e 5f69 6e74  t_keys["mean_int
-00001990: 656e 7369 7479 225d 0d0a 2020 2020 2020  ensity"]..      
-000019a0: 2020 7365 6c66 2e74 6f74 616c 5f69 6e74    self.total_int
-000019b0: 656e 7369 7479 5f6b 6579 203d 2073 656c  ensity_key = sel
-000019c0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
-000019d0: 5f73 706f 745f 6b65 7973 5b22 746f 7461  _spot_keys["tota
-000019e0: 6c5f 696e 7465 6e73 6974 7922 5d0d 0a0d  l_intensity"]...
-000019f0: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
-00001a00: 6f74 5f73 6f75 7263 655f 6964 5f6b 6579  ot_source_id_key
-00001a10: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
-00001a20: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
-00001a30: 735b 2273 706f 745f 736f 7572 6365 5f69  s["spot_source_i
-00001a40: 6422 5d0d 0a20 2020 2020 2020 2073 656c  d"]..        sel
-00001a50: 662e 7370 6f74 5f74 6172 6765 745f 6964  f.spot_target_id
-00001a60: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
-00001a70: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
-00001a80: 5f6b 6579 735b 2273 706f 745f 7461 7267  _keys["spot_targ
-00001a90: 6574 5f69 6422 5d0d 0a20 2020 2020 2020  et_id"]..       
-00001aa0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00001ab0: 2020 2020 7365 6c66 2e73 7065 6564 5f6b      self.speed_k
-00001ac0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
-00001ad0: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
-00001ae0: 6579 735b 2273 7065 6564 225d 0d0a 2020  eys["speed"]..  
-00001af0: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
-00001b00: 6163 656d 656e 745f 6b65 7920 3d20 7365  acement_key = se
-00001b10: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
-00001b20: 735f 6564 6765 735f 6b65 7973 5b22 6469  s_edges_keys["di
-00001b30: 7370 6c61 6365 6d65 6e74 225d 0d0a 2020  splacement"]..  
-00001b40: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
-00001b50: 7469 6d65 5f6b 6579 203d 2073 656c 662e  time_key = self.
-00001b60: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
-00001b70: 6467 6573 5f6b 6579 735b 2265 6467 655f  dges_keys["edge_
-00001b80: 7469 6d65 225d 0d0a 2020 2020 2020 2020  time"]..        
-00001b90: 7365 6c66 2e65 6467 655f 785f 6c6f 6361  self.edge_x_loca
-00001ba0: 7469 6f6e 5f6b 6579 203d 2073 656c 662e  tion_key = self.
-00001bb0: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
-00001bc0: 6467 6573 5f6b 6579 735b 2265 6467 655f  dges_keys["edge_
-00001bd0: 785f 6c6f 6361 7469 6f6e 225d 0d0a 2020  x_location"]..  
-00001be0: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
-00001bf0: 795f 6c6f 6361 7469 6f6e 5f6b 6579 203d  y_location_key =
-00001c00: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001c10: 7973 6973 5f65 6467 6573 5f6b 6579 735b  ysis_edges_keys[
-00001c20: 2265 6467 655f 795f 6c6f 6361 7469 6f6e  "edge_y_location
-00001c30: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
-00001c40: 2e65 6467 655f 7a5f 6c6f 6361 7469 6f6e  .edge_z_location
-00001c50: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
-00001c60: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
-00001c70: 5f6b 6579 735b 2265 6467 655f 7a5f 6c6f  _keys["edge_z_lo
-00001c80: 6361 7469 6f6e 225d 0d0a 2020 2020 2020  cation"]..      
-00001c90: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
-00001ca0: 2e75 6e69 7175 655f 7472 6163 6b73 203d  .unique_tracks =
-00001cb0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-00001cc0: 662e 756e 6971 7565 5f74 7261 636b 5f6d  f.unique_track_m
-00001cd0: 6974 6f73 6973 5f6c 6162 656c 203d 207b  itosis_label = {
-00001ce0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
-00001cf0: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
-00001d00: 7065 7274 6965 7320 3d20 7b7d 0d0a 2020  perties = {}..  
-00001d10: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00001d20: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
-00001d30: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
-00001d40: 656c 662e 756e 6971 7565 5f63 6c75 7374  elf.unique_clust
-00001d50: 6572 5f70 726f 7065 7274 6965 7320 3d20  er_properties = 
-00001d60: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
-00001d70: 2e75 6e69 7175 655f 7368 6170 655f 7072  .unique_shape_pr
-00001d80: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
-00001d90: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00001da0: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
-00001db0: 7274 6965 7320 3d20 7b7d 0d0a 2020 2020  rties = {}..    
-00001dc0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00001dd0: 7370 6f74 5f70 726f 7065 7274 6965 7320  spot_properties 
-00001de0: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
-00001df0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f63  lf.unique_spot_c
-00001e00: 656e 7472 6f69 6420 3d20 7b7d 0d0a 2020  entroid = {}..  
-00001e10: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00001e20: 655f 7472 6163 6b5f 6365 6e74 726f 6964  e_track_centroid
-00001e30: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
-00001e40: 656c 662e 726f 6f74 5f73 706f 7473 203d  elf.root_spots =
-00001e50: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-00001e60: 662e 616c 6c5f 6375 7272 656e 745f 6365  f.all_current_ce
-00001e70: 6c6c 5f69 6473 203d 207b 7d0d 0a20 2020  ll_ids = {}..   
-00001e80: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-00001e90: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-00001ea0: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
-00001eb0: 2020 2020 2020 2073 656c 662e 6564 6765         self.edge
-00001ec0: 5f74 6172 6765 745f 6c6f 6f6b 7570 203d  _target_lookup =
-00001ed0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-00001ee0: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
-00001ef0: 6f6b 7570 203d 207b 7d0d 0a20 2020 2020  okup = {}..     
-00001f00: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
-00001f10: 6f6e 5f64 6963 7420 3d20 7b7d 0d0a 2020  on_dict = {}..  
-00001f20: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-00001f30: 6c65 745f 6469 6374 203d 207b 7d0d 0a20  let_dict = {}.. 
-00001f40: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
-00001f50: 685f 7370 6c69 7420 3d20 7b7d 0d0a 2020  h_split = {}..  
-00001f60: 2020 2020 2020 7365 6c66 2e67 7261 7068        self.graph
-00001f70: 5f74 7261 636b 7320 3d20 7b7d 0d0a 2020  _tracks = {}..  
-00001f80: 2020 2020 2020 7365 6c66 2e5f 7469 6d65        self._time
-00001f90: 645f 6365 6e74 726f 6964 203d 207b 7d0d  d_centroid = {}.
-00001fa0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00001fb0: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
-00001fc0: 2078 6d6c 5f70 6172 7365 7220 3d20 6574   xml_parser = et
-00001fd0: 2e58 4d4c 5061 7273 6572 2868 7567 655f  .XMLParser(huge_
-00001fe0: 7472 6565 3d54 7275 6529 0d0a 2020 2020  tree=True)..    
-00001ff0: 2020 2020 6966 2073 656c 662e 6d61 7374      if self.mast
-00002000: 6572 5f78 6d6c 5f70 6174 6820 6973 204e  er_xml_path is N
-00002010: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00002020: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
-00002030: 5f78 6d6c 5f70 6174 6820 3d20 5061 7468  _xml_path = Path
-00002040: 2827 2e27 290d 0a20 2020 2020 2020 200d  ('.')..        .
-00002050: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00002060: 2e6d 6173 7465 725f 786d 6c5f 7061 7468  .master_xml_path
-00002070: 2e69 735f 6469 7228 2920 616e 6420 7365  .is_dir() and se
-00002080: 6c66 2e78 6d6c 5f70 6174 6820 6973 206e  lf.xml_path is n
-00002090: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-000020a0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000020b0: 2752 6561 6469 6e67 2058 4d4c 2729 0d0a  'Reading XML')..
-000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020d0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
-000020e0: 203d 2065 742e 6672 6f6d 7374 7269 6e67   = et.fromstring
-000020f0: 286f 7065 6e28 7365 6c66 2e78 6d6c 5f70  (open(self.xml_p
-00002100: 6174 6829 2e72 6561 6428 292e 656e 636f  ath).read().enco
-00002110: 6465 2829 2c20 786d 6c5f 7061 7273 6572  de(), xml_parser
-00002120: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002130: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00002140: 2020 2020 2073 656c 662e 6669 6c74 6572       self.filter
-00002150: 6564 5f74 7261 636b 5f69 6473 203d 205b  ed_track_ids = [
-00002160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002170: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00002180: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
-00002190: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000021c0: 7472 6163 6b20 696e 2073 656c 662e 786d  track in self.xm
-000021d0: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
-000021e0: 4d6f 6465 6c22 290d 0a20 2020 2020 2020  Model")..       
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 2020 2020 202e 6669 6e64 2822 4669 6c74       .find("Filt
-00002210: 6572 6564 5472 6163 6b73 2229 0d0a 2020  eredTracks")..  
-00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002230: 2020 2020 2020 2020 2020 2e66 696e 6461            .finda
-00002240: 6c6c 2822 5472 6163 6b49 4422 290d 0a20  ll("TrackID").. 
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
-00002270: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00002280: 6178 5f74 7261 636b 5f69 6420 3d20 6d61  ax_track_id = ma
-00002290: 7828 7365 6c66 2e66 696c 7465 7265 645f  x(self.filtered_
-000022a0: 7472 6163 6b5f 6964 7329 2020 2020 2020  track_ids)      
-000022b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000022c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000022d0: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
-000022e0: 786d 6c5f 6461 7461 2829 0d0a 2020 2020  xml_data()..    
-000022f0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-00002300: 7461 6e63 6528 7365 6c66 2e6d 6173 7465  tance(self.maste
-00002310: 725f 786d 6c5f 7061 7468 2c20 7374 7229  r_xml_path, str)
-00002320: 3a20 2020 2020 200d 0a20 2020 2020 2020  :      ..       
-00002330: 2020 2069 6620 7365 6c66 2e6d 6173 7465     if self.maste
-00002340: 725f 786d 6c5f 7061 7468 2e69 735f 6669  r_xml_path.is_fi
-00002350: 6c65 2829 3a0d 0a20 2020 2020 2020 2020  le():..         
-00002360: 2020 2020 2020 7072 696e 7428 2752 6561        print('Rea
-00002370: 6469 6e67 204d 6173 7465 7220 584d 4c27  ding Master XML'
-00002380: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002390: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000023a0: 2020 2073 656c 662e 786d 6c5f 636f 6e74     self.xml_cont
-000023b0: 656e 7420 3d20 6574 2e66 726f 6d73 7472  ent = et.fromstr
-000023c0: 696e 6728 6f70 656e 2873 656c 662e 6d61  ing(open(self.ma
-000023d0: 7374 6572 5f78 6d6c 5f70 6174 6829 2e72  ster_xml_path).r
-000023e0: 6561 6428 292e 656e 636f 6465 2829 2c20  ead().encode(), 
-000023f0: 786d 6c5f 7061 7273 6572 290d 0a20 2020  xml_parser)..   
-00002400: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00002410: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002420: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
-00002430: 5f69 6473 203d 205b 0d0a 2020 2020 2020  _ids = [..      
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 2020 2020 696e 7428 7472 6163 6b2e        int(track.
-00002460: 6765 7428 7365 6c66 2e74 7261 636b 6964  get(self.trackid
-00002470: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002490: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
-000024a0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-000024b0: 742e 6669 6e64 2822 4d6f 6465 6c22 290d  t.find("Model").
-000024c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000024d0: 2020 2020 2020 2020 2020 2020 202e 6669               .fi
-000024e0: 6e64 2822 4669 6c74 6572 6564 5472 6163  nd("FilteredTrac
-000024f0: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 2020 2e66 696e 6461 6c6c 2822 5472 6163    .findall("Trac
-00002520: 6b49 4422 290d 0a20 2020 2020 2020 2020  kID")..         
-00002530: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00002540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002550: 2073 656c 662e 6d61 785f 7472 6163 6b5f   self.max_track_
-00002560: 6964 203d 206d 6178 2873 656c 662e 6669  id = max(self.fi
-00002570: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-00002580: 2920 2020 2020 2020 200d 0a20 2020 2020  )        ..     
-00002590: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000025a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000025b0: 2e5f 6765 745f 6d61 7374 6572 5f78 6d6c  ._get_master_xml
-000025c0: 5f64 6174 6128 290d 0a20 2020 2020 2020  _data()..       
-000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025e0: 0d0a 0d0a 2020 2020 200d 0a0d 0a0d 0a20  ....     ...... 
-000025f0: 2020 2064 6566 205f 6372 6561 7465 5f63     def _create_c
-00002600: 6861 6e6e 656c 5f74 7265 6528 7365 6c66  hannel_tree(self
-00002610: 293a 0d0a 2020 2020 2020 2020 2020 7365  ):..          se
-00002620: 6c66 2e5f 7469 6d65 645f 6368 616e 6e65  lf._timed_channe
-00002630: 6c5f 7365 675f 696d 6167 6520 3d20 7b7d  l_seg_image = {}
-00002640: 0d0a 2020 2020 2020 2020 2020 7365 6c66  ..          self
-00002650: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
-00002660: 2020 2020 2020 6675 7475 7265 7320 3d20        futures = 
-00002670: 5b5d 0d0a 2020 2020 2020 2020 2020 7769  []..          wi
-00002680: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
-00002690: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
-000026a0: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
-000026b0: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
-000026c0: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
-000026d0: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-000026e0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000026f0: 6e20 7261 6e67 6528 7365 6c66 2e63 6861  n range(self.cha
-00002700: 6e6e 656c 5f73 6567 5f69 6d61 6765 2e73  nnel_seg_image.s
-00002710: 6861 7065 5b30 5d29 3a0d 0a20 2020 2020  hape[0]):..     
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
-00002740: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
-00002750: 7428 7365 6c66 2e5f 6368 616e 6e65 6c5f  t(self._channel_
-00002760: 636f 6d70 7574 6572 2c20 6929 290d 0a20  computer, i)).. 
-00002770: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00002780: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002790: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-000027a0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-000027b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00002800: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
-00002810: 203d 2022 446f 696e 6720 6368 616e 6e65   = "Doing channe
-00002820: 6c20 636f 6d70 7574 6174 696f 6e22 0d0a  l computation"..
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002850: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-00002860: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
-00002870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002890: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028c0: 2020 2020 206c 656e 2866 7574 7572 6573       len(futures
-000028d0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+000002e0: 272c 2073 6567 5f69 6d61 6765 3a6e 702e  ', seg_image:np.
+000002f0: 6e64 6172 7261 7920 3d20 4e6f 6e65 2c20  ndarray = None, 
+00000300: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
+00000310: 653a 6e70 2e6e 6461 7272 6179 203d 204e  e:np.ndarray = N
+00000320: 6f6e 652c 2069 6d61 6765 203a 6e70 2e6e  one, image :np.n
+00000330: 6461 7272 6179 203d 204e 6f6e 652c 206d  darray = None, m
+00000340: 6173 6b3a 6e70 2e6e 6461 7272 6179 203d  ask:np.ndarray =
+00000350: 204e 6f6e 652c 2066 6f75 7269 6572 203d   None, fourier =
+00000360: 2054 7275 652c 2063 6c75 7374 6572 5f6d   True, cluster_m
+00000370: 6f64 656c 203d 204e 6f6e 652c 206e 756d  odel = None, num
+00000380: 5f70 6f69 6e74 7320 3d20 3230 3438 2c20  _points = 2048, 
+00000390: 6261 7463 685f 7369 7a65 203d 2031 293a  batch_size = 1):
+000003a0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000003b0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+000003c0: 6c66 2e78 6d6c 5f70 6174 6820 3d20 786d  lf.xml_path = xm
+000003d0: 6c5f 7061 7468 0d0a 2020 2020 2020 2020  l_path..        
+000003e0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+000003f0: 7061 7468 203d 206d 6173 7465 725f 786d  path = master_xm
+00000400: 6c5f 7061 7468 0d0a 2020 2020 2020 2020  l_path..        
+00000410: 7365 6c66 2e73 706f 745f 6373 765f 7061  self.spot_csv_pa
+00000420: 7468 203d 2073 706f 745f 6373 765f 7061  th = spot_csv_pa
+00000430: 7468 0d0a 2020 2020 2020 2020 7365 6c66  th..        self
+00000440: 2e74 7261 636b 5f63 7376 5f70 6174 6820  .track_csv_path 
+00000450: 3d20 7472 6163 6b5f 6373 765f 7061 7468  = track_csv_path
+00000460: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
+00000470: 6564 6765 735f 6373 765f 7061 7468 203d  edges_csv_path =
+00000480: 2065 6467 6573 5f63 7376 5f70 6174 680d   edges_csv_path.
+00000490: 0a20 2020 2020 2020 2069 6620 696d 6167  .        if imag
+000004a0: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
+000004b0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+000004c0: 6d61 6765 203d 2069 6d61 6765 2e61 7374  mage = image.ast
+000004d0: 7970 6528 6e70 2e66 6c6f 6174 3136 2920  ype(np.float16) 
+000004e0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+000004f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000500: 662e 696d 6167 6520 3d20 696d 6167 650d  f.image = image.
+00000510: 0a20 2020 2020 2020 2069 6620 6d61 736b  .        if mask
+00000520: 2069 7320 6e6f 7420 4e6f 6e65 3a20 2020   is not None:   
+00000530: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00000540: 2073 656c 662e 6d61 736b 203d 206d 6173   self.mask = mas
+00000550: 6b2e 6173 7479 7065 286e 702e 7569 6e74  k.astype(np.uint
+00000560: 3136 290d 0a20 2020 2020 2020 2065 6c73  16)..        els
+00000570: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000580: 7365 6c66 2e6d 6173 6b20 3d20 6d61 736b  self.mask = mask
+00000590: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+000005a0: 2e66 6f75 7269 6572 203d 2066 6f75 7269  .fourier = fouri
+000005b0: 6572 0d0a 2020 2020 2020 2020 7365 6c66  er..        self
+000005c0: 2e63 6c75 7374 6572 5f6d 6f64 656c 203d  .cluster_model =
+000005d0: 2063 6c75 7374 6572 5f6d 6f64 656c 200d   cluster_model .
+000005e0: 0a20 2020 2020 2020 2069 6620 6368 616e  .        if chan
+000005f0: 6e65 6c5f 7365 675f 696d 6167 6520 6973  nel_seg_image is
+00000600: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00000610: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+00000620: 6e65 6c5f 7365 675f 696d 6167 6520 3d20  nel_seg_image = 
+00000630: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
+00000640: 652e 6173 7479 7065 286e 702e 7569 6e74  e.astype(np.uint
+00000650: 3136 290d 0a20 2020 2020 2020 2065 6c73  16)..        els
+00000660: 653a 0d0a 2020 2020 2020 2020 2020 2073  e:..           s
+00000670: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
+00000680: 696d 6167 6520 3d20 6368 616e 6e65 6c5f  image = channel_
+00000690: 7365 675f 696d 6167 650d 0a20 2020 2020  seg_image..     
+000006a0: 2020 2069 6620 7365 675f 696d 6167 6520     if seg_image 
+000006b0: 6973 206e 6f74 204e 6f6e 653a 2020 2020  is not None:    
+000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006d0: 0d0a 2020 2020 2020 2020 2020 2073 656c  ..           sel
+000006e0: 662e 7365 675f 696d 6167 6520 3d20 7365  f.seg_image = se
+000006f0: 675f 696d 6167 652e 6173 7479 7065 286e  g_image.astype(n
+00000700: 702e 7569 6e74 3136 290d 0a20 2020 2020  p.uint16)..     
+00000710: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000720: 2020 2020 2073 656c 662e 7365 675f 696d       self.seg_im
+00000730: 6167 6520 3d20 7365 675f 696d 6167 6520  age = seg_image 
+00000740: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00000750: 7365 6c66 2e41 7474 7269 6275 7465 426f  self.AttributeBo
+00000760: 786e 616d 6520 3d20 4174 7472 6962 7574  xname = Attribut
+00000770: 6542 6f78 6e61 6d65 0d0a 2020 2020 2020  eBoxname..      
+00000780: 2020 7365 6c66 2e54 7261 636b 4174 7472    self.TrackAttr
+00000790: 6962 7574 6542 6f78 6e61 6d65 203d 2054  ibuteBoxname = T
+000007a0: 7261 636b 4174 7472 6962 7574 6542 6f78  rackAttributeBox
+000007b0: 6e61 6d65 0d0a 2020 2020 2020 2020 7365  name..        se
+000007c0: 6c66 2e54 7261 636b 6964 426f 7820 3d20  lf.TrackidBox = 
+000007d0: 5472 6163 6b69 6442 6f78 0d0a 2020 2020  TrackidBox..    
+000007e0: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
+000007f0: 6578 7472 615f 6e61 6d65 203d 206d 6173  extra_name = mas
+00000800: 7465 725f 6578 7472 615f 6e61 6d65 0d0a  ter_extra_name..
+00000810: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00000820: 0d0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
+00000830: 756d 5f70 6f69 6e74 7320 3d20 6e75 6d5f  um_points = num_
+00000840: 706f 696e 7473 0d0a 2020 2020 2020 2020  points..        
+00000850: 7365 6c66 2e73 706f 745f 6461 7461 7365  self.spot_datase
+00000860: 742c 2073 656c 662e 7370 6f74 5f64 6174  t, self.spot_dat
+00000870: 6173 6574 5f69 6e64 6578 203d 2067 6574  aset_index = get
+00000880: 5f63 7376 5f64 6174 6128 7365 6c66 2e73  _csv_data(self.s
+00000890: 706f 745f 6373 765f 7061 7468 290d 0a20  pot_csv_path).. 
+000008a0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+000008b0: 6b5f 6461 7461 7365 742c 2073 656c 662e  k_dataset, self.
+000008c0: 7472 6163 6b5f 6461 7461 7365 745f 696e  track_dataset_in
+000008d0: 6465 7820 3d20 6765 745f 6373 765f 6461  dex = get_csv_da
+000008e0: 7461 2873 656c 662e 7472 6163 6b5f 6373  ta(self.track_cs
+000008f0: 765f 7061 7468 290d 0a20 2020 2020 2020  v_path)..       
+00000900: 2073 656c 662e 6564 6765 735f 6461 7461   self.edges_data
+00000910: 7365 742c 2073 656c 662e 6564 6765 735f  set, self.edges_
+00000920: 6461 7461 7365 745f 696e 6465 7820 3d20  dataset_index = 
+00000930: 6765 745f 6373 765f 6461 7461 2873 656c  get_csv_data(sel
+00000940: 662e 6564 6765 735f 6373 765f 7061 7468  f.edges_csv_path
+00000950: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00000960: 7072 6f67 7265 7373 5f62 6172 203d 2070  progress_bar = p
+00000970: 726f 6772 6573 735f 6261 720d 0a20 2020  rogress_bar..   
+00000980: 2020 2020 2073 656c 662e 6178 6573 203d       self.axes =
+00000990: 2061 7865 7320 2020 2020 2020 2020 2020   axes           
+000009a0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+000009b0: 656c 662e 6261 7463 685f 7369 7a65 203d  elf.batch_size =
+000009c0: 2062 6174 6368 5f73 697a 6520 0d0a 2020   batch_size ..  
+000009d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+00000a10: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00000a20: 6973 5f73 706f 745f 6b65 7973 203d 2064  is_spot_keys = d
+00000a30: 6963 7428 0d0a 2020 2020 2020 2020 2020  ict(..          
+00000a40: 2020 2020 2020 7370 6f74 5f69 643d 2249        spot_id="I
+00000a50: 4422 2c0d 0a20 2020 2020 2020 2020 2020  D",..           
+00000a60: 2020 2020 2074 7261 636b 5f69 643d 2254       track_id="T
+00000a70: 5241 434b 5f49 4422 2c0d 0a20 2020 2020  RACK_ID",..     
+00000a80: 2020 2020 2020 2020 2020 2071 7561 6c69             quali
+00000a90: 7479 3d22 5155 414c 4954 5922 2c0d 0a20  ty="QUALITY",.. 
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00000ab0: 6f73 6978 3d22 504f 5349 5449 4f4e 5f58  osix="POSITION_X
+00000ac0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000ad0: 2020 2020 706f 7369 793d 2250 4f53 4954      posiy="POSIT
+00000ae0: 494f 4e5f 5922 2c0d 0a20 2020 2020 2020  ION_Y",..       
+00000af0: 2020 2020 2020 2020 2070 6f73 697a 3d22           posiz="
+00000b00: 504f 5349 5449 4f4e 5f5a 222c 0d0a 2020  POSITION_Z",..  
+00000b10: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00000b20: 7369 743d 2250 4f53 4954 494f 4e5f 5422  sit="POSITION_T"
+00000b30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000b40: 2020 2066 7261 6d65 3d22 4652 414d 4522     frame="FRAME"
+00000b50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000b60: 2020 2072 6164 6975 733d 2252 4144 4955     radius="RADIU
+00000b70: 5322 2c0d 0a20 2020 2020 2020 2020 2020  S",..           
+00000b80: 2020 2020 206d 6561 6e5f 696e 7465 6e73       mean_intens
+00000b90: 6974 795f 6368 313d 224d 4541 4e5f 494e  ity_ch1="MEAN_IN
+00000ba0: 5445 4e53 4954 595f 4348 3122 2c0d 0a20  TENSITY_CH1",.. 
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00000bc0: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
+00000bd0: 6831 3d22 544f 5441 4c5f 494e 5445 4e53  h1="TOTAL_INTENS
+00000be0: 4954 595f 4348 3122 2c0d 0a20 2020 2020  ITY_CH1",..     
+00000bf0: 2020 2020 2020 2020 2020 206d 6561 6e5f             mean_
+00000c00: 696e 7465 6e73 6974 795f 6368 323d 224d  intensity_ch2="M
+00000c10: 4541 4e5f 494e 5445 4e53 4954 595f 4348  EAN_INTENSITY_CH
+00000c20: 3222 2c0d 0a20 2020 2020 2020 2020 2020  2",..           
+00000c30: 2020 2020 2074 6f74 616c 5f69 6e74 656e       total_inten
+00000c40: 7369 7479 5f63 6832 3d22 544f 5441 4c5f  sity_ch2="TOTAL_
+00000c50: 494e 5445 4e53 4954 595f 4348 3222 2c0d  INTENSITY_CH2",.
+00000c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c70: 206d 6561 6e5f 696e 7465 6e73 6974 793d   mean_intensity=
+00000c80: 224d 4541 4e5f 494e 5445 4e53 4954 5922  "MEAN_INTENSITY"
+00000c90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000ca0: 2020 2074 6f74 616c 5f69 6e74 656e 7369     total_intensi
+00000cb0: 7479 3d22 544f 5441 4c5f 494e 5445 4e53  ty="TOTAL_INTENS
+00000cc0: 4954 5922 0d0a 2020 2020 2020 2020 2020  ITY"..          
+00000cd0: 2020 290d 0a20 2020 2020 2020 2073 656c    )..        sel
+00000ce0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
+00000cf0: 5f65 6467 6573 5f6b 6579 7320 3d20 6469  _edges_keys = di
+00000d00: 6374 280d 0a20 2020 2020 2020 2020 2020  ct(..           
+00000d10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00000d20: 2020 2020 2020 2073 706f 745f 736f 7572         spot_sour
+00000d30: 6365 5f69 643d 2253 504f 545f 534f 5552  ce_id="SPOT_SOUR
+00000d40: 4345 5f49 4422 2c0d 0a20 2020 2020 2020  CE_ID",..       
+00000d50: 2020 2020 2020 2020 2073 706f 745f 7461           spot_ta
+00000d60: 7267 6574 5f69 643d 2253 504f 545f 5441  rget_id="SPOT_TA
+00000d70: 5247 4554 5f49 4422 2c0d 0a20 2020 2020  RGET_ID",..     
+00000d80: 2020 2020 2020 2020 2020 2073 7065 6564             speed
+00000d90: 3d22 5350 4545 4422 2c0d 0a20 2020 2020  ="SPEED",..     
+00000da0: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+00000db0: 6163 656d 656e 743d 2244 4953 504c 4143  acement="DISPLAC
+00000dc0: 454d 454e 5422 2c0d 0a20 2020 2020 2020  EMENT",..       
+00000dd0: 2020 2020 2020 2020 2065 6467 655f 7469           edge_ti
+00000de0: 6d65 3d22 4544 4745 5f54 494d 4522 2c0d  me="EDGE_TIME",.
+00000df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e00: 2065 6467 655f 785f 6c6f 6361 7469 6f6e   edge_x_location
+00000e10: 3d22 4544 4745 5f58 5f4c 4f43 4154 494f  ="EDGE_X_LOCATIO
+00000e20: 4e22 2c0d 0a20 2020 2020 2020 2020 2020  N",..           
+00000e30: 2020 2020 2065 6467 655f 795f 6c6f 6361       edge_y_loca
+00000e40: 7469 6f6e 3d22 4544 4745 5f59 5f4c 4f43  tion="EDGE_Y_LOC
+00000e50: 4154 494f 4e22 2c0d 0a20 2020 2020 2020  ATION",..       
+00000e60: 2020 2020 2020 2020 2065 6467 655f 7a5f           edge_z_
+00000e70: 6c6f 6361 7469 6f6e 3d22 4544 4745 5f5a  location="EDGE_Z
+00000e80: 5f4c 4f43 4154 494f 4e22 2c0d 0a20 2020  _LOCATION",..   
+00000e90: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00000ea0: 2020 2020 7365 6c66 2e74 7261 636b 5f61      self.track_a
+00000eb0: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
+00000ec0: 7973 203d 2064 6963 7428 0d0a 2020 2020  ys = dict(..    
+00000ed0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+00000ee0: 6572 5f73 706f 7473 3d22 4e55 4d42 4552  er_spots="NUMBER
+00000ef0: 5f53 504f 5453 222c 0d0a 2020 2020 2020  _SPOTS",..      
+00000f00: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+00000f10: 5f67 6170 733d 224e 554d 4245 525f 4741  _gaps="NUMBER_GA
+00000f20: 5053 222c 0d0a 2020 2020 2020 2020 2020  PS",..          
+00000f30: 2020 2020 2020 6e75 6d62 6572 5f73 706c        number_spl
+00000f40: 6974 733d 224e 554d 4245 525f 5350 4c49  its="NUMBER_SPLI
+00000f50: 5453 222c 0d0a 2020 2020 2020 2020 2020  TS",..          
+00000f60: 2020 2020 2020 6e75 6d62 6572 5f6d 6572        number_mer
+00000f70: 6765 733d 224e 554d 4245 525f 4d45 5247  ges="NUMBER_MERG
+00000f80: 4553 222c 0d0a 2020 2020 2020 2020 2020  ES",..          
+00000f90: 2020 2020 2020 7472 6163 6b5f 6475 7261        track_dura
+00000fa0: 7469 6f6e 3d22 5452 4143 4b5f 4455 5241  tion="TRACK_DURA
+00000fb0: 5449 4f4e 222c 0d0a 2020 2020 2020 2020  TION",..        
+00000fc0: 2020 2020 2020 2020 7472 6163 6b5f 7374          track_st
+00000fd0: 6172 743d 2254 5241 434b 5f53 5441 5254  art="TRACK_START
+00000fe0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000ff0: 2020 2020 7472 6163 6b5f 7374 6f70 3d22      track_stop="
+00001000: 5452 4143 4b5f 5354 4f50 222c 0d0a 2020  TRACK_STOP",..  
+00001010: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00001020: 6163 6b5f 6469 7370 6c61 6365 6d65 6e74  ack_displacement
+00001030: 3d22 5452 4143 4b5f 4449 5350 4c41 4345  ="TRACK_DISPLACE
+00001040: 4d45 4e54 222c 0d0a 2020 2020 2020 2020  MENT",..        
+00001050: 2020 2020 2020 2020 7472 6163 6b5f 785f          track_x_
+00001060: 6c6f 6361 7469 6f6e 3d22 5452 4143 4b5f  location="TRACK_
+00001070: 585f 4c4f 4341 5449 4f4e 222c 0d0a 2020  X_LOCATION",..  
+00001080: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00001090: 6163 6b5f 795f 6c6f 6361 7469 6f6e 3d22  ack_y_location="
+000010a0: 5452 4143 4b5f 595f 4c4f 4341 5449 4f4e  TRACK_Y_LOCATION
+000010b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000010c0: 2020 2020 7472 6163 6b5f 7a5f 6c6f 6361      track_z_loca
+000010d0: 7469 6f6e 3d22 5452 4143 4b5f 5a5f 4c4f  tion="TRACK_Z_LO
+000010e0: 4341 5449 4f4e 222c 0d0a 2020 2020 2020  CATION",..      
+000010f0: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
+00001100: 6d65 616e 5f73 7065 6564 3d22 5452 4143  mean_speed="TRAC
+00001110: 4b5f 4d45 414e 5f53 5045 4544 222c 0d0a  K_MEAN_SPEED",..
+00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001130: 7472 6163 6b5f 6d61 785f 7370 6565 643d  track_max_speed=
+00001140: 2254 5241 434b 5f4d 4158 5f53 5045 4544  "TRACK_MAX_SPEED
+00001150: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00001160: 2020 2020 7472 6163 6b5f 6d69 6e5f 7370      track_min_sp
+00001170: 6565 643d 2254 5241 434b 5f4d 494e 5f53  eed="TRACK_MIN_S
+00001180: 5045 4544 222c 0d0a 2020 2020 2020 2020  PEED",..        
+00001190: 2020 2020 2020 2020 7472 6163 6b5f 6d65          track_me
+000011a0: 6469 616e 5f73 7065 6564 3d22 5452 4143  dian_speed="TRAC
+000011b0: 4b5f 4d45 4449 414e 5f53 5045 4544 222c  K_MEDIAN_SPEED",
+000011c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000011d0: 2020 7472 6163 6b5f 7374 645f 7370 6565    track_std_spee
+000011e0: 643d 2254 5241 434b 5f53 5444 5f53 5045  d="TRACK_STD_SPE
+000011f0: 4544 222c 0d0a 2020 2020 2020 2020 2020  ED",..          
+00001200: 2020 2020 2020 7472 6163 6b5f 6d65 616e        track_mean
+00001210: 5f71 7561 6c69 7479 3d22 5452 4143 4b5f  _quality="TRACK_
+00001220: 4d45 414e 5f51 5541 4c49 5459 222c 0d0a  MEAN_QUALITY",..
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 746f 7461 6c5f 7472 6163 6b5f 6469 7374  total_track_dist
+00001250: 616e 6365 3d22 544f 5441 4c5f 4449 5354  ance="TOTAL_DIST
+00001260: 414e 4345 5f54 5241 5645 4c45 4422 2c0d  ANCE_TRAVELED",.
+00001270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001280: 206d 6178 5f74 7261 636b 5f64 6973 7461   max_track_dista
+00001290: 6e63 653d 224d 4158 5f44 4953 5441 4e43  nce="MAX_DISTANC
+000012a0: 455f 5452 4156 454c 4544 222c 0d0a 2020  E_TRAVELED",..  
+000012b0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+000012c0: 616e 5f73 7472 6169 6768 745f 6c69 6e65  an_straight_line
+000012d0: 5f73 7065 6564 3d22 4d45 414e 5f53 5452  _speed="MEAN_STR
+000012e0: 4149 4748 545f 4c49 4e45 5f53 5045 4544  AIGHT_LINE_SPEED
+000012f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00001300: 2020 2020 6c69 6e65 6172 6974 795f 666f      linearity_fo
+00001310: 7277 6172 645f 7072 6f67 7265 7373 696f  rward_progressio
+00001320: 6e3d 224c 494e 4541 5249 5459 5f4f 465f  n="LINEARITY_OF_
+00001330: 464f 5257 4152 445f 5052 4f47 5245 5353  FORWARD_PROGRESS
+00001340: 494f 4e22 0d0a 2020 2020 2020 2020 2020  ION"..          
+00001350: 2020 290d 0a0d 0a20 2020 2020 2020 2073    )....        s
+00001360: 656c 662e 6672 616d 6569 645f 6b65 7920  elf.frameid_key 
+00001370: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
+00001380: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+00001390: 2266 7261 6d65 225d 0d0a 2020 2020 2020  "frame"]..      
+000013a0: 2020 7365 6c66 2e7a 706f 7369 645f 6b65    self.zposid_ke
+000013b0: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
+000013c0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+000013d0: 735b 2270 6f73 697a 225d 0d0a 2020 2020  s["posiz"]..    
+000013e0: 2020 2020 7365 6c66 2e79 706f 7369 645f      self.yposid_
+000013f0: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
+00001400: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00001410: 6579 735b 2270 6f73 6979 225d 0d0a 2020  eys["posiy"]..  
+00001420: 2020 2020 2020 7365 6c66 2e78 706f 7369        self.xposi
+00001430: 645f 6b65 7920 3d20 7365 6c66 2e74 7261  d_key = self.tra
+00001440: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00001450: 5f6b 6579 735b 2270 6f73 6978 225d 0d0a  _keys["posix"]..
+00001460: 2020 2020 2020 2020 7365 6c66 2e73 706f          self.spo
+00001470: 7469 645f 6b65 7920 3d20 7365 6c66 2e74  tid_key = self.t
+00001480: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00001490: 6f74 5f6b 6579 735b 2273 706f 745f 6964  ot_keys["spot_id
+000014a0: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
+000014b0: 2e74 7261 636b 6964 5f6b 6579 203d 2073  .trackid_key = s
+000014c0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+000014d0: 6973 5f73 706f 745f 6b65 7973 5b22 7472  is_spot_keys["tr
+000014e0: 6163 6b5f 6964 225d 0d0a 2020 2020 2020  ack_id"]..      
+000014f0: 2020 7365 6c66 2e72 6164 6975 735f 6b65    self.radius_ke
+00001500: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
+00001510: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+00001520: 735b 2272 6164 6975 7322 5d0d 0a20 2020  s["radius"]..   
+00001530: 2020 2020 2073 656c 662e 7175 616c 6974       self.qualit
+00001540: 795f 6b65 7920 3d20 7365 6c66 2e74 7261  y_key = self.tra
+00001550: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00001560: 5f6b 6579 735b 2271 7561 6c69 7479 225d  _keys["quality"]
+00001570: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00001580: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
+00001590: 7920 3d20 2767 656e 6572 6174 696f 6e5f  y = 'generation_
+000015a0: 6964 270d 0a20 2020 2020 2020 2073 656c  id'..        sel
+000015b0: 662e 7472 6163 6b6c 6574 6964 5f6b 6579  f.trackletid_key
+000015c0: 203d 2027 7472 6163 6b6c 6574 5f69 6427   = 'tracklet_id'
+000015d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+000015e0: 6e69 7175 6569 645f 6b65 7920 3d20 2775  niqueid_key = 'u
+000015f0: 6e69 7175 655f 6964 270d 0a20 2020 2020  nique_id'..     
+00001600: 2020 2073 656c 662e 6166 7465 7269 645f     self.afterid_
+00001610: 6b65 7920 3d20 2761 6674 6572 5f69 6427  key = 'after_id'
+00001620: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
+00001630: 6566 6f72 6569 645f 6b65 7920 3d20 2762  eforeid_key = 'b
+00001640: 6566 6f72 655f 6964 270d 0a20 2020 2020  efore_id'..     
+00001650: 2020 2073 656c 662e 6469 7669 6469 6e67     self.dividing
+00001660: 5f6b 6579 203d 2027 6469 7669 6469 6e67  _key = 'dividing
+00001670: 5f6e 6f72 6d61 6c27 0d0a 2020 2020 2020  _normal'..      
+00001680: 2020 7365 6c66 2e6e 756d 6265 725f 6469    self.number_di
+00001690: 7669 6469 6e67 5f6b 6579 203d 2027 6e75  viding_key = 'nu
+000016a0: 6d62 6572 5f64 6976 6964 696e 6727 0d0a  mber_dividing'..
+000016b0: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
+000016c0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
+000016d0: 6b65 7920 3d20 2764 6973 7461 6e63 655f  key = 'distance_
+000016e0: 6365 6c6c 5f6d 6173 6b27 0d0a 2020 2020  cell_mask'..    
+000016f0: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
+00001700: 7472 6f69 645f 785f 6b65 7920 3d20 276d  troid_x_key = 'm
+00001710: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
+00001720: 7927 0d0a 2020 2020 2020 2020 7365 6c66  y'..        self
+00001730: 2e6d 6173 6b63 656e 7472 6f69 645f 7a5f  .maskcentroid_z_
+00001740: 6b65 7920 3d20 276d 6173 6b63 656e 7472  key = 'maskcentr
+00001750: 6f69 645f 7a5f 6b65 7927 0d0a 2020 2020  oid_z_key'..    
+00001760: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
+00001770: 7472 6f69 645f 795f 6b65 7920 3d20 276d  troid_y_key = 'm
+00001780: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
+00001790: 7927 0d0a 2020 2020 2020 2020 7365 6c66  y'..        self
+000017a0: 2e63 656c 6c61 7869 735f 6d61 736b 5f6b  .cellaxis_mask_k
+000017b0: 6579 203d 2027 6365 6c6c 6178 6973 5f6d  ey = 'cellaxis_m
+000017c0: 6173 6b5f 6b65 7927 0d0a 2020 2020 2020  ask_key'..      
+000017d0: 2020 7365 6c66 2e63 656c 6c69 645f 6b65    self.cellid_ke
+000017e0: 7920 3d20 2763 656c 6c5f 6964 270d 0a20  y = 'cell_id'.. 
+000017f0: 2020 2020 2020 2073 656c 662e 6163 6365         self.acce
+00001800: 6c65 7261 7469 6f6e 5f6b 6579 203d 2027  leration_key = '
+00001810: 6163 6365 6c65 7261 7469 6f6e 270d 0a20  acceleration'.. 
+00001820: 2020 2020 2020 2073 656c 662e 6365 6e74         self.cent
+00001830: 726f 6964 5f6b 6579 203d 2027 6365 6e74  roid_key = 'cent
+00001840: 726f 6964 270d 0a20 2020 2020 2020 2073  roid'..        s
+00001850: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
+00001860: 5f6b 6579 203d 2027 636c 7573 7465 725f  _key = 'cluster_
+00001870: 636c 6173 7327 0d0a 2020 2020 2020 2020  class'..        
+00001880: 7365 6c66 2e63 6c75 7374 6572 7363 6f72  self.clusterscor
+00001890: 655f 6b65 7920 3d20 2763 6c75 7374 6572  e_key = 'cluster
+000018a0: 5f73 636f 7265 270d 0a20 2020 2020 2020  _score'..       
+000018b0: 2073 656c 662e 6563 6365 6e74 7269 6369   self.eccentrici
+000018c0: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
+000018d0: 203d 2027 636c 6f75 645f 6563 6365 6e74   = 'cloud_eccent
+000018e0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+000018f0: 7427 0d0a 2020 2020 2020 2020 7365 6c66  t'..        self
+00001900: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+00001910: 6d70 5f73 6563 6f6e 646b 6579 203d 2027  mp_secondkey = '
+00001920: 636c 6f75 645f 6563 6365 6e74 7269 6369  cloud_eccentrici
+00001930: 7479 5f63 6f6d 705f 7365 636f 6e64 270d  ty_comp_second'.
+00001940: 0a20 2020 2020 2020 2073 656c 662e 7375  .        self.su
+00001950: 7266 6163 655f 6172 6561 5f6b 6579 203d  rface_area_key =
+00001960: 2027 636c 6f75 645f 7375 7266 6163 6561   'cloud_surfacea
+00001970: 7265 6127 0d0a 2020 2020 2020 2020 7365  rea'..        se
+00001980: 6c66 2e72 6164 6961 6c5f 616e 676c 655f  lf.radial_angle_
+00001990: 6b65 7920 3d20 2772 6164 6961 6c5f 616e  key = 'radial_an
+000019a0: 676c 655f 6b65 7927 0d0a 2020 2020 2020  gle_key'..      
+000019b0: 2020 7365 6c66 2e6d 6f74 696f 6e5f 616e    self.motion_an
+000019c0: 676c 655f 6b65 7920 3d20 276d 6f74 696f  gle_key = 'motio
+000019d0: 6e5f 616e 676c 6527 200d 0a0d 0a20 2020  n_angle' ....   
+000019e0: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
+000019f0: 6e74 656e 7369 7479 5f63 6831 5f6b 6579  ntensity_ch1_key
+00001a00: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
+00001a10: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00001a20: 5b22 6d65 616e 5f69 6e74 656e 7369 7479  ["mean_intensity
+00001a30: 5f63 6831 225d 0d0a 2020 2020 2020 2020  _ch1"]..        
+00001a40: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+00001a50: 6974 795f 6368 325f 6b65 7920 3d20 7365  ity_ch2_key = se
+00001a60: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
+00001a70: 735f 7370 6f74 5f6b 6579 735b 226d 6561  s_spot_keys["mea
+00001a80: 6e5f 696e 7465 6e73 6974 795f 6368 3222  n_intensity_ch2"
+00001a90: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+00001aa0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+00001ab0: 6368 315f 6b65 7920 3d20 7365 6c66 2e74  ch1_key = self.t
+00001ac0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00001ad0: 6f74 5f6b 6579 735b 2274 6f74 616c 5f69  ot_keys["total_i
+00001ae0: 6e74 656e 7369 7479 5f63 6831 225d 0d0a  ntensity_ch1"]..
+00001af0: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+00001b00: 616c 5f69 6e74 656e 7369 7479 5f63 6832  al_intensity_ch2
+00001b10: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
+00001b20: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+00001b30: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
+00001b40: 6e73 6974 795f 6368 3222 5d0d 0a0d 0a20  nsity_ch2"].... 
+00001b50: 2020 2020 2020 2073 656c 662e 6d65 616e         self.mean
+00001b60: 5f69 6e74 656e 7369 7479 5f6b 6579 203d  _intensity_key =
+00001b70: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001b80: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00001b90: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
+00001ba0: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00001bb0: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
+00001bc0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
+00001bd0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00001be0: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
+00001bf0: 6974 7922 5d0d 0a0d 0a20 2020 2020 2020  ity"]....       
+00001c00: 2073 656c 662e 7370 6f74 5f73 6f75 7263   self.spot_sourc
+00001c10: 655f 6964 5f6b 6579 203d 2073 656c 662e  e_id_key = self.
+00001c20: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
+00001c30: 6467 6573 5f6b 6579 735b 2273 706f 745f  dges_keys["spot_
+00001c40: 736f 7572 6365 5f69 6422 5d0d 0a20 2020  source_id"]..   
+00001c50: 2020 2020 2073 656c 662e 7370 6f74 5f74       self.spot_t
+00001c60: 6172 6765 745f 6964 5f6b 6579 203d 2073  arget_id_key = s
+00001c70: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001c80: 6973 5f65 6467 6573 5f6b 6579 735b 2273  is_edges_keys["s
+00001c90: 706f 745f 7461 7267 6574 5f69 6422 5d0d  pot_target_id"].
+00001ca0: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
+00001cb0: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+00001cc0: 2e73 7065 6564 5f6b 6579 203d 2073 656c  .speed_key = sel
+00001cd0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
+00001ce0: 5f65 6467 6573 5f6b 6579 735b 2273 7065  _edges_keys["spe
+00001cf0: 6564 225d 0d0a 2020 2020 2020 2020 7365  ed"]..        se
+00001d00: 6c66 2e64 6973 706c 6163 656d 656e 745f  lf.displacement_
+00001d10: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
+00001d20: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
+00001d30: 6b65 7973 5b22 6469 7370 6c61 6365 6d65  keys["displaceme
+00001d40: 6e74 225d 0d0a 2020 2020 2020 2020 7365  nt"]..        se
+00001d50: 6c66 2e65 6467 655f 7469 6d65 5f6b 6579  lf.edge_time_key
+00001d60: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
+00001d70: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
+00001d80: 735b 2265 6467 655f 7469 6d65 225d 0d0a  s["edge_time"]..
+00001d90: 2020 2020 2020 2020 7365 6c66 2e65 6467          self.edg
+00001da0: 655f 785f 6c6f 6361 7469 6f6e 5f6b 6579  e_x_location_key
+00001db0: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
+00001dc0: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
+00001dd0: 735b 2265 6467 655f 785f 6c6f 6361 7469  s["edge_x_locati
+00001de0: 6f6e 225d 0d0a 2020 2020 2020 2020 7365  on"]..        se
+00001df0: 6c66 2e65 6467 655f 795f 6c6f 6361 7469  lf.edge_y_locati
+00001e00: 6f6e 5f6b 6579 203d 2073 656c 662e 7472  on_key = self.tr
+00001e10: 6163 6b5f 616e 616c 7973 6973 5f65 6467  ack_analysis_edg
+00001e20: 6573 5f6b 6579 735b 2265 6467 655f 795f  es_keys["edge_y_
+00001e30: 6c6f 6361 7469 6f6e 225d 0d0a 2020 2020  location"]..    
+00001e40: 2020 2020 7365 6c66 2e65 6467 655f 7a5f      self.edge_z_
+00001e50: 6c6f 6361 7469 6f6e 5f6b 6579 203d 2073  location_key = s
+00001e60: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001e70: 6973 5f65 6467 6573 5f6b 6579 735b 2265  is_edges_keys["e
+00001e80: 6467 655f 7a5f 6c6f 6361 7469 6f6e 225d  dge_z_location"]
+00001e90: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00001ea0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00001eb0: 7472 6163 6b73 203d 207b 7d0d 0a20 2020  tracks = {}..   
+00001ec0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00001ed0: 5f74 7261 636b 5f6d 6974 6f73 6973 5f6c  _track_mitosis_l
+00001ee0: 6162 656c 203d 207b 7d0d 0a20 2020 2020  abel = {}..     
+00001ef0: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
+00001f00: 7261 636b 5f70 726f 7065 7274 6965 7320  rack_properties 
+00001f10: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
+00001f20: 6c66 2e75 6e69 7175 655f 6666 745f 7072  lf.unique_fft_pr
+00001f30: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
+00001f40: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00001f50: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
+00001f60: 7274 6965 7320 3d20 7b7d 0d0a 2020 2020  rties = {}..    
+00001f70: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00001f80: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
+00001f90: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
+00001fa0: 656c 662e 756e 6971 7565 5f64 796e 616d  elf.unique_dynam
+00001fb0: 6963 5f70 726f 7065 7274 6965 7320 3d20  ic_properties = 
+00001fc0: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
+00001fd0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00001fe0: 7065 7274 6965 7320 3d20 7b7d 0d0a 2020  perties = {}..  
+00001ff0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00002000: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
+00002010: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
+00002020: 6c66 2e75 6e69 7175 655f 7472 6163 6b5f  lf.unique_track_
+00002030: 6365 6e74 726f 6964 203d 207b 7d0d 0a20  centroid = {}.. 
+00002040: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
+00002050: 5f73 706f 7473 203d 207b 7d0d 0a20 2020  _spots = {}..   
+00002060: 2020 2020 2073 656c 662e 616c 6c5f 6375       self.all_cu
+00002070: 7272 656e 745f 6365 6c6c 5f69 6473 203d  rrent_cell_ids =
+00002080: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
+00002090: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+000020a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000020b0: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
+000020c0: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
+000020d0: 6c6f 6f6b 7570 203d 207b 7d0d 0a20 2020  lookup = {}..   
+000020e0: 2020 2020 2073 656c 662e 6564 6765 5f73       self.edge_s
+000020f0: 6f75 7263 655f 6c6f 6f6b 7570 203d 207b  ource_lookup = {
+00002100: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+00002110: 6765 6e65 7261 7469 6f6e 5f64 6963 7420  generation_dict 
+00002120: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
+00002130: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
+00002140: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
+00002150: 656c 662e 6772 6170 685f 7370 6c69 7420  elf.graph_split 
+00002160: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
+00002170: 6c66 2e67 7261 7068 5f74 7261 636b 7320  lf.graph_tracks 
+00002180: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
+00002190: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
+000021a0: 6964 203d 207b 7d0d 0a20 2020 2020 2020  id = {}..       
+000021b0: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
+000021c0: 0a20 2020 2020 2020 2078 6d6c 5f70 6172  .        xml_par
+000021d0: 7365 7220 3d20 6574 2e58 4d4c 5061 7273  ser = et.XMLPars
+000021e0: 6572 2868 7567 655f 7472 6565 3d54 7275  er(huge_tree=Tru
+000021f0: 6529 0d0a 2020 2020 2020 2020 6966 2073  e)..        if s
+00002200: 656c 662e 6d61 7374 6572 5f78 6d6c 5f70  elf.master_xml_p
+00002210: 6174 6820 6973 204e 6f6e 653a 0d0a 2020  ath is None:..  
+00002220: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002230: 662e 6d61 7374 6572 5f78 6d6c 5f70 6174  f.master_xml_pat
+00002240: 6820 3d20 5061 7468 2827 2e27 290d 0a20  h = Path('.').. 
+00002250: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002260: 2069 6620 7365 6c66 2e6d 6173 7465 725f   if self.master_
+00002270: 786d 6c5f 7061 7468 2e69 735f 6469 7228  xml_path.is_dir(
+00002280: 2920 616e 6420 7365 6c66 2e78 6d6c 5f70  ) and self.xml_p
+00002290: 6174 6820 6973 206e 6f74 204e 6f6e 653a  ath is not None:
+000022a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000022b0: 2020 7072 696e 7428 2752 6561 6469 6e67    print('Reading
+000022c0: 2058 4d4c 2729 0d0a 2020 2020 2020 2020   XML')..        
+000022d0: 2020 2020 2020 2020 7365 6c66 2e78 6d6c          self.xml
+000022e0: 5f63 6f6e 7465 6e74 203d 2065 742e 6672  _content = et.fr
+000022f0: 6f6d 7374 7269 6e67 286f 7065 6e28 7365  omstring(open(se
+00002300: 6c66 2e78 6d6c 5f70 6174 6829 2e72 6561  lf.xml_path).rea
+00002310: 6428 292e 656e 636f 6465 2829 2c20 786d  d().encode(), xm
+00002320: 6c5f 7061 7273 6572 290d 0a20 2020 2020  l_parser)..     
+00002330: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00002340: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002350: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
+00002360: 5f69 6473 203d 205b 0d0a 2020 2020 2020  _ids = [..      
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 696e 7428 7472 6163 6b2e        int(track.
+00002390: 6765 7428 7365 6c66 2e74 7261 636b 6964  get(self.trackid
+000023a0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
+000023d0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
+000023e0: 742e 6669 6e64 2822 4d6f 6465 6c22 290d  t.find("Model").
+000023f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002400: 2020 2020 2020 2020 2020 2020 202e 6669               .fi
+00002410: 6e64 2822 4669 6c74 6572 6564 5472 6163  nd("FilteredTrac
+00002420: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
+00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002440: 2020 2e66 696e 6461 6c6c 2822 5472 6163    .findall("Trac
+00002450: 6b49 4422 290d 0a20 2020 2020 2020 2020  kID")..         
+00002460: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00002470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002480: 2020 7365 6c66 2e6d 6178 5f74 7261 636b    self.max_track
+00002490: 5f69 6420 3d20 6d61 7828 7365 6c66 2e66  _id = max(self.f
+000024a0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+000024b0: 7329 2020 2020 2020 2020 0d0a 2020 2020  s)        ..    
+000024c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000024d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000024e0: 6c66 2e5f 6765 745f 786d 6c5f 6461 7461  lf._get_xml_data
+000024f0: 2829 0d0a 2020 2020 2020 2020 6966 206e  ()..        if n
+00002500: 6f74 2069 7369 6e73 7461 6e63 6528 7365  ot isinstance(se
+00002510: 6c66 2e6d 6173 7465 725f 786d 6c5f 7061  lf.master_xml_pa
+00002520: 7468 2c20 7374 7229 3a20 2020 2020 200d  th, str):      .
+00002530: 0a20 2020 2020 2020 2020 2069 6620 7365  .          if se
+00002540: 6c66 2e6d 6173 7465 725f 786d 6c5f 7061  lf.master_xml_pa
+00002550: 7468 2e69 735f 6669 6c65 2829 3a0d 0a20  th.is_file():.. 
+00002560: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00002570: 696e 7428 2752 6561 6469 6e67 204d 6173  int('Reading Mas
+00002580: 7465 7220 584d 4c27 290d 0a20 2020 2020  ter XML')..     
+00002590: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000025a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000025b0: 786d 6c5f 636f 6e74 656e 7420 3d20 6574  xml_content = et
+000025c0: 2e66 726f 6d73 7472 696e 6728 6f70 656e  .fromstring(open
+000025d0: 2873 656c 662e 6d61 7374 6572 5f78 6d6c  (self.master_xml
+000025e0: 5f70 6174 6829 2e72 6561 6428 292e 656e  _path).read().en
+000025f0: 636f 6465 2829 2c20 786d 6c5f 7061 7273  code(), xml_pars
+00002600: 6572 290d 0a20 2020 2020 2020 2020 2020  er)..           
+00002610: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00002620: 2020 2020 2073 656c 662e 6669 6c74 6572       self.filter
+00002630: 6564 5f74 7261 636b 5f69 6473 203d 205b  ed_track_ids = [
+00002640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002650: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00002660: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
+00002670: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
+00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002690: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000026a0: 7472 6163 6b20 696e 2073 656c 662e 786d  track in self.xm
+000026b0: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
+000026c0: 4d6f 6465 6c22 290d 0a20 2020 2020 2020  Model")..       
+000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026e0: 2020 2020 202e 6669 6e64 2822 4669 6c74       .find("Filt
+000026f0: 6572 6564 5472 6163 6b73 2229 0d0a 2020  eredTracks")..  
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 2020 2020 2020 2020 2e66 696e 6461            .finda
+00002720: 6c6c 2822 5472 6163 6b49 4422 290d 0a20  ll("TrackID").. 
+00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002740: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+00002750: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00002760: 785f 7472 6163 6b5f 6964 203d 206d 6178  x_track_id = max
+00002770: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
+00002780: 7261 636b 5f69 6473 2920 2020 2020 2020  rack_ids)       
+00002790: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000027a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000027b0: 2020 2020 7365 6c66 2e5f 6765 745f 6d61      self._get_ma
+000027c0: 7374 6572 5f78 6d6c 5f64 6174 6128 290d  ster_xml_data().
+000027d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027e0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+000027f0: 200d 0a0d 0a0d 0a20 2020 2064 6566 205f   ......    def _
+00002800: 6372 6561 7465 5f63 6861 6e6e 656c 5f74  create_channel_t
+00002810: 7265 6528 7365 6c66 293a 0d0a 2020 2020  ree(self):..    
+00002820: 2020 2020 2020 7365 6c66 2e5f 7469 6d65        self._time
+00002830: 645f 6368 616e 6e65 6c5f 7365 675f 696d  d_channel_seg_im
+00002840: 6167 6520 3d20 7b7d 0d0a 2020 2020 2020  age = {}..      
+00002850: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+00002860: 2030 0d0a 2020 2020 2020 2020 2020 6675   0..          fu
+00002870: 7475 7265 7320 3d20 5b5d 0d0a 2020 2020  tures = []..    
+00002880: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
+00002890: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
+000028a0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
+000028b0: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
+000028c0: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
+000028d0: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
 000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002920: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00002930: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
-00002940: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00002950: 6f72 2072 2069 6e20 636f 6e63 7572 7265  or r in concurre
-00002960: 6e74 2e66 7574 7572 6573 2e61 735f 636f  nt.futures.as_co
-00002970: 6d70 6c65 7465 6428 6675 7475 7265 7329  mpleted(futures)
-00002980: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029a0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
-000029b0: 7420 3d20 7365 6c66 2e63 6f75 6e74 202b  t = self.count +
-000029c0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000029f0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
-00002a00: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a30: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00002a40: 6172 2e76 616c 7565 203d 2020 7365 6c66  ar.value =  self
-00002a50: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 2020 2020 2020 722e 7265              r.re
-00002a80: 7375 6c74 2829 0d0a 0d0a 200d 0a0d 0a20  sult().... .... 
-00002a90: 2020 2064 6566 205f 6368 616e 6e65 6c5f     def _channel_
-00002aa0: 636f 6d70 7574 6572 2873 656c 662c 2069  computer(self, i
-00002ab0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00002ac0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00002ad0: 2020 2020 2020 6966 2073 656c 662e 696d        if self.im
-00002ae0: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
-00002af0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002b00: 2020 2020 2020 2020 2020 696e 7465 6e73            intens
-00002b10: 6974 795f 696d 6167 6520 3d20 7365 6c66  ity_image = self
-00002b20: 2e69 6d61 6765 0d0a 2020 2020 2020 2020  .image..        
-00002b30: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2020 2020 2020 2069 6e74 656e 7369 7479         intensity
-00002b60: 5f69 6d61 6765 203d 2073 656c 662e 6368  _image = self.ch
-00002b70: 616e 6e65 6c5f 7365 675f 696d 6167 650d  annel_seg_image.
-00002b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b90: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00002ba0: 2020 2070 726f 7065 7274 6965 7320 3d20     properties = 
-00002bb0: 7265 6769 6f6e 7072 6f70 7328 7365 6c66  regionprops(self
-00002bc0: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
-00002bd0: 6765 5b69 2c3a 5d2c 2069 6e74 656e 7369  ge[i,:], intensi
-00002be0: 7479 5f69 6d61 6765 5b69 2c3a 5d29 0d0a  ty_image[i,:])..
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 6365 6e74 726f 6964 7320 3d20 5b70 726f  centroids = [pro
-00002c10: 702e 6365 6e74 726f 6964 2066 6f72 2070  p.centroid for p
-00002c20: 726f 7020 696e 2070 726f 7065 7274 6965  rop in propertie
-00002c30: 735d 0d0a 2020 2020 2020 2020 2020 2020  s]..            
-00002c40: 2020 2020 6c61 6265 6c73 203d 205b 7072      labels = [pr
-00002c50: 6f70 2e6c 6162 656c 2066 6f72 2070 726f  op.label for pro
-00002c60: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
-00002c70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002c80: 2020 766f 6c75 6d65 203d 205b 7072 6f70    volume = [prop
-00002c90: 2e61 7265 6120 666f 7220 7072 6f70 2069  .area for prop i
-00002ca0: 6e20 7072 6f70 6572 7469 6573 5d0d 0a20  n properties].. 
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002cc0: 6e74 656e 7369 7479 5f6d 6561 6e20 3d20  ntensity_mean = 
-00002cd0: 5b70 726f 702e 696e 7465 6e73 6974 795f  [prop.intensity_
-00002ce0: 6d65 616e 2066 6f72 2070 726f 7020 696e  mean for prop in
-00002cf0: 2070 726f 7065 7274 6965 735d 0d0a 2020   properties]..  
-00002d00: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00002d10: 7465 6e73 6974 795f 746f 7461 6c20 3d20  tensity_total = 
-00002d20: 5b70 726f 702e 696e 7465 6e73 6974 795f  [prop.intensity_
-00002d30: 6d65 616e 202a 2070 726f 702e 6172 6561  mean * prop.area
-00002d40: 2066 6f72 2070 726f 7020 696e 2070 726f   for prop in pro
-00002d50: 7065 7274 6965 735d 0d0a 2020 2020 2020  perties]..      
-00002d60: 2020 2020 2020 2020 2020 626f 756e 6469            boundi
-00002d70: 6e67 5f62 6f78 6573 203d 205b 7072 6f70  ng_boxes = [prop
-00002d80: 2e62 626f 7820 666f 7220 7072 6f70 2069  .bbox for prop i
-00002d90: 6e20 7072 6f70 6572 7469 6573 5d0d 0a0d  n properties]...
-00002da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002db0: 2074 7265 6520 3d20 7370 6174 6961 6c2e   tree = spatial.
-00002dc0: 634b 4454 7265 6528 6365 6e74 726f 6964  cKDTree(centroid
-00002dd0: 7329 0d0a 0d0a 2020 2020 2020 2020 2020  s)....          
-00002de0: 2020 2020 2020 7365 6c66 2e5f 7469 6d65        self._time
-00002df0: 645f 6368 616e 6e65 6c5f 7365 675f 696d  d_channel_seg_im
-00002e00: 6167 655b 7374 7228 6929 5d20 3d20 2074  age[str(i)] =  t
-00002e10: 7265 652c 2063 656e 7472 6f69 6473 2c20  ree, centroids, 
-00002e20: 6c61 6265 6c73 2c20 766f 6c75 6d65 2c20  labels, volume, 
-00002e30: 696e 7465 6e73 6974 795f 6d65 616e 2c20  intensity_mean, 
-00002e40: 696e 7465 6e73 6974 795f 746f 7461 6c2c  intensity_total,
-00002e50: 2062 6f75 6e64 696e 675f 626f 7865 730d   bounding_boxes.
-00002e60: 0a20 2020 2020 2020 2020 200d 0a0d 0a20  .          .... 
-00002e70: 2020 2064 6566 205f 6765 745f 6174 7472     def _get_attr
-00002e80: 6962 7574 6573 2873 656c 6629 3a0d 0a20  ibutes(self):.. 
-00002e90: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00002ea0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-00002eb0: 7474 7269 6275 7465 6964 732c 2073 656c  ttributeids, sel
-00002ec0: 662e 416c 6c56 616c 7565 7320 3d20 2067  f.AllValues =  g
-00002ed0: 6574 5f73 706f 745f 6461 7461 7365 7428  et_spot_dataset(
-00002ee0: 7365 6c66 2e73 706f 745f 6461 7461 7365  self.spot_datase
-00002ef0: 742c 2073 656c 662e 7472 6163 6b5f 616e  t, self.track_an
-00002f00: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00002f10: 2c20 7365 6c66 2e78 6361 6c69 6272 6174  , self.xcalibrat
-00002f20: 696f 6e2c 2073 656c 662e 7963 616c 6962  ion, self.ycalib
-00002f30: 7261 7469 6f6e 2c20 7365 6c66 2e7a 6361  ration, self.zca
-00002f40: 6c69 6272 6174 696f 6e2c 2073 656c 662e  libration, self.
-00002f50: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
-00002f60: 2c20 7365 6c66 2e64 6574 6563 746f 7263  , self.detectorc
-00002f70: 6861 6e6e 656c 290d 0a20 2020 2020 2020  hannel)..       
-00002f80: 2020 2020 2020 7072 696e 7428 276f 6274        print('obt
-00002f90: 6961 6e65 6420 7370 6f74 2061 7474 7269  ianed spot attri
-00002fa0: 6275 7465 7327 290d 0a20 2020 2020 2020  butes')..       
-00002fb0: 2020 2020 2020 7365 6c66 2e54 7261 636b        self.Track
-00002fc0: 4174 7472 6962 7574 6569 6473 2c20 7365  Attributeids, se
-00002fd0: 6c66 2e41 6c6c 5472 6163 6b56 616c 7565  lf.AllTrackValue
-00002fe0: 7320 3d20 6765 745f 7472 6163 6b5f 6461  s = get_track_da
-00002ff0: 7461 7365 7428 7365 6c66 2e74 7261 636b  taset(self.track
-00003000: 5f64 6174 6173 6574 2c20 2073 656c 662e  _dataset,  self.
-00003010: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-00003020: 706f 745f 6b65 7973 2c20 7365 6c66 2e74  pot_keys, self.t
-00003030: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
-00003040: 6163 6b5f 6b65 7973 2c20 7365 6c66 2e54  ack_keys, self.T
-00003050: 7261 636b 4174 7472 6962 7574 6542 6f78  rackAttributeBox
-00003060: 6e61 6d65 290d 0a20 2020 2020 2020 2020  name)..         
-00003070: 2020 2020 7072 696e 7428 276f 6274 6169      print('obtai
-00003080: 6e65 6420 7472 6163 6b20 6174 7472 6962  ned track attrib
-00003090: 7574 6573 2729 0d0a 2020 2020 2020 2020  utes')..        
-000030a0: 2020 2020 2073 656c 662e 416c 6c45 6467       self.AllEdg
-000030b0: 6573 5661 6c75 6573 203d 2067 6574 5f65  esValues = get_e
-000030c0: 6467 6573 5f64 6174 6173 6574 2873 656c  dges_dataset(sel
-000030d0: 662e 6564 6765 735f 6461 7461 7365 742c  f.edges_dataset,
-000030e0: 2073 656c 662e 6564 6765 735f 6461 7461   self.edges_data
-000030f0: 7365 745f 696e 6465 782c 2073 656c 662e  set_index, self.
+000028f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00002900: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
+00002910: 5f69 6d61 6765 2e73 6861 7065 5b30 5d29  _image.shape[0])
+00002920: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002930: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+00002940: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
+00002950: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
+00002960: 6368 616e 6e65 6c5f 636f 6d70 7574 6572  channel_computer
+00002970: 2c20 6929 290d 0a20 2020 2020 2020 2020  , i))..         
+00002980: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00002990: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+000029a0: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+000029b0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a00: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00002a10: 6172 2e6c 6162 656c 203d 2022 446f 696e  ar.label = "Doin
+00002a20: 6720 6368 616e 6e65 6c20 636f 6d70 7574  g channel comput
+00002a30: 6174 696f 6e22 0d0a 2020 2020 2020 2020  ation"..        
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002a60: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
+00002a70: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002aa0: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ac0: 2020 2020 2020 2020 2020 2020 206c 656e               len
+00002ad0: 2866 7574 7572 6573 292c 0d0a 2020 2020  (futures),..    
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b20: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+00002b30: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
+00002b40: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00002b50: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
+00002b60: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+00002b70: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
+00002b80: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002bb0: 656c 662e 636f 756e 7420 3d20 7365 6c66  elf.count = self
+00002bc0: 2e63 6f75 6e74 202b 2031 0d0a 2020 2020  .count + 1..    
+00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
+00002c00: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
+00002c10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00002c40: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+00002c50: 203d 2020 7365 6c66 2e63 6f75 6e74 0d0a   =  self.count..
+00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 2020 2020 722e 7265 7375 6c74 2829 0d0a      r.result()..
+00002c90: 0d0a 200d 0a0d 0a20 2020 2064 6566 205f  .. ....    def _
+00002ca0: 6368 616e 6e65 6c5f 636f 6d70 7574 6572  channel_computer
+00002cb0: 2873 656c 662c 2069 293a 0d0a 2020 2020  (self, i):..    
+00002cc0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002ce0: 2073 656c 662e 696d 6167 6520 6973 206e   self.image is n
+00002cf0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d10: 2020 696e 7465 6e73 6974 795f 696d 6167    intensity_imag
+00002d20: 6520 3d20 7365 6c66 2e69 6d61 6765 0d0a  e = self.image..
+00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d40: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00002d50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002d60: 6e74 656e 7369 7479 5f69 6d61 6765 203d  ntensity_image =
+00002d70: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+00002d80: 675f 696d 6167 650d 0a20 2020 2020 2020  g_image..       
+00002d90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00002da0: 2020 2020 2020 2020 2020 2070 726f 7065             prope
+00002db0: 7274 6965 7320 3d20 7265 6769 6f6e 7072  rties = regionpr
+00002dc0: 6f70 7328 7365 6c66 2e63 6861 6e6e 656c  ops(self.channel
+00002dd0: 5f73 6567 5f69 6d61 6765 5b69 2c3a 5d2c  _seg_image[i,:],
+00002de0: 2069 6e74 656e 7369 7479 5f69 6d61 6765   intensity_image
+00002df0: 5b69 2c3a 5d29 0d0a 2020 2020 2020 2020  [i,:])..        
+00002e00: 2020 2020 2020 2020 6365 6e74 726f 6964          centroid
+00002e10: 7320 3d20 5b70 726f 702e 6365 6e74 726f  s = [prop.centro
+00002e20: 6964 2066 6f72 2070 726f 7020 696e 2070  id for prop in p
+00002e30: 726f 7065 7274 6965 735d 0d0a 2020 2020  roperties]..    
+00002e40: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00002e50: 6c73 203d 205b 7072 6f70 2e6c 6162 656c  ls = [prop.label
+00002e60: 2066 6f72 2070 726f 7020 696e 2070 726f   for prop in pro
+00002e70: 7065 7274 6965 735d 0d0a 2020 2020 2020  perties]..      
+00002e80: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
+00002e90: 203d 205b 7072 6f70 2e61 7265 6120 666f   = [prop.area fo
+00002ea0: 7220 7072 6f70 2069 6e20 7072 6f70 6572  r prop in proper
+00002eb0: 7469 6573 5d0d 0a20 2020 2020 2020 2020  ties]..         
+00002ec0: 2020 2020 2020 2069 6e74 656e 7369 7479         intensity
+00002ed0: 5f6d 6561 6e20 3d20 5b70 726f 702e 696e  _mean = [prop.in
+00002ee0: 7465 6e73 6974 795f 6d65 616e 2066 6f72  tensity_mean for
+00002ef0: 2070 726f 7020 696e 2070 726f 7065 7274   prop in propert
+00002f00: 6965 735d 0d0a 2020 2020 2020 2020 2020  ies]..          
+00002f10: 2020 2020 2020 696e 7465 6e73 6974 795f        intensity_
+00002f20: 746f 7461 6c20 3d20 5b70 726f 702e 696e  total = [prop.in
+00002f30: 7465 6e73 6974 795f 6d65 616e 202a 2070  tensity_mean * p
+00002f40: 726f 702e 6172 6561 2066 6f72 2070 726f  rop.area for pro
+00002f50: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
+00002f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002f70: 2020 626f 756e 6469 6e67 5f62 6f78 6573    bounding_boxes
+00002f80: 203d 205b 7072 6f70 2e62 626f 7820 666f   = [prop.bbox fo
+00002f90: 7220 7072 6f70 2069 6e20 7072 6f70 6572  r prop in proper
+00002fa0: 7469 6573 5d0d 0a0d 0a20 2020 2020 2020  ties]....       
+00002fb0: 2020 2020 2020 2020 2074 7265 6520 3d20           tree = 
+00002fc0: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
+00002fd0: 6365 6e74 726f 6964 7329 0d0a 0d0a 2020  centroids)....  
+00002fe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00002ff0: 6c66 2e5f 7469 6d65 645f 6368 616e 6e65  lf._timed_channe
+00003000: 6c5f 7365 675f 696d 6167 655b 7374 7228  l_seg_image[str(
+00003010: 6929 5d20 3d20 2074 7265 652c 2063 656e  i)] =  tree, cen
+00003020: 7472 6f69 6473 2c20 6c61 6265 6c73 2c20  troids, labels, 
+00003030: 766f 6c75 6d65 2c20 696e 7465 6e73 6974  volume, intensit
+00003040: 795f 6d65 616e 2c20 696e 7465 6e73 6974  y_mean, intensit
+00003050: 795f 746f 7461 6c2c 2062 6f75 6e64 696e  y_total, boundin
+00003060: 675f 626f 7865 730d 0a20 2020 2020 2020  g_boxes..       
+00003070: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
+00003080: 6765 745f 6174 7472 6962 7574 6573 2873  get_attributes(s
+00003090: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
+000030a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000030b0: 2020 7365 6c66 2e41 7474 7269 6275 7465    self.Attribute
+000030c0: 6964 732c 2073 656c 662e 416c 6c56 616c  ids, self.AllVal
+000030d0: 7565 7320 3d20 2067 6574 5f73 706f 745f  ues =  get_spot_
+000030e0: 6461 7461 7365 7428 7365 6c66 2e73 706f  dataset(self.spo
+000030f0: 745f 6461 7461 7365 742c 2073 656c 662e  t_dataset, self.
 00003100: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-00003110: 706f 745f 6b65 7973 2c20 7365 6c66 2e74  pot_keys, self.t
-00003120: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
-00003130: 6765 735f 6b65 7973 290d 0a20 2020 2020  ges_keys)..     
-00003140: 2020 2020 2020 2020 7072 696e 7428 276f          print('o
-00003150: 6274 6169 6e65 6420 6564 6765 2061 7474  btained edge att
-00003160: 7269 6275 7465 7327 290d 0a0d 0a20 2020  ributes')....   
-00003170: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00003180: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-00003190: 205f 6765 745f 626f 756e 6461 7279 5f70   _get_boundary_p
-000031a0: 6f69 6e74 7328 7365 6c66 293a 0d0a 2020  oints(self):..  
-000031b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000031c0: 2070 7269 6e74 2827 436f 6d70 7574 696e   print('Computin
-000031d0: 6720 626f 756e 6461 7279 2070 6f69 6e74  g boundary point
-000031e0: 7327 2920 0d0a 2020 2020 2020 2020 6966  s') ..        if
-000031f0: 2020 7365 6c66 2e6d 6173 6b20 6973 206e    self.mask is n
-00003200: 6f74 204e 6f6e 653a 0d0a 0d0a 2020 2020  ot None:....    
-00003210: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003220: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
-00003230: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
-00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00003260: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00003270: 7064 6174 655f 6d61 736b 203d 2063 6865  pdate_mask = che
-00003280: 636b 5f61 6e64 5f75 7064 6174 655f 6d61  ck_and_update_ma
-00003290: 736b 2873 656c 662e 6d61 736b 2c20 7365  sk(self.mask, se
-000032a0: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
-000032b0: 6d61 6765 290d 0a0d 0a20 2020 2020 2020  mage)....       
-000032c0: 2020 2020 2069 6620 7365 6c66 2e73 6567       if self.seg
-000032d0: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
-000032e0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000032f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003310: 2020 2073 656c 662e 7570 6461 7465 5f6d     self.update_m
-00003320: 6173 6b20 3d20 6368 6563 6b5f 616e 645f  ask = check_and_
-00003330: 7570 6461 7465 5f6d 6173 6b28 7365 6c66  update_mask(self
-00003340: 2e6d 6173 6b2c 2073 656c 662e 7365 675f  .mask, self.seg_
-00003350: 696d 6167 6529 0d0a 2020 2020 2020 2020  image)..        
-00003360: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00003370: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00003380: 656c 662e 7365 675f 696d 6167 6520 6973  elf.seg_image is
-00003390: 204e 6f6e 6520 616e 6420 7365 6c66 2e69   None and self.i
-000033a0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-000033b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000033c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033e0: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
-000033f0: 5f6d 6173 6b20 3d20 6368 6563 6b5f 616e  _mask = check_an
-00003400: 645f 7570 6461 7465 5f6d 6173 6b28 7365  d_update_mask(se
-00003410: 6c66 2e6d 6173 6b2c 2073 656c 662e 696d  lf.mask, self.im
-00003420: 6167 6529 2020 2020 0d0a 2020 2020 2020  age)    ..      
-00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003440: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00003450: 2020 2073 656c 662e 6d61 736b 203d 2073     self.mask = s
-00003460: 656c 662e 7570 6461 7465 5f6d 6173 6b2e  elf.update_mask.
-00003470: 6173 7479 7065 2827 7569 6e74 3136 2729  astype('uint16')
-00003480: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00003490: 6c66 2e74 696d 6564 5f6d 6173 6b2c 2073  lf.timed_mask, s
-000034a0: 656c 662e 626f 756e 6461 7279 203d 2062  elf.boundary = b
-000034b0: 6f75 6e64 6172 795f 706f 696e 7473 2873  oundary_points(s
-000034c0: 656c 662e 6d61 736b 2c20 7365 6c66 2e78  elf.mask, self.x
-000034d0: 6361 6c69 6272 6174 696f 6e2c 2073 656c  calibration, sel
-000034e0: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
-000034f0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00003500: 6e29 0d0a 2020 2020 2020 2020 656c 6966  n)..        elif
-00003510: 2073 656c 662e 6d61 736b 2069 7320 4e6f   self.mask is No
-00003520: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00003530: 2069 6620 7365 6c66 2e73 6567 5f69 6d61   if self.seg_ima
-00003540: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
-00003550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003560: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00003570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003580: 7570 6461 7465 5f6d 6173 6b20 3d20 6e70  update_mask = np
-00003590: 2e7a 6572 6f73 2873 656c 662e 7365 675f  .zeros(self.seg_
-000035a0: 696d 6167 652e 7368 6170 6529 0d0a 2020  image.shape)..  
-000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000035d0: 2020 2020 6966 2073 656c 662e 7365 675f      if self.seg_
-000035e0: 696d 6167 6520 6973 204e 6f6e 6520 616e  image is None an
-000035f0: 6420 7365 6c66 2e69 6d61 6765 2069 7320  d self.image is 
-00003600: 6e6f 7420 4e6f 6e65 3a0d 0a0d 0a20 2020  not None:....   
-00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003620: 2073 656c 662e 7570 6461 7465 5f6d 6173   self.update_mas
-00003630: 6b20 3d20 6e70 2e7a 6572 6f73 2873 656c  k = np.zeros(sel
-00003640: 662e 696d 6167 652e 7368 6170 6529 200d  f.image.shape) .
-00003650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003660: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00003670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003680: 6d61 736b 203d 2073 656c 662e 7570 6461  mask = self.upda
-00003690: 7465 5f6d 6173 6b2e 6173 7479 7065 2827  te_mask.astype('
-000036a0: 7569 6e74 3136 2729 0d0a 2020 2020 2020  uint16')..      
-000036b0: 2020 2020 2020 7365 6c66 2e6d 6173 6b5b        self.mask[
-000036c0: 3a2c 3a2c 313a 2d31 2c31 3a2d 315d 203d  :,:,1:-1,1:-1] =
-000036d0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-000036e0: 7365 6c66 2e74 696d 6564 5f6d 6173 6b2c  self.timed_mask,
-000036f0: 2073 656c 662e 626f 756e 6461 7279 203d   self.boundary =
-00003700: 2062 6f75 6e64 6172 795f 706f 696e 7473   boundary_points
-00003710: 2873 656c 662e 6d61 736b 2c20 7365 6c66  (self.mask, self
-00003720: 2e78 6361 6c69 6272 6174 696f 6e2c 2073  .xcalibration, s
-00003730: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-00003740: 2c20 7365 6c66 2e7a 6361 6c69 6272 6174  , self.zcalibrat
-00003750: 696f 6e29 0d0a 0d0a 2020 2020 2020 2020  ion)....        
-00003760: 2020 0d0a 0d0a 0d0a 2020 2020 6465 6620    ......    def 
-00003770: 5f67 656e 6572 6174 655f 6765 6e65 7261  _generate_genera
-00003780: 7469 6f6e 7328 7365 6c66 2c20 7472 6163  tions(self, trac
-00003790: 6b29 3a0d 0a20 2020 2020 2020 2020 0d0a  k):..         ..
-000037a0: 2020 2020 2020 2020 616c 6c5f 736f 7572          all_sour
-000037b0: 6365 5f69 6473 203d 205b 5d0d 0a20 2020  ce_ids = []..   
-000037c0: 2020 2020 2061 6c6c 5f74 6172 6765 745f       all_target_
-000037d0: 6964 7320 3d20 5b5d 200d 0a0d 0a0d 0a20  ids = [] ...... 
-000037e0: 2020 2020 2020 2066 6f72 2065 6467 6520         for edge 
-000037f0: 696e 2074 7261 636b 2e66 696e 6461 6c6c  in track.findall
-00003800: 2827 4564 6765 2729 3a0d 0a0d 0a20 2020  ('Edge'):....   
-00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 2020 2020 2020 2020 2073 6f75 7263 655f           source_
-00003830: 6964 203d 2069 6e74 2865 6467 652e 6765  id = int(edge.ge
-00003840: 7428 7365 6c66 2e73 706f 745f 736f 7572  t(self.spot_sour
-00003850: 6365 5f69 645f 6b65 7929 290d 0a20 2020  ce_id_key))..   
+00003110: 706f 745f 6b65 7973 2c20 7365 6c66 2e78  pot_keys, self.x
+00003120: 6361 6c69 6272 6174 696f 6e2c 2073 656c  calibration, sel
+00003130: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
+00003140: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00003150: 6e2c 2073 656c 662e 4174 7472 6962 7574  n, self.Attribut
+00003160: 6542 6f78 6e61 6d65 2c20 7365 6c66 2e64  eBoxname, self.d
+00003170: 6574 6563 746f 7263 6861 6e6e 656c 290d  etectorchannel).
+00003180: 0a20 2020 2020 2020 2020 2020 2020 7072  .             pr
+00003190: 696e 7428 276f 6274 6961 6e65 6420 7370  int('obtianed sp
+000031a0: 6f74 2061 7474 7269 6275 7465 7327 290d  ot attributes').
+000031b0: 0a20 2020 2020 2020 2020 2020 2020 7365  .             se
+000031c0: 6c66 2e54 7261 636b 4174 7472 6962 7574  lf.TrackAttribut
+000031d0: 6569 6473 2c20 7365 6c66 2e41 6c6c 5472  eids, self.AllTr
+000031e0: 6163 6b56 616c 7565 7320 3d20 6765 745f  ackValues = get_
+000031f0: 7472 6163 6b5f 6461 7461 7365 7428 7365  track_dataset(se
+00003200: 6c66 2e74 7261 636b 5f64 6174 6173 6574  lf.track_dataset
+00003210: 2c20 2073 656c 662e 7472 6163 6b5f 616e  ,  self.track_an
+00003220: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00003230: 2c20 7365 6c66 2e74 7261 636b 5f61 6e61  , self.track_ana
+00003240: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
+00003250: 2c20 7365 6c66 2e54 7261 636b 4174 7472  , self.TrackAttr
+00003260: 6962 7574 6542 6f78 6e61 6d65 290d 0a20  ibuteBoxname).. 
+00003270: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00003280: 7428 276f 6274 6169 6e65 6420 7472 6163  t('obtained trac
+00003290: 6b20 6174 7472 6962 7574 6573 2729 0d0a  k attributes')..
+000032a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000032b0: 662e 416c 6c45 6467 6573 5661 6c75 6573  f.AllEdgesValues
+000032c0: 203d 2067 6574 5f65 6467 6573 5f64 6174   = get_edges_dat
+000032d0: 6173 6574 2873 656c 662e 6564 6765 735f  aset(self.edges_
+000032e0: 6461 7461 7365 742c 2073 656c 662e 6564  dataset, self.ed
+000032f0: 6765 735f 6461 7461 7365 745f 696e 6465  ges_dataset_inde
+00003300: 782c 2073 656c 662e 7472 6163 6b5f 616e  x, self.track_an
+00003310: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00003320: 2c20 7365 6c66 2e74 7261 636b 5f61 6e61  , self.track_ana
+00003330: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
+00003340: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003350: 7072 696e 7428 276f 6274 6169 6e65 6420  print('obtained 
+00003360: 6564 6765 2061 7474 7269 6275 7465 7327  edge attributes'
+00003370: 290d 0a0d 0a20 2020 200d 0a20 2020 2020  )....    ..     
+00003380: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00003390: 0a20 2020 2064 6566 205f 6765 745f 626f  .    def _get_bo
+000033a0: 756e 6461 7279 5f70 6f69 6e74 7328 7365  undary_points(se
+000033b0: 6c66 293a 0d0a 2020 2020 2020 2020 200d  lf):..         .
+000033c0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+000033d0: 436f 6d70 7574 696e 6720 626f 756e 6461  Computing bounda
+000033e0: 7279 2070 6f69 6e74 7327 2920 0d0a 2020  ry points') ..  
+000033f0: 2020 2020 2020 6966 2020 7365 6c66 2e6d        if  self.m
+00003400: 6173 6b20 6973 206e 6f74 204e 6f6e 653a  ask is not None:
+00003410: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00003420: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
+00003430: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
+00003440: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00003450: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003470: 2020 7365 6c66 2e75 7064 6174 655f 6d61    self.update_ma
+00003480: 736b 203d 2063 6865 636b 5f61 6e64 5f75  sk = check_and_u
+00003490: 7064 6174 655f 6d61 736b 2873 656c 662e  pdate_mask(self.
+000034a0: 6d61 736b 2c20 7365 6c66 2e63 6861 6e6e  mask, self.chann
+000034b0: 656c 5f73 6567 5f69 6d61 6765 290d 0a0d  el_seg_image)...
+000034c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000034d0: 7365 6c66 2e73 6567 5f69 6d61 6765 2069  self.seg_image i
+000034e0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003500: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00003510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003520: 7570 6461 7465 5f6d 6173 6b20 3d20 6368  update_mask = ch
+00003530: 6563 6b5f 616e 645f 7570 6461 7465 5f6d  eck_and_update_m
+00003540: 6173 6b28 7365 6c66 2e6d 6173 6b2c 2073  ask(self.mask, s
+00003550: 656c 662e 7365 675f 696d 6167 6529 0d0a  elf.seg_image)..
+00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003570: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003580: 2020 2020 6966 2073 656c 662e 7365 675f      if self.seg_
+00003590: 696d 6167 6520 6973 204e 6f6e 6520 616e  image is None an
+000035a0: 6420 7365 6c66 2e69 6d61 6765 2069 7320  d self.image is 
+000035b0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000035e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000035f0: 662e 7570 6461 7465 5f6d 6173 6b20 3d20  f.update_mask = 
+00003600: 6368 6563 6b5f 616e 645f 7570 6461 7465  check_and_update
+00003610: 5f6d 6173 6b28 7365 6c66 2e6d 6173 6b2c  _mask(self.mask,
+00003620: 2073 656c 662e 696d 6167 6529 2020 2020   self.image)    
+00003630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003640: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00003650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003660: 6d61 736b 203d 2073 656c 662e 7570 6461  mask = self.upda
+00003670: 7465 5f6d 6173 6b2e 6173 7479 7065 2827  te_mask.astype('
+00003680: 7569 6e74 3136 2729 0d0a 2020 2020 2020  uint16')..      
+00003690: 2020 2020 2020 7365 6c66 2e74 696d 6564        self.timed
+000036a0: 5f6d 6173 6b2c 2073 656c 662e 626f 756e  _mask, self.boun
+000036b0: 6461 7279 203d 2062 6f75 6e64 6172 795f  dary = boundary_
+000036c0: 706f 696e 7473 2873 656c 662e 6d61 736b  points(self.mask
+000036d0: 2c20 7365 6c66 2e78 6361 6c69 6272 6174  , self.xcalibrat
+000036e0: 696f 6e2c 2073 656c 662e 7963 616c 6962  ion, self.ycalib
+000036f0: 7261 7469 6f6e 2c20 7365 6c66 2e7a 6361  ration, self.zca
+00003700: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
+00003710: 2020 2020 656c 6966 2073 656c 662e 6d61      elif self.ma
+00003720: 736b 2069 7320 4e6f 6e65 3a0d 0a20 2020  sk is None:..   
+00003730: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00003740: 2e73 6567 5f69 6d61 6765 2069 7320 6e6f  .seg_image is no
+00003750: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00003760: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003780: 2020 2073 656c 662e 7570 6461 7465 5f6d     self.update_m
+00003790: 6173 6b20 3d20 6e70 2e7a 6572 6f73 2873  ask = np.zeros(s
+000037a0: 656c 662e 7365 675f 696d 6167 652e 7368  elf.seg_image.sh
+000037b0: 6170 6529 0d0a 2020 2020 2020 2020 2020  ape)..          
+000037c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000037d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000037e0: 656c 662e 7365 675f 696d 6167 6520 6973  elf.seg_image is
+000037f0: 204e 6f6e 6520 616e 6420 7365 6c66 2e69   None and self.i
+00003800: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+00003810: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+00003820: 2020 2020 2020 2020 2073 656c 662e 7570           self.up
+00003830: 6461 7465 5f6d 6173 6b20 3d20 6e70 2e7a  date_mask = np.z
+00003840: 6572 6f73 2873 656c 662e 696d 6167 652e  eros(self.image.
+00003850: 7368 6170 6529 200d 0a20 2020 2020 2020  shape) ..       
 00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003870: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00003880: 6964 203d 2069 6e74 2865 6467 652e 6765  id = int(edge.ge
-00003890: 7428 7365 6c66 2e73 706f 745f 7461 7267  t(self.spot_targ
-000038a0: 6574 5f69 645f 6b65 7929 290d 0a20 2020  et_id_key))..   
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038c0: 2020 2020 2020 2020 2061 6c6c 5f73 6f75           all_sou
-000038d0: 7263 655f 6964 732e 6170 7065 6e64 2873  rce_ids.append(s
-000038e0: 6f75 7263 655f 6964 290d 0a20 2020 2020  ource_id)..     
-000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003900: 2020 2020 2020 2061 6c6c 5f74 6172 6765         all_targe
-00003910: 745f 6964 732e 6170 7065 6e64 2874 6172  t_ids.append(tar
-00003920: 6765 745f 6964 290d 0a20 2020 2020 2020  get_id)..       
-00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003940: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00003950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003960: 2020 2069 6620 736f 7572 6365 5f69 6420     if source_id 
-00003970: 696e 2073 656c 662e 6564 6765 5f74 6172  in self.edge_tar
-00003980: 6765 745f 6c6f 6f6b 7570 2e6b 6579 7328  get_lookup.keys(
-00003990: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039b0: 2020 2073 656c 662e 6564 6765 5f74 6172     self.edge_tar
-000039c0: 6765 745f 6c6f 6f6b 7570 5b73 6f75 7263  get_lookup[sourc
-000039d0: 655f 6964 5d2e 6170 7065 6e64 2874 6172  e_id].append(tar
-000039e0: 6765 745f 6964 290d 0a20 2020 2020 2020  get_id)..       
-000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a00: 2020 2020 2065 6c73 653a 2020 2020 2020       else:      
-00003a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003870: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00003880: 2020 2073 656c 662e 6d61 736b 203d 2073     self.mask = s
+00003890: 656c 662e 7570 6461 7465 5f6d 6173 6b2e  elf.update_mask.
+000038a0: 6173 7479 7065 2827 7569 6e74 3136 2729  astype('uint16')
+000038b0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000038c0: 6c66 2e6d 6173 6b5b 3a2c 3a2c 313a 2d31  lf.mask[:,:,1:-1
+000038d0: 2c31 3a2d 315d 203d 2031 0d0a 2020 2020  ,1:-1] = 1..    
+000038e0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+000038f0: 6564 5f6d 6173 6b2c 2073 656c 662e 626f  ed_mask, self.bo
+00003900: 756e 6461 7279 203d 2062 6f75 6e64 6172  undary = boundar
+00003910: 795f 706f 696e 7473 2873 656c 662e 6d61  y_points(self.ma
+00003920: 736b 2c20 7365 6c66 2e78 6361 6c69 6272  sk, self.xcalibr
+00003930: 6174 696f 6e2c 2073 656c 662e 7963 616c  ation, self.ycal
+00003940: 6962 7261 7469 6f6e 2c20 7365 6c66 2e7a  ibration, self.z
+00003950: 6361 6c69 6272 6174 696f 6e29 0d0a 0d0a  calibration)....
+00003960: 2020 2020 2020 2020 2020 0d0a 0d0a 0d0a            ......
+00003970: 2020 2020 6465 6620 5f67 656e 6572 6174      def _generat
+00003980: 655f 6765 6e65 7261 7469 6f6e 7328 7365  e_generations(se
+00003990: 6c66 2c20 7472 6163 6b29 3a0d 0a20 2020  lf, track):..   
+000039a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000039b0: 616c 6c5f 736f 7572 6365 5f69 6473 203d  all_source_ids =
+000039c0: 205b 5d0d 0a20 2020 2020 2020 2061 6c6c   []..        all
+000039d0: 5f74 6172 6765 745f 6964 7320 3d20 5b5d  _target_ids = []
+000039e0: 200d 0a0d 0a0d 0a20 2020 2020 2020 2066   ......        f
+000039f0: 6f72 2065 6467 6520 696e 2074 7261 636b  or edge in track
+00003a00: 2e66 696e 6461 6c6c 2827 4564 6765 2729  .findall('Edge')
+00003a10: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
 00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a30: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
-00003a40: 745f 6c6f 6f6b 7570 5b73 6f75 7263 655f  t_lookup[source_
-00003a50: 6964 5d20 3d20 5b74 6172 6765 745f 6964  id] = [target_id
-00003a60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003a80: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
-00003a90: 6c6f 6f6b 7570 5b74 6172 6765 745f 6964  lookup[target_id
-00003aa0: 5d20 3d20 736f 7572 6365 5f69 6420 0d0a  ] = source_id ..
-00003ab0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00003ac0: 2061 6c6c 5f73 6f75 7263 655f 6964 732c   all_source_ids,
-00003ad0: 2061 6c6c 5f74 6172 6765 745f 6964 7320   all_target_ids 
-00003ae0: 0d0a 0d0a 0d0a 2020 2020 6465 6620 5f63  ......    def _c
-00003af0: 7265 6174 655f 6765 6e65 7261 7469 6f6e  reate_generation
-00003b00: 7328 7365 6c66 2c20 616c 6c5f 736f 7572  s(self, all_sour
-00003b10: 6365 5f69 6473 2c20 616c 6c5f 7461 7267  ce_ids, all_targ
-00003b20: 6574 5f69 6473 293a 0d0a 2020 2020 2020  et_ids):..      
-00003b30: 2020 200d 0a20 2020 2020 2020 2072 6f6f     ..        roo
-00003b40: 745f 6c65 6166 203d 205b 5d0d 0a20 2020  t_leaf = []..   
-00003b50: 2020 2020 2072 6f6f 745f 726f 6f74 203d       root_root =
-00003b60: 205b 5d0d 0a20 2020 2020 2020 2072 6f6f   []..        roo
-00003b70: 745f 7370 6c69 7473 203d 205b 5d0d 0a20  t_splits = [].. 
-00003b80: 2020 2020 2020 2073 706c 6974 5f63 6f75         split_cou
-00003b90: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
-00003ba0: 2347 6574 2074 6865 2072 6f6f 7420 6964  #Get the root id
-00003bb0: 0d0a 2020 2020 2020 2020 666f 7220 736f  ..        for so
-00003bc0: 7572 6365 5f69 6420 696e 2061 6c6c 5f73  urce_id in all_s
-00003bd0: 6f75 7263 655f 6964 733a 0d0a 2020 2020  ource_ids:..    
-00003be0: 2020 2020 2020 2020 2020 6966 2073 6f75            if sou
-00003bf0: 7263 655f 6964 206e 6f74 2069 6e20 616c  rce_id not in al
-00003c00: 6c5f 7461 7267 6574 5f69 6473 3a0d 0a20  l_target_ids:.. 
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c20: 2020 726f 6f74 5f72 6f6f 742e 6170 7065    root_root.appe
-00003c30: 6e64 2873 6f75 7263 655f 6964 2920 0d0a  nd(source_id) ..
-00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c50: 2020 200d 0a20 2020 2020 2020 0d0a 2020     ..       ..  
-00003c60: 2020 2020 2020 2347 6574 2074 6865 206c        #Get the l
-00003c70: 6561 6673 2061 6e64 2073 706c 6974 7320  eafs and splits 
-00003c80: 2020 2020 0d0a 2020 2020 2020 2020 666f      ..        fo
-00003c90: 7220 7461 7267 6574 5f69 6420 696e 2061  r target_id in a
-00003ca0: 6c6c 5f74 6172 6765 745f 6964 733a 0d0a  ll_target_ids:..
-00003cb0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00003cc0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00003cd0: 6172 6765 745f 6964 206e 6f74 2069 6e20  arget_id not in 
-00003ce0: 616c 6c5f 736f 7572 6365 5f69 6473 3a0d  all_source_ids:.
-00003cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d00: 2020 2072 6f6f 745f 6c65 6166 2e61 7070     root_leaf.app
-00003d10: 656e 6428 7461 7267 6574 5f69 6429 0d0a  end(target_id)..
-00003d20: 2020 2020 2020 2020 2020 2020 2073 706c               spl
-00003d30: 6974 5f63 6f75 6e74 203d 2061 6c6c 5f73  it_count = all_s
-00003d40: 6f75 7263 655f 6964 732e 636f 756e 7428  ource_ids.count(
-00003d50: 7461 7267 6574 5f69 6429 0d0a 2020 2020  target_id)..    
-00003d60: 2020 2020 2020 2020 2069 6620 7370 6c69           if spli
-00003d70: 745f 636f 756e 7420 3e20 313a 0d0a 2020  t_count > 1:..  
-00003d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d90: 2020 2020 726f 6f74 5f73 706c 6974 732e      root_splits.
-00003da0: 6170 7065 6e64 2874 6172 6765 745f 6964  append(target_id
-00003db0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00003dc0: 2020 0d0a 2020 2020 2020 2020 2370 7269    ..        #pri
-00003dd0: 6e74 2827 726f 6f74 2061 6e64 2073 706c  nt('root and spl
-00003de0: 6974 7327 2c72 6f6f 745f 726f 6f74 2c20  its',root_root, 
-00003df0: 726f 6f74 5f6c 6561 662c 2072 6f6f 745f  root_leaf, root_
-00003e00: 7370 6c69 7473 290d 0a20 2020 2020 2020  splits)..       
-00003e10: 2073 656c 662e 5f64 6973 7461 6e63 655f   self._distance_
-00003e20: 726f 6f74 5f6c 6561 6628 726f 6f74 5f72  root_leaf(root_r
-00003e30: 6f6f 742c 2072 6f6f 745f 6c65 6166 2c20  oot, root_leaf, 
-00003e40: 726f 6f74 5f73 706c 6974 7329 0d0a 0d0a  root_splits)....
-00003e50: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00003e60: 6f6f 745f 726f 6f74 2c20 726f 6f74 5f73  oot_root, root_s
-00003e70: 706c 6974 732c 2072 6f6f 745f 6c65 6166  plits, root_leaf
-00003e80: 0d0a 0d0a 0d0a 2020 2020 6465 6620 5f69  ......    def _i
-00003e90: 7465 7261 7465 5f73 706c 6974 5f64 6f77  terate_split_dow
-00003ea0: 6e28 7365 6c66 2c20 726f 6f74 5f72 6f6f  n(self, root_roo
-00003eb0: 742c 2072 6f6f 745f 6c65 6166 2c20 726f  t, root_leaf, ro
-00003ec0: 6f74 5f73 706c 6974 7329 3a0d 0a20 2020  ot_splits):..   
-00003ed0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00003ee0: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
-00003ef0: 3d20 7374 7228 3029 0d0a 2020 2020 2020  = str(0)..      
-00003f00: 2020 2073 656c 662e 6173 7369 676e 6564     self.assigned
-00003f10: 5f74 7261 636b 6574 5f63 6f75 6e74 7320  _tracket_counts 
-00003f20: 3d20 5b5d 0d0a 2020 2020 2020 2020 2066  = []..         f
-00003f30: 6f72 2072 6f6f 745f 616c 6c20 696e 2072  or root_all in r
-00003f40: 6f6f 745f 726f 6f74 3a0d 0a20 2020 2020  oot_root:..     
-00003f50: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00003f60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003f70: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
-00003f80: 726f 6f74 5f61 6c6c 5d20 3d20 7374 7228  root_all] = str(
-00003f90: 7472 6163 6b6c 6574 5f63 6f75 6e74 290d  tracklet_count).
-00003fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003fb0: 2073 656c 662e 6173 7369 676e 6564 5f74   self.assigned_t
-00003fc0: 7261 636b 6574 5f63 6f75 6e74 732e 6170  racket_counts.ap
-00003fd0: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
-00003fe0: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
-00003ff0: 2020 2020 2020 6966 2072 6f6f 745f 616c        if root_al
-00004000: 6c20 696e 2073 656c 662e 6564 6765 5f74  l in self.edge_t
-00004010: 6172 6765 745f 6c6f 6f6b 7570 3a0d 0a20  arget_lookup:.. 
-00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004030: 2020 7461 7267 6574 5f63 656c 6c73 203d    target_cells =
-00004040: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
-00004050: 745f 6c6f 6f6b 7570 5b72 6f6f 745f 616c  t_lookup[root_al
-00004060: 6c5d 0d0a 2020 2020 2020 2020 2020 2020  l]..            
-00004070: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00004080: 7261 6e67 6528 6c65 6e28 7461 7267 6574  range(len(target
-00004090: 5f63 656c 6c73 2929 3a0d 0a20 2020 2020  _cells)):..     
-000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040b0: 2020 2074 6172 6765 745f 6365 6c6c 5f69     target_cell_i
-000040c0: 6420 3d20 7461 7267 6574 5f63 656c 6c73  d = target_cells
-000040d0: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-000040e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000040f0: 7461 7267 6574 5f63 656c 6c5f 6964 2069  target_cell_id i
-00004100: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
-00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004120: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00004130: 6c65 745f 636f 756e 7420 3d20 7374 7228  let_count = str(
-00004140: 7472 6163 6b6c 6574 5f63 6f75 6e74 2920  tracklet_count) 
-00004150: 2b20 7374 7228 6929 202b 2073 7472 2831  + str(i) + str(1
-00004160: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004170: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004180: 6c66 2e5f 6173 7369 676e 5f74 7261 636b  lf._assign_track
-00004190: 6c65 745f 6964 2874 6172 6765 745f 6365  let_id(target_ce
-000041a0: 6c6c 5f69 642c 2072 6f6f 745f 7370 6c69  ll_id, root_spli
-000041b0: 7473 2c20 726f 6f74 5f6c 6561 662c 2074  ts, root_leaf, t
-000041c0: 7261 636b 6c65 745f 636f 756e 7429 2020  racklet_count)  
-000041d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000041e0: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
-000041f0: 6765 745f 6365 6c6c 5f69 6420 6e6f 7420  get_cell_id not 
-00004200: 696e 2072 6f6f 745f 7370 6c69 7473 3a0d  in root_splits:.
-00004210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004230: 2e5f 6173 7369 676e 5f74 7261 636b 6c65  ._assign_trackle
-00004240: 745f 6964 2874 6172 6765 745f 6365 6c6c  t_id(target_cell
-00004250: 5f69 642c 2072 6f6f 745f 7370 6c69 7473  _id, root_splits
-00004260: 2c20 726f 6f74 5f6c 6561 662c 2074 7261  , root_leaf, tra
-00004270: 636b 6c65 745f 636f 756e 7429 2020 2020  cklet_count)    
-00004280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000042b0: 2020 0d0a 2020 2020 6465 6620 5f61 7373    ..    def _ass
-000042c0: 6967 6e5f 7472 6163 6b6c 6574 5f69 6428  ign_tracklet_id(
-000042d0: 7365 6c66 2c20 7461 7267 6574 5f69 642c  self, target_id,
-000042e0: 2072 6f6f 745f 7370 6c69 7473 2c20 726f   root_splits, ro
-000042f0: 6f74 5f6c 6561 662c 2074 7261 636b 6c65  ot_leaf, trackle
-00004300: 745f 636f 756e 7420 293a 0d0a 2020 2020  t_count ):..    
-00004310: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-00004320: 6620 7461 7267 6574 5f69 6420 696e 2072  f target_id in r
-00004330: 6f6f 745f 6c65 6166 3a0d 0a20 2020 2020  oot_leaf:..     
-00004340: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00004350: 7261 636b 6c65 745f 6469 6374 5b74 6172  racklet_dict[tar
-00004360: 6765 745f 6964 5d20 3d20 2073 7472 2874  get_id] =  str(t
-00004370: 7261 636b 6c65 745f 636f 756e 7429 0d0a  racklet_count)..
-00004380: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004390: 656c 662e 6173 7369 676e 6564 5f74 7261  elf.assigned_tra
-000043a0: 636b 6574 5f63 6f75 6e74 732e 6170 7065  cket_counts.appe
-000043b0: 6e64 2874 7261 636b 6c65 745f 636f 756e  nd(tracklet_coun
-000043c0: 7429 0d0a 2020 2020 2020 2020 6966 2074  t)..        if t
-000043d0: 6172 6765 745f 6964 206e 6f74 2069 6e20  arget_id not in 
-000043e0: 726f 6f74 5f6c 6561 663a 2020 0d0a 2020  root_leaf:  ..  
-000043f0: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
-00004400: 6765 745f 6964 206e 6f74 2069 6e20 726f  get_id not in ro
-00004410: 6f74 5f73 706c 6974 733a 0d0a 2020 2020  ot_splits:..    
+00003a30: 2073 6f75 7263 655f 6964 203d 2069 6e74   source_id = int
+00003a40: 2865 6467 652e 6765 7428 7365 6c66 2e73  (edge.get(self.s
+00003a50: 706f 745f 736f 7572 6365 5f69 645f 6b65  pot_source_id_ke
+00003a60: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a80: 2074 6172 6765 745f 6964 203d 2069 6e74   target_id = int
+00003a90: 2865 6467 652e 6765 7428 7365 6c66 2e73  (edge.get(self.s
+00003aa0: 706f 745f 7461 7267 6574 5f69 645f 6b65  pot_target_id_ke
+00003ab0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ad0: 2061 6c6c 5f73 6f75 7263 655f 6964 732e   all_source_ids.
+00003ae0: 6170 7065 6e64 2873 6f75 7263 655f 6964  append(source_id
+00003af0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003b00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00003b10: 6c6c 5f74 6172 6765 745f 6964 732e 6170  ll_target_ids.ap
+00003b20: 7065 6e64 2874 6172 6765 745f 6964 290d  pend(target_id).
+00003b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b40: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b60: 2020 2020 2020 2020 2020 2069 6620 736f             if so
+00003b70: 7572 6365 5f69 6420 696e 2073 656c 662e  urce_id in self.
+00003b80: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00003b90: 7570 2e6b 6579 7328 293a 0d0a 2020 2020  up.keys():..    
+00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003bc0: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00003bd0: 7570 5b73 6f75 7263 655f 6964 5d2e 6170  up[source_id].ap
+00003be0: 7065 6e64 2874 6172 6765 745f 6964 290d  pend(target_id).
+00003bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003c00: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00003c10: 653a 2020 2020 2020 0d0a 2020 2020 2020  e:      ..      
+00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c30: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
+00003c40: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00003c50: 5b73 6f75 7263 655f 6964 5d20 3d20 5b74  [source_id] = [t
+00003c60: 6172 6765 745f 6964 5d0d 0a20 2020 2020  arget_id]..     
+00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c80: 2020 2020 2020 2073 656c 662e 6564 6765         self.edge
+00003c90: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b74  _source_lookup[t
+00003ca0: 6172 6765 745f 6964 5d20 3d20 736f 7572  arget_id] = sour
+00003cb0: 6365 5f69 6420 0d0a 0d0a 2020 2020 2020  ce_id ....      
+00003cc0: 2020 7265 7475 726e 2061 6c6c 5f73 6f75    return all_sou
+00003cd0: 7263 655f 6964 732c 2061 6c6c 5f74 6172  rce_ids, all_tar
+00003ce0: 6765 745f 6964 7320 0d0a 0d0a 0d0a 2020  get_ids ......  
+00003cf0: 2020 6465 6620 5f63 7265 6174 655f 6765    def _create_ge
+00003d00: 6e65 7261 7469 6f6e 7328 7365 6c66 2c20  nerations(self, 
+00003d10: 616c 6c5f 736f 7572 6365 5f69 6473 2c20  all_source_ids, 
+00003d20: 616c 6c5f 7461 7267 6574 5f69 6473 293a  all_target_ids):
+00003d30: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
+00003d40: 2020 2020 2072 6f6f 745f 6c65 6166 203d       root_leaf =
+00003d50: 205b 5d0d 0a20 2020 2020 2020 2072 6f6f   []..        roo
+00003d60: 745f 726f 6f74 203d 205b 5d0d 0a20 2020  t_root = []..   
+00003d70: 2020 2020 2072 6f6f 745f 7370 6c69 7473       root_splits
+00003d80: 203d 205b 5d0d 0a20 2020 2020 2020 2073   = []..        s
+00003d90: 706c 6974 5f63 6f75 6e74 203d 2030 0d0a  plit_count = 0..
+00003da0: 2020 2020 2020 2020 2347 6574 2074 6865          #Get the
+00003db0: 2072 6f6f 7420 6964 0d0a 2020 2020 2020   root id..      
+00003dc0: 2020 666f 7220 736f 7572 6365 5f69 6420    for source_id 
+00003dd0: 696e 2061 6c6c 5f73 6f75 7263 655f 6964  in all_source_id
+00003de0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00003df0: 2020 6966 2073 6f75 7263 655f 6964 206e    if source_id n
+00003e00: 6f74 2069 6e20 616c 6c5f 7461 7267 6574  ot in all_target
+00003e10: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
+00003e20: 2020 2020 2020 2020 2020 726f 6f74 5f72            root_r
+00003e30: 6f6f 742e 6170 7065 6e64 2873 6f75 7263  oot.append(sourc
+00003e40: 655f 6964 2920 0d0a 2020 2020 2020 2020  e_id) ..        
+00003e50: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00003e60: 2020 2020 0d0a 2020 2020 2020 2020 2347      ..        #G
+00003e70: 6574 2074 6865 206c 6561 6673 2061 6e64  et the leafs and
+00003e80: 2073 706c 6974 7320 2020 2020 0d0a 2020   splits     ..  
+00003e90: 2020 2020 2020 666f 7220 7461 7267 6574        for target
+00003ea0: 5f69 6420 696e 2061 6c6c 5f74 6172 6765  _id in all_targe
+00003eb0: 745f 6964 733a 0d0a 2020 2020 2020 2020  t_ids:..        
+00003ec0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00003ed0: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
+00003ee0: 206e 6f74 2069 6e20 616c 6c5f 736f 7572   not in all_sour
+00003ef0: 6365 5f69 6473 3a0d 0a20 2020 2020 2020  ce_ids:..       
+00003f00: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00003f10: 6c65 6166 2e61 7070 656e 6428 7461 7267  leaf.append(targ
+00003f20: 6574 5f69 6429 0d0a 2020 2020 2020 2020  et_id)..        
+00003f30: 2020 2020 2073 706c 6974 5f63 6f75 6e74       split_count
+00003f40: 203d 2061 6c6c 5f73 6f75 7263 655f 6964   = all_source_id
+00003f50: 732e 636f 756e 7428 7461 7267 6574 5f69  s.count(target_i
+00003f60: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00003f70: 2069 6620 7370 6c69 745f 636f 756e 7420   if split_count 
+00003f80: 3e20 313a 0d0a 2020 2020 2020 2020 2020  > 1:..          
+00003f90: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+00003fa0: 5f73 706c 6974 732e 6170 7065 6e64 2874  _splits.append(t
+00003fb0: 6172 6765 745f 6964 290d 0a0d 0a20 2020  arget_id)....   
+00003fc0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00003fd0: 2020 2020 2370 7269 6e74 2827 726f 6f74      #print('root
+00003fe0: 2061 6e64 2073 706c 6974 7327 2c72 6f6f   and splits',roo
+00003ff0: 745f 726f 6f74 2c20 726f 6f74 5f6c 6561  t_root, root_lea
+00004000: 662c 2072 6f6f 745f 7370 6c69 7473 290d  f, root_splits).
+00004010: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+00004020: 6973 7461 6e63 655f 726f 6f74 5f6c 6561  istance_root_lea
+00004030: 6628 726f 6f74 5f72 6f6f 742c 2072 6f6f  f(root_root, roo
+00004040: 745f 6c65 6166 2c20 726f 6f74 5f73 706c  t_leaf, root_spl
+00004050: 6974 7329 0d0a 0d0a 2020 2020 2020 2020  its)....        
+00004060: 7265 7475 726e 2072 6f6f 745f 726f 6f74  return root_root
+00004070: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
+00004080: 6f6f 745f 6c65 6166 0d0a 0d0a 0d0a 2020  oot_leaf......  
+00004090: 2020 6465 6620 5f69 7465 7261 7465 5f73    def _iterate_s
+000040a0: 706c 6974 5f64 6f77 6e28 7365 6c66 2c20  plit_down(self, 
+000040b0: 726f 6f74 5f72 6f6f 742c 2072 6f6f 745f  root_root, root_
+000040c0: 6c65 6166 2c20 726f 6f74 5f73 706c 6974  leaf, root_split
+000040d0: 7329 3a0d 0a20 2020 2020 2020 2020 0d0a  s):..         ..
+000040e0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
+000040f0: 745f 636f 756e 7420 3d20 7374 7228 3029  t_count = str(0)
+00004100: 0d0a 2020 2020 2020 2020 2073 656c 662e  ..         self.
+00004110: 6173 7369 676e 6564 5f74 7261 636b 6574  assigned_tracket
+00004120: 5f63 6f75 6e74 7320 3d20 5b5d 0d0a 2020  _counts = []..  
+00004130: 2020 2020 2020 2066 6f72 2072 6f6f 745f         for root_
+00004140: 616c 6c20 696e 2072 6f6f 745f 726f 6f74  all in root_root
+00004150: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004160: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00004170: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
+00004180: 6574 5f64 6963 745b 726f 6f74 5f61 6c6c  et_dict[root_all
+00004190: 5d20 3d20 7374 7228 7472 6163 6b6c 6574  ] = str(tracklet
+000041a0: 5f63 6f75 6e74 290d 0a20 2020 2020 2020  _count)..       
+000041b0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+000041c0: 7369 676e 6564 5f74 7261 636b 6574 5f63  signed_tracket_c
+000041d0: 6f75 6e74 732e 6170 7065 6e64 2874 7261  ounts.append(tra
+000041e0: 636b 6c65 745f 636f 756e 7429 0d0a 2020  cklet_count)..  
+000041f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004200: 2072 6f6f 745f 616c 6c20 696e 2073 656c   root_all in sel
+00004210: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
+00004220: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
+00004230: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00004240: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
+00004250: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00004260: 5b72 6f6f 745f 616c 6c5d 0d0a 2020 2020  [root_all]..    
+00004270: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004280: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00004290: 6e28 7461 7267 6574 5f63 656c 6c73 2929  n(target_cells))
+000042a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000042b0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+000042c0: 745f 6365 6c6c 5f69 6420 3d20 7461 7267  t_cell_id = targ
+000042d0: 6574 5f63 656c 6c73 5b69 5d0d 0a20 2020  et_cells[i]..   
+000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042f0: 2020 2020 2069 6620 7461 7267 6574 5f63       if target_c
+00004300: 656c 6c5f 6964 2069 6e20 726f 6f74 5f73  ell_id in root_s
+00004310: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
+00004320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004330: 2020 2074 7261 636b 6c65 745f 636f 756e     tracklet_coun
+00004340: 7420 3d20 7374 7228 7472 6163 6b6c 6574  t = str(tracklet
+00004350: 5f63 6f75 6e74 2920 2b20 7374 7228 6929  _count) + str(i)
+00004360: 202b 2073 7472 2831 290d 0a20 2020 2020   + str(1)..     
+00004370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004380: 2020 2020 2020 7365 6c66 2e5f 6173 7369        self._assi
+00004390: 676e 5f74 7261 636b 6c65 745f 6964 2874  gn_tracklet_id(t
+000043a0: 6172 6765 745f 6365 6c6c 5f69 642c 2072  arget_cell_id, r
+000043b0: 6f6f 745f 7370 6c69 7473 2c20 726f 6f74  oot_splits, root
+000043c0: 5f6c 6561 662c 2074 7261 636b 6c65 745f  _leaf, tracklet_
+000043d0: 636f 756e 7429 2020 0d0a 2020 2020 2020  count)  ..      
+000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043f0: 2020 6966 2074 6172 6765 745f 6365 6c6c    if target_cell
+00004400: 5f69 6420 6e6f 7420 696e 2072 6f6f 745f  _id not in root_
+00004410: 7370 6c69 7473 3a0d 0a20 2020 2020 2020  splits:..       
 00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004450: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-00004460: 6c65 745f 6469 6374 5b74 6172 6765 745f  let_dict[target_
-00004470: 6964 5d20 3d20 7374 7228 7472 6163 6b6c  id] = str(trackl
-00004480: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
+00004430: 2020 2020 7365 6c66 2e5f 6173 7369 676e      self._assign
+00004440: 5f74 7261 636b 6c65 745f 6964 2874 6172  _tracklet_id(tar
+00004450: 6765 745f 6365 6c6c 5f69 642c 2072 6f6f  get_cell_id, roo
+00004460: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
+00004470: 6561 662c 2074 7261 636b 6c65 745f 636f  eaf, tracklet_co
+00004480: 756e 7429 2020 2020 0d0a 2020 2020 2020  unt)    ..      
 00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044a0: 2020 2020 2020 2073 656c 662e 6173 7369         self.assi
-000044b0: 676e 6564 5f74 7261 636b 6574 5f63 6f75  gned_tracket_cou
-000044c0: 6e74 732e 6170 7065 6e64 2874 7261 636b  nts.append(track
-000044d0: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
-000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044f0: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
-00004500: 745f 6964 2069 6e20 7365 6c66 2e65 6467  t_id in self.edg
-00004510: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
-00004520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004540: 2020 7461 7267 6574 5f63 656c 6c73 203d    target_cells =
-00004550: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
-00004560: 745f 6c6f 6f6b 7570 5b74 6172 6765 745f  t_lookup[target_
-00004570: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
-00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004590: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045b0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000045c0: 7261 6e67 6528 6c65 6e28 7461 7267 6574  range(len(target
-000045d0: 5f63 656c 6c73 2929 3a0d 0a20 2020 2020  _cells)):..     
-000045e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00004600: 6172 6765 745f 6365 6c6c 5f69 6420 3d20  arget_cell_id = 
-00004610: 7461 7267 6574 5f63 656c 6c73 5b69 5d0d  target_cells[i].
-00004620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000044a0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000044b0: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
+000044c0: 6465 6620 5f61 7373 6967 6e5f 7472 6163  def _assign_trac
+000044d0: 6b6c 6574 5f69 6428 7365 6c66 2c20 7461  klet_id(self, ta
+000044e0: 7267 6574 5f69 642c 2072 6f6f 745f 7370  rget_id, root_sp
+000044f0: 6c69 7473 2c20 726f 6f74 5f6c 6561 662c  lits, root_leaf,
+00004500: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
+00004510: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
+00004520: 2020 2020 2020 2069 6620 7461 7267 6574         if target
+00004530: 5f69 6420 696e 2072 6f6f 745f 6c65 6166  _id in root_leaf
+00004540: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004550: 2020 7365 6c66 2e74 7261 636b 6c65 745f    self.tracklet_
+00004560: 6469 6374 5b74 6172 6765 745f 6964 5d20  dict[target_id] 
+00004570: 3d20 2073 7472 2874 7261 636b 6c65 745f  =  str(tracklet_
+00004580: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
+00004590: 2020 2020 2020 2073 656c 662e 6173 7369         self.assi
+000045a0: 676e 6564 5f74 7261 636b 6574 5f63 6f75  gned_tracket_cou
+000045b0: 6e74 732e 6170 7065 6e64 2874 7261 636b  nts.append(track
+000045c0: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
+000045d0: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
+000045e0: 206e 6f74 2069 6e20 726f 6f74 5f6c 6561   not in root_lea
+000045f0: 663a 2020 0d0a 2020 2020 2020 2020 2020  f:  ..          
+00004600: 2020 6966 2074 6172 6765 745f 6964 206e    if target_id n
+00004610: 6f74 2069 6e20 726f 6f74 5f73 706c 6974  ot in root_split
+00004620: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
 00004630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004640: 2020 2020 2073 656c 662e 5f61 7373 6967       self._assig
-00004650: 6e5f 7472 6163 6b6c 6574 5f69 6428 7461  n_tracklet_id(ta
-00004660: 7267 6574 5f63 656c 6c5f 6964 2c20 726f  rget_cell_id, ro
-00004670: 6f74 5f73 706c 6974 732c 2072 6f6f 745f  ot_splits, root_
-00004680: 6c65 6166 2c20 7472 6163 6b6c 6574 5f63  leaf, tracklet_c
-00004690: 6f75 6e74 2029 0d0a 2020 2020 2020 2020  ount )..        
-000046a0: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
-000046b0: 2069 6e20 726f 6f74 5f73 706c 6974 733a   in root_splits:
-000046c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00004640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004650: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004660: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
+00004670: 5b74 6172 6765 745f 6964 5d20 3d20 7374  [target_id] = st
+00004680: 7228 7472 6163 6b6c 6574 5f63 6f75 6e74  r(tracklet_count
+00004690: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000046b0: 656c 662e 6173 7369 676e 6564 5f74 7261  elf.assigned_tra
+000046c0: 636b 6574 5f63 6f75 6e74 732e 6170 7065  cket_counts.appe
+000046d0: 6e64 2874 7261 636b 6c65 745f 636f 756e  nd(tracklet_coun
+000046e0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
 000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004700: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00004710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004730: 2020 7365 6c66 2e74 7261 636b 6c65 745f    self.tracklet_
-00004740: 6469 6374 5b74 6172 6765 745f 6964 5d20  dict[target_id] 
-00004750: 3d20 7374 7228 7472 6163 6b6c 6574 5f63  = str(tracklet_c
-00004760: 6f75 6e74 290d 0a20 2020 2020 2020 2020  ount)..         
-00004770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004790: 6173 7369 676e 6564 5f74 7261 636b 6574  assigned_tracket
-000047a0: 5f63 6f75 6e74 732e 6170 7065 6e64 2874  _counts.append(t
-000047b0: 7261 636b 6c65 745f 636f 756e 7429 0d0a  racklet_count)..
-000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047e0: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
-000047f0: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
-00004800: 7267 6574 5f6c 6f6f 6b75 703a 0d0a 2020  rget_lookup:..  
-00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004830: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
-00004840: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
-00004850: 6172 6765 745f 6c6f 6f6b 7570 5b74 6172  arget_lookup[tar
-00004860: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
-00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004890: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-000048a0: 6c65 6e28 7461 7267 6574 5f63 656c 6c73  len(target_cells
-000048b0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004700: 6966 2074 6172 6765 745f 6964 2069 6e20  if target_id in 
+00004710: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
+00004720: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
+00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004740: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00004750: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
+00004760: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00004770: 5b74 6172 6765 745f 6964 5d0d 0a20 2020  [target_id]..   
+00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004790: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000047c0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+000047d0: 6e28 7461 7267 6574 5f63 656c 6c73 2929  n(target_cells))
+000047e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004800: 2020 2020 2020 2074 6172 6765 745f 6365         target_ce
+00004810: 6c6c 5f69 6420 3d20 7461 7267 6574 5f63  ll_id = target_c
+00004820: 656c 6c73 5b69 5d0d 0a20 2020 2020 2020  ells[i]..       
+00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004840: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00004850: 662e 5f61 7373 6967 6e5f 7472 6163 6b6c  f._assign_trackl
+00004860: 6574 5f69 6428 7461 7267 6574 5f63 656c  et_id(target_cel
+00004870: 6c5f 6964 2c20 726f 6f74 5f73 706c 6974  l_id, root_split
+00004880: 732c 2072 6f6f 745f 6c65 6166 2c20 7472  s, root_leaf, tr
+00004890: 6163 6b6c 6574 5f63 6f75 6e74 2029 0d0a  acklet_count )..
+000048a0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+000048b0: 6172 6765 745f 6964 2069 6e20 726f 6f74  arget_id in root
+000048c0: 5f73 706c 6974 733a 0d0a 2020 2020 2020  _splits:..      
 000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2074 6172 6765 745f 6365 6c6c 5f69 6420   target_cell_id 
-000048f0: 3d20 7461 7267 6574 5f63 656c 6c73 5b69  = target_cells[i
-00004900: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004930: 6620 7365 6c66 2e65 6467 655f 736f 7572  f self.edge_sour
-00004940: 6365 5f6c 6f6f 6b75 705b 7461 7267 6574  ce_lookup[target
-00004950: 5f63 656c 6c5f 6964 5d20 696e 2072 6f6f  _cell_id] in roo
-00004960: 745f 7370 6c69 7473 3a0d 0a20 2020 2020  t_splits:..     
+000048e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004910: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00004940: 7261 636b 6c65 745f 6469 6374 5b74 6172  racklet_dict[tar
+00004950: 6765 745f 6964 5d20 3d20 7374 7228 7472  get_id] = str(tr
+00004960: 6163 6b6c 6574 5f63 6f75 6e74 290d 0a20  acklet_count).. 
 00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000049a0: 5f75 6e69 7175 655f 7370 6c69 745f 6964  _unique_split_id
-000049b0: 2874 6172 6765 745f 6365 6c6c 5f69 642c  (target_cell_id,
-000049c0: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
-000049d0: 2b20 7374 7228 6929 202b 2073 7472 2831  + str(i) + str(1
-000049e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a10: 7365 6c66 2e5f 6173 7369 676e 5f74 7261  self._assign_tra
-00004a20: 636b 6c65 745f 6964 2874 6172 6765 745f  cklet_id(target_
-00004a30: 6365 6c6c 5f69 642c 2072 6f6f 745f 7370  cell_id, root_sp
-00004a40: 6c69 7473 2c20 726f 6f74 5f6c 6561 662c  lits, root_leaf,
-00004a50: 2020 7472 6163 6b6c 6574 5f63 6f75 6e74    tracklet_count
-00004a60: 202b 2073 7472 2869 2920 2b20 7374 7228   + str(i) + str(
-00004a70: 3129 2029 0d0a 0d0a 2020 2020 2020 2020  1) )....        
+00004990: 2020 2073 656c 662e 6173 7369 676e 6564     self.assigned
+000049a0: 5f74 7261 636b 6574 5f63 6f75 6e74 732e  _tracket_counts.
+000049b0: 6170 7065 6e64 2874 7261 636b 6c65 745f  append(tracklet_
+000049c0: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
+000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049e0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+000049f0: 6172 6765 745f 6964 2069 6e20 7365 6c66  arget_id in self
+00004a00: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+00004a10: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
+00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a30: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00004a40: 7267 6574 5f63 656c 6c73 203d 2073 656c  rget_cells = sel
+00004a50: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
+00004a60: 6f6b 7570 5b74 6172 6765 745f 6964 5d0d  okup[target_id].
+00004a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00004aa0: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
-00004ab0: 2064 6566 205f 756e 6971 7565 5f73 706c   def _unique_spl
-00004ac0: 6974 5f69 6428 7365 6c66 2c20 7461 7267  it_id(self, targ
-00004ad0: 6574 5f69 642c 2074 7261 636b 6c65 745f  et_id, tracklet_
-00004ae0: 636f 756e 7429 3a0d 0a0d 0a20 2020 2020  count):....     
-00004af0: 2020 2069 6620 7472 6163 6b6c 6574 5f63     if tracklet_c
-00004b00: 6f75 6e74 206e 6f74 2069 6e20 7365 6c66  ount not in self
-00004b10: 2e61 7373 6967 6e65 645f 7472 6163 6b65  .assigned_tracke
-00004b20: 745f 636f 756e 7473 3a0d 0a20 2020 2020  t_counts:..     
-00004b30: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00004b40: 7261 636b 6c65 745f 6469 6374 5b74 6172  racklet_dict[tar
-00004b50: 6765 745f 6964 5d20 3d20 7374 7228 7472  get_id] = str(tr
-00004b60: 6163 6b6c 6574 5f63 6f75 6e74 290d 0a20  acklet_count).. 
-00004b70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004b80: 6c66 2e61 7373 6967 6e65 645f 7472 6163  lf.assigned_trac
-00004b90: 6b65 745f 636f 756e 7473 2e61 7070 656e  ket_counts.appen
-00004ba0: 6428 7472 6163 6b6c 6574 5f63 6f75 6e74  d(tracklet_count
-00004bb0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-00004bc0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00004bd0: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
-00004be0: 5f63 6f75 6e74 203d 2073 7472 2874 7261  _count = str(tra
-00004bf0: 636b 6c65 745f 636f 756e 7429 202b 2073  cklet_count) + s
-00004c00: 7472 2831 290d 0a20 2020 2020 2020 2020  tr(1)..         
-00004c10: 2020 2073 656c 662e 5f75 6e69 7175 655f     self._unique_
-00004c20: 7370 6c69 745f 6964 2874 6172 6765 745f  split_id(target_
-00004c30: 6964 2c20 7472 6163 6b6c 6574 5f63 6f75  id, tracklet_cou
-00004c40: 6e74 290d 0a0d 0a0d 0a20 2020 2064 6566  nt)......    def
-00004c50: 205f 6469 7374 616e 6365 5f72 6f6f 745f   _distance_root_
-00004c60: 6c65 6166 2873 656c 662c 2072 6f6f 745f  leaf(self, root_
-00004c70: 726f 6f74 2c20 726f 6f74 5f6c 6561 662c  root, root_leaf,
-00004c80: 2072 6f6f 745f 7370 6c69 7473 293a 0d0a   root_splits):..
-00004c90: 0d0a 0d0a 2020 2020 2020 2020 0d0a 2020  ....        ..  
-00004ca0: 2020 2020 2020 2067 656e 5f63 6f75 6e74         gen_count
-00004cb0: 203d 2030 0d0a 2020 2020 2020 2020 2066   = 0..         f
-00004cc0: 6f72 2072 6f6f 745f 616c 6c20 696e 2072  or root_all in r
-00004cd0: 6f6f 745f 726f 6f74 3a0d 0a20 2020 2020  oot_root:..     
-00004ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004cf0: 6765 6e65 7261 7469 6f6e 5f64 6963 745b  generation_dict[
-00004d00: 726f 6f74 5f61 6c6c 5d20 3d20 300d 0a20  root_all] = 0.. 
-00004d10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004d20: 6620 726f 6f74 5f61 6c6c 2069 6e20 7365  f root_all in se
-00004d30: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
-00004d40: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
-00004d50: 2020 2020 2020 2020 2020 2074 6172 6765             targe
-00004d60: 745f 6365 6c6c 7320 3d20 7365 6c66 2e65  t_cells = self.e
-00004d70: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-00004d80: 705b 726f 6f74 5f61 6c6c 5d0d 0a20 2020  p[root_all]..   
-00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004da0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00004db0: 656e 2874 6172 6765 745f 6365 6c6c 7329  en(target_cells)
-00004dc0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00004dd0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00004de0: 6574 5f63 656c 6c5f 6964 203d 2074 6172  et_cell_id = tar
-00004df0: 6765 745f 6365 6c6c 735b 695d 0d0a 2020  get_cells[i]..  
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2020 2020 6966 2074 6172 6765 745f        if target_
-00004e20: 6365 6c6c 5f69 6420 6e6f 7420 696e 2072  cell_id not in r
-00004e30: 6f6f 745f 7370 6c69 7473 3a0d 0a20 2020  oot_splits:..   
-00004e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e50: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00004e80: 662e 5f72 6563 7572 7369 7665 5f70 6174  f._recursive_pat
-00004e90: 6828 7461 7267 6574 5f63 656c 6c5f 6964  h(target_cell_id
-00004ea0: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
-00004eb0: 6f6f 745f 6c65 6166 2c20 6765 6e5f 636f  oot_leaf, gen_co
-00004ec0: 756e 7420 290d 0a20 2020 2020 2020 2020  unt )..         
-00004ed0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004ee0: 6620 7461 7267 6574 5f63 656c 6c5f 6964  f target_cell_id
-00004ef0: 2069 6e20 726f 6f74 5f73 706c 6974 733a   in root_splits:
-00004f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f20: 2020 2020 2020 2020 2067 656e 5f63 6f75           gen_cou
-00004f30: 6e74 203d 2067 656e 5f63 6f75 6e74 202b  nt = gen_count +
-00004f40: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+00004a90: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00004aa0: 6e20 7261 6e67 6528 6c65 6e28 7461 7267  n range(len(targ
+00004ab0: 6574 5f63 656c 6c73 2929 3a0d 0a20 2020  et_cells)):..   
+00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ae0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00004af0: 6365 6c6c 5f69 6420 3d20 7461 7267 6574  cell_id = target
+00004b00: 5f63 656c 6c73 5b69 5d0d 0a20 2020 2020  _cells[i]..     
+00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b30: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+00004b40: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
+00004b50: 705b 7461 7267 6574 5f63 656c 6c5f 6964  p[target_cell_id
+00004b60: 5d20 696e 2072 6f6f 745f 7370 6c69 7473  ] in root_splits
+00004b70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ba0: 2020 2073 656c 662e 5f75 6e69 7175 655f     self._unique_
+00004bb0: 7370 6c69 745f 6964 2874 6172 6765 745f  split_id(target_
+00004bc0: 6365 6c6c 5f69 642c 2074 7261 636b 6c65  cell_id, trackle
+00004bd0: 745f 636f 756e 7420 2b20 7374 7228 6929  t_count + str(i)
+00004be0: 202b 2073 7472 2831 2929 0d0a 2020 2020   + str(1))..    
+00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c10: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
+00004c20: 7369 676e 5f74 7261 636b 6c65 745f 6964  sign_tracklet_id
+00004c30: 2874 6172 6765 745f 6365 6c6c 5f69 642c  (target_cell_id,
+00004c40: 2072 6f6f 745f 7370 6c69 7473 2c20 726f   root_splits, ro
+00004c50: 6f74 5f6c 6561 662c 2020 7472 6163 6b6c  ot_leaf,  trackl
+00004c60: 6574 5f63 6f75 6e74 202b 2073 7472 2869  et_count + str(i
+00004c70: 2920 2b20 7374 7228 3129 2029 0d0a 0d0a  ) + str(1) )....
+00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ca0: 2020 2020 0d0a 2020 0d0a 2020 2020 2020      ..  ..      
+00004cb0: 2020 200d 0a20 2020 2064 6566 205f 756e     ..    def _un
+00004cc0: 6971 7565 5f73 706c 6974 5f69 6428 7365  ique_split_id(se
+00004cd0: 6c66 2c20 7461 7267 6574 5f69 642c 2074  lf, target_id, t
+00004ce0: 7261 636b 6c65 745f 636f 756e 7429 3a0d  racklet_count):.
+00004cf0: 0a0d 0a20 2020 2020 2020 2069 6620 7472  ...        if tr
+00004d00: 6163 6b6c 6574 5f63 6f75 6e74 206e 6f74  acklet_count not
+00004d10: 2069 6e20 7365 6c66 2e61 7373 6967 6e65   in self.assigne
+00004d20: 645f 7472 6163 6b65 745f 636f 756e 7473  d_tracket_counts
+00004d30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004d40: 2020 7365 6c66 2e74 7261 636b 6c65 745f    self.tracklet_
+00004d50: 6469 6374 5b74 6172 6765 745f 6964 5d20  dict[target_id] 
+00004d60: 3d20 7374 7228 7472 6163 6b6c 6574 5f63  = str(tracklet_c
+00004d70: 6f75 6e74 290d 0a20 2020 2020 2020 2020  ount)..         
+00004d80: 2020 2020 2020 7365 6c66 2e61 7373 6967        self.assig
+00004d90: 6e65 645f 7472 6163 6b65 745f 636f 756e  ned_tracket_coun
+00004da0: 7473 2e61 7070 656e 6428 7472 6163 6b6c  ts.append(trackl
+00004db0: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
+00004dc0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00004dd0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00004de0: 7472 6163 6b6c 6574 5f63 6f75 6e74 203d  tracklet_count =
+00004df0: 2073 7472 2874 7261 636b 6c65 745f 636f   str(tracklet_co
+00004e00: 756e 7429 202b 2073 7472 2831 290d 0a20  unt) + str(1).. 
+00004e10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004e20: 5f75 6e69 7175 655f 7370 6c69 745f 6964  _unique_split_id
+00004e30: 2874 6172 6765 745f 6964 2c20 7472 6163  (target_id, trac
+00004e40: 6b6c 6574 5f63 6f75 6e74 290d 0a0d 0a0d  klet_count).....
+00004e50: 0a20 2020 2064 6566 205f 6469 7374 616e  .    def _distan
+00004e60: 6365 5f72 6f6f 745f 6c65 6166 2873 656c  ce_root_leaf(sel
+00004e70: 662c 2072 6f6f 745f 726f 6f74 2c20 726f  f, root_root, ro
+00004e80: 6f74 5f6c 6561 662c 2072 6f6f 745f 7370  ot_leaf, root_sp
+00004e90: 6c69 7473 293a 0d0a 0d0a 0d0a 2020 2020  lits):......    
+00004ea0: 2020 2020 0d0a 2020 2020 2020 2020 2067      ..         g
+00004eb0: 656e 5f63 6f75 6e74 203d 2030 0d0a 2020  en_count = 0..  
+00004ec0: 2020 2020 2020 2066 6f72 2072 6f6f 745f         for root_
+00004ed0: 616c 6c20 696e 2072 6f6f 745f 726f 6f74  all in root_root
+00004ee0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004ef0: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00004f00: 6f6e 5f64 6963 745b 726f 6f74 5f61 6c6c  on_dict[root_all
+00004f10: 5d20 3d20 300d 0a20 2020 2020 2020 2020  ] = 0..         
+00004f20: 2020 2020 2020 2069 6620 726f 6f74 5f61         if root_a
+00004f30: 6c6c 2069 6e20 7365 6c66 2e65 6467 655f  ll in self.edge_
+00004f40: 7461 7267 6574 5f6c 6f6f 6b75 703a 0d0a  target_lookup:..
 00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004f70: 5f72 6563 7572 7369 7665 5f70 6174 6828  _recursive_path(
-00004f80: 7461 7267 6574 5f63 656c 6c5f 6964 2c20  target_cell_id, 
-00004f90: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
-00004fa0: 745f 6c65 6166 2c20 6765 6e5f 636f 756e  t_leaf, gen_coun
-00004fb0: 7420 290d 0a0d 0a20 2020 2020 2020 2020  t )....         
-00004fc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004f60: 2020 2074 6172 6765 745f 6365 6c6c 7320     target_cells 
+00004f70: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
+00004f80: 6574 5f6c 6f6f 6b75 705b 726f 6f74 5f61  et_lookup[root_a
+00004f90: 6c6c 5d0d 0a20 2020 2020 2020 2020 2020  ll]..           
+00004fa0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00004fb0: 2072 616e 6765 286c 656e 2874 6172 6765   range(len(targe
+00004fc0: 745f 6365 6c6c 7329 293a 0d0a 2020 2020  t_cells)):..    
 00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 0d0a 2020 2020 2341 7373 6967 6e20 6765  ..    #Assign ge
-00004ff0: 6e65 7261 7469 6f6e 2049 4420 746f 2065  neration ID to e
-00005000: 6163 6820 6365 6c6c 2020 2020 2020 2020  ach cell        
-00005010: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-00005020: 205f 7265 6375 7273 6976 655f 7061 7468   _recursive_path
-00005030: 2873 656c 662c 2074 6172 6765 745f 6964  (self, target_id
-00005040: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
-00005050: 6f6f 745f 6c65 6166 2c20 6765 6e5f 636f  oot_leaf, gen_co
-00005060: 756e 7420 293a 0d0a 2020 2020 2020 2020  unt ):..        
-00005070: 200d 0a20 2020 2020 2020 2069 6620 7461   ..        if ta
-00005080: 7267 6574 5f69 6420 696e 2072 6f6f 745f  rget_id in root_
-00005090: 6c65 6166 3a0d 0a20 2020 2020 2020 2020  leaf:..         
-000050a0: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
-000050b0: 6174 696f 6e5f 6469 6374 5b74 6172 6765  ation_dict[targe
-000050c0: 745f 6964 5d20 3d20 2067 656e 5f63 6f75  t_id] =  gen_cou
-000050d0: 6e74 0d0a 2020 2020 2020 200d 0a20 2020  nt..       ..   
-000050e0: 2020 2020 2069 6620 7461 7267 6574 5f69       if target_i
-000050f0: 6420 6e6f 7420 696e 2072 6f6f 745f 6c65  d not in root_le
-00005100: 6166 3a20 200d 0a20 2020 2020 2020 2020  af:  ..         
-00005110: 2020 2069 6620 7461 7267 6574 5f69 6420     if target_id 
-00005120: 6e6f 7420 696e 2072 6f6f 745f 7370 6c69  not in root_spli
-00005130: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
-00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005150: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00005160: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005170: 656c 662e 6765 6e65 7261 7469 6f6e 5f64  elf.generation_d
-00005180: 6963 745b 7461 7267 6574 5f69 645d 203d  ict[target_id] =
-00005190: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
-000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051b0: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
-000051c0: 745f 6964 2069 6e20 7365 6c66 2e65 6467  t_id in self.edg
-000051d0: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
-000051e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005200: 2020 7461 7267 6574 5f63 656c 6c73 203d    target_cells =
-00005210: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
-00005220: 745f 6c6f 6f6b 7570 5b74 6172 6765 745f  t_lookup[target_
-00005230: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
-00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005250: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00005260: 6e67 6528 6c65 6e28 7461 7267 6574 5f63  nge(len(target_c
-00005270: 656c 6c73 2929 3a0d 0a20 2020 2020 2020  ells)):..       
-00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005290: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-000052a0: 6765 745f 6365 6c6c 5f69 6420 3d20 7461  get_cell_id = ta
-000052b0: 7267 6574 5f63 656c 6c73 5b69 5d0d 0a20  rget_cells[i].. 
-000052c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052e0: 2020 2073 656c 662e 5f72 6563 7572 7369     self._recursi
-000052f0: 7665 5f70 6174 6828 7461 7267 6574 5f63  ve_path(target_c
-00005300: 656c 6c5f 6964 2c20 726f 6f74 5f73 706c  ell_id, root_spl
-00005310: 6974 732c 2072 6f6f 745f 6c65 6166 2c20  its, root_leaf, 
-00005320: 6765 6e5f 636f 756e 7420 3d20 6765 6e5f  gen_count = gen_
-00005330: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-00005340: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
-00005350: 2069 6e20 726f 6f74 5f73 706c 6974 733a   in root_splits:
-00005360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053a0: 2020 2020 2020 2020 2020 2020 6765 6e5f              gen_
-000053b0: 636f 756e 7420 3d20 6765 6e5f 636f 756e  count = gen_coun
-000053c0: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
-000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000053f0: 6765 6e65 7261 7469 6f6e 5f64 6963 745b  generation_dict[
-00005400: 7461 7267 6574 5f69 645d 203d 2067 656e  target_id] = gen
-00005410: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
-00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005430: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00005440: 6172 6765 745f 6964 2069 6e20 7365 6c66  arget_id in self
-00005450: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-00005460: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005480: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00005490: 7267 6574 5f63 656c 6c73 203d 2073 656c  rget_cells = sel
-000054a0: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
-000054b0: 6f6b 7570 5b74 6172 6765 745f 6964 5d0d  okup[target_id].
-000054c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004fe0: 2020 2020 7461 7267 6574 5f63 656c 6c5f      target_cell_
+00004ff0: 6964 203d 2074 6172 6765 745f 6365 6c6c  id = target_cell
+00005000: 735b 695d 0d0a 2020 2020 2020 2020 2020  s[i]..          
+00005010: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005020: 2074 6172 6765 745f 6365 6c6c 5f69 6420   target_cell_id 
+00005030: 6e6f 7420 696e 2072 6f6f 745f 7370 6c69  not in root_spli
+00005040: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005060: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005080: 2020 2020 2073 656c 662e 5f72 6563 7572       self._recur
+00005090: 7369 7665 5f70 6174 6828 7461 7267 6574  sive_path(target
+000050a0: 5f63 656c 6c5f 6964 2c20 726f 6f74 5f73  _cell_id, root_s
+000050b0: 706c 6974 732c 2072 6f6f 745f 6c65 6166  plits, root_leaf
+000050c0: 2c20 6765 6e5f 636f 756e 7420 290d 0a20  , gen_count ).. 
+000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050e0: 2020 2020 2020 2069 6620 7461 7267 6574         if target
+000050f0: 5f63 656c 6c5f 6964 2069 6e20 726f 6f74  _cell_id in root
+00005100: 5f73 706c 6974 733a 0d0a 2020 2020 2020  _splits:..      
+00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005130: 2067 656e 5f63 6f75 6e74 203d 2067 656e   gen_count = gen
+00005140: 5f63 6f75 6e74 202b 2031 0d0a 2020 2020  _count + 1..    
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005170: 2020 2073 656c 662e 5f72 6563 7572 7369     self._recursi
+00005180: 7665 5f70 6174 6828 7461 7267 6574 5f63  ve_path(target_c
+00005190: 656c 6c5f 6964 2c20 726f 6f74 5f73 706c  ell_id, root_spl
+000051a0: 6974 732c 2072 6f6f 745f 6c65 6166 2c20  its, root_leaf, 
+000051b0: 6765 6e5f 636f 756e 7420 290d 0a0d 0a20  gen_count ).... 
+000051c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051e0: 2020 2020 2020 2020 0d0a 2020 2020 2341          ..    #A
+000051f0: 7373 6967 6e20 6765 6e65 7261 7469 6f6e  ssign generation
+00005200: 2049 4420 746f 2065 6163 6820 6365 6c6c   ID to each cell
+00005210: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00005220: 0a20 2020 2064 6566 205f 7265 6375 7273  .    def _recurs
+00005230: 6976 655f 7061 7468 2873 656c 662c 2074  ive_path(self, t
+00005240: 6172 6765 745f 6964 2c20 726f 6f74 5f73  arget_id, root_s
+00005250: 706c 6974 732c 2072 6f6f 745f 6c65 6166  plits, root_leaf
+00005260: 2c20 6765 6e5f 636f 756e 7420 293a 0d0a  , gen_count ):..
+00005270: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00005280: 2020 2069 6620 7461 7267 6574 5f69 6420     if target_id 
+00005290: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
+000052a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000052b0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+000052c0: 6374 5b74 6172 6765 745f 6964 5d20 3d20  ct[target_id] = 
+000052d0: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
+000052e0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+000052f0: 7461 7267 6574 5f69 6420 6e6f 7420 696e  target_id not in
+00005300: 2072 6f6f 745f 6c65 6166 3a20 200d 0a20   root_leaf:  .. 
+00005310: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+00005320: 7267 6574 5f69 6420 6e6f 7420 696e 2072  rget_id not in r
+00005330: 6f6f 745f 7370 6c69 7473 3a0d 0a20 2020  oot_splits:..   
+00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005350: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005370: 2020 2020 2020 2073 656c 662e 6765 6e65         self.gene
+00005380: 7261 7469 6f6e 5f64 6963 745b 7461 7267  ration_dict[targ
+00005390: 6574 5f69 645d 203d 2067 656e 5f63 6f75  et_id] = gen_cou
+000053a0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053c0: 6966 2074 6172 6765 745f 6964 2069 6e20  if target_id in 
+000053d0: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
+000053e0: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
+000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005400: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00005410: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
+00005420: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00005430: 5b74 6172 6765 745f 6964 5d0d 0a20 2020  [target_id]..   
+00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005450: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00005460: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00005470: 7461 7267 6574 5f63 656c 6c73 2929 3a0d  target_cells)):.
+00005480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054a0: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
+000054b0: 5f69 6420 3d20 7461 7267 6574 5f63 656c  _id = target_cel
+000054c0: 6c73 5b69 5d0d 0a20 2020 2020 2020 2020  ls[i]..         
 000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000054f0: 6e20 7261 6e67 6528 6c65 6e28 7461 7267  n range(len(targ
-00005500: 6574 5f63 656c 6c73 2929 3a0d 0a20 2020  et_cells)):..   
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005530: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00005540: 6365 6c6c 5f69 6420 3d20 7461 7267 6574  cell_id = target
-00005550: 5f63 656c 6c73 5b69 5d0d 0a20 2020 2020  _cells[i]..     
-00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000054f0: 5f72 6563 7572 7369 7665 5f70 6174 6828  _recursive_path(
+00005500: 7461 7267 6574 5f63 656c 6c5f 6964 2c20  target_cell_id, 
+00005510: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
+00005520: 745f 6c65 6166 2c20 6765 6e5f 636f 756e  t_leaf, gen_coun
+00005530: 7420 3d20 6765 6e5f 636f 756e 7429 0d0a  t = gen_count)..
+00005540: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00005550: 6172 6765 745f 6964 2069 6e20 726f 6f74  arget_id in root
+00005560: 5f73 706c 6974 733a 0d0a 2020 2020 2020  _splits:..      
 00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005580: 2020 2020 2020 2073 656c 662e 5f72 6563         self._rec
-00005590: 7572 7369 7665 5f70 6174 6828 7461 7267  ursive_path(targ
-000055a0: 6574 5f63 656c 6c5f 6964 2c20 726f 6f74  et_cell_id, root
-000055b0: 5f73 706c 6974 732c 2072 6f6f 745f 6c65  _splits, root_le
-000055c0: 6166 2c20 6765 6e5f 636f 756e 7420 3d20  af, gen_count = 
-000055d0: 6765 6e5f 636f 756e 7429 0d0a 0d0a 2020  gen_count)....  
+00005580: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055b0: 2020 2020 6765 6e5f 636f 756e 7420 3d20      gen_count = 
+000055c0: 6765 6e5f 636f 756e 7420 2b20 310d 0a20  gen_count + 1.. 
+000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005600: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005620: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000055f0: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00005600: 6f6e 5f64 6963 745b 7461 7267 6574 5f69  on_dict[target_i
+00005610: 645d 203d 2067 656e 5f63 6f75 6e74 0d0a  d] = gen_count..
+00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005640: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-00005650: 5f67 6574 5f62 6f75 6e64 6172 795f 6469  _get_boundary_di
-00005660: 7374 2873 656c 662c 2066 7261 6d65 2c20  st(self, frame, 
-00005670: 7465 7374 6c6f 6361 7469 6f6e 293a 0d0a  testlocation):..
-00005680: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00005690: 2020 2069 6620 7365 6c66 2e6d 6173 6b20     if self.mask 
-000056a0: 6973 206e 6f74 204e 6f6e 653a 0d0a 0d0a  is not None:....
-000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056c0: 7472 6565 2c20 696e 6469 6365 732c 206d  tree, indices, m
-000056d0: 6173 6b63 656e 7472 6f69 6420 3d20 7365  askcentroid = se
-000056e0: 6c66 2e74 696d 6564 5f6d 6173 6b5b 7374  lf.timed_mask[st
-000056f0: 7228 696e 7428 666c 6f61 7428 6672 616d  r(int(float(fram
-00005700: 6529 2929 5d0d 0a20 2020 2020 2020 2020  e)))]..         
-00005710: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00005720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005730: 2023 2047 6574 2074 6865 206c 6f63 6174   # Get the locat
-00005740: 696f 6e20 616e 6420 6469 7374 616e 6365  ion and distance
-00005750: 2074 6f20 7468 6520 6e65 6172 6573 7420   to the nearest 
-00005760: 626f 756e 6461 7279 2070 6f69 6e74 0d0a  boundary point..
+00005640: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
+00005650: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
+00005660: 7267 6574 5f6c 6f6f 6b75 703a 0d0a 2020  rget_lookup:..  
+00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005690: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
+000056a0: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
+000056b0: 6172 6765 745f 6c6f 6f6b 7570 5b74 6172  arget_lookup[tar
+000056c0: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
+000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00005700: 6c65 6e28 7461 7267 6574 5f63 656c 6c73  len(target_cells
+00005710: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00005720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005740: 2074 6172 6765 745f 6365 6c6c 5f69 6420   target_cell_id 
+00005750: 3d20 7461 7267 6574 5f63 656c 6c73 5b69  = target_cells[i
+00005760: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
 00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00005790: 736b 2c20 6c6f 6361 7469 6f6e 696e 6465  sk, locationinde
-000057a0: 7820 3d20 7472 6565 2e71 7565 7279 2874  x = tree.query(t
-000057b0: 6573 746c 6f63 6174 696f 6e29 0d0a 2020  estlocation)..  
-000057c0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-000057d0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000057e0: 203d 206d 6178 2830 2c20 6469 7374 616e   = max(0, distan
-000057f0: 6365 5f63 656c 6c5f 6d61 736b 290d 0a20  ce_cell_mask).. 
-00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005810: 2020 0d0a 2020 2020 2020 2020 656c 7365    ..        else
-00005820: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005830: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
-00005840: 5f6d 6173 6b20 3d20 300d 0a20 2020 2020  _mask = 0..     
-00005850: 2020 2020 2020 2020 2020 206d 6173 6b63             maskc
-00005860: 656e 7472 6f69 6420 3d20 2831 2c31 2c31  entroid = (1,1,1
-00005870: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
-00005880: 7572 6e20 6469 7374 616e 6365 5f63 656c  urn distance_cel
-00005890: 6c5f 6d61 736b 2c20 6d61 736b 6365 6e74  l_mask, maskcent
-000058a0: 726f 6964 2020 2020 2020 2020 0d0a 2020  roid        ..  
-000058b0: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
-000058c0: 6566 205f 7472 6163 6b5f 636f 6d70 7574  ef _track_comput
-000058d0: 6572 2873 656c 662c 2074 7261 636b 2c20  er(self, track, 
-000058e0: 7472 6163 6b5f 6964 293a 0d0a 2020 2020  track_id):..    
-000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005900: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00005780: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005790: 656c 662e 5f72 6563 7572 7369 7665 5f70  elf._recursive_p
+000057a0: 6174 6828 7461 7267 6574 5f63 656c 6c5f  ath(target_cell_
+000057b0: 6964 2c20 726f 6f74 5f73 706c 6974 732c  id, root_splits,
+000057c0: 2072 6f6f 745f 6c65 6166 2c20 6765 6e5f   root_leaf, gen_
+000057d0: 636f 756e 7420 3d20 6765 6e5f 636f 756e  count = gen_coun
+000057e0: 7429 0d0a 0d0a 2020 2020 2020 2020 2020  t)....          
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005800: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005840: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00005850: 2020 2020 6465 6620 5f67 6574 5f62 6f75      def _get_bou
+00005860: 6e64 6172 795f 6469 7374 2873 656c 662c  ndary_dist(self,
+00005870: 2066 7261 6d65 2c20 7465 7374 6c6f 6361   frame, testloca
+00005880: 7469 6f6e 293a 0d0a 2020 2020 2020 2020  tion):..        
+00005890: 200d 0a20 2020 2020 2020 2069 6620 7365   ..        if se
+000058a0: 6c66 2e6d 6173 6b20 6973 206e 6f74 204e  lf.mask is not N
+000058b0: 6f6e 653a 0d0a 0d0a 2020 2020 2020 2020  one:....        
+000058c0: 2020 2020 2020 2020 7472 6565 2c20 696e          tree, in
+000058d0: 6469 6365 732c 206d 6173 6b63 656e 7472  dices, maskcentr
+000058e0: 6f69 6420 3d20 7365 6c66 2e74 696d 6564  oid = self.timed
+000058f0: 5f6d 6173 6b5b 7374 7228 696e 7428 666c  _mask[str(int(fl
+00005900: 6f61 7428 6672 616d 6529 2929 5d0d 0a20  oat(frame)))].. 
 00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005920: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
-00005950: 6c5f 6964 7320 3d20 5b5d 0d0a 2020 2020  l_ids = []..    
-00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005970: 2020 2020 2020 2020 756e 6971 7565 5f74          unique_t
-00005980: 7261 636b 6c65 745f 6964 7320 3d20 5b5d  racklet_ids = []
-00005990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000059a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059c0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-000059d0: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
-000059e0: 7461 7267 6574 5f69 6473 203d 2020 7365  target_ids =  se
-000059f0: 6c66 2e5f 6765 6e65 7261 7465 5f67 656e  lf._generate_gen
-00005a00: 6572 6174 696f 6e73 2874 7261 636b 290d  erations(track).
-00005a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005a20: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00005a30: 745f 726f 6f74 2c20 726f 6f74 5f73 706c  t_root, root_spl
-00005a40: 6974 732c 2072 6f6f 745f 6c65 6166 203d  its, root_leaf =
-00005a50: 2073 656c 662e 5f63 7265 6174 655f 6765   self._create_ge
-00005a60: 6e65 7261 7469 6f6e 7328 616c 6c5f 736f  nerations(all_so
-00005a70: 7572 6365 5f69 6473 2c20 616c 6c5f 7461  urce_ids, all_ta
-00005a80: 7267 6574 5f69 6473 2920 0d0a 2020 2020  rget_ids) ..    
-00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005aa0: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-00005ab0: 6572 6174 655f 7370 6c69 745f 646f 776e  erate_split_down
-00005ac0: 2872 6f6f 745f 726f 6f74 2c20 726f 6f74  (root_root, root
-00005ad0: 5f6c 6561 662c 2072 6f6f 745f 7370 6c69  _leaf, root_spli
-00005ae0: 7473 290d 0a20 2020 2020 2020 2020 2020  ts)..           
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00005b10: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00005b20: 756d 6265 725f 6469 7669 6469 6e67 203d  umber_dividing =
-00005b30: 206c 656e 2872 6f6f 745f 7370 6c69 7473   len(root_splits
-00005b40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005b50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005b60: 2044 6574 6572 6d69 6e65 2069 6620 6120   Determine if a 
-00005b70: 7472 6163 6b20 6861 7320 6469 7669 7369  track has divisi
-00005b80: 6f6e 7320 6f72 206e 6f6e 650d 0a20 2020  ons or none..   
-00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ba0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00005bb0: 726f 6f74 5f73 706c 6974 7329 203e 2030  root_splits) > 0
-00005bc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005be0: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00005bf0: 7261 636b 5f6d 6974 6f73 6973 5f6c 6162  rack_mitosis_lab
-00005c00: 656c 5b74 7261 636b 5f69 645d 203d 205b  el[track_id] = [
-00005c10: 312c 206e 756d 6265 725f 6469 7669 6469  1, number_dividi
-00005c20: 6e67 5d0d 0a20 2020 2020 2020 2020 2020  ng]..           
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 2020 2064 6976 6964 696e 675f 7472       dividing_tr
-00005c50: 616a 6563 746f 7279 203d 2054 7275 650d  ajectory = True.
-00005c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
-00005c90: 2920 6e6f 7420 696e 2073 656c 662e 416c  ) not in self.Al
-00005ca0: 6c54 7261 636b 4964 733a 0d0a 2020 2020  lTrackIds:..    
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-00005ce0: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
-00005cf0: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
-00005d20: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
-00005d30: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
-00005d40: 636b 4964 733a 2020 2020 200d 0a20 2020  ckIds:     ..   
+00005930: 2020 2020 2020 2020 2023 2047 6574 2074           # Get t
+00005940: 6865 206c 6f63 6174 696f 6e20 616e 6420  he location and 
+00005950: 6469 7374 616e 6365 2074 6f20 7468 6520  distance to the 
+00005960: 6e65 6172 6573 7420 626f 756e 6461 7279  nearest boundary
+00005970: 2070 6f69 6e74 0d0a 2020 2020 2020 2020   point..        
+00005980: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+00005990: 5f63 656c 6c5f 6d61 736b 2c20 6c6f 6361  _cell_mask, loca
+000059a0: 7469 6f6e 696e 6465 7820 3d20 7472 6565  tionindex = tree
+000059b0: 2e71 7565 7279 2874 6573 746c 6f63 6174  .query(testlocat
+000059c0: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+000059d0: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
+000059e0: 656c 6c5f 6d61 736b 203d 206d 6178 2830  ell_mask = max(0
+000059f0: 2c20 6469 7374 616e 6365 5f63 656c 6c5f  , distance_cell_
+00005a00: 6d61 736b 290d 0a20 2020 2020 2020 2020  mask)..         
+00005a10: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00005a20: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00005a30: 2020 2020 2020 2020 2020 2064 6973 7461             dista
+00005a40: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00005a50: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+00005a60: 2020 206d 6173 6b63 656e 7472 6f69 6420     maskcentroid 
+00005a70: 3d20 2831 2c31 2c31 290d 0a0d 0a20 2020  = (1,1,1)....   
+00005a80: 2020 2020 2072 6574 7572 6e20 6469 7374       return dist
+00005a90: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+00005aa0: 6d61 736b 6365 6e74 726f 6964 2020 2020  maskcentroid    
+00005ab0: 2020 2020 0d0a 2020 2020 2020 2020 200d      ..         .
+00005ac0: 0a0d 0a20 2020 2064 6566 205f 7472 6163  ...    def _trac
+00005ad0: 6b5f 636f 6d70 7574 6572 2873 656c 662c  k_computer(self,
+00005ae0: 2074 7261 636b 2c20 7472 6163 6b5f 6964   track, track_id
+00005af0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b10: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00005b20: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00005b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005b40: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00005b50: 7265 6e74 5f63 656c 6c5f 6964 7320 3d20  rent_cell_ids = 
+00005b60: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b80: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
+00005b90: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
+00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bb0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bd0: 2020 2020 616c 6c5f 736f 7572 6365 5f69      all_source_i
+00005be0: 6473 2c20 616c 6c5f 7461 7267 6574 5f69  ds, all_target_i
+00005bf0: 6473 203d 2020 7365 6c66 2e5f 6765 6e65  ds =  self._gene
+00005c00: 7261 7465 5f67 656e 6572 6174 696f 6e73  rate_generations
+00005c10: 2874 7261 636b 290d 0a20 2020 2020 2020  (track)..       
+00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 2020 2020 2072 6f6f 745f 726f 6f74 2c20       root_root, 
+00005c40: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
+00005c50: 745f 6c65 6166 203d 2073 656c 662e 5f63  t_leaf = self._c
+00005c60: 7265 6174 655f 6765 6e65 7261 7469 6f6e  reate_generation
+00005c70: 7328 616c 6c5f 736f 7572 6365 5f69 6473  s(all_source_ids
+00005c80: 2c20 616c 6c5f 7461 7267 6574 5f69 6473  , all_target_ids
+00005c90: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cb0: 7365 6c66 2e5f 6974 6572 6174 655f 7370  self._iterate_sp
+00005cc0: 6c69 745f 646f 776e 2872 6f6f 745f 726f  lit_down(root_ro
+00005cd0: 6f74 2c20 726f 6f74 5f6c 6561 662c 2072  ot, root_leaf, r
+00005ce0: 6f6f 745f 7370 6c69 7473 290d 0a20 2020  oot_splits)..   
+00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d00: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d20: 2020 2020 2020 206e 756d 6265 725f 6469         number_di
+00005d30: 7669 6469 6e67 203d 206c 656e 2872 6f6f  viding = len(roo
+00005d40: 745f 7370 6c69 7473 290d 0a20 2020 2020  t_splits)..     
 00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d70: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-00005d80: 6163 6b49 6473 2e61 7070 656e 6428 696e  ackIds.append(in
-00005d90: 7428 7472 6163 6b5f 6964 2929 0d0a 2020  t(track_id))..  
+00005d60: 2020 2020 2020 2023 2044 6574 6572 6d69         # Determi
+00005d70: 6e65 2069 6620 6120 7472 6163 6b20 6861  ne if a track ha
+00005d80: 7320 6469 7669 7369 6f6e 7320 6f72 206e  s divisions or n
+00005d90: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
 00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005db0: 2069 6620 6c65 6e28 726f 6f74 5f73 706c   if len(root_spl
+00005dc0: 6974 7329 203e 2030 3a0d 0a20 2020 2020  its) > 0:..     
 00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005de0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005e10: 756e 6971 7565 5f74 7261 636b 5f6d 6974  unique_track_mit
-00005e20: 6f73 6973 5f6c 6162 656c 5b74 7261 636b  osis_label[track
-00005e30: 5f69 645d 203d 205b 302c 2030 5d0d 0a20  _id] = [0, 0].. 
-00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00005e60: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
-00005e70: 7279 203d 2046 616c 7365 0d0a 2020 2020  ry = False..    
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00005ea0: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
-00005eb0: 2069 6e20 7365 6c66 2e41 6c6c 5472 6163   in self.AllTrac
-00005ec0: 6b49 6473 3a0d 0a20 2020 2020 2020 2020  kIds:..         
-00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005ef0: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
-00005f00: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
-00005f10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f30: 2020 2069 6620 696e 7428 7472 6163 6b5f     if int(track_
-00005f40: 6964 2920 6e6f 7420 696e 2073 656c 662e  id) not in self.
-00005f50: 4e6f 726d 616c 5472 6163 6b49 6473 3a20  NormalTrackIds: 
-00005f60: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f80: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
-00005f90: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
-00005fa0: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
-00005fb0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 2020 666f 7220 6c65 6166 2069 6e20 726f    for leaf in ro
-00005fe0: 6f74 5f6c 6561 663a 0d0a 2020 2020 2020  ot_leaf:..      
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
-00006010: 7263 655f 6c65 6166 203d 2073 656c 662e  rce_leaf = self.
-00006020: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
-00006030: 7570 5b6c 6561 665d 0d0a 2020 2020 2020  up[leaf]..      
-00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006050: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00006060: 7265 6e74 5f63 656c 6c5f 6964 732e 6170  rent_cell_ids.ap
-00006070: 7065 6e64 286c 6561 6629 200d 0a20 2020  pend(leaf) ..   
-00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005de0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005df0: 756e 6971 7565 5f74 7261 636b 5f6d 6974  unique_track_mit
+00005e00: 6f73 6973 5f6c 6162 656c 5b74 7261 636b  osis_label[track
+00005e10: 5f69 645d 203d 205b 312c 206e 756d 6265  _id] = [1, numbe
+00005e20: 725f 6469 7669 6469 6e67 5d0d 0a20 2020  r_dividing]..   
+00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 2020 2020 2020 2020 2020 2020 2064 6976               div
+00005e50: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
+00005e60: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
+00005e90: 7472 6163 6b5f 6964 2920 6e6f 7420 696e  track_id) not in
+00005ea0: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
+00005eb0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ed0: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
+00005ee0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+00005ef0: 696e 7428 7472 6163 6b5f 6964 2929 0d0a  int(track_id))..
+00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
+00005f30: 206e 6f74 2069 6e20 7365 6c66 2e44 6976   not in self.Div
+00005f40: 6964 696e 6754 7261 636b 4964 733a 2020  idingTrackIds:  
+00005f50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f70: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
+00005f80: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
+00005f90: 7070 656e 6428 696e 7428 7472 6163 6b5f  ppend(int(track_
+00005fa0: 6964 2929 0d0a 2020 2020 2020 2020 2020  id))..          
+00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fc0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fe0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00005ff0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006010: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
+00006020: 7261 636b 5f6d 6974 6f73 6973 5f6c 6162  rack_mitosis_lab
+00006030: 656c 5b74 7261 636b 5f69 645d 203d 205b  el[track_id] = [
+00006040: 302c 2030 5d0d 0a20 2020 2020 2020 2020  0, 0]..         
+00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006060: 2020 2020 2020 2064 6976 6964 696e 675f         dividing_
+00006070: 7472 616a 6563 746f 7279 203d 2046 616c  trajectory = Fal
+00006080: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
 00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 7365 6c66 2e5f 6469 6374 5f75 7064 6174  self._dict_updat
-000060b0: 6528 756e 6971 7565 5f74 7261 636b 6c65  e(unique_trackle
-000060c0: 745f 6964 732c 206c 6561 662c 2074 7261  t_ids, leaf, tra
-000060d0: 636b 5f69 642c 2073 6f75 7263 655f 6c65  ck_id, source_le
-000060e0: 6166 2c20 4e6f 6e65 290d 0a20 2020 2020  af, None)..     
-000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006100: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006110: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00006120: 726f 7065 7274 6965 735b 6c65 6166 5d2e  roperties[leaf].
-00006130: 7570 6461 7465 287b 7365 6c66 2e64 6976  update({self.div
-00006140: 6964 696e 675f 6b65 7920 3a20 6469 7669  iding_key : divi
-00006150: 6469 6e67 5f74 7261 6a65 6374 6f72 797d  ding_trajectory}
-00006160: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000060a0: 2020 2020 6966 2069 6e74 2874 7261 636b      if int(track
+000060b0: 5f69 6429 206e 6f74 2069 6e20 7365 6c66  _id) not in self
+000060c0: 2e41 6c6c 5472 6163 6b49 6473 3a0d 0a20  .AllTrackIds:.. 
+000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060f0: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+00006100: 4964 732e 6170 7065 6e64 2869 6e74 2874  Ids.append(int(t
+00006110: 7261 636b 5f69 6429 290d 0a20 2020 2020  rack_id))..     
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00006140: 7428 7472 6163 6b5f 6964 2920 6e6f 7420  t(track_id) not 
+00006150: 696e 2073 656c 662e 4e6f 726d 616c 5472  in self.NormalTr
+00006160: 6163 6b49 6473 3a20 2020 200d 0a20 2020  ackIds:    ..   
 00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006180: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00006190: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000061a0: 735b 6c65 6166 5d2e 7570 6461 7465 287b  s[leaf].update({
-000061b0: 7365 6c66 2e6e 756d 6265 725f 6469 7669  self.number_divi
-000061c0: 6469 6e67 5f6b 6579 203a 206e 756d 6265  ding_key : numbe
-000061d0: 725f 6469 7669 6469 6e67 7d29 0d0a 0d0a  r_dividing})....
-000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00006200: 736f 7572 6365 5f69 6420 696e 2061 6c6c  source_id in all
-00006210: 5f73 6f75 7263 655f 6964 733a 0d0a 2020  _source_ids:..  
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 2020 2020 2020 7461 7267 6574 5f69 6473        target_ids
-00006250: 203d 2073 656c 662e 6564 6765 5f74 6172   = self.edge_tar
-00006260: 6765 745f 6c6f 6f6b 7570 5b73 6f75 7263  get_lookup[sourc
-00006270: 655f 6964 5d0d 0a20 2020 2020 2020 2020  e_id]..         
-00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006290: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000062a0: 7572 7265 6e74 5f63 656c 6c5f 6964 732e  urrent_cell_ids.
-000062b0: 6170 7065 6e64 2873 6f75 7263 655f 6964  append(source_id
-000062c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 2020 2020 2020 2020 2023 526f 6f74             #Root
-000062f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006190: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
+000061a0: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
+000061b0: 7472 6163 6b5f 6964 2929 0d0a 0d0a 2020  track_id))....  
+000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061d0: 2020 2020 2020 2020 2020 666f 7220 6c65            for le
+000061e0: 6166 2069 6e20 726f 6f74 5f6c 6561 663a  af in root_leaf:
+000061f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006210: 2020 2020 2073 6f75 7263 655f 6c65 6166       source_leaf
+00006220: 203d 2073 656c 662e 6564 6765 5f73 6f75   = self.edge_sou
+00006230: 7263 655f 6c6f 6f6b 7570 5b6c 6561 665d  rce_lookup[leaf]
+00006240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006260: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
+00006270: 6c5f 6964 732e 6170 7065 6e64 286c 6561  l_ids.append(lea
+00006280: 6629 200d 0a20 2020 2020 2020 2020 2020  f) ..           
+00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062a0: 2020 2020 2020 2020 7365 6c66 2e5f 6469          self._di
+000062b0: 6374 5f75 7064 6174 6528 756e 6971 7565  ct_update(unique
+000062c0: 5f74 7261 636b 6c65 745f 6964 732c 206c  _tracklet_ids, l
+000062d0: 6561 662c 2074 7261 636b 5f69 642c 2073  eaf, track_id, s
+000062e0: 6f75 7263 655f 6c65 6166 2c20 4e6f 6e65  ource_leaf, None
+000062f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006310: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00006320: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00006330: 7274 6965 735b 736f 7572 6365 5f69 645d  rties[source_id]
-00006340: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
-00006350: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
-00006360: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
-00006370: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000063a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000063b0: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
-000063c0: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
-000063d0: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
-000063e0: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
-000063f0: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
-00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006420: 2069 6620 736f 7572 6365 5f69 6420 6e6f   if source_id no
-00006430: 7420 696e 2061 6c6c 5f74 6172 6765 745f  t in all_target_
-00006440: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006470: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00006310: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00006320: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00006330: 735b 6c65 6166 5d2e 7570 6461 7465 287b  s[leaf].update({
+00006340: 7365 6c66 2e64 6976 6964 696e 675f 6b65  self.dividing_ke
+00006350: 7920 3a20 6469 7669 6469 6e67 5f74 7261  y : dividing_tra
+00006360: 6a65 6374 6f72 797d 290d 0a20 2020 2020  jectory})..     
+00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006380: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006390: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000063a0: 726f 7065 7274 6965 735b 6c65 6166 5d2e  roperties[leaf].
+000063b0: 7570 6461 7465 287b 7365 6c66 2e6e 756d  update({self.num
+000063c0: 6265 725f 6469 7669 6469 6e67 5f6b 6579  ber_dividing_key
+000063d0: 203a 206e 756d 6265 725f 6469 7669 6469   : number_dividi
+000063e0: 6e67 7d29 0d0a 0d0a 2020 2020 2020 2020  ng})....        
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006400: 2020 2020 666f 7220 736f 7572 6365 5f69      for source_i
+00006410: 6420 696e 2061 6c6c 5f73 6f75 7263 655f  d in all_source_
+00006420: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
+00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006440: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00006450: 7267 6574 5f69 6473 203d 2073 656c 662e  rget_ids = self.
+00006460: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00006470: 7570 5b73 6f75 7263 655f 6964 5d0d 0a20  up[source_id].. 
 00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064a0: 2020 2020 2020 2020 666f 7220 7461 7267          for targ
-000064b0: 6574 5f69 6420 696e 2074 6172 6765 745f  et_id in target_
-000064c0: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
+000064a0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+000064b0: 656c 6c5f 6964 732e 6170 7065 6e64 2873  ell_ids.append(s
+000064c0: 6f75 7263 655f 6964 290d 0a20 2020 2020  ource_id)..     
 000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000064e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064f0: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
-00006500: 6963 745f 7570 6461 7465 2875 6e69 7175  ict_update(uniqu
-00006510: 655f 7472 6163 6b6c 6574 5f69 6473 2c20  e_tracklet_ids, 
-00006520: 736f 7572 6365 5f69 642c 2074 7261 636b  source_id, track
-00006530: 5f69 642c 204e 6f6e 652c 2074 6172 6765  _id, None, targe
-00006540: 745f 6964 290d 0a20 2020 2020 2020 2020  t_id)..         
-00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006570: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00006580: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00006590: 7274 6965 735b 7461 7267 6574 5f69 645d  rties[target_id]
-000065a0: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
-000065b0: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
-000065c0: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
-000065d0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00006610: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00006620: 6573 5b74 6172 6765 745f 6964 5d2e 7570  es[target_id].up
-00006630: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
-00006640: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
-00006650: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
-00006660: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00006690: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000064f0: 2020 2023 526f 6f74 0d0a 2020 2020 2020     #Root..      
+00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006520: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00006530: 6f74 5f70 726f 7065 7274 6965 735b 736f  ot_properties[so
+00006540: 7572 6365 5f69 645d 2e75 7064 6174 6528  urce_id].update(
+00006550: 7b73 656c 662e 6469 7669 6469 6e67 5f6b  {self.dividing_k
+00006560: 6579 203a 2064 6976 6964 696e 675f 7472  ey : dividing_tr
+00006570: 616a 6563 746f 7279 7d29 0d0a 2020 2020  ajectory})..    
+00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065a0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000065b0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000065c0: 736f 7572 6365 5f69 645d 2e75 7064 6174  source_id].updat
+000065d0: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
+000065e0: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
+000065f0: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
+00006600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006620: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
+00006630: 6365 5f69 6420 6e6f 7420 696e 2061 6c6c  ce_id not in all
+00006640: 5f74 6172 6765 745f 6964 733a 0d0a 2020  _target_ids:..  
+00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006670: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000066a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066c0: 2023 4e6f 726d 616c 2020 2020 2020 2020   #Normal        
-000066d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000066b0: 666f 7220 7461 7267 6574 5f69 6420 696e  for target_id in
+000066c0: 2074 6172 6765 745f 6964 733a 0d0a 2020   target_ids:..  
+000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 736f 7572 6365 5f73 6f75 7263 655f 6964  source_source_id
-00006710: 203d 2073 656c 662e 6564 6765 5f73 6f75   = self.edge_sou
-00006720: 7263 655f 6c6f 6f6b 7570 5b73 6f75 7263  rce_lookup[sourc
-00006730: 655f 6964 5d0d 0a20 2020 2020 2020 2020  e_id]..         
-00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006700: 2073 656c 662e 5f64 6963 745f 7570 6461   self._dict_upda
+00006710: 7465 2875 6e69 7175 655f 7472 6163 6b6c  te(unique_trackl
+00006720: 6574 5f69 6473 2c20 736f 7572 6365 5f69  et_ids, source_i
+00006730: 642c 2074 7261 636b 5f69 642c 204e 6f6e  d, track_id, Non
+00006740: 652c 2074 6172 6765 745f 6964 290d 0a20  e, target_id).. 
 00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006760: 2020 2020 2066 6f72 2074 6172 6765 745f       for target_
-00006770: 6964 2069 6e20 7461 7267 6574 5f69 6473  id in target_ids
-00006780: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 2020 2020 2020 2073 656c 662e 5f64 6963         self._dic
-000067c0: 745f 7570 6461 7465 2875 6e69 7175 655f  t_update(unique_
-000067d0: 7472 6163 6b6c 6574 5f69 6473 2c20 736f  tracklet_ids, so
-000067e0: 7572 6365 5f69 642c 2074 7261 636b 5f69  urce_id, track_i
-000067f0: 642c 2073 6f75 7263 655f 736f 7572 6365  d, source_source
-00006800: 5f69 642c 2074 6172 6765 745f 6964 2920  _id, target_id) 
-00006810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006840: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00006850: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00006860: 735b 7461 7267 6574 5f69 645d 2e75 7064  s[target_id].upd
-00006870: 6174 6528 7b73 656c 662e 6469 7669 6469  ate({self.dividi
-00006880: 6e67 5f6b 6579 203a 2064 6976 6964 696e  ng_key : dividin
-00006890: 675f 7472 616a 6563 746f 7279 7d29 200d  g_trajectory}) .
-000068a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006780: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00006790: 6f74 5f70 726f 7065 7274 6965 735b 7461  ot_properties[ta
+000067a0: 7267 6574 5f69 645d 2e75 7064 6174 6528  rget_id].update(
+000067b0: 7b73 656c 662e 6469 7669 6469 6e67 5f6b  {self.dividing_k
+000067c0: 6579 203a 2064 6976 6964 696e 675f 7472  ey : dividing_tr
+000067d0: 616a 6563 746f 7279 7d29 0d0a 2020 2020  ajectory})..    
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006800: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006810: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00006820: 7072 6f70 6572 7469 6573 5b74 6172 6765  properties[targe
+00006830: 745f 6964 5d2e 7570 6461 7465 287b 7365  t_id].update({se
+00006840: 6c66 2e6e 756d 6265 725f 6469 7669 6469  lf.number_dividi
+00006850: 6e67 5f6b 6579 203a 206e 756d 6265 725f  ng_key : number_
+00006860: 6469 7669 6469 6e67 7d29 0d0a 2020 2020  dividing})..    
+00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006890: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000068b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000068e0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000068f0: 5b74 6172 6765 745f 6964 5d2e 7570 6461  [target_id].upda
-00006900: 7465 287b 7365 6c66 2e6e 756d 6265 725f  te({self.number_
-00006910: 6469 7669 6469 6e67 5f6b 6579 203a 206e  dividing_key : n
-00006920: 756d 6265 725f 6469 7669 6469 6e67 7d29  umber_dividing})
-00006930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000068c0: 2020 2020 2020 2020 2023 4e6f 726d 616c           #Normal
+000068d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006900: 2020 2020 2020 2020 736f 7572 6365 5f73          source_s
+00006910: 6f75 7263 655f 6964 203d 2073 656c 662e  ource_id = self.
+00006920: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
+00006930: 7570 5b73 6f75 7263 655f 6964 5d0d 0a20  up[source_id].. 
 00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006950: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006980: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006960: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00006970: 2074 6172 6765 745f 6964 2069 6e20 7461   target_id in ta
+00006980: 7267 6574 5f69 6473 3a0d 0a20 2020 2020  rget_ids:..     
 00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069c0: 2020 2020 2066 6f72 2063 7572 7265 6e74       for current
-000069d0: 5f72 6f6f 7420 696e 2072 6f6f 745f 726f  _root in root_ro
-000069e0: 6f74 3a0d 0a20 2020 2020 2020 2020 2020  ot:..           
-000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a00: 2020 2020 2020 2020 7365 6c66 2e72 6f6f          self.roo
-00006a10: 745f 7370 6f74 735b 696e 7428 6375 7272  t_spots[int(curr
-00006a20: 656e 745f 726f 6f74 295d 203d 2073 656c  ent_root)] = sel
-00006a30: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00006a40: 6f70 6572 7469 6573 5b69 6e74 2863 7572  operties[int(cur
-00006a50: 7265 6e74 5f72 6f6f 7429 5d0d 0a20 2020  rent_root)]..   
-00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a90: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00006aa0: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
-00006ab0: 5b69 6e74 2874 7261 636b 5f69 6429 5d20  [int(track_id)] 
-00006ac0: 3d20 6375 7272 656e 745f 6365 6c6c 5f69  = current_cell_i
-00006ad0: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00006b00: 656e 2863 7572 7265 6e74 5f63 656c 6c5f  en(current_cell_
-00006b10: 6964 7329 293a 0d0a 2020 2020 2020 2020  ids)):..        
-00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000069c0: 656c 662e 5f64 6963 745f 7570 6461 7465  elf._dict_update
+000069d0: 2875 6e69 7175 655f 7472 6163 6b6c 6574  (unique_tracklet
+000069e0: 5f69 6473 2c20 736f 7572 6365 5f69 642c  _ids, source_id,
+000069f0: 2074 7261 636b 5f69 642c 2073 6f75 7263   track_id, sourc
+00006a00: 655f 736f 7572 6365 5f69 642c 2074 6172  e_source_id, tar
+00006a10: 6765 745f 6964 2920 0d0a 2020 2020 2020  get_id) ..      
+00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006a50: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00006a60: 726f 7065 7274 6965 735b 7461 7267 6574  roperties[target
+00006a70: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+00006a80: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
+00006a90: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
+00006aa0: 746f 7279 7d29 200d 0a20 2020 2020 2020  tory}) ..       
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ad0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006ae0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00006af0: 6f70 6572 7469 6573 5b74 6172 6765 745f  operties[target_
+00006b00: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00006b10: 2e6e 756d 6265 725f 6469 7669 6469 6e67  .number_dividing
+00006b20: 5f6b 6579 203a 206e 756d 6265 725f 6469  _key : number_di
+00006b30: 7669 6469 6e67 7d29 0d0a 2020 2020 2020  viding})..      
+00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 2020 2020 2020 6b20 3d20 696e 7428 6375        k = int(cu
-00006b70: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
-00006b80: 5d29 2020 2020 0d0a 2020 2020 2020 2020  ])    ..        
-00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ba0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00006bb0: 6469 6374 5f76 616c 7565 7320 3d20 7365  dict_values = se
-00006bc0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00006bd0: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
-00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b60: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b90: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00006ba0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00006bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006bc0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00006bd0: 2063 7572 7265 6e74 5f72 6f6f 7420 696e   current_root in
+00006be0: 2072 6f6f 745f 726f 6f74 3a0d 0a20 2020   root_root:..   
 00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c20: 2020 2020 2020 2074 203d 2069 6e74 2866         t = int(f
-00006c30: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-00006c40: 6c75 6573 5b73 656c 662e 6672 616d 6569  lues[self.framei
-00006c50: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
-00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c70: 2020 2020 2020 2020 2020 2020 2020 7a20                z 
-00006c80: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00006c90: 5f76 616c 7565 735b 7365 6c66 2e7a 706f  _values[self.zpo
-00006ca0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cc0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-00006cd0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00006ce0: 745f 7661 6c75 6573 5b73 656c 662e 7970  t_values[self.yp
-00006cf0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 7820 3d20 666c 6f61 7428 616c 6c5f 6469  x = float(all_di
-00006d30: 6374 5f76 616c 7565 735b 7365 6c66 2e78  ct_values[self.x
-00006d40: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 7365 6c66 2e72 6f6f 745f 7370 6f74 735b  self.root_spots[
+00006c20: 696e 7428 6375 7272 656e 745f 726f 6f74  int(current_root
+00006c30: 295d 203d 2073 656c 662e 756e 6971 7565  )] = self.unique
+00006c40: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00006c50: 5b69 6e74 2863 7572 7265 6e74 5f72 6f6f  [int(current_roo
+00006c60: 7429 5d0d 0a20 2020 2020 2020 2020 2020  t)]..           
+00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00006c90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006ca0: 656c 662e 616c 6c5f 6375 7272 656e 745f  elf.all_current_
+00006cb0: 6365 6c6c 5f69 6473 5b69 6e74 2874 7261  cell_ids[int(tra
+00006cc0: 636b 5f69 6429 5d20 3d20 6375 7272 656e  ck_id)] = curren
+00006cd0: 745f 6365 6c6c 5f69 6473 0d0a 2020 2020  t_cell_ids..    
+00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cf0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00006d00: 2072 616e 6765 286c 656e 2863 7572 7265   range(len(curre
+00006d10: 6e74 5f63 656c 6c5f 6964 7329 293a 0d0a  nt_cell_ids)):..
+00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d70: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d90: 2020 2020 2020 2020 2020 2020 2020 7370                sp
-00006da0: 6f74 5f63 656e 7472 6f69 6420 3d20 2872  ot_centroid = (r
-00006db0: 6f75 6e64 287a 292f 7365 6c66 2e7a 6361  ound(z)/self.zca
-00006dc0: 6c69 6272 6174 696f 6e2c 2072 6f75 6e64  libration, round
-00006dd0: 2879 292f 7365 6c66 2e79 6361 6c69 6272  (y)/self.ycalibr
-00006de0: 6174 696f 6e2c 2072 6f75 6e64 2878 292f  ation, round(x)/
-00006df0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00006e00: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00006d60: 2020 2020 2020 2020 2020 2020 2020 6b20                k 
+00006d70: 3d20 696e 7428 6375 7272 656e 745f 6365  = int(current_ce
+00006d80: 6c6c 5f69 6473 5b69 5d29 2020 2020 0d0a  ll_ids[i])    ..
+00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006db0: 2020 2020 616c 6c5f 6469 6374 5f76 616c      all_dict_val
+00006dc0: 7565 7320 3d20 7365 6c66 2e75 6e69 7175  ues = self.uniqu
+00006dd0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00006de0: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
+00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e00: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 00006e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e20: 2020 2020 2020 2020 6672 616d 655f 7370          frame_sp
-00006e30: 6f74 5f63 656e 7472 6f69 6420 3d20 2874  ot_centroid = (t
-00006e40: 2c72 6f75 6e64 287a 292f 7365 6c66 2e7a  ,round(z)/self.z
-00006e50: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-00006e60: 6e64 2879 292f 7365 6c66 2e79 6361 6c69  nd(y)/self.ycali
-00006e70: 6272 6174 696f 6e2c 2072 6f75 6e64 2878  bration, round(x
-00006e80: 292f 7365 6c66 2e78 6361 6c69 6272 6174  )/self.xcalibrat
-00006e90: 696f 6e29 0d0a 0d0a 2020 2020 2020 2020  ion)....        
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006ec0: 2e75 6e69 7175 655f 7370 6f74 5f63 656e  .unique_spot_cen
-00006ed0: 7472 6f69 645b 6672 616d 655f 7370 6f74  troid[frame_spot
-00006ee0: 5f63 656e 7472 6f69 645d 203d 206b 0d0a  _centroid] = k..
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f10: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00006f20: 7472 6163 6b5f 6365 6e74 726f 6964 5b66  track_centroid[f
-00006f30: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
-00006f40: 6964 5d20 3d20 7472 6163 6b5f 6964 0d0a  id] = track_id..
-00006f50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006e20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00006e30: 203d 2069 6e74 2866 6c6f 6174 2861 6c6c   = int(float(all
+00006e40: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00006e50: 662e 6672 616d 6569 645f 6b65 795d 2929  f.frameid_key]))
+00006e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e80: 2020 2020 2020 7a20 3d20 666c 6f61 7428        z = float(
+00006e90: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00006ea0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00006eb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ed0: 2020 2020 2020 2079 203d 2066 6c6f 6174         y = float
+00006ee0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+00006ef0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00006f00: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f20: 2020 2020 2020 2020 7820 3d20 666c 6f61          x = floa
+00006f30: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+00006f40: 735b 7365 6c66 2e78 706f 7369 645f 6b65  s[self.xposid_ke
+00006f50: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
 00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f70: 2020 2020 2020 6966 2073 7472 2874 2920        if str(t) 
-00006f80: 696e 2073 656c 662e 5f74 696d 6564 5f63  in self._timed_c
-00006f90: 656e 7472 6f69 643a 0d0a 2020 2020 2020  entroid:..      
-00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 2020 2020 2074 7265 652c 2073 706f 745f       tree, spot_
-00006fd0: 6365 6e74 726f 6964 7320 3d20 7365 6c66  centroids = self
-00006fe0: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
-00006ff0: 5b73 7472 2874 295d 0d0a 2020 2020 2020  [str(t)]..      
-00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f70: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00006f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fa0: 2020 2020 2020 7370 6f74 5f63 656e 7472        spot_centr
+00006fb0: 6f69 6420 3d20 2872 6f75 6e64 287a 292f  oid = (round(z)/
+00006fc0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00006fd0: 6e2c 2072 6f75 6e64 2879 292f 7365 6c66  n, round(y)/self
+00006fe0: 2e79 6361 6c69 6272 6174 696f 6e2c 2072  .ycalibration, r
+00006ff0: 6f75 6e64 2878 292f 7365 6c66 2e78 6361  ound(x)/self.xca
+00007000: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
 00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007020: 2020 2020 2073 706f 745f 6365 6e74 726f       spot_centro
-00007030: 6964 732e 6170 7065 6e64 2873 706f 745f  ids.append(spot_
-00007040: 6365 6e74 726f 6964 290d 0a20 2020 2020  centroid)..     
-00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007070: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
-00007080: 7469 616c 2e63 4b44 5472 6565 2873 706f  tial.cKDTree(spo
-00007090: 745f 6365 6e74 726f 6964 7329 0d0a 2020  t_centroids)..  
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007030: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
+00007040: 6f69 6420 3d20 2874 2c72 6f75 6e64 287a  oid = (t,round(z
+00007050: 292f 7365 6c66 2e7a 6361 6c69 6272 6174  )/self.zcalibrat
+00007060: 696f 6e2c 2072 6f75 6e64 2879 292f 7365  ion, round(y)/se
+00007070: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
+00007080: 2072 6f75 6e64 2878 292f 7365 6c66 2e78   round(x)/self.x
+00007090: 6361 6c69 6272 6174 696f 6e29 0d0a 0d0a  calibration)....
 000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-000070d0: 696d 6564 5f63 656e 7472 6f69 645b 7374  imed_centroid[st
-000070e0: 7228 7429 5d20 3d20 7472 6565 2c20 7370  r(t)] = tree, sp
-000070f0: 6f74 5f63 656e 7472 6f69 6473 200d 0a20  ot_centroids .. 
+000070c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000070d0: 7370 6f74 5f63 656e 7472 6f69 645b 6672  spot_centroid[fr
+000070e0: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+000070f0: 645d 203d 206b 0d0a 2020 2020 2020 2020  d] = k..        
 00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007120: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2020 2020 2073 706f 745f 6365 6e74 726f       spot_centro
-00007160: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
-00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007190: 2020 2020 2073 706f 745f 6365 6e74 726f       spot_centro
-000071a0: 6964 732e 6170 7065 6e64 2873 706f 745f  ids.append(spot_
-000071b0: 6365 6e74 726f 6964 290d 0a20 2020 2020  centroid)..     
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071e0: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
-000071f0: 7469 616c 2e63 4b44 5472 6565 2873 706f  tial.cKDTree(spo
-00007200: 745f 6365 6e74 726f 6964 7329 0d0a 2020  t_centroids)..  
+00007110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007120: 2e75 6e69 7175 655f 7472 6163 6b5f 6365  .unique_track_ce
+00007130: 6e74 726f 6964 5b66 7261 6d65 5f73 706f  ntroid[frame_spo
+00007140: 745f 6365 6e74 726f 6964 5d20 3d20 7472  t_centroid] = tr
+00007150: 6163 6b5f 6964 0d0a 0d0a 2020 2020 2020  ack_id....      
+00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007170: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007180: 2073 7472 2874 2920 696e 2073 656c 662e   str(t) in self.
+00007190: 5f74 696d 6564 5f63 656e 7472 6f69 643a  _timed_centroid:
+000071a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071c0: 2020 2020 2020 2020 2020 2020 2074 7265               tre
+000071d0: 652c 2073 706f 745f 6365 6e74 726f 6964  e, spot_centroid
+000071e0: 7320 3d20 7365 6c66 2e5f 7469 6d65 645f  s = self._timed_
+000071f0: 6365 6e74 726f 6964 5b73 7472 2874 295d  centroid[str(t)]
+00007200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007230: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-00007240: 696d 6564 5f63 656e 7472 6f69 645b 7374  imed_centroid[st
-00007250: 7228 7429 5d20 3d20 7472 6565 2c20 7370  r(t)] = tree, sp
-00007260: 6f74 5f63 656e 7472 6f69 6473 0d0a 2020  ot_centroids..  
-00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007280: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00007290: 2020 6465 6620 5f6d 6173 7465 725f 7472    def _master_tr
-000072a0: 6163 6b5f 636f 6d70 7574 6572 2873 656c  ack_computer(sel
-000072b0: 662c 2074 7261 636b 2c20 7472 6163 6b5f  f, track, track_
-000072c0: 6964 293a 0d0a 2020 2020 2020 2020 2020  id):..          
-000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00007310: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00007320: 7572 7265 6e74 5f63 656c 6c5f 6964 7320  urrent_cell_ids 
-00007330: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00007220: 2020 2020 2020 2020 2020 2020 2073 706f               spo
+00007230: 745f 6365 6e74 726f 6964 732e 6170 7065  t_centroids.appe
+00007240: 6e64 2873 706f 745f 6365 6e74 726f 6964  nd(spot_centroid
+00007250: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007270: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00007280: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
+00007290: 5472 6565 2873 706f 745f 6365 6e74 726f  Tree(spot_centro
+000072a0: 6964 7329 0d0a 2020 2020 2020 2020 2020  ids)..          
+000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072d0: 2073 656c 662e 5f74 696d 6564 5f63 656e   self._timed_cen
+000072e0: 7472 6f69 645b 7374 7228 7429 5d20 3d20  troid[str(t)] = 
+000072f0: 7472 6565 2c20 7370 6f74 5f63 656e 7472  tree, spot_centr
+00007300: 6f69 6473 200d 0a20 2020 2020 2020 2020  oids ..         
+00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007320: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00007330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007350: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00007360: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00007370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007380: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00007390: 5f73 6f75 7263 655f 6964 732c 2061 6c6c  _source_ids, all
-000073a0: 5f74 6172 6765 745f 6964 7320 3d20 2073  _target_ids =  s
-000073b0: 656c 662e 5f67 656e 6572 6174 655f 6765  elf._generate_ge
-000073c0: 6e65 7261 7469 6f6e 7328 7472 6163 6b29  nerations(track)
-000073d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000073e0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-000073f0: 6f74 5f72 6f6f 742c 2072 6f6f 745f 7370  ot_root, root_sp
-00007400: 6c69 7473 2c20 726f 6f74 5f6c 6561 6620  lits, root_leaf 
-00007410: 3d20 7365 6c66 2e5f 6372 6561 7465 5f67  = self._create_g
-00007420: 656e 6572 6174 696f 6e73 2861 6c6c 5f73  enerations(all_s
-00007430: 6f75 7263 655f 6964 732c 2061 6c6c 5f74  ource_ids, all_t
-00007440: 6172 6765 745f 6964 7329 200d 0a20 2020  arget_ids) ..   
-00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007460: 2020 2020 2020 2020 2073 656c 662e 5f69           self._i
-00007470: 7465 7261 7465 5f73 706c 6974 5f64 6f77  terate_split_dow
-00007480: 6e28 726f 6f74 5f72 6f6f 742c 2072 6f6f  n(root_root, roo
-00007490: 745f 6c65 6166 2c20 726f 6f74 5f73 706c  t_leaf, root_spl
-000074a0: 6974 7329 0d0a 2020 2020 2020 2020 2020  its)..          
-000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00007350: 2020 2020 2020 2020 2020 2020 2073 706f               spo
+00007360: 745f 6365 6e74 726f 6964 7320 3d20 5b5d  t_centroids = []
+00007370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007390: 2020 2020 2020 2020 2020 2020 2073 706f               spo
+000073a0: 745f 6365 6e74 726f 6964 732e 6170 7065  t_centroids.appe
+000073b0: 6e64 2873 706f 745f 6365 6e74 726f 6964  nd(spot_centroid
+000073c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000073d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073e0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000073f0: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
+00007400: 5472 6565 2873 706f 745f 6365 6e74 726f  Tree(spot_centro
+00007410: 6964 7329 0d0a 2020 2020 2020 2020 2020  ids)..          
+00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007440: 2073 656c 662e 5f74 696d 6564 5f63 656e   self._timed_cen
+00007450: 7472 6f69 645b 7374 7228 7429 5d20 3d20  troid[str(t)] = 
+00007460: 7472 6565 2c20 7370 6f74 5f63 656e 7472  tree, spot_centr
+00007470: 6f69 6473 0d0a 2020 2020 2020 2020 2020  oids..          
+00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007490: 2020 0d0a 0d0a 2020 2020 6465 6620 5f6d    ....    def _m
+000074a0: 6173 7465 725f 7472 6163 6b5f 636f 6d70  aster_track_comp
+000074b0: 7574 6572 2873 656c 662c 2074 7261 636b  uter(self, track
+000074c0: 2c20 7472 6163 6b5f 6964 293a 0d0a 2020  , track_id):..  
 000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074e0: 2320 4465 7465 726d 696e 6520 6966 2061  # Determine if a
-000074f0: 2074 7261 636b 2068 6173 2064 6976 6973   track has divis
-00007500: 696f 6e73 206f 7220 6e6f 6e65 0d0a 2020  ions or none..  
+000074e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007500: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-00007530: 5f64 6976 6964 696e 6720 3d20 6c65 6e28  _dividing = len(
-00007540: 726f 6f74 5f73 706c 6974 7329 0d0a 2020  root_splits)..  
-00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007560: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00007570: 2872 6f6f 745f 7370 6c69 7473 2920 3e20  (root_splits) > 
-00007580: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075a0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000075b0: 7472 6163 6b5f 6d69 746f 7369 735f 6c61  track_mitosis_la
-000075c0: 6265 6c5b 7472 6163 6b5f 6964 5d20 3d20  bel[track_id] = 
-000075d0: 5b31 2c20 6e75 6d62 6572 5f64 6976 6964  [1, number_divid
-000075e0: 696e 675d 0d0a 2020 2020 2020 2020 2020  ing]..          
-000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007600: 2020 2020 2020 6469 7669 6469 6e67 5f74        dividing_t
-00007610: 7261 6a65 6374 6f72 7920 3d20 5472 7565  rajectory = True
-00007620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007640: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
-00007650: 6429 206e 6f74 2069 6e20 7365 6c66 2e41  d) not in self.A
-00007660: 6c6c 5472 6163 6b49 6473 3a0d 0a20 2020  llTrackIds:..   
-00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-000076a0: 732e 6170 7065 6e64 2869 6e74 2874 7261  s.append(int(tra
-000076b0: 636b 5f69 6429 290d 0a20 2020 2020 2020  ck_id))..       
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
-000076e0: 7472 6163 6b5f 6964 2920 6e6f 7420 696e  track_id) not in
-000076f0: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-00007700: 6163 6b49 6473 3a20 2020 2020 0d0a 2020  ackIds:     ..  
-00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007520: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+00007530: 656c 6c5f 6964 7320 3d20 5b5d 0d0a 2020  ell_ids = []..  
+00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007550: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007570: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007590: 2020 2020 2061 6c6c 5f73 6f75 7263 655f       all_source_
+000075a0: 6964 732c 2061 6c6c 5f74 6172 6765 745f  ids, all_target_
+000075b0: 6964 7320 3d20 2073 656c 662e 5f67 656e  ids =  self._gen
+000075c0: 6572 6174 655f 6765 6e65 7261 7469 6f6e  erate_generation
+000075d0: 7328 7472 6163 6b29 0d0a 2020 2020 2020  s(track)..      
+000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075f0: 2020 2020 2020 726f 6f74 5f72 6f6f 742c        root_root,
+00007600: 2072 6f6f 745f 7370 6c69 7473 2c20 726f   root_splits, ro
+00007610: 6f74 5f6c 6561 6620 3d20 7365 6c66 2e5f  ot_leaf = self._
+00007620: 6372 6561 7465 5f67 656e 6572 6174 696f  create_generatio
+00007630: 6e73 2861 6c6c 5f73 6f75 7263 655f 6964  ns(all_source_id
+00007640: 732c 2061 6c6c 5f74 6172 6765 745f 6964  s, all_target_id
+00007650: 7329 200d 0a20 2020 2020 2020 2020 2020  s) ..           
+00007660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007670: 2073 656c 662e 5f69 7465 7261 7465 5f73   self._iterate_s
+00007680: 706c 6974 5f64 6f77 6e28 726f 6f74 5f72  plit_down(root_r
+00007690: 6f6f 742c 2072 6f6f 745f 6c65 6166 2c20  oot, root_leaf, 
+000076a0: 726f 6f74 5f73 706c 6974 7329 0d0a 2020  root_splits)..  
+000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076e0: 2020 2020 2020 2020 2320 4465 7465 726d          # Determ
+000076f0: 696e 6520 6966 2061 2074 7261 636b 2068  ine if a track h
+00007700: 6173 2064 6976 6973 696f 6e73 206f 7220  as divisions or 
+00007710: 6e6f 6e65 0d0a 2020 2020 2020 2020 2020  none..          
 00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007730: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
-00007740: 7261 636b 4964 732e 6170 7065 6e64 2869  rackIds.append(i
-00007750: 6e74 2874 7261 636b 5f69 6429 290d 0a20  nt(track_id)).. 
+00007730: 2020 6e75 6d62 6572 5f64 6976 6964 696e    number_dividin
+00007740: 6720 3d20 6c65 6e28 726f 6f74 5f73 706c  g = len(root_spl
+00007750: 6974 7329 0d0a 2020 2020 2020 2020 2020  its)..          
 00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007780: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00007770: 2020 6966 206c 656e 2872 6f6f 745f 7370    if len(root_sp
+00007780: 6c69 7473 2920 3e20 303a 0d0a 2020 2020  lits) > 0:..    
 00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000077d0: 2e75 6e69 7175 655f 7472 6163 6b5f 6d69  .unique_track_mi
-000077e0: 746f 7369 735f 6c61 6265 6c5b 7472 6163  tosis_label[trac
-000077f0: 6b5f 6964 5d20 3d20 5b30 2c20 305d 0d0a  k_id] = [0, 0]..
-00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
-00007830: 6f72 7920 3d20 4661 6c73 650d 0a20 2020  ory = False..   
-00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00007860: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
-00007870: 7420 696e 2073 656c 662e 416c 6c54 7261  t in self.AllTra
-00007880: 636b 4964 733a 0d0a 2020 2020 2020 2020  ckIds:..        
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000078b0: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
-000078c0: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
-000078d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078f0: 2020 2020 6966 2069 6e74 2874 7261 636b      if int(track
-00007900: 5f69 6429 206e 6f74 2069 6e20 7365 6c66  _id) not in self
-00007910: 2e4e 6f72 6d61 6c54 7261 636b 4964 733a  .NormalTrackIds:
-00007920: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 2020 2020 2020 2020 2020 7365 6c66 2e4e            self.N
-00007950: 6f72 6d61 6c54 7261 636b 4964 732e 6170  ormalTrackIds.ap
-00007960: 7065 6e64 2869 6e74 2874 7261 636b 5f69  pend(int(track_i
-00007970: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
-00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 2020 2066 6f72 206c 6561 6620 696e 2072     for leaf in r
-000079a0: 6f6f 745f 6c65 6166 3a0d 0a20 2020 2020  oot_leaf:..     
-000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000079d0: 6c66 2e5f 7365 636f 6e64 5f63 6861 6e6e  lf._second_chann
-000079e0: 656c 5f75 7064 6174 6528 6c65 6166 2c20  el_update(leaf, 
-000079f0: 7472 6163 6b5f 6964 290d 0a20 2020 2020  track_id)..     
-00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a10: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00007a20: 7272 656e 745f 6365 6c6c 5f69 6473 2e61  rrent_cell_ids.a
-00007a30: 7070 656e 6428 6c65 6166 2920 0d0a 2020  ppend(leaf) ..  
-00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000077b0: 2e75 6e69 7175 655f 7472 6163 6b5f 6d69  .unique_track_mi
+000077c0: 746f 7369 735f 6c61 6265 6c5b 7472 6163  tosis_label[trac
+000077d0: 6b5f 6964 5d20 3d20 5b31 2c20 6e75 6d62  k_id] = [1, numb
+000077e0: 6572 5f64 6976 6964 696e 675d 0d0a 2020  er_dividing]..  
+000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007800: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00007810: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
+00007820: 7920 3d20 5472 7565 0d0a 2020 2020 2020  y = True..      
+00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007840: 2020 2020 2020 2020 2020 6966 2069 6e74            if int
+00007850: 2874 7261 636b 5f69 6429 206e 6f74 2069  (track_id) not i
+00007860: 6e20 7365 6c66 2e41 6c6c 5472 6163 6b49  n self.AllTrackI
+00007870: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007890: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
+000078a0: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+000078b0: 2869 6e74 2874 7261 636b 5f69 6429 290d  (int(track_id)).
+000078c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078e0: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
+000078f0: 2920 6e6f 7420 696e 2073 656c 662e 4469  ) not in self.Di
+00007900: 7669 6469 6e67 5472 6163 6b49 6473 3a20  vidingTrackIds: 
+00007910: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007930: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
+00007940: 6976 6964 696e 6754 7261 636b 4964 732e  ividingTrackIds.
+00007950: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
+00007960: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
+00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007980: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00007990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000079a0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000079b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079d0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000079e0: 7472 6163 6b5f 6d69 746f 7369 735f 6c61  track_mitosis_la
+000079f0: 6265 6c5b 7472 6163 6b5f 6964 5d20 3d20  bel[track_id] = 
+00007a00: 5b30 2c20 305d 0d0a 2020 2020 2020 2020  [0, 0]..        
+00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a20: 2020 2020 2020 2020 6469 7669 6469 6e67          dividing
+00007a30: 5f74 7261 6a65 6374 6f72 7920 3d20 4661  _trajectory = Fa
+00007a40: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
 00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a60: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00007a70: 745f 7072 6f70 6572 7469 6573 5b6c 6561  t_properties[lea
-00007a80: 665d 2e75 7064 6174 6528 7b73 656c 662e  f].update({self.
-00007a90: 6469 7669 6469 6e67 5f6b 6579 203a 2064  dividing_key : d
-00007aa0: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
-00007ab0: 7279 7d29 0d0a 2020 2020 2020 2020 2020  ry})..          
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00007ae0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00007af0: 7469 6573 5b6c 6561 665d 2e75 7064 6174  ties[leaf].updat
-00007b00: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
-00007b10: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
-00007b20: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
-00007b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b40: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00007b50: 2073 6f75 7263 655f 6964 2069 6e20 616c   source_id in al
-00007b60: 6c5f 736f 7572 6365 5f69 6473 3a0d 0a20  l_source_ids:.. 
-00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a60: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
+00007a70: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
+00007a80: 662e 416c 6c54 7261 636b 4964 733a 0d0a  f.AllTrackIds:..
+00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ab0: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+00007ac0: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
+00007ad0: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007af0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00007b00: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
+00007b10: 2069 6e20 7365 6c66 2e4e 6f72 6d61 6c54   in self.NormalT
+00007b20: 7261 636b 4964 733a 2020 2020 0d0a 2020  rackIds:    ..  
+00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b50: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
+00007b60: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
+00007b70: 2874 7261 636b 5f69 6429 290d 0a0d 0a20  (track_id)).... 
 00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b90: 2020 7365 6c66 2e5f 7365 636f 6e64 5f63    self._second_c
-00007ba0: 6861 6e6e 656c 5f75 7064 6174 6528 736f  hannel_update(so
-00007bb0: 7572 6365 5f69 642c 2074 7261 636b 5f69  urce_id, track_i
-00007bc0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00007bf0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00007c00: 6573 5b73 6f75 7263 655f 6964 5d2e 7570  es[source_id].up
-00007c10: 6461 7465 287b 7365 6c66 2e64 6976 6964  date({self.divid
-00007c20: 696e 675f 6b65 7920 3a20 6469 7669 6469  ing_key : dividi
-00007c30: 6e67 5f74 7261 6a65 6374 6f72 797d 290d  ng_trajectory}).
-00007c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b90: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
+00007ba0: 6561 6620 696e 2072 6f6f 745f 6c65 6166  eaf in root_leaf
+00007bb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bd0: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
+00007be0: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
+00007bf0: 6528 6c65 6166 2c20 7472 6163 6b5f 6964  e(leaf, track_id
+00007c00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c20: 2020 2020 2020 6375 7272 656e 745f 6365        current_ce
+00007c30: 6c6c 5f69 6473 2e61 7070 656e 6428 6c65  ll_ids.append(le
+00007c40: 6166 2920 0d0a 2020 2020 2020 2020 2020  af) ..          
 00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c60: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00007c70: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00007c80: 736f 7572 6365 5f69 645d 2e75 7064 6174  source_id].updat
-00007c90: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
-00007ca0: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
-00007cb0: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
-00007cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007c60: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00007c70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00007c80: 7469 6573 5b6c 6561 665d 2e75 7064 6174  ties[leaf].updat
+00007c90: 6528 7b73 656c 662e 6469 7669 6469 6e67  e({self.dividing
+00007ca0: 5f6b 6579 203a 2064 6976 6964 696e 675f  _key : dividing_
+00007cb0: 7472 616a 6563 746f 7279 7d29 0d0a 2020  trajectory})..  
+00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ce0: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
-00007cf0: 5f69 6473 2e61 7070 656e 6428 736f 7572  _ids.append(sour
-00007d00: 6365 5f69 6429 0d0a 2020 2020 2020 2020  ce_id)..        
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00007ce0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00007cf0: 745f 7072 6f70 6572 7469 6573 5b6c 6561  t_properties[lea
+00007d00: 665d 2e75 7064 6174 6528 7b73 656c 662e  f].update({self.
+00007d10: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
+00007d20: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
+00007d30: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
 00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d50: 2020 2020 2020 2020 666f 7220 6375 7272          for curr
-00007d60: 656e 745f 726f 6f74 2069 6e20 726f 6f74  ent_root in root
-00007d70: 5f72 6f6f 743a 0d0a 2020 2020 2020 2020  _root:..        
+00007d50: 2020 2020 2066 6f72 2073 6f75 7263 655f       for source_
+00007d60: 6964 2069 6e20 616c 6c5f 736f 7572 6365  id in all_source
+00007d70: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
 00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007da0: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
-00007db0: 7570 6461 7465 2863 7572 7265 6e74 5f72  update(current_r
-00007dc0: 6f6f 742c 2074 7261 636b 5f69 6429 0d0a  oot, track_id)..
+00007d90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00007da0: 7365 636f 6e64 5f63 6861 6e6e 656c 5f75  second_channel_u
+00007db0: 7064 6174 6528 736f 7572 6365 5f69 642c  pdate(source_id,
+00007dc0: 2074 7261 636b 5f69 6429 0d0a 2020 2020   track_id)..    
 00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007df0: 2020 2073 656c 662e 726f 6f74 5f73 706f     self.root_spo
-00007e00: 7473 5b69 6e74 2863 7572 7265 6e74 5f72  ts[int(current_r
-00007e10: 6f6f 7429 5d20 3d20 7365 6c66 2e75 6e69  oot)] = self.uni
-00007e20: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00007e30: 6965 735b 696e 7428 6375 7272 656e 745f  ies[int(current_
-00007e40: 726f 6f74 295d 0d0a 2020 2020 2020 2020  root)]..        
+00007de0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007df0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00007e00: 7072 6f70 6572 7469 6573 5b73 6f75 7263  properties[sourc
+00007e10: 655f 6964 5d2e 7570 6461 7465 287b 7365  e_id].update({se
+00007e20: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
+00007e30: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
+00007e40: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
 00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007e70: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00007e80: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
-00007e90: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
-00007ea0: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
-00007eb0: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
-00007ec0: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
+00007e60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007e70: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00007e80: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
+00007e90: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00007ea0: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
+00007eb0: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
+00007ec0: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
 00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00007ef0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00007f00: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
-00007f10: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
-00007f20: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
-00007f30: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
-00007f40: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
+00007ee0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00007ef0: 656e 745f 6365 6c6c 5f69 6473 2e61 7070  ent_cell_ids.app
+00007f00: 656e 6428 736f 7572 6365 5f69 6429 0d0a  end(source_id)..
+00007f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f60: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007f80: 656c 662e 616c 6c5f 6375 7272 656e 745f  elf.all_current_
-00007f90: 6365 6c6c 5f69 6473 5b69 6e74 2874 7261  cell_ids[int(tra
-00007fa0: 636b 5f69 6429 5d20 3d20 6375 7272 656e  ck_id)] = curren
-00007fb0: 745f 6365 6c6c 5f69 6473 0d0a 2020 2020  t_cell_ids..    
-00007fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00007f60: 666f 7220 6375 7272 656e 745f 726f 6f74  for current_root
+00007f70: 2069 6e20 726f 6f74 5f72 6f6f 743a 0d0a   in root_root:..
+00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fa0: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
+00007fb0: 6368 616e 6e65 6c5f 7570 6461 7465 2863  channel_update(c
+00007fc0: 7572 7265 6e74 5f72 6f6f 742c 2074 7261  urrent_root, tra
+00007fd0: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
 00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ff0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00008000: 6e67 6528 6c65 6e28 6375 7272 656e 745f  nge(len(current_
-00008010: 6365 6c6c 5f69 6473 2929 3a0d 0a20 2020  cell_ids)):..   
-00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008040: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00007ff0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008000: 726f 6f74 5f73 706f 7473 5b69 6e74 2863  root_spots[int(c
+00008010: 7572 7265 6e74 5f72 6f6f 7429 5d20 3d20  urrent_root)] = 
+00008020: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00008030: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00008040: 6375 7272 656e 745f 726f 6f74 295d 0d0a  current_root)]..
 00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008060: 2020 2020 2020 2020 2020 206b 203d 2069             k = i
-00008070: 6e74 2863 7572 7265 6e74 5f63 656c 6c5f  nt(current_cell_
-00008080: 6964 735b 695d 2920 2020 0d0a 2020 2020  ids[i])   ..    
-00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080d0: 2020 2020 2020 616c 6c5f 6469 6374 5f76        all_dict_v
-000080e0: 616c 7565 7320 3d20 7365 6c66 2e75 6e69  alues = self.uni
-000080f0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00008100: 6965 735b 6b5d 0d0a 2020 2020 2020 2020  ies[k]..        
-00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008120: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008170: 2020 2020 2020 7420 3d20 696e 7428 666c        t = int(fl
-00008180: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00008190: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
-000081a0: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
-000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081c0: 2020 2020 2020 2020 2020 2020 207a 203d               z =
-000081d0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-000081e0: 7661 6c75 6573 5b73 656c 662e 7a70 6f73  values[self.zpos
-000081f0: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008210: 2020 2020 2020 2020 2020 2020 2020 7920                y 
-00008220: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00008230: 5f76 616c 7565 735b 7365 6c66 2e79 706f  _values[self.ypo
-00008240: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008070: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00008080: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
+00008090: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
+000080a0: 287b 7365 6c66 2e64 6976 6964 696e 675f  ({self.dividing_
+000080b0: 6b65 7920 3a20 6469 7669 6469 6e67 5f74  key : dividing_t
+000080c0: 7261 6a65 6374 6f72 797d 290d 0a20 2020  rajectory})..   
+000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080f0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00008100: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
+00008110: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
+00008120: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
+00008130: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
+00008140: 5f64 6976 6964 696e 677d 290d 0a20 2020  _dividing})..   
+00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008160: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008180: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00008190: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
+000081a0: 5b69 6e74 2874 7261 636b 5f69 6429 5d20  [int(track_id)] 
+000081b0: 3d20 6375 7272 656e 745f 6365 6c6c 5f69  = current_cell_i
+000081c0: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
+000081d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000081e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000081f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00008200: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00008210: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
+00008220: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008240: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008260: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00008270: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00008280: 745f 7661 6c75 6573 5b73 656c 662e 7870  t_values[self.xp
-00008290: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008270: 2020 206b 203d 2069 6e74 2863 7572 7265     k = int(curre
+00008280: 6e74 5f63 656c 6c5f 6964 735b 695d 2920  nt_cell_ids[i]) 
+00008290: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 000082a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082e0: 2020 2020 2020 2020 6672 616d 655f 7370          frame_sp
-000082f0: 6f74 5f63 656e 7472 6f69 6420 3d20 2874  ot_centroid = (t
-00008300: 2c72 6f75 6e64 287a 292f 7365 6c66 2e7a  ,round(z)/self.z
-00008310: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-00008320: 6e64 2879 292f 7365 6c66 2e79 6361 6c69  nd(y)/self.ycali
-00008330: 6272 6174 696f 6e2c 2072 6f75 6e64 2878  bration, round(x
-00008340: 292f 7365 6c66 2e78 6361 6c69 6272 6174  )/self.xcalibrat
-00008350: 696f 6e29 200d 0a0d 0a20 2020 2020 2020  ion) ....       
+000082b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082d0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+000082e0: 6c5f 6469 6374 5f76 616c 7565 7320 3d20  l_dict_values = 
+000082f0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00008300: 5f70 726f 7065 7274 6965 735b 6b5d 0d0a  _properties[k]..
+00008310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008330: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008350: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008370: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008380: 662e 756e 6971 7565 5f73 706f 745f 6365  f.unique_spot_ce
-00008390: 6e74 726f 6964 5b66 7261 6d65 5f73 706f  ntroid[frame_spo
-000083a0: 745f 6365 6e74 726f 6964 5d20 3d20 6b0d  t_centroid] = k.
+00008370: 2020 2020 2020 2020 2020 2020 2020 7420                t 
+00008380: 3d20 696e 7428 666c 6f61 7428 616c 6c5f  = int(float(all_
+00008390: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+000083a0: 2e66 7261 6d65 6964 5f6b 6579 5d29 290d  .frameid_key])).
 000083b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083d0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000083e0: 5f74 7261 636b 5f63 656e 7472 6f69 645b  _track_centroid[
-000083f0: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
-00008400: 6f69 645d 203d 2074 7261 636b 5f69 640d  oid] = track_id.
-00008410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008430: 2020 2020 0d0a 2020 2020 6465 6620 5f73      ..    def _s
-00008440: 6563 6f6e 645f 6368 616e 6e65 6c5f 7570  econd_channel_up
-00008450: 6461 7465 2873 656c 662c 2063 656c 6c5f  date(self, cell_
-00008460: 6964 2c20 7472 6163 6b5f 6964 293a 0d0a  id, track_id):..
-00008470: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00008480: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00008490: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
-000084a0: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
-000084b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000084c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000084d0: 2020 2020 6672 616d 6520 3d20 7365 6c66      frame = self
-000084e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000084f0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00008500: 5f69 6429 5d5b 7365 6c66 2e66 7261 6d65  _id)][self.frame
-00008510: 6964 5f6b 6579 5d0d 0a20 2020 2020 2020  id_key]..       
-00008520: 2020 2020 2020 2020 207a 203d 2073 656c           z = sel
-00008530: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00008540: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00008550: 6c5f 6964 295d 5b73 656c 662e 7a70 6f73  l_id)][self.zpos
-00008560: 6964 5f6b 6579 5d2f 7365 6c66 2e7a 6361  id_key]/self.zca
-00008570: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-00008580: 2020 2020 2020 2020 2020 2079 203d 2073             y = s
-00008590: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000085a0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-000085b0: 656c 6c5f 6964 295d 5b73 656c 662e 7970  ell_id)][self.yp
-000085c0: 6f73 6964 5f6b 6579 5d2f 7365 6c66 2e79  osid_key]/self.y
-000085d0: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-000085e0: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-000085f0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00008600: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00008610: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00008620: 7870 6f73 6964 5f6b 6579 5d2f 7365 6c66  xposid_key]/self
-00008630: 2e78 6361 6c69 6272 6174 696f 6e0d 0a20  .xcalibration.. 
-00008640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008650: 656c 662e 5f73 6563 6f6e 645f 6368 616e  elf._second_chan
-00008660: 6e65 6c5f 7370 6f74 7328 6672 616d 652c  nel_spots(frame,
-00008670: 207a 2c20 792c 2078 2c20 6365 6c6c 5f69   z, y, x, cell_i
-00008680: 642c 2074 7261 636b 5f69 6429 0d0a 2020  d, track_id)..  
-00008690: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-000086a0: 5f66 696e 616c 5f74 7261 636b 7328 7365  _final_tracks(se
-000086b0: 6c66 2c20 7472 6163 6b5f 6964 293a 0d0a  lf, track_id):..
-000086c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000086d0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000086e0: 7272 656e 745f 6365 6c6c 5f69 6473 203d  rrent_cell_ids =
-000086f0: 2073 656c 662e 616c 6c5f 6375 7272 656e   self.all_curren
-00008700: 745f 6365 6c6c 5f69 6473 5b69 6e74 2874  t_cell_ids[int(t
-00008710: 7261 636b 5f69 6429 5d0d 0a20 2020 2020  rack_id)]..     
-00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008730: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-00008740: 7261 636b 6c65 7473 203d 207b 7d0d 0a20  racklets = {}.. 
-00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008760: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00008770: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-00008780: 7065 7274 6965 7320 3d20 7b7d 0d0a 2020  perties = {}..  
-00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087c0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-000087d0: 2072 616e 6765 286c 656e 2863 7572 7265   range(len(curre
-000087e0: 6e74 5f63 656c 6c5f 6964 7329 293a 0d0a  nt_cell_ids)):..
-000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008830: 2020 2020 2020 2020 2020 2020 2020 6b20                k 
-00008840: 3d20 696e 7428 6375 7272 656e 745f 6365  = int(current_ce
-00008850: 6c6c 5f69 6473 5b69 5d29 2020 2020 0d0a  ll_ids[i])    ..
-00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008880: 2020 2020 616c 6c5f 6469 6374 5f76 616c      all_dict_val
-00008890: 7565 7320 3d20 7365 6c66 2e75 6e69 7175  ues = self.uniqu
-000088a0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000088b0: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
-000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088d0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-000088e0: 5f69 6420 3d20 7374 7228 616c 6c5f 6469  _id = str(all_di
-000088f0: 6374 5f76 616c 7565 735b 7365 6c66 2e75  ct_values[self.u
-00008900: 6e69 7175 6569 645f 6b65 795d 290d 0a20  niqueid_key]).. 
-00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
-00008940: 5f69 6420 3d20 7374 7228 616c 6c5f 6469  _id = str(all_di
-00008950: 6374 5f76 616c 7565 735b 7365 6c66 2e74  ct_values[self.t
-00008960: 7261 636b 6964 5f6b 6579 5d29 0d0a 2020  rackid_key])..  
-00008970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008990: 2020 7420 3d20 696e 7428 666c 6f61 7428    t = int(float(
-000089a0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-000089b0: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-000089c0: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
-000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2020 2020 2020 207a 203d 2066 6c6f           z = flo
-000089f0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00008a00: 6573 5b73 656c 662e 7a70 6f73 6964 5f6b  es[self.zposid_k
-00008a10: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 2020 2020 2020 2020 7920 3d20 666c            y = fl
-00008a40: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00008a50: 7565 735b 7365 6c66 2e79 706f 7369 645f  ues[self.yposid_
-00008a60: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000083d0: 2020 2020 207a 203d 2066 6c6f 6174 2861       z = float(a
+000083e0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+000083f0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00008400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008420: 2020 2020 2020 7920 3d20 666c 6f61 7428        y = float(
+00008430: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00008440: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+00008450: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008470: 2020 2020 2020 2078 203d 2066 6c6f 6174         x = float
+00008480: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+00008490: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
+000084a0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084c0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
+00008500: 6f69 6420 3d20 2874 2c72 6f75 6e64 287a  oid = (t,round(z
+00008510: 292f 7365 6c66 2e7a 6361 6c69 6272 6174  )/self.zcalibrat
+00008520: 696f 6e2c 2072 6f75 6e64 2879 292f 7365  ion, round(y)/se
+00008530: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
+00008540: 2072 6f75 6e64 2878 292f 7365 6c66 2e78   round(x)/self.x
+00008550: 6361 6c69 6272 6174 696f 6e29 200d 0a0d  calibration) ...
+00008560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008580: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00008590: 5f73 706f 745f 6365 6e74 726f 6964 5b66  _spot_centroid[f
+000085a0: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
+000085b0: 6964 5d20 3d20 6b0d 0a20 2020 2020 2020  id] = k..       
+000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000085e0: 662e 756e 6971 7565 5f74 7261 636b 5f63  f.unique_track_c
+000085f0: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
+00008600: 6f74 5f63 656e 7472 6f69 645d 203d 2074  ot_centroid] = t
+00008610: 7261 636b 5f69 640d 0a20 2020 2020 2020  rack_id..       
+00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008630: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00008640: 2020 6465 6620 5f73 6563 6f6e 645f 6368    def _second_ch
+00008650: 616e 6e65 6c5f 7570 6461 7465 2873 656c  annel_update(sel
+00008660: 662c 2063 656c 6c5f 6964 2c20 7472 6163  f, cell_id, trac
+00008670: 6b5f 6964 293a 0d0a 2020 2020 2020 2020  k_id):..        
+00008680: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008690: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
+000086a0: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
+000086b0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000086c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000086d0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+000086e0: 6520 3d20 7365 6c66 2e75 6e69 7175 655f  e = self.unique_
+000086f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00008700: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00008710: 6c66 2e66 7261 6d65 6964 5f6b 6579 5d0d  lf.frameid_key].
+00008720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008730: 207a 203d 2073 656c 662e 756e 6971 7565   z = self.unique
+00008740: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00008750: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00008760: 656c 662e 7a70 6f73 6964 5f6b 6579 5d2f  elf.zposid_key]/
+00008770: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00008780: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00008790: 2020 2079 203d 2073 656c 662e 756e 6971     y = self.uniq
+000087a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000087b0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+000087c0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+000087d0: 5d2f 7365 6c66 2e79 6361 6c69 6272 6174  ]/self.ycalibrat
+000087e0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+000087f0: 2020 2020 2078 203d 2073 656c 662e 756e       x = self.un
+00008800: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00008810: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00008820: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
+00008830: 6579 5d2f 7365 6c66 2e78 6361 6c69 6272  ey]/self.xcalibr
+00008840: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+00008850: 2020 2020 2020 2073 656c 662e 5f73 6563         self._sec
+00008860: 6f6e 645f 6368 616e 6e65 6c5f 7370 6f74  ond_channel_spot
+00008870: 7328 6672 616d 652c 207a 2c20 792c 2078  s(frame, z, y, x
+00008880: 2c20 6365 6c6c 5f69 642c 2074 7261 636b  , cell_id, track
+00008890: 5f69 6429 0d0a 2020 2020 2020 2020 0d0a  _id)..        ..
+000088a0: 2020 2020 6465 6620 5f66 696e 616c 5f74      def _final_t
+000088b0: 7261 636b 7328 7365 6c66 2c20 7472 6163  racks(self, trac
+000088c0: 6b5f 6964 293a 0d0a 0d0a 2020 2020 2020  k_id):....      
+000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088e0: 2020 2020 2020 6375 7272 656e 745f 6365        current_ce
+000088f0: 6c6c 5f69 6473 203d 2073 656c 662e 616c  ll_ids = self.al
+00008900: 6c5f 6375 7272 656e 745f 6365 6c6c 5f69  l_current_cell_i
+00008910: 6473 5b69 6e74 2874 7261 636b 5f69 6429  ds[int(track_id)
+00008920: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00008930: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00008940: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00008950: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008970: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
+00008980: 6c65 7473 5f70 726f 7065 7274 6965 7320  lets_properties 
+00008990: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089d0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+000089e0: 656e 2863 7572 7265 6e74 5f63 656c 6c5f  en(current_cell_
+000089f0: 6964 7329 293a 0d0a 2020 2020 2020 2020  ids)):..        
+00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a40: 2020 2020 2020 6b20 3d20 696e 7428 6375        k = int(cu
+00008a50: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
+00008a60: 5d29 2020 2020 0d0a 2020 2020 2020 2020  ])    ..        
 00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a80: 2020 2020 2020 2020 2020 2078 203d 2066             x = f
-00008a90: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-00008aa0: 6c75 6573 5b73 656c 662e 7870 6f73 6964  lues[self.xposid
-00008ab0: 5f6b 6579 5d29 0d0a 0d0a 2020 2020 2020  _key])....      
+00008a80: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00008a90: 6469 6374 5f76 616c 7565 7320 3d20 7365  dict_values = se
+00008aa0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00008ab0: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
 00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00008ae0: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
-00008af0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008b00: 7473 5f70 726f 7065 7274 6965 7320 3d20  ts_properties = 
-00008b10: 7365 6c66 2e5f 7472 6163 6b6c 6574 5f61  self._tracklet_a
-00008b20: 6e64 5f70 726f 7065 7274 6965 7328 616c  nd_properties(al
-00008b30: 6c5f 6469 6374 5f76 616c 7565 732c 2074  l_dict_values, t
-00008b40: 2c20 7a2c 2079 2c20 782c 206b 2c20 6375  , z, y, x, k, cu
-00008b50: 7272 656e 745f 7472 6163 6b5f 6964 2c20  rrent_track_id, 
-00008b60: 756e 6971 7565 5f69 642c 2063 7572 7265  unique_id, curre
-00008b70: 6e74 5f74 7261 636b 6c65 7473 2c20 6375  nt_tracklets, cu
-00008b80: 7272 656e 745f 7472 6163 6b6c 6574 735f  rrent_tracklets_
-00008b90: 7072 6f70 6572 7469 6573 290d 0a20 2020  properties)..   
-00008ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bc0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ae0: 2020 756e 6971 7565 5f69 6420 3d20 7374    unique_id = st
+00008af0: 7228 616c 6c5f 6469 6374 5f76 616c 7565  r(all_dict_value
+00008b00: 735b 7365 6c66 2e75 6e69 7175 6569 645f  s[self.uniqueid_
+00008b10: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b30: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00008b40: 6e74 5f74 7261 636b 5f69 6420 3d20 7374  nt_track_id = st
+00008b50: 7228 616c 6c5f 6469 6374 5f76 616c 7565  r(all_dict_value
+00008b60: 735b 7365 6c66 2e74 7261 636b 6964 5f6b  s[self.trackid_k
+00008b70: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b90: 2020 2020 2020 2020 2020 7420 3d20 696e            t = in
+00008ba0: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
+00008bb0: 5f76 616c 7565 735b 7365 6c66 2e66 7261  _values[self.fra
+00008bc0: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
 00008bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008be0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008bf0: 7473 203d 206e 702e 6173 6172 7261 7928  ts = np.asarray(
-00008c00: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00008c10: 735b 7374 7228 7472 6163 6b5f 6964 295d  s[str(track_id)]
-00008c20: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00008c30: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-00008c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c50: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008c60: 7473 5f70 726f 7065 7274 6965 7320 3d20  ts_properties = 
-00008c70: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-00008c80: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-00008c90: 7065 7274 6965 735b 7374 7228 7472 6163  perties[str(trac
-00008ca0: 6b5f 6964 295d 2c20 6474 7970 653d 6e70  k_id)], dtype=np
-00008cb0: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
-00008cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cf0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00008d00: 5f74 7261 636b 735b 7472 6163 6b5f 6964  _tracks[track_id
-00008d10: 5d20 3d20 6375 7272 656e 745f 7472 6163  ] = current_trac
-00008d20: 6b6c 6574 7320 2020 2020 0d0a 2020 2020  klets     ..    
-00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d40: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00008d50: 7175 655f 7472 6163 6b5f 7072 6f70 6572  que_track_proper
-00008d60: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
-00008d70: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008d80: 7473 5f70 726f 7065 7274 6965 7320 2020  ts_properties   
-00008d90: 200d 0a0d 0a20 2020 2064 6566 205f 7472   ....    def _tr
-00008da0: 6163 6b6c 6574 5f61 6e64 5f70 726f 7065  acklet_and_prope
-00008db0: 7274 6965 7328 7365 6c66 2c20 616c 6c5f  rties(self, all_
-00008dc0: 6469 6374 5f76 616c 7565 732c 2074 2c20  dict_values, t, 
-00008dd0: 7a2c 2079 2c20 782c 206b 2c20 6375 7272  z, y, x, k, curr
-00008de0: 656e 745f 7472 6163 6b5f 6964 2c20 756e  ent_track_id, un
-00008df0: 6971 7565 5f69 642c 2063 7572 7265 6e74  ique_id, current
-00008e00: 5f74 7261 636b 6c65 7473 2c20 6375 7272  _tracklets, curr
-00008e10: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
-00008e20: 6f70 6572 7469 6573 293a 0d0a 2020 2020  operties):..    
-00008e30: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bf0: 207a 203d 2066 6c6f 6174 2861 6c6c 5f64   z = float(all_d
+00008c00: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00008c10: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
+00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c40: 2020 7920 3d20 666c 6f61 7428 616c 6c5f    y = float(all_
+00008c50: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+00008c60: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
+00008c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c90: 2020 2078 203d 2066 6c6f 6174 2861 6c6c     x = float(all
+00008ca0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00008cb0: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
+00008cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ce0: 2020 2020 2020 6375 7272 656e 745f 7472        current_tr
+00008cf0: 6163 6b6c 6574 732c 2063 7572 7265 6e74  acklets, current
+00008d00: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
+00008d10: 7274 6965 7320 3d20 7365 6c66 2e5f 7472  rties = self._tr
+00008d20: 6163 6b6c 6574 5f61 6e64 5f70 726f 7065  acklet_and_prope
+00008d30: 7274 6965 7328 616c 6c5f 6469 6374 5f76  rties(all_dict_v
+00008d40: 616c 7565 732c 2074 2c20 7a2c 2079 2c20  alues, t, z, y, 
+00008d50: 782c 206b 2c20 6375 7272 656e 745f 7472  x, k, current_tr
+00008d60: 6163 6b5f 6964 2c20 756e 6971 7565 5f69  ack_id, unique_i
+00008d70: 642c 2063 7572 7265 6e74 5f74 7261 636b  d, current_track
+00008d80: 6c65 7473 2c20 6375 7272 656e 745f 7472  lets, current_tr
+00008d90: 6163 6b6c 6574 735f 7072 6f70 6572 7469  acklets_properti
+00008da0: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dc0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008de0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00008df0: 5f74 7261 636b 6c65 7473 203d 206e 702e  _tracklets = np.
+00008e00: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00008e10: 7472 6163 6b6c 6574 735b 7374 7228 7472  tracklets[str(tr
+00008e20: 6163 6b5f 6964 295d 2c20 6474 7970 653d  ack_id)], dtype=
+00008e30: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
 00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e50: 2020 2020 2020 2020 2020 2020 2067 656e               gen
-00008e60: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
-00008e70: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00008e80: 7365 6c66 2e67 656e 6572 6174 696f 6e69  self.generationi
-00008e90: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
-00008ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008eb0: 2020 2020 2020 2020 2020 2020 2020 7370                sp
-00008ec0: 6565 6420 3d20 666c 6f61 7428 616c 6c5f  eed = float(all_
-00008ed0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00008ee0: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
-00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f10: 2020 6163 6365 6c65 7261 7469 6f6e 203d    acceleration =
-00008f20: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00008f30: 7661 6c75 6573 5b73 656c 662e 6163 6365  values[self.acce
-00008f40: 6c65 7261 7469 6f6e 5f6b 6579 5d29 0d0a  leration_key])..
-00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f70: 2020 2020 6d6f 7469 6f6e 5f61 6e67 6c65      motion_angle
-00008f80: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00008f90: 745f 7661 6c75 6573 5b73 656c 662e 6d6f  t_values[self.mo
-00008fa0: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 5d29  tion_angle_key])
-00008fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fd0: 2020 2020 2020 7261 6469 616c 5f61 6e67        radial_ang
-00008fe0: 6c65 203d 2066 6c6f 6174 2861 6c6c 5f64  le = float(all_d
-00008ff0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00009000: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
-00009010: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009030: 2020 2020 2020 2020 7261 6469 7573 203d          radius =
-00009040: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00009050: 7661 6c75 6573 5b73 656c 662e 7261 6469  values[self.radi
-00009060: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
-00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009080: 2020 2020 2020 2020 2020 2020 2020 766f                vo
-00009090: 6c75 6d65 5f70 6978 656c 7320 3d20 696e  lume_pixels = in
-000090a0: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
-000090b0: 5f76 616c 7565 735b 7365 6c66 2e71 7561  _values[self.qua
-000090c0: 6c69 7479 5f6b 6579 5d29 290d 0a20 2020  lity_key]))..   
-000090d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090f0: 2074 6f74 616c 5f69 6e74 656e 7369 7479   total_intensity
-00009100: 203d 2020 666c 6f61 7428 616c 6c5f 6469   =  float(all_di
-00009110: 6374 5f76 616c 7565 735b 7365 6c66 2e74  ct_values[self.t
-00009120: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
-00009130: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00009140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009150: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00008e50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00008e60: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
+00008e70: 7274 6965 7320 3d20 6e70 2e61 7361 7272  rties = np.asarr
+00008e80: 6179 2863 7572 7265 6e74 5f74 7261 636b  ay(current_track
+00008e90: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
+00008ea0: 7374 7228 7472 6163 6b5f 6964 295d 2c20  str(track_id)], 
+00008eb0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00008ec0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00008ed0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00008ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008ef0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00008f00: 662e 756e 6971 7565 5f74 7261 636b 735b  f.unique_tracks[
+00008f10: 7472 6163 6b5f 6964 5d20 3d20 6375 7272  track_id] = curr
+00008f20: 656e 745f 7472 6163 6b6c 6574 7320 2020  ent_tracklets   
+00008f30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f50: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
+00008f60: 6b5f 7072 6f70 6572 7469 6573 5b74 7261  k_properties[tra
+00008f70: 636b 5f69 645d 203d 2063 7572 7265 6e74  ck_id] = current
+00008f80: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
+00008f90: 7274 6965 7320 2020 200d 0a0d 0a20 2020  rties    ....   
+00008fa0: 2064 6566 205f 7472 6163 6b6c 6574 5f61   def _tracklet_a
+00008fb0: 6e64 5f70 726f 7065 7274 6965 7328 7365  nd_properties(se
+00008fc0: 6c66 2c20 616c 6c5f 6469 6374 5f76 616c  lf, all_dict_val
+00008fd0: 7565 732c 2074 2c20 7a2c 2079 2c20 782c  ues, t, z, y, x,
+00008fe0: 206b 2c20 6375 7272 656e 745f 7472 6163   k, current_trac
+00008ff0: 6b5f 6964 2c20 756e 6971 7565 5f69 642c  k_id, unique_id,
+00009000: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00009010: 7473 2c20 6375 7272 656e 745f 7472 6163  ts, current_trac
+00009020: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+00009030: 293a 0d0a 2020 2020 2020 2020 2020 200d  ):..           .
+00009040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009060: 2020 2020 2067 656e 5f69 6420 3d20 696e       gen_id = in
+00009070: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
+00009080: 5f76 616c 7565 735b 7365 6c66 2e67 656e  _values[self.gen
+00009090: 6572 6174 696f 6e69 645f 6b65 795d 2929  erationid_key]))
+000090a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090c0: 2020 2020 2020 7370 6565 6420 3d20 666c        speed = fl
+000090d0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+000090e0: 7565 735b 7365 6c66 2e73 7065 6564 5f6b  ues[self.speed_k
+000090f0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009110: 2020 2020 2020 2020 2020 6163 6365 6c65            accele
+00009120: 7261 7469 6f6e 203d 2066 6c6f 6174 2861  ration = float(a
+00009130: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+00009140: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+00009150: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
 00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009170: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00009180: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00009190: 6b20 3d20 666c 6f61 7428 616c 6c5f 6469  k = float(all_di
-000091a0: 6374 5f76 616c 7565 735b 7365 6c66 2e64  ct_values[self.d
-000091b0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000091c0: 6b5f 6b65 795d 290d 0a20 2020 2020 2020  k_key])..       
-000091d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000091f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009210: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00009170: 2020 2020 2020 2020 2020 2020 6d6f 7469              moti
+00009180: 6f6e 5f61 6e67 6c65 203d 2066 6c6f 6174  on_angle = float
+00009190: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+000091a0: 5b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  [self.motion_ang
+000091b0: 6c65 5f6b 6579 5d29 0d0a 2020 2020 2020  le_key])..      
+000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091d0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000091e0: 6469 616c 5f61 6e67 6c65 203d 2066 6c6f  dial_angle = flo
+000091f0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+00009200: 6573 5b73 656c 662e 7261 6469 616c 5f61  es[self.radial_a
+00009210: 6e67 6c65 5f6b 6579 5d29 0d0a 2020 2020  ngle_key])..    
 00009220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009230: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-00009240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009260: 2020 2069 6620 7365 6c66 2e63 6c75 7374     if self.clust
-00009270: 6572 636c 6173 735f 6b65 7920 696e 2061  erclass_key in a
-00009280: 6c6c 5f64 6963 745f 7661 6c75 6573 2e6b  ll_dict_values.k
-00009290: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-000092a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000092d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009240: 7261 6469 7573 203d 2066 6c6f 6174 2861  radius = float(a
+00009250: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+00009260: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
+00009270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009290: 2020 2020 2020 766f 6c75 6d65 5f70 6978        volume_pix
+000092a0: 656c 7320 3d20 696e 7428 666c 6f61 7428  els = int(float(
+000092b0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+000092c0: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
+000092d0: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
 000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092f0: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
-00009300: 696e 7428 666c 6f61 7428 616c 6c5f 6469  int(float(all_di
-00009310: 6374 5f76 616c 7565 735b 7365 6c66 2e63  ct_values[self.c
-00009320: 6c75 7374 6572 636c 6173 735f 6b65 795d  lusterclass_key]
-00009330: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000092f0: 2020 2020 2020 2020 2074 6f74 616c 5f69           total_i
+00009300: 6e74 656e 7369 7479 203d 2020 666c 6f61  ntensity =  floa
+00009310: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+00009320: 735b 7365 6c66 2e74 6f74 616c 5f69 6e74  s[self.total_int
+00009330: 656e 7369 7479 5f6b 6579 5d29 0d0a 2020  ensity_key])..  
 00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009350: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009360: 6c75 7374 6572 5f63 6c61 7373 5f73 636f  luster_class_sco
-00009370: 7265 203d 2066 6c6f 6174 2861 6c6c 5f64  re = float(all_d
-00009380: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00009390: 636c 7573 7465 7273 636f 7265 5f6b 6579  clusterscore_key
-000093a0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000093b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000093d0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-000093e0: 5f66 6972 7374 203d 2066 6c6f 6174 2861  _first = float(a
-000093f0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009400: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
-00009410: 5f63 6f6d 705f 6669 7273 746b 6579 5d29  _comp_firstkey])
-00009420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009360: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009380: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
+00009390: 6365 6c6c 5f6d 6173 6b20 3d20 666c 6f61  cell_mask = floa
+000093a0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+000093b0: 735b 7365 6c66 2e64 6973 7461 6e63 655f  s[self.distance_
+000093c0: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 290d  cell_mask_key]).
+000093d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009410: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00009420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009440: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
-00009450: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00009460: 6563 6f6e 6420 3d20 666c 6f61 7428 616c  econd = float(al
-00009470: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00009480: 6c66 2e65 6363 656e 7472 6963 6974 795f  lf.eccentricity_
-00009490: 636f 6d70 5f73 6563 6f6e 646b 6579 5d29  comp_secondkey])
-000094a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009440: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009460: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00009470: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
+00009480: 6b65 7920 696e 2061 6c6c 5f64 6963 745f  key in all_dict_
+00009490: 7661 6c75 6573 2e6b 6579 7328 293a 0d0a  values.keys():..
+000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2020 2020 2020 2020 2020 2073 7572               sur
-000094d0: 6661 6365 5f61 7265 6120 3d20 666c 6f61  face_area = floa
-000094e0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-000094f0: 735b 7365 6c66 2e73 7572 6661 6365 5f61  s[self.surface_a
-00009500: 7265 615f 6b65 795d 290d 0a20 2020 2020  rea_key])..     
-00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009530: 2020 2020 2020 6365 6c6c 5f61 7869 735f        cell_axis_
-00009540: 6d61 736b 203d 2066 6c6f 6174 2861 6c6c  mask = float(all
-00009550: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-00009560: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
-00009570: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00009580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000094c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094f0: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+00009500: 636c 6173 7320 3d20 696e 7428 666c 6f61  class = int(floa
+00009510: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+00009520: 735b 7365 6c66 2e63 6c75 7374 6572 636c  s[self.clustercl
+00009530: 6173 735f 6b65 795d 2929 0d0a 2020 2020  ass_key]))..    
+00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009560: 2020 2020 2020 2063 6c75 7374 6572 5f63         cluster_c
+00009570: 6c61 7373 5f73 636f 7265 203d 2066 6c6f  lass_score = flo
+00009580: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+00009590: 6573 5b73 656c 662e 636c 7573 7465 7273  es[self.clusters
+000095a0: 636f 7265 5f6b 6579 5d29 0d0a 2020 2020  core_key])..    
 000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095f0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00009600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009620: 2020 2020 2020 2020 2020 2020 636c 7573              clus
-00009630: 7465 725f 636c 6173 7320 3d20 2d31 0d0a  ter_class = -1..
+000095d0: 2020 2020 2020 2065 6363 656e 7472 6963         eccentric
+000095e0: 6974 795f 636f 6d70 5f66 6972 7374 203d  ity_comp_first =
+000095f0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+00009600: 7661 6c75 6573 5b73 656c 662e 6563 6365  values[self.ecce
+00009610: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00009620: 7273 746b 6579 5d29 0d0a 2020 2020 2020  rstkey])..      
+00009630: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009660: 2020 2020 2020 2020 2020 2020 636c 7573              clus
-00009670: 7465 725f 636c 6173 735f 7363 6f72 6520  ter_class_score 
-00009680: 3d20 2d31 2020 0d0a 2020 2020 2020 2020  = -1  ..        
-00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096b0: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
-000096c0: 5f63 6f6d 705f 6669 7273 7420 3d20 2d31  _comp_first = -1
-000096d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096f0: 2020 2020 2020 2020 2020 2020 2020 6563                ec
-00009700: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00009710: 7365 636f 6e64 203d 202d 310d 0a20 2020  second = -1..   
+00009650: 2020 2020 2065 6363 656e 7472 6963 6974       eccentricit
+00009660: 795f 636f 6d70 5f73 6563 6f6e 6420 3d20  y_comp_second = 
+00009670: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+00009680: 616c 7565 735b 7365 6c66 2e65 6363 656e  alues[self.eccen
+00009690: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+000096a0: 6f6e 646b 6579 5d29 0d0a 2020 2020 2020  ondkey])..      
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096d0: 2020 2020 2073 7572 6661 6365 5f61 7265       surface_are
+000096e0: 6120 3d20 666c 6f61 7428 616c 6c5f 6469  a = float(all_di
+000096f0: 6374 5f76 616c 7565 735b 7365 6c66 2e73  ct_values[self.s
+00009700: 7572 6661 6365 5f61 7265 615f 6b65 795d  urface_area_key]
+00009710: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2020 2020 2020 2073 7572 6661 6365           surface
-00009750: 5f61 7265 6120 3d20 2d31 0d0a 2020 2020  _area = -1..    
-00009760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009780: 2020 2020 2020 2020 6365 6c6c 5f61 7869          cell_axi
-00009790: 735f 6d61 736b 203d 202d 3120 2020 2020  s_mask = -1     
-000097a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00009730: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00009740: 6c6c 5f61 7869 735f 6d61 736b 203d 2066  ll_axis_mask = f
+00009750: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
+00009760: 6c75 6573 5b73 656c 662e 6365 6c6c 6178  lues[self.cellax
+00009770: 6973 5f6d 6173 6b5f 6b65 795d 290d 0a20  is_mask_key]).. 
+00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 000097b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097c0: 2020 2020 2020 2020 6672 616d 655f 7370          frame_sp
-000097d0: 6f74 5f63 656e 7472 6f69 6420 3d20 2874  ot_centroid = (t
-000097e0: 2c72 6f75 6e64 287a 292f 7365 6c66 2e7a  ,round(z)/self.z
-000097f0: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-00009800: 6e64 2879 292f 7365 6c66 2e79 6361 6c69  nd(y)/self.ycali
-00009810: 6272 6174 696f 6e2c 2072 6f75 6e64 2878  bration, round(x
-00009820: 292f 7365 6c66 2e78 6361 6c69 6272 6174  )/self.xcalibrat
-00009830: 696f 6e29 200d 0a20 2020 2020 2020 2020  ion) ..         
-00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009860: 756e 6971 7565 5f73 706f 745f 6365 6e74  unique_spot_cent
-00009870: 726f 6964 5b66 7261 6d65 5f73 706f 745f  roid[frame_spot_
-00009880: 6365 6e74 726f 6964 5d20 3d20 6b0d 0a0d  centroid] = k...
-00009890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009800: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009830: 2020 2020 636c 7573 7465 725f 636c 6173      cluster_clas
+00009840: 7320 3d20 2d31 0d0a 2020 2020 2020 2020  s = -1..        
+00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009870: 2020 2020 636c 7573 7465 725f 636c 6173      cluster_clas
+00009880: 735f 7363 6f72 6520 3d20 2d31 2020 0d0a  s_score = -1  ..
+00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098b0: 2020 2020 2069 6620 6375 7272 656e 745f       if current_
-000098c0: 7472 6163 6b5f 6964 2069 6e20 6375 7272  track_id in curr
-000098d0: 656e 745f 7472 6163 6b6c 6574 733a 0d0a  ent_tracklets:..
+000098b0: 2020 2020 2020 2020 2020 2020 6563 6365              ecce
+000098c0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+000098d0: 7273 7420 3d20 2d31 0d0a 2020 2020 2020  rst = -1..      
 000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009900: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
-00009910: 5f61 7272 6179 203d 2063 7572 7265 6e74  _array = current
-00009920: 5f74 7261 636b 6c65 7473 5b63 7572 7265  _tracklets[curre
-00009930: 6e74 5f74 7261 636b 5f69 645d 0d0a 2020  nt_track_id]..  
+00009900: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
+00009910: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
+00009920: 202d 310d 0a20 2020 2020 2020 2020 2020   -1..           
+00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009960: 2020 2020 2020 6375 7272 656e 745f 7472        current_tr
-00009970: 6163 6b6c 6574 5f61 7272 6179 203d 206e  acklet_array = n
-00009980: 702e 6172 7261 7928 5b69 6e74 2866 6c6f  p.array([int(flo
-00009990: 6174 2875 6e69 7175 655f 6964 2929 2c20  at(unique_id)), 
-000099a0: 742c 207a 2f73 656c 662e 7a63 616c 6962  t, z/self.zcalib
-000099b0: 7261 7469 6f6e 2c20 792f 7365 6c66 2e79  ration, y/self.y
-000099c0: 6361 6c69 6272 6174 696f 6e2c 2078 2f73  calibration, x/s
-000099d0: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
-000099e0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a00: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00009a10: 656e 745f 7472 6163 6b6c 6574 735b 6375  ent_tracklets[cu
-00009a20: 7272 656e 745f 7472 6163 6b5f 6964 5d20  rrent_track_id] 
-00009a30: 3d20 6e70 2e76 7374 6163 6b28 2874 7261  = np.vstack((tra
-00009a40: 636b 6c65 745f 6172 7261 792c 2063 7572  cklet_array, cur
-00009a50: 7265 6e74 5f74 7261 636b 6c65 745f 6172  rent_tracklet_ar
-00009a60: 7261 7929 290d 0a0d 0a20 2020 2020 2020  ray))....       
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a90: 2076 616c 7565 5f61 7272 6179 203d 2063   value_array = c
-00009aa0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009ab0: 5f70 726f 7065 7274 6965 735b 6375 7272  _properties[curr
-00009ac0: 656e 745f 7472 6163 6b5f 6964 5d0d 0a20  ent_track_id].. 
-00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
-00009b00: 616c 7565 5f61 7272 6179 203d 206e 702e  alue_array = np.
-00009b10: 6172 7261 7928 5b74 2c20 696e 7428 666c  array([t, int(fl
-00009b20: 6f61 7428 756e 6971 7565 5f69 6429 292c  oat(unique_id)),
-00009b30: 2067 656e 5f69 642c 2072 6164 6975 732c   gen_id, radius,
-00009b40: 2076 6f6c 756d 655f 7069 7865 6c73 2c20   volume_pixels, 
-00009b50: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00009b60: 705f 6669 7273 742c 2065 6363 656e 7472  p_first, eccentr
-00009b70: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-00009b80: 642c 2073 7572 6661 6365 5f61 7265 612c  d, surface_area,
-00009b90: 2063 6c75 7374 6572 5f63 6c61 7373 2c20   cluster_class, 
-00009ba0: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
-00009bb0: 6f72 652c 2074 6f74 616c 5f69 6e74 656e  ore, total_inten
-00009bc0: 7369 7479 2c20 7370 6565 642c 206d 6f74  sity, speed, mot
-00009bd0: 696f 6e5f 616e 676c 652c 2061 6363 656c  ion_angle, accel
-00009be0: 6572 6174 696f 6e2c 2064 6973 7461 6e63  eration, distanc
-00009bf0: 655f 6365 6c6c 5f6d 6173 6b2c 2072 6164  e_cell_mask, rad
-00009c00: 6961 6c5f 616e 676c 652c 2063 656c 6c5f  ial_angle, cell_
-00009c10: 6178 6973 5f6d 6173 6b5d 290d 0a20 2020  axis_mask])..   
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c40: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009c70: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009c80: 5f70 726f 7065 7274 6965 735b 6375 7272  _properties[curr
-00009c90: 656e 745f 7472 6163 6b5f 6964 5d20 3d20  ent_track_id] = 
-00009ca0: 6e70 2e76 7374 6163 6b28 2876 616c 7565  np.vstack((value
-00009cb0: 5f61 7272 6179 2c20 6375 7272 656e 745f  _array, current_
-00009cc0: 7661 6c75 655f 6172 7261 7929 290d 0a0d  value_array))...
-00009cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009950: 2073 7572 6661 6365 5f61 7265 6120 3d20   surface_area = 
+00009960: 2d31 0d0a 2020 2020 2020 2020 2020 2020  -1..            
+00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009990: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
+000099a0: 202d 3120 2020 2020 0d0a 0d0a 2020 2020   -1     ....    
+000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099d0: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
+000099e0: 6f69 6420 3d20 2874 2c72 6f75 6e64 287a  oid = (t,round(z
+000099f0: 292f 7365 6c66 2e7a 6361 6c69 6272 6174  )/self.zcalibrat
+00009a00: 696f 6e2c 2072 6f75 6e64 2879 292f 7365  ion, round(y)/se
+00009a10: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
+00009a20: 2072 6f75 6e64 2878 292f 7365 6c66 2e78   round(x)/self.x
+00009a30: 6361 6c69 6272 6174 696f 6e29 200d 0a20  calibration) .. 
+00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a60: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00009a70: 706f 745f 6365 6e74 726f 6964 5b66 7261  pot_centroid[fra
+00009a80: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
+00009a90: 5d20 3d20 6b0d 0a0d 0a20 2020 2020 2020  ] = k....       
+00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ab0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00009ac0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
+00009ad0: 2069 6e20 6375 7272 656e 745f 7472 6163   in current_trac
+00009ae0: 6b6c 6574 733a 0d0a 2020 2020 2020 2020  klets:..        
+00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b10: 7472 6163 6b6c 6574 5f61 7272 6179 203d  tracklet_array =
+00009b20: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00009b30: 7473 5b63 7572 7265 6e74 5f74 7261 636b  ts[current_track
+00009b40: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
+00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b60: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00009b70: 7272 656e 745f 7472 6163 6b6c 6574 5f61  rrent_tracklet_a
+00009b80: 7272 6179 203d 206e 702e 6172 7261 7928  rray = np.array(
+00009b90: 5b69 6e74 2866 6c6f 6174 2875 6e69 7175  [int(float(uniqu
+00009ba0: 655f 6964 2929 2c20 742c 207a 2f73 656c  e_id)), t, z/sel
+00009bb0: 662e 7a63 616c 6962 7261 7469 6f6e 2c20  f.zcalibration, 
+00009bc0: 792f 7365 6c66 2e79 6361 6c69 6272 6174  y/self.ycalibrat
+00009bd0: 696f 6e2c 2078 2f73 656c 662e 7863 616c  ion, x/self.xcal
+00009be0: 6962 7261 7469 6f6e 5d29 0d0a 2020 2020  ibration])..    
+00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c10: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00009c20: 6b6c 6574 735b 6375 7272 656e 745f 7472  klets[current_tr
+00009c30: 6163 6b5f 6964 5d20 3d20 6e70 2e76 7374  ack_id] = np.vst
+00009c40: 6163 6b28 2874 7261 636b 6c65 745f 6172  ack((tracklet_ar
+00009c50: 7261 792c 2063 7572 7265 6e74 5f74 7261  ray, current_tra
+00009c60: 636b 6c65 745f 6172 7261 7929 290d 0a0d  cklet_array))...
+00009c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c90: 2020 2020 2020 2020 2076 616c 7565 5f61           value_a
+00009ca0: 7272 6179 203d 2063 7572 7265 6e74 5f74  rray = current_t
+00009cb0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
+00009cc0: 6965 735b 6375 7272 656e 745f 7472 6163  ies[current_trac
+00009cd0: 6b5f 6964 5d0d 0a20 2020 2020 2020 2020  k_id]..         
 00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cf0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d20: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
-00009d30: 6b6c 6574 5f61 7272 6179 203d 206e 702e  klet_array = np.
-00009d40: 6172 7261 7928 5b69 6e74 2866 6c6f 6174  array([int(float
-00009d50: 2875 6e69 7175 655f 6964 2929 2c20 742c  (unique_id)), t,
-00009d60: 207a 2f73 656c 662e 7a63 616c 6962 7261   z/self.zcalibra
-00009d70: 7469 6f6e 2c20 792f 7365 6c66 2e79 6361  tion, y/self.yca
-00009d80: 6c69 6272 6174 696f 6e2c 2078 2f73 656c  libration, x/sel
-00009d90: 662e 7863 616c 6962 7261 7469 6f6e 5d29  f.xcalibration])
-00009da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dc0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00009dd0: 745f 7472 6163 6b6c 6574 735b 6375 7272  t_tracklets[curr
-00009de0: 656e 745f 7472 6163 6b5f 6964 5d20 3d20  ent_track_id] = 
-00009df0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00009e00: 5f61 7272 6179 200d 0a0d 0a20 2020 2020  _array ....     
-00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e30: 2020 2063 7572 7265 6e74 5f76 616c 7565     current_value
-00009e40: 5f61 7272 6179 203d 206e 702e 6172 7261  _array = np.arra
-00009e50: 7928 5b74 2c20 696e 7428 666c 6f61 7428  y([t, int(float(
-00009e60: 756e 6971 7565 5f69 6429 292c 2067 656e  unique_id)), gen
-00009e70: 5f69 642c 2072 6164 6975 732c 2076 6f6c  _id, radius, vol
-00009e80: 756d 655f 7069 7865 6c73 2c20 2065 6363  ume_pixels,  ecc
-00009e90: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00009ea0: 6972 7374 2c20 6563 6365 6e74 7269 6369  irst, eccentrici
-00009eb0: 7479 5f63 6f6d 705f 7365 636f 6e64 2c20  ty_comp_second, 
-00009ec0: 7375 7266 6163 655f 6172 6561 2c20 636c  surface_area, cl
-00009ed0: 7573 7465 725f 636c 6173 732c 2063 6c75  uster_class, clu
-00009ee0: 7374 6572 5f63 6c61 7373 5f73 636f 7265  ster_class_score
-00009ef0: 2c20 746f 7461 6c5f 696e 7465 6e73 6974  , total_intensit
-00009f00: 792c 2073 7065 6564 2c20 6d6f 7469 6f6e  y, speed, motion
-00009f10: 5f61 6e67 6c65 2c20 6163 6365 6c65 7261  _angle, accelera
-00009f20: 7469 6f6e 2c20 6469 7374 616e 6365 5f63  tion, distance_c
-00009f30: 656c 6c5f 6d61 736b 2c20 7261 6469 616c  ell_mask, radial
-00009f40: 5f61 6e67 6c65 2c20 6365 6c6c 5f61 7869  _angle, cell_axi
-00009f50: 735f 6d61 736b 205d 290d 0a20 2020 2020  s_mask ])..     
-00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f80: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
-00009f90: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
-00009fa0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
-00009fb0: 5d20 3d20 6375 7272 656e 745f 7661 6c75  ] = current_valu
-00009fc0: 655f 6172 7261 790d 0a0d 0a20 2020 2020  e_array....     
-00009fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fe0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009ff0: 6574 7572 6e20 6375 7272 656e 745f 7472  eturn current_tr
-0000a000: 6163 6b6c 6574 732c 2063 7572 7265 6e74  acklets, current
-0000a010: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
-0000a020: 7274 6965 7320 2020 2020 0d0a 0d0a 2020  rties     ....  
-0000a030: 2020 6465 6620 5f6d 6173 7465 725f 7370    def _master_sp
-0000a040: 6f74 5f63 6f6d 7075 7465 7228 7365 6c66  ot_computer(self
-0000a050: 2c20 6672 616d 6529 3a0d 0a20 2020 2020  , frame):..     
-0000a060: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000a070: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
-0000a080: 696e 2066 7261 6d65 2e66 696e 6461 6c6c  in frame.findall
-0000a090: 2827 5370 6f74 2729 3a0d 0a20 2020 2020  ('Spot'):..     
-0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000a0c0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-0000a0d0: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
-0000a0e0: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
-0000a0f0: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
-0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a110: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000a120: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000a130: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
-0000a140: 2069 6e20 5370 6f74 6f62 6a65 6374 2e6b   in Spotobject.k
-0000a150: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a190: 2020 7261 6469 7573 203d 2066 6c6f 6174    radius = float
-0000a1a0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000a1b0: 7365 6c66 2e72 6164 6975 735f 6b65 7929  self.radius_key)
-0000a1c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1e0: 2020 2071 7561 6c69 7479 203d 2066 6c6f     quality = flo
-0000a1f0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000a200: 7428 7365 6c66 2e71 7561 6c69 7479 5f6b  t(self.quality_k
-0000a210: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a230: 2020 2020 2020 746f 7461 6c5f 696e 7465        total_inte
-0000a240: 6e73 6974 7920 3d20 666c 6f61 7428 5370  nsity = float(Sp
-0000a250: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000a260: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000a270: 795f 6b65 7929 290d 0a20 2020 2020 2020  y_key))..       
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2020 2020 2020 2020 206d 6561 6e5f 696e           mean_in
-0000a2a0: 7465 6e73 6974 7920 3d20 666c 6f61 7428  tensity = float(
-0000a2b0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000a2c0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-0000a2d0: 7479 5f6b 6579 2929 0d0a 0d0a 2020 2020  ty_key))....    
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2f0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-0000a300: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a320: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-0000a330: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000a340: 656c 6c5f 6964 5d20 3d20 7b0d 0a20 2020  ell_id] = {..   
-0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cf0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009d00: 7572 7265 6e74 5f76 616c 7565 5f61 7272  urrent_value_arr
+00009d10: 6179 203d 206e 702e 6172 7261 7928 5b74  ay = np.array([t
+00009d20: 2c20 696e 7428 666c 6f61 7428 756e 6971  , int(float(uniq
+00009d30: 7565 5f69 6429 292c 2067 656e 5f69 642c  ue_id)), gen_id,
+00009d40: 2072 6164 6975 732c 2076 6f6c 756d 655f   radius, volume_
+00009d50: 7069 7865 6c73 2c20 6563 6365 6e74 7269  pixels, eccentri
+00009d60: 6369 7479 5f63 6f6d 705f 6669 7273 742c  city_comp_first,
+00009d70: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+00009d80: 6d70 5f73 6563 6f6e 642c 2073 7572 6661  mp_second, surfa
+00009d90: 6365 5f61 7265 612c 2063 6c75 7374 6572  ce_area, cluster
+00009da0: 5f63 6c61 7373 2c20 636c 7573 7465 725f  _class, cluster_
+00009db0: 636c 6173 735f 7363 6f72 652c 2074 6f74  class_score, tot
+00009dc0: 616c 5f69 6e74 656e 7369 7479 2c20 7370  al_intensity, sp
+00009dd0: 6565 642c 206d 6f74 696f 6e5f 616e 676c  eed, motion_angl
+00009de0: 652c 2061 6363 656c 6572 6174 696f 6e2c  e, acceleration,
+00009df0: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
+00009e00: 6173 6b2c 2072 6164 6961 6c5f 616e 676c  ask, radial_angl
+00009e10: 652c 2063 656c 6c5f 6178 6973 5f6d 6173  e, cell_axis_mas
+00009e20: 6b5d 290d 0a20 2020 2020 2020 2020 2020  k])..           
+00009e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e40: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00009e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e70: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+00009e80: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
+00009e90: 6965 735b 6375 7272 656e 745f 7472 6163  ies[current_trac
+00009ea0: 6b5f 6964 5d20 3d20 6e70 2e76 7374 6163  k_id] = np.vstac
+00009eb0: 6b28 2876 616c 7565 5f61 7272 6179 2c20  k((value_array, 
+00009ec0: 6375 7272 656e 745f 7661 6c75 655f 6172  current_value_ar
+00009ed0: 7261 7929 290d 0a0d 0a20 2020 2020 2020  ray))....       
+00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ef0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00009f00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f20: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00009f30: 656e 745f 7472 6163 6b6c 6574 5f61 7272  ent_tracklet_arr
+00009f40: 6179 203d 206e 702e 6172 7261 7928 5b69  ay = np.array([i
+00009f50: 6e74 2866 6c6f 6174 2875 6e69 7175 655f  nt(float(unique_
+00009f60: 6964 2929 2c20 742c 207a 2f73 656c 662e  id)), t, z/self.
+00009f70: 7a63 616c 6962 7261 7469 6f6e 2c20 792f  zcalibration, y/
+00009f80: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
+00009f90: 6e2c 2078 2f73 656c 662e 7863 616c 6962  n, x/self.xcalib
+00009fa0: 7261 7469 6f6e 5d29 0d0a 2020 2020 2020  ration])..      
+00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fd0: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+00009fe0: 6574 735b 6375 7272 656e 745f 7472 6163  ets[current_trac
+00009ff0: 6b5f 6964 5d20 3d20 6375 7272 656e 745f  k_id] = current_
+0000a000: 7472 6163 6b6c 6574 5f61 7272 6179 200d  tracklet_array .
+0000a010: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a030: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+0000a040: 6e74 5f76 616c 7565 5f61 7272 6179 203d  nt_value_array =
+0000a050: 206e 702e 6172 7261 7928 5b74 2c20 696e   np.array([t, in
+0000a060: 7428 666c 6f61 7428 756e 6971 7565 5f69  t(float(unique_i
+0000a070: 6429 292c 2067 656e 5f69 642c 2072 6164  d)), gen_id, rad
+0000a080: 6975 732c 2076 6f6c 756d 655f 7069 7865  ius, volume_pixe
+0000a090: 6c73 2c20 2065 6363 656e 7472 6963 6974  ls,  eccentricit
+0000a0a0: 795f 636f 6d70 5f66 6972 7374 2c20 6563  y_comp_first, ec
+0000a0b0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+0000a0c0: 7365 636f 6e64 2c20 7375 7266 6163 655f  second, surface_
+0000a0d0: 6172 6561 2c20 636c 7573 7465 725f 636c  area, cluster_cl
+0000a0e0: 6173 732c 2063 6c75 7374 6572 5f63 6c61  ass, cluster_cla
+0000a0f0: 7373 5f73 636f 7265 2c20 746f 7461 6c5f  ss_score, total_
+0000a100: 696e 7465 6e73 6974 792c 2073 7065 6564  intensity, speed
+0000a110: 2c20 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  , motion_angle, 
+0000a120: 6163 6365 6c65 7261 7469 6f6e 2c20 6469  acceleration, di
+0000a130: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0000a140: 2c20 7261 6469 616c 5f61 6e67 6c65 2c20  , radial_angle, 
+0000a150: 6365 6c6c 5f61 7869 735f 6d61 736b 205d  cell_axis_mask ]
+0000a160: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a180: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+0000a190: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
+0000a1a0: 7065 7274 6965 735b 6375 7272 656e 745f  perties[current_
+0000a1b0: 7472 6163 6b5f 6964 5d20 3d20 6375 7272  track_id] = curr
+0000a1c0: 656e 745f 7661 6c75 655f 6172 7261 790d  ent_value_array.
+0000a1d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1f0: 2020 2020 2020 2072 6574 7572 6e20 6375         return cu
+0000a200: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
+0000a210: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+0000a220: 7473 5f70 726f 7065 7274 6965 7320 2020  ts_properties   
+0000a230: 2020 0d0a 0d0a 2020 2020 6465 6620 5f6d    ....    def _m
+0000a240: 6173 7465 725f 7370 6f74 5f63 6f6d 7075  aster_spot_compu
+0000a250: 7465 7228 7365 6c66 2c20 6672 616d 6529  ter(self, frame)
+0000a260: 3a0d 0a20 2020 2020 2020 2020 200d 0a20  :..          .. 
+0000a270: 2020 2020 2020 2020 2066 6f72 2053 706f           for Spo
+0000a280: 746f 626a 6563 7420 696e 2066 7261 6d65  tobject in frame
+0000a290: 2e66 696e 6461 6c6c 2827 5370 6f74 2729  .findall('Spot')
+0000a2a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000a2b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2d0: 2020 2020 6365 6c6c 5f69 6420 3d20 696e      cell_id = in
+0000a2e0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000a2f0: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
+0000a300: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000a310: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a330: 2020 2020 6966 2073 656c 662e 756e 6971      if self.uniq
+0000a340: 7565 6964 5f6b 6579 2069 6e20 5370 6f74  ueid_key in Spot
+0000a350: 6f62 6a65 6374 2e6b 6579 7328 293a 0d0a  object.keys():..
 0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a370: 2073 656c 662e 6365 6c6c 6964 5f6b 6579   self.cellid_key
-0000a380: 3a20 696e 7428 666c 6f61 7428 5370 6f74  : int(float(Spot
-0000a390: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000a3a0: 7370 6f74 6964 5f6b 6579 2929 292c 200d  spotid_key))), .
-0000a3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3d0: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
-0000a3e0: 645f 6b65 7920 3a20 696e 7428 666c 6f61  d_key : int(floa
-0000a3f0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000a400: 2873 656c 662e 6672 616d 6569 645f 6b65  (self.frameid_ke
-0000a410: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
+0000a370: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a390: 2020 2020 2020 2020 2020 7261 6469 7573            radius
+0000a3a0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
+0000a3b0: 6563 742e 6765 7428 7365 6c66 2e72 6164  ect.get(self.rad
+0000a3c0: 6975 735f 6b65 7929 290d 0a20 2020 2020  ius_key))..     
+0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3e0: 2020 2020 2020 2020 2020 2071 7561 6c69             quali
+0000a3f0: 7479 203d 2066 6c6f 6174 2853 706f 746f  ty = float(Spoto
+0000a400: 626a 6563 742e 6765 7428 7365 6c66 2e71  bject.get(self.q
+0000a410: 7561 6c69 7479 5f6b 6579 2929 0d0a 2020  uality_key))..  
 0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a430: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a440: 7a70 6f73 6964 5f6b 6579 203a 2066 6c6f  zposid_key : flo
-0000a450: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000a460: 7428 7365 6c66 2e7a 706f 7369 645f 6b65  t(self.zposid_ke
-0000a470: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
-0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a490: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
-0000a4a0: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-0000a4b0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000a4c0: 2873 656c 662e 7970 6f73 6964 5f6b 6579  (self.yposid_key
-0000a4d0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4f0: 2020 2020 2020 2020 2073 656c 662e 7870           self.xp
-0000a500: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
-0000a510: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000a520: 7365 6c66 2e78 706f 7369 645f 6b65 7929  self.xposid_key)
-0000a530: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
-0000a560: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-0000a570: 203a 2074 6f74 616c 5f69 6e74 656e 7369   : total_intensi
-0000a580: 7479 2c0d 0a20 2020 2020 2020 2020 2020  ty,..           
-0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5a0: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
-0000a5b0: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
-0000a5c0: 203a 206d 6561 6e5f 696e 7465 6e73 6974   : mean_intensit
-0000a5d0: 792c 0d0a 2020 2020 2020 2020 2020 2020  y,..            
-0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5f0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-0000a600: 6975 735f 6b65 7920 3a20 7261 6469 7573  ius_key : radius
-0000a610: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a430: 2020 2020 2020 2020 2020 2020 2020 746f                to
+0000a440: 7461 6c5f 696e 7465 6e73 6974 7920 3d20  tal_intensity = 
+0000a450: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000a460: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
+0000a470: 696e 7465 6e73 6974 795f 6b65 7929 290d  intensity_key)).
+0000a480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 206d 6561 6e5f 696e 7465 6e73 6974 7920   mean_intensity 
+0000a4b0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000a4c0: 6374 2e67 6574 2873 656c 662e 6d65 616e  ct.get(self.mean
+0000a4d0: 5f69 6e74 656e 7369 7479 5f6b 6579 2929  _intensity_key))
+0000a4e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a500: 2020 2020 200d 0a0d 0a0d 0a20 2020 2020       ......     
+0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a530: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000a540: 6572 7469 6573 5b63 656c 6c5f 6964 5d20  erties[cell_id] 
+0000a550: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 2020 2020 2020 2020 2073 656c 662e 6365           self.ce
+0000a580: 6c6c 6964 5f6b 6579 3a20 696e 7428 666c  llid_key: int(fl
+0000a590: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000a5a0: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
+0000a5b0: 6579 2929 292c 200d 0a20 2020 2020 2020  ey))), ..       
+0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a5e0: 662e 6672 616d 6569 645f 6b65 7920 3a20  f.frameid_key : 
+0000a5f0: 696e 7428 666c 6f61 7428 5370 6f74 6f62  int(float(Spotob
+0000a600: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
+0000a610: 616d 6569 645f 6b65 7929 2929 2c0d 0a20  ameid_key))),.. 
 0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 2020 2020 2020 2073 656c 662e 7175 616c         self.qual
-0000a640: 6974 795f 6b65 7920 3a20 7175 616c 6974  ity_key : qualit
-0000a650: 792c 0d0a 2020 2020 2020 2020 2020 2020  y,..            
-0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a670: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-0000a680: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-0000a690: 6b65 793a 2028 666c 6f61 7428 5370 6f74  key: (float(Spot
-0000a6a0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000a6b0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000a6c0: 736b 5f6b 6579 2929 292c 0d0a 2020 2020  sk_key))),..    
-0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a640: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
+0000a650: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000a660: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
+0000a670: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6a0: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
+0000a6b0: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
+0000a6c0: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
+0000a6d0: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
 0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6f0: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
-0000a700: 7920 3a20 7374 7228 5370 6f74 6f62 6a65  y : str(Spotobje
-0000a710: 6374 2e67 6574 2873 656c 662e 756e 6971  ct.get(self.uniq
-0000a720: 7565 6964 5f6b 6579 2929 2c0d 0a20 2020  ueid_key)),..   
-0000a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+0000a710: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000a720: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
+0000a730: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
 0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a750: 2073 656c 662e 7472 6163 6b6c 6574 6964   self.trackletid
-0000a760: 5f6b 6579 203a 2073 7472 2853 706f 746f  _key : str(Spoto
-0000a770: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
-0000a780: 7261 636b 6c65 7469 645f 6b65 7929 292c  rackletid_key)),
-0000a790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a760: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000a770: 7369 7479 5f6b 6579 203a 2074 6f74 616c  sity_key : total
+0000a780: 5f69 6e74 656e 7369 7479 2c0d 0a20 2020  _intensity,..   
+0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7b0: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
-0000a7c0: 6174 696f 6e69 645f 6b65 7920 3a20 7374  ationid_key : st
-0000a7d0: 7228 5370 6f74 6f62 6a65 6374 2e67 6574  r(Spotobject.get
-0000a7e0: 2873 656c 662e 6765 6e65 7261 7469 6f6e  (self.generation
-0000a7f0: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
-0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a820: 656c 662e 7472 6163 6b69 645f 6b65 7920  elf.trackid_key 
-0000a830: 3a20 7374 7228 5370 6f74 6f62 6a65 6374  : str(Spotobject
-0000a840: 2e67 6574 2873 656c 662e 7472 6163 6b69  .get(self.tracki
-0000a850: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000a7b0: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
+0000a7c0: 7369 7479 5f6b 6579 203a 206d 6561 6e5f  sity_key : mean_
+0000a7d0: 696e 7465 6e73 6974 792c 0d0a 2020 2020  intensity,..    
+0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a800: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
+0000a810: 3a20 7261 6469 7573 2c0d 0a20 2020 2020  : radius,..     
+0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a840: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
+0000a850: 3a20 7175 616c 6974 792c 0d0a 2020 2020  : quality,..    
 0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a870: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a880: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
-0000a890: 6b65 7920 3a20 2866 6c6f 6174 2853 706f  key : (float(Spo
-0000a8a0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000a8b0: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
-0000a8c0: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a8f0: 7370 6565 645f 6b65 7920 3a20 2866 6c6f  speed_key : (flo
-0000a900: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000a910: 7428 7365 6c66 2e73 7065 6564 5f6b 6579  t(self.speed_key
-0000a920: 2929 292c 0d0a 2020 2020 2020 2020 2020  ))),..          
-0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a940: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000a950: 6363 656c 6572 6174 696f 6e5f 6b65 7920  cceleration_key 
-0000a960: 3a20 2866 6c6f 6174 2853 706f 746f 626a  : (float(Spotobj
-0000a970: 6563 742e 6765 7428 7365 6c66 2e61 6363  ect.get(self.acc
-0000a980: 656c 6572 6174 696f 6e5f 6b65 7929 2929  eleration_key)))
-0000a990: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a880: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
+0000a890: 6c6c 5f6d 6173 6b5f 6b65 793a 2028 666c  ll_mask_key: (fl
+0000a8a0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000a8b0: 6574 2873 656c 662e 6469 7374 616e 6365  et(self.distance
+0000a8c0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 2929  _cell_mask_key))
+0000a8d0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8f0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+0000a900: 7175 6569 645f 6b65 7920 3a20 7374 7228  queid_key : str(
+0000a910: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000a920: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+0000a930: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a950: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+0000a960: 6163 6b6c 6574 6964 5f6b 6579 203a 2073  ackletid_key : s
+0000a970: 7472 2853 706f 746f 626a 6563 742e 6765  tr(Spotobject.ge
+0000a980: 7428 7365 6c66 2e74 7261 636b 6c65 7469  t(self.trackleti
+0000a990: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
 0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9b0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-0000a9c0: 616c 5f61 6e67 6c65 5f6b 6579 3a20 666c  al_angle_key: fl
-0000a9d0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000a9e0: 6574 2873 656c 662e 7261 6469 616c 5f61  et(self.radial_a
-0000a9f0: 6e67 6c65 5f6b 6579 2929 2c0d 0a20 2020  ngle_key)),..   
-0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa10: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
-0000aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa40: 6966 2073 656c 662e 636c 7573 7465 7263  if self.clusterc
-0000aa50: 6c61 7373 5f6b 6579 2069 6e20 5370 6f74  lass_key in Spot
-0000aa60: 6f62 6a65 6374 2e6b 6579 7328 293a 0d0a  object.keys():..
+0000a9b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a9c0: 6c66 2e67 656e 6572 6174 696f 6e69 645f  lf.generationid_
+0000a9d0: 6b65 7920 3a20 7374 7228 5370 6f74 6f62  key : str(Spotob
+0000a9e0: 6a65 6374 2e67 6574 2873 656c 662e 6765  ject.get(self.ge
+0000a9f0: 6e65 7261 7469 6f6e 6964 5f6b 6579 2929  nerationid_key))
+0000aa00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000aa30: 6b69 645f 6b65 7920 3a20 7374 7228 5370  kid_key : str(Sp
+0000aa40: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000aa50: 662e 7472 6163 6b69 645f 6b65 7929 292c  f.trackid_key)),
+0000aa60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa90: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-0000aaa0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000aab0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-0000aac0: 6461 7465 287b 7365 6c66 2e63 6c75 7374  date({self.clust
-0000aad0: 6572 636c 6173 735f 6b65 7920 3a20 696e  erclass_key : in
-0000aae0: 7428 666c 6f61 7428 5370 6f74 6f62 6a65  t(float(Spotobje
-0000aaf0: 6374 2e67 6574 2873 656c 662e 636c 7573  ct.get(self.clus
-0000ab00: 7465 7263 6c61 7373 5f6b 6579 2929 292c  terclass_key))),
-0000ab10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa80: 2020 2020 2020 7365 6c66 2e6d 6f74 696f        self.motio
+0000aa90: 6e5f 616e 676c 655f 6b65 7920 3a20 2866  n_angle_key : (f
+0000aaa0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000aab0: 6765 7428 7365 6c66 2e6d 6f74 696f 6e5f  get(self.motion_
+0000aac0: 616e 676c 655f 6b65 7929 2929 2c0d 0a20  angle_key))),.. 
+0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aaf0: 2020 2073 656c 662e 7370 6565 645f 6b65     self.speed_ke
+0000ab00: 7920 3a20 2866 6c6f 6174 2853 706f 746f  y : (float(Spoto
+0000ab10: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+0000ab20: 7065 6564 5f6b 6579 2929 292c 0d0a 2020  peed_key))),..  
 0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000ab70: 6c75 7374 6572 7363 6f72 655f 6b65 7920  lusterscore_key 
-0000ab80: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
-0000ab90: 6374 2e67 6574 2873 656c 662e 636c 7573  ct.get(self.clus
-0000aba0: 7465 7273 636f 7265 5f6b 6579 2929 2c0d  terscore_key)),.
-0000abb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 2020 2020 2020 2020 2073 656c 662e 6563           self.ec
-0000ac10: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-0000ac20: 6669 7273 746b 6579 203a 2066 6c6f 6174  firstkey : float
-0000ac30: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000ac40: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-0000ac50: 795f 636f 6d70 5f66 6972 7374 6b65 7929  y_comp_firstkey)
-0000ac60: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab50: 2020 7365 6c66 2e61 6363 656c 6572 6174    self.accelerat
+0000ab60: 696f 6e5f 6b65 7920 3a20 2866 6c6f 6174  ion_key : (float
+0000ab70: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000ab80: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+0000ab90: 6e5f 6b65 7929 2929 2c0d 0a20 2020 2020  n_key))),..     
+0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000abc0: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
+0000abd0: 5f6b 6579 3a20 666c 6f61 7428 5370 6f74  _key: float(Spot
+0000abe0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000abf0: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
+0000ac00: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac20: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ac50: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+0000ac60: 2069 6e20 5370 6f74 6f62 6a65 6374 2e6b   in Spotobject.k
+0000ac70: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
 0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000acc0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
-0000acd0: 6d70 5f73 6563 6f6e 646b 6579 203a 2066  mp_secondkey : f
-0000ace0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000acf0: 6765 7428 7365 6c66 2e65 6363 656e 7472  get(self.eccentr
-0000ad00: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-0000ad10: 646b 6579 2929 2c0d 0a20 2020 2020 2020  dkey)),..       
+0000ac90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000aca0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+0000acb0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+0000acc0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+0000acd0: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
+0000ace0: 6b65 7920 3a20 696e 7428 666c 6f61 7428  key : int(float(
+0000acf0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000ad00: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
+0000ad10: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
 0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad70: 2073 656c 662e 7375 7266 6163 655f 6172   self.surface_ar
-0000ad80: 6561 5f6b 6579 203a 2066 6c6f 6174 2853  ea_key : float(S
-0000ad90: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000ada0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-0000adb0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000ad70: 2020 7365 6c66 2e63 6c75 7374 6572 7363    self.clustersc
+0000ad80: 6f72 655f 6b65 7920 3a20 666c 6f61 7428  ore_key : float(
+0000ad90: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000ada0: 656c 662e 636c 7573 7465 7273 636f 7265  elf.clusterscore
+0000adb0: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
 0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
-0000ae20: 736b 5f6b 6579 3a20 666c 6f61 7428 5370  sk_key: float(Sp
-0000ae30: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000ae40: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
-0000ae50: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae10: 2073 656c 662e 6563 6365 6e74 7269 6369   self.eccentrici
+0000ae20: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
+0000ae30: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000ae40: 6563 742e 6765 7428 7365 6c66 2e65 6363  ect.get(self.ecc
+0000ae50: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+0000ae60: 6972 7374 6b65 7929 292c 0d0a 2020 2020  irstkey)),..    
 0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aeb0: 2020 207d 290d 0a20 2020 2020 2020 2020     })..         
-0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aee0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af10: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aec0: 2020 2020 7365 6c66 2e65 6363 656e 7472      self.eccentr
+0000aed0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+0000aee0: 646b 6579 203a 2066 6c6f 6174 2853 706f  dkey : float(Spo
+0000aef0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000af00: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+0000af10: 6d70 5f73 6563 6f6e 646b 6579 2929 2c0d  mp_secondkey)),.
+0000af20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af50: 656c 6966 2073 656c 662e 756e 6971 7565  elif self.unique
-0000af60: 6964 5f6b 6579 206e 6f74 2069 6e20 5370  id_key not in Sp
-0000af70: 6f74 6f62 6a65 6374 2e6b 6579 7328 293a  otobject.keys():
-0000af80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afb0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af70: 2020 2020 2020 2020 2073 656c 662e 7375           self.su
+0000af80: 7266 6163 655f 6172 6561 5f6b 6579 203a  rface_area_key :
+0000af90: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000afa0: 742e 6765 7428 7365 6c66 2e73 7572 6661  t.get(self.surfa
+0000afb0: 6365 5f61 7265 615f 6b65 7929 292c 0d0a  ce_area_key)),..
 0000afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afe0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000aff0: 662e 6465 7465 6374 6f72 6368 616e 6e65  f.detectorchanne
-0000b000: 6c20 3d3d 2031 3a0d 0a20 2020 2020 2020  l == 1:..       
-0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b030: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
-0000b040: 414c 5f49 4e54 454e 5349 5459 203d 2053  AL_INTENSITY = S
-0000b050: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000b060: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000b070: 7479 5f63 6832 5f6b 6579 290d 0a20 2020  ty_ch2_key)..   
+0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b010: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
+0000b020: 6c61 7869 735f 6d61 736b 5f6b 6579 3a20  laxis_mask_key: 
+0000b030: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000b040: 2e67 6574 2873 656c 662e 6365 6c6c 6178  .get(self.cellax
+0000b050: 6973 5f6d 6173 6b5f 6b65 7929 290d 0a20  is_mask_key)).. 
+0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0b0: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
-0000b0c0: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
-0000b0d0: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
-0000b0e0: 7369 7479 5f63 6832 5f6b 6579 290d 0a20  sity_ch2_key).. 
+0000b0b0: 2020 2020 2020 2020 2020 207d 290d 0a20             }).. 
+0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b110: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000b120: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b110: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b130: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b150: 2020 2020 2020 2020 2020 2020 2020 544f                TO
-0000b160: 5441 4c5f 494e 5445 4e53 4954 5920 3d20  TAL_INTENSITY = 
-0000b170: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000b180: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-0000b190: 6974 795f 6368 315f 6b65 7929 0d0a 2020  ity_ch1_key)..  
+0000b150: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+0000b160: 662e 756e 6971 7565 6964 5f6b 6579 206e  f.uniqueid_key n
+0000b170: 6f74 2069 6e20 5370 6f74 6f62 6a65 6374  ot in Spotobject
+0000b180: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
-0000b1e0: 203d 2053 706f 746f 626a 6563 742e 6765   = Spotobject.ge
-0000b1f0: 7428 7365 6c66 2e6d 6561 6e5f 696e 7465  t(self.mean_inte
-0000b200: 6e73 6974 795f 6368 315f 6b65 7929 0d0a  nsity_ch1_key)..
-0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1f0: 2020 6966 2073 656c 662e 6465 7465 6374    if self.detect
+0000b200: 6f72 6368 616e 6e65 6c20 3d3d 2031 3a0d  orchannel == 1:.
+0000b210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 2020 2020 2020 2020 2020 2020 5241 4449              RADI
-0000b240: 5553 203d 2066 6c6f 6174 2853 706f 746f  US = float(Spoto
-0000b250: 626a 6563 742e 6765 7428 7365 6c66 2e72  bject.get(self.r
-0000b260: 6164 6975 735f 6b65 7929 290d 0a20 2020  adius_key))..   
-0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b290: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
-0000b2a0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000b2b0: 6563 742e 6765 7428 7365 6c66 2e71 7561  ect.get(self.qua
-0000b2c0: 6c69 7479 5f6b 6579 2929 2020 2020 200d  lity_key))     .
-0000b2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2f0: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
-0000b300: 414c 5f49 4e54 454e 5349 5459 203d 2066  AL_INTENSITY = f
-0000b310: 6c6f 6174 2854 4f54 414c 5f49 4e54 454e  loat(TOTAL_INTEN
-0000b320: 5349 5459 290d 0a20 2020 2020 2020 2020  SITY)..         
-0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b240: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
+0000b250: 5349 5459 203d 2053 706f 746f 626a 6563  SITY = Spotobjec
+0000b260: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
+0000b270: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
+0000b280: 6579 290d 0a20 2020 2020 2020 2020 2020  ey)..           
+0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2b0: 2020 2020 2020 2020 204d 4541 4e5f 494e           MEAN_IN
+0000b2c0: 5445 4e53 4954 5920 3d20 5370 6f74 6f62  TENSITY = Spotob
+0000b2d0: 6a65 6374 2e67 6574 2873 656c 662e 6d65  ject.get(self.me
+0000b2e0: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
+0000b2f0: 5f6b 6579 290d 0a20 2020 2020 2020 2020  _key)..         
+0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b320: 2020 2065 6c73 653a 2020 2020 2020 2020     else:        
+0000b330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b350: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
-0000b360: 5920 3d20 666c 6f61 7428 4d45 414e 5f49  Y = float(MEAN_I
-0000b370: 4e54 454e 5349 5459 290d 0a20 2020 2020  NTENSITY)..     
-0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b360: 2020 2020 2020 544f 5441 4c5f 494e 5445        TOTAL_INTE
+0000b370: 4e53 4954 5920 3d20 5370 6f74 6f62 6a65  NSITY = Spotobje
+0000b380: 6374 2e67 6574 2873 656c 662e 746f 7461  ct.get(self.tota
+0000b390: 6c5f 696e 7465 6e73 6974 795f 6368 315f  l_intensity_ch1_
+0000b3a0: 6b65 7929 0d0a 2020 2020 2020 2020 2020  key)..          
+0000b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3e0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000b3f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000b400: 5b63 656c 6c5f 6964 5d20 3d20 7b0d 0a20  [cell_id] = {.. 
-0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3d0: 2020 2020 2020 2020 2020 4d45 414e 5f49            MEAN_I
+0000b3e0: 4e54 454e 5349 5459 203d 2053 706f 746f  NTENSITY = Spoto
+0000b3f0: 626a 6563 742e 6765 7428 7365 6c66 2e6d  bject.get(self.m
+0000b400: 6561 6e5f 696e 7465 6e73 6974 795f 6368  ean_intensity_ch
+0000b410: 315f 6b65 7929 0d0a 2020 2020 2020 2020  1_key)..        
 0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b430: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b440: 6365 6c6c 6964 5f6b 6579 3a20 696e 7428  cellid_key: int(
-0000b450: 6365 6c6c 5f69 6429 2c20 0d0a 2020 2020  cell_id), ..    
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b480: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
-0000b490: 6d65 6964 5f6b 6579 203a 2069 6e74 2866  meid_key : int(f
-0000b4a0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b4b0: 6765 7428 7365 6c66 2e66 7261 6d65 6964  get(self.frameid
-0000b4c0: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
-0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b440: 2020 2020 5241 4449 5553 203d 2066 6c6f      RADIUS = flo
+0000b450: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000b460: 7428 7365 6c66 2e72 6164 6975 735f 6b65  t(self.radius_ke
+0000b470: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4a0: 2051 5541 4c49 5459 203d 2066 6c6f 6174   QUALITY = float
+0000b4b0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000b4c0: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
+0000b4d0: 2929 2020 2020 200d 0a20 2020 2020 2020  ))     ..       
 0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4f0: 2020 2020 2020 7365 6c66 2e7a 706f 7369        self.zposi
-0000b500: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
-0000b510: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b520: 662e 7a70 6f73 6964 5f6b 6579 2929 2c0d  f.zposid_key)),.
-0000b530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b500: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
+0000b510: 5349 5459 203d 2066 6c6f 6174 2854 4f54  SITY = float(TOT
+0000b520: 414c 5f49 4e54 454e 5349 5459 290d 0a20  AL_INTENSITY).. 
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b560: 662e 7970 6f73 6964 5f6b 6579 203a 2066  f.yposid_key : f
-0000b570: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b580: 6765 7428 7365 6c66 2e79 706f 7369 645f  get(self.yposid_
-0000b590: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000b550: 2020 2020 2020 2020 2020 204d 4541 4e5f             MEAN_
+0000b560: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
+0000b570: 7428 4d45 414e 5f49 4e54 454e 5349 5459  t(MEAN_INTENSITY
+0000b580: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5c0: 2020 2020 7365 6c66 2e78 706f 7369 645f      self.xposid_
-0000b5d0: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
-0000b5e0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b5f0: 7870 6f73 6964 5f6b 6579 2929 2c0d 0a20  xposid_key)),.. 
-0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b620: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000b5b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000b5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b5f0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+0000b600: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+0000b610: 5d20 3d20 7b0d 0a20 2020 2020 2020 2020  ] = {..         
+0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b650: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
-0000b660: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
-0000b670: 7920 3a20 544f 5441 4c5f 494e 5445 4e53  y : TOTAL_INTENS
-0000b680: 4954 592c 0d0a 2020 2020 2020 2020 2020  ITY,..          
-0000b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6b0: 2020 7365 6c66 2e6d 6561 6e5f 696e 7465    self.mean_inte
-0000b6c0: 6e73 6974 795f 6b65 7920 3a20 4d45 414e  nsity_key : MEAN
-0000b6d0: 5f49 4e54 454e 5349 5459 2c0d 0a20 2020  _INTENSITY,..   
+0000b640: 2020 2073 656c 662e 6365 6c6c 6964 5f6b     self.cellid_k
+0000b650: 6579 3a20 696e 7428 6365 6c6c 5f69 6429  ey: int(cell_id)
+0000b660: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b690: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
+0000b6a0: 203a 2069 6e74 2866 6c6f 6174 2853 706f   : int(float(Spo
+0000b6b0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b6c0: 2e66 7261 6d65 6964 5f6b 6579 2929 292c  .frameid_key))),
+0000b6d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b700: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-0000b710: 6469 7573 5f6b 6579 203a 2052 4144 4955  dius_key : RADIU
-0000b720: 532c 0d0a 2020 2020 2020 2020 2020 2020  S,..            
-0000b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b700: 6c66 2e7a 706f 7369 645f 6b65 7920 3a20  lf.zposid_key : 
+0000b710: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000b720: 2e67 6574 2873 656c 662e 7a70 6f73 6964  .get(self.zposid
+0000b730: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
 0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b750: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-0000b760: 203a 2051 5541 4c49 5459 0d0a 2020 2020   : QUALITY..    
-0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b790: 2020 2020 7d0d 0a20 2020 2020 2020 0d0a      }..       ..
+0000b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b760: 2020 2020 2073 656c 662e 7970 6f73 6964       self.yposid
+0000b770: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000b780: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b790: 2e79 706f 7369 645f 6b65 7929 292c 0d0a  .yposid_key)),..
 0000b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7b0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000b7c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7e0: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
-0000b7f0: 7370 6f74 5f63 6f6d 7075 7465 7228 7365  spot_computer(se
-0000b800: 6c66 2c20 6672 616d 6529 3a0d 0a0d 0a20  lf, frame):.... 
-0000b810: 2020 2020 2020 2020 2066 6f72 2053 706f           for Spo
-0000b820: 746f 626a 6563 7420 696e 2066 7261 6d65  tobject in frame
-0000b830: 2e66 696e 6461 6c6c 2827 5370 6f74 2729  .findall('Spot')
-0000b840: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000b850: 2020 2020 2020 2020 2020 2023 2043 7265             # Cre
-0000b860: 6174 6520 6f62 6a65 6374 2077 6974 6820  ate object with 
-0000b870: 756e 6971 7565 2063 656c 6c20 4944 0d0a  unique cell ID..
-0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b890: 2020 2020 2020 2020 6365 6c6c 5f69 6420          cell_id 
-0000b8a0: 3d20 696e 7428 5370 6f74 6f62 6a65 6374  = int(Spotobject
-0000b8b0: 2e67 6574 2873 656c 662e 7370 6f74 6964  .get(self.spotid
-0000b8c0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8e0: 2320 4765 7420 7468 6520 545a 5958 206c  # Get the TZYX l
-0000b8f0: 6f63 6174 696f 6e20 6f66 2074 6865 2063  ocation of the c
-0000b900: 656c 6c73 2069 6e20 7468 6174 2066 7261  ells in that fra
-0000b910: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
-0000b920: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000b930: 656c 662e 6465 7465 6374 6f72 6368 616e  elf.detectorchan
-0000b940: 6e65 6c20 3d3d 2031 3a0d 0a20 2020 2020  nel == 1:..     
-0000b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b960: 2020 2020 2020 2020 2020 2069 6620 5370             if Sp
-0000b970: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b980: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000b990: 795f 6368 325f 6b65 7929 2069 7320 6e6f  y_ch2_key) is no
-0000b9a0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b7d0: 2e78 706f 7369 645f 6b65 7920 3a20 666c  .xposid_key : fl
+0000b7e0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000b7f0: 6574 2873 656c 662e 7870 6f73 6964 5f6b  et(self.xposid_k
+0000b800: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b830: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b860: 2073 656c 662e 746f 7461 6c5f 696e 7465   self.total_inte
+0000b870: 6e73 6974 795f 6b65 7920 3a20 544f 5441  nsity_key : TOTA
+0000b880: 4c5f 494e 5445 4e53 4954 592c 0d0a 2020  L_INTENSITY,..  
+0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0000b8c0: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
+0000b8d0: 7920 3a20 4d45 414e 5f49 4e54 454e 5349  y : MEAN_INTENSI
+0000b8e0: 5459 2c0d 0a20 2020 2020 2020 2020 2020  TY,..           
+0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b910: 2073 656c 662e 7261 6469 7573 5f6b 6579   self.radius_key
+0000b920: 203a 2052 4144 4955 532c 0d0a 2020 2020   : RADIUS,..    
+0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b950: 2020 2020 2020 2020 7365 6c66 2e71 7561          self.qua
+0000b960: 6c69 7479 5f6b 6579 203a 2051 5541 4c49  lity_key : QUALI
+0000b970: 5459 0d0a 2020 2020 2020 2020 2020 2020  TY..            
+0000b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b990: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+0000b9a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000b9b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 0000b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9d0: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
-0000b9e0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000b9f0: 6563 742e 6765 7428 7365 6c66 2e74 6f74  ect.get(self.tot
-0000ba00: 616c 5f69 6e74 656e 7369 7479 5f63 6832  al_intensity_ch2
-0000ba10: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba40: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
-0000ba50: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000ba60: 742e 6765 7428 7365 6c66 2e6d 6561 6e5f  t.get(self.mean_
-0000ba70: 696e 7465 6e73 6974 795f 6368 325f 6b65  intensity_ch2_ke
-0000ba80: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000b9d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000b9e0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+0000b9f0: 2020 2064 6566 205f 7370 6f74 5f63 6f6d     def _spot_com
+0000ba00: 7075 7465 7228 7365 6c66 2c20 6672 616d  puter(self, fram
+0000ba10: 6529 3a0d 0a0d 0a20 2020 2020 2020 2020  e):....         
+0000ba20: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
+0000ba30: 696e 2066 7261 6d65 2e66 696e 6461 6c6c  in frame.findall
+0000ba40: 2827 5370 6f74 2729 3a0d 0a20 2020 2020  ('Spot'):..     
+0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba60: 2020 2023 2043 7265 6174 6520 6f62 6a65     # Create obje
+0000ba70: 6374 2077 6974 6820 756e 6971 7565 2063  ct with unique c
+0000ba80: 656c 6c20 4944 0d0a 2020 2020 2020 2020  ell ID..        
 0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baa0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bad0: 2020 2054 4f54 414c 5f49 4e54 454e 5349     TOTAL_INTENSI
-0000bae0: 5459 203d 202d 310d 0a20 2020 2020 2020  TY = -1..       
-0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb10: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
-0000bb20: 202d 3120 2020 2020 2020 0d0a 2020 2020   -1       ..    
-0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb40: 2020 2020 656c 7365 3a20 2020 2020 2020      else:       
-0000bb50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000baa0: 6365 6c6c 5f69 6420 3d20 696e 7428 5370  cell_id = int(Sp
+0000bab0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000bac0: 662e 7370 6f74 6964 5f6b 6579 2929 0d0a  f.spotid_key))..
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2020 2020 2020 2320 4765 7420 7468          # Get th
+0000baf0: 6520 545a 5958 206c 6f63 6174 696f 6e20  e TZYX location 
+0000bb00: 6f66 2074 6865 2063 656c 6c73 2069 6e20  of the cells in 
+0000bb10: 7468 6174 2066 7261 6d65 0d0a 2020 2020  that frame..    
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2020 2020 6966 2073 656c 662e 6465 7465      if self.dete
+0000bb40: 6374 6f72 6368 616e 6e65 6c20 3d3d 2031  ctorchannel == 1
+0000bb50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
 0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bb70: 2020 2069 6620 5370 6f74 6f62 6a65 6374     if Spotobject
 0000bb80: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
-0000bb90: 696e 7465 6e73 6974 795f 6368 315f 6b65  intensity_ch1_ke
+0000bb90: 696e 7465 6e73 6974 795f 6368 325f 6b65  intensity_ch2_ke
 0000bba0: 7929 2069 7320 6e6f 7420 4e6f 6e65 3a0d  y) is not None:.
 0000bbb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bbd0: 2020 2020 2020 2020 2054 4f54 414c 5f49           TOTAL_I
 0000bbe0: 4e54 454e 5349 5459 203d 2066 6c6f 6174  NTENSITY = float
 0000bbf0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
 0000bc00: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-0000bc10: 7369 7479 5f63 6831 5f6b 6579 2929 0d0a  sity_ch1_key))..
+0000bc10: 7369 7479 5f63 6832 5f6b 6579 2929 0d0a  sity_ch2_key))..
 0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bc40: 2020 2020 2020 2020 4d45 414e 5f49 4e54          MEAN_INT
 0000bc50: 454e 5349 5459 203d 2066 6c6f 6174 2853  ENSITY = float(S
 0000bc60: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
 0000bc70: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-0000bc80: 795f 6368 315f 6b65 7929 290d 0a20 2020  y_ch1_key))..   
+0000bc80: 795f 6368 325f 6b65 7929 290d 0a20 2020  y_ch2_key))..   
 0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bca0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
 0000bcb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
 0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcd0: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
-0000bce0: 4c5f 494e 5445 4e53 4954 5920 3d20 2d31  L_INTENSITY = -1
-0000bcf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bcd0: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
+0000bce0: 5f49 4e54 454e 5349 5459 203d 202d 310d  _INTENSITY = -1.
+0000bcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 2020 2020 2020 2020 2020 4d45 414e 5f49            MEAN_I
-0000bd20: 4e54 454e 5349 5459 203d 202d 3120 2020  NTENSITY = -1   
-0000bd30: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd50: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000bd10: 2020 2020 2020 2020 4d45 414e 5f49 4e54          MEAN_INT
+0000bd20: 454e 5349 5459 203d 202d 3120 2020 2020  ENSITY = -1     
+0000bd30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000bd40: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000bd50: 3a20 2020 2020 2020 200d 0a20 2020 2020  :        ..     
 0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2020 2020 5241 4449 5553 203d 2066 6c6f      RADIUS = flo
-0000bd80: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000bd90: 7428 7365 6c66 2e72 6164 6975 735f 6b65  t(self.radius_ke
-0000bda0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-0000bdb0: 2020 2020 2020 2020 2020 2020 2051 5541               QUA
-0000bdc0: 4c49 5459 203d 2066 6c6f 6174 2853 706f  LITY = float(Spo
-0000bdd0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000bde0: 2e71 7561 6c69 7479 5f6b 6579 2929 0d0a  .quality_key))..
-0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be00: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be20: 2020 2074 6573 746c 6f63 6174 696f 6e20     testlocation 
-0000be30: 3d20 2866 6c6f 6174 2853 706f 746f 626a  = (float(Spotobj
-0000be40: 6563 742e 6765 7428 7365 6c66 2e7a 706f  ect.get(self.zpo
-0000be50: 7369 645f 6b65 7929 292c 2066 6c6f 6174  sid_key)), float
-0000be60: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000be70: 7365 6c66 2e79 706f 7369 645f 6b65 7929  self.yposid_key)
-0000be80: 292c 2020 666c 6f61 7428 5370 6f74 6f62  ),  float(Spotob
-0000be90: 6a65 6374 2e67 6574 2873 656c 662e 7870  ject.get(self.xp
-0000bea0: 6f73 6964 5f6b 6579 2929 290d 0a20 2020  osid_key)))..   
-0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bec0: 2020 2020 2066 7261 6d65 203d 2053 706f       frame = Spo
-0000bed0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000bee0: 2e66 7261 6d65 6964 5f6b 6579 290d 0a20  .frameid_key).. 
-0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf00: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
-0000bf10: 6365 6c6c 5f6d 6173 6b2c 206d 6173 6b63  cell_mask, maskc
-0000bf20: 656e 7472 6f69 6420 3d20 7365 6c66 2e5f  entroid = self._
-0000bf30: 6765 745f 626f 756e 6461 7279 5f64 6973  get_boundary_dis
-0000bf40: 7428 6672 616d 652c 2074 6573 746c 6f63  t(frame, testloc
-0000bf50: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
-0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bf80: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000bf90: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000bfa0: 7274 6965 735b 6365 6c6c 5f69 645d 203d  rties[cell_id] =
-0000bfb0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfd0: 7365 6c66 2e63 656c 6c69 645f 6b65 793a  self.cellid_key:
-0000bfe0: 2069 6e74 2863 656c 6c5f 6964 292c 200d   int(cell_id), .
-0000bff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c000: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c010: 662e 6672 616d 6569 645f 6b65 7920 3a20  f.frameid_key : 
-0000c020: 696e 7428 666c 6f61 7428 5370 6f74 6f62  int(float(Spotob
-0000c030: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
-0000c040: 616d 6569 645f 6b65 7929 2929 2c0d 0a20  ameid_key))),.. 
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c070: 7a70 6f73 6964 5f6b 6579 203a 2066 6c6f  zposid_key : flo
-0000c080: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000c090: 7428 7365 6c66 2e7a 706f 7369 645f 6b65  t(self.zposid_ke
-0000c0a0: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
-0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
-0000c0d0: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000c0e0: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
-0000c0f0: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2020 2020 2020 2073 656c 662e 7870           self.xp
-0000c120: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
-0000c130: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000c140: 7365 6c66 2e78 706f 7369 645f 6b65 7929  self.xposid_key)
-0000c150: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000bd70: 2020 2020 2020 2020 2020 2069 6620 5370             if Sp
+0000bd80: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000bd90: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000bda0: 795f 6368 315f 6b65 7929 2069 7320 6e6f  y_ch1_key) is no
+0000bdb0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bde0: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
+0000bdf0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
+0000be00: 6563 742e 6765 7428 7365 6c66 2e74 6f74  ect.get(self.tot
+0000be10: 616c 5f69 6e74 656e 7369 7479 5f63 6831  al_intensity_ch1
+0000be20: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be50: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
+0000be60: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000be70: 742e 6765 7428 7365 6c66 2e6d 6561 6e5f  t.get(self.mean_
+0000be80: 696e 7465 6e73 6974 795f 6368 315f 6b65  intensity_ch1_ke
+0000be90: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000beb0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bee0: 2020 2020 544f 5441 4c5f 494e 5445 4e53      TOTAL_INTENS
+0000bef0: 4954 5920 3d20 2d31 0d0a 2020 2020 2020  ITY = -1..      
+0000bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf20: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
+0000bf30: 203d 202d 3120 2020 2020 2020 2020 0d0a   = -1         ..
+0000bf40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf60: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000bf70: 2020 2020 2020 2020 2020 2020 5241 4449              RADI
+0000bf80: 5553 203d 2066 6c6f 6174 2853 706f 746f  US = float(Spoto
+0000bf90: 626a 6563 742e 6765 7428 7365 6c66 2e72  bject.get(self.r
+0000bfa0: 6164 6975 735f 6b65 7929 290d 0a20 2020  adius_key))..   
+0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfc0: 2020 2020 2051 5541 4c49 5459 203d 2066       QUALITY = f
+0000bfd0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000bfe0: 6765 7428 7365 6c66 2e71 7561 6c69 7479  get(self.quality
+0000bff0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c010: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000c020: 2020 2020 2020 2020 2020 2074 6573 746c             testl
+0000c030: 6f63 6174 696f 6e20 3d20 2866 6c6f 6174  ocation = (float
+0000c040: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000c050: 7365 6c66 2e7a 706f 7369 645f 6b65 7929  self.zposid_key)
+0000c060: 292c 2066 6c6f 6174 2853 706f 746f 626a  ), float(Spotobj
+0000c070: 6563 742e 6765 7428 7365 6c66 2e79 706f  ect.get(self.ypo
+0000c080: 7369 645f 6b65 7929 292c 2020 666c 6f61  sid_key)),  floa
+0000c090: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000c0a0: 2873 656c 662e 7870 6f73 6964 5f6b 6579  (self.xposid_key
+0000c0b0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000c0c0: 2020 2020 2020 2020 2020 2020 2066 7261               fra
+0000c0d0: 6d65 203d 2053 706f 746f 626a 6563 742e  me = Spotobject.
+0000c0e0: 6765 7428 7365 6c66 2e66 7261 6d65 6964  get(self.frameid
+0000c0f0: 5f6b 6579 290d 0a20 2020 2020 2020 2020  _key)..         
+0000c100: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000c110: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0000c120: 6b2c 206d 6173 6b63 656e 7472 6f69 6420  k, maskcentroid 
+0000c130: 3d20 7365 6c66 2e5f 6765 745f 626f 756e  = self._get_boun
+0000c140: 6461 7279 5f64 6973 7428 6672 616d 652c  dary_dist(frame,
+0000c150: 2074 6573 746c 6f63 6174 696f 6e29 0d0a   testlocation)..
 0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c170: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-0000c180: 7369 7479 5f6b 6579 203a 2054 4f54 414c  sity_key : TOTAL
-0000c190: 5f49 4e54 454e 5349 5459 2c0d 0a20 2020  _INTENSITY,..   
-0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1b0: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
-0000c1c0: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
-0000c1d0: 203a 204d 4541 4e5f 494e 5445 4e53 4954   : MEAN_INTENSIT
-0000c1e0: 592c 0d0a 2020 2020 2020 2020 2020 2020  Y,..            
-0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c200: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
-0000c210: 3a20 5241 4449 5553 2c0d 0a20 2020 2020  : RADIUS,..     
-0000c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c230: 2020 2020 2020 2073 656c 662e 7175 616c         self.qual
-0000c240: 6974 795f 6b65 7920 3a20 5155 414c 4954  ity_key : QUALIT
-0000c250: 592c 0d0a 2020 2020 2020 2020 2020 2020  Y,..            
+0000c170: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c190: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+0000c1a0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+0000c1b0: 6c6c 5f69 645d 203d 207b 0d0a 2020 2020  ll_id] = {..    
+0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1d0: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
+0000c1e0: 6c69 645f 6b65 793a 2069 6e74 2863 656c  lid_key: int(cel
+0000c1f0: 6c5f 6964 292c 200d 0a20 2020 2020 2020  l_id), ..       
+0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c210: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
+0000c220: 645f 6b65 7920 3a20 696e 7428 666c 6f61  d_key : int(floa
+0000c230: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000c240: 2873 656c 662e 6672 616d 6569 645f 6b65  (self.frameid_ke
+0000c250: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
 0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c270: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-0000c280: 6c6c 5f6d 6173 6b5f 6b65 793a 2066 6c6f  ll_mask_key: flo
-0000c290: 6174 2864 6973 7461 6e63 655f 6365 6c6c  at(distance_cell
-0000c2a0: 5f6d 6173 6b29 2c0d 0a20 2020 2020 2020  _mask),..       
+0000c270: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
+0000c280: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000c290: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
+0000c2a0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
 0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2c0: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
-0000c2d0: 6e74 726f 6964 5f7a 5f6b 6579 3a20 666c  ntroid_z_key: fl
-0000c2e0: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
-0000c2f0: 5b30 5d29 2c0d 0a20 2020 2020 2020 2020  [0]),..         
-0000c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c310: 2020 2073 656c 662e 6d61 736b 6365 6e74     self.maskcent
-0000c320: 726f 6964 5f79 5f6b 6579 3a20 666c 6f61  roid_y_key: floa
-0000c330: 7428 6d61 736b 6365 6e74 726f 6964 5b31  t(maskcentroid[1
-0000c340: 5d29 2c0d 0a20 2020 2020 2020 2020 2020  ]),..           
-0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c360: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
-0000c370: 6964 5f78 5f6b 6579 3a20 666c 6f61 7428  id_x_key: float(
-0000c380: 6d61 736b 6365 6e74 726f 6964 5b32 5d29  maskcentroid[2])
-0000c390: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000c3a0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-0000c3b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000c3c0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000c3d0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c410: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-0000c420: 0a20 2020 200d 0a20 2020 2020 2020 2020  .    ..         
-0000c430: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000c440: 0a0d 0a20 2020 2064 6566 205f 6765 745f  ...    def _get_
-0000c450: 6d61 7374 6572 5f78 6d6c 5f64 6174 6128  master_xml_data(
-0000c460: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-0000c470: 2020 2020 6966 2073 656c 662e 6368 616e      if self.chan
-0000c480: 6e65 6c5f 7365 675f 696d 6167 6520 6973  nel_seg_image is
-0000c490: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4b0: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
-0000c4c0: 6d6c 5f63 6f6e 7465 6e74 203d 2073 656c  ml_content = sel
-0000c4d0: 662e 786d 6c5f 636f 6e74 656e 740d 0a20  f.xml_content.. 
-0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4f0: 2020 2020 2073 656c 662e 786d 6c5f 7472       self.xml_tr
-0000c500: 6565 203d 2065 742e 7061 7273 6528 7365  ee = et.parse(se
-0000c510: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
-0000c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c530: 2020 2020 7365 6c66 2e78 6d6c 5f72 6f6f      self.xml_roo
-0000c540: 7420 3d20 7365 6c66 2e78 6d6c 5f74 7265  t = self.xml_tre
-0000c550: 652e 6765 7472 6f6f 7428 290d 0a20 2020  e.getroot()..   
-0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c570: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
-0000c580: 786d 6c5f 6e61 6d65 203d 2027 7365 636f  xml_name = 'seco
-0000c590: 6e64 5f63 6861 6e6e 656c 5f27 202b 206f  nd_channel_' + o
-0000c5a0: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
-0000c5b0: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
-0000c5c0: 2873 656c 662e 786d 6c5f 7061 7468 2929  (self.xml_path))
-0000c5d0: 5b30 5d20 2b20 272e 786d 6c27 0d0a 2020  [0] + '.xml'..  
-0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5f0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-0000c600: 5f78 6d6c 5f70 6174 6820 3d20 6f73 2e70  _xml_path = os.p
-0000c610: 6174 682e 6469 726e 616d 6528 7365 6c66  ath.dirname(self
-0000c620: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
+0000c2c0: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
+0000c2d0: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
+0000c2e0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000c2f0: 2873 656c 662e 7970 6f73 6964 5f6b 6579  (self.yposid_key
+0000c300: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c320: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+0000c330: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000c340: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
+0000c350: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c370: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+0000c380: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
+0000c390: 203a 2054 4f54 414c 5f49 4e54 454e 5349   : TOTAL_INTENSI
+0000c3a0: 5459 2c0d 0a20 2020 2020 2020 2020 2020  TY,..           
+0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3c0: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
+0000c3d0: 7369 7479 5f6b 6579 203a 204d 4541 4e5f  sity_key : MEAN_
+0000c3e0: 494e 5445 4e53 4954 592c 0d0a 2020 2020  INTENSITY,..    
+0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c400: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+0000c410: 6975 735f 6b65 7920 3a20 5241 4449 5553  ius_key : RADIUS
+0000c420: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c430: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c440: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
+0000c450: 3a20 5155 414c 4954 592c 0d0a 2020 2020  : QUALITY,..    
+0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c470: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
+0000c480: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
+0000c490: 6b65 793a 2066 6c6f 6174 2864 6973 7461  key: float(dista
+0000c4a0: 6e63 655f 6365 6c6c 5f6d 6173 6b29 2c0d  nce_cell_mask),.
+0000c4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c4c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c4d0: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
+0000c4e0: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
+0000c4f0: 6365 6e74 726f 6964 5b30 5d29 2c0d 0a20  centroid[0]),.. 
+0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c520: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
+0000c530: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
+0000c540: 6e74 726f 6964 5b31 5d29 2c0d 0a20 2020  ntroid[1]),..   
+0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c560: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+0000c570: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
+0000c580: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
+0000c590: 726f 6964 5b32 5d29 200d 0a20 2020 2020  roid[2]) ..     
+0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5b0: 2020 207d 0d0a 2020 2020 2020 200d 0a20     }..       .. 
+0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000c5e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000c5f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000c600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c620: 2020 2020 200d 0a0d 0a20 2020 200d 0a20       ....    .. 
 0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c640: 2020 7365 6c66 2e5f 6372 6561 7465 5f63    self._create_c
-0000c650: 6861 6e6e 656c 5f74 7265 6528 290d 0a0d  hannel_tree()...
-0000c660: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c670: 662e 756e 6971 7565 5f6f 626a 6563 7473  f.unique_objects
-0000c680: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-0000c690: 2020 2073 656c 662e 756e 6971 7565 5f70     self.unique_p
-0000c6a0: 726f 7065 7274 6965 7320 3d20 7b7d 0d0a  roperties = {}..
-0000c6b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c6c0: 2e41 6c6c 5472 6163 6b49 6473 203d 205b  .AllTrackIds = [
-0000c6d0: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
-0000c6e0: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
-0000c6f0: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
-0000c700: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
-0000c710: 616c 5472 6163 6b49 6473 203d 205b 5d0d  alTrackIds = [].
-0000c720: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c730: 662e 616c 6c5f 7472 6163 6b5f 7072 6f70  f.all_track_prop
-0000c740: 6572 7469 6573 203d 205b 5d0d 0a20 2020  erties = []..   
-0000c750: 2020 2020 2020 2020 2073 656c 662e 7370           self.sp
-0000c760: 6c69 745f 706f 696e 7473 5f74 696d 6573  lit_points_times
-0000c770: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-0000c780: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000c790: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000c7a0: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-0000c7b0: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
-0000c7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c7d0: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
-0000c7e0: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
+0000c640: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
+0000c650: 6566 205f 6765 745f 6d61 7374 6572 5f78  ef _get_master_x
+0000c660: 6d6c 5f64 6174 6128 7365 6c66 293a 0d0a  ml_data(self):..
+0000c670: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000c680: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
+0000c690: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+0000c6a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000c6b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000c6c0: 6861 6e6e 656c 5f78 6d6c 5f63 6f6e 7465  hannel_xml_conte
+0000c6d0: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
+0000c6e0: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
+0000c6f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c700: 662e 786d 6c5f 7472 6565 203d 2065 742e  f.xml_tree = et.
+0000c710: 7061 7273 6528 7365 6c66 2e78 6d6c 5f70  parse(self.xml_p
+0000c720: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000c730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c740: 2e78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  .xml_root = self
+0000c750: 2e78 6d6c 5f74 7265 652e 6765 7472 6f6f  .xml_tree.getroo
+0000c760: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+0000c770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c780: 6368 616e 6e65 6c5f 786d 6c5f 6e61 6d65  channel_xml_name
+0000c790: 203d 2027 7365 636f 6e64 5f63 6861 6e6e   = 'second_chann
+0000c7a0: 656c 5f27 202b 206f 732e 7061 7468 2e73  el_' + os.path.s
+0000c7b0: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
+0000c7c0: 6261 7365 6e61 6d65 2873 656c 662e 786d  basename(self.xm
+0000c7d0: 6c5f 7061 7468 2929 5b30 5d20 2b20 272e  l_path))[0] + '.
+0000c7e0: 786d 6c27 0d0a 2020 2020 2020 2020 2020  xml'..          
 0000c7f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c800: 2e4e 6f72 6d61 6c54 7261 636b 4964 732e  .NormalTrackIds.
-0000c810: 6170 7065 6e64 284e 6f6e 6529 0d0a 2020  append(None)..  
-0000c820: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000c830: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
-0000c840: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000c850: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
-0000c860: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000c870: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
-0000c880: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
-0000c890: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
-0000c8a0: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
-0000c8b0: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
-0000c8c0: 656e 6428 7365 6c66 2e54 7261 636b 6964  end(self.Trackid
-0000c8d0: 426f 7829 0d0a 2020 2020 2020 2020 2020  Box)..          
-0000c8e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000c8f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000c900: 6c66 2e53 706f 746f 626a 6563 7473 203d  lf.Spotobjects =
-0000c910: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000c920: 742e 6669 6e64 2827 4d6f 6465 6c27 292e  t.find('Model').
-0000c930: 6669 6e64 2827 416c 6c53 706f 7473 2729  find('AllSpots')
-0000c940: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000c950: 4578 7472 6163 7420 7468 6520 7472 6163  Extract the trac
-0000c960: 6b73 2066 726f 6d20 786d 6c0d 0a20 2020  ks from xml..   
-0000c970: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-0000c980: 6163 6b73 203d 2073 656c 662e 786d 6c5f  acks = self.xml_
-0000c990: 636f 6e74 656e 742e 6669 6e64 2822 4d6f  content.find("Mo
-0000c9a0: 6465 6c22 292e 6669 6e64 2822 416c 6c54  del").find("AllT
-0000c9b0: 7261 636b 7322 290d 0a20 2020 2020 2020  racks")..       
-0000c9c0: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000c9d0: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
-0000c9e0: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
-0000c9f0: 696e 6773 2229 2e66 696e 6428 2249 6d61  ings").find("Ima
-0000ca00: 6765 4461 7461 2229 0d0a 2020 2020 2020  geData")..      
-0000ca10: 2020 2020 2020 7365 6c66 2e78 6361 6c69        self.xcali
-0000ca20: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
-0000ca30: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
-0000ca40: 7428 2270 6978 656c 7769 6474 6822 2929  t("pixelwidth"))
-0000ca50: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000ca60: 6c66 2e79 6361 6c69 6272 6174 696f 6e20  lf.ycalibration 
-0000ca70: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
-0000ca80: 7469 6e67 732e 6765 7428 2270 6978 656c  tings.get("pixel
-0000ca90: 6865 6967 6874 2229 290d 0a20 2020 2020  height"))..     
-0000caa0: 2020 2020 2020 2073 656c 662e 7a63 616c         self.zcal
-0000cab0: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
-0000cac0: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
-0000cad0: 6574 2822 766f 7865 6c64 6570 7468 2229  et("voxeldepth")
-0000cae0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0000caf0: 656c 662e 7463 616c 6962 7261 7469 6f6e  elf.tcalibration
-0000cb00: 203d 2069 6e74 2866 6c6f 6174 2873 656c   = int(float(sel
-0000cb10: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
-0000cb20: 7469 6d65 696e 7465 7276 616c 2229 2929  timeinterval")))
-0000cb30: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000cb40: 6c66 2e64 6574 6563 746f 7273 6574 7469  lf.detectorsetti
-0000cb50: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
-0000cb60: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
-0000cb70: 7469 6e67 7322 292e 6669 6e64 2822 4465  tings").find("De
-0000cb80: 7465 6374 6f72 5365 7474 696e 6773 2229  tectorSettings")
-0000cb90: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000cba0: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
-0000cbb0: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000cbc0: 656e 742e 6669 6e64 2822 5365 7474 696e  ent.find("Settin
-0000cbd0: 6773 2229 2e66 696e 6428 2242 6173 6963  gs").find("Basic
-0000cbe0: 5365 7474 696e 6773 2229 0d0a 2020 2020  Settings")..    
-0000cbf0: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
-0000cc00: 6563 746f 7263 6861 6e6e 656c 203d 2069  ectorchannel = i
-0000cc10: 6e74 2866 6c6f 6174 2873 656c 662e 6465  nt(float(self.de
-0000cc20: 7465 6374 6f72 7365 7474 696e 6773 2e67  tectorsettings.g
-0000cc30: 6574 2822 5441 5247 4554 5f43 4841 4e4e  et("TARGET_CHANN
-0000cc40: 454c 2229 2929 0d0a 2020 2020 2020 2020  EL")))..        
-0000cc50: 2020 2020 7365 6c66 2e74 7374 6172 7420      self.tstart 
-0000cc60: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
-0000cc70: 2e62 6173 6963 7365 7474 696e 6773 2e67  .basicsettings.g
-0000cc80: 6574 2822 7473 7461 7274 2229 2929 0d0a  et("tstart")))..
-0000cc90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cca0: 2e74 656e 6420 3d20 696e 7428 666c 6f61  .tend = int(floa
-0000ccb0: 7428 7365 6c66 2e62 6173 6963 7365 7474  t(self.basicsett
-0000ccc0: 696e 6773 2e67 6574 2822 7465 6e64 2229  ings.get("tend")
-0000ccd0: 2929 2020 2020 2020 0d0a 0d0a 2020 2020  ))      ....    
-0000cce0: 2020 2020 2020 2020 7072 696e 7428 2749          print('I
-0000ccf0: 7465 7261 7469 6e67 206f 7665 7220 7370  terating over sp
-0000cd00: 6f74 7320 696e 2066 7261 6d65 2729 0d0a  ots in frame')..
-0000cd10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cd20: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
-0000cd30: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
-0000cd40: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-0000cd50: 2020 2020 7769 7468 2063 6f6e 6375 7272      with concurr
-0000cd60: 656e 742e 6675 7475 7265 732e 5468 7265  ent.futures.Thre
-0000cd70: 6164 506f 6f6c 4578 6563 7574 6f72 286d  adPoolExecutor(m
-0000cd80: 6178 5f77 6f72 6b65 7273 203d 206f 732e  ax_workers = os.
-0000cd90: 6370 755f 636f 756e 7428 2929 2061 7320  cpu_count()) as 
-0000cda0: 6578 6563 7574 6f72 3a0d 0a20 2020 2020  executor:..     
-0000cdb0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000cdc0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000cdd0: 2066 7261 6d65 2069 6e20 7365 6c66 2e53   frame in self.S
-0000cde0: 706f 746f 626a 6563 7473 2e66 696e 6461  potobjects.finda
-0000cdf0: 6c6c 2827 5370 6f74 7349 6e46 7261 6d65  ll('SpotsInFrame
-0000ce00: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce20: 2066 7574 7572 6573 2e61 7070 656e 6428   futures.append(
-0000ce30: 6578 6563 7574 6f72 2e73 7562 6d69 7428  executor.submit(
-0000ce40: 7365 6c66 2e5f 6d61 7374 6572 5f73 706f  self._master_spo
-0000ce50: 745f 636f 6d70 7574 6572 2c20 6672 616d  t_computer, fram
-0000ce60: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
-0000ce70: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-0000ce80: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-0000ce90: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ceb0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ced0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000cee0: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
-0000cef0: 6c20 3d20 2243 6f6c 6c65 6374 696e 6720  l = "Collecting 
-0000cf00: 5370 6f74 7322 0d0a 2020 2020 2020 2020  Spots"..        
-0000cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf20: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000cf30: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
-0000cf40: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf60: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
-0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf90: 206c 656e 2866 7574 7572 6573 292c 0d0a   len(futures),..
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfe0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000cff0: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
-0000d000: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000d010: 6f72 2072 2069 6e20 636f 6e63 7572 7265  or r in concurre
-0000d020: 6e74 2e66 7574 7572 6573 2e61 735f 636f  nt.futures.as_co
-0000d030: 6d70 6c65 7465 6428 6675 7475 7265 7329  mpleted(futures)
-0000d040: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d060: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-0000d070: 7365 6c66 2e63 6f75 6e74 202b 2031 0d0a  self.count + 1..
-0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0a0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-0000d0b0: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-0000d0c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000c800: 2e63 6861 6e6e 656c 5f78 6d6c 5f70 6174  .channel_xml_pat
+0000c810: 6820 3d20 6f73 2e70 6174 682e 6469 726e  h = os.path.dirn
+0000c820: 616d 6528 7365 6c66 2e78 6d6c 5f70 6174  ame(self.xml_pat
+0000c830: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+0000c840: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000c850: 6372 6561 7465 5f63 6861 6e6e 656c 5f74  create_channel_t
+0000c860: 7265 6528 290d 0a0d 0a20 2020 2020 2020  ree()....       
+0000c870: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+0000c880: 5f6f 626a 6563 7473 203d 207b 7d0d 0a20  _objects = {}.. 
+0000c890: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c8a0: 756e 6971 7565 5f70 726f 7065 7274 6965  unique_propertie
+0000c8b0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+0000c8c0: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+0000c8d0: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
+0000c8e0: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
+0000c8f0: 6469 6e67 5472 6163 6b49 6473 203d 205b  dingTrackIds = [
+0000c900: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+0000c910: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+0000c920: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
+0000c930: 2020 2020 2073 656c 662e 616c 6c5f 7472       self.all_tr
+0000c940: 6163 6b5f 7072 6f70 6572 7469 6573 203d  ack_properties =
+0000c950: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000c960: 2073 656c 662e 7370 6c69 745f 706f 696e   self.split_poin
+0000c970: 7473 5f74 696d 6573 203d 205b 5d0d 0a0d  ts_times = []...
+0000c980: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000c990: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000c9a0: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
+0000c9b0: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000c9c0: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000c9d0: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+0000c9e0: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
+0000c9f0: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000ca00: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
+0000ca10: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
+0000ca20: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+0000ca30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ca40: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
+0000ca50: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
+0000ca60: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
+0000ca70: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+0000ca80: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+0000ca90: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
+0000caa0: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
+0000cab0: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
+0000cac0: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
+0000cad0: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
+0000cae0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000caf0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000cb00: 2020 2020 2020 7365 6c66 2e53 706f 746f        self.Spoto
+0000cb10: 626a 6563 7473 203d 2073 656c 662e 786d  bjects = self.xm
+0000cb20: 6c5f 636f 6e74 656e 742e 6669 6e64 2827  l_content.find('
+0000cb30: 4d6f 6465 6c27 292e 6669 6e64 2827 416c  Model').find('Al
+0000cb40: 6c53 706f 7473 2729 0d0a 2020 2020 2020  lSpots')..      
+0000cb50: 2020 2020 2020 2320 4578 7472 6163 7420        # Extract 
+0000cb60: 7468 6520 7472 6163 6b73 2066 726f 6d20  the tracks from 
+0000cb70: 786d 6c0d 0a20 2020 2020 2020 2020 2020  xml..           
+0000cb80: 2073 656c 662e 7472 6163 6b73 203d 2073   self.tracks = s
+0000cb90: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000cba0: 6669 6e64 2822 4d6f 6465 6c22 292e 6669  find("Model").fi
+0000cbb0: 6e64 2822 416c 6c54 7261 636b 7322 290d  nd("AllTracks").
+0000cbc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000cbd0: 662e 7365 7474 696e 6773 203d 2073 656c  f.settings = sel
+0000cbe0: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000cbf0: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+0000cc00: 696e 6428 2249 6d61 6765 4461 7461 2229  ind("ImageData")
+0000cc10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000cc20: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
+0000cc30: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
+0000cc40: 7469 6e67 732e 6765 7428 2270 6978 656c  tings.get("pixel
+0000cc50: 7769 6474 6822 2929 0d0a 2020 2020 2020  width"))..      
+0000cc60: 2020 2020 2020 7365 6c66 2e79 6361 6c69        self.ycali
+0000cc70: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
+0000cc80: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+0000cc90: 7428 2270 6978 656c 6865 6967 6874 2229  t("pixelheight")
+0000cca0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000ccb0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+0000ccc0: 203d 2066 6c6f 6174 2873 656c 662e 7365   = float(self.se
+0000ccd0: 7474 696e 6773 2e67 6574 2822 766f 7865  ttings.get("voxe
+0000cce0: 6c64 6570 7468 2229 290d 0a20 2020 2020  ldepth"))..     
+0000ccf0: 2020 2020 2020 2073 656c 662e 7463 616c         self.tcal
+0000cd00: 6962 7261 7469 6f6e 203d 2069 6e74 2866  ibration = int(f
+0000cd10: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
+0000cd20: 6773 2e67 6574 2822 7469 6d65 696e 7465  gs.get("timeinte
+0000cd30: 7276 616c 2229 2929 0d0a 2020 2020 2020  rval")))..      
+0000cd40: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
+0000cd50: 746f 7273 6574 7469 6e67 7320 3d20 7365  torsettings = se
+0000cd60: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000cd70: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
+0000cd80: 6669 6e64 2822 4465 7465 6374 6f72 5365  find("DetectorSe
+0000cd90: 7474 696e 6773 2229 0d0a 2020 2020 2020  ttings")..      
+0000cda0: 2020 2020 2020 7365 6c66 2e62 6173 6963        self.basic
+0000cdb0: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
+0000cdc0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
+0000cdd0: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
+0000cde0: 6428 2242 6173 6963 5365 7474 696e 6773  d("BasicSettings
+0000cdf0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000ce00: 7365 6c66 2e64 6574 6563 746f 7263 6861  self.detectorcha
+0000ce10: 6e6e 656c 203d 2069 6e74 2866 6c6f 6174  nnel = int(float
+0000ce20: 2873 656c 662e 6465 7465 6374 6f72 7365  (self.detectorse
+0000ce30: 7474 696e 6773 2e67 6574 2822 5441 5247  ttings.get("TARG
+0000ce40: 4554 5f43 4841 4e4e 454c 2229 2929 0d0a  ET_CHANNEL")))..
+0000ce50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ce60: 2e74 7374 6172 7420 3d20 696e 7428 666c  .tstart = int(fl
+0000ce70: 6f61 7428 7365 6c66 2e62 6173 6963 7365  oat(self.basicse
+0000ce80: 7474 696e 6773 2e67 6574 2822 7473 7461  ttings.get("tsta
+0000ce90: 7274 2229 2929 0d0a 2020 2020 2020 2020  rt")))..        
+0000cea0: 2020 2020 7365 6c66 2e74 656e 6420 3d20      self.tend = 
+0000ceb0: 696e 7428 666c 6f61 7428 7365 6c66 2e62  int(float(self.b
+0000cec0: 6173 6963 7365 7474 696e 6773 2e67 6574  asicsettings.get
+0000ced0: 2822 7465 6e64 2229 2929 2020 2020 2020  ("tend")))      
+0000cee0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000cef0: 7072 696e 7428 2749 7465 7261 7469 6e67  print('Iterating
+0000cf00: 206f 7665 7220 7370 6f74 7320 696e 2066   over spots in f
+0000cf10: 7261 6d65 2729 0d0a 2020 2020 2020 2020  rame')..        
+0000cf20: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+0000cf30: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
+0000cf40: 6675 7475 7265 7320 3d20 5b5d 0d0a 0d0a  futures = []....
+0000cf50: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000cf60: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+0000cf70: 7265 732e 5468 7265 6164 506f 6f6c 4578  res.ThreadPoolEx
+0000cf80: 6563 7574 6f72 286d 6178 5f77 6f72 6b65  ecutor(max_worke
+0000cf90: 7273 203d 206f 732e 6370 755f 636f 756e  rs = os.cpu_coun
+0000cfa0: 7428 2929 2061 7320 6578 6563 7574 6f72  t()) as executor
+0000cfb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000cfc0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000cfd0: 2020 2020 2066 6f72 2066 7261 6d65 2069       for frame i
+0000cfe0: 6e20 7365 6c66 2e53 706f 746f 626a 6563  n self.Spotobjec
+0000cff0: 7473 2e66 696e 6461 6c6c 2827 5370 6f74  ts.findall('Spot
+0000d000: 7349 6e46 7261 6d65 2729 3a0d 0a20 2020  sInFrame'):..   
+0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d020: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+0000d030: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
+0000d040: 2e73 7562 6d69 7428 7365 6c66 2e5f 6d61  .submit(self._ma
+0000d050: 7374 6572 5f73 706f 745f 636f 6d70 7574  ster_spot_comput
+0000d060: 6572 2c20 6672 616d 6529 290d 0a20 2020  er, frame))..   
+0000d070: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d080: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000d090: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0e0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000d0f0: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
-0000d100: 2020 7365 6c66 2e63 6f75 6e74 0d0a 2020    self.count..  
+0000d0e0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000d0f0: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
+0000d100: 6c65 6374 696e 6720 5370 6f74 7322 0d0a  lecting Spots"..
 0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d120: 2020 2020 2020 2020 2020 2020 2020 722e                r.
-0000d130: 7265 7375 6c74 2829 2020 2020 0d0a 0d0a  result()    ....
-0000d140: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000d150: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000d160: 6627 4974 6572 6174 696e 6720 6f76 6572  f'Iterating over
-0000d170: 2074 7261 636b 7320 7b6c 656e 2873 656c   tracks {len(sel
-0000d180: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
-0000d190: 5f69 6473 297d 2729 2020 0d0a 2020 2020  _ids)}')  ..    
-0000d1a0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-0000d1b0: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
-0000d1c0: 2020 2020 6675 7475 7265 7320 3d20 5b5d      futures = []
-0000d1d0: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-0000d1e0: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
-0000d1f0: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
-0000d200: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
-0000d210: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
-0000d220: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
-0000d230: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-0000d240: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000d250: 2020 2020 2020 2066 6f72 2074 7261 636b         for track
-0000d260: 2069 6e20 7365 6c66 2e74 7261 636b 732e   in self.tracks.
-0000d270: 6669 6e64 616c 6c28 2754 7261 636b 2729  findall('Track')
-0000d280: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d290: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2b0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-0000d2c0: 696e 7428 7472 6163 6b2e 6765 7428 7365  int(track.get(se
-0000d2d0: 6c66 2e74 7261 636b 6964 5f6b 6579 2929  lf.trackid_key))
-0000d2e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d2f0: 2020 2020 2020 2020 2020 6966 2074 7261            if tra
-0000d300: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
-0000d310: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-0000d320: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d340: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
-0000d350: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
-0000d360: 7428 7365 6c66 2e5f 6d61 7374 6572 5f74  t(self._master_t
-0000d370: 7261 636b 5f63 6f6d 7075 7465 722c 2074  rack_computer, t
-0000d380: 7261 636b 2c20 7472 6163 6b5f 6964 2929  rack, track_id))
-0000d390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d3a0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-0000d3b0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-0000d3c0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d400: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000d410: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
-0000d420: 2022 436f 6c6c 6563 7469 6e67 2054 7261   "Collecting Tra
-0000d430: 636b 7322 0d0a 2020 2020 2020 2020 2020  cks"..          
-0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d450: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000d460: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
-0000d470: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d490: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
-0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000d4c0: 656e 2873 656c 662e 6669 6c74 6572 6564  en(self.filtered
-0000d4d0: 5f74 7261 636b 5f69 6473 292c 0d0a 2020  _track_ids),..  
-0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4f0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-0000d500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d520: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000d530: 6172 2e73 686f 7728 290d 0a0d 0a0d 0a20  ar.show()...... 
-0000d540: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000d550: 6f72 2072 2069 6e20 636f 6e63 7572 7265  or r in concurre
-0000d560: 6e74 2e66 7574 7572 6573 2e61 735f 636f  nt.futures.as_co
-0000d570: 6d70 6c65 7465 6428 6675 7475 7265 7329  mpleted(futures)
-0000d580: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5a0: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-0000d5b0: 7365 6c66 2e63 6f75 6e74 202b 2031 0d0a  self.count + 1..
-0000d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d130: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000d140: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
+0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d170: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d190: 2020 2020 2020 2020 206c 656e 2866 7574           len(fut
+0000d1a0: 7572 6573 292c 0d0a 2020 2020 2020 2020  ures),..        
+0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1c0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d1f0: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
+0000d200: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
+0000d210: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
+0000d220: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+0000d230: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
+0000d240: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
+0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d260: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d270: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
+0000d280: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d2b0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+0000d2c0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d2f0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000d300: 2e76 616c 7565 203d 2020 7365 6c66 2e63  .value =  self.c
+0000d310: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d330: 2020 2020 2020 722e 7265 7375 6c74 2829        r.result()
+0000d340: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0000d350: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000d360: 2020 7072 696e 7428 6627 4974 6572 6174    print(f'Iterat
+0000d370: 696e 6720 6f76 6572 2074 7261 636b 7320  ing over tracks 
+0000d380: 7b6c 656e 2873 656c 662e 6669 6c74 6572  {len(self.filter
+0000d390: 6564 5f74 7261 636b 5f69 6473 297d 2729  ed_track_ids)}')
+0000d3a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d3b0: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
+0000d3c0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
+0000d3d0: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
+0000d3e0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
+0000d3f0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
+0000d400: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
+0000d410: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
+0000d420: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
+0000d430: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
+0000d440: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000d450: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000d460: 6f72 2074 7261 636b 2069 6e20 7365 6c66  or track in self
+0000d470: 2e74 7261 636b 732e 6669 6e64 616c 6c28  .tracks.findall(
+0000d480: 2754 7261 636b 2729 3a0d 0a20 2020 2020  'Track'):..     
+0000d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000d4b0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+0000d4c0: 636b 5f69 6420 3d20 696e 7428 7472 6163  ck_id = int(trac
+0000d4d0: 6b2e 6765 7428 7365 6c66 2e74 7261 636b  k.get(self.track
+0000d4e0: 6964 5f6b 6579 2929 0d0a 2020 2020 2020  id_key))..      
+0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d500: 2020 6966 2074 7261 636b 5f69 6420 696e    if track_id in
+0000d510: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
+0000d520: 7261 636b 5f69 6473 3a0d 0a20 2020 2020  rack_ids:..     
+0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d540: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+0000d550: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
+0000d560: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
+0000d570: 6d61 7374 6572 5f74 7261 636b 5f63 6f6d  master_track_com
+0000d580: 7075 7465 722c 2074 7261 636b 2c20 7472  puter, track, tr
+0000d590: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
+0000d5a0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000d5b0: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000d5c0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
 0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5e0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-0000d5f0: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-0000d600: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d620: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000d630: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
-0000d640: 2073 656c 662e 636f 756e 740d 0a20 2020   self.count..   
-0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d660: 2020 2020 2020 2020 2020 2020 2072 2e72               r.r
-0000d670: 6573 756c 7428 290d 0a20 2020 2020 2020  esult()..       
-0000d680: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000d690: 2020 2069 6620 7365 6c66 2e63 6861 6e6e     if self.chann
-0000d6a0: 656c 5f73 6567 5f69 6d61 6765 2069 7320  el_seg_image is 
-0000d6b0: 6e6f 7420 4e6f 6e65 3a20 200d 0a20 2020  not None:  ..   
-0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000d6e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000d6f0: 662e 5f63 7265 6174 655f 7365 636f 6e64  f._create_second
-0000d700: 5f63 6861 6e6e 656c 5f78 6d6c 2829 0d0a  _channel_xml()..
+0000d5e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d600: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d610: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000d620: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
+0000d630: 7469 6e67 2054 7261 636b 7322 0d0a 2020  ting Tracks"..  
+0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d650: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d660: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000d670: 7261 6e67 6520 3d20 280d 0a20 2020 2020  range = (..     
+0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d690: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+0000d6a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6c0: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
+0000d6d0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+0000d6e0: 6473 292c 0d0a 2020 2020 2020 2020 2020  ds),..          
+0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d700: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
 0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d720: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-0000d730: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
-0000d740: 2c76 2920 696e 2073 656c 662e 6772 6170  ,v) in self.grap
-0000d750: 685f 7370 6c69 742e 6974 656d 7328 293a  h_split.items():
-0000d760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d770: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d790: 2020 2020 2020 2020 2020 2064 6175 6768             daugh
-0000d7a0: 7465 725f 7472 6163 6b5f 6964 203d 2020  ter_track_id =  
-0000d7b0: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
-0000d7c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-0000d7d0: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
-0000d7e0: 6f61 7428 6b29 295d 5b73 656c 662e 756e  oat(k))][self.un
-0000d7f0: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
-0000d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d810: 2020 2020 2020 2020 2020 2020 7061 7265              pare
-0000d820: 6e74 5f74 7261 636b 5f69 6420 3d20 696e  nt_track_id = in
-0000d830: 7428 666c 6f61 7428 7374 7228 7365 6c66  t(float(str(self
-0000d840: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-0000d850: 7065 7274 6965 735b 696e 7428 666c 6f61  perties[int(floa
-0000d860: 7428 7629 295d 5b73 656c 662e 756e 6971  t(v))][self.uniq
-0000d870: 7565 6964 5f6b 6579 5d29 2929 0d0a 2020  ueid_key])))..  
-0000d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d890: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-0000d8a0: 7261 7068 5f74 7261 636b 735b 6461 7567  raph_tracks[daug
-0000d8b0: 6874 6572 5f74 7261 636b 5f69 645d 203d  hter_track_id] =
-0000d8c0: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
-0000d8d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000d8e0: 7072 696e 7428 2767 6574 7469 6e67 2061  print('getting a
-0000d8f0: 7474 7269 6275 7465 7327 2920 2020 2020  ttributes')     
-0000d900: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000d910: 2020 2020 2020 2020 2073 656c 662e 5f67           self._g
-0000d920: 6574 5f61 7474 7269 6275 7465 7328 290d  et_attributes().
-0000d930: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
-0000d940: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000d950: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
-0000d960: 2020 2020 2020 666f 7220 7472 6163 6b5f        for track_
-0000d970: 6964 2069 6e20 7365 6c66 2e66 696c 7465  id in self.filte
-0000d980: 7265 645f 7472 6163 6b5f 6964 733a 0d0a  red_track_ids:..
+0000d720: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000d730: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+0000d740: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+0000d750: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
+0000d760: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+0000d770: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
+0000d780: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
+0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d7b0: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
+0000d7c0: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d7f0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+0000d800: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d820: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d830: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000d840: 2e76 616c 7565 203d 2073 656c 662e 636f  .value = self.co
+0000d850: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d870: 2020 2020 2072 2e72 6573 756c 7428 290d       r.result().
+0000d880: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000d890: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000d8a0: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+0000d8b0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+0000d8c0: 3a20 200d 0a20 2020 2020 2020 2020 2020  :  ..           
+0000d8d0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8f0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
+0000d900: 655f 7365 636f 6e64 5f63 6861 6e6e 656c  e_second_channel
+0000d910: 5f78 6d6c 2829 0d0a 2020 2020 2020 2020  _xml()..        
+0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d930: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000d940: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+0000d950: 656c 662e 6772 6170 685f 7370 6c69 742e  elf.graph_split.
+0000d960: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+0000d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d980: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9b0: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-0000d9c0: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-0000d9d0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000da00: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000da10: 2e6c 6162 656c 203d 2022 4a75 7374 206f  .label = "Just o
-0000da20: 6e65 206d 6f72 6520 7468 696e 6722 0d0a  ne more thing"..
-0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da50: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000da60: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
-0000da70: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-0000da80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9a0: 2020 2064 6175 6768 7465 725f 7472 6163     daughter_trac
+0000d9b0: 6b5f 6964 203d 2020 696e 7428 666c 6f61  k_id =  int(floa
+0000d9c0: 7428 7374 7228 7365 6c66 2e75 6e69 7175  t(str(self.uniqu
+0000d9d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000d9e0: 735b 696e 7428 666c 6f61 7428 6b29 295d  s[int(float(k))]
+0000d9f0: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
+0000da00: 6579 5d29 2929 0d0a 2020 2020 2020 2020  ey])))..        
+0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da20: 2020 2020 7061 7265 6e74 5f74 7261 636b      parent_track
+0000da30: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
+0000da40: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
+0000da50: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000da60: 696e 7428 666c 6f61 7428 7629 295d 5b73  int(float(v))][s
+0000da70: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+0000da80: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
 0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 2020 2020 2030 2c0d 0a20 2020 2020 2020       0,..       
-0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dad0: 2020 2020 2020 2020 206c 656e 2873 656c           len(sel
-0000dae0: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
-0000daf0: 5f69 6473 292c 0d0a 2020 2020 2020 2020  _ids),..        
-0000db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db20: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000db50: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000db60: 2e73 686f 7728 290d 0a20 2020 2020 2020  .show()..       
-0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db90: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
-0000dba0: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
-0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbd0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000dbe0: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
-0000dbf0: 7365 6c66 2e63 6f75 6e74 0d0a 2020 2020  self.count..    
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc20: 7365 6c66 2e5f 6669 6e61 6c5f 7472 6163  self._final_trac
-0000dc30: 6b73 2874 7261 636b 5f69 6429 200d 0a0d  ks(track_id) ...
-0000dc40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000dc50: 7365 6c66 2e66 6f75 7269 6572 3a0d 0a20  self.fourier:.. 
-0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc70: 2020 7072 696e 7428 2763 6f6d 7075 7469    print('computi
-0000dc80: 6e67 2046 6f75 7269 6572 2729 0d0a 2020  ng Fourier')..  
+0000daa0: 2020 7365 6c66 2e67 7261 7068 5f74 7261    self.graph_tra
+0000dab0: 636b 735b 6461 7567 6874 6572 5f74 7261  cks[daughter_tra
+0000dac0: 636b 5f69 645d 203d 2070 6172 656e 745f  ck_id] = parent_
+0000dad0: 7472 6163 6b5f 6964 0d0a 0d0a 2020 2020  track_id....    
+0000dae0: 2020 2020 2020 2020 7072 696e 7428 2767          print('g
+0000daf0: 6574 7469 6e67 2061 7474 7269 6275 7465  etting attribute
+0000db00: 7327 2920 2020 2020 2020 2020 2020 2020  s')             
+0000db10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000db20: 2073 656c 662e 5f67 6574 5f61 7474 7269   self._get_attri
+0000db30: 6275 7465 7328 290d 0a20 2020 2020 2020  butes()..       
+0000db40: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000db50: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
+0000db60: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000db70: 7220 7472 6163 6b5f 6964 2069 6e20 7365  r track_id in se
+0000db80: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
+0000db90: 6b5f 6964 733a 0d0a 2020 2020 2020 2020  k_ids:..        
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbb0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000dbc0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000dbd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc00: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000dc10: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
+0000dc20: 2022 4a75 7374 206f 6e65 206d 6f72 6520   "Just one more 
+0000dc30: 7468 696e 6722 0d0a 2020 2020 2020 2020  thing"..        
+0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc60: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000dc70: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
+0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dca0: 2073 656c 662e 5f63 6f6d 7075 7465 5f70   self._compute_p
-0000dcb0: 6865 6e6f 7479 7065 7328 2920 2020 2020  henotypes()     
+0000dca0: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
+0000dcb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000dce0: 2073 656c 662e 5f74 656d 706f 7261 6c5f   self._temporal_
-0000dcf0: 706c 6f74 735f 7472 6163 6b6d 6174 6528  plots_trackmate(
-0000dd00: 2920 2020 2020 2020 200d 0a0d 0a0d 0a20  )        ...... 
-0000dd10: 2020 2064 6566 205f 6372 6561 7465 5f73     def _create_s
-0000dd20: 6563 6f6e 645f 6368 616e 6e65 6c5f 786d  econd_channel_xm
-0000dd30: 6c28 7365 6c66 293a 0d0a 2020 2020 2020  l(self):..      
-0000dd40: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000dd50: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000dd60: 2827 5472 616e 7366 6572 7269 6e67 2058  ('Transferring X
-0000dd70: 4d4c 2729 2020 200d 0a20 2020 2020 2020  ML')   ..       
-0000dd80: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-0000dd90: 6e6e 656c 5f66 696c 7465 7265 645f 7472  nnel_filtered_tr
-0000dda0: 6163 6b73 203d 205b 5d20 2020 2020 2020  acks = []       
-0000ddb0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000ddc0: 2020 2020 2020 2020 2020 2066 6f72 2053             for S
-0000ddd0: 706f 746f 626a 6563 7420 696e 2073 656c  potobject in sel
-0000dde0: 662e 786d 6c5f 726f 6f74 2e69 7465 7228  f.xml_root.iter(
-0000ddf0: 2753 706f 7427 293a 0d0a 2020 2020 2020  'Spot'):..      
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 2020 2020 6365 6c6c 5f69 6420 3d20        cell_id = 
-0000de20: 696e 7428 5370 6f74 6f62 6a65 6374 2e67  int(Spotobject.g
-0000de30: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
-0000de40: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de60: 2020 6966 2063 656c 6c5f 6964 2069 6e20    if cell_id in 
-0000de70: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-0000de80: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000de90: 6965 732e 6b65 7973 2829 3a20 2020 2020  ies.keys():     
-0000dea0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dec0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dee0: 2020 2020 2020 206e 6577 5f70 6f73 6974         new_posit
-0000def0: 696f 6e78 203d 2020 7365 6c66 2e63 6861  ionx =  self.cha
-0000df00: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000df10: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-0000df20: 5f69 645d 5b73 656c 662e 7870 6f73 6964  _id][self.xposid
-0000df30: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-0000df40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df50: 2020 2020 2020 2020 2020 206e 6577 5f70             new_p
-0000df60: 6f73 6974 696f 6e79 203d 2020 7365 6c66  ositiony =  self
-0000df70: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000df80: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000df90: 6365 6c6c 5f69 645d 5b73 656c 662e 7970  cell_id][self.yp
-0000dfa0: 6f73 6964 5f6b 6579 5d0d 0a20 2020 2020  osid_key]..     
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfc0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000dfd0: 6577 5f70 6f73 6974 696f 6e7a 203d 2020  ew_positionz =  
-0000dfe0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-0000dff0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000e000: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
-0000e010: 662e 7a70 6f73 6964 5f6b 6579 5d0d 0a0d  f.zposid_key]...
-0000e020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e040: 2020 2020 206e 6577 5f74 6f74 616c 5f69       new_total_i
-0000e050: 6e74 656e 7369 7479 203d 2073 656c 662e  ntensity = self.
-0000e060: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000e070: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000e080: 656c 6c5f 6964 5d5b 7365 6c66 2e74 6f74  ell_id][self.tot
-0000e090: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-0000e0a0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dce0: 206c 656e 2873 656c 662e 6669 6c74 6572   len(self.filter
+0000dcf0: 6564 5f74 7261 636b 5f69 6473 292c 0d0a  ed_track_ids),..
+0000dd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd20: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd50: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000dd60: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
+0000dd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd90: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000dda0: 756e 7420 3d20 7365 6c66 2e63 6f75 6e74  unt = self.count
+0000ddb0: 202b 2031 0d0a 2020 2020 2020 2020 2020   + 1..          
+0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000dde0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000ddf0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f75  value = self.cou
+0000de00: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
+0000de30: 6e61 6c5f 7472 6163 6b73 2874 7261 636b  nal_tracks(track
+0000de40: 5f69 6429 200d 0a0d 0a20 2020 2020 2020  _id) ....       
+0000de50: 2020 2020 2069 6620 7365 6c66 2e66 6f75       if self.fou
+0000de60: 7269 6572 3a0d 0a20 2020 2020 2020 2020  rier:..         
+0000de70: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000de80: 2763 6f6d 7075 7469 6e67 2046 6f75 7269  'computing Fouri
+0000de90: 6572 2729 0d0a 2020 2020 2020 2020 2020  er')..          
+0000dea0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+0000deb0: 6f6d 7075 7465 5f70 6865 6e6f 7479 7065  ompute_phenotype
+0000dec0: 7328 2920 2020 2020 2020 2020 2020 2020  s()             
+0000ded0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000dee0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
+0000def0: 656d 706f 7261 6c5f 706c 6f74 735f 7472  emporal_plots_tr
+0000df00: 6163 6b6d 6174 6528 2920 2020 2020 2020  ackmate()       
+0000df10: 200d 0a0d 0a0d 0a20 2020 2064 6566 205f   ......    def _
+0000df20: 6372 6561 7465 5f73 6563 6f6e 645f 6368  create_second_ch
+0000df30: 616e 6e65 6c5f 786d 6c28 7365 6c66 293a  annel_xml(self):
+0000df40: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
+0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df60: 2020 2070 7269 6e74 2827 5472 616e 7366     print('Transf
+0000df70: 6572 7269 6e67 2058 4d4c 2729 2020 200d  erring XML')   .
+0000df80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000df90: 2020 2020 2063 6861 6e6e 656c 5f66 696c       channel_fil
+0000dfa0: 7465 7265 645f 7472 6163 6b73 203d 205b  tered_tracks = [
+0000dfb0: 5d20 2020 2020 2020 2020 2020 200d 0a20  ]            .. 
+0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfd0: 2020 2066 6f72 2053 706f 746f 626a 6563     for Spotobjec
+0000dfe0: 7420 696e 2073 656c 662e 786d 6c5f 726f  t in self.xml_ro
+0000dff0: 6f74 2e69 7465 7228 2753 706f 7427 293a  ot.iter('Spot'):
+0000e000: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e010: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+0000e020: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
+0000e030: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000e040: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
+0000e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e060: 2020 2020 2020 2020 2020 6966 2063 656c            if cel
+0000e070: 6c5f 6964 2069 6e20 7365 6c66 2e63 6861  l_id in self.cha
+0000e080: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+0000e090: 5f70 726f 7065 7274 6965 732e 6b65 7973  _properties.keys
+0000e0a0: 2829 3a20 2020 2020 2020 200d 0a20 2020  ():        ..   
 0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0c0: 2020 2020 2020 206e 6577 5f6d 6561 6e5f         new_mean_
-0000e0d0: 696e 7465 6e73 6974 7920 3d20 7365 6c66  intensity = self
-0000e0e0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000e0f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000e100: 6365 6c6c 5f69 645d 5b73 656c 662e 6d65  cell_id][self.me
-0000e110: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
-0000e120: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-0000e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e140: 2020 2020 2020 2020 206e 6577 5f72 6164           new_rad
-0000e150: 6975 7320 3d20 7365 6c66 2e63 6861 6e6e  ius = self.chann
-0000e160: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-0000e170: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-0000e180: 645d 5b73 656c 662e 7261 6469 7573 5f6b  d][self.radius_k
-0000e190: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1b0: 2020 2020 2020 2020 206e 6577 5f71 7561           new_qua
-0000e1c0: 6c69 7479 203d 2073 656c 662e 6368 616e  lity = self.chan
-0000e1d0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-0000e1e0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-0000e1f0: 6964 5d5b 7365 6c66 2e71 7561 6c69 7479  id][self.quality
-0000e200: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-0000e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e220: 2020 2020 2020 2020 2020 206e 6577 5f64             new_d
-0000e230: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-0000e240: 6b20 3d20 7365 6c66 2e63 6861 6e6e 656c  k = self.channel
-0000e250: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
-0000e260: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-0000e270: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
-0000e280: 656c 6c5f 6d61 736b 5f6b 6579 5d0d 0a0d  ell_mask_key]...
-0000e290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2b0: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
-0000e2c0: 7365 7428 7365 6c66 2e78 706f 7369 645f  set(self.xposid_
-0000e2d0: 6b65 792c 2073 7472 286e 6577 5f70 6f73  key, str(new_pos
-0000e2e0: 6974 696f 6e78 2929 2020 2020 200d 0a20  itionx))     .. 
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e310: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
-0000e320: 7428 7365 6c66 2e79 706f 7369 645f 6b65  t(self.yposid_ke
-0000e330: 792c 2073 7472 286e 6577 5f70 6f73 6974  y, str(new_posit
-0000e340: 696f 6e79 2929 0d0a 2020 2020 2020 2020  iony))..        
-0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e360: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-0000e370: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
-0000e380: 7a70 6f73 6964 5f6b 6579 2c20 7374 7228  zposid_key, str(
-0000e390: 6e65 775f 706f 7369 7469 6f6e 7a29 290d  new_positionz)).
-0000e3a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000e0c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e0f0: 6577 5f70 6f73 6974 696f 6e78 203d 2020  ew_positionx =  
+0000e100: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+0000e110: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000e120: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
+0000e130: 662e 7870 6f73 6964 5f6b 6579 5d0d 0a20  f.xposid_key].. 
+0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e160: 2020 206e 6577 5f70 6f73 6974 696f 6e79     new_positiony
+0000e170: 203d 2020 7365 6c66 2e63 6861 6e6e 656c   =  self.channel
+0000e180: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000e190: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000e1a0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+0000e1b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1d0: 2020 2020 2020 206e 6577 5f70 6f73 6974         new_posit
+0000e1e0: 696f 6e7a 203d 2020 7365 6c66 2e63 6861  ionz =  self.cha
+0000e1f0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+0000e200: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+0000e210: 5f69 645d 5b73 656c 662e 7a70 6f73 6964  _id][self.zposid
+0000e220: 5f6b 6579 5d0d 0a0d 0a20 2020 2020 2020  _key]....       
+0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e240: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000e250: 5f74 6f74 616c 5f69 6e74 656e 7369 7479  _total_intensity
+0000e260: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
+0000e270: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000e280: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+0000e290: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000e2a0: 7369 7479 5f6b 6579 5d0d 0a20 2020 2020  sity_key]..     
+0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e2d0: 6577 5f6d 6561 6e5f 696e 7465 6e73 6974  ew_mean_intensit
+0000e2e0: 7920 3d20 7365 6c66 2e63 6861 6e6e 656c  y = self.channel
+0000e2f0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000e300: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000e310: 5b73 656c 662e 6d65 616e 5f69 6e74 656e  [self.mean_inten
+0000e320: 7369 7479 5f6b 6579 5d0d 0a0d 0a20 2020  sity_key]....   
+0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e350: 206e 6577 5f72 6164 6975 7320 3d20 7365   new_radius = se
+0000e360: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000e370: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000e380: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
+0000e390: 7261 6469 7573 5f6b 6579 5d0d 0a20 2020  radius_key]..   
+0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3c0: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
-0000e3d0: 742e 7365 7428 7365 6c66 2e74 6f74 616c  t.set(self.total
-0000e3e0: 5f69 6e74 656e 7369 7479 5f6b 6579 2c20  _intensity_key, 
-0000e3f0: 7374 7228 6e65 775f 746f 7461 6c5f 696e  str(new_total_in
-0000e400: 7465 6e73 6974 7929 2920 2020 2020 0d0a  tensity))     ..
+0000e3c0: 206e 6577 5f71 7561 6c69 7479 203d 2073   new_quality = s
+0000e3d0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+0000e3e0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000e3f0: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
+0000e400: 2e71 7561 6c69 7479 5f6b 6579 5d0d 0a20  .quality_key].. 
 0000e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e430: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-0000e440: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
-0000e450: 656e 7369 7479 5f6b 6579 2c20 7374 7228  ensity_key, str(
-0000e460: 6e65 775f 6d65 616e 5f69 6e74 656e 7369  new_mean_intensi
-0000e470: 7479 2929 0d0a 0d0a 2020 2020 2020 2020  ty))....        
-0000e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e490: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-0000e4a0: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
-0000e4b0: 7261 6469 7573 5f6b 6579 2c20 7374 7228  radius_key, str(
-0000e4c0: 6e65 775f 7261 6469 7573 2929 2020 2020  new_radius))    
-0000e4d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4f0: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
-0000e500: 742e 7365 7428 7365 6c66 2e71 7561 6c69  t.set(self.quali
-0000e510: 7479 5f6b 6579 2c20 7374 7228 6e65 775f  ty_key, str(new_
-0000e520: 7175 616c 6974 7929 290d 0a20 2020 2020  quality))..     
-0000e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e540: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000e550: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
-0000e560: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-0000e570: 5f6d 6173 6b5f 6b65 792c 2073 7472 286e  _mask_key, str(n
-0000e580: 6577 5f64 6973 7461 6e63 655f 6365 6c6c  ew_distance_cell
-0000e590: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
-0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5b0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-0000e5c0: 636b 5f69 6420 3d20 7365 6c66 2e63 6861  ck_id = self.cha
-0000e5d0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000e5e0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-0000e5f0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e74  cell_id)][self.t
-0000e600: 7261 636b 6964 5f6b 6579 5d0d 0a20 2020  rackid_key]..   
-0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e430: 2020 206e 6577 5f64 6973 7461 6e63 655f     new_distance_
+0000e440: 6365 6c6c 5f6d 6173 6b20 3d20 7365 6c66  cell_mask = self
+0000e450: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000e460: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000e470: 6365 6c6c 5f69 645d 5b73 656c 662e 6469  cell_id][self.di
+0000e480: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0000e490: 5f6b 6579 5d0d 0a0d 0a20 2020 2020 2020  _key]....       
+0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4b0: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000e4c0: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000e4d0: 2e78 706f 7369 645f 6b65 792c 2073 7472  .xposid_key, str
+0000e4e0: 286e 6577 5f70 6f73 6974 696f 6e78 2929  (new_positionx))
+0000e4f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e510: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000e520: 626a 6563 742e 7365 7428 7365 6c66 2e79  bject.set(self.y
+0000e530: 706f 7369 645f 6b65 792c 2073 7472 286e  posid_key, str(n
+0000e540: 6577 5f70 6f73 6974 696f 6e79 2929 0d0a  ew_positiony))..
+0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e570: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000e580: 6574 2873 656c 662e 7a70 6f73 6964 5f6b  et(self.zposid_k
+0000e590: 6579 2c20 7374 7228 6e65 775f 706f 7369  ey, str(new_posi
+0000e5a0: 7469 6f6e 7a29 290d 0a0d 0a20 2020 2020  tionz))....     
+0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000e5d0: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
+0000e5e0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000e5f0: 7479 5f6b 6579 2c20 7374 7228 6e65 775f  ty_key, str(new_
+0000e600: 746f 7461 6c5f 696e 7465 6e73 6974 7929  total_intensity)
+0000e610: 2920 2020 2020 0d0a 2020 2020 2020 2020  )     ..        
 0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e630: 2063 6861 6e6e 656c 5f66 696c 7465 7265   channel_filtere
-0000e640: 645f 7472 6163 6b73 2e61 7070 656e 6428  d_tracks.append(
-0000e650: 7472 6163 6b5f 6964 290d 0a20 2020 2020  track_id)..     
-0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e670: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000e680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e690: 2020 2020 2073 656c 662e 786d 6c5f 7472       self.xml_tr
-0000e6a0: 6565 2e77 7269 7465 286f 732e 7061 7468  ee.write(os.path
-0000e6b0: 2e6a 6f69 6e28 7365 6c66 2e63 6861 6e6e  .join(self.chann
-0000e6c0: 656c 5f78 6d6c 5f70 6174 682c 2073 656c  el_xml_path, sel
-0000e6d0: 662e 6368 616e 6e65 6c5f 786d 6c5f 6e61  f.channel_xml_na
-0000e6e0: 6d65 2929 200d 0a0d 0a20 2020 2064 6566  me)) ....    def
-0000e6f0: 205f 6765 745f 786d 6c5f 6461 7461 2873   _get_xml_data(s
-0000e700: 656c 6629 3a0d 0a0d 0a20 2020 2020 2020  elf):....       
-0000e710: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-0000e720: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000e730: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
-0000e740: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
-0000e750: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000e760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e770: 6368 616e 6e65 6c5f 786d 6c5f 636f 6e74  channel_xml_cont
-0000e780: 656e 7420 3d20 7365 6c66 2e78 6d6c 5f63  ent = self.xml_c
-0000e790: 6f6e 7465 6e74 0d0a 2020 2020 2020 2020  ontent..        
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e7b0: 6c66 2e78 6d6c 5f74 7265 6520 3d20 6574  lf.xml_tree = et
-0000e7c0: 2e70 6172 7365 2873 656c 662e 786d 6c5f  .parse(self.xml_
-0000e7d0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-0000e7e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e7f0: 662e 786d 6c5f 726f 6f74 203d 2073 656c  f.xml_root = sel
-0000e800: 662e 786d 6c5f 7472 6565 2e67 6574 726f  f.xml_tree.getro
-0000e810: 6f74 2829 0d0a 2020 2020 2020 2020 2020  ot()..          
-0000e820: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e830: 2e63 6861 6e6e 656c 5f78 6d6c 5f6e 616d  .channel_xml_nam
-0000e840: 6520 3d20 2773 6563 6f6e 645f 6368 616e  e = 'second_chan
-0000e850: 6e65 6c5f 2720 2b20 6f73 2e70 6174 682e  nel_' + os.path.
-0000e860: 7370 6c69 7465 7874 286f 732e 7061 7468  splitext(os.path
-0000e870: 2e62 6173 656e 616d 6528 7365 6c66 2e78  .basename(self.x
-0000e880: 6d6c 5f70 6174 6829 295b 305d 202b 2027  ml_path))[0] + '
-0000e890: 2e78 6d6c 270d 0a20 2020 2020 2020 2020  .xml'..         
-0000e8a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e8b0: 662e 6368 616e 6e65 6c5f 786d 6c5f 7061  f.channel_xml_pa
-0000e8c0: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
-0000e8d0: 6e61 6d65 2873 656c 662e 786d 6c5f 7061  name(self.xml_pa
-0000e8e0: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
-0000e8f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e900: 5f63 7265 6174 655f 6368 616e 6e65 6c5f  _create_channel_
-0000e910: 7472 6565 2829 0d0a 2020 2020 2020 2020  tree()..        
-0000e920: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000e930: 636c 7573 7465 725f 6d6f 6465 6c20 6973  cluster_model is
-0000e940: 206e 6f74 204e 6f6e 6520 616e 6420 7365   not None and se
-0000e950: 6c66 2e73 6567 5f69 6d61 6765 2069 7320  lf.seg_image is 
-0000e960: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e980: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
-0000e990: 6c5f 636f 6e74 656e 7420 3d20 7365 6c66  l_content = self
-0000e9a0: 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a 2020  .xml_content..  
-0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9c0: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
-0000e9d0: 5f78 6d6c 5f74 7265 6520 3d20 6574 2e70  _xml_tree = et.p
-0000e9e0: 6172 7365 2873 656c 662e 786d 6c5f 7061  arse(self.xml_pa
-0000e9f0: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
-0000ea00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ea10: 2e6d 6173 7465 725f 786d 6c5f 726f 6f74  .master_xml_root
-0000ea20: 203d 2073 656c 662e 6d61 7374 6572 5f78   = self.master_x
-0000ea30: 6d6c 5f74 7265 652e 6765 7472 6f6f 7428  ml_tree.getroot(
-0000ea40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ea50: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000ea60: 6173 7465 725f 786d 6c5f 6e61 6d65 203d  aster_xml_name =
-0000ea70: 2027 6d61 7374 6572 5f27 202b 2073 656c   'master_' + sel
-0000ea80: 662e 6d61 7374 6572 5f65 7874 7261 5f6e  f.master_extra_n
-0000ea90: 616d 6520 202b 206f 732e 7061 7468 2e73  ame  + os.path.s
-0000eaa0: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
-0000eab0: 6261 7365 6e61 6d65 2873 656c 662e 786d  basename(self.xm
-0000eac0: 6c5f 7061 7468 2929 5b30 5d20 2b20 272e  l_path))[0] + '.
-0000ead0: 786d 6c27 0d0a 2020 2020 2020 2020 2020  xml'..          
-0000eae0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000eaf0: 662e 6d61 7374 6572 5f78 6d6c 5f70 6174  f.master_xml_pat
-0000eb00: 6820 3d20 6f73 2e70 6174 682e 6469 726e  h = os.path.dirn
-0000eb10: 616d 6528 7365 6c66 2e78 6d6c 5f70 6174  ame(self.xml_pat
-0000eb20: 6829 2020 2020 2020 0d0a 2020 2020 2020  h)      ..      
-0000eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb40: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000eb50: 2020 2073 656c 662e 756e 6971 7565 5f6f     self.unique_o
-0000eb60: 626a 6563 7473 203d 207b 7d0d 0a20 2020  bjects = {}..   
-0000eb70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000eb80: 662e 756e 6971 7565 5f70 726f 7065 7274  f.unique_propert
-0000eb90: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
-0000eba0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-0000ebb0: 6c6c 5472 6163 6b49 6473 203d 205b 5d0d  llTrackIds = [].
-0000ebc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ebd0: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-0000ebe0: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
-0000ebf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ec00: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
-0000ec10: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-0000ec20: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-0000ec30: 7472 6163 6b5f 7072 6f70 6572 7469 6573  track_properties
-0000ec40: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-0000ec50: 2020 2020 2020 2073 656c 662e 7370 6c69         self.spli
-0000ec60: 745f 706f 696e 7473 5f74 696d 6573 203d  t_points_times =
-0000ec70: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-0000ec80: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000ec90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000eca0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ecb0: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
-0000ecc0: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
-0000ecd0: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
-0000ece0: 6976 6964 696e 6754 7261 636b 4964 732e  ividingTrackIds.
-0000ecf0: 6170 7065 6e64 284e 6f6e 6529 0d0a 2020  append(None)..  
-0000ed00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ed10: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-0000ed20: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
-0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ed50: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
-0000ed60: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
-0000ed70: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
-0000ed80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ed90: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
-0000eda0: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
-0000edb0: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
-0000edc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000edd0: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
-0000ede0: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
-0000edf0: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
-0000ee00: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000ee10: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000ee20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ee30: 2e53 706f 746f 626a 6563 7473 203d 2073  .Spotobjects = s
-0000ee40: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
-0000ee50: 6669 6e64 2827 4d6f 6465 6c27 292e 6669  find('Model').fi
-0000ee60: 6e64 2827 416c 6c53 706f 7473 2729 0d0a  nd('AllSpots')..
-0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee80: 2320 4578 7472 6163 7420 7468 6520 7472  # Extract the tr
-0000ee90: 6163 6b73 2066 726f 6d20 786d 6c0d 0a20  acks from xml.. 
-0000eea0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000eeb0: 656c 662e 7472 6163 6b73 203d 2073 656c  elf.tracks = sel
-0000eec0: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
-0000eed0: 6e64 2822 4d6f 6465 6c22 292e 6669 6e64  nd("Model").find
-0000eee0: 2822 416c 6c54 7261 636b 7322 290d 0a20  ("AllTracks").. 
-0000eef0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ef00: 656c 662e 7365 7474 696e 6773 203d 2073  elf.settings = s
-0000ef10: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
-0000ef20: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
-0000ef30: 2e66 696e 6428 2249 6d61 6765 4461 7461  .find("ImageData
-0000ef40: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000ef50: 2020 2020 7365 6c66 2e78 6361 6c69 6272      self.xcalibr
-0000ef60: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
-0000ef70: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000ef80: 2270 6978 656c 7769 6474 6822 2929 0d0a  "pixelwidth"))..
-0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efa0: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
-0000efb0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
-0000efc0: 6574 7469 6e67 732e 6765 7428 2270 6978  ettings.get("pix
-0000efd0: 656c 6865 6967 6874 2229 290d 0a20 2020  elheight"))..   
-0000efe0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000eff0: 662e 7a63 616c 6962 7261 7469 6f6e 203d  f.zcalibration =
-0000f000: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
-0000f010: 696e 6773 2e67 6574 2822 766f 7865 6c64  ings.get("voxeld
-0000f020: 6570 7468 2229 290d 0a20 2020 2020 2020  epth"))..       
-0000f030: 2020 2020 2020 2020 2073 656c 662e 7463           self.tc
-0000f040: 616c 6962 7261 7469 6f6e 203d 2069 6e74  alibration = int
-0000f050: 2866 6c6f 6174 2873 656c 662e 7365 7474  (float(self.sett
-0000f060: 696e 6773 2e67 6574 2822 7469 6d65 696e  ings.get("timein
-0000f070: 7465 7276 616c 2229 2929 0d0a 2020 2020  terval")))..    
-0000f080: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f090: 2e64 6574 6563 746f 7273 6574 7469 6e67  .detectorsetting
-0000f0a0: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000f0b0: 7465 6e74 2e66 696e 6428 2253 6574 7469  tent.find("Setti
-0000f0c0: 6e67 7322 292e 6669 6e64 2822 4465 7465  ngs").find("Dete
-0000f0d0: 6374 6f72 5365 7474 696e 6773 2229 0d0a  ctorSettings")..
-0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0f0: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
-0000f100: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
-0000f110: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
-0000f120: 696e 6773 2229 2e66 696e 6428 2242 6173  ings").find("Bas
-0000f130: 6963 5365 7474 696e 6773 2229 0d0a 2020  icSettings")..  
-0000f140: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f150: 6c66 2e64 6574 6563 746f 7263 6861 6e6e  lf.detectorchann
-0000f160: 656c 203d 2069 6e74 2866 6c6f 6174 2873  el = int(float(s
-0000f170: 656c 662e 6465 7465 6374 6f72 7365 7474  elf.detectorsett
-0000f180: 696e 6773 2e67 6574 2822 5441 5247 4554  ings.get("TARGET
-0000f190: 5f43 4841 4e4e 454c 2229 2929 0d0a 2020  _CHANNEL")))..  
-0000f1a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f1b0: 6c66 2e74 7374 6172 7420 3d20 696e 7428  lf.tstart = int(
-0000f1c0: 666c 6f61 7428 7365 6c66 2e62 6173 6963  float(self.basic
-0000f1d0: 7365 7474 696e 6773 2e67 6574 2822 7473  settings.get("ts
-0000f1e0: 7461 7274 2229 2929 0d0a 2020 2020 2020  tart")))..      
-0000f1f0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000f200: 656e 6420 3d20 696e 7428 666c 6f61 7428  end = int(float(
-0000f210: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
-0000f220: 6773 2e67 6574 2822 7465 6e64 2229 2929  gs.get("tend")))
-0000f230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f240: 2020 7365 6c66 2e5f 6765 745f 626f 756e    self._get_boun
-0000f250: 6461 7279 5f70 6f69 6e74 7328 290d 0a20  dary_points().. 
-0000f260: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000f270: 7269 6e74 2827 4974 6572 6174 696e 6720  rint('Iterating 
-0000f280: 6f76 6572 2073 706f 7473 2069 6e20 6672  over spots in fr
-0000f290: 616d 6527 290d 0a20 2020 2020 2020 2020  ame')..         
-0000f2a0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
-0000f2b0: 7420 3d20 300d 0a20 2020 2020 2020 2020  t = 0..         
-0000f2c0: 2020 2020 2020 2066 7574 7572 6573 203d         futures =
-0000f2d0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-0000f2e0: 2020 2020 2020 2077 6974 6820 636f 6e63         with conc
-0000f2f0: 7572 7265 6e74 2e66 7574 7572 6573 2e54  urrent.futures.T
-0000f300: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
-0000f310: 7228 6d61 785f 776f 726b 6572 7320 3d20  r(max_workers = 
-0000f320: 6f73 2e63 7075 5f63 6f75 6e74 2829 2920  os.cpu_count()) 
-0000f330: 6173 2065 7865 6375 746f 723a 0d0a 2020  as executor:..  
-0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f350: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000f360: 2020 2020 2020 2020 666f 7220 6672 616d          for fram
-0000f370: 6520 696e 2073 656c 662e 5370 6f74 6f62  e in self.Spotob
-0000f380: 6a65 6374 732e 6669 6e64 616c 6c28 2753  jects.findall('S
-0000f390: 706f 7473 496e 4672 616d 6527 293a 0d0a  potsInFrame'):..
-0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3b0: 2020 2020 2020 2020 2020 2020 2066 7574               fut
-0000f3c0: 7572 6573 2e61 7070 656e 6428 6578 6563  ures.append(exec
-0000f3d0: 7574 6f72 2e73 7562 6d69 7428 7365 6c66  utor.submit(self
-0000f3e0: 2e5f 7370 6f74 5f63 6f6d 7075 7465 722c  ._spot_computer,
-0000f3f0: 2066 7261 6d65 2929 0d0a 2020 2020 2020   frame))..      
-0000f400: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000f410: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000f420: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
-0000f430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f450: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f470: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000f480: 6772 6573 735f 6261 722e 6c61 6265 6c20  gress_bar.label 
-0000f490: 3d20 2243 6f6c 6c65 6374 696e 6720 5370  = "Collecting Sp
-0000f4a0: 6f74 7322 0d0a 2020 2020 2020 2020 2020  ots"..          
-0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4c0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000f4d0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
-0000f4e0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
-0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f500: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-0000f510: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000f520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f530: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
-0000f540: 7574 7572 6573 292c 0d0a 2020 2020 2020  utures),..      
-0000f550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f560: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-0000f570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f590: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000f5a0: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
-0000f5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f5c0: 2020 2020 2066 6f72 2072 2069 6e20 636f       for r in co
-0000f5d0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
-0000f5e0: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
-0000f5f0: 7475 7265 7329 3a0d 0a20 2020 2020 2020  tures):..       
-0000f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f610: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f620: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
-0000f630: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+0000e630: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+0000e640: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+0000e650: 6d65 616e 5f69 6e74 656e 7369 7479 5f6b  mean_intensity_k
+0000e660: 6579 2c20 7374 7228 6e65 775f 6d65 616e  ey, str(new_mean
+0000e670: 5f69 6e74 656e 7369 7479 2929 0d0a 0d0a  _intensity))....
+0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6a0: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000e6b0: 6574 2873 656c 662e 7261 6469 7573 5f6b  et(self.radius_k
+0000e6c0: 6579 2c20 7374 7228 6e65 775f 7261 6469  ey, str(new_radi
+0000e6d0: 7573 2929 2020 2020 200d 0a20 2020 2020  us))     ..     
+0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000e700: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
+0000e710: 6c66 2e71 7561 6c69 7479 5f6b 6579 2c20  lf.quality_key, 
+0000e720: 7374 7228 6e65 775f 7175 616c 6974 7929  str(new_quality)
+0000e730: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e750: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
+0000e760: 742e 7365 7428 7365 6c66 2e64 6973 7461  t.set(self.dista
+0000e770: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+0000e780: 792c 2073 7472 286e 6577 5f64 6973 7461  y, str(new_dista
+0000e790: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
+0000e7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7c0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
+0000e7d0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+0000e7e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000e7f0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+0000e800: 5d5b 7365 6c66 2e74 7261 636b 6964 5f6b  ][self.trackid_k
+0000e810: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e830: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
+0000e840: 5f66 696c 7465 7265 645f 7472 6163 6b73  _filtered_tracks
+0000e850: 2e61 7070 656e 6428 7472 6163 6b5f 6964  .append(track_id
+0000e860: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e880: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000e890: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e8a0: 662e 786d 6c5f 7472 6565 2e77 7269 7465  f.xml_tree.write
+0000e8b0: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
+0000e8c0: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f70  lf.channel_xml_p
+0000e8d0: 6174 682c 2073 656c 662e 6368 616e 6e65  ath, self.channe
+0000e8e0: 6c5f 786d 6c5f 6e61 6d65 2929 200d 0a0d  l_xml_name)) ...
+0000e8f0: 0a20 2020 2064 6566 205f 6765 745f 786d  .    def _get_xm
+0000e900: 6c5f 6461 7461 2873 656c 6629 3a0d 0a0d  l_data(self):...
+0000e910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e920: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+0000e930: 2020 2020 2069 6620 7365 6c66 2e63 6861       if self.cha
+0000e940: 6e6e 656c 5f73 6567 5f69 6d61 6765 2069  nnel_seg_image i
+0000e950: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e970: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+0000e980: 786d 6c5f 636f 6e74 656e 7420 3d20 7365  xml_content = se
+0000e990: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a  lf.xml_content..
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9b0: 2020 2020 2020 7365 6c66 2e78 6d6c 5f74        self.xml_t
+0000e9c0: 7265 6520 3d20 6574 2e70 6172 7365 2873  ree = et.parse(s
+0000e9d0: 656c 662e 786d 6c5f 7061 7468 290d 0a20  elf.xml_path).. 
+0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9f0: 2020 2020 2073 656c 662e 786d 6c5f 726f       self.xml_ro
+0000ea00: 6f74 203d 2073 656c 662e 786d 6c5f 7472  ot = self.xml_tr
+0000ea10: 6565 2e67 6574 726f 6f74 2829 0d0a 2020  ee.getroot()..  
+0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea30: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+0000ea40: 5f78 6d6c 5f6e 616d 6520 3d20 2773 6563  _xml_name = 'sec
+0000ea50: 6f6e 645f 6368 616e 6e65 6c5f 2720 2b20  ond_channel_' + 
+0000ea60: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
+0000ea70: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
+0000ea80: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
+0000ea90: 295b 305d 202b 2027 2e78 6d6c 270d 0a20  )[0] + '.xml'.. 
+0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eab0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+0000eac0: 6c5f 786d 6c5f 7061 7468 203d 206f 732e  l_xml_path = os.
+0000ead0: 7061 7468 2e64 6972 6e61 6d65 2873 656c  path.dirname(sel
+0000eae0: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
+0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb00: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
+0000eb10: 6368 616e 6e65 6c5f 7472 6565 2829 0d0a  channel_tree()..
+0000eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb30: 6966 2073 656c 662e 636c 7573 7465 725f  if self.cluster_
+0000eb40: 6d6f 6465 6c20 6973 206e 6f74 204e 6f6e  model is not Non
+0000eb50: 6520 616e 6420 7365 6c66 2e73 6567 5f69  e and self.seg_i
+0000eb60: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+0000eb70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000eb80: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0000eb90: 6173 7465 725f 786d 6c5f 636f 6e74 656e  aster_xml_conten
+0000eba0: 7420 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  t = self.xml_con
+0000ebb0: 7465 6e74 0d0a 2020 2020 2020 2020 2020  tent..          
+0000ebc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ebd0: 662e 6d61 7374 6572 5f78 6d6c 5f74 7265  f.master_xml_tre
+0000ebe0: 6520 3d20 6574 2e70 6172 7365 2873 656c  e = et.parse(sel
+0000ebf0: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
+0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec10: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
+0000ec20: 786d 6c5f 726f 6f74 203d 2073 656c 662e  xml_root = self.
+0000ec30: 6d61 7374 6572 5f78 6d6c 5f74 7265 652e  master_xml_tree.
+0000ec40: 6765 7472 6f6f 7428 290d 0a20 2020 2020  getroot()..     
+0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec60: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
+0000ec70: 6c5f 6e61 6d65 203d 2027 6d61 7374 6572  l_name = 'master
+0000ec80: 5f27 202b 2073 656c 662e 6d61 7374 6572  _' + self.master
+0000ec90: 5f65 7874 7261 5f6e 616d 6520 202b 206f  _extra_name  + o
+0000eca0: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
+0000ecb0: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
+0000ecc0: 2873 656c 662e 786d 6c5f 7061 7468 2929  (self.xml_path))
+0000ecd0: 5b30 5d20 2b20 272e 786d 6c27 0d0a 2020  [0] + '.xml'..  
+0000ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecf0: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+0000ed00: 5f78 6d6c 5f70 6174 6820 3d20 6f73 2e70  _xml_path = os.p
+0000ed10: 6174 682e 6469 726e 616d 6528 7365 6c66  ath.dirname(self
+0000ed20: 2e78 6d6c 5f70 6174 6829 2020 2020 2020  .xml_path)      
+0000ed30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ed40: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000ed50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ed60: 756e 6971 7565 5f6f 626a 6563 7473 203d  unique_objects =
+0000ed70: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+0000ed80: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+0000ed90: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+0000eda0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000edb0: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+0000edc0: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
+0000edd0: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
+0000ede0: 7669 6469 6e67 5472 6163 6b49 6473 203d  vidingTrackIds =
+0000edf0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000ee00: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
+0000ee10: 5472 6163 6b49 6473 203d 205b 5d0d 0a20  TrackIds = [].. 
+0000ee20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ee30: 656c 662e 616c 6c5f 7472 6163 6b5f 7072  elf.all_track_pr
+0000ee40: 6f70 6572 7469 6573 203d 205b 5d0d 0a20  operties = [].. 
+0000ee50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ee60: 656c 662e 7370 6c69 745f 706f 696e 7473  elf.split_points
+0000ee70: 5f74 696d 6573 203d 205b 5d0d 0a0d 0a20  _times = [].... 
+0000ee80: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000ee90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eea0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000eeb0: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+0000eec0: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
+0000eed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000eee0: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
+0000eef0: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
+0000ef00: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+0000ef10: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000ef20: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000ef30: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000ef40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000ef50: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+0000ef60: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
+0000ef70: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
+0000ef80: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0000ef90: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+0000efa0: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
+0000efb0: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
+0000efc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000efd0: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
+0000efe0: 6163 6b49 6473 2e61 7070 656e 6428 7365  ackIds.append(se
+0000eff0: 6c66 2e54 7261 636b 6964 426f 7829 0d0a  lf.TrackidBox)..
+0000f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f020: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000f030: 2020 2020 7365 6c66 2e53 706f 746f 626a      self.Spotobj
+0000f040: 6563 7473 203d 2073 656c 662e 786d 6c5f  ects = self.xml_
+0000f050: 636f 6e74 656e 742e 6669 6e64 2827 4d6f  content.find('Mo
+0000f060: 6465 6c27 292e 6669 6e64 2827 416c 6c53  del').find('AllS
+0000f070: 706f 7473 2729 0d0a 2020 2020 2020 2020  pots')..        
+0000f080: 2020 2020 2020 2020 2320 4578 7472 6163          # Extrac
+0000f090: 7420 7468 6520 7472 6163 6b73 2066 726f  t the tracks fro
+0000f0a0: 6d20 786d 6c0d 0a20 2020 2020 2020 2020  m xml..         
+0000f0b0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000f0c0: 6b73 203d 2073 656c 662e 786d 6c5f 636f  ks = self.xml_co
+0000f0d0: 6e74 656e 742e 6669 6e64 2822 4d6f 6465  ntent.find("Mode
+0000f0e0: 6c22 292e 6669 6e64 2822 416c 6c54 7261  l").find("AllTra
+0000f0f0: 636b 7322 290d 0a20 2020 2020 2020 2020  cks")..         
+0000f100: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+0000f110: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
+0000f120: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
+0000f130: 7474 696e 6773 2229 2e66 696e 6428 2249  ttings").find("I
+0000f140: 6d61 6765 4461 7461 2229 0d0a 2020 2020  mageData")..    
+0000f150: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f160: 2e78 6361 6c69 6272 6174 696f 6e20 3d20  .xcalibration = 
+0000f170: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
+0000f180: 6e67 732e 6765 7428 2270 6978 656c 7769  ngs.get("pixelwi
+0000f190: 6474 6822 2929 0d0a 2020 2020 2020 2020  dth"))..        
+0000f1a0: 2020 2020 2020 2020 7365 6c66 2e79 6361          self.yca
+0000f1b0: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
+0000f1c0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000f1d0: 6765 7428 2270 6978 656c 6865 6967 6874  get("pixelheight
+0000f1e0: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
+0000f1f0: 2020 2020 2073 656c 662e 7a63 616c 6962       self.zcalib
+0000f200: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
+0000f210: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000f220: 2822 766f 7865 6c64 6570 7468 2229 290d  ("voxeldepth")).
+0000f230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f240: 2073 656c 662e 7463 616c 6962 7261 7469   self.tcalibrati
+0000f250: 6f6e 203d 2069 6e74 2866 6c6f 6174 2873  on = int(float(s
+0000f260: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000f270: 2822 7469 6d65 696e 7465 7276 616c 2229  ("timeinterval")
+0000f280: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000f290: 2020 2020 7365 6c66 2e64 6574 6563 746f      self.detecto
+0000f2a0: 7273 6574 7469 6e67 7320 3d20 7365 6c66  rsettings = self
+0000f2b0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
+0000f2c0: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
+0000f2d0: 6e64 2822 4465 7465 6374 6f72 5365 7474  nd("DetectorSett
+0000f2e0: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
+0000f2f0: 2020 2020 2020 2020 7365 6c66 2e62 6173          self.bas
+0000f300: 6963 7365 7474 696e 6773 203d 2073 656c  icsettings = sel
+0000f310: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000f320: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+0000f330: 696e 6428 2242 6173 6963 5365 7474 696e  ind("BasicSettin
+0000f340: 6773 2229 0d0a 2020 2020 2020 2020 2020  gs")..          
+0000f350: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
+0000f360: 746f 7263 6861 6e6e 656c 203d 2069 6e74  torchannel = int
+0000f370: 2866 6c6f 6174 2873 656c 662e 6465 7465  (float(self.dete
+0000f380: 6374 6f72 7365 7474 696e 6773 2e67 6574  ctorsettings.get
+0000f390: 2822 5441 5247 4554 5f43 4841 4e4e 454c  ("TARGET_CHANNEL
+0000f3a0: 2229 2929 0d0a 2020 2020 2020 2020 2020  ")))..          
+0000f3b0: 2020 2020 2020 7365 6c66 2e74 7374 6172        self.tstar
+0000f3c0: 7420 3d20 696e 7428 666c 6f61 7428 7365  t = int(float(se
+0000f3d0: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
+0000f3e0: 2e67 6574 2822 7473 7461 7274 2229 2929  .get("tstart")))
+0000f3f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f400: 2020 7365 6c66 2e74 656e 6420 3d20 696e    self.tend = in
+0000f410: 7428 666c 6f61 7428 7365 6c66 2e62 6173  t(float(self.bas
+0000f420: 6963 7365 7474 696e 6773 2e67 6574 2822  icsettings.get("
+0000f430: 7465 6e64 2229 2929 0d0a 2020 2020 2020  tend")))..      
+0000f440: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000f450: 6765 745f 626f 756e 6461 7279 5f70 6f69  get_boundary_poi
+0000f460: 6e74 7328 290d 0a20 2020 2020 2020 2020  nts()..         
+0000f470: 2020 2020 2020 2070 7269 6e74 2827 4974         print('It
+0000f480: 6572 6174 696e 6720 6f76 6572 2073 706f  erating over spo
+0000f490: 7473 2069 6e20 6672 616d 6527 290d 0a20  ts in frame').. 
+0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f4b0: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
+0000f4c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000f4d0: 7574 7572 6573 203d 205b 5d0d 0a0d 0a20  utures = [].... 
+0000f4e0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000f4f0: 6974 6820 636f 6e63 7572 7265 6e74 2e66  ith concurrent.f
+0000f500: 7574 7572 6573 2e54 6872 6561 6450 6f6f  utures.ThreadPoo
+0000f510: 6c45 7865 6375 746f 7228 6d61 785f 776f  lExecutor(max_wo
+0000f520: 726b 6572 7320 3d20 6f73 2e63 7075 5f63  rkers = os.cpu_c
+0000f530: 6f75 6e74 2829 2920 6173 2065 7865 6375  ount()) as execu
+0000f540: 746f 723a 0d0a 2020 2020 2020 2020 2020  tor:..          
+0000f550: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f570: 666f 7220 6672 616d 6520 696e 2073 656c  for frame in sel
+0000f580: 662e 5370 6f74 6f62 6a65 6374 732e 6669  f.Spotobjects.fi
+0000f590: 6e64 616c 6c28 2753 706f 7473 496e 4672  ndall('SpotsInFr
+0000f5a0: 616d 6527 293a 0d0a 2020 2020 2020 2020  ame'):..        
+0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5c0: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
+0000f5d0: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
+0000f5e0: 6d69 7428 7365 6c66 2e5f 7370 6f74 5f63  mit(self._spot_c
+0000f5f0: 6f6d 7075 7465 722c 2066 7261 6d65 2929  omputer, frame))
+0000f600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f610: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000f620: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+0000f630: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
 0000f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f650: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000f660: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000f670: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
-0000f680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6a0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000f6b0: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
-0000f6c0: 2020 7365 6c66 2e63 6f75 6e74 0d0a 2020    self.count..  
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6f0: 2020 722e 7265 7375 6c74 2829 0d0a 0d0a    r.result()....
+0000f650: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f680: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000f690: 722e 6c61 6265 6c20 3d20 2243 6f6c 6c65  r.label = "Colle
+0000f6a0: 6374 696e 6720 5370 6f74 7322 0d0a 2020  cting Spots"..  
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6d0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000f6e0: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f710: 7072 696e 7428 6627 4974 6572 6174 696e  print(f'Iteratin
-0000f720: 6720 6f76 6572 2074 7261 636b 7320 7b6c  g over tracks {l
-0000f730: 656e 2873 656c 662e 6669 6c74 6572 6564  en(self.filtered
-0000f740: 5f74 7261 636b 5f69 6473 297d 2729 2020  _track_ids)}')  
+0000f710: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
+0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f740: 2020 206c 656e 2866 7574 7572 6573 292c     len(futures),
 0000f750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f760: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
-0000f770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f780: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
-0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
-0000f7b0: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
-0000f7c0: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
-0000f7d0: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
-0000f7e0: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
-0000f7f0: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
-0000f800: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f770: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f790: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f7a0: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
+0000f7b0: 686f 7728 290d 0a0d 0a20 2020 2020 2020  how()....       
+0000f7c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000f7d0: 2072 2069 6e20 636f 6e63 7572 7265 6e74   r in concurrent
+0000f7e0: 2e66 7574 7572 6573 2e61 735f 636f 6d70  .futures.as_comp
+0000f7f0: 6c65 7465 6428 6675 7475 7265 7329 3a0d  leted(futures):.
+0000f800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f820: 2066 6f72 2074 7261 636b 2069 6e20 7365   for track in se
-0000f830: 6c66 2e74 7261 636b 732e 6669 6e64 616c  lf.tracks.findal
-0000f840: 6c28 2754 7261 636b 2729 3a0d 0a20 2020  l('Track'):..   
+0000f820: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000f830: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
+0000f840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f880: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-0000f890: 3d20 696e 7428 7472 6163 6b2e 6765 7428  = int(track.get(
-0000f8a0: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-0000f8b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8d0: 6966 2074 7261 636b 5f69 6420 696e 2073  if track_id in s
-0000f8e0: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
-0000f8f0: 636b 5f69 6473 3a0d 0a20 2020 2020 2020  ck_ids:..       
-0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f910: 2020 2020 2020 2020 2020 2066 7574 7572             futur
-0000f920: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
-0000f930: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
-0000f940: 7472 6163 6b5f 636f 6d70 7574 6572 2c20  track_computer, 
-0000f950: 7472 6163 6b2c 2074 7261 636b 5f69 6429  track, track_id)
-0000f960: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f970: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000f980: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000f990: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9e0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000f9f0: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
-0000fa00: 6563 7469 6e67 2054 7261 636b 7322 0d0a  ecting Tracks"..
-0000fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa30: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000fa40: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
-0000fa50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f860: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000f870: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+0000f880: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f8b0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000f8c0: 2e76 616c 7565 203d 2020 7365 6c66 2e63  .value =  self.c
+0000f8d0: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8f0: 2020 2020 2020 2020 2020 722e 7265 7375            r.resu
+0000f900: 6c74 2829 0d0a 0d0a 2020 2020 2020 2020  lt()....        
+0000f910: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+0000f920: 4974 6572 6174 696e 6720 6f76 6572 2074  Iterating over t
+0000f930: 7261 636b 7320 7b6c 656e 2873 656c 662e  racks {len(self.
+0000f940: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+0000f950: 6473 297d 2729 2020 0d0a 2020 2020 2020  ds)}')  ..      
+0000f960: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000f970: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+0000f980: 2020 2020 2020 2020 2020 6675 7475 7265            future
+0000f990: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000f9a0: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
+0000f9b0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
+0000f9c0: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
+0000f9d0: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
+0000f9e0: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
+0000f9f0: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
+0000fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000fa20: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
+0000fa30: 636b 2069 6e20 7365 6c66 2e74 7261 636b  ck in self.track
+0000fa40: 732e 6669 6e64 616c 6c28 2754 7261 636b  s.findall('Track
+0000fa50: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
 0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa70: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000faa0: 2020 2020 206c 656e 2873 656c 662e 6669       len(self.fi
-0000fab0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-0000fac0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fae0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fb10: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000fb20: 2e73 686f 7728 290d 0a0d 0a0d 0a20 2020  .show()......   
-0000fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb40: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
-0000fb50: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
-0000fb60: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
-0000fb70: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
-0000fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb90: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000fba0: 756e 7420 3d20 7365 6c66 2e63 6f75 6e74  unt = self.count
-0000fbb0: 202b 2031 0d0a 2020 2020 2020 2020 2020   + 1..          
-0000fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbd0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000fbe0: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
-0000fbf0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-0000fc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc20: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000fc30: 735f 6261 722e 7661 6c75 6520 3d20 7365  s_bar.value = se
-0000fc40: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
-0000fc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc60: 2020 2020 2020 2020 2020 2020 2020 722e                r.
-0000fc70: 7265 7375 6c74 2829 0d0a 2020 2020 2020  result()..      
-0000fc80: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000fc90: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
-0000fca0: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
-0000fcb0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000fcc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fcd0: 5f63 7265 6174 655f 7365 636f 6e64 5f63  _create_second_c
-0000fce0: 6861 6e6e 656c 5f78 6d6c 2829 0d0a 2020  hannel_xml()..  
-0000fcf0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000fd00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fd10: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
-0000fd20: 656c 662e 6772 6170 685f 7370 6c69 742e  elf.graph_split.
-0000fd30: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd50: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd70: 2020 2064 6175 6768 7465 725f 7472 6163     daughter_trac
-0000fd80: 6b5f 6964 203d 2020 696e 7428 666c 6f61  k_id =  int(floa
-0000fd90: 7428 7374 7228 7365 6c66 2e75 6e69 7175  t(str(self.uniqu
-0000fda0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000fdb0: 735b 696e 7428 666c 6f61 7428 6b29 295d  s[int(float(k))]
-0000fdc0: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
-0000fdd0: 6579 5d29 2929 0d0a 2020 2020 2020 2020  ey])))..        
-0000fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdf0: 2020 2020 7061 7265 6e74 5f74 7261 636b      parent_track
-0000fe00: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
-0000fe10: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
-0000fe20: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000fe30: 696e 7428 666c 6f61 7428 7629 295d 5b73  int(float(v))][s
-0000fe40: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
-0000fe50: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
+0000fa70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000fa80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000fa90: 7261 636b 5f69 6420 3d20 696e 7428 7472  rack_id = int(tr
+0000faa0: 6163 6b2e 6765 7428 7365 6c66 2e74 7261  ack.get(self.tra
+0000fab0: 636b 6964 5f6b 6579 2929 0d0a 2020 2020  ckid_key))..    
+0000fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fad0: 2020 2020 2020 2020 6966 2074 7261 636b          if track
+0000fae0: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
+0000faf0: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
+0000fb00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb20: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
+0000fb30: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
+0000fb40: 7428 7365 6c66 2e5f 7472 6163 6b5f 636f  t(self._track_co
+0000fb50: 6d70 7574 6572 2c20 7472 6163 6b2c 2074  mputer, track, t
+0000fb60: 7261 636b 5f69 6429 290d 0a20 2020 2020  rack_id))..     
+0000fb70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000fb80: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000fb90: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000fba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbc0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbe0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000fbf0: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+0000fc00: 203d 2022 436f 6c6c 6563 7469 6e67 2054   = "Collecting T
+0000fc10: 7261 636b 7322 0d0a 2020 2020 2020 2020  racks"..        
+0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fc40: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
+0000fc50: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
+0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc80: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fca0: 2020 2020 2020 2020 2020 2020 206c 656e               len
+0000fcb0: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
+0000fcc0: 7261 636b 5f69 6473 292c 0d0a 2020 2020  rack_ids),..    
+0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcf0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd10: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000fd20: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
+0000fd30: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+0000fd40: 2020 2020 2020 2020 2066 6f72 2072 2069           for r i
+0000fd50: 6e20 636f 6e63 7572 7265 6e74 2e66 7574  n concurrent.fut
+0000fd60: 7572 6573 2e61 735f 636f 6d70 6c65 7465  ures.as_complete
+0000fd70: 6428 6675 7475 7265 7329 3a0d 0a20 2020  d(futures):..   
+0000fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fda0: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
+0000fdb0: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
+0000fdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fde0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000fdf0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000fe00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fe30: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
+0000fe40: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
+0000fe50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe70: 2020 7365 6c66 2e67 7261 7068 5f74 7261    self.graph_tra
-0000fe80: 636b 735b 6461 7567 6874 6572 5f74 7261  cks[daughter_tra
-0000fe90: 636b 5f69 645d 203d 2070 6172 656e 745f  ck_id] = parent_
-0000fea0: 7472 6163 6b5f 6964 0d0a 2020 2020 2020  track_id..      
-0000feb0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000fec0: 6765 745f 6174 7472 6962 7574 6573 2829  get_attributes()
-0000fed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fee0: 2020 6966 2073 656c 662e 636c 7573 7465    if self.cluste
-0000fef0: 725f 6d6f 6465 6c20 616e 6420 7365 6c66  r_model and self
-0000ff00: 2e73 6567 5f69 6d61 6765 2069 7320 6e6f  .seg_image is no
-0000ff10: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff30: 7365 6c66 2e5f 6173 7369 676e 5f63 6c75  self._assign_clu
-0000ff40: 7374 6572 5f63 6c61 7373 2829 0d0a 2020  ster_class()..  
-0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff60: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
-0000ff70: 655f 6d61 7374 6572 5f78 6d6c 2829 0d0a  e_master_xml()..
-0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff90: 7365 6c66 2e63 6f75 6e74 203d 2030 200d  self.count = 0 .
-0000ffa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ffb0: 2066 6f72 2074 7261 636b 5f69 6420 696e   for track_id in
-0000ffc0: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
-0000ffd0: 7261 636b 5f69 6473 3a0d 0a20 2020 2020  rack_ids:..     
+0000fe70: 2020 2020 2020 722e 7265 7375 6c74 2829        r.result()
+0000fe80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fe90: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
+0000fea0: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
+0000feb0: 6f74 204e 6f6e 653a 2020 0d0a 2020 2020  ot None:  ..    
+0000fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fed0: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
+0000fee0: 7365 636f 6e64 5f63 6861 6e6e 656c 5f78  second_channel_x
+0000fef0: 6d6c 2829 0d0a 2020 2020 2020 2020 2020  ml()..          
+0000ff00: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+0000ff10: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
+0000ff20: 2c76 2920 696e 2073 656c 662e 6772 6170  ,v) in self.grap
+0000ff30: 685f 7370 6c69 742e 6974 656d 7328 293a  h_split.items():
+0000ff40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ff50: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff70: 2020 2020 2020 2020 2020 2064 6175 6768             daugh
+0000ff80: 7465 725f 7472 6163 6b5f 6964 203d 2020  ter_track_id =  
+0000ff90: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
+0000ffa0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+0000ffb0: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
+0000ffc0: 6f61 7428 6b29 295d 5b73 656c 662e 756e  oat(k))][self.un
+0000ffd0: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
 0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fff0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010000: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-00010010: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-00010020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010040: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010050: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
-00010060: 6c20 3d20 224a 7573 7420 6f6e 6520 6d6f  l = "Just one mo
-00010070: 7265 2074 6869 6e67 220d 0a20 2020 2020  re thing"..     
-00010080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100a0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-000100b0: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
-000100c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100f0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010120: 2020 2020 6c65 6e28 7365 6c66 2e66 696c      len(self.fil
-00010130: 7465 7265 645f 7472 6163 6b5f 6964 7329  tered_track_ids)
-00010140: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010160: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00010170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010190: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000101a0: 726f 6772 6573 735f 6261 722e 7368 6f77  rogress_bar.show
-000101b0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000101e0: 2e63 6f75 6e74 203d 2073 656c 662e 636f  .count = self.co
-000101f0: 756e 7420 2b20 310d 0a20 2020 2020 2020  unt + 1..       
-00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010220: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00010230: 6172 2e76 616c 7565 203d 2073 656c 662e  ar.value = self.
-00010240: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010270: 5f66 696e 616c 5f74 7261 636b 7328 7472  _final_tracks(tr
-00010280: 6163 6b5f 6964 2920 0d0a 0d0a 2020 2020  ack_id) ....    
-00010290: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000102a0: 656c 662e 666f 7572 6965 723a 0d0a 2020  elf.fourier:..  
-000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102c0: 2070 7269 6e74 2827 636f 6d70 7574 696e   print('computin
-000102d0: 6720 466f 7572 6965 7227 290d 0a20 2020  g Fourier')..   
+0000fff0: 2020 2020 2020 2020 2020 2020 7061 7265              pare
+00010000: 6e74 5f74 7261 636b 5f69 6420 3d20 696e  nt_track_id = in
+00010010: 7428 666c 6f61 7428 7374 7228 7365 6c66  t(float(str(self
+00010020: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00010030: 7065 7274 6965 735b 696e 7428 666c 6f61  perties[int(floa
+00010040: 7428 7629 295d 5b73 656c 662e 756e 6971  t(v))][self.uniq
+00010050: 7565 6964 5f6b 6579 5d29 2929 0d0a 2020  ueid_key])))..  
+00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010070: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00010080: 7261 7068 5f74 7261 636b 735b 6461 7567  raph_tracks[daug
+00010090: 6874 6572 5f74 7261 636b 5f69 645d 203d  hter_track_id] =
+000100a0: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
+000100b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000100c0: 2020 7365 6c66 2e5f 6765 745f 6174 7472    self._get_attr
+000100d0: 6962 7574 6573 2829 0d0a 2020 2020 2020  ibutes()..      
+000100e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000100f0: 662e 636c 7573 7465 725f 6d6f 6465 6c20  f.cluster_model 
+00010100: 616e 6420 7365 6c66 2e73 6567 5f69 6d61  and self.seg_ima
+00010110: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
+00010120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010130: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
+00010140: 7369 676e 5f63 6c75 7374 6572 5f63 6c61  sign_cluster_cla
+00010150: 7373 2829 0d0a 2020 2020 2020 2020 2020  ss()..          
+00010160: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010170: 662e 5f63 7265 6174 655f 6d61 7374 6572  f._create_master
+00010180: 5f78 6d6c 2829 0d0a 2020 2020 2020 2020  _xml()..        
+00010190: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
+000101a0: 6e74 203d 2030 200d 0a20 2020 2020 2020  nt = 0 ..       
+000101b0: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
+000101c0: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
+000101d0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+000101e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010200: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00010210: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+00010220: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010250: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+00010260: 6261 722e 6c61 6265 6c20 3d20 224a 7573  bar.label = "Jus
+00010270: 7420 6f6e 6520 6d6f 7265 2074 6869 6e67  t one more thing
+00010280: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000102b0: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
+000102c0: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
+000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102f0: 7365 6c66 2e5f 636f 6d70 7574 655f 7068  self._compute_ph
-00010300: 656e 6f74 7970 6573 2829 2020 2020 2020  enotypes()      
+000102f0: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
+00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010320: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00010330: 2020 2020 7365 6c66 2e5f 7465 6d70 6f72      self._tempor
-00010340: 616c 5f70 6c6f 7473 5f74 7261 636b 6d61  al_plots_trackma
-00010350: 7465 2829 0d0a 2020 2020 2020 2020 2020  te()..          
-00010360: 2020 2020 2020 0d0a 0d0a 2020 2020 6465        ....    de
-00010370: 6620 5f63 7265 6174 655f 6d61 7374 6572  f _create_master
-00010380: 5f78 6d6c 2873 656c 6629 3a0d 0a20 2020  _xml(self):..   
-00010390: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000103a0: 2020 0d0a 2020 2020 2020 2020 2020 2066    ..           f
-000103b0: 6f72 2053 706f 746f 626a 6563 7420 696e  or Spotobject in
-000103c0: 2073 656c 662e 6d61 7374 6572 5f78 6d6c   self.master_xml
-000103d0: 5f72 6f6f 742e 6974 6572 2827 5370 6f74  _root.iter('Spot
-000103e0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-000103f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010400: 2020 2020 2063 656c 6c5f 6964 203d 2069       cell_id = i
-00010410: 6e74 2853 706f 746f 626a 6563 742e 6765  nt(Spotobject.ge
-00010420: 7428 7365 6c66 2e73 706f 7469 645f 6b65  t(self.spotid_ke
-00010430: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 2020 2020 2069 6620 6365 6c6c 5f69 6420       if cell_id 
-00010460: 696e 2073 656c 662e 756e 6971 7565 5f73  in self.unique_s
-00010470: 706f 745f 7072 6f70 6572 7469 6573 2e6b  pot_properties.k
-00010480: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000104b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-000104e0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000104f0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-00010500: 6c5f 6964 5d2e 6b65 7973 2829 3a0d 0a0d  l_id].keys():...
-00010510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010530: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-00010540: 6f62 6a65 6374 2e73 6574 286b 2c20 7374  object.set(k, st
-00010550: 7228 7365 6c66 2e75 6e69 7175 655f 7370  r(self.unique_sp
-00010560: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-00010570: 6c6c 5f69 645d 5b6b 5d29 2920 2020 0d0a  ll_id][k]))   ..
-00010580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-000105b0: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
-000105c0: 6572 5f78 6d6c 5f74 7265 652e 7772 6974  er_xml_tree.writ
-000105d0: 6528 6f73 2e70 6174 682e 6a6f 696e 2873  e(os.path.join(s
-000105e0: 656c 662e 6d61 7374 6572 5f78 6d6c 5f70  elf.master_xml_p
-000105f0: 6174 682c 2073 656c 662e 6d61 7374 6572  ath, self.master
-00010600: 5f78 6d6c 5f6e 616d 6529 290d 0a20 2020  _xml_name))..   
-00010610: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010640: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010660: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00010670: 2020 6465 6620 5f61 7373 6967 6e5f 636c    def _assign_cl
-00010680: 7573 7465 725f 636c 6173 7328 7365 6c66  uster_class(self
-00010690: 293a 0d0a 2020 2020 2020 2020 2020 200d  ):..           .
-000106a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000106b0: 2020 2020 2073 656c 662e 6178 6573 203d       self.axes =
-000106c0: 2073 656c 662e 6178 6573 2e72 6570 6c61   self.axes.repla
-000106d0: 6365 2822 5422 2c20 2222 290d 0a20 2020  ce("T", "")..   
-000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010700: 2020 2020 2020 2066 6f72 2063 6f75 6e74         for count
-00010710: 2c20 7469 6d65 5f6b 6579 2069 6e20 656e  , time_key in en
-00010720: 756d 6572 6174 6528 7365 6c66 2e5f 7469  umerate(self._ti
-00010730: 6d65 645f 6365 6e74 726f 6964 2e6b 6579  med_centroid.key
-00010740: 7328 2929 3a0d 0a20 2020 2020 2020 2020  s()):..         
-00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010760: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00010770: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00010780: 7265 652c 2073 706f 745f 6365 6e74 726f  ree, spot_centro
-00010790: 6964 7320 3d20 7365 6c66 2e5f 7469 6d65  ids = self._time
-000107a0: 645f 6365 6e74 726f 6964 5b74 696d 655f  d_centroid[time_
-000107b0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
-000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107d0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-000107e0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-000107f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010810: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-00010820: 735f 6261 722e 6c61 6265 6c20 3d20 2243  s_bar.label = "C
-00010830: 6f6d 7075 7469 6e67 2063 6c75 7374 6572  omputing cluster
-00010840: 696e 6720 636c 6173 7365 7322 0d0a 2020  ing classes"..  
+00010320: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+00010330: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+00010340: 6163 6b5f 6964 7329 2c0d 0a20 2020 2020  ack_ids),..     
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010370: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103a0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+000103b0: 6261 722e 7368 6f77 2829 0d0a 2020 2020  bar.show()..    
+000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103e0: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+000103f0: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
+00010400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010420: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00010430: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+00010440: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
+00010450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010470: 2020 2073 656c 662e 5f66 696e 616c 5f74     self._final_t
+00010480: 7261 636b 7328 7472 6163 6b5f 6964 2920  racks(track_id) 
+00010490: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000104a0: 2020 2020 6966 2073 656c 662e 666f 7572      if self.four
+000104b0: 6965 723a 0d0a 2020 2020 2020 2020 2020  ier:..          
+000104c0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+000104d0: 636f 6d70 7574 696e 6720 466f 7572 6965  computing Fourie
+000104e0: 7227 290d 0a20 2020 2020 2020 2020 2020  r')..           
+000104f0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+00010500: 6d70 7574 655f 7068 656e 6f74 7970 6573  mpute_phenotypes
+00010510: 2829 2020 2020 2020 2020 2020 2020 2020  ()              
+00010520: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00010530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010540: 2e5f 7465 6d70 6f72 616c 5f70 6c6f 7473  ._temporal_plots
+00010550: 5f74 7261 636b 6d61 7465 2829 0d0a 2020  _trackmate()..  
+00010560: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00010570: 0d0a 2020 2020 6465 6620 5f63 7265 6174  ..    def _creat
+00010580: 655f 6d61 7374 6572 5f78 6d6c 2873 656c  e_master_xml(sel
+00010590: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+000105a0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000105b0: 2020 2020 2020 2066 6f72 2053 706f 746f         for Spoto
+000105c0: 626a 6563 7420 696e 2073 656c 662e 6d61  bject in self.ma
+000105d0: 7374 6572 5f78 6d6c 5f72 6f6f 742e 6974  ster_xml_root.it
+000105e0: 6572 2827 5370 6f74 2729 3a0d 0a20 2020  er('Spot'):..   
+000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010600: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+00010610: 6c5f 6964 203d 2069 6e74 2853 706f 746f  l_id = int(Spoto
+00010620: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+00010630: 706f 7469 645f 6b65 7929 290d 0a20 2020  potid_key))..   
+00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010650: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010660: 6365 6c6c 5f69 6420 696e 2073 656c 662e  cell_id in self.
+00010670: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00010680: 6572 7469 6573 2e6b 6579 7328 293a 0d0a  erties.keys():..
+00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000106c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106e0: 666f 7220 6b20 696e 2073 656c 662e 756e  for k in self.un
+000106f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00010700: 7469 6573 5b63 656c 6c5f 6964 5d2e 6b65  ties[cell_id].ke
+00010710: 7973 2829 3a0d 0a0d 0a20 2020 2020 2020  ys():....       
+00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010740: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+00010750: 6574 286b 2c20 7374 7228 7365 6c66 2e75  et(k, str(self.u
+00010760: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00010770: 7274 6965 735b 6365 6c6c 5f69 645d 5b6b  rties[cell_id][k
+00010780: 5d29 2920 2020 0d0a 0d0a 2020 2020 2020  ]))   ....      
+00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2073  ....           s
+000107c0: 656c 662e 6d61 7374 6572 5f78 6d6c 5f74  elf.master_xml_t
+000107d0: 7265 652e 7772 6974 6528 6f73 2e70 6174  ree.write(os.pat
+000107e0: 682e 6a6f 696e 2873 656c 662e 6d61 7374  h.join(self.mast
+000107f0: 6572 5f78 6d6c 5f70 6174 682c 2073 656c  er_xml_path, sel
+00010800: 662e 6d61 7374 6572 5f78 6d6c 5f6e 616d  f.master_xml_nam
+00010810: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+00010820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010840: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010860: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010870: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-00010880: 7261 6e67 6520 3d20 280d 0a20 2020 2020  range = (..     
-00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108c0: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010900: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00010910: 656e 2873 656c 662e 5f74 696d 6564 5f63  en(self._timed_c
-00010920: 656e 7472 6f69 642e 6b65 7973 2829 2920  entroid.keys()) 
-00010930: 2b20 312c 0d0a 2020 2020 2020 2020 2020  + 1,..          
-00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010870: 2020 0d0a 0d0a 2020 2020 6465 6620 5f61    ....    def _a
+00010880: 7373 6967 6e5f 636c 7573 7465 725f 636c  ssign_cluster_cl
+00010890: 6173 7328 7365 6c66 293a 0d0a 2020 2020  ass(self):..    
+000108a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000108b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000108c0: 662e 6178 6573 203d 2073 656c 662e 6178  f.axes = self.ax
+000108d0: 6573 2e72 6570 6c61 6365 2822 5422 2c20  es.replace("T", 
+000108e0: 2222 290d 0a20 2020 2020 2020 2020 2020  "")..           
+000108f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00010900: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010910: 6f72 2063 6f75 6e74 2c20 7469 6d65 5f6b  or count, time_k
+00010920: 6579 2069 6e20 656e 756d 6572 6174 6528  ey in enumerate(
+00010930: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
+00010940: 726f 6964 2e6b 6579 7328 2929 3a0d 0a20  roid.keys()):.. 
 00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010970: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-000109a0: 7373 5f62 6172 2e76 616c 7565 203d 2020  ss_bar.value =  
-000109b0: 636f 756e 7420 0d0a 2020 2020 2020 2020  count ..        
+00010960: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010980: 2020 2020 2020 2074 7265 652c 2073 706f         tree, spo
+00010990: 745f 6365 6e74 726f 6964 7320 3d20 7365  t_centroids = se
+000109a0: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
+000109b0: 6964 5b74 696d 655f 6b65 795d 0d0a 2020  id[time_key]..  
 000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109d0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-000109e0: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
-000109f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00010a00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00010a10: 6c75 7374 6572 5f65 7661 6c20 3d20 436c  luster_eval = Cl
-00010a20: 7573 7465 7269 6e67 2873 656c 662e 7365  ustering(self.se
-00010a30: 675f 696d 6167 655b 696e 7428 7469 6d65  g_image[int(time
-00010a40: 5f6b 6579 292c 3a5d 2c20 2073 656c 662e  _key),:],  self.
-00010a50: 6178 6573 2c20 7365 6c66 2e6e 756d 5f70  axes, self.num_p
-00010a60: 6f69 6e74 732c 2073 656c 662e 636c 7573  oints, self.clus
-00010a70: 7465 725f 6d6f 6465 6c2c 206b 6579 203d  ter_model, key =
-00010a80: 2074 696d 655f 6b65 792c 2070 726f 6772   time_key, progr
-00010a90: 6573 735f 6261 723d 7365 6c66 2e70 726f  ess_bar=self.pro
-00010aa0: 6772 6573 735f 6261 722c 2062 6174 6368  gress_bar, batch
-00010ab0: 5f73 697a 6520 3d20 7365 6c66 2e62 6174  _size = self.bat
-00010ac0: 6368 5f73 697a 6529 2020 2020 2020 200d  ch_size)       .
-00010ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ae0: 2020 2020 2020 2020 2020 2020 636c 7573              clus
-00010af0: 7465 725f 6576 616c 2e5f 6372 6561 7465  ter_eval._create
-00010b00: 5f63 6c75 7374 6572 5f6c 6162 656c 7328  _cluster_labels(
-00010b10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010b20: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00010b30: 6d65 645f 636c 7573 7465 725f 6c61 6265  med_cluster_labe
-00010b40: 6c20 3d20 636c 7573 7465 725f 6576 616c  l = cluster_eval
-00010b50: 2e74 696d 6564 5f63 6c75 7374 6572 5f6c  .timed_cluster_l
-00010b60: 6162 656c 200d 0a20 2020 2020 2020 2020  abel ..         
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 2020 6f75 7470 7574 5f6c 6162 656c 732c    output_labels,
-00010b90: 206f 7574 7075 745f 636c 7573 7465 725f   output_cluster_
-00010ba0: 7363 6f72 652c 206f 7574 7075 745f 636c  score, output_cl
-00010bb0: 7573 7465 725f 636c 6173 732c 206f 7574  uster_class, out
-00010bc0: 7075 745f 636c 7573 7465 725f 6365 6e74  put_cluster_cent
-00010bd0: 726f 6964 2c20 6f75 7470 7574 5f63 6c6f  roid, output_clo
-00010be0: 7564 5f65 6363 656e 7472 6963 6974 792c  ud_eccentricity,
-00010bf0: 206f 7574 7075 745f 6c61 7267 6573 745f   output_largest_
-00010c00: 6569 6765 6e76 6563 746f 722c 206f 7574  eigenvector, out
-00010c10: 7075 745f 6c61 7267 6573 745f 6569 6765  put_largest_eige
-00010c20: 6e76 616c 7565 2c20 6f75 7470 7574 5f63  nvalue, output_c
-00010c30: 6c6f 7564 5f73 7572 6661 6365 5f61 7265  loud_surface_are
-00010c40: 6120 3d20 7469 6d65 645f 636c 7573 7465  a = timed_cluste
-00010c50: 725f 6c61 6265 6c5b 7469 6d65 5f6b 6579  r_label[time_key
-00010c60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00010c70: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00010c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c90: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00010ca0: 2069 6e20 7261 6e67 6528 6c65 6e28 6f75   in range(len(ou
-00010cb0: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
-00010cc0: 7472 6f69 6429 293a 0d0a 2020 2020 2020  troid)):..      
-00010cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ce0: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00010cf0: 6e74 726f 6964 203d 206f 7574 7075 745f  ntroid = output_
-00010d00: 636c 7573 7465 725f 6365 6e74 726f 6964  cluster_centroid
-00010d10: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
+000109d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000109e0: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
+000109f0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00010a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010a20: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
+00010a30: 6265 6c20 3d20 2243 6f6d 7075 7469 6e67  bel = "Computing
+00010a40: 2063 6c75 7374 6572 696e 6720 636c 6173   clustering clas
+00010a50: 7365 7322 0d0a 2020 2020 2020 2020 2020  ses"..          
+00010a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a70: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+00010a80: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
+00010a90: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00010aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ad0: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
+00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b10: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
+00010b20: 5f74 696d 6564 5f63 656e 7472 6f69 642e  _timed_centroid.
+00010b30: 6b65 7973 2829 2920 2b20 312c 0d0a 2020  keys()) + 1,..  
+00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b70: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00010b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010ba0: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
+00010bb0: 616c 7565 203d 2020 636f 756e 7420 0d0a  alue =  count ..
+00010bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010be0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00010bf0: 722e 7368 6f77 2829 0d0a 0d0a 2020 2020  r.show()....    
+00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c10: 2020 2020 2020 2063 6c75 7374 6572 5f65         cluster_e
+00010c20: 7661 6c20 3d20 436c 7573 7465 7269 6e67  val = Clustering
+00010c30: 2873 656c 662e 7365 675f 696d 6167 655b  (self.seg_image[
+00010c40: 696e 7428 7469 6d65 5f6b 6579 292c 3a5d  int(time_key),:]
+00010c50: 2c20 2073 656c 662e 6178 6573 2c20 7365  ,  self.axes, se
+00010c60: 6c66 2e6e 756d 5f70 6f69 6e74 732c 2073  lf.num_points, s
+00010c70: 656c 662e 636c 7573 7465 725f 6d6f 6465  elf.cluster_mode
+00010c80: 6c2c 206b 6579 203d 2074 696d 655f 6b65  l, key = time_ke
+00010c90: 792c 2070 726f 6772 6573 735f 6261 723d  y, progress_bar=
+00010ca0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00010cb0: 722c 2062 6174 6368 5f73 697a 6520 3d20  r, batch_size = 
+00010cc0: 7365 6c66 2e62 6174 6368 5f73 697a 6529  self.batch_size)
+00010cd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cf0: 2020 2020 636c 7573 7465 725f 6576 616c      cluster_eval
+00010d00: 2e5f 6372 6561 7465 5f63 6c75 7374 6572  ._create_cluster
+00010d10: 5f6c 6162 656c 7328 290d 0a20 2020 2020  _labels()..     
 00010d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d30: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
-00010d40: 5f63 6c61 7373 203d 206f 7574 7075 745f  _class = output_
-00010d50: 636c 7573 7465 725f 636c 6173 735b 695d  cluster_class[i]
-00010d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010d30: 2020 2020 2020 7469 6d65 645f 636c 7573        timed_clus
+00010d40: 7465 725f 6c61 6265 6c20 3d20 636c 7573  ter_label = clus
+00010d50: 7465 725f 6576 616c 2e74 696d 6564 5f63  ter_eval.timed_c
+00010d60: 6c75 7374 6572 5f6c 6162 656c 200d 0a20  luster_label .. 
 00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d80: 2020 2020 2020 636c 7573 7465 725f 7363        cluster_sc
-00010d90: 6f72 6520 3d20 6f75 7470 7574 5f63 6c75  ore = output_clu
-00010da0: 7374 6572 5f73 636f 7265 5b69 5d0d 0a20  ster_score[i].. 
-00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dd0: 2020 2071 7561 6c69 7479 203d 206f 7574     quality = out
-00010de0: 7075 745f 6c61 7267 6573 745f 6569 6765  put_largest_eige
-00010df0: 6e76 616c 7565 5b69 5d0d 0a20 2020 2020  nvalue[i]..     
-00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00010e20: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00010e30: 5f66 6972 7374 797a 203d 206f 7574 7075  _firstyz = outpu
-00010e40: 745f 636c 6f75 645f 6563 6365 6e74 7269  t_cloud_eccentri
-00010e50: 6369 7479 5b69 5d0d 0a20 2020 2020 2020  city[i]..       
-00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e70: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00010e80: 6c5f 6178 6973 203d 206f 7574 7075 745f  l_axis = output_
-00010e90: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
-00010ea0: 746f 725b 695d 0d0a 2020 2020 2020 2020  tor[i]..        
-00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ec0: 2020 2020 2020 2020 2020 2020 7375 7266              surf
-00010ed0: 6163 655f 6172 6561 203d 206f 7574 7075  ace_area = outpu
-00010ee0: 745f 636c 6f75 645f 7375 7266 6163 655f  t_cloud_surface_
-00010ef0: 6172 6561 5b69 5d0d 0a20 2020 2020 2020  area[i]..       
-00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f10: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00010f20: 742c 2069 6e64 6578 203d 2074 7265 652e  t, index = tree.
-00010f30: 7175 6572 7928 6365 6e74 726f 6964 290d  query(centroid).
-00010f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f60: 2020 2020 2069 6620 6469 7374 203c 2071       if dist < q
-00010f70: 7561 6c69 7479 3a0d 0a20 2020 2020 2020  uality:..       
-00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fa0: 2020 2020 2063 6c6f 7365 7374 5f63 656e       closest_cen
-00010fb0: 7472 6f69 6420 3d20 7370 6f74 5f63 656e  troid = spot_cen
-00010fc0: 7472 6f69 6473 5b69 6e64 6578 5d0d 0a20  troids[index].. 
-00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ff0: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
-00011000: 5f73 706f 745f 6365 6e74 726f 6964 203d  _spot_centroid =
-00011010: 2028 696e 7428 7469 6d65 5f6b 6579 292c   (int(time_key),
-00011020: 636c 6f73 6573 745f 6365 6e74 726f 6964  closest_centroid
-00011030: 5b30 5d2c 2063 6c6f 7365 7374 5f63 656e  [0], closest_cen
-00011040: 7472 6f69 645b 315d 2c20 636c 6f73 6573  troid[1], closes
-00011050: 745f 6365 6e74 726f 6964 5b32 5d29 0d0a  t_centroid[2])..
-00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d80: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00010d90: 5f6c 6162 656c 732c 206f 7574 7075 745f  _labels, output_
+00010da0: 636c 7573 7465 725f 7363 6f72 652c 206f  cluster_score, o
+00010db0: 7574 7075 745f 636c 7573 7465 725f 636c  utput_cluster_cl
+00010dc0: 6173 732c 206f 7574 7075 745f 636c 7573  ass, output_clus
+00010dd0: 7465 725f 6365 6e74 726f 6964 2c20 6f75  ter_centroid, ou
+00010de0: 7470 7574 5f63 6c6f 7564 5f65 6363 656e  tput_cloud_eccen
+00010df0: 7472 6963 6974 792c 206f 7574 7075 745f  tricity, output_
+00010e00: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
+00010e10: 746f 722c 206f 7574 7075 745f 6c61 7267  tor, output_larg
+00010e20: 6573 745f 6569 6765 6e76 616c 7565 2c20  est_eigenvalue, 
+00010e30: 6f75 7470 7574 5f63 6c6f 7564 5f73 7572  output_cloud_sur
+00010e40: 6661 6365 5f61 7265 6120 3d20 7469 6d65  face_area = time
+00010e50: 645f 636c 7573 7465 725f 6c61 6265 6c5b  d_cluster_label[
+00010e60: 7469 6d65 5f6b 6579 5d0d 0a20 2020 2020  time_key]..     
+00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e80: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ea0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00010eb0: 6528 6c65 6e28 6f75 7470 7574 5f63 6c75  e(len(output_clu
+00010ec0: 7374 6572 5f63 656e 7472 6f69 6429 293a  ster_centroid)):
+00010ed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ef0: 2020 2020 2020 6365 6e74 726f 6964 203d        centroid =
+00010f00: 206f 7574 7075 745f 636c 7573 7465 725f   output_cluster_
+00010f10: 6365 6e74 726f 6964 5b69 5d0d 0a20 2020  centroid[i]..   
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f40: 2063 6c75 7374 6572 5f63 6c61 7373 203d   cluster_class =
+00010f50: 206f 7574 7075 745f 636c 7573 7465 725f   output_cluster_
+00010f60: 636c 6173 735b 695d 0d0a 2020 2020 2020  class[i]..      
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00010f90: 7573 7465 725f 7363 6f72 6520 3d20 6f75  uster_score = ou
+00010fa0: 7470 7574 5f63 6c75 7374 6572 5f73 636f  tput_cluster_sco
+00010fb0: 7265 5b69 5d0d 0a20 2020 2020 2020 2020  re[i]..         
+00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fd0: 2020 2020 2020 2020 2020 2071 7561 6c69             quali
+00010fe0: 7479 203d 206f 7574 7075 745f 6c61 7267  ty = output_larg
+00010ff0: 6573 745f 6569 6765 6e76 616c 7565 5b69  est_eigenvalue[i
+00011000: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011020: 2020 2020 2020 2065 6363 656e 7472 6963         eccentric
+00011030: 6974 795f 636f 6d70 5f66 6972 7374 797a  ity_comp_firstyz
+00011040: 203d 206f 7574 7075 745f 636c 6f75 645f   = output_cloud_
+00011050: 6563 6365 6e74 7269 6369 7479 5b69 5d0d  eccentricity[i].
+00011060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011080: 2020 2020 2020 2020 2020 2020 636c 6f73              clos
-00011090: 6573 745f 6365 6c6c 5f69 6420 3d20 7365  est_cell_id = se
-000110a0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f63  lf.unique_spot_c
-000110b0: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
-000110c0: 6f74 5f63 656e 7472 6f69 645d 0d0a 2020  ot_centroid]..  
-000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 2020 2020 2020 2020 6d61 736b 5f76            mask_v
-00011100: 6563 746f 7220 3d20 5b20 666c 6f61 7428  ector = [ float(
-00011110: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00011120: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00011130: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00011140: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
-00011150: 6f69 645f 785f 6b65 795d 292c 2066 6c6f  oid_x_key]), flo
-00011160: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00011170: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00011180: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-00011190: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
-000111a0: 6e74 726f 6964 5f79 5f6b 6579 5d29 2c20  ntroid_y_key]), 
-000111b0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-000111c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000111d0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-000111e0: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
-000111f0: 6b63 656e 7472 6f69 645f 7a5f 6b65 795d  kcentroid_z_key]
-00011200: 2920 5d0d 0a20 2020 2020 2020 2020 2020  ) ]..           
-00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011230: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
-00011240: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
-00011250: 2863 656c 6c5f 6178 6973 2c20 6d61 736b  (cell_axis, mask
-00011260: 5f76 6563 746f 7229 0d0a 2020 2020 2020  _vector)..      
+00011080: 2020 2020 2063 656c 6c5f 6178 6973 203d       cell_axis =
+00011090: 206f 7574 7075 745f 6c61 7267 6573 745f   output_largest_
+000110a0: 6569 6765 6e76 6563 746f 725b 695d 0d0a  eigenvector[i]..
+000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110d0: 2020 2020 7375 7266 6163 655f 6172 6561      surface_area
+000110e0: 203d 206f 7574 7075 745f 636c 6f75 645f   = output_cloud_
+000110f0: 7375 7266 6163 655f 6172 6561 5b69 5d0d  surface_area[i].
+00011100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 2020 2020 2064 6973 742c 2069 6e64 6578       dist, index
+00011130: 203d 2074 7265 652e 7175 6572 7928 6365   = tree.query(ce
+00011140: 6e74 726f 6964 290d 0a20 2020 2020 2020  ntroid)..       
+00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011160: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011170: 6469 7374 203c 2071 7561 6c69 7479 3a0d  dist < quality:.
+00011180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111a0: 2020 2020 2020 2020 2020 2020 2063 6c6f               clo
+000111b0: 7365 7374 5f63 656e 7472 6f69 6420 3d20  sest_centroid = 
+000111c0: 7370 6f74 5f63 656e 7472 6f69 6473 5b69  spot_centroids[i
+000111d0: 6e64 6578 5d0d 0a20 2020 2020 2020 2020  ndex]..         
+000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011200: 2020 2066 7261 6d65 5f73 706f 745f 6365     frame_spot_ce
+00011210: 6e74 726f 6964 203d 2028 696e 7428 7469  ntroid = (int(ti
+00011220: 6d65 5f6b 6579 292c 636c 6f73 6573 745f  me_key),closest_
+00011230: 6365 6e74 726f 6964 5b30 5d2c 2063 6c6f  centroid[0], clo
+00011240: 7365 7374 5f63 656e 7472 6f69 645b 315d  sest_centroid[1]
+00011250: 2c20 636c 6f73 6573 745f 6365 6e74 726f  , closest_centro
+00011260: 6964 5b32 5d29 0d0a 2020 2020 2020 2020  id[2])..        
 00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011290: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000112d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000112e0: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-000112f0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00011300: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
-00011310: 5f6b 6579 203a 2063 656c 6c5f 6178 6973  _key : cell_axis
-00011320: 5f6d 6173 6b7d 290d 0a20 2020 2020 2020  _mask})..       
-00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011350: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00011360: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011370: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-00011380: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00011390: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-000113a0: 5f6b 6579 203a 2063 6c75 7374 6572 5f63  _key : cluster_c
-000113b0: 6c61 7373 7d29 0d0a 2020 2020 2020 2020  lass})..        
-000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113e0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000113f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00011400: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-00011410: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00011420: 6c66 2e63 6c75 7374 6572 7363 6f72 655f  lf.clusterscore_
-00011430: 6b65 7920 3a20 636c 7573 7465 725f 7363  key : cluster_sc
-00011440: 6f72 657d 290d 0a20 2020 2020 2020 2020  ore})..         
-00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011470: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00011480: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00011490: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-000114a0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000114b0: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
-000114c0: 6f6d 705f 6669 7273 746b 6579 203a 2065  omp_firstkey : e
-000114d0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-000114e0: 5f66 6972 7374 797a 5b30 5d7d 290d 0a20  _firstyz[0]}).. 
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011520: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00011530: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00011540: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
-00011550: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
-00011560: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00011570: 6e64 6b65 7920 3a20 6563 6365 6e74 7269  ndkey : eccentri
-00011580: 6369 7479 5f63 6f6d 705f 6669 7273 7479  city_comp_firsty
-00011590: 7a5b 315d 7d29 0d0a 2020 2020 2020 2020  z[1]})..        
-000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000115d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000115e0: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-000115f0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00011600: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-00011610: 6b65 7920 3a20 7375 7266 6163 655f 6172  key : surface_ar
-00011620: 6561 7d29 0d0a 2020 2020 2020 2020 2020  ea})..          
-00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011650: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00011660: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00011670: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
-00011680: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00011690: 2e71 7561 6c69 7479 5f6b 6579 203a 2071  .quality_key : q
-000116a0: 7561 6c69 7479 7d29 0d0a 2020 2020 2020  uality})..      
-000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116d0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000116e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000116f0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00011700: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00011710: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
-00011720: 3a20 7175 616c 6974 7920 2a20 6d61 7468  : quality * math
-00011730: 2e70 6f77 2873 656c 662e 7a63 616c 6962  .pow(self.zcalib
-00011740: 7261 7469 6f6e 202a 2073 656c 662e 7863  ration * self.xc
-00011750: 616c 6962 7261 7469 6f6e 202a 2073 656c  alibration * sel
-00011760: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
-00011770: 312e 302f 332e 3029 207d 290d 0a0d 0a0d  1.0/3.0) }).....
-00011780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00011290: 2020 2020 636c 6f73 6573 745f 6365 6c6c      closest_cell
+000112a0: 5f69 6420 3d20 7365 6c66 2e75 6e69 7175  _id = self.uniqu
+000112b0: 655f 7370 6f74 5f63 656e 7472 6f69 645b  e_spot_centroid[
+000112c0: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
+000112d0: 6f69 645d 0d0a 2020 2020 2020 2020 2020  oid]..          
+000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011300: 2020 6d61 736b 5f76 6563 746f 7220 3d20    mask_vector = 
+00011310: 5b20 666c 6f61 7428 7365 6c66 2e75 6e69  [ float(self.uni
+00011320: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011330: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00011340: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00011350: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
+00011360: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
+00011370: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00011380: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+00011390: 7374 5f63 656c 6c5f 6964 295d 5b73 656c  st_cell_id)][sel
+000113a0: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
+000113b0: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
+000113c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000113d0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+000113e0: 6f73 6573 745f 6365 6c6c 5f69 6429 5d5b  osest_cell_id)][
+000113f0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+00011400: 645f 7a5f 6b65 795d 2920 5d0d 0a20 2020  d_z_key]) ]..   
+00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011430: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
+00011440: 6973 5f6d 6173 6b20 3d20 616e 6775 6c61  is_mask = angula
+00011450: 725f 6368 616e 6765 2863 656c 6c5f 6178  r_change(cell_ax
+00011460: 6973 2c20 6d61 736b 5f76 6563 746f 7229  is, mask_vector)
+00011470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000114d0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000114e0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+000114f0: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+00011500: 6461 7465 287b 7365 6c66 2e63 656c 6c61  date({self.cella
+00011510: 7869 735f 6d61 736b 5f6b 6579 203a 2063  xis_mask_key : c
+00011520: 656c 6c5f 6178 6973 5f6d 6173 6b7d 290d  ell_axis_mask}).
+00011530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011550: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011560: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00011570: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+00011580: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+00011590: 7064 6174 6528 7b73 656c 662e 636c 7573  pdate({self.clus
+000115a0: 7465 7263 6c61 7373 5f6b 6579 203a 2063  terclass_key : c
+000115b0: 6c75 7374 6572 5f63 6c61 7373 7d29 0d0a  luster_class})..
+000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000115f0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00011600: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00011610: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+00011620: 6461 7465 287b 7365 6c66 2e63 6c75 7374  date({self.clust
+00011630: 6572 7363 6f72 655f 6b65 7920 3a20 636c  erscore_key : cl
+00011640: 7573 7465 725f 7363 6f72 657d 290d 0a20  uster_score}).. 
+00011650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011680: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00011690: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+000116a0: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
+000116b0: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
+000116c0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+000116d0: 746b 6579 203a 2065 6363 656e 7472 6963  tkey : eccentric
+000116e0: 6974 795f 636f 6d70 5f66 6972 7374 797a  ity_comp_firstyz
+000116f0: 5b30 5d7d 290d 0a20 2020 2020 2020 2020  [0]})..         
+00011700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011720: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00011730: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00011740: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
+00011750: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00011760: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+00011770: 6f6d 705f 7365 636f 6e64 6b65 7920 3a20  omp_secondkey : 
+00011780: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00011790: 705f 6669 7273 7479 7a5b 315d 7d29 0d0a  p_firstyz[1]})..
+000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117c0: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
-000117d0: 656c 662e 726f 6f74 5f73 706f 7473 2e69  elf.root_spots.i
-000117e0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011810: 726f 6f74 5f73 706f 7473 5b6b 5d20 3d20  root_spots[k] = 
-00011820: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00011830: 5f70 726f 7065 7274 6965 735b 6b5d 2020  _properties[k]  
-00011840: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00011850: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
-00011860: 6566 205f 636f 6d70 7574 655f 7068 656e  ef _compute_phen
-00011870: 6f74 7970 6573 2873 656c 6629 3a0d 0a0d  otypes(self):...
-00011880: 0a20 2020 2020 2020 2020 2066 6f72 2028  .          for (
-00011890: 6b2c 7629 2069 6e20 7365 6c66 2e75 6e69  k,v) in self.uni
-000118a0: 7175 655f 7472 6163 6b73 2e69 7465 6d73  que_tracks.items
-000118b0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-000118c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000118d0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-000118e0: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
-000118f0: 2020 2020 2074 7261 636b 6c65 745f 7072       tracklet_pr
-00011900: 6f70 6572 7469 6573 203d 2073 656c 662e  operties = self.
-00011910: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
-00011920: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
-00011930: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00011940: 6b73 203d 2073 656c 662e 756e 6971 7565  ks = self.unique
-00011950: 5f74 7261 636b 735b 6b5d 0d0a 2020 2020  _tracks[k]..    
-00011960: 2020 2020 2020 2020 2020 2020 5a20 3d20              Z = 
-00011970: 7472 6163 6b73 5b3a 2c32 5d0d 0a20 2020  tracks[:,2]..   
-00011980: 2020 2020 2020 2020 2020 2020 2059 203d               Y =
-00011990: 2074 7261 636b 735b 3a2c 335d 0d0a 2020   tracks[:,3]..  
-000119a0: 2020 2020 2020 2020 2020 2020 2020 5820                X 
-000119b0: 3d20 7472 6163 6b73 5b3a 2c34 5d0d 0a20  = tracks[:,4].. 
-000119c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000119d0: 696d 6520 3d20 7472 6163 6b6c 6574 5f70  ime = tracklet_p
-000119e0: 726f 7065 7274 6965 735b 3a2c 305d 0d0a  roperties[:,0]..
-000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a00: 756e 6971 7565 5f69 6473 203d 2074 7261  unique_ids = tra
-00011a10: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00011a20: 5b3a 2c31 5d0d 0a20 2020 2020 2020 2020  [:,1]..         
-00011a30: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
-00011a40: 735f 7365 7420 3d20 7365 7428 756e 6971  s_set = set(uniq
-00011a50: 7565 5f69 6473 290d 0a20 2020 2020 2020  ue_ids)..       
-00011a60: 2020 2020 2020 2020 2067 656e 6572 6174           generat
-00011a70: 696f 6e5f 6964 7320 3d20 7472 6163 6b6c  ion_ids = trackl
-00011a80: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00011a90: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
-00011aa0: 2020 2020 7261 6469 7573 203d 2074 7261      radius = tra
-00011ab0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00011ac0: 5b3a 2c33 5d0d 0a20 2020 2020 2020 2020  [:,3]..         
-00011ad0: 2020 2020 2020 2076 6f6c 756d 6520 3d20         volume = 
-00011ae0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00011af0: 6965 735b 3a2c 345d 0d0a 2020 2020 2020  ies[:,4]..      
-00011b00: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
-00011b10: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00011b20: 7420 3d20 7472 6163 6b6c 6574 5f70 726f  t = tracklet_pro
-00011b30: 7065 7274 6965 735b 3a2c 355d 0d0a 2020  perties[:,5]..  
-00011b40: 2020 2020 2020 2020 2020 2020 2020 6563                ec
-00011b50: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00011b60: 7365 636f 6e64 203d 2074 7261 636b 6c65  second = trackle
-00011b70: 745f 7072 6f70 6572 7469 6573 5b3a 2c36  t_properties[:,6
-00011b80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00011b90: 2020 2073 7572 6661 6365 5f61 7265 6120     surface_area 
-00011ba0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00011bb0: 7274 6965 735b 3a2c 375d 0d0a 2020 2020  rties[:,7]..    
-00011bc0: 2020 2020 2020 2020 2020 2020 636c 7573              clus
-00011bd0: 7465 725f 636c 6173 7320 3d20 7472 6163  ter_class = trac
-00011be0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00011bf0: 3a2c 385d 0d0a 2020 2020 2020 2020 2020  :,8]..          
-00011c00: 2020 2020 2020 636c 7573 7465 725f 636c        cluster_cl
-00011c10: 6173 735f 7363 6f72 6520 3d20 7472 6163  ass_score = trac
-00011c20: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00011c30: 3a2c 395d 0d0a 2020 2020 2020 2020 2020  :,9]..          
-00011c40: 2020 2020 2020 696e 7465 6e73 6974 7920        intensity 
-00011c50: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00011c60: 7274 6965 735b 3a2c 3130 5d0d 0a20 2020  rties[:,10]..   
-00011c70: 2020 2020 2020 2020 2020 2020 2073 7065               spe
-00011c80: 6564 203d 2074 7261 636b 6c65 745f 7072  ed = tracklet_pr
-00011c90: 6f70 6572 7469 6573 5b3a 2c31 315d 0d0a  operties[:,11]..
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 6d6f 7469 6f6e 5f61 6e67 6c65 203d 2074  motion_angle = t
-00011cc0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-00011cd0: 6573 5b3a 2c31 325d 0d0a 2020 2020 2020  es[:,12]..      
-00011ce0: 2020 2020 2020 2020 2020 6163 6365 6c65            accele
-00011cf0: 7261 7469 6f6e 203d 2074 7261 636b 6c65  ration = trackle
-00011d00: 745f 7072 6f70 6572 7469 6573 5b3a 2c31  t_properties[:,1
-00011d10: 335d 0d0a 2020 2020 2020 2020 2020 2020  3]..            
-00011d20: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
-00011d30: 6c5f 6d61 736b 203d 2074 7261 636b 6c65  l_mask = trackle
-00011d40: 745f 7072 6f70 6572 7469 6573 5b3a 2c31  t_properties[:,1
-00011d50: 345d 0d0a 2020 2020 2020 2020 2020 2020  4]..            
-00011d60: 2020 2020 7261 6469 616c 5f61 6e67 6c65      radial_angle
-00011d70: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00011d80: 6572 7469 6573 5b3a 2c31 355d 0d0a 2020  erties[:,15]..  
-00011d90: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00011da0: 6c6c 5f61 7869 735f 6d61 736b 203d 2074  ll_axis_mask = t
-00011db0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-00011dc0: 6573 5b3a 2c31 365d 0d0a 0d0a 0d0a 2020  es[:,16]......  
-00011dd0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011df0: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
-00011e00: 7274 6965 735f 7472 6163 6b6c 6574 203d  rties_tracklet =
-00011e10: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00011e20: 2020 2020 2075 6e69 7175 655f 636c 7573       unique_clus
-00011e30: 7465 725f 7072 6f70 6572 7469 6573 5f74  ter_properties_t
-00011e40: 7261 636b 6c65 7420 3d20 7b7d 0d0a 2020  racklet = {}..  
-00011e50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011e60: 6c66 2e75 6e69 7175 655f 6666 745f 7072  lf.unique_fft_pr
-00011e70: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
-00011e80: 645d 203d 207b 7d0d 0a20 2020 2020 2020  d] = {}..       
-00011e90: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00011ea0: 6971 7565 5f63 6c75 7374 6572 5f70 726f  ique_cluster_pro
-00011eb0: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
-00011ec0: 5d20 3d20 7b7d 0d0a 0d0a 2020 2020 2020  ] = {}....      
-00011ed0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00011ee0: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
-00011ef0: 735f 7472 6163 6b6c 6574 203d 207b 7d0d  s_tracklet = {}.
-00011f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011f10: 2075 6e69 7175 655f 6479 6e61 6d69 635f   unique_dynamic_
-00011f20: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00011f30: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
-00011f40: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00011f50: 6e69 7175 655f 7368 6170 655f 7072 6f70  nique_shape_prop
-00011f60: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-00011f70: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00011f80: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00011f90: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
-00011fa0: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
-00011fb0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-00011fc0: 2020 2020 2020 6578 7061 6e64 6564 5f74        expanded_t
-00011fd0: 696d 6520 3d20 6e70 2e7a 6572 6f73 2873  ime = np.zeros(s
-00011fe0: 656c 662e 7465 6e64 202d 2073 656c 662e  elf.tend - self.
-00011ff0: 7473 7461 7274 202b 2031 290d 0a20 2020  tstart + 1)..   
-00012000: 2020 2020 2020 2020 2020 2020 2070 6f69               poi
-00012010: 6e74 5f73 616d 706c 6520 3d20 6578 7061  nt_sample = expa
-00012020: 6e64 6564 5f74 696d 652e 7368 6170 655b  nded_time.shape[
-00012030: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00012040: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00012050: 6765 286c 656e 2865 7870 616e 6465 645f  ge(len(expanded_
-00012060: 7469 6d65 2929 3a0d 0a20 2020 2020 2020  time)):..       
-00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012080: 6578 7061 6e64 6564 5f74 696d 655b 695d  expanded_time[i]
-00012090: 203d 2069 200d 0a20 2020 2020 2020 2020   = i ..         
-000120a0: 2020 2020 2020 2066 6f72 2063 7572 7265         for curre
-000120b0: 6e74 5f75 6e69 7175 655f 6964 2069 6e20  nt_unique_id in 
-000120c0: 756e 6971 7565 5f69 6473 5f73 6574 3a0d  unique_ids_set:.
-000120d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000120e0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000120f0: 2020 2020 2020 2020 2065 7870 616e 6465           expande
-00012100: 645f 696e 7465 6e73 6974 7920 3d20 6e70  d_intensity = np
-00012110: 2e7a 6572 6f73 2873 656c 662e 7465 6e64  .zeros(self.tend
-00012120: 202d 2073 656c 662e 7473 7461 7274 202b   - self.tstart +
-00012130: 2031 290d 0a20 2020 2020 2020 2020 2020   1)..           
-00012140: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00012150: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012170: 2020 6375 7272 656e 745f 7469 6d65 203d    current_time =
-00012180: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012190: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000121a0: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-000121b0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-000121c0: 6e74 5f79 203d 205b 5d0d 0a20 2020 2020  nt_y = []..     
-000121d0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000121e0: 7272 656e 745f 7820 3d20 5b5d 0d0a 2020  rrent_x = []..  
-000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012200: 2063 7572 7265 6e74 5f69 6e74 656e 7369   current_intensi
-00012210: 7479 203d 205b 5d0d 0a20 2020 2020 2020  ty = []..       
-00012220: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012230: 656e 745f 636c 7573 7465 725f 636c 6173  ent_cluster_clas
-00012240: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00012250: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012260: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00012270: 5f73 636f 7265 203d 205b 5d0d 0a20 2020  _score = []..   
-00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012290: 6375 7272 656e 745f 7261 6469 7573 203d  current_radius =
-000122a0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000122b0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000122c0: 766f 6c75 6d65 203d 205b 5d0d 0a20 2020  volume = []..   
-000122d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122e0: 6375 7272 656e 745f 7370 6565 6420 3d20  current_speed = 
-000122f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00012300: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
-00012310: 6f74 696f 6e5f 616e 676c 6520 3d20 5b5d  otion_angle = []
-00012320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012330: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
-00012340: 656c 6572 6174 696f 6e20 3d20 5b5d 0d0a  eleration = []..
-00012350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012360: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
-00012370: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
-00012380: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00012390: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
-000123a0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-000123b0: 5f66 6972 7374 203d 205b 5d0d 0a20 2020  _first = []..   
-000123c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123d0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-000123e0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-000123f0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012400: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012410: 745f 7375 7266 6163 655f 6172 6561 203d  t_surface_area =
-00012420: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00012430: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012440: 745f 7261 6469 616c 5f61 6e67 6c65 203d  t_radial_angle =
-00012450: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012460: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012470: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
-00012480: 205b 5d20 0d0a 2020 2020 2020 2020 2020   [] ..          
-00012490: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000124a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000124b0: 7220 6a20 696e 2072 616e 6765 2874 696d  r j in range(tim
-000124c0: 652e 7368 6170 655b 305d 293a 0d0a 2020  e.shape[0]):..  
-000124d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124e0: 2020 2020 2020 2020 6966 2063 7572 7265          if curre
-000124f0: 6e74 5f75 6e69 7175 655f 6964 203d 3d20  nt_unique_id == 
-00012500: 756e 6971 7565 5f69 6473 5b6a 5d3a 0d0a  unique_ids[j]:..
-00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012530: 2063 7572 7265 6e74 5f74 696d 652e 6170   current_time.ap
-00012540: 7065 6e64 2874 696d 655b 6a5d 290d 0a20  pend(time[j]).. 
-00012550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 6375 7272 656e 745f 7a2e 6170 7065 6e64  current_z.append
-00012580: 285a 5b6a 5d29 0d0a 2020 2020 2020 2020  (Z[j])..        
-00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125a0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000125b0: 5f79 2e61 7070 656e 6428 595b 6a5d 290d  _y.append(Y[j]).
-000125c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 6375 7272 656e 745f 782e 6170 7065    current_x.appe
-000125f0: 6e64 2858 5b6a 5d29 0d0a 2020 2020 2020  nd(X[j])..      
+000117c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000117d0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000117e0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+000117f0: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+00011800: 6461 7465 287b 7365 6c66 2e73 7572 6661  date({self.surfa
+00011810: 6365 5f61 7265 615f 6b65 7920 3a20 7375  ce_area_key : su
+00011820: 7266 6163 655f 6172 6561 7d29 0d0a 2020  rface_area})..  
+00011830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011850: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00011860: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00011870: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00011880: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
+00011890: 7465 287b 7365 6c66 2e71 7561 6c69 7479  te({self.quality
+000118a0: 5f6b 6579 203a 2071 7561 6c69 7479 7d29  _key : quality})
+000118b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000118e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000118f0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00011900: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00011910: 7570 6461 7465 287b 7365 6c66 2e72 6164  update({self.rad
+00011920: 6975 735f 6b65 7920 3a20 7175 616c 6974  ius_key : qualit
+00011930: 7920 2a20 6d61 7468 2e70 6f77 2873 656c  y * math.pow(sel
+00011940: 662e 7a63 616c 6962 7261 7469 6f6e 202a  f.zcalibration *
+00011950: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
+00011960: 6f6e 202a 2073 656c 662e 7963 616c 6962  on * self.ycalib
+00011970: 7261 7469 6f6e 2c20 312e 302f 332e 3029  ration, 1.0/3.0)
+00011980: 207d 290d 0a0d 0a0d 0a20 2020 2020 2020   })......       
+00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119a0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119c0: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
+000119d0: 2c76 2920 696e 2073 656c 662e 726f 6f74  ,v) in self.root
+000119e0: 5f73 706f 7473 2e69 7465 6d73 2829 3a0d  _spots.items():.
+000119f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a10: 2020 2073 656c 662e 726f 6f74 5f73 706f     self.root_spo
+00011a20: 7473 5b6b 5d20 3d20 7365 6c66 2e75 6e69  ts[k] = self.uni
+00011a30: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011a40: 6965 735b 6b5d 2020 2020 2020 2020 200d  ies[k]         .
+00011a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011a60: 200d 0a20 2020 2064 6566 205f 636f 6d70   ..    def _comp
+00011a70: 7574 655f 7068 656e 6f74 7970 6573 2873  ute_phenotypes(s
+00011a80: 656c 6629 3a0d 0a0d 0a20 2020 2020 2020  elf):....       
+00011a90: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+00011aa0: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
+00011ab0: 6b73 2e69 7465 6d73 2829 3a0d 0a20 2020  ks.items():..   
+00011ac0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00011ad0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00011ae0: 7261 636b 5f69 6420 3d20 6b0d 0a20 2020  rack_id = k..   
+00011af0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00011b00: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00011b10: 203d 2073 656c 662e 756e 6971 7565 5f74   = self.unique_t
+00011b20: 7261 636b 5f70 726f 7065 7274 6965 735b  rack_properties[
+00011b30: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
+00011b40: 2020 2020 7472 6163 6b73 203d 2073 656c      tracks = sel
+00011b50: 662e 756e 6971 7565 5f74 7261 636b 735b  f.unique_tracks[
+00011b60: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
+00011b70: 2020 2020 5a20 3d20 7472 6163 6b73 5b3a      Z = tracks[:
+00011b80: 2c32 5d0d 0a20 2020 2020 2020 2020 2020  ,2]..           
+00011b90: 2020 2020 2059 203d 2074 7261 636b 735b       Y = tracks[
+00011ba0: 3a2c 335d 0d0a 2020 2020 2020 2020 2020  :,3]..          
+00011bb0: 2020 2020 2020 5820 3d20 7472 6163 6b73        X = tracks
+00011bc0: 5b3a 2c34 5d0d 0a20 2020 2020 2020 2020  [:,4]..         
+00011bd0: 2020 2020 2020 2074 696d 6520 3d20 7472         time = tr
+00011be0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00011bf0: 735b 3a2c 305d 0d0a 2020 2020 2020 2020  s[:,0]..        
+00011c00: 2020 2020 2020 2020 756e 6971 7565 5f69          unique_i
+00011c10: 6473 203d 2074 7261 636b 6c65 745f 7072  ds = tracklet_pr
+00011c20: 6f70 6572 7469 6573 5b3a 2c31 5d0d 0a20  operties[:,1].. 
+00011c30: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00011c40: 6e69 7175 655f 6964 735f 7365 7420 3d20  nique_ids_set = 
+00011c50: 7365 7428 756e 6971 7565 5f69 6473 290d  set(unique_ids).
+00011c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011c70: 2067 656e 6572 6174 696f 6e5f 6964 7320   generation_ids 
+00011c80: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00011c90: 7274 6965 735b 3a2c 325d 0d0a 2020 2020  rties[:,2]..    
+00011ca0: 2020 2020 2020 2020 2020 2020 7261 6469              radi
+00011cb0: 7573 203d 2074 7261 636b 6c65 745f 7072  us = tracklet_pr
+00011cc0: 6f70 6572 7469 6573 5b3a 2c33 5d0d 0a20  operties[:,3].. 
+00011cd0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00011ce0: 6f6c 756d 6520 3d20 7472 6163 6b6c 6574  olume = tracklet
+00011cf0: 5f70 726f 7065 7274 6965 735b 3a2c 345d  _properties[:,4]
+00011d00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011d10: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
+00011d20: 6f6d 705f 6669 7273 7420 3d20 7472 6163  omp_first = trac
+00011d30: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00011d40: 3a2c 355d 0d0a 2020 2020 2020 2020 2020  :,5]..          
+00011d50: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
+00011d60: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
+00011d70: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00011d80: 7469 6573 5b3a 2c36 5d0d 0a20 2020 2020  ties[:,6]..     
+00011d90: 2020 2020 2020 2020 2020 2073 7572 6661             surfa
+00011da0: 6365 5f61 7265 6120 3d20 7472 6163 6b6c  ce_area = trackl
+00011db0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00011dc0: 375d 0d0a 2020 2020 2020 2020 2020 2020  7]..            
+00011dd0: 2020 2020 636c 7573 7465 725f 636c 6173      cluster_clas
+00011de0: 7320 3d20 7472 6163 6b6c 6574 5f70 726f  s = tracklet_pro
+00011df0: 7065 7274 6965 735b 3a2c 385d 0d0a 2020  perties[:,8]..  
+00011e00: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00011e10: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
+00011e20: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
+00011e30: 7065 7274 6965 735b 3a2c 395d 0d0a 2020  perties[:,9]..  
+00011e40: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00011e50: 7465 6e73 6974 7920 3d20 7472 6163 6b6c  tensity = trackl
+00011e60: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00011e70: 3130 5d0d 0a20 2020 2020 2020 2020 2020  10]..           
+00011e80: 2020 2020 2073 7065 6564 203d 2074 7261       speed = tra
+00011e90: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00011ea0: 5b3a 2c31 315d 0d0a 2020 2020 2020 2020  [:,11]..        
+00011eb0: 2020 2020 2020 2020 6d6f 7469 6f6e 5f61          motion_a
+00011ec0: 6e67 6c65 203d 2074 7261 636b 6c65 745f  ngle = tracklet_
+00011ed0: 7072 6f70 6572 7469 6573 5b3a 2c31 325d  properties[:,12]
+00011ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011ef0: 2020 6163 6365 6c65 7261 7469 6f6e 203d    acceleration =
+00011f00: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00011f10: 7469 6573 5b3a 2c31 335d 0d0a 2020 2020  ties[:,13]..    
+00011f20: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+00011f30: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00011f40: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00011f50: 7469 6573 5b3a 2c31 345d 0d0a 2020 2020  ties[:,14]..    
+00011f60: 2020 2020 2020 2020 2020 2020 7261 6469              radi
+00011f70: 616c 5f61 6e67 6c65 203d 2074 7261 636b  al_angle = track
+00011f80: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00011f90: 2c31 355d 0d0a 2020 2020 2020 2020 2020  ,15]..          
+00011fa0: 2020 2020 2020 6365 6c6c 5f61 7869 735f        cell_axis_
+00011fb0: 6d61 736b 203d 2074 7261 636b 6c65 745f  mask = tracklet_
+00011fc0: 7072 6f70 6572 7469 6573 5b3a 2c31 365d  properties[:,16]
+00011fd0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00011fe0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00011ff0: 2020 2020 2020 2020 756e 6971 7565 5f66          unique_f
+00012000: 6674 5f70 726f 7065 7274 6965 735f 7472  ft_properties_tr
+00012010: 6163 6b6c 6574 203d 207b 7d0d 0a20 2020  acklet = {}..   
+00012020: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00012030: 7175 655f 636c 7573 7465 725f 7072 6f70  que_cluster_prop
+00012040: 6572 7469 6573 5f74 7261 636b 6c65 7420  erties_tracklet 
+00012050: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00012060: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00012070: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
+00012080: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
+00012090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000120a0: 2073 656c 662e 756e 6971 7565 5f63 6c75   self.unique_clu
+000120b0: 7374 6572 5f70 726f 7065 7274 6965 735b  ster_properties[
+000120c0: 7472 6163 6b5f 6964 5d20 3d20 7b7d 0d0a  track_id] = {}..
+000120d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000120e0: 2020 756e 6971 7565 5f73 6861 7065 5f70    unique_shape_p
+000120f0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00012100: 6574 203d 207b 7d0d 0a20 2020 2020 2020  et = {}..       
+00012110: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
+00012120: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
+00012130: 6573 5f74 7261 636b 6c65 7420 3d20 7b7d  es_tracklet = {}
+00012140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012150: 2020 7365 6c66 2e75 6e69 7175 655f 7368    self.unique_sh
+00012160: 6170 655f 7072 6f70 6572 7469 6573 5b74  ape_properties[t
+00012170: 7261 636b 5f69 645d 203d 207b 7d0d 0a20  rack_id] = {}.. 
+00012180: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012190: 656c 662e 756e 6971 7565 5f64 796e 616d  elf.unique_dynam
+000121a0: 6963 5f70 726f 7065 7274 6965 735b 7472  ic_properties[tr
+000121b0: 6163 6b5f 6964 5d20 3d20 7b7d 0d0a 2020  ack_id] = {}..  
+000121c0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+000121d0: 7061 6e64 6564 5f74 696d 6520 3d20 6e70  panded_time = np
+000121e0: 2e7a 6572 6f73 2873 656c 662e 7465 6e64  .zeros(self.tend
+000121f0: 202d 2073 656c 662e 7473 7461 7274 202b   - self.tstart +
+00012200: 2031 290d 0a20 2020 2020 2020 2020 2020   1)..           
+00012210: 2020 2020 2070 6f69 6e74 5f73 616d 706c       point_sampl
+00012220: 6520 3d20 6578 7061 6e64 6564 5f74 696d  e = expanded_tim
+00012230: 652e 7368 6170 655b 305d 0d0a 2020 2020  e.shape[0]..    
+00012240: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00012250: 6920 696e 2072 616e 6765 286c 656e 2865  i in range(len(e
+00012260: 7870 616e 6465 645f 7469 6d65 2929 3a0d  xpanded_time)):.
+00012270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012280: 2020 2020 2020 2020 6578 7061 6e64 6564          expanded
+00012290: 5f74 696d 655b 695d 203d 2069 200d 0a20  _time[i] = i .. 
+000122a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000122b0: 6f72 2063 7572 7265 6e74 5f75 6e69 7175  or current_uniqu
+000122c0: 655f 6964 2069 6e20 756e 6971 7565 5f69  e_id in unique_i
+000122d0: 6473 5f73 6574 3a0d 0a20 2020 2020 2020  ds_set:..       
+000122e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000122f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012300: 2065 7870 616e 6465 645f 696e 7465 6e73   expanded_intens
+00012310: 6974 7920 3d20 6e70 2e7a 6572 6f73 2873  ity = np.zeros(s
+00012320: 656c 662e 7465 6e64 202d 2073 656c 662e  elf.tend - self.
+00012330: 7473 7461 7274 202b 2031 290d 0a20 2020  tstart + 1)..   
+00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012360: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00012370: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012380: 745f 7469 6d65 203d 205b 5d0d 0a20 2020  t_time = []..   
+00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123a0: 6375 7272 656e 745f 7a20 3d20 5b5d 0d0a  current_z = []..
+000123b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123c0: 2020 2063 7572 7265 6e74 5f79 203d 205b     current_y = [
+000123d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000123e0: 2020 2020 2020 6375 7272 656e 745f 7820        current_x 
+000123f0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012400: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012410: 5f69 6e74 656e 7369 7479 203d 205b 5d0d  _intensity = [].
+00012420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012430: 2020 2020 6375 7272 656e 745f 636c 7573      current_clus
+00012440: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
+00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012460: 2020 2063 7572 7265 6e74 5f63 6c75 7374     current_clust
+00012470: 6572 5f63 6c61 7373 5f73 636f 7265 203d  er_class_score =
+00012480: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00012490: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000124a0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124c0: 6375 7272 656e 745f 766f 6c75 6d65 203d  current_volume =
+000124d0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000124e0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000124f0: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00012500: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012510: 7572 7265 6e74 5f6d 6f74 696f 6e5f 616e  urrent_motion_an
+00012520: 676c 6520 3d20 5b5d 0d0a 2020 2020 2020  gle = []..      
+00012530: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012540: 7265 6e74 5f61 6363 656c 6572 6174 696f  rent_acceleratio
+00012550: 6e20 3d20 5b5d 0d0a 2020 2020 2020 2020  n = []..        
+00012560: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012570: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
+00012580: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
+00012590: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000125a0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+000125b0: 6974 795f 636f 6d70 5f66 6972 7374 203d  ity_comp_first =
+000125c0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000125d0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000125e0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+000125f0: 705f 7365 636f 6e64 203d 205b 5d0d 0a20  p_second = [].. 
 00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012610: 2020 2020 2020 2020 2020 2065 7870 616e             expan
-00012620: 6465 645f 696e 7465 6e73 6974 795b 696e  ded_intensity[in
-00012630: 7428 7469 6d65 5b6a 5d29 5d20 3d20 696e  t(time[j])] = in
-00012640: 7465 6e73 6974 795b 6a5d 0d0a 2020 2020  tensity[j]..    
-00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012660: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012670: 7265 6e74 5f69 6e74 656e 7369 7479 2e61  rent_intensity.a
-00012680: 7070 656e 6428 696e 7465 6e73 6974 795b  ppend(intensity[
-00012690: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-000126a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126b0: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
-000126c0: 7573 7465 725f 636c 6173 732e 6170 7065  uster_class.appe
-000126d0: 6e64 2863 6c75 7374 6572 5f63 6c61 7373  nd(cluster_class
-000126e0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-000126f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012700: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00012710: 6c75 7374 6572 5f63 6c61 7373 5f73 636f  luster_class_sco
-00012720: 7265 2e61 7070 656e 6428 636c 7573 7465  re.append(cluste
-00012730: 725f 636c 6173 735f 7363 6f72 655b 6a5d  r_class_score[j]
-00012740: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 2020 2020 6375 7272 656e 745f 7261 6469      current_radi
-00012770: 7573 2e61 7070 656e 6428 7261 6469 7573  us.append(radius
-00012780: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00012610: 2020 6375 7272 656e 745f 7375 7266 6163    current_surfac
+00012620: 655f 6172 6561 203d 205b 5d0d 0a0d 0a20  e_area = [].... 
+00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012640: 2020 6375 7272 656e 745f 7261 6469 616c    current_radial
+00012650: 5f61 6e67 6c65 203d 205b 5d0d 0a20 2020  _angle = []..   
+00012660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012670: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
+00012680: 735f 6d61 736b 203d 205b 5d20 0d0a 2020  s_mask = [] ..  
+00012690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000126b0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+000126c0: 616e 6765 2874 696d 652e 7368 6170 655b  ange(time.shape[
+000126d0: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
+000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126f0: 6966 2063 7572 7265 6e74 5f75 6e69 7175  if current_uniqu
+00012700: 655f 6964 203d 3d20 756e 6971 7565 5f69  e_id == unique_i
+00012710: 6473 5b6a 5d3a 0d0a 2020 2020 2020 2020  ds[j]:..        
+00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012730: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012740: 5f74 696d 652e 6170 7065 6e64 2874 696d  _time.append(tim
+00012750: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
+00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012770: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012780: 7a2e 6170 7065 6e64 285a 5b6a 5d29 0d0a  z.append(Z[j])..
 00012790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127a0: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
-000127b0: 6f6c 756d 652e 6170 7065 6e64 2876 6f6c  olume.append(vol
-000127c0: 756d 655b 6a5d 290d 0a20 2020 2020 2020  ume[j])..       
+000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127b0: 2063 7572 7265 6e74 5f79 2e61 7070 656e   current_y.appen
+000127c0: 6428 595b 6a5d 290d 0a20 2020 2020 2020  d(Y[j])..       
 000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000127e0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000127f0: 745f 7370 6565 642e 6170 7065 6e64 2873  t_speed.append(s
-00012800: 7065 6564 5b6a 5d29 0d0a 2020 2020 2020  peed[j])..      
+000127f0: 745f 782e 6170 7065 6e64 2858 5b6a 5d29  t_x.append(X[j])
+00012800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012820: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012830: 6e74 5f6d 6f74 696f 6e5f 616e 676c 652e  nt_motion_angle.
-00012840: 6170 7065 6e64 286d 6f74 696f 6e5f 616e  append(motion_an
-00012850: 676c 655b 6a5d 290d 0a20 2020 2020 2020  gle[j])..       
+00012820: 2020 2065 7870 616e 6465 645f 696e 7465     expanded_inte
+00012830: 6e73 6974 795b 696e 7428 7469 6d65 5b6a  nsity[int(time[j
+00012840: 5d29 5d20 3d20 696e 7465 6e73 6974 795b  ])] = intensity[
+00012850: 6a5d 0d0a 2020 2020 2020 2020 2020 2020  j]..            
 00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012870: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012880: 745f 6163 6365 6c65 7261 7469 6f6e 2e61  t_acceleration.a
-00012890: 7070 656e 6428 6163 6365 6c65 7261 7469  ppend(accelerati
-000128a0: 6f6e 5b6a 5d29 0d0a 2020 2020 2020 2020  on[j])..        
-000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128c0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000128d0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-000128e0: 6173 6b2e 6170 7065 6e64 2864 6973 7461  ask.append(dista
-000128f0: 6e63 655f 6365 6c6c 5f6d 6173 6b5b 6a5d  nce_cell_mask[j]
-00012900: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012920: 2020 2020 6375 7272 656e 745f 6563 6365      current_ecce
-00012930: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00012940: 7273 742e 6170 7065 6e64 2865 6363 656e  rst.append(eccen
-00012950: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00012960: 7374 5b6a 5d29 0d0a 2020 2020 2020 2020  st[j])..        
-00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012980: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012990: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-000129a0: 6d70 5f73 6563 6f6e 642e 6170 7065 6e64  mp_second.append
-000129b0: 2865 6363 656e 7472 6963 6974 795f 636f  (eccentricity_co
-000129c0: 6d70 5f73 6563 6f6e 645b 6a5d 290d 0a20  mp_second[j]).. 
-000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012870: 2020 2020 2063 7572 7265 6e74 5f69 6e74       current_int
+00012880: 656e 7369 7479 2e61 7070 656e 6428 696e  ensity.append(in
+00012890: 7465 6e73 6974 795b 6a5d 290d 0a20 2020  tensity[j])..   
+000128a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128b0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000128c0: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
+000128d0: 6173 732e 6170 7065 6e64 2863 6c75 7374  ass.append(clust
+000128e0: 6572 5f63 6c61 7373 5b6a 5d29 0d0a 2020  er_class[j])..  
+000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012900: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012910: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
+00012920: 6c61 7373 5f73 636f 7265 2e61 7070 656e  lass_score.appen
+00012930: 6428 636c 7573 7465 725f 636c 6173 735f  d(cluster_class_
+00012940: 7363 6f72 655b 6a5d 290d 0a20 2020 2020  score[j])..     
+00012950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012960: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012970: 656e 745f 7261 6469 7573 2e61 7070 656e  ent_radius.appen
+00012980: 6428 7261 6469 7573 5b6a 5d29 0d0a 2020  d(radius[j])..  
+00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000129b0: 7572 7265 6e74 5f76 6f6c 756d 652e 6170  urrent_volume.ap
+000129c0: 7065 6e64 2876 6f6c 756d 655b 6a5d 290d  pend(volume[j]).
+000129d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000129e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129f0: 6375 7272 656e 745f 7375 7266 6163 655f  current_surface_
-00012a00: 6172 6561 2e61 7070 656e 6428 7375 7266  area.append(surf
-00012a10: 6163 655f 6172 6561 5b6a 5d29 0d0a 2020  ace_area[j])..  
+000129f0: 2020 6375 7272 656e 745f 7370 6565 642e    current_speed.
+00012a00: 6170 7065 6e64 2873 7065 6564 5b6a 5d29  append(speed[j])
+00012a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012a40: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
-00012a50: 676c 652e 6170 7065 6e64 2872 6164 6961  gle.append(radia
-00012a60: 6c5f 616e 676c 655b 6a5d 290d 0a20 2020  l_angle[j])..   
+00012a30: 2020 2063 7572 7265 6e74 5f6d 6f74 696f     current_motio
+00012a40: 6e5f 616e 676c 652e 6170 7065 6e64 286d  n_angle.append(m
+00012a50: 6f74 696f 6e5f 616e 676c 655b 6a5d 290d  otion_angle[j]).
+00012a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a80: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012a90: 7272 656e 745f 6365 6c6c 5f61 7869 735f  rrent_cell_axis_
-00012aa0: 6d61 736b 2e61 7070 656e 6428 6365 6c6c  mask.append(cell
-00012ab0: 5f61 7869 735f 6d61 736b 5b6a 5d29 0d0a  _axis_mask[j])..
+00012a80: 2020 6375 7272 656e 745f 6163 6365 6c65    current_accele
+00012a90: 7261 7469 6f6e 2e61 7070 656e 6428 6163  ration.append(ac
+00012aa0: 6365 6c65 7261 7469 6f6e 5b6a 5d29 0d0a  celeration[j])..
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ad0: 2020 2063 7572 7265 6e74 5f74 696d 6520     current_time 
-00012ae0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-00012af0: 7265 6e74 5f74 696d 652c 2064 7479 7065  rent_time, dtype
-00012b00: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+00012ad0: 2063 7572 7265 6e74 5f64 6973 7461 6e63   current_distanc
+00012ae0: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00012af0: 6e64 2864 6973 7461 6e63 655f 6365 6c6c  nd(distance_cell
+00012b00: 5f6d 6173 6b5b 6a5d 290d 0a20 2020 2020  _mask[j])..     
 00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b20: 2063 7572 7265 6e74 5f69 6e74 656e 7369   current_intensi
-00012b30: 7479 203d 206e 702e 6173 6172 7261 7928  ty = np.asarray(
-00012b40: 6375 7272 656e 745f 696e 7465 6e73 6974  current_intensit
-00012b50: 792c 2064 7479 7065 3d6e 702e 666c 6f61  y, dtype=np.floa
-00012b60: 7433 3229 0d0a 0d0a 0d0a 2020 2020 2020  t32)......      
-00012b70: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012b80: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
-00012b90: 7373 203d 206e 702e 6173 6172 7261 7928  ss = np.asarray(
-00012ba0: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
-00012bb0: 636c 6173 732c 2064 7479 7065 3d6e 702e  class, dtype=np.
-00012bc0: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
-00012bd0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012be0: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
-00012bf0: 7373 5f73 636f 7265 203d 206e 702e 6173  ss_score = np.as
-00012c00: 6172 7261 7928 6375 7272 656e 745f 636c  array(current_cl
-00012c10: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
-00012c20: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
-00012c30: 7433 3229 2020 200d 0a0d 0a20 2020 2020  t32)   ....     
-00012c40: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012c50: 7272 656e 745f 7261 6469 7573 203d 206e  rrent_radius = n
-00012c60: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-00012c70: 745f 7261 6469 7573 2c20 6474 7970 653d  t_radius, dtype=
-00012c80: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
-00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ca0: 6375 7272 656e 745f 766f 6c75 6d65 203d  current_volume =
-00012cb0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00012cc0: 656e 745f 766f 6c75 6d65 2c20 6474 7970  ent_volume, dtyp
-00012cd0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cf0: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
-00012d00: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00012d10: 7420 3d20 6e70 2e61 7361 7272 6179 2863  t = np.asarray(c
-00012d20: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-00012d30: 6974 795f 636f 6d70 5f66 6972 7374 2c20  ity_comp_first, 
-00012d40: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00012d50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012d60: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
-00012d70: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00012d80: 7365 636f 6e64 203d 206e 702e 6173 6172  second = np.asar
-00012d90: 7261 7928 6375 7272 656e 745f 6563 6365  ray(current_ecce
-00012da0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00012db0: 636f 6e64 2c20 6474 7970 653d 6e70 2e66  cond, dtype=np.f
-00012dc0: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-00012dd0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012de0: 656e 745f 7375 7266 6163 655f 6172 6561  ent_surface_area
-00012df0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00012e00: 7272 656e 745f 7375 7266 6163 655f 6172  rrent_surface_ar
-00012e10: 6561 2c20 6474 7970 653d 6e70 2e66 6c6f  ea, dtype=np.flo
-00012e20: 6174 3332 290d 0a0d 0a20 2020 2020 2020  at32)....       
-00012e30: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012e40: 656e 745f 7370 6565 6420 3d20 6e70 2e61  ent_speed = np.a
-00012e50: 7361 7272 6179 2863 7572 7265 6e74 5f73  sarray(current_s
-00012e60: 7065 6564 2c20 6474 7970 653d 6e70 2e66  peed, dtype=np.f
-00012e70: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-00012e80: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012e90: 656e 745f 6d6f 7469 6f6e 5f61 6e67 6c65  ent_motion_angle
-00012ea0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00012eb0: 7272 656e 745f 6d6f 7469 6f6e 5f61 6e67  rrent_motion_ang
-00012ec0: 6c65 2c20 6474 7970 653d 6e70 2e66 6c6f  le, dtype=np.flo
-00012ed0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-00012ee0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012ef0: 745f 6163 6365 6c65 7261 7469 6f6e 203d  t_acceleration =
-00012f00: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00012f10: 656e 745f 6163 6365 6c65 7261 7469 6f6e  ent_acceleration
-00012f20: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00012f30: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-00012f40: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012f50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00012f60: 736b 203d 206e 702e 6173 6172 7261 7928  sk = np.asarray(
-00012f70: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
-00012f80: 5f63 656c 6c5f 6d61 736b 2c20 6474 7970  _cell_mask, dtyp
-00012f90: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fb0: 2020 6375 7272 656e 745f 7261 6469 616c    current_radial
-00012fc0: 5f61 6e67 6c65 203d 206e 702e 6173 6172  _angle = np.asar
-00012fd0: 7261 7928 6375 7272 656e 745f 7261 6469  ray(current_radi
-00012fe0: 616c 5f61 6e67 6c65 2c20 6474 7970 653d  al_angle, dtype=
-00012ff0: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
-00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013010: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
-00013020: 735f 6d61 736b 203d 206e 702e 6173 6172  s_mask = np.asar
-00013030: 7261 7928 6375 7272 656e 745f 6365 6c6c  ray(current_cell
-00013040: 5f61 7869 735f 6d61 736b 2c20 6474 7970  _axis_mask, dtyp
-00013050: 653d 6e70 2e66 6c6f 6174 3332 290d 0a0d  e=np.float32)...
-00013060: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00013070: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00013080: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00013090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130a0: 6966 2070 6f69 6e74 5f73 616d 706c 6520  if point_sample 
-000130b0: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
-000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130d0: 2020 2020 2020 7866 5f73 616d 706c 6520        xf_sample 
-000130e0: 3d20 6666 7466 7265 7128 706f 696e 745f  = fftfreq(point_
-000130f0: 7361 6d70 6c65 2c20 7365 6c66 2e74 6361  sample, self.tca
-00013100: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
-00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013120: 2020 2020 2020 2020 2020 2020 6666 7473              ffts
-00013130: 7472 6970 5f73 616d 706c 6520 3d20 6666  trip_sample = ff
-00013140: 7428 6578 7061 6e64 6564 5f69 6e74 656e  t(expanded_inten
-00013150: 7369 7479 290d 0a20 2020 2020 2020 2020  sity)..         
-00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013170: 2020 2020 2020 2066 6674 746f 7461 6c5f         ffttotal_
-00013180: 7361 6d70 6c65 203d 206e 702e 6162 7328  sample = np.abs(
-00013190: 6666 7473 7472 6970 5f73 616d 706c 6529  fftstrip_sample)
-000131a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000131b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131c0: 2020 7866 5f73 616d 706c 6520 3d20 7866    xf_sample = xf
-000131d0: 5f73 616d 706c 655b 3020 3a20 6c65 6e28  _sample[0 : len(
-000131e0: 7866 5f73 616d 706c 6529 202f 2f20 325d  xf_sample) // 2]
-000131f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013210: 2020 6666 7474 6f74 616c 5f73 616d 706c    ffttotal_sampl
-00013220: 6520 3d20 6666 7474 6f74 616c 5f73 616d  e = ffttotal_sam
-00013230: 706c 655b 3020 3a20 6c65 6e28 6666 7474  ple[0 : len(fftt
-00013240: 6f74 616c 5f73 616d 706c 6529 202f 2f20  otal_sample) // 
-00013250: 325d 0d0a 0d0a 2020 2020 2020 2020 2020  2]....          
-00013260: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-00013270: 6666 745f 7072 6f70 6572 7469 6573 5f74  fft_properties_t
-00013280: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
-00013290: 756e 6971 7565 5f69 645d 203d 2065 7870  unique_id] = exp
-000132a0: 616e 6465 645f 7469 6d65 2c20 6578 7061  anded_time, expa
-000132b0: 6e64 6564 5f69 6e74 656e 7369 7479 2c20  nded_intensity, 
-000132c0: 7866 5f73 616d 706c 652c 2066 6674 746f  xf_sample, fftto
-000132d0: 7461 6c5f 7361 6d70 6c65 0d0a 2020 2020  tal_sample..    
-000132e0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-000132f0: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
-00013300: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-00013310: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
-00013320: 5f69 645d 203d 2020 6375 7272 656e 745f  _id] =  current_
-00013330: 7469 6d65 2c20 6375 7272 656e 745f 636c  time, current_cl
-00013340: 7573 7465 725f 636c 6173 732c 2063 7572  uster_class, cur
-00013350: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
-00013360: 7373 5f73 636f 7265 0d0a 2020 2020 2020  ss_score..      
-00013370: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-00013380: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
-00013390: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
-000133a0: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
-000133b0: 203d 2063 7572 7265 6e74 5f74 696d 652c   = current_time,
-000133c0: 2063 7572 7265 6e74 5f7a 2c20 6375 7272   current_z, curr
-000133d0: 656e 745f 792c 2063 7572 7265 6e74 5f78  ent_y, current_x
-000133e0: 2c20 6375 7272 656e 745f 7261 6469 7573  , current_radius
-000133f0: 2c20 6375 7272 656e 745f 766f 6c75 6d65  , current_volume
-00013400: 2c20 6375 7272 656e 745f 6563 6365 6e74  , current_eccent
-00013410: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00013420: 742c 2063 7572 7265 6e74 5f65 6363 656e  t, current_eccen
-00013430: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00013440: 6f6e 642c 2063 7572 7265 6e74 5f73 7572  ond, current_sur
-00013450: 6661 6365 5f61 7265 612c 2063 7572 7265  face_area, curre
-00013460: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00013470: 2c20 6375 7272 656e 745f 636c 7573 7465  , current_cluste
-00013480: 725f 636c 6173 735f 7363 6f72 650d 0a20  r_class_score.. 
-00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134a0: 2020 756e 6971 7565 5f64 796e 616d 6963    unique_dynamic
-000134b0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-000134c0: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-000134d0: 7175 655f 6964 5d20 3d20 6375 7272 656e  que_id] = curren
-000134e0: 745f 7469 6d65 2c20 6375 7272 656e 745f  t_time, current_
-000134f0: 7370 6565 642c 2063 7572 7265 6e74 5f6d  speed, current_m
-00013500: 6f74 696f 6e5f 616e 676c 652c 2063 7572  otion_angle, cur
-00013510: 7265 6e74 5f61 6363 656c 6572 6174 696f  rent_acceleratio
-00013520: 6e2c 2063 7572 7265 6e74 5f64 6973 7461  n, current_dista
-00013530: 6e63 655f 6365 6c6c 5f6d 6173 6b2c 2063  nce_cell_mask, c
-00013540: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
-00013550: 676c 652c 2063 7572 7265 6e74 5f63 656c  gle, current_cel
-00013560: 6c5f 6178 6973 5f6d 6173 6b0d 0a20 2020  l_axis_mask..   
-00013570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013580: 7365 6c66 2e75 6e69 7175 655f 6666 745f  self.unique_fft_
-00013590: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
-000135a0: 5f69 645d 2e75 7064 6174 6528 7b63 7572  _id].update({cur
-000135b0: 7265 6e74 5f75 6e69 7175 655f 6964 3a75  rent_unique_id:u
-000135c0: 6e69 7175 655f 6666 745f 7072 6f70 6572  nique_fft_proper
-000135d0: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
-000135e0: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
-000135f0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00013600: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00013610: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
-00013620: 7274 6965 735b 7472 6163 6b5f 6964 5d2e  rties[track_id].
-00013630: 7570 6461 7465 287b 6375 7272 656e 745f  update({current_
-00013640: 756e 6971 7565 5f69 643a 756e 6971 7565  unique_id:unique
-00013650: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
-00013660: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
-00013670: 7265 6e74 5f75 6e69 7175 655f 6964 5d7d  rent_unique_id]}
-00013680: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00013690: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000136a0: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
-000136b0: 7469 6573 5b74 7261 636b 5f69 645d 2e75  ties[track_id].u
-000136c0: 7064 6174 6528 7b63 7572 7265 6e74 5f75  pdate({current_u
-000136d0: 6e69 7175 655f 6964 3a75 6e69 7175 655f  nique_id:unique_
-000136e0: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
-000136f0: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-00013700: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
-00013710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013720: 2020 2073 656c 662e 756e 6971 7565 5f64     self.unique_d
-00013730: 796e 616d 6963 5f70 726f 7065 7274 6965  ynamic_propertie
-00013740: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
-00013750: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
-00013760: 7565 5f69 643a 756e 6971 7565 5f64 796e  ue_id:unique_dyn
-00013770: 616d 6963 5f70 726f 7065 7274 6965 735f  amic_properties_
-00013780: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
-00013790: 5f75 6e69 7175 655f 6964 5d7d 290d 0a0d  _unique_id]})...
-000137a0: 0a20 2020 2064 6566 205f 7365 636f 6e64  .    def _second
-000137b0: 5f63 6861 6e6e 656c 5f73 706f 7473 2873  _channel_spots(s
-000137c0: 656c 662c 2066 7261 6d65 2c20 7a2c 2079  elf, frame, z, y
-000137d0: 2c20 782c 2063 656c 6c5f 6964 2c20 7472  , x, cell_id, tr
-000137e0: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
-000137f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00013800: 2020 2074 7265 652c 2063 656e 7472 6f69     tree, centroi
-00013810: 6473 2c20 6c61 6265 6c73 2c20 766f 6c75  ds, labels, volu
-00013820: 6d65 2c20 696e 7465 6e73 6974 795f 6d65  me, intensity_me
-00013830: 616e 2c20 696e 7465 6e73 6974 795f 746f  an, intensity_to
-00013840: 7461 6c2c 2062 6f75 6e64 696e 675f 626f  tal, bounding_bo
-00013850: 7865 7320 3d20 7365 6c66 2e5f 7469 6d65  xes = self._time
-00013860: 645f 6368 616e 6e65 6c5f 7365 675f 696d  d_channel_seg_im
-00013870: 6167 655b 7374 7228 696e 7428 666c 6f61  age[str(int(floa
-00013880: 7428 6672 616d 6529 2929 5d0d 0a20 2020  t(frame)))]..   
-00013890: 2020 2020 2020 2020 2070 6978 656c 7465           pixelte
-000138a0: 7374 6c6f 6361 7469 6f6e 203d 2028 7a2c  stlocation = (z,
-000138b0: 792c 7829 0d0a 2020 2020 2020 2020 2020  y,x)..          
-000138c0: 2020 6469 7374 2c20 696e 6465 7820 3d20    dist, index = 
-000138d0: 7472 6565 2e71 7565 7279 2870 6978 656c  tree.query(pixel
-000138e0: 7465 7374 6c6f 6361 7469 6f6e 290d 0a0d  testlocation)...
-000138f0: 0a0d 0a20 2020 2020 2020 2020 2020 2062  ...            b
-00013900: 626f 7820 3d20 626f 756e 6469 6e67 5f62  box = bounding_b
-00013910: 6f78 6573 5b69 6e64 6578 5d0d 0a20 2020  oxes[index]..   
-00013920: 2020 2020 2020 2020 2073 697a 657a 203d           sizez =
-00013930: 2061 6273 2862 626f 785b 305d 202d 2062   abs(bbox[0] - b
-00013940: 626f 785b 335d 290d 0a20 2020 2020 2020  box[3])..       
-00013950: 2020 2020 2073 697a 6579 203d 2061 6273       sizey = abs
-00013960: 2862 626f 785b 315d 202d 2062 626f 785b  (bbox[1] - bbox[
-00013970: 345d 290d 0a20 2020 2020 2020 2020 2020  4])..           
-00013980: 2073 697a 6578 203d 2061 6273 2862 626f   sizex = abs(bbo
-00013990: 785b 325d 202d 2062 626f 785b 355d 2920  x[2] - bbox[5]) 
-000139a0: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
-000139b0: 746f 5f76 6f6c 756d 6520 3d20 7369 7a65  to_volume = size
-000139c0: 7820 2a20 7369 7a65 7920 2a20 7369 7a65  x * sizey * size
-000139d0: 7a0d 0a20 2020 2020 2020 2020 2020 2076  z..            v
-000139e0: 6574 6f5f 7261 6469 7573 203d 206d 6174  eto_radius = mat
-000139f0: 682e 706f 7728 3320 2a20 7665 746f 5f76  h.pow(3 * veto_v
-00013a00: 6f6c 756d 6520 2f20 2834 202a 206d 6174  olume / (4 * mat
-00013a10: 682e 7069 292c 2031 2e30 202f 2033 2e30  h.pi), 1.0 / 3.0
-00013a20: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00013a30: 206c 6f63 6174 696f 6e20 3d20 2863 656e   location = (cen
-00013a40: 7472 6f69 6473 5b69 6e64 6578 5d5b 305d  troids[index][0]
-00013a50: 202a 2073 656c 662e 7a63 616c 6962 7261   * self.zcalibra
-00013a60: 7469 6f6e 2c20 6365 6e74 726f 6964 735b  tion, centroids[
-00013a70: 696e 6465 785d 5b31 5d2a 7365 6c66 2e79  index][1]*self.y
-00013a80: 6361 6c69 6272 6174 696f 6e2c 2063 656e  calibration, cen
-00013a90: 7472 6f69 6473 5b69 6e64 6578 5d5b 325d  troids[index][2]
-00013aa0: 2a73 656c 662e 7863 616c 6962 7261 7469  *self.xcalibrati
-00013ab0: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
-00013ac0: 2051 5541 4c49 5459 203d 206d 6174 682e   QUALITY = math.
-00013ad0: 706f 7728 766f 6c75 6d65 5b69 6e64 6578  pow(volume[index
-00013ae0: 5d2c 2031 2e30 2f33 2e30 290d 0a20 2020  ], 1.0/3.0)..   
-00013af0: 2020 2020 2020 2020 2052 4144 4955 5320           RADIUS 
-00013b00: 3d20 6d61 7468 2e70 6f77 2876 6f6c 756d  = math.pow(volum
-00013b10: 655b 696e 6465 785d 202a 2073 656c 662e  e[index] * self.
-00013b20: 7863 616c 6962 7261 7469 6f6e 202a 2073  xcalibration * s
-00013b30: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-00013b40: 202a 2073 656c 662e 7a63 616c 6962 7261   * self.zcalibra
-00013b50: 7469 6f6e 2c20 312e 302f 332e 3029 200d  tion, 1.0/3.0) .
-00013b60: 0a0d 0a20 2020 2020 2020 2020 2020 2064  ...            d
-00013b70: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00013b80: 6b2c 206d 6173 6b63 656e 7472 6f69 6420  k, maskcentroid 
-00013b90: 3d20 7365 6c66 2e5f 6765 745f 626f 756e  = self._get_boun
-00013ba0: 6461 7279 5f64 6973 7428 6672 616d 652c  dary_dist(frame,
-00013bb0: 206c 6f63 6174 696f 6e29 0d0a 2020 2020   location)..    
-00013bc0: 2020 2020 2020 2020 6966 2064 6973 7420          if dist 
-00013bd0: 3c3d 2032 202a 2076 6574 6f5f 7261 6469  <= 2 * veto_radi
-00013be0: 7573 3a0d 0a20 2020 2020 2020 2020 2020  us:..           
-00013bf0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-00013c00: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-00013c10: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-00013c20: 5d20 3d20 7b0d 0a20 2020 2020 2020 2020  ] = {..         
-00013c30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013c40: 656c 662e 6365 6c6c 6964 5f6b 6579 3a20  elf.cellid_key: 
-00013c50: 696e 7428 6365 6c6c 5f69 6429 2c20 0d0a  int(cell_id), ..
-00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c70: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
-00013c80: 6d65 6964 5f6b 6579 203a 2069 6e74 2866  meid_key : int(f
-00013c90: 7261 6d65 292c 0d0a 2020 2020 2020 2020  rame),..        
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cb0: 7365 6c66 2e7a 706f 7369 645f 6b65 7920  self.zposid_key 
-00013cc0: 3a20 666c 6f61 7428 6365 6e74 726f 6964  : float(centroid
-00013cd0: 735b 696e 6465 785d 5b30 5d2a 2073 656c  s[index][0]* sel
-00013ce0: 662e 7a63 616c 6962 7261 7469 6f6e 292c  f.zcalibration),
-00013cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013d00: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
-00013d10: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-00013d20: 7428 6365 6e74 726f 6964 735b 696e 6465  t(centroids[inde
-00013d30: 785d 5b31 5d2a 2073 656c 662e 7963 616c  x][1]* self.ycal
-00013d40: 6962 7261 7469 6f6e 292c 0d0a 2020 2020  ibration),..    
-00013d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d60: 2020 2020 7365 6c66 2e78 706f 7369 645f      self.xposid_
-00013d70: 6b65 7920 3a20 666c 6f61 7428 6365 6e74  key : float(cent
-00013d80: 726f 6964 735b 696e 6465 785d 5b32 5d2a  roids[index][2]*
-00013d90: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-00013da0: 6f6e 292c 0d0a 2020 2020 2020 2020 2020  on),..          
-00013db0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013dc0: 6c66 2e74 7261 636b 6964 5f6b 6579 3a20  lf.trackid_key: 
-00013dd0: 696e 7428 7472 6163 6b5f 6964 292c 0d0a  int(track_id),..
-00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013df0: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
-00013e00: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-00013e10: 203a 2028 666c 6f61 7428 696e 7465 6e73   : (float(intens
-00013e20: 6974 795f 746f 7461 6c5b 696e 6465 785d  ity_total[index]
-00013e30: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-00013e40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013e50: 662e 6d65 616e 5f69 6e74 656e 7369 7479  f.mean_intensity
-00013e60: 5f6b 6579 203a 2028 666c 6f61 7428 696e  _key : (float(in
-00013e70: 7465 6e73 6974 795f 6d65 616e 5b69 6e64  tensity_mean[ind
-00013e80: 6578 5d29 292c 0d0a 0d0a 2020 2020 2020  ex])),....      
-00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ea0: 2020 7365 6c66 2e72 6164 6975 735f 6b65    self.radius_ke
-00013eb0: 7920 3a20 2866 6c6f 6174 2852 4144 4955  y : (float(RADIU
-00013ec0: 5329 292c 0d0a 2020 2020 2020 2020 2020  S)),..          
-00013ed0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013ee0: 6c66 2e71 7561 6c69 7479 5f6b 6579 203a  lf.quality_key :
-00013ef0: 2028 666c 6f61 7428 5155 414c 4954 5929   (float(QUALITY)
-00013f00: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00013f10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013f20: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
-00013f30: 6173 6b5f 6b65 793a 2066 6c6f 6174 2864  ask_key: float(d
-00013f40: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00013f50: 6b29 2c0d 0a20 2020 2020 2020 2020 2020  k),..           
-00013f60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013f70: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
-00013f80: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
-00013f90: 6365 6e74 726f 6964 5b30 5d29 2c0d 0a20  centroid[0]),.. 
-00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fb0: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
-00013fc0: 6365 6e74 726f 6964 5f79 5f6b 6579 3a20  centroid_y_key: 
-00013fd0: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
-00013fe0: 6964 5b31 5d29 2c0d 0a20 2020 2020 2020  id[1]),..       
+00012b20: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012b30: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+00012b40: 5f63 6f6d 705f 6669 7273 742e 6170 7065  _comp_first.appe
+00012b50: 6e64 2865 6363 656e 7472 6963 6974 795f  nd(eccentricity_
+00012b60: 636f 6d70 5f66 6972 7374 5b6a 5d29 0d0a  comp_first[j])..
+00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b90: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+00012ba0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+00012bb0: 642e 6170 7065 6e64 2865 6363 656e 7472  d.append(eccentr
+00012bc0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+00012bd0: 645b 6a5d 290d 0a20 2020 2020 2020 2020  d[j])..         
+00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bf0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012c00: 7375 7266 6163 655f 6172 6561 2e61 7070  surface_area.app
+00012c10: 656e 6428 7375 7266 6163 655f 6172 6561  end(surface_area
+00012c20: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c40: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
+00012c50: 6164 6961 6c5f 616e 676c 652e 6170 7065  adial_angle.appe
+00012c60: 6e64 2872 6164 6961 6c5f 616e 676c 655b  nd(radial_angle[
+00012c70: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c90: 2020 2020 2020 6375 7272 656e 745f 6365        current_ce
+00012ca0: 6c6c 5f61 7869 735f 6d61 736b 2e61 7070  ll_axis_mask.app
+00012cb0: 656e 6428 6365 6c6c 5f61 7869 735f 6d61  end(cell_axis_ma
+00012cc0: 736b 5b6a 5d29 0d0a 2020 2020 2020 2020  sk[j])..        
+00012cd0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012ce0: 6e74 5f74 696d 6520 3d20 6e70 2e61 7361  nt_time = np.asa
+00012cf0: 7272 6179 2863 7572 7265 6e74 5f74 696d  rray(current_tim
+00012d00: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
+00012d10: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+00012d20: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012d30: 5f69 6e74 656e 7369 7479 203d 206e 702e  _intensity = np.
+00012d40: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00012d50: 696e 7465 6e73 6974 792c 2064 7479 7065  intensity, dtype
+00012d60: 3d6e 702e 666c 6f61 7433 3229 0d0a 0d0a  =np.float32)....
+00012d70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012d80: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
+00012d90: 7374 6572 5f63 6c61 7373 203d 206e 702e  ster_class = np.
+00012da0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00012db0: 636c 7573 7465 725f 636c 6173 732c 2064  cluster_class, d
+00012dc0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00012dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012de0: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
+00012df0: 7374 6572 5f63 6c61 7373 5f73 636f 7265  ster_class_score
+00012e00: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+00012e10: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
+00012e20: 6173 735f 7363 6f72 652c 2064 7479 7065  ass_score, dtype
+00012e30: 3d6e 702e 666c 6f61 7433 3229 2020 200d  =np.float32)   .
+00012e40: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00012e50: 2020 2020 2020 6375 7272 656e 745f 7261        current_ra
+00012e60: 6469 7573 203d 206e 702e 6173 6172 7261  dius = np.asarra
+00012e70: 7928 6375 7272 656e 745f 7261 6469 7573  y(current_radius
+00012e80: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00012e90: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
+00012ea0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012eb0: 766f 6c75 6d65 203d 206e 702e 6173 6172  volume = np.asar
+00012ec0: 7261 7928 6375 7272 656e 745f 766f 6c75  ray(current_volu
+00012ed0: 6d65 2c20 6474 7970 653d 6e70 2e66 6c6f  me, dtype=np.flo
+00012ee0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00012ef0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012f00: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00012f10: 6f6d 705f 6669 7273 7420 3d20 6e70 2e61  omp_first = np.a
+00012f20: 7361 7272 6179 2863 7572 7265 6e74 5f65  sarray(current_e
+00012f30: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00012f40: 5f66 6972 7374 2c20 6474 7970 653d 6e70  _first, dtype=np
+00012f50: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
+00012f60: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012f70: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+00012f80: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
+00012f90: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+00012fa0: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+00012fb0: 5f63 6f6d 705f 7365 636f 6e64 2c20 6474  _comp_second, dt
+00012fc0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+00012fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012fe0: 2020 2020 6375 7272 656e 745f 7375 7266      current_surf
+00012ff0: 6163 655f 6172 6561 203d 206e 702e 6173  ace_area = np.as
+00013000: 6172 7261 7928 6375 7272 656e 745f 7375  array(current_su
+00013010: 7266 6163 655f 6172 6561 2c20 6474 7970  rface_area, dtyp
+00013020: 653d 6e70 2e66 6c6f 6174 3332 290d 0a0d  e=np.float32)...
+00013030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013040: 2020 2020 6375 7272 656e 745f 7370 6565      current_spee
+00013050: 6420 3d20 6e70 2e61 7361 7272 6179 2863  d = np.asarray(c
+00013060: 7572 7265 6e74 5f73 7065 6564 2c20 6474  urrent_speed, dt
+00013070: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+00013080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013090: 2020 2020 6375 7272 656e 745f 6d6f 7469      current_moti
+000130a0: 6f6e 5f61 6e67 6c65 203d 206e 702e 6173  on_angle = np.as
+000130b0: 6172 7261 7928 6375 7272 656e 745f 6d6f  array(current_mo
+000130c0: 7469 6f6e 5f61 6e67 6c65 2c20 6474 7970  tion_angle, dtyp
+000130d0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
+000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130f0: 2020 6375 7272 656e 745f 6163 6365 6c65    current_accele
+00013100: 7261 7469 6f6e 203d 206e 702e 6173 6172  ration = np.asar
+00013110: 7261 7928 6375 7272 656e 745f 6163 6365  ray(current_acce
+00013120: 6c65 7261 7469 6f6e 2c20 6474 7970 653d  leration, dtype=
+00013130: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
+00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013150: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
+00013160: 5f63 656c 6c5f 6d61 736b 203d 206e 702e  _cell_mask = np.
+00013170: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00013180: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00013190: 736b 2c20 6474 7970 653d 6e70 2e66 6c6f  sk, dtype=np.flo
+000131a0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+000131b0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000131c0: 745f 7261 6469 616c 5f61 6e67 6c65 203d  t_radial_angle =
+000131d0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+000131e0: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
+000131f0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00013200: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
+00013210: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013220: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
+00013230: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+00013240: 656e 745f 6365 6c6c 5f61 7869 735f 6d61  ent_cell_axis_ma
+00013250: 736b 2c20 6474 7970 653d 6e70 2e66 6c6f  sk, dtype=np.flo
+00013260: 6174 3332 290d 0a0d 0a0d 0a20 2020 2020  at32)......     
+00013270: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013290: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000132a0: 2020 2020 2020 2020 6966 2070 6f69 6e74          if point
+000132b0: 5f73 616d 706c 6520 3e20 303a 0d0a 2020  _sample > 0:..  
+000132c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132d0: 2020 2020 2020 2020 2020 2020 2020 7866                xf
+000132e0: 5f73 616d 706c 6520 3d20 6666 7466 7265  _sample = fftfre
+000132f0: 7128 706f 696e 745f 7361 6d70 6c65 2c20  q(point_sample, 
+00013300: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
+00013310: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013330: 2020 2020 6666 7473 7472 6970 5f73 616d      fftstrip_sam
+00013340: 706c 6520 3d20 6666 7428 6578 7061 6e64  ple = fft(expand
+00013350: 6564 5f69 6e74 656e 7369 7479 290d 0a20  ed_intensity).. 
+00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013370: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013380: 6674 746f 7461 6c5f 7361 6d70 6c65 203d  fttotal_sample =
+00013390: 206e 702e 6162 7328 6666 7473 7472 6970   np.abs(fftstrip
+000133a0: 5f73 616d 706c 6529 0d0a 2020 2020 2020  _sample)..      
+000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133c0: 2020 2020 2020 2020 2020 7866 5f73 616d            xf_sam
+000133d0: 706c 6520 3d20 7866 5f73 616d 706c 655b  ple = xf_sample[
+000133e0: 3020 3a20 6c65 6e28 7866 5f73 616d 706c  0 : len(xf_sampl
+000133f0: 6529 202f 2f20 325d 0d0a 2020 2020 2020  e) // 2]..      
+00013400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013410: 2020 2020 2020 2020 2020 6666 7474 6f74            ffttot
+00013420: 616c 5f73 616d 706c 6520 3d20 6666 7474  al_sample = fftt
+00013430: 6f74 616c 5f73 616d 706c 655b 3020 3a20  otal_sample[0 : 
+00013440: 6c65 6e28 6666 7474 6f74 616c 5f73 616d  len(ffttotal_sam
+00013450: 706c 6529 202f 2f20 325d 0d0a 0d0a 2020  ple) // 2]....  
+00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013470: 2075 6e69 7175 655f 6666 745f 7072 6f70   unique_fft_prop
+00013480: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
+00013490: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+000134a0: 645d 203d 2065 7870 616e 6465 645f 7469  d] = expanded_ti
+000134b0: 6d65 2c20 6578 7061 6e64 6564 5f69 6e74  me, expanded_int
+000134c0: 656e 7369 7479 2c20 7866 5f73 616d 706c  ensity, xf_sampl
+000134d0: 652c 2066 6674 746f 7461 6c5f 7361 6d70  e, ffttotal_samp
+000134e0: 6c65 0d0a 2020 2020 2020 2020 2020 2020  le..            
+000134f0: 2020 2020 2020 2075 6e69 7175 655f 636c         unique_cl
+00013500: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+00013510: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
+00013520: 745f 756e 6971 7565 5f69 645d 203d 2020  t_unique_id] =  
+00013530: 6375 7272 656e 745f 7469 6d65 2c20 6375  current_time, cu
+00013540: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
+00013550: 6173 732c 2063 7572 7265 6e74 5f63 6c75  ass, current_clu
+00013560: 7374 6572 5f63 6c61 7373 5f73 636f 7265  ster_class_score
+00013570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013580: 2020 2020 2075 6e69 7175 655f 7368 6170       unique_shap
+00013590: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
+000135a0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+000135b0: 6971 7565 5f69 645d 203d 2063 7572 7265  ique_id] = curre
+000135c0: 6e74 5f74 696d 652c 2063 7572 7265 6e74  nt_time, current
+000135d0: 5f7a 2c20 6375 7272 656e 745f 792c 2063  _z, current_y, c
+000135e0: 7572 7265 6e74 5f78 2c20 6375 7272 656e  urrent_x, curren
+000135f0: 745f 7261 6469 7573 2c20 6375 7272 656e  t_radius, curren
+00013600: 745f 766f 6c75 6d65 2c20 6375 7272 656e  t_volume, curren
+00013610: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00013620: 6f6d 705f 6669 7273 742c 2063 7572 7265  omp_first, curre
+00013630: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
+00013640: 636f 6d70 5f73 6563 6f6e 642c 2063 7572  comp_second, cur
+00013650: 7265 6e74 5f73 7572 6661 6365 5f61 7265  rent_surface_are
+00013660: 612c 2063 7572 7265 6e74 5f63 6c75 7374  a, current_clust
+00013670: 6572 5f63 6c61 7373 2c20 6375 7272 656e  er_class, curren
+00013680: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
+00013690: 7363 6f72 650d 0a20 2020 2020 2020 2020  score..         
+000136a0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+000136b0: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
+000136c0: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+000136d0: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
+000136e0: 3d20 6375 7272 656e 745f 7469 6d65 2c20  = current_time, 
+000136f0: 6375 7272 656e 745f 7370 6565 642c 2063  current_speed, c
+00013700: 7572 7265 6e74 5f6d 6f74 696f 6e5f 616e  urrent_motion_an
+00013710: 676c 652c 2063 7572 7265 6e74 5f61 6363  gle, current_acc
+00013720: 656c 6572 6174 696f 6e2c 2063 7572 7265  eleration, curre
+00013730: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
+00013740: 5f6d 6173 6b2c 2063 7572 7265 6e74 5f72  _mask, current_r
+00013750: 6164 6961 6c5f 616e 676c 652c 2063 7572  adial_angle, cur
+00013760: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
+00013770: 6173 6b0d 0a20 2020 2020 2020 2020 2020  ask..           
+00013780: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00013790: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
+000137a0: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
+000137b0: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
+000137c0: 7175 655f 6964 3a75 6e69 7175 655f 6666  que_id:unique_ff
+000137d0: 745f 7072 6f70 6572 7469 6573 5f74 7261  t_properties_tra
+000137e0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+000137f0: 6971 7565 5f69 645d 7d29 0d0a 2020 2020  ique_id]})..    
+00013800: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013810: 656c 662e 756e 6971 7565 5f63 6c75 7374  elf.unique_clust
+00013820: 6572 5f70 726f 7065 7274 6965 735b 7472  er_properties[tr
+00013830: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
+00013840: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00013850: 643a 756e 6971 7565 5f63 6c75 7374 6572  d:unique_cluster
+00013860: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00013870: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+00013880: 7175 655f 6964 5d7d 290d 0a0d 0a20 2020  que_id]})....   
+00013890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138a0: 7365 6c66 2e75 6e69 7175 655f 7368 6170  self.unique_shap
+000138b0: 655f 7072 6f70 6572 7469 6573 5b74 7261  e_properties[tra
+000138c0: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
+000138d0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+000138e0: 3a75 6e69 7175 655f 7368 6170 655f 7072  :unique_shape_pr
+000138f0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00013900: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
+00013910: 5f69 645d 7d29 0d0a 2020 2020 2020 2020  _id]})..        
+00013920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013930: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
+00013940: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
+00013950: 6964 5d2e 7570 6461 7465 287b 6375 7272  id].update({curr
+00013960: 656e 745f 756e 6971 7565 5f69 643a 756e  ent_unique_id:un
+00013970: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
+00013980: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00013990: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
+000139a0: 6964 5d7d 290d 0a0d 0a20 2020 2064 6566  id]})....    def
+000139b0: 205f 7365 636f 6e64 5f63 6861 6e6e 656c   _second_channel
+000139c0: 5f73 706f 7473 2873 656c 662c 2066 7261  _spots(self, fra
+000139d0: 6d65 2c20 7a2c 2079 2c20 782c 2063 656c  me, z, y, x, cel
+000139e0: 6c5f 6964 2c20 7472 6163 6b5f 6964 293a  l_id, track_id):
+000139f0: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
+00013a00: 2020 2020 2020 2020 2020 2074 7265 652c             tree,
+00013a10: 2063 656e 7472 6f69 6473 2c20 6c61 6265   centroids, labe
+00013a20: 6c73 2c20 766f 6c75 6d65 2c20 696e 7465  ls, volume, inte
+00013a30: 6e73 6974 795f 6d65 616e 2c20 696e 7465  nsity_mean, inte
+00013a40: 6e73 6974 795f 746f 7461 6c2c 2062 6f75  nsity_total, bou
+00013a50: 6e64 696e 675f 626f 7865 7320 3d20 7365  nding_boxes = se
+00013a60: 6c66 2e5f 7469 6d65 645f 6368 616e 6e65  lf._timed_channe
+00013a70: 6c5f 7365 675f 696d 6167 655b 7374 7228  l_seg_image[str(
+00013a80: 696e 7428 666c 6f61 7428 6672 616d 6529  int(float(frame)
+00013a90: 2929 5d0d 0a20 2020 2020 2020 2020 2020  ))]..           
+00013aa0: 2070 6978 656c 7465 7374 6c6f 6361 7469   pixeltestlocati
+00013ab0: 6f6e 203d 2028 7a2c 792c 7829 0d0a 2020  on = (z,y,x)..  
+00013ac0: 2020 2020 2020 2020 2020 6469 7374 2c20            dist, 
+00013ad0: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
+00013ae0: 7279 2870 6978 656c 7465 7374 6c6f 6361  ry(pixeltestloca
+00013af0: 7469 6f6e 290d 0a0d 0a0d 0a20 2020 2020  tion)......     
+00013b00: 2020 2020 2020 2062 626f 7820 3d20 626f         bbox = bo
+00013b10: 756e 6469 6e67 5f62 6f78 6573 5b69 6e64  unding_boxes[ind
+00013b20: 6578 5d0d 0a20 2020 2020 2020 2020 2020  ex]..           
+00013b30: 2073 697a 657a 203d 2061 6273 2862 626f   sizez = abs(bbo
+00013b40: 785b 305d 202d 2062 626f 785b 335d 290d  x[0] - bbox[3]).
+00013b50: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00013b60: 6579 203d 2061 6273 2862 626f 785b 315d  ey = abs(bbox[1]
+00013b70: 202d 2062 626f 785b 345d 290d 0a20 2020   - bbox[4])..   
+00013b80: 2020 2020 2020 2020 2073 697a 6578 203d           sizex =
+00013b90: 2061 6273 2862 626f 785b 325d 202d 2062   abs(bbox[2] - b
+00013ba0: 626f 785b 355d 2920 0d0a 2020 2020 2020  box[5]) ..      
+00013bb0: 2020 2020 2020 7665 746f 5f76 6f6c 756d        veto_volum
+00013bc0: 6520 3d20 7369 7a65 7820 2a20 7369 7a65  e = sizex * size
+00013bd0: 7920 2a20 7369 7a65 7a0d 0a20 2020 2020  y * sizez..     
+00013be0: 2020 2020 2020 2076 6574 6f5f 7261 6469         veto_radi
+00013bf0: 7573 203d 206d 6174 682e 706f 7728 3320  us = math.pow(3 
+00013c00: 2a20 7665 746f 5f76 6f6c 756d 6520 2f20  * veto_volume / 
+00013c10: 2834 202a 206d 6174 682e 7069 292c 2031  (4 * math.pi), 1
+00013c20: 2e30 202f 2033 2e30 290d 0a0d 0a20 2020  .0 / 3.0)....   
+00013c30: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
+00013c40: 6e20 3d20 2863 656e 7472 6f69 6473 5b69  n = (centroids[i
+00013c50: 6e64 6578 5d5b 305d 202a 2073 656c 662e  ndex][0] * self.
+00013c60: 7a63 616c 6962 7261 7469 6f6e 2c20 6365  zcalibration, ce
+00013c70: 6e74 726f 6964 735b 696e 6465 785d 5b31  ntroids[index][1
+00013c80: 5d2a 7365 6c66 2e79 6361 6c69 6272 6174  ]*self.ycalibrat
+00013c90: 696f 6e2c 2063 656e 7472 6f69 6473 5b69  ion, centroids[i
+00013ca0: 6e64 6578 5d5b 325d 2a73 656c 662e 7863  ndex][2]*self.xc
+00013cb0: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
+00013cc0: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
+00013cd0: 203d 206d 6174 682e 706f 7728 766f 6c75   = math.pow(volu
+00013ce0: 6d65 5b69 6e64 6578 5d2c 2031 2e30 2f33  me[index], 1.0/3
+00013cf0: 2e30 290d 0a20 2020 2020 2020 2020 2020  .0)..           
+00013d00: 2052 4144 4955 5320 3d20 6d61 7468 2e70   RADIUS = math.p
+00013d10: 6f77 2876 6f6c 756d 655b 696e 6465 785d  ow(volume[index]
+00013d20: 202a 2073 656c 662e 7863 616c 6962 7261   * self.xcalibra
+00013d30: 7469 6f6e 202a 2073 656c 662e 7963 616c  tion * self.ycal
+00013d40: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
+00013d50: 7a63 616c 6962 7261 7469 6f6e 2c20 312e  zcalibration, 1.
+00013d60: 302f 332e 3029 200d 0a0d 0a20 2020 2020  0/3.0) ....     
+00013d70: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
+00013d80: 6365 6c6c 5f6d 6173 6b2c 206d 6173 6b63  cell_mask, maskc
+00013d90: 656e 7472 6f69 6420 3d20 7365 6c66 2e5f  entroid = self._
+00013da0: 6765 745f 626f 756e 6461 7279 5f64 6973  get_boundary_dis
+00013db0: 7428 6672 616d 652c 206c 6f63 6174 696f  t(frame, locatio
+00013dc0: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00013dd0: 6966 2064 6973 7420 3c3d 2032 202a 2076  if dist <= 2 * v
+00013de0: 6574 6f5f 7261 6469 7573 3a0d 0a20 2020  eto_radius:..   
+00013df0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013e00: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+00013e10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00013e20: 5b63 656c 6c5f 6964 5d20 3d20 7b0d 0a20  [cell_id] = {.. 
+00013e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e40: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
+00013e50: 6964 5f6b 6579 3a20 696e 7428 6365 6c6c  id_key: int(cell
+00013e60: 5f69 6429 2c20 0d0a 2020 2020 2020 2020  _id), ..        
+00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e80: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
+00013e90: 203a 2069 6e74 2866 7261 6d65 292c 0d0a   : int(frame),..
+00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013eb0: 2020 2020 2020 2020 7365 6c66 2e7a 706f          self.zpo
+00013ec0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+00013ed0: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
+00013ee0: 5b30 5d2a 2073 656c 662e 7a63 616c 6962  [0]* self.zcalib
+00013ef0: 7261 7469 6f6e 292c 0d0a 2020 2020 2020  ration),..      
+00013f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f10: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
+00013f20: 7920 3a20 666c 6f61 7428 6365 6e74 726f  y : float(centro
+00013f30: 6964 735b 696e 6465 785d 5b31 5d2a 2073  ids[index][1]* s
+00013f40: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+00013f50: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00013f60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013f70: 2e78 706f 7369 645f 6b65 7920 3a20 666c  .xposid_key : fl
+00013f80: 6f61 7428 6365 6e74 726f 6964 735b 696e  oat(centroids[in
+00013f90: 6465 785d 5b32 5d2a 2073 656c 662e 7863  dex][2]* self.xc
+00013fa0: 616c 6962 7261 7469 6f6e 292c 0d0a 2020  alibration),..  
+00013fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fc0: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+00013fd0: 6964 5f6b 6579 3a20 696e 7428 7472 6163  id_key: int(trac
+00013fe0: 6b5f 6964 292c 0d0a 2020 2020 2020 2020  k_id),..        
 00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014000: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
-00014010: 6964 5f78 5f6b 6579 3a20 666c 6f61 7428  id_x_key: float(
-00014020: 6d61 736b 6365 6e74 726f 6964 5b32 5d29  maskcentroid[2])
-00014030: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00014040: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00014050: 2020 2020 656c 6966 2063 656c 6c5f 6964      elif cell_id
-00014060: 2069 6e20 7365 6c66 2e65 6467 655f 736f   in self.edge_so
-00014070: 7572 6365 5f6c 6f6f 6b75 702e 6b65 7973  urce_lookup.keys
-00014080: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00014090: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000140a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000140b0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-000140c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000140d0: 6573 5b63 656c 6c5f 6964 5d20 3d20 7365  es[cell_id] = se
-000140e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000140f0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-00014100: 645d 0d0a 0d0a 2020 2020 2020 2020 2020  d]....          
-00014110: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00014120: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-00014130: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-00014140: 6c6c 5f69 645d 2e75 7064 6174 6528 7b73  ll_id].update({s
-00014150: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-00014160: 6974 795f 6b65 793a 202d 317d 290d 0a20  ity_key: -1}).. 
-00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014180: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
-00014190: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000141a0: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
-000141b0: 7570 6461 7465 287b 7365 6c66 2e6d 6561  update({self.mea
-000141c0: 6e5f 696e 7465 6e73 6974 795f 6b65 793a  n_intensity_key:
-000141d0: 202d 317d 290d 0a20 2020 2020 2020 2020   -1})..         
-000141e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000141f0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-00014200: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-00014210: 656c 6c5f 6964 5d2e 7570 6461 7465 287b  ell_id].update({
-00014220: 7365 6c66 2e72 6164 6975 735f 6b65 793a  self.radius_key:
-00014230: 202d 317d 290d 0a20 2020 2020 2020 2020   -1})..         
-00014240: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014250: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-00014260: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-00014270: 656c 6c5f 6964 5d2e 7570 6461 7465 287b  ell_id].update({
-00014280: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-00014290: 3a20 2d31 7d29 0d0a 0d0a 0d0a 2020 2020  : -1})......    
-000142a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000142c0: 2020 2064 6566 205f 6469 6374 5f75 7064     def _dict_upd
-000142d0: 6174 6528 7365 6c66 2c20 756e 6971 7565  ate(self, unique
-000142e0: 5f74 7261 636b 6c65 745f 6964 733a 204c  _tracklet_ids: L
-000142f0: 6973 742c 2020 6365 6c6c 5f69 643a 2069  ist,  cell_id: i
-00014300: 6e74 2c20 7472 6163 6b5f 6964 3a20 696e  nt, track_id: in
-00014310: 742c 2073 6f75 7263 655f 6964 3a20 696e  t, source_id: in
-00014320: 742c 2074 6172 6765 745f 6964 3a20 696e  t, target_id: in
-00014330: 7429 3a0d 0a0d 0a20 0d0a 2020 2020 2020  t):.... ..      
-00014340: 2020 6765 6e65 7261 7469 6f6e 5f69 6420    generation_id 
-00014350: 3d20 7365 6c66 2e67 656e 6572 6174 696f  = self.generatio
-00014360: 6e5f 6469 6374 5b63 656c 6c5f 6964 5d0d  n_dict[cell_id].
-00014370: 0a20 2020 2020 2020 2074 7261 636b 6c65  .        trackle
-00014380: 745f 6964 203d 2073 656c 662e 7472 6163  t_id = self.trac
-00014390: 6b6c 6574 5f64 6963 745b 6365 6c6c 5f69  klet_dict[cell_i
-000143a0: 645d 0d0a 0d0a 2020 2020 2020 2020 756e  d]....        un
-000143b0: 6971 7565 5f69 6420 3d20 7374 7228 7472  ique_id = str(tr
-000143c0: 6163 6b5f 6964 2920 2b20 7374 7228 7365  ack_id) + str(se
-000143d0: 6c66 2e6d 6178 5f74 7261 636b 5f69 6429  lf.max_track_id)
-000143e0: 202b 2073 7472 2867 656e 6572 6174 696f   + str(generatio
-000143f0: 6e5f 6964 2920 2b20 7374 7228 7472 6163  n_id) + str(trac
-00014400: 6b6c 6574 5f69 6429 0d0a 2020 2020 2020  klet_id)..      
-00014410: 2020 0d0a 2020 2020 2020 2020 7665 635f    ..        vec_
-00014420: 6d61 736b 203d 205b 666c 6f61 7428 7365  mask = [float(se
-00014430: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014440: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014450: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
-00014460: 6b63 656e 7472 6f69 645f 785f 6b65 795d  kcentroid_x_key]
-00014470: 292c 2066 6c6f 6174 2873 656c 662e 756e  ), float(self.un
-00014480: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014490: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-000144a0: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
-000144b0: 726f 6964 5f79 5f6b 6579 5d29 2c20 666c  roid_y_key]), fl
-000144c0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-000144d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000144e0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
-000144f0: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-00014500: 7a5f 6b65 795d 2920 5d0d 0a0d 0a20 2020  z_key]) ]....   
-00014510: 2020 2020 2076 6563 5f63 656c 6c20 3d20       vec_cell = 
-00014520: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
-00014530: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014540: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014550: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00014560: 5d29 202c 200d 0a20 2020 2020 2020 2020  ]) , ..         
-00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014580: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
-00014590: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000145a0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-000145b0: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
-000145c0: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
-000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145e0: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-000145f0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014600: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014610: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
-00014620: 6b65 795d 295d 0d0a 0d0a 2020 2020 2020  key])]....      
-00014630: 2020 616e 676c 6520 3d20 616e 6775 6c61    angle = angula
-00014640: 725f 6368 616e 6765 2876 6563 5f6d 6173  r_change(vec_mas
-00014650: 6b2c 2076 6563 5f63 656c 6c29 0d0a 0d0a  k, vec_cell)....
-00014660: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00014670: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014680: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014690: 5d2e 7570 6461 7465 287b 7365 6c66 2e72  ].update({self.r
-000146a0: 6164 6961 6c5f 616e 676c 655f 6b65 7920  adial_angle_key 
-000146b0: 3a20 616e 676c 657d 2920 2020 2020 2020  : angle})       
-000146c0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-000146d0: 0a20 2020 2020 2020 2075 6e69 7175 655f  .        unique_
-000146e0: 7472 6163 6b6c 6574 5f69 6473 2e61 7070  tracklet_ids.app
-000146f0: 656e 6428 7374 7228 756e 6971 7565 5f69  end(str(unique_i
-00014700: 6429 290d 0a20 2020 2020 2020 2073 656c  d))..        sel
-00014710: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014720: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014730: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00014740: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-00014750: 5f6b 6579 203a 202d 317d 290d 0a20 2020  _key : -1})..   
-00014760: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00014770: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014780: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00014790: 7064 6174 6528 7b73 656c 662e 636c 7573  pdate({self.clus
-000147a0: 7465 7273 636f 7265 5f6b 6579 203a 2030  terscore_key : 0
-000147b0: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
-000147c0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000147d0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000147e0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-000147f0: 6c66 2e75 6e69 7175 6569 645f 6b65 7920  lf.uniqueid_key 
-00014800: 3a20 7374 7228 756e 6971 7565 5f69 6429  : str(unique_id)
-00014810: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
-00014820: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014830: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014840: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00014850: 6c66 2e74 7261 636b 6c65 7469 645f 6b65  lf.trackletid_ke
-00014860: 7920 3a20 7374 7228 7472 6163 6b6c 6574  y : str(tracklet
-00014870: 5f69 6429 7d29 200d 0a20 2020 2020 2020  _id)}) ..       
-00014880: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014890: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000148a0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-000148b0: 6528 7b73 656c 662e 6765 6e65 7261 7469  e({self.generati
-000148c0: 6f6e 6964 5f6b 6579 203a 2073 7472 2867  onid_key : str(g
-000148d0: 656e 6572 6174 696f 6e5f 6964 297d 2920  eneration_id)}) 
-000148e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-000148f0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014900: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014910: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00014920: 2e74 7261 636b 6964 5f6b 6579 203a 2073  .trackid_key : s
-00014930: 7472 2874 7261 636b 5f69 6429 7d29 0d0a  tr(track_id)})..
-00014940: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00014950: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014960: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014970: 5d2e 7570 6461 7465 287b 7365 6c66 2e6d  ].update({self.m
-00014980: 6f74 696f 6e5f 616e 676c 655f 6b65 7920  otion_angle_key 
-00014990: 3a20 302e 307d 290d 0a20 2020 2020 2020  : 0.0})..       
-000149a0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000149b0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000149c0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-000149d0: 6528 7b73 656c 662e 7370 6565 645f 6b65  e({self.speed_ke
-000149e0: 7920 3a20 302e 307d 290d 0a20 2020 2020  y : 0.0})..     
-000149f0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00014a00: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014a10: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00014a20: 6174 6528 7b73 656c 662e 6163 6365 6c65  ate({self.accele
-00014a30: 7261 7469 6f6e 5f6b 6579 203a 2030 2e30  ration_key : 0.0
-00014a40: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
-00014a50: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014a60: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014a70: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00014a80: 6c66 2e65 6363 656e 7472 6963 6974 795f  lf.eccentricity_
-00014a90: 636f 6d70 5f66 6972 7374 6b65 7920 3a20  comp_firstkey : 
-00014aa0: 2d31 7d29 0d0a 2020 2020 2020 2020 7365  -1})..        se
-00014ab0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014ac0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014ad0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00014ae0: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-00014af0: 795f 636f 6d70 5f73 6563 6f6e 646b 6579  y_comp_secondkey
-00014b00: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
-00014b10: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014b20: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014b30: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00014b40: 6528 7b73 656c 662e 7375 7266 6163 655f  e({self.surface_
-00014b50: 6172 6561 5f6b 6579 203a 202d 317d 290d  area_key : -1}).
-00014b60: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00014b70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014b80: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014b90: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014ba0: 6365 6c6c 6178 6973 5f6d 6173 6b5f 6b65  cellaxis_mask_ke
-00014bb0: 7920 3a20 2d31 7d29 0d0a 0d0a 2020 2020  y : -1})....    
-00014bc0: 2020 2020 6966 2073 6f75 7263 655f 6964      if source_id
-00014bd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00014be0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014bf0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014c00: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014c10: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00014c20: 662e 6265 666f 7265 6964 5f6b 6579 203a  f.beforeid_key :
-00014c30: 2069 6e74 2873 6f75 7263 655f 6964 297d   int(source_id)}
-00014c40: 290d 0a20 2020 2020 2020 2020 2020 2076  )..            v
-00014c50: 6563 5f31 203d 205b 666c 6f61 7428 7365  ec_1 = [float(se
-00014c60: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014c70: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014c80: 6c6c 5f69 6429 5d5b 7365 6c66 2e78 706f  ll_id)][self.xpo
-00014c90: 7369 645f 6b65 795d 2920 2d20 666c 6f61  sid_key]) - floa
-00014ca0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00014cb0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014cc0: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
-00014cd0: 6c66 2e78 706f 7369 645f 6b65 795d 292c  lf.xposid_key]),
-00014ce0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00014cf0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00014d00: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00014d10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014d20: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00014d30: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-00014d40: 202d 2066 6c6f 6174 2873 656c 662e 756e   - float(self.un
-00014d50: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014d60: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
-00014d70: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
-00014d80: 5f6b 6579 5d29 2c20 0d0a 2020 2020 2020  _key]), ..      
-00014d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014da0: 2020 2020 2020 666c 6f61 7428 7365 6c66        float(self
-00014db0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014dc0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014dd0: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
-00014de0: 645f 6b65 795d 2920 2d20 2066 6c6f 6174  d_key]) -  float
-00014df0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00014e00: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014e10: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
-00014e20: 662e 7a70 6f73 6964 5f6b 6579 5d29 5d0d  f.zposid_key])].
-00014e30: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
-00014e40: 6564 203d 206e 702e 7371 7274 286e 702e  ed = np.sqrt(np.
-00014e50: 646f 7428 7665 635f 312c 2076 6563 5f31  dot(vec_1, vec_1
-00014e60: 2929 2f73 656c 662e 7463 616c 6962 7261  ))/self.tcalibra
-00014e70: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00014e80: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014e90: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014ea0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00014eb0: 7465 287b 7365 6c66 2e73 7065 6564 5f6b  te({self.speed_k
-00014ec0: 6579 203a 2073 7065 6564 7d29 0d0a 0d0a  ey : speed})....
-00014ed0: 2020 2020 2020 2020 2020 2020 6d6f 7469              moti
-00014ee0: 6f6e 5f61 6e67 6c65 203d 2061 6e67 756c  on_angle = angul
-00014ef0: 6172 5f63 6861 6e67 6528 7665 635f 6d61  ar_change(vec_ma
-00014f00: 736b 2c20 7665 635f 3129 0d0a 0d0a 2020  sk, vec_1)....  
-00014f10: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00014f20: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014f30: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014f40: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00014f50: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
-00014f60: 7920 3a20 6d6f 7469 6f6e 5f61 6e67 6c65  y : motion_angle
-00014f70: 7d29 200d 0a0d 0a20 2020 2020 2020 2020  }) ....         
-00014f80: 2020 2069 6620 736f 7572 6365 5f69 6420     if source_id 
-00014f90: 696e 2073 656c 662e 6564 6765 5f73 6f75  in self.edge_sou
-00014fa0: 7263 655f 6c6f 6f6b 7570 3a0d 0a20 2020  rce_lookup:..   
-00014fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fc0: 2070 7265 5f73 6f75 7263 655f 6964 203d   pre_source_id =
-00014fd0: 2073 656c 662e 6564 6765 5f73 6f75 7263   self.edge_sourc
-00014fe0: 655f 6c6f 6f6b 7570 5b73 6f75 7263 655f  e_lookup[source_
-00014ff0: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
-00015000: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00015010: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00015020: 6563 5f32 203d 205b 666c 6f61 7428 7365  ec_2 = [float(se
-00015030: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015040: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015050: 6c6c 5f69 6429 5d5b 7365 6c66 2e78 706f  ll_id)][self.xpo
-00015060: 7369 645f 6b65 795d 2920 2d20 3220 2a20  sid_key]) - 2 * 
-00015070: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00015080: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015090: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
-000150a0: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-000150b0: 795d 2920 2b20 666c 6f61 7428 7365 6c66  y]) + float(self
-000150c0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000150d0: 7065 7274 6965 735b 696e 7428 7072 655f  perties[int(pre_
-000150e0: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-000150f0: 2e78 706f 7369 645f 6b65 795d 292c 200d  .xposid_key]), .
-00015100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015110: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-00015120: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00015130: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015140: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00015150: 662e 7970 6f73 6964 5f6b 6579 5d29 202d  f.yposid_key]) -
-00015160: 2032 202a 2066 6c6f 6174 2873 656c 662e   2 * float(self.
-00015170: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015180: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00015190: 655f 6964 295d 5b73 656c 662e 7970 6f73  e_id)][self.ypos
-000151a0: 6964 5f6b 6579 5d29 202b 2066 6c6f 6174  id_key]) + float
-000151b0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-000151c0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000151d0: 2870 7265 5f73 6f75 7263 655f 6964 295d  (pre_source_id)]
-000151e0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-000151f0: 5d29 2c20 0d0a 2020 2020 2020 2020 2020  ]), ..          
+00014000: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+00014010: 7369 7479 5f6b 6579 203a 2028 666c 6f61  sity_key : (floa
+00014020: 7428 696e 7465 6e73 6974 795f 746f 7461  t(intensity_tota
+00014030: 6c5b 696e 6465 785d 2929 2c0d 0a20 2020  l[index])),..   
+00014040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014050: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
+00014060: 6e74 656e 7369 7479 5f6b 6579 203a 2028  ntensity_key : (
+00014070: 666c 6f61 7428 696e 7465 6e73 6974 795f  float(intensity_
+00014080: 6d65 616e 5b69 6e64 6578 5d29 292c 0d0a  mean[index])),..
+00014090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000140a0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000140b0: 6164 6975 735f 6b65 7920 3a20 2866 6c6f  adius_key : (flo
+000140c0: 6174 2852 4144 4955 5329 292c 0d0a 2020  at(RADIUS)),..  
+000140d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140e0: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
+000140f0: 7479 5f6b 6579 203a 2028 666c 6f61 7428  ty_key : (float(
+00014100: 5155 414c 4954 5929 292c 0d0a 2020 2020  QUALITY)),..    
+00014110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014120: 2020 2020 7365 6c66 2e64 6973 7461 6e63      self.distanc
+00014130: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 793a  e_cell_mask_key:
+00014140: 2066 6c6f 6174 2864 6973 7461 6e63 655f   float(distance_
+00014150: 6365 6c6c 5f6d 6173 6b29 2c0d 0a20 2020  cell_mask),..   
+00014160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014170: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
+00014180: 6e74 726f 6964 5f7a 5f6b 6579 3a20 666c  ntroid_z_key: fl
+00014190: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
+000141a0: 5b30 5d29 2c0d 0a20 2020 2020 2020 2020  [0]),..         
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000141c0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+000141d0: 5f79 5f6b 6579 3a20 666c 6f61 7428 6d61  _y_key: float(ma
+000141e0: 736b 6365 6e74 726f 6964 5b31 5d29 2c0d  skcentroid[1]),.
+000141f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014200: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00014210: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
+00014220: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
+00014230: 726f 6964 5b32 5d29 200d 0a0d 0a20 2020  roid[2]) ....   
+00014240: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
+00014250: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00014260: 2063 656c 6c5f 6964 2069 6e20 7365 6c66   cell_id in self
+00014270: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
+00014280: 6b75 702e 6b65 7973 2829 3a0d 0a20 2020  kup.keys():..   
+00014290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000142b0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+000142c0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+000142d0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+000142e0: 6964 5d20 3d20 7365 6c66 2e75 6e69 7175  id] = self.uniqu
+000142f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014300: 735b 6365 6c6c 5f69 645d 0d0a 0d0a 2020  s[cell_id]....  
+00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014320: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
+00014330: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014340: 7274 6965 735b 6365 6c6c 5f69 645d 2e75  rties[cell_id].u
+00014350: 7064 6174 6528 7b73 656c 662e 746f 7461  pdate({self.tota
+00014360: 6c5f 696e 7465 6e73 6974 795f 6b65 793a  l_intensity_key:
+00014370: 202d 317d 290d 0a20 2020 2020 2020 2020   -1})..         
+00014380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014390: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+000143a0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+000143b0: 656c 6c5f 6964 5d2e 7570 6461 7465 287b  ell_id].update({
+000143c0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+000143d0: 6974 795f 6b65 793a 202d 317d 290d 0a20  ity_key: -1}).. 
+000143e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143f0: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+00014400: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014410: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
+00014420: 7570 6461 7465 287b 7365 6c66 2e72 6164  update({self.rad
+00014430: 6975 735f 6b65 793a 202d 317d 290d 0a20  ius_key: -1}).. 
+00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014450: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+00014460: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014470: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
+00014480: 7570 6461 7465 287b 7365 6c66 2e71 7561  update({self.qua
+00014490: 6c69 7479 5f6b 6579 3a20 2d31 7d29 0d0a  lity_key: -1})..
+000144a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144c0: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
+000144d0: 6469 6374 5f75 7064 6174 6528 7365 6c66  dict_update(self
+000144e0: 2c20 756e 6971 7565 5f74 7261 636b 6c65  , unique_trackle
+000144f0: 745f 6964 733a 204c 6973 742c 2020 6365  t_ids: List,  ce
+00014500: 6c6c 5f69 643a 2069 6e74 2c20 7472 6163  ll_id: int, trac
+00014510: 6b5f 6964 3a20 696e 742c 2073 6f75 7263  k_id: int, sourc
+00014520: 655f 6964 3a20 696e 742c 2074 6172 6765  e_id: int, targe
+00014530: 745f 6964 3a20 696e 7429 3a0d 0a0d 0a20  t_id: int):.... 
+00014540: 0d0a 2020 2020 2020 2020 6765 6e65 7261  ..        genera
+00014550: 7469 6f6e 5f69 6420 3d20 7365 6c66 2e67  tion_id = self.g
+00014560: 656e 6572 6174 696f 6e5f 6469 6374 5b63  eneration_dict[c
+00014570: 656c 6c5f 6964 5d0d 0a20 2020 2020 2020  ell_id]..       
+00014580: 2074 7261 636b 6c65 745f 6964 203d 2073   tracklet_id = s
+00014590: 656c 662e 7472 6163 6b6c 6574 5f64 6963  elf.tracklet_dic
+000145a0: 745b 6365 6c6c 5f69 645d 0d0a 0d0a 2020  t[cell_id]....  
+000145b0: 2020 2020 2020 756e 6971 7565 5f69 6420        unique_id 
+000145c0: 3d20 7374 7228 7472 6163 6b5f 6964 2920  = str(track_id) 
+000145d0: 2b20 7374 7228 7365 6c66 2e6d 6178 5f74  + str(self.max_t
+000145e0: 7261 636b 5f69 6429 202b 2073 7472 2867  rack_id) + str(g
+000145f0: 656e 6572 6174 696f 6e5f 6964 2920 2b20  eneration_id) + 
+00014600: 7374 7228 7472 6163 6b6c 6574 5f69 6429  str(tracklet_id)
+00014610: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00014620: 2020 2020 7665 635f 6d61 736b 203d 205b      vec_mask = [
+00014630: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00014640: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014650: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00014660: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+00014670: 645f 785f 6b65 795d 292c 2066 6c6f 6174  d_x_key]), float
+00014680: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014690: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000146a0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+000146b0: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
+000146c0: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
+000146d0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000146e0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+000146f0: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
+00014700: 656e 7472 6f69 645f 7a5f 6b65 795d 2920  entroid_z_key]) 
+00014710: 5d0d 0a0d 0a20 2020 2020 2020 2076 6563  ]....        vec
+00014720: 5f63 656c 6c20 3d20 5b66 6c6f 6174 2873  _cell = [float(s
+00014730: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014740: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014750: 656c 6c5f 6964 295d 5b73 656c 662e 7870  ell_id)][self.xp
+00014760: 6f73 6964 5f6b 6579 5d29 202c 200d 0a20  osid_key]) , .. 
+00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014780: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+00014790: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+000147a0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000147b0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+000147c0: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
+000147d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147e0: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+000147f0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00014800: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014810: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00014820: 2e7a 706f 7369 645f 6b65 795d 295d 0d0a  .zposid_key])]..
+00014830: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
+00014840: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
+00014850: 2876 6563 5f6d 6173 6b2c 2076 6563 5f63  (vec_mask, vec_c
+00014860: 656c 6c29 0d0a 0d0a 2020 2020 2020 2020  ell)....        
+00014870: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014880: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014890: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+000148a0: 287b 7365 6c66 2e72 6164 6961 6c5f 616e  ({self.radial_an
+000148b0: 676c 655f 6b65 7920 3a20 616e 676c 657d  gle_key : angle}
+000148c0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+000148d0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+000148e0: 2075 6e69 7175 655f 7472 6163 6b6c 6574   unique_tracklet
+000148f0: 5f69 6473 2e61 7070 656e 6428 7374 7228  _ids.append(str(
+00014900: 756e 6971 7565 5f69 6429 290d 0a20 2020  unique_id))..   
+00014910: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00014920: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014930: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00014940: 7064 6174 6528 7b73 656c 662e 636c 7573  pdate({self.clus
+00014950: 7465 7263 6c61 7373 5f6b 6579 203a 202d  terclass_key : -
+00014960: 317d 290d 0a20 2020 2020 2020 2073 656c  1})..        sel
+00014970: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014980: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014990: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+000149a0: 656c 662e 636c 7573 7465 7273 636f 7265  elf.clusterscore
+000149b0: 5f6b 6579 203a 2030 7d29 0d0a 2020 2020  _key : 0})..    
+000149c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000149d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000149e0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+000149f0: 6461 7465 287b 7365 6c66 2e75 6e69 7175  date({self.uniqu
+00014a00: 6569 645f 6b65 7920 3a20 7374 7228 756e  eid_key : str(un
+00014a10: 6971 7565 5f69 6429 7d29 0d0a 2020 2020  ique_id)})..    
+00014a20: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014a30: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014a40: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00014a50: 6461 7465 287b 7365 6c66 2e74 7261 636b  date({self.track
+00014a60: 6c65 7469 645f 6b65 7920 3a20 7374 7228  letid_key : str(
+00014a70: 7472 6163 6b6c 6574 5f69 6429 7d29 200d  tracklet_id)}) .
+00014a80: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00014a90: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014aa0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014ab0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00014ac0: 6765 6e65 7261 7469 6f6e 6964 5f6b 6579  generationid_key
+00014ad0: 203a 2073 7472 2867 656e 6572 6174 696f   : str(generatio
+00014ae0: 6e5f 6964 297d 2920 0d0a 2020 2020 2020  n_id)}) ..      
+00014af0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00014b00: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014b10: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00014b20: 7465 287b 7365 6c66 2e74 7261 636b 6964  te({self.trackid
+00014b30: 5f6b 6579 203a 2073 7472 2874 7261 636b  _key : str(track
+00014b40: 5f69 6429 7d29 0d0a 2020 2020 2020 2020  _id)})..        
+00014b50: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014b60: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014b70: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00014b80: 287b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ({self.motion_an
+00014b90: 676c 655f 6b65 7920 3a20 302e 307d 290d  gle_key : 0.0}).
+00014ba0: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00014bb0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014bc0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014bd0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00014be0: 7370 6565 645f 6b65 7920 3a20 302e 307d  speed_key : 0.0}
+00014bf0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00014c00: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014c10: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00014c20: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00014c30: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+00014c40: 6579 203a 2030 2e30 7d29 0d0a 2020 2020  ey : 0.0})..    
+00014c50: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014c60: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014c70: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00014c80: 6461 7465 287b 7365 6c66 2e65 6363 656e  date({self.eccen
+00014c90: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00014ca0: 7374 6b65 7920 3a20 2d31 7d29 0d0a 2020  stkey : -1})..  
+00014cb0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00014cc0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014cd0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00014ce0: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
+00014cf0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+00014d00: 6563 6f6e 646b 6579 203a 202d 317d 290d  econdkey : -1}).
+00014d10: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00014d20: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014d30: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014d40: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00014d50: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
+00014d60: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
+00014d70: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00014d80: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014d90: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00014da0: 6528 7b73 656c 662e 6365 6c6c 6178 6973  e({self.cellaxis
+00014db0: 5f6d 6173 6b5f 6b65 7920 3a20 2d31 7d29  _mask_key : -1})
+00014dc0: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
+00014dd0: 6f75 7263 655f 6964 2069 7320 6e6f 7420  ource_id is not 
+00014de0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00014df0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00014e00: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014e10: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00014e20: 6174 6528 7b73 656c 662e 6265 666f 7265  ate({self.before
+00014e30: 6964 5f6b 6579 203a 2069 6e74 2873 6f75  id_key : int(sou
+00014e40: 7263 655f 6964 297d 290d 0a20 2020 2020  rce_id)})..     
+00014e50: 2020 2020 2020 2076 6563 5f31 203d 205b         vec_1 = [
+00014e60: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00014e70: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014e80: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00014e90: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+00014ea0: 2920 2d20 666c 6f61 7428 7365 6c66 2e75  ) - float(self.u
+00014eb0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014ec0: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
+00014ed0: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
+00014ee0: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
+00014ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f00: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
+00014f10: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014f20: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014f30: 6c5f 6964 295d 5b73 656c 662e 7970 6f73  l_id)][self.ypos
+00014f40: 6964 5f6b 6579 5d29 202d 2066 6c6f 6174  id_key]) - float
+00014f50: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014f60: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014f70: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
+00014f80: 662e 7970 6f73 6964 5f6b 6579 5d29 2c20  f.yposid_key]), 
+00014f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014fa0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+00014fb0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014fc0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014fd0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00014fe0: 6c66 2e7a 706f 7369 645f 6b65 795d 2920  lf.zposid_key]) 
+00014ff0: 2d20 2066 6c6f 6174 2873 656c 662e 756e  -  float(self.un
+00015000: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015010: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
+00015020: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
+00015030: 5f6b 6579 5d29 5d0d 0a20 2020 2020 2020  _key])]..       
+00015040: 2020 2020 2073 7065 6564 203d 206e 702e       speed = np.
+00015050: 7371 7274 286e 702e 646f 7428 7665 635f  sqrt(np.dot(vec_
+00015060: 312c 2076 6563 5f31 2929 2f73 656c 662e  1, vec_1))/self.
+00015070: 7463 616c 6962 7261 7469 6f6e 0d0a 2020  tcalibration..  
+00015080: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00015090: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000150a0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000150b0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+000150c0: 2e73 7065 6564 5f6b 6579 203a 2073 7065  .speed_key : spe
+000150d0: 6564 7d29 0d0a 0d0a 2020 2020 2020 2020  ed})....        
+000150e0: 2020 2020 6d6f 7469 6f6e 5f61 6e67 6c65      motion_angle
+000150f0: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
+00015100: 6528 7665 635f 6d61 736b 2c20 7665 635f  e(vec_mask, vec_
+00015110: 3129 0d0a 0d0a 2020 2020 2020 2020 2020  1)....          
+00015120: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00015130: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015140: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00015150: 7465 287b 7365 6c66 2e6d 6f74 696f 6e5f  te({self.motion_
+00015160: 616e 676c 655f 6b65 7920 3a20 6d6f 7469  angle_key : moti
+00015170: 6f6e 5f61 6e67 6c65 7d29 200d 0a0d 0a20  on_angle}) .... 
+00015180: 2020 2020 2020 2020 2020 2069 6620 736f             if so
+00015190: 7572 6365 5f69 6420 696e 2073 656c 662e  urce_id in self.
+000151a0: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
+000151b0: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
+000151c0: 2020 2020 2020 2020 2070 7265 5f73 6f75           pre_sou
+000151d0: 7263 655f 6964 203d 2073 656c 662e 6564  rce_id = self.ed
+000151e0: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
+000151f0: 5b73 6f75 7263 655f 6964 5d0d 0a20 2020  [source_id]..   
 00015200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015210: 2020 666c 6f61 7428 7365 6c66 2e75 6e69    float(self.uni
-00015220: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015230: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00015240: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-00015250: 795d 2920 2d20 2032 202a 2066 6c6f 6174  y]) -  2 * float
-00015260: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015270: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015280: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
-00015290: 662e 7a70 6f73 6964 5f6b 6579 5d29 202b  f.zposid_key]) +
-000152a0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-000152b0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000152c0: 6573 5b69 6e74 2870 7265 5f73 6f75 7263  es[int(pre_sourc
-000152d0: 655f 6964 295d 5b73 656c 662e 7a70 6f73  e_id)][self.zpos
-000152e0: 6964 5f6b 6579 5d29 5d0d 0a20 2020 2020  id_key])]..     
-000152f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00015300: 6363 203d 206e 702e 7371 7274 286e 702e  cc = np.sqrt(np.
-00015310: 646f 7428 7665 635f 322c 2076 6563 5f32  dot(vec_2, vec_2
-00015320: 2929 2f73 656c 662e 7463 616c 6962 7261  ))/self.tcalibra
-00015330: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00015340: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00015350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015360: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015370: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015380: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00015390: 287b 7365 6c66 2e61 6363 656c 6572 6174  ({self.accelerat
-000153a0: 696f 6e5f 6b65 7920 3a20 6163 637d 290d  ion_key : acc}).
-000153b0: 0a20 2020 2020 2020 2065 6c69 6620 736f  .        elif so
-000153c0: 7572 6365 5f69 6420 6973 204e 6f6e 653a  urce_id is None:
-000153d0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000153e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000153f0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015400: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00015410: 7365 6c66 2e62 6566 6f72 6569 645f 6b65  self.beforeid_ke
-00015420: 7920 3a20 4e6f 6e65 7d29 200d 0a20 2020  y : None}) ..   
-00015430: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-00015440: 2020 2020 2069 6620 7461 7267 6574 5f69       if target_i
-00015450: 6420 6973 206e 6f74 204e 6f6e 653a 2020  d is not None:  
-00015460: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00015470: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015480: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015490: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-000154a0: 6174 6528 7b73 656c 662e 6166 7465 7269  ate({self.afteri
-000154b0: 645f 6b65 7920 3a20 696e 7428 7461 7267  d_key : int(targ
-000154c0: 6574 5f69 6429 7d29 200d 0a20 2020 2020  et_id)}) ..     
-000154d0: 2020 2065 6c69 6620 7461 7267 6574 5f69     elif target_i
-000154e0: 6420 6973 204e 6f6e 653a 0d0a 2020 2020  d is None:..    
-000154f0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00015500: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015510: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00015520: 5d2e 7570 6461 7465 287b 7365 6c66 2e61  ].update({self.a
-00015530: 6674 6572 6964 5f6b 6579 203a 204e 6f6e  fterid_key : Non
-00015540: 657d 290d 0a20 2020 2020 2020 2020 2020  e})..           
-00015550: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-00015560: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
-00015570: 7570 6461 7465 2863 656c 6c5f 6964 2c20  update(cell_id, 
-00015580: 7472 6163 6b5f 6964 2920 2020 200d 0a0d  track_id)    ...
-00015590: 0a0d 0a20 2020 2064 6566 205f 7465 6d70  ...    def _temp
-000155a0: 6f72 616c 5f70 6c6f 7473 5f74 7261 636b  oral_plots_track
-000155b0: 6d61 7465 2873 656c 6629 3a0d 0a20 2020  mate(self):..   
-000155c0: 200d 0a20 2020 200d 0a20 2020 200d 0a20   ..    ..    .. 
-000155d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000155e0: 656c 662e 4174 7472 203d 207b 7d0d 0a20  elf.Attr = {}.. 
-000155f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015600: 7461 7274 7469 6d65 203d 2069 6e74 286d  tarttime = int(m
-00015610: 696e 2873 656c 662e 416c 6c56 616c 7565  in(self.AllValue
-00015620: 735b 7365 6c66 2e66 7261 6d65 6964 5f6b  s[self.frameid_k
-00015630: 6579 5d29 290d 0a20 2020 2020 2020 2020  ey]))..         
-00015640: 2020 2020 2020 2065 6e64 7469 6d65 203d         endtime =
-00015650: 2069 6e74 286d 6178 2873 656c 662e 416c   int(max(self.Al
-00015660: 6c56 616c 7565 735b 7365 6c66 2e66 7261  lValues[self.fra
-00015670: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
-00015680: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00015690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156a0: 7365 6c66 2e74 696d 6520 3d20 5b5d 0d0a  self.time = []..
-000156b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156c0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-000156d0: 6e5f 6469 7370 5f7a 203d 205b 5d0d 0a20  n_disp_z = [].. 
-000156e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000156f0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00015700: 6469 7370 5f7a 203d 205b 5d0d 0a0d 0a20  disp_z = [].... 
-00015710: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015720: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00015730: 5f64 6973 705f 7920 3d20 5b5d 0d0a 2020  _disp_y = []..  
-00015740: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015750: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
-00015760: 6973 705f 7920 3d20 5b5d 0d0a 0d0a 2020  isp_y = []....  
-00015770: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015780: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00015790: 6469 7370 5f78 203d 205b 5d0d 0a20 2020  disp_x = []..   
-000157a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000157b0: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-000157c0: 7370 5f78 203d 205b 5d0d 0a0d 0a20 2020  sp_x = []....   
-000157d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000157e0: 662e 6d69 746f 7469 635f 6d65 616e 5f72  f.mitotic_mean_r
-000157f0: 6164 6975 7320 3d20 5b5d 0d0a 2020 2020  adius = []..    
-00015800: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015810: 2e6d 6974 6f74 6963 5f76 6172 5f72 6164  .mitotic_var_rad
-00015820: 6975 7320 3d20 5b5d 0d0a 0d0a 2020 2020  ius = []....    
-00015830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015840: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 7370  .mitotic_mean_sp
-00015850: 6565 6420 3d20 5b5d 0d0a 2020 2020 2020  eed = []..      
-00015860: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015870: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
-00015880: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015890: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000158a0: 746f 7469 635f 6d65 616e 5f61 6363 203d  totic_mean_acc =
-000158b0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000158c0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000158d0: 635f 7661 725f 6163 6320 3d20 5b5d 0d0a  c_var_acc = []..
-000158e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000158f0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00015900: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
-00015910: 6368 616e 6765 203d 205b 5d0d 0a20 2020  change = []..   
-00015920: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015930: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00015940: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00015950: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015960: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015970: 746f 7469 635f 6d65 616e 5f64 6973 7461  totic_mean_dista
-00015980: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
-00015990: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000159a0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000159b0: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
-000159c0: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a  ll_mask = []....
-000159d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159e0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-000159f0: 5f6d 6561 6e5f 6469 7370 5f7a 203d 205b  _mean_disp_z = [
-00015a00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015a10: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00015a20: 7469 635f 7661 725f 6469 7370 5f7a 203d  tic_var_disp_z =
-00015a30: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015a40: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00015a50: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00015a60: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
-00015a70: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015a80: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00015a90: 6973 705f 7920 3d20 5b5d 0d0a 0d0a 2020  isp_y = []....  
-00015aa0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015ab0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00015ac0: 6561 6e5f 6469 7370 5f78 203d 205b 5d0d  ean_disp_x = [].
-00015ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ae0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00015af0: 635f 7661 725f 6469 7370 5f78 203d 205b  c_var_disp_x = [
-00015b00: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00015b10: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00015b20: 746f 7469 635f 6d65 616e 5f72 6164 6975  totic_mean_radiu
-00015b30: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00015b40: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00015b50: 5f6d 6974 6f74 6963 5f76 6172 5f72 6164  _mitotic_var_rad
-00015b60: 6975 7320 3d20 5b5d 0d0a 0d0a 2020 2020  ius = []....    
-00015b70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015b80: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00015b90: 6e5f 7370 6565 6420 3d20 5b5d 0d0a 2020  n_speed = []..  
-00015ba0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015bb0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00015bc0: 6172 5f73 7065 6564 203d 205b 5d0d 0a0d  ar_speed = []...
-00015bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015be0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00015bf0: 635f 6d65 616e 5f61 6363 203d 205b 5d0d  c_mean_acc = [].
-00015c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015c10: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00015c20: 635f 7661 725f 6163 6320 3d20 5b5d 0d0a  c_var_acc = []..
-00015c30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015c40: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00015c50: 6963 5f6d 6561 6e5f 6469 7265 6374 696f  ic_mean_directio
-00015c60: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-00015c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015c80: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00015c90: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
-00015ca0: 6c5f 6368 616e 6765 203d 205b 5d0d 0a0d  l_change = []...
-00015cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015cc0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00015cd0: 635f 6d65 616e 5f64 6973 7461 6e63 655f  c_mean_distance_
-00015ce0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
-00015cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d00: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015d10: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
-00015d20: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a  ll_mask = []....
-00015d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d40: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00015d50: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
-00015d60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015d70: 616c 6c5f 7661 725f 6469 7370 5f7a 203d  all_var_disp_z =
-00015d80: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015d90: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00015da0: 6d65 616e 5f64 6973 705f 7920 3d20 5b5d  mean_disp_y = []
-00015db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015dc0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00015dd0: 6973 705f 7920 3d20 5b5d 0d0a 0d0a 2020  isp_y = []....  
-00015de0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015df0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
-00015e00: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
-00015e10: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00015e20: 6c5f 7661 725f 6469 7370 5f78 203d 205b  l_var_disp_x = [
-00015e30: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00015e40: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00015e50: 616e 5f72 6164 6975 7320 3d20 5b5d 0d0a  an_radius = []..
-00015e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e70: 7365 6c66 2e61 6c6c 5f76 6172 5f72 6164  self.all_var_rad
-00015e80: 6975 7320 3d20 5b5d 0d0a 0d0a 2020 2020  ius = []....    
-00015e90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015ea0: 2e61 6c6c 5f6d 6561 6e5f 7370 6565 6420  .all_mean_speed 
-00015eb0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015ec0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00015ed0: 6172 5f73 7065 6564 203d 205b 5d0d 0a0d  ar_speed = []...
-00015ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ef0: 2073 656c 662e 616c 6c5f 6d65 616e 5f61   self.all_mean_a
-00015f00: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
-00015f10: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00015f20: 6c5f 7661 725f 6163 6320 3d20 5b5d 0d0a  l_var_acc = []..
-00015f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015f40: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00015f50: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00015f60: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
-00015f70: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00015f80: 6c5f 7661 725f 6469 7265 6374 696f 6e61  l_var_directiona
-00015f90: 6c5f 6368 616e 6765 203d 205b 5d0d 0a0d  l_change = []...
-00015fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015fb0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00015fc0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00015fd0: 6b20 3d20 5b5d 0d0a 2020 2020 2020 2020  k = []..        
-00015fe0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00015ff0: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
-00016000: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a  ll_mask = []....
-00016010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016020: 7365 6c66 2e6d 6974 6f74 6963 5f63 6c75  self.mitotic_clu
-00016030: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
-00016040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016050: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00016060: 635f 636c 7573 7465 725f 636c 6173 7320  c_cluster_class 
-00016070: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016080: 2020 2020 2020 7365 6c66 2e61 6c6c 5f63        self.all_c
-00016090: 6c75 7374 6572 5f63 6c61 7373 203d 205b  luster_class = [
-000160a0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-000160b0: 2020 2020 2061 6c6c 5f73 706f 7473 5f74       all_spots_t
-000160c0: 7261 636b 7320 3d20 7b7d 0d0a 2020 2020  racks = {}..    
-000160d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000160e0: 286b 2c76 2920 696e 2073 656c 662e 756e  (k,v) in self.un
-000160f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016100: 7469 6573 2e69 7465 6d73 2829 3a0d 0a20  ties.items():.. 
-00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016120: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00016130: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00016140: 5f73 706f 7473 203d 2073 656c 662e 756e  _spots = self.un
-00016150: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016160: 7469 6573 5b6b 5d0d 0a20 2020 2020 2020  ties[k]..       
-00016170: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016180: 6620 7365 6c66 2e74 7261 636b 6964 5f6b  f self.trackid_k
-00016190: 6579 2069 6e20 616c 6c5f 7370 6f74 733a  ey in all_spots:
-000161a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000161b0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-000161c0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d20  spots_tracks[k] 
-000161d0: 3d20 616c 6c5f 7370 6f74 730d 0a20 2020  = all_spots..   
-000161e0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-000161f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016200: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00016210: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
-00016220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016230: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
-00016240: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
-00016250: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
-00016260: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
-00016270: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
-00016280: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
-00016290: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162b0: 2020 2020 666f 7220 6920 696e 2074 7164      for i in tqd
-000162c0: 6d28 7261 6e67 6528 7374 6172 7474 696d  m(range(starttim
-000162d0: 652c 2065 6e64 7469 6d65 292c 2074 6f74  e, endtime), tot
-000162e0: 616c 3d65 6e64 7469 6d65 202d 2073 7461  al=endtime - sta
-000162f0: 7274 7469 6d65 293a 0d0a 2020 2020 2020  rttime):..      
-00016300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016320: 2020 2020 2020 2020 2020 6675 7475 7265            future
-00016330: 732e 6170 7065 6e64 2865 7865 6375 746f  s.append(executo
-00016340: 722e 7375 626d 6974 2873 656c 662e 5f63  r.submit(self._c
-00016350: 6f6d 7075 7465 5f74 656d 706f 7261 6c2c  ompute_temporal,
-00016360: 2069 2c20 616c 6c5f 7370 6f74 735f 7472   i, all_spots_tr
-00016370: 6163 6b73 2929 0d0a 200d 0a20 2020 2020  acks)).. ..     
-00016380: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00016390: 722e 7265 7375 6c74 2829 2066 6f72 2072  r.result() for r
-000163a0: 2069 6e20 636f 6e63 7572 7265 6e74 2e66   in concurrent.f
-000163b0: 7574 7572 6573 2e61 735f 636f 6d70 6c65  utures.as_comple
-000163c0: 7465 6428 6675 7475 7265 7329 5d0d 0a0d  ted(futures)]...
-000163d0: 0a0d 0a20 2020 2064 6566 205f 636f 6d70  ...    def _comp
-000163e0: 7574 655f 7465 6d70 6f72 616c 2873 656c  ute_temporal(sel
-000163f0: 662c 2069 2c20 616c 6c5f 7370 6f74 735f  f, i, all_spots_
-00016400: 7472 6163 6b73 293a 2020 2020 2020 2020  tracks):        
-00016410: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00016420: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016430: 746f 7469 635f 6469 7370 5f7a 203d 205b  totic_disp_z = [
-00016440: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016450: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00016460: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
-00016470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016480: 6d69 746f 7469 635f 6469 7370 5f78 203d  mitotic_disp_x =
-00016490: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000164a0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-000164b0: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
-000164c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164d0: 2020 6d69 746f 7469 635f 7370 6565 6420    mitotic_speed 
-000164e0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000164f0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-00016500: 635f 6163 6320 3d20 5b5d 0d0a 2020 2020  c_acc = []..    
-00016510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016520: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
-00016530: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-00016540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016550: 2020 2020 206d 6974 6f74 6963 5f63 6c75       mitotic_clu
-00016560: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
-00016570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016580: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00016590: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-000165a0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-000165b0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-000165c0: 6d69 746f 7469 635f 6469 7370 5f7a 203d  mitotic_disp_z =
-000165d0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000165e0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-000165f0: 6f74 6963 5f64 6973 705f 7920 3d20 5b5d  otic_disp_y = []
-00016600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016610: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00016620: 635f 6469 7370 5f78 203d 205b 5d0d 0a20  c_disp_x = [].. 
-00016630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016640: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f72     non_mitotic_r
-00016650: 6164 6975 7320 3d20 5b5d 0d0a 2020 2020  adius = []..    
-00016660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016670: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-00016680: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
-00016690: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-000166a0: 6d69 746f 7469 635f 6163 6320 3d20 5b5d  mitotic_acc = []
-000166b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000166c0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-000166d0: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
-000166e0: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
-000166f0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016700: 6f6e 5f6d 6974 6f74 6963 5f63 6c75 7374  on_mitotic_clust
-00016710: 6572 5f63 6c61 7373 203d 205b 5d0d 0a20  er_class = [].. 
-00016720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016730: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00016740: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00016750: 6b20 3d20 5b5d 0d0a 2020 2020 2020 2020  k = []..        
-00016760: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00016770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016780: 2020 616c 6c5f 6469 7370 5f7a 203d 205b    all_disp_z = [
-00016790: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000167a0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-000167b0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
-000167c0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-000167d0: 6469 7370 5f78 203d 205b 5d0d 0a20 2020  disp_x = []..   
+00015210: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00015220: 2020 2020 2020 2076 6563 5f32 203d 205b         vec_2 = [
+00015230: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00015240: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015250: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00015260: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+00015270: 2920 2d20 3220 2a20 666c 6f61 7428 7365  ) - 2 * float(se
+00015280: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015290: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
+000152a0: 7572 6365 5f69 6429 5d5b 7365 6c66 2e78  urce_id)][self.x
+000152b0: 706f 7369 645f 6b65 795d 2920 2b20 666c  posid_key]) + fl
+000152c0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000152d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000152e0: 696e 7428 7072 655f 736f 7572 6365 5f69  int(pre_source_i
+000152f0: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+00015300: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
+00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015320: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
+00015330: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015340: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015350: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
+00015360: 5f6b 6579 5d29 202d 2032 202a 2066 6c6f  _key]) - 2 * flo
+00015370: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015380: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015390: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
+000153a0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+000153b0: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
+000153c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000153d0: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
+000153e0: 7263 655f 6964 295d 5b73 656c 662e 7970  rce_id)][self.yp
+000153f0: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
+00015400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015410: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00015420: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015430: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015440: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e7a  cell_id)][self.z
+00015450: 706f 7369 645f 6b65 795d 2920 2d20 2032  posid_key]) -  2
+00015460: 202a 2066 6c6f 6174 2873 656c 662e 756e   * float(self.un
+00015470: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015480: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
+00015490: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
+000154a0: 5f6b 6579 5d29 202b 2066 6c6f 6174 2873  _key]) + float(s
+000154b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000154c0: 7072 6f70 6572 7469 6573 5b69 6e74 2870  properties[int(p
+000154d0: 7265 5f73 6f75 7263 655f 6964 295d 5b73  re_source_id)][s
+000154e0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+000154f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015500: 2020 2020 2020 2061 6363 203d 206e 702e         acc = np.
+00015510: 7371 7274 286e 702e 646f 7428 7665 635f  sqrt(np.dot(vec_
+00015520: 322c 2076 6563 5f32 2929 2f73 656c 662e  2, vec_2))/self.
+00015530: 7463 616c 6962 7261 7469 6f6e 0d0a 2020  tcalibration..  
+00015540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015550: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00015560: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00015570: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015580: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00015590: 5d2e 7570 6461 7465 287b 7365 6c66 2e61  ].update({self.a
+000155a0: 6363 656c 6572 6174 696f 6e5f 6b65 7920  cceleration_key 
+000155b0: 3a20 6163 637d 290d 0a20 2020 2020 2020  : acc})..       
+000155c0: 2065 6c69 6620 736f 7572 6365 5f69 6420   elif source_id 
+000155d0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+000155e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000155f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015600: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00015610: 7570 6461 7465 287b 7365 6c66 2e62 6566  update({self.bef
+00015620: 6f72 6569 645f 6b65 7920 3a20 4e6f 6e65  oreid_key : None
+00015630: 7d29 200d 0a20 2020 2020 2020 2020 2020  }) ..           
+00015640: 200d 0a0d 0a20 2020 2020 2020 2069 6620   ....        if 
+00015650: 7461 7267 6574 5f69 6420 6973 206e 6f74  target_id is not
+00015660: 204e 6f6e 653a 2020 2020 2020 200d 0a20   None:       .. 
+00015670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015680: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015690: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+000156a0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+000156b0: 662e 6166 7465 7269 645f 6b65 7920 3a20  f.afterid_key : 
+000156c0: 696e 7428 7461 7267 6574 5f69 6429 7d29  int(target_id)})
+000156d0: 200d 0a20 2020 2020 2020 2065 6c69 6620   ..        elif 
+000156e0: 7461 7267 6574 5f69 6420 6973 204e 6f6e  target_id is Non
+000156f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00015700: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015710: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015720: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00015730: 287b 7365 6c66 2e61 6674 6572 6964 5f6b  ({self.afterid_k
+00015740: 6579 203a 204e 6f6e 657d 290d 0a20 2020  ey : None})..   
+00015750: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00015760: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
+00015770: 6368 616e 6e65 6c5f 7570 6461 7465 2863  channel_update(c
+00015780: 656c 6c5f 6964 2c20 7472 6163 6b5f 6964  ell_id, track_id
+00015790: 2920 2020 200d 0a0d 0a0d 0a20 2020 2064  )    ......    d
+000157a0: 6566 205f 7465 6d70 6f72 616c 5f70 6c6f  ef _temporal_plo
+000157b0: 7473 5f74 7261 636b 6d61 7465 2873 656c  ts_trackmate(sel
+000157c0: 6629 3a0d 0a20 2020 200d 0a20 2020 200d  f):..    ..    .
+000157d0: 0a20 2020 200d 0a20 2020 2020 2020 2020  .    ..         
+000157e0: 2020 2020 2020 2073 656c 662e 4174 7472         self.Attr
+000157f0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00015800: 2020 2020 2020 2073 7461 7274 7469 6d65         starttime
+00015810: 203d 2069 6e74 286d 696e 2873 656c 662e   = int(min(self.
+00015820: 416c 6c56 616c 7565 735b 7365 6c66 2e66  AllValues[self.f
+00015830: 7261 6d65 6964 5f6b 6579 5d29 290d 0a20  rameid_key])).. 
+00015840: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00015850: 6e64 7469 6d65 203d 2069 6e74 286d 6178  ndtime = int(max
+00015860: 2873 656c 662e 416c 6c56 616c 7565 735b  (self.AllValues[
+00015870: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
+00015880: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
+00015890: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000158a0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+000158b0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+000158c0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+000158d0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
+000158e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000158f0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00015900: 7469 635f 7661 725f 6469 7370 5f7a 203d  tic_var_disp_z =
+00015910: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015920: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00015930: 7469 635f 6d65 616e 5f64 6973 705f 7920  tic_mean_disp_y 
+00015940: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015950: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00015960: 6963 5f76 6172 5f64 6973 705f 7920 3d20  ic_var_disp_y = 
+00015970: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015980: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00015990: 6963 5f6d 6561 6e5f 6469 7370 5f78 203d  ic_mean_disp_x =
+000159a0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000159b0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+000159c0: 635f 7661 725f 6469 7370 5f78 203d 205b  c_var_disp_x = [
+000159d0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+000159e0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+000159f0: 635f 6d65 616e 5f72 6164 6975 7320 3d20  c_mean_radius = 
+00015a00: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00015a10: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00015a20: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
+00015a30: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015a40: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00015a50: 5f6d 6561 6e5f 7370 6565 6420 3d20 5b5d  _mean_speed = []
+00015a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015a70: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00015a80: 6172 5f73 7065 6564 203d 205b 5d0d 0a0d  ar_speed = []...
+00015a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015aa0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00015ab0: 616e 5f61 6363 203d 205b 5d0d 0a20 2020  an_acc = []..   
+00015ac0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015ad0: 662e 6d69 746f 7469 635f 7661 725f 6163  f.mitotic_var_ac
+00015ae0: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
+00015af0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015b00: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
+00015b10: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00015b20: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00015b30: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00015b40: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
+00015b50: 6c5f 6368 616e 6765 203d 205b 5d0d 0a0d  l_change = []...
+00015b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015b70: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00015b80: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
+00015b90: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
+00015ba0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015bb0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+00015bc0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00015bd0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015be0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00015bf0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+00015c00: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+00015c10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015c20: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00015c30: 6469 7370 5f7a 203d 205b 5d0d 0a0d 0a20  disp_z = [].... 
+00015c40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015c50: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00015c60: 6d65 616e 5f64 6973 705f 7920 3d20 5b5d  mean_disp_y = []
+00015c70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015c80: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015c90: 6963 5f76 6172 5f64 6973 705f 7920 3d20  ic_var_disp_y = 
+00015ca0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015cb0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00015cc0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00015cd0: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+00015ce0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00015cf0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00015d00: 7370 5f78 203d 205b 5d0d 0a0d 0a20 2020  sp_x = []....   
+00015d10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015d20: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00015d30: 616e 5f72 6164 6975 7320 3d20 5b5d 0d0a  an_radius = []..
+00015d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d50: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00015d60: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
+00015d70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015d80: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00015d90: 6f74 6963 5f6d 6561 6e5f 7370 6565 6420  otic_mean_speed 
+00015da0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015db0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00015dc0: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
+00015dd0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00015de0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00015df0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f61  n_mitotic_mean_a
+00015e00: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
+00015e10: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00015e20: 6e5f 6d69 746f 7469 635f 7661 725f 6163  n_mitotic_var_ac
+00015e30: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
+00015e40: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00015e50: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00015e60: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00015e70: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
+00015e80: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00015e90: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00015ea0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00015eb0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00015ec0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00015ed0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+00015ee0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00015ef0: 6b20 3d20 5b5d 0d0a 2020 2020 2020 2020  k = []..        
+00015f00: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00015f10: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+00015f20: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00015f30: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015f40: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00015f50: 5f6d 6561 6e5f 6469 7370 5f7a 203d 205b  _mean_disp_z = [
+00015f60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015f70: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00015f80: 6469 7370 5f7a 203d 205b 5d0d 0a0d 0a20  disp_z = [].... 
+00015f90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015fa0: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
+00015fb0: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
+00015fc0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00015fd0: 6c6c 5f76 6172 5f64 6973 705f 7920 3d20  ll_var_disp_y = 
+00015fe0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015ff0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00016000: 6561 6e5f 6469 7370 5f78 203d 205b 5d0d  ean_disp_x = [].
+00016010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016020: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00016030: 7370 5f78 203d 205b 5d0d 0a0d 0a20 2020  sp_x = []....   
+00016040: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016050: 662e 616c 6c5f 6d65 616e 5f72 6164 6975  f.all_mean_radiu
+00016060: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00016070: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00016080: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
+00016090: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000160a0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+000160b0: 6e5f 7370 6565 6420 3d20 5b5d 0d0a 2020  n_speed = []..  
+000160c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000160d0: 6c66 2e61 6c6c 5f76 6172 5f73 7065 6564  lf.all_var_speed
+000160e0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+000160f0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00016100: 6c5f 6d65 616e 5f61 6363 203d 205b 5d0d  l_mean_acc = [].
+00016110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016120: 2073 656c 662e 616c 6c5f 7661 725f 6163   self.all_var_ac
+00016130: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
+00016140: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00016150: 6c6c 5f6d 6561 6e5f 6469 7265 6374 696f  ll_mean_directio
+00016160: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
+00016170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016180: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00016190: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+000161a0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+000161b0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000161c0: 6c5f 6d65 616e 5f64 6973 7461 6e63 655f  l_mean_distance_
+000161d0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
+000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161f0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00016200: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00016210: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00016220: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00016230: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
+00016240: 7373 203d 205b 5d0d 0a20 2020 2020 2020  ss = []..       
+00016250: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00016260: 6e5f 6d69 746f 7469 635f 636c 7573 7465  n_mitotic_cluste
+00016270: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
+00016280: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016290: 6c66 2e61 6c6c 5f63 6c75 7374 6572 5f63  lf.all_cluster_c
+000162a0: 6c61 7373 203d 205b 5d0d 0a0d 0a20 2020  lass = []....   
+000162b0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000162c0: 5f73 706f 7473 5f74 7261 636b 7320 3d20  _spots_tracks = 
+000162d0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+000162e0: 2020 2020 666f 7220 286b 2c76 2920 696e      for (k,v) in
+000162f0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00016300: 745f 7072 6f70 6572 7469 6573 2e69 7465  t_properties.ite
+00016310: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+00016320: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00016330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016340: 2020 2020 2061 6c6c 5f73 706f 7473 203d       all_spots =
+00016350: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00016360: 745f 7072 6f70 6572 7469 6573 5b6b 5d0d  t_properties[k].
+00016370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016380: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00016390: 7261 636b 6964 5f6b 6579 2069 6e20 616c  rackid_key in al
+000163a0: 6c5f 7370 6f74 733a 0d0a 2020 2020 2020  l_spots:..      
+000163b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163c0: 2020 2020 616c 6c5f 7370 6f74 735f 7472      all_spots_tr
+000163d0: 6163 6b73 5b6b 5d20 3d20 616c 6c5f 7370  acks[k] = all_sp
+000163e0: 6f74 730d 0a20 2020 2020 2020 2020 2020  ots..           
+000163f0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00016400: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00016410: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+00016420: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+00016430: 2020 2020 2020 2020 2077 6974 6820 636f           with co
+00016440: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+00016450: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
+00016460: 746f 7228 6d61 785f 776f 726b 6572 7320  tor(max_workers 
+00016470: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
+00016480: 2920 6173 2065 7865 6375 746f 723a 0d0a  ) as executor:..
+00016490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000164a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000164b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000164c0: 6920 696e 2074 7164 6d28 7261 6e67 6528  i in tqdm(range(
+000164d0: 7374 6172 7474 696d 652c 2065 6e64 7469  starttime, endti
+000164e0: 6d65 292c 2074 6f74 616c 3d65 6e64 7469  me), total=endti
+000164f0: 6d65 202d 2073 7461 7274 7469 6d65 293a  me - starttime):
+00016500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016510: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00016520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016530: 2020 6675 7475 7265 732e 6170 7065 6e64    futures.append
+00016540: 2865 7865 6375 746f 722e 7375 626d 6974  (executor.submit
+00016550: 2873 656c 662e 5f63 6f6d 7075 7465 5f74  (self._compute_t
+00016560: 656d 706f 7261 6c2c 2069 2c20 616c 6c5f  emporal, i, all_
+00016570: 7370 6f74 735f 7472 6163 6b73 2929 0d0a  spots_tracks))..
+00016580: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00016590: 2020 2020 2020 205b 722e 7265 7375 6c74         [r.result
+000165a0: 2829 2066 6f72 2072 2069 6e20 636f 6e63  () for r in conc
+000165b0: 7572 7265 6e74 2e66 7574 7572 6573 2e61  urrent.futures.a
+000165c0: 735f 636f 6d70 6c65 7465 6428 6675 7475  s_completed(futu
+000165d0: 7265 7329 5d0d 0a0d 0a0d 0a20 2020 2064  res)]......    d
+000165e0: 6566 205f 636f 6d70 7574 655f 7465 6d70  ef _compute_temp
+000165f0: 6f72 616c 2873 656c 662c 2069 2c20 616c  oral(self, i, al
+00016600: 6c5f 7370 6f74 735f 7472 6163 6b73 293a  l_spots_tracks):
+00016610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016630: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016640: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+00016650: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016660: 6974 6f74 6963 5f64 6973 705f 7920 3d20  itotic_disp_y = 
+00016670: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016680: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016690: 6469 7370 5f78 203d 205b 5d0d 0a20 2020  disp_x = []..   
+000166a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166b0: 206d 6974 6f74 6963 5f72 6164 6975 7320   mitotic_radius 
+000166c0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000166d0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000166e0: 635f 7370 6565 6420 3d20 5b5d 0d0a 2020  c_speed = []..  
+000166f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016700: 2020 6d69 746f 7469 635f 6163 6320 3d20    mitotic_acc = 
+00016710: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016720: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016730: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00016740: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
+00016750: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016760: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
+00016770: 7373 203d 205b 5d0d 0a20 2020 2020 2020  ss = []..       
+00016780: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016790: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
+000167a0: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a  ll_mask = []....
+000167b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167c0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+000167d0: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
 000167e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167f0: 2061 6c6c 5f72 6164 6975 7320 3d20 5b5d   all_radius = []
-00016800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016810: 2020 2020 2020 616c 6c5f 7370 6565 6420        all_speed 
-00016820: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016830: 2020 2020 2020 2020 2020 616c 6c5f 6163            all_ac
-00016840: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
-00016850: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00016860: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00016870: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
-00016880: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00016890: 5f63 6c75 7374 6572 5f63 6c61 7373 203d  _cluster_class =
-000168a0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000168b0: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-000168c0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-000168d0: 3d20 5b5d 0d0a 0d0a 0d0a 0d0a 0d0a 2020  = []..........  
-000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168f0: 2020 666f 7220 286b 2c76 2920 696e 2061    for (k,v) in a
-00016900: 6c6c 5f73 706f 7473 5f74 7261 636b 732e  ll_spots_tracks.
-00016910: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
-00016920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016930: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00016940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016950: 2020 2020 6375 7272 656e 745f 7469 6d65      current_time
-00016960: 203d 2061 6c6c 5f73 706f 7473 5f74 7261   = all_spots_tra
-00016970: 636b 735b 6b5d 5b73 656c 662e 6672 616d  cks[k][self.fram
-00016980: 6569 645f 6b65 795d 0d0a 2020 2020 2020  eid_key]..      
-00016990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169a0: 2020 2020 2020 6d69 746f 7469 6320 3d20        mitotic = 
-000169b0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-000169c0: 5b6b 5d5b 7365 6c66 2e64 6976 6964 696e  [k][self.dividin
-000169d0: 675f 6b65 795d 0d0a 2020 2020 2020 2020  g_key]..        
-000169e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00016a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a10: 2069 6620 6920 3d3d 2069 6e74 2863 7572   if i == int(cur
-00016a20: 7265 6e74 5f74 696d 6529 3a0d 0a20 2020  rent_time):..   
+000167f0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00016800: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
+00016810: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00016820: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
+00016830: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016840: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00016850: 6974 6f74 6963 5f72 6164 6975 7320 3d20  itotic_radius = 
+00016860: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016870: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00016880: 7469 635f 7370 6565 6420 3d20 5b5d 0d0a  tic_speed = []..
+00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168a0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+000168b0: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
+000168c0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+000168d0: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
+000168e0: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
+000168f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016900: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00016910: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+00016920: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016930: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00016940: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00016950: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
+00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016970: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00016980: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00016990: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+000169a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000169b0: 6c6c 5f64 6973 705f 7920 3d20 5b5d 0d0a  ll_disp_y = []..
+000169c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169d0: 2020 2020 616c 6c5f 6469 7370 5f78 203d      all_disp_x =
+000169e0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000169f0: 2020 2020 2020 2020 2061 6c6c 5f72 6164           all_rad
+00016a00: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
+00016a10: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00016a20: 6c5f 7370 6565 6420 3d20 5b5d 0d0a 2020  l_speed = []..  
 00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016a50: 6620 6d69 746f 7469 633a 0d0a 2020 2020  f mitotic:..    
-00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a80: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
-00016a90: 5f7a 2e61 7070 656e 6428 616c 6c5f 7370  _z.append(all_sp
-00016aa0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00016ab0: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
-00016ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ae0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016af0: 5f64 6973 705f 792e 6170 7065 6e64 2861  _disp_y.append(a
-00016b00: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00016b10: 6b5d 5b73 656c 662e 7970 6f73 6964 5f6b  k][self.yposid_k
-00016b20: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00016b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b40: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016b50: 746f 7469 635f 6469 7370 5f78 2e61 7070  totic_disp_x.app
-00016b60: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00016b70: 6163 6b73 5b6b 5d5b 7365 6c66 2e78 706f  acks[k][self.xpo
-00016b80: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bb0: 2020 206d 6974 6f74 6963 5f72 6164 6975     mitotic_radiu
-00016bc0: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
-00016bd0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00016be0: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
-00016bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a40: 2020 616c 6c5f 6163 6320 3d20 5b5d 0d0a    all_acc = []..
+00016a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a60: 2020 2020 616c 6c5f 6469 7265 6374 696f      all_directio
+00016a70: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
+00016a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016a90: 2020 2020 2061 6c6c 5f63 6c75 7374 6572       all_cluster
+00016aa0: 5f63 6c61 7373 203d 205b 5d0d 0a20 2020  _class = []..   
+00016ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ac0: 2061 6c6c 5f64 6973 7461 6e63 655f 6365   all_distance_ce
+00016ad0: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a  ll_mask = []....
+00016ae0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00016af0: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
+00016b00: 2c76 2920 696e 2061 6c6c 5f73 706f 7473  ,v) in all_spots
+00016b10: 5f74 7261 636b 732e 6974 656d 7328 293a  _tracks.items():
+00016b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016b30: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b50: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00016b60: 656e 745f 7469 6d65 203d 2061 6c6c 5f73  ent_time = all_s
+00016b70: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00016b80: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
+00016b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016ba0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00016bb0: 746f 7469 6320 3d20 616c 6c5f 7370 6f74  totic = all_spot
+00016bc0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00016bd0: 2e64 6976 6964 696e 675f 6b65 795d 0d0a  .dividing_key]..
+00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bf0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 00016c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c10: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00016c20: 7370 6565 642e 6170 7065 6e64 2861 6c6c  speed.append(all
-00016c30: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00016c40: 5b73 656c 662e 7370 6565 645f 6b65 795d  [self.speed_key]
-00016c50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00016c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c70: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016c80: 6963 5f61 6363 2e61 7070 656e 6428 616c  ic_acc.append(al
-00016c90: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00016ca0: 5d5b 7365 6c66 2e61 6363 656c 6572 6174  ][self.accelerat
-00016cb0: 696f 6e5f 6b65 795d 290d 0a20 2020 2020  ion_key])..     
-00016cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c10: 2020 2020 2020 2020 2069 6620 6920 3d3d           if i ==
+00016c20: 2069 6e74 2863 7572 7265 6e74 5f74 696d   int(current_tim
+00016c30: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+00016c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c50: 2020 2020 2020 2069 6620 6d69 746f 7469         if mitoti
+00016c60: 633a 0d0a 2020 2020 2020 2020 2020 2020  c:..            
+00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c80: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00016c90: 7469 635f 6469 7370 5f7a 2e61 7070 656e  tic_disp_z.appen
+00016ca0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00016cb0: 6b73 5b6b 5d5b 7365 6c66 2e7a 706f 7369  ks[k][self.zposi
+00016cc0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
 00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ce0: 2020 206d 6974 6f74 6963 5f64 6972 6563     mitotic_direc
-00016cf0: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
-00016d00: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00016d10: 7261 636b 735b 6b5d 5b73 656c 662e 6d6f  racks[k][self.mo
-00016d20: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 5d29  tion_angle_key])
-00016d30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016cf0: 206d 6974 6f74 6963 5f64 6973 705f 792e   mitotic_disp_y.
+00016d00: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00016d10: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00016d20: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
+00016d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d50: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-00016d60: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00016d70: 6d61 736b 2e61 7070 656e 6428 616c 6c5f  mask.append(all_
-00016d80: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00016d90: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-00016da0: 6c6c 5f6d 6173 6b5f 6b65 795d 290d 0a20  ll_mask_key]).. 
-00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dd0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00016de0: 6c75 7374 6572 636c 6173 735f 6b65 7920  lusterclass_key 
-00016df0: 696e 2061 6c6c 5f73 706f 7473 5f74 7261  in all_spots_tra
-00016e00: 636b 735b 6b5d 2e6b 6579 7328 2920 3a0d  cks[k].keys() :.
-00016e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e40: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
-00016e50: 636c 6173 732e 6170 7065 6e64 2861 6c6c  class.append(all
-00016e60: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00016e70: 5b73 656c 662e 636c 7573 7465 7263 6c61  [self.clustercla
-00016e80: 7373 5f6b 6579 5d29 0d0a 0d0a 0d0a 2020  ss_key])......  
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016eb0: 6966 206e 6f74 206d 6974 6f74 6963 3a0d  if not mitotic:.
-00016ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d50: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016d60: 7370 5f78 2e61 7070 656e 6428 616c 6c5f  sp_x.append(all_
+00016d70: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00016d80: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+00016d90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016db0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016dc0: 6963 5f72 6164 6975 732e 6170 7065 6e64  ic_radius.append
+00016dd0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00016de0: 735b 6b5d 5b73 656c 662e 7261 6469 7573  s[k][self.radius
+00016df0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e20: 6d69 746f 7469 635f 7370 6565 642e 6170  mitotic_speed.ap
+00016e30: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00016e40: 7261 636b 735b 6b5d 5b73 656c 662e 7370  racks[k][self.sp
+00016e50: 6565 645f 6b65 795d 290d 0a20 2020 2020  eed_key])..     
+00016e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e80: 2020 206d 6974 6f74 6963 5f61 6363 2e61     mitotic_acc.a
+00016e90: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00016ea0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e61  tracks[k][self.a
+00016eb0: 6363 656c 6572 6174 696f 6e5f 6b65 795d  cceleration_key]
+00016ec0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ee0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00016ef0: 6f74 6963 5f64 6973 705f 7a2e 6170 7065  otic_disp_z.appe
-00016f00: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00016f10: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
-00016f20: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00016f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ee0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016ef0: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+00016f00: 6861 6e67 652e 6170 7065 6e64 2861 6c6c  hange.append(all
+00016f10: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00016f20: 5b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  [self.motion_ang
+00016f30: 6c65 5f6b 6579 5d29 0d0a 2020 2020 2020  le_key])..      
 00016f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f50: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00016f60: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
-00016f70: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00016f80: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00016f90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fb0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016fc0: 6974 6f74 6963 5f64 6973 705f 782e 6170  itotic_disp_x.ap
-00016fd0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00016fe0: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
-00016ff0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00017000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017020: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017030: 7261 6469 7573 2e61 7070 656e 6428 616c  radius.append(al
-00017040: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017050: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
-00017060: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017080: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017090: 5f6d 6974 6f74 6963 5f73 7065 6564 2e61  _mitotic_speed.a
-000170a0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-000170b0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e73  tracks[k][self.s
-000170c0: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
+00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f60: 2020 6d69 746f 7469 635f 6469 7374 616e    mitotic_distan
+00016f70: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+00016f80: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00016f90: 6163 6b73 5b6b 5d5b 7365 6c66 2e64 6973  acks[k][self.dis
+00016fa0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
+00016fb0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00016fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00016fe0: 6620 7365 6c66 2e63 6c75 7374 6572 636c  f self.clustercl
+00016ff0: 6173 735f 6b65 7920 696e 2061 6c6c 5f73  ass_key in all_s
+00017000: 706f 7473 5f74 7261 636b 735b 6b5d 2e6b  pots_tracks[k].k
+00017010: 6579 7328 2920 3a0d 0a20 2020 2020 2020  eys() :..       
+00017020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017040: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00017050: 636c 7573 7465 725f 636c 6173 732e 6170  cluster_class.ap
+00017060: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017070: 7261 636b 735b 6b5d 5b73 656c 662e 636c  racks[k][self.cl
+00017080: 7573 7465 7263 6c61 7373 5f6b 6579 5d29  usterclass_key])
+00017090: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+000170a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170b0: 2020 2020 2020 2020 6966 206e 6f74 206d          if not m
+000170c0: 6974 6f74 6963 3a0d 0a20 2020 2020 2020  itotic:..       
 000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170f0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017100: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
+000170f0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00017100: 705f 7a2e 6170 7065 6e64 2861 6c6c 5f73  p_z.append(all_s
 00017110: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017120: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00017130: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00017120: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00017130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017160: 6e6f 6e5f 6d69 746f 7469 635f 6469 7265  non_mitotic_dire
-00017170: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
-00017180: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017190: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e6d  tracks[k][self.m
-000171a0: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
-000171b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000171c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171d0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-000171e0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
-000171f0: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-00017200: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017210: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
-00017220: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
-00017230: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017250: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00017260: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-00017270: 5f6b 6579 2069 6e20 616c 6c5f 7370 6f74  _key in all_spot
-00017280: 735f 7472 6163 6b73 5b6b 5d2e 6b65 7973  s_tracks[k].keys
-00017290: 2829 203a 0d0a 2020 2020 2020 2020 2020  () :..          
-000172a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172c0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000172d0: 5f63 6c75 7374 6572 5f63 6c61 7373 2e61  _cluster_class.a
-000172e0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-000172f0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e63  tracks[k][self.c
-00017300: 6c75 7374 6572 636c 6173 735f 6b65 795d  lusterclass_key]
-00017310: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00017320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017330: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00017340: 7a2e 6170 7065 6e64 2861 6c6c 5f73 706f  z.append(all_spo
-00017350: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017360: 662e 7a70 6f73 6964 5f6b 6579 5d29 0d0a  f.zposid_key])..
-00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017390: 2020 616c 6c5f 6469 7370 5f79 2e61 7070    all_disp_y.app
-000173a0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-000173b0: 6163 6b73 5b6b 5d5b 7365 6c66 2e79 706f  acks[k][self.ypo
-000173c0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00017150: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00017160: 746f 7469 635f 6469 7370 5f79 2e61 7070  totic_disp_y.app
+00017170: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017180: 6163 6b73 5b6b 5d5b 7365 6c66 2e79 706f  acks[k][self.ypo
+00017190: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+000171a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171c0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+000171d0: 6973 705f 782e 6170 7065 6e64 2861 6c6c  isp_x.append(all
+000171e0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+000171f0: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
+00017200: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017220: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00017230: 6d69 746f 7469 635f 7261 6469 7573 2e61  mitotic_radius.a
+00017240: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017250: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e72  tracks[k][self.r
+00017260: 6164 6975 735f 6b65 795d 290d 0a20 2020  adius_key])..   
+00017270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017290: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+000172a0: 5f73 7065 6564 2e61 7070 656e 6428 616c  _speed.append(al
+000172b0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000172c0: 5d5b 7365 6c66 2e73 7065 6564 5f6b 6579  ][self.speed_key
+000172d0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172f0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00017300: 6d69 746f 7469 635f 6163 632e 6170 7065  mitotic_acc.appe
+00017310: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017320: 636b 735b 6b5d 5b73 656c 662e 6163 6365  cks[k][self.acce
+00017330: 6c65 7261 7469 6f6e 5f6b 6579 5d29 0d0a  leration_key])..
+00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017360: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00017370: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
+00017380: 6368 616e 6765 2e61 7070 656e 6428 616c  change.append(al
+00017390: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000173a0: 5d5b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ][self.motion_an
+000173b0: 676c 655f 6b65 795d 290d 0a20 2020 2020  gle_key])..     
+000173c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173e0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-000173f0: 5f64 6973 705f 782e 6170 7065 6e64 2861  _disp_x.append(a
-00017400: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017410: 6b5d 5b73 656c 662e 7870 6f73 6964 5f6b  k][self.xposid_k
-00017420: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00017430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017440: 2020 2020 2020 2020 616c 6c5f 7261 6469          all_radi
-00017450: 7573 2e61 7070 656e 6428 616c 6c5f 7370  us.append(all_sp
-00017460: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017470: 6c66 2e72 6164 6975 735f 6b65 795d 290d  lf.radius_key]).
-00017480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174a0: 2020 2061 6c6c 5f73 7065 6564 2e61 7070     all_speed.app
-000174b0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-000174c0: 6163 6b73 5b6b 5d5b 7365 6c66 2e73 7065  acks[k][self.spe
-000174d0: 6564 5f6b 6579 5d29 0d0a 2020 2020 2020  ed_key])..      
-000174e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174f0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00017500: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
-00017510: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017520: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00017530: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017550: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-00017560: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00017570: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017580: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017590: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
-000175a0: 795d 2920 2020 0d0a 2020 2020 2020 2020  y])   ..        
-000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-000175d0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000175e0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-000175f0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017600: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
-00017610: 6173 6b5f 6b65 795d 290d 0a20 2020 2020  ask_key])..     
-00017620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017630: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00017640: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
-00017650: 735f 6b65 7920 696e 2061 6c6c 5f73 706f  s_key in all_spo
-00017660: 7473 5f74 7261 636b 735b 6b5d 2e6b 6579  ts_tracks[k].key
-00017670: 7328 2920 3a0d 0a20 2020 2020 2020 2020  s() :..         
-00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173e0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+000173f0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00017400: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
+00017410: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017420: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+00017430: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
+00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017460: 2020 2020 6966 2073 656c 662e 636c 7573      if self.clus
+00017470: 7465 7263 6c61 7373 5f6b 6579 2069 6e20  terclass_key in 
+00017480: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017490: 5b6b 5d2e 6b65 7973 2829 203a 0d0a 2020  [k].keys() :..  
+000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174c0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+000174d0: 5f6d 6974 6f74 6963 5f63 6c75 7374 6572  _mitotic_cluster
+000174e0: 5f63 6c61 7373 2e61 7070 656e 6428 616c  _class.append(al
+000174f0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017500: 5d5b 7365 6c66 2e63 6c75 7374 6572 636c  ][self.clustercl
+00017510: 6173 735f 6b65 795d 290d 0a0d 0a20 2020  ass_key])....   
+00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017530: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00017540: 6c6c 5f64 6973 705f 7a2e 6170 7065 6e64  ll_disp_z.append
+00017550: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017560: 735b 6b5d 5b73 656c 662e 7a70 6f73 6964  s[k][self.zposid
+00017570: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00017580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017590: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+000175a0: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
+000175b0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000175c0: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+000175d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175f0: 2020 2020 2061 6c6c 5f64 6973 705f 782e       all_disp_x.
+00017600: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017610: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017620: 7870 6f73 6964 5f6b 6579 5d29 0d0a 2020  xposid_key])..  
+00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017650: 616c 6c5f 7261 6469 7573 2e61 7070 656e  all_radius.appen
+00017660: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00017670: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
+00017680: 735f 6b65 795d 290d 0a20 2020 2020 2020  s_key])..       
 00017690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176a0: 2020 2020 2020 616c 6c5f 636c 7573 7465        all_cluste
-000176b0: 725f 636c 6173 732e 6170 7065 6e64 2861  r_class.append(a
-000176c0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000176d0: 6b5d 5b73 656c 662e 636c 7573 7465 7263  k][self.clusterc
-000176e0: 6c61 7373 5f6b 6579 5d29 2020 2020 0d0a  lass_key])    ..
+000176a0: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
+000176b0: 7065 6564 2e61 7070 656e 6428 616c 6c5f  peed.append(all_
+000176c0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000176d0: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
+000176e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000176f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017710: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00017720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017730: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00017740: 7370 5f7a 203d 206e 702e 6162 7328 6e70  sp_z = np.abs(np
-00017750: 2e64 6966 6628 6d69 746f 7469 635f 6469  .diff(mitotic_di
-00017760: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00017770: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00017780: 7469 635f 6469 7370 5f79 203d 206e 702e  tic_disp_y = np.
-00017790: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
-000177a0: 7469 635f 6469 7370 5f79 2929 0d0a 2020  tic_disp_y))..  
+00017700: 2020 2020 616c 6c5f 6163 632e 6170 7065      all_acc.appe
+00017710: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017720: 636b 735b 6b5d 5b73 656c 662e 6163 6365  cks[k][self.acce
+00017730: 6c65 7261 7469 6f6e 5f6b 6579 5d29 0d0a  leration_key])..
+00017740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017760: 2020 616c 6c5f 6469 7265 6374 696f 6e61    all_directiona
+00017770: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00017780: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017790: 5b6b 5d5b 7365 6c66 2e6d 6f74 696f 6e5f  [k][self.motion_
+000177a0: 616e 676c 655f 6b65 795d 2920 2020 0d0a  angle_key])   ..
 000177b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177c0: 2020 6d69 746f 7469 635f 6469 7370 5f78    mitotic_disp_x
-000177d0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
-000177e0: 6628 6d69 746f 7469 635f 6469 7370 5f78  f(mitotic_disp_x
-000177f0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00017800: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00017810: 746f 7469 635f 6469 7370 5f7a 203d 206e  totic_disp_z = n
-00017820: 702e 6162 7328 6e70 2e64 6966 6628 6e6f  p.abs(np.diff(no
-00017830: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
-00017840: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00017850: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00017860: 7469 635f 6469 7370 5f79 203d 206e 702e  tic_disp_y = np.
-00017870: 6162 7328 6e70 2e64 6966 6628 6e6f 6e5f  abs(np.diff(non_
-00017880: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
-00017890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000178a0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-000178b0: 635f 6469 7370 5f78 203d 206e 702e 6162  c_disp_x = np.ab
-000178c0: 7328 6e70 2e64 6966 6628 6e6f 6e5f 6d69  s(np.diff(non_mi
-000178d0: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
-000178e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000178f0: 2020 2020 2020 616c 6c5f 6469 7370 5f7a        all_disp_z
-00017900: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
-00017910: 6628 616c 6c5f 6469 7370 5f7a 2929 0d0a  f(all_disp_z))..
-00017920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017930: 2020 2020 616c 6c5f 6469 7370 5f79 203d      all_disp_y =
-00017940: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-00017950: 616c 6c5f 6469 7370 5f79 2929 0d0a 2020  all_disp_y))..  
-00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017970: 2020 616c 6c5f 6469 7370 5f78 203d 206e    all_disp_x = n
-00017980: 702e 6162 7328 6e70 2e64 6966 6628 616c  p.abs(np.diff(al
-00017990: 6c5f 6469 7370 5f78 2929 0d0a 0d0a 0d0a  l_disp_x))......
-000179a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000179d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000179e0: 6c66 2e74 696d 652e 6170 7065 6e64 2869  lf.time.append(i
-000179f0: 202a 2073 656c 662e 7463 616c 6962 7261   * self.tcalibra
-00017a00: 7469 6f6e 290d 0a0d 0a20 2020 2020 2020  tion)....       
-00017a10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017a20: 662e 6d69 746f 7469 635f 636c 7573 7465  f.mitotic_cluste
-00017a30: 725f 636c 6173 732e 6170 7065 6e64 286e  r_class.append(n
-00017a40: 702e 6173 6172 7261 7928 6d69 746f 7469  p.asarray(mitoti
-00017a50: 635f 636c 7573 7465 725f 636c 6173 732c  c_cluster_class,
-00017a60: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00017a70: 3229 290d 0a20 2020 2020 2020 2020 2020  2))..           
-00017a80: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00017a90: 6e5f 6d69 746f 7469 635f 636c 7573 7465  n_mitotic_cluste
-00017aa0: 725f 636c 6173 732e 6170 7065 6e64 286e  r_class.append(n
-00017ab0: 702e 6173 6172 7261 7928 6e6f 6e5f 6d69  p.asarray(non_mi
-00017ac0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00017ad0: 6173 732c 2064 7479 7065 3d6e 702e 666c  ass, dtype=np.fl
-00017ae0: 6f61 7433 3229 290d 0a20 2020 2020 2020  oat32))..       
-00017af0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017b00: 662e 616c 6c5f 636c 7573 7465 725f 636c  f.all_cluster_cl
-00017b10: 6173 732e 6170 7065 6e64 286e 702e 6173  ass.append(np.as
-00017b20: 6172 7261 7928 616c 6c5f 636c 7573 7465  array(all_cluste
-00017b30: 725f 636c 6173 732c 2064 7479 7065 3d6e  r_class, dtype=n
-00017b40: 702e 666c 6f61 7433 3229 290d 0a0d 0a20  p.float32)).... 
-00017b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b60: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00017b70: 6d65 616e 5f64 6973 705f 7a2e 6170 7065  mean_disp_z.appe
-00017b80: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
-00017b90: 6963 5f64 6973 705f 7a29 290d 0a20 2020  ic_disp_z))..   
-00017ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bb0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00017bc0: 725f 6469 7370 5f7a 2e61 7070 656e 6428  r_disp_z.append(
-00017bd0: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
-00017be0: 6973 705f 7a29 290d 0a0d 0a20 2020 2020  isp_z))....     
-00017bf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017c00: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00017c10: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
-00017c20: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
-00017c30: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
-00017c40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017c50: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00017c60: 7370 5f79 2e61 7070 656e 6428 6e70 2e73  sp_y.append(np.s
-00017c70: 7464 286d 6974 6f74 6963 5f64 6973 705f  td(mitotic_disp_
-00017c80: 7929 290d 0a0d 0a20 2020 2020 2020 2020  y))....         
-00017c90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017ca0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00017cb0: 705f 782e 6170 7065 6e64 286e 702e 6d65  p_x.append(np.me
-00017cc0: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
-00017cd0: 7829 290d 0a20 2020 2020 2020 2020 2020  x))..           
-00017ce0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00017cf0: 746f 7469 635f 7661 725f 6469 7370 5f78  totic_var_disp_x
-00017d00: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
-00017d10: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
-00017d20: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00017d30: 2020 2020 2020 2069 6620 6c65 6e28 6d69         if len(mi
-00017d40: 746f 7469 635f 7261 6469 7573 2920 3e20  totic_radius) > 
-00017d50: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00017d60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017d70: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 7261  .mitotic_mean_ra
-00017d80: 6469 7573 2e61 7070 656e 6428 6e70 2e6d  dius.append(np.m
-00017d90: 6561 6e28 6d69 746f 7469 635f 7261 6469  ean(mitotic_radi
-00017da0: 7573 2929 0d0a 2020 2020 2020 2020 2020  us))..          
-00017db0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017dc0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f72  lf.mitotic_var_r
-00017dd0: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00017de0: 7374 6428 6d69 746f 7469 635f 7261 6469  std(mitotic_radi
-00017df0: 7573 2929 0d0a 0d0a 2020 2020 2020 2020  us))....        
-00017e00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017e10: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 7370  .mitotic_mean_sp
-00017e20: 6565 642e 6170 7065 6e64 286e 702e 6d65  eed.append(np.me
-00017e30: 616e 286d 6974 6f74 6963 5f73 7065 6564  an(mitotic_speed
-00017e40: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00017e50: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00017e60: 6f74 6963 5f76 6172 5f73 7065 6564 2e61  otic_var_speed.a
-00017e70: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00017e80: 6f74 6963 5f73 7065 6564 2929 0d0a 0d0a  otic_speed))....
+000177c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177d0: 2020 616c 6c5f 6469 7374 616e 6365 5f63    all_distance_c
+000177e0: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+000177f0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017800: 5b6b 5d5b 7365 6c66 2e64 6973 7461 6e63  [k][self.distanc
+00017810: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 795d  e_cell_mask_key]
+00017820: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017840: 2020 2020 2069 6620 7365 6c66 2e63 6c75       if self.clu
+00017850: 7374 6572 636c 6173 735f 6b65 7920 696e  sterclass_key in
+00017860: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00017870: 735b 6b5d 2e6b 6579 7328 2920 3a0d 0a20  s[k].keys() :.. 
+00017880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178a0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+000178b0: 6c5f 636c 7573 7465 725f 636c 6173 732e  l_cluster_class.
+000178c0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+000178d0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+000178e0: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+000178f0: 5d29 2020 2020 0d0a 2020 2020 2020 2020  ])    ..        
+00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017920: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00017930: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00017940: 746f 7469 635f 6469 7370 5f7a 203d 206e  totic_disp_z = n
+00017950: 702e 6162 7328 6e70 2e64 6966 6628 6d69  p.abs(np.diff(mi
+00017960: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
+00017970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017980: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00017990: 5f79 203d 206e 702e 6162 7328 6e70 2e64  _y = np.abs(np.d
+000179a0: 6966 6628 6d69 746f 7469 635f 6469 7370  iff(mitotic_disp
+000179b0: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
+000179c0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000179d0: 635f 6469 7370 5f78 203d 206e 702e 6162  c_disp_x = np.ab
+000179e0: 7328 6e70 2e64 6966 6628 6d69 746f 7469  s(np.diff(mitoti
+000179f0: 635f 6469 7370 5f78 2929 0d0a 0d0a 2020  c_disp_x))....  
+00017a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a10: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+00017a20: 7370 5f7a 203d 206e 702e 6162 7328 6e70  sp_z = np.abs(np
+00017a30: 2e64 6966 6628 6e6f 6e5f 6d69 746f 7469  .diff(non_mitoti
+00017a40: 635f 6469 7370 5f7a 2929 0d0a 2020 2020  c_disp_z))..    
+00017a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a60: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00017a70: 5f79 203d 206e 702e 6162 7328 6e70 2e64  _y = np.abs(np.d
+00017a80: 6966 6628 6e6f 6e5f 6d69 746f 7469 635f  iff(non_mitotic_
+00017a90: 6469 7370 5f79 2929 0d0a 2020 2020 2020  disp_y))..      
+00017aa0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00017ab0: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
+00017ac0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+00017ad0: 6628 6e6f 6e5f 6d69 746f 7469 635f 6469  f(non_mitotic_di
+00017ae0: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+00017af0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017b00: 6c5f 6469 7370 5f7a 203d 206e 702e 6162  l_disp_z = np.ab
+00017b10: 7328 6e70 2e64 6966 6628 616c 6c5f 6469  s(np.diff(all_di
+00017b20: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+00017b30: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017b40: 6469 7370 5f79 203d 206e 702e 6162 7328  disp_y = np.abs(
+00017b50: 6e70 2e64 6966 6628 616c 6c5f 6469 7370  np.diff(all_disp
+00017b60: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
+00017b70: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00017b80: 7370 5f78 203d 206e 702e 6162 7328 6e70  sp_x = np.abs(np
+00017b90: 2e64 6966 6628 616c 6c5f 6469 7370 5f78  .diff(all_disp_x
+00017ba0: 2929 0d0a 0d0a 0d0a 2020 2020 2020 2020  ))......        
+00017bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017be0: 2020 2020 2020 7365 6c66 2e74 696d 652e        self.time.
+00017bf0: 6170 7065 6e64 2869 202a 2073 656c 662e  append(i * self.
+00017c00: 7463 616c 6962 7261 7469 6f6e 290d 0a0d  tcalibration)...
+00017c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017c20: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00017c30: 635f 636c 7573 7465 725f 636c 6173 732e  c_cluster_class.
+00017c40: 6170 7065 6e64 286e 702e 6173 6172 7261  append(np.asarra
+00017c50: 7928 6d69 746f 7469 635f 636c 7573 7465  y(mitotic_cluste
+00017c60: 725f 636c 6173 732c 2064 7479 7065 3d6e  r_class, dtype=n
+00017c70: 702e 666c 6f61 7433 3229 290d 0a20 2020  p.float32))..   
+00017c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c90: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00017ca0: 635f 636c 7573 7465 725f 636c 6173 732e  c_cluster_class.
+00017cb0: 6170 7065 6e64 286e 702e 6173 6172 7261  append(np.asarra
+00017cc0: 7928 6e6f 6e5f 6d69 746f 7469 635f 636c  y(non_mitotic_cl
+00017cd0: 7573 7465 725f 636c 6173 732c 2064 7479  uster_class, dty
+00017ce0: 7065 3d6e 702e 666c 6f61 7433 3229 290d  pe=np.float32)).
+00017cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017d00: 2020 2020 2073 656c 662e 616c 6c5f 636c       self.all_cl
+00017d10: 7573 7465 725f 636c 6173 732e 6170 7065  uster_class.appe
+00017d20: 6e64 286e 702e 6173 6172 7261 7928 616c  nd(np.asarray(al
+00017d30: 6c5f 636c 7573 7465 725f 636c 6173 732c  l_cluster_class,
+00017d40: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00017d50: 3229 290d 0a0d 0a20 2020 2020 2020 2020  2))....         
+00017d60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017d70: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00017d80: 705f 7a2e 6170 7065 6e64 286e 702e 6d65  p_z.append(np.me
+00017d90: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
+00017da0: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
+00017db0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00017dc0: 746f 7469 635f 7661 725f 6469 7370 5f7a  totic_var_disp_z
+00017dd0: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+00017de0: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
+00017df0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017e00: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017e10: 7469 635f 6d65 616e 5f64 6973 705f 792e  tic_mean_disp_y.
+00017e20: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00017e30: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
+00017e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017e50: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00017e60: 635f 7661 725f 6469 7370 5f79 2e61 7070  c_var_disp_y.app
+00017e70: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+00017e80: 6963 5f64 6973 705f 7929 290d 0a0d 0a20  ic_disp_y)).... 
 00017e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ea0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017eb0: 5f6d 6561 6e5f 6163 632e 6170 7065 6e64  _mean_acc.append
-00017ec0: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-00017ed0: 5f61 6363 2929 0d0a 2020 2020 2020 2020  _acc))..        
-00017ee0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017ef0: 2e6d 6974 6f74 6963 5f76 6172 5f61 6363  .mitotic_var_acc
-00017f00: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
-00017f10: 6974 6f74 6963 5f61 6363 2929 0d0a 0d0a  itotic_acc))....
-00017f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f30: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017f40: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
-00017f50: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-00017f60: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
-00017f70: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00017f80: 6765 2929 0d0a 2020 2020 2020 2020 2020  ge))..          
-00017f90: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017fa0: 6974 6f74 6963 5f76 6172 5f64 6972 6563  itotic_var_direc
-00017fb0: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
-00017fc0: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
-00017fd0: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
-00017fe0: 6368 616e 6765 2929 0d0a 0d0a 2020 2020  change))....    
-00017ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018000: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-00018010: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
-00018020: 6d61 736b 2e61 7070 656e 6428 6e70 2e6d  mask.append(np.m
-00018030: 6561 6e28 6d69 746f 7469 635f 6469 7374  ean(mitotic_dist
-00018040: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-00018050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018060: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018070: 6963 5f76 6172 5f64 6973 7461 6e63 655f  ic_var_distance_
-00018080: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-00018090: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-000180a0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000180b0: 736b 2929 0d0a 0d0a 2020 2020 2020 2020  sk))....        
-000180c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000180d0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-000180e0: 6e5f 6469 7370 5f7a 2e61 7070 656e 6428  n_disp_z.append(
-000180f0: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
-00018100: 7469 635f 6469 7370 5f7a 2929 0d0a 2020  tic_disp_z))..  
-00018110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018120: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00018130: 6963 5f76 6172 5f64 6973 705f 7a2e 6170  ic_var_disp_z.ap
-00018140: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-00018150: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
-00018160: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018170: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00018180: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00018190: 7370 5f79 2e61 7070 656e 6428 6e70 2e6d  sp_y.append(np.m
-000181a0: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
-000181b0: 6469 7370 5f79 2929 0d0a 2020 2020 2020  disp_y))..      
-000181c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000181d0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-000181e0: 6172 5f64 6973 705f 792e 6170 7065 6e64  ar_disp_y.append
-000181f0: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
-00018200: 7469 635f 6469 7370 5f79 2929 0d0a 0d0a  tic_disp_y))....
-00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018220: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00018230: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
-00018240: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018250: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00018260: 5f78 2929 0d0a 2020 2020 2020 2020 2020  _x))..          
-00018270: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018280: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00018290: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
-000182a0: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-000182b0: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
+00017ea0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00017eb0: 6d65 616e 5f64 6973 705f 782e 6170 7065  mean_disp_x.appe
+00017ec0: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+00017ed0: 6963 5f64 6973 705f 7829 290d 0a20 2020  ic_disp_x))..   
+00017ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ef0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00017f00: 725f 6469 7370 5f78 2e61 7070 656e 6428  r_disp_x.append(
+00017f10: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
+00017f20: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
+00017f30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017f40: 6620 6c65 6e28 6d69 746f 7469 635f 7261  f len(mitotic_ra
+00017f50: 6469 7573 2920 3e20 303a 0d0a 2020 2020  dius) > 0:..    
+00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f70: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00017f80: 5f6d 6561 6e5f 7261 6469 7573 2e61 7070  _mean_radius.app
+00017f90: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
+00017fa0: 7469 635f 7261 6469 7573 2929 0d0a 2020  tic_radius))..  
+00017fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fc0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00017fd0: 6963 5f76 6172 5f72 6164 6975 732e 6170  ic_var_radius.ap
+00017fe0: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
+00017ff0: 7469 635f 7261 6469 7573 2929 0d0a 0d0a  tic_radius))....
+00018000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018010: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018020: 5f6d 6561 6e5f 7370 6565 642e 6170 7065  _mean_speed.appe
+00018030: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+00018040: 6963 5f73 7065 6564 2929 0d0a 2020 2020  ic_speed))..    
+00018050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018060: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00018070: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
+00018080: 2e73 7464 286d 6974 6f74 6963 5f73 7065  .std(mitotic_spe
+00018090: 6564 2929 0d0a 0d0a 2020 2020 2020 2020  ed))....        
+000180a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000180b0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6163  .mitotic_mean_ac
+000180c0: 632e 6170 7065 6e64 286e 702e 6d65 616e  c.append(np.mean
+000180d0: 286d 6974 6f74 6963 5f61 6363 2929 0d0a  (mitotic_acc))..
+000180e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180f0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018100: 5f76 6172 5f61 6363 2e61 7070 656e 6428  _var_acc.append(
+00018110: 6e70 2e73 7464 286d 6974 6f74 6963 5f61  np.std(mitotic_a
+00018120: 6363 2929 0d0a 0d0a 2020 2020 2020 2020  cc))....        
+00018130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018140: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00018150: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00018160: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018170: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+00018180: 6e61 6c5f 6368 616e 6765 2929 0d0a 2020  nal_change))..  
+00018190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181a0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+000181b0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+000181c0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+000181d0: 7374 6428 6d69 746f 7469 635f 6469 7265  std(mitotic_dire
+000181e0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
+000181f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018200: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018210: 6f74 6963 5f6d 6561 6e5f 6469 7374 616e  otic_mean_distan
+00018220: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+00018230: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
+00018240: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
+00018250: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
+00018260: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018270: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+00018280: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00018290: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
+000182a0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+000182b0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
 000182c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182d0: 6966 206c 656e 286e 6f6e 5f6d 6974 6f74  if len(non_mitot
-000182e0: 6963 5f72 6164 6975 7329 203e 2030 3a0d  ic_radius) > 0:.
-000182f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018300: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00018310: 6e5f 6d69 746f 7469 635f 6d65 616e 5f72  n_mitotic_mean_r
-00018320: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00018330: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-00018340: 5f72 6164 6975 7329 290d 0a20 2020 2020  _radius))..     
-00018350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018360: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00018370: 7469 635f 7661 725f 7261 6469 7573 2e61  tic_var_radius.a
-00018380: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
-00018390: 5f6d 6974 6f74 6963 5f72 6164 6975 7329  _mitotic_radius)
-000183a0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000183b0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000183c0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f73  n_mitotic_mean_s
-000183d0: 7065 6564 2e61 7070 656e 6428 6e70 2e6d  peed.append(np.m
-000183e0: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
-000183f0: 7370 6565 6429 290d 0a20 2020 2020 2020  speed))..       
-00018400: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018410: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00018420: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
-00018430: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-00018440: 635f 7370 6565 6429 290d 0a0d 0a20 2020  c_speed))....   
-00018450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018460: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00018470: 635f 6d65 616e 5f61 6363 2e61 7070 656e  c_mean_acc.appen
-00018480: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-00018490: 746f 7469 635f 6163 6329 290d 0a20 2020  totic_acc))..   
-000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184b0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-000184c0: 635f 7661 725f 6163 632e 6170 7065 6e64  c_var_acc.append
-000184d0: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
-000184e0: 7469 635f 6163 6329 290d 0a0d 0a20 2020  tic_acc))....   
-000184f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018500: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00018510: 635f 6d65 616e 5f64 6972 6563 7469 6f6e  c_mean_direction
-00018520: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-00018530: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00018540: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
-00018550: 5f63 6861 6e67 6529 290d 0a20 2020 2020  _change))..     
-00018560: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018570: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00018580: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
-00018590: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-000185a0: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-000185b0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000185c0: 6e67 6529 2920 0d0a 0d0a 2020 2020 2020  nge)) ....      
-000185d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000185e0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-000185f0: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00018600: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
-00018610: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018620: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00018630: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
-00018640: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018650: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018660: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018670: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
-00018680: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-00018690: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000186a0: 2929 0d0a 0d0a 0d0a 2020 2020 2020 2020  ))......        
-000186b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000186c0: 2e61 6c6c 5f6d 6561 6e5f 6469 7370 5f7a  .all_mean_disp_z
-000186d0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-000186e0: 616c 6c5f 6469 7370 5f7a 2929 0d0a 2020  all_disp_z))..  
-000186f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018700: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00018710: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
-00018720: 7374 6428 616c 6c5f 6469 7370 5f7a 2929  std(all_disp_z))
-00018730: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018740: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018750: 5f6d 6561 6e5f 6469 7370 5f79 2e61 7070  _mean_disp_y.app
-00018760: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-00018770: 6469 7370 5f79 2929 0d0a 2020 2020 2020  disp_y))..      
-00018780: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018790: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
-000187a0: 792e 6170 7065 6e64 286e 702e 7374 6428  y.append(np.std(
-000187b0: 616c 6c5f 6469 7370 5f79 2929 0d0a 0d0a  all_disp_y))....
-000187c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187d0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-000187e0: 6e5f 6469 7370 5f78 2e61 7070 656e 6428  n_disp_x.append(
-000187f0: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7370  np.mean(all_disp
-00018800: 5f78 2929 0d0a 2020 2020 2020 2020 2020  _x))..          
-00018810: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00018820: 6c6c 5f76 6172 5f64 6973 705f 782e 6170  ll_var_disp_x.ap
-00018830: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-00018840: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
-00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018860: 6966 206c 656e 2861 6c6c 5f72 6164 6975  if len(all_radiu
-00018870: 7329 203e 2030 3a0d 0a20 2020 2020 2020  s) > 0:..       
-00018880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018890: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-000188a0: 616e 5f72 6164 6975 732e 6170 7065 6e64  an_radius.append
-000188b0: 286e 702e 6d65 616e 2861 6c6c 5f72 6164  (np.mean(all_rad
-000188c0: 6975 7329 290d 0a20 2020 2020 2020 2020  ius))..         
-000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188e0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-000188f0: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
-00018900: 2e73 7464 2861 6c6c 5f72 6164 6975 7329  .std(all_radius)
-00018910: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018920: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018930: 6c5f 6d65 616e 5f73 7065 6564 2e61 7070  l_mean_speed.app
-00018940: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-00018950: 7370 6565 6429 290d 0a20 2020 2020 2020  speed))..       
-00018960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018970: 662e 616c 6c5f 7661 725f 7370 6565 642e  f.all_var_speed.
-00018980: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-00018990: 6c5f 7370 6565 6429 290d 0a0d 0a20 2020  l_speed))....   
-000189a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189b0: 2073 656c 662e 616c 6c5f 6d65 616e 5f61   self.all_mean_a
-000189c0: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
-000189d0: 6e28 616c 6c5f 6163 6329 290d 0a20 2020  n(all_acc))..   
-000189e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189f0: 2073 656c 662e 616c 6c5f 7661 725f 6163   self.all_var_ac
-00018a00: 632e 6170 7065 6e64 286e 702e 7374 6428  c.append(np.std(
-00018a10: 616c 6c5f 6163 6329 290d 0a0d 0a0d 0a0d  all_acc)).......
-00018a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018a30: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018a40: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-00018a50: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00018a60: 6d65 616e 2861 6c6c 5f64 6972 6563 7469  mean(all_directi
-00018a70: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
-00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a90: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00018aa0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018ab0: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
-00018ac0: 2861 6c6c 5f64 6972 6563 7469 6f6e 616c  (all_directional
-00018ad0: 5f63 6861 6e67 6529 290d 0a0d 0a20 2020  _change))....   
-00018ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018af0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00018b00: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00018b10: 6b2e 6170 7065 6e64 286e 702e 6d65 616e  k.append(np.mean
-00018b20: 2861 6c6c 5f64 6973 7461 6e63 655f 6365  (all_distance_ce
-00018b30: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-00018b40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018b50: 656c 662e 616c 6c5f 7661 725f 6469 7374  elf.all_var_dist
-00018b60: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00018b70: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00018b80: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018b90: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
-00018ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018bb0: 2020 200d 0a20 2020 2020 2020 200d 0a64     ..        ..d
-00018bc0: 6566 2062 6f75 6e64 6172 795f 706f 696e  ef boundary_poin
-00018bd0: 7473 286d 6173 6b2c 2078 6361 6c69 6272  ts(mask, xcalibr
-00018be0: 6174 696f 6e2c 2079 6361 6c69 6272 6174  ation, ycalibrat
-00018bf0: 696f 6e2c 207a 6361 6c69 6272 6174 696f  ion, zcalibratio
-00018c00: 6e29 3a0d 0a0d 0a20 2020 206e 6469 6d20  n):....    ndim 
-00018c10: 3d20 6c65 6e28 6d61 736b 2e73 6861 7065  = len(mask.shape
-00018c20: 290d 0a20 2020 2074 696d 6564 5f6d 6173  )..    timed_mas
-00018c30: 6b20 3d20 7b7d 0d0a 2020 2020 6d61 736b  k = {}..    mask
-00018c40: 203d 206d 6173 6b20 3e20 300d 0a20 2020   = mask > 0..   
-00018c50: 206d 6173 6b20 3d20 6d61 736b 2e61 7374   mask = mask.ast
-00018c60: 7970 6528 2775 696e 7438 2729 0d0a 2020  ype('uint8')..  
-00018c70: 2020 2320 5958 2073 6861 7065 6420 6f62    # YX shaped ob
-00018c80: 6a65 6374 0d0a 2020 2020 6966 206e 6469  ject..    if ndi
-00018c90: 6d20 3d3d 2032 3a0d 0a20 2020 2020 2020  m == 2:..       
-00018ca0: 200d 0a20 2020 2020 2020 2062 6f75 6e64   ..        bound
-00018cb0: 6172 7920 3d20 6669 6e64 5f62 6f75 6e64  ary = find_bound
-00018cc0: 6172 6965 7328 6d61 736b 290d 0a20 2020  aries(mask)..   
-00018cd0: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
-00018ce0: 6f69 6420 3d20 2830 2c29 202b 2063 6f6d  oid = (0,) + com
-00018cf0: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
-00018d00: 756e 6461 7279 2920 0d0a 2020 2020 2020  undary) ..      
-00018d10: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-00018d20: 6865 7265 2862 6f75 6e64 6172 7920 3e20  here(boundary > 
-00018d30: 3029 0d0a 2020 2020 2020 2020 7265 616c  0)..        real
-00018d40: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
-00018d50: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
-00018d60: 6179 2869 6e64 6963 6573 2c20 6474 7970  ay(indices, dtyp
-00018d70: 653d 6e70 2e66 6c6f 6174 3332 2929 2e63  e=np.float32)).c
-00018d80: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
-00018d90: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-00018da0: 302c 206c 656e 2872 6561 6c5f 696e 6469  0, len(real_indi
-00018db0: 6365 7329 293a 0d0a 0d0a 2020 2020 2020  ces)):....      
-00018dc0: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-00018dd0: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
-00018de0: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
-00018df0: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
-00018e00: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-00018e10: 6e64 6963 6573 5b6a 5d5b 315d 203d 2072  ndices[j][1] = r
-00018e20: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
-00018e30: 5d20 2a20 7863 616c 6962 7261 7469 6f6e  ] * xcalibration
-00018e40: 0d0a 0d0a 2020 2020 2020 2020 7472 6565  ....        tree
-00018e50: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
-00018e60: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
-00018e70: 0d0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
-00018e80: 206f 626a 6563 7420 636f 6e74 6169 6e73   object contains
-00018e90: 206c 6973 7420 6f66 2061 6c6c 2074 6865   list of all the
-00018ea0: 2070 6f69 6e74 7320 666f 7220 616c 6c20   points for all 
-00018eb0: 7468 6520 6c61 6265 6c73 2069 6e20 7468  the labels in th
-00018ec0: 6520 4d61 736b 2069 6d61 6765 2077 6974  e Mask image wit
-00018ed0: 6820 7468 6520 6c61 6265 6c20 6964 2061  h the label id a
-00018ee0: 6e64 2076 6f6c 756d 6520 6f66 2065 6163  nd volume of eac
-00018ef0: 6820 6c61 6265 6c0d 0a20 2020 2020 2020  h label..       
-00018f00: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
-00018f10: 3029 5d20 3d20 5b74 7265 652c 2069 6e64  0)] = [tree, ind
-00018f20: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
-00018f30: 726f 6964 5d0d 0a0d 0a20 2020 2023 2054  roid]....    # T
-00018f40: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
-00018f50: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
-00018f60: 2033 3a0d 0a0d 0a0d 0a20 2020 2020 2020   3:......       
-00018f70: 2066 6f72 2069 2069 6e20 7471 646d 2872   for i in tqdm(r
-00018f80: 616e 6765 2830 2c20 6d61 736b 2e73 6861  ange(0, mask.sha
-00018f90: 7065 5b30 5d29 293a 0d0a 2020 2020 2020  pe[0])):..      
-00018fa0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00018fb0: 2020 2020 2020 2020 2020 2020 626f 756e              boun
-00018fc0: 6461 7279 203d 2066 696e 645f 626f 756e  dary = find_boun
-00018fd0: 6461 7269 6573 286d 6173 6b5b 692c 3a5d  daries(mask[i,:]
-00018fe0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018ff0: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
-00019000: 6420 3d20 2830 2c29 202b 2063 6f6d 7075  d = (0,) + compu
-00019010: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
-00019020: 6461 7279 2920 0d0a 2020 2020 2020 2020  dary) ..        
-00019030: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-00019040: 3d20 6e70 2e77 6865 7265 2862 6f75 6e64  = np.where(bound
-00019050: 6172 7920 3e20 3029 0d0a 2020 2020 2020  ary > 0)..      
-00019060: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-00019070: 6e64 6963 6573 203d 206e 702e 7472 616e  ndices = np.tran
-00019080: 7370 6f73 6528 6e70 2e61 7361 7272 6179  spose(np.asarray
-00019090: 2869 6e64 6963 6573 2c20 6474 7970 653d  (indices, dtype=
-000190a0: 6e70 2e66 6c6f 6174 3332 2929 2e63 6f70  np.float32)).cop
-000190b0: 7928 290d 0a0d 0a20 2020 2020 2020 2020  y()....         
-000190c0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-000190d0: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
-000190e0: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
-000190f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019100: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-00019110: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
-00019120: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
-00019130: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00019140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019150: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-00019160: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
-00019170: 735b 6a5d 5b31 5d20 2a20 7863 616c 6962  s[j][1] * xcalib
-00019180: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
-00019190: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
-000191a0: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-000191b0: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
-000191c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000191d0: 2020 7469 6d65 645f 6d61 736b 5b73 7472    timed_mask[str
-000191e0: 2869 295d 203d 205b 7472 6565 2c20 696e  (i)] = [tree, in
-000191f0: 6469 6365 732c 2072 6567 696f 6e63 656e  dices, regioncen
-00019200: 7472 6f69 645d 0d0a 2020 2020 2020 2020  troid]..        
-00019210: 2020 2020 0d0a 2020 2020 2320 545a 5958      ..    # TZYX
-00019220: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
-00019230: 2020 2020 6966 206e 6469 6d20 3d3d 2034      if ndim == 4
-00019240: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
-00019250: 2827 4d61 736b 7320 6d61 6465 2069 6e74  ('Masks made int
-00019260: 6f20 6120 3444 2063 796c 696e 6465 722c  o a 4D cylinder,
-00019270: 2075 7027 290d 0a20 2020 2020 2020 2062   up')..        b
-00019280: 6f75 6e64 6172 7920 3d20 6e70 2e7a 6572  oundary = np.zer
-00019290: 6f73 280d 0a20 2020 2020 2020 2020 2020  os(..           
-000192a0: 205b 6d61 736b 2e73 6861 7065 5b30 5d2c   [mask.shape[0],
-000192b0: 206d 6173 6b2e 7368 6170 655b 315d 2c20   mask.shape[1], 
-000192c0: 6d61 736b 2e73 6861 7065 5b32 5d2c 206d  mask.shape[2], m
-000192d0: 6173 6b2e 7368 6170 655b 335d 5d0d 0a20  ask.shape[3]].. 
-000192e0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000192f0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00019300: 2830 2c20 6d61 736b 2e73 6861 7065 5b30  (0, mask.shape[0
-00019310: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
-00019320: 200d 0a20 2020 2020 2020 2020 2020 2062   ..            b
-00019330: 6f75 6e64 6172 795b 692c 3a5d 203d 2066  oundary[i,:] = f
-00019340: 696e 645f 626f 756e 6461 7269 6573 286d  ind_boundaries(m
-00019350: 6173 6b5b 692c 3a5d 290d 0a20 2020 2020  ask[i,:])..     
-00019360: 2020 2020 2020 2072 6567 696f 6e63 656e         regioncen
-00019370: 7472 6f69 6420 3d20 636f 6d70 7574 655f  troid = compute_
-00019380: 6365 6e74 726f 6964 2862 6f75 6e64 6172  centroid(boundar
-00019390: 795b 692c 3a5d 2920 0d0a 2020 2020 2020  y[i,:]) ..      
-000193a0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-000193b0: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
-000193c0: 795b 692c 3a5d 203e 2030 290d 0a20 2020  y[i,:] > 0)..   
-000193d0: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-000193e0: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
-000193f0: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
-00019400: 696e 6469 6365 732c 2064 7479 7065 3d6e  indices, dtype=n
-00019410: 702e 666c 6f61 7433 3229 292e 636f 7079  p.float32)).copy
-00019420: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-00019430: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
-00019440: 2830 2c20 6c65 6e28 7265 616c 5f69 6e64  (0, len(real_ind
-00019450: 6963 6573 2929 3a0d 0a0d 0a20 2020 2020  ices)):....     
-00019460: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00019470: 6561 6c5f 696e 6469 6365 735b 6a5d 5b30  eal_indices[j][0
-00019480: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
-00019490: 5b6a 5d5b 305d 202a 207a 6361 6c69 6272  [j][0] * zcalibr
-000194a0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-000194b0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-000194c0: 696e 6469 6365 735b 6a5d 5b31 5d20 3d20  indices[j][1] = 
-000194d0: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-000194e0: 315d 202a 2079 6361 6c69 6272 6174 696f  1] * ycalibratio
-000194f0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00019500: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-00019510: 6365 735b 6a5d 5b32 5d20 3d20 7265 616c  ces[j][2] = real
-00019520: 5f69 6e64 6963 6573 5b6a 5d5b 325d 202a  _indices[j][2] *
-00019530: 2078 6361 6c69 6272 6174 696f 6e0d 0a0d   xcalibration...
-00019540: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
-00019550: 6520 3d20 7370 6174 6961 6c2e 634b 4454  e = spatial.cKDT
-00019560: 7265 6528 7265 616c 5f69 6e64 6963 6573  ree(real_indices
-00019570: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00019580: 696d 6564 5f6d 6173 6b5b 7374 7228 6929  imed_mask[str(i)
-00019590: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
-000195a0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
-000195b0: 6964 5d0d 0a20 2020 2070 7269 6e74 2827  id]..    print('
-000195c0: 436f 6d70 7574 6564 2074 6865 2062 6f75  Computed the bou
-000195d0: 6e64 6172 7920 706f 696e 7473 2729 0d0a  ndary points')..
-000195e0: 0d0a 2020 2020 7265 7475 726e 2074 696d  ..    return tim
-000195f0: 6564 5f6d 6173 6b2c 2062 6f75 6e64 6172  ed_mask, boundar
-00019600: 7920 2020 2020 2020 200d 0a0d 0a64 6566  y        ....def
-00019610: 2063 6f6d 7075 7465 5f63 656e 7472 6f69   compute_centroi
-00019620: 6428 6269 6e61 7279 5f69 6d61 6765 293a  d(binary_image):
-00019630: 0d0a 2020 2020 2320 456e 7375 7265 2062  ..    # Ensure b
-00019640: 696e 6172 7920 696d 6167 6520 6973 2061  inary image is a
-00019650: 204e 756d 5079 2061 7272 6179 0d0a 2020   NumPy array..  
-00019660: 2020 6269 6e61 7279 5f69 6d61 6765 203d    binary_image =
-00019670: 206e 702e 6172 7261 7928 6269 6e61 7279   np.array(binary
-00019680: 5f69 6d61 6765 290d 0a0d 0a20 2020 2077  _image)....    w
-00019690: 6869 7465 5f70 6978 656c 7320 3d20 6e70  hite_pixels = np
-000196a0: 2e77 6865 7265 2862 696e 6172 795f 696d  .where(binary_im
-000196b0: 6167 6520 3d3d 2031 290d 0a20 2020 206e  age == 1)..    n
-000196c0: 756d 5f70 6978 656c 7320 3d20 6c65 6e28  um_pixels = len(
-000196d0: 7768 6974 655f 7069 7865 6c73 5b30 5d29  white_pixels[0])
-000196e0: 0d0a 0d0a 2020 2020 2320 436f 6d70 7574  ....    # Comput
-000196f0: 6520 7468 6520 6365 6e74 726f 6964 206f  e the centroid o
-00019700: 6620 7468 6520 7768 6974 6520 7069 7865  f the white pixe
-00019710: 6c73 2069 6e20 7468 6520 626f 756e 6461  ls in the bounda
-00019720: 7279 2069 6d61 6765 0d0a 2020 2020 6365  ry image..    ce
-00019730: 6e74 726f 6964 203d 206e 702e 7a65 726f  ntroid = np.zero
-00019740: 7328 6269 6e61 7279 5f69 6d61 6765 2e6e  s(binary_image.n
-00019750: 6469 6d29 0d0a 2020 2020 666f 7220 6469  dim)..    for di
-00019760: 6d20 696e 2072 616e 6765 2862 696e 6172  m in range(binar
-00019770: 795f 696d 6167 652e 6e64 696d 293a 0d0a  y_image.ndim):..
-00019780: 2020 2020 2020 2020 6365 6e74 726f 6964          centroid
-00019790: 5b64 696d 5d20 3d20 7768 6974 655f 7069  [dim] = white_pi
-000197a0: 7865 6c73 5b64 696d 5d2e 7375 6d28 2920  xels[dim].sum() 
-000197b0: 2f20 6e75 6d5f 7069 7865 6c73 0d0a 0d0a  / num_pixels....
-000197c0: 2020 2020 7265 7475 726e 2063 656e 7472      return centr
-000197d0: 6f69 640d 0a0d 0a0d 0a0d 0a20 0d0a 0d0a  oid........ ....
-000197e0: 6465 6620 6765 745f 6373 765f 6461 7461  def get_csv_data
-000197f0: 2863 7376 293a 0d0a 0d0a 2020 2020 2020  (csv):....      
-00019800: 2020 6461 7461 7365 7420 3d20 7064 2e72    dataset = pd.r
-00019810: 6561 645f 6373 7628 0d0a 2020 2020 2020  ead_csv(..      
-00019820: 2020 2020 2020 6373 762c 2064 656c 696d        csv, delim
-00019830: 6974 6572 3d22 2c22 2c20 656e 636f 6469  iter=",", encodi
-00019840: 6e67 3d22 756e 6963 6f64 655f 6573 6361  ng="unicode_esca
-00019850: 7065 222c 206c 6f77 5f6d 656d 6f72 793d  pe", low_memory=
-00019860: 4661 6c73 650d 0a20 2020 2020 2020 2029  False..        )
-00019870: 5b33 3a5d 0d0a 2020 2020 2020 2020 6461  [3:]..        da
-00019880: 7461 7365 745f 696e 6465 7820 3d20 6461  taset_index = da
-00019890: 7461 7365 742e 696e 6465 780d 0a20 2020  taset.index..   
-000198a0: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
-000198b0: 7365 742c 2064 6174 6173 6574 5f69 6e64  set, dataset_ind
-000198c0: 6578 0d0a 2020 2020 0d0a 6465 6620 6765  ex..    ..def ge
-000198d0: 745f 7370 6f74 5f64 6174 6173 6574 2873  t_spot_dataset(s
-000198e0: 706f 745f 6461 7461 7365 742c 2074 7261  pot_dataset, tra
-000198f0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00019900: 5f6b 6579 732c 2078 6361 6c69 6272 6174  _keys, xcalibrat
-00019910: 696f 6e2c 2079 6361 6c69 6272 6174 696f  ion, ycalibratio
-00019920: 6e2c 207a 6361 6c69 6272 6174 696f 6e2c  n, zcalibration,
-00019930: 2041 7474 7269 6275 7465 426f 786e 616d   AttributeBoxnam
-00019940: 652c 2064 6574 6563 7469 6f6e 6368 616e  e, detectionchan
-00019950: 6e65 6c29 3a0d 0a20 2020 2020 2020 2041  nel):..        A
-00019960: 6c6c 5661 6c75 6573 203d 207b 7d0d 0a20  llValues = {}.. 
-00019970: 2020 2020 2020 2070 6f73 6978 203d 2074         posix = t
-00019980: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00019990: 6f74 5f6b 6579 735b 2270 6f73 6978 225d  ot_keys["posix"]
-000199a0: 0d0a 2020 2020 2020 2020 706f 7369 7920  ..        posiy 
-000199b0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-000199c0: 5f73 706f 745f 6b65 7973 5b22 706f 7369  _spot_keys["posi
-000199d0: 7922 5d0d 0a20 2020 2020 2020 2070 6f73  y"]..        pos
-000199e0: 697a 203d 2074 7261 636b 5f61 6e61 6c79  iz = track_analy
-000199f0: 7369 735f 7370 6f74 5f6b 6579 735b 2270  sis_spot_keys["p
-00019a00: 6f73 697a 225d 0d0a 2020 2020 2020 2020  osiz"]..        
-00019a10: 6672 616d 6520 3d20 7472 6163 6b5f 616e  frame = track_an
-00019a20: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00019a30: 5b22 6672 616d 6522 5d0d 0a20 2020 2020  ["frame"]..     
-00019a40: 2020 200d 0a20 2020 2020 2020 204c 6f63     ..        Loc
-00019a50: 6174 696f 6e58 203d 2028 0d0a 2020 2020  ationX = (..    
-00019a60: 2020 2020 2020 2020 7370 6f74 5f64 6174          spot_dat
-00019a70: 6173 6574 5b70 6f73 6978 5d2e 6173 7479  aset[posix].asty
-00019a80: 7065 2822 666c 6f61 7422 2920 2f20 7863  pe("float") / xc
-00019a90: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00019aa0: 2020 2020 292e 6173 7479 7065 2822 696e      ).astype("in
-00019ab0: 7422 290d 0a20 2020 2020 2020 204c 6f63  t")..        Loc
-00019ac0: 6174 696f 6e59 203d 2028 0d0a 2020 2020  ationY = (..    
-00019ad0: 2020 2020 2020 2020 7370 6f74 5f64 6174          spot_dat
-00019ae0: 6173 6574 5b70 6f73 6979 5d2e 6173 7479  aset[posiy].asty
-00019af0: 7065 2822 666c 6f61 7422 2920 2f20 7963  pe("float") / yc
-00019b00: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00019b10: 2020 2020 292e 6173 7479 7065 2822 696e      ).astype("in
-00019b20: 7422 290d 0a20 2020 2020 2020 204c 6f63  t")..        Loc
-00019b30: 6174 696f 6e5a 203d 2028 0d0a 2020 2020  ationZ = (..    
-00019b40: 2020 2020 2020 2020 7370 6f74 5f64 6174          spot_dat
-00019b50: 6173 6574 5b70 6f73 697a 5d2e 6173 7479  aset[posiz].asty
-00019b60: 7065 2822 666c 6f61 7422 2920 2f20 7a63  pe("float") / zc
-00019b70: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00019b80: 2020 2020 292e 6173 7479 7065 2822 696e      ).astype("in
-00019b90: 7422 290d 0a20 2020 2020 2020 204c 6f63  t")..        Loc
-00019ba0: 6174 696f 6e54 203d 2028 7370 6f74 5f64  ationT = (spot_d
-00019bb0: 6174 6173 6574 5b66 7261 6d65 5d2e 6173  ataset[frame].as
-00019bc0: 7479 7065 2822 666c 6f61 7422 2929 2e61  type("float")).a
-00019bd0: 7374 7970 6528 2269 6e74 2229 0d0a 2020  stype("int")..  
-00019be0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00019bf0: 2020 6967 6e6f 7265 5f76 616c 7565 7320    ignore_values 
-00019c00: 3d20 5b74 7261 636b 5f61 6e61 6c79 7369  = [track_analysi
-00019c10: 735f 7370 6f74 5f6b 6579 735b 226d 6561  s_spot_keys["mea
-00019c20: 6e5f 696e 7465 6e73 6974 7922 5d2c 7472  n_intensity"],tr
-00019c30: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00019c40: 745f 6b65 7973 5b22 746f 7461 6c5f 696e  t_keys["total_in
-00019c50: 7465 6e73 6974 7922 5d5d 200d 0a20 2020  tensity"]] ..   
-00019c60: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
-00019c70: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
-00019c80: 5f73 706f 745f 6b65 7973 2e69 7465 6d73  _spot_keys.items
-00019c90: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
-00019ca0: 2020 2020 2020 2069 6620 6465 7465 6374         if detect
-00019cb0: 696f 6e63 6861 6e6e 656c 203d 3d20 313a  ionchannel == 1:
-00019cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019cd0: 2020 2020 2020 2069 6620 6b20 3d3d 2022         if k == "
-00019ce0: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
-00019cf0: 6832 223a 0d0a 2020 2020 2020 2020 2020  h2":..          
-00019d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d10: 2076 616c 7565 203d 2074 7261 636b 5f61   value = track_a
-00019d20: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-00019d30: 735b 226d 6561 6e5f 696e 7465 6e73 6974  s["mean_intensit
-00019d40: 7922 5d0d 0a20 2020 2020 2020 2020 2020  y"]..           
-00019d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d60: 416c 6c56 616c 7565 735b 7661 6c75 655d  AllValues[value]
-00019d70: 203d 2073 706f 745f 6461 7461 7365 745b   = spot_dataset[
-00019d80: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
-00019d90: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00019da0: 2020 2020 2020 2020 2069 6620 6b20 3d3d           if k ==
-00019db0: 2022 746f 7461 6c5f 696e 7465 6e73 6974   "total_intensit
-00019dc0: 795f 6368 3222 3a0d 0a20 2020 2020 2020  y_ch2":..       
-00019dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019de0: 2020 2020 7661 6c75 6520 3d20 7472 6163      value = trac
-00019df0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00019e00: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
-00019e10: 6e73 6974 7922 5d0d 0a20 2020 2020 2020  nsity"]..       
-00019e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e30: 2020 2020 416c 6c56 616c 7565 735b 7661      AllValues[va
-00019e40: 6c75 655d 203d 2073 706f 745f 6461 7461  lue] = spot_data
-00019e50: 7365 745b 765d 2e61 7374 7970 6528 2266  set[v].astype("f
-00019e60: 6c6f 6174 2229 2020 2020 2020 200d 0a0d  loat")       ...
-00019e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019e80: 2069 6620 7620 6e6f 7420 696e 2069 676e   if v not in ign
-00019e90: 6f72 655f 7661 6c75 6573 3a0d 0a20 2020  ore_values:..   
-00019ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019eb0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00019ec0: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
-00019ed0: 5661 6c75 6573 5b76 5d20 3d20 7370 6f74  Values[v] = spot
-00019ee0: 5f64 6174 6173 6574 5b76 5d2e 6173 7479  _dataset[v].asty
-00019ef0: 7065 2822 666c 6f61 7422 290d 0a0d 0a20  pe("float").... 
-00019f00: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-00019f10: 5b70 6f73 6978 5d20 3d20 726f 756e 6428  [posix] = round(
-00019f20: 4c6f 6361 7469 6f6e 582c 3329 0d0a 2020  LocationX,3)..  
-00019f30: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-00019f40: 706f 7369 795d 203d 2072 6f75 6e64 284c  posiy] = round(L
-00019f50: 6f63 6174 696f 6e59 2c33 290d 0a20 2020  ocationY,3)..   
-00019f60: 2020 2020 2041 6c6c 5661 6c75 6573 5b70       AllValues[p
-00019f70: 6f73 697a 5d20 3d20 726f 756e 6428 4c6f  osiz] = round(Lo
-00019f80: 6361 7469 6f6e 5a2c 3329 0d0a 2020 2020  cationZ,3)..    
-00019f90: 2020 2020 416c 6c56 616c 7565 735b 6672      AllValues[fr
-00019fa0: 616d 655d 203d 2072 6f75 6e64 284c 6f63  ame] = round(Loc
-00019fb0: 6174 696f 6e54 2c33 290d 0a20 2020 2020  ationT,3)..     
-00019fc0: 2020 2041 7474 7269 6275 7465 6964 7320     Attributeids 
-00019fd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 4174  = []..        At
-00019fe0: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
-00019ff0: 6428 4174 7472 6962 7574 6542 6f78 6e61  d(AttributeBoxna
-0001a000: 6d65 290d 0a20 2020 2020 2020 2066 6f72  me)..        for
-0001a010: 2061 7474 7269 6275 7465 6e61 6d65 2069   attributename i
-0001a020: 6e20 416c 6c56 616c 7565 732e 6b65 7973  n AllValues.keys
-0001a030: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-0001a040: 2020 2041 7474 7269 6275 7465 6964 732e     Attributeids.
-0001a050: 6170 7065 6e64 2861 7474 7269 6275 7465  append(attribute
-0001a060: 6e61 6d65 2920 2020 200d 0a20 2020 2020  name)    ..     
-0001a070: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001a080: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
-0001a090: 6e20 4174 7472 6962 7574 6569 6473 2c20  n Attributeids, 
-0001a0a0: 416c 6c56 616c 7565 7320 2020 2020 0d0a  AllValues     ..
-0001a0b0: 2020 2020 0d0a 6465 6620 6765 745f 7472      ..def get_tr
-0001a0c0: 6163 6b5f 6461 7461 7365 7428 7472 6163  ack_dataset(trac
-0001a0d0: 6b5f 6461 7461 7365 742c 2074 7261 636b  k_dataset, track
-0001a0e0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001a0f0: 6579 732c 2074 7261 636b 5f61 6e61 6c79  eys, track_analy
-0001a100: 7369 735f 7472 6163 6b5f 6b65 7973 2c20  sis_track_keys, 
-0001a110: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
-0001a120: 786e 616d 6529 3a0d 0a0d 0a20 2020 2020  xname):....     
-0001a130: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
-0001a140: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
-0001a150: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
-0001a160: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001a170: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
-0001a180: 0a20 2020 2020 2020 2054 6964 203d 2074  .        Tid = t
-0001a190: 7261 636b 5f64 6174 6173 6574 5b74 7261  rack_dataset[tra
-0001a1a0: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
-0001a1b0: 6c6f 6174 2229 0d0a 2020 2020 2020 200d  loat")..       .
-0001a1c0: 0a20 2020 2020 2020 2041 6c6c 5472 6163  .        AllTrac
-0001a1d0: 6b56 616c 7565 735b 7472 6163 6b5f 6964  kValues[track_id
-0001a1e0: 5d20 3d20 5469 640d 0a20 2020 2020 200d  ] = Tid..      .
-0001a1f0: 0a20 2020 2020 2020 2066 6f72 2028 6b2c  .        for (k,
-0001a200: 2076 2920 696e 2074 7261 636b 5f61 6e61   v) in track_ana
-0001a210: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
-0001a220: 2e69 7465 6d73 2829 3a0d 0a0d 0a20 2020  .items():....   
-0001a230: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-0001a240: 2074 7261 636b 5f64 6174 6173 6574 5b76   track_dataset[v
-0001a250: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-0001a260: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001a270: 2020 206d 696e 7661 6c20 3d20 6d69 6e28     minval = min(
-0001a280: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-0001a290: 2020 2020 6d61 7876 616c 203d 206d 6178      maxval = max
-0001a2a0: 2878 290d 0a0d 0a20 2020 2020 2020 2020  (x)....         
-0001a2b0: 2020 2020 2020 2069 6620 6d69 6e76 616c         if minval
-0001a2c0: 203e 2030 2061 6e64 206d 6178 7661 6c20   > 0 and maxval 
-0001a2d0: 3c3d 2031 3a0d 0a0d 0a20 2020 2020 2020  <= 1:....       
-0001a2e0: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-0001a2f0: 2078 202b 2031 0d0a 0d0a 2020 2020 2020   x + 1....      
-0001a300: 2020 2020 2020 2020 2020 416c 6c54 7261            AllTra
-0001a310: 636b 5661 6c75 6573 5b6b 5d20 3d20 726f  ckValues[k] = ro
-0001a320: 756e 6428 782c 2033 290d 0a0d 0a20 2020  und(x, 3)....   
-0001a330: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
-0001a340: 7574 6569 6473 203d 205b 5d0d 0a20 2020  uteids = []..   
-0001a350: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
-0001a360: 7574 6569 6473 2e61 7070 656e 6428 5472  uteids.append(Tr
-0001a370: 6163 6b41 7474 7269 6275 7465 426f 786e  ackAttributeBoxn
-0001a380: 616d 6529 0d0a 2020 2020 2020 2020 666f  ame)..        fo
-0001a390: 7220 6174 7472 6962 7574 656e 616d 6520  r attributename 
-0001a3a0: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
-0001a3b0: 735f 7472 6163 6b5f 6b65 7973 2e6b 6579  s_track_keys.key
-0001a3c0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-0001a3d0: 2020 5472 6163 6b41 7474 7269 6275 7465    TrackAttribute
-0001a3e0: 6964 732e 6170 7065 6e64 2861 7474 7269  ids.append(attri
-0001a3f0: 6275 7465 6e61 6d65 2920 2020 200d 0a20  butename)    .. 
-0001a400: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
-0001a410: 7572 6e20 5472 6163 6b41 7474 7269 6275  urn TrackAttribu
-0001a420: 7465 6964 732c 2041 6c6c 5472 6163 6b56  teids, AllTrackV
-0001a430: 616c 7565 730d 0a20 2020 200d 0a64 6566  alues..    ..def
-0001a440: 2067 6574 5f65 6467 6573 5f64 6174 6173   get_edges_datas
-0001a450: 6574 2865 6467 6573 5f64 6174 6173 6574  et(edges_dataset
-0001a460: 2c20 6564 6765 735f 6461 7461 7365 745f  , edges_dataset_
-0001a470: 696e 6465 782c 2074 7261 636b 5f61 6e61  index, track_ana
-0001a480: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
-0001a490: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a4a0: 6564 6765 735f 6b65 7973 293a 0d0a 0d0a  edges_keys):....
-0001a4b0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
-0001a4c0: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
-0001a4d0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-0001a4e0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001a4f0: 706f 745f 6b65 7973 5b22 7472 6163 6b5f  pot_keys["track_
-0001a500: 6964 225d 0d0a 2020 2020 2020 2020 5469  id"]..        Ti
-0001a510: 6420 3d20 6564 6765 735f 6461 7461 7365  d = edges_datase
-0001a520: 745b 7472 6163 6b5f 6964 5d2e 6173 7479  t[track_id].asty
-0001a530: 7065 2822 666c 6f61 7422 290d 0a20 2020  pe("float")..   
-0001a540: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
-0001a550: 702e 7768 6572 6528 5469 6420 3d3d 2030  p.where(Tid == 0
-0001a560: 290d 0a20 2020 2020 2020 206d 6178 7472  )..        maxtr
-0001a570: 6163 6b5f 6964 203d 206d 6178 2854 6964  ack_id = max(Tid
-0001a580: 290d 0a20 2020 2020 2020 2063 6f6e 6469  )..        condi
-0001a590: 7469 6f6e 5f69 6e64 6963 6573 203d 2065  tion_indices = e
-0001a5a0: 6467 6573 5f64 6174 6173 6574 5f69 6e64  dges_dataset_ind
-0001a5b0: 6578 5b69 6e64 6963 6573 5d0d 0a20 2020  ex[indices]..   
-0001a5c0: 2020 2020 2054 6964 5b63 6f6e 6469 7469       Tid[conditi
-0001a5d0: 6f6e 5f69 6e64 6963 6573 5d20 3d20 6d61  on_indices] = ma
-0001a5e0: 7874 7261 636b 5f69 6420 2b20 310d 0a20  xtrack_id + 1.. 
-0001a5f0: 2020 2020 2020 2041 6c6c 4564 6765 7356         AllEdgesV
-0001a600: 616c 7565 735b 7472 6163 6b5f 6964 5d20  alues[track_id] 
-0001a610: 3d20 5469 640d 0a0d 0a20 2020 2020 2020  = Tid....       
-0001a620: 2066 6f72 206b 2069 6e20 7472 6163 6b5f   for k in track_
-0001a630: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
-0001a640: 6579 732e 7661 6c75 6573 2829 3a0d 0a0d  eys.values():...
-0001a650: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001a660: 6b20 213d 2074 7261 636b 5f69 643a 0d0a  k != track_id:..
-0001a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a680: 7820 3d20 6564 6765 735f 6461 7461 7365  x = edges_datase
-0001a690: 745b 6b5d 2e61 7374 7970 6528 2266 6c6f  t[k].astype("flo
-0001a6a0: 6174 2229 0d0a 0d0a 2020 2020 2020 2020  at")....        
-0001a6b0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
-0001a6c0: 5661 6c75 6573 5b6b 5d20 3d20 7820 2020  Values[k] = x   
-0001a6d0: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
-0001a6e0: 2020 2020 2072 6574 7572 6e20 416c 6c45       return AllE
-0001a6f0: 6467 6573 5661 6c75 6573 2020 200d 0a20  dgesValues   .. 
-0001a700: 2020 200d 0a20 2020 2020 2020 0d0a 2020     ..       ..  
-0001a710: 2020 0d0a 6465 6620 7363 616c 655f 7661    ..def scale_va
-0001a720: 6c75 6528 782c 2073 6361 6c65 203d 2032  lue(x, scale = 2
-0001a730: 3535 202a 2032 3535 293a 0d0a 0d0a 0d0a  55 * 255):......
-0001a740: 2020 2020 2072 6574 7572 6e20 7820 2a20       return x * 
-0001a750: 7363 616c 6520 2020 0d0a 2020 2020 0d0a  scale   ..    ..
-0001a760: 0d0a 0d0a 6465 6620 7072 6f62 5f73 6967  ....def prob_sig
-0001a770: 6d6f 6964 2878 293a 0d0a 2020 2020 7265  moid(x):..    re
-0001a780: 7475 726e 2031 202d 206d 6174 682e 6578  turn 1 - math.ex
-0001a790: 7028 2d78 290d 0a0d 0a0d 0a64 6566 2061  p(-x)......def a
-0001a7a0: 6e67 756c 6172 5f63 6861 6e67 6528 7665  ngular_change(ve
-0001a7b0: 635f 302c 2076 6563 5f31 293a 0d0a 2020  c_0, vec_1):..  
-0001a7c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001a7d0: 7665 635f 3020 3d20 7665 635f 3020 2f20  vec_0 = vec_0 / 
-0001a7e0: 6e70 2e6c 696e 616c 672e 6e6f 726d 2876  np.linalg.norm(v
-0001a7f0: 6563 5f30 290d 0a20 2020 2020 2020 2076  ec_0)..        v
-0001a800: 6563 5f31 203d 2076 6563 5f31 202f 206e  ec_1 = vec_1 / n
-0001a810: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 7665  p.linalg.norm(ve
-0001a820: 635f 3129 0d0a 2020 2020 2020 2020 616e  c_1)..        an
-0001a830: 676c 6520 3d20 6e70 2e61 7263 636f 7328  gle = np.arccos(
-0001a840: 6e70 2e63 6c69 7028 6e70 2e64 6f74 2876  np.clip(np.dot(v
-0001a850: 6563 5f30 2c20 7665 635f 3129 2c20 2d31  ec_0, vec_1), -1
-0001a860: 2e30 2c20 312e 3029 290d 0a20 2020 2020  .0, 1.0))..     
-0001a870: 2020 2061 6e67 6c65 203d 2061 6e67 6c65     angle = angle
-0001a880: 202a 2031 3830 202f 206e 702e 7069 0d0a   * 180 / np.pi..
-0001a890: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0001a8a0: 6e67 6c65 0d0a 2020 2020 200d 0a0d 0a64  ngle..     ....d
-0001a8b0: 6566 2065 7661 6c5f 626f 6f6c 2876 616c  ef eval_bool(val
-0001a8c0: 7565 293a 0d0a 2020 2020 2020 2020 2020  ue):..          
-0001a8d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001a8e0: 2020 6966 2076 616c 7565 2020 3d3d 2027    if value  == '
-0001a8f0: 5472 7565 273a 200d 0a20 2020 2020 2020  True': ..       
-0001a900: 2020 2020 2020 2020 2064 6976 5f6b 6579           div_key
-0001a910: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
-0001a920: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0001a930: 2020 2020 2020 2020 6469 765f 6b65 7920          div_key 
-0001a940: 3d20 4661 6c73 6520 0d0a 0d0a 2020 2020  = False ....    
-0001a950: 2020 2020 7265 7475 726e 2064 6976 5f6b      return div_k
-0001a960: 6579 2020 2020 2020 2020 2020 2020 2020  ey              
-0001a970: 2020 0d0a 0d0a 6465 6620 6368 6563 6b5f    ....def check_
-0001a980: 616e 645f 7570 6461 7465 5f6d 6173 6b28  and_update_mask(
-0001a990: 6d61 736b 2c69 6d61 6765 293a 0d0a 2020  mask,image):..  
-0001a9a0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-0001a9b0: 6620 6c65 6e28 6d61 736b 2e73 6861 7065  f len(mask.shape
-0001a9c0: 2920 3c20 6c65 6e28 696d 6167 652e 7368  ) < len(image.sh
-0001a9d0: 6170 6529 3a0d 0a20 2020 2020 2020 2020  ape):..         
-0001a9e0: 2020 2075 7064 6174 655f 6d61 736b 203d     update_mask =
-0001a9f0: 206e 702e 7a65 726f 7328 0d0a 2020 2020   np.zeros(..    
-0001aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa10: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
-0001aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa30: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-0001aa40: 2e73 6861 7065 5b30 5d2c 0d0a 2020 2020  .shape[0],..    
-0001aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa60: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-0001aa70: 652e 7368 6170 655b 315d 2c0d 0a20 2020  e.shape[1],..   
-0001aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa90: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-0001aaa0: 6765 2e73 6861 7065 5b32 5d2c 0d0a 2020  ge.shape[2],..  
-0001aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aac0: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001aad0: 6167 652e 7368 6170 655b 335d 2c0d 0a20  age.shape[3],.. 
-0001aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aaf0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-0001ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab10: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001ab20: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0001ab30: 6e67 6528 302c 2075 7064 6174 655f 6d61  nge(0, update_ma
-0001ab40: 736b 2e73 6861 7065 5b30 5d29 3a0d 0a20  sk.shape[0]):.. 
-0001ab50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001ab60: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-0001ab70: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
-0001ab80: 7065 5b31 5d29 3a0d 0a0d 0a20 2020 2020  pe[1]):....     
-0001ab90: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0001aba0: 7064 6174 655f 6d61 736b 5b69 2c20 6a2c  pdate_mask[i, j,
-0001abb0: 203a 2c20 3a5d 203d 206d 6173 6b5b 692c   :, :] = mask[i,
-0001abc0: 203a 2c20 3a5d 0d0a 2020 2020 2020 2020   :, :]..        
-0001abd0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0001abe0: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
-0001abf0: 736b 203d 206d 6173 6b0d 0a0d 0a20 2020  sk = mask....   
-0001ac00: 2020 2020 2072 6574 7572 6e20 7570 6461       return upda
-0001ac10: 7465 5f6d 6173 6b20 2020 2020 2020 200d  te_mask        .
-0001ac20: 0a20 2020 2020 2020 0d0a                 .       ..
+000182d0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+000182e0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
+000182f0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018300: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00018310: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
+00018320: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018330: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+00018340: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+00018350: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+00018360: 6469 7370 5f7a 2929 0d0a 0d0a 2020 2020  disp_z))....    
+00018370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018380: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00018390: 5f6d 6561 6e5f 6469 7370 5f79 2e61 7070  _mean_disp_y.app
+000183a0: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
+000183b0: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
+000183c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000183d0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000183e0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+000183f0: 792e 6170 7065 6e64 286e 702e 7374 6428  y.append(np.std(
+00018400: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00018410: 5f79 2929 0d0a 0d0a 2020 2020 2020 2020  _y))....        
+00018420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018430: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00018440: 6e5f 6469 7370 5f78 2e61 7070 656e 6428  n_disp_x.append(
+00018450: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+00018460: 7469 635f 6469 7370 5f78 2929 0d0a 2020  tic_disp_x))..  
+00018470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018480: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018490: 6963 5f76 6172 5f64 6973 705f 782e 6170  ic_var_disp_x.ap
+000184a0: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
+000184b0: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
+000184c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000184d0: 2020 2020 2020 2020 6966 206c 656e 286e          if len(n
+000184e0: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
+000184f0: 7329 203e 2030 3a0d 0a20 2020 2020 2020  s) > 0:..       
+00018500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018510: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00018520: 635f 6d65 616e 5f72 6164 6975 732e 6170  c_mean_radius.ap
+00018530: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
+00018540: 5f6d 6974 6f74 6963 5f72 6164 6975 7329  _mitotic_radius)
+00018550: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018570: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00018580: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
+00018590: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
+000185a0: 5f72 6164 6975 7329 290d 0a0d 0a20 2020  _radius))....   
+000185b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185c0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+000185d0: 635f 6d65 616e 5f73 7065 6564 2e61 7070  c_mean_speed.app
+000185e0: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
+000185f0: 6d69 746f 7469 635f 7370 6565 6429 290d  mitotic_speed)).
+00018600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018610: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00018620: 746f 7469 635f 7661 725f 7370 6565 642e  totic_var_speed.
+00018630: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+00018640: 6e5f 6d69 746f 7469 635f 7370 6565 6429  n_mitotic_speed)
+00018650: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018660: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018670: 6e5f 6d69 746f 7469 635f 6d65 616e 5f61  n_mitotic_mean_a
+00018680: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
+00018690: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6163  n(non_mitotic_ac
+000186a0: 6329 290d 0a20 2020 2020 2020 2020 2020  c))..           
+000186b0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000186c0: 6e5f 6d69 746f 7469 635f 7661 725f 6163  n_mitotic_var_ac
+000186d0: 632e 6170 7065 6e64 286e 702e 7374 6428  c.append(np.std(
+000186e0: 6e6f 6e5f 6d69 746f 7469 635f 6163 6329  non_mitotic_acc)
+000186f0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018700: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018710: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+00018720: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00018730: 652e 6170 7065 6e64 286e 702e 6d65 616e  e.append(np.mean
+00018740: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6972  (non_mitotic_dir
+00018750: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00018760: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018770: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018780: 6d69 746f 7469 635f 7661 725f 6469 7265  mitotic_var_dire
+00018790: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+000187a0: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
+000187b0: 5f6d 6974 6f74 6963 5f64 6972 6563 7469  _mitotic_directi
+000187c0: 6f6e 616c 5f63 6861 6e67 6529 2920 0d0a  onal_change)) ..
+000187d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000187e0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000187f0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
+00018800: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00018810: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00018820: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
+00018830: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+00018840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018850: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018860: 6f74 6963 5f76 6172 5f64 6973 7461 6e63  otic_var_distanc
+00018870: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00018880: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00018890: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
+000188a0: 656c 6c5f 6d61 736b 2929 0d0a 0d0a 0d0a  ell_mask))......
+000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188c0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+000188d0: 6e5f 6469 7370 5f7a 2e61 7070 656e 6428  n_disp_z.append(
+000188e0: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7370  np.mean(all_disp
+000188f0: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
+00018900: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018910: 6c6c 5f76 6172 5f64 6973 705f 7a2e 6170  ll_var_disp_z.ap
+00018920: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
+00018930: 6469 7370 5f7a 2929 0d0a 0d0a 2020 2020  disp_z))....    
+00018940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018950: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
+00018960: 7370 5f79 2e61 7070 656e 6428 6e70 2e6d  sp_y.append(np.m
+00018970: 6561 6e28 616c 6c5f 6469 7370 5f79 2929  ean(all_disp_y))
+00018980: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018990: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+000189a0: 6172 5f64 6973 705f 792e 6170 7065 6e64  ar_disp_y.append
+000189b0: 286e 702e 7374 6428 616c 6c5f 6469 7370  (np.std(all_disp
+000189c0: 5f79 2929 0d0a 0d0a 2020 2020 2020 2020  _y))....        
+000189d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000189e0: 2e61 6c6c 5f6d 6561 6e5f 6469 7370 5f78  .all_mean_disp_x
+000189f0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018a00: 616c 6c5f 6469 7370 5f78 2929 0d0a 2020  all_disp_x))..  
+00018a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a20: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
+00018a30: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
+00018a40: 7374 6428 616c 6c5f 6469 7370 5f78 2929  std(all_disp_x))
+00018a50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018a60: 2020 2020 2020 2020 6966 206c 656e 2861          if len(a
+00018a70: 6c6c 5f72 6164 6975 7329 203e 2030 3a0d  ll_radius) > 0:.
+00018a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018a90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018aa0: 662e 616c 6c5f 6d65 616e 5f72 6164 6975  f.all_mean_radiu
+00018ab0: 732e 6170 7065 6e64 286e 702e 6d65 616e  s.append(np.mean
+00018ac0: 2861 6c6c 5f72 6164 6975 7329 290d 0a20  (all_radius)).. 
+00018ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ae0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018af0: 616c 6c5f 7661 725f 7261 6469 7573 2e61  all_var_radius.a
+00018b00: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00018b10: 5f72 6164 6975 7329 290d 0a0d 0a20 2020  _radius))....   
+00018b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b30: 2073 656c 662e 616c 6c5f 6d65 616e 5f73   self.all_mean_s
+00018b40: 7065 6564 2e61 7070 656e 6428 6e70 2e6d  peed.append(np.m
+00018b50: 6561 6e28 616c 6c5f 7370 6565 6429 290d  ean(all_speed)).
+00018b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018b70: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00018b80: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
+00018b90: 702e 7374 6428 616c 6c5f 7370 6565 6429  p.std(all_speed)
+00018ba0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018bb0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018bc0: 6c5f 6d65 616e 5f61 6363 2e61 7070 656e  l_mean_acc.appen
+00018bd0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6163  d(np.mean(all_ac
+00018be0: 6329 290d 0a20 2020 2020 2020 2020 2020  c))..           
+00018bf0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018c00: 6c5f 7661 725f 6163 632e 6170 7065 6e64  l_var_acc.append
+00018c10: 286e 702e 7374 6428 616c 6c5f 6163 6329  (np.std(all_acc)
+00018c20: 290d 0a0d 0a0d 0a0d 0a20 2020 2020 2020  )........       
+00018c30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018c40: 662e 616c 6c5f 6d65 616e 5f64 6972 6563  f.all_mean_direc
+00018c50: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
+00018c60: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+00018c70: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018c80: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
+00018c90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018ca0: 616c 6c5f 7661 725f 6469 7265 6374 696f  all_var_directio
+00018cb0: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00018cc0: 6428 6e70 2e73 7464 2861 6c6c 5f64 6972  d(np.std(all_dir
+00018cd0: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00018ce0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018cf0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018d00: 6c5f 6d65 616e 5f64 6973 7461 6e63 655f  l_mean_distance_
+00018d10: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
+00018d20: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
+00018d30: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+00018d40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018d50: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018d60: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
+00018d70: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00018d80: 2e73 7464 2861 6c6c 5f64 6973 7461 6e63  .std(all_distanc
+00018d90: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
+00018da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018db0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00018dc0: 2020 2020 200d 0a64 6566 2062 6f75 6e64       ..def bound
+00018dd0: 6172 795f 706f 696e 7473 286d 6173 6b2c  ary_points(mask,
+00018de0: 2078 6361 6c69 6272 6174 696f 6e2c 2079   xcalibration, y
+00018df0: 6361 6c69 6272 6174 696f 6e2c 207a 6361  calibration, zca
+00018e00: 6c69 6272 6174 696f 6e29 3a0d 0a0d 0a20  libration):.... 
+00018e10: 2020 206e 6469 6d20 3d20 6c65 6e28 6d61     ndim = len(ma
+00018e20: 736b 2e73 6861 7065 290d 0a20 2020 2074  sk.shape)..    t
+00018e30: 696d 6564 5f6d 6173 6b20 3d20 7b7d 0d0a  imed_mask = {}..
+00018e40: 2020 2020 6d61 736b 203d 206d 6173 6b20      mask = mask 
+00018e50: 3e20 300d 0a20 2020 206d 6173 6b20 3d20  > 0..    mask = 
+00018e60: 6d61 736b 2e61 7374 7970 6528 2775 696e  mask.astype('uin
+00018e70: 7438 2729 0d0a 2020 2020 2320 5958 2073  t8')..    # YX s
+00018e80: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
+00018e90: 2020 6966 206e 6469 6d20 3d3d 2032 3a0d    if ndim == 2:.
+00018ea0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00018eb0: 2020 2062 6f75 6e64 6172 7920 3d20 6669     boundary = fi
+00018ec0: 6e64 5f62 6f75 6e64 6172 6965 7328 6d61  nd_boundaries(ma
+00018ed0: 736b 290d 0a20 2020 2020 2020 2072 6567  sk)..        reg
+00018ee0: 696f 6e63 656e 7472 6f69 6420 3d20 2830  ioncentroid = (0
+00018ef0: 2c29 202b 2063 6f6d 7075 7465 5f63 656e  ,) + compute_cen
+00018f00: 7472 6f69 6428 626f 756e 6461 7279 2920  troid(boundary) 
+00018f10: 0d0a 2020 2020 2020 2020 696e 6469 6365  ..        indice
+00018f20: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
+00018f30: 6e64 6172 7920 3e20 3029 0d0a 2020 2020  ndary > 0)..    
+00018f40: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+00018f50: 203d 206e 702e 7472 616e 7370 6f73 6528   = np.transpose(
+00018f60: 6e70 2e61 7361 7272 6179 2869 6e64 6963  np.asarray(indic
+00018f70: 6573 2c20 6474 7970 653d 6e70 2e66 6c6f  es, dtype=np.flo
+00018f80: 6174 3332 2929 2e63 6f70 7928 290d 0a0d  at32)).copy()...
+00018f90: 0a20 2020 2020 2020 2066 6f72 206a 2069  .        for j i
+00018fa0: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
+00018fb0: 6561 6c5f 696e 6469 6365 7329 293a 0d0a  eal_indices)):..
+00018fc0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00018fd0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
+00018fe0: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
+00018ff0: 6a5d 5b30 5d20 2a20 7963 616c 6962 7261  j][0] * ycalibra
+00019000: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+00019010: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+00019020: 5d5b 315d 203d 2072 6561 6c5f 696e 6469  ][1] = real_indi
+00019030: 6365 735b 6a5d 5b31 5d20 2a20 7863 616c  ces[j][1] * xcal
+00019040: 6962 7261 7469 6f6e 0d0a 0d0a 2020 2020  ibration....    
+00019050: 2020 2020 7472 6565 203d 2073 7061 7469      tree = spati
+00019060: 616c 2e63 4b44 5472 6565 2872 6561 6c5f  al.cKDTree(real_
+00019070: 696e 6469 6365 7329 0d0a 2020 2020 2020  indices)..      
+00019080: 2020 2320 5468 6973 206f 626a 6563 7420    # This object 
+00019090: 636f 6e74 6169 6e73 206c 6973 7420 6f66  contains list of
+000190a0: 2061 6c6c 2074 6865 2070 6f69 6e74 7320   all the points 
+000190b0: 666f 7220 616c 6c20 7468 6520 6c61 6265  for all the labe
+000190c0: 6c73 2069 6e20 7468 6520 4d61 736b 2069  ls in the Mask i
+000190d0: 6d61 6765 2077 6974 6820 7468 6520 6c61  mage with the la
+000190e0: 6265 6c20 6964 2061 6e64 2076 6f6c 756d  bel id and volum
+000190f0: 6520 6f66 2065 6163 6820 6c61 6265 6c0d  e of each label.
+00019100: 0a20 2020 2020 2020 2074 696d 6564 5f6d  .        timed_m
+00019110: 6173 6b5b 7374 7228 3029 5d20 3d20 5b74  ask[str(0)] = [t
+00019120: 7265 652c 2069 6e64 6963 6573 2c20 7265  ree, indices, re
+00019130: 6769 6f6e 6365 6e74 726f 6964 5d0d 0a0d  gioncentroid]...
+00019140: 0a20 2020 2023 2054 5958 2073 6861 7065  .    # TYX shape
+00019150: 6420 6f62 6a65 6374 0d0a 2020 2020 6966  d object..    if
+00019160: 206e 6469 6d20 3d3d 2033 3a0d 0a0d 0a0d   ndim == 3:.....
+00019170: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+00019180: 6e20 7471 646d 2872 616e 6765 2830 2c20  n tqdm(range(0, 
+00019190: 6d61 736b 2e73 6861 7065 5b30 5d29 293a  mask.shape[0])):
+000191a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000191b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000191c0: 2020 2020 626f 756e 6461 7279 203d 2066      boundary = f
+000191d0: 696e 645f 626f 756e 6461 7269 6573 286d  ind_boundaries(m
+000191e0: 6173 6b5b 692c 3a5d 290d 0a20 2020 2020  ask[i,:])..     
+000191f0: 2020 2020 2020 2020 2020 2072 6567 696f             regio
+00019200: 6e63 656e 7472 6f69 6420 3d20 2830 2c29  ncentroid = (0,)
+00019210: 202b 2063 6f6d 7075 7465 5f63 656e 7472   + compute_centr
+00019220: 6f69 6428 626f 756e 6461 7279 2920 0d0a  oid(boundary) ..
+00019230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019240: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
+00019250: 7265 2862 6f75 6e64 6172 7920 3e20 3029  re(boundary > 0)
+00019260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019270: 2020 7265 616c 5f69 6e64 6963 6573 203d    real_indices =
+00019280: 206e 702e 7472 616e 7370 6f73 6528 6e70   np.transpose(np
+00019290: 2e61 7361 7272 6179 2869 6e64 6963 6573  .asarray(indices
+000192a0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+000192b0: 3332 2929 2e63 6f70 7928 290d 0a0d 0a20  32)).copy().... 
+000192c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000192d0: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
+000192e0: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
+000192f0: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
+00019300: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00019310: 5f69 6e64 6963 6573 5b6a 5d5b 305d 203d  _indices[j][0] =
+00019320: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00019330: 5b30 5d20 2a20 7963 616c 6962 7261 7469  [0] * ycalibrati
+00019340: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00019350: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+00019360: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
+00019370: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+00019380: 2a20 7863 616c 6962 7261 7469 6f6e 0d0a  * xcalibration..
+00019390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000193a0: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
+000193b0: 2e63 4b44 5472 6565 2872 6561 6c5f 696e  .cKDTree(real_in
+000193c0: 6469 6365 7329 0d0a 0d0a 2020 2020 2020  dices)....      
+000193d0: 2020 2020 2020 2020 2020 7469 6d65 645f            timed_
+000193e0: 6d61 736b 5b73 7472 2869 295d 203d 205b  mask[str(i)] = [
+000193f0: 7472 6565 2c20 696e 6469 6365 732c 2072  tree, indices, r
+00019400: 6567 696f 6e63 656e 7472 6f69 645d 0d0a  egioncentroid]..
+00019410: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00019420: 2020 2320 545a 5958 2073 6861 7065 6420    # TZYX shaped 
+00019430: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
+00019440: 6469 6d20 3d3d 2034 3a0d 0a20 2020 2020  dim == 4:..     
+00019450: 2020 2070 7269 6e74 2827 4d61 736b 7320     print('Masks 
+00019460: 6d61 6465 2069 6e74 6f20 6120 3444 2063  made into a 4D c
+00019470: 796c 696e 6465 722c 2075 7027 290d 0a20  ylinder, up').. 
+00019480: 2020 2020 2020 2062 6f75 6e64 6172 7920         boundary 
+00019490: 3d20 6e70 2e7a 6572 6f73 280d 0a20 2020  = np.zeros(..   
+000194a0: 2020 2020 2020 2020 205b 6d61 736b 2e73           [mask.s
+000194b0: 6861 7065 5b30 5d2c 206d 6173 6b2e 7368  hape[0], mask.sh
+000194c0: 6170 655b 315d 2c20 6d61 736b 2e73 6861  ape[1], mask.sha
+000194d0: 7065 5b32 5d2c 206d 6173 6b2e 7368 6170  pe[2], mask.shap
+000194e0: 655b 335d 5d0d 0a20 2020 2020 2020 2029  e[3]]..        )
+000194f0: 0d0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
+00019500: 696e 2072 616e 6765 2830 2c20 6d61 736b  in range(0, mask
+00019510: 2e73 6861 7065 5b30 5d29 3a0d 0a20 2020  .shape[0]):..   
+00019520: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00019530: 2020 2020 2020 2062 6f75 6e64 6172 795b         boundary[
+00019540: 692c 3a5d 203d 2066 696e 645f 626f 756e  i,:] = find_boun
+00019550: 6461 7269 6573 286d 6173 6b5b 692c 3a5d  daries(mask[i,:]
+00019560: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00019570: 6567 696f 6e63 656e 7472 6f69 6420 3d20  egioncentroid = 
+00019580: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
+00019590: 2862 6f75 6e64 6172 795b 692c 3a5d 2920  (boundary[i,:]) 
+000195a0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+000195b0: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
+000195c0: 2862 6f75 6e64 6172 795b 692c 3a5d 203e  (boundary[i,:] >
+000195d0: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
+000195e0: 2072 6561 6c5f 696e 6469 6365 7320 3d20   real_indices = 
+000195f0: 6e70 2e74 7261 6e73 706f 7365 286e 702e  np.transpose(np.
+00019600: 6173 6172 7261 7928 696e 6469 6365 732c  asarray(indices,
+00019610: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00019620: 3229 292e 636f 7079 2829 0d0a 0d0a 2020  2)).copy()....  
+00019630: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+00019640: 696e 2072 616e 6765 2830 2c20 6c65 6e28  in range(0, len(
+00019650: 7265 616c 5f69 6e64 6963 6573 2929 3a0d  real_indices)):.
+00019660: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00019670: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+00019680: 6365 735b 6a5d 5b30 5d20 3d20 7265 616c  ces[j][0] = real
+00019690: 5f69 6e64 6963 6573 5b6a 5d5b 305d 202a  _indices[j][0] *
+000196a0: 207a 6361 6c69 6272 6174 696f 6e0d 0a20   zcalibration.. 
+000196b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196c0: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
+000196d0: 6a5d 5b31 5d20 3d20 7265 616c 5f69 6e64  j][1] = real_ind
+000196e0: 6963 6573 5b6a 5d5b 315d 202a 2079 6361  ices[j][1] * yca
+000196f0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+00019700: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00019710: 6561 6c5f 696e 6469 6365 735b 6a5d 5b32  eal_indices[j][2
+00019720: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
+00019730: 5b6a 5d5b 325d 202a 2078 6361 6c69 6272  [j][2] * xcalibr
+00019740: 6174 696f 6e0d 0a0d 0a20 2020 2020 2020  ation....       
+00019750: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
+00019760: 6961 6c2e 634b 4454 7265 6528 7265 616c  ial.cKDTree(real
+00019770: 5f69 6e64 6963 6573 290d 0a20 2020 2020  _indices)..     
+00019780: 2020 2020 2020 2074 696d 6564 5f6d 6173         timed_mas
+00019790: 6b5b 7374 7228 6929 5d20 3d20 5b74 7265  k[str(i)] = [tre
+000197a0: 652c 2069 6e64 6963 6573 2c20 7265 6769  e, indices, regi
+000197b0: 6f6e 6365 6e74 726f 6964 5d0d 0a20 2020  oncentroid]..   
+000197c0: 2070 7269 6e74 2827 436f 6d70 7574 6564   print('Computed
+000197d0: 2074 6865 2062 6f75 6e64 6172 7920 706f   the boundary po
+000197e0: 696e 7473 2729 0d0a 0d0a 2020 2020 7265  ints')....    re
+000197f0: 7475 726e 2074 696d 6564 5f6d 6173 6b2c  turn timed_mask,
+00019800: 2062 6f75 6e64 6172 7920 2020 2020 2020   boundary       
+00019810: 200d 0a0d 0a64 6566 2063 6f6d 7075 7465   ....def compute
+00019820: 5f63 656e 7472 6f69 6428 6269 6e61 7279  _centroid(binary
+00019830: 5f69 6d61 6765 293a 0d0a 2020 2020 2320  _image):..    # 
+00019840: 456e 7375 7265 2062 696e 6172 7920 696d  Ensure binary im
+00019850: 6167 6520 6973 2061 204e 756d 5079 2061  age is a NumPy a
+00019860: 7272 6179 0d0a 2020 2020 6269 6e61 7279  rray..    binary
+00019870: 5f69 6d61 6765 203d 206e 702e 6172 7261  _image = np.arra
+00019880: 7928 6269 6e61 7279 5f69 6d61 6765 290d  y(binary_image).
+00019890: 0a0d 0a20 2020 2077 6869 7465 5f70 6978  ...    white_pix
+000198a0: 656c 7320 3d20 6e70 2e77 6865 7265 2862  els = np.where(b
+000198b0: 696e 6172 795f 696d 6167 6520 3d3d 2031  inary_image == 1
+000198c0: 290d 0a20 2020 206e 756d 5f70 6978 656c  )..    num_pixel
+000198d0: 7320 3d20 6c65 6e28 7768 6974 655f 7069  s = len(white_pi
+000198e0: 7865 6c73 5b30 5d29 0d0a 0d0a 2020 2020  xels[0])....    
+000198f0: 2320 436f 6d70 7574 6520 7468 6520 6365  # Compute the ce
+00019900: 6e74 726f 6964 206f 6620 7468 6520 7768  ntroid of the wh
+00019910: 6974 6520 7069 7865 6c73 2069 6e20 7468  ite pixels in th
+00019920: 6520 626f 756e 6461 7279 2069 6d61 6765  e boundary image
+00019930: 0d0a 2020 2020 6365 6e74 726f 6964 203d  ..    centroid =
+00019940: 206e 702e 7a65 726f 7328 6269 6e61 7279   np.zeros(binary
+00019950: 5f69 6d61 6765 2e6e 6469 6d29 0d0a 2020  _image.ndim)..  
+00019960: 2020 666f 7220 6469 6d20 696e 2072 616e    for dim in ran
+00019970: 6765 2862 696e 6172 795f 696d 6167 652e  ge(binary_image.
+00019980: 6e64 696d 293a 0d0a 2020 2020 2020 2020  ndim):..        
+00019990: 6365 6e74 726f 6964 5b64 696d 5d20 3d20  centroid[dim] = 
+000199a0: 7768 6974 655f 7069 7865 6c73 5b64 696d  white_pixels[dim
+000199b0: 5d2e 7375 6d28 2920 2f20 6e75 6d5f 7069  ].sum() / num_pi
+000199c0: 7865 6c73 0d0a 0d0a 2020 2020 7265 7475  xels....    retu
+000199d0: 726e 2063 656e 7472 6f69 640d 0a0d 0a0d  rn centroid.....
+000199e0: 0a0d 0a20 0d0a 0d0a 6465 6620 6765 745f  ... ....def get_
+000199f0: 6373 765f 6461 7461 2863 7376 293a 0d0a  csv_data(csv):..
+00019a00: 0d0a 2020 2020 2020 2020 6461 7461 7365  ..        datase
+00019a10: 7420 3d20 7064 2e72 6561 645f 6373 7628  t = pd.read_csv(
+00019a20: 0d0a 2020 2020 2020 2020 2020 2020 6373  ..            cs
+00019a30: 762c 2064 656c 696d 6974 6572 3d22 2c22  v, delimiter=","
+00019a40: 2c20 656e 636f 6469 6e67 3d22 756e 6963  , encoding="unic
+00019a50: 6f64 655f 6573 6361 7065 222c 206c 6f77  ode_escape", low
+00019a60: 5f6d 656d 6f72 793d 4661 6c73 650d 0a20  _memory=False.. 
+00019a70: 2020 2020 2020 2029 5b33 3a5d 0d0a 2020         )[3:]..  
+00019a80: 2020 2020 2020 6461 7461 7365 745f 696e        dataset_in
+00019a90: 6465 7820 3d20 6461 7461 7365 742e 696e  dex = dataset.in
+00019aa0: 6465 780d 0a20 2020 2020 2020 2072 6574  dex..        ret
+00019ab0: 7572 6e20 6461 7461 7365 742c 2064 6174  urn dataset, dat
+00019ac0: 6173 6574 5f69 6e64 6578 0d0a 2020 2020  aset_index..    
+00019ad0: 0d0a 6465 6620 6765 745f 7370 6f74 5f64  ..def get_spot_d
+00019ae0: 6174 6173 6574 2873 706f 745f 6461 7461  ataset(spot_data
+00019af0: 7365 742c 2074 7261 636b 5f61 6e61 6c79  set, track_analy
+00019b00: 7369 735f 7370 6f74 5f6b 6579 732c 2078  sis_spot_keys, x
+00019b10: 6361 6c69 6272 6174 696f 6e2c 2079 6361  calibration, yca
+00019b20: 6c69 6272 6174 696f 6e2c 207a 6361 6c69  libration, zcali
+00019b30: 6272 6174 696f 6e2c 2041 7474 7269 6275  bration, Attribu
+00019b40: 7465 426f 786e 616d 652c 2064 6574 6563  teBoxname, detec
+00019b50: 7469 6f6e 6368 616e 6e65 6c29 3a0d 0a20  tionchannel):.. 
+00019b60: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+00019b70: 203d 207b 7d0d 0a20 2020 2020 2020 2070   = {}..        p
+00019b80: 6f73 6978 203d 2074 7261 636b 5f61 6e61  osix = track_ana
+00019b90: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+00019ba0: 2270 6f73 6978 225d 0d0a 2020 2020 2020  "posix"]..      
+00019bb0: 2020 706f 7369 7920 3d20 7472 6163 6b5f    posiy = track_
+00019bc0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00019bd0: 7973 5b22 706f 7369 7922 5d0d 0a20 2020  ys["posiy"]..   
+00019be0: 2020 2020 2070 6f73 697a 203d 2074 7261       posiz = tra
+00019bf0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00019c00: 5f6b 6579 735b 2270 6f73 697a 225d 0d0a  _keys["posiz"]..
+00019c10: 2020 2020 2020 2020 6672 616d 6520 3d20          frame = 
+00019c20: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00019c30: 706f 745f 6b65 7973 5b22 6672 616d 6522  pot_keys["frame"
+00019c40: 5d0d 0a20 2020 2020 2020 200d 0a20 2020  ]..        ..   
+00019c50: 2020 2020 204c 6f63 6174 696f 6e58 203d       LocationX =
+00019c60: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00019c70: 7370 6f74 5f64 6174 6173 6574 5b70 6f73  spot_dataset[pos
+00019c80: 6978 5d2e 6173 7479 7065 2822 666c 6f61  ix].astype("floa
+00019c90: 7422 2920 2f20 7863 616c 6962 7261 7469  t") / xcalibrati
+00019ca0: 6f6e 0d0a 2020 2020 2020 2020 292e 6173  on..        ).as
+00019cb0: 7479 7065 2822 696e 7422 290d 0a20 2020  type("int")..   
+00019cc0: 2020 2020 204c 6f63 6174 696f 6e59 203d       LocationY =
+00019cd0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00019ce0: 7370 6f74 5f64 6174 6173 6574 5b70 6f73  spot_dataset[pos
+00019cf0: 6979 5d2e 6173 7479 7065 2822 666c 6f61  iy].astype("floa
+00019d00: 7422 2920 2f20 7963 616c 6962 7261 7469  t") / ycalibrati
+00019d10: 6f6e 0d0a 2020 2020 2020 2020 292e 6173  on..        ).as
+00019d20: 7479 7065 2822 696e 7422 290d 0a20 2020  type("int")..   
+00019d30: 2020 2020 204c 6f63 6174 696f 6e5a 203d       LocationZ =
+00019d40: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00019d50: 7370 6f74 5f64 6174 6173 6574 5b70 6f73  spot_dataset[pos
+00019d60: 697a 5d2e 6173 7479 7065 2822 666c 6f61  iz].astype("floa
+00019d70: 7422 2920 2f20 7a63 616c 6962 7261 7469  t") / zcalibrati
+00019d80: 6f6e 0d0a 2020 2020 2020 2020 292e 6173  on..        ).as
+00019d90: 7479 7065 2822 696e 7422 290d 0a20 2020  type("int")..   
+00019da0: 2020 2020 204c 6f63 6174 696f 6e54 203d       LocationT =
+00019db0: 2028 7370 6f74 5f64 6174 6173 6574 5b66   (spot_dataset[f
+00019dc0: 7261 6d65 5d2e 6173 7479 7065 2822 666c  rame].astype("fl
+00019dd0: 6f61 7422 2929 2e61 7374 7970 6528 2269  oat")).astype("i
+00019de0: 6e74 2229 0d0a 2020 2020 2020 2020 0d0a  nt")..        ..
+00019df0: 0d0a 2020 2020 2020 2020 6967 6e6f 7265  ..        ignore
+00019e00: 5f76 616c 7565 7320 3d20 5b74 7261 636b  _values = [track
+00019e10: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00019e20: 6579 735b 226d 6561 6e5f 696e 7465 6e73  eys["mean_intens
+00019e30: 6974 7922 5d2c 7472 6163 6b5f 616e 616c  ity"],track_anal
+00019e40: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00019e50: 746f 7461 6c5f 696e 7465 6e73 6974 7922  total_intensity"
+00019e60: 5d5d 200d 0a20 2020 2020 2020 2066 6f72  ]] ..        for
+00019e70: 2028 6b2c 7629 2069 6e20 7472 6163 6b5f   (k,v) in track_
+00019e80: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00019e90: 7973 2e69 7465 6d73 2829 3a0d 0a0d 0a20  ys.items():.... 
+00019ea0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00019eb0: 6620 6465 7465 6374 696f 6e63 6861 6e6e  f detectionchann
+00019ec0: 656c 203d 3d20 313a 0d0a 2020 2020 2020  el == 1:..      
+00019ed0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00019ee0: 6620 6b20 3d3d 2022 6d65 616e 5f69 6e74  f k == "mean_int
+00019ef0: 656e 7369 7479 5f63 6832 223a 0d0a 2020  ensity_ch2":..  
+00019f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f10: 2020 2020 2020 2020 2076 616c 7565 203d           value =
+00019f20: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+00019f30: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
+00019f40: 696e 7465 6e73 6974 7922 5d0d 0a20 2020  intensity"]..   
+00019f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f60: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+00019f70: 735b 7661 6c75 655d 203d 2073 706f 745f  s[value] = spot_
+00019f80: 6461 7461 7365 745b 765d 2e61 7374 7970  dataset[v].astyp
+00019f90: 6528 2266 6c6f 6174 2229 0d0a 2020 2020  e("float")..    
+00019fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fb0: 2069 6620 6b20 3d3d 2022 746f 7461 6c5f   if k == "total_
+00019fc0: 696e 7465 6e73 6974 795f 6368 3222 3a0d  intensity_ch2":.
+00019fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019fe0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00019ff0: 6520 3d20 7472 6163 6b5f 616e 616c 7973  e = track_analys
+0001a000: 6973 5f73 706f 745f 6b65 7973 5b22 746f  is_spot_keys["to
+0001a010: 7461 6c5f 696e 7465 6e73 6974 7922 5d0d  tal_intensity"].
+0001a020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a030: 2020 2020 2020 2020 2020 2020 416c 6c56              AllV
+0001a040: 616c 7565 735b 7661 6c75 655d 203d 2073  alues[value] = s
+0001a050: 706f 745f 6461 7461 7365 745b 765d 2e61  pot_dataset[v].a
+0001a060: 7374 7970 6528 2266 6c6f 6174 2229 2020  stype("float")  
+0001a070: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+0001a080: 2020 2020 2020 2020 2069 6620 7620 6e6f           if v no
+0001a090: 7420 696e 2069 676e 6f72 655f 7661 6c75  t in ignore_valu
+0001a0a0: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+0001a0b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0001a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0d0: 2020 2020 2041 6c6c 5661 6c75 6573 5b76       AllValues[v
+0001a0e0: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
+0001a0f0: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+0001a100: 7422 290d 0a0d 0a20 2020 2020 2020 2041  t")....        A
+0001a110: 6c6c 5661 6c75 6573 5b70 6f73 6978 5d20  llValues[posix] 
+0001a120: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
+0001a130: 582c 3329 0d0a 2020 2020 2020 2020 416c  X,3)..        Al
+0001a140: 6c56 616c 7565 735b 706f 7369 795d 203d  lValues[posiy] =
+0001a150: 2072 6f75 6e64 284c 6f63 6174 696f 6e59   round(LocationY
+0001a160: 2c33 290d 0a20 2020 2020 2020 2041 6c6c  ,3)..        All
+0001a170: 5661 6c75 6573 5b70 6f73 697a 5d20 3d20  Values[posiz] = 
+0001a180: 726f 756e 6428 4c6f 6361 7469 6f6e 5a2c  round(LocationZ,
+0001a190: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
+0001a1a0: 616c 7565 735b 6672 616d 655d 203d 2072  alues[frame] = r
+0001a1b0: 6f75 6e64 284c 6f63 6174 696f 6e54 2c33  ound(LocationT,3
+0001a1c0: 290d 0a20 2020 2020 2020 2041 7474 7269  )..        Attri
+0001a1d0: 6275 7465 6964 7320 3d20 5b5d 0d0a 2020  buteids = []..  
+0001a1e0: 2020 2020 2020 4174 7472 6962 7574 6569        Attributei
+0001a1f0: 6473 2e61 7070 656e 6428 4174 7472 6962  ds.append(Attrib
+0001a200: 7574 6542 6f78 6e61 6d65 290d 0a20 2020  uteBoxname)..   
+0001a210: 2020 2020 2066 6f72 2061 7474 7269 6275       for attribu
+0001a220: 7465 6e61 6d65 2069 6e20 416c 6c56 616c  tename in AllVal
+0001a230: 7565 732e 6b65 7973 2829 3a0d 0a20 2020  ues.keys():..   
+0001a240: 2020 2020 2020 2020 2020 2041 7474 7269             Attri
+0001a250: 6275 7465 6964 732e 6170 7065 6e64 2861  buteids.append(a
+0001a260: 7474 7269 6275 7465 6e61 6d65 2920 2020  ttributename)   
+0001a270: 200d 0a20 2020 2020 2020 2020 2020 200d   ..            .
+0001a280: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+0001a290: 2020 2072 6574 7572 6e20 4174 7472 6962     return Attrib
+0001a2a0: 7574 6569 6473 2c20 416c 6c56 616c 7565  uteids, AllValue
+0001a2b0: 7320 2020 2020 0d0a 2020 2020 0d0a 6465  s     ..    ..de
+0001a2c0: 6620 6765 745f 7472 6163 6b5f 6461 7461  f get_track_data
+0001a2d0: 7365 7428 7472 6163 6b5f 6461 7461 7365  set(track_datase
+0001a2e0: 742c 2074 7261 636b 5f61 6e61 6c79 7369  t, track_analysi
+0001a2f0: 735f 7370 6f74 5f6b 6579 732c 2074 7261  s_spot_keys, tra
+0001a300: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
+0001a310: 6b5f 6b65 7973 2c20 5472 6163 6b41 7474  k_keys, TrackAtt
+0001a320: 7269 6275 7465 426f 786e 616d 6529 3a0d  ributeBoxname):.
+0001a330: 0a0d 0a20 2020 2020 2020 2041 6c6c 5472  ...        AllTr
+0001a340: 6163 6b56 616c 7565 7320 3d20 7b7d 0d0a  ackValues = {}..
+0001a350: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
+0001a360: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
+0001a370: 735f 7370 6f74 5f6b 6579 735b 2274 7261  s_spot_keys["tra
+0001a380: 636b 5f69 6422 5d0d 0a20 2020 2020 2020  ck_id"]..       
+0001a390: 2054 6964 203d 2074 7261 636b 5f64 6174   Tid = track_dat
+0001a3a0: 6173 6574 5b74 7261 636b 5f69 645d 2e61  aset[track_id].a
+0001a3b0: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
+0001a3c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001a3d0: 2041 6c6c 5472 6163 6b56 616c 7565 735b   AllTrackValues[
+0001a3e0: 7472 6163 6b5f 6964 5d20 3d20 5469 640d  track_id] = Tid.
+0001a3f0: 0a20 2020 2020 200d 0a20 2020 2020 2020  .      ..       
+0001a400: 2066 6f72 2028 6b2c 2076 2920 696e 2074   for (k, v) in t
+0001a410: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
+0001a420: 6163 6b5f 6b65 7973 2e69 7465 6d73 2829  ack_keys.items()
+0001a430: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+0001a440: 2020 2020 2078 203d 2074 7261 636b 5f64       x = track_d
+0001a450: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
+0001a460: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
+0001a470: 2020 2020 2020 2020 2020 206d 696e 7661             minva
+0001a480: 6c20 3d20 6d69 6e28 7829 0d0a 2020 2020  l = min(x)..    
+0001a490: 2020 2020 2020 2020 2020 2020 6d61 7876              maxv
+0001a4a0: 616c 203d 206d 6178 2878 290d 0a0d 0a20  al = max(x).... 
+0001a4b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a4c0: 6620 6d69 6e76 616c 203e 2030 2061 6e64  f minval > 0 and
+0001a4d0: 206d 6178 7661 6c20 3c3d 2031 3a0d 0a0d   maxval <= 1:...
+0001a4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a4f0: 2020 2020 2078 203d 2078 202b 2031 0d0a       x = x + 1..
+0001a500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a510: 2020 416c 6c54 7261 636b 5661 6c75 6573    AllTrackValues
+0001a520: 5b6b 5d20 3d20 726f 756e 6428 782c 2033  [k] = round(x, 3
+0001a530: 290d 0a0d 0a20 2020 2020 2020 2054 7261  )....        Tra
+0001a540: 636b 4174 7472 6962 7574 6569 6473 203d  ckAttributeids =
+0001a550: 205b 5d0d 0a20 2020 2020 2020 2054 7261   []..        Tra
+0001a560: 636b 4174 7472 6962 7574 6569 6473 2e61  ckAttributeids.a
+0001a570: 7070 656e 6428 5472 6163 6b41 7474 7269  ppend(TrackAttri
+0001a580: 6275 7465 426f 786e 616d 6529 0d0a 2020  buteBoxname)..  
+0001a590: 2020 2020 2020 666f 7220 6174 7472 6962        for attrib
+0001a5a0: 7574 656e 616d 6520 696e 2074 7261 636b  utename in track
+0001a5b0: 5f61 6e61 6c79 7369 735f 7472 6163 6b5f  _analysis_track_
+0001a5c0: 6b65 7973 2e6b 6579 7328 293a 0d0a 2020  keys.keys():..  
+0001a5d0: 2020 2020 2020 2020 2020 5472 6163 6b41            TrackA
+0001a5e0: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
+0001a5f0: 6e64 2861 7474 7269 6275 7465 6e61 6d65  nd(attributename
+0001a600: 2920 2020 200d 0a20 2020 200d 0a20 2020  )    ..    ..   
+0001a610: 2020 2020 2072 6574 7572 6e20 5472 6163       return Trac
+0001a620: 6b41 7474 7269 6275 7465 6964 732c 2041  kAttributeids, A
+0001a630: 6c6c 5472 6163 6b56 616c 7565 730d 0a20  llTrackValues.. 
+0001a640: 2020 200d 0a64 6566 2067 6574 5f65 6467     ..def get_edg
+0001a650: 6573 5f64 6174 6173 6574 2865 6467 6573  es_dataset(edges
+0001a660: 5f64 6174 6173 6574 2c20 6564 6765 735f  _dataset, edges_
+0001a670: 6461 7461 7365 745f 696e 6465 782c 2074  dataset_index, t
+0001a680: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001a690: 6f74 5f6b 6579 732c 2074 7261 636b 5f61  ot_keys, track_a
+0001a6a0: 6e61 6c79 7369 735f 6564 6765 735f 6b65  nalysis_edges_ke
+0001a6b0: 7973 293a 0d0a 0d0a 2020 2020 2020 2020  ys):....        
+0001a6c0: 416c 6c45 6467 6573 5661 6c75 6573 203d  AllEdgesValues =
+0001a6d0: 207b 7d0d 0a20 2020 2020 2020 2074 7261   {}..        tra
+0001a6e0: 636b 5f69 6420 3d20 7472 6163 6b5f 616e  ck_id = track_an
+0001a6f0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001a700: 5b22 7472 6163 6b5f 6964 225d 0d0a 2020  ["track_id"]..  
+0001a710: 2020 2020 2020 5469 6420 3d20 6564 6765        Tid = edge
+0001a720: 735f 6461 7461 7365 745b 7472 6163 6b5f  s_dataset[track_
+0001a730: 6964 5d2e 6173 7479 7065 2822 666c 6f61  id].astype("floa
+0001a740: 7422 290d 0a20 2020 2020 2020 2069 6e64  t")..        ind
+0001a750: 6963 6573 203d 206e 702e 7768 6572 6528  ices = np.where(
+0001a760: 5469 6420 3d3d 2030 290d 0a20 2020 2020  Tid == 0)..     
+0001a770: 2020 206d 6178 7472 6163 6b5f 6964 203d     maxtrack_id =
+0001a780: 206d 6178 2854 6964 290d 0a20 2020 2020   max(Tid)..     
+0001a790: 2020 2063 6f6e 6469 7469 6f6e 5f69 6e64     condition_ind
+0001a7a0: 6963 6573 203d 2065 6467 6573 5f64 6174  ices = edges_dat
+0001a7b0: 6173 6574 5f69 6e64 6578 5b69 6e64 6963  aset_index[indic
+0001a7c0: 6573 5d0d 0a20 2020 2020 2020 2054 6964  es]..        Tid
+0001a7d0: 5b63 6f6e 6469 7469 6f6e 5f69 6e64 6963  [condition_indic
+0001a7e0: 6573 5d20 3d20 6d61 7874 7261 636b 5f69  es] = maxtrack_i
+0001a7f0: 6420 2b20 310d 0a20 2020 2020 2020 2041  d + 1..        A
+0001a800: 6c6c 4564 6765 7356 616c 7565 735b 7472  llEdgesValues[tr
+0001a810: 6163 6b5f 6964 5d20 3d20 5469 640d 0a0d  ack_id] = Tid...
+0001a820: 0a20 2020 2020 2020 2066 6f72 206b 2069  .        for k i
+0001a830: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
+0001a840: 5f65 6467 6573 5f6b 6579 732e 7661 6c75  _edges_keys.valu
+0001a850: 6573 2829 3a0d 0a0d 0a20 2020 2020 2020  es():....       
+0001a860: 2020 2020 2069 6620 6b20 213d 2074 7261       if k != tra
+0001a870: 636b 5f69 643a 0d0a 2020 2020 2020 2020  ck_id:..        
+0001a880: 2020 2020 2020 2020 7820 3d20 6564 6765          x = edge
+0001a890: 735f 6461 7461 7365 745b 6b5d 2e61 7374  s_dataset[k].ast
+0001a8a0: 7970 6528 2266 6c6f 6174 2229 0d0a 0d0a  ype("float")....
+0001a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a8c0: 416c 6c45 6467 6573 5661 6c75 6573 5b6b  AllEdgesValues[k
+0001a8d0: 5d20 3d20 7820 2020 0d0a 2020 2020 2020  ] = x   ..      
+0001a8e0: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
+0001a8f0: 7572 6e20 416c 6c45 6467 6573 5661 6c75  urn AllEdgesValu
+0001a900: 6573 2020 200d 0a20 2020 200d 0a20 2020  es   ..    ..   
+0001a910: 2020 2020 0d0a 2020 2020 0d0a 6465 6620      ..    ..def 
+0001a920: 7363 616c 655f 7661 6c75 6528 782c 2073  scale_value(x, s
+0001a930: 6361 6c65 203d 2032 3535 202a 2032 3535  cale = 255 * 255
+0001a940: 293a 0d0a 0d0a 0d0a 2020 2020 2072 6574  ):......     ret
+0001a950: 7572 6e20 7820 2a20 7363 616c 6520 2020  urn x * scale   
+0001a960: 0d0a 2020 2020 0d0a 0d0a 0d0a 6465 6620  ..    ......def 
+0001a970: 7072 6f62 5f73 6967 6d6f 6964 2878 293a  prob_sigmoid(x):
+0001a980: 0d0a 2020 2020 7265 7475 726e 2031 202d  ..    return 1 -
+0001a990: 206d 6174 682e 6578 7028 2d78 290d 0a0d   math.exp(-x)...
+0001a9a0: 0a0d 0a64 6566 2061 6e67 756c 6172 5f63  ...def angular_c
+0001a9b0: 6861 6e67 6528 7665 635f 302c 2076 6563  hange(vec_0, vec
+0001a9c0: 5f31 293a 0d0a 2020 2020 2020 2020 0d0a  _1):..        ..
+0001a9d0: 2020 2020 2020 2020 7665 635f 3020 3d20          vec_0 = 
+0001a9e0: 7665 635f 3020 2f20 6e70 2e6c 696e 616c  vec_0 / np.linal
+0001a9f0: 672e 6e6f 726d 2876 6563 5f30 290d 0a20  g.norm(vec_0).. 
+0001aa00: 2020 2020 2020 2076 6563 5f31 203d 2076         vec_1 = v
+0001aa10: 6563 5f31 202f 206e 702e 6c69 6e61 6c67  ec_1 / np.linalg
+0001aa20: 2e6e 6f72 6d28 7665 635f 3129 0d0a 2020  .norm(vec_1)..  
+0001aa30: 2020 2020 2020 616e 676c 6520 3d20 6e70        angle = np
+0001aa40: 2e61 7263 636f 7328 6e70 2e63 6c69 7028  .arccos(np.clip(
+0001aa50: 6e70 2e64 6f74 2876 6563 5f30 2c20 7665  np.dot(vec_0, ve
+0001aa60: 635f 3129 2c20 2d31 2e30 2c20 312e 3029  c_1), -1.0, 1.0)
+0001aa70: 290d 0a20 2020 2020 2020 2061 6e67 6c65  )..        angle
+0001aa80: 203d 2061 6e67 6c65 202a 2031 3830 202f   = angle * 180 /
+0001aa90: 206e 702e 7069 0d0a 2020 2020 2020 2020   np.pi..        
+0001aaa0: 7265 7475 726e 2061 6e67 6c65 0d0a 2020  return angle..  
+0001aab0: 2020 200d 0a0d 0a64 6566 2065 7661 6c5f     ....def eval_
+0001aac0: 626f 6f6c 2876 616c 7565 293a 0d0a 2020  bool(value):..  
+0001aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aae0: 0d0a 2020 2020 2020 2020 6966 2076 616c  ..        if val
+0001aaf0: 7565 2020 3d3d 2027 5472 7565 273a 200d  ue  == 'True': .
+0001ab00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ab10: 2064 6976 5f6b 6579 203d 2054 7275 650d   div_key = True.
+0001ab20: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+0001ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab40: 6469 765f 6b65 7920 3d20 4661 6c73 6520  div_key = False 
+0001ab50: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+0001ab60: 726e 2064 6976 5f6b 6579 2020 2020 2020  rn div_key      
+0001ab70: 2020 2020 2020 2020 2020 0d0a 0d0a 6465            ....de
+0001ab80: 6620 6368 6563 6b5f 616e 645f 7570 6461  f check_and_upda
+0001ab90: 7465 5f6d 6173 6b28 6d61 736b 2c69 6d61  te_mask(mask,ima
+0001aba0: 6765 293a 0d0a 2020 2020 2020 200d 0a20  ge):..       .. 
+0001abb0: 2020 2020 2020 2069 6620 6c65 6e28 6d61         if len(ma
+0001abc0: 736b 2e73 6861 7065 2920 3c20 6c65 6e28  sk.shape) < len(
+0001abd0: 696d 6167 652e 7368 6170 6529 3a0d 0a20  image.shape):.. 
+0001abe0: 2020 2020 2020 2020 2020 2075 7064 6174             updat
+0001abf0: 655f 6d61 736b 203d 206e 702e 7a65 726f  e_mask = np.zero
+0001ac00: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
+0001ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac20: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+0001ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac40: 2020 2069 6d61 6765 2e73 6861 7065 5b30     image.shape[0
+0001ac50: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+0001ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac70: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
+0001ac80: 315d 2c0d 0a20 2020 2020 2020 2020 2020  1],..           
+0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aca0: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
+0001acb0: 5b32 5d2c 0d0a 2020 2020 2020 2020 2020  [2],..          
+0001acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acd0: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
+0001ace0: 655b 335d 2c0d 0a20 2020 2020 2020 2020  e[3],..         
+0001acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad00: 2020 205d 2c20 6474 7970 653d 2275 696e     ], dtype="uin
+0001ad10: 7438 220d 0a20 2020 2020 2020 2020 2020  t8"..           
+0001ad20: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0001ad30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001ad40: 6920 696e 2072 616e 6765 2830 2c20 7570  i in range(0, up
+0001ad50: 6461 7465 5f6d 6173 6b2e 7368 6170 655b  date_mask.shape[
+0001ad60: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
+0001ad70: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+0001ad80: 616e 6765 2830 2c20 7570 6461 7465 5f6d  ange(0, update_m
+0001ad90: 6173 6b2e 7368 6170 655b 315d 293a 0d0a  ask.shape[1]):..
+0001ada0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001adb0: 2020 2020 2020 7570 6461 7465 5f6d 6173        update_mas
+0001adc0: 6b5b 692c 206a 2c20 3a2c 203a 5d20 3d20  k[i, j, :, :] = 
+0001add0: 6d61 736b 5b69 2c20 3a2c 203a 5d0d 0a20  mask[i, :, :].. 
+0001ade0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0001adf0: 2020 2020 2020 2020 2020 2020 2020 7570                up
+0001ae00: 6461 7465 5f6d 6173 6b20 3d20 6d61 736b  date_mask = mask
+0001ae10: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+0001ae20: 726e 2075 7064 6174 655f 6d61 736b 2020  rn update_mask  
+0001ae30: 2020 2020 2020 0d0a 2020 2020 2020 200d        ..       .
+0001ae40: 0a                                       .
```

### Comparing `napatrackmater-3.5.7/napatrackmater/Trackvector.py` & `napatrackmater-3.5.8/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.7/napatrackmater/__init__.py` & `napatrackmater-3.5.8/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.7/napatrackmater/clustering.py` & `napatrackmater-3.5.8/napatrackmater/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from cellshape_cluster import DeepEmbeddedClustering
-from cellshape_cloud import CloudAutoEncoder
+from kapoorlabs_lightning.pytorch_models import DeepEmbeddedClustering
 from cellshape_helper.vendor.pytorch_geometric_files import read_off, sample_points
 import numpy as np
 import concurrent 
 import os
 from pathlib import Path
 from skimage.measure import regionprops, marching_cubes
 from pyntcloud import PyntCloud
@@ -120,15 +119,15 @@
         output_labels = []
         output_cluster_score = []
         output_cluster_class = []
         output_cluster_centroid = []
         output_cloud_eccentricity = [] 
         output_cloud_surface_area = []
         output_largest_eigenvector = []
-
+        output_largest_eigenvalue = []
         dataset = PointCloudDataset(clouds, labels, centroids)
         dataloader = DataLoader(dataset, batch_size = batch_size)
         model.eval()
        
         for data in dataloader:
                 cloud_inputs, label_inputs, centroid_inputs = data
                 try:
```

### Comparing `napatrackmater-3.5.7/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.5.8/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.7/napatrackmater/fate_mapping.py` & `napatrackmater-3.5.8/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.7/napatrackmater/pretrained.py` & `napatrackmater-3.5.8/napatrackmater/pretrained.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, unicode_literals, absolute_import, division
 
 from collections import OrderedDict
 from warnings import warn
 import torch
 from pathlib import Path
-from tensorflow.keras.utils import get_file
+import tensorflow as tf
 import os 
 import json
 
 def _raise(e):
     if isinstance(e, BaseException):
         raise e
     else:
@@ -101,15 +101,15 @@
         model=key, clazz=cls.__name__, alias_str=('' if alias is None else " with alias '%s'" % alias)))
     return key, alias, models[key]
 
 
 def get_model_folder(cls, key_or_alias):
     key, alias, m = get_model_details(cls, key_or_alias)
     target = str(Path('models') / cls.__name__ / key)
-    path = Path(get_file(fname=key+'.zip', origin=m['url'], file_hash=m['hash'],
+    path = Path(tf.keras.utils.get_file(fname=key+'.zip', origin=m['url'], file_hash=m['hash'],
                          cache_subdir=target, extract=True))
     assert path.exists() and path.parent.exists()
     return path.parent, key
 
 def load_json(fpath):
     with open(fpath) as f:
```

### Comparing `napatrackmater-3.5.7/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.5.8/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.5.7
+Version: 3.5.8
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.5.7/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.5.8/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.7/setup.py` & `napatrackmater-3.5.8/setup.py`

 * *Files identical despite different names*

