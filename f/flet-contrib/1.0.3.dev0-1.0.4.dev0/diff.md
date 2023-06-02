# Comparing `tmp/flet_contrib-1.0.3.dev0.tar.gz` & `tmp/flet_contrib-1.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib-1.0.3.dev0.tar", max compression
+gzip compressed data, was "flet_contrib-1.0.4.dev0.tar", max compression
```

## Comparing `flet_contrib-1.0.3.dev0.tar` & `flet_contrib-1.0.4.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/LICENSE
--rw-r--r--   0        0        0      396 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/README.md
--rw-r--r--   0        0        0     1643 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/README.md
--rw-r--r--   0        0        0      215 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/__init__.py
--rw-r--r--   0        0        0      859 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/examples/color_picker_dialog.py
--rw-r--r--   0        0        0      538 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/examples/hue_slider_example.py
--rw-r--r--   0        0        0      416 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/examples/update_color_property.py
--rw-r--r--   0        0        0   128246 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/media/color_picker.png
--rw-r--r--   0        0        0     7249 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/src/color_picker.py
--rw-r--r--   0        0        0     2644 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/src/hue_slider.py
--rw-r--r--   0        0        0     4709 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/src/palette_color_picker.py
--rw-r--r--   0        0        0      464 2023-06-02 18:37:04.473387 flet_contrib-1.0.3.dev0/flet_contrib/color_picker/src/utils.py
--rw-r--r--   0        0        0      444 2023-06-02 18:37:30.393189 flet_contrib-1.0.3.dev0/pyproject.toml
--rw-r--r--   0        0        0     1046 1970-01-01 00:00:00.000000 flet_contrib-1.0.3.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/LICENSE
+-rw-r--r--   0        0        0      396 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/README.md
+-rw-r--r--   0        0        0     1642 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/README.md
+-rw-r--r--   0        0        0      215 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/__init__.py
+-rw-r--r--   0        0        0      859 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/examples/color_picker_dialog.py
+-rw-r--r--   0        0        0      538 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/examples/hue_slider_example.py
+-rw-r--r--   0        0        0      416 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/examples/update_color_property.py
+-rw-r--r--   0        0        0   128246 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/media/color_picker.png
+-rw-r--r--   0        0        0     7249 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/src/color_picker.py
+-rw-r--r--   0        0        0     2644 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/src/hue_slider.py
+-rw-r--r--   0        0        0     4709 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/src/palette_color_picker.py
+-rw-r--r--   0        0        0      464 2023-06-02 19:26:44.596231 flet_contrib-1.0.4.dev0/flet_contrib/color_picker/src/utils.py
+-rw-r--r--   0        0        0      444 2023-06-02 19:27:12.249205 flet_contrib-1.0.4.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1046 1970-01-01 00:00:00.000000 flet_contrib-1.0.4.dev0/PKG-INFO
```

### Comparing `flet_contrib-1.0.3.dev0/LICENSE` & `flet_contrib-1.0.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_contrib-1.0.3.dev0/flet_contrib/color_picker/README.md` & `flet_contrib-1.0.4.dev0/flet_contrib/color_picker/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 `ColorPicker` control is used for picking a color from color map in hex (rgb) format.
 
 `ColorPicker` inherits from [`Column`](https://flet.dev/docs/controls/column) and can be used as a content for [`AlertDialog`](https://flet.dev/docs/controls/alertdialog) or other control or placed directly on a page.
 
 ## Examples
 
-[Live example](https://flet-controls-gallery.fly.dev/contribs/colorpicker)
+[Live example](https://flet-controls-gallery.fly.dev/contrib/colorpicker)
 
 ### ColorPicker dialog
 
 <img src="media/color_picker.png" width="50%"/>
 
 ```python
 import flet as ft
```

### Comparing `flet_contrib-1.0.3.dev0/flet_contrib/color_picker/examples/color_picker_dialog.py` & `flet_contrib-1.0.4.dev0/flet_contrib/color_picker/examples/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-1.0.3.dev0/flet_contrib/color_picker/examples/hue_slider_example.py` & `flet_contrib-1.0.4.dev0/flet_contrib/color_picker/examples/hue_slider_example.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-1.0.3.dev0/flet_contrib/color_picker/media/color_picker.png` & `flet_contrib-1.0.4.dev0/flet_contrib/color_picker/media/color_picker.png`

 * *Files identical despite different names*

### Comparing `flet_contrib-1.0.3.dev0/flet_contrib/color_picker/src/color_picker.py` & `flet_contrib-1.0.4.dev0/flet_contrib/color_picker/src/color_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-1.0.3.dev0/flet_contrib/color_picker/src/hue_slider.py` & `flet_contrib-1.0.4.dev0/flet_contrib/color_picker/src/hue_slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-1.0.3.dev0/flet_contrib/color_picker/src/palette_color_picker.py` & `flet_contrib-1.0.4.dev0/flet_contrib/color_picker/src/palette_color_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-1.0.3.dev0/PKG-INFO` & `flet_contrib-1.0.4.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-contrib
-Version: 1.0.3.dev0
+Version: 1.0.4.dev0
 Summary: Flet controls by the community
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

