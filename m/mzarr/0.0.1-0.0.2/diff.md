# Comparing `tmp/Mzarr-0.0.1.tar.gz` & `tmp/mzarr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mzarr-0.0.1.tar", last modified: Fri Jun  2 06:58:13 2023, max compression
+gzip compressed data, was "mzarr-0.0.2.tar", last modified: Fri Jun  2 08:10:37 2023, max compression
```

## Comparing `Mzarr-0.0.1.tar` & `mzarr-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:58:13.975516 Mzarr-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 06:57:47.000000 Mzarr-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 06:57:47.000000 Mzarr-0.0.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:58:13.971516 Mzarr-0.0.1/Mzarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-02 06:58:13.000000 Mzarr-0.0.1/Mzarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-02 06:58:13.000000 Mzarr-0.0.1/Mzarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:58:13.000000 Mzarr-0.0.1/Mzarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 06:58:13.000000 Mzarr-0.0.1/Mzarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 06:58:13.000000 Mzarr-0.0.1/Mzarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-02 06:58:13.975516 Mzarr-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-02 06:57:47.000000 Mzarr-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:58:13.975516 Mzarr-0.0.1/mzarr/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 06:57:47.000000 Mzarr-0.0.1/mzarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:58:13.975516 Mzarr-0.0.1/mzarr/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:47.000000 Mzarr-0.0.1/mzarr/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-02 06:57:47.000000 Mzarr-0.0.1/mzarr/mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-02 06:57:47.000000 Mzarr-0.0.1/mzarr/nifti2mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-02 06:57:47.000000 Mzarr-0.0.1/mzarr/tiff2mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 06:57:47.000000 Mzarr-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-02 06:58:13.975516 Mzarr-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:58:13.975516 Mzarr-0.0.1/speed_testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:47.000000 Mzarr-0.0.1/speed_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:37.872817 mzarr-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 08:10:19.000000 mzarr-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 08:10:19.000000 mzarr-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-02 08:10:37.872817 mzarr-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-02 08:10:19.000000 mzarr-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:37.872817 mzarr-0.0.2/mzarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 08:10:19.000000 mzarr-0.0.2/mzarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:37.872817 mzarr-0.0.2/mzarr/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:19.000000 mzarr-0.0.2/mzarr/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-02 08:10:19.000000 mzarr-0.0.2/mzarr/mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-02 08:10:19.000000 mzarr-0.0.2/mzarr/nifti2mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-02 08:10:19.000000 mzarr-0.0.2/mzarr/tiff2mzarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:37.872817 mzarr-0.0.2/mzarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-02 08:10:37.000000 mzarr-0.0.2/mzarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 08:10:37.000000 mzarr-0.0.2/mzarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:10:37.000000 mzarr-0.0.2/mzarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 08:10:37.000000 mzarr-0.0.2/mzarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 08:10:37.000000 mzarr-0.0.2/mzarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 08:10:19.000000 mzarr-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-02 08:10:37.872817 mzarr-0.0.2/setup.cfg
```

### Comparing `Mzarr-0.0.1/LICENSE` & `mzarr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Mzarr-0.0.1/Mzarr.egg-info/PKG-INFO` & `mzarr-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Mzarr
-Version: 0.0.1
+Name: mzarr
+Version: 0.0.2
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -45,23 +45,17 @@
 
 - **Lossy Compression (Optional)**: In addition to lossless compression, Mzarr provides an option for using lossy JpegXL compression. This option offers even better compression ratios, which can be advantageous in scenarios where the preservation of every detail is not critical.
 
 - **Arbitrary Metadata**: Mzarr supports the storage of arbitrary metadata along with the image data. This feature allows you to associate additional information, such as annotations, tags, or custom properties, with the image.
 
 ## Installation
 
-To use the Mzarr library, follow these steps:
+You can install `mzarr` via [pip](https://pypi.org/project/Mzarr/):
 
-1. Ensure that Python 3.6 or later is installed on your system.
-2. Install the required dependencies by running the following command:
-```
-pip install numpy zarr scikit-image imagecodecs
-```
-3. Download the Mzarr library from the official repository: [Mzarr Library](https://github.com/example/Mzarr-library).
-4. Extract the library files to your desired location.
+    pip install mzarr
 
 ## Getting Started
 
 To begin using the Mzarr library, you can refer to the example code provided below:
 
 ```python
 import numpy as np
```

### Comparing `Mzarr-0.0.1/PKG-INFO` & `mzarr-0.0.2/mzarr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Mzarr
-Version: 0.0.1
+Name: mzarr
+Version: 0.0.2
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -45,23 +45,17 @@
 
 - **Lossy Compression (Optional)**: In addition to lossless compression, Mzarr provides an option for using lossy JpegXL compression. This option offers even better compression ratios, which can be advantageous in scenarios where the preservation of every detail is not critical.
 
 - **Arbitrary Metadata**: Mzarr supports the storage of arbitrary metadata along with the image data. This feature allows you to associate additional information, such as annotations, tags, or custom properties, with the image.
 
 ## Installation
 
-To use the Mzarr library, follow these steps:
+You can install `mzarr` via [pip](https://pypi.org/project/Mzarr/):
 
-1. Ensure that Python 3.6 or later is installed on your system.
-2. Install the required dependencies by running the following command:
-```
-pip install numpy zarr scikit-image imagecodecs
-```
-3. Download the Mzarr library from the official repository: [Mzarr Library](https://github.com/example/Mzarr-library).
-4. Extract the library files to your desired location.
+    pip install mzarr
 
 ## Getting Started
 
 To begin using the Mzarr library, you can refer to the example code provided below:
 
 ```python
 import numpy as np
```

### Comparing `Mzarr-0.0.1/README.md` & `mzarr-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,23 +22,17 @@
 
 - **Lossy Compression (Optional)**: In addition to lossless compression, Mzarr provides an option for using lossy JpegXL compression. This option offers even better compression ratios, which can be advantageous in scenarios where the preservation of every detail is not critical.
 
 - **Arbitrary Metadata**: Mzarr supports the storage of arbitrary metadata along with the image data. This feature allows you to associate additional information, such as annotations, tags, or custom properties, with the image.
 
 ## Installation
 
-To use the Mzarr library, follow these steps:
+You can install `mzarr` via [pip](https://pypi.org/project/Mzarr/):
 
-1. Ensure that Python 3.6 or later is installed on your system.
-2. Install the required dependencies by running the following command:
-```
-pip install numpy zarr scikit-image imagecodecs
-```
-3. Download the Mzarr library from the official repository: [Mzarr Library](https://github.com/example/Mzarr-library).
-4. Extract the library files to your desired location.
+    pip install mzarr
 
 ## Getting Started
 
 To begin using the Mzarr library, you can refer to the example code provided below:
 
 ```python
 import numpy as np
```

### Comparing `Mzarr-0.0.1/mzarr/mzarr.py` & `mzarr-0.0.2/mzarr/mzarr.py`

 * *Files identical despite different names*

### Comparing `Mzarr-0.0.1/mzarr/nifti2mzarr.py` & `mzarr-0.0.2/mzarr/nifti2mzarr.py`

 * *Files identical despite different names*

### Comparing `Mzarr-0.0.1/mzarr/tiff2mzarr.py` & `mzarr-0.0.2/mzarr/tiff2mzarr.py`

 * *Files identical despite different names*

### Comparing `Mzarr-0.0.1/pyproject.toml` & `mzarr-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Mzarr-0.0.1/setup.cfg` & `mzarr-0.0.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-name = Mzarr
+name = mzarr
 version = attr: mzarr.__version__
 description = Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Karol Gotkowski
 author_email = karol.gotkowski@dkfz.de
 license = Apache-2.0
```

