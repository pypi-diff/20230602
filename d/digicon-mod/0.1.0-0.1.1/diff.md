# Comparing `tmp/digicon_mod-0.1.0.tar.gz` & `tmp/digicon_mod-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digicon_mod-0.1.0.tar", max compression
+gzip compressed data, was "digicon_mod-0.1.1.tar", max compression
```

## Comparing `digicon_mod-0.1.0.tar` & `digicon_mod-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-01 16:28:14.355409 digicon_mod-0.1.0/digicon_mod/__init__.py
--rw-r--r--   0        0        0      614 2023-06-01 17:50:52.045396 digicon_mod-0.1.0/digicon_mod/pid.py
--rw-r--r--   0        0        0     1056 2023-06-01 17:48:21.246507 digicon_mod-0.1.0/digicon_mod/plc.py
--rw-r--r--   0        0        0      901 2023-06-01 17:47:42.202484 digicon_mod-0.1.0/digicon_mod/sim.py
--rw-r--r--   0        0        0        0 2023-06-01 16:28:14.355409 digicon_mod-0.1.0/digicon_mod/test/__init__.py
--rw-r--r--   0        0        0      654 2023-06-01 18:55:23.371206 digicon_mod-0.1.0/digicon_mod/test/pid_control.py
--rw-r--r--   0        0        0    11357 2023-06-01 16:18:33.296904 digicon_mod-0.1.0/LICENSE
--rw-r--r--   0        0        0      571 2023-06-01 19:00:43.086091 digicon_mod-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      302 2023-06-01 16:18:33.296904 digicon_mod-0.1.0/README.md
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 digicon_mod-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-01 16:28:14.355409 digicon_mod-0.1.1/digicon_mod/__init__.py
+-rw-r--r--   0        0        0      614 2023-06-01 17:50:52.045396 digicon_mod-0.1.1/digicon_mod/pid.py
+-rw-r--r--   0        0        0     1056 2023-06-01 17:48:21.246507 digicon_mod-0.1.1/digicon_mod/plc.py
+-rw-r--r--   0        0        0      901 2023-06-01 17:47:42.202484 digicon_mod-0.1.1/digicon_mod/sim.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:28:14.355409 digicon_mod-0.1.1/digicon_mod/test/__init__.py
+-rw-r--r--   0        0        0      654 2023-06-01 18:55:23.371206 digicon_mod-0.1.1/digicon_mod/test/pid_control.py
+-rw-r--r--   0        0        0    11357 2023-06-01 16:18:33.296904 digicon_mod-0.1.1/LICENSE
+-rw-r--r--   0        0        0      572 2023-06-02 06:54:35.559802 digicon_mod-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      302 2023-06-01 16:18:33.296904 digicon_mod-0.1.1/README.md
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 digicon_mod-0.1.1/PKG-INFO
```

### Comparing `digicon_mod-0.1.0/digicon_mod/pid.py` & `digicon_mod-0.1.1/digicon_mod/pid.py`

 * *Files identical despite different names*

### Comparing `digicon_mod-0.1.0/digicon_mod/plc.py` & `digicon_mod-0.1.1/digicon_mod/plc.py`

 * *Files identical despite different names*

### Comparing `digicon_mod-0.1.0/digicon_mod/sim.py` & `digicon_mod-0.1.1/digicon_mod/sim.py`

 * *Files identical despite different names*

### Comparing `digicon_mod-0.1.0/digicon_mod/test/pid_control.py` & `digicon_mod-0.1.1/digicon_mod/test/pid_control.py`

 * *Files identical despite different names*

### Comparing `digicon_mod-0.1.0/LICENSE` & `digicon_mod-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `digicon_mod-0.1.0/pyproject.toml` & `digicon_mod-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "digicon_mod"
-version = "0.1.0"
-description = "Simple simulation tools for hybrid systems with digital control and continous process. See more details at https://github.com/ant-nik/digicon-mod"
+version = "0.1.1"
+description = "Simple simulation tools for hybrid systems with digital control and continous process. More details can be found at https://github.com/ant-nik/digicon-mod."
 authors = ["Anton Nikonov <ant.nik.nik@mail.ru>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "digicon_mod"}]
 
 [tool.poetry.dependencies]
-python = "3.11.1"
-numpy = "^1.24.3"
-scipy = "^1.10.1"
+python = "^3.9"
+numpy = "^1.23"
+scipy = "^1.9"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
+pytest = "^7.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `digicon_mod-0.1.0/PKG-INFO` & `digicon_mod-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: digicon-mod
-Version: 0.1.0
-Summary: Simple simulation tools for hybrid systems with digital control and continous process. See more details at https://github.com/ant-nik/digicon-mod
+Version: 0.1.1
+Summary: Simple simulation tools for hybrid systems with digital control and continous process. More details can be found at https://github.com/ant-nik/digicon-mod.
 License: Apache 2.0
 Author: Anton Nikonov
 Author-email: ant.nik.nik@mail.ru
-Requires-Python: ==3.11.1
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.23,<2.0)
+Requires-Dist: scipy (>=1.9,<2.0)
 Description-Content-Type: text/markdown
 
 # Digital control system modeling tools (digicon-mod)
 Simple implementation of hybrid continous and discrette closed-loop systems modeling tools based on ordinary differential equations solver (continous part of the system) and a custom python program with control logic (discrete part of the system).
```

