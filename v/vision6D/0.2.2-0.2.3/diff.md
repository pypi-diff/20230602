# Comparing `tmp/vision6D-0.2.2.tar.gz` & `tmp/vision6D-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision6D-0.2.2.tar", last modified: Wed May 31 22:35:53 2023, max compression
+gzip compressed data, was "vision6D-0.2.3.tar", last modified: Fri Jun  2 01:17:23 2023, max compression
```

## Comparing `vision6D-0.2.2.tar` & `vision6D-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:35:53.131219 vision6D-0.2.2/
--rw-rw-rw-   0        0        0     1086 2023-05-31 22:25:29.000000 vision6D-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1365 2023-05-31 22:35:53.132218 vision6D-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-05-31 22:34:31.000000 vision6D-0.2.2/README.md
--rw-rw-rw-   0        0        0      406 2023-05-31 22:25:29.000000 vision6D-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0     2050 2023-05-31 22:35:53.137219 vision6D-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      282 2023-05-31 22:25:29.000000 vision6D-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:35:52.786213 vision6D-0.2.2/test/
--rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.2/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.2/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:35:52.989220 vision6D-0.2.2/vision6D/
--rw-rw-rw-   0        0        0    51735 2023-05-31 22:25:29.000000 vision6D-0.2.2/vision6D/GUI.py
--rw-rw-rw-   0        0        0      913 2023-05-31 22:25:29.000000 vision6D-0.2.2/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.2.2/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-31 22:25:29.000000 vision6D-0.2.2/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:35:53.121218 vision6D-0.2.2/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.2/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.2/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.2.2/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.2.2/vision6D/interface.py
--rw-rw-rw-   0        0        0    26253 2023-05-31 22:25:29.000000 vision6D-0.2.2/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.2.2/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.2.2/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.2.2/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.2.2/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:35:53.061218 vision6D-0.2.2/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1365 2023-05-31 22:35:52.000000 vision6D-0.2.2/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-05-31 22:35:52.000000 vision6D-0.2.2/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:35:52.000000 vision6D-0.2.2/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-31 22:35:52.000000 vision6D-0.2.2/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-05-31 22:35:52.000000 vision6D-0.2.2/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 22:35:52.000000 vision6D-0.2.2/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 01:17:23.606736 vision6D-0.2.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-01 02:48:31.000000 vision6D-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1365 2023-06-02 01:17:23.607365 vision6D-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-06-01 02:48:31.000000 vision6D-0.2.3/README.md
+-rw-rw-rw-   0        0        0      406 2023-06-01 02:48:31.000000 vision6D-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0     2050 2023-06-02 01:17:23.614366 vision6D-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      282 2023-06-01 02:48:31.000000 vision6D-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:17:23.416368 vision6D-0.2.3/test/
+-rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.3/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.3/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:17:23.472000 vision6D-0.2.3/vision6D/
+-rw-rw-rw-   0        0        0    51909 2023-06-02 01:15:28.000000 vision6D-0.2.3/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      913 2023-06-01 02:48:31.000000 vision6D-0.2.3/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.2.3/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-06-01 02:48:31.000000 vision6D-0.2.3/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:17:23.601096 vision6D-0.2.3/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.3/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.3/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.2.3/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.2.3/vision6D/interface.py
+-rw-rw-rw-   0        0        0    26253 2023-06-01 02:48:31.000000 vision6D-0.2.3/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.2.3/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.2.3/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.2.3/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.2.3/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:17:23.549804 vision6D-0.2.3/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1365 2023-06-02 01:17:22.000000 vision6D-0.2.3/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-06-02 01:17:23.000000 vision6D-0.2.3/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 01:17:22.000000 vision6D-0.2.3/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-02 01:17:22.000000 vision6D-0.2.3/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-06-02 01:17:23.000000 vision6D-0.2.3/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 01:17:23.000000 vision6D-0.2.3/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.2.2/LICENSE` & `vision6D-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/PKG-INFO` & `vision6D-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.2
+Version: 0.2.3
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.2.2/README.md` & `vision6D-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/setup.cfg` & `vision6D-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e32 2e32 0d0a 7572  sion = 0.2.2..ur
+00000020: 7369 6f6e 203d 2030 2e32 2e33 0d0a 7572  sion = 0.2.3..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.2.2/test/test_create_dataset.py` & `vision6D-0.2.3/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/test/test_projection.py` & `vision6D-0.2.3/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/GUI.py` & `vision6D-0.2.3/vision6D/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,15 @@
 
     def dropEvent(self, e):
         for url in e.mimeData().urls():
             file_path = url.toLocalFile()
             if file_path.endswith(('.mesh', '.ply', '.stl', '.obj', '.off', '.dae', '.fbx', '.3ds', '.x3d')):  # add mesh
                 self.mesh_path = file_path
                 self.add_mesh_file(prompt=False)
-            elif file_path.endswith(('.png', '.jpg')):  # add image/mask
+            elif file_path.endswith(('.png', '.jpg', 'jpeg', '.tiff', '.bmp', '.webp', '.ico')):  # add image/mask
                 yes_no_box = YesNoBox()
                 yes_no_box.setIcon(QtWidgets.QMessageBox.Question)
                 yes_no_box.setWindowTitle("Vision6D")
                 yes_no_box.setText("Do you want to load the image as mask?")
                 yes_no_box.setStandardButtons(QtWidgets.QMessageBox.Yes | QtWidgets.QMessageBox.No)
                 button_clicked = yes_no_box.exec_()
                 if not yes_no_box.canceled:
@@ -480,30 +480,30 @@
 
             # reset camera
             self.reset_camera()
 
     def add_image_file(self, prompt=True):
         if prompt:
             if self.image_path == None or self.image_path == '':
-                self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg)")
+                self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)")
             else:
-                self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.image_path).parent), "Files (*.png *.jpg)")
+                self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.image_path).parent), "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)")
 
         if self.image_path != '' and self.image_path is not None:
             self.hintLabel.hide()
             image_source = np.array(PIL.Image.open(self.image_path), dtype='uint8')
             if len(image_source.shape) == 2: image_source = image_source[..., None]
             self.add_image(image_source)
             
     def add_mask_file(self, prompt=True):
         if prompt:
             if self.mask_path == None or self.mask_path == '':
-                self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg)")
+                self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)")
             else:
-                self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.mask_path).parent), "Files (*.png *.jpg)")
+                self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.mask_path).parent), "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)")
         
         if self.mask_path != '' and self.mask_path is not None:
             self.hintLabel.hide()
             mask_source = np.array(PIL.Image.open(self.mask_path), dtype='uint8')
             if len(mask_source.shape) == 2: mask_source = mask_source[..., None]
             self.add_mask(mask_source)
```

### Comparing `vision6D-0.2.2/vision6D/__init__.py` & `vision6D-0.2.3/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/app.py` & `vision6D-0.2.3/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/config.py` & `vision6D-0.2.3/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.2.3/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.2.3/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/data/style.qss` & `vision6D-0.2.3/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/interface.py` & `vision6D-0.2.3/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/interface_gui.py` & `vision6D-0.2.3/vision6D/interface_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/mainwindow.py` & `vision6D-0.2.3/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/run_gui.py` & `vision6D-0.2.3/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D/utils.py` & `vision6D-0.2.3/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.2/vision6D.egg-info/PKG-INFO` & `vision6D-0.2.3/vision6D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.2
+Version: 0.2.3
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.2.2/vision6D.egg-info/SOURCES.txt` & `vision6D-0.2.3/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

