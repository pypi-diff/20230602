# Comparing `tmp/python_equilibrium-0.6.1.tar.gz` & `tmp/python_equilibrium-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.6.1.tar", max compression
+gzip compressed data, was "python_equilibrium-0.6.2.tar", max compression
```

## Comparing `python_equilibrium-0.6.1.tar` & `python_equilibrium-0.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.6.1/LICENSE
--rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.6.1/README.md
--rw-r--r--   0        0        0     1661 2023-06-02 13:17:51.125647 python_equilibrium-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      449 2023-06-02 09:59:54.391350 python_equilibrium-0.6.1/src/equilibrium/AdmissionController.py
--rw-r--r--   0        0        0      899 2023-06-02 09:59:54.391350 python_equilibrium-0.6.1/src/equilibrium/BaseController.py
--rw-r--r--   0        0        0     1928 2023-06-02 09:59:54.391350 python_equilibrium-0.6.1/src/equilibrium/ControllerRegistry.py
--rw-r--r--   0        0        0     8949 2023-06-02 09:59:54.395350 python_equilibrium-0.6.1/src/equilibrium/CrudResourceController.py
--rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.6.1/src/equilibrium/JsonResourceStore.py
--rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.6.1/src/equilibrium/JsonResourceStore_test.py
--rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.6.1/src/equilibrium/Namespace.py
--rw-r--r--   0        0        0       58 2023-06-02 09:59:54.395350 python_equilibrium-0.6.1/src/equilibrium/NotSet.py
--rw-r--r--   0        0        0    15468 2023-06-02 13:16:38.134008 python_equilibrium-0.6.1/src/equilibrium/Resource.py
--rw-r--r--   0        0        0     3474 2023-06-02 09:59:54.395350 python_equilibrium-0.6.1/src/equilibrium/ResourceContext.py
--rw-r--r--   0        0        0      258 2023-06-02 09:59:54.395350 python_equilibrium-0.6.1/src/equilibrium/ResourceController.py
--rw-r--r--   0        0        0     8691 2023-06-02 09:59:54.395350 python_equilibrium-0.6.1/src/equilibrium/ResourceRegistry.py
--rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.6.1/src/equilibrium/ResourceStore.py
--rw-r--r--   0        0        0     1248 2023-06-02 09:59:54.395350 python_equilibrium-0.6.1/src/equilibrium/ResourceTypeRegistry.py
--rw-r--r--   0        0        0     4202 2023-05-26 17:59:04.238639 python_equilibrium-0.6.1/src/equilibrium/Resource_test.py
--rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.6.1/src/equilibrium/Service.py
--rw-r--r--   0        0        0     2913 2023-06-02 09:59:54.395350 python_equilibrium-0.6.1/src/equilibrium/ServiceRegistry.py
--rw-r--r--   0        0        0     1261 2023-06-02 13:17:51.125647 python_equilibrium-0.6.1/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.6.1/src/equilibrium/py.typed
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 python_equilibrium-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.6.2/README.md
+-rw-r--r--   0        0        0     1661 2023-06-02 13:55:59.596952 python_equilibrium-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-06-02 09:59:54.391350 python_equilibrium-0.6.2/src/equilibrium/AdmissionController.py
+-rw-r--r--   0        0        0      899 2023-06-02 09:59:54.391350 python_equilibrium-0.6.2/src/equilibrium/BaseController.py
+-rw-r--r--   0        0        0     1928 2023-06-02 09:59:54.391350 python_equilibrium-0.6.2/src/equilibrium/ControllerRegistry.py
+-rw-r--r--   0        0        0     8949 2023-06-02 09:59:54.395350 python_equilibrium-0.6.2/src/equilibrium/CrudResourceController.py
+-rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.6.2/src/equilibrium/JsonResourceStore.py
+-rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.6.2/src/equilibrium/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.6.2/src/equilibrium/Namespace.py
+-rw-r--r--   0        0        0       58 2023-06-02 09:59:54.395350 python_equilibrium-0.6.2/src/equilibrium/NotSet.py
+-rw-r--r--   0        0        0    15426 2023-06-02 13:55:34.545025 python_equilibrium-0.6.2/src/equilibrium/Resource.py
+-rw-r--r--   0        0        0     3474 2023-06-02 09:59:54.395350 python_equilibrium-0.6.2/src/equilibrium/ResourceContext.py
+-rw-r--r--   0        0        0      258 2023-06-02 09:59:54.395350 python_equilibrium-0.6.2/src/equilibrium/ResourceController.py
+-rw-r--r--   0        0        0     8691 2023-06-02 09:59:54.395350 python_equilibrium-0.6.2/src/equilibrium/ResourceRegistry.py
+-rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.6.2/src/equilibrium/ResourceStore.py
+-rw-r--r--   0        0        0     1248 2023-06-02 09:59:54.395350 python_equilibrium-0.6.2/src/equilibrium/ResourceTypeRegistry.py
+-rw-r--r--   0        0        0     4202 2023-05-26 17:59:04.238639 python_equilibrium-0.6.2/src/equilibrium/Resource_test.py
+-rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.6.2/src/equilibrium/Service.py
+-rw-r--r--   0        0        0     2913 2023-06-02 09:59:54.395350 python_equilibrium-0.6.2/src/equilibrium/ServiceRegistry.py
+-rw-r--r--   0        0        0     1261 2023-06-02 13:55:59.596952 python_equilibrium-0.6.2/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.6.2/src/equilibrium/py.typed
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 python_equilibrium-0.6.2/PKG-INFO
```

### Comparing `python_equilibrium-0.6.1/LICENSE` & `python_equilibrium-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/README.md` & `python_equilibrium-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/pyproject.toml` & `python_equilibrium-0.6.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_equilibrium-0.6.1/src/equilibrium/BaseController.py` & `python_equilibrium-0.6.2/src/equilibrium/BaseController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/ControllerRegistry.py` & `python_equilibrium-0.6.2/src/equilibrium/ControllerRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/CrudResourceController.py` & `python_equilibrium-0.6.2/src/equilibrium/CrudResourceController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/JsonResourceStore.py` & `python_equilibrium-0.6.2/src/equilibrium/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/JsonResourceStore_test.py` & `python_equilibrium-0.6.2/src/equilibrium/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/Namespace.py` & `python_equilibrium-0.6.2/src/equilibrium/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/Resource.py` & `python_equilibrium-0.6.2/src/equilibrium/Resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,14 @@
             return f"{self.apiVersion}/{self.kind}"
 
         @classmethod
         def of(cls, s: str) -> Resource.Type:
             apiVersion, kind = s.rpartition("/")[::2]
             return cls(apiVersion, kind)
 
-        @classmethod
         def uri(self, namespace: str | None, name: str) -> Resource.URI:
             return Resource.URI(self.apiVersion, self.kind, namespace, name)
 
     @JsonConverter.using_classmethods(serialize="__str__", deserialize="of")
     @dataclass(frozen=True)
     class Locator:
         namespace: str | None
@@ -255,15 +254,14 @@
             return f"{self.namespace}/{self.name}"
 
         @classmethod
         def of(cls, s: str) -> Resource.Locator:
             namespace, name = s.rpartition("/")[::2]
             return cls(namespace or None, name)
 
-        @classmethod
         def uri(self, apiVersion: str, kind: str, name: str) -> Resource.URI:
             return Resource.URI(apiVersion, kind, self.namespace, name)
 
     @dataclass(frozen=True)
     class Metadata:
         namespace: str | None
         name: str
```

### Comparing `python_equilibrium-0.6.1/src/equilibrium/ResourceContext.py` & `python_equilibrium-0.6.2/src/equilibrium/ResourceContext.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/ResourceRegistry.py` & `python_equilibrium-0.6.2/src/equilibrium/ResourceRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/ResourceStore.py` & `python_equilibrium-0.6.2/src/equilibrium/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/ResourceTypeRegistry.py` & `python_equilibrium-0.6.2/src/equilibrium/ResourceTypeRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/Resource_test.py` & `python_equilibrium-0.6.2/src/equilibrium/Resource_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/Service.py` & `python_equilibrium-0.6.2/src/equilibrium/Service.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/ServiceRegistry.py` & `python_equilibrium-0.6.2/src/equilibrium/ServiceRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.6.1/src/equilibrium/__init__.py` & `python_equilibrium-0.6.2/src/equilibrium/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     "ResourceRegistry",
     "ResourceStore",
     "ResourceTypeRegistry",
     "Service",
     "ServiceRegistry",
 ]
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
```

### Comparing `python_equilibrium-0.6.1/PKG-INFO` & `python_equilibrium-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

