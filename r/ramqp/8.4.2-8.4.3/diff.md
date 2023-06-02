# Comparing `tmp/ramqp-8.4.2.tar.gz` & `tmp/ramqp-8.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-8.4.2.tar", max compression
+gzip compressed data, was "ramqp-8.4.3.tar", max compression
```

## Comparing `ramqp-8.4.2.tar` & `ramqp-8.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-06-02 12:52:44.157356 ramqp-8.4.2/LICENSES/
--rw-r--r--   0        0        0    15177 2023-06-02 12:52:44.157356 ramqp-8.4.2/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-06-02 12:52:44.157356 ramqp-8.4.2/README.md
--rw-r--r--   0        0        0     1460 2023-06-02 12:53:09.858684 ramqp-8.4.2/pyproject.toml
--rw-r--r--   0        0        0      321 2023-06-02 12:52:44.159356 ramqp-8.4.2/ramqp/__init__.py
--rw-r--r--   0        0        0    16392 2023-06-02 12:52:44.160356 ramqp-8.4.2/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-06-02 12:52:44.160356 ramqp-8.4.2/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-06-02 12:52:44.160356 ramqp-8.4.2/ramqp/config.py
--rw-r--r--   0        0        0    10021 2023-06-02 12:52:44.160356 ramqp-8.4.2/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-06-02 12:52:44.161356 ramqp-8.4.2/ramqp/metrics.py
--rw-r--r--   0        0        0     8652 2023-06-02 12:52:44.161356 ramqp-8.4.2/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-06-02 12:52:44.331372 ramqp-8.4.2/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-06-02 12:52:44.161356 ramqp-8.4.2/ramqp/utils.py
--rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.4.2/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-06-02 12:57:26.499595 ramqp-8.4.3/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-06-02 12:57:26.499595 ramqp-8.4.3/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-06-02 12:57:26.499595 ramqp-8.4.3/README.md
+-rw-r--r--   0        0        0     1465 2023-06-02 12:57:38.331385 ramqp-8.4.3/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-06-02 12:57:26.501595 ramqp-8.4.3/ramqp/__init__.py
+-rw-r--r--   0        0        0    16392 2023-06-02 12:57:26.502595 ramqp-8.4.3/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-06-02 12:57:26.502595 ramqp-8.4.3/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-06-02 12:57:26.503595 ramqp-8.4.3/ramqp/config.py
+-rw-r--r--   0        0        0    10021 2023-06-02 12:57:26.503595 ramqp-8.4.3/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-06-02 12:57:26.503595 ramqp-8.4.3/ramqp/metrics.py
+-rw-r--r--   0        0        0     8652 2023-06-02 12:57:26.504595 ramqp-8.4.3/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-06-02 12:57:26.547598 ramqp-8.4.3/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-06-02 12:57:26.504595 ramqp-8.4.3/ramqp/utils.py
+-rw-r--r--   0        0        0     8357 1970-01-01 00:00:00.000000 ramqp-8.4.3/PKG-INFO
```

### Comparing `ramqp-8.4.2/LICENSES/MPL-2.0.txt` & `ramqp-8.4.3/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.2/README.md` & `ramqp-8.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.2/pyproject.toml` & `ramqp-8.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "ramqp"
-version = "8.4.2"
+version = "8.4.3"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
 packages = [ { include = "ramqp" } ]
 include = ["ramqp/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aio-pika = ">=8.3,<10.0"
 structlog = "^23.1.0"
-prometheus-client = "^0.16.0"
+prometheus-client = ">=0.16,<0.18"
 pydantic = "^1.10.5"
 more-itertools = "^9.1.0"
 fastapi = ">=0.95.0,<1.0"
 anyio = "^3.6.2"
 ra-utils = "^1.12.4"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `ramqp-8.4.2/ramqp/abstract.py` & `ramqp-8.4.3/ramqp/abstract.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.2/ramqp/amqp.py` & `ramqp-8.4.3/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.2/ramqp/config.py` & `ramqp-8.4.3/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.2/ramqp/depends.py` & `ramqp-8.4.3/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.2/ramqp/metrics.py` & `ramqp-8.4.3/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.2/ramqp/mo.py` & `ramqp-8.4.3/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.2/ramqp/utils.py` & `ramqp-8.4.3/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.2/PKG-INFO` & `ramqp-8.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 8.4.2
+Version: 8.4.3
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aio-pika (>=8.3,<10.0)
 Requires-Dist: anyio (>=3.6.2,<4.0.0)
 Requires-Dist: fastapi (>=0.95.0,<1.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
-Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
+Requires-Dist: prometheus-client (>=0.16,<0.18)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: ra-utils (>=1.12.4,<2.0.0)
 Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/ramqp
 Description-Content-Type: text/markdown
 
 <!--
```

