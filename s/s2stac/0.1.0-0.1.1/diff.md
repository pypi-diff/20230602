# Comparing `tmp/s2stac-0.1.0.tar.gz` & `tmp/s2stac-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2stac-0.1.0.tar", max compression
+gzip compressed data, was "s2stac-0.1.1.tar", max compression
```

## Comparing `s2stac-0.1.0.tar` & `s2stac-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-05-12 11:45:52.630479 s2stac-0.1.0/LICENSE
--rw-r--r--   0        0        0      180 2023-05-12 11:49:10.724550 s2stac-0.1.0/README.md
--rw-r--r--   0        0        0      842 2023-05-17 14:05:25.774454 s2stac-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      257 2023-06-02 14:18:31.109651 s2stac-0.1.0/src/s2stac/__init__.py
--rw-r--r--   0        0        0     1547 2023-06-02 14:01:10.199802 s2stac-0.1.0/src/s2stac/_asset.py
--rw-r--r--   0        0        0     2083 2023-06-02 14:04:14.981564 s2stac-0.1.0/src/s2stac/_aux_data.py
--rw-r--r--   0        0        0     5341 2023-06-02 14:11:15.429545 s2stac-0.1.0/src/s2stac/_catalog.py
--rw-r--r--   0        0        0     1897 2023-06-02 14:12:37.734322 s2stac-0.1.0/src/s2stac/_img_data.py
--rw-r--r--   0        0        0     8005 2023-06-02 14:11:18.809577 s2stac-0.1.0/src/s2stac/_mtd_tl.py
--rw-r--r--   0        0        0     2147 2023-06-02 13:07:54.221429 s2stac-0.1.0/src/s2stac/_preview.py
--rw-r--r--   0        0        0     5299 2023-06-02 14:07:20.715326 s2stac-0.1.0/src/s2stac/_qi_data.py
--rw-r--r--   0        0        0     1347 2023-06-02 14:24:16.588701 s2stac-0.1.0/src/s2stac/_stacify.py
--rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 s2stac-0.1.0/setup.py
--rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 s2stac-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-12 11:45:52.630479 s2stac-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2706 2023-06-02 15:15:37.888859 s2stac-0.1.1/README.md
+-rw-r--r--   0        0        0      843 2023-06-02 15:24:35.301230 s2stac-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      257 2023-06-02 14:18:31.109651 s2stac-0.1.1/src/s2stac/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-02 14:01:10.199802 s2stac-0.1.1/src/s2stac/_asset.py
+-rw-r--r--   0        0        0     2083 2023-06-02 14:04:14.981564 s2stac-0.1.1/src/s2stac/_aux_data.py
+-rw-r--r--   0        0        0     5341 2023-06-02 14:11:15.429545 s2stac-0.1.1/src/s2stac/_catalog.py
+-rw-r--r--   0        0        0     1897 2023-06-02 14:12:37.734322 s2stac-0.1.1/src/s2stac/_img_data.py
+-rw-r--r--   0        0        0     8005 2023-06-02 14:11:18.809577 s2stac-0.1.1/src/s2stac/_mtd_tl.py
+-rw-r--r--   0        0        0     2147 2023-06-02 13:07:54.221429 s2stac-0.1.1/src/s2stac/_preview.py
+-rw-r--r--   0        0        0     5299 2023-06-02 14:07:20.715326 s2stac-0.1.1/src/s2stac/_qi_data.py
+-rw-r--r--   0        0        0     1347 2023-06-02 14:24:16.588701 s2stac-0.1.1/src/s2stac/_stacify.py
+-rw-r--r--   0        0        0     4016 1970-01-01 00:00:00.000000 s2stac-0.1.1/setup.py
+-rw-r--r--   0        0        0     3916 1970-01-01 00:00:00.000000 s2stac-0.1.1/PKG-INFO
```

### Comparing `s2stac-0.1.0/LICENSE` & `s2stac-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.0/pyproject.toml` & `s2stac-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "s2stac"
-version = "0.1.0"
+version = "0.1.1"
 description = "Create a STAC from local S2 data."
 authors = ["Pierre Louvart <pierre.louvart@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "3.10.5"
+python = "^3.10.5"
 xarray = "^2023.4.2"
 pystac = "^1.7.3"
 shapely = "1.8.5"
 rasterio = "^1.3.6"
 rioxarray = "^0.14.1"
 numpy = "^1.24.3"
 stackstac = "^0.4.3"
```

### Comparing `s2stac-0.1.0/src/s2stac/_asset.py` & `s2stac-0.1.1/src/s2stac/_asset.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.0/src/s2stac/_aux_data.py` & `s2stac-0.1.1/src/s2stac/_aux_data.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.0/src/s2stac/_catalog.py` & `s2stac-0.1.1/src/s2stac/_catalog.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.0/src/s2stac/_img_data.py` & `s2stac-0.1.1/src/s2stac/_img_data.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.0/src/s2stac/_mtd_tl.py` & `s2stac-0.1.1/src/s2stac/_mtd_tl.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.0/src/s2stac/_preview.py` & `s2stac-0.1.1/src/s2stac/_preview.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.0/src/s2stac/_qi_data.py` & `s2stac-0.1.1/src/s2stac/_qi_data.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.0/src/s2stac/_stacify.py` & `s2stac-0.1.1/src/s2stac/_stacify.py`

 * *Files identical despite different names*

