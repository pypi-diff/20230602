# Comparing `tmp/poetry_plugin_dotenv-0.4.1.tar.gz` & `tmp/poetry_plugin_dotenv-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dotenv-0.4.1.tar", max compression
+gzip compressed data, was "poetry_plugin_dotenv-0.5.0.tar", max compression
```

## Comparing `poetry_plugin_dotenv-0.4.1.tar` & `poetry_plugin_dotenv-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-04-07 16:59:07.544749 poetry_plugin_dotenv-0.4.1/LICENSE
--rw-r--r--   0        0        0     8651 2023-04-07 16:59:07.544749 poetry_plugin_dotenv-0.4.1/README.md
--rw-r--r--   0        0        0     6238 2023-04-07 16:59:35.758122 poetry_plugin_dotenv-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      699 2023-04-07 16:59:35.662117 poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0      335 2023-04-07 16:59:07.548749 poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5423 2023-04-07 16:59:07.548749 poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     6010 2023-04-07 16:59:07.548749 poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1445 2023-04-07 16:59:07.548749 poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     3395 2023-04-07 16:59:07.548749 poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2023-04-07 16:59:07.548749 poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/py.typed
--rw-r--r--   0        0        0    10737 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-02 19:26:20.715203 poetry_plugin_dotenv-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8640 2023-06-02 19:26:20.715203 poetry_plugin_dotenv-0.5.0/README.md
+-rw-r--r--   0        0        0     5555 2023-06-02 19:26:42.763749 poetry_plugin_dotenv-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      699 2023-06-02 19:26:42.683747 poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0      335 2023-06-02 19:26:20.719203 poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0     5235 2023-06-02 19:26:20.719203 poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     5983 2023-06-02 19:26:20.719203 poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1445 2023-06-02 19:26:20.719203 poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     3469 2023-06-02 19:26:20.719203 poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-02 19:26:20.719203 poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/py.typed
+-rw-r--r--   0        0        0    10577 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-0.5.0/PKG-INFO
```

### Comparing `poetry_plugin_dotenv-0.4.1/LICENSE` & `poetry_plugin_dotenv-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.4.1/README.md` & `poetry_plugin_dotenv-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -94,27 +94,25 @@
     </a>
     <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/commits/main">
         <img alt="commit" src="https://img.shields.io/github/last-commit/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
 </p>
 
 <p align="center">
-    <!-- <a href="https://www.buymeacoffee.com/volopivoshenko" target="_blank">
+    <a href="https://www.buymeacoffee.com/volopivoshenko" target="_blank">
         <img alt="buymeacoffee" src="https://img.shields.io/badge/buy_me_-a_coffee-ff6964?logo=buymeacoffee">
-    </a> -->
+    </a>
     <a href="https://stand-with-ukraine.pp.ua/">
         <img alt="standwithukraine" src="https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB">
     </a>
     <a href="https://stand-with-ukraine.pp.ua">
         <img alt="standwithukraine" src="https://img.shields.io/badge/made_in-Ukraine-ffd700.svg?labelColor=0057b7">
     </a>
 </p>
 
-
-
 - [🔮 Overview](#-overview)
 - [⚙️ Installation](#️-installation)
 - [👩🏻‍💻 Usage](#-usage)
 
 # 🔮 Overview
 
 `poetry-plugin-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                     [logo]
                 [license] [python] [pypi] [release] [numpydoc]
               [black] [isort] [wemake] [mypy] [semantic_release]
           [dependabot] [CI] [CD] [CodeQL] [Dependency_Review] [wheel]
                  [coverage] [codeclimate] [downloads] [stars]
               [issues] [issues] [pr] [pr] [contributors] [commit]
-                     [standwithukraine] [standwithukraine]
+             [buymeacoffee] [standwithukraine] [standwithukraine]
 - [ð® Overview](#-overview) - [âï¸ Installation](#ï¸-installation) -
 [ð©ð»âð» Usage](#-usage) # ð® Overview `poetry-plugin-dotenv` - is
 the plugin that automatically loads environment variables from a dotenv file
 into the environment before `poetry` commands are run. **This plugin doesn't
 have any dependencies, but therefore it also supports features that `python-
 dotenv` supports (e.g. templates, interpolating variables using `POSIX`
 variable expansions etc).** # âï¸ Installation ```bash poetry self add
```

### Comparing `poetry_plugin_dotenv-0.4.1/pyproject.toml` & `poetry_plugin_dotenv-0.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dotenv"
-version = "0.4.1"
+version = "0.5.0"
 description = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
     "python",
     "pypi",
@@ -28,14 +28,15 @@
     "Operating System :: OS Independent",
     "Environment :: Other Environment",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering",
     "Natural Language :: English",
@@ -45,49 +46,49 @@
 [tool.poetry.urls]
 "Issues" = "https://github.com/volopivoshenko/poetry-plugin-dotenv/issues"
 "Releases" = "https://github.com/volopivoshenko/poetry-plugin-dotenv/releases"
 "Say Thanks!" = "https://www.buymeacoffee.com/volopivoshenko"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-poetry = "^1.4.2"
+poetry = "^1.5.1"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.2.1"
-poethepoet = "^0.19.0"
-ipython = "^8.11.0"
+pre-commit = "^3.3.1"
+poethepoet = "^0.20.0"
+ipython = "^8.12.0"
 ipdb = "^0.13.13"
 nitpick = "^0.33.1"
 
 [tool.poetry.group.formatters.dependencies]
 isort = "^5.12.0"
 black = "^23.3.0"
-pyupgrade = "^3.3.1"
+pyupgrade = "^3.4.0"
 yesqa = "^1.4.0"
 
 [tool.poetry.group.linters.dependencies]
-mypy = "^1.1.1"
-wemake-python-styleguide = "^0.17.0"
-pyproject-flake8 = "^3.9.2"
-flake8-pytest-style = "^1.7.2"
-deptry = "^0.8.0"
+mypy = "^1.3.0"
+ruff = "^0.0.270"
+deptry = "^0.11.0"
+memestra = "^0.2.1"
 codespell = "^2.2.4"
 
 [tool.poetry.group.tests.dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 xdoctest = "^1.1.1"
 pytest-lazy-fixture = "^0.6.3"
+pytest-codeblocks = "^0.16.1"
 pytest-mock = "^3.10.0"
-pytest-cov = "^4.0.0"
-pytest-sugar = "^0.9.6"
-coverage = { version = "^7.2.2", extras = ["toml"] }
-sh = "^2.0.3"
+pytest-cov = "^4.1.0"
+pytest-sugar = "^0.9.7"
+coverage = { version = "^7.2.7", extras = ["toml"] }
+sh = "^2.0.4"
 
 [tool.poetry.group.ci.dependencies]
-python-semantic-release = "^7.33.2"
+python-semantic-release = "^7.34.3"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 poetry-plugin-dotenv = "poetry_plugin_dotenv.plugin:DotenvPlugin"
 
 [tool.semantic_release]
 branch = "main"
 changelog_file = "CHANGELOG.md"
@@ -95,14 +96,17 @@
 dist_path = "dist"
 upload_to_repository = false
 upload_to_release = true
 remove_dist = false
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = ["src/poetry_plugin_dotenv/__init__.py:__version__"]
 
+[tool.nitpick]
+style = "github://volopivoshenko/cookiecutter-poetry/nitpick/nitpick.toml"
+
 [tool.isort]
 profile = "black"
 line_length = 100
 lines_after_imports = 2
 lines_between_types = 1
 atomic = false
 color_output = true
@@ -120,42 +124,41 @@
 warn_unused_configs = true
 ignore_missing_imports = true
 show_error_codes = true
 namespace_packages = false
 explicit_package_bases = false
 files = ["src", "tests"]
 
-[tool.flake8]
-max-line-length = 100
-max-cognitive-score = 15
-max-imports = 15
-max-module-members = 15
-max-local-variables = 10
-max-annotation-complexity = 5
-inline-quotes = '"'
-docstring_style = "numpy"
+[tool.ruff]
+target-version = "py311"
+line-length = 100
 exclude = ["__init__.py"]
-allowed-domain-names = ["info", "variable", "value", "values", "key", "result"]
-per-file-ignores = [
-    "tests/*.py: S101, WPS118, WPS204, WPS221, WPS226, WPS342, WPS430, WPS440, WPS442",
-]
-# S101 - asserts are necessary for the tests
-# WPS118 - long names for the tests contain description of the tests
-# WPS226 - overuse of the literals is a common thing in the tests
-# WPS342 - raw strings are necessary for the parsers' tests
-# WPS430 - nested functions are necessary for the parameterized pytest fixtures
-# WPS204, WPS440 - overuse of the expression is a common thing in the tests
-# WPS442 - pytest fixtures don't violate "variables from outer scopes"
-extend-ignore = ["NIP", "D202", "DAR", "WPS305", "WPS306", "WPS472"]
-# NIP - no need to use nitpick plugin
-# D202 - code is hard to read without a blank line after a docstring
-# DAR - there is no sense to put all sections in docstring
-# WPS305 - f-strings are more readable than .format()
-# WPS306 - no need to inherit from object
-# WPS472 - unpacking for the single variable is more readable than indexing
+select = ["ALL"]
+ignore = [
+    "ARG002",
+    "ANN002",
+    "ANN003",
+    "ANN101",
+    "ANN102",
+    "D202",
+    "I001",
+    "PTH",
+    "FBT",
+]
+
+[tool.ruff.per-file-ignores]
+"tests/*.*" = ["INP001", "S101"]
+
+[tool.ruff.isort]
+lines-after-imports = 2
+lines-between-types = 1
+order-by-type = false
+force-single-line = true
+force-sort-within-sections = true
+required-imports = ["from __future__ import annotations"]
 
 [tool.codespell]
 skip = "tests,pyproject.toml,poetry.lock,.git,.mypy_cache,.pytest_cache,.idea,.vscode"
 
 [tool.deptry]
 ignore_transitive = ["cleo", "poetry_plugin_dotenv"]
 
@@ -182,23 +185,23 @@
 
 [tool.poe.tasks.format]
 help = "Run formatters"
 sequence = [
     { shell = "find . -type f -name '*.py' | xargs pyupgrade --py311-plus", help = "Run annotations formatter" },
     { shell = "isort .", help = "Run imports formatter" },
     { shell = "black .", help = "Run code formatter" },
-    { shell = "yesqa", help = "Run flake8 formatter" },
+    { shell = "yesqa", help = "Run comments formatter" },
 ]
 
 [tool.poe.tasks.lint]
 help = "Run linters"
 sequence = [
     { shell = "deptry .", help = "Run dependencies linter" },
     { shell = "mypy .", help = "Run types linter" },
-    { shell = "pflake8 .", help = "Run code linter" },
+    { shell = "ruff check .", help = "Run code linter" },
     { shell = "codespell .", help = "Run spell linter" },
 ]
 
 [tool.poe.tasks.tests]
 help = "Run tests"
 shell = "pytest"
```

### Comparing `poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/__init__.py` & `poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."""
 
 __title__ = "poetry-plugin-dotenv"
 __summary__ = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 __uri__ = "https://github.com/volopivoshenko/poetry-plugin-dotenv"
 
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 
 __author__ = "Volodymyr Pivoshenko"
 __email__ = "volodymyr.pivoshenko@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Volodymyr Pivoshenko"
```

### Comparing `poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/dotenv/core.py` & `poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/dotenv/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.filepath = filepath
         self.interpolate = interpolate
 
         self.encoding = "utf-8"
 
         self._dict: typing.OrderedDict[str, str] | None = None
 
-    def dict(self) -> typing.OrderedDict[str, str]:
+    def dict(self) -> typing.OrderedDict[str, str]:  # noqa: A003
         """Return content of a dotenv file."""
 
         if self._dict:
             return self._dict
 
         raw_values = self.parse()
 
@@ -47,21 +47,21 @@
             self._dict = resolve(raw_values, override=self.override)
 
         else:
             self._dict = OrderedDict(raw_values)
 
         return self._dict
 
-    def parse(self) -> typing.Iterator[tuple[str, str]]:
+    def parse(self) -> typing.Generator:
         """Parse a dotenv file."""
 
         with self._get_stream() as stream:
             for mapping in parsers.parse_stream(stream):
                 if mapping.key is not None:
-                    yield mapping.key, mapping.value  # type: ignore
+                    yield mapping.key, mapping.value
 
     def set_as_environment_variables(self) -> bool:
         """Load current dotenv as a system environment variable."""
 
         if self.dict():
             for key, value in self.dict().items():
                 if key in os.environ and not self.override:
@@ -85,15 +85,14 @@
         elif self.stream:
             yield self.stream
 
         else:
             yield io.StringIO("")  # pragma: nocover
 
 
-# noinspection PyShadowingNames
 def resolve(
     values: typing.Iterable[tuple[str, str]],
     override: bool,
 ) -> typing.OrderedDict[str, str]:
     """Resolve dotenv variables."""
 
     new_values: typing.OrderedDict[str, str] = OrderedDict()
@@ -112,24 +111,25 @@
 
             else:
                 env.update(new_values)
                 env.update(os.environ)
 
             result = "".join(atom.resolve(env) for atom in atoms)
 
-        new_values[name] = result  # type: ignore
+        new_values[name] = result
 
     return new_values
 
 
 def walk_to_root(path: str) -> typing.Iterator[str]:
     """Yield directories starting from the given directory up to the root."""
 
     if not os.path.exists(path):
-        raise OSError("Starting path not found.")  # pragma: nocover
+        msg = "Starting path not found."
+        raise OSError(msg)  # pragma: nocover
 
     if os.path.isfile(path):
         path = os.path.dirname(path)  # pragma: nocover
 
     last_dir = None
     current_dir = os.path.abspath(path)
 
@@ -142,17 +142,15 @@
 def find(filename: str = ".env", usecwd: bool = False) -> str:
     """Search in increasingly higher folders for the given file."""
 
     if usecwd or getattr(sys, "frozen", False):
         path = os.getcwd()
 
     else:  # pragma: no cover
-        # WPS437 - call of a protected method is an only way to get a frame
-        # noinspection PyUnresolvedReferences,PyProtectedMember
-        frame = sys._getframe()  # noqa: WPS437
+        frame = sys._getframe()  # noqa: SLF001
         current_file = __file__
 
         while frame.f_code.co_filename == current_file:
             # S101 - this asserts is part of the original package
             assert frame.f_back is not None  # noqa: S101
             frame = frame.f_back
```

### Comparing `poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/dotenv/parsers.py` & `poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/dotenv/parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 from __future__ import annotations
 
 import re
 import codecs
 import dataclasses
 
-from collections.abc import Iterator
 from typing import IO
 from typing import NamedTuple
+from typing import TYPE_CHECKING
+
+
+if TYPE_CHECKING:
+    from collections.abc import Iterator
 
 
 class Original(NamedTuple):
     """Position of the original string in the file."""
 
     string: str
     line: int
@@ -63,15 +67,15 @@
 
     @classmethod
     def start(cls) -> Position:
         """Get a start position."""
 
         return cls(chars=0, line=1)
 
-    def set(self, other: Position) -> None:
+    def set(self, other: Position) -> None:  # noqa: A003
         """Set a position."""
 
         self.chars = other.chars
         self.line = other.line
 
     def advance(self, string: str) -> None:
         """Update a position."""
@@ -91,19 +95,17 @@
         self.mark = Position.start()
 
     def has_next(self) -> bool:
         """Check if a dotenv has the next position."""
 
         return self.position.chars < len(self.string)
 
-    def set_mark(self) -> None:  # noqa: WPS615
+    def set_mark(self) -> None:
         """Set a mark."""
 
-        # WPS615 - this setter is not a standard OOP setter
-
         self.mark.set(self.position)
 
     def get_marked(self) -> Original:
         """Get a mark."""
 
         # fmt: off
         return Original(
@@ -121,15 +123,16 @@
 
     def read_regex(self, regex: re.Pattern[str]) -> tuple[str, ...]:
         """Read a dotenv with a regex."""
 
         match = regex.match(self.string, self.position.chars)
 
         if match is None:
-            raise DotenvParseError("Pattern not found.")
+            msg = "Pattern not found."
+            raise DotenvParseError(msg)
 
         # fmt: off
         matched = self.string[match.start(): match.end()]
         # fmt: on
 
         self.position.advance(matched)
         return match.groups()
@@ -151,15 +154,15 @@
     """Parse a dotenv key."""
 
     char = reader.peek(1)
 
     if char == "#":
         return None
 
-    elif char == "'":
+    elif char == "'":  # noqa: RET505
         key, *_ = reader.read_regex(_single_quoted_key)
 
     else:
         key, *_ = reader.read_regex(_unquoted_key)
 
     return key
 
@@ -176,31 +179,30 @@
 
     char = reader.peek(1)
 
     if char == "'":
         value, *_ = reader.read_regex(_single_quoted_value)
         return decode_escapes(_single_quote_escapes, value)
 
-    elif char == '"':
+    elif char == '"':  # noqa: RET505
         value, *_ = reader.read_regex(_double_quoted_value)
         return decode_escapes(_double_quote_escapes, value)
 
     elif char in {"", "\n", "\r"}:
         return ""
 
     return parse_unquoted_value(reader)
 
 
 def parse_binding(reader: Reader) -> Binding:
     """Parse a dotenv binding."""
 
     reader.set_mark()
 
-    # WPS229 - this part is a part of the original package
-    try:  # noqa: WPS229
+    try:
         reader.read_regex(_multiline_whitespace)
 
         if not reader.has_next():
             return Binding(
                 key=None,
                 value=None,
                 original=reader.get_marked(),
```

### Comparing `poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/dotenv/variables.py` & `poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/dotenv/variables.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.4.1/src/poetry_plugin_dotenv/plugin.py` & `poetry_plugin_dotenv-0.5.0/src/poetry_plugin_dotenv/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """Module that contains the core functionality of the plugin."""
 
 from __future__ import annotations
 
 import os
 import enum
 
-from cleo.events.console_command_event import ConsoleCommandEvent
+from typing import TYPE_CHECKING
+
 from cleo.events.console_events import COMMAND
-from poetry.console.application import Application
 from poetry.console.commands.env_command import EnvCommand
 from poetry.plugins.application_plugin import ApplicationPlugin
 
 from poetry_plugin_dotenv import dotenv
 
 
+if TYPE_CHECKING:
+    from cleo.events.console_command_event import ConsoleCommandEvent
+    from poetry.console.application import Application
+
+
 class Verbosity(enum.Enum):  # pragma: no cover
     """Levels of verbosity."""
 
     info = "<info>{0!s}</info>"
     debug = "<debug>{0!s}</debug>"
     warning = "<warning>{0!s}</warning>"
     error = "<error>{0!s}</error>"
@@ -74,15 +79,15 @@
     If your dotenv file is located in a different path or has a different name you may set
     the ``POETRY_DOTENV_LOCATION`` environment variable.
     """
 
     def activate(self, application: Application) -> None:  # pragma: no cover
         """Activate the plugin."""
 
-        application.event_dispatcher.add_listener(COMMAND, listener=self.load)  # type: ignore
+        application.event_dispatcher.add_listener(COMMAND, listener=self.load)
 
     def load(self, event: ConsoleCommandEvent, *args, **kwargs) -> None:
         """Load a dotenv file."""
 
         logger = Logger(event)
 
         dont_load_dotenv = os.getenv("POETRY_DONT_LOAD_DOTENV")
@@ -92,12 +97,12 @@
         if is_env_command and dont_load_dotenv:
             logger.warning("Not loading environment variables.")
 
         elif is_env_command and not dont_load_dotenv:
             filepath = dotenv_location if dotenv_location else dotenv.core.find(usecwd=True)
 
             if os.path.isfile(filepath):
-                logger.info(f"Loading environment variables from {filepath!r}.")
+                logger.info(f"Loading environment variables from {filepath!r}.")  # noqa: G004
                 dotenv.core.load(filepath=filepath)
 
             else:
-                logger.error(f"File {filepath!r} doesn't exist.")
+                logger.error(f"File {filepath!r} doesn't exist.")  # noqa: G004
```

### Comparing `poetry_plugin_dotenv-0.4.1/PKG-INFO` & `poetry_plugin_dotenv-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dotenv
-Version: 0.4.1
+Version: 0.5.0
 Summary: poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
 Home-page: https://github.com/volopivoshenko/poetry-plugin-dotenv
 License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
@@ -18,23 +18,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: poetry (>=1.4.2,<2.0.0)
+Requires-Dist: poetry (>=1.5.1,<2.0.0)
 Project-URL: Documentation, https://github.com/volopivoshenko/poetry-plugin-dotenv
 Project-URL: Issues, https://github.com/volopivoshenko/poetry-plugin-dotenv/issues
 Project-URL: Repository, https://github.com/volopivoshenko/poetry-plugin-dotenv
 Project-URL: Releases, https://github.com/volopivoshenko/poetry-plugin-dotenv/releases
 Project-URL: Say Thanks!, https://www.buymeacoffee.com/volopivoshenko
 Description-Content-Type: text/markdown
 
@@ -134,27 +131,25 @@
     </a>
     <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/commits/main">
         <img alt="commit" src="https://img.shields.io/github/last-commit/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
 </p>
 
 <p align="center">
-    <!-- <a href="https://www.buymeacoffee.com/volopivoshenko" target="_blank">
+    <a href="https://www.buymeacoffee.com/volopivoshenko" target="_blank">
         <img alt="buymeacoffee" src="https://img.shields.io/badge/buy_me_-a_coffee-ff6964?logo=buymeacoffee">
-    </a> -->
+    </a>
     <a href="https://stand-with-ukraine.pp.ua/">
         <img alt="standwithukraine" src="https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB">
     </a>
     <a href="https://stand-with-ukraine.pp.ua">
         <img alt="standwithukraine" src="https://img.shields.io/badge/made_in-Ukraine-ffd700.svg?labelColor=0057b7">
     </a>
 </p>
 
-
-
 - [🔮 Overview](#-overview)
 - [⚙️ Installation](#️-installation)
 - [👩🏻‍💻 Usage](#-usage)
 
 # 🔮 Overview
 
 `poetry-plugin-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 0.4.1 Summary:
+Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 0.5.0 Summary:
 poetry-plugin-dotenv - is the plugin that automatically loads environment
 variables from a dotenv file into the environment before poetry commands are
 run. Home-page: https://github.com/volopivoshenko/poetry-plugin-dotenv License:
 MIT Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
 plugins,env,dotenv,cross-platform,hacktoberfest Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko
 Maintainer-email: volodymyr.pivoshenko@gmail.com Requires-Python: >=3.8.1,<4.0
@@ -10,33 +10,31 @@
 :: Other Environment Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Python :: 3.8 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Software Development Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: poetry (>=1.4.2,<2.0.0) Project-URL: Documentation, https://
+Requires-Dist: poetry (>=1.5.1,<2.0.0) Project-URL: Documentation, https://
 github.com/volopivoshenko/poetry-plugin-dotenv Project-URL: Issues, https://
 github.com/volopivoshenko/poetry-plugin-dotenv/issues Project-URL: Repository,
 https://github.com/volopivoshenko/poetry-plugin-dotenv Project-URL: Releases,
 https://github.com/volopivoshenko/poetry-plugin-dotenv/releases Project-URL:
 Say Thanks!, https://www.buymeacoffee.com/volopivoshenko Description-Content-
 Type: text/markdown
                                     [logo]
                 [license] [python] [pypi] [release] [numpydoc]
               [black] [isort] [wemake] [mypy] [semantic_release]
           [dependabot] [CI] [CD] [CodeQL] [Dependency_Review] [wheel]
                  [coverage] [codeclimate] [downloads] [stars]
               [issues] [issues] [pr] [pr] [contributors] [commit]
-                     [standwithukraine] [standwithukraine]
+             [buymeacoffee] [standwithukraine] [standwithukraine]
 - [ð® Overview](#-overview) - [âï¸ Installation](#ï¸-installation) -
 [ð©ð»âð» Usage](#-usage) # ð® Overview `poetry-plugin-dotenv` - is
 the plugin that automatically loads environment variables from a dotenv file
 into the environment before `poetry` commands are run. **This plugin doesn't
 have any dependencies, but therefore it also supports features that `python-
 dotenv` supports (e.g. templates, interpolating variables using `POSIX`
 variable expansions etc).** # âï¸ Installation ```bash poetry self add
```

