# Comparing `tmp/xor_cipher-3.0.0.tar.gz` & `tmp/xor_cipher-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xor_cipher-3.0.0.tar", max compression
+gzip compressed data, was "xor_cipher-3.0.1.tar", max compression
```

## Comparing `xor_cipher-3.0.0.tar` & `xor_cipher-3.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1106 2023-01-05 21:14:35.031227 xor_cipher-3.0.0/LICENSE
--rw-r--r--   0        0        0     3800 2023-01-05 21:14:35.031551 xor_cipher-3.0.0/README.md
--rw-r--r--   0        0        0     2128 2023-01-05 21:14:35.032126 xor_cipher-3.0.0/build.py
--rw-r--r--   0        0        0     3290 2023-01-05 21:14:35.035186 xor_cipher-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1078 2023-01-05 21:14:35.036191 xor_cipher-3.0.0/xor_cipher/__init__.py
--rw-r--r--   0        0        0     4976 2023-01-05 21:14:35.036455 xor_cipher-3.0.0/xor_cipher/core.py
--rw-r--r--   0        0        0     2638 2023-01-05 21:14:35.036734 xor_cipher-3.0.0/xor_cipher/extension.pyx
--rw-r--r--   0        0        0        0 2023-01-05 21:14:35.036957 xor_cipher-3.0.0/xor_cipher/py.typed
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 xor_cipher-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1106 2023-06-02 06:35:59.736930 xor_cipher-3.0.1/LICENSE
+-rw-r--r--   0        0        0     3975 2023-06-02 06:35:59.736930 xor_cipher-3.0.1/README.md
+-rw-r--r--   0        0        0     2128 2023-06-02 06:35:59.736930 xor_cipher-3.0.1/build.py
+-rw-r--r--   0        0        0     3430 2023-06-02 06:35:59.736930 xor_cipher-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1078 2023-06-02 06:35:59.736930 xor_cipher-3.0.1/xor_cipher/__init__.py
+-rw-r--r--   0        0        0     4976 2023-06-02 06:35:59.736930 xor_cipher-3.0.1/xor_cipher/core.py
+-rw-r--r--   0        0        0     2638 2023-06-02 06:35:59.736930 xor_cipher-3.0.1/xor_cipher/extension.pyx
+-rw-r--r--   0        0        0        0 2023-06-02 06:35:59.736930 xor_cipher-3.0.1/xor_cipher/py.typed
+-rw-r--r--   0        0        0     5016 1970-01-01 00:00:00.000000 xor_cipher-3.0.1/PKG-INFO
```

### Comparing `xor_cipher-3.0.0/LICENSE` & `xor_cipher-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xor_cipher-3.0.0/README.md` & `xor_cipher-3.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![License][License Badge]][License]
 [![Version][Version Badge]][Package]
 [![Downloads][Downloads Badge]][Package]
 
 [![Documentation][Documentation Badge]][Documentation]
 [![Check][Check Badge]][Actions]
 [![Test][Test Badge]][Actions]
+[![Coverage][Coverage Badge]][Coverage]
 
 > *Simple, reusable and optimized XOR ciphers in Python.*
 
 `xor-cipher` is a fast implementation of the XOR cipher written using Cython.
 Our tests show that it can be `1000x` faster than pure Python implementations.
 It has been optimized to breeze through datasets of any size.
 
@@ -42,15 +43,15 @@
 $ poetry add xor-cipher
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-xor-cipher = "^2.3.1"
+xor-cipher = "^3.0.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.xor-cipher]
 git = "https://github.com/xor-cipher/xor-cipher.git"
@@ -134,16 +135,18 @@
 [Code of Conduct]: https://github.com/xor-cipher/xor-cipher/blob/main/CODE_OF_CONDUCT.md
 [Contributing Guide]: https://github.com/xor-cipher/xor-cipher/blob/main/CONTRIBUTING.md
 [Security]: https://github.com/xor-cipher/xor-cipher/blob/main/SECURITY.md
 
 [License]: https://github.com/xor-cipher/xor-cipher/blob/main/LICENSE
 
 [Package]: https://pypi.org/project/xor-cipher
-[Documentation]: https://xor-cipher.github.io/xor-cipher
+[Coverage]: https://codecov.io/gh/xor-cipher/xor-cipher
+[Documentation]: https://docs.xor-cipher.com/
 
 [License Badge]: https://img.shields.io/pypi/l/xor-cipher
 [Version Badge]: https://img.shields.io/pypi/v/xor-cipher
 [Downloads Badge]: https://img.shields.io/pypi/dm/xor-cipher
 
 [Documentation Badge]: https://github.com/xor-cipher/xor-cipher/workflows/docs/badge.svg
 [Check Badge]: https://github.com/xor-cipher/xor-cipher/workflows/check/badge.svg
 [Test Badge]: https://github.com/xor-cipher/xor-cipher/workflows/test/badge.svg
+[Coverage Badge]: https://codecov.io/gh/xor-cipher/xor-cipher/branch/main/graph/badge.svg
```

### Comparing `xor_cipher-3.0.0/build.py` & `xor_cipher-3.0.1/build.py`

 * *Files identical despite different names*

### Comparing `xor_cipher-3.0.0/pyproject.toml` & `xor_cipher-3.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "xor-cipher"
-version = "3.0.0"
+version = "3.0.1"
 description = "Simple, reusable and optimized XOR ciphers in Python."
 authors = ["nekitdev", "RealistikDash"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/xor-cipher/xor-cipher"
 repository = "https://github.com/xor-cipher/xor-cipher"
-documentation = "https://xor-cipher.github.io/xor-cipher"
+documentation = "https://docs.xor-cipher.com/"
 
 keywords = ["python", "xor", "cipher"]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
@@ -46,50 +46,58 @@
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.8.0"
+black = "23.3.0"
+flake8-pyproject = "1.2.3"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.10.1"
-python = "^3.7"
+version = "5.12.0"
+python = ">= 3.8"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "0.991"
+mypy = "1.3.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.1.3"
-pytest-cov = "3.0.0"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.3.1"
-mkdocs-material = "8.5.3"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.14"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
-version = "0.19.0"
+version = "0.21.2"
 extras = ["python"]
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.0.0"
+changelogging = "1.3.0"
 
 [tool.black]
 line_length = 100
 
+[tool.flake8]
+max_line_length = 100
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "--cov xor_cipher"
 testpaths = ["tests"]
@@ -100,15 +108,15 @@
 [tool.coverage.report]
 ignore_errors = true
 exclude_lines = [
     "pragma: never",
     "pragma: no cover",
     "if TYPE_CHECKING",
     "@overload",
-    "@abstractmethod",
+    "@required",
     "raise NotImplementedError",
     "raise AssertionError",
     "def __repr__",
 ]
 
 [tool.coverage.html]
 directory = "coverage"
@@ -134,17 +142,17 @@
 
 warn_no_return = true
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
-[tool.changelog]
+[tool.changelogging]
 name = "xor-cipher"
-version = "3.0.0"
+version = "3.0.1"
 url = "https://github.com/xor-cipher/xor-cipher"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
@@ -153,9 +161,9 @@
 bullet = "-"
 wrap = true
 wrap_size = 100
 
 display = ["feature", "change", "fix", "security", "deprecation", "removal", "internal"]
 
 [build-system]
-requires = ["poetry-core >= 1.3.2", "cython >= 0.29.32", "entrypoint >= 1.3.0", "setuptools >= 65.6.3"]
+requires = ["poetry-core >= 1.5.2", "cython >= 0.29.34", "entrypoint >= 1.4.0", "setuptools >= 67.8.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xor_cipher-3.0.0/xor_cipher/__init__.py` & `xor_cipher-3.0.1/xor_cipher/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Simple, reusable and optimized XOR ciphers in Python."
 __url__ = "https://github.com/xor-cipher/xor-cipher"
 
 __title__ = "xor_cipher"
 __author__ = "nekitdev, RealistikDash"
 __license__ = "MIT"
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 
 from xor_cipher.core import (
     DEFAULT_ENCODING,
     DEFAULT_ERRORS,
     cyclic_xor,
     cyclic_xor_in_place,
     cyclic_xor_in_place_unsafe,
```

### Comparing `xor_cipher-3.0.0/xor_cipher/core.py` & `xor_cipher-3.0.1/xor_cipher/core.py`

 * *Files identical despite different names*

### Comparing `xor_cipher-3.0.0/xor_cipher/extension.pyx` & `xor_cipher-3.0.1/xor_cipher/extension.pyx`

 * *Files identical despite different names*

### Comparing `xor_cipher-3.0.0/PKG-INFO` & `xor_cipher-3.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xor-cipher
-Version: 3.0.0
+Version: 3.0.1
 Summary: Simple, reusable and optimized XOR ciphers in Python.
 Home-page: https://github.com/xor-cipher/xor-cipher
 License: MIT
 Keywords: python,xor,cipher
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,28 +15,29 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Project-URL: Documentation, https://xor-cipher.github.io/xor-cipher
+Project-URL: Documentation, https://docs.xor-cipher.com/
 Project-URL: Issues, https://github.com/xor-cipher/xor-cipher/issues
 Project-URL: Repository, https://github.com/xor-cipher/xor-cipher
 Description-Content-Type: text/markdown
 
 # `xor-cipher`
 
 [![License][License Badge]][License]
 [![Version][Version Badge]][Package]
 [![Downloads][Downloads Badge]][Package]
 
 [![Documentation][Documentation Badge]][Documentation]
 [![Check][Check Badge]][Actions]
 [![Test][Test Badge]][Actions]
+[![Coverage][Coverage Badge]][Coverage]
 
 > *Simple, reusable and optimized XOR ciphers in Python.*
 
 `xor-cipher` is a fast implementation of the XOR cipher written using Cython.
 Our tests show that it can be `1000x` faster than pure Python implementations.
 It has been optimized to breeze through datasets of any size.
 
@@ -68,15 +69,15 @@
 $ poetry add xor-cipher
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-xor-cipher = "^2.3.1"
+xor-cipher = "^3.0.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.xor-cipher]
 git = "https://github.com/xor-cipher/xor-cipher.git"
@@ -160,17 +161,19 @@
 [Code of Conduct]: https://github.com/xor-cipher/xor-cipher/blob/main/CODE_OF_CONDUCT.md
 [Contributing Guide]: https://github.com/xor-cipher/xor-cipher/blob/main/CONTRIBUTING.md
 [Security]: https://github.com/xor-cipher/xor-cipher/blob/main/SECURITY.md
 
 [License]: https://github.com/xor-cipher/xor-cipher/blob/main/LICENSE
 
 [Package]: https://pypi.org/project/xor-cipher
-[Documentation]: https://xor-cipher.github.io/xor-cipher
+[Coverage]: https://codecov.io/gh/xor-cipher/xor-cipher
+[Documentation]: https://docs.xor-cipher.com/
 
 [License Badge]: https://img.shields.io/pypi/l/xor-cipher
 [Version Badge]: https://img.shields.io/pypi/v/xor-cipher
 [Downloads Badge]: https://img.shields.io/pypi/dm/xor-cipher
 
 [Documentation Badge]: https://github.com/xor-cipher/xor-cipher/workflows/docs/badge.svg
 [Check Badge]: https://github.com/xor-cipher/xor-cipher/workflows/check/badge.svg
 [Test Badge]: https://github.com/xor-cipher/xor-cipher/workflows/test/badge.svg
+[Coverage Badge]: https://codecov.io/gh/xor-cipher/xor-cipher/branch/main/graph/badge.svg
```

