# Comparing `tmp/mzarr-0.0.5.tar.gz` & `tmp/mzarr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzarr-0.0.5.tar", last modified: Fri Jun  2 09:07:46 2023, max compression
+gzip compressed data, was "mzarr-0.0.6.tar", last modified: Fri Jun  2 09:21:28 2023, max compression
```

## Comparing `mzarr-0.0.5.tar` & `mzarr-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:46.961016 mzarr-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 09:07:24.000000 mzarr-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 09:07:24.000000 mzarr-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 09:07:46.961016 mzarr-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-02 09:07:24.000000 mzarr-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:46.961016 mzarr-0.0.5/mzarr/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:46.961016 mzarr-0.0.5/mzarr/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/nifti2mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/tiff2mzarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:46.961016 mzarr-0.0.5/mzarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 09:07:24.000000 mzarr-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-02 09:07:46.965016 mzarr-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:28.849953 mzarr-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 09:21:08.000000 mzarr-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 09:21:08.000000 mzarr-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 09:21:28.849953 mzarr-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-02 09:21:08.000000 mzarr-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:28.845953 mzarr-0.0.6/mzarr/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:28.849953 mzarr-0.0.6/mzarr/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/nifti2mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/tiff2mzarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:28.849953 mzarr-0.0.6/mzarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 09:21:08.000000 mzarr-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-02 09:21:28.849953 mzarr-0.0.6/setup.cfg
```

### Comparing `mzarr-0.0.5/LICENSE` & `mzarr-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.5/PKG-INFO` & `mzarr-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzarr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mzarr-0.0.5/README.md` & `mzarr-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.5/mzarr/mzarr.py` & `mzarr-0.0.6/mzarr/mzarr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import numpy as np
 import zarr
 from zarr.util import guess_chunks, normalize_dtype
 from skimage.transform import pyramid_gaussian
 from imagecodecs.numcodecs import JpegXl
 from typing import Optional, List, Union, Literal, Any
 import os
+import numcodecs
 
 
+numcodecs.register_codec(JpegXl)
+
 class Mzarr:
     def __init__(self, store: Union[np.ndarray, str], mode: Literal['r', 'r+', 'a', 'w', 'w-'] = 'a') -> None:
         """
         Initialize the Mzarr instance.
 
         Args:
             store (Union[np.ndarray, str]): The array to be handled by the instance, or the
@@ -28,15 +31,18 @@
         self.path = None
         self.store = None
         self.array = None
 
         if isinstance(store, str):
             self.load(store, mode)
         else:
-            self.array = store
+            if store.dtype in [np.uint8, np.uint16, np.float16, np.float32]:
+                self.array = store
+            else:
+                raise RuntimeError("Currently only the dtypes 'uint8', 'uint16', 'float16', 'float32' are supported. Dtype {} is not supported".format(store.dtype))
 
     def load(self, path: str, mode: Literal['r', 'r+', 'a', 'a'] = 'a') -> None:
         """
         Load the Mzarr instance from a file on disk.
 
         Args:
             path (str): The path to the Mzarr file to load.
```

### Comparing `mzarr-0.0.5/mzarr/nifti2mzarr.py` & `mzarr-0.0.6/mzarr/nifti2mzarr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from tqdm import tqdm
 from os.path import join
 import os
 from natsort import natsorted
 import SimpleITK as sitk
-from mzarr.mzarr import Mzarr
+from mzarr import Mzarr
 import numpy as np
 from typing import Union, Tuple
 
 
 def all_nifti2mzarr(load_dir: str, save_dir: str, is_seg: bool, lossy: bool) -> None:
     """
     Converts all nifti files into mzarr files.
```

### Comparing `mzarr-0.0.5/mzarr/tiff2mzarr.py` & `mzarr-0.0.6/mzarr/tiff2mzarr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from os.path import join
 import os
 from os.path import join
 from natsort import natsorted
 import tifffile
-from mzarr.mzarr import Mzarr
+from mzarr import Mzarr
 import numpy as np
 
 
 def tiff2mzarr(load_dir: str, save_dir: str, is_seg: bool, lossy: bool) -> None:
     """
     Converts a tiff files of an image to a mzarr file.
```

### Comparing `mzarr-0.0.5/mzarr.egg-info/PKG-INFO` & `mzarr-0.0.6/mzarr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzarr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mzarr-0.0.5/pyproject.toml` & `mzarr-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.5/setup.cfg` & `mzarr-0.0.6/setup.cfg`

 * *Files identical despite different names*

