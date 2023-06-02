# Comparing `tmp/kiwi_cogs-0.1.0.tar.gz` & `tmp/kiwi_cogs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwi_cogs-0.1.0.tar", max compression
+gzip compressed data, was "kiwi_cogs-0.1.1.tar", max compression
```

## Comparing `kiwi_cogs-0.1.0.tar` & `kiwi_cogs-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-06-01 21:09:32.501623 kiwi_cogs-0.1.0/LICENSE
--rw-r--r--   0        0        0     5738 2023-06-01 21:09:32.501623 kiwi_cogs-0.1.0/README.md
--rw-r--r--   0        0        0      169 2023-06-01 21:09:32.501623 kiwi_cogs-0.1.0/kiwi_cogs/__init__.py
--rw-r--r--   0        0        0     2528 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/event.py
--rw-r--r--   0        0        0      210 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/exceptions.py
--rw-r--r--   0        0        0     7700 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/machine.py
--rw-r--r--   0        0        0    10253 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/state.py
--rw-r--r--   0        0        0     4098 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/transition.py
--rw-r--r--   0        0        0      465 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/utils.py
--rw-r--r--   0        0        0     2060 2023-06-01 21:09:52.445905 kiwi_cogs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6459 1970-01-01 00:00:00.000000 kiwi_cogs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6014 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/README.md
+-rw-r--r--   0        0        0      169 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/kiwi_cogs/__init__.py
+-rw-r--r--   0        0        0     2528 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/kiwi_cogs/event.py
+-rw-r--r--   0        0        0      210 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/kiwi_cogs/exceptions.py
+-rw-r--r--   0        0        0     7700 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/kiwi_cogs/machine.py
+-rw-r--r--   0        0        0    10253 2023-06-02 10:31:28.595719 kiwi_cogs-0.1.1/kiwi_cogs/state.py
+-rw-r--r--   0        0        0     4098 2023-06-02 10:31:28.595719 kiwi_cogs-0.1.1/kiwi_cogs/transition.py
+-rw-r--r--   0        0        0      465 2023-06-02 10:31:28.595719 kiwi_cogs-0.1.1/kiwi_cogs/utils.py
+-rw-r--r--   0        0        0     2061 2023-06-02 10:31:50.964050 kiwi_cogs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6735 1970-01-01 00:00:00.000000 kiwi_cogs-0.1.1/PKG-INFO
```

### Comparing `kiwi_cogs-0.1.0/LICENSE` & `kiwi_cogs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.1.0/README.md` & `kiwi_cogs-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # Kiwi Cogs
 
 <div align="center">
 
 [![Release](https://img.shields.io/github/v/release/mopeyjellyfish/KiwiCogs)](https://img.shields.io/github/v/release/mopeyjellyfish/KiwiCogs)
 [![Build](https://github.com/mopeyjellyfish/KiwiCogs/actions/workflows/main.yml/badge.svg)](https://github.com/mopeyjellyfish/KiwiCogs/actions/workflows/main.yml)
+[![Python Version](https://img.shields.io/pypi/pyversions/kiwi-cogs.svg)](https://pypi.org/project/kiwi-cogs)
 [![codecov](https://codecov.io/gh/mopeyjellyfish/KiwiCogs/branch/main/graph/badge.svg)](https://codecov.io/gh/mopeyjellyfish/KiwiCogs)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/mopeyjellyfish/KiwiCogs)](https://img.shields.io/github/commit-activity/m/mopeyjellyfish/KiwiCogs)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/mopeyjellyfish/KiwiCogs/blob/main/.pre-commit-config.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/mopeyjellyfish/KiwiCogs/releases)
 [![License](https://img.shields.io/github/license/mopeyjellyfish/KiwiCogs)](https://github.com/mopeyjellyfish/KiwiCogs/blob/main/LICENSE)
 
 </div>
 
 A simple and easy to use state machine library.
 
 - **Github repository**: <https://github.com/mopeyjellyfish/KiwiCogs/>
 - **Documentation** <https://mopeyjellyfish.github.io/KiwiCogs/>
 
-
 ## Installation
 
 ### Pip
 
 ```bash
 pip install -U kiwi-cogs
 ```
```

### Comparing `kiwi_cogs-0.1.0/kiwi_cogs/event.py` & `kiwi_cogs-0.1.1/kiwi_cogs/event.py`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.1.0/kiwi_cogs/machine.py` & `kiwi_cogs-0.1.1/kiwi_cogs/machine.py`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.1.0/kiwi_cogs/state.py` & `kiwi_cogs-0.1.1/kiwi_cogs/state.py`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.1.0/kiwi_cogs/transition.py` & `kiwi_cogs-0.1.1/kiwi_cogs/transition.py`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.1.0/pyproject.toml` & `kiwi_cogs-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kiwi_cogs"
-version = "0.1.0"
+version = "v0.1.1"
 description = "A simple and easy to use state machine library "
 authors = ["David Hall <fdev@davidhall.tech>"]
 repository = "https://github.com/mopeyjellyfish/kiwi-cogs"
 documentation = "https://mopeyjellyfish.github.io/kiwi-cogs/"
 readme = "README.md"
 packages = [
   {include = "kiwi_cogs"}
```

### Comparing `kiwi_cogs-0.1.0/PKG-INFO` & `kiwi_cogs-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwi-cogs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple and easy to use state machine library 
 Home-page: https://github.com/mopeyjellyfish/kiwi-cogs
 Author: David Hall
 Author-email: fdev@davidhall.tech
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -18,28 +18,29 @@
 
 # Kiwi Cogs
 
 <div align="center">
 
 [![Release](https://img.shields.io/github/v/release/mopeyjellyfish/KiwiCogs)](https://img.shields.io/github/v/release/mopeyjellyfish/KiwiCogs)
 [![Build](https://github.com/mopeyjellyfish/KiwiCogs/actions/workflows/main.yml/badge.svg)](https://github.com/mopeyjellyfish/KiwiCogs/actions/workflows/main.yml)
+[![Python Version](https://img.shields.io/pypi/pyversions/kiwi-cogs.svg)](https://pypi.org/project/kiwi-cogs)
 [![codecov](https://codecov.io/gh/mopeyjellyfish/KiwiCogs/branch/main/graph/badge.svg)](https://codecov.io/gh/mopeyjellyfish/KiwiCogs)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/mopeyjellyfish/KiwiCogs)](https://img.shields.io/github/commit-activity/m/mopeyjellyfish/KiwiCogs)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/mopeyjellyfish/KiwiCogs/blob/main/.pre-commit-config.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/mopeyjellyfish/KiwiCogs/releases)
 [![License](https://img.shields.io/github/license/mopeyjellyfish/KiwiCogs)](https://github.com/mopeyjellyfish/KiwiCogs/blob/main/LICENSE)
 
 </div>
 
 A simple and easy to use state machine library.
 
 - **Github repository**: <https://github.com/mopeyjellyfish/KiwiCogs/>
 - **Documentation** <https://mopeyjellyfish.github.io/KiwiCogs/>
 
-
 ## Installation
 
 ### Pip
 
 ```bash
 pip install -U kiwi-cogs
 ```
```

