# Comparing `tmp/edge_orm-0.7.2.tar.gz` & `tmp/edge_orm-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_orm-0.7.2.tar", max compression
+gzip compressed data, was "edge_orm-0.8.1.tar", max compression
```

## Comparing `edge_orm-0.7.2.tar` & `edge_orm-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.7.2/README.md
--rw-r--r--   0        0        0      806 2023-04-19 18:28:11.434516 edge_orm-0.7.2/edge_orm/__init__.py
--rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.7.2/edge_orm/cache.py
--rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.7.2/edge_orm/errors.py
--rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.7.2/edge_orm/execute.py
--rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.7.2/edge_orm/external/encoders.py
--rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.7.2/edge_orm/helpers.py
--rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.7.2/edge_orm/logs.py
--rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.7.2/edge_orm/node/__init__.py
--rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.7.2/edge_orm/node/errors.py
--rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.7.2/edge_orm/node/models.py
--rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.7.2/edge_orm/resolver/__init__.py
--rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.7.2/edge_orm/resolver/enums.py
--rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.7.2/edge_orm/resolver/errors.py
--rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.7.2/edge_orm/resolver/merging.py
--rw-r--r--   0        0        0    42200 2023-05-29 17:49:40.834437 edge_orm-0.7.2/edge_orm/resolver/model.py
--rw-r--r--   0        0        0     5300 2023-05-26 15:22:47.425858 edge_orm-0.7.2/edge_orm/resolver/nested_resolvers.py
--rw-r--r--   0        0        0     3711 2023-04-13 17:11:22.267717 edge_orm-0.7.2/edge_orm/resolver/utils.py
--rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.7.2/edge_orm/span.py
--rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.7.2/edge_orm/types_generator/__init__.py
--rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.7.2/edge_orm/types_generator/introspection.py
--rw-r--r--   0        0        0    39663 2023-04-13 18:56:59.500577 edge_orm-0.7.2/edge_orm/types_generator/main.py
--rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.7.2/edge_orm/unset.py
--rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.7.2/edge_orm/validators.py
--rw-r--r--   0        0        0      785 2023-05-29 17:48:35.504338 edge_orm-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.8.1/README.md
+-rw-r--r--   0        0        0      842 2023-06-02 19:51:59.698747 edge_orm-0.8.1/edge_orm/__init__.py
+-rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.8.1/edge_orm/cache.py
+-rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.8.1/edge_orm/errors.py
+-rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.8.1/edge_orm/execute.py
+-rw-r--r--   0        0        0     5463 2023-06-02 18:07:35.502233 edge_orm-0.8.1/edge_orm/external/encoders.py
+-rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.8.1/edge_orm/helpers.py
+-rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.8.1/edge_orm/logs.py
+-rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.8.1/edge_orm/node/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.8.1/edge_orm/node/errors.py
+-rw-r--r--   0        0        0     4514 2023-06-02 17:45:03.025272 edge_orm-0.8.1/edge_orm/node/models.py
+-rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.8.1/edge_orm/resolver/__init__.py
+-rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.8.1/edge_orm/resolver/enums.py
+-rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.8.1/edge_orm/resolver/errors.py
+-rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.8.1/edge_orm/resolver/merging.py
+-rw-r--r--   0        0        0    42417 2023-06-02 18:10:30.983018 edge_orm-0.8.1/edge_orm/resolver/model.py
+-rw-r--r--   0        0        0     5300 2023-05-26 15:22:47.425858 edge_orm-0.8.1/edge_orm/resolver/nested_resolvers.py
+-rw-r--r--   0        0        0     3975 2023-06-02 18:08:35.542034 edge_orm-0.8.1/edge_orm/resolver/utils.py
+-rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.8.1/edge_orm/span.py
+-rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.8.1/edge_orm/types_generator/__init__.py
+-rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.8.1/edge_orm/types_generator/introspection.py
+-rw-r--r--   0        0        0    38602 2023-06-02 20:46:59.525691 edge_orm-0.8.1/edge_orm/types_generator/main.py
+-rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.8.1/edge_orm/unset.py
+-rw-r--r--   0        0        0     1080 2023-06-02 20:49:32.592882 edge_orm-0.8.1/edge_orm/validators.py
+-rw-r--r--   0        0        0      277 2023-06-02 20:41:12.570547 edge_orm-0.8.1/edge_orm/validators_v2.py
+-rw-r--r--   0        0        0      807 2023-06-02 20:51:14.974448 edge_orm-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 edge_orm-0.8.1/PKG-INFO
```

### Comparing `edge_orm-0.7.2/edge_orm/__init__.py` & `edge_orm-0.8.1/edge_orm/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ResolverException,
     CHANGES,
     CHANGES_D,
     ObjectNotFound,
     PermissionsError,
 )
 from .resolver import enums as resolver_enums
-from . import types_generator, validators
+from . import types_generator, validators, validators_v2
 from .execute import ExecuteConstraintViolationException, ExecuteException
 
 __all__ = [
     "UNSET",
     "UnsetType",
     "Node",
     "Insert",
@@ -28,8 +28,9 @@
     "resolver_enums",
     "create_logger",
     "logger",
     "types_generator",
     "validators",
     "ExecuteConstraintViolationException",
     "ExecuteException",
+    "validators_v2",
 ]
```

### Comparing `edge_orm-0.7.2/edge_orm/cache.py` & `edge_orm-0.8.1/edge_orm/cache.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.2/edge_orm/execute.py` & `edge_orm-0.8.1/edge_orm/execute.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.2/edge_orm/external/encoders.py` & `edge_orm-0.8.1/edge_orm/external/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
 from pydantic import BaseModel
-from pydantic.json import ENCODERS_BY_TYPE
+from pydantic.deprecated.json import ENCODERS_BY_TYPE
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
@@ -50,15 +50,15 @@
         include = set(include)
     if exclude is not None and not isinstance(exclude, (set, dict)):
         exclude = set(exclude)
     if isinstance(obj, BaseModel):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
-        obj_dict = obj.dict(
+        obj_dict = obj.model_dump(
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_none=exclude_none,
             exclude_defaults=exclude_defaults,
         )
```

### Comparing `edge_orm-0.7.2/edge_orm/helpers.py` & `edge_orm-0.8.1/edge_orm/helpers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.2/edge_orm/logs.py` & `edge_orm-0.8.1/edge_orm/logs.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.2/edge_orm/node/models.py` & `edge_orm-0.8.1/edge_orm/node/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     required: bool
 
 
 CONVERSION_MAP = dict[str, FieldInfo]
 
 
 class EdgeConfigBase(BaseModel):
-    model_name: str
+    edb_model_name: str
     client: AsyncIOClient
 
     updatable_fields: set[str]
     exclusive_fields: set[str]
 
     appendix_properties: set[str]
     computed_properties: set[str]
@@ -62,46 +62,46 @@
 
 class SetFields(BaseModel):
     _purged_unsets: bool = PrivateAttr(False)
 
     @property
     def set_fields_(self) -> set[str]:
         if not self._purged_unsets:
-            for key in self.__fields_set__.copy():
+            for key in self.model_fields_set.copy():
                 if getattr(self, key, None) is UNSET:
-                    self.__fields_set__.remove(key)
+                    self.model_fields_set.remove(key)
             self._purged_unsets = True
-        return self.__fields_set__
+        return self.model_fields_set
 
 
 class IgnoreUnset(SetFields):
     def __setattr__(self, key: T.Any, value: T.Any) -> None:
         if value is UNSET:
             return
         super().__setattr__(key, value)
 
 
 class Insert(IgnoreUnset):
     pass
 
     class Config:
-        allow_mutation = True
+        frozen = False
         validate_assignment = True
         arbitrary_types_allowed = True
-        anystr_strip_whitespace = True
+        str_strip_whitespace = True
 
 
 class Patch(IgnoreUnset):
     pass
 
     class Config:
-        allow_mutation = True
+        frozen = False
         validate_assignment = True
         arbitrary_types_allowed = True
-        anystr_strip_whitespace = True
+        str_strip_whitespace = True
 
 
 class classproperty(property):
     def __get__(self, owner_self, owner_cls):  # type: ignore
         return self.fget(owner_cls)  # type: ignore
 
 
@@ -165,10 +165,10 @@
     """
     @classproperty
     def Insert(self) -> T.Type[Insert]:  # example of how this could work
         return Insert
     """
 
     class Config:
-        allow_mutation = False
+        frozen = True
         validate_assignment = True
         arbitrary_types_allowed = True
```

### Comparing `edge_orm-0.7.2/edge_orm/resolver/merging.py` & `edge_orm-0.8.1/edge_orm/resolver/merging.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.2/edge_orm/resolver/model.py` & `edge_orm-0.8.1/edge_orm/resolver/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as T
 import json
 import re
 import uuid
 import edgedb
 from pydantic import BaseModel, PrivateAttr
-from pydantic.main import ModelMetaclass
+from pydantic._internal._model_construction import ModelMetaclass
 from edge_orm.node import Node, Insert, Patch, EdgeConfigBase
 from edge_orm.logs import logger
 from edge_orm.external import encoders
 from edge_orm import helpers, execute, span
 from . import enums, errors, utils
 from .nested_resolvers import NestedResolvers
 from devtools import debug
@@ -79,19 +79,25 @@
                 self.node_field_names()
                 - self._node_config.appendix_properties
                 - self._node_config.computed_properties
             )
 
     @property
     def model_name(self) -> str:
-        return self._node_config.model_name
+        return self._node_config.edb_model_name
 
     @classmethod
     def node_field_names(cls: T.Type[ThisResolverType]) -> set[str]:
-        return {field.alias for field in cls._node_cls.__fields__.values()}
+        field_names: set[str] = set()
+        for field_name, v in cls._node_cls.model_fields.items():
+            if alias := v.alias:
+                field_names.add(alias)
+            else:
+                field_names.add(field_name)
+        return field_names
 
     """RESOLVER BUILDING METHODS"""
 
     def set_update_operation(
         self: ThisResolverType,
         replace: bool = False,
         add: bool = False,
```

### Comparing `edge_orm-0.7.2/edge_orm/resolver/nested_resolvers.py` & `edge_orm-0.8.1/edge_orm/resolver/nested_resolvers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.2/edge_orm/resolver/utils.py` & `edge_orm-0.8.1/edge_orm/resolver/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,23 @@
         if not json_get_item
         else f'json_get({json_get_item}, "{field_name}")'
     )
     field_str = f"{field_name} := <{type_cast}>{var_field_name}"
     if isinstance(val, (dict, list)):
         if type_cast.endswith("::str") or type_cast.endswith("::json"):
             val = json.dumps(encoders.jsonable_encoder(val))
+        elif (
+            isinstance(val, list)
+            and type_cast.endswith("::str>")
+            or type_cast.endswith("::json>")
+        ):
+            # it is a list of Images, for example
+            val = [v.model_dump_json() for v in val]
     elif isinstance(val, BaseModel):
-        val = val.json()
+        val = val.model_dump_json()
     elif isinstance(val, set):
         val = list(val)
         field_str = (
             f"{field_name} := array_unpack(<array<{type_cast}>>{var_field_name})"
         )
     elif isinstance(val, Enum):
         val = val.value
```

### Comparing `edge_orm-0.7.2/edge_orm/span.py` & `edge_orm-0.8.1/edge_orm/span.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.2/edge_orm/types_generator/introspection.py` & `edge_orm-0.8.1/edge_orm/types_generator/introspection.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.2/edge_orm/types_generator/main.py` & `edge_orm-0.8.1/edge_orm/types_generator/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import typing as T
 from enum import Enum
 import os
 from pathlib import Path
 from black import format_str, FileMode
 import edgedb
-from pydantic import BaseModel, parse_raw_as, Field
+from pydantic import BaseModel, Field
 from .introspection import (
     introspect_objects,
     introspect_scalars,
     ObjectType,
     Link,
     Property,
 )
@@ -27,15 +27,14 @@
 class DBVendor(str, Enum):
     edgedb = "edgedb"
 
 
 class PropertyConfig(BaseModel):
     module_path: str
     module_name: str
-    validate_as_basemodel: bool = True
     cardinality: PropertyCardinality = PropertyCardinality.ONE
 
 
 class NodeConfig(BaseModel):
     module_path: str | None = None
     insert_path: str | None = None
     patch_path: str | None = None
@@ -97,17 +96,18 @@
         "import os",
         "import typing as T",
         "from enum import Enum",
         "from datetime import datetime, date, timedelta, time",
         "from uuid import UUID",
         "from decimal import Decimal",
         "from edgedb import RelativeDuration, AsyncIOClient, create_async_client",
-        "from pydantic import BaseModel, Field, PrivateAttr, validator",
+        "from pydantic import BaseModel, Field, PrivateAttr",
+        "from pydantic.functional_validators import BeforeValidator",
         f"from {PATH_TO_MODULE}.node.models import Cardinality, FieldInfo, classproperty",
-        f"from {PATH_TO_MODULE} import Node, Insert, Patch, EdgeConfigBase, Resolver, NodeException, ResolverException, UNSET, UnsetType, validators, errors, resolver_enums, CHANGES",
+        f"from {PATH_TO_MODULE} import Node, Insert, Patch, EdgeConfigBase, Resolver, NodeException, ResolverException, UNSET, UnsetType, validators_v2, errors, resolver_enums, CHANGES",
         "FilterConnector = resolver_enums.FilterConnector",
         f"from . import {enums_module} as enums",
         f"from .{client_module} import CLIENT",
     ]
     if resolver_mixin_path:
         lines.append(resolver_mixin_path)
     return "\n".join(lines)
@@ -315,15 +315,15 @@
     node_edgedb_conversion_map: CONVERSION_MAP,
     insert_edgedb_conversion_map: CONVERSION_MAP,
     patch_edgedb_conversion_map: CONVERSION_MAP,
     insert_link_conversion_map: CONVERSION_MAP,
 ) -> str:
     return f"""
 EdgeConfig: T.ClassVar[EdgeConfigBase] = EdgeConfigBase(
-    model_name = "{model_name}",
+    edb_model_name = "{model_name}",
     client = CLIENT,
 
     updatable_fields = {{{', '.join(add_quotes(sorted(list(updatable_fields))))}}},
     exclusive_fields = {{{', '.join(add_quotes(sorted(list(exclusive_fields))))}}},
 
     appendix_properties = {stringify_set(appendix_properties)},
     computed_properties = {stringify_set(computed_properties)},
@@ -422,40 +422,14 @@
     k = f_name
     if f_name in node_config.appendix_properties or f_name in computed_properties:
         k += "_"
     # also if it is a computed, add this
     return f'"{k}"'
 
 
-def build_from_str_validator_str(
-    node_config: NodeConfig | None, computed_properties: set[str]
-) -> str:
-    if node_config is None:
-        return ""
-    field_name_strs: T.List[str] = []
-
-    for field_name in node_config.custom_annotations.keys():
-        field_name_strs.append(key_from_field_name(field_name, node_config=node_config))
-    for field_name, props_config in node_config.basemodel_properties.items():
-        if props_config.validate_as_basemodel is False:
-            continue
-        field_name_strs.append(
-            key_from_field_name(
-                field_name,
-                node_config=node_config,
-                computed_properties=computed_properties,
-            )
-        )
-    if not field_name_strs:
-        return ""
-    return f"""
-_from_str = validator({", ".join(field_name_strs)}, pre=True, allow_reuse=True)(validators.from_str)
-    """
-
-
 ListType = T.TypeVar("ListType")
 
 
 def remove_falsies(lst: list[ListType]) -> list[ListType]:
     return [i for i in lst if i]
 
 
@@ -757,20 +731,16 @@
         property_strs=patch_property_strs,
         model_name=patch_model_name,
         insert_patch=InsertPatch.PATCH,
     )
 
     # node
     node_properties_str = "\n".join(property_strs)
-    from_str_validator_str = build_from_str_validator_str(
-        node_config=node_config, computed_properties=computed_properties
-    )
     if hydrate:
         node_properties_str = ""
-        from_str_validator_str = ""
 
     computed_property_getter_str = "\n".join(computed_property_getter_strs)
     node_conversion_map_str = f"_edgedb_conversion_map: T.Dict[str, T.Dict[str, T.Union[str, bool]]] = {stringify_dict(node_edgedb_conversion_map)}"
     insert_link_conversion_map_str = f"_link_conversion_map: T.Dict[str, T.Dict[str, T.Union[str, bool]]] = {stringify_dict(link_conversion_map)}"
     computed_properties_str = f"_computed_properties: T.ClassVar[T.Set[str]] = {stringify_set(computed_properties)}"
     appendix_properties_str = f"_appendix_properties: T.ClassVar[T.Set[str]] = {stringify_set(appendix_properties)}"
 
@@ -780,16 +750,14 @@
     node_link_functions_str = "\n".join(link_function_strs)
 
     if dehydrate:
         node_link_functions_str = ""
     node_inner_strs = [
         node_properties_str,
         "\n",
-        from_str_validator_str,
-        "\n",
         computed_property_getter_str,
         # node_conversion_map_str,
         # insert_link_conversion_map_str,
         # computed_properties_str,
         # appendix_properties_str,
         # basemodel_properties_str,
         # custom_annotations_str,
@@ -1010,15 +978,17 @@
     if config_path is not None and db_config_map is not None:
         raise GeneratorException(
             "Provide either a config_path or db_config_map, not both."
         )
     if config_path is not None:
         validate_output_path(output_path)
         all_config_json_str = open(config_path).read()
-        all_config_d = parse_raw_as(T.Dict[str, DBConfig], all_config_json_str)
+        all_config_d = {
+            k: DBConfig.model_validate_json(v) for k, v in all_config_json_str
+        }
     elif db_config_map is not None:
         all_config_d = db_config_map
     else:
         raise GeneratorException("Provide either a config_path or a config_model_map.")
     for db_name, db_config in all_config_d.items():
         if db_config.copy_config:
             db_config_to_copy = all_config_d[db_config.copy_config]
```

### Comparing `edge_orm-0.7.2/edge_orm/unset.py` & `edge_orm-0.8.1/edge_orm/unset.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.2/edge_orm/validators.py` & `edge_orm-0.8.1/edge_orm/validators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,13 @@
 import typing as T
-from pydantic import BaseModel, parse_raw_as
-from pydantic.fields import ModelField
-
-ModelType = T.TypeVar("ModelType", bound=BaseModel)
-
-
-def from_str(
-    cls: T.Type[BaseModel], v: str | ModelType, field: ModelField
-) -> ModelType | None:
-    if isinstance(v, str):
-        if v == "null":
-            return None
-        if field.sub_fields:
-            res = parse_raw_as(field.sub_fields[0].annotation, v)
-        else:
-            res = parse_raw_as(field.outer_type_, v)
-        return res
-    else:
-        return v
-
-
+from pydantic import BaseModel, FieldValidationInfo
+from devtools import debug
 from enum import Enum
 
+ModelType = T.TypeVar("ModelType", bound=BaseModel)
 EnumType = T.TypeVar("EnumType", bound=Enum)
 
 
 def transform_enum(
     original_value: str | Enum,
     new_enum_type: T.Type[EnumType],
     ignore_null: bool = False,
@@ -40,13 +22,16 @@
     new_value = (
         og_val.replace("/", "").replace("-", "_").replace("  ", " ").replace(" ", "_")
     )
     return new_enum_type(new_value)
 
 
 def enum_from_str(
-    cls: T.Type[BaseModel], v: EnumType | str, field: ModelField
+    cls: T.Type[BaseModel], v: EnumType | str, info: FieldValidationInfo
 ) -> EnumType | None:
+    # idk who uses this
+    field = cls.model_fields[info.field_name]
+    debug(field)
     if isinstance(v, str) or not isinstance(v, field.type_):
         return transform_enum(original_value=v, new_enum_type=field.type_)
     else:
         return v
```

### Comparing `edge_orm-0.7.2/pyproject.toml` & `edge_orm-0.8.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "edge-orm"
-version = "0.7.2"
+version = "0.8.1"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = "edge_orm" }]
 exclude = ["tests/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 edgedb = "^1.2.0"
-#pydantic = {version = ">=2.0a1", allow-prereleases = true}
-pydantic = { extras = ["email"], version = "^1.10" }
+pydantic = { version = ">=2.0b1", allow-prereleases = true, extras = ['email'] }
+#pydantic = { extras = ["email"], version = "^1.10" }
 orjson = "^3.8.0"
 devtools = "*"
 black = "*"
 
 
 mkdocs-material = { version = "^8.5.7", optional = true }
```

### Comparing `edge_orm-0.7.2/PKG-INFO` & `edge_orm-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: edge-orm
-Version: 0.7.2
+Version: 0.8.1
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: black
 Requires-Dist: devtools
 Requires-Dist: edgedb (>=1.2.0,<2.0.0)
 Requires-Dist: mkdocs-material (>=8.5.7,<9.0.0) ; extra == "docs"
 Requires-Dist: orjson (>=3.8.0,<4.0.0)
-Requires-Dist: pydantic[email] (>=1.10,<2.0)
+Requires-Dist: pydantic[email] (>=2.0b1)
 Description-Content-Type: text/markdown
 
 # edge orm
```

