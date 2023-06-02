# Comparing `tmp/ramqp-8.4.0.tar.gz` & `tmp/ramqp-8.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-8.4.0.tar", max compression
+gzip compressed data, was "ramqp-8.4.1.tar", max compression
```

## Comparing `ramqp-8.4.0.tar` & `ramqp-8.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-05-22 14:48:16.191417 ramqp-8.4.0/LICENSES/
--rw-r--r--   0        0        0    15177 2023-05-22 14:48:16.191417 ramqp-8.4.0/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-05-22 14:48:16.192417 ramqp-8.4.0/README.md
--rw-r--r--   0        0        0     1460 2023-05-22 14:48:28.848330 ramqp-8.4.0/pyproject.toml
--rw-r--r--   0        0        0      321 2023-05-22 14:48:16.194417 ramqp-8.4.0/ramqp/__init__.py
--rw-r--r--   0        0        0    16392 2023-05-22 14:48:16.194417 ramqp-8.4.0/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-05-22 14:48:16.194417 ramqp-8.4.0/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-05-22 14:48:16.194417 ramqp-8.4.0/ramqp/config.py
--rw-r--r--   0        0        0    10021 2023-05-22 14:48:16.195417 ramqp-8.4.0/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-05-22 14:48:16.195417 ramqp-8.4.0/ramqp/metrics.py
--rw-r--r--   0        0        0     8652 2023-05-22 14:48:16.195417 ramqp-8.4.0/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-05-22 14:48:16.253421 ramqp-8.4.0/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-05-22 14:48:16.196417 ramqp-8.4.0/ramqp/utils.py
--rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.4.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-06-02 12:49:17.671696 ramqp-8.4.1/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-06-02 12:49:17.671696 ramqp-8.4.1/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-06-02 12:49:17.671696 ramqp-8.4.1/README.md
+-rw-r--r--   0        0        0     1460 2023-06-02 12:49:39.984673 ramqp-8.4.1/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-06-02 12:49:17.685697 ramqp-8.4.1/ramqp/__init__.py
+-rw-r--r--   0        0        0    16392 2023-06-02 12:49:17.686698 ramqp-8.4.1/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-06-02 12:49:17.686698 ramqp-8.4.1/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-06-02 12:49:17.686698 ramqp-8.4.1/ramqp/config.py
+-rw-r--r--   0        0        0    10021 2023-06-02 12:49:17.686698 ramqp-8.4.1/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-06-02 12:49:17.686698 ramqp-8.4.1/ramqp/metrics.py
+-rw-r--r--   0        0        0     8652 2023-06-02 12:49:17.687698 ramqp-8.4.1/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-06-02 12:49:17.851712 ramqp-8.4.1/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-06-02 12:49:17.687698 ramqp-8.4.1/ramqp/utils.py
+-rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.4.1/PKG-INFO
```

### Comparing `ramqp-8.4.0/LICENSES/MPL-2.0.txt` & `ramqp-8.4.1/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.0/README.md` & `ramqp-8.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.0/pyproject.toml` & `ramqp-8.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramqp"
-version = "8.4.0"
+version = "8.4.1"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
```

### Comparing `ramqp-8.4.0/ramqp/abstract.py` & `ramqp-8.4.1/ramqp/abstract.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.0/ramqp/amqp.py` & `ramqp-8.4.1/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.0/ramqp/config.py` & `ramqp-8.4.1/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.0/ramqp/depends.py` & `ramqp-8.4.1/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.0/ramqp/metrics.py` & `ramqp-8.4.1/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.0/ramqp/mo.py` & `ramqp-8.4.1/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.0/ramqp/utils.py` & `ramqp-8.4.1/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.0/PKG-INFO` & `ramqp-8.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 8.4.0
+Version: 8.4.1
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

