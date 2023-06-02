# Comparing `tmp/liquid_jsonpath-0.1.0.tar.gz` & `tmp/liquid_jsonpath-0.2.0.tar.gz`

## Comparing `liquid_jsonpath-0.1.0.tar` & `liquid_jsonpath-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/liquid_jsonpath/__about__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/liquid_jsonpath/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/liquid_jsonpath/default.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/liquid_jsonpath/py.typed
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/liquid_jsonpath/filters/__init__.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/liquid_jsonpath/filters/find.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/liquid_jsonpath/tags/__init__.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/liquid_jsonpath/tags/for_tag.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/README.md
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 liquid_jsonpath-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/liquid_jsonpath/__about__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/liquid_jsonpath/__init__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/liquid_jsonpath/default.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/liquid_jsonpath/env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/liquid_jsonpath/py.typed
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/liquid_jsonpath/filters/__init__.py
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/liquid_jsonpath/filters/find.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/liquid_jsonpath/tags/__init__.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/liquid_jsonpath/tags/for_tag.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/README.md
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 liquid_jsonpath-0.2.0/PKG-INFO
```

### Comparing `liquid_jsonpath-0.1.0/liquid_jsonpath/default.py` & `liquid_jsonpath-0.2.0/liquid_jsonpath/default.py`

 * *Files identical despite different names*

### Comparing `liquid_jsonpath-0.1.0/liquid_jsonpath/filters/find.py` & `liquid_jsonpath-0.2.0/liquid_jsonpath/filters/find.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """A Liquid filter bringing JSONPath syntax to Liquid templates."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Mapping
 from typing import Optional
 from typing import Sequence
+from typing import Type
 
-from jsonpath import JSONPathEnvironment
 from jsonpath import JSONPathError
 from liquid.exceptions import FilterArgumentError
 
 from liquid_jsonpath import Default
+from liquid_jsonpath.env import LiquidJSONPathEnvironment
 
 if TYPE_CHECKING:
+    from jsonpath import JSONPathEnvironment
+    from liquid import Context
     from liquid import Environment
 
 
 class Find:
     """A Liquid filter bringing JSONPath syntax to Liquid templates.
 
     Args:
@@ -24,61 +27,61 @@
             value or the JSONPath are invalid.
 
     Attributes:
         jsonpath_class: The `JSONPathEnvironment` to use. Override this with
             as custom `JSONPathEnvironment` subclass to configure JSONPath.
     """
 
-    jsonpath_class = JSONPathEnvironment
-    with_environment = True
+    jsonpath_class: Type[JSONPathEnvironment] = LiquidJSONPathEnvironment
+    with_context = True
 
     def __init__(self, default: Default = Default.UNDEFINED) -> None:
         self.default = default
         self.jsonpath = self.jsonpath_class()
 
-    def __call__(self, obj: object, path: str, environment: Environment) -> object:
+    def __call__(self, obj: object, path: str, context: Context) -> object:
         """Find all objects in _obj_ matching the JSONPath _path_.
 
         If _obj_ is not a mapping or sequence - like a list or dictionary - a
         default value is returned or an exceptions is raised, depending on the
         value of _self.default_.
         """
         if isinstance(obj, str):
-            return self._default(obj, environment)
+            return self._default(obj, context.env)
 
         if isinstance(obj, (Mapping, Sequence)):
             try:
-                return self.jsonpath.findall(path, obj)
+                return self.jsonpath.findall(path, obj, filter_context=context.scope)
             except JSONPathError as err:
-                return self._default(obj, environment, err)
+                return self._default(obj, context.env, err)
 
-        return self._default(obj, environment)
+        return self._default(obj, context.env)
 
-    async def filter_async(
-        self, obj: object, path: str, environment: Environment
-    ) -> object:
+    async def filter_async(self, obj: object, path: str, context: Context) -> object:
         """Find all objects in _obj_ matching the JSONPath _path_.
 
         Where _obj_ and its children implement `__getitem_async__`, it will
         be awaited instead of calling `getitem()`.
 
         If _obj_ is not a mapping or sequence - like a list or dictionary - a
         default value is returned or an exceptions is raised, depending on the
         value of _self.default_.
         """
         if isinstance(obj, str):
-            return self._default(obj, environment)
+            return self._default(obj, context.env)
 
         if isinstance(obj, (Mapping, Sequence)):
             try:
-                return await self.jsonpath.findall_async(path, obj)
+                return await self.jsonpath.findall_async(
+                    path, obj, filter_context=context.scope
+                )
             except JSONPathError as err:
-                return self._default(obj, environment, err)
+                return self._default(obj, context.env, err)
 
-        return self._default(obj, environment)
+        return self._default(obj, context.env)
 
     def _default(
         self, obj: object, env: Environment, err: Optional[Exception] = None
     ) -> object:
         if self.default == Default.EMPTY:
             return []
         if self.default == Default.UNDEFINED:
```

### Comparing `liquid_jsonpath-0.1.0/liquid_jsonpath/tags/for_tag.py` & `liquid_jsonpath-0.2.0/liquid_jsonpath/tags/for_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """A _for_ tag that allows iterables to be piped through a JSONPath."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Mapping
 from typing import Optional
 from typing import Sequence
+from typing import Type
 from typing import Union
 
 from jsonpath import CompoundJSONPath
 from jsonpath import JSONPath
-from jsonpath import JSONPathEnvironment
 from jsonpath.exceptions import JSONPathError
 from liquid.ast import BlockNode
 from liquid.builtin.tags.for_tag import ENDFORBLOCK
 from liquid.builtin.tags.for_tag import ENDFORELSEBLOCK
 from liquid.builtin.tags.for_tag import TAG_ELSE
 from liquid.builtin.tags.for_tag import TAG_ENDFOR
 from liquid.builtin.tags.for_tag import ForNode
@@ -37,16 +37,18 @@
 from liquid.token import TOKEN_IN
 from liquid.token import TOKEN_LPAREN
 from liquid.token import TOKEN_PIPE
 from liquid.token import TOKEN_STRING
 from liquid.token import TOKEN_TAG
 
 from liquid_jsonpath import Default
+from liquid_jsonpath.env import LiquidJSONPathEnvironment
 
 if TYPE_CHECKING:
+    from jsonpath import JSONPathEnvironment
     from liquid import Context
     from liquid import Environment
     from liquid.ast import Node
 
 
 class JSONPathExpression(Expression):
     """A Liquid expression that evaluates a JSONPath against an object."""
@@ -65,26 +67,26 @@
 
     def evaluate(self, context: Context) -> object:  # noqa: D102
         obj = self.expression.evaluate(context)
         if isinstance(obj, str):
             return self._default(obj, context.env)
         if isinstance(obj, (Mapping, Sequence)):
             try:
-                return self.path.findall(obj)
+                return self.path.findall(obj, filter_context=context.scope)
             except JSONPathError as err:
                 return self._default(obj, context.env, err)
         return self._default(obj, context.env)
 
     async def evaluate_async(self, context: Context) -> object:  # noqa: D102
         obj = await self.expression.evaluate_async(context)
         if isinstance(obj, str):
             return self._default(obj, context.env)
         if isinstance(obj, (Mapping, Sequence)):
             try:
-                return await self.path.findall_async(obj)
+                return await self.path.findall_async(obj, filter_context=context.scope)
             except JSONPathError as err:
                 return self._default(obj, context.env, err)
         return self._default(obj, context.env)
 
     def _default(
         self, obj: object, env: Environment, err: Optional[Exception] = None
     ) -> object:
@@ -100,15 +102,15 @@
         raise LiquidTypeError(msg)
 
 
 class JSONPathForTag(ForTag):
     """A _for_ tag that allows iterables to be piped through a JSONPath."""
 
     default = Default.UNDEFINED
-    jsonpath_class = JSONPathEnvironment
+    jsonpath_class: Type[JSONPathEnvironment] = LiquidJSONPathEnvironment
 
     def __init__(self, env: Environment):
         super().__init__(env)
         self.jsonpath = self.jsonpath_class()
 
     def parse(self, stream: TokenStream) -> Node:  # noqa: D102
         tok = stream.next_token()
```

### Comparing `liquid_jsonpath-0.1.0/.gitignore` & `liquid_jsonpath-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `liquid_jsonpath-0.1.0/LICENSE.txt` & `liquid_jsonpath-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `liquid_jsonpath-0.1.0/README.md` & `liquid_jsonpath-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `liquid_jsonpath-0.1.0/pyproject.toml` & `liquid_jsonpath-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [{ name = "James Prior", email = "jamesgr.prior@gmail.com" }]
 classifiers = [
   "Development Status :: 4 - Beta",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
-dependencies = ["python-liquid>=1.9.2", "python-jsonpath>=0.5.0"]
+dependencies = ["python-liquid>=1.9.2", "python-jsonpath>=0.7.1"]
 
 [project.urls]
 Documentation = "https://jg-rp.github.io/liquid/jsonpath/introduction"
 Issues = "https://github.com/jg-rp/liquid-jsonpath/issues"
 Source = "https://github.com/jg-rp/liquid-jsonpath"
 
 [tool.hatch.version]
@@ -53,15 +55,15 @@
   "types-python-dateutil",
 ]
 
 
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 cov = "pytest --cov-report=term-missing --cov-fail-under=98 --cov-config=pyproject.toml --cov=liquid_jsonpath --cov=tests {args}"
-cov-html = ["test-cov", "- coverage combine", "coverage html"]
+cov-html = "pytest --cov-report=html --cov-config=pyproject.toml --cov=liquid_jsonpath --cov=tests {args}"
 lint = "ruff check ."
 typing = "mypy"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
 [tool.black]
```

### Comparing `liquid_jsonpath-0.1.0/PKG-INFO` & `liquid_jsonpath-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: liquid-jsonpath
-Version: 0.1.0
+Version: 0.2.0
 Summary: JSONPath selectors for Python Liquid.
 Project-URL: Documentation, https://jg-rp.github.io/liquid/jsonpath/introduction
 Project-URL: Issues, https://github.com/jg-rp/liquid-jsonpath/issues
 Project-URL: Source, https://github.com/jg-rp/liquid-jsonpath
 Author-email: James Prior <jamesgr.prior@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: python-jsonpath>=0.5.0
+Requires-Dist: python-jsonpath>=0.7.1
 Requires-Dist: python-liquid>=1.9.2
 Description-Content-Type: text/markdown
 
 <h1 align="center">Liquid JSONPath</h1>
 
 <p align="center">
 <a href="https://github.com/jg-rp/python-jsonpath">JSONPath</a> selectors for <a href="https://jg-rp.github.io/liquid/">Python Liquid</a>.
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: liquid-jsonpath Version: 0.1.0 Summary: JSONPath
+Metadata-Version: 2.1 Name: liquid-jsonpath Version: 0.2.0 Summary: JSONPath
 selectors for Python Liquid. Project-URL: Documentation, https://jg-
 rp.github.io/liquid/jsonpath/introduction Project-URL: Issues, https://
 github.com/jg-rp/liquid-jsonpath/issues Project-URL: Source, https://
 github.com/jg-rp/liquid-jsonpath Author-email: James Prior
 prior@gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
-Development Status :: 4 - Beta Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
-Implementation :: CPython Classifier: Programming Language :: Python ::
-Implementation :: PyPy Requires-Python: >=3.7 Requires-Dist: python-
-jsonpath>=0.5.0 Requires-Dist: python-liquid>=1.9.2 Description-Content-Type:
-text/markdown
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Programming
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7 Requires-
+Dist: python-jsonpath>=0.7.1 Requires-Dist: python-liquid>=1.9.2 Description-
+Content-Type: text/markdown
                          ****** Liquid JSONPath ******
                      JSONPath selectors for Python_Liquid.
                                   [License]
                       [PyPi_-_Version] [Python_versions]
                               [Tests] [Coverage]
 --- **Table of Contents** - [Installation](#installation) - [Links](#links) -
 [Examples](#examples) - [License](#license) ## Installation Install JSONPath
```

