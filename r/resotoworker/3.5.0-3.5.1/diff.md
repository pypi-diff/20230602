# Comparing `tmp/resotoworker-3.5.0.tar.gz` & `tmp/resotoworker-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.5.0.tar", last modified: Fri May 26 18:23:59 2023, max compression
+gzip compressed data, was "resotoworker-3.5.1.tar", last modified: Fri Jun  2 14:49:51 2023, max compression
```

## Comparing `resotoworker-3.5.0.tar` & `resotoworker-3.5.1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:59.023646 resotoworker-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:44.000000 resotoworker-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-26 18:23:59.023646 resotoworker-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-26 18:21:44.000000 resotoworker-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-26 18:21:44.000000 resotoworker-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:59.023646 resotoworker-3.5.0/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 18:21:44.000000 resotoworker-3.5.0/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:59.023646 resotoworker-3.5.0/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-26 18:23:59.000000 resotoworker-3.5.0/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-26 18:23:59.000000 resotoworker-3.5.0/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:59.000000 resotoworker-3.5.0/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 18:23:59.000000 resotoworker-3.5.0/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:59.000000 resotoworker-3.5.0/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:23:59.000000 resotoworker-3.5.0/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 18:23:59.000000 resotoworker-3.5.0/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:59.023646 resotoworker-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-26 18:21:44.000000 resotoworker-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:59.023646 resotoworker-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:44.000000 resotoworker-3.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-26 18:21:44.000000 resotoworker-3.5.0/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-26 18:21:44.000000 resotoworker-3.5.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-26 18:21:44.000000 resotoworker-3.5.0/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-26 18:21:44.000000 resotoworker-3.5.0/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-26 18:21:44.000000 resotoworker-3.5.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:51.866352 resotoworker-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:46:08.000000 resotoworker-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-02 14:49:51.866352 resotoworker-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-02 14:46:08.000000 resotoworker-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-02 14:46:08.000000 resotoworker-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:51.866352 resotoworker-3.5.1/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:51.866352 resotoworker-3.5.1/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:47:17.000000 resotoworker-3.5.1/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:49:51.866352 resotoworker-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:51.866352 resotoworker-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/test_utils.py
```

### Comparing `resotoworker-3.5.0/PKG-INFO` & `resotoworker-3.5.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.5.0
+Version: 3.5.1
 Summary: Runs collector plugins and sends the result to resotocore.
-Home-page: https://github.com/someengineering/resoto/tree/main/resotoworker
-License: Apache 2.0
-Keywords: cloud security
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Environment :: Console
-Classifier: Natural Language :: English
-Classifier: Topic :: Security
-Classifier: Topic :: Utilities
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # `resotoworker`
 Resoto worker daemon
 
 
 ## Table of contents
```

### Comparing `resotoworker-3.5.0/README.md` & `resotoworker-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.0/resotoworker/__main__.py` & `resotoworker-3.5.1/resotoworker/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         tls_data=tls_data,
     )
 
     add_config(config, plugin_loader.all_collector_plugins())
     plugin_loader.add_plugin_config(config)
     config.load_config()
 
-    write_files_to_home_dir(config.resotoworker.write_files_to_home_dir, write_utf8_file)
+    write_files_to_home_dir(config.resotoworker.all_files_in_home_dir(), write_utf8_file)
 
     def send_request(request: requests.Request) -> requests.Response:
         prepared = request.prepare()
         s = requests.Session()
         verify = None
         if tls_data:
             verify = tls_data.verify
```

### Comparing `resotoworker-3.5.0/resotoworker/cleanup.py` & `resotoworker-3.5.1/resotoworker/cleanup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 
 class Cleaner:
     def __init__(self, graph: Graph, feedback: CoreFeedback) -> None:
         self.graph = graph
         self.feedback = feedback
 
-    @metrics_cleanup.time()  # type: ignore
+    @metrics_cleanup.time()
     def cleanup(self, config: Config, plugins: Dict[str, Type[BaseCollectorPlugin]]) -> None:
         if not Config.resotoworker.cleanup:
             log.debug("Cleanup called but resotoworker.cleanup not configured" " - ignoring call")
             return
 
         log.info("Running cleanup")
         # create a subgraph of all the nodes that have a delete edge
```

### Comparing `resotoworker-3.5.0/resotoworker/collect.py` & `resotoworker-3.5.1/resotoworker/collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.0/resotoworker/config.py` & `resotoworker-3.5.1/resotoworker/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from concurrent.futures import ThreadPoolExecutor, TimeoutError
 from resotolib.graph import GraphMergeKind
 from resotolib.config import Config
 from resotolib.proc import num_default_threads
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.logger import log
 from attrs import define, field, frozen
-from typing import ClassVar, Optional, List, Type
-
+from typing import ClassVar, Optional, List, Type, Dict
 
 _default_collectors: List[str] = []
 
 
 @frozen
 class PluginAutoEnabledResult:
     cloud: str
@@ -102,15 +101,31 @@
             "description": "Web root in browser (change if running behind an ingress proxy)",
             "restart_required": True,
         },
     )
     write_files_to_home_dir: List[HomeDirectoryFile] = field(
         factory=list,
         metadata={
+            "description": "Deprecated. Use files_in_home_dir instead.",
+            "restart_required": True,
+        },
+    )
+    # optional for backwards compatibility
+    files_in_home_dir: Optional[Dict[str, str]] = field(  # type: ignore
+        factory=dict,
+        metadata={
             "description": (
-                "All entries that are defined in this section are created as files on demand. "
+                "All entries that are defined in this section are created as files on demand.\n"
                 "Use this option to define .aws/credentials, .kube/config file or other "
-                "credential files that should be passed to the worker as file."
+                "credential files that should be passed to the worker as file.\n"
+                "The key is the path to the file, the value is the content of the file."
             ),
             "restart_required": True,
         },
     )
+
+    def all_files_in_home_dir(self) -> List[HomeDirectoryFile]:
+        files = self.write_files_to_home_dir.copy()
+        if self.files_in_home_dir is not None:
+            for path, content in self.files_in_home_dir.items():
+                files.append(HomeDirectoryFile(path=path, content=content))
+        return files
```

### Comparing `resotoworker-3.5.0/resotoworker/pluginloader.py` & `resotoworker-3.5.1/resotoworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.0/resotoworker/resotocore.py` & `resotoworker-3.5.1/resotoworker/resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.0/resotoworker/tag.py` & `resotoworker-3.5.1/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.0/resotoworker/utils.py` & `resotoworker-3.5.1/resotoworker/utils.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.0/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.5.1/resotoworker.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.5.0
+Version: 3.5.1
 Summary: Runs collector plugins and sends the result to resotocore.
-Home-page: https://github.com/someengineering/resoto/tree/main/resotoworker
-License: Apache 2.0
-Keywords: cloud security
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Environment :: Console
-Classifier: Natural Language :: English
-Classifier: Topic :: Security
-Classifier: Topic :: Utilities
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # `resotoworker`
 Resoto worker daemon
 
 
 ## Table of contents
```

### Comparing `resotoworker-3.5.0/test/test_collect.py` & `resotoworker-3.5.1/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.0/test/test_resotocore.py` & `resotoworker-3.5.1/test/test_resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.0/test/test_utils.py` & `resotoworker-3.5.1/test/test_utils.py`

 * *Files identical despite different names*

