# Comparing `tmp/patchwork-node-0.1.2.tar.gz` & `tmp/patchwork-node-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/patchwork-node-0.1.2.tar", last modified: Thu Jan 12 16:10:40 2023, max compression
+gzip compressed data, was "dist/patchwork-node-0.1.3.tar", last modified: Fri Jun  2 17:00:25 2023, max compression
```

## Comparing `patchwork-node-0.1.2.tar` & `patchwork-node-0.1.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      996 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork/node/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork/node/contrib/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/contrib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1378 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/contrib/tortoise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork/node/core/
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/core/dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/core/module.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/core/router.py
--rw-rw-rw-   0 root         (0) root         (0)    17442 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/core/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork/node/executor/
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/executor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24435 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/executor/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork/node/executor/unit/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/executor/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6842 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/executor/unit/base.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/executor/unit/inline.py
--rw-rw-rw-   0 root         (0) root         (0)     8383 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/executor/unit/threads.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork/node/manager/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/manager/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/manager/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork/node/testutils/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/testutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9576 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/patchwork/node/testutils/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork_node.egg-info/
--rw-r--r--   0 root         (0) root         (0)      996 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork_node.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1266 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork_node.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork_node.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork_node.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      138 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork_node.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/patchwork_node.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1691 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/message.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/router.py
--rw-rw-rw-   0 root         (0) root         (0)     1545 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/test_exception_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     7158 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/test_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/test_inlineunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/test_router.py
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/test_worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 16:10:40.000000 patchwork-node-0.1.2/tests/testutils/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/testutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/testutils/test_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2159 2023-01-12 16:10:26.000000 patchwork-node-0.1.2/tests/testutils/test_worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      996 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork/node/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork/node/contrib/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/contrib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1378 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/contrib/tortoise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork/node/core/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/core/dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/core/module.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/core/router.py
+-rw-rw-rw-   0 root         (0) root         (0)    17442 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/core/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork/node/executor/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/executor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26337 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/executor/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork/node/executor/unit/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/executor/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6842 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/executor/unit/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/executor/unit/inline.py
+-rw-rw-rw-   0 root         (0) root         (0)     8383 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/executor/unit/threads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork/node/manager/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/manager/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/manager/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork/node/testutils/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/testutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9576 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/patchwork/node/testutils/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork_node.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      996 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork_node.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork_node.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork_node.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork_node.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork_node.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/patchwork_node.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/message.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/router.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/test_exception_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7158 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/test_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/test_inlineunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/test_router.py
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/test_worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:00:25.000000 patchwork-node-0.1.3/tests/testutils/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/testutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3063 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/testutils/test_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2023-06-02 17:00:14.000000 patchwork-node-0.1.3/tests/testutils/test_worker.py
```

### Comparing `patchwork-node-0.1.2/LICENSE` & `patchwork-node-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/PKG-INFO` & `patchwork-node-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-node
-Version: 0.1.2
+Version: 0.1.3
 Summary: Worker node for Patchwork - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-node-0.1.2/patchwork/node/contrib/tortoise.py` & `patchwork-node-0.1.3/patchwork/node/contrib/tortoise.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/core/dependencies.py` & `patchwork-node-0.1.3/patchwork/node/core/dependencies.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/core/exceptions.py` & `patchwork-node-0.1.3/patchwork/node/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/core/module.py` & `patchwork-node-0.1.3/patchwork/node/core/module.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/core/router.py` & `patchwork-node-0.1.3/patchwork/node/core/router.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/core/worker.py` & `patchwork-node-0.1.3/patchwork/node/core/worker.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/executor/base.py` & `patchwork-node-0.1.3/patchwork/node/executor/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 # -*- coding: utf-8 -*-
 
 import asyncio
 import logging
-from collections import defaultdict
 from datetime import datetime
 from functools import partial, lru_cache
 from itertools import chain
 from operator import itemgetter
+from time import time
 from typing import MutableMapping, List, Union, Coroutine, Type, Sequence, Dict, Callable, Awaitable, Optional, \
     Iterator, NoReturn, Tuple
 
+try:
+    from prometheus_client import Counter, Gauge, Histogram
+except ImportError:
+    # prometheus not installed, use stubs instead
+    from patchwork.core.stubs.prometheus import Counter, Gauge, Histogram
+
+
 import pytz as pytz
 from patchwork.core import Task, AsyncSubscriber, TaskMetadata
 from patchwork.core.config.base import ComponentConfig
 from patchwork.core.typing import FuncPath
 from patchwork.core.utils import cached_property, Flag
 from patchwork.node.core import Module
 from patchwork.node.core.exceptions import TaskControlException, TaskRetry, TaskFatal, TaskDrop, TaskNoHandler
@@ -30,14 +37,25 @@
 # if middleware does not return new finalizer, passed finalizer will be used
 # middlewares are run on the worker async loop, before passing task to processing unit!
 # keep this in mind as middleware execution may slow down whole executor
 MiddlewareType = Callable[[Task, AsyncSubscriber, FinalizerType], Awaitable[Optional[FinalizerType]]]
 
 ExceptionHandler = Callable[[Task, Exception], Awaitable]
 
+# prometheus metrics
+tasks_processed = Counter('patchwork_node_tasks_total', "Number of tasks processed", ['task_type'])
+tasks_success = Counter('patchwork_node_success_total', "Number of tasks succeeded", ['task_type'])
+tasks_failed = Counter('patchwork_node_failed_total', "Number of tasks failed", ['task_type'])
+tasks_cancelled = Counter('patchwork_node_cancelled_total', "Number of tasks cancelled", ['task_type'])
+tasks_backoffed = Counter('patchwork_node_backoff_total', "Number of tasks backoffed", ['task_type'])
+tasks_in_progress = Gauge('patchwork_node_in_progress', "Number of tasks in progress", ['task_type'])
+tasks_time = Histogram('patchwork_node_tasks_time', "Tasks processing time", ['task_type'])
+tasks_wait_get_time = Histogram('patchwork_node_get_time', "Task fetching time")
+tasks_wait_unit_time = Histogram('patchwork_node_unit_time', "Task waiting time for processing unit slot")
+
 
 async def check_task_middleware(task: Task, receiver: AsyncSubscriber, finalizer: FinalizerType):
     now = datetime.now(pytz.UTC)
     if task.meta.expires and task.meta.expires < now:
         # task has expired
         raise TaskFatal(reason="Task has expired")
     elif task.meta.not_before and task.meta.not_before > now:
@@ -277,16 +295,17 @@
         term_future = asyncio.create_task(self._terminate_request.wait())
         subscriber = self.worker.get_subscriber()
         self._busy.set(False)
 
         while True:
 
             try:
-                done, pending = await asyncio.wait((asyncio.create_task(subscriber.get()), term_future,),
-                                                   return_when=asyncio.FIRST_COMPLETED)
+                with tasks_wait_get_time.time():
+                    done, pending = await asyncio.wait((asyncio.create_task(subscriber.get()), term_future,),
+                                                       return_when=asyncio.FIRST_COMPLETED)
             except Exception as e:
                 self.logger.error(f"Client get() raises exception: {e.__class__.__name__}({e})",
                                   exc_info=True)
             else:
                 for task in done:
                     if task == term_future:
                         # termination future done, even if there is more done futures skip them
@@ -372,26 +391,27 @@
         if not_before is not None:
             new_task.meta.not_before = not_before
 
         publisher = self.worker.get_publisher()
         await publisher.send_task(new_task)
         return new_task
 
-    async def backoff_task(self, task, reason: str = None):
+    async def backoff_task(self, task: Task, reason: str = None):
         """
         Stores given task on backoff queue. If task cannot be executed for some reason (eg retries limit exceeded)
         can be logged and saved in special place for future investigation. This method allows to notify administrator
         that something has been not executed and should be manually verified.
 
         In base implementation this method just logs task using 'backoff' standard python logger and passes
         task in `extra` argument, which means that in basic configuration task contents might be lost.
         :param task:
         :param reason:
         :return:
         """
+        tasks_backoffed.labels(task_type=task.task_type).inc()
         backoff_log = logging.getLogger('backoff')
         backoff_log.log(logging.NOTSET,
                         f"Task '{task.uuid}' backoffed.{(' Reason: ' + reason) if reason is not None else ''}",
                         extra={'task': task})
         self.logger.debug(f"Task '{task.uuid}' backoffed.{(' Reason: ' + reason) if reason is not None else ''}")
 
     async def handle(self, task: Task, receiver: AsyncSubscriber, task_future: asyncio.Future):
@@ -408,28 +428,30 @@
             future.
 
         :param task: task to process
         :param receiver: a subscriber (receiver) which receives the task
         :param task_future: a future associated with the task which should resolved when task processing completes
         """
         finalizer = self._handle_task_result
+        tasks_in_progress.labels(task_type=task.task_type).inc()
+        task._local['_executor_start_time'] = time()
 
         try:
             for middleware in self._middlewares:
                 finalizer = (await middleware(task, receiver, finalizer)) or finalizer
 
             exec_fut = await self._execute(task, receiver)
         except Exception as exc:
             exec_fut = self.app_loop.create_future()
             exec_fut.set_exception(exc)
 
         finalizer = partial(finalizer, task=task, receiver=receiver)
 
         exec_fut.add_done_callback(
-            partial(self._task_done_callback, finalizer=finalizer(processing_fut=exec_fut), task_future=task_future)
+            partial(self._task_done_callback, finalizer=finalizer(processing_fut=exec_fut), task_future=task_future, task=task)
         )
 
     def _task_handling_completed(self, task_future: asyncio.Future):
         exc = task_future.exception()
         if exc is not None:
             # debug, there is many exceptions which are OK, if there was an error
             # it should be already reported
@@ -449,24 +471,26 @@
         for prefix, router in self._routers:
             if not task.task_type.startswith(prefix):
                 continue
 
             processor = router.handle(task, receiver)
             if processor is not None:
                 # await for submit which may hold if processing unit is full
-                pu_fut = await self.unit.submit(processor)
+                with tasks_wait_unit_time.time():
+                    pu_fut = await self.unit.submit(processor)
                 return pu_fut
 
         self.logger.error(f"No route to handle message type '{task.task_type}'")
         raise TaskNoHandler()
 
     def _task_done_callback(self,
                             processing_fut: asyncio.Future,
                             finalizer: Coroutine,
-                            task_future: asyncio.Future
+                            task_future: asyncio.Future,
+                            task: Task
                             ):
         """
         Handles value returned by task processing future.
         :param finalizer:
         :param processing_fut:
         :param task_future:
         :return:
@@ -483,22 +507,29 @@
             if exc is not None:
                 # if finalizer ends with unhandled exception it's internal fatal error
                 # kill the executor
                 task_future.set_result(None)
                 self.logger.fatal(f"Can't handle task result: {exc.__class__.__name__}({exc})")
                 self.harakiri(exc)
 
+            tasks_processed.labels(task_type=task.task_type).inc()
+            tasks_time.labels(task_type=task.task_type).observe(time() - task._local['_executor_start_time'])
+
             # otherwise pass processing future result to task result
             if processing_fut.cancelled():
                 task_future.cancel()
+                tasks_cancelled.labels(task_type=task.task_type).inc()
             elif processing_fut.exception():
                 task_future.set_exception(processing_fut.exception())
+                tasks_failed.labels(task_type=task.task_type).inc()
             else:
                 task_future.set_result(processing_fut.result())
+                tasks_success.labels(task_type=task.task_type).inc()
 
+        tasks_in_progress.labels(task_type=task.task_type).dec()
         handle_fut = self.app_loop.create_task(finalizer)
         handle_fut.add_done_callback(_callback)
 
     @lru_cache(maxsize=None)
     def _get_exception_handler(self, exc_class: Type[Exception]) -> Iterator[ExceptionHandler]:
         handlers = []
```

### Comparing `patchwork-node-0.1.2/patchwork/node/executor/unit/base.py` & `patchwork-node-0.1.3/patchwork/node/executor/unit/base.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/executor/unit/threads.py` & `patchwork-node-0.1.3/patchwork/node/executor/unit/threads.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/manager/base.py` & `patchwork-node-0.1.3/patchwork/node/manager/base.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/manager/http.py` & `patchwork-node-0.1.3/patchwork/node/manager/http.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork/node/testutils/worker.py` & `patchwork-node-0.1.3/patchwork/node/testutils/worker.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/patchwork_node.egg-info/PKG-INFO` & `patchwork-node-0.1.3/patchwork_node.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-node
-Version: 0.1.2
+Version: 0.1.3
 Summary: Worker node for Patchwork - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-node-0.1.2/patchwork_node.egg-info/SOURCES.txt` & `patchwork-node-0.1.3/patchwork_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/setup.py` & `patchwork-node-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/tests/router.py` & `patchwork-node-0.1.3/tests/router.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/tests/test_exception_handlers.py` & `patchwork-node-0.1.3/tests/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/tests/test_executor.py` & `patchwork-node-0.1.3/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/tests/test_inlineunit.py` & `patchwork-node-0.1.3/tests/test_inlineunit.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/tests/test_node.py` & `patchwork-node-0.1.3/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/tests/test_router.py` & `patchwork-node-0.1.3/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/tests/testutils/test_catcher.py` & `patchwork-node-0.1.3/tests/testutils/test_catcher.py`

 * *Files identical despite different names*

### Comparing `patchwork-node-0.1.2/tests/testutils/test_worker.py` & `patchwork-node-0.1.3/tests/testutils/test_worker.py`

 * *Files identical despite different names*

