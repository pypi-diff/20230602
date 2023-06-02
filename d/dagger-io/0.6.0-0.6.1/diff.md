# Comparing `tmp/dagger_io-0.6.0.tar.gz` & `tmp/dagger_io-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagger_io-0.6.0.tar", max compression
+gzip compressed data, was "dagger_io-0.6.1.tar", max compression
```

## Comparing `dagger_io-0.6.0.tar` & `dagger_io-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    10758 2023-05-25 16:59:18.260135 dagger_io-0.6.0/LICENSE
--rw-r--r--   0        0        0     4727 2023-05-25 16:59:18.260135 dagger_io-0.6.0/README.md
--rw-r--r--   0        0        0     6344 2023-05-25 17:00:26.780909 dagger_io-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      360 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/__init__.py
--rw-r--r--   0        0        0       71 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/__main__.py
--rw-r--r--   0        0        0       69 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/.gitattributes
--rw-r--r--   0        0        0        0 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/__init__.py
--rw-r--r--   0        0        0    11873 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/base.py
--rw-r--r--   0        0        0    89082 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/gen.py
--rw-r--r--   0        0        0    88681 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/gen_sync.py
--rw-r--r--   0        0        0     1683 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/cli.py
--rw-r--r--   0        0        0    20021 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/codegen.py
--rw-r--r--   0        0        0     1302 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/config.py
--rw-r--r--   0        0        0     1884 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/connection.py
--rw-r--r--   0        0        0      964 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/context.py
--rw-r--r--   0        0        0       37 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/.gitattributes
--rw-r--r--   0        0        0       35 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/__init__.py
--rw-r--r--   0        0        0       64 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/_version.py
--rw-r--r--   0        0        0     4202 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/cli.py
--rw-r--r--   0        0        0     2068 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/conn.py
--rw-r--r--   0        0        0     8163 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/download.py
--rw-r--r--   0        0        0     4262 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/exceptions.py
--rw-r--r--   0        0        0      677 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/log.py
--rw-r--r--   0        0        0        0 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/py.typed
--rw-r--r--   0        0        0     2320 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/server/__init__.py
--rw-r--r--   0        0        0       78 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/server/__main__.py
--rw-r--r--   0        0        0      911 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/server/cli.py
--rw-r--r--   0        0        0      865 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/server/converter.py
--rw-r--r--   0        0        0     3892 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/session.py
--rw-r--r--   0        0        0        0 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/transport/__init__.py
--rw-r--r--   0        0        0     5820 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/transport/httpx.py
--rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.6.0/setup.py
--rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-06-02 13:32:48.480901 dagger_io-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4727 2023-06-02 13:32:48.480901 dagger_io-0.6.1/README.md
+-rw-r--r--   0        0        0     6403 2023-06-02 13:33:57.833945 dagger_io-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      360 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/__main__.py
+-rw-r--r--   0        0        0       69 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/api/.gitattributes
+-rw-r--r--   0        0        0        0 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/api/__init__.py
+-rw-r--r--   0        0        0    11873 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/api/base.py
+-rw-r--r--   0        0        0    90131 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/api/gen.py
+-rw-r--r--   0        0        0    89730 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/api/gen_sync.py
+-rw-r--r--   0        0        0     1683 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/cli.py
+-rw-r--r--   0        0        0    20500 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/codegen.py
+-rw-r--r--   0        0        0     1302 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/config.py
+-rw-r--r--   0        0        0     1884 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/connection.py
+-rw-r--r--   0        0        0      964 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/context.py
+-rw-r--r--   0        0        0       37 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/.gitattributes
+-rw-r--r--   0        0        0       35 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/_version.py
+-rw-r--r--   0        0        0     4202 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/cli.py
+-rw-r--r--   0        0        0     2068 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/conn.py
+-rw-r--r--   0        0        0     8163 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/download.py
+-rw-r--r--   0        0        0     4262 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/exceptions.py
+-rw-r--r--   0        0        0      677 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/log.py
+-rw-r--r--   0        0        0        0 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/py.typed
+-rw-r--r--   0        0        0     2320 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/server/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/server/__main__.py
+-rw-r--r--   0        0        0      911 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/server/cli.py
+-rw-r--r--   0        0        0      865 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/server/converter.py
+-rw-r--r--   0        0        0     3892 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/session.py
+-rw-r--r--   0        0        0        0 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/transport/__init__.py
+-rw-r--r--   0        0        0     5820 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/transport/httpx.py
+-rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.6.1/setup.py
+-rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.6.1/PKG-INFO
```

### Comparing `dagger_io-0.6.0/LICENSE` & `dagger_io-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/README.md` & `dagger_io-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/pyproject.toml` & `dagger_io-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dagger-io"
-version = "0.6.0"
+version = "0.6.1"
 description = "A client package for running Dagger pipelines in Python."
 license = "Apache-2.0"
 authors = ["Dagger <hello@dagger.io>"]
 readme = "README.md"
 homepage = "https://dagger.io"
 documentation = "https://docs.dagger.io/sdk/python"
 repository = "https://github.com/dagger/dagger/tree/main/sdk/python"
@@ -164,15 +164,15 @@
 src = ["src", "tests"]
 target-version = "py310"
 select = ["ALL"]
 ignore = [
     # Type inferrance is ok in a lot of places.
     "ANN",
     # This rule doesn't know to ignore a subclass override
-    # so we get false positives for unused arguments. 
+    # so we get false positives for unused arguments.
     "ARG002",
     # Black can handle trailing commas automatically.
     "COM812",
     # FIXME: prefix everything internal with an underscore and document
     # what's left (public).
     "D1",
     # Imperative mood only makes sense in functions, not classes.
@@ -184,18 +184,18 @@
     # Valid use in pytest, docs and examples.
     "INP001",
     # Unnecessary variable assignment before `return` statement
     # doesn't seem to work as expected.
     "RET504",
     # We don't use asserts as runtime validation guarantees.
     "S101",
-    # Don't guard types. Don't want to stringize them. 
+    # Don't guard types. Don't want to stringize them.
     "TCH",
     # Pandas
-    "PD", 
+    "PD",
 ]
 unfixable = [
     # Don't remove `print` statements, just warn.
     "T201",
 ]
 
 [tool.ruff.isort]
@@ -209,27 +209,29 @@
 "../../docs/current/sdk/python/*.py" = ["T201"]
 "./examples/*" = ["T201"]
 "./src/dagger/api/gen*.py" = [
     # Not much control over field names and docs coming from the API.
     # Note: We could detect built-in shadowing like the reserved
     # keywords but these built-ins aren't being used in the generated
     # code so no need to bother.
-    "A", 
-    "D", 
+    "A",
+    "D",
+    # Too hard to properly wrap long lines in codegen.
+    "E501",
     # Too many arguments to function call.
     "PLR0913",
-    # `Optional` is preferred over `| None` because of how 
+    # `Optional` is preferred over `| None` because of how
     # beartype handles forward references.
     "UP007",
 ]
-# Ignore built-in shadowing in test mocks. 
+# Ignore built-in shadowing in test mocks.
 "./tests/api/test_inputs.py" = ["A", "ERA001"]
 "./tests/*.py" = [
     # Ignore security issues in tests.
-    "S", 
+    "S",
     # Magic value comparison doesn't apply to tests.
     "PLR2004",
     # Allow more than one statement in pytest.raises.
     "PT012",
 ]
 # Allow some patterns to redefine imports in __init__.
 "__init__.py" = ["F401", "F403", "PLC0414"]
```

### Comparing `dagger_io-0.6.0/src/dagger/api/base.py` & `dagger_io-0.6.1/src/dagger/api/base.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/api/gen.py` & `dagger_io-0.6.1/src/dagger/api/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Code generated by dagger. DO NOT EDIT.
 
+import warnings
 from collections.abc import Sequence
 from typing import Optional
 
 import attrs
 
 from dagger.api.base import Arg, Enum, Input, Root, Scalar, Type, typecheck
 
@@ -345,14 +346,19 @@
         experimental_privileged_nesting:
             Provide dagger access to the executed command.
             Do not use this option unless you trust the command being
             executed.
             The command being executed WILL BE GRANTED FULL ACCESS TO YOUR
             HOST FILESYSTEM.
         """
+        warnings.warn(
+            'Method "exec" is deprecated: Replaced by "with_exec".',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args = [
             Arg("args", args, None),
             Arg("stdin", stdin, None),
             Arg("redirectStdout", redirect_stdout, None),
             Arg("redirectStderr", redirect_stderr, None),
             Arg("experimentalPrivilegedNesting", experimental_privileged_nesting, None),
         ]
@@ -484,14 +490,19 @@
     @typecheck
     def fs(self) -> "Directory":
         """Retrieves this container's root filesystem. Mounts are not included.
 
         .. deprecated::
             Replaced by :py:meth:`rootfs`.
         """
+        warnings.warn(
+            'Method "fs" is deprecated: Replaced by "rootfs".',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args: list[Arg] = []
         _ctx = self._select("fs", _args)
         return Directory(_ctx)
 
     @typecheck
     async def hostname(self) -> str:
         """Retrieves a hostname which can be used by clients to reach this
@@ -1046,14 +1057,19 @@
     @typecheck
     def with_fs(self, id: "Directory") -> "Container":
         """Initializes this container from this DirectoryID.
 
         .. deprecated::
             Replaced by :py:meth:`with_rootfs`.
         """
+        warnings.warn(
+            'Method "with_fs" is deprecated: Replaced by "with_rootfs".',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args = [
             Arg("id", id),
         ]
         _ctx = self._select("withFS", _args)
         return Container(_ctx)
 
     @typecheck
@@ -2045,14 +2061,19 @@
     def secret(self) -> "Secret":
         """Retrieves a secret referencing the contents of this file.
 
         .. deprecated::
             insecure, leaves secret in cache. Superseded by
             :py:meth:`set_secret`
         """
+        warnings.warn(
+            'Method "secret" is deprecated: insecure, leaves secret in cache. Superseded by "set_secret"',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
     async def size(self) -> int:
         """Gets the size of the file, in bytes.
@@ -2304,14 +2325,19 @@
         exclude:
             Exclude artifacts that match the given pattern (e.g.,
             ["node_modules/", ".git*"]).
         include:
             Include only artifacts that match the given pattern (e.g.,
             ["app/", "package.*"]).
         """
+        warnings.warn(
+            'Method "workdir" is deprecated: Use "directory" with path set to \'.\' instead.',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args = [
             Arg("exclude", exclude, None),
             Arg("include", include, None),
         ]
         _ctx = self._select("workdir", _args)
         return Directory(_ctx)
 
@@ -2322,14 +2348,19 @@
     @typecheck
     def secret(self) -> "Secret":
         """A secret referencing the value of this variable.
 
         .. deprecated::
             been superseded by :py:meth:`set_secret`
         """
+        warnings.warn(
+            'Method "secret" is deprecated: been superseded by "set_secret"',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
     async def value(self) -> str:
         """The value of this variable.
```

### Comparing `dagger_io-0.6.0/src/dagger/api/gen_sync.py` & `dagger_io-0.6.1/src/dagger/api/gen_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Code generated by dagger. DO NOT EDIT.
 
+import warnings
 from collections.abc import Sequence
 from typing import Optional
 
 import attrs
 
 from dagger.api.base import Arg, Enum, Input, Root, Scalar, Type, typecheck
 
@@ -345,14 +346,19 @@
         experimental_privileged_nesting:
             Provide dagger access to the executed command.
             Do not use this option unless you trust the command being
             executed.
             The command being executed WILL BE GRANTED FULL ACCESS TO YOUR
             HOST FILESYSTEM.
         """
+        warnings.warn(
+            'Method "exec" is deprecated: Replaced by "with_exec".',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args = [
             Arg("args", args, None),
             Arg("stdin", stdin, None),
             Arg("redirectStdout", redirect_stdout, None),
             Arg("redirectStderr", redirect_stderr, None),
             Arg("experimentalPrivilegedNesting", experimental_privileged_nesting, None),
         ]
@@ -484,14 +490,19 @@
     @typecheck
     def fs(self) -> "Directory":
         """Retrieves this container's root filesystem. Mounts are not included.
 
         .. deprecated::
             Replaced by :py:meth:`rootfs`.
         """
+        warnings.warn(
+            'Method "fs" is deprecated: Replaced by "rootfs".',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args: list[Arg] = []
         _ctx = self._select("fs", _args)
         return Directory(_ctx)
 
     @typecheck
     def hostname(self) -> str:
         """Retrieves a hostname which can be used by clients to reach this
@@ -1043,14 +1054,19 @@
     @typecheck
     def with_fs(self, id: "Directory") -> "Container":
         """Initializes this container from this DirectoryID.
 
         .. deprecated::
             Replaced by :py:meth:`with_rootfs`.
         """
+        warnings.warn(
+            'Method "with_fs" is deprecated: Replaced by "with_rootfs".',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args = [
             Arg("id", id),
         ]
         _ctx = self._select("withFS", _args)
         return Container(_ctx)
 
     @typecheck
@@ -2042,14 +2058,19 @@
     def secret(self) -> "Secret":
         """Retrieves a secret referencing the contents of this file.
 
         .. deprecated::
             insecure, leaves secret in cache. Superseded by
             :py:meth:`set_secret`
         """
+        warnings.warn(
+            'Method "secret" is deprecated: insecure, leaves secret in cache. Superseded by "set_secret"',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
     def size(self) -> int:
         """Gets the size of the file, in bytes.
@@ -2301,14 +2322,19 @@
         exclude:
             Exclude artifacts that match the given pattern (e.g.,
             ["node_modules/", ".git*"]).
         include:
             Include only artifacts that match the given pattern (e.g.,
             ["app/", "package.*"]).
         """
+        warnings.warn(
+            'Method "workdir" is deprecated: Use "directory" with path set to \'.\' instead.',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args = [
             Arg("exclude", exclude, None),
             Arg("include", include, None),
         ]
         _ctx = self._select("workdir", _args)
         return Directory(_ctx)
 
@@ -2319,14 +2345,19 @@
     @typecheck
     def secret(self) -> "Secret":
         """A secret referencing the value of this variable.
 
         .. deprecated::
             been superseded by :py:meth:`set_secret`
         """
+        warnings.warn(
+            'Method "secret" is deprecated: been superseded by "set_secret"',
+            DeprecationWarning,
+            stacklevel=4,
+        )
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
     def value(self) -> str:
         """The value of this variable.
```

### Comparing `dagger_io-0.6.0/src/dagger/cli.py` & `dagger_io-0.6.1/src/dagger/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/codegen.py` & `dagger_io-0.6.1/src/dagger/codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     sync: bool = False,  # noqa: FBT001, FBT002
 ) -> Iterator[str]:
     """Code generation main function."""
     yield textwrap.dedent(
         """\
         # Code generated by dagger. DO NOT EDIT.
 
+        import warnings
         from collections.abc import Sequence
         from typing import Optional
 
         import attrs
 
         from dagger.api.base import Arg, Enum, Input, Root, Scalar, Type, typecheck
         """,
@@ -450,14 +451,28 @@
         return sig
 
     @joiner
     def func_body(self) -> Iterator[str]:
         if docstring := self.func_doc():
             yield doc(docstring)
 
+        if deprecated := self.deprecated():
+            msg = f'Method "{self.name}" is deprecated: {deprecated}'.replace(
+                '"', '\\"'
+            )
+            yield textwrap.dedent(
+                f"""\
+                warnings.warn(
+                    "{msg}",
+                    DeprecationWarning,
+                    stacklevel=4,
+                )\
+                """
+            )
+
         if not self.args:
             yield "_args: list[Arg] = []"
         else:
             yield "_args = ["
             yield from (indent(arg.as_arg()) for arg in self.args)
             yield "]"
 
@@ -474,15 +489,15 @@
             yield f"return {self.type}(_ctx)"
 
     def func_doc(self) -> str:
         def _out():
             if self.description:
                 yield (textwrap.fill(line) for line in self.description.splitlines())
 
-            if deprecated := self.deprecated():
+            if deprecated := self.deprecated(":py:meth:`", "`"):
                 yield chain(
                     (".. deprecated::",),
                     wrap_indent(deprecated),
                 )
 
             if self.name == "id":
                 yield (
@@ -526,18 +541,18 @@
                         "QueryError",
                         indent("If the API returns an error."),
                     ),
                 )
 
         return "\n\n".join("\n".join(section) for section in _out())
 
-    def deprecated(self) -> str:
+    def deprecated(self, prefix='"', suffix='"') -> str:
         def _format_name(m):
             name = format_name(m.group().strip("`"))
-            return f":py:meth:`{name}`"
+            return f"{prefix}{name}{suffix}"
 
         return (
             DEPRECATION_RE.sub(_format_name, reason)
             if (reason := self.graphql.deprecation_reason)
             else ""
         )
```

### Comparing `dagger_io-0.6.0/src/dagger/config.py` & `dagger_io-0.6.1/src/dagger/config.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/connection.py` & `dagger_io-0.6.1/src/dagger/connection.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/context.py` & `dagger_io-0.6.1/src/dagger/context.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/engine/cli.py` & `dagger_io-0.6.1/src/dagger/engine/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/engine/conn.py` & `dagger_io-0.6.1/src/dagger/engine/conn.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/engine/download.py` & `dagger_io-0.6.1/src/dagger/engine/download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/exceptions.py` & `dagger_io-0.6.1/src/dagger/exceptions.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/log.py` & `dagger_io-0.6.1/src/dagger/log.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/server/__init__.py` & `dagger_io-0.6.1/src/dagger/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/server/cli.py` & `dagger_io-0.6.1/src/dagger/server/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/server/converter.py` & `dagger_io-0.6.1/src/dagger/server/converter.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/session.py` & `dagger_io-0.6.1/src/dagger/session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/src/dagger/transport/httpx.py` & `dagger_io-0.6.1/src/dagger/transport/httpx.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.0/setup.py` & `dagger_io-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'typing_extensions>=4.4.0']
 
 extras_require = \
 {'server': ['strawberry-graphql>=0.133.5']}
 
 setup_kwargs = {
     'name': 'dagger-io',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'A client package for running Dagger pipelines in Python.',
     'long_description': '# Dagger Python SDK\n\n[![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/) \n[![Conda Version](https://img.shields.io/conda/vn/conda-forge/dagger-io.svg)](https://anaconda.org/conda-forge/dagger-io)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dagger-io.svg)](https://pypi.org/project/dagger-io/)\n[![License](https://img.shields.io/pypi/l/dagger-io.svg)](https://pypi.python.org/pypi/dagger-io)\n[![Code style](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n\nA client package for running [Dagger](https://dagger.io/) pipelines.\n\n## What is the Dagger Python SDK?\n\nThe Dagger Python SDK contains everything you need to develop CI/CD pipelines in Python, and run them on any OCI-compatible container runtime.\n\n## Requirements\n\n- Python 3.10 or later\n- [Docker](https://docs.docker.com/engine/install/), or another OCI-compatible container runtime\n\nA compatible version of the  [Dagger CLI](https://docs.dagger.io/cli) is automatically downloaded and run by the SDK for you, although it’s possible to manage it manually.\n\n## Installation\n\nFrom [PyPI](https://pypi.org/project/dagger-io/), using `pip`:\n\n```shell\npip install dagger-io\n```\n\nYou can also install via [Conda](https://anaconda.org/conda-forge/dagger-io), from the [conda-forge](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge) channel:\n\n```shell\nconda install dagger-io\n```\n\n## Example\n\nCreate a `main.py` file:\n\n```python\nimport sys\n\nimport anyio\nimport dagger\n\n\nasync def main(args: list[str]):\n    async with dagger.Connection() as client:\n        # build container with cowsay entrypoint\n        ctr = (\n            client.container()\n            .from_("python:alpine")\n            .with_exec(["pip", "install", "cowsay"])\n            .with_entrypoint(["cowsay"])\n        )\n\n        # run cowsay with requested message\n        result = await ctr.with_exec(args).stdout()\n\n    print(result)\n\n\nanyio.run(main, sys.argv[1:])\n```\n\nRun with:\n\n```console\n$ python main.py "Simple is better than complex"\n  _____________________________\n| Simple is better than complex |\n  =============================\n                             \\\n                              \\\n                                ^__^\n                                (oo)\\_______\n                                (__)\\       )\\/\\\n                                    ||----w |\n                                    ||     ||\n```\n\n> **Note**\n> It may take a while for it to finish, especially on first run with cold cache.\n\nIf you need to debug, you can stream the logs from the engine with the `log_output`  config:\n\n```python\nconfig = dagger.Config(log_output=sys.stderr)\nasync with dagger.Connection(config) as client:\n    ...\n```\n\n## Learn more\n\n- [Documentation](https://docs.dagger.io/sdk/python)\n- [API Reference](https://dagger-io.readthedocs.org)\n- [Source code](https://github.com/dagger/dagger/tree/main/sdk/python)\n\n## Development\n\nThis library is maintained with [Poetry](https://python-poetry.org/docs/).\n\nIf you already have a [Python 3.10 or later](https://docs.python.org/3/using/index.html) interpreter in your `$PATH`, you can let [Poetry manage](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) the [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments) automatically. Otherwise you need to activate it first, before installing dependencies:\n\n```shell\npoetry install\n```\n\nThe following commands are available:\n- `poe test`: Run tests.\n- `poe fmt`: Re-format code following common styling conventions.\n- `poe lint`: Check for linting violations.\n- `poe generate`: Regenerate API client after changes to the codegen.\n- `poe docs`: Build reference docs locally.\n\n### Engine changes\n\nTesting and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet. \n\nThe simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :\n\n```shell\n../../hack/make sdk:python:test\n../../hack/make sdk:python:generate\n```\n\nYou can also build the CLI and use it directly within the Python SDK:\n\n```shell\n../../hack/dev poe test\n```\n\nOr build it separately and tell the SDK to use it directly (or any other CLI binary):\n\n```shell\n../../hack/make\n_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger poe test\n```\n\n',
     'author': 'Dagger',
     'author_email': 'hello@dagger.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dagger.io',
```

### Comparing `dagger_io-0.6.0/PKG-INFO` & `dagger_io-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagger-io
-Version: 0.6.0
+Version: 0.6.1
 Summary: A client package for running Dagger pipelines in Python.
 Home-page: https://dagger.io
 License: Apache-2.0
 Author: Dagger
 Author-email: hello@dagger.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

