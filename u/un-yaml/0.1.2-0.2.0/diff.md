# Comparing `tmp/un_yaml-0.1.2.tar.gz` & `tmp/un_yaml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "un_yaml-0.1.2.tar", max compression
+gzip compressed data, was "un_yaml-0.2.0.tar", max compression
```

## Comparing `un_yaml-0.1.2.tar` & `un_yaml-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.1.2/LICENSE
--rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.1.2/README.md
--rw-r--r--   0        0        0      652 2023-05-31 23:54:18.885846 un_yaml-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      119 2023-05-31 13:33:07.341430 un_yaml-0.1.2/un_yaml/__init__.py
--rw-r--r--   0        0        0     3755 2023-05-31 23:54:18.886677 un_yaml-0.1.2/un_yaml/un_cli.py
--rw-r--r--   0        0        0     1420 2023-05-31 12:54:36.393499 un_yaml-0.1.2/un_yaml/un_uri.py
--rw-r--r--   0        0        0     2180 2023-05-31 12:54:36.393871 un_yaml-0.1.2/un_yaml/un_yaml.py
--rw-r--r--   0        0        0       24 2023-05-31 13:33:07.342331 un_yaml-0.1.2/un_yaml/wrapper.py
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 un_yaml-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.2.0/LICENSE
+-rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.2.0/README.md
+-rw-r--r--   0        0        0      751 2023-06-02 07:14:32.759061 un_yaml-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      441 2023-06-02 07:14:32.763817 un_yaml-0.2.0/un_yaml/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 07:14:32.763900 un_yaml-0.2.0/un_yaml/py.typed
+-rw-r--r--   0        0        0     4071 2023-06-02 07:14:32.764583 un_yaml-0.2.0/un_yaml/un_cli.py
+-rw-r--r--   0        0        0     1769 2023-06-02 07:14:32.765229 un_yaml-0.2.0/un_yaml/un_conf.py
+-rw-r--r--   0        0        0     2180 2023-06-02 07:14:32.765632 un_yaml-0.2.0/un_yaml/un_uri.py
+-rw-r--r--   0        0        0     2232 2023-06-02 07:14:32.766373 un_yaml-0.2.0/un_yaml/un_yaml.py
+-rw-r--r--   0        0        0      190 2023-06-02 07:14:32.766902 un_yaml-0.2.0/un_yaml/wrapper.py
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 un_yaml-0.2.0/PKG-INFO
```

### Comparing `un_yaml-0.1.2/LICENSE` & `un_yaml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `un_yaml-0.1.2/un_yaml/un_cli.py` & `un_yaml-0.2.0/un_yaml/un_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from argparse import ArgumentParser, Namespace
 from collections.abc import Sequence
 from importlib.metadata import version
 from pathlib import Path  # NOQA F401
 from sys import stdout
 from typing import Any
 
-__version__ = version("un_yaml")
+__version__: str = version("un_yaml")
 
+from .un_conf import UnConf
 from .un_uri import UnUri
 from .un_yaml import UnYaml
 
 # Harcode most parameters for now
 # TODO: infer them from the YAML file
 
 
@@ -26,21 +27,23 @@
 
     @staticmethod
     def ARG_KWS(arg: dict):
         kwargs = {k: v for k, v in arg.items() if k in UnCli.ARG_KEYS}
         kwargs["type"] = eval(kwargs["type"]) if "type" in kwargs else str
         return kwargs
 
-    def __init__(self, file=CLI_YAML) -> None:
-        yaml_data = UnYaml.load_yaml(file, "tests")
+    def __init__(self, file=CLI_YAML, dir=".") -> None:
+        yaml_data = UnYaml.LoadYaml(file, "tests")
         super().__init__(yaml_data)
-        if UnCli.CMD not in self.cfg:
-            raise ValueError(f"'{UnCli.CMD}' not in file '{file}':\n{self.cfg}")
+        if UnCli.CMD not in self.data:
+            raise ValueError(f"'{UnCli.CMD}' not in file '{file}':\n{self.data}")
         self.cmds = self.get(UnCli.CMD)
         self.doc = self.get_handler("doc")()
+        self.path = Path(dir) / UnConf.DEFAULT
+        self.conf = UnConf(self.path, doc=type(self.doc).__name__)
 
     def parse_version(self, parser: ArgumentParser) -> None:
         doc_name = self.info("doc")
         __version__ = version(doc_name)
         parser.add_argument(
             "-v",
             "--version",
@@ -64,17 +67,14 @@
     async def run(self, argv: Sequence[str] | None, out=stdout):
         args: Any = self.parse(argv)
         if not args:
             return False
         if hasattr(args, "version") and args.version:
             print(args.version, file=out)
             return False
-        if not hasattr(args, "command"):
-            logging.error(f"No command found in: {args}\n{argv}")
-            return False
         return await self.execute(args, out)
 
     def parse(self, argv: Sequence[str] | None) -> Namespace | None:
         parser = self.make_parser()
         args = parser.parse_args(argv)
         if args.command is None and not args.version:
             parser.print_help()
@@ -82,18 +82,27 @@
         return args
 
     def get_resource(self, uri: UnUri) -> Any:
         handler = self.get_handler(uri.tool())
         logging.debug(f"handler: {handler}")
         return handler(uri.attrs)
 
+    def log_resource(self, argv: dict):
+        uri = argv[UnUri.ARG_URI]
+        tool = uri.tool()
+        opts = {str(uri): argv}
+        logging.debug(f"tool[{tool}] {opts}")
+        self.conf.put(tool, opts)
+        self.conf.save()
+
     def resource(self, argv: dict) -> dict:
-        """Hardcode resource transformation, for now"""
+        """Hardcode resource transformation to key named URI, for now"""
         if UnUri.ARG_URI in argv:
             uri = argv[UnUri.ARG_URI]
+            self.log_resource(argv)
             argv[UnUri.ARG_RESOURCE] = self.get_resource(uri)
         return argv
 
     async def execute(self, args: Namespace, out=stdout):
         """Invoke Appropriate Command."""
         cmd = args.command
         if cmd not in self.cmds:
```

### Comparing `un_yaml-0.1.2/un_yaml/un_uri.py` & `un_yaml-0.2.0/un_yaml/un_uri.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,62 @@
 # Parse a UDC "app+protocol://" URI
 
+from json import loads
+from typing import Any
 from urllib.parse import parse_qs, urlparse
 
 
 class UnUri:
     ARG_URI = "uri"
     ARG_RESOURCE = "resource"
     SEP = "+"
     K_HOST = "_hostname"
     K_PROT = "_protocol"
+    K_UPTH = "_uri_paths"
     K_QRY = "_query"
     K_TOOL = "_tool"
     K_URI = "_uri"
 
+    @staticmethod
+    def ExtractJson(result):
+        if not isinstance(result, str) or result[0] != "{":
+            return result
+        if "'" in result:
+            result = result.replace("'", '"')  # JSON parser requires double quotes
+        return loads(result)
+
+    @staticmethod
+    def NormalizeQuery(query: dict) -> dict:
+        for key, value in query.items():
+            if isinstance(value, list):  # non-parsed
+                query[key] = UnUri.ExtractJson(value[0])
+        return query
+
     def __init__(self, uri_string: str):
         self.uri = urlparse(uri_string)
-        self.attrs = self.parse_fragments(self.uri.fragment)
+        self.attrs = self.parse_query(self.uri.fragment)
         self.parse_scheme(self.uri.scheme)
         self.attrs[UnUri.K_HOST] = self.uri.hostname or "localhost"
-        self.attrs[UnUri.K_QRY] = self.uri.query
+        self.attrs[UnUri.K_UPTH] = self.uri.path.strip("/").split("/")
+        self.attrs[UnUri.K_QRY] = self.parse_query(self.uri.query)
         self.attrs[UnUri.K_URI] = uri_string
 
     def __repr__(self):
         return f"UnUri({self.attrs[UnUri.K_URI]})"
 
+    def __str__(self):
+        return self.attrs[UnUri.K_URI]
+
     def get(self, key):
         return self.attrs.get(key)
 
-    def parse_fragments(self, fragment: str):
-        list_dict = parse_qs(fragment)
+    def parse_query(self, query: str) -> dict[str, Any]:
+        list_dict = parse_qs(query)
         scalars = {k: v[0] for k, v in list_dict.items()}
-        return scalars
+        return UnUri.NormalizeQuery(scalars)
 
     def parse_scheme(self, scheme: str):
         schemes = scheme.split(UnUri.SEP)
         if len(schemes) != 2:
             raise ValueError(
                 f"Error: URI scheme `{self.uri.scheme}` does not contain '{UnUri.SEP}'"
             )
```

### Comparing `un_yaml-0.1.2/un_yaml/un_yaml.py` & `un_yaml-0.2.0/un_yaml/un_yaml.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,26 +8,27 @@
     KEY = "_yaml"
     SEP = "/"
     PREFIX = "#/"
     REF = "$ref"
     REF_ERROR = f"Value for Key {REF} does not start with {PREFIX}"
 
     @staticmethod
-    def load_yaml(filename: str, pkg: str, sub: str = "") -> dict:
+    def LoadYaml(filename: str, pkg: str, sub: str = "") -> dict:
         yaml_dir = resources.files(pkg)
         if len(sub) > 0:
             yaml_dir = yaml_dir / sub
         yaml_file = yaml_dir / filename
         yaml_string = yaml_file.read_text()
         yaml_data = safe_load(yaml_string)
         return yaml_data
 
     def __init__(self, yaml_data: dict) -> None:
-        self.cfg = yaml_data
-        self._info = self.cfg[UnYaml.KEY]
+        self.data = yaml_data
+        assert self.data, "UnYaml: no data"
+        self._info = self.data[UnYaml.KEY]
 
     def info(self, key: str) -> Any:
         return self._info.get(key)
 
     def expand(self, item):
         if isinstance(item, dict):
             if UnYaml.REF in item:
@@ -50,17 +51,17 @@
     def _get(self, result, key: str):
         if not result:
             return False
         if isinstance(result, list):
             return result[int(key)]
         return result.get(key)
 
-    def get(self, keys: str) -> Any:
-        result = self.cfg
-        for key in keys.split(UnYaml.SEP):
+    def get(self, keylist: str) -> Any:
+        result = self.data
+        for key in keylist.split(UnYaml.SEP):
             item = self._get(result, key)
             result = self.expand(item)
 
         return result
 
     def get_handler(self, key: str) -> Callable:
         handlers = self.info("handlers")
```

### Comparing `un_yaml-0.1.2/PKG-INFO` & `un_yaml-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: un-yaml
-Version: 0.1.2
+Version: 0.2.0
 Summary: Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: asyncclick (>=8.1.3.4,<9.0.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: trio (>=0.22.0,<0.23.0)
+Requires-Dist: types-pyyaml (>=6.0.12.10,<7.0.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # un-yaml
 
 Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)
```

