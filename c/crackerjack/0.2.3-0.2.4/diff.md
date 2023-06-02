# Comparing `tmp/crackerjack-0.2.3.tar.gz` & `tmp/crackerjack-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.2.3.tar", last modified: Sun May 28 14:58:34 2023, max compression
+gzip compressed data, was "crackerjack-0.2.4.tar", last modified: Fri Jun  2 10:00:54 2023, max compression
```

## Comparing `crackerjack-0.2.3.tar` & `crackerjack-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.3/LICENSE
--rw-r--r--   0        0        0     3265 2023-05-28 14:44:40.883556 crackerjack-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-05-28 14:57:32.147967 crackerjack-0.2.3/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      163 2023-05-28 14:57:32.136981 crackerjack-0.2.3/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-05-28 14:57:32.144421 crackerjack-0.2.3/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2065 2023-05-28 14:57:32.140236 crackerjack-0.2.3/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.3/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.3/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.3/crackerjack/__init__.py
--rw-r--r--   0        0        0     1238 2023-05-27 10:07:36.046052 crackerjack-0.2.3/crackerjack/__main__.py
--rw-r--r--   0        0        0     5570 2023-05-28 14:53:32.418909 crackerjack-0.2.3/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1603 2023-05-28 14:57:33.100620 crackerjack-0.2.3/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     1827 2023-05-28 14:58:34.751666 crackerjack-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4269 1970-01-01 00:00:00.000000 crackerjack-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3208 2023-06-02 09:59:18.505246 crackerjack-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 09:59:42.631901 crackerjack-0.2.4/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      163 2023-06-02 09:59:42.607073 crackerjack-0.2.4/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-06-02 09:59:42.625124 crackerjack-0.2.4/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     1723 2023-06-02 09:59:42.614915 crackerjack-0.2.4/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.4/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.4/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.4/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1238 2023-05-27 10:07:36.046052 crackerjack-0.2.4/crackerjack/__main__.py
+-rw-r--r--   0        0        0     5570 2023-05-28 14:53:32.418909 crackerjack-0.2.4/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1603 2023-06-02 09:59:43.739879 crackerjack-0.2.4/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     1828 2023-06-02 10:00:54.189526 crackerjack-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4212 1970-01-01 00:00:00.000000 crackerjack-0.2.4/PKG-INFO
```

### Comparing `crackerjack-0.2.3/LICENSE` & `crackerjack-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.3/README.md` & `crackerjack-0.2.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Crackerjack Python
 
-[![Python: 3.7](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
+[![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 
 Crackerjack is a python coding style which uses a minimalist approach to produce elegant, easy to read, code.
 
 crack·​er·​jack ˈkra-kər-ˌjak
@@ -22,19 +22,17 @@
 
 This package:
 
 - identifies and removes unused dependencies with creosote
 
 - reformats the code with [Black](https://github.com/ambv/black)
 
-- uses autotype to add missing type annotations to the code
-
 - does import sorting, linting, and complexity analysis with ruff
 
-- uses mypy for type checking
+- uses pyright for type checking
 
 - streamlines code with refurb
 
 - installs, or updates, a project's pre-commit tools and gitignore
   to comply with evolving crackerjack standards
 
 - removes pipenv, poetry, and hatch build, dependency management, and virtual environment
```

### Comparing `crackerjack-0.2.3/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.2.4/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.3/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.2.4/crackerjack/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -34,27 +34,16 @@
     rev: '0.78'
     hooks:
       - id: flynt
   - repo: https://github.com/dosisod/refurb
     rev: v1.16.0
     hooks:
       - id: refurb
-  - repo: local
-    hooks:
-      - id: autotyping
-        name: autotyping
-        entry: python -m libcst.tool codemod autotyping.AutotypeCommand --aggressive crackerjack
-        types_or: [ python, pyi ]
-        language: python
-        files: \.py$
-        additional_dependencies:
-          - autotyping==23.3.0
-          - libcst==0.4.9
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.310
+    rev: v1.1.311
     hooks:
       - id: pyright
   #  - repo: https://github.com/pdoc3/pdoc
   #    rev: master
   #    hooks:
   #      - id: pdoc
   #        name: pdoc
```

### Comparing `crackerjack-0.2.3/crackerjack/__main__.py` & `crackerjack-0.2.4/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.3/crackerjack/crackerjack.py` & `crackerjack-0.2.4/crackerjack/crackerjack.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.3/crackerjack/pyproject.toml` & `crackerjack-0.2.4/crackerjack/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 enable_all = true
 
 [tool.pytype]
 inputs = ["package_name"]
 
 [project]
 name = "Crackerjack"
-version = "0.2.3"
+version = "0.2.4"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = ["black", "ruff", "mypy", "creosote", "refurb"]
 classifiers = ["Environment :: Console", "Operating System :: OS Independent", "Programming Language :: Python", "Programming Language :: Python :: 3.11"]
 dependencies = ["click>=8.1.3", "pdoc3>=0.10.0", "pdm-bump>=0.7.0", "pydantic>=1.10.7", "aiopath>=0.6.11", "acb>=0.1.2", "aioconsole>=0.6.1", "inflection>=0.5.1"]
```

### Comparing `crackerjack-0.2.3/pyproject.toml` & `crackerjack-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.black]
 target-version = [
     "py311",
 ]
 
 [tool.mypy]
 strict = false
-pretty = true
+pretty = false
 ignore_missing_imports = false
 plugins = [
     "pydantic.mypy",
 ]
 python_version = 3.11
 
 [tool.refurb]
@@ -44,15 +44,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.2.3"
+version = "0.2.4"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.2.3/PKG-INFO` & `crackerjack-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.2.3
+Version: 0.2.4
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
@@ -23,15 +23,15 @@
 Requires-Dist: acb>=0.1.2
 Requires-Dist: aioconsole>=0.6.1
 Requires-Dist: inflection>=0.5.1
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
 
-[![Python: 3.7](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
+[![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 
 Crackerjack is a python coding style which uses a minimalist approach to produce elegant, easy to read, code.
 
 crack·​er·​jack ˈkra-kər-ˌjak
@@ -49,19 +49,17 @@
 
 This package:
 
 - identifies and removes unused dependencies with creosote
 
 - reformats the code with [Black](https://github.com/ambv/black)
 
-- uses autotype to add missing type annotations to the code
-
 - does import sorting, linting, and complexity analysis with ruff
 
-- uses mypy for type checking
+- uses pyright for type checking
 
 - streamlines code with refurb
 
 - installs, or updates, a project's pre-commit tools and gitignore
   to comply with evolving crackerjack standards
 
 - removes pipenv, poetry, and hatch build, dependency management, and virtual environment
```

