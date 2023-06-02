# Comparing `tmp/index_503-2.1.0.tar.gz` & `tmp/index_503-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-2.1.0.tar", max compression
+gzip compressed data, was "index_503-2.1.1.tar", max compression
```

## Comparing `index_503-2.1.0.tar` & `index_503-2.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-06-01 19:51:55.260210 index_503-2.1.0/LICENSE
--rw-r--r--   0        0        0     3477 2023-06-01 19:51:55.260210 index_503-2.1.0/README.md
--rw-r--r--   0        0        0     2299 2023-06-01 19:51:56.032204 index_503-2.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-01 19:51:55.992205 index_503-2.1.0/src/index_503/__init__.py
--rw-r--r--   0        0        0     1147 2023-06-01 19:51:55.264210 index_503-2.1.0/src/index_503/cache.py
--rw-r--r--   0        0        0     1336 2023-06-01 19:51:55.264210 index_503-2.1.0/src/index_503/file.py
--rw-r--r--   0        0        0     6947 2023-06-01 19:51:55.264210 index_503-2.1.0/src/index_503/index.py
--rw-r--r--   0        0        0      434 2023-06-01 19:51:55.264210 index_503-2.1.0/src/index_503/main.py
--rw-r--r--   0        0        0     1840 2023-06-01 19:51:55.264210 index_503-2.1.0/src/index_503/metadata.py
--rw-r--r--   0        0        0     2384 2023-06-01 19:51:55.264210 index_503-2.1.0/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 19:51:55.264210 index_503-2.1.0/src/index_503/py.typed
--rw-r--r--   0        0        0     1513 2023-06-01 19:51:55.264210 index_503-2.1.0/src/index_503/util.py
--rw-r--r--   0        0        0     5246 2023-06-01 19:51:55.264210 index_503-2.1.0/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4742 1970-01-01 00:00:00.000000 index_503-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-02 12:00:40.339733 index_503-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3477 2023-06-02 12:00:40.339733 index_503-2.1.1/README.md
+-rw-r--r--   0        0        0     2299 2023-06-02 12:00:41.115740 index_503-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-02 12:00:41.075740 index_503-2.1.1/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/cache.py
+-rw-r--r--   0        0        0     1336 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/file.py
+-rw-r--r--   0        0        0     6947 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/main.py
+-rw-r--r--   0        0        0     1840 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/py.typed
+-rw-r--r--   0        0        0     1513 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/util.py
+-rw-r--r--   0        0        0     5152 2023-06-02 12:00:40.339733 index_503-2.1.1/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4742 1970-01-01 00:00:00.000000 index_503-2.1.1/PKG-INFO
```

### Comparing `index_503-2.1.0/LICENSE` & `index_503-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-2.1.0/README.md` & `index_503-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `index_503-2.1.0/pyproject.toml` & `index_503-2.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "2.1.0"
+version = "2.1.1"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-2.1.0/src/index_503/cache.py` & `index_503-2.1.1/src/index_503/cache.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.0/src/index_503/file.py` & `index_503-2.1.1/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.0/src/index_503/index.py` & `index_503-2.1.1/src/index_503/index.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.0/src/index_503/metadata.py` & `index_503-2.1.1/src/index_503/metadata.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.0/src/index_503/page_generator.py` & `index_503-2.1.1/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.0/src/index_503/util.py` & `index_503-2.1.1/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-2.1.0/src/index_503/wheel_file.py` & `index_503-2.1.1/src/index_503/wheel_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,14 @@
         base_url = URL(base_url)
 
         href = f"{base_url / self.filename}#{HASH_FORMAT}={self.wheel_hash}"
         kwargs = {"href": href}
 
         if self.requires_python is not None:
             kwargs["data-requires-python"] = escape(self.requires_python)
-        if self.metadata_hash is True:
-            kwargs["data-dist-info-metadata"] = "true"
         elif self.metadata_hash is not None:
             kwargs["data-dist-info-metadata"] = f"{HASH_FORMAT}={self.metadata_hash}"
 
         with page.a(**kwargs):
             page(posixpath.basename(self.filename))
 
     def update_metadata(self, metadata_path: Path) -> None:
```

### Comparing `index_503-2.1.0/PKG-INFO` & `index_503-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 2.1.0
+Version: 2.1.1
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
-Metadata-Version: 2.1 Name: index-503 Version: 2.1.0 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 2.1.1 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

