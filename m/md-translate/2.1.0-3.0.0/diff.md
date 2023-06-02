# Comparing `tmp/md_translate-2.1.0.tar.gz` & `tmp/md_translate-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md_translate-2.1.0.tar", last modified: Wed Oct 21 22:23:21 2020, max compression
+gzip compressed data, was "md_translate-3.0.0.tar", max compression
```

## Comparing `md_translate-2.1.0.tar` & `md_translate-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,24 @@
--rw-r--r--   0        0        0     1069 2020-10-21 22:22:24.040557 md_translate-2.1.0/LICENSE
--rw-r--r--   0        0        0     1453 2020-10-21 22:22:24.040557 md_translate-2.1.0/README.md
--rw-r--r--   0        0        0        0 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/__init__.py
--rw-r--r--   0        0        0      881 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/app.py
--rw-r--r--   0        0        0      403 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/const.py
--rw-r--r--   0        0        0     1350 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/exceptions.py
--rw-r--r--   0        0        0     1786 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/file_translator.py
--rw-r--r--   0        0        0     1475 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/files_worker.py
--rw-r--r--   0        0        0     2535 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/line_processor.py
--rw-r--r--   0        0        0      165 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/logs.py
--rw-r--r--   0        0        0     2882 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/settings.py
--rw-r--r--   0        0        0      385 2020-10-21 22:22:24.040557 md_translate-2.1.0/md_translate/utils.py
--rw-r--r--   0        0        0     1728 2020-10-21 22:22:24.044556 md_translate-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2375 2020-10-21 22:23:21.850038 md_translate-2.1.0/setup.py
--rw-r--r--   0        0        0     2753 2020-10-21 22:23:21.850368 md_translate-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-02 10:39:28.552558 md_translate-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3503 2023-06-02 10:39:28.552558 md_translate-3.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/__init__.py
+-rw-r--r--   0        0        0     4198 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/application.py
+-rw-r--r--   0        0        0      230 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/document/__init__.py
+-rw-r--r--   0        0        0     6485 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/document/blocks.py
+-rw-r--r--   0        0        0     5960 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/document/document.py
+-rw-r--r--   0        0        0     3654 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/document/parser.py
+-rw-r--r--   0        0        0      763 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/main.py
+-rw-r--r--   0        0        0      157 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/settings/__init__.py
+-rw-r--r--   0        0        0     4683 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/settings/_base_settings.py
+-rw-r--r--   0        0        0     2687 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/settings/_settings_to_cli.py
+-rw-r--r--   0        0        0      439 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/__init__.py
+-rw-r--r--   0        0        0      650 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/_base_translator.py
+-rw-r--r--   0        0        0     4960 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/_selenium_base.py
+-rw-r--r--   0        0        0     1559 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/bing.py
+-rw-r--r--   0        0        0     2089 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/deepl.py
+-rw-r--r--   0        0        0     1812 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/google.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/randomizer/__init__.py
+-rw-r--r--   0        0        0     6618 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/randomizer/const.py
+-rw-r--r--   0        0        0     1107 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/randomizer/randomizer.py
+-rw-r--r--   0        0        0     1660 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/yandex.py
+-rw-r--r--   0        0        0     2179 2023-06-02 10:39:28.556558 md_translate-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4791 1970-01-01 00:00:00.000000 md_translate-3.0.0/PKG-INFO
```

### Comparing `md_translate-2.1.0/LICENSE` & `md_translate-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `md_translate-2.1.0/pyproject.toml` & `md_translate-3.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md_translate"
-version = "2.1.0"
+version = "3.0.0"
 description = "CLI tool to translate markdown files"
 authors = ["Ilya Chichak <ilyachch@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/ilyachch/md_docs-trans-app"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -12,72 +12,90 @@
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed"
 ]
 
 [tool.poetry.scripts]
-md-translate = 'md_translate.app:run'
+md-translate = "md_translate.main:main"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.10"
 requests = "^2.24.0"
-translators = "^4.7.2"
-langdetect = "^1.0.8"
-loguru = "^0.5.3"
-
-[tool.poetry.dev-dependencies]
-coverage = "^5.2"
-mypy = "^0.782"
-black = "^19.10b0"
-isort = "^5.6.4"
-pytest = "^6.1.1"
-pytest-cov = "^2.10.1"
+selenium = "^4.5.0"
+mistune = "^2.0.4"
+pydantic = "^1.10.2"
+click = "^8.1.3"
+webdriver-manager = "^3.8.6"
+
+[tool.poetry.group.dev.dependencies]
+types-selenium = "^3.141.9"
+black = "^22.10.0"
+coverage = "^6.5.0"
+mypy = "^0.982"
+isort = "^5.10.1"
+pytest = "^7.1.3"
+pytest-cov = "^4.0.0"
+pre-commit = "^2.20.0"
+types-requests = "^2.28.11.2"
+flake8 = "^5.0.4"
+Flake8-pyproject = "^1.1.0.post0"
 
 [tool.black]
+line-length = 99
+skip-string-normalization = true
 exclude = """
 (
     tests
 )
 """
 
-# Coverage section
+[tool.isort]
+profile = "black"
+line_length = 99
+src_paths = ["md_translate"]
+
+[tool.pytest.ini_options]
+addopts = """"""
 
 [tool.coverage.run]
 source = [
-    'md_translate',
+    "md_translate",
 ]
 omit = [
-    'tests/*',
-    'md_translate/app.py'
+    "tests/*",
+    "md_translate/app.py",
+    "md_translate/translators/*",
 ]
 
-[tool.coverage.html]
-directory = '.coverage_html'
-
 [tool.coverage.report]
-fail_under = 80
-
 exclude_lines = [
-    '# pragma: no cover',
-    'raise NotImplementedError()',
-    'if TYPE_CHECKING:'
+    "# pragma: no cover",
+    "raise NotImplementedError",
+    "if TYPE_CHECKING:",
 ]
-[tool.isort]
-profile = "black"
-src_paths = ["md_translate"]
 
-[build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
-
-# Black section
+[tool.mypy]
+python_version = "3.10"
+disallow_untyped_defs = true
+ignore_missing_imports = true
+warn_unused_configs = true
+exclude = [
+    "tests",
+]
 
+[tool.flake8]
+extend-ignore = ["E501", ]
+max-complexity = 6
```

