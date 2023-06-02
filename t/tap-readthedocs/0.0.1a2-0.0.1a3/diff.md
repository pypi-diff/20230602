# Comparing `tmp/tap_readthedocs-0.0.1a2.tar.gz` & `tmp/tap_readthedocs-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_readthedocs-0.0.1a2.tar", max compression
+gzip compressed data, was "tap_readthedocs-0.0.1a3.tar", max compression
```

## Comparing `tap_readthedocs-0.0.1a2.tar` & `tap_readthedocs-0.0.1a3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-05-25 03:02:57.374803 tap_readthedocs-0.0.1a2/LICENSE
--rw-r--r--   0        0        0     2734 2023-05-25 03:02:57.374803 tap_readthedocs-0.0.1a2/README.md
--rw-r--r--   0        0        0     2295 2023-05-25 03:03:15.327073 tap_readthedocs-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0       46 2023-05-25 03:02:57.374803 tap_readthedocs-0.0.1a2/tap_readthedocs/__init__.py
--rw-r--r--   0        0        0     3690 2023-05-25 03:02:57.374803 tap_readthedocs-0.0.1a2/tap_readthedocs/client.py
--rw-r--r--   0        0        0     7210 2023-05-25 03:02:57.374803 tap_readthedocs-0.0.1a2/tap_readthedocs/streams.py
--rw-r--r--   0        0        0      836 2023-05-25 03:02:57.374803 tap_readthedocs-0.0.1a2/tap_readthedocs/tap.py
--rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 tap_readthedocs-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/LICENSE
+-rw-r--r--   0        0        0     2734 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/README.md
+-rw-r--r--   0        0        0     2296 2023-06-02 04:03:56.301317 tap_readthedocs-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/tap_readthedocs/__init__.py
+-rw-r--r--   0        0        0     3690 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/tap_readthedocs/client.py
+-rw-r--r--   0        0        0     7210 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/tap_readthedocs/streams.py
+-rw-r--r--   0        0        0      836 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/tap_readthedocs/tap.py
+-rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 tap_readthedocs-0.0.1a3/PKG-INFO
```

### Comparing `tap_readthedocs-0.0.1a2/LICENSE` & `tap_readthedocs-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.0.1a2/README.md` & `tap_readthedocs-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.0.1a2/pyproject.toml` & `tap_readthedocs-0.0.1a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core==1.6",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-readthedocs"
-version = "0.0.1a2"
+version = "0.0.1a3"
 description = "`tap-readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
     "ELT",
     "ReadTheDocs",
     "singer.io",
 ]
@@ -80,13 +80,14 @@
   "ANN201",  # missing-return-type-public-function
   "S101",    # assert
   "SLF001",  # private-member-access
 ]
 
 [tool.ruff.flake8-annotations]
 allow-star-arg-any = true
+
 [tool.ruff.isort]
 known-first-party = ["tap_readthedocs"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `tap_readthedocs-0.0.1a2/tap_readthedocs/client.py` & `tap_readthedocs-0.0.1a3/tap_readthedocs/client.py`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.0.1a2/tap_readthedocs/streams.py` & `tap_readthedocs-0.0.1a3/tap_readthedocs/streams.py`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.0.1a2/tap_readthedocs/tap.py` & `tap_readthedocs-0.0.1a3/tap_readthedocs/tap.py`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.0.1a2/PKG-INFO` & `tap_readthedocs-0.0.1a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-readthedocs
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: `tap-readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-readthedocs
 License: Apache-2.0
 Keywords: ELT,ReadTheDocs,singer.io
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tap-readthedocs Version: 0.0.1a2 Summary: `tap-
+Metadata-Version: 2.1 Name: tap-readthedocs Version: 0.0.1a3 Summary: `tap-
 readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for
 Singer Taps. Home-page: https://github.com/edgarrmondragon/tap-readthedocs
 License: Apache-2.0 Keywords: ELT,ReadTheDocs,singer.io Author: Edgar RamÃ­rez-
 MondragÃ³n Author-email: edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

