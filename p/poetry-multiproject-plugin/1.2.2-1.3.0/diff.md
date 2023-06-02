# Comparing `tmp/poetry_multiproject_plugin-1.2.2.tar.gz` & `tmp/poetry_multiproject_plugin-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_multiproject_plugin-1.2.2.tar", max compression
+gzip compressed data, was "poetry_multiproject_plugin-1.3.0.tar", max compression
```

## Comparing `poetry_multiproject_plugin-1.2.2.tar` & `poetry_multiproject_plugin-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1068 2022-01-23 14:15:18.822524 poetry_multiproject_plugin-1.2.2/LICENSE
--rw-r--r--   0        0        0     5409 2023-02-13 19:04:54.429748 poetry_multiproject_plugin-1.2.2/README.md
--rw-r--r--   0        0        0      122 2022-10-30 09:31:55.254657 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/__init__.py
--rw-r--r--   0        0        0        0 2022-01-27 21:12:19.215558 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/__init__.py
--rw-r--r--   0        0        0       92 2022-10-29 17:34:08.279274 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/buildproject/__init__.py
--rw-r--r--   0        0        0     2848 2023-02-15 17:23:23.134947 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/buildproject/project.py
--rw-r--r--   0        0        0       88 2022-12-26 11:25:28.111604 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/checkproject/__init__.py
--rw-r--r--   0        0        0     2462 2023-01-06 16:42:40.541575 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/checkproject/check.py
--rw-r--r--   0        0        0        0 2022-10-29 17:34:08.280190 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/__init__.py
--rw-r--r--   0        0        0      118 2022-12-26 11:25:28.113080 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/check/__init__.py
--rw-r--r--   0        0        0     1080 2023-01-06 16:42:40.542392 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/check/mypy_checker.py
--rw-r--r--   0        0        0      106 2022-12-27 09:13:24.664513 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/deps/__init__.py
--rw-r--r--   0        0        0      683 2023-01-06 22:56:24.237617 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/deps/installer.py
--rw-r--r--   0        0        0      111 2023-02-13 19:04:54.452935 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/parsing/__init__.py
--rw-r--r--   0        0        0     1713 2023-05-22 19:10:23.672824 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/parsing/rewrite.py
--rw-r--r--   0        0        0      141 2022-10-29 17:34:08.281001 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/__init__.py
--rw-r--r--   0        0        0      274 2022-12-28 08:58:51.305973 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/cleanup.py
--rw-r--r--   0        0        0      541 2023-05-22 19:10:23.673577 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/create.py
--rw-r--r--   0        0        0      304 2022-12-26 11:25:28.115615 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/dist.py
--rw-r--r--   0        0        0      875 2023-02-13 19:04:54.455402 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/packages.py
--rw-r--r--   0        0        0     1016 2023-02-13 19:04:54.456329 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/prepare.py
--rw-r--r--   0        0        0      125 2022-10-29 17:34:08.284437 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/__init__.py
--rw-r--r--   0        0        0     1634 2023-02-13 19:04:54.457639 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/generate.py
--rw-r--r--   0        0        0      592 2023-02-12 16:50:12.589435 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/packages.py
--rw-r--r--   0        0        0      631 2023-02-13 19:04:54.458759 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/read.py
--rw-r--r--   0        0        0      909 2022-12-26 11:25:28.122982 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/plugin.py
--rw-r--r--   0        0        0      841 2023-05-22 19:10:23.674333 poetry_multiproject_plugin-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 poetry_multiproject_plugin-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-01-23 14:15:18.822524 poetry_multiproject_plugin-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6182 2023-06-02 16:10:42.637369 poetry_multiproject_plugin-1.3.0/README.md
+-rw-r--r--   0        0        0      122 2022-10-30 09:31:55.254657 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-27 21:12:19.215558 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/__init__.py
+-rw-r--r--   0        0        0       92 2022-10-29 17:34:08.279274 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/buildproject/__init__.py
+-rw-r--r--   0        0        0     2848 2023-02-15 17:23:23.134947 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/buildproject/project.py
+-rw-r--r--   0        0        0       88 2022-12-26 11:25:28.111604 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/checkproject/__init__.py
+-rw-r--r--   0        0        0     2462 2023-01-06 16:42:40.541575 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/checkproject/check.py
+-rw-r--r--   0        0        0        0 2022-10-29 17:34:08.280190 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/__init__.py
+-rw-r--r--   0        0        0      118 2022-12-26 11:25:28.113080 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/check/__init__.py
+-rw-r--r--   0        0        0     1080 2023-01-06 16:42:40.542392 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/check/mypy_checker.py
+-rw-r--r--   0        0        0      106 2022-12-27 09:13:24.664513 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/deps/__init__.py
+-rw-r--r--   0        0        0      683 2023-01-06 22:56:24.237617 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/deps/installer.py
+-rw-r--r--   0        0        0      111 2023-02-13 19:04:54.452935 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/parsing/__init__.py
+-rw-r--r--   0        0        0     1775 2023-06-02 15:48:12.775242 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/parsing/rewrite.py
+-rw-r--r--   0        0        0      141 2022-10-29 17:34:08.281001 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/__init__.py
+-rw-r--r--   0        0        0      274 2022-12-28 08:58:51.305973 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/cleanup.py
+-rw-r--r--   0        0        0      541 2023-05-22 19:10:23.673577 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/create.py
+-rw-r--r--   0        0        0      304 2022-12-26 11:25:28.115615 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/dist.py
+-rw-r--r--   0        0        0      875 2023-02-13 19:04:54.455402 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/packages.py
+-rw-r--r--   0        0        0     1028 2023-06-02 15:48:12.776344 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/prepare.py
+-rw-r--r--   0        0        0      125 2022-10-29 17:34:08.284437 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/__init__.py
+-rw-r--r--   0        0        0     1634 2023-02-13 19:04:54.457639 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/generate.py
+-rw-r--r--   0        0        0      592 2023-02-12 16:50:12.589435 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/packages.py
+-rw-r--r--   0        0        0      631 2023-02-13 19:04:54.458759 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/read.py
+-rw-r--r--   0        0        0      909 2022-12-26 11:25:28.122982 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/plugin.py
+-rw-r--r--   0        0        0      841 2023-06-02 16:10:42.638022 poetry_multiproject_plugin-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6938 1970-01-01 00:00:00.000000 poetry_multiproject_plugin-1.3.0/PKG-INFO
```

### Comparing `poetry_multiproject_plugin-1.2.2/LICENSE` & `poetry_multiproject_plugin-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/README.md` & `poetry_multiproject_plugin-1.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Poetry Multiproject Plugin
 
 This is a Python `Poetry` plugin, adding the `build-project` and `check-project` commands.
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/DavidVujic/poetry-multiproject-plugin/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/DavidVujic/poetry-multiproject-plugin/tree/main)
 
+[![CodeScene Code Health](https://codescene.io/projects/36629/status-badges/code-health)](https://codescene.io/projects/36629)
+
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=DavidVujic_poetry-multiproject-plugin&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=DavidVujic_poetry-multiproject-plugin)
+
+[![Download Stats](https://img.shields.io/pypi/dm/poetry-multiproject-plugin)](https://pypistats.org/packages/poetry-multiproject-plugin)
+
+
 The `build-project` command will make it possible to use relative package includes.
 This feature is very useful for monorepos and when sharing code between projects.
 
 The `check-project` command is useful to check that dependencies are added properly in a project.
 It uses the `MyPy` tool under the hood, and will output any errors from the static type checker.
 
 
@@ -55,41 +62,54 @@
 The `build-project` command, with a custom top namespace:
 ```shell
 poetry build-project --with-top-namespace my_namespace
 ```
 
 #### The build output
 
-Default behaviour of `build-project` (i.e. without any custom top namespace flag):
+###### Default(no flag)
 ```shell
 /my_package
    __init__.py
    my_module.py
 ```
 
-By using the `--with-top-namespace` flag, the built artifact will look something like this:
+###### Namespace(`--with-top-namespace=my_namespace`)
 ```shell
 my_namespace/
     /my_package
        __init__.py
        my_module.py
 ```
 
+###### Namespace with path(`--with-top-namespace=my_namespace/subdir`)
+```shell
+my_namespace/
+    /subdir
+        /my_package
+           __init__.py
+           my_module.py
+```
 And will re-write the relevant module(s):
 
-(before)
+###### Default(no flag)
 ```python
 from my_package import my_function
 ```
 
-(after)
+###### Namespace(`--with-top-namespace=my_namespace`)
 ```python
 from my_namespace.my_package import my_function
 ```
 
+###### Namespace with path(`--with-top-namespace=my_namespace/subdir`)
+```python
+from my_namespace.subdir.my_package import my_function
+```
+
 ##### How is this done?
 The code in this repo uses AST (Abstract Syntax Tree) parsing to modify source code.
 The Python built-in `ast` module is used to parse and un-parse Python code.
 
 ## Installation
 This plugin can be installed according to the official [Poetry docs](https://python-poetry.org/docs/plugins/#using-plugins).
```

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/buildproject/project.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/buildproject/project.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/checkproject/check.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/checkproject/check.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/check/mypy_checker.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/check/mypy_checker.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/deps/installer.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/deps/installer.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/parsing/rewrite.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/parsing/rewrite.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import ast
 import pathlib
 from typing import List
 
 
 def create_namespace_path(top_ns: str, current: str) -> str:
-    return f"{top_ns}.{current}"
+    top_ns_module_path = top_ns.replace("/", ".")
+    return f"{top_ns_module_path}.{current}"
 
 
 def mutate_import(node: ast.Import, namespaces: List[str], top_ns: str) -> bool:
     did_mutate = False
 
     for alias in node.names:
         if alias.name in namespaces:
```

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/create.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/create.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/packages.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/packages.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/prepare.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/prepare.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,8 +30,8 @@
         dirs_exist_ok=True,
     )
 
     return Path(res)
 
 
 def normalize_top_namespace(namespace: Union[str, None]) -> Union[str, None]:
-    return re.sub("[^a-zA-Z_]", "", namespace) if namespace else None
+    return re.sub("[^a-zA-Z_/]", "", namespace.strip("/")) if namespace else None
```

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/generate.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/generate.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/packages.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/packages.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/read.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/read.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/plugin.py` & `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.2/pyproject.toml` & `poetry_multiproject_plugin-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-multiproject-plugin"
-version = "1.2.2"
+version = "1.3.0"
 description = "A Poetry plugin that makes it possible to use relative package includes."
 authors = ["David Vujic"]
 homepage = "https://github.com/davidvujic/poetry-multiproject-plugin"
 repository = "https://github.com/davidvujic/poetry-multiproject-plugin"
 readme = "README.md"
 packages = [{include = "poetry_multiproject_plugin"}]
```

### Comparing `poetry_multiproject_plugin-1.2.2/PKG-INFO` & `poetry_multiproject_plugin-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-multiproject-plugin
-Version: 1.2.2
+Version: 1.3.0
 Summary: A Poetry plugin that makes it possible to use relative package includes.
 Home-page: https://github.com/davidvujic/poetry-multiproject-plugin
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,21 @@
 
 # Poetry Multiproject Plugin
 
 This is a Python `Poetry` plugin, adding the `build-project` and `check-project` commands.
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/DavidVujic/poetry-multiproject-plugin/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/DavidVujic/poetry-multiproject-plugin/tree/main)
 
+[![CodeScene Code Health](https://codescene.io/projects/36629/status-badges/code-health)](https://codescene.io/projects/36629)
+
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=DavidVujic_poetry-multiproject-plugin&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=DavidVujic_poetry-multiproject-plugin)
+
+[![Download Stats](https://img.shields.io/pypi/dm/poetry-multiproject-plugin)](https://pypistats.org/packages/poetry-multiproject-plugin)
+
+
 The `build-project` command will make it possible to use relative package includes.
 This feature is very useful for monorepos and when sharing code between projects.
 
 The `check-project` command is useful to check that dependencies are added properly in a project.
 It uses the `MyPy` tool under the hood, and will output any errors from the static type checker.
 
 
@@ -73,41 +80,54 @@
 The `build-project` command, with a custom top namespace:
 ```shell
 poetry build-project --with-top-namespace my_namespace
 ```
 
 #### The build output
 
-Default behaviour of `build-project` (i.e. without any custom top namespace flag):
+###### Default(no flag)
 ```shell
 /my_package
    __init__.py
    my_module.py
 ```
 
-By using the `--with-top-namespace` flag, the built artifact will look something like this:
+###### Namespace(`--with-top-namespace=my_namespace`)
 ```shell
 my_namespace/
     /my_package
        __init__.py
        my_module.py
 ```
 
+###### Namespace with path(`--with-top-namespace=my_namespace/subdir`)
+```shell
+my_namespace/
+    /subdir
+        /my_package
+           __init__.py
+           my_module.py
+```
 And will re-write the relevant module(s):
 
-(before)
+###### Default(no flag)
 ```python
 from my_package import my_function
 ```
 
-(after)
+###### Namespace(`--with-top-namespace=my_namespace`)
 ```python
 from my_namespace.my_package import my_function
 ```
 
+###### Namespace with path(`--with-top-namespace=my_namespace/subdir`)
+```python
+from my_namespace.subdir.my_package import my_function
+```
+
 ##### How is this done?
 The code in this repo uses AST (Abstract Syntax Tree) parsing to modify source code.
 The Python built-in `ast` module is used to parse and un-parse Python code.
 
 ## Installation
 This plugin can be installed according to the official [Poetry docs](https://python-poetry.org/docs/plugins/#using-plugins).
```

