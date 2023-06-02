# Comparing `tmp/eodc_faas_sen2like-2023.5.0rc4.tar.gz` & `tmp/eodc_faas_sen2like-2023.5.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_sen2like-2023.5.0rc4.tar", max compression
+gzip compressed data, was "eodc_faas_sen2like-2023.5.0rc5.tar", max compression
```

## Comparing `eodc_faas_sen2like-2023.5.0rc4.tar` & `eodc_faas_sen2like-2023.5.0rc5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.5.0rc4/README.md
--rw-r--r--   0        0        0      689 2023-06-02 07:20:12.647253 eodc_faas_sen2like-2023.5.0rc4/pyproject.toml
--rw-r--r--   0        0        0      193 2023-06-02 07:20:12.647253 eodc_faas_sen2like-2023.5.0rc4/sen2like_processor_bindings/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-08 06:47:08.055253 eodc_faas_sen2like-2023.5.0rc4/sen2like_processor_bindings/model.py
--rw-r--r--   0        0        0     4743 2023-05-08 06:47:08.055253 eodc_faas_sen2like-2023.5.0rc4/sen2like_processor_bindings/workflows.py
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.5.0rc4/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.5.0rc5/README.md
+-rw-r--r--   0        0        0      689 2023-06-02 07:31:19.463253 eodc_faas_sen2like-2023.5.0rc5/pyproject.toml
+-rw-r--r--   0        0        0      193 2023-06-02 07:31:19.467253 eodc_faas_sen2like-2023.5.0rc5/sen2like_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-08 06:47:08.055253 eodc_faas_sen2like-2023.5.0rc5/sen2like_processor_bindings/model.py
+-rw-r--r--   0        0        0     4743 2023-05-08 06:47:08.055253 eodc_faas_sen2like-2023.5.0rc5/sen2like_processor_bindings/workflows.py
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.5.0rc5/PKG-INFO
```

### Comparing `eodc_faas_sen2like-2023.5.0rc4/pyproject.toml` & `eodc_faas_sen2like-2023.5.0rc5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-sen2like"
-version = "2023.05.0-rc.4"
+version = "2023.05.0-rc.5"
 description = "Bindings for the sen2like processor exposed at EODC"
 authors = ["Valentina Hutter <valentina.hutter@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "sen2like_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_sen2like-2023.5.0rc4/sen2like_processor_bindings/model.py` & `eodc_faas_sen2like-2023.5.0rc5/sen2like_processor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_sen2like-2023.5.0rc4/sen2like_processor_bindings/workflows.py` & `eodc_faas_sen2like-2023.5.0rc5/sen2like_processor_bindings/workflows.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_sen2like-2023.5.0rc4/PKG-INFO` & `eodc_faas_sen2like-2023.5.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-sen2like
-Version: 2023.5.0rc4
+Version: 2023.5.0rc5
 Summary: Bindings for the sen2like processor exposed at EODC
 Author: Valentina Hutter
 Author-email: valentina.hutter@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```
