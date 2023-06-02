# Comparing `tmp/eodc_faas_sen2like-2023.5.0rc6.tar.gz` & `tmp/eodc_faas_sen2like-2023.5.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_sen2like-2023.5.0rc6.tar", max compression
+gzip compressed data, was "eodc_faas_sen2like-2023.5.0rc7.tar", max compression
```

## Comparing `eodc_faas_sen2like-2023.5.0rc6.tar` & `eodc_faas_sen2like-2023.5.0rc7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       27 2023-04-03 14:47:47.787253 eodc_faas_sen2like-2023.5.0rc6/README.md
--rw-r--r--   0        0        0      689 2023-06-02 08:09:31.355253 eodc_faas_sen2like-2023.5.0rc6/pyproject.toml
--rw-r--r--   0        0        0      193 2023-06-02 08:09:31.355253 eodc_faas_sen2like-2023.5.0rc6/sen2like_processor_bindings/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-08 06:47:08.031253 eodc_faas_sen2like-2023.5.0rc6/sen2like_processor_bindings/model.py
--rw-r--r--   0        0        0     4743 2023-05-08 06:47:08.031253 eodc_faas_sen2like-2023.5.0rc6/sen2like_processor_bindings/workflows.py
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.5.0rc6/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-04-03 14:47:47.787253 eodc_faas_sen2like-2023.5.0rc7/README.md
+-rw-r--r--   0        0        0      689 2023-06-02 09:41:26.919253 eodc_faas_sen2like-2023.5.0rc7/pyproject.toml
+-rw-r--r--   0        0        0      193 2023-06-02 09:41:26.919253 eodc_faas_sen2like-2023.5.0rc7/sen2like_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-08 06:47:08.031253 eodc_faas_sen2like-2023.5.0rc7/sen2like_processor_bindings/model.py
+-rw-r--r--   0        0        0     4743 2023-05-08 06:47:08.031253 eodc_faas_sen2like-2023.5.0rc7/sen2like_processor_bindings/workflows.py
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.5.0rc7/PKG-INFO
```

### Comparing `eodc_faas_sen2like-2023.5.0rc6/pyproject.toml` & `eodc_faas_sen2like-2023.5.0rc7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-sen2like"
-version = "2023.05.0-rc.6"
+version = "2023.05.0-rc.7"
 description = "Bindings for the sen2like processor exposed at EODC"
 authors = ["Valentina Hutter <valentina.hutter@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "sen2like_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_sen2like-2023.5.0rc6/sen2like_processor_bindings/model.py` & `eodc_faas_sen2like-2023.5.0rc7/sen2like_processor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_sen2like-2023.5.0rc6/sen2like_processor_bindings/workflows.py` & `eodc_faas_sen2like-2023.5.0rc7/sen2like_processor_bindings/workflows.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_sen2like-2023.5.0rc6/PKG-INFO` & `eodc_faas_sen2like-2023.5.0rc7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-sen2like
-Version: 2023.5.0rc6
+Version: 2023.5.0rc7
 Summary: Bindings for the sen2like processor exposed at EODC
 Author: Valentina Hutter
 Author-email: valentina.hutter@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

