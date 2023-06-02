# Comparing `tmp/tap_checkly-0.0.3.tar.gz` & `tmp/tap_checkly-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_checkly-0.0.3.tar", max compression
+gzip compressed data, was "tap_checkly-0.0.3a1.tar", max compression
```

## Comparing `tap_checkly-0.0.3.tar` & `tap_checkly-0.0.3a1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-06-02 03:56:24.097936 tap_checkly-0.0.3/LICENSE
--rw-r--r--   0        0        0     4709 2023-06-02 03:56:24.097936 tap_checkly-0.0.3/README.md
--rw-r--r--   0        0        0     2105 2023-06-02 03:56:43.250263 tap_checkly-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       82 2023-06-02 03:56:24.097936 tap_checkly-0.0.3/tap_checkly/__init__.py
--rw-r--r--   0        0        0      116 2023-06-02 03:56:24.101936 tap_checkly-0.0.3/tap_checkly/__main__.py
--rw-r--r--   0        0        0     4867 2023-06-02 03:56:24.101936 tap_checkly-0.0.3/tap_checkly/client.py
--rw-r--r--   0        0        0   313417 2023-06-02 03:56:24.101936 tap_checkly-0.0.3/tap_checkly/openapi.json
--rw-r--r--   0        0        0     3263 2023-06-02 03:56:24.101936 tap_checkly-0.0.3/tap_checkly/streams.py
--rw-r--r--   0        0        0     1869 2023-06-02 03:56:24.101936 tap_checkly-0.0.3/tap_checkly/tap.py
--rw-r--r--   0        0        0     5679 1970-01-01 00:00:00.000000 tap_checkly-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-02 03:53:57.799993 tap_checkly-0.0.3a1/LICENSE
+-rw-r--r--   0        0        0     4709 2023-06-02 03:53:57.799993 tap_checkly-0.0.3a1/README.md
+-rw-r--r--   0        0        0     2107 2023-06-02 03:54:14.411843 tap_checkly-0.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-06-02 03:53:57.799993 tap_checkly-0.0.3a1/tap_checkly/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-02 03:53:57.799993 tap_checkly-0.0.3a1/tap_checkly/__main__.py
+-rw-r--r--   0        0        0     4867 2023-06-02 03:53:57.799993 tap_checkly-0.0.3a1/tap_checkly/client.py
+-rw-r--r--   0        0        0   313417 2023-06-02 03:53:57.803993 tap_checkly-0.0.3a1/tap_checkly/openapi.json
+-rw-r--r--   0        0        0     3263 2023-06-02 03:53:57.803993 tap_checkly-0.0.3a1/tap_checkly/streams.py
+-rw-r--r--   0        0        0     1869 2023-06-02 03:53:57.803993 tap_checkly-0.0.3a1/tap_checkly/tap.py
+-rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 tap_checkly-0.0.3a1/PKG-INFO
```

### Comparing `tap_checkly-0.0.3/LICENSE` & `tap_checkly-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.3/README.md` & `tap_checkly-0.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.3/pyproject.toml` & `tap_checkly-0.0.3a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-checkly"
-version = "0.0.3"
+version = "0.0.3a1"
 description = "Singer tap for Checkly, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-checkly"
 repository = "https://github.com/edgarrmondragon/tap-checkly"
```

### Comparing `tap_checkly-0.0.3/tap_checkly/client.py` & `tap_checkly-0.0.3a1/tap_checkly/client.py`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.3/tap_checkly/openapi.json` & `tap_checkly-0.0.3a1/tap_checkly/openapi.json`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.3/tap_checkly/streams.py` & `tap_checkly-0.0.3a1/tap_checkly/streams.py`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.3/tap_checkly/tap.py` & `tap_checkly-0.0.3a1/tap_checkly/tap.py`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.3/PKG-INFO` & `tap_checkly-0.0.3a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-checkly
-Version: 0.0.3
+Version: 0.0.3a1
 Summary: Singer tap for Checkly, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-checkly
 License: Apache-2.0
 Keywords: ELT,singer.io,Checkly
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tap-checkly Version: 0.0.3 Summary: Singer tap for
-Checkly, built with the Meltano SDK for Singer Taps. Home-page: https://
+Metadata-Version: 2.1 Name: tap-checkly Version: 0.0.3a1 Summary: Singer tap
+for Checkly, built with the Meltano SDK for Singer Taps. Home-page: https://
 github.com/edgarrmondragon/tap-checkly License: Apache-2.0 Keywords:
 ELT,singer.io,Checkly Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
 edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email:
 edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

