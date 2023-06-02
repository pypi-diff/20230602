# Comparing `tmp/transformer_embeddings-4.0.1.tar.gz` & `tmp/transformer_embeddings-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer_embeddings-4.0.1.tar", max compression
+gzip compressed data, was "transformer_embeddings-4.0.2.tar", max compression
```

## Comparing `transformer_embeddings-4.0.1.tar` & `transformer_embeddings-4.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11334 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/LICENSE
--rw-r--r--   0        0        0     5529 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/README.md
--rw-r--r--   0        0        0     1833 2023-05-23 15:09:07.689742 transformer_embeddings-4.0.1/pyproject.toml
--rw-r--r--   0        0        0      192 2023-05-23 15:09:07.669742 transformer_embeddings-4.0.1/src/transformer_embeddings/__init__.py
--rw-r--r--   0        0        0     2100 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/src/transformer_embeddings/helpers.py
--rw-r--r--   0        0        0    11612 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/src/transformer_embeddings/model.py
--rw-r--r--   0        0        0     1828 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/src/transformer_embeddings/poolers.py
--rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 transformer_embeddings-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-06-02 21:06:54.687532 transformer_embeddings-4.0.2/LICENSE
+-rw-r--r--   0        0        0     5529 2023-06-02 21:06:54.687532 transformer_embeddings-4.0.2/README.md
+-rw-r--r--   0        0        0     1833 2023-06-02 21:07:11.767737 transformer_embeddings-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-06-02 21:07:11.751737 transformer_embeddings-4.0.2/src/transformer_embeddings/__init__.py
+-rw-r--r--   0        0        0     2100 2023-06-02 21:06:54.691532 transformer_embeddings-4.0.2/src/transformer_embeddings/helpers.py
+-rw-r--r--   0        0        0    11612 2023-06-02 21:06:54.691532 transformer_embeddings-4.0.2/src/transformer_embeddings/model.py
+-rw-r--r--   0        0        0     1828 2023-06-02 21:06:54.691532 transformer_embeddings-4.0.2/src/transformer_embeddings/poolers.py
+-rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 transformer_embeddings-4.0.2/PKG-INFO
```

### Comparing `transformer_embeddings-4.0.1/LICENSE` & `transformer_embeddings-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.1/README.md` & `transformer_embeddings-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.1/pyproject.toml` & `transformer_embeddings-4.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformer-embeddings"
-version = "4.0.1"
+version = "4.0.2"
 description = "Transformer Embeddings"
 authors = ["Headspace Health <transformer-embeddings@headspace.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ginger-io/transformer-embeddings"
 repository = "https://github.com/ginger-io/transformer-embeddings"
 documentation = "https://github.com/ginger-io/transformer-embeddings"
```

### Comparing `transformer_embeddings-4.0.1/src/transformer_embeddings/helpers.py` & `transformer_embeddings-4.0.2/src/transformer_embeddings/helpers.py`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.1/src/transformer_embeddings/model.py` & `transformer_embeddings-4.0.2/src/transformer_embeddings/model.py`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.1/src/transformer_embeddings/poolers.py` & `transformer_embeddings-4.0.2/src/transformer_embeddings/poolers.py`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.1/PKG-INFO` & `transformer_embeddings-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformer-embeddings
-Version: 4.0.1
+Version: 4.0.2
 Summary: Transformer Embeddings
 Home-page: https://github.com/ginger-io/transformer-embeddings
 License: Apache-2.0
 Author: Headspace Health
 Author-email: transformer-embeddings@headspace.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 5 - Production/Stable
```

