# Comparing `tmp/pydantic_settings-2.0a4.tar.gz` & `tmp/pydantic_settings-2.0b1.tar.gz`

## Comparing `pydantic_settings-2.0a4.tar` & `pydantic_settings-2.0b1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/Makefile
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/.github/FUNDING.yml
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/.github/workflows/ci.yml
--rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/docs/index.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/__init__.py
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/py.typed
--rw-r--r--   0        0        0    20460 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/sources.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/utils.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/version.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/all.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/linting.in
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/linting.txt
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/pyproject.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/testing.in
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/testing.txt
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/tests/conftest.py
--rw-r--r--   0        0        0    45543 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/tests/test_settings.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/LICENSE
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/README.md
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pyproject.toml
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/Makefile
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    18908 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/docs/index.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/__init__.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/py.typed
+-rw-r--r--   0        0        0    20920 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/sources.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/utils.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pydantic_settings/version.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/all.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/linting.in
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/linting.txt
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/pyproject.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/testing.in
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/requirements/testing.txt
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/tests/conftest.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/tests/example_test_config.json
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/tests/test_docs.py
+-rw-r--r--   0        0        0    46791 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/tests/test_settings.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/LICENSE
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/README.md
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 pydantic_settings-2.0b1/PKG-INFO
```

### Comparing `pydantic_settings-2.0a4/.pre-commit-config.yaml` & `pydantic_settings-2.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a4/Makefile` & `pydantic_settings-2.0b1/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -5,22 +5,20 @@
 install:
 	python -m pip install -U pip
 	pip install -r requirements/all.txt
 	pip install -e .
 
 .PHONY: format
 format:
-	pyupgrade --py37-plus --exit-zero-even-if-changed `find $(sources) -name "*.py" -type f`
-	isort $(sources)
 	black $(sources)
+	ruff --fix $(sources)
 
 .PHONY: lint
 lint:
-	flake8 $(sources)
-	isort $(sources) --check-only --df
+	ruff $(sources)
 	black $(sources) --check --diff
 
 .PHONY: mypy
 mypy:
 	mypy pydantic_settings
 
 .PHONY: test
```

### Comparing `pydantic_settings-2.0a4/.github/workflows/ci.yml` & `pydantic_settings-2.0b1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a4/docs/index.md` & `pydantic_settings-2.0b1/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 If you create a model that inherits from `BaseSettings`, the model initialiser will attempt to determine
 the values of any fields not passed as keyword arguments by reading from the environment. (Default values
 will still be used if the matching environment variable is not set.)
 
 This makes it easy to:
 
 * Create a clearly-defined, type-hinted application configuration class
@@ -11,62 +12,64 @@
 For example:
 
 ```py
 from typing import Any, Callable, Set
 
 from pydantic import (
     AliasChoices,
+    AmqpDsn,
     BaseModel,
     ConfigDict,
+    Field,
     ImportString,
-    RedisDsn,
     PostgresDsn,
-    AmqpDsn,
-    Field,
+    RedisDsn,
 )
+
 from pydantic_settings import BaseSettings
 
 
 class SubModel(BaseModel):
     foo: str = 'bar'
     apple: int = 1
 
 
 class Settings(BaseSettings):
     auth_key: str = Field(validation_alias='my_auth_key')
     api_key: str = Field(validation_alias='my_api_key')
 
     redis_dsn: RedisDsn = Field(
         'redis://user:pass@localhost:6379/1',
-        validation_alias=AliasChoices('service_redis_dsn', 'redis_url')
+        validation_alias=AliasChoices('service_redis_dsn', 'redis_url'),
     )
     pg_dsn: PostgresDsn = 'postgres://user:pass@localhost:5432/foobar'
     amqp_dsn: AmqpDsn = 'amqp://user:pass@localhost:5672/'
 
     special_function: ImportString[Callable[[Any], Any]] = 'math.cos'
 
     # to override domains:
     # export my_prefix_domains='["foo.com", "bar.com"]'
     domains: Set[str] = set()
 
     # to override more_settings:
     # export my_prefix_more_settings='{"foo": "x", "apple": 1}'
     more_settings: SubModel = SubModel()
 
-    model_config = ConfigDict(env_prefix = 'my_prefix_')  # defaults to no prefix, i.e. ""
+    model_config = ConfigDict(env_prefix='my_prefix_')  # defaults to no prefix, i.e. ""
+
 
 print(Settings().model_dump())
 """
 {
     'auth_key': 'xxx',
     'api_key': 'xxx',
     'redis_dsn': Url('redis://user:pass@localhost:6379/1'),
     'pg_dsn': Url('postgres://user:pass@localhost:5432/foobar'),
     'amqp_dsn': Url('amqp://user:pass@localhost:5672/'),
-    'special_function': <built-in function cos>,
+    'special_function': math.cos,
     'domains': set(),
     'more_settings': {'foo': 'bar', 'apple': 1},
 }
 """
 ```
 
 ## Environment variable names
@@ -87,14 +90,15 @@
   * When specifying a `AliasChoices`, order matters: the first detected value is used.
   * For example, for `redis_dsn` above, `service_redis_dsn` would take precedence over `redis_url`.
 
 Case-sensitivity can be turned on through the `model_config`:
 
 ```py
 from pydantic import ConfigDict
+
 from pydantic_settings import BaseSettings
 
 
 class Settings(BaseSettings):
     redis_host: str = 'localhost'
 
     model_config = ConfigDict(case_sensitive=True)
@@ -139,14 +143,15 @@
 export SUB_MODEL__DEEP__V4=v4
 ```
 
 You could load a settings module thus:
 
 ```py
 from pydantic import BaseModel, ConfigDict
+
 from pydantic_settings import BaseSettings
 
 
 class DeepSubModel(BaseModel):
     v4: str
 
 
@@ -164,20 +169,15 @@
     model_config = ConfigDict(env_nested_delimiter='__')
 
 
 print(Settings().model_dump())
 """
 {
     'v0': '0',
-    'sub_model': {
-        'v1': 'json-1',
-        'v2': b'nested-2',
-        'v3': 3,
-        'deep': {'v4': 'v4'},
-    },
+    'sub_model': {'v1': 'json-1', 'v2': b'nested-2', 'v3': 3, 'deep': {'v4': 'v4'}},
 }
 """
 ```
 
 `env_nested_delimiter` can be configured via the `model_config` as shown above, or via the
 `_env_nested_delimiter` keyword argument on instantiation.
 
@@ -191,19 +191,26 @@
 
 ```py
 import json
 import os
 from typing import Any, List, Tuple, Type
 
 from pydantic.fields import FieldInfo
-from pydantic_settings import BaseSettings, EnvSettingsSource, PydanticBaseSettingsSource
+
+from pydantic_settings import (
+    BaseSettings,
+    EnvSettingsSource,
+    PydanticBaseSettingsSource,
+)
 
 
 class MyCustomSource(EnvSettingsSource):
-    def prepare_field_value(self, field_name: str, field: FieldInfo, value: Any, value_is_complex: bool) -> Any:
+    def prepare_field_value(
+        self, field_name: str, field: FieldInfo, value: Any, value_is_complex: bool
+    ) -> Any:
         if field_name == 'numbers':
             return [int(x) for x in value.split(',')]
         return json.loads(value)
 
 
 class Settings(BaseSettings):
     numbers: List[int]
@@ -246,25 +253,25 @@
 ```
 
 Once you have your `.env` file filled with variables, *pydantic* supports loading it in two ways:
 
 **1.** setting `env_file` (and `env_file_encoding` if you don't want the default encoding of your OS) on `model_config`
 in a `BaseSettings` class:
 
-```py
+```py test="skip" lint="skip"
 class Settings(BaseSettings):
     ...
 
     model_config = ConfigDict(env_file='.env', env_file_encoding = 'utf-8')
 ```
 
 **2.** instantiating a `BaseSettings` derived class with the `_env_file` keyword argument
 (and the `_env_file_encoding` if needed):
 
-```py
+```py test="skip" lint="skip"
 settings = Settings(_env_file='prod.env', _env_file_encoding='utf-8')
 ```
 
 In either case, the value of the passed argument can be any valid path or filename, either absolute or relative to the
 current working directory. From there, *pydantic* will handle everything for you by loading in your variables and
 validating them.
 
@@ -280,20 +287,26 @@
 while `.env` would be ignored.
 
 If you need to load multiple dotenv files, you can pass the file paths as a `list` or `tuple`.
 
 Later files in the list/tuple will take priority over earlier files.
 
 ```py
-from pydantic import BaseSettings
+from pydantic import ConfigDict
+
+from pydantic_settings import BaseSettings
+
 
 class Settings(BaseSettings):
     ...
 
-    model_config = ConfigDict(env_file=('.env', '.env.prod'))  # `.env.prod` takes priority over `.env`
+    model_config = ConfigDict(
+        # `.env.prod` takes priority over `.env`
+        env_file=('.env', '.env.prod')
+    )
 ```
 
 You can also use the keyword argument override to tell Pydantic not to load any file at all (even if one is set in
 the `model_config` class) by passing `None` as the instantiation keyword argument, e.g. `settings = Settings(_env_file=None)`.
 
 Because python-dotenv is used to parse the file, bash-like semantics such as `export` can be used which
 (depending on your OS and environment) may allow your dotenv file to also be used with `source`,
@@ -315,25 +328,25 @@
 super_secret_database_password
 ```
 
 Once you have your secret files, *pydantic* supports loading it in two ways:
 
 **1.** setting `secrets_dir` on `model_config` in a `BaseSettings` class to the directory where your secret files are stored:
 
-```py
+```py test="skip" lint="skip"
 class Settings(BaseSettings):
     ...
     database_password: str
 
     model_config = ConfigDict(secrets_dir='/var/run')
 ```
 
 **2.** instantiating a `BaseSettings` derived class with the `_secrets_dir` keyword argument:
 
-```py
+```py test="skip" lint="skip"
 settings = Settings(_secrets_dir='/var/run')
 ```
 
 In either case, the value of the passed argument can be any valid directory, either absolute or relative to the
 current working directory. **Note that a non existent directory will only generate a warning**.
 From there, *pydantic* will handle everything for you by loading in your variables and validating them.
 
@@ -347,15 +360,15 @@
 
 Docker Secrets can be used to provide sensitive configuration to an application running in a Docker container.
 To use these secrets in a *pydantic* application the process is simple. More information regarding creating, managing
 and using secrets in Docker see the official
 [Docker documentation](https://docs.docker.com/engine/reference/commandline/secret/).
 
 First, define your Settings
-```py
+```py test="skip" lint="skip"
 class Settings(BaseSettings):
     my_secret_data: str
 
     model_config = ConfigDict(secrets_dir='/run/secrets')
 ```
 !!! note
     By default Docker uses `/run/secrets` as the target mount point. If you want to use a different location, change
@@ -394,15 +407,17 @@
 
 ### Changing Priority
 
 The order of the returned callables decides the priority of inputs; first item is the highest priority.
 
 ```py
 from typing import Tuple, Type
+
 from pydantic import PostgresDsn
+
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 
 
 class Settings(BaseSettings):
     database_dsn: PostgresDsn
 
     @classmethod
@@ -431,42 +446,52 @@
 ```py
 import json
 from pathlib import Path
 from typing import Any, Dict, Tuple, Type
 
 from pydantic import ConfigDict
 from pydantic.fields import FieldInfo
+
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 
 
 class JsonConfigSettingsSource(PydanticBaseSettingsSource):
     """
     A simple settings source class that loads variables from a JSON file
     at the project's root.
 
     Here we happen to choose to use the `env_file_encoding` from Config
     when reading `config.json`
     """
 
-    def get_field_value(self, field: FieldInfo, field_name: str) -> Tuple[Any, str, bool]:
+    def get_field_value(
+        self, field: FieldInfo, field_name: str
+    ) -> Tuple[Any, str, bool]:
         encoding = self.config.get('env_file_encoding')
-        file_content_json = json.loads(Path('config.json').read_text(encoding))
+        file_content_json = json.loads(
+            Path('tests/example_test_config.json').read_text(encoding)
+        )
         fiel_value = file_content_json.get(field_name)
         return fiel_value, field_name, False
 
-
-    def prepare_field_value(self, field_name: str, field: FieldInfo, value: Any, value_is_complex: bool) -> Any:
+    def prepare_field_value(
+        self, field_name: str, field: FieldInfo, value: Any, value_is_complex: bool
+    ) -> Any:
         return value
 
     def __call__(self) -> Dict[str, Any]:
         d: Dict[str, Any] = {}
 
         for field_name, field in self.settings_cls.model_fields.items():
-            field_value, field_key, value_is_complex = self.get_field_value(field, field_name)
-            field_value = self.prepare_field_value(field_name, field, field_value, value_is_complex)
+            field_value, field_key, value_is_complex = self.get_field_value(
+                field, field_name
+            )
+            field_value = self.prepare_field_value(
+                field_name, field, field_value, value_is_complex
+            )
             if field_value is not None:
                 d[field_key] = field_value
 
         return d
 
 
 class Settings(BaseSettings):
@@ -488,24 +513,26 @@
             JsonConfigSettingsSource(settings_cls),
             env_settings,
             file_secret_settings,
         )
 
 
 print(Settings())
-#> foobar='spam'
+#> foobar='test'
 ```
 
 ### Removing sources
 
 You might also want to disable a source:
 
 ```py
 from typing import Tuple, Type
 
+from pydantic import ValidationError
+
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 
 
 class Settings(BaseSettings):
     my_api_key: str
 
     @classmethod
@@ -517,10 +544,18 @@
         dotenv_settings: PydanticBaseSettingsSource,
         file_secret_settings: PydanticBaseSettingsSource,
     ) -> Tuple[PydanticBaseSettingsSource, ...]:
         # here we choose to ignore arguments from init_settings
         return env_settings, file_secret_settings
 
 
-print(Settings(my_api_key='this is ignored'))
-# requires: `MY_API_KEY` env variable to be set, e.g. `export MY_API_KEY=xxx`
+try:
+    Settings(my_api_key='this is ignored')
+except ValidationError as exc_info:
+    print(exc_info)
+    """
+    1 validation error for Settings
+    my_api_key
+      Field required [type=missing, input_value={}, input_type=dict]
+        For further information visit https://errors.pydantic.dev/2/v/missing
+    """
 ```
```

### Comparing `pydantic_settings-2.0a4/pydantic_settings/main.py` & `pydantic_settings-2.0b1/pydantic_settings/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,8 +123,9 @@
         validate_default=True,
         case_sensitive=False,
         env_prefix='',
         env_file=None,
         env_file_encoding=None,
         env_nested_delimiter=None,
         secrets_dir=None,
+        protected_namespaces=('model_', 'settings_'),
     )
```

### Comparing `pydantic_settings-2.0a4/pydantic_settings/sources.py` & `pydantic_settings-2.0b1/pydantic_settings/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import json
 import os
 import warnings
 from abc import ABC, abstractmethod
 from collections import deque
 from dataclasses import is_dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, List, Mapping, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Any, List, Mapping, Sequence, Tuple, Union, cast
 
-from pydantic import BaseModel
+from pydantic import AliasChoices, AliasPath, BaseModel
 from pydantic._internal._typing_extra import origin_is_union
 from pydantic._internal._utils import deep_update, lenient_issubclass
 from pydantic.fields import FieldInfo
 from typing_extensions import get_origin
 
 from pydantic_settings.utils import path_type_label
 
@@ -89,15 +89,16 @@
 
 class InitSettingsSource(PydanticBaseSettingsSource):
     def __init__(self, settings_cls: type[BaseSettings], init_kwargs: dict[str, Any]):
         self.init_kwargs = init_kwargs
         super().__init__(settings_cls)
 
     def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
-        pass
+        # Nothing to do here. Only implement the return statement to make mypy happy
+        return None, '', False
 
     def __call__(self) -> dict[str, Any]:
         return self.init_kwargs
 
     def __repr__(self) -> str:
         return f'InitSettingsSource(init_kwargs={self.init_kwargs!r})'
 
@@ -117,27 +118,31 @@
               is complex and has to be parsed.
 
         Args:
             field (FieldInfo): The field.
             field_name (str): The field name.
 
         Returns:
-            list[tuple[str, str, bool]]: List of tuples, each tuple contanis field_key, env_name, and value_is_complex.
+            list[tuple[str, str, bool]]: List of tuples, each tuple contains field_key, env_name, and value_is_complex.
         """
         field_info: list[tuple[str, str, bool]] = []
-        v_alias = field.validation_alias
+        if isinstance(field.validation_alias, (AliasChoices, AliasPath)):
+            v_alias: str | list[str | int] | list[list[str | int]] | None = field.validation_alias.convert_to_aliases()
+        else:
+            v_alias = field.validation_alias
 
         if v_alias:
             if isinstance(v_alias, list):  # AliasChoices, AliasPath
                 for alias in v_alias:
                     if isinstance(alias, str):  # AliasPath
                         field_info.append((alias, self._apply_case_sensitive(alias), True if len(alias) > 1 else False))
                     elif isinstance(alias, list):  # AliasChoices
+                        first_arg = cast(str, alias[0])  # first item of an AliasChoices must be a str
                         field_info.append(
-                            (alias[0], self._apply_case_sensitive(alias[0]), True if len(alias) > 1 else False)
+                            (first_arg, self._apply_case_sensitive(first_arg), True if len(alias) > 1 else False)
                         )
             else:  # string validation alias
                 field_info.append((v_alias, self._apply_case_sensitive(v_alias), False))
         else:
             field_info.append(
                 (field_name, self._apply_case_sensitive(self.config.get('env_prefix', '') + field_name), False)
             )
@@ -465,15 +470,15 @@
                 )
 
         return dotenv_vars
 
     def __call__(self) -> dict[str, Any]:
         data: dict[str, Any] = super().__call__()
 
-        data_lower_keys: List[str] = []
+        data_lower_keys: list[str] = []
         if not self.settings_cls.model_config.get('case_sensitive', False):
             data_lower_keys = [x.lower() for x in data.keys()]
 
         # As `extra` config is allowed in dotenv settings source, We have to
         # update data with extra env variabels from dotenv file.
         for env_name, env_value in self.env_vars.items():
             if env_value is not None:
@@ -528,13 +533,13 @@
         or _annotation_is_complex_inner(origin)
         or hasattr(origin, '__pydantic_core_schema__')
         or hasattr(origin, '__get_pydantic_core_schema__')
     )
 
 
 def _annotation_is_complex_inner(annotation: type[Any] | None) -> bool:
-    if lenient_issubclass(annotation, str):
+    if lenient_issubclass(annotation, (str, bytes)):
         return False
 
     return lenient_issubclass(annotation, (BaseModel, Mapping, Sequence, tuple, set, frozenset, deque)) or is_dataclass(
         annotation
     )
```

### Comparing `pydantic_settings-2.0a4/pydantic_settings/utils.py` & `pydantic_settings-2.0b1/pydantic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a4/requirements/linting.txt` & `pydantic_settings-2.0b1/requirements/linting.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,70 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.7
+# by the following command:
 #
 #    pip-compile --output-file=requirements/linting.txt requirements/linting.in
 #
-attrs==22.1.0
-    # via hypothesis
-black==22.8.0
+black==23.3.0
     # via -r requirements/linting.in
 cfgv==3.3.1
     # via pre-commit
 click==8.1.3
     # via black
 distlib==0.3.6
     # via virtualenv
-exceptiongroup==1.0.0rc9
-    # via hypothesis
-filelock==3.8.0
+filelock==3.12.0
     # via virtualenv
-flake8==5.0.4
-    # via
-    #   -r requirements/linting.in
-    #   flake8-pyproject
-    #   flake8-quotes
-flake8-pyproject==1.1.0.post0
-    # via -r requirements/linting.in
-flake8-quotes==3.3.1
-    # via -r requirements/linting.in
-hypothesis==6.54.4
-    # via -r requirements/linting.in
-identify==2.5.3
+identify==2.5.24
     # via pre-commit
-isort==5.10.1
-    # via -r requirements/linting.in
-mccabe==0.7.0
-    # via flake8
-mypy==0.971
+importlib-metadata==6.6.0
+    # via
+    #   click
+    #   pre-commit
+    #   virtualenv
+mypy==1.3.0
     # via -r requirements/linting.in
-mypy-extensions==0.4.3
+mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
-pathspec==0.10.1
+packaging==23.1
+    # via black
+pathspec==0.11.1
     # via black
-platformdirs==2.5.2
+platformdirs==3.5.1
     # via
     #   black
     #   virtualenv
-pre-commit==2.20.0
+pre-commit==2.21.0
     # via -r requirements/linting.in
-pycodestyle==2.9.1
-    # via flake8
-pyflakes==2.5.0
-    # via flake8
-pyupgrade==2.37.3
+pyupgrade==3.3.2
     # via -r requirements/linting.in
 pyyaml==6.0
     # via pre-commit
-sortedcontainers==2.4.0
-    # via hypothesis
-tokenize-rt==4.2.1
+ruff==0.0.270
+    # via -r requirements/linting.in
+tokenize-rt==5.0.0
     # via pyupgrade
-toml==0.10.2
-    # via pre-commit
 tomli==2.0.1
     # via
     #   black
-    #   flake8-pyproject
     #   mypy
-typing-extensions==4.5.0
-    # via mypy
-virtualenv==20.16.4
+typed-ast==1.5.4
+    # via
+    #   black
+    #   mypy
+typing-extensions==4.6.2
+    # via
+    #   black
+    #   importlib-metadata
+    #   mypy
+    #   platformdirs
+virtualenv==20.23.0
     # via pre-commit
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `pydantic_settings-2.0a4/tests/test_settings.py` & `pydantic_settings-2.0b1/tests/test_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     AliasPath,
     BaseModel,
     ConfigDict,
     Field,
     HttpUrl,
     SecretStr,
     ValidationError,
+)
+from pydantic import (
     dataclasses as pydantic_dataclasses,
 )
 from pydantic.fields import FieldInfo
 from typing_extensions import Annotated
 
 from pydantic_settings import (
     BaseSettings,
@@ -53,15 +55,17 @@
     s = SimpleSettings(apple='goodbye')
     assert s.apple == 'goodbye'
 
 
 def test_sub_env_missing():
     with pytest.raises(ValidationError) as exc_info:
         SimpleSettings()
-    assert exc_info.value.errors() == [{'type': 'missing', 'loc': ('apple',), 'msg': 'Field required', 'input': {}}]
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'missing', 'loc': ('apple',), 'msg': 'Field required', 'input': {}}
+    ]
 
 
 def test_other_setting():
     with pytest.raises(ValidationError):
         SimpleSettings(apple='a', foobar=42)
 
 
@@ -223,15 +227,15 @@
     env.set('apples', '["russet", "granny smith"]')
     s = AnnotatedComplexSettings()
     assert s.apples == ['russet', 'granny smith']
 
     env.set('apples', '["russet"]')
     with pytest.raises(ValidationError) as exc_info:
         AnnotatedComplexSettings()
-    assert exc_info.value.errors() == [
+    assert exc_info.value.errors(include_url=False) == [
         {
             'ctx': {'actual_length': 1, 'field_type': 'List', 'min_length': 2},
             'input': ['russet'],
             'loc': ('apples',),
             'msg': 'List should have at least 2 items after validation, not 1',
             'type': 'too_short',
         }
@@ -288,15 +292,15 @@
     env.set('field', '{"x": 1}')
     s = ComplexSettings()
     assert s.field.x == 1
 
     env.set('field', '{"x": "a"}')
     with pytest.raises(ValidationError) as exc_info:
         ComplexSettings()
-    assert exc_info.value.errors() == [
+    assert exc_info.value.errors(include_url=False) == [
         {
             'input': 'a',
             'loc': ('field', 'x'),
             'msg': 'Input should be a valid integer, unable to parse string as an integer',
             'type': 'int_parsing',
         }
     ]
@@ -314,15 +318,15 @@
     env.set('field', '{"x": 1}')
     s = ComplexSettings()
     assert s.field.x == 1
 
     env.set('field', '{"x": "a"}')
     with pytest.raises(ValidationError) as exc_info:
         ComplexSettings()
-    assert exc_info.value.errors() == [
+    assert exc_info.value.errors(include_url=False) == [
         {
             'input': 'a',
             'loc': ('field', 'x'),
             'msg': 'Input should be a valid integer, unable to parse string as an integer',
             'type': 'int_parsing',
         }
     ]
@@ -340,15 +344,15 @@
     env.set('field', '{"x": 1}')
     s = ComplexSettings()
     assert s.field.x == 1
 
     env.set('field', '{"x": "a"}')
     with pytest.raises(ValidationError) as exc_info:
         ComplexSettings()
-    assert exc_info.value.errors() == [
+    assert exc_info.value.errors(include_url=False) == [
         {
             'input': 'a',
             'loc': ('field', 'x'),
             'msg': 'Input should be a valid integer, unable to parse string as an integer',
             'type': 'int_parsing',
         }
     ]
@@ -503,15 +507,17 @@
         foobar: str = Field(validation_alias='foo')
 
         model_config = ConfigDict(env_prefix='p_')
 
     env.set('p_foo', 'bar')
     with pytest.raises(ValidationError) as exc_info:
         Settings()
-    assert exc_info.value.errors() == [{'type': 'missing', 'loc': ('foo',), 'msg': 'Field required', 'input': {}}]
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'missing', 'loc': ('foo',), 'msg': 'Field required', 'input': {}}
+    ]
 
     env.set('foo', 'bar')
     assert Settings().foobar == 'bar'
 
 
 def test_case_sensitive(monkeypatch):
     class Settings(BaseSettings):
@@ -519,15 +525,17 @@
 
         model_config = ConfigDict(case_sensitive=True)
 
     # Need to patch os.environ to get build to work on Windows, where os.environ is case insensitive
     monkeypatch.setattr(os, 'environ', value={'Foo': 'foo'})
     with pytest.raises(ValidationError) as exc_info:
         Settings()
-    assert exc_info.value.errors() == [{'type': 'missing', 'loc': ('foo',), 'msg': 'Field required', 'input': {}}]
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'missing', 'loc': ('foo',), 'msg': 'Field required', 'input': {}}
+    ]
 
 
 def test_nested_dataclass(env):
     @pydantic_dataclasses.dataclass
     class MyDataclass:
         foo: int
         bar: str
@@ -680,15 +688,15 @@
         b: str
         c: str
 
         model_config = ConfigDict(env_file=p, case_sensitive=True, extra='ignore')
 
     with pytest.raises(ValidationError) as exc_info:
         Settings()
-    assert exc_info.value.errors() == [
+    assert exc_info.value.errors(include_url=False) == [
         {
             'type': 'missing',
             'loc': ('a',),
             'msg': 'Field required',
             'input': {'b': 'better string', 'c': 'best string', 'A': 'good string'},
         }
     ]
@@ -1123,15 +1131,17 @@
         foo: str
 
         model_config = ConfigDict(secrets_dir=tmp_path)
 
     with pytest.raises(ValidationError) as exc_info:
         Settings()
 
-    assert exc_info.value.errors() == [{'type': 'missing', 'loc': ('foo',), 'msg': 'Field required', 'input': {}}]
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'missing', 'loc': ('foo',), 'msg': 'Field required', 'input': {}}
+    ]
 
 
 def test_secrets_invalid_secrets_dir(tmp_path):
     p1 = tmp_path / 'foo'
     p1.write_text('foo_secret_value_str')
 
     class Settings(BaseSettings):
@@ -1542,15 +1552,15 @@
     class Settings(BaseSettings):
         a: str
 
         model_config = ConfigDict(env_file=p, extra='forbid')
 
     with pytest.raises(ValidationError) as exc_info:
         Settings()
-    assert exc_info.value.errors() == [
+    assert exc_info.value.errors(include_url=False) == [
         {'type': 'extra_forbidden', 'loc': ('x',), 'msg': 'Extra inputs are not permitted', 'input': 'y'}
     ]
 
 
 @pytest.mark.skipif(not dotenv, reason='python-dotenv not installed')
 def test_dotenv_extra_case_insensitive(tmp_path):
     p = tmp_path / '.env'
@@ -1578,7 +1588,45 @@
         sub_MODEL: SubModel
 
         model_config = ConfigDict(env_file=p, extra='forbid')
 
     s = Settings()
     assert s.A == 'b'
     assert s.sub_MODEL.v == 'v1'
+
+
+def test_nested_bytes_field(env):
+    class SubModel(BaseModel):
+        v1: str
+        v2: bytes
+
+    class Settings(BaseSettings):
+        v0: str
+        sub_model: SubModel
+
+        model_config = ConfigDict(env_nested_delimiter='__', env_prefix='TEST_')
+
+    env.set('TEST_V0', 'v0')
+    env.set('TEST_SUB_MODEL__V1', 'v1')
+    env.set('TEST_SUB_MODEL__V2', 'v2')
+
+    s = Settings()
+
+    assert s.v0 == 'v0'
+    assert s.sub_model.v1 == 'v1'
+    assert s.sub_model.v2 == b'v2'
+
+
+def test_protected_namespace_defaults():
+    # pydantic default
+    with pytest.raises(NameError, match='Field "model_prefixed_field" has conflict with protected namespace "model_"'):
+
+        class Model(BaseSettings):
+            model_prefixed_field: str
+
+    # pydantic-settings default
+    with pytest.raises(
+        NameError, match='Field "settings_prefixed_field" has conflict with protected namespace "settings_"'
+    ):
+
+        class Model1(BaseSettings):
+            settings_prefixed_field: str
```

### Comparing `pydantic_settings-2.0a4/LICENSE` & `pydantic_settings-2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a4/README.md` & `pydantic_settings-2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a4/pyproject.toml` & `pydantic_settings-2.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     'Environment :: Console',
     'Environment :: MacOS X',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 requires-python = '>=3.7'
 dependencies = [
-    'pydantic==v2.0a3',
+    'pydantic>=2.0b1',
     'python-dotenv>=0.21.0',
 ]
 dynamic = ['version']
 
 [project.urls]
 Homepage = 'https://github.com/pydantic/pydantic-settings'
 Funding = 'https://github.com/sponsors/samuelcolvin'
@@ -55,21 +55,14 @@
 [tool.pytest.ini_options]
 testpaths = 'tests'
 filterwarnings = [
     'error',
     'ignore:This is a placeholder until pydantic-settings.*:UserWarning',
 ]
 
-[tool.flake8]
-max_line_length = 120
-max_complexity = 14
-inline_quotes = 'single'
-multiline_quotes = 'double'
-ignore = ['E203', 'W503']
-
 [tool.coverage.run]
 source = ['pydantic_settings']
 branch = true
 context = '${CONTEXT}'
 
 [tool.coverage.report]
 precision = 2
@@ -82,29 +75,28 @@
 ]
 
 [tool.coverage.paths]
 source = [
     'pydantic_settings/',
 ]
 
+[tool.ruff]
+line-length = 120
+extend-select = ['Q', 'RUF100', 'C90', 'UP', 'I']
+flake8-quotes = {inline-quotes = 'single', multiline-quotes = 'double'}
+mccabe = { max-complexity = 14 }
+isort = { known-first-party = ['pydantic_settings', 'tests'] }
+target-version = 'py37'
+
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
 
-[tool.isort]
-line_length = 120
-known_first_party = 'pydantic_settings'
-known_third_party = 'pydantic'
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-combine_as_imports = true
-
 [tool.mypy]
 python_version = '3.10'
 show_error_codes = true
 follow_imports = 'silent'
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
```

### Comparing `pydantic_settings-2.0a4/PKG-INFO` & `pydantic_settings-2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-settings
-Version: 2.0a4
+Version: 2.0b1
 Summary: Settings management using Pydantic
 Project-URL: Homepage, https://github.com/pydantic/pydantic-settings
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic-settings
 Project-URL: Changelog, https://github.com/pydantic/pydantic-settings/releases
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>
 License-Expression: MIT
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: pydantic==v2.0a3
+Requires-Dist: pydantic>=2.0b1
 Requires-Dist: python-dotenv>=0.21.0
 Description-Content-Type: text/markdown
 
 # pydantic-settings
 
 [![CI](https://github.com/pydantic/pydantic-settings/workflows/CI/badge.svg?event=push)](https://github.com/pydantic/pydantic-settings/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![Coverage](https://codecov.io/gh/pydantic/pydantic-settings/branch/main/graph/badge.svg)](https://codecov.io/gh/pydantic/pydantic-settings)
```

