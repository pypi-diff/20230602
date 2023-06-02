# Comparing `tmp/cattrs-23.1.1.tar.gz` & `tmp/cattrs-23.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cattrs-23.1.1.tar", max compression
+gzip compressed data, was "cattrs-23.1.2.tar", max compression
```

## Comparing `cattrs-23.1.1.tar` & `cattrs-23.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1074 2022-02-11 01:34:09.478875 cattrs-23.1.1/LICENSE
--rw-r--r--   0        0        0     7516 2023-04-15 23:55:47.832298 cattrs-23.1.1/README.md
--rw-r--r--   0        0        0     2450 2023-05-30 21:15:10.640943 cattrs-23.1.1/pyproject.toml
--rw-r--r--   0        0        0      906 2022-04-16 01:20:23.203198 cattrs-23.1.1/src/cattr/__init__.py
--rw-r--r--   0        0        0      192 2022-04-16 01:20:23.203198 cattrs-23.1.1/src/cattr/converters.py
--rw-r--r--   0        0        0      103 2022-04-16 01:20:23.203198 cattrs-23.1.1/src/cattr/disambiguators.py
--rw-r--r--   0        0        0      125 2022-04-16 01:20:23.203198 cattrs-23.1.1/src/cattr/dispatch.py
--rw-r--r--   0        0        0      343 2022-07-06 00:23:52.229650 cattrs-23.1.1/src/cattr/errors.py
--rw-r--r--   0        0        0      520 2022-02-11 01:34:09.486876 cattrs-23.1.1/src/cattr/gen.py
--rw-r--r--   0        0        0       78 2022-04-16 01:20:23.203198 cattrs-23.1.1/src/cattr/preconf/__init__.py
--rw-r--r--   0        0        0      194 2023-03-02 01:10:10.360770 cattrs-23.1.1/src/cattr/preconf/bson.py
--rw-r--r--   0        0        0      205 2023-03-02 01:10:10.360770 cattrs-23.1.1/src/cattr/preconf/json.py
--rw-r--r--   0        0        0      206 2023-03-02 01:10:10.360770 cattrs-23.1.1/src/cattr/preconf/msgpack.py
--rw-r--r--   0        0        0      202 2023-03-02 01:10:10.360770 cattrs-23.1.1/src/cattr/preconf/orjson.py
--rw-r--r--   0        0        0      202 2023-03-02 01:10:10.360770 cattrs-23.1.1/src/cattr/preconf/pyyaml.py
--rw-r--r--   0        0        0      206 2023-03-02 01:10:10.360770 cattrs-23.1.1/src/cattr/preconf/tomlkit.py
--rw-r--r--   0        0        0      198 2023-03-02 01:10:10.360770 cattrs-23.1.1/src/cattr/preconf/ujson.py
--rw-r--r--   0        0        0        0 2022-02-11 01:34:09.486876 cattrs-23.1.1/src/cattr/py.typed
--rw-r--r--   0        0        0     1631 2023-04-15 23:55:47.836298 cattrs-23.1.1/src/cattrs/__init__.py
--rw-r--r--   0        0        0    15501 2023-05-23 23:14:04.606233 cattrs-23.1.1/src/cattrs/_compat.py
--rw-r--r--   0        0        0      678 2022-04-10 01:46:50.855243 cattrs-23.1.1/src/cattrs/_generics.py
--rw-r--r--   0        0        0    41450 2023-05-22 17:11:08.762741 cattrs-23.1.1/src/cattrs/converters.py
--rw-r--r--   0        0        0     2243 2023-03-02 01:10:10.360770 cattrs-23.1.1/src/cattrs/disambiguators.py
--rw-r--r--   0        0        0     4654 2023-03-02 01:10:10.360770 cattrs-23.1.1/src/cattrs/dispatch.py
--rw-r--r--   0        0        0     3850 2023-04-15 23:55:47.836298 cattrs-23.1.1/src/cattrs/errors.py
--rw-r--r--   0        0        0    26575 2023-05-22 17:11:08.766741 cattrs-23.1.1/src/cattrs/gen/__init__.py
--rw-r--r--   0        0        0      490 2023-05-22 17:11:08.766741 cattrs-23.1.1/src/cattrs/gen/_consts.py
--rw-r--r--   0        0        0     1503 2023-05-22 17:11:08.766741 cattrs-23.1.1/src/cattrs/gen/_generics.py
--rw-r--r--   0        0        0     1017 2023-05-22 17:11:08.766741 cattrs-23.1.1/src/cattrs/gen/_lc.py
--rw-r--r--   0        0        0     1737 2023-05-22 17:11:08.770741 cattrs-23.1.1/src/cattrs/gen/_shared.py
--rw-r--r--   0        0        0    22059 2023-05-22 17:11:08.774741 cattrs-23.1.1/src/cattrs/gen/typeddicts.py
--rw-r--r--   0        0        0      165 2022-04-16 01:20:23.203198 cattrs-23.1.1/src/cattrs/preconf/__init__.py
--rw-r--r--   0        0        0     3087 2023-05-22 17:11:08.782741 cattrs-23.1.1/src/cattrs/preconf/bson.py
--rw-r--r--   0        0        0     1290 2023-05-22 17:11:08.786741 cattrs-23.1.1/src/cattrs/preconf/cbor2.py
--rw-r--r--   0        0        0     1615 2023-05-22 17:11:08.786741 cattrs-23.1.1/src/cattrs/preconf/json.py
--rw-r--r--   0        0        0     1302 2023-05-22 17:11:08.790742 cattrs-23.1.1/src/cattrs/preconf/msgpack.py
--rw-r--r--   0        0        0     2573 2023-05-22 17:11:08.798742 cattrs-23.1.1/src/cattrs/preconf/orjson.py
--rw-r--r--   0        0        0     1320 2023-05-22 17:11:08.798742 cattrs-23.1.1/src/cattrs/preconf/pyyaml.py
--rw-r--r--   0        0        0     2534 2023-05-22 17:11:08.802742 cattrs-23.1.1/src/cattrs/preconf/tomlkit.py
--rw-r--r--   0        0        0     1525 2023-05-22 17:11:08.806742 cattrs-23.1.1/src/cattrs/preconf/ujson.py
--rw-r--r--   0        0        0        0 2022-02-11 01:34:09.486876 cattrs-23.1.1/src/cattrs/py.typed
--rw-r--r--   0        0        0      192 2023-05-22 17:11:08.810742 cattrs-23.1.1/src/cattrs/strategies/__init__.py
--rw-r--r--   0        0        0     8677 2023-05-22 17:16:50.127698 cattrs-23.1.1/src/cattrs/strategies/_subclasses.py
--rw-r--r--   0        0        0     3440 2023-05-22 17:11:08.814742 cattrs-23.1.1/src/cattrs/strategies/_unions.py
--rw-r--r--   0        0        0     4360 2023-05-22 17:11:08.814742 cattrs-23.1.1/src/cattrs/v.py
--rw-r--r--   0        0        0     9250 1970-01-01 00:00:00.000000 cattrs-23.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-02-11 01:34:09.478875 cattrs-23.1.2/LICENSE
+-rw-r--r--   0        0        0     7516 2023-04-15 23:55:47.832298 cattrs-23.1.2/README.md
+-rw-r--r--   0        0        0     2456 2023-06-02 00:15:43.263152 cattrs-23.1.2/pyproject.toml
+-rw-r--r--   0        0        0      906 2022-04-16 01:20:23.203198 cattrs-23.1.2/src/cattr/__init__.py
+-rw-r--r--   0        0        0      192 2022-04-16 01:20:23.203198 cattrs-23.1.2/src/cattr/converters.py
+-rw-r--r--   0        0        0      103 2022-04-16 01:20:23.203198 cattrs-23.1.2/src/cattr/disambiguators.py
+-rw-r--r--   0        0        0      125 2022-04-16 01:20:23.203198 cattrs-23.1.2/src/cattr/dispatch.py
+-rw-r--r--   0        0        0      343 2022-07-06 00:23:52.229650 cattrs-23.1.2/src/cattr/errors.py
+-rw-r--r--   0        0        0      520 2022-02-11 01:34:09.486876 cattrs-23.1.2/src/cattr/gen.py
+-rw-r--r--   0        0        0       78 2022-04-16 01:20:23.203198 cattrs-23.1.2/src/cattr/preconf/__init__.py
+-rw-r--r--   0        0        0      194 2023-03-02 01:10:10.360770 cattrs-23.1.2/src/cattr/preconf/bson.py
+-rw-r--r--   0        0        0      205 2023-03-02 01:10:10.360770 cattrs-23.1.2/src/cattr/preconf/json.py
+-rw-r--r--   0        0        0      206 2023-03-02 01:10:10.360770 cattrs-23.1.2/src/cattr/preconf/msgpack.py
+-rw-r--r--   0        0        0      202 2023-03-02 01:10:10.360770 cattrs-23.1.2/src/cattr/preconf/orjson.py
+-rw-r--r--   0        0        0      202 2023-03-02 01:10:10.360770 cattrs-23.1.2/src/cattr/preconf/pyyaml.py
+-rw-r--r--   0        0        0      206 2023-03-02 01:10:10.360770 cattrs-23.1.2/src/cattr/preconf/tomlkit.py
+-rw-r--r--   0        0        0      198 2023-03-02 01:10:10.360770 cattrs-23.1.2/src/cattr/preconf/ujson.py
+-rw-r--r--   0        0        0        0 2022-02-11 01:34:09.486876 cattrs-23.1.2/src/cattr/py.typed
+-rw-r--r--   0        0        0     1631 2023-04-15 23:55:47.836298 cattrs-23.1.2/src/cattrs/__init__.py
+-rw-r--r--   0        0        0    15501 2023-05-23 23:14:04.606233 cattrs-23.1.2/src/cattrs/_compat.py
+-rw-r--r--   0        0        0      678 2022-04-10 01:46:50.855243 cattrs-23.1.2/src/cattrs/_generics.py
+-rw-r--r--   0        0        0    41450 2023-06-02 00:07:38.976973 cattrs-23.1.2/src/cattrs/converters.py
+-rw-r--r--   0        0        0     2243 2023-03-02 01:10:10.360770 cattrs-23.1.2/src/cattrs/disambiguators.py
+-rw-r--r--   0        0        0     4654 2023-03-02 01:10:10.360770 cattrs-23.1.2/src/cattrs/dispatch.py
+-rw-r--r--   0        0        0     3850 2023-06-02 00:07:38.976973 cattrs-23.1.2/src/cattrs/errors.py
+-rw-r--r--   0        0        0    26575 2023-06-02 00:07:38.976973 cattrs-23.1.2/src/cattrs/gen/__init__.py
+-rw-r--r--   0        0        0      490 2023-05-22 17:11:08.766741 cattrs-23.1.2/src/cattrs/gen/_consts.py
+-rw-r--r--   0        0        0     1503 2023-05-22 17:11:08.766741 cattrs-23.1.2/src/cattrs/gen/_generics.py
+-rw-r--r--   0        0        0     1017 2023-05-22 17:11:08.766741 cattrs-23.1.2/src/cattrs/gen/_lc.py
+-rw-r--r--   0        0        0     1737 2023-05-22 17:11:08.770741 cattrs-23.1.2/src/cattrs/gen/_shared.py
+-rw-r--r--   0        0        0    22059 2023-06-02 00:07:38.976973 cattrs-23.1.2/src/cattrs/gen/typeddicts.py
+-rw-r--r--   0        0        0      165 2022-04-16 01:20:23.203198 cattrs-23.1.2/src/cattrs/preconf/__init__.py
+-rw-r--r--   0        0        0     3087 2023-05-22 17:11:08.782741 cattrs-23.1.2/src/cattrs/preconf/bson.py
+-rw-r--r--   0        0        0     1290 2023-05-22 17:11:08.786741 cattrs-23.1.2/src/cattrs/preconf/cbor2.py
+-rw-r--r--   0        0        0     1615 2023-05-22 17:11:08.786741 cattrs-23.1.2/src/cattrs/preconf/json.py
+-rw-r--r--   0        0        0     1302 2023-05-22 17:11:08.790742 cattrs-23.1.2/src/cattrs/preconf/msgpack.py
+-rw-r--r--   0        0        0     2573 2023-05-22 17:11:08.798742 cattrs-23.1.2/src/cattrs/preconf/orjson.py
+-rw-r--r--   0        0        0     1320 2023-05-22 17:11:08.798742 cattrs-23.1.2/src/cattrs/preconf/pyyaml.py
+-rw-r--r--   0        0        0     2534 2023-05-22 17:11:08.802742 cattrs-23.1.2/src/cattrs/preconf/tomlkit.py
+-rw-r--r--   0        0        0     1525 2023-05-22 17:11:08.806742 cattrs-23.1.2/src/cattrs/preconf/ujson.py
+-rw-r--r--   0        0        0        0 2022-02-11 01:34:09.486876 cattrs-23.1.2/src/cattrs/py.typed
+-rw-r--r--   0        0        0      192 2023-05-22 17:11:08.810742 cattrs-23.1.2/src/cattrs/strategies/__init__.py
+-rw-r--r--   0        0        0     8677 2023-06-02 00:07:38.976973 cattrs-23.1.2/src/cattrs/strategies/_subclasses.py
+-rw-r--r--   0        0        0     3440 2023-05-22 17:11:08.814742 cattrs-23.1.2/src/cattrs/strategies/_unions.py
+-rw-r--r--   0        0        0     4360 2023-06-02 00:07:38.976973 cattrs-23.1.2/src/cattrs/v.py
+-rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 cattrs-23.1.2/PKG-INFO
```

### Comparing `cattrs-23.1.1/LICENSE` & `cattrs-23.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/README.md` & `cattrs-23.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/pyproject.toml` & `cattrs-23.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [tool.isort]
 profile = "black"
 known_first_party = ["cattr"]
 
 [tool.poetry]
 name = "cattrs"
-version = "23.1.1"
+version = "23.1.2"
 description = "Composable complex class support for attrs and dataclasses."
 authors = ["Tin Tvrtkovic <tinchester@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/python-attrs/cattrs"
 documentation = "https://catt.rs/en/stable/"
 keywords = ["attrs", "serialization", "dataclasses"]
 packages = [
@@ -19,15 +19,15 @@
     { include = "cattrs", from = "src" },
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 attrs = ">= 20"
-typing_extensions = { version = "*", python = "< 3.11" }
+typing_extensions = { version = ">=4.1.0", python = "< 3.11" }
 exceptiongroup = { version = "*", python = "< 3.11" }
 ujson = { version = "^5.4.0", optional = true }
 orjson = { version = "^3.5.2", markers = "implementation_name == 'cpython'", optional = true }
 msgpack = { version = "^1.0.2", optional = true }
 PyYAML = { version = "^6.0", optional = true }
 tomlkit = { version = "^0.11.4", python = "<4", optional = true }
 cbor2 = { version = "^5.4.6", optional = true }
```

### Comparing `cattrs-23.1.1/src/cattr/__init__.py` & `cattrs-23.1.2/src/cattr/__init__.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattr/gen.py` & `cattrs-23.1.2/src/cattr/gen.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/__init__.py` & `cattrs-23.1.2/src/cattrs/__init__.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/_compat.py` & `cattrs-23.1.2/src/cattrs/_compat.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/_generics.py` & `cattrs-23.1.2/src/cattrs/_generics.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/converters.py` & `cattrs-23.1.2/src/cattrs/converters.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/disambiguators.py` & `cattrs-23.1.2/src/cattrs/disambiguators.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/dispatch.py` & `cattrs-23.1.2/src/cattrs/dispatch.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/errors.py` & `cattrs-23.1.2/src/cattrs/errors.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/gen/__init__.py` & `cattrs-23.1.2/src/cattrs/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/gen/_generics.py` & `cattrs-23.1.2/src/cattrs/gen/_generics.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/gen/_lc.py` & `cattrs-23.1.2/src/cattrs/gen/_lc.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/gen/_shared.py` & `cattrs-23.1.2/src/cattrs/gen/_shared.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/gen/typeddicts.py` & `cattrs-23.1.2/src/cattrs/gen/typeddicts.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/preconf/bson.py` & `cattrs-23.1.2/src/cattrs/preconf/bson.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/preconf/cbor2.py` & `cattrs-23.1.2/src/cattrs/preconf/cbor2.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/preconf/json.py` & `cattrs-23.1.2/src/cattrs/preconf/json.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/preconf/msgpack.py` & `cattrs-23.1.2/src/cattrs/preconf/msgpack.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/preconf/orjson.py` & `cattrs-23.1.2/src/cattrs/preconf/orjson.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/preconf/pyyaml.py` & `cattrs-23.1.2/src/cattrs/preconf/pyyaml.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/preconf/tomlkit.py` & `cattrs-23.1.2/src/cattrs/preconf/tomlkit.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/preconf/ujson.py` & `cattrs-23.1.2/src/cattrs/preconf/ujson.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/strategies/_subclasses.py` & `cattrs-23.1.2/src/cattrs/strategies/_subclasses.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/strategies/_unions.py` & `cattrs-23.1.2/src/cattrs/strategies/_unions.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/src/cattrs/v.py` & `cattrs-23.1.2/src/cattrs/v.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.1/PKG-INFO` & `cattrs-23.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cattrs
-Version: 23.1.1
+Version: 23.1.2
 Summary: Composable complex class support for attrs and dataclasses.
 Home-page: https://github.com/python-attrs/cattrs
 License: MIT
 Keywords: attrs,serialization,dataclasses
 Author: Tin Tvrtkovic
 Author-email: tinchester@gmail.com
 Requires-Python: >=3.7
@@ -26,15 +26,15 @@
 Requires-Dist: attrs (>=20)
 Requires-Dist: cbor2 (>=5.4.6,<6.0.0) ; extra == "cbor2"
 Requires-Dist: exceptiongroup ; python_version < "3.11"
 Requires-Dist: msgpack (>=1.0.2,<2.0.0) ; extra == "msgpack"
 Requires-Dist: orjson (>=3.5.2,<4.0.0) ; (implementation_name == "cpython") and (extra == "orjson")
 Requires-Dist: pymongo (>=4.2.0,<5.0.0) ; extra == "bson"
 Requires-Dist: tomlkit (>=0.11.4,<0.12.0) ; (python_version < "4") and (extra == "tomlkit")
-Requires-Dist: typing_extensions ; python_version < "3.11"
+Requires-Dist: typing_extensions (>=4.1.0) ; python_version < "3.11"
 Requires-Dist: ujson (>=5.4.0,<6.0.0) ; extra == "ujson"
 Project-URL: Bug Tracker, https://github.com/python-attrs/cattrs/issues
 Project-URL: Changelog, https://catt.rs/en/latest/history.html
 Project-URL: Documentation, https://catt.rs/en/stable/
 Project-URL: Repository, https://github.com/python-attrs/cattrs
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cattrs Version: 23.1.1 Summary: Composable complex
+Metadata-Version: 2.1 Name: cattrs Version: 23.1.2 Summary: Composable complex
 class support for attrs and dataclasses. Home-page: https://github.com/python-
 attrs/cattrs License: MIT Keywords: attrs,serialization,dataclasses Author: Tin
 Tvrtkovic Author-email: tinchester@gmail.com Requires-Python: >=3.7 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -11,57 +11,57 @@
 Provides-Extra: tomlkit Provides-Extra: ujson Requires-Dist: PyYAML
 (>=6.0,<7.0) ; extra == "pyyaml" Requires-Dist: attrs (>=20) Requires-Dist:
 cbor2 (>=5.4.6,<6.0.0) ; extra == "cbor2" Requires-Dist: exceptiongroup ;
 python_version < "3.11" Requires-Dist: msgpack (>=1.0.2,<2.0.0) ; extra ==
 "msgpack" Requires-Dist: orjson (>=3.5.2,<4.0.0) ; (implementation_name ==
 "cpython") and (extra == "orjson") Requires-Dist: pymongo (>=4.2.0,<5.0.0) ;
 extra == "bson" Requires-Dist: tomlkit (>=0.11.4,<0.12.0) ; (python_version <
-"4") and (extra == "tomlkit") Requires-Dist: typing_extensions ; python_version
-< "3.11" Requires-Dist: ujson (>=5.4.0,<6.0.0) ; extra == "ujson" Project-URL:
-Bug Tracker, https://github.com/python-attrs/cattrs/issues Project-URL:
-Changelog, https://catt.rs/en/latest/history.html Project-URL: Documentation,
-https://catt.rs/en/stable/ Project-URL: Repository, https://github.com/python-
-attrs/cattrs Description-Content-Type: text/markdown # cattrs [https://
-img.shields.io/pypi/v/cattrs.svg] [https://github.com/python-attrs/cattrs/
-workflows/CI/badge.svg] [Documentation_Status] [Supported_Python_versions]
-[https://codecov.io/gh/python-attrs/cattrs/branch/master/graph/badge.svg]
-[https://img.shields.io/badge/code%20style-black-000000.svg] --- **cattrs** is
-an open source Python library for structuring and unstructuring data. _cattrs_
-works best with _attrs_ classes, dataclasses and the usual Python collections,
-but other kinds of classes are supported by manually registering converters.
-Python has a rich set of powerful, easy to use, built-in data types like
-dictionaries, lists and tuples. These data types are also the lingua franca of
-most data serialization libraries, for formats like json, msgpack, cbor, yaml
-or toml. Data types like this, and mappings like `dict` s in particular,
-represent unstructured data. Your data is, in all likelihood, structured: not
-all combinations of field names or values are valid inputs to your programs. In
-Python, structured data is better represented with classes and enumerations.
-_attrs_ is an excellent library for declaratively describing the structure of
-your data, and validating it. When you're handed unstructured data (by your
-network, file system, database...), _cattrs_ helps to convert this data into
-structured data. When you have to convert your structured data into data types
-other libraries can handle, _cattrs_ turns your classes and enumerations into
-dictionaries, integers and strings. Here's a simple taste. The list containing
-a float, an int and a string gets converted into a tuple of three ints.
-```python >>> import cattrs >>> cattrs.structure([1.0, 2, "3"], tuple[int, int,
-int]) (1, 2, 3) ``` _cattrs_ works well with _attrs_ classes out of the box.
-```python >>> from attrs import frozen >>> import cattrs >>> @frozen # It works
-with non-frozen classes too. ... class C: ... a: int ... b: str >>> instance =
-C(1, 'a') >>> cattrs.unstructure(instance) {'a': 1, 'b': 'a'} >>>
-cattrs.structure({'a': 1, 'b': 'a'}, C) C(a=1, b='a') ``` Here's a much more
-complex example, involving `attrs` classes with type metadata. ```python >>>
-from enum import unique, Enum >>> from typing import Optional, Sequence, Union
->>> from cattrs import structure, unstructure >>> from attrs import define,
-field >>> @unique ... class CatBreed(Enum): ... SIAMESE = "siamese" ...
-MAINE_COON = "maine_coon" ... SACRED_BIRMAN = "birman" >>> @define ... class
-Cat: ... breed: CatBreed ... names: Sequence[str] >>> @define ... class
-DogMicrochip: ... chip_id = field() # Type annotations are optional, but
-recommended ... time_chipped: float = field() >>> @define ... class Dog: ...
-cuteness: int ... chip: Optional[DogMicrochip] = None >>> p = unstructure([Dog
-(cuteness=1, chip=DogMicrochip(chip_id=1, time_chipped=10.0)), ... Cat
+"4") and (extra == "tomlkit") Requires-Dist: typing_extensions (>=4.1.0) ;
+python_version < "3.11" Requires-Dist: ujson (>=5.4.0,<6.0.0) ; extra ==
+"ujson" Project-URL: Bug Tracker, https://github.com/python-attrs/cattrs/issues
+Project-URL: Changelog, https://catt.rs/en/latest/history.html Project-URL:
+Documentation, https://catt.rs/en/stable/ Project-URL: Repository, https://
+github.com/python-attrs/cattrs Description-Content-Type: text/markdown # cattrs
+[https://img.shields.io/pypi/v/cattrs.svg] [https://github.com/python-attrs/
+cattrs/workflows/CI/badge.svg] [Documentation_Status] [Supported_Python
+versions] [https://codecov.io/gh/python-attrs/cattrs/branch/master/graph/
+badge.svg] [https://img.shields.io/badge/code%20style-black-000000.svg] --
+- **cattrs** is an open source Python library for structuring and unstructuring
+data. _cattrs_ works best with _attrs_ classes, dataclasses and the usual
+Python collections, but other kinds of classes are supported by manually
+registering converters. Python has a rich set of powerful, easy to use, built-
+in data types like dictionaries, lists and tuples. These data types are also
+the lingua franca of most data serialization libraries, for formats like json,
+msgpack, cbor, yaml or toml. Data types like this, and mappings like `dict` s
+in particular, represent unstructured data. Your data is, in all likelihood,
+structured: not all combinations of field names or values are valid inputs to
+your programs. In Python, structured data is better represented with classes
+and enumerations. _attrs_ is an excellent library for declaratively describing
+the structure of your data, and validating it. When you're handed unstructured
+data (by your network, file system, database...), _cattrs_ helps to convert
+this data into structured data. When you have to convert your structured data
+into data types other libraries can handle, _cattrs_ turns your classes and
+enumerations into dictionaries, integers and strings. Here's a simple taste.
+The list containing a float, an int and a string gets converted into a tuple of
+three ints. ```python >>> import cattrs >>> cattrs.structure([1.0, 2, "3"],
+tuple[int, int, int]) (1, 2, 3) ``` _cattrs_ works well with _attrs_ classes
+out of the box. ```python >>> from attrs import frozen >>> import cattrs >>>
+@frozen # It works with non-frozen classes too. ... class C: ... a: int ... b:
+str >>> instance = C(1, 'a') >>> cattrs.unstructure(instance) {'a': 1, 'b':
+'a'} >>> cattrs.structure({'a': 1, 'b': 'a'}, C) C(a=1, b='a') ``` Here's a
+much more complex example, involving `attrs` classes with type metadata.
+```python >>> from enum import unique, Enum >>> from typing import Optional,
+Sequence, Union >>> from cattrs import structure, unstructure >>> from attrs
+import define, field >>> @unique ... class CatBreed(Enum): ... SIAMESE =
+"siamese" ... MAINE_COON = "maine_coon" ... SACRED_BIRMAN = "birman" >>>
+@define ... class Cat: ... breed: CatBreed ... names: Sequence[str] >>> @define
+... class DogMicrochip: ... chip_id = field() # Type annotations are optional,
+but recommended ... time_chipped: float = field() >>> @define ... class Dog:
+... cuteness: int ... chip: Optional[DogMicrochip] = None >>> p = unstructure(
+[Dog(cuteness=1, chip=DogMicrochip(chip_id=1, time_chipped=10.0)), ... Cat
 (breed=CatBreed.MAINE_COON, names=('Fluffly', 'Fluffer'))]) >>> print(p) [
 {'cuteness': 1, 'chip': {'chip_id': 1, 'time_chipped': 10.0}}, {'breed':
 'maine_coon', 'names': ('Fluffly', 'Fluffer')}] >>> print(structure(p, list
 [Union[Dog, Cat]])) [Dog(cuteness=1, chip=DogMicrochip(chip_id=1,
 time_chipped=10.0)), Cat(breed=
 MAINE_COON: 'maine_coon'>, names=['Fluffly', 'Fluffer'])] ``` Consider
 unstructured data a low-level representation that needs to be converted to
```

