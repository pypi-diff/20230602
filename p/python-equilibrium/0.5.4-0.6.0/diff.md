# Comparing `tmp/python_equilibrium-0.5.4.tar.gz` & `tmp/python_equilibrium-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.5.4.tar", max compression
+gzip compressed data, was "python_equilibrium-0.6.0.tar", max compression
```

## Comparing `python_equilibrium-0.5.4.tar` & `python_equilibrium-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,23 @@
--rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.5.4/LICENSE
--rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.5.4/README.md
--rw-r--r--   0        0        0     1661 2023-05-26 18:06:30.619111 python_equilibrium-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      714 2023-05-19 08:58:20.216493 python_equilibrium-0.5.4/src/equilibrium/AdmissionController.py
--rw-r--r--   0        0        0     8461 2023-05-19 08:58:20.216493 python_equilibrium-0.5.4/src/equilibrium/CrudResourceController.py
--rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.5.4/src/equilibrium/JsonResourceStore.py
--rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.5.4/src/equilibrium/JsonResourceStore_test.py
--rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.5.4/src/equilibrium/Namespace.py
--rw-r--r--   0        0        0    15124 2023-05-26 18:05:36.210790 python_equilibrium-0.5.4/src/equilibrium/Resource.py
--rw-r--r--   0        0        0    15825 2023-05-25 22:02:39.509291 python_equilibrium-0.5.4/src/equilibrium/ResourceContext.py
--rw-r--r--   0        0        0      482 2023-05-19 08:58:20.216493 python_equilibrium-0.5.4/src/equilibrium/ResourceController.py
--rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.5.4/src/equilibrium/ResourceStore.py
--rw-r--r--   0        0        0     4202 2023-05-26 17:59:04.238639 python_equilibrium-0.5.4/src/equilibrium/Resource_test.py
--rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.5.4/src/equilibrium/Service.py
--rw-r--r--   0        0        0     1045 2023-05-26 18:06:30.619111 python_equilibrium-0.5.4/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.5.4/src/equilibrium/py.typed
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 python_equilibrium-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.6.0/README.md
+-rw-r--r--   0        0        0     1661 2023-06-02 09:59:59.791329 python_equilibrium-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-06-02 09:59:54.391350 python_equilibrium-0.6.0/src/equilibrium/AdmissionController.py
+-rw-r--r--   0        0        0      899 2023-06-02 09:59:54.391350 python_equilibrium-0.6.0/src/equilibrium/BaseController.py
+-rw-r--r--   0        0        0     1928 2023-06-02 09:59:54.391350 python_equilibrium-0.6.0/src/equilibrium/ControllerRegistry.py
+-rw-r--r--   0        0        0     8949 2023-06-02 09:59:54.395350 python_equilibrium-0.6.0/src/equilibrium/CrudResourceController.py
+-rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.6.0/src/equilibrium/JsonResourceStore.py
+-rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.6.0/src/equilibrium/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.6.0/src/equilibrium/Namespace.py
+-rw-r--r--   0        0        0       58 2023-06-02 09:59:54.395350 python_equilibrium-0.6.0/src/equilibrium/NotSet.py
+-rw-r--r--   0        0        0    15124 2023-05-26 18:05:36.210790 python_equilibrium-0.6.0/src/equilibrium/Resource.py
+-rw-r--r--   0        0        0     3474 2023-06-02 09:59:54.395350 python_equilibrium-0.6.0/src/equilibrium/ResourceContext.py
+-rw-r--r--   0        0        0      258 2023-06-02 09:59:54.395350 python_equilibrium-0.6.0/src/equilibrium/ResourceController.py
+-rw-r--r--   0        0        0     8691 2023-06-02 09:59:54.395350 python_equilibrium-0.6.0/src/equilibrium/ResourceRegistry.py
+-rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.6.0/src/equilibrium/ResourceStore.py
+-rw-r--r--   0        0        0     1248 2023-06-02 09:59:54.395350 python_equilibrium-0.6.0/src/equilibrium/ResourceTypeRegistry.py
+-rw-r--r--   0        0        0     4202 2023-05-26 17:59:04.238639 python_equilibrium-0.6.0/src/equilibrium/Resource_test.py
+-rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.6.0/src/equilibrium/Service.py
+-rw-r--r--   0        0        0     2913 2023-06-02 09:59:54.395350 python_equilibrium-0.6.0/src/equilibrium/ServiceRegistry.py
+-rw-r--r--   0        0        0     1261 2023-06-02 09:59:59.791329 python_equilibrium-0.6.0/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.6.0/src/equilibrium/py.typed
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 python_equilibrium-0.6.0/PKG-INFO
```

### Comparing `python_equilibrium-0.5.4/LICENSE` & `python_equilibrium-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.4/README.md` & `python_equilibrium-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.4/pyproject.toml` & `python_equilibrium-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.5.4"
+version = "0.6.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_equilibrium-0.5.4/src/equilibrium/CrudResourceController.py` & `python_equilibrium-0.6.0/src/equilibrium/CrudResourceController.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from abc import abstractmethod
 from enum import Enum
 from logging import Logger
 from typing import Any, ClassVar, Generic
 
 from equilibrium.AdmissionController import AdmissionController
+from equilibrium.BaseController import BaseController
 from equilibrium.Resource import Resource
 from equilibrium.ResourceController import ResourceController
 from equilibrium.ResourceStore import ResourceStore
 
 __all__ = ["CrudResourceController"]
 
 
@@ -17,14 +18,15 @@
     A base class for resource controllers that follow a CRUD pattern and may also control admittance.
     """
 
     spec_type: type[Resource.T_Spec]
     state_type: type[Resource.T_State]
     _logger_name: ClassVar[str]
     log: Logger
+    ctx: BaseController.Context  # Set in reconcile() and admit_resource().
 
     class Status(Enum):
         Deleted = "deleted"
 
     Deleted = Status.Deleted
 
     def __init_subclass__(
@@ -34,14 +36,18 @@
         **kwargs: Any,
     ) -> None:
         super().__init_subclass__(**kwargs)
         cls._logger_name = f"{cls.__module__}.{cls.__name__}"
         cls.spec_type = spec_type
         cls.state_type = state_type
 
+    @property
+    def store(self) -> ResourceStore:
+        return self.ctx.resources.store
+
     def admit(self, resource: Resource[Resource.T_Spec]) -> Resource[Resource.T_Spec]:
         """
         Test for the admission of the resource into the system. A potentially modified version is returned. An
         exception shall be raised if the resource cannot be admitted to the system. If the previous spec of the
         resource is of interest, it can be retrieved with the #resources manager.
         """
 
@@ -71,15 +77,15 @@
         log = logging.getLogger(self._logger_name)
         if uri:
             log = log.getChild(str(uri))
         return log
 
     def _reconcile_internal(self, lock: ResourceStore.LockID, uri: Resource.URI) -> None:
         log = self._get_logger(uri)
-        raw_resource = self.resources.get(lock, uri)
+        raw_resource = self.store.get(lock, uri)
         if raw_resource is None:
             log.warning("Resource %r no longer exists, skipping reconciliation.", uri)
             return
 
         log.debug("Reconciling resource '%s'.", uri)
         try:
             resource: Resource[Resource.T_Spec] = raw_resource.into(self.spec_type)
@@ -136,56 +142,61 @@
                         raise RuntimeError(
                             f"{type(self).__name__}.update() is expected to return an object of type "
                             f"{self.state_type.__name__}, got {type(current_state).__name__} instead."
                         )
 
             if current_state is None:
                 log.debug("Resource '%s' has been deleted.", uri)
-                self.resources.delete(lock, uri)
+                self.store.delete(lock, uri)
             else:
                 log.debug("Resource '%s' has been updated.", uri)
                 resource.set_state(self.state_type, current_state)
-                self.resources.put(lock, resource.into_generic())
+
+                # NOTE(@NiklasRosenstein): We go through the #put() method of the #ResourceRegistry instead to invoke
+                #       admission controllers.
+                self.ctx.resources.put(resource, stateful=True, existing_lock=lock)
 
         except Exception:
             log.exception("An unhandled exception occurred reconciling a resource.")
 
     # ResourceController
 
-    def reconcile(self) -> None:
+    def reconcile(self, ctx: ResourceController.Context) -> None:
         self.log = self._get_logger(None)
+        self.ctx = ctx
 
-        namespaces = self.resources.namespaces()
+        namespaces = self.store.namespaces()
         self.log.info(
             "Reconciling resources of type '%s' (namespaces: %r)",
             self.spec_type.TYPE,
             {ns.metadata.name for ns in namespaces},
         )
         for namespace in namespaces:
-            lock_request = self.resources.LockRequest(apiVersion=self.spec_type.API_VERSION, kind=self.spec_type.KIND)
-            with self.resources.enter(lock_request) as lock:
-                search_request = self.resources.SearchRequest(
+            lock_request = self.store.LockRequest(apiVersion=self.spec_type.API_VERSION, kind=self.spec_type.KIND)
+            with self.store.enter(lock_request) as lock:
+                search_request = self.store.SearchRequest(
                     apiVersion=self.spec_type.API_VERSION,
                     kind=self.spec_type.KIND,
                     namespace=namespace.metadata.name,
                 )
-                resource_uris = self.resources.search(lock, search_request)
+                resource_uris = self.store.search(lock, search_request)
 
             self.log.debug(
                 "Found %d resources of type '%s' in namespace '%s'.",
                 len(resource_uris),
                 self.spec_type.TYPE,
                 namespace.metadata.name,
             )
             for uri in resource_uris:
-                lock_request = self.resources.LockRequest.from_uri(uri)
-                with self.resources.enter(lock_request) as lock:
+                lock_request = self.store.LockRequest.from_uri(uri)
+                with self.store.enter(lock_request) as lock:
                     self._reconcile_internal(lock, uri)
 
     # AdmissionController
 
-    def admit_resource(self, resource: Resource[Any]) -> Resource[Any]:
+    def admit_resource(self, ctx: AdmissionController.Context, resource: Resource[Any]) -> Resource[Any]:
         if self.spec_type.check_uri(resource.uri):
             self.log = self._get_logger(resource.uri)
             self.log.debug("Checking for admittance of resource '%s'.", resource.uri)
+            self.ctx = ctx
             return self.admit(resource.into(self.spec_type))
         return resource
```

### Comparing `python_equilibrium-0.5.4/src/equilibrium/JsonResourceStore.py` & `python_equilibrium-0.6.0/src/equilibrium/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.4/src/equilibrium/JsonResourceStore_test.py` & `python_equilibrium-0.6.0/src/equilibrium/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.4/src/equilibrium/Namespace.py` & `python_equilibrium-0.6.0/src/equilibrium/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.4/src/equilibrium/Resource.py` & `python_equilibrium-0.6.0/src/equilibrium/Resource.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.4/src/equilibrium/ResourceStore.py` & `python_equilibrium-0.6.0/src/equilibrium/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.4/src/equilibrium/Resource_test.py` & `python_equilibrium-0.6.0/src/equilibrium/Resource_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.4/src/equilibrium/Service.py` & `python_equilibrium-0.6.0/src/equilibrium/Service.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.4/PKG-INFO` & `python_equilibrium-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.5.4
+Version: 0.6.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

