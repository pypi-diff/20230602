# Comparing `tmp/taipan_di-0.0.2.tar.gz` & `tmp/taipan_di-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipan_di-0.0.2.tar", max compression
+gzip compressed data, was "taipan_di-0.0.3.tar", max compression
```

## Comparing `taipan_di-0.0.2.tar` & `taipan_di-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-05-28 19:09:58.108375 taipan_di-0.0.2/LICENSE
--rw-r--r--   0        0        0     2894 2023-05-28 19:09:58.108375 taipan_di-0.0.2/README.md
--rw-r--r--   0        0        0     1025 2023-05-28 19:09:58.108375 taipan_di-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      110 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/__init__.py
--rw-r--r--   0        0        0       21 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/__version__.py
--rw-r--r--   0        0        0       55 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/__init__.py
--rw-r--r--   0        0        0     2832 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/dependency_collection.py
--rw-r--r--   0        0        0      676 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/dependency_container.py
--rw-r--r--   0        0        0      703 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/dependency_provider.py
--rw-r--r--   0        0        0     3651 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/instanciate_service.py
--rw-r--r--   0        0        0       83 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/scopes/__init__.py
--rw-r--r--   0        0        0      686 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/scopes/factory_scope.py
--rw-r--r--   0        0        0      800 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/scopes/singleton_scope.py
--rw-r--r--   0        0        0      204 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/__init__.py
--rw-r--r--   0        0        0       38 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/taipan_error.py
--rw-r--r--   0        0        0      105 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/taipan_injection_error.py
--rw-r--r--   0        0        0      100 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/taipan_type_error.py
--rw-r--r--   0        0        0      108 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/taipan_unregistered_error.py
--rw-r--r--   0        0        0      157 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/interfaces/__init__.py
--rw-r--r--   0        0        0      938 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/interfaces/base_dependency_container.py
--rw-r--r--   0        0        0      614 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/interfaces/base_dependency_provider.py
--rw-r--r--   0        0        0      519 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/interfaces/base_scope.py
--rw-r--r--   0        0        0        0 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/py.typed
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 taipan_di-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-02 10:28:17.804484 taipan_di-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2894 2023-06-02 10:28:17.804484 taipan_di-0.0.3/README.md
+-rw-r--r--   0        0        0     1004 2023-06-02 10:28:17.804484 taipan_di-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/__init__.py
+-rw-r--r--   0        0        0       21 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/__version__.py
+-rw-r--r--   0        0        0       55 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/__init__.py
+-rw-r--r--   0        0        0     3181 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/dependency_collection.py
+-rw-r--r--   0        0        0      676 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/dependency_container.py
+-rw-r--r--   0        0        0      703 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/dependency_provider.py
+-rw-r--r--   0        0        0     3677 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/instanciate_service.py
+-rw-r--r--   0        0        0       83 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/scopes/__init__.py
+-rw-r--r--   0        0        0      474 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/scopes/factory_scope.py
+-rw-r--r--   0        0        0      594 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/scopes/singleton_scope.py
+-rw-r--r--   0        0        0      204 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/taipan_error.py
+-rw-r--r--   0        0        0      105 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/taipan_injection_error.py
+-rw-r--r--   0        0        0      100 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/taipan_type_error.py
+-rw-r--r--   0        0        0      108 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/taipan_unregistered_error.py
+-rw-r--r--   0        0        0      157 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/interfaces/__init__.py
+-rw-r--r--   0        0        0      938 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/interfaces/base_dependency_container.py
+-rw-r--r--   0        0        0     1029 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/interfaces/base_dependency_provider.py
+-rw-r--r--   0        0        0      519 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/interfaces/base_scope.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/py.typed
+-rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 taipan_di-0.0.3/PKG-INFO
```

### Comparing `taipan_di-0.0.2/LICENSE` & `taipan_di-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.2/README.md` & `taipan_di-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.2/pyproject.toml` & `taipan_di-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Taipan-DI"
-version = "0.0.2"
+version = "0.0.3"
 description = "Truly Amazing Inversion of control Python library Analogous to .Net's DI"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 keywords = ["taipan", "dependency injection", "dependency", "python"]
 
@@ -18,15 +18,14 @@
 ]
 
 include = ["taipan_di/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.6.0"
-typeguard = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 black = "^23.3.0"
 mypy = "^1.3.0"
```

### Comparing `taipan_di-0.0.2/taipan_di/classes/dependency_collection.py` & `taipan_di-0.0.3/taipan_di/classes/dependency_collection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from typing import Any, Callable, Type, TypeVar
+from typing import Callable, Type, TypeVar
 
 from taipan_di.interfaces import BaseDependencyProvider
-from taipan_di.errors import TaipanTypeError
-from typeguard import check_type
 
 from .dependency_container import DependencyContainer
 from .instanciate_service import instanciate_service
 from .scopes import FactoryScope, SingletonScope
 
 
 T = TypeVar("T")
@@ -18,64 +16,70 @@
         self._container = DependencyContainer()
 
     # Public methods
 
     def register_singleton_creator(
         self, type: Type[T], creator: Callable[[BaseDependencyProvider], T]
     ) -> None:
+        """
+        Registers a service as a singleton by specifying how to create its instance.
+        """
         service = SingletonScope(creator)
         self._container.register(type, service)
 
     def register_singleton_instance(self, type: Type[T], instance: T) -> None:
-        self._assert_instance_type(instance, type)
-
+        """
+        Registers a service as a singleton by providing the instance to return.
+        """
         creator = lambda provider: instance
         self.register_singleton_creator(type, creator)
 
     def register_singleton(
         self, interface_type: Type[T], implementation_type: Type[U] = None
     ) -> None:
+        """
+        Register a service as a singleton by specifying the implementation type to use.
+        
+        On resolve, the implementation will be instanciated with its dependencies automatically resolved.
+        
+        If the implementation type isn't provided, the interface type will be used as the implementation type.
+        
+        If the implementation type don't possess an __init__ method, the resolve will fail.
+        """
         if implementation_type is None:
             implementation_type = interface_type
             
-        self._assert_implementation_derives_interface(implementation_type, interface_type)
-
         creator = lambda provider: instanciate_service(implementation_type, provider)
         self.register_singleton_creator(interface_type, creator)
 
     def register_factory_creator(
         self, type: Type[T], creator: Callable[[BaseDependencyProvider], T]
     ) -> None:
+        """
+        Registers a service as a factory by specifying how to create its instances.
+        """
         service = FactoryScope(creator)
         self._container.register(type, service)
 
     def register_factory(
         self, interface_type: Type[T], implementation_type: Type[U] = None
     ) -> None:
+        """
+        Register a service as a factory by specifying the implementation type to use.
+        
+        On resolve, the implementation will be instanciated with its dependencies automatically resolved.
+        
+        If the implementation type isn't provided, the interface type will be used as the implementation type.
+        
+        If the implementation type don't possess an __init__ method, the resolve will fail.
+        """
         if implementation_type is None:
             implementation_type = interface_type
-            
-        self._assert_implementation_derives_interface(implementation_type, interface_type)
 
         creator = lambda provider: instanciate_service(implementation_type, provider)
         self.register_factory_creator(interface_type, creator)
 
     def build(self) -> BaseDependencyProvider:
+        """
+        Builds the service provider containing the services registered by this collection.
+        """
         return self._container.build()
-
-    # Private methods
-
-    def _assert_instance_type(self, instance: Any, type: Type) -> None:
-        try:
-            check_type(instance, type)
-        except:
-            raise TaipanTypeError(f"Provided instance is not of type {str(type)}")
-
-    def _assert_implementation_derives_interface(
-        self, implementation_type: Type[U], interface_type: Type[T]
-    ) -> None:
-        if not issubclass(implementation_type, interface_type):
-            raise TaipanTypeError(
-                "Implementation type %s must derive from interface type %s",
-                str(implementation_type),
-                str(interface_type),
-            )
```

### Comparing `taipan_di-0.0.2/taipan_di/classes/dependency_container.py` & `taipan_di-0.0.3/taipan_di/classes/dependency_container.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.2/taipan_di/classes/dependency_provider.py` & `taipan_di-0.0.3/taipan_di/classes/dependency_provider.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.2/taipan_di/classes/instanciate_service.py` & `taipan_di-0.0.3/taipan_di/classes/instanciate_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Union,
     ForwardRef,
     cast,
 )
 from typing_extensions import Protocol
 
 from taipan_di.interfaces import BaseDependencyProvider
-from taipan_di.errors import TaipanInjectionError
+from taipan_di.errors import TaipanInjectionError, TaipanTypeError
 
 
 S = TypeVar("S")
 
 ServiceDefinition = Type[S]
 ServiceResult = S
 
@@ -103,16 +103,16 @@
 
 def instanciate_service(service: Type[S], provider: BaseDependencyProvider) -> S:
     constructor = getattr(service, "__init__")
 
     # ignore abstract class initialiser and protocol initialisers
     if (
         constructor in [ABC.__init__, _no_init] or constructor.__name__ == "_no_init"
-    ):  # FIXME: fix this when typing_extensions library gets fixed
-        return constructor
+    ):
+        raise TaipanTypeError(f"{str(service)} has no __init__, cannot instanciate the service")
 
     # Add class definition to dependency injection
     parameters = _inspect_function_arguments(constructor)
     parameters_name = tuple([p for p in parameters.keys() if p != "self"])
 
     def _resolve_kwargs() -> dict:
         if len(parameters_name) == 0:
```

### Comparing `taipan_di-0.0.2/taipan_di/classes/scopes/singleton_scope.py` & `taipan_di-0.0.3/taipan_di/classes/scopes/singleton_scope.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from typing import Any, Callable, Type, TypeVar, cast
 
 from taipan_di.interfaces import BaseDependencyProvider, BaseScope
-from taipan_di.errors import TaipanTypeError
-from typeguard import check_type
 
 T = TypeVar("T")
 
 class SingletonScope(BaseScope):
     def __init__(self, creator: Callable[[BaseDependencyProvider], Any]) -> None:
         self._creator = creator
         self._memoized_instance = None
 
     def get_instance(self, type: Type[T], container: BaseDependencyProvider) -> T:
         if self._memoized_instance is None:
             self._memoized_instance = self._creator(container)
 
-        try:
-            result = check_type(self._memoized_instance, type)
-            return result
-        except:
-            raise TaipanTypeError(f"Registered instance is not of type {str(type)}")
+        result = cast(type, self._memoized_instance)
+        return result
```

### Comparing `taipan_di-0.0.2/taipan_di/interfaces/base_dependency_container.py` & `taipan_di-0.0.3/taipan_di/interfaces/base_dependency_container.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.2/taipan_di/interfaces/base_dependency_provider.py` & `taipan_di-0.0.3/taipan_di/interfaces/base_scope.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import abc
 from typing import Type, TypeVar
 
+from .base_dependency_provider import BaseDependencyProvider
+
 T = TypeVar("T")
 
 
-class BaseDependencyProvider(metaclass=abc.ABCMeta):
+class BaseScope(metaclass=abc.ABCMeta):
     @classmethod
     def __subclasshook__(cls, subclass):
         return (
-            hasattr(subclass, "contains")
-            and callable(subclass.contains)
-            and hasattr(subclass, "resolve")
-            and callable(subclass.resolve)
+            hasattr(subclass, "get_instance")
+            and callable(subclass.get_instance)
             or NotImplemented
         )
 
     @abc.abstractmethod
-    def contains(self, type: Type[T]) -> bool:
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def resolve(self, type: Type[T]) -> T:
-        raise NotImplementedError
+    def get_instance(self, type: Type[T], container: BaseDependencyProvider) -> T:
+        raise NotImplementedError()
```

### Comparing `taipan_di-0.0.2/PKG-INFO` & `taipan_di-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: taipan-di
-Version: 0.0.2
+Version: 0.0.3
 Summary: Truly Amazing Inversion of control Python library Analogous to .Net's DI
 Home-page: https://github.com/Billuc/Taipan-DI
 License: MIT
 Keywords: taipan,dependency injection,dependency,python
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: typeguard (>=4.0.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.6.0,<5.0.0)
 Project-URL: Documentation, https://github.com/Billuc/Taipan-DI
 Project-URL: Repository, https://github.com/Billuc/Taipan-DI
 Description-Content-Type: text/markdown
 
 # Taipan-DI
```

