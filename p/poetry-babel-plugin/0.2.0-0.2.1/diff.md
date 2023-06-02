# Comparing `tmp/poetry-babel-plugin-0.2.0.tar.gz` & `tmp/poetry_babel_plugin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-babel-plugin-0.2.0.tar", max compression
+gzip compressed data, was "poetry_babel_plugin-0.2.1.tar", max compression
```

## Comparing `poetry-babel-plugin-0.2.0.tar` & `poetry_babel_plugin-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1052 2022-05-20 09:13:56.875108 poetry-babel-plugin-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2022-05-20 09:13:56.879108 poetry-babel-plugin-0.2.0/poetry_babel_plugin/__init__.py
--rw-r--r--   0        0        0     3723 2022-09-01 08:30:41.943211 poetry-babel-plugin-0.2.0/poetry_babel_plugin/plugin.py
--rw-r--r--   0        0        0      991 2022-09-01 08:34:24.938107 poetry-babel-plugin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 poetry-babel-plugin-0.2.0/setup.py
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 poetry-babel-plugin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2022-05-20 09:13:56.875108 poetry_babel_plugin-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2022-05-20 09:13:56.879108 poetry_babel_plugin-0.2.1/poetry_babel_plugin/__init__.py
+-rw-r--r--   0        0        0     3717 2023-06-02 13:26:21.127895 poetry_babel_plugin-0.2.1/poetry_babel_plugin/plugin.py
+-rw-r--r--   0        0        0      992 2023-06-02 13:35:30.598911 poetry_babel_plugin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 poetry_babel_plugin-0.2.1/PKG-INFO
```

### Comparing `poetry-babel-plugin-0.2.0/LICENSE` & `poetry_babel_plugin-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-babel-plugin-0.2.0/poetry_babel_plugin/plugin.py` & `poetry_babel_plugin-0.2.1/poetry_babel_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         io.write_line("")
 
     def compile_message(
         self, io: IO, domain: str, dir_path: Path, locales: Optional[Iterable[str]] = None, fuzzy: bool = False
     ):
         if locales is None:
             # Detect locales by listing the directory
-            locale_paths = [(p.name, p) for p in dir_path.glob("*") if p.is_directory()]
+            locale_paths = [(p.name, p) for p in dir_path.glob("*") if p.is_dir()]
         else:
             locale_paths = [(locale, dir_path / locale) for locale in locales]
 
         in_paths: List[Tuple[str, Path, Path]] = []
         for locale, locale_path in locale_paths:
             po_path = locale_path / "LC_MESSAGES" / f"{domain}.po"
             if po_path.exists():
```

### Comparing `poetry-babel-plugin-0.2.0/pyproject.toml` & `poetry_babel_plugin-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.isort]
 line_length = 120
 profile = 'black'
 
 [tool.poetry]
 name = "poetry-babel-plugin"
-version = "0.2.0"
+version = "0.2.1"
 description = "Babel plugin for poetry"
 authors = ["Stepan Henek <stepan@henek.name>"]
 license = "MIT"
 classifiers = [
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Topic :: Software Development :: Localization"
@@ -24,15 +24,15 @@
 keywords = ["poetry", "babel"]
 documentation = "https://github.com/shenek/poetry-babel-plugin/blob/master/README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 babel = "^2.10.1"
-poetry = "~1.2.0"
+poetry = ">=1.2.0"
 
 [tool.poetry.dev-dependencies]
 black = "22.3.0"
 pre-commit = "^2.19.0"
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
```

### Comparing `poetry-babel-plugin-0.2.0/PKG-INFO` & `poetry_babel_plugin-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: poetry-babel-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Babel plugin for poetry
 License: MIT
 Keywords: poetry,babel
 Author: Stepan Henek
 Author-email: stepan@henek.name
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Localization
 Requires-Dist: babel (>=2.10.1,<3.0.0)
-Requires-Dist: poetry (>=1.2.0,<1.3.0)
+Requires-Dist: poetry (>=1.2.0)
 Project-URL: Documentation, https://github.com/shenek/poetry-babel-plugin/blob/master/README.md
```

