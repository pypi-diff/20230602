# Comparing `tmp/patchwork-core-0.1.6.tar.gz` & `tmp/patchwork-core-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/patchwork-core-0.1.6.tar", last modified: Sat Dec  3 17:14:38 2022, max compression
+gzip compressed data, was "dist/patchwork-core-0.1.7.tar", last modified: Fri Jun  2 15:27:53 2023, max compression
```

## Comparing `patchwork-core-0.1.6.tar` & `patchwork-core-0.1.7.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1284 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      571 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork/core/
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork/core/client/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14216 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/client/base.py
--rw-rw-rw-   0 root         (0) root         (0)    11601 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/client/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork/core/client/serializers/
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/client/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/client/serializers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4448 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/client/serializers/betterproto.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/client/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7208 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/component.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork/core/config/
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4254 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/config/base.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/config/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork/core/proto/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/proto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork/core/proto/google/
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/proto/google/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70859 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/proto/google/protobuf.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/proto/task.py
--rw-rw-rw-   0 root         (0) root         (0)     5124 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/pydantic.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     5192 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     6680 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/patchwork/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1284 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/patchwork_core.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      342 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/scripts/compile-protoc.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1649 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 17:14:38.000000 patchwork-core-0.1.6/tests/core/
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/tests/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/tests/core/test_classpath.py
--rw-rw-rw-   0 root         (0) root         (0)     4052 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/tests/core/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/tests/core/test_component.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/tests/core/test_fnpath.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2022-12-03 17:14:25.000000 patchwork-core-0.1.6/tests/core/test_pydantic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork/core/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork/core/client/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14216 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/client/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11601 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/client/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork/core/client/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/client/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/client/serializers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4448 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/client/serializers/betterproto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/client/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7208 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/component.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork/core/config/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4254 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/config/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/config/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork/core/proto/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/proto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork/core/proto/google/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/proto/google/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70859 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/proto/google/protobuf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/proto/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     5124 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/pydantic.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork/core/stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/stubs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/stubs/prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)     5192 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     6680 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/patchwork/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork_core.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/patchwork_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/scripts/compile-protoc.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:27:53.000000 patchwork-core-0.1.7/tests/core/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/tests/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/tests/core/test_classpath.py
+-rw-rw-rw-   0 root         (0) root         (0)     4052 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/tests/core/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/tests/core/test_component.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/tests/core/test_fnpath.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-06-02 15:27:42.000000 patchwork-core-0.1.7/tests/core/test_pydantic.py
```

### Comparing `patchwork-core-0.1.6/LICENSE` & `patchwork-core-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/PKG-INFO` & `patchwork-core-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-core
-Version: 0.1.6
+Version: 0.1.7
 Summary: Core of the Patchwork Framework - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-core-0.1.6/README.md` & `patchwork-core-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/client/base.py` & `patchwork-core-0.1.7/patchwork/core/client/base.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/client/local.py` & `patchwork-core-0.1.7/patchwork/core/client/local.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/client/serializers/betterproto.py` & `patchwork-core-0.1.7/patchwork/core/client/serializers/betterproto.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/client/task.py` & `patchwork-core-0.1.7/patchwork/core/client/task.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/component.py` & `patchwork-core-0.1.7/patchwork/core/component.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/config/base.py` & `patchwork-core-0.1.7/patchwork/core/config/base.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/proto/google/protobuf.py` & `patchwork-core-0.1.7/patchwork/core/proto/google/protobuf.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/proto/task.py` & `patchwork-core-0.1.7/patchwork/core/proto/task.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/pydantic.py` & `patchwork-core-0.1.7/patchwork/core/pydantic.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/serializers.py` & `patchwork-core-0.1.7/patchwork/core/serializers.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/typing.py` & `patchwork-core-0.1.7/patchwork/core/typing.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork/core/utils.py` & `patchwork-core-0.1.7/patchwork/core/utils.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/patchwork_core.egg-info/PKG-INFO` & `patchwork-core-0.1.7/patchwork_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-core
-Version: 0.1.6
+Version: 0.1.7
 Summary: Core of the Patchwork Framework - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-core-0.1.6/patchwork_core.egg-info/SOURCES.txt` & `patchwork-core-0.1.7/patchwork_core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 patchwork/core/config/__init__.py
 patchwork/core/config/base.py
 patchwork/core/config/providers.py
 patchwork/core/proto/__init__.py
 patchwork/core/proto/task.py
 patchwork/core/proto/google/__init__.py
 patchwork/core/proto/google/protobuf.py
+patchwork/core/stubs/__init__.py
+patchwork/core/stubs/prometheus.py
 patchwork_core.egg-info/PKG-INFO
 patchwork_core.egg-info/SOURCES.txt
 patchwork_core.egg-info/dependency_links.txt
 patchwork_core.egg-info/not-zip-safe
 patchwork_core.egg-info/requires.txt
 patchwork_core.egg-info/top_level.txt
 scripts/compile-protoc.py
```

### Comparing `patchwork-core-0.1.6/setup.py` & `patchwork-core-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/tests/core/test_classpath.py` & `patchwork-core-0.1.7/tests/core/test_classpath.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/tests/core/test_client.py` & `patchwork-core-0.1.7/tests/core/test_client.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/tests/core/test_component.py` & `patchwork-core-0.1.7/tests/core/test_component.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/tests/core/test_fnpath.py` & `patchwork-core-0.1.7/tests/core/test_fnpath.py`

 * *Files identical despite different names*

### Comparing `patchwork-core-0.1.6/tests/core/test_pydantic.py` & `patchwork-core-0.1.7/tests/core/test_pydantic.py`

 * *Files identical despite different names*

