# Comparing `tmp/fastramqpi-1.4.2.tar.gz` & `tmp/fastramqpi-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-1.4.2.tar", max compression
+gzip compressed data, was "fastramqpi-1.4.3.tar", max compression
```

## Comparing `fastramqpi-1.4.2.tar` & `fastramqpi-1.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0        0        0        0 2023-05-22 06:56:22.561112 fastramqpi-1.4.2/LICENSES/
--rw-r--r--   0        0        0    15177 2023-05-22 06:56:22.561112 fastramqpi-1.4.2/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     2932 2023-05-22 06:56:22.561112 fastramqpi-1.4.2/README.md
--rw-r--r--   0        0        0       85 2023-05-22 06:56:22.562112 fastramqpi-1.4.2/fastramqpi/__init__.py
--rw-r--r--   0        0        0     2206 2023-05-22 06:56:22.562112 fastramqpi-1.4.2/fastramqpi/config.py
--rw-r--r--   0        0        0     1144 2023-05-22 06:56:22.562112 fastramqpi-1.4.2/fastramqpi/context.py
--rw-r--r--   0        0        0     7100 2023-05-22 06:56:22.562112 fastramqpi-1.4.2/fastramqpi/fastapi.py
--rw-r--r--   0        0        0     1577 2023-05-22 06:56:22.562112 fastramqpi-1.4.2/fastramqpi/healthcheck.py
--rw-r--r--   0        0        0     3930 2023-05-22 06:56:22.562112 fastramqpi-1.4.2/fastramqpi/main.py
--rw-r--r--   0        0        0        0 2023-05-22 06:56:22.605114 fastramqpi-1.4.2/fastramqpi/py.typed
--rw-r--r--   0        0        0     1390 2023-05-22 06:56:34.285863 fastramqpi-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 fastramqpi-1.4.2/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     2932 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/README.md
+-rw-r--r--   0        0        0       85 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     2206 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/fastramqpi/config.py
+-rw-r--r--   0        0        0     1144 2023-06-02 13:35:23.337033 fastramqpi-1.4.3/fastramqpi/context.py
+-rw-r--r--   0        0        0     7100 2023-06-02 13:35:23.337033 fastramqpi-1.4.3/fastramqpi/fastapi.py
+-rw-r--r--   0        0        0     1577 2023-06-02 13:35:23.337033 fastramqpi-1.4.3/fastramqpi/healthcheck.py
+-rw-r--r--   0        0        0     3930 2023-06-02 13:35:23.337033 fastramqpi-1.4.3/fastramqpi/main.py
+-rw-r--r--   0        0        0        0 2023-06-02 13:35:23.379037 fastramqpi-1.4.3/fastramqpi/py.typed
+-rw-r--r--   0        0        0     1390 2023-06-02 13:35:36.797252 fastramqpi-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 fastramqpi-1.4.3/PKG-INFO
```

### Comparing `fastramqpi-1.4.2/LICENSES/MPL-2.0.txt` & `fastramqpi-1.4.3/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.2/README.md` & `fastramqpi-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.2/fastramqpi/config.py` & `fastramqpi-1.4.3/fastramqpi/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.2/fastramqpi/context.py` & `fastramqpi-1.4.3/fastramqpi/context.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.2/fastramqpi/fastapi.py` & `fastramqpi-1.4.3/fastramqpi/fastapi.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.2/fastramqpi/healthcheck.py` & `fastramqpi-1.4.3/fastramqpi/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.2/fastramqpi/main.py` & `fastramqpi-1.4.3/fastramqpi/main.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.2/pyproject.toml` & `fastramqpi-1.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "1.4.2"
+version = "1.4.3"
 description = "Rammearkitektur AMQP framework (FastAPI + RAMQP)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo", "amqp"]
 packages = [ { include = "fastramqpi" } ]
 include = ["fastramqpi/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 structlog = "^23.1.0"
-ramqp = "^8.3.0"
+ramqp = "^9.0.0"
 pydantic = "^1.10.5"
 raclients = "^3.0.5"
 gql = "^3.4.0"
 more-itertools = "^9.1.0"
 ra-utils = "^1.12.2"
 prometheus-fastapi-instrumentator = ">=5.9.1,<7.0.0"
 fastapi = ">=0.93, <1.0"
```

### Comparing `fastramqpi-1.4.2/PKG-INFO` & `fastramqpi-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastramqpi
-Version: 1.4.2
+Version: 1.4.3
 Summary: Rammearkitektur AMQP framework (FastAPI + RAMQP)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
@@ -15,15 +15,15 @@
 Requires-Dist: fastapi (>=0.93,<1.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: prometheus-fastapi-instrumentator (>=5.9.1,<7.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: ra-utils (>=1.12.2,<2.0.0)
 Requires-Dist: raclients (>=3.0.5,<4.0.0)
-Requires-Dist: ramqp (>=8.3.0,<9.0.0)
+Requires-Dist: ramqp (>=9.0.0,<10.0.0)
 Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/FastRAMQPI
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2021 Magenta ApS <https://magenta.dk>
 SPDX-License-Identifier: MPL-2.0
```

