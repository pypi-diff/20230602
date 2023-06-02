# Comparing `tmp/mzarr-0.0.3.tar.gz` & `tmp/mzarr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzarr-0.0.3.tar", last modified: Fri Jun  2 08:12:16 2023, max compression
+gzip compressed data, was "mzarr-0.0.4.tar", last modified: Fri Jun  2 08:14:58 2023, max compression
```

## Comparing `mzarr-0.0.3.tar` & `mzarr-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:12:16.891579 mzarr-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 08:12:00.000000 mzarr-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 08:12:00.000000 mzarr-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-02 08:12:16.891579 mzarr-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-02 08:12:00.000000 mzarr-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:12:16.891579 mzarr-0.0.3/mzarr/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 08:12:00.000000 mzarr-0.0.3/mzarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:12:16.891579 mzarr-0.0.3/mzarr/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:12:00.000000 mzarr-0.0.3/mzarr/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-02 08:12:00.000000 mzarr-0.0.3/mzarr/mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-02 08:12:00.000000 mzarr-0.0.3/mzarr/nifti2mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-02 08:12:00.000000 mzarr-0.0.3/mzarr/tiff2mzarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:12:16.891579 mzarr-0.0.3/mzarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-02 08:12:16.000000 mzarr-0.0.3/mzarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 08:12:16.000000 mzarr-0.0.3/mzarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:12:16.000000 mzarr-0.0.3/mzarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 08:12:16.000000 mzarr-0.0.3/mzarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 08:12:16.000000 mzarr-0.0.3/mzarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 08:12:00.000000 mzarr-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-02 08:12:16.891579 mzarr-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:58.449194 mzarr-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 08:14:36.000000 mzarr-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 08:14:36.000000 mzarr-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 08:14:58.449194 mzarr-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-02 08:14:36.000000 mzarr-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:58.449194 mzarr-0.0.4/mzarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:58.449194 mzarr-0.0.4/mzarr/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/nifti2mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/tiff2mzarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:58.449194 mzarr-0.0.4/mzarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 08:14:36.000000 mzarr-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-02 08:14:58.449194 mzarr-0.0.4/setup.cfg
```

### Comparing `mzarr-0.0.3/LICENSE` & `mzarr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.3/PKG-INFO` & `mzarr-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzarr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,24 +22,23 @@
 License-File: LICENSE
 
 # Mzarr
 
 [![License Apache Software License 2.0](https://img.shields.io/pypi/l/mzarr.svg?color=green)](https://github.com/Karol-G/mzarr/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/mzarr.svg?color=green)](https://pypi.org/project/mzarr)
 [![Python Version](https://img.shields.io/pypi/pyversions/mzarr.svg?color=green)](https://python.org)
-[![tests](https://github.com/Karol-G/mzarr/workflows/tests/badge.svg)](https://github.com/Karol-G/mzarr/actions)
 [![codecov](https://codecov.io/gh/Karol-G/mzarr/branch/main/graph/badge.svg)](https://codecov.io/gh/Karol-G/mzarr)
 
 Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format, designed specifically for 2D and 3D data. Mzarr provides a comprehensive solution for storing, compressing, and efficiently manipulating image data with multi-resolution views. This readme provides an overview of the Mzarr library and its key features.
 
 ## Features
 
 - **Multi-Resolution Views**: Mzarr supports multi-resolution representations of image data, allowing fast and efficient viewing at different levels of detail. This feature enables quick navigation and exploration of large images. Typically, this creates only a ~10% overhead.
 
-  **Low Memory Consumption** Mzarr requires almost no memory even when loading and vieweing large multi-dimensional images due to memory-mapping, chunking and its multi-resolution views.
+- **Low Memory Consumption** Mzarr requires almost no memory even when loading and vieweing large multi-dimensional images due to memory-mapping, chunking and its multi-resolution views.
 
 - **Automatic Chunking**: Mzarr incorporates automatic chunking for optimal performance. The library intelligently divides the image data into smaller chunks, resulting in fast loading, saving, and manipulation operations. Chunking also enables memory mapping of the image for efficient usage of system resources.
 
 - **Array-Like Slicing**: Mzarr supports array-like slicing, allowing users to extract specific regions or subsets of the image data. This feature enables the selection of portions of the image based on desired coordinates, indices, or ranges. Array-like slicing provides flexibility in manipulating and analyzing the image data by operating only on the selected regions of interest. It avoids the need to load the entire dataset into memory, resulting in efficient memory usage and faster processing times.
 
 - **Lossless Compression**: Mzarr utilizes the modern lossless JpegXL compressor for compressing the image data on a chunk basis. This compression method offers improved compression benefits compared to other 2D and 3D image formats. The chunk-based compression enables memory mapping of the image while still achieving high compression ratios.
```

### Comparing `mzarr-0.0.3/README.md` & `mzarr-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Mzarr
 
 [![License Apache Software License 2.0](https://img.shields.io/pypi/l/mzarr.svg?color=green)](https://github.com/Karol-G/mzarr/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/mzarr.svg?color=green)](https://pypi.org/project/mzarr)
 [![Python Version](https://img.shields.io/pypi/pyversions/mzarr.svg?color=green)](https://python.org)
-[![tests](https://github.com/Karol-G/mzarr/workflows/tests/badge.svg)](https://github.com/Karol-G/mzarr/actions)
 [![codecov](https://codecov.io/gh/Karol-G/mzarr/branch/main/graph/badge.svg)](https://codecov.io/gh/Karol-G/mzarr)
 
 Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format, designed specifically for 2D and 3D data. Mzarr provides a comprehensive solution for storing, compressing, and efficiently manipulating image data with multi-resolution views. This readme provides an overview of the Mzarr library and its key features.
 
 ## Features
 
 - **Multi-Resolution Views**: Mzarr supports multi-resolution representations of image data, allowing fast and efficient viewing at different levels of detail. This feature enables quick navigation and exploration of large images. Typically, this creates only a ~10% overhead.
 
-  **Low Memory Consumption** Mzarr requires almost no memory even when loading and vieweing large multi-dimensional images due to memory-mapping, chunking and its multi-resolution views.
+- **Low Memory Consumption** Mzarr requires almost no memory even when loading and vieweing large multi-dimensional images due to memory-mapping, chunking and its multi-resolution views.
 
 - **Automatic Chunking**: Mzarr incorporates automatic chunking for optimal performance. The library intelligently divides the image data into smaller chunks, resulting in fast loading, saving, and manipulation operations. Chunking also enables memory mapping of the image for efficient usage of system resources.
 
 - **Array-Like Slicing**: Mzarr supports array-like slicing, allowing users to extract specific regions or subsets of the image data. This feature enables the selection of portions of the image based on desired coordinates, indices, or ranges. Array-like slicing provides flexibility in manipulating and analyzing the image data by operating only on the selected regions of interest. It avoids the need to load the entire dataset into memory, resulting in efficient memory usage and faster processing times.
 
 - **Lossless Compression**: Mzarr utilizes the modern lossless JpegXL compressor for compressing the image data on a chunk basis. This compression method offers improved compression benefits compared to other 2D and 3D image formats. The chunk-based compression enables memory mapping of the image while still achieving high compression ratios.
```

### Comparing `mzarr-0.0.3/mzarr/mzarr.py` & `mzarr-0.0.4/mzarr/mzarr.py`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.3/mzarr/nifti2mzarr.py` & `mzarr-0.0.4/mzarr/nifti2mzarr.py`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.3/mzarr/tiff2mzarr.py` & `mzarr-0.0.4/mzarr/tiff2mzarr.py`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.3/mzarr.egg-info/PKG-INFO` & `mzarr-0.0.4/mzarr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzarr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,24 +22,23 @@
 License-File: LICENSE
 
 # Mzarr
 
 [![License Apache Software License 2.0](https://img.shields.io/pypi/l/mzarr.svg?color=green)](https://github.com/Karol-G/mzarr/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/mzarr.svg?color=green)](https://pypi.org/project/mzarr)
 [![Python Version](https://img.shields.io/pypi/pyversions/mzarr.svg?color=green)](https://python.org)
-[![tests](https://github.com/Karol-G/mzarr/workflows/tests/badge.svg)](https://github.com/Karol-G/mzarr/actions)
 [![codecov](https://codecov.io/gh/Karol-G/mzarr/branch/main/graph/badge.svg)](https://codecov.io/gh/Karol-G/mzarr)
 
 Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format, designed specifically for 2D and 3D data. Mzarr provides a comprehensive solution for storing, compressing, and efficiently manipulating image data with multi-resolution views. This readme provides an overview of the Mzarr library and its key features.
 
 ## Features
 
 - **Multi-Resolution Views**: Mzarr supports multi-resolution representations of image data, allowing fast and efficient viewing at different levels of detail. This feature enables quick navigation and exploration of large images. Typically, this creates only a ~10% overhead.
 
-  **Low Memory Consumption** Mzarr requires almost no memory even when loading and vieweing large multi-dimensional images due to memory-mapping, chunking and its multi-resolution views.
+- **Low Memory Consumption** Mzarr requires almost no memory even when loading and vieweing large multi-dimensional images due to memory-mapping, chunking and its multi-resolution views.
 
 - **Automatic Chunking**: Mzarr incorporates automatic chunking for optimal performance. The library intelligently divides the image data into smaller chunks, resulting in fast loading, saving, and manipulation operations. Chunking also enables memory mapping of the image for efficient usage of system resources.
 
 - **Array-Like Slicing**: Mzarr supports array-like slicing, allowing users to extract specific regions or subsets of the image data. This feature enables the selection of portions of the image based on desired coordinates, indices, or ranges. Array-like slicing provides flexibility in manipulating and analyzing the image data by operating only on the selected regions of interest. It avoids the need to load the entire dataset into memory, resulting in efficient memory usage and faster processing times.
 
 - **Lossless Compression**: Mzarr utilizes the modern lossless JpegXL compressor for compressing the image data on a chunk basis. This compression method offers improved compression benefits compared to other 2D and 3D image formats. The chunk-based compression enables memory mapping of the image while still achieving high compression ratios.
```

### Comparing `mzarr-0.0.3/pyproject.toml` & `mzarr-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.3/setup.cfg` & `mzarr-0.0.4/setup.cfg`

 * *Files identical despite different names*

