# Comparing `tmp/mzarr-0.0.4.tar.gz` & `tmp/mzarr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzarr-0.0.4.tar", last modified: Fri Jun  2 08:14:58 2023, max compression
+gzip compressed data, was "mzarr-0.0.5.tar", last modified: Fri Jun  2 09:07:46 2023, max compression
```

## Comparing `mzarr-0.0.4.tar` & `mzarr-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:58.449194 mzarr-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 08:14:36.000000 mzarr-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 08:14:36.000000 mzarr-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 08:14:58.449194 mzarr-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-02 08:14:36.000000 mzarr-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:58.449194 mzarr-0.0.4/mzarr/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:58.449194 mzarr-0.0.4/mzarr/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/nifti2mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-02 08:14:36.000000 mzarr-0.0.4/mzarr/tiff2mzarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:14:58.449194 mzarr-0.0.4/mzarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 08:14:58.000000 mzarr-0.0.4/mzarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 08:14:36.000000 mzarr-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-02 08:14:58.449194 mzarr-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:46.961016 mzarr-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 09:07:24.000000 mzarr-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 09:07:24.000000 mzarr-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 09:07:46.961016 mzarr-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-02 09:07:24.000000 mzarr-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:46.961016 mzarr-0.0.5/mzarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:46.961016 mzarr-0.0.5/mzarr/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/nifti2mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-02 09:07:24.000000 mzarr-0.0.5/mzarr/tiff2mzarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:07:46.961016 mzarr-0.0.5/mzarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 09:07:46.000000 mzarr-0.0.5/mzarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 09:07:24.000000 mzarr-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-02 09:07:46.965016 mzarr-0.0.5/setup.cfg
```

### Comparing `mzarr-0.0.4/LICENSE` & `mzarr-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.4/PKG-INFO` & `mzarr-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzarr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mzarr-0.0.4/README.md` & `mzarr-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.4/mzarr/mzarr.py` & `mzarr-0.0.5/mzarr/mzarr.py`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.4/mzarr/nifti2mzarr.py` & `mzarr-0.0.5/mzarr/nifti2mzarr.py`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.4/mzarr/tiff2mzarr.py` & `mzarr-0.0.5/mzarr/tiff2mzarr.py`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.4/mzarr.egg-info/PKG-INFO` & `mzarr-0.0.5/mzarr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzarr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mzarr-0.0.4/pyproject.toml` & `mzarr-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.4/setup.cfg` & `mzarr-0.0.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering :: Image Processing
 
 [options]
 packages = find:
 install_requires = 
 	numpy
+	scikit-image>=0.19
+	natsort
+	numcodecs
+	imagecodecs==2023.1.23
+	zarr
+	tifffile
 python_requires = >=3.8
 include_package_data = True
 
 [options.extras_require]
 testing = 
 	tox
 	pytest  # https://docs.pytest.org/en/latest/contents.html
```

