# Comparing `tmp/qualtrics_utils-0.5.7.tar.gz` & `tmp/qualtrics_utils-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualtrics_utils-0.5.7.tar", max compression
+gzip compressed data, was "qualtrics_utils-0.5.8.tar", max compression
```

## Comparing `qualtrics_utils-0.5.7.tar` & `qualtrics_utils-0.5.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1320 2023-05-15 18:07:27.778131 qualtrics_utils-0.5.7/README.md
--rw-r--r--   0        0        0      611 2023-05-30 19:20:14.599478 qualtrics_utils-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      282 2023-05-30 19:18:28.891837 qualtrics_utils-0.5.7/qualtrics_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 17:42:52.914230 qualtrics_utils-0.5.7/qualtrics_utils/codebook/__init__.py
--rw-r--r--   0        0        0     8037 2023-05-30 15:28:59.264868 qualtrics_utils-0.5.7/qualtrics_utils/codebook/generate.py
--rw-r--r--   0        0        0     3520 2023-05-30 15:27:01.951352 qualtrics_utils-0.5.7/qualtrics_utils/codebook/map_columns.py
--rw-r--r--   0        0        0     9590 2023-05-30 19:04:18.578923 qualtrics_utils-0.5.7/qualtrics_utils/survey.py
--rw-r--r--   0        0        0     2425 2023-05-30 19:11:09.822025 qualtrics_utils-0.5.7/qualtrics_utils/utils.py
--rw-r--r--   0        0        0     1978 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1320 2023-05-15 18:07:27.778131 qualtrics_utils-0.5.8/README.md
+-rw-r--r--   0        0        0      611 2023-06-02 19:34:42.840508 qualtrics_utils-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-05-30 19:18:28.891837 qualtrics_utils-0.5.8/qualtrics_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 17:42:52.914230 qualtrics_utils-0.5.8/qualtrics_utils/codebook/__init__.py
+-rw-r--r--   0        0        0     8037 2023-05-30 15:28:59.264868 qualtrics_utils-0.5.8/qualtrics_utils/codebook/generate.py
+-rw-r--r--   0        0        0     3520 2023-05-30 15:27:01.951352 qualtrics_utils-0.5.8/qualtrics_utils/codebook/map_columns.py
+-rw-r--r--   0        0        0     9590 2023-05-30 19:04:18.578923 qualtrics_utils-0.5.8/qualtrics_utils/survey.py
+-rw-r--r--   0        0        0     2434 2023-06-02 19:34:08.897522 qualtrics_utils-0.5.8/qualtrics_utils/utils.py
+-rw-r--r--   0        0        0     1978 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.8/PKG-INFO
```

### Comparing `qualtrics_utils-0.5.7/README.md` & `qualtrics_utils-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `qualtrics_utils-0.5.7/pyproject.toml` & `qualtrics_utils-0.5.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qualtrics-utils"
-version = "0.5.7"
+version = "0.5.8"
 description = "Utilities for qualtrics surveys."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 readme = "README.md"
 keywords = ["qualtrics"]
 license = "MIT"
 repository = "https://github.com/mkbabb/qualtrics-utils"
 
@@ -12,15 +12,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.2"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 numpy = "^1.24.3"
-googleapiutils2 = "^0.5.9"
+googleapiutils2 = "^0.8.5"
 mypy = "^1.3.0"
 black = "^23.3.0"
 types-requests = "^2.31.0.1"
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `qualtrics_utils-0.5.7/qualtrics_utils/codebook/generate.py` & `qualtrics_utils-0.5.8/qualtrics_utils/codebook/generate.py`

 * *Files identical despite different names*

### Comparing `qualtrics_utils-0.5.7/qualtrics_utils/codebook/map_columns.py` & `qualtrics_utils-0.5.8/qualtrics_utils/codebook/map_columns.py`

 * *Files identical despite different names*

### Comparing `qualtrics_utils-0.5.7/qualtrics_utils/survey.py` & `qualtrics_utils-0.5.8/qualtrics_utils/survey.py`

 * *Files identical despite different names*

### Comparing `qualtrics_utils-0.5.7/qualtrics_utils/utils.py` & `qualtrics_utils-0.5.8/qualtrics_utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,21 +40,21 @@
     return df
 
 
 def coalesce_multiselect(
     df: pd.DataFrame,
     codebook: list[dict[str, Any]],
     delimiter: str = ", ",
-    use_other: bool = True,
+    use_multiple: bool = True,
 ) -> pd.DataFrame:
     def join(x: pd.Series) -> str:
         l = x.dropna().tolist()
 
-        if use_other and len(l) > 1:
-            return "Other"
+        if use_multiple and len(l) > 1:
+            return "Multiple"
         else:
             return delimiter.join(l)
 
     root_questions = {}
 
     for question in codebook:
         if question["question_type"] == "MC":
```

### Comparing `qualtrics_utils-0.5.7/PKG-INFO` & `qualtrics_utils-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualtrics-utils
-Version: 0.5.7
+Version: 0.5.8
 Summary: Utilities for qualtrics surveys.
 Home-page: https://github.com/mkbabb/qualtrics-utils
 License: MIT
 Keywords: qualtrics
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

