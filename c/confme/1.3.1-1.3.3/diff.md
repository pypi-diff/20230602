# Comparing `tmp/confme-1.3.1.tar.gz` & `tmp/confme-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confme-1.3.1.tar", max compression
+gzip compressed data, was "confme-1.3.3.tar", max compression
```

## Comparing `confme-1.3.1.tar` & `confme-1.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1085 2022-01-21 15:01:39.964027 confme-1.3.1/LICENSE
--rw-r--r--   0        0        0     8192 2022-01-21 15:01:39.964027 confme-1.3.1/README.md
--rw-r--r--   0        0        0      238 2022-01-21 15:01:39.964027 confme-1.3.1/confme/__init__.py
--rw-r--r--   0        0        0      550 2022-01-21 15:01:39.964027 confme-1.3.1/confme/annotation.py
--rw-r--r--   0        0        0        0 2022-01-21 15:01:39.964027 confme-1.3.1/confme/core/__init__.py
--rw-r--r--   0        0        0     1076 2022-01-21 15:01:39.964027 confme-1.3.1/confme/core/argument_overwrite.py
--rw-r--r--   0        0        0     6487 2022-01-21 15:01:39.964027 confme-1.3.1/confme/core/base_config.py
--rw-r--r--   0        0        0      728 2022-01-21 15:01:39.968027 confme-1.3.1/confme/core/env_overwrite.py
--rw-r--r--   0        0        0     1988 2022-01-21 15:01:39.968027 confme-1.3.1/confme/core/global_config.py
--rw-r--r--   0        0        0    18170 2022-01-21 15:01:39.968027 confme-1.3.1/confme/pylintrc
--rw-r--r--   0        0        0      841 2022-01-21 15:01:39.968027 confme-1.3.1/confme/source_backend/__init__.py
--rw-r--r--   0        0        0      728 2022-01-21 15:01:39.968027 confme-1.3.1/confme/source_backend/backend_base.py
--rw-r--r--   0        0        0      847 2022-01-21 15:01:39.968027 confme-1.3.1/confme/source_backend/backend_yaml.py
--rw-r--r--   0        0        0        0 2022-01-21 15:01:39.968027 confme-1.3.1/confme/utils/__init__.py
--rw-r--r--   0        0        0      121 2022-01-21 15:01:39.968027 confme-1.3.1/confme/utils/base_exception.py
--rw-r--r--   0        0        0     1099 2022-01-21 15:01:39.968027 confme-1.3.1/confme/utils/dict_util.py
--rw-r--r--   0        0        0      832 2022-01-21 15:01:39.968027 confme-1.3.1/confme/utils/typing.py
--rw-r--r--   0        0        0     1332 2022-01-21 15:01:39.968027 confme-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     9223 2022-01-21 15:01:47.927342 confme-1.3.1/setup.py
--rw-r--r--   0        0        0     9438 2022-01-21 15:01:47.927872 confme-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-02 10:05:49.127710 confme-1.3.3/LICENSE
+-rw-r--r--   0        0        0     8192 2023-06-02 10:05:49.127710 confme-1.3.3/README.md
+-rw-r--r--   0        0        0      238 2023-06-02 10:05:49.127710 confme-1.3.3/confme/__init__.py
+-rw-r--r--   0        0        0      550 2023-06-02 10:05:49.127710 confme-1.3.3/confme/annotation.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/__init__.py
+-rw-r--r--   0        0        0     1076 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/argument_overwrite.py
+-rw-r--r--   0        0        0     6785 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/base_config.py
+-rw-r--r--   0        0        0      728 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/env_overwrite.py
+-rw-r--r--   0        0        0     2262 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/global_config.py
+-rw-r--r--   0        0        0    18170 2023-06-02 10:05:49.127710 confme-1.3.3/confme/pylintrc
+-rw-r--r--   0        0        0      841 2023-06-02 10:05:49.127710 confme-1.3.3/confme/source_backend/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-02 10:05:49.127710 confme-1.3.3/confme/source_backend/backend_base.py
+-rw-r--r--   0        0        0      847 2023-06-02 10:05:49.127710 confme-1.3.3/confme/source_backend/backend_yaml.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/base_exception.py
+-rw-r--r--   0        0        0      974 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/deprecated.py
+-rw-r--r--   0        0        0     1099 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/dict_util.py
+-rw-r--r--   0        0        0      832 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/typing.py
+-rw-r--r--   0        0        0     1353 2023-06-02 10:05:49.127710 confme-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     9443 1970-01-01 00:00:00.000000 confme-1.3.3/PKG-INFO
```

### Comparing `confme-1.3.1/LICENSE` & `confme-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/README.md` & `confme-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/confme/annotation.py` & `confme-1.3.3/confme/annotation.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/confme/core/argument_overwrite.py` & `confme-1.3.3/confme/core/argument_overwrite.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/confme/core/base_config.py` & `confme-1.3.3/confme/core/base_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,21 +38,23 @@
     def load_from_dict(cls, config_content: Dict) -> 'BaseConfig':
         config_content = recursive_update(config_content, env_overwrite(cls))
         config_content = recursive_update(config_content, argument_overwrite(cls))
 
         return cls.parse_obj(config_content)
 
     @classmethod
-    def register_folder(cls, config_folder: Path, default_env: str = None):
+    def register_folder(cls, config_folder: Path, default_env: str = None, strict: bool = False):
         """Register a folder where configuration files are drawn based on the environment.
         :param config_folder: Path to the folder with configuration files per environment
         :param default_env: Default environment that should be used if none is specified via environment variable
+        :param strict: If True, an exception is raised if no configuration file is found that exactly matches env name.
         """
         cls._config_path = config_folder
         cls._default_env = default_env
+        cls._strict = strict
         cls._cache = {}
 
     @classmethod
     def get(cls) -> T:
         """Get the corresponding configuration based on the environment. Thereby, the configuration class is loaded
         once and cached for subsequent calls.
         :return: instance of config_class with all values added from the config file
@@ -62,19 +64,22 @@
             cls._cache[env] = cls._load_file(env)
 
         return cls._cache[env]
 
     @classmethod
     def _load_file(cls, environment: str) -> T:
         files = Path(cls._config_path).glob(pattern='*')
-        selected_files = [f for f in files if environment in f.name]
+        if cls._strict:
+            selected_files = [f for f in files if f.name == environment]
+        else:
+            selected_files = [f for f in files if environment in f.name]
 
         if len(selected_files) <= 0:
-            raise Exception(f'No configuration found for environment {environment} in '
-                            f'files {files}')
+            raise ConfmeException(f'No configuration found for environment {environment} in '
+                                  f'files {files}')
         elif len(selected_files) > 1:
             logging.warning(f'More than one file found matching environment {environment} in'
                             f'files {files}. Using file {selected_files[0]}')
             file = selected_files[0]
         else:
             file = selected_files[0]
```

### Comparing `confme-1.3.1/confme/core/env_overwrite.py` & `confme-1.3.3/confme/core/env_overwrite.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/confme/core/global_config.py` & `confme-1.3.3/confme/core/global_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import logging
 import os
 from pathlib import Path
 from typing import Dict, TypeVar
 
 from confme import BaseConfig
+from confme.utils.deprecated import deprecated
+from confme.utils.base_exception import ConfmeException
 
 T = TypeVar('T', bound='BaseConfig')
 
 
+@deprecated(reason='GlobalConfig is not maintained anymore and all functionality is transferred to BaseConfig. '
+                   'Use BaseConfig instead.')
 class GlobalConfig(BaseConfig):
     _KEY_LOOKUP = ['env', 'environment', 'environ', 'stage']
     _config_path: Path = None
     _cache: Dict[str, T] = {}
 
     @classmethod
     def register_folder(cls, config_folder: Path):
@@ -28,16 +32,16 @@
 
     @classmethod
     def _load_file(cls, environment: str) -> T:
         files = Path(cls._config_path).glob(pattern='*')
         selected_files = [f for f in files if environment in f.name]
 
         if len(selected_files) <= 0:
-            raise Exception(f'No configuration found for environment {environment} in '
-                            f'files {files}')
+            raise ConfmeException(f'No configuration found for environment {environment} in '
+                                  f'files {files}')
         elif len(selected_files) > 1:
             logging.warning(f'More than one file found matching environment {environment} in'
                             f'files {files}. Using file {selected_files[0]}')
             file = selected_files[0]
         else:
             file = selected_files[0]
```

### Comparing `confme-1.3.1/confme/pylintrc` & `confme-1.3.3/confme/pylintrc`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/confme/source_backend/__init__.py` & `confme-1.3.3/confme/source_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/confme/source_backend/backend_base.py` & `confme-1.3.3/confme/source_backend/backend_base.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/confme/source_backend/backend_yaml.py` & `confme-1.3.3/confme/source_backend/backend_yaml.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/confme/utils/dict_util.py` & `confme-1.3.3/confme/utils/dict_util.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/confme/utils/typing.py` & `confme-1.3.3/confme/utils/typing.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.1/pyproject.toml` & `confme-1.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 [tool.poetry]
 name = "confme"
-version = "1.3.1"
+version = "1.3.3"
 description = "Easy configuration management in python"
 authors = ["Iwan Silvan Bolzern <iwan.bolzern@roche.com>"]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/iwanbolzern/confme"
 repository = "https://github.com/iwanbolzern/confme"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Healthcare Industry",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 packages = [
     { include = "confme" },
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7.2"
 pyyaml = "^5.3"
 pydantic = "^1.4"
 tabulate = "^0.8.9"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^6.1.2"
-pylint = "^2.4.4"
+pylint = "^2.17.4"
 sphinx = "^3.2.1"
 recommonmark = "^0.6.0"
 pytest-cov = "^2.11.1"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `confme-1.3.1/setup.py` & `confme-1.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,258 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: confme
+Version: 1.3.3
+Summary: Easy configuration management in python
+Home-page: https://github.com/iwanbolzern/confme
+License: LICENSE
+Author: Iwan Silvan Bolzern
+Author-email: iwan.bolzern@roche.com
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: pydantic (>=1.4,<2.0)
+Requires-Dist: pyyaml (>=5.3,<6.0)
+Requires-Dist: tabulate (>=0.8.9,<0.9.0)
+Project-URL: Repository, https://github.com/iwanbolzern/confme
+Description-Content-Type: text/markdown
 
-packages = \
-['confme', 'confme.core', 'confme.source_backend', 'confme.utils']
+# ConfMe: Configuration Made Easy 💖
 
-package_data = \
-{'': ['*']}
+[![image](https://img.shields.io/pypi/v/confme?color=blue)](https://pypi.org/project/confme/) [![image](https://img.shields.io/pypi/l/confme)](https://pypi.org/project/confme/) [![image](https://github.com/iwanbolzern/ConfMe/workflows/Test/badge.svg?branch=master)](https://pypi.org/project/confme/)
+[![image](https://img.shields.io/pypi/pyversions/confme?color=blue)](https://pypi.org/project/confme/)
 
-install_requires = \
-['pydantic>=1.4,<2.0', 'pyyaml>=5.3,<6.0', 'tabulate>=0.8.9,<0.9.0']
-
-setup_kwargs = {
-    'name': 'confme',
-    'version': '1.3.1',
-    'description': 'Easy configuration management in python',
-    'long_description': '# ConfMe: Configuration Made Easy 💖\n\n[![image](https://img.shields.io/pypi/v/confme?color=blue)](https://pypi.org/project/confme/) [![image](https://img.shields.io/pypi/l/confme)](https://pypi.org/project/confme/) [![image](https://github.com/iwanbolzern/ConfMe/workflows/Test/badge.svg?branch=master)](https://pypi.org/project/confme/)\n[![image](https://img.shields.io/pypi/pyversions/confme?color=blue)](https://pypi.org/project/confme/)\n\nConfMe is a simple to use, production ready application configuration management library, which takes into consideration the following three thoughts:\n1. Access to configuration values must be safe at runtime. **No ```myconfig[\'value1\'][\'subvalue\']``` anymore!**\n2. The configuration must be checked for consistency at startup e.g. type check, range check, ...\n3. Secrets shall be injectable from environment variables\n\nConfMe makes all these features possible with just a few type annotations on plain Python objects.\n\n## Installation\nConfMe can be installed from the official python package repository [pypi](https://pypi.org/project/confme/)\n\n```\npip install confme\n```\n\nOr, if you\'re using pipenv:\n\n```\npipenv install confme\n```\n\nOr, if you\'re using poetry:\n\n```\npoetry add confme\n```\n\n## Basic Usage of confme\nDefine your config structure as plain python objects with type annotations:\n\n```python\nfrom confme import BaseConfig\n\nclass DatabaseConfig(BaseConfig):\n    host: str\n    port: int\n    user: str\n\nclass MyConfig(BaseConfig):\n    name: str\n    database: DatabaseConfig\n```\n\nCreate a configuration yaml file with the same structure as your configuration classes have:\n\n```yaml\nname: "Database Application"\ndatabase:\n    host: "localhost"\n    port: 5000\n    user: "any-db-user"\n```\n\nLoad the yaml file into your Python object structure and access it in a secure manner:\n\n```python\nmy_config = MyConfig.load(\'config.yaml\')\n\nprint(f\'Using database connection {my_config.database.host} \'\n      f\'on port {my_config.database.port}\')\n```\n\nIn the background the yaml file is parsed and mapped to the defined object structure. While mapping the values to object properties, type checks are performed. If a value is not available or is not of the correct type, an error is generated already when the configuration is loaded.\n\n## Supported Annotations\nConfMe is based on pydantic and supports all annotations provided by pydantic. The most important annotations are listed and explain bellow. For the whole list, please checkout [Field Types](https://pydantic-docs.helpmanual.io/usage/types/):\n- str\n- int\n- float\n- bool\n- typing.List[x]\n- typing.Optional[x]\n- [Secret](#secret)\n- [Range](#range)\n- [Enum](#enum)\n\n### Secret\nWith the Secret annotation you can inject secrets from environment variables directly into your configuration structure. This is especially handy when you\'re deploying applications by using docker. Therefore, let\'s extend the previous example with a Secret annotation:\n\n```python\nfrom confme import BaseConfig\nfrom confme.annotation import Secret\n\nclass DatabaseConfig(BaseConfig):\n    ...\n    password: str = Secret(\'highSecurePassword\')\n```\n\nNow set the password to the defined environment variable:\n\n```bash\nexport highSecurePassword="This is my password"\n```\n\nLoad your config and check for the injected password.\n\n```\nmy_config = MyConfig.load(\'config.yaml\')\nprint(f\'My password is: {my_config.database.password}\')\n```\n\n### Range\n\nConfME supports OpenRange, ClosedRange and MixedRange values. The terms open and close are similar to open and closed intervals in mathematics. This means, if you want to include the lower and upper range use ClosedRange otherwise OpenRange:\n* ```ClosedRange(2, 3)``` will include 2 and 3\n* ```OpenRange(2, 3)``` will not include 2 and 3\n\nIf you want to have a mixture of both, e.g. include 2 but exclude 3 use MixedRange:\n* ```MixedRange(ge=2, lt=3)``` will include 2 but exclude 3\n\n```python\nfrom confme import BaseConfig\nfrom confme.annotation import ClosedRange\n\nclass DatabaseConfig(BaseConfig):\n    ...\n    password: int = ClosedRange(2, 3)\n```\n\n### Enum\n\nIf a Python Enum is set as type annotation, ConfMe expect to find the enum value in the configuration file.\n\n```python\nfrom confme import BaseConfig\nfrom enum import Enum\n\nclass DatabaseConnection(Enum):\n    TCP = \'tcp\'\n    UDP = \'udp\'\n\nclass DatabaseConfig(BaseConfig):\n    ...\n    connection_type: DatabaseConnection\n```\n\n## Switching configuration based on Environment\nA very common situation is that configurations must be changed based on the execution environment (dev, test, prod). This can be accomplished \nby registering a folder with one .yaml file per environment and seting the `ENV` environment variable to the value you need. An example could look \nlike this:  \n\nLet\'s assume we have three environments (dev, test, prod) and one configuration file per environment in the following folder structure:\n```\nproject\n│\n└───config\n│   │   my_prod_config.yaml\n│   │   my_test_config.yaml\n│   │   my_dev_config.yaml\n│   \n└───src\n│   │   app.py\n│   │   my_config.py\n```\nThe definition of `my_config.py` is equivalent to the one used in the basic introduction section and `app.py` uses our configuration the \nfollowing way:\n```python\n# we register the folder where ConfME can find the configuration files\nMyConfig.register_folder(Path(__file__).parent / \'../config\')\n...\n\n# we access the instance of the corresponding configuration file anywhere in our project. \nmy_config = MyConfig.get()\nprint(f\'Using database connection {my_config.database.host} \'\n      f\'on port {my_config.database.port}\')\n```\nIf now one of the following environment variables (precedence in descending order): `[\'env\', \'environment\', \'environ\', \'stage\']` is \nset e.g. `export ENV=prod` it will load the configuration file with `prod` in its name.\n\n## Parameter overwrite\nIn addition to loading configuration parameters from the configuration file, they can be passed/overwritten from the command line or environment variables. Thereby, the following precedences apply (lower number means higher precedence):\n1. **Command Line Arguments**: Check if parameter is set as command line argument. If not go one line done...\n2. **Environment Variables**: Check if parameter is set as environment variable. If not go one line done...\n3. **Configuration File**: If value was not found in one of the previous sources, it will check in the configuration file.\n\n### Overwrite Parameters from Command Line\nEspecially in the Data Science and Machine Learning area it is useful to pass certain parameters for experimental purposes as command line arguments. Therefore, all properties defined in the configuration classes are automatically offered as command line arguments in the following format:\n\n**my_program.py:**\n\n```python\nfrom confme import BaseConfig\n\nclass DatabaseConfig(BaseConfig):\n    host: str\n    port: int\n    user: str\n\nclass MyConfig(BaseConfig):\n    name: int\n    database: DatabaseConfig\n\nconfig = MyConfig.load(\'test.yaml\')\n```\n\nWhen you now start your program from the command line with the ```++help``` argument, you get the full list of all configuration options. **CAVEAT!** In order to not interfere with other cli tools, the prefix - was changed to +:\n```shell\n$ python my_program.py --help\nusage: my_program.py [+h] [++name NAME] [++database.host DATABASE.HOST] [++database.port DATABASE.PORT] [++database.user DATABASE.USER]\n\noptional arguments:\n  +h, ++help            show this help message and exit\n\nConfiguration Parameters:\n  With the parameters specified bellow, the configuration values from the config file can be overwritten.\n\n  ++name NAME\n  ++database.host DATABASE.HOST\n  ++database.port DATABASE.PORT\n  ++database.user DATABASE.USER\n```\n\n### Overwrite Parameters with Environment Variables\nLikewise to overwriting parameters from the commandline you can also overwrite by passing environment variables. Therefore, simply set the environment variable in the same format as it would be passed as command line arguments and run your application:\n```shell\n$ export database.host=localhost\n$ python my_programm.py\n```\n\n## LICENSE\n\nConfMe is released under the [MIT](LICENSE) license.\n\n',
-    'author': 'Iwan Silvan Bolzern',
-    'author_email': 'iwan.bolzern@roche.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/iwanbolzern/confme',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
+ConfMe is a simple to use, production ready application configuration management library, which takes into consideration the following three thoughts:
+1. Access to configuration values must be safe at runtime. **No ```myconfig['value1']['subvalue']``` anymore!**
+2. The configuration must be checked for consistency at startup e.g. type check, range check, ...
+3. Secrets shall be injectable from environment variables
+
+ConfMe makes all these features possible with just a few type annotations on plain Python objects.
+
+## Installation
+ConfMe can be installed from the official python package repository [pypi](https://pypi.org/project/confme/)
+
+```
+pip install confme
+```
+
+Or, if you're using pipenv:
+
+```
+pipenv install confme
+```
+
+Or, if you're using poetry:
+
+```
+poetry add confme
+```
+
+## Basic Usage of confme
+Define your config structure as plain python objects with type annotations:
+
+```python
+from confme import BaseConfig
+
+class DatabaseConfig(BaseConfig):
+    host: str
+    port: int
+    user: str
+
+class MyConfig(BaseConfig):
+    name: str
+    database: DatabaseConfig
+```
+
+Create a configuration yaml file with the same structure as your configuration classes have:
+
+```yaml
+name: "Database Application"
+database:
+    host: "localhost"
+    port: 5000
+    user: "any-db-user"
+```
+
+Load the yaml file into your Python object structure and access it in a secure manner:
+
+```python
+my_config = MyConfig.load('config.yaml')
+
+print(f'Using database connection {my_config.database.host} '
+      f'on port {my_config.database.port}')
+```
+
+In the background the yaml file is parsed and mapped to the defined object structure. While mapping the values to object properties, type checks are performed. If a value is not available or is not of the correct type, an error is generated already when the configuration is loaded.
+
+## Supported Annotations
+ConfMe is based on pydantic and supports all annotations provided by pydantic. The most important annotations are listed and explain bellow. For the whole list, please checkout [Field Types](https://pydantic-docs.helpmanual.io/usage/types/):
+- str
+- int
+- float
+- bool
+- typing.List[x]
+- typing.Optional[x]
+- [Secret](#secret)
+- [Range](#range)
+- [Enum](#enum)
+
+### Secret
+With the Secret annotation you can inject secrets from environment variables directly into your configuration structure. This is especially handy when you're deploying applications by using docker. Therefore, let's extend the previous example with a Secret annotation:
+
+```python
+from confme import BaseConfig
+from confme.annotation import Secret
+
+class DatabaseConfig(BaseConfig):
+    ...
+    password: str = Secret('highSecurePassword')
+```
+
+Now set the password to the defined environment variable:
+
+```bash
+export highSecurePassword="This is my password"
+```
+
+Load your config and check for the injected password.
+
+```
+my_config = MyConfig.load('config.yaml')
+print(f'My password is: {my_config.database.password}')
+```
+
+### Range
+
+ConfME supports OpenRange, ClosedRange and MixedRange values. The terms open and close are similar to open and closed intervals in mathematics. This means, if you want to include the lower and upper range use ClosedRange otherwise OpenRange:
+* ```ClosedRange(2, 3)``` will include 2 and 3
+* ```OpenRange(2, 3)``` will not include 2 and 3
+
+If you want to have a mixture of both, e.g. include 2 but exclude 3 use MixedRange:
+* ```MixedRange(ge=2, lt=3)``` will include 2 but exclude 3
+
+```python
+from confme import BaseConfig
+from confme.annotation import ClosedRange
+
+class DatabaseConfig(BaseConfig):
+    ...
+    password: int = ClosedRange(2, 3)
+```
+
+### Enum
+
+If a Python Enum is set as type annotation, ConfMe expect to find the enum value in the configuration file.
+
+```python
+from confme import BaseConfig
+from enum import Enum
+
+class DatabaseConnection(Enum):
+    TCP = 'tcp'
+    UDP = 'udp'
+
+class DatabaseConfig(BaseConfig):
+    ...
+    connection_type: DatabaseConnection
+```
+
+## Switching configuration based on Environment
+A very common situation is that configurations must be changed based on the execution environment (dev, test, prod). This can be accomplished 
+by registering a folder with one .yaml file per environment and seting the `ENV` environment variable to the value you need. An example could look 
+like this:  
+
+Let's assume we have three environments (dev, test, prod) and one configuration file per environment in the following folder structure:
+```
+project
+│
+└───config
+│   │   my_prod_config.yaml
+│   │   my_test_config.yaml
+│   │   my_dev_config.yaml
+│   
+└───src
+│   │   app.py
+│   │   my_config.py
+```
+The definition of `my_config.py` is equivalent to the one used in the basic introduction section and `app.py` uses our configuration the 
+following way:
+```python
+# we register the folder where ConfME can find the configuration files
+MyConfig.register_folder(Path(__file__).parent / '../config')
+...
+
+# we access the instance of the corresponding configuration file anywhere in our project. 
+my_config = MyConfig.get()
+print(f'Using database connection {my_config.database.host} '
+      f'on port {my_config.database.port}')
+```
+If now one of the following environment variables (precedence in descending order): `['env', 'environment', 'environ', 'stage']` is 
+set e.g. `export ENV=prod` it will load the configuration file with `prod` in its name.
+
+## Parameter overwrite
+In addition to loading configuration parameters from the configuration file, they can be passed/overwritten from the command line or environment variables. Thereby, the following precedences apply (lower number means higher precedence):
+1. **Command Line Arguments**: Check if parameter is set as command line argument. If not go one line done...
+2. **Environment Variables**: Check if parameter is set as environment variable. If not go one line done...
+3. **Configuration File**: If value was not found in one of the previous sources, it will check in the configuration file.
+
+### Overwrite Parameters from Command Line
+Especially in the Data Science and Machine Learning area it is useful to pass certain parameters for experimental purposes as command line arguments. Therefore, all properties defined in the configuration classes are automatically offered as command line arguments in the following format:
+
+**my_program.py:**
+
+```python
+from confme import BaseConfig
+
+class DatabaseConfig(BaseConfig):
+    host: str
+    port: int
+    user: str
+
+class MyConfig(BaseConfig):
+    name: int
+    database: DatabaseConfig
+
+config = MyConfig.load('test.yaml')
+```
+
+When you now start your program from the command line with the ```++help``` argument, you get the full list of all configuration options. **CAVEAT!** In order to not interfere with other cli tools, the prefix - was changed to +:
+```shell
+$ python my_program.py --help
+usage: my_program.py [+h] [++name NAME] [++database.host DATABASE.HOST] [++database.port DATABASE.PORT] [++database.user DATABASE.USER]
+
+optional arguments:
+  +h, ++help            show this help message and exit
+
+Configuration Parameters:
+  With the parameters specified bellow, the configuration values from the config file can be overwritten.
+
+  ++name NAME
+  ++database.host DATABASE.HOST
+  ++database.port DATABASE.PORT
+  ++database.user DATABASE.USER
+```
+
+### Overwrite Parameters with Environment Variables
+Likewise to overwriting parameters from the commandline you can also overwrite by passing environment variables. Therefore, simply set the environment variable in the same format as it would be passed as command line arguments and run your application:
+```shell
+$ export database.host=localhost
+$ python my_programm.py
+```
+
+## LICENSE
+
+ConfMe is released under the [MIT](LICENSE) license.
 
 
-setup(**setup_kwargs)
```

