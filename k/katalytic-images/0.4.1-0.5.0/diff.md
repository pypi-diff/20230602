# Comparing `tmp/katalytic_images-0.4.1.tar.gz` & `tmp/katalytic_images-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic_images-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "katalytic_images-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic_images-0.4.1.tar` & `katalytic_images-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.4.1/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.4.1/.gitignore
--rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.4.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     2716 2023-05-31 06:43:54.787954 katalytic_images-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.4.1/README.md
--rw-r--r--   0        0        0     1549 2023-05-31 06:43:54.787954 katalytic_images-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    21782 2023-05-31 06:26:00.533837 katalytic_images-0.4.1/src/katalytic/images.py
--rw-r--r--   0        0        0    15603 2023-05-31 06:18:31.089140 katalytic_images-0.4.1/tests/test_images.py
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.5.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.5.0/.gitignore
+-rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2970 2023-06-02 05:42:41.662349 katalytic_images-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.5.0/README.md
+-rw-r--r--   0        0        0     1549 2023-06-02 05:42:41.662349 katalytic_images-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    22846 2023-06-02 05:33:42.682090 katalytic_images-0.5.0/src/katalytic/images.py
+-rw-r--r--   0        0        0    16369 2023-06-02 05:38:26.405653 katalytic_images-0.5.0/tests/test_images.py
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.5.0/PKG-INFO
```

### Comparing `katalytic_images-0.4.1/.gitignore` & `katalytic_images-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.4.1/.gitlab-ci.yml` & `katalytic_images-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.4.1/CHANGELOG.md` & `katalytic_images-0.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.5.0 (2023-06-02)
+### feat
+- [[`37afcb5`](https://gitlab.com/katalytic/katalytic-images/commit/37afcb5e74c8f6b081b8261136a873c291358cdd)] load_image(..., *, default=_UNDEFINED) and save_image(..., exists='replace', make_dirs=True, mode='RGB', ...)
+
+
 ## 0.4.1 (2023-05-31)
 ### fix
 - [[`dc2fff6`](https://gitlab.com/katalytic/katalytic-images/commit/dc2fff66953ee47de40d78702ab6b55079800969)] ValueError -> TypeError
 - [[`44c3801`](https://gitlab.com/katalytic/katalytic-images/commit/44c38013096021262cdb3c5e8da0ff50972468cb)] convert types to what opencv expects
 - [[`c6fe7fa`](https://gitlab.com/katalytic/katalytic-images/commit/c6fe7fae2868c1340929704ba20cbcd303647aa1)] readme
 - [[`ecaef54`](https://gitlab.com/katalytic/katalytic-images/commit/ecaef54965aaaec043b8fd170a5d82c15071a8df)] remove unnecessary function and convert circle radius to int
```

### Comparing `katalytic_images-0.4.1/LICENSE.txt` & `katalytic_images-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.4.1/README.md` & `katalytic_images-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.4.1/pyproject.toml` & `katalytic_images-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.4.1"
+version = "0.5.0"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic_images-0.4.1/src/katalytic/images.py` & `katalytic_images-0.5.0/src/katalytic/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
     ndarray as __np_ndarray
 )
 
 import PIL.Image
 __PIL_Image_open = PIL.Image.open
 __PIL_Image_Image = PIL.Image.Image
 
+from katalytic.files import copy_file
+from katalytic.files import make_dir
 from katalytic.data.checks import is_iterable, is_number, is_sequence
+from katalytic.data import _UNDEFINED
 from katalytic.pkg import get_version, mark
 
 __version__, __version_info__ = get_version(__name__)
 
 
 def bhwc(arr):
     """
@@ -435,35 +438,40 @@
     else:
         return fn[shape_type]
 
 
 @mark('load::png')
 @mark('load::jpg')
 @mark('load::jpeg')
-def load_image(image, mode=None):
+def load_image(image, mode=None, *, default=_UNDEFINED):
     """
     Load an image and return it as a NumPy array.
 
     Parameters:
         image: The image to be loaded. It can be specified as a file path (string or Path object), a PIL Image object, or a NumPy array.
         mode (str, optional): The mode to be used when loading the image. It should be a string representing the desired mode, e.g., 'RGB', 'L', 'RGBA'. If None, the default mode of the image will be used.
+        default (Any):
+            The default value to return if the specified file path does not exist.
 
     Returns:
         numpy.ndarray: The loaded image as a NumPy array.
 
     Raises:
         TypeError: If the 'mode' parameter is not None or a string.
         TypeError: If the 'image' parameter has an unsupported type.
 
     """
     if not(mode is None or isinstance(mode, str)):
         raise TypeError(f'mode expected None or str. Got {type(mode)!r}')
 
     if isinstance(image, (str, Path)):
-        return __np_array(__PIL_Image_open(image))
+        if not Path(image).exists() and default is not _UNDEFINED:
+            return default
+        else:
+            return __np_array(__PIL_Image_open(image))
     elif isinstance(image, __PIL_Image_Image):
         return __np_array(image)
     elif isinstance(image, __np_ndarray):
         return image.copy()
     else:
         raise TypeError(f'type(image) = {type(image)!r}')
 
@@ -526,24 +534,34 @@
     else:
         return (image_1 == image_2).all()
 
 
 @mark('save::png')
 @mark('save::jpg')
 @mark('save::jpeg')
-def save_image(image, path, *, exists='error', mode='RGB'):
+def save_image(image, path, *, exists='replace', make_dirs=True, mode='RGB'):
     """
     Save an image to the specified file path.
     The image can be provided as a PIL Image object, a NumPy array, or a file path.
     The function supports specifying the behavior when the target file already exists.
 
     Parameters:
         image: The image to be saved. It can be specified as a PIL Image object, a NumPy array, or a file path (string or Path object).
         path: The file path to save the image to. It should be a string or Path object.
-        exists (str, optional): The behavior when the target file already exists. It can be one of the following options: 'error' to raise an error, 'skip' to skip saving the image, or 'replace' to replace the existing file. Defaults to 'error'.
+        exists (str, optional):
+            Specifies the behavior if the destination file already exists. Defaults to 'replace'.
+
+            - 'error': Raise an error.
+            - 'replace': Replace the existing file.
+            - 'skip': Skip copying the file.
+        make_dirs (bool or str, optional):
+            Specifies whether to create the destination directory if it doesn't exist. Defaults to True.
+
+            - True: Create the directory if it doesn't exist.
+            - False: Raise an error if the destination directory doesn't exist.
         mode (str, optional): The mode to be used when saving the image. It should be a string representing the desired mode, e.g., 'RGB', 'BGR'. Defaults to 'RGB'.
 
     Raises:
         TypeError: If the 'mode' parameter is not a string.
         ValueError: If the 'exists' parameter is not one of 'error', 'skip', 'replace'.
         FileExistsError: If the target file already exists and the 'exists' parameter is set to 'error'.
 
@@ -552,23 +570,32 @@
         raise TypeError(f'type(mode) = {type(mode)!r}')
     elif exists not in ('error', 'skip', 'replace'):
         raise ValueError(f'exists must be one of \'error\', \'skip\', \'replace\'. Got {exists!r}')
 
     if Path(path).exists():
         if exists == 'error':
             raise FileExistsError(f'[Errno 17] File exists: {str(path)!r}')
+        elif exists == 'replace':
+            pass  # continue executing
         elif exists == 'skip':
             return
 
+    dest_dir = Path(path).parent
+    if make_dirs:
+        make_dir(dest_dir, create_parents=True, exists_ok=True)
+    elif not dest_dir.exists():
+        raise FileNotFoundError(f'[Errno 2] Directory does not exist: {str(dest_dir)!r}')
+    elif not dest_dir.is_dir():
+        raise NotADirectoryError(f'[Errno 20] Not a directory: {str(dest_dir)!r}')
+
     if isinstance(image, __PIL_Image_Image):
         image = __np_array(image)
 
     if isinstance(image, __np_ndarray):
         if mode != 'BGR':
             image = convert_image(image, mode, 'BGR')
 
         __cv2_imwrite(str(path), image)
     elif isinstance(image, (str, Path)):
-        from katalytic.files import copy_file
         copy_file(image, path, exists=exists)
     else:
         raise TypeError(f'type(image) = {type(image)!r}')
```

### Comparing `katalytic_images-0.4.1/tests/test_images.py` & `katalytic_images-0.5.0/tests/test_images.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import cv2
 import numpy as np
 import PIL.Image
 import pytest
 from PIL import Image
 
 from katalytic.data import all_types_besides
-from katalytic.files import get_unique_path, load, save
+from katalytic.files import get_unique_path, load, move_file, save
 from katalytic.images import bhwc, convert_image, create_circle, create_line, create_mask, create_polylines, create_rectangle, create_text, draw, hw, hwc, are_arrays_equal, load_image, save_image
 
 
 def _create_RGB(dtype=np.uint8):
     return np.array([
         [[255, 0, 0], [0, 255, 0], [0, 0, 255]],        # RGB
         [[0, 255, 255], [255, 0, 255], [255, 255, 0]],  # CMY
@@ -378,14 +378,34 @@
 
     def test_universal_load_and_save(self):
         path = get_unique_path('{}.png')
         img = _create_RGB()
         save(img, path)
         assert are_arrays_equal(load(path), img)
 
+    def test_default(self):
+        path = get_unique_path('{}.png')
+        img = load_image(path, default=_create_RGB())
+        assert are_arrays_equal(img, _create_RGB())
+
+    def test_make_dirs_False(self):
+        img = _create_RGB()
+        path = get_unique_path('{}/data.csv')
+        with pytest.raises(FileNotFoundError):
+            save_image(img, path, make_dirs=False)
+
+        # save image, then move it to a filename without extension
+        path = get_unique_path('{}/data')
+        save_image(img, f'{path}.png', make_dirs=True)
+        move_file(f'{path}.png', path)
+
+        # then try to use that filename as a directory
+        with pytest.raises(NotADirectoryError):
+            save_image(img, f'{path}/x.csv', make_dirs=False)
+
     @pytest.mark.parametrize('img', [1, True, None, [], {}, (), object()])
     def test_load_raises_TypeError_for_image(self, img):
         with pytest.raises(TypeError):
             load_image(img)
 
     @pytest.mark.parametrize('mode', [1, True, [], {}, (), object()])
     def test_load_raises_TypeError_for_mode(self, mode):
```

### Comparing `katalytic_images-0.4.1/PKG-INFO` & `katalytic_images-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.4.1
+Version: 0.5.0
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

