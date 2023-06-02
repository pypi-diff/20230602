# Comparing `tmp/usls-0.2.5-py3-none-any.whl.zip` & `tmp/usls-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 43227 bytes, number of entries: 20
--rw-r--r--  2.0 unx      256 b- defN 23-May-07 10:05 usls/__init__.py
--rw-r--r--  2.0 unx    12485 b- defN 23-May-07 09:50 usls/cli.py
--rw-r--r--  2.0 unx      276 b- defN 23-May-07 06:11 usls/src/__init__.py
--rw-r--r--  2.0 unx     2171 b- defN 23-May-07 06:11 usls/src/class_modify.py
--rw-r--r--  2.0 unx     6119 b- defN 23-May-07 06:11 usls/src/cleanup.py
--rw-r--r--  2.0 unx     5518 b- defN 23-May-07 07:36 usls/src/deduplicate.py
--rw-r--r--  2.0 unx     2071 b- defN 23-May-07 06:11 usls/src/dir_combine.py
--rw-r--r--  2.0 unx     4010 b- defN 23-May-07 06:11 usls/src/info.py
--rw-r--r--  2.0 unx     3204 b- defN 23-May-07 06:11 usls/src/label_combine.py
--rw-r--r--  2.0 unx    35075 b- defN 23-May-07 10:00 usls/src/labelling.py
--rw-r--r--  2.0 unx     2616 b- defN 23-May-07 06:11 usls/src/rename.py
--rw-r--r--  2.0 unx     3462 b- defN 23-May-07 07:36 usls/src/spider.py
--rw-r--r--  2.0 unx     9547 b- defN 23-May-07 10:05 usls/src/utils.py
--rw-r--r--  2.0 unx     9396 b- defN 23-May-07 07:38 usls/src/video_tools.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-07 10:09 usls-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      540 b- defN 23-May-07 10:09 usls-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 10:09 usls-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       34 b- defN 23-May-07 10:09 usls-0.2.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-May-07 10:09 usls-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1534 b- defN 23-May-07 10:09 usls-0.2.5.dist-info/RECORD
-20 files, 133560 bytes uncompressed, 40775 bytes compressed:  69.5%
+Zip file size: 43201 bytes, number of entries: 20
+-rwxrwxrwx  2.0 unx      256 b- defN 23-Jun-02 02:40 usls/__init__.py
+-rwxrwxrwx  2.0 unx    12485 b- defN 23-Jun-02 02:17 usls/cli.py
+-rwxrwxrwx  2.0 unx      276 b- defN 23-Jun-02 02:17 usls/src/__init__.py
+-rwxrwxrwx  2.0 unx     2171 b- defN 23-Jun-02 02:17 usls/src/class_modify.py
+-rwxrwxrwx  2.0 unx     6119 b- defN 23-Jun-02 02:17 usls/src/cleanup.py
+-rwxrwxrwx  2.0 unx     5518 b- defN 23-Jun-02 02:17 usls/src/deduplicate.py
+-rwxrwxrwx  2.0 unx     2071 b- defN 23-Jun-02 02:17 usls/src/dir_combine.py
+-rwxrwxrwx  2.0 unx     4010 b- defN 23-Jun-02 02:17 usls/src/info.py
+-rwxrwxrwx  2.0 unx     3204 b- defN 23-Jun-02 02:17 usls/src/label_combine.py
+-rwxrwxrwx  2.0 unx    35024 b- defN 23-Jun-02 02:39 usls/src/labelling.py
+-rwxrwxrwx  2.0 unx     2616 b- defN 23-Jun-02 02:17 usls/src/rename.py
+-rwxrwxrwx  2.0 unx     3462 b- defN 23-Jun-02 02:17 usls/src/spider.py
+-rwxrwxrwx  2.0 unx     9547 b- defN 23-Jun-02 02:17 usls/src/utils.py
+-rwxrwxrwx  2.0 unx     9396 b- defN 23-Jun-02 02:17 usls/src/video_tools.py
+-rwxrwxrwx  2.0 unx    35149 b- defN 23-Jun-02 02:40 usls-0.2.6.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx      540 b- defN 23-Jun-02 02:40 usls-0.2.6.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-02 02:40 usls-0.2.6.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       34 b- defN 23-Jun-02 02:40 usls-0.2.6.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx        5 b- defN 23-Jun-02 02:40 usls-0.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1534 b- defN 23-Jun-02 02:40 usls-0.2.6.dist-info/RECORD
+20 files, 133509 bytes uncompressed, 40749 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: usls/src/utils.py
 Comment: 
 
 Filename: usls/src/video_tools.py
 Comment: 
 
-Filename: usls-0.2.5.dist-info/LICENSE
+Filename: usls-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: usls-0.2.5.dist-info/METADATA
+Filename: usls-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: usls-0.2.5.dist-info/WHEEL
+Filename: usls-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: usls-0.2.5.dist-info/entry_points.txt
+Filename: usls-0.2.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: usls-0.2.5.dist-info/top_level.txt
+Filename: usls-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: usls-0.2.5.dist-info/RECORD
+Filename: usls-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## usls/__init__.py

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*- 
 
-__version__ = '0.2.5'
+__version__ = '0.2.6'
 
 
 from usls.cli import cli
 from usls.src.utils import (
 	SmartDir, smart_path, TIMER, Palette
 )
```

## usls/src/labelling.py

```diff
@@ -480,17 +480,17 @@
             img_h, 
             eps=1e-8
         ):
         # idxyxy -> idcxcywh
 
         # boundary check and rectify
         det_points.tl.x = min(max(eps, det_points.tl.x), img_w - eps) 
-        det_points.br.x = max(min(img_w - eps, det_points.br.x), eps)
+        det_points.br.x = min(max(eps, det_points.br.x), img_w - eps) 
         det_points.tl.y = min(max(eps, det_points.tl.y), img_h - eps) 
-        det_points.br.y = max(min(img_w - eps, det_points.br.y), eps)
+        det_points.br.y = min(max(eps, det_points.br.y), img_h - eps)
 
         # check again
         # if (det_points.tl.x >= det_points.br.x) or (det_points.tl.y >= det_points.br.y):
         #     raise ValueError(f'point of bottom-right {det_points.br} should greater than point of top-left {det_points.tl}')
 
         # convert
         cx = float((det_points.tl.x + det_points.br.x) / (2.0 * img_w) )
@@ -651,15 +651,14 @@
         if self.mode == InspectMode.mark_dets:
             if event == cv2.EVENT_MOUSEMOVE:
                 self.CURSOR.x = x
                 self.CURSOR.y = y
 
             # left button double click -> select object
             elif event == cv2.EVENT_LBUTTONDBLCLK:
-                print(f'----> double click')
                 self.PRVE_WAS_DOUBLE_CLICK = True    
                 self.POINTS_DET.tl = Point(-1, -1)   # reset top_left point
 
                 # if clicked inside a bounding box we set that bbox
                 self.set_selected_bbox(set_cls_trackbar=True)
 
             # right button pressed down
@@ -683,15 +682,16 @@
                             self.HAS_BBOX_SELECTED = False
                         else:  # first click
                             self.POINTS_DET.tl = Point(x, y)  # top-left point
                     else:  # second click
                         _threshold = 5  # minimal size for bounding box to avoid errors
                         if abs(x - self.POINTS_DET.tl.x) > _threshold or abs(y - self.POINTS_DET.tl.y) > _threshold:
                             self.POINTS_DET.br = Point(x, y)    # bottom-right point
-        
+
+
         # -------------------------
         #   doodle mode
         # -------------------------            
         elif self.mode == InspectMode.doodle:
             pass
```

## Comparing `usls-0.2.5.dist-info/LICENSE` & `usls-0.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `usls-0.2.5.dist-info/METADATA` & `usls-0.2.6.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usls
-Version: 0.2.5
+Version: 0.2.6
 Summary: Useless CV toolkits
 Home-page: https://github.com/jamjamjon/usls
 Author: jamjamjon
 License: GPL-3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `usls-0.2.5.dist-info/RECORD` & `usls-0.2.6.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-usls/__init__.py,sha256=5f4GnvcJh9-H--K448SdJTlBIs5TOfqv17HjxxDzdUc,256
+usls/__init__.py,sha256=z5BgLTWUVYdJbrbi3zBTxE5wEjeVC8q3NJ5hFBBvv8Q,256
 usls/cli.py,sha256=6KW57Z5r3x4uxi2JT8KVtzVJEWpW6SAR67PSxX1dsRA,12485
 usls/src/__init__.py,sha256=x_CWzE-z_jOmeRTUbEjDZ7jMmw1vc2ZYes2ztGRYWyg,276
 usls/src/class_modify.py,sha256=MVwj18Z47GV67EfLv77wEKMfRLT2DgOmckQPFQQkU2I,2171
 usls/src/cleanup.py,sha256=owKLqy3pUI9O7e1FiIJz2JWKl4Y0bLlbdZYccZmPFtk,6119
 usls/src/deduplicate.py,sha256=JyPoGQEySFVgMmabDOtxRvd16Y3-W0rk8y4BXuiqkFk,5518
 usls/src/dir_combine.py,sha256=7xlIFvksHWn53awmp_0jCFbJPbglTEsRiWIgrFNZFwo,2071
 usls/src/info.py,sha256=bYY6yaWDGnv1Fz5E2tBNCKaqKVQbxEom1Ba8vHGrNqA,4010
 usls/src/label_combine.py,sha256=T99nvA4fcHt94cCV9zZVPJvmgj_Lus-5H3lowCbp9So,3204
-usls/src/labelling.py,sha256=FRtd2RA_xOkMXB7jLmdJF4v0C7VzLwCUpvZd4W3Jun0,35075
+usls/src/labelling.py,sha256=qSvDr0WQboM-6k9YzRdhDxFwf4DdpakxaAdJSWwqUXk,35024
 usls/src/rename.py,sha256=2vqbHZUCjuxVOwM99Mz8Mng9SQ6Li0SE2HQxa7yq9k8,2616
 usls/src/spider.py,sha256=RKU2xcopolQx2Sae_J4J7-TDXVkfwkgfAg7llA3piWU,3462
 usls/src/utils.py,sha256=S7-S9qbae3VD-ON4vQZRgnxGr4v1TBZpyVTz5Q4Qulk,9547
 usls/src/video_tools.py,sha256=EKx3Zg1Vg6A-8HjuH4s9oPBxYS2upSkbDGQpwdlGIng,9396
-usls-0.2.5.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-usls-0.2.5.dist-info/METADATA,sha256=jvhtt9TjFI4cesOuD_QR3_313WkZIkjf-LRPBnvAajw,540
-usls-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-usls-0.2.5.dist-info/entry_points.txt,sha256=NtT7OjVpekraB5xlzXzTbTQ9q8VOKMUrByrtciZMJms,34
-usls-0.2.5.dist-info/top_level.txt,sha256=oS7b-J2DgqOuJIQaKnSyirCC_Rt6yeQCLkbNqh2H_DM,5
-usls-0.2.5.dist-info/RECORD,,
+usls-0.2.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+usls-0.2.6.dist-info/METADATA,sha256=IJ7R_id7gEWbviZOVTwLk0UfdgX5J2XnJsF3is-Uksw,540
+usls-0.2.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+usls-0.2.6.dist-info/entry_points.txt,sha256=NtT7OjVpekraB5xlzXzTbTQ9q8VOKMUrByrtciZMJms,34
+usls-0.2.6.dist-info/top_level.txt,sha256=oS7b-J2DgqOuJIQaKnSyirCC_Rt6yeQCLkbNqh2H_DM,5
+usls-0.2.6.dist-info/RECORD,,
```

