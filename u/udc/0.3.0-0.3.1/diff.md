# Comparing `tmp/udc-0.3.0.tar.gz` & `tmp/udc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udc-0.3.0.tar", max compression
+gzip compressed data, was "udc-0.3.1.tar", max compression
```

## Comparing `udc-0.3.0.tar` & `udc-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.3.0/LICENSE
--rw-r--r--   0        0        0     2545 2023-06-01 02:59:07.585224 udc-0.3.0/README.md
--rw-r--r--   0        0        0      799 2023-06-01 02:59:07.588789 udc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      232 2023-06-01 02:59:07.594491 udc-0.3.0/udc/__init__.py
--rw-r--r--   0        0        0     1130 2023-06-01 02:59:07.595367 udc-0.3.0/udc/benchling/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-01 02:59:07.596228 udc-0.3.0/udc/benchling/entry.py
--rw-r--r--   0        0        0      693 2023-06-01 02:59:07.596749 udc-0.3.0/udc/benchling/resource.py
--rw-r--r--   0        0        0     2244 2023-06-01 02:59:07.597617 udc-0.3.0/udc/benchling/root.py
--rw-r--r--   0        0        0      357 2023-05-31 06:12:37.912100 udc-0.3.0/udc/benchling/schema.py
--rw-r--r--   0        0        0      353 2023-05-31 06:12:37.911714 udc-0.3.0/udc/benchling/sequence.py
--rw-r--r--   0        0        0      334 2023-06-01 02:59:07.598493 udc-0.3.0/udc/main.py
--rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.3.0/udc/quilt/__init__.py
--rw-r--r--   0        0        0      275 2023-05-31 00:13:14.714433 udc-0.3.0/udc/quilt/resource.py
--rw-r--r--   0        0        0      496 2023-06-01 02:59:07.599263 udc-0.3.0/udc/types.py
--rw-r--r--   0        0        0      276 2023-06-01 02:59:07.599906 udc-0.3.0/udc/wrapper.py
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 udc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2767 2023-06-01 22:23:26.719321 udc-0.3.1/README.md
+-rw-r--r--   0        0        0      858 2023-06-01 22:23:26.722167 udc-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-06-01 02:59:07.594491 udc-0.3.1/udc/__init__.py
+-rw-r--r--   0        0        0     1130 2023-06-01 02:59:07.595367 udc-0.3.1/udc/benchling/__init__.py
+-rw-r--r--   0        0        0     3211 2023-06-01 22:23:26.724318 udc-0.3.1/udc/benchling/entry.py
+-rw-r--r--   0        0        0      693 2023-06-01 02:59:07.596749 udc-0.3.1/udc/benchling/resource.py
+-rw-r--r--   0        0        0     2944 2023-06-01 22:23:26.724733 udc-0.3.1/udc/benchling/root.py
+-rw-r--r--   0        0        0      357 2023-05-31 06:12:37.912100 udc-0.3.1/udc/benchling/schema.py
+-rw-r--r--   0        0        0      353 2023-05-31 06:12:37.911714 udc-0.3.1/udc/benchling/sequence.py
+-rw-r--r--   0        0        0      334 2023-06-01 02:59:07.598493 udc-0.3.1/udc/main.py
+-rw-r--r--   0        0        0        0 2023-06-01 22:23:26.724816 udc-0.3.1/udc/py.typed
+-rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.3.1/udc/quilt/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-31 00:13:14.714433 udc-0.3.1/udc/quilt/resource.py
+-rw-r--r--   0        0        0      558 2023-06-01 22:23:26.726307 udc-0.3.1/udc/types.py
+-rw-r--r--   0        0        0      276 2023-06-01 02:59:07.599906 udc-0.3.1/udc/wrapper.py
+-rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 udc-0.3.1/PKG-INFO
```

### Comparing `udc-0.3.0/LICENSE` & `udc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `udc-0.3.0/README.md` & `udc-0.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # UDC
 
 ## The Universal Data Client
 
 ### What is UDC?
 
-Universal Data is an open source initiative to build a decentralized, cryptographically-secure ecosystem containerizing both structured and unstructured data.
+Universal Data is an open source initiative to build
+a decentralized, cryptographically-secure ecosystem
+containerizing both structured and unstructured data.
+
 UDC is the initial (alpha) client for that system.
+It currently supports both Quilt and Benchling URIs.
+For example:
+
+- `udc list "quilt+s3://quilt-example#package=examples/wellplates"`
+- `udc patch "benchling+https://dtt.benchling.com?name=Update#type=Entry&id=etr_123"`
 
 ## Installation
 
 ### Production Package
 
 From PyPi:
```

### Comparing `udc-0.3.0/pyproject.toml` & `udc-0.3.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "udc"
-version = "0.3.0"
-description = ""
+version = "0.3.1"
+description = "The Universal Data Client command-line tool"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anyio = "^3.7.0"
 trio = "^0.22.0"
@@ -21,14 +21,15 @@
 [tool.poetry.group.dev.dependencies]
 pytest-coverage = "^0.0"
 pytest-watcher = "^0.2.6"
 pytest-asyncio = "^0.21.0"
 pytest-trio = "^0.8.0"
 pytest-codeblocks = "^0.16.1"
 ipykernel = "^6.23.1"
+mypy = "^1.3.0"
 
 [tool.poetry.scripts]
 udc = "udc.main:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `udc-0.3.0/udc/benchling/__init__.py` & `udc-0.3.1/udc/benchling/__init__.py`

 * *Files identical despite different names*

### Comparing `udc-0.3.0/udc/benchling/resource.py` & `udc-0.3.1/udc/benchling/resource.py`

 * *Files identical despite different names*

### Comparing `udc-0.3.0/udc/benchling/root.py` & `udc-0.3.1/udc/benchling/root.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 import logging
 import os
 import urllib.parse
 
 from benchling_sdk.auth.api_key_auth import ApiKeyAuth
 from benchling_sdk.benchling import Benchling
+from json import loads
 
 BENCH_ID = "id"
 BENCH_TYPE = "type"
 BENCH_TYPE_DEFAULT = "entries"
 
 
 class BenchlingRoot:
+    @staticmethod
+    def ExtractJson(result):
+        if  not isinstance(result, str) or result[0] != '{':
+            return result
+        if "'" in result:
+            result = result.replace("'", '"')
+        return loads(result)
+    
+    @staticmethod
+    def NormalizeQuery(query: dict) -> dict:
+        for key, value in query.items():
+            if isinstance(value, list): # non-parsed
+                query[key] = BenchlingRoot.ExtractJson(value[0])
+        return query
+
     BENCH_TENANT = os.environ.get("BENCHLING_TENANT_DNS")
     BENCH_ENTRY = os.environ.get("BENCHLING_ENTRY_ID")
     BENCH_AUTHOR = os.environ.get("BENCHLING_AUTHOR_ID")
     BENCH_KEY = os.environ.get("BENCHLING_API_KEY") or ""
     CLIENT = Benchling(url=f"https://{BENCH_TENANT}", auth_method=ApiKeyAuth(BENCH_KEY))
     DEFAULT_URI = f"benchling+https://{BENCH_TENANT}#type=entries"
 
@@ -44,14 +60,20 @@
 
     def base_uri(self, sub_type=None) -> str:
         type = f"{self.type}.{sub_type}" if sub_type else self.type
         base = f"benchling+https://{BenchlingRoot.BENCH_TENANT}#type={type}"
         base += f"&id={self.id}" if self.id else ""
         return base
 
+    def query_uri(self, query: dict) -> str:
+        quoted = self.quote(str(query))
+        base = self.base_uri().split("#")
+        uri = f"{base[0]}?{quoted}#{base[1]}"
+        return uri
+
     def item_uri(self, item, sub_type=None) -> str:
         base = self.base_uri(sub_type)
         logging.debug(f"item_uri.base: {base}")
         if hasattr(item, "id"):
             if "&id=" not in base:
                 base += f"&id={item.id}"
         if sub_type and hasattr(item, sub_type):
```

### Comparing `udc-0.3.0/PKG-INFO` & `udc-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: udc
-Version: 0.3.0
-Summary: 
+Version: 0.3.1
+Summary: The Universal Data Client command-line tool
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
@@ -21,16 +21,24 @@
 
 # UDC
 
 ## The Universal Data Client
 
 ### What is UDC?
 
-Universal Data is an open source initiative to build a decentralized, cryptographically-secure ecosystem containerizing both structured and unstructured data.
+Universal Data is an open source initiative to build
+a decentralized, cryptographically-secure ecosystem
+containerizing both structured and unstructured data.
+
 UDC is the initial (alpha) client for that system.
+It currently supports both Quilt and Benchling URIs.
+For example:
+
+- `udc list "quilt+s3://quilt-example#package=examples/wellplates"`
+- `udc patch "benchling+https://dtt.benchling.com?name=Update#type=Entry&id=etr_123"`
 
 ## Installation
 
 ### Production Package
 
 From PyPi:
```

