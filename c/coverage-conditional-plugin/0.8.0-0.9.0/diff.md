# Comparing `tmp/coverage-conditional-plugin-0.8.0.tar.gz` & `tmp/coverage_conditional_plugin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-conditional-plugin-0.8.0.tar", max compression
+gzip compressed data, was "coverage_conditional_plugin-0.9.0.tar", max compression
```

## Comparing `coverage-conditional-plugin-0.8.0.tar` & `coverage_conditional_plugin-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1103 2022-12-22 09:58:54.329294 coverage-conditional-plugin-0.8.0/LICENSE
--rw-r--r--   0        0        0     4809 2022-12-22 09:58:54.329581 coverage-conditional-plugin-0.8.0/README.md
--rw-r--r--   0        0        0     4259 2022-12-22 09:58:54.329868 coverage-conditional-plugin-0.8.0/coverage_conditional_plugin/__init__.py
--rw-r--r--   0        0        0        0 2022-12-22 09:58:54.329986 coverage-conditional-plugin-0.8.0/coverage_conditional_plugin/py.typed
--rw-r--r--   0        0        0      628 2022-12-22 09:58:54.330120 coverage-conditional-plugin-0.8.0/coverage_conditional_plugin/version.py
--rw-r--r--   0        0        0     1469 2022-12-22 10:09:20.282773 coverage-conditional-plugin-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      311 2022-12-22 09:58:54.332152 coverage-conditional-plugin-0.8.0/test_project/.coveragerc
--rw-r--r--   0        0        0        0 2022-12-22 09:58:54.335063 coverage-conditional-plugin-0.8.0/test_project/__init__.py
--rw-r--r--   0        0        0      982 2022-12-22 09:58:54.336148 coverage-conditional-plugin-0.8.0/test_project/example.py
--rw-r--r--   0        0        0      320 2022-12-22 09:58:54.337561 coverage-conditional-plugin-0.8.0/test_project/pyproject.toml
--rw-r--r--   0        0        0      739 2022-12-22 09:58:54.338798 coverage-conditional-plugin-0.8.0/tests/test_implementation.py
--rw-r--r--   0        0        0     1580 2022-12-22 09:58:54.339147 coverage-conditional-plugin-0.8.0/tests/test_integration.py
--rw-r--r--   0        0        0      573 2022-12-22 09:58:54.339381 coverage-conditional-plugin-0.8.0/tests/test_plugin.py
--rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 coverage-conditional-plugin-0.8.0/setup.py
--rw-r--r--   0        0        0     5983 1970-01-01 00:00:00.000000 coverage-conditional-plugin-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1103 2023-06-02 07:58:56.587111 coverage_conditional_plugin-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5716 2023-06-02 10:09:25.591260 coverage_conditional_plugin-0.9.0/README.md
+-rw-r--r--   0        0        0     5957 2023-06-02 10:09:25.591480 coverage_conditional_plugin-0.9.0/coverage_conditional_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 07:58:56.587431 coverage_conditional_plugin-0.9.0/coverage_conditional_plugin/py.typed
+-rw-r--r--   0        0        0      628 2023-06-02 07:58:56.587527 coverage_conditional_plugin-0.9.0/coverage_conditional_plugin/version.py
+-rw-r--r--   0        0        0     1467 2023-06-02 10:15:33.093843 coverage_conditional_plugin-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-06-02 10:09:25.592942 coverage_conditional_plugin-0.9.0/test_project/.coveragerc
+-rw-r--r--   0        0        0        0 2023-06-02 07:58:56.588324 coverage_conditional_plugin-0.9.0/test_project/__init__.py
+-rw-r--r--   0        0        0       90 2023-06-02 10:09:25.593217 coverage_conditional_plugin-0.9.0/test_project/compat.py
+-rw-r--r--   0        0        0     1119 2023-06-02 10:09:25.593490 coverage_conditional_plugin-0.9.0/test_project/example.py
+-rw-r--r--   0        0        0       90 2023-06-02 10:09:25.593626 coverage_conditional_plugin-0.9.0/test_project/omit1.py
+-rw-r--r--   0        0        0       90 2023-06-02 10:09:25.593752 coverage_conditional_plugin-0.9.0/test_project/omit2.py
+-rw-r--r--   0        0        0      657 2023-06-02 10:09:25.593964 coverage_conditional_plugin-0.9.0/test_project/pyproject.toml
+-rw-r--r--   0        0        0      739 2023-06-02 07:58:56.588603 coverage_conditional_plugin-0.9.0/tests/test_implementation.py
+-rw-r--r--   0        0        0     2034 2023-06-02 10:09:25.594190 coverage_conditional_plugin-0.9.0/tests/test_integration.py
+-rw-r--r--   0        0        0      708 2023-06-02 10:09:25.594349 coverage_conditional_plugin-0.9.0/tests/test_omits.py
+-rw-r--r--   0        0        0      510 2023-06-02 10:09:25.594549 coverage_conditional_plugin-0.9.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     6942 1970-01-01 00:00:00.000000 coverage_conditional_plugin-0.9.0/PKG-INFO
```

### Comparing `coverage-conditional-plugin-0.8.0/LICENSE` & `coverage_conditional_plugin-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coverage-conditional-plugin-0.8.0/README.md` & `coverage_conditional_plugin-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -34,27 +34,37 @@
 ```ini
 [coverage:run]
 # Here we specify plugins for coverage to be used:
 plugins =
   coverage_conditional_plugin
 
 [coverage:coverage_conditional_plugin]
+# Here we specify files to conditionally omit:
+omit =
+  "sys_platform == 'win32'":
+      "my_project/omit*.py"
+      "my_project/win.py"
 # Here we specify our pragma rules:
 rules =
   "sys_version_info >= (3, 8)": py-gte-38
   "is_installed('mypy')": has-mypy
 
 ```
 
 Or to your `pyproject.toml`:
+
 ```toml
 [tool.coverage.run]
 # Here we specify plugins for coverage to be used:
 plugins = ["coverage_conditional_plugin"]
 
+[tool.coverage.coverage_conditional_plugin.omit]
+# Here we specify files to conditionally omit:
+"my_project/omit*.py" = "sys_platform == 'win32'"
+
 [tool.coverage.coverage_conditional_plugin.rules]
 # Here we specify our pragma rules:
 py-gte-38 = "sys_version_info >= (3, 8)"
 has-mypy = "is_installed('mypy')"
 ```
 
 
@@ -124,10 +134,31 @@
 ```python
 from coverage_conditional_plugin import get_env_info
 
 get_env_info()
 ```
 
 
+## Writing omits
+
+Omits allow entire files to be conditionally omitted from coverage measurement.
+
+The TOML format for omits is:
+
+```toml
+[tool.coverage.coverage_conditional_plugin.omit]
+"pragma-condition" = ["project/prefix*.py", "project/filename.py"]
+# or
+"pragma-condition" = "project/filename.py"
+```
+
+**Note**: `ini` format is not supported for `omit` configuration option,
+because there's no easy way to parse `ini` complex configuration. 
+PRs with the fix are welcome!
+
+File name patterns should follow coverage.py's `[run] omit` syntax.
+See [coverage.py](https://coverage.readthedocs.io/en/stable/source.html).
+
+
 ## License
 
 [MIT](https://github.com/wemake.services/coverage-conditional-plugin/blob/master/LICENSE)
```

### Comparing `coverage-conditional-plugin-0.8.0/coverage_conditional_plugin/__init__.py` & `coverage_conditional_plugin-0.9.0/coverage_conditional_plugin/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import os
 import sys
 import traceback
 from importlib import import_module
-from typing import ClassVar, Dict, Iterable, Tuple, Union
+from typing import Any, ClassVar, Dict, List, Tuple, Union
 
 from coverage import CoveragePlugin
 from coverage.config import CoverageConfig
 from packaging.markers import default_environment
 
 from coverage_conditional_plugin.version import package_version
 
+#: Used for `omit` specification.
+_OmitConfigSpec = Dict[str, Union[str, List[str]]]
+
+_INI_OMIT_ERROR = (
+    'Improperly configured: `ini` does not ' +
+    'support `omit` specification, ' +
+    'current setting is: {0}'
+)
+
 
 def get_env_info() -> Dict[str, object]:
     """Public helper to get the same env we pass to the plugin."""
     env_info: Dict[str, object] = {}
     env_info.update(default_environment())
     # Feel free to send PRs that extend this dict:
     env_info.update({
@@ -25,32 +34,57 @@
         'sys': sys,
     })
     return env_info
 
 
 class _ConditionalCovPlugin(CoveragePlugin):
     _rules_opt_name: ClassVar[str] = 'coverage_conditional_plugin:rules'
+    # We use `exlude_line` and not `exclude_also`,
+    # because settings are already post-processed, which means that
+    # `exlude_line` and `exclude_also` are already joined:
     _ignore_opt_name: ClassVar[str] = 'report:exclude_lines'
+    _omit_opt_name_plugin: ClassVar[str] = 'coverage_conditional_plugin:omit'
+    _omit_opt_name_coverage: ClassVar[str] = 'run:omit'
 
-    def configure(self, config: CoverageConfig) -> None:
+    def configure(  # type: ignore[override]
+        self, config: CoverageConfig,
+    ) -> None:
         """
         Main hook for adding extra configuration.
 
         Part of the ``coverage`` public API.
         Called right after ``coverage_init`` function.
         """
-        rules: Iterable[str]
+        self._configure_omits(config)
+        self._configure_rules(config)
+
+    def _configure_omits(self, config: CoverageConfig) -> None:
+        omits: Union[str, _OmitConfigSpec, None] = _get_option(
+            config,
+            self._omit_opt_name_plugin,
+        )
+        if omits is None:
+            return  # No setting, ignoring
+        elif not isinstance(omits, dict):
+            raise RuntimeError(_INI_OMIT_ERROR.format(omits))
+
+        for code, patterns in omits.items():
+            if isinstance(patterns, str):
+                patterns = [patterns]
+            if _should_be_applied(code):
+                self._omit_pattern(config, patterns)
 
+    def _configure_rules(self, config: CoverageConfig) -> None:
         try:  # ini format
             rules = filter(
                 bool,
-                config.get_option(self._rules_opt_name).splitlines(),
+                _get_option(config, self._rules_opt_name).splitlines(),
             )
         except AttributeError:  # toml format
-            rules = config.get_option(self._rules_opt_name).items()
+            rules = _get_option(config, self._rules_opt_name).items()
 
         for rule in rules:
             self._process_rule(config, rule)
 
     def _process_rule(
         self, config: CoverageConfig, rule: Union[str, Tuple[str, str]],
     ) -> None:
@@ -58,68 +92,86 @@
             code, marker = [part.strip() for part in rule.rsplit(':', 1)]
             code = code[1:-1]  # removes quotes
         elif isinstance(rule, tuple):
             marker = rule[0]
             code = rule[1]
         else:
             raise ValueError("Invalid type for 'rule'.")
-        if self._should_be_applied(code):
+        if _should_be_applied(code):
             self._ignore_marker(config, marker)
 
-    def _should_be_applied(self, code: str) -> bool:
-        """
-        Determines whether some specific marker should be applied or not.
+    def _ignore_marker(
+        self, config: CoverageConfig, marker: str,
+    ) -> None:
+        """Adds a marker to the ignore list."""
+        exclude_lines = _get_option(config, self._ignore_opt_name)
+        exclude_lines.append(marker)
+        config.set_option(self._ignore_opt_name, exclude_lines)
+
+    def _omit_pattern(
+        self, config: CoverageConfig, patterns: List[str],
+    ) -> None:
+        """Adds a file name pattern to the omit list."""
+        omit_patterns = _get_option(config, self._omit_opt_name_coverage)
+        omit_patterns.extend(patterns)
+        config.set_option(self._omit_opt_name_coverage, omit_patterns)
+
 
-        Uses ``exec`` on the code you pass with the marker.
-        Be sure, that this code is safe.
+def _is_installed(package: str) -> bool:
+    """Helper function to detect if some package is installed."""
+    try:
+        import_module(package)
+    except ImportError:
+        return False
+    return True
 
-        We also try to provide useful global functions
-        to cover the most popular cases, like:
 
-        - python version
-        - OS name, platform, and version
-        - helpers to work with installed packages
+def _should_be_applied(code: str) -> bool:
+    """
+    Determines whether some specific marker should be applied or not.
 
-        Some examples:
+    Uses ``exec`` on the code you pass with the marker.
+    Be sure, that this code is safe.
 
-        .. code:: ini
+    We also try to provide useful global functions
+    to cover the most popular cases, like:
 
-          [coverage:coverage_conditional_plugin]
-          rules =
-            "sys_version_info >= (3, 8)": py-gte-38
-            "is_installed('mypy')": has-mypy
+    - python version
+    - OS name, platform, and version
+    - helpers to work with installed packages
 
-        So, code marked with `# pragma: py-gte-38` will be ignored
-        for all version of Python prior to 3.8 release.
-        And at the same time,
-        this code will be included to the coverage on 3.8+ releases.
+    Some examples:
 
-        """
-        env_info = get_env_info()
-        try:
-            return eval(code, env_info)  # noqa: WPS421, S307
-        except Exception:
-            msg = 'Exception during conditional coverage evaluation:'
-            print(msg, traceback.format_exc())  # noqa: WPS421
-            return False
+    .. code:: ini
 
-    def _ignore_marker(self, config: CoverageConfig, marker: str) -> None:
-        """Adds a marker to the ignore list."""
-        exclude_lines = config.get_option(self._ignore_opt_name)
-        exclude_lines.append(marker)
-        config.set_option(self._ignore_opt_name, exclude_lines)
+        [coverage:coverage_conditional_plugin]
+        rules =
+        "sys_version_info >= (3, 8)": py-gte-38
+        "is_installed('mypy')": has-mypy
 
+    So, code marked with `# pragma: py-gte-38` will be ignored
+    for all version of Python prior to 3.8 release.
+    And at the same time,
+    this code will be included to the coverage on 3.8+ releases.
 
-def _is_installed(package: str) -> bool:
-    """Helper function to detect if some package is installed."""
+    """
+    env_info = get_env_info()
     try:
-        import_module(package)
-    except ImportError:
+        return eval(code, env_info)  # noqa: WPS421, S307
+    except Exception:
+        msg = 'Exception during conditional coverage evaluation:'
+        print(msg, traceback.format_exc())  # noqa: WPS421
         return False
-    return True
+
+
+def _get_option(  # type: ignore[misc]
+    config: CoverageConfig, option: str,
+) -> Any:
+    # Hack to silence all new typing issues.
+    return config.get_option(option)
 
 
 def coverage_init(reg, options) -> None:
     """
     Entrypoint, part of the ``coverage`` API.
 
     This is called when we specify:
```

### Comparing `coverage-conditional-plugin-0.8.0/coverage_conditional_plugin/version.py` & `coverage_conditional_plugin-0.9.0/coverage_conditional_plugin/version.py`

 * *Files identical despite different names*

### Comparing `coverage-conditional-plugin-0.8.0/pyproject.toml` & `coverage_conditional_plugin-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coverage-conditional-plugin"
-version = "0.8.0"
+version = "0.9.0"
 description = "Conditional coverage based on any rules you define!"
 license = "MIT"
 
 authors = [
   "sobolevn <mail@sobolevn.me>"
 ]
 
@@ -34,33 +34,33 @@
 
 [tool.poetry.urls]
 "Funding" = "https://github.com/sponsors/wemake-services"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
-coverage = ">=5,<8"
+coverage = ">=7,<8"
 packaging = ">=20.4"
 importlib_metadata = { version = "*", python = "<3.10" }
 
 [tool.poetry.group.test.dependencies]
-mypy = "^0.990"
+mypy = "^1.3"
 types-setuptools = "^65.3"
 
 wemake-python-styleguide = "^0.17"
 flake8-pytest-style = "^1.5"
-nitpick = "^0.29"
+nitpick = "^0.33"
 
-safety = "^2.1"
+safety = "^2.3"
 
-pytest = "^7.2"
+pytest = "^7.3"
 pytest-cov = "^3.0"
-pytest-randomly = "^3.10"
+pytest-randomly = "^3.12"
 
 
 [build-system]
-requires = ["poetry_core>=1.2.0"]
+requires = ["poetry_core>=1.6.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.nitpick]
 style = "https://raw.githubusercontent.com/wemake-services/wemake-python-styleguide/master/styles/nitpick-style-wemake.toml"
```

### Comparing `coverage-conditional-plugin-0.8.0/test_project/example.py` & `coverage_conditional_plugin-0.9.0/test_project/example.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from typing import Tuple
 
 
+def if_gte_python311() -> Tuple[int, int]:  # pragma: py-gte-311
+    """Test function for pragma ``py-gte-311``."""
+    return (3, 11)
+
+
 def if_gte_python310() -> Tuple[int, int]:  # pragma: py-gte-310
     """Test function for pragma ``py-gte-310``."""
     return (3, 10)
 
 
 def if_gte_python39() -> Tuple[int, int]:  # pragma: py-gte-39
     """Test function for pragma ``py-gte-39``."""
```

### Comparing `coverage-conditional-plugin-0.8.0/tests/test_implementation.py` & `coverage_conditional_plugin-0.9.0/tests/test_implementation.py`

 * *Files identical despite different names*

### Comparing `coverage-conditional-plugin-0.8.0/tests/test_integration.py` & `coverage_conditional_plugin-0.9.0/tests/test_integration.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,43 +8,54 @@
 from test_project.example import (
     always,
     if_gte_python36,
     if_gte_python37,
     if_gte_python38,
     if_gte_python39,
     if_gte_python310,
+    if_gte_python311,
 )
 
 #: This is just our specific example.
 _EXCUDED_LINES = (sys.version_info[1] - 6) * 3 + 6
+# 3.11 = 21
+# 3.10 = 18
 # 3.9 = 15
 # 3.8 = 12
 # 3.7 = 9
 # 3.6 = 6
 
+#: This is just a result of the coverage run.
+#: It might change if you add new files / change something in `test_project/`.
+_COVERAGE_PERCENT = 63
+
+#: Lines that are not convered due to `omit` setting:
+_MISSING_LINES = 4  # 1 uncovered + 3 in omits
+
 
 def test_integration(cov, capsys):
     """Ensures that coverage is executed correctly."""
     # We call all functions without any actual version checks.
     if_gte_python36()
     if_gte_python37()
     if_gte_python38()
     if_gte_python39()
     if_gte_python310()
+    if_gte_python311()
     always()
 
     cov.json_report(outfile='-')
     captured = capsys.readouterr()
     coverage = json.loads(captured.out)
 
     assert len(
         coverage['files']['test_project/example.py']['excluded_lines'],
     ) == _EXCUDED_LINES
-    assert int(coverage['totals']['percent_covered']) >= 80
-    assert coverage['totals']['missing_lines'] == 1
+    assert int(coverage['totals']['percent_covered']) >= _COVERAGE_PERCENT
+    assert coverage['totals']['missing_lines'] == _MISSING_LINES
 
 
 @pytest.mark.parametrize('configfile', ['.coveragerc', 'pyproject.toml'])
 def test_config_file_parsing(configfile):
     """Ensures that coverage is executed correctly."""
     config_file_path = Path(__file__).parents[1] / 'test_project' / configfile
 
@@ -55,7 +66,9 @@
     cov.start()
     cov.stop()
 
     assert (
         'py-gte-3{minor_ver}'.format(minor_ver=sys.version_info[1])
         in cov.config.exclude_list
     )
+    # Default exclude must not be lost:
+    assert 'raise NotImplementedError' in cov.config.exclude_list
```

### Comparing `coverage-conditional-plugin-0.8.0/setup.py` & `coverage_conditional_plugin-0.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,193 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: coverage-conditional-plugin
+Version: 0.9.0
+Summary: Conditional coverage based on any rules you define!
+Home-page: https://github.com/wemake-services/coverage-conditional-plugin
+License: MIT
+Keywords: coverage,coverage.py,pytest-cov,testing
+Author: sobolevn
+Author-email: mail@sobolevn.me
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: coverage (>=7,<8)
+Requires-Dist: importlib_metadata ; python_version < "3.10"
+Requires-Dist: packaging (>=20.4)
+Project-URL: Funding, https://github.com/sponsors/wemake-services
+Project-URL: Repository, https://github.com/wemake-services/coverage-conditional-plugin
+Description-Content-Type: text/markdown
 
-packages = \
-['coverage_conditional_plugin']
+# coverage-conditional-plugin
 
-package_data = \
-{'': ['*']}
+[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)
+[![Build Status](https://github.com/wemake-services/coverage-conditional-plugin/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/coverage-conditional-plugin/actions?query=workflow%3Atest)
+[![codecov](https://codecov.io/gh/wemake-services/coverage-conditional-plugin/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/coverage-conditional-plugin)
+[![Python Version](https://img.shields.io/pypi/pyversions/coverage-conditional-plugin.svg)](https://pypi.org/project/coverage-conditional-plugin/)
+[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 
-install_requires = \
-['coverage>=5,<8', 'packaging>=20.4']
-
-extras_require = \
-{':python_version < "3.10"': ['importlib_metadata']}
-
-setup_kwargs = {
-    'name': 'coverage-conditional-plugin',
-    'version': '0.8.0',
-    'description': 'Conditional coverage based on any rules you define!',
-    'long_description': '# coverage-conditional-plugin\n\n[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)\n[![Build Status](https://github.com/wemake-services/coverage-conditional-plugin/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/coverage-conditional-plugin/actions?query=workflow%3Atest)\n[![codecov](https://codecov.io/gh/wemake-services/coverage-conditional-plugin/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/coverage-conditional-plugin)\n[![Python Version](https://img.shields.io/pypi/pyversions/coverage-conditional-plugin.svg)](https://pypi.org/project/coverage-conditional-plugin/)\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\nConditional coverage based on any rules you define!\n\nSome projects have different parts that relies on different environments:\n\n- Python version, some code is only executed on specific versions and ignored on others\n- OS version, some code might be Windows, Mac, or Linux only\n- External packages, some code is only executed when some 3rd party package is installed\n\nCurrent best practice is to use `# pragma: no cover` for this places in our project.\nThis project allows to use configurable pragmas\nthat include code to the coverage if some condition evaluates to true,\nand fallback to ignoring this code when condition is false.\n\nRead [the announcing post](https://sobolevn.me/2020/02/conditional-coverage).\n\n\n## Installation\n\n```bash\npip install coverage-conditional-plugin\n```\n\nThen you will need to add to your `setup.cfg` or `.coveragerc` file\nsome extra configuration:\n\n```ini\n[coverage:run]\n# Here we specify plugins for coverage to be used:\nplugins =\n  coverage_conditional_plugin\n\n[coverage:coverage_conditional_plugin]\n# Here we specify our pragma rules:\nrules =\n  "sys_version_info >= (3, 8)": py-gte-38\n  "is_installed(\'mypy\')": has-mypy\n\n```\n\nOr to your `pyproject.toml`:\n```toml\n[tool.coverage.run]\n# Here we specify plugins for coverage to be used:\nplugins = ["coverage_conditional_plugin"]\n\n[tool.coverage.coverage_conditional_plugin.rules]\n# Here we specify our pragma rules:\npy-gte-38 = "sys_version_info >= (3, 8)"\nhas-mypy = "is_installed(\'mypy\')"\n```\n\n\nAdapt rules to suit your needs!\n\n\n## Example\n\nImagine that we have this code:\n\n```python\ntry:  # pragma: has-django\n    import django\nexcept ImportError:  # pragma: has-no-django\n    django = None\n\ndef run_if_django_is_installed():\n    if django is not None:  # pragma: has-django\n        ...\n```\n\nAnd here\'s the configuration you might use:\n\n```ini\n[coverage:coverage_conditional_plugin]\nrules =\n  "is_installed(\'django\')": has-django\n  "not is_installed(\'django\')": has-no-django\n\n```\n\nWhen running tests with and without `django` installed\nyou will have `100%` coverage in both cases.\n\nBut, different lines will be included.\nWith `django` installed it will include\nboth `try:` and `if django is not None:` conditions.\n\nWhen running without `django` installed,\nit will include `except ImportError:` line.\n\n\n## Writing pragma rules\n\nFormat for pragma rules is:\n\n```\n"pragma-condition": pragma-name\n```\n\nCode inside `"pragma-condition"` is evaluted with `eval`.\nMake sure that the input you pass there is trusted!\n`"pragma-condition"` must return `bool` value after evaluation.\n\nWe support all environment markers specified in [PEP-496](https://www.python.org/dev/peps/pep-0496/).\nSee [Strings](https://www.python.org/dev/peps/pep-0496/#strings)\nand [Version Numbers](https://www.python.org/dev/peps/pep-0496/#version-numbers)\nsections for available values. Also, we provide a bunch of additional markers:\n\n- `sys_version_info` is the same as [`sys.version_info`](https://docs.python.org/3/library/sys.html#sys.version_info)\n- `os_environ` is the same as [`os.environ`](https://docs.python.org/3/library/os.html#os.environ)\n- `is_installed` is our custom function that tries to import the passed string, returns `bool` value\n- `package_version` is our custom function that tries to get package version from `pkg_resources` and returns its [parsed version](https://packaging.pypa.io/en/latest/version/#packaging.version.parse)\n\nUse `get_env_info` to get values for the current environment:\n\n```python\nfrom coverage_conditional_plugin import get_env_info\n\nget_env_info()\n```\n\n\n## License\n\n[MIT](https://github.com/wemake.services/coverage-conditional-plugin/blob/master/LICENSE)\n',
-    'author': 'sobolevn',
-    'author_email': 'mail@sobolevn.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/wemake-services/coverage-conditional-plugin',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+Conditional coverage based on any rules you define!
 
+Some projects have different parts that relies on different environments:
+
+- Python version, some code is only executed on specific versions and ignored on others
+- OS version, some code might be Windows, Mac, or Linux only
+- External packages, some code is only executed when some 3rd party package is installed
+
+Current best practice is to use `# pragma: no cover` for this places in our project.
+This project allows to use configurable pragmas
+that include code to the coverage if some condition evaluates to true,
+and fallback to ignoring this code when condition is false.
+
+Read [the announcing post](https://sobolevn.me/2020/02/conditional-coverage).
+
+
+## Installation
+
+```bash
+pip install coverage-conditional-plugin
+```
+
+Then you will need to add to your `setup.cfg` or `.coveragerc` file
+some extra configuration:
+
+```ini
+[coverage:run]
+# Here we specify plugins for coverage to be used:
+plugins =
+  coverage_conditional_plugin
+
+[coverage:coverage_conditional_plugin]
+# Here we specify files to conditionally omit:
+omit =
+  "sys_platform == 'win32'":
+      "my_project/omit*.py"
+      "my_project/win.py"
+# Here we specify our pragma rules:
+rules =
+  "sys_version_info >= (3, 8)": py-gte-38
+  "is_installed('mypy')": has-mypy
+
+```
+
+Or to your `pyproject.toml`:
+
+```toml
+[tool.coverage.run]
+# Here we specify plugins for coverage to be used:
+plugins = ["coverage_conditional_plugin"]
+
+[tool.coverage.coverage_conditional_plugin.omit]
+# Here we specify files to conditionally omit:
+"my_project/omit*.py" = "sys_platform == 'win32'"
+
+[tool.coverage.coverage_conditional_plugin.rules]
+# Here we specify our pragma rules:
+py-gte-38 = "sys_version_info >= (3, 8)"
+has-mypy = "is_installed('mypy')"
+```
+
+
+Adapt rules to suit your needs!
+
+
+## Example
+
+Imagine that we have this code:
+
+```python
+try:  # pragma: has-django
+    import django
+except ImportError:  # pragma: has-no-django
+    django = None
+
+def run_if_django_is_installed():
+    if django is not None:  # pragma: has-django
+        ...
+```
+
+And here's the configuration you might use:
+
+```ini
+[coverage:coverage_conditional_plugin]
+rules =
+  "is_installed('django')": has-django
+  "not is_installed('django')": has-no-django
+
+```
+
+When running tests with and without `django` installed
+you will have `100%` coverage in both cases.
+
+But, different lines will be included.
+With `django` installed it will include
+both `try:` and `if django is not None:` conditions.
+
+When running without `django` installed,
+it will include `except ImportError:` line.
+
+
+## Writing pragma rules
+
+Format for pragma rules is:
+
+```
+"pragma-condition": pragma-name
+```
+
+Code inside `"pragma-condition"` is evaluted with `eval`.
+Make sure that the input you pass there is trusted!
+`"pragma-condition"` must return `bool` value after evaluation.
+
+We support all environment markers specified in [PEP-496](https://www.python.org/dev/peps/pep-0496/).
+See [Strings](https://www.python.org/dev/peps/pep-0496/#strings)
+and [Version Numbers](https://www.python.org/dev/peps/pep-0496/#version-numbers)
+sections for available values. Also, we provide a bunch of additional markers:
+
+- `sys_version_info` is the same as [`sys.version_info`](https://docs.python.org/3/library/sys.html#sys.version_info)
+- `os_environ` is the same as [`os.environ`](https://docs.python.org/3/library/os.html#os.environ)
+- `is_installed` is our custom function that tries to import the passed string, returns `bool` value
+- `package_version` is our custom function that tries to get package version from `pkg_resources` and returns its [parsed version](https://packaging.pypa.io/en/latest/version/#packaging.version.parse)
+
+Use `get_env_info` to get values for the current environment:
+
+```python
+from coverage_conditional_plugin import get_env_info
+
+get_env_info()
+```
+
+
+## Writing omits
+
+Omits allow entire files to be conditionally omitted from coverage measurement.
+
+The TOML format for omits is:
+
+```toml
+[tool.coverage.coverage_conditional_plugin.omit]
+"pragma-condition" = ["project/prefix*.py", "project/filename.py"]
+# or
+"pragma-condition" = "project/filename.py"
+```
+
+**Note**: `ini` format is not supported for `omit` configuration option,
+because there's no easy way to parse `ini` complex configuration. 
+PRs with the fix are welcome!
+
+File name patterns should follow coverage.py's `[run] omit` syntax.
+See [coverage.py](https://coverage.readthedocs.io/en/stable/source.html).
+
+
+## License
+
+[MIT](https://github.com/wemake.services/coverage-conditional-plugin/blob/master/LICENSE)
 
-setup(**setup_kwargs)
```

