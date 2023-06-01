# Comparing `tmp/mecsimcalc-0.1.2.tar.gz` & `tmp/mecsimcalc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecsimcalc-0.1.2.tar", last modified: Wed May 31 23:17:17 2023, max compression
+gzip compressed data, was "mecsimcalc-0.1.3.tar", last modified: Thu Jun  1 23:43:10 2023, max compression
```

## Comparing `mecsimcalc-0.1.2.tar` & `mecsimcalc-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:17:17.191629 mecsimcalc-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-31 23:17:17.191629 mecsimcalc-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22654 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:17:17.191629 mecsimcalc-0.1.2/mecsimcalc/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/mecsimcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/mecsimcalc/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/mecsimcalc/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/mecsimcalc/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/mecsimcalc/spreadsheet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/mecsimcalc/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/mecsimcalc/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:17:17.191629 mecsimcalc-0.1.2/mecsimcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-31 23:17:17.000000 mecsimcalc-0.1.2/mecsimcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-31 23:17:17.000000 mecsimcalc-0.1.2/mecsimcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:17:17.000000 mecsimcalc-0.1.2/mecsimcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 23:17:17.000000 mecsimcalc-0.1.2/mecsimcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 23:17:17.000000 mecsimcalc-0.1.2/mecsimcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:17:17.191629 mecsimcalc-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-31 23:17:04.000000 mecsimcalc-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:10.654651 mecsimcalc-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23493 2023-06-01 23:43:10.654651 mecsimcalc-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22679 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:10.650651 mecsimcalc-0.1.3/mecsimcalc/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/mecsimcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/mecsimcalc/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/mecsimcalc/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/mecsimcalc/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/mecsimcalc/spreadsheet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/mecsimcalc/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/mecsimcalc/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:10.654651 mecsimcalc-0.1.3/mecsimcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23493 2023-06-01 23:43:10.000000 mecsimcalc-0.1.3/mecsimcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 23:43:10.000000 mecsimcalc-0.1.3/mecsimcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:43:10.000000 mecsimcalc-0.1.3/mecsimcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 23:43:10.000000 mecsimcalc-0.1.3/mecsimcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 23:43:10.000000 mecsimcalc-0.1.3/mecsimcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:43:10.654651 mecsimcalc-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-01 23:42:59.000000 mecsimcalc-0.1.3/setup.py
```

### Comparing `mecsimcalc-0.1.2/LICENSE` & `mecsimcalc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.2/PKG-INFO` & `mecsimcalc-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecsimcalc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Useful functions for MecSimCalc.com
 Author: MecSimCalc
 Author-email: <info@mecsimcalc.com>
 Keywords: python,MecSimCalc,Calculator,Simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Mecsimcalc v0.1.2 documentation
+# Mecsimcalc v0.1.3 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
@@ -482,29 +482,29 @@
 | **`PIL.Image.Image`**             | Pillow Image object      | get_file_type is False |
 | **`Tuple[PIL.Image.Image, str]`** | (pillow image, metadata) | get_file_type is True  |
 
 #### Example:
 
 ```python
 >>> input_file = inputs['file']
->>> img, file_type = input_to_PIL(input_file, get_file_type=True)
+>>> image, file_type = input_to_PIL(input_file, get_file_type=True)
 >>> print(file_type)
 jpeg
->>> type(img)
+>>> type(image)
 <class 'PIL.JpegImagePlugin.JpegImageFile'>
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">print_img</h3>
+  <h3 style="margin: 5px; padding: 0;">print_image</h3>
   <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL60C1-L126C32" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def print_img(
-    img,
+def print_image(
+    image,
     width = 200,
     height = 200,
     original_size = False,
     download = False,
     download_text = "Download Image",
     download_file_name= "myimg",
     download_file_type = "png",
@@ -515,15 +515,15 @@
 
 Transforms a Pillow image into an HTML image, with an optional download link
 
 #### Arguments:
 
 | Argument                 | Type                | Description                                                                        |
 | ------------------------ | ------------------- | ---------------------------------------------------------------------------------- |
-| **`img`**                | **PIL.Image.Image** | Pillow image                                                                       |
+| **`image`**              | **PIL.Image.Image** | Pillow image                                                                       |
 | **`width`**              | **int** (optional)  | Output width of the image in pixels (Defaults to 200)                              |
 | **`height`**             | **int** (optional)  | Output height of the image in pixels (Defaults to 200)                             |
 | **`original_size`**      | **bool** (optional) | If True, the HTML image will be displayed in its original size (Defaults to False) |
 | **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)                      |
 | **`download_text`**      | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Image")       |
 | **`download_file_name`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myimg")                   |
 | **`download_file_type`** | **str** (optional)  | The file type of the image when downloaded (Defaults to "png")                     |
@@ -537,18 +537,18 @@
 
 #### Example:
 
 #### Python Code:
 
 ```python
 >>> input_file = inputs['file']
->>> img, metadata = input_to_PIL(input_file)
->>> image, download = print_img(img,, original_size = True, download = True, download_text = "Download Image Here", download_file_name = "myimage", download_file_type = "jpeg")
+>>> image, metadata = input_to_PIL(input_file)
+>>> html_image, download = print_image(image, original_size = True, download = True, download_text = "Download Image Here", download_file_name = "myimage", download_file_type = "jpeg")
 >>> return {
-        "image":image,
+        "image":html_image,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
 
 ```python
```

### Comparing `mecsimcalc-0.1.2/README.md` & `mecsimcalc-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Mecsimcalc v0.1.2 documentation
+# Mecsimcalc v0.1.3 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
@@ -459,29 +459,29 @@
 | **`PIL.Image.Image`**             | Pillow Image object      | get_file_type is False |
 | **`Tuple[PIL.Image.Image, str]`** | (pillow image, metadata) | get_file_type is True  |
 
 #### Example:
 
 ```python
 >>> input_file = inputs['file']
->>> img, file_type = input_to_PIL(input_file, get_file_type=True)
+>>> image, file_type = input_to_PIL(input_file, get_file_type=True)
 >>> print(file_type)
 jpeg
->>> type(img)
+>>> type(image)
 <class 'PIL.JpegImagePlugin.JpegImageFile'>
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">print_img</h3>
+  <h3 style="margin: 5px; padding: 0;">print_image</h3>
   <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL60C1-L126C32" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def print_img(
-    img,
+def print_image(
+    image,
     width = 200,
     height = 200,
     original_size = False,
     download = False,
     download_text = "Download Image",
     download_file_name= "myimg",
     download_file_type = "png",
@@ -492,15 +492,15 @@
 
 Transforms a Pillow image into an HTML image, with an optional download link
 
 #### Arguments:
 
 | Argument                 | Type                | Description                                                                        |
 | ------------------------ | ------------------- | ---------------------------------------------------------------------------------- |
-| **`img`**                | **PIL.Image.Image** | Pillow image                                                                       |
+| **`image`**              | **PIL.Image.Image** | Pillow image                                                                       |
 | **`width`**              | **int** (optional)  | Output width of the image in pixels (Defaults to 200)                              |
 | **`height`**             | **int** (optional)  | Output height of the image in pixels (Defaults to 200)                             |
 | **`original_size`**      | **bool** (optional) | If True, the HTML image will be displayed in its original size (Defaults to False) |
 | **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)                      |
 | **`download_text`**      | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Image")       |
 | **`download_file_name`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myimg")                   |
 | **`download_file_type`** | **str** (optional)  | The file type of the image when downloaded (Defaults to "png")                     |
@@ -514,18 +514,18 @@
 
 #### Example:
 
 #### Python Code:
 
 ```python
 >>> input_file = inputs['file']
->>> img, metadata = input_to_PIL(input_file)
->>> image, download = print_img(img,, original_size = True, download = True, download_text = "Download Image Here", download_file_name = "myimage", download_file_type = "jpeg")
+>>> image, metadata = input_to_PIL(input_file)
+>>> html_image, download = print_image(image, original_size = True, download = True, download_text = "Download Image Here", download_file_name = "myimage", download_file_type = "jpeg")
 >>> return {
-        "image":image,
+        "image":html_image,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
 
 ```python
```

### Comparing `mecsimcalc-0.1.2/mecsimcalc/general_utils.py` & `mecsimcalc-0.1.3/mecsimcalc/general_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.2/mecsimcalc/image_utils.py` & `mecsimcalc-0.1.3/mecsimcalc/image_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from PIL import Image
 
 from mecsimcalc import input_to_file, metadata_to_filetype
 
 # Define a dictionary for file type conversions
 file_type_mappings = {"jpg": "jpeg", "tif": "tiff", "ico": "x-icon", "svg": "svg+xml", "jpeg": "jpeg", "tiff": "tiff", "x-icon": "x-icon", "svg+xml": "svg+xml"}
 
-
 def file_to_PIL(file: io.BytesIO) -> Image.Image:
     """
     Transforms a file into a Pillow Image object.
 
     Args:
         file (io.BytesIO): A file object containing image data (using open with 'rb' mode)
 
@@ -44,83 +43,83 @@
         Union[PIL.Image.Image, Tuple[PIL.Image.Image, str]]: If get_file_type is False, a Pillow image object is returned.
                                                              If get_file_type is True, a tuple containing the Pillow image object and the file type is returned.
     """
     # Decode the base64 string into a file-like object and extract metadata
     file_data, metadata = input_to_file(input_file, metadata=True)
 
     # Load the file data into a Pillow Image
-    img = file_to_PIL(file_data)
+    image = file_to_PIL(file_data)
 
     if get_file_type:
         file_type = metadata_to_filetype(metadata)
-        return img, file_type
+        return image, file_type
 
-    return img
+    return image
 
 
-def print_img(
-    img: Image.Image,
+def print_image(
+    image: Image.Image,
     width: int = 200,
     height: int = 200,
     original_size: bool = False,
     download: bool = False,
     download_text: str = "Download Image",
     download_file_name: str = "myimg",
     download_file_type: str = "png",
 ) -> Union[str, Tuple[str, str]]:
     """
     Transforms a Pillow image into an HTML image, with an optional download link.
 
     Args:
-        img (PIL.Image.Image): A Pillow image object.
+        image (PIL.Image.Image): A Pillow image object.
         width (int, optional): The width for the displayed image, in pixels. (Defaults to 200)
         height (int, optional): The height for the displayed image, in pixels. (Defaults to 200)
         original_size (bool, optional): If True, the image will retain its original size. (Defaults to False)
         download (bool, optional): If True, a download link will be provided. (Defaults to False)
         download_text (str, optional): The text for the download link. (Defaults to "Download Image")
         download_file_name (str, optional): The name for the downloaded file. (Defaults to 'myimg')
         download_file_type (str, optional): The file type for the downloaded file. (Defaults to "png")
 
     Returns:
         Union[str, Tuple[str, str]]: If download is False, an HTML string containing the image is returned.
-                                      If download is True, a tuple containing the HTML string for the image and the download link is returned.
+                                     If download is True, a tuple containing the HTML string for the image and the download link is returned.
     """
     # Create a copy for display, preserving the original image
-    display_img = img.copy()
+    display_image = image.copy()
 
     # Correct file type using the mappings dictionary
     file_type = file_type_mappings.get(
         download_file_type.lower().replace(".", ""), "png"
     )
 
     # Create metadata with correct file type
     metadata = f"data:image/{file_type};base64,"
 
     if not original_size:
-        display_img.thumbnail((width, height))
+        display_image.thumbnail((width, height))
 
     # Get downloadable data (Full Resolution)
     buffer = io.BytesIO()
-    img.save(buffer, format=img.format)
+    image.save(buffer, format=image.format)
     encoded_data = metadata + base64.b64encode(buffer.getvalue()).decode()
 
     # Get displayable data (Custom Resolution)
     display_buffer = io.BytesIO()
 
     # Save the display image to the buffer
-    display_img.save(display_buffer, format=img.format)
+    display_image.save(display_buffer, format=image.format)
 
     # Get the encoded display data
     encoded_display_data = (
         metadata + base64.b64encode(display_buffer.getvalue()).decode()
     )
 
     # Convert Display image to HTML
     image = f"<img src='{encoded_display_data}'>"
 
     if not download:
         return image
 
     # Convert full resolution image to an HTML download link
-    download_link = f"<a href='{encoded_data}' download='{download_file_name}.{img.format}'>{download_text}</a>"
+    download_link = f"<a href='{encoded_data}' download='{download_file_name}.{image.format}'>{download_text}</a>"
 
     return image, download_link
```

### Comparing `mecsimcalc-0.1.2/mecsimcalc/plotting_utils.py` & `mecsimcalc-0.1.3/mecsimcalc/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.2/mecsimcalc/spreadsheet_utils.py` & `mecsimcalc-0.1.3/mecsimcalc/spreadsheet_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.2/mecsimcalc/table_utils.py` & `mecsimcalc-0.1.3/mecsimcalc/table_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.2/mecsimcalc/text_utils.py` & `mecsimcalc-0.1.3/mecsimcalc/text_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.1.2/mecsimcalc.egg-info/PKG-INFO` & `mecsimcalc-0.1.3/mecsimcalc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecsimcalc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Useful functions for MecSimCalc.com
 Author: MecSimCalc
 Author-email: <info@mecsimcalc.com>
 Keywords: python,MecSimCalc,Calculator,Simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Mecsimcalc v0.1.2 documentation
+# Mecsimcalc v0.1.3 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
@@ -482,29 +482,29 @@
 | **`PIL.Image.Image`**             | Pillow Image object      | get_file_type is False |
 | **`Tuple[PIL.Image.Image, str]`** | (pillow image, metadata) | get_file_type is True  |
 
 #### Example:
 
 ```python
 >>> input_file = inputs['file']
->>> img, file_type = input_to_PIL(input_file, get_file_type=True)
+>>> image, file_type = input_to_PIL(input_file, get_file_type=True)
 >>> print(file_type)
 jpeg
->>> type(img)
+>>> type(image)
 <class 'PIL.JpegImagePlugin.JpegImageFile'>
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">print_img</h3>
+  <h3 style="margin: 5px; padding: 0;">print_image</h3>
   <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL60C1-L126C32" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def print_img(
-    img,
+def print_image(
+    image,
     width = 200,
     height = 200,
     original_size = False,
     download = False,
     download_text = "Download Image",
     download_file_name= "myimg",
     download_file_type = "png",
@@ -515,15 +515,15 @@
 
 Transforms a Pillow image into an HTML image, with an optional download link
 
 #### Arguments:
 
 | Argument                 | Type                | Description                                                                        |
 | ------------------------ | ------------------- | ---------------------------------------------------------------------------------- |
-| **`img`**                | **PIL.Image.Image** | Pillow image                                                                       |
+| **`image`**              | **PIL.Image.Image** | Pillow image                                                                       |
 | **`width`**              | **int** (optional)  | Output width of the image in pixels (Defaults to 200)                              |
 | **`height`**             | **int** (optional)  | Output height of the image in pixels (Defaults to 200)                             |
 | **`original_size`**      | **bool** (optional) | If True, the HTML image will be displayed in its original size (Defaults to False) |
 | **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)                      |
 | **`download_text`**      | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Image")       |
 | **`download_file_name`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myimg")                   |
 | **`download_file_type`** | **str** (optional)  | The file type of the image when downloaded (Defaults to "png")                     |
@@ -537,18 +537,18 @@
 
 #### Example:
 
 #### Python Code:
 
 ```python
 >>> input_file = inputs['file']
->>> img, metadata = input_to_PIL(input_file)
->>> image, download = print_img(img,, original_size = True, download = True, download_text = "Download Image Here", download_file_name = "myimage", download_file_type = "jpeg")
+>>> image, metadata = input_to_PIL(input_file)
+>>> html_image, download = print_image(image, original_size = True, download = True, download_text = "Download Image Here", download_file_name = "myimage", download_file_type = "jpeg")
 >>> return {
-        "image":image,
+        "image":html_image,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
 
 ```python
```

### Comparing `mecsimcalc-0.1.2/setup.py` & `mecsimcalc-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 DESCRIPTION = "Useful functions for MecSimCalc.com"
 
 # Setting up
 setup(
     name="mecsimcalc",
     version=VERSION,
     author="MecSimCalc",
```

