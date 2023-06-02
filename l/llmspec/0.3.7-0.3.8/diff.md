# Comparing `tmp/llmspec-0.3.7.tar.gz` & `tmp/llmspec-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmspec-0.3.7.tar", last modified: Wed May 31 08:16:23 2023, max compression
+gzip compressed data, was "llmspec-0.3.8.tar", last modified: Fri Jun  2 03:35:36 2023, max compression
```

## Comparing `llmspec-0.3.7.tar` & `llmspec-0.3.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11098 2023-05-31 08:16:07.065581 llmspec-0.3.7/LICENSE
--rw-r--r--   0        0        0       33 2023-05-31 08:16:07.065581 llmspec-0.3.7/README.md
--rw-r--r--   0        0        0      659 2023-05-31 08:16:07.065581 llmspec-0.3.7/llmspec/__init__.py
--rw-r--r--   0        0        0     9917 2023-05-31 08:16:07.065581 llmspec-0.3.7/llmspec/llmspec.py
--rw-r--r--   0        0        0      215 2023-05-31 08:16:07.065581 llmspec-0.3.7/llmspec/mixins.py
--rw-r--r--   0        0        0     1130 2023-05-31 08:16:23.211062 llmspec-0.3.7/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-31 08:16:07.065581 llmspec-0.3.7/tests/dummy_test.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11098 2023-06-02 03:35:25.098366 llmspec-0.3.8/LICENSE
+-rw-r--r--   0        0        0       33 2023-06-02 03:35:25.098366 llmspec-0.3.8/README.md
+-rw-r--r--   0        0        0      659 2023-06-02 03:35:25.098366 llmspec-0.3.8/llmspec/__init__.py
+-rw-r--r--   0        0        0     9928 2023-06-02 03:35:25.102367 llmspec-0.3.8/llmspec/llmspec.py
+-rw-r--r--   0        0        0      215 2023-06-02 03:35:25.102367 llmspec-0.3.8/llmspec/mixins.py
+-rw-r--r--   0        0        0     1130 2023-06-02 03:35:36.530713 llmspec-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-06-02 03:35:25.102367 llmspec-0.3.8/tests/dummy_test.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.8/PKG-INFO
```

### Comparing `llmspec-0.3.7/LICENSE` & `llmspec-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.7/llmspec/__init__.py` & `llmspec-0.3.8/llmspec/__init__.py`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.7/llmspec/llmspec.py` & `llmspec-0.3.8/llmspec/llmspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,20 +321,19 @@
                 completion_tokens=completion_token,
                 total_tokens=prompt_token + completion_token,
             ),
         )
 
 
 class EmbeddingRequest(msgspec.Struct, JSONSerializableMixin):
-    model: str
-    input: Union[str, List[str]]
+    model: str = ""
+    input: Union[str, List[str]] = None
     user: str = ""
     encoding_format: str = "json"
 
-
 class EmbeddingData(msgspec.Struct):
     embedding: Union[List[float], str]
     index: int
     object: str = "embedding"
 
 
 class EmbeddingResponse(msgspec.Struct, JSONSerializableMixin):
```

### Comparing `llmspec-0.3.7/pyproject.toml` & `llmspec-0.3.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "msgspec>=0.15.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.7"
+version = "0.3.8"
 
 [project.license]
 text = "Apache-2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
```

