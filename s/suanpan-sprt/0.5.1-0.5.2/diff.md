# Comparing `tmp/suanpan-sprt-0.5.1.tar.gz` & `tmp/suanpan-sprt-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.5.1.tar", last modified: Tue May 23 01:43:36 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.5.2.tar", last modified: Fri Jun  2 08:38:15 2023, max compression
```

## Comparing `suanpan-sprt-0.5.1.tar` & `suanpan-sprt-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      437 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       84 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.1/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.1/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5072 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4853 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      605 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      437 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.2/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.2/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.2/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5072 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.2/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.2/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.2/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.2/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.2/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.2/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.2/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5000 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.2/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.2/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.2/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.2/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.2/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-06-02 08:38:15.000000 suanpan-sprt-0.5.2/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.5.1/setup.py` & `suanpan-sprt-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.1/sprt/__main__.py` & `suanpan-sprt-0.5.2/sprt/__main__.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.1/sprt/arguments.py` & `suanpan-sprt-0.5.2/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.1/sprt/envs.py` & `suanpan-sprt-0.5.2/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.1/sprt/loader.py` & `suanpan-sprt-0.5.2/sprt/loader.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.1/sprt/log.py` & `suanpan-sprt-0.5.2/sprt/log.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.1/sprt/master.py` & `suanpan-sprt-0.5.2/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.1/sprt/server.py` & `suanpan-sprt-0.5.2/sprt/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pathlib
 import dataclasses
 import pydantic
 from contextlib import redirect_stdout, redirect_stderr, contextmanager
 from quart import Quart
 from quart_schema import QuartSchema, validate_request, validate_response, RequestSchemaValidationError
 from quart_schema import validation
-from . import loader, envs, exceptions
+from . import loader, envs, exceptions, utils
 
 
 @dataclasses.dataclass
 class FunctionContext:
     request_id: str
     node_id: str
     # 右面板参数
@@ -63,14 +63,17 @@
     QuartSchema(app)
 
     @app.post("/")
     @validate_request(FunctionParams)
     @validate_response(FunctionResponse)
     async def handle_post(data: FunctionParams) -> FunctionResponse:
         node_id = data.context.node_id
+        log_name = log_path / node_id
+        if utils.should_log_rollover(str(log_name)):
+            utils.do_log_rollover(str(log_name))
         with open(log_path / node_id, 'a', encoding='utf8') as f:
             with redirect_stdout(f), redirect_stderr(f), node_context(node_id):
                 function = None
                 try:
                     logging.debug(f'event: {data.context.args}')
                     function = load(data, working_dir)
                     ret = await function.call_func(data.context.request_id, data.context.args, data.context.params)
```

### Comparing `suanpan-sprt-0.5.1/sprt/storage.py` & `suanpan-sprt-0.5.2/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.1/sprt/testing.py` & `suanpan-sprt-0.5.2/sprt/testing.py`

 * *Files identical despite different names*

