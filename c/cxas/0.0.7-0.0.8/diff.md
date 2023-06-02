# Comparing `tmp/cxas-0.0.7.tar.gz` & `tmp/cxas-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxas-0.0.7.tar", last modified: Fri Jun  2 14:41:29 2023, max compression
+gzip compressed data, was "cxas-0.0.8.tar", last modified: Fri Jun  2 15:24:44 2023, max compression
```

## Comparing `cxas-0.0.7.tar` & `cxas-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 14:41:15.018508 cxas-0.0.7/
--rw-rw-r--   0 constantin (477800017) constantin (477800017)    20716 2023-06-02 08:46:00.000000 cxas-0.0.7/LICENSE.txt
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     2956 2023-06-02 14:41:15.018508 cxas-0.0.7/PKG-INFO
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     8505 2023-06-02 10:07:12.000000 cxas-0.0.7/README.md
-drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 14:41:14.834513 cxas-0.0.7/bin/
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     3845 2023-06-02 12:52:09.000000 cxas-0.0.7/bin/cxas
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     2975 2023-06-02 13:57:54.000000 cxas-0.0.7/bin/cxas_feat_extract
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     2131 2023-06-02 09:13:49.000000 cxas-0.0.7/bin/cxas_segment
-drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 14:41:14.862512 cxas-0.0.7/cxas/
--rw-rw-r--   0 constantin (477800017) constantin (477800017)       31 2023-06-02 10:42:34.000000 cxas-0.0.7/cxas/__init__.py
-drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 14:41:14.930510 cxas-0.0.7/cxas/data/
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     1157 2023-05-31 11:14:27.000000 cxas-0.0.7/cxas/data/metainfo.json
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     4294 2023-05-25 07:52:27.000000 cxas-0.0.7/cxas/data/paxray_labels.json
-drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 14:41:14.962509 cxas-0.0.7/cxas/extraction/
--rw-rw-r--   0 constantin (477800017) constantin (477800017)      892 2023-05-31 20:32:57.000000 cxas-0.0.7/cxas/extraction/__init__.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     3912 2023-06-02 08:09:51.000000 cxas-0.0.7/cxas/extraction/cardiothoracic_ratio.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)      457 2023-05-25 08:59:53.000000 cxas-0.0.7/cxas/extraction/draw_helpers.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     1107 2023-06-01 14:56:31.000000 cxas-0.0.7/cxas/extraction/func_helpers.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     2508 2023-06-02 08:11:36.000000 cxas-0.0.7/cxas/extraction/spinecenter_distance.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     9875 2023-06-02 13:47:07.000000 cxas-0.0.7/cxas/file_io.py
-drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 14:41:14.990509 cxas-0.0.7/cxas/io_utils/
--rw-rw-r--   0 constantin (477800017) constantin (477800017)      872 2023-06-02 11:55:37.000000 cxas-0.0.7/cxas/io_utils/create_annotations.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     2598 2023-06-02 13:46:23.000000 cxas-0.0.7/cxas/io_utils/dicomseg_2d.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     1357 2023-05-31 15:20:39.000000 cxas-0.0.7/cxas/io_utils/mask_to_coco.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     6337 2023-06-02 10:55:21.000000 cxas-0.0.7/cxas/label_mapper.py
-drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 14:41:14.994509 cxas-0.0.7/cxas/models/
-drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 14:41:15.014508 cxas-0.0.7/cxas/models/UNet/
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     2848 2023-05-25 15:48:49.000000 cxas-0.0.7/cxas/models/UNet/backbone_unet.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     6929 2023-05-25 15:30:59.000000 cxas-0.0.7/cxas/models/UNet/backbones.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     2973 2023-05-25 10:02:20.000000 cxas-0.0.7/cxas/models/UNet/unet_components.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     2346 2023-06-02 14:07:13.000000 cxas-0.0.7/cxas/models/__init__.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)    15854 2023-06-02 14:40:16.000000 cxas-0.0.7/cxas/segmentor.py
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     6551 2023-06-01 15:30:20.000000 cxas-0.0.7/cxas/visualize.py
-drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 14:41:14.914511 cxas-0.0.7/cxas.egg-info/
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     2956 2023-06-02 14:41:14.000000 cxas-0.0.7/cxas.egg-info/PKG-INFO
--rw-rw-r--   0 constantin (477800017) constantin (477800017)      788 2023-06-02 14:41:14.000000 cxas-0.0.7/cxas.egg-info/SOURCES.txt
--rw-rw-r--   0 constantin (477800017) constantin (477800017)        1 2023-06-02 14:41:14.000000 cxas-0.0.7/cxas.egg-info/dependency_links.txt
--rw-rw-r--   0 constantin (477800017) constantin (477800017)        1 2023-06-02 14:41:14.000000 cxas-0.0.7/cxas.egg-info/not-zip-safe
--rw-rw-r--   0 constantin (477800017) constantin (477800017)      140 2023-06-02 14:41:14.000000 cxas-0.0.7/cxas.egg-info/requires.txt
--rw-rw-r--   0 constantin (477800017) constantin (477800017)        5 2023-06-02 14:41:14.000000 cxas-0.0.7/cxas.egg-info/top_level.txt
--rw-rw-r--   0 constantin (477800017) constantin (477800017)      107 2023-06-02 14:41:15.022508 cxas-0.0.7/setup.cfg
--rw-rw-r--   0 constantin (477800017) constantin (477800017)     1685 2023-06-02 14:40:31.000000 cxas-0.0.7/setup.py
+drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 15:24:29.816887 cxas-0.0.8/
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)    20716 2023-06-02 08:46:00.000000 cxas-0.0.8/LICENSE.txt
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     2956 2023-06-02 15:24:29.820887 cxas-0.0.8/PKG-INFO
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     8505 2023-06-02 10:07:12.000000 cxas-0.0.8/README.md
+drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 15:24:29.592893 cxas-0.0.8/bin/
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     3845 2023-06-02 12:52:09.000000 cxas-0.0.8/bin/cxas
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     2975 2023-06-02 13:57:54.000000 cxas-0.0.8/bin/cxas_feat_extract
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     2131 2023-06-02 09:13:49.000000 cxas-0.0.8/bin/cxas_segment
+drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 15:24:29.628892 cxas-0.0.8/cxas/
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)       31 2023-06-02 10:42:34.000000 cxas-0.0.8/cxas/__init__.py
+drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 15:24:29.680891 cxas-0.0.8/cxas/data/
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     1157 2023-05-31 11:14:27.000000 cxas-0.0.8/cxas/data/metainfo.json
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     4294 2023-05-25 07:52:27.000000 cxas-0.0.8/cxas/data/paxray_labels.json
+drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 15:24:29.732889 cxas-0.0.8/cxas/extraction/
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)      892 2023-05-31 20:32:57.000000 cxas-0.0.8/cxas/extraction/__init__.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     3912 2023-06-02 08:09:51.000000 cxas-0.0.8/cxas/extraction/cardiothoracic_ratio.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)      457 2023-05-25 08:59:53.000000 cxas-0.0.8/cxas/extraction/draw_helpers.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     1107 2023-06-01 14:56:31.000000 cxas-0.0.8/cxas/extraction/func_helpers.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     2508 2023-06-02 08:11:36.000000 cxas-0.0.8/cxas/extraction/spinecenter_distance.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     9965 2023-06-02 15:11:43.000000 cxas-0.0.8/cxas/file_io.py
+drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 15:24:29.744889 cxas-0.0.8/cxas/io_utils/
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)      872 2023-06-02 11:55:37.000000 cxas-0.0.8/cxas/io_utils/create_annotations.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     2598 2023-06-02 13:46:23.000000 cxas-0.0.8/cxas/io_utils/dicomseg_2d.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     1357 2023-05-31 15:20:39.000000 cxas-0.0.8/cxas/io_utils/mask_to_coco.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     6337 2023-06-02 10:55:21.000000 cxas-0.0.8/cxas/label_mapper.py
+drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 15:24:29.744889 cxas-0.0.8/cxas/models/
+drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 15:24:29.808887 cxas-0.0.8/cxas/models/UNet/
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     2848 2023-05-25 15:48:49.000000 cxas-0.0.8/cxas/models/UNet/backbone_unet.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     6929 2023-05-25 15:30:59.000000 cxas-0.0.8/cxas/models/UNet/backbones.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     2973 2023-05-25 10:02:20.000000 cxas-0.0.8/cxas/models/UNet/unet_components.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     2346 2023-06-02 14:07:13.000000 cxas-0.0.8/cxas/models/__init__.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)    15854 2023-06-02 14:40:16.000000 cxas-0.0.8/cxas/segmentor.py
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     6551 2023-06-01 15:30:20.000000 cxas-0.0.8/cxas/visualize.py
+drwxrwsr-x   0 constantin (477800017) constantin (477800017)        0 2023-06-02 15:24:29.664891 cxas-0.0.8/cxas.egg-info/
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     2956 2023-06-02 15:24:28.000000 cxas-0.0.8/cxas.egg-info/PKG-INFO
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)      788 2023-06-02 15:24:29.000000 cxas-0.0.8/cxas.egg-info/SOURCES.txt
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)        1 2023-06-02 15:24:28.000000 cxas-0.0.8/cxas.egg-info/dependency_links.txt
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)        1 2023-06-02 15:24:28.000000 cxas-0.0.8/cxas.egg-info/not-zip-safe
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)      140 2023-06-02 15:24:28.000000 cxas-0.0.8/cxas.egg-info/requires.txt
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)        5 2023-06-02 15:24:28.000000 cxas-0.0.8/cxas.egg-info/top_level.txt
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)      107 2023-06-02 15:24:29.824887 cxas-0.0.8/setup.cfg
+-rw-rw-r--   0 constantin (477800017) constantin (477800017)     1685 2023-06-02 15:24:19.000000 cxas-0.0.8/setup.py
```

### Comparing `cxas-0.0.7/LICENSE.txt` & `cxas-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/PKG-INFO` & `cxas-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxas
-Version: 0.0.7
+Version: 0.0.8
 Summary: Segmentation of 159 anatomical classes for Chest X-Rays.
 Home-page: https://github.com/ConstantinSeibold/ChestXRayAnatomySegmentation
 Author: Constantin Seibold
 Author-email: constantin.seibold2@uk-essen.de
 Keywords: chest x-ray anatomy segmntation pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cxas-0.0.7/README.md` & `cxas-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/bin/cxas` & `cxas-0.0.8/bin/cxas`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/bin/cxas_feat_extract` & `cxas-0.0.8/bin/cxas_feat_extract`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/bin/cxas_segment` & `cxas-0.0.8/bin/cxas_segment`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/data/metainfo.json` & `cxas-0.0.8/cxas/data/metainfo.json`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/data/paxray_labels.json` & `cxas-0.0.8/cxas/data/paxray_labels.json`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/extraction/__init__.py` & `cxas-0.0.8/cxas/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/extraction/cardiothoracic_ratio.py` & `cxas-0.0.8/cxas/extraction/cardiothoracic_ratio.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/extraction/func_helpers.py` & `cxas-0.0.8/cxas/extraction/func_helpers.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/extraction/spinecenter_distance.py` & `cxas-0.0.8/cxas/extraction/spinecenter_distance.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/file_io.py` & `cxas-0.0.8/cxas/file_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,15 +177,15 @@
                                       outdir:str,  
                                       file_name:str
                                      ) -> None:
         """
         """
         assert os.path.splitext(file_name)[-1] == 'dcm', 'Input file has to be dicom to be stored \
             as dicom-seg, it was --{}--'.format(os.path.splitext(file_name)[-1])
-        out_dir = os.path.join(outdir, os.path.splitext(file_name)[0])
+        out_dir = os.path.join(outdir, os.path.splitext(file_name)[0].split('/')[-1])
         os.makedirs(out_dir,exist_ok=True)
         
         write_dicom_seg(
                             metainfo = os.path.join(str(this_directory), 'data/metainfo.json'),
                             dcm_file = file_name,
                             mask = mask.astype(np.uint8),
                             out_dir = out_dir,
@@ -197,15 +197,15 @@
                                  mask:np.array, 
                                  outdir:str,  
                                  file_name:str
                                 ) -> None:
         """
         """
         assert len(mask.shape) == 3
-        fileroot = os.path.splitext(file_name)[0]
+        fileroot = os.path.splitext(file_name)[0].split('/')[-1]
         outdir = os.path.join(outdir, fileroot)
         os.makedirs(outdir,exist_ok=True)
         
         for i in range(len(mask)):
             out_path = os.path.join(outdir, id2label_dict[str(i)] + '.jpg')
             Image.fromarray(mask[i]).convert('1').save(out_path)
     
@@ -213,15 +213,15 @@
                                  mask:np.array, 
                                  outdir:str,  
                                  file_name:str
                                 ) -> None:
         """
         """
         assert len(mask.shape) == 3
-        fileroot = os.path.splitext(file_name)[0]
+        fileroot = os.path.splitext(file_name)[0].split('/')[-1]
         outdir = os.path.join(outdir, fileroot)
         os.makedirs(outdir,exist_ok=True)
         
         for i in range(len(mask)):
             out_path = os.path.join(outdir, id2label_dict[str(i)] + '.png')
             Image.fromarray(mask[i]).convert('1').save(out_path)
 
@@ -229,24 +229,24 @@
                                    mask:np.array, 
                                    outdir:str,  
                                    file_name:str
                                   ) -> None:
         """
         """
         os.makedirs(outdir,exist_ok=True)
-        out_path = os.path.join(outdir, os.path.splitext(file_name)[0]+'.npy')
+        out_path = os.path.join(outdir, os.path.splitext(file_name)[0].split('/')[-1]+'.npy')
         np.save(out_path, mask)
     
     def export_prediction_as_npz(self, 
                                  mask:np.array,
                                  outdir:str,  
                                  file_name:str
                                 ) -> None:
         os.makedirs(outdir,exist_ok=True)
-        out_path = os.path.join(outdir, os.path.splitext(file_name)[0]+'.npz')
+        out_path = os.path.join(outdir, os.path.splitext(file_name)[0].split('/')[-1]+'.npz')
         np.savez_compressed(out_path, mask)
 
     
     def export_prediction_as_json(self, 
                                   mask:np.array, 
                                   outdir:str,  
                                   file_name:str,
@@ -263,11 +263,11 @@
         coco_format["annotations"] = mask_to_annotation(
                                         mask = mask, 
                                         base_ann_id = base_ann_id, 
                                         img_id = img_id
                                     ) 
         
         os.makedirs(outdir,exist_ok=True)
-        out_path = os.path.join(outdir, os.path.splitext(file_name)[0]+'.json')
+        out_path = os.path.join(outdir, os.path.splitext(file_name)[0].split('/')[-1]+'.json')
         
         with open(out_path,"w") as outfile:
             json.dump(coco_format, outfile)
```

### Comparing `cxas-0.0.7/cxas/io_utils/create_annotations.py` & `cxas-0.0.8/cxas/io_utils/create_annotations.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/io_utils/dicomseg_2d.py` & `cxas-0.0.8/cxas/io_utils/dicomseg_2d.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/io_utils/mask_to_coco.py` & `cxas-0.0.8/cxas/io_utils/mask_to_coco.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/label_mapper.py` & `cxas-0.0.8/cxas/label_mapper.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/models/UNet/backbone_unet.py` & `cxas-0.0.8/cxas/models/UNet/backbone_unet.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/models/UNet/backbones.py` & `cxas-0.0.8/cxas/models/UNet/backbones.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/models/UNet/unet_components.py` & `cxas-0.0.8/cxas/models/UNet/unet_components.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/models/__init__.py` & `cxas-0.0.8/cxas/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/segmentor.py` & `cxas-0.0.8/cxas/segmentor.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas/visualize.py` & `cxas-0.0.8/cxas/visualize.py`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/cxas.egg-info/PKG-INFO` & `cxas-0.0.8/cxas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxas
-Version: 0.0.7
+Version: 0.0.8
 Summary: Segmentation of 159 anatomical classes for Chest X-Rays.
 Home-page: https://github.com/ConstantinSeibold/ChestXRayAnatomySegmentation
 Author: Constantin Seibold
 Author-email: constantin.seibold2@uk-essen.de
 Keywords: chest x-ray anatomy segmntation pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cxas-0.0.7/cxas.egg-info/SOURCES.txt` & `cxas-0.0.8/cxas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cxas-0.0.7/setup.py` & `cxas-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "docs/shortREADME.rst").read_text()
 
 setup(name='cxas',
-        version='0.0.7',
+        version='0.0.8',
         description='Segmentation of 159 anatomical classes for Chest X-Rays.',
         long_description = long_description,
         long_description_content_type="text/x-rst",
         url='https://github.com/ConstantinSeibold/ChestXRayAnatomySegmentation',
         author='Constantin Seibold',
         author_email='constantin.seibold2@uk-essen.de',
         python_requires='>=3.9',
```

