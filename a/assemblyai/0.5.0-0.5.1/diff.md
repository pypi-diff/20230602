# Comparing `tmp/assemblyai-0.5.0.tar.gz` & `tmp/assemblyai-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.5.0.tar", last modified: Fri Jun  2 10:53:50 2023, max compression
+gzip compressed data, was "assemblyai-0.5.1.tar", last modified: Fri Jun  2 12:46:12 2023, max compression
```

## Comparing `assemblyai-0.5.0.tar` & `assemblyai-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.867332 assemblyai-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-02 10:53:30.000000 assemblyai-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-06-02 10:53:50.863332 assemblyai-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-02 10:53:30.000000 assemblyai-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.863332 assemblyai-0.5.0/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    45979 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.863332 assemblyai-0.5.0/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 10:53:50.867332 assemblyai-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-02 10:53:30.000000 assemblyai-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.863332 assemblyai-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.863332 assemblyai-0.5.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:46:12.275158 assemblyai-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-02 12:45:59.000000 assemblyai-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-06-02 12:46:12.275158 assemblyai-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-02 12:45:59.000000 assemblyai-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:46:12.267158 assemblyai-0.5.1/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-02 12:45:59.000000 assemblyai-0.5.1/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-02 12:45:59.000000 assemblyai-0.5.1/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-02 12:45:59.000000 assemblyai-0.5.1/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-02 12:45:59.000000 assemblyai-0.5.1/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-06-02 12:45:59.000000 assemblyai-0.5.1/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45979 2023-06-02 12:45:59.000000 assemblyai-0.5.1/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:46:12.271158 assemblyai-0.5.1/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-06-02 12:46:12.000000 assemblyai-0.5.1/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-02 12:46:12.000000 assemblyai-0.5.1/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:46:12.000000 assemblyai-0.5.1/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 12:46:12.000000 assemblyai-0.5.1/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 12:46:12.000000 assemblyai-0.5.1/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 12:46:12.275158 assemblyai-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-02 12:45:59.000000 assemblyai-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:46:12.271158 assemblyai-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 12:45:59.000000 assemblyai-0.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:46:12.275158 assemblyai-0.5.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 12:45:59.000000 assemblyai-0.5.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 12:45:59.000000 assemblyai-0.5.1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-02 12:45:59.000000 assemblyai-0.5.1/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 12:45:59.000000 assemblyai-0.5.1/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-02 12:45:59.000000 assemblyai-0.5.1/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-02 12:45:59.000000 assemblyai-0.5.1/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-02 12:45:59.000000 assemblyai-0.5.1/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-02 12:45:59.000000 assemblyai-0.5.1/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.5.0/LICENSE` & `assemblyai-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/PKG-INFO` & `assemblyai-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.5.0
+Version: 0.5.1
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
```

### Comparing `assemblyai-0.5.0/README.md` & `assemblyai-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/assemblyai/__init__.py` & `assemblyai-0.5.1/assemblyai/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/assemblyai/api.py` & `assemblyai-0.5.1/assemblyai/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import BinaryIO, List, Optional
+from urllib.parse import urlencode
 
 import httpx
 
 from . import types
 
 
 def _get_error_message(response: httpx.Response) -> str:
@@ -138,17 +139,19 @@
 def word_search(
     client: httpx.Client,
     transcript_id: str,
     words: List[str],
 ) -> types.WordSearchMatchResponse:
     response = client.get(
         f"/transcript/{transcript_id}/word-search",
-        params={
-            "words": words,
-        },
+        params=urlencode(
+            {
+                "words": ",".join(words),
+            }
+        ),
     )
 
     if response.status_code != httpx.codes.ok:
         raise types.TranscriptError(
             f"failed to search words in transcript {transcript_id}: {_get_error_message(response)}"
         )
```

### Comparing `assemblyai-0.5.0/assemblyai/client.py` & `assemblyai-0.5.1/assemblyai/client.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/assemblyai/lemur.py` & `assemblyai-0.5.1/assemblyai/lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/assemblyai/transcriber.py` & `assemblyai-0.5.1/assemblyai/transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/assemblyai/types.py` & `assemblyai-0.5.1/assemblyai/types.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.5.1/assemblyai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.5.0
+Version: 0.5.1
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
```

### Comparing `assemblyai-0.5.0/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.5.1/assemblyai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/setup.py` & `assemblyai-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.5.0",
+    version="0.5.1",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.5.0/tests/unit/factories.py` & `assemblyai-0.5.1/tests/unit/factories.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/tests/unit/test_domains.py` & `assemblyai-0.5.1/tests/unit/test_domains.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/tests/unit/test_lemur.py` & `assemblyai-0.5.1/tests/unit/test_lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/tests/unit/test_transcriber.py` & `assemblyai-0.5.1/tests/unit/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.5.0/tests/unit/test_transcript.py` & `assemblyai-0.5.1/tests/unit/test_transcript.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Dict, List
+from urllib.parse import urlencode
 
 import httpx
 import pytest
 from faker import Faker
 from pytest_httpx import HTTPXMock
 
 import assemblyai as aai
@@ -110,28 +111,31 @@
     )
 
     # create a mock response for the word search
     mock_word_search_response = factories.generate_dict_factory(
         factories.WordSearchMatchResponseFactory
     )()
 
+    search_words = {
+        "words": ",".join(["test", "me"]),
+    }
     # mock the specific endpoints
     url = httpx.URL(
-        f"{aai.settings.base_url}/transcript/{transcript.id}/word-search?words=test",
+        f"{aai.settings.base_url}/transcript/{transcript.id}/word-search?{urlencode(search_words)}",
     )
 
     httpx_mock.add_response(
         url=url,
         status_code=httpx.codes.OK,
         method="GET",
         json=mock_word_search_response,
     )
 
     # mimic the SDK call
-    matches = transcript.word_search(words=["test"])
+    matches = transcript.word_search(words=["test", "me"])
 
     # check integrity of the response
 
     for idx, word_search in enumerate(matches):
         assert isinstance(word_search, aai.WordSearchMatch)
         assert word_search.count == mock_word_search_response["matches"][idx]["count"]
         assert (
```

