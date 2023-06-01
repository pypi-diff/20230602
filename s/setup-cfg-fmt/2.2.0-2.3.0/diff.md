# Comparing `tmp/setup_cfg_fmt-2.2.0.tar.gz` & `tmp/setup_cfg_fmt-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup_cfg_fmt-2.2.0.tar", last modified: Mon Oct 24 23:14:13 2022, max compression
+gzip compressed data, was "setup_cfg_fmt-2.3.0.tar", last modified: Thu Jun  1 23:40:41 2023, max compression
```

## Comparing `setup_cfg_fmt-2.2.0.tar` & `setup_cfg_fmt-2.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-24 23:14:13.690069 setup_cfg_fmt-2.2.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-07-31 23:00:24.000000 setup_cfg_fmt-2.2.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5494 2022-10-24 23:14:13.690069 setup_cfg_fmt-2.2.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4876 2022-10-24 23:14:13.000000 setup_cfg_fmt-2.2.0/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1185 2022-10-24 23:14:13.694067 setup_cfg_fmt-2.2.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-07-31 23:00:24.000000 setup_cfg_fmt-2.2.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-24 23:14:13.690069 setup_cfg_fmt-2.2.0/setup_cfg_fmt.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5494 2022-10-24 23:14:13.000000 setup_cfg_fmt-2.2.0/setup_cfg_fmt.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      277 2022-10-24 23:14:13.000000 setup_cfg_fmt-2.2.0/setup_cfg_fmt.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-10-24 23:14:13.000000 setup_cfg_fmt-2.2.0/setup_cfg_fmt.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       53 2022-10-24 23:14:13.000000 setup_cfg_fmt-2.2.0/setup_cfg_fmt.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       25 2022-10-24 23:14:13.000000 setup_cfg_fmt-2.2.0/setup_cfg_fmt.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       14 2022-10-24 23:14:13.000000 setup_cfg_fmt-2.2.0/setup_cfg_fmt.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)    17804 2022-10-24 23:13:56.000000 setup_cfg_fmt-2.2.0/setup_cfg_fmt.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 23:40:41.347571 setup_cfg_fmt-2.3.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-01 21:59:49.000000 setup_cfg_fmt-2.3.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4739 2023-06-01 23:40:41.347571 setup_cfg_fmt-2.3.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4121 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1158 2023-06-01 23:40:41.351571 setup_cfg_fmt-2.3.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-01 21:59:49.000000 setup_cfg_fmt-2.3.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 23:40:41.347571 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4739 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      277 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       53 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       25 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       14 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    17808 2023-06-01 23:40:38.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.py
```

### Comparing `setup_cfg_fmt-2.2.0/LICENSE` & `setup_cfg_fmt-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setup_cfg_fmt-2.2.0/PKG-INFO` & `setup_cfg_fmt-2.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: setup_cfg_fmt
-Version: 2.2.0
+Version: 2.3.0
 Summary: apply a consistent format to `setup.cfg` files
 Home-page: https://github.com/asottile/setup-cfg-fmt
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.setup-cfg-fmt?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=51&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/51/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=51&branchName=main)
+[![build status](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setup-cfg-fmt/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setup-cfg-fmt/main)
 
 setup-cfg-fmt
 =============
 
 apply a consistent format to `setup.cfg` files
 
@@ -34,32 +33,25 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.2.0
+    rev: v2.3.0
     hooks:
     -   id: setup-cfg-fmt
 ```
 
 ## cli
 
 Consult the help for the latest usage:
 
 ```console
 $ setup-cfg-fmt --help
-usage: setup-cfg-fmt [-h] [filenames [filenames ...]]
-
-positional arguments:
-  filenames
-
-optional arguments:
-  -h, --help  show this help message and exit
 ```
 
 ## what does it do?
 
 ### sets a consistent ordering for attributes
 
 For example, `name` and `version` (the most important metadata) will always
@@ -141,54 +133,42 @@
 ### set `python_requires`
 
 A few sources are searched for guessing `python_requires`:
 
 - the existing `python_requires` setting itself
 - `envlist` in `tox.ini` if present
 - python version `classifiers` that are already set
-- the `--min-py3-version` argument (currently defaulting to `3.7`)
-
-If the minimum version is detected as python2, the `--min-py3-version`
-argument will be used to exclude python3.x versions (see below).
-
-```diff
- [options]
- py_modules = pre_commit
-+python_requires = >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-```
+- the `--min-py-version` argument (currently defaulting to `3.7`)
 
 ### adds python version classifiers
 
 classifiers are generated based on:
 
 - the `python_requires` setting
 - the `--max-py-version` argument (currently defaulting to `3.11`)
 - `--include-version-classifiers` is specified
 
 ```diff
  name = pkg
  version = 1.0
 +classifiers =
-+    Programming Language :: Python :: 2
-+    Programming Language :: Python :: 2.7
 +    Programming Language :: Python :: 3
 +    Programming Language :: Python :: 3.7
 +    Programming Language :: Python :: 3.8
 +    Programming Language :: Python :: 3.9
 +    Programming Language :: Python :: 3.10
 +    Programming Language :: Python :: 3.11
 ```
 
 without `--include-version-classifiers` only the major version will be included:
 
 ```diff
  name = pkg
  version = 1.0
 +classifiers =
-+    Programming Language :: Python :: 2
 +    Programming Language :: Python :: 3
 ```
 
 ### sorts classifiers
 
 ```diff
  [metadata]
```

### Comparing `setup_cfg_fmt-2.2.0/README.md` & `setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,25 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.setup-cfg-fmt?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=51&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/51/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=51&branchName=main)
+Metadata-Version: 2.1
+Name: setup-cfg-fmt
+Version: 2.3.0
+Summary: apply a consistent format to `setup.cfg` files
+Home-page: https://github.com/asottile/setup-cfg-fmt
+Author: Anthony Sottile
+Author-email: asottile@umich.edu
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![build status](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setup-cfg-fmt/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setup-cfg-fmt/main)
 
 setup-cfg-fmt
 =============
 
 apply a consistent format to `setup.cfg` files
 
@@ -17,32 +33,25 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.2.0
+    rev: v2.3.0
     hooks:
     -   id: setup-cfg-fmt
 ```
 
 ## cli
 
 Consult the help for the latest usage:
 
 ```console
 $ setup-cfg-fmt --help
-usage: setup-cfg-fmt [-h] [filenames [filenames ...]]
-
-positional arguments:
-  filenames
-
-optional arguments:
-  -h, --help  show this help message and exit
 ```
 
 ## what does it do?
 
 ### sets a consistent ordering for attributes
 
 For example, `name` and `version` (the most important metadata) will always
@@ -124,54 +133,42 @@
 ### set `python_requires`
 
 A few sources are searched for guessing `python_requires`:
 
 - the existing `python_requires` setting itself
 - `envlist` in `tox.ini` if present
 - python version `classifiers` that are already set
-- the `--min-py3-version` argument (currently defaulting to `3.7`)
-
-If the minimum version is detected as python2, the `--min-py3-version`
-argument will be used to exclude python3.x versions (see below).
-
-```diff
- [options]
- py_modules = pre_commit
-+python_requires = >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-```
+- the `--min-py-version` argument (currently defaulting to `3.7`)
 
 ### adds python version classifiers
 
 classifiers are generated based on:
 
 - the `python_requires` setting
 - the `--max-py-version` argument (currently defaulting to `3.11`)
 - `--include-version-classifiers` is specified
 
 ```diff
  name = pkg
  version = 1.0
 +classifiers =
-+    Programming Language :: Python :: 2
-+    Programming Language :: Python :: 2.7
 +    Programming Language :: Python :: 3
 +    Programming Language :: Python :: 3.7
 +    Programming Language :: Python :: 3.8
 +    Programming Language :: Python :: 3.9
 +    Programming Language :: Python :: 3.10
 +    Programming Language :: Python :: 3.11
 ```
 
 without `--include-version-classifiers` only the major version will be included:
 
 ```diff
  name = pkg
  version = 1.0
 +classifiers =
-+    Programming Language :: Python :: 2
 +    Programming Language :: Python :: 3
 ```
 
 ### sorts classifiers
 
 ```diff
  [metadata]
```

### Comparing `setup_cfg_fmt-2.2.0/setup.cfg` & `setup_cfg_fmt-2.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = setup_cfg_fmt
-version = 2.2.0
+version = 2.3.0
 description = apply a consistent format to `setup.cfg` files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/setup-cfg-fmt
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
@@ -33,15 +33,14 @@
 plugins = covdefaults
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
```

### Comparing `setup_cfg_fmt-2.2.0/setup_cfg_fmt.egg-info/PKG-INFO` & `setup_cfg_fmt-2.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,8 @@
-Metadata-Version: 2.1
-Name: setup-cfg-fmt
-Version: 2.2.0
-Summary: apply a consistent format to `setup.cfg` files
-Home-page: https://github.com/asottile/setup-cfg-fmt
-Author: Anthony Sottile
-Author-email: asottile@umich.edu
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.setup-cfg-fmt?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=51&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/51/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=51&branchName=main)
+[![build status](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setup-cfg-fmt/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setup-cfg-fmt/main)
 
 setup-cfg-fmt
 =============
 
 apply a consistent format to `setup.cfg` files
 
@@ -34,32 +16,25 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.2.0
+    rev: v2.3.0
     hooks:
     -   id: setup-cfg-fmt
 ```
 
 ## cli
 
 Consult the help for the latest usage:
 
 ```console
 $ setup-cfg-fmt --help
-usage: setup-cfg-fmt [-h] [filenames [filenames ...]]
-
-positional arguments:
-  filenames
-
-optional arguments:
-  -h, --help  show this help message and exit
 ```
 
 ## what does it do?
 
 ### sets a consistent ordering for attributes
 
 For example, `name` and `version` (the most important metadata) will always
@@ -141,54 +116,42 @@
 ### set `python_requires`
 
 A few sources are searched for guessing `python_requires`:
 
 - the existing `python_requires` setting itself
 - `envlist` in `tox.ini` if present
 - python version `classifiers` that are already set
-- the `--min-py3-version` argument (currently defaulting to `3.7`)
-
-If the minimum version is detected as python2, the `--min-py3-version`
-argument will be used to exclude python3.x versions (see below).
-
-```diff
- [options]
- py_modules = pre_commit
-+python_requires = >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-```
+- the `--min-py-version` argument (currently defaulting to `3.7`)
 
 ### adds python version classifiers
 
 classifiers are generated based on:
 
 - the `python_requires` setting
 - the `--max-py-version` argument (currently defaulting to `3.11`)
 - `--include-version-classifiers` is specified
 
 ```diff
  name = pkg
  version = 1.0
 +classifiers =
-+    Programming Language :: Python :: 2
-+    Programming Language :: Python :: 2.7
 +    Programming Language :: Python :: 3
 +    Programming Language :: Python :: 3.7
 +    Programming Language :: Python :: 3.8
 +    Programming Language :: Python :: 3.9
 +    Programming Language :: Python :: 3.10
 +    Programming Language :: Python :: 3.11
 ```
 
 without `--include-version-classifiers` only the major version will be included:
 
 ```diff
  name = pkg
  version = 1.0
 +classifiers =
-+    Programming Language :: Python :: 2
 +    Programming Language :: Python :: 3
 ```
 
 ### sorts classifiers
 
 ```diff
  [metadata]
```

### Comparing `setup_cfg_fmt-2.2.0/setup_cfg_fmt.py` & `setup_cfg_fmt-2.3.0/setup_cfg_fmt.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import argparse
 import configparser
 import glob
 import io
 import os.path
 import re
 import string
+import sys
 from typing import Generator
 from typing import Match
 from typing import Sequence
 from typing import Tuple
 
 from identify import identify
 
@@ -19,15 +20,15 @@
 KEYS_ORDER: tuple[tuple[str, tuple[str, ...]], ...] = (
     (
         'metadata', (
             'name', 'version', 'description',
             'long_description', 'long_description_content_type',
             'url',
             'author', 'author_email', 'maintainer', 'maintainer_email',
-            'license', 'license_file', 'license_files',
+            'license', 'license_files',
             'platforms', 'classifiers',
         ),
     ),
     (
         'options', (
             'packages', 'py_modules', 'install_requires', 'python_requires',
         ),
@@ -112,17 +113,27 @@
     for filename in sorted(glob.iglob(f'{path}*'), key=sort_key):
         if os.path.isfile(filename):
             return filename
     else:
         return None
 
 
-def _py3_excluded(min_py3_version: tuple[int, int]) -> set[tuple[int, int]]:
-    _, end = min_py3_version
-    return {(3, i) for i in range(end)}
+def _parse_list(s: str) -> list[str]:
+    return s.strip().splitlines()
+
+
+def _fmt_list_always(items: list[str]) -> str:
+    return '\n'.join(['', *items])
+
+
+def _fmt_list(items: list[str]) -> str:
+    if len(items) == 1:
+        return items[0]
+    else:
+        return _fmt_list_always(items)
 
 
 def _format_python_requires(minimum: Version, excluded: set[Version]) -> str:
     return ', '.join((
         f'>={_v(minimum)}', *(f'!={_v(v)}.*' for v in sorted(excluded)),
     ))
 
@@ -171,72 +182,67 @@
         envlist = cfg.get('tox', 'envlist', fallback='')
         if envlist:
             for env in envlist.split(','):
                 env, _, _ = env.strip().partition('-')  # py36-foo
                 yield env
 
 
+TOX_ENV = re.compile(r'py3(\d+)')
+
+
 def _python_requires(
-        setup_cfg: str, *, min_py3_version: tuple[int, int],
+        setup_cfg: str, *, min_py_version: tuple[int, int],
 ) -> str | None:
     cfg = NoTransformConfigParser()
     cfg.read(setup_cfg)
     current_value = cfg.get('options', 'python_requires', fallback='')
     classifiers = cfg.get('metadata', 'classifiers', fallback='')
 
     try:
         minimum, excluded = _parse_python_requires(current_value)
     except UnknownVersionError:  # assume they know what's up with weird things
         return current_value
 
     for env in _tox_envlist(setup_cfg):
-        if (
-                env.startswith('py') and
-                len(env) == 4 and
-                env[2:].isdigit()
-        ):
-            version = _to_ver('.'.join(env[2:]))
+        match = TOX_ENV.match(env)
+        if match:
+            version = _to_ver(f'3.{match[1]}')
             if minimum is None or version < minimum[:2]:
                 minimum = version
 
-    for classifier in classifiers.strip().splitlines():
-        if classifier.startswith('Programming Language :: Python ::'):
+    for classifier in _parse_list(classifiers):
+        if classifier.startswith('Programming Language :: Python :: 3'):
             version_part = classifier.split()[-1]
             if '.' not in version_part:
                 continue
             version = _to_ver(version_part)
             if minimum is None or version < minimum[:2]:
                 minimum = version
 
     if minimum is None:
         return None
-    elif minimum[0] == 2:
-        excluded.update(_py3_excluded(min_py3_version))
-        return _format_python_requires(minimum, excluded)
-    elif min_py3_version > minimum:
-        return _format_python_requires(min_py3_version, excluded)
+    elif min_py_version > minimum:
+        return _format_python_requires(min_py_version, excluded)
     else:
         return _format_python_requires(minimum, excluded)
 
 
 def _requires(
         cfg: NoTransformConfigParser, which: str, section: str = 'options',
 ) -> list[str]:
     raw = cfg.get(section, which, fallback='')
 
-    require_group = raw.strip().splitlines()
+    require_group = _parse_list(raw)
     if not require_group:
         return []
 
-    normalized = sorted(
+    return sorted(
         (_normalize_req(req) for req in require_group),
         key=lambda req: (';' in req, _req_base(req), req),
     )
-    normalized.insert(0, '')
-    return normalized
 
 
 def _normalize_req(req: str) -> str:
     lib, _, envs = req.partition(';')
     normalized = _normalize_lib(lib)
 
     envs = envs.strip()
@@ -271,43 +277,39 @@
     assert basem
     # pip replaces _ with - in package names
     return basem.group(0).replace('_', '-')
 
 
 def _py_classifiers(
         python_requires: str | None, *, max_py_version: tuple[int, int],
-) -> str | None:
+) -> list[str]:
     try:
         minimum, exclude = _parse_python_requires(python_requires)
     except UnknownVersionError:
-        return None
+        return []
 
     if minimum is None:  # don't have a sequence of versions to iterate over
-        return None
+        return []
     else:
         # classifiers only use the first two segments of version
         minimum = minimum[:2]
 
     versions: set[Version] = set()
     while minimum <= max_py_version:
         if minimum not in exclude:
             versions.add(minimum)
             versions.add(minimum[:1])
-        if minimum == (2, 7):
-            minimum = (3, 0)
-        else:
-            minimum = (minimum[0], minimum[1] + 1)
+        minimum = (minimum[0], minimum[1] + 1)
 
     classifiers = [
         f'Programming Language :: Python :: {_v(v)}' for v in versions
     ]
-    if (3,) in versions and (2,) not in versions:
-        classifiers.append('Programming Language :: Python :: 3 :: Only')
+    classifiers.append('Programming Language :: Python :: 3 :: Only')
 
-    return '\n'.join(classifiers)
+    return classifiers
 
 
 def _trim_py_classifiers(
         classifiers: list[str],
         python_requires: str | None,
         *,
         include_version_classifiers: bool,
@@ -328,35 +330,35 @@
                 not s.startswith('Programming Language :: Python :: ')
         ):
             return True
 
         ver = tuple(int(p) for p in parts[-1].strip().split('.'))
         size = len(ver)
         return (
-            ver not in exclude and (
+            ver >= (3,) and ver not in exclude and (
                 size == 1 or (
                     include_version_classifiers and
                     minimum[:size] <= ver <= max_py_version[:size]
                 )
             )
         )
 
     return [s for s in classifiers if _is_ok_classifier(s)]
 
 
-def _imp_classifiers(setup_cfg: str) -> str:
+def _imp_classifiers(setup_cfg: str) -> list[str]:
     classifiers = set()
 
     for env in _tox_envlist(setup_cfg):
         # remove trailing digits: py39-django31
         classifier = TOX_TO_CLASSIFIERS.get(env.rstrip(string.digits))
         if classifier is not None:
             classifiers.add(classifier)
 
-    return '\n'.join(sorted(classifiers))
+    return sorted(classifiers)
 
 
 def _natural_sort(items: Sequence[str]) -> list[str]:
     return sorted(
         set(items),
         key=lambda s: [
             int(part) if part.isdigit() else part.lower()
@@ -364,15 +366,15 @@
         ],
     )
 
 
 def format_file(
         filename: str, *,
         include_version_classifiers: bool,
-        min_py3_version: tuple[int, int],
+        min_py_version: tuple[int, int],
         max_py_version: tuple[int, int],
 ) -> bool:
     with open(filename) as f:
         contents = f.read()
 
     cfg = NoTransformConfigParser()
     cfg.read_string(contents)
@@ -391,77 +393,71 @@
         if 'markdown' in tags:
             cfg['metadata']['long_description_content_type'] = 'text/markdown'
         elif 'rst' in tags:
             cfg['metadata']['long_description_content_type'] = 'text/x-rst'
         else:
             cfg['metadata']['long_description_content_type'] = 'text/plain'
 
+    classifiers = _parse_list(cfg['metadata'].get('classifiers', ''))
+    licenses = _parse_list(cfg['metadata'].get('license_files', ''))
+
+    # combines license_file and license_files
+    if 'license_file' in cfg['metadata']:
+        licenses.append(cfg['metadata'].pop('license_file'))
+
     # set license fields if a license exists
     license_filename = _first_file(filename, 'licen[sc]e')
     if license_filename is not None:
         license_basename = os.path.basename(license_filename)
-        known_license_files = (
-            cfg['metadata'].get('license_files', '').strip().splitlines()
-        )
-        if license_basename not in known_license_files:
-            cfg['metadata']['license_file'] = license_basename
+        licenses.append(license_basename)
 
         license_id = identify.license_id(license_filename)
         if license_id is not None:
             cfg['metadata']['license'] = license_id
 
         if license_id in LICENSE_TO_CLASSIFIER:
-            cfg['metadata']['classifiers'] = (
-                cfg['metadata'].get('classifiers', '').rstrip() +
-                f'\n{LICENSE_TO_CLASSIFIER[license_id]}'
-            )
+            classifiers.append(LICENSE_TO_CLASSIFIER[license_id])
 
-    requires = _python_requires(filename, min_py3_version=min_py3_version)
+    # sort license_files if it exists
+    if licenses:
+        cfg['metadata']['license_files'] = _fmt_list(sorted(set(licenses)))
+
+    requires = _python_requires(filename, min_py_version=min_py_version)
     if requires is not None:
         if not cfg.has_section('options'):
             cfg.add_section('options')
         cfg['options']['python_requires'] = requires
 
     install_requires = _requires(cfg, 'install_requires')
     if install_requires:
-        cfg['options']['install_requires'] = '\n'.join(install_requires)
+        cfg['options']['install_requires'] = _fmt_list_always(install_requires)
 
     setup_requires = _requires(cfg, 'setup_requires')
     if setup_requires:
-        cfg['options']['setup_requires'] = '\n'.join(setup_requires)
+        cfg['options']['setup_requires'] = _fmt_list_always(setup_requires)
 
     if cfg.has_section('options.extras_require'):
         for key in cfg['options.extras_require']:
-            group_requires = _requires(cfg, key, 'options.extras_require')
-            cfg['options.extras_require'][key] = '\n'.join(group_requires)
+            cfg['options.extras_require'][key] = _fmt_list_always(
+                _requires(cfg, key, 'options.extras_require'),
+            )
 
     py_classifiers = _py_classifiers(requires, max_py_version=max_py_version)
-    if py_classifiers:
-        cfg['metadata']['classifiers'] = (
-            cfg['metadata'].get('classifiers', '').rstrip() +
-            f'\n{py_classifiers}'
-        )
-
-    imp_classifiers = _imp_classifiers(filename)
-    if imp_classifiers:
-        cfg['metadata']['classifiers'] = (
-            cfg['metadata'].get('classifiers', '').rstrip() +
-            f'\n{imp_classifiers}'
-        )
+    classifiers.extend(py_classifiers)
+    classifiers.extend(_imp_classifiers(filename))
 
     # sort the classifiers if present
-    if 'classifiers' in cfg['metadata']:
-        classifiers = _natural_sort(cfg['metadata']['classifiers'].split('\n'))
+    if classifiers:
         classifiers = _trim_py_classifiers(
-            classifiers,
+            _natural_sort(classifiers),
             requires,
             max_py_version=max_py_version,
             include_version_classifiers=include_version_classifiers,
         )
-        cfg['metadata']['classifiers'] = '\n'.join(classifiers)
+        cfg['metadata']['classifiers'] = _fmt_list_always(classifiers)
 
     sections: dict[str, dict[str, str]] = {}
     for section, key_order in KEYS_ORDER:
         if section not in cfg:
             continue
 
         entries = {k.replace('-', '_'): v for k, v in cfg[section].items()}
@@ -507,32 +503,48 @@
     try:
         version = _to_ver(s)
     except UnknownVersionError:
         version = ()
 
     if len(version) != 2:
         raise argparse.ArgumentTypeError(f'expected #.#, got {s!r}')
+    elif version[0] < 3:
+        raise argparse.ArgumentTypeError(f'must be at least 3, got {s!r}')
     else:
         return version
 
 
 def main(argv: Sequence[str] | None = None) -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('filenames', nargs='*')
     parser.add_argument('--include-version-classifiers', action='store_true')
-    parser.add_argument('--min-py3-version', type=_ver_type, default=(3, 7))
+    parser.add_argument(
+        '--min-py3-version', type=_ver_type, default=None,
+        help=argparse.SUPPRESS,
+    )
+    parser.add_argument('--min-py-version', type=_ver_type, default=(3, 7))
     parser.add_argument('--max-py-version', type=_ver_type, default=(3, 11))
     args = parser.parse_args(argv)
 
+    if args.min_py3_version:
+        print(
+            'WARNING: setup-cfg-fmt will replace --min-py3-version '
+            'with --min-py-version in a future release',
+            file=sys.stderr,
+        )
+        min_py_version = args.min_py3_version
+    else:
+        min_py_version = args.min_py_version
+
     retv = 0
     for filename in args.filenames:
         if format_file(
                 filename,
                 include_version_classifiers=args.include_version_classifiers,
-                min_py3_version=args.min_py3_version,
+                min_py_version=min_py_version,
                 max_py_version=args.max_py_version,
         ):
             print(f'Rewriting {filename}')
             retv = 1
     return retv
```

