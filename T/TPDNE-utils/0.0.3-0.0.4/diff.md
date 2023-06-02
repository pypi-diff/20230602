# Comparing `tmp/TPDNE-utils-0.0.3.tar.gz` & `tmp/TPDNE-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPDNE-utils-0.0.3.tar", last modified: Fri Jun  2 19:49:31 2023, max compression
+gzip compressed data, was "TPDNE-utils-0.0.4.tar", last modified: Fri Jun  2 19:51:31 2023, max compression
```

## Comparing `TPDNE-utils-0.0.3.tar` & `TPDNE-utils-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:49:31.630852 TPDNE-utils-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-02 19:49:19.000000 TPDNE-utils-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-02 19:49:31.630852 TPDNE-utils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-02 19:49:19.000000 TPDNE-utils-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:49:31.630852 TPDNE-utils-0.0.3/TPDNE_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 19:49:19.000000 TPDNE-utils-0.0.3/TPDNE_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-02 19:49:19.000000 TPDNE-utils-0.0.3/TPDNE_utils/tpdne.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:49:31.630852 TPDNE-utils-0.0.3/TPDNE_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-02 19:49:31.000000 TPDNE-utils-0.0.3/TPDNE_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-02 19:49:31.000000 TPDNE-utils-0.0.3/TPDNE_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:49:31.000000 TPDNE-utils-0.0.3/TPDNE_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 19:49:31.000000 TPDNE-utils-0.0.3/TPDNE_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 19:49:31.000000 TPDNE-utils-0.0.3/TPDNE_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 19:49:31.630852 TPDNE-utils-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-02 19:49:19.000000 TPDNE-utils-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:51:31.633036 TPDNE-utils-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-02 19:51:22.000000 TPDNE-utils-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-02 19:51:31.633036 TPDNE-utils-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-02 19:51:22.000000 TPDNE-utils-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:51:31.629036 TPDNE-utils-0.0.4/TPDNE_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 19:51:22.000000 TPDNE-utils-0.0.4/TPDNE_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-02 19:51:22.000000 TPDNE-utils-0.0.4/TPDNE_utils/tpdne.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:51:31.633036 TPDNE-utils-0.0.4/TPDNE_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-02 19:51:31.000000 TPDNE-utils-0.0.4/TPDNE_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-02 19:51:31.000000 TPDNE-utils-0.0.4/TPDNE_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:51:31.000000 TPDNE-utils-0.0.4/TPDNE_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 19:51:31.000000 TPDNE-utils-0.0.4/TPDNE_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 19:51:31.000000 TPDNE-utils-0.0.4/TPDNE_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 19:51:31.633036 TPDNE-utils-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-02 19:51:22.000000 TPDNE-utils-0.0.4/setup.py
```

### Comparing `TPDNE-utils-0.0.3/LICENSE` & `TPDNE-utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TPDNE-utils-0.0.3/README.md` & `TPDNE-utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `TPDNE-utils-0.0.3/TPDNE_utils/tpdne.py` & `TPDNE-utils-0.0.4/TPDNE_utils/tpdne.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 import numpy as np
 from time import time, sleep
 from pathlib import Path
 from functools import wraps
 from PIL import Image
 
 from beartype import beartype
-from beartype.typing import Callable
+from beartype.typing import Callable, Optional
+
+def exists(val):
+    return val is not None
 
 @beartype
 def sample_image_and_save_repeatedly(
     fn: Callable[..., np.ndarray],         # function that returns a ndarray of shape (3, <width>, <height>)
     output_path: str = './out/random',     # path to the output image, without extension (will be saved as webp)
     *,
     call_every_ms: int = 250,              # how often to sample
     tmp_dir: str = '/tmp',                 # to store temporary images, before symbolically linking to the output path
     num_rotated_tmp_images: int = 10,
     image_format: str = 'webp',
     verbose: bool = True,
     quality = 99,
+    resize_image_to: Optional[int] = None,
     generate_favicon: bool = True,
     favicon_size: int = 32
 ):
     assert 0 < quality <= 100
     assert favicon_size in {16, 32}
     assert image_format in {'webp', 'png', 'jpeg'}
 
@@ -43,14 +47,18 @@
         start = time()
         image_tensor = fn()
 
         tmp_image_index = (tmp_image_index + 1) % num_rotated_tmp_images
         tmp_path = str(tmp_dir / f'{tmp_image_index}.{image_format}')
 
         pil_image = Image.fromarray(image_tensor, 'RGB')
+
+        if exists(resize_image_to):
+            pil_image = pil_image.resize((resize_image_to, resize_image_to))
+
         pil_image.save(tmp_path, format = image_format, quality = quality)
         os.system(f'ln -nfs {tmp_path} {output_path}')
 
         if generate_favicon:
             tmp_favicon_path = str(tmp_dir / f'favicon_{tmp_image_index}.png')
             output_favicon_path = output_path.parents[0] / 'favicon.png'
```

### Comparing `TPDNE-utils-0.0.3/setup.py` & `TPDNE-utils-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'TPDNE-utils',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'TPDNE',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/TPDNE',
   keywords = [],
```

