# Comparing `tmp/index_503-2.1.1.tar.gz` & `tmp/index_503-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-2.1.1.tar", max compression
+gzip compressed data, was "index_503-2.2.0.tar", max compression
```

## Comparing `index_503-2.1.1.tar` & `index_503-2.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-06-02 12:00:40.339733 index_503-2.1.1/LICENSE
--rw-r--r--   0        0        0     3477 2023-06-02 12:00:40.339733 index_503-2.1.1/README.md
--rw-r--r--   0        0        0     2299 2023-06-02 12:00:41.115740 index_503-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-02 12:00:41.075740 index_503-2.1.1/src/index_503/__init__.py
--rw-r--r--   0        0        0     1147 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/cache.py
--rw-r--r--   0        0        0     1336 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/file.py
--rw-r--r--   0        0        0     6947 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/index.py
--rw-r--r--   0        0        0      434 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/main.py
--rw-r--r--   0        0        0     1840 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/metadata.py
--rw-r--r--   0        0        0     2384 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/py.typed
--rw-r--r--   0        0        0     1513 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/util.py
--rw-r--r--   0        0        0     5152 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4742 1970-01-01 00:00:00.000000 index_503-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-02 12:04:11.586886 index_503-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3477 2023-06-02 12:04:11.586886 index_503-2.2.0/README.md
+-rw-r--r--   0        0        0     2299 2023-06-02 12:04:12.386897 index_503-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-02 12:04:12.342896 index_503-2.2.0/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/cache.py
+-rw-r--r--   0        0        0     1336 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/file.py
+-rw-r--r--   0        0        0     6936 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/main.py
+-rw-r--r--   0        0        0     1840 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/py.typed
+-rw-r--r--   0        0        0     1513 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/util.py
+-rw-r--r--   0        0        0     5152 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4742 1970-01-01 00:00:00.000000 index_503-2.2.0/PKG-INFO
```

### Comparing `index_503-2.1.1/LICENSE` & `index_503-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-2.1.1/README.md` & `index_503-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `index_503-2.1.1/pyproject.toml` & `index_503-2.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "2.1.1"
+version = "2.2.0"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-2.1.1/src/index_503/cache.py` & `index_503-2.2.0/src/index_503/cache.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.1/src/index_503/file.py` & `index_503-2.2.0/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.1/src/index_503/index.py` & `index_503-2.2.0/src/index_503/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob
 import logging
 import os
 from collections import defaultdict
 from operator import attrgetter
 from pathlib import Path
-from shutil import copyfile, rmtree
+from shutil import rmtree
 from tempfile import mkdtemp
 from typing import Dict, List, Set
 
 from natsort import natsorted
 from yarl import URL
 
 from .cache import IndexCache
@@ -105,15 +105,15 @@
             target_file = temp_dir_path.joinpath(wheel_file_name)
             metadata_path = target_file.with_suffix(f"{target_file.suffix}.metadata")
             wheel_file_symlink_target = f"../{self.origin_name}/{wheel_file_name}"
 
             if (wheel_cache := raw_cache.get(wheel_file_name)) and (
                 wheel_file_obj := WheelFile.from_cache(wheel_cache)
             ):
-                copyfile(self.target_path.joinpath(metadata_path.name), metadata_path)
+                os.link(self.target_path.joinpath(metadata_path.name), metadata_path)
             elif wheel_file_obj := WheelFile.from_wheel(wheel_path, metadata_path):
                 wheel_file_name_to_metadata_path[wheel_file_name] = metadata_path
                 new_wheel_file_objects.append(wheel_file_obj)
                 raw_cache[wheel_file_name] = wheel_file_obj.as_dict()
             else:
                 continue
```

### Comparing `index_503-2.1.1/src/index_503/metadata.py` & `index_503-2.2.0/src/index_503/metadata.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.1/src/index_503/page_generator.py` & `index_503-2.2.0/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.1/src/index_503/util.py` & `index_503-2.2.0/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.1/src/index_503/wheel_file.py` & `index_503-2.2.0/src/index_503/wheel_file.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.1/PKG-INFO` & `index_503-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 2.1.1
+Version: 2.2.0
 Summary: PEP 503 index builder
 Home-page: https://github.com/bdraco/index-503
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: index-503 Version: 2.1.1 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 2.2.0 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

