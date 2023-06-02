# Comparing `tmp/labelme2yolo-0.1.1.tar.gz` & `tmp/labelme2yolo-0.1.2.tar.gz`

## Comparing `labelme2yolo-0.1.1.tar` & `labelme2yolo-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/requirements.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/__about__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/__main__.py
--rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/l2y.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/cli/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/LICENSE
--rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/README.md
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    21203 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/.pylintrc
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/src/labelme2yolo/__about__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/src/labelme2yolo/__init__.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/src/labelme2yolo/__main__.py
+-rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/src/labelme2yolo/l2y.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/src/labelme2yolo/cli/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/README.md
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 labelme2yolo-0.1.2/PKG-INFO
```

### Comparing `labelme2yolo-0.1.1/src/labelme2yolo/l2y.py` & `labelme2yolo-0.1.2/src/labelme2yolo/l2y.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,106 +23,122 @@
 
 # number of LabelMe2YOLO multiprocessing threads
 NUM_THREADS = max(1, os.cpu_count() - 1)
 
 
 # copy form https://github.com/wkentaro/labelme/blob/main/labelme/utils/image.py
 def img_data_to_pil(img_data):
-    f = io.BytesIO()
-    f.write(img_data)
-    img_pil = PIL.Image.open(f)
+    '''Convert img_data(byte) to PIL.Image'''
+    file = io.BytesIO()
+    file.write(img_data)
+    img_pil = PIL.Image.open(file)
     return img_pil
 
 
 # copy form https://github.com/wkentaro/labelme/blob/main/labelme/utils/image.py
 def img_data_to_arr(img_data):
+    '''Convert img_data(byte) to numpy.ndarray'''
     img_pil = img_data_to_pil(img_data)
     img_arr = np.array(img_pil)
     return img_arr
 
 
 # copy form https://github.com/wkentaro/labelme/blob/main/labelme/utils/image.py
 def img_b64_to_arr(img_b64):
+    '''Convert img_b64(str) to numpy.ndarray'''
     img_data = base64.b64decode(img_b64)
     img_arr = img_data_to_arr(img_data)
     return img_arr
 
 
 # copy form https://github.com/wkentaro/labelme/blob/main/labelme/utils/image.py
 def img_pil_to_data(img_pil):
-    f = io.BytesIO()
-    img_pil.save(f, format="PNG")
-    img_data = f.getvalue()
+    '''Convert PIL.Image to img_data(byte)'''
+    file = io.BytesIO()
+    img_pil.save(file, format="PNG")
+    img_data = file.getvalue()
     return img_data
 
 
 # copy form https://github.com/wkentaro/labelme/blob/main/labelme/utils/image.py
 def img_arr_to_b64(img_arr):
+    '''Convert numpy.ndarray to img_b64(str)'''
     img_pil = PIL.Image.fromarray(img_arr)
-    f = io.BytesIO()
-    img_pil.save(f, format="PNG")
-    img_bin = f.getvalue()
+    file = io.BytesIO()
+    img_pil.save(file, format="PNG")
+    img_bin = file.getvalue()
     if hasattr(base64, "encodebytes"):
         img_b64 = base64.encodebytes(img_bin)
     else:
         img_b64 = base64.encodestring(img_bin)
     return img_b64
 
 
 # copy form https://github.com/wkentaro/labelme/blob/main/labelme/utils/image.py
 def img_data_to_png_data(img_data):
+    '''Convert img_data(byte) to png_data(byte)'''
     with io.BytesIO() as f_out:
         f_out.write(img_data)
         img = PIL.Image.open(f_out)
 
         with io.BytesIO() as f_in:
             img.save(f_in, "PNG")
             f_in.seek(0)
             return f_in.read()
 
 
 def get_label_id_map(json_dir: str):
+    '''Get label id map from json files in json_dir'''
     label_set = set()
 
     for file_name in os.listdir(json_dir):
         if file_name.endswith("json"):
             json_path = os.path.join(json_dir, file_name)
             data = json.load(open(json_path))
             for shape in data["shapes"]:
                 label_set.add(shape["label"])
 
     return OrderedDict([(label, label_id) for label_id, label in enumerate(label_set)])
 
 
 def extend_point_list(point_list, out_format="polygon"):
+    '''Extend point list to polygon or bbox'''
     xmin = min([float(point) for point in point_list[::2]])
     xmax = max([float(point) for point in point_list[::2]])
     ymin = min([float(point) for point in point_list[1::2]])
     ymax = max([float(point) for point in point_list[1::2]])
 
-    if (out_format == "polygon"):
+    if out_format == "polygon":
         return np.array([xmin, ymin, xmax, ymin, xmax, ymax, xmin, ymax])
-    if (out_format == "bbox"):
-        return np.array([xmin, ymin, xmax - xmin, ymax - ymin])
+    if out_format == "bbox":
+        x = xmin
+        y = ymin
+        w = xmax - xmin
+        h = ymax - ymin
+        x = x + w / 2
+        y = y + h / 2
+        return np.array([x, y, w, h])
 
 
 def save_yolo_label(json_name, label_dir_path, target_dir, yolo_obj_list):
+    '''Save yolo label to txt file'''
     txt_path = os.path.join(label_dir_path,
                             target_dir,
                             json_name.replace(".json", ".txt"))
 
     with open(txt_path, "w+") as f:
         for yolo_obj in yolo_obj_list:
             label, points = yolo_obj
             points = [str(item) for item in points]
             yolo_obj_line = f"{label} {' '.join(points)}\n"
             f.write(yolo_obj_line)
 
 
 def save_yolo_image(json_data, json_path, image_dir_path, target_dir):
+    '''Save yolo image to image_dir_path/target_dir'''
     json_name = os.path.basename(json_path)
     img_name = json_name.replace(".json", ".png")
 
     # make image_path and save image
     img_path = os.path.join(image_dir_path, target_dir, img_name)
 
     if json_data["imageData"] is None:
@@ -135,15 +151,15 @@
         img = img_b64_to_arr(json_data["imageData"])
         PIL.Image.fromarray(img).save(img_path)
 
     return img_path
 
 
 class Labelme2YOLO(object):
-
+    '''Labelme to YOLO format converter'''
     def __init__(self, json_dir, output_format, label_list):
         self._json_dir = json_dir
         self._output_format = output_format
         self._label_list = label_list
 
         if label_list:
             self._label_id_map = {label: label_id
@@ -166,35 +182,34 @@
                           os.path.join(self._image_dir_path + 'test/')):
             if os.path.exists(yolo_path):
                 shutil.rmtree(yolo_path)
 
             os.makedirs(yolo_path)
 
     def _train_test_split(self, folders, json_names, val_size, test_size):
-        if len(folders) > 0 and 'train' in folders and 'val' in folders and 'test' in folders:
+        if len(folders) > 0 and 'train' in folders and 'val' in folders and 'test' in folders:  # noqa: E501
             train_folder = os.path.join(self._json_dir, 'train/')
             train_json_names = [train_sample_name + '.json'
                                 for train_sample_name in os.listdir(train_folder)
-                                if os.path.isdir(os.path.join(train_folder, train_sample_name))]
+                                if os.path.isdir(os.path.join(train_folder, train_sample_name))]  # noqa: E501
 
             val_folder = os.path.join(self._json_dir, 'val/')
             val_json_names = [val_sample_name + '.json'
                               for val_sample_name in os.listdir(val_folder)
-                              if os.path.isdir(os.path.join(val_folder, val_sample_name))]
+                              if os.path.isdir(os.path.join(val_folder, val_sample_name))]  # noqa: E501
 
             test_folder = os.path.join(self._json_dir, 'test/')
             test_json_names = [test_sample_name + '.json'
                                for test_sample_name in os.listdir(test_folder)
-                               if os.path.isdir(os.path.join(test_folder, test_sample_name))]
+                               if os.path.isdir(os.path.join(test_folder, test_sample_name))]  # noqa: E501
 
             return train_json_names, val_json_names, test_json_names
 
         train_idxs, val_idxs = train_test_split(range(len(json_names)),
                                                 test_size=val_size)
-        tmp_train_len = len(train_idxs)
         test_idxs = []
         if test_size is None:
             test_size = 0.0
         if test_size > 1e-8:
             train_idxs, test_idxs = train_test_split(
                 train_idxs, test_size=test_size / (1 - val_size))
         train_json_names = [json_names[train_idx] for train_idx in train_idxs]
@@ -213,15 +228,15 @@
             folders, json_names, val_size, test_size)
 
         self._make_train_val_dir()
 
         # convert labelme object to yolo format object, and save them to files
         # also get image from labelme json file and save them under images folder
         for target_dir, json_names in zip(('train/', 'val/', 'test/'),
-                                          (train_json_names, val_json_names, test_json_names)):
+                                          (train_json_names, val_json_names, test_json_names)):  # noqa: E501
             pool = Pool(NUM_THREADS)
 
             for json_name in json_names:
                 pool.apply_async(self.covert_json_to_text,
                                  args=(target_dir, json_name))
             pool.close()
             pool.join()
```

### Comparing `labelme2yolo-0.1.1/src/labelme2yolo/cli/__init__.py` & `labelme2yolo-0.1.2/src/labelme2yolo/cli/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # SPDX-FileCopyrightText: 2022-present Wang Xin <xinwang614@gmail.com>
 #
 # SPDX-License-Identifier: MIT
+"""
+cli init
+"""
 import argparse
 
 from labelme2yolo.l2y import Labelme2YOLO
 
 
 def run():
+    '''
+    run cli
+    '''
     parser = argparse.ArgumentParser("labelme2yolo")
     parser.add_argument(
         "--json_dir", type=str, help="Please input the path of the labelme json files."
     )
     parser.add_argument(
         "--val_size",
         type=float,
```

### Comparing `labelme2yolo-0.1.1/.gitignore` & `labelme2yolo-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `labelme2yolo-0.1.1/LICENSE` & `labelme2yolo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `labelme2yolo-0.1.1/README.md` & `labelme2yolo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `labelme2yolo-0.1.1/pyproject.toml` & `labelme2yolo-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labelme2yolo-0.1.1/PKG-INFO` & `labelme2yolo-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelme2yolo
-Version: 0.1.1
+Version: 0.1.2
 Summary: This script converts the JSON format output by LabelMe to the text format required by YOLO serirs.
 Project-URL: Documentation, https://github.com/greatv/labelme2yolo#readme
 Project-URL: Issues, https://github.com/greatv/labelme2yolo/issues
 Project-URL: Source, https://github.com/greatv/labelme2yolo
 Author-email: "GreatV(Wang Xin)" <xinwang614@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

