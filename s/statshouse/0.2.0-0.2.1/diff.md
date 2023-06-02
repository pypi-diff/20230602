# Comparing `tmp/statshouse-0.2.0.tar.gz` & `tmp/statshouse-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statshouse-0.2.0.tar", last modified: Thu May 25 16:10:34 2023, max compression
+gzip compressed data, was "statshouse-0.2.1.tar", last modified: Fri Jun  2 11:34:29 2023, max compression
```

## Comparing `statshouse-0.2.0.tar` & `statshouse-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    16727 2022-11-28 20:50:24.714223 statshouse-0.2.0/LICENSE
--rw-r--r--   0        0        0      943 2023-05-25 16:09:41.327601 statshouse-0.2.0/README.md
--rw-r--r--   0        0        0     1083 2023-05-25 16:10:34.331503 statshouse-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       83 2023-05-25 16:09:41.327601 statshouse-0.2.0/src/statshouse/__init__.py
--rw-r--r--   0        0        0     3813 2023-05-25 16:09:41.327601 statshouse-0.2.0/src/statshouse/_statshouse.py
--rw-r--r--   0        0        0      104 2023-05-25 16:09:41.327601 statshouse-0.2.0/tests/test_statshouse.py
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 statshouse-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    16727 2022-11-28 20:50:24.714223 statshouse-0.2.1/LICENSE
+-rw-r--r--   0        0        0      943 2023-05-25 16:09:41.327601 statshouse-0.2.1/README.md
+-rw-r--r--   0        0        0     1083 2023-06-02 11:34:29.307764 statshouse-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-06-02 11:18:06.879315 statshouse-0.2.1/src/statshouse/__init__.py
+-rw-r--r--   0        0        0     3852 2023-06-02 11:17:34.943336 statshouse-0.2.1/src/statshouse/_statshouse.py
+-rw-r--r--   0        0        0      195 2023-06-02 11:18:06.879315 statshouse-0.2.1/tests/test_statshouse.py
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 statshouse-0.2.1/PKG-INFO
```

### Comparing `statshouse-0.2.0/LICENSE` & `statshouse-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statshouse-0.2.0/README.md` & `statshouse-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `statshouse-0.2.0/pyproject.toml` & `statshouse-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "statshouse"
-version = "0.2.0"
+version = "0.2.1"
 description = "StatsHouse client library for Python"
 authors = [
     { name = "Gregory Petrosyan", email = "pgregory@pgregory.net" },
 ]
 dependencies = [
     "msgpack>=1.0.5",
 ]
```

### Comparing `statshouse-0.2.0/src/statshouse/_statshouse.py` & `statshouse-0.2.1/src/statshouse/_statshouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from typing import Dict, List, Optional, Sequence, Tuple, TypeVar, Union
 
 import msgpack
 
 
 DEFAULT_STATSHOUSE_ADDR = "127.0.0.1:13337"
 
+TAG_STRING_TOP = "_s"
+TAG_HOST = "_h"
+
 T = TypeVar("T")
 OneOrMany = Union[T, Sequence[T]]
 Tags = Union[Tuple[Optional[str], ...], List[Optional[str]], Dict[str, str]]
 
 
 class StatsHouse:
     def __init__(self, addr: str, env: str):
```

### Comparing `statshouse-0.2.0/PKG-INFO` & `statshouse-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statshouse
-Version: 0.2.0
+Version: 0.2.1
 Summary: StatsHouse client library for Python
 Author-Email: Gregory Petrosyan <pgregory@pgregory.net>
 License: MPL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

