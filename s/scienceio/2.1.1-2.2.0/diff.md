# Comparing `tmp/scienceio-2.1.1.tar.gz` & `tmp/scienceio-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scienceio-2.1.1.tar", last modified: Wed May 24 16:09:01 2023, max compression
+gzip compressed data, was "scienceio-2.2.0.tar", last modified: Fri Jun  2 17:34:41 2023, max compression
```

## Comparing `scienceio-2.1.1.tar` & `scienceio-2.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      148 2023-05-24 16:08:46.229284 scienceio-2.1.1/.flake8
--rw-r--r--   0        0        0        2 2023-05-24 16:08:46.229284 scienceio-2.1.1/.fourmat
--rw-r--r--   0        0        0      107 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      226 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1773 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/workflows/deploy_staging.yml
--rw-r--r--   0        0        0     1485 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/workflows/pull_request.yml
--rw-r--r--   0        0        0     1728 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     2371 2023-05-24 16:08:46.229284 scienceio-2.1.1/.gitignore
--rw-r--r--   0        0        0      234 2023-05-24 16:08:46.229284 scienceio-2.1.1/CODEOWNERS
--rw-r--r--   0        0        0     2588 2023-05-24 16:08:46.229284 scienceio-2.1.1/PUBLISHING.md
--rw-r--r--   0        0        0      336 2023-05-24 16:08:46.229284 scienceio-2.1.1/Pipfile
--rw-r--r--   0        0        0    36713 2023-05-24 16:08:46.229284 scienceio-2.1.1/Pipfile.lock
--rw-r--r--   0        0        0     1366 2023-05-24 16:08:46.229284 scienceio-2.1.1/README.md
--rw-r--r--   0        0        0     3083 2023-05-24 16:08:46.229284 scienceio-2.1.1/examples/analytics.py
--rw-r--r--   0        0        0     2591 2023-05-24 16:08:46.229284 scienceio-2.1.1/examples/convert_data_model.py
--rw-r--r--   0        0        0    10051 2023-05-24 16:08:46.229284 scienceio-2.1.1/examples/example-analytics-1.ipynb
--rw-r--r--   0        0        0    46436 2023-05-24 16:08:46.233284 scienceio-2.1.1/examples/example-analytics-2.ipynb
--rw-r--r--   0        0        0    12058 2023-05-24 16:08:46.233284 scienceio-2.1.1/examples/example-annotate-onboarding-text.ipynb
--rw-r--r--   0        0        0     9677 2023-05-24 16:08:46.233284 scienceio-2.1.1/examples/example-onboarding.ipynb
--rw-r--r--   0        0        0      877 2023-05-24 16:08:46.233284 scienceio-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      165 2023-05-24 16:08:46.233284 scienceio-2.1.1/src/scienceio/__init__.py
--rw-r--r--   0        0        0    10465 2023-05-24 16:08:46.233284 scienceio-2.1.1/src/scienceio/scienceio.py
--rwxr-xr-x   0        0        0       47 2023-05-24 16:08:46.233284 scienceio-2.1.1/test.sh
--rw-r--r--   0        0        0        0 2023-05-24 16:08:46.233284 scienceio-2.1.1/tests/__init__.py
--rw-r--r--   0        0        0    14998 2023-05-24 16:08:46.233284 scienceio-2.1.1/tests/__snapshots__/test_scienceio.ambr
--rw-r--r--   0        0        0     4839 2023-05-24 16:08:46.233284 scienceio-2.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2634 2023-05-24 16:08:46.233284 scienceio-2.1.1/tests/test_scienceio.py
--rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 scienceio-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      148 2023-06-02 17:34:23.499251 scienceio-2.2.0/.flake8
+-rw-r--r--   0        0        0        2 2023-06-02 17:34:23.499251 scienceio-2.2.0/.fourmat
+-rw-r--r--   0        0        0      107 2023-06-02 17:34:23.499251 scienceio-2.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      226 2023-06-02 17:34:23.499251 scienceio-2.2.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1773 2023-06-02 17:34:23.499251 scienceio-2.2.0/.github/workflows/deploy_staging.yml
+-rw-r--r--   0        0        0     1485 2023-06-02 17:34:23.499251 scienceio-2.2.0/.github/workflows/pull_request.yml
+-rw-r--r--   0        0        0     1728 2023-06-02 17:34:23.499251 scienceio-2.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2371 2023-06-02 17:34:23.499251 scienceio-2.2.0/.gitignore
+-rw-r--r--   0        0        0      234 2023-06-02 17:34:23.499251 scienceio-2.2.0/CODEOWNERS
+-rw-r--r--   0        0        0     2588 2023-06-02 17:34:23.499251 scienceio-2.2.0/PUBLISHING.md
+-rw-r--r--   0        0        0      336 2023-06-02 17:34:23.499251 scienceio-2.2.0/Pipfile
+-rw-r--r--   0        0        0    36713 2023-06-02 17:34:23.503252 scienceio-2.2.0/Pipfile.lock
+-rw-r--r--   0        0        0     1366 2023-06-02 17:34:23.503252 scienceio-2.2.0/README.md
+-rw-r--r--   0        0        0     3083 2023-06-02 17:34:23.503252 scienceio-2.2.0/examples/analytics.py
+-rw-r--r--   0        0        0     2591 2023-06-02 17:34:23.503252 scienceio-2.2.0/examples/convert_data_model.py
+-rw-r--r--   0        0        0    10051 2023-06-02 17:34:23.503252 scienceio-2.2.0/examples/example-analytics-1.ipynb
+-rw-r--r--   0        0        0    46436 2023-06-02 17:34:23.503252 scienceio-2.2.0/examples/example-analytics-2.ipynb
+-rw-r--r--   0        0        0    12058 2023-06-02 17:34:23.503252 scienceio-2.2.0/examples/example-annotate-onboarding-text.ipynb
+-rw-r--r--   0        0        0     9677 2023-06-02 17:34:23.503252 scienceio-2.2.0/examples/example-onboarding.ipynb
+-rw-r--r--   0        0        0      877 2023-06-02 17:34:23.503252 scienceio-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      165 2023-06-02 17:34:23.503252 scienceio-2.2.0/src/scienceio/__init__.py
+-rw-r--r--   0        0        0    10468 2023-06-02 17:34:23.503252 scienceio-2.2.0/src/scienceio/scienceio.py
+-rwxr-xr-x   0        0        0       47 2023-06-02 17:34:23.503252 scienceio-2.2.0/test.sh
+-rw-r--r--   0        0        0        0 2023-06-02 17:34:23.503252 scienceio-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    70505 2023-06-02 17:34:23.503252 scienceio-2.2.0/tests/__snapshots__/test_scienceio.ambr
+-rw-r--r--   0        0        0     5332 2023-06-02 17:34:23.503252 scienceio-2.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     2629 2023-06-02 17:34:23.503252 scienceio-2.2.0/tests/test_scienceio.py
+-rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 scienceio-2.2.0/PKG-INFO
```

### Comparing `scienceio-2.1.1/.github/workflows/deploy_staging.yml` & `scienceio-2.2.0/.github/workflows/deploy_staging.yml`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/.github/workflows/pull_request.yml` & `scienceio-2.2.0/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/.github/workflows/release.yml` & `scienceio-2.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/.gitignore` & `scienceio-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/PUBLISHING.md` & `scienceio-2.2.0/PUBLISHING.md`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/Pipfile.lock` & `scienceio-2.2.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/README.md` & `scienceio-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/examples/analytics.py` & `scienceio-2.2.0/examples/analytics.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/examples/convert_data_model.py` & `scienceio-2.2.0/examples/convert_data_model.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/examples/example-analytics-1.ipynb` & `scienceio-2.2.0/examples/example-analytics-1.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/examples/example-analytics-2.ipynb` & `scienceio-2.2.0/examples/example-analytics-2.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/examples/example-annotate-onboarding-text.ipynb` & `scienceio-2.2.0/examples/example-annotate-onboarding-text.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/examples/example-onboarding.ipynb` & `scienceio-2.2.0/examples/example-onboarding.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/pyproject.toml` & `scienceio-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.1/src/scienceio/scienceio.py` & `scienceio-2.2.0/src/scienceio/scienceio.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 RETRY_AFTER_HEADER = "retry-after"
 
 
 class Model(str, enum.Enum):
     STRUCTURE = "structure"
     IDENTIFY_PHI = "identify-phi"
     REDACT_PHI = "redact-phi"
+    EMBEDDINGS = "embeddings"
 
     @property
     def input_text_key_name(self) -> str:
-        if self is Model.IDENTIFY_PHI or self is Model.REDACT_PHI:
+        if self is not Model.STRUCTURE:
             return "input_text"
 
         return "text"
 
 
 class ScienceIOError(Exception):
     """Base class for all exceptions that are raised by the ScienceIO SDK."""
```

### Comparing `scienceio-2.1.1/tests/conftest.py` & `scienceio-2.2.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,36 +2,48 @@
 import pytest
 import requests_mock
 
 from typing import NamedTuple
 
 from src.scienceio import Model, ScienceIO
 
-STRUCTURE_INPUT_TEXT = (
-    "The COVID-19 pandemic has shown a markedly low proportion of cases among "
-    "children 1-4. Age disparities in observed cases could be explained by "
-    "children having lower susceptibility to infection, lower propensity to "
-    "show clinical symptoms or both."
-)
-PHI_INPUT_TEXT = (
-    "Romeo Santos made an appointment with Dr. Geoffrey Royce on December 21, "
-    "2020. Mr. Santos was complaining of symptoms of alcohol overdose, and "
-    "showed signs of possible Capgras delusion."
-)
+INPUT_TEXTS = {
+    "structure": (
+        "The COVID-19 pandemic has shown a markedly low proportion of cases among "
+        "children 1-4. Age disparities in observed cases could be explained by "
+        "children having lower susceptibility to infection, lower propensity to "
+        "show clinical symptoms or both."
+    ),
+    "identify-phi": (
+        "Romeo Santos made an appointment with Dr. Geoffrey Royce on December 21, "
+        "2020. Mr. Santos was complaining of symptoms of alcohol overdose, and "
+        "showed signs of possible Capgras delusion."
+    ),
+    "redact-phi": (
+        "Romeo Santos made an appointment with Dr. Geoffrey Royce on December 21, "
+        "2020. Mr. Santos was complaining of symptoms of alcohol overdose, and "
+        "showed signs of possible Capgras delusion."
+    ),
+    "embeddings": (
+        "Romeo Santos made an appointment with Dr. Geoffrey Royce on December 21, "
+        "2020. Mr. Santos was complaining of symptoms of alcohol overdose, and "
+        "showed signs of possible Capgras delusion."
+    ),
+}
 
 
 class ModelTestCase(NamedTuple):
     model: Model
     input_text: str
 
 
 MODEL_TEST_CASES = tuple(
     ModelTestCase(
         model=m,
-        input_text=STRUCTURE_INPUT_TEXT if m is Model.STRUCTURE else PHI_INPUT_TEXT,
+        input_text=INPUT_TEXTS[m],
     )
     for m in Model
 )
 
 MODEL_TEST_CASE_IDS = tuple(mtc.model.name.lower() for mtc in MODEL_TEST_CASES)
 
 DUMMY_REQUEST_ID = "DUMMY_REQUEST_ID"
```

### Comparing `scienceio-2.1.1/tests/test_scienceio.py` & `scienceio-2.2.0/tests/test_scienceio.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import uuid
 
 from src.scienceio import HTTPError
 
 from .conftest import (
     ERROR_TEST_CASE_IDS,
     ERROR_TEST_CASES,
+    INPUT_TEXTS,
     MODEL_TEST_CASE_IDS,
     MODEL_TEST_CASES,
-    STRUCTURE_INPUT_TEXT,
     exclude_floats,
 )
 
 
 @pytest.mark.parametrize(
     ("input_obj", "error_match"),
     (
@@ -71,15 +71,15 @@
 
 @pytest.mark.parametrize("error_test_case", ERROR_TEST_CASES, ids=ERROR_TEST_CASE_IDS)
 def test_error_cases(scio, snapshot, error_test_case):
     with requests_mock.mock() as m:
         error_test_case.patch_requests_mocker(requests_mocker=m, api_url=scio.api_url)
 
         with pytest.raises(HTTPError) as exc_info:
-            scio.structure(text=STRUCTURE_INPUT_TEXT)
+            scio.structure(text=INPUT_TEXTS["structure"])
 
         exc = exc_info.value
 
         # We want to match on status code AND error payload contents.
         error_info = {
             "status_code": exc.status_code,
             "serialized_exception": str(exc),
```

### Comparing `scienceio-2.1.1/PKG-INFO` & `scienceio-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scienceio
-Version: 2.1.1
+Version: 2.2.0
 Summary: ScienceIO Python SDK
 Author-email: ScienceIO <info@science.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Dist: requests >=2.26
```

