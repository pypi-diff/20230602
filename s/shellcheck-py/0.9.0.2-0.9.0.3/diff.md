# Comparing `tmp/shellcheck_py-0.9.0.2.tar.gz` & `tmp/shellcheck_py-0.9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcheck_py-0.9.0.2.tar", last modified: Sat Dec 17 19:00:05 2022, max compression
+gzip compressed data, was "shellcheck_py-0.9.0.3.tar", last modified: Thu Jun  1 22:46:05 2023, max compression
```

## Comparing `shellcheck_py-0.9.0.2.tar` & `shellcheck_py-0.9.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-17 19:00:05.028344 shellcheck_py-0.9.0.2/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1066 2022-12-17 18:14:46.000000 shellcheck_py-0.9.0.2/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1736 2022-12-17 19:00:05.028344 shellcheck_py-0.9.0.2/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1103 2022-12-17 18:59:44.000000 shellcheck_py-0.9.0.2/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)      661 2022-12-17 19:00:05.028344 shellcheck_py-0.9.0.2/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5271 2022-12-17 18:59:41.000000 shellcheck_py-0.9.0.2/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-17 19:00:05.028344 shellcheck_py-0.9.0.2/shellcheck_py.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1736 2022-12-17 19:00:04.000000 shellcheck_py-0.9.0.2/shellcheck_py.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      184 2022-12-17 19:00:04.000000 shellcheck_py-0.9.0.2/shellcheck_py.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-12-17 19:00:04.000000 shellcheck_py-0.9.0.2/shellcheck_py.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-12-17 19:00:04.000000 shellcheck_py-0.9.0.2/shellcheck_py.egg-info/top_level.txt
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 22:46:05.787488 shellcheck_py-0.9.0.3/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1066 2023-06-01 22:33:55.000000 shellcheck_py-0.9.0.3/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-01 22:46:05.787488 shellcheck_py-0.9.0.3/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1053 2023-06-01 22:45:45.000000 shellcheck_py-0.9.0.3/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      661 2023-06-01 22:46:05.787488 shellcheck_py-0.9.0.3/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5286 2023-06-01 22:45:48.000000 shellcheck_py-0.9.0.3/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 22:46:05.787488 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-01 22:46:05.000000 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      184 2023-06-01 22:46:05.000000 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 22:46:05.000000 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 22:46:05.000000 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/top_level.txt
```

### Comparing `shellcheck_py-0.9.0.2/LICENSE` & `shellcheck_py-0.9.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shellcheck_py-0.9.0.2/PKG-INFO` & `shellcheck_py-0.9.0.3/shellcheck_py.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
-Name: shellcheck_py
-Version: 0.9.0.2
+Name: shellcheck-py
+Version: 0.9.0.3
 Summary: Python wrapper around invoking shellcheck (https://www.shellcheck.net/)
 Home-page: https://github.com/ryanrhee/shellcheck-py
 Author: Ryan Rhee
 Author-email: pypi@rhee.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/shellcheck-py/shellcheck-py/_apis/build/status/shellcheck-py.shellcheck-py?branchName=main)](https://dev.azure.com/shellcheck-py/shellcheck-py/_build/latest?definitionId=1&branchName=main)
+[![build status](https://github.com/shellcheck-py/shellcheck-py/actions/workflows/main.yml/badge.svg)](https://github.com/shellcheck-py/shellcheck-py/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/shellcheck-py/shellcheck-py/main.svg)](https://results.pre-commit.ci/latest/github/shellcheck-py/shellcheck-py/main)
 
 # shellcheck-py
 
 A python wrapper to provide a pip-installable [shellcheck] binary.
 
 Internally this package provides a convenient way to download the pre-built
@@ -40,14 +40,14 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.2
+    rev: v0.9.0.3
     hooks:
     -   id: shellcheck
 ```
 
 [shellcheck]: https://shellcheck.net
 [pre-commit]: https://pre-commit.com
```

### Comparing `shellcheck_py-0.9.0.2/README.md` & `shellcheck_py-0.9.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://dev.azure.com/shellcheck-py/shellcheck-py/_apis/build/status/shellcheck-py.shellcheck-py?branchName=main)](https://dev.azure.com/shellcheck-py/shellcheck-py/_build/latest?definitionId=1&branchName=main)
+[![build status](https://github.com/shellcheck-py/shellcheck-py/actions/workflows/main.yml/badge.svg)](https://github.com/shellcheck-py/shellcheck-py/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/shellcheck-py/shellcheck-py/main.svg)](https://results.pre-commit.ci/latest/github/shellcheck-py/shellcheck-py/main)
 
 # shellcheck-py
 
 A python wrapper to provide a pip-installable [shellcheck] binary.
 
 Internally this package provides a convenient way to download the pre-built
@@ -23,14 +23,14 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.2
+    rev: v0.9.0.3
     hooks:
     -   id: shellcheck
 ```
 
 [shellcheck]: https://shellcheck.net
 [pre-commit]: https://pre-commit.com
```

### Comparing `shellcheck_py-0.9.0.2/setup.cfg` & `shellcheck_py-0.9.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `shellcheck_py-0.9.0.2/setup.py` & `shellcheck_py-0.9.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         'zip',
         'ae58191b1ea4ffd9e5b15da9134146e636440302ce3e2f46863e8d71c8be1bbb',
     ),
 }
 POSTFIX_SHA256[('cygwin', 'x86_64')] = POSTFIX_SHA256[('win32', 'AMD64')]
 POSTFIX_SHA256[('darwin', 'arm64')] = POSTFIX_SHA256[('darwin', 'x86_64')]
 POSTFIX_SHA256[('linux', 'armv7l')] = POSTFIX_SHA256[('linux', 'armv6hf')]
-PY_VERSION = '2'
+PY_VERSION = '3'
 
 
 def get_download_url() -> tuple[str, str]:
     postfix, sha256 = POSTFIX_SHA256[(sys.platform, platform.machine())]
     url = (
         f'https://github.com/koalaman/shellcheck/releases/download/'
         f'v{SHELLCHECK_VERSION}/shellcheck-v{SHELLCHECK_VERSION}.{postfix}'
@@ -84,15 +84,15 @@
 
     raise AssertionError(f'unreachable {url}')
 
 
 def save_executable(data: bytes, base_dir: str):
     exe = 'shellcheck' if sys.platform != 'win32' else 'shellcheck.exe'
     output_path = os.path.join(base_dir, exe)
-    os.makedirs(base_dir)
+    os.makedirs(base_dir, exist_ok=True)
 
     with open(output_path, 'wb') as fp:
         fp.write(data)
 
     # Mark as executable.
     # https://stackoverflow.com/a/14105527
     mode = os.stat(output_path).st_mode
```

### Comparing `shellcheck_py-0.9.0.2/shellcheck_py.egg-info/PKG-INFO` & `shellcheck_py-0.9.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
-Name: shellcheck-py
-Version: 0.9.0.2
+Name: shellcheck_py
+Version: 0.9.0.3
 Summary: Python wrapper around invoking shellcheck (https://www.shellcheck.net/)
 Home-page: https://github.com/ryanrhee/shellcheck-py
 Author: Ryan Rhee
 Author-email: pypi@rhee.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/shellcheck-py/shellcheck-py/_apis/build/status/shellcheck-py.shellcheck-py?branchName=main)](https://dev.azure.com/shellcheck-py/shellcheck-py/_build/latest?definitionId=1&branchName=main)
+[![build status](https://github.com/shellcheck-py/shellcheck-py/actions/workflows/main.yml/badge.svg)](https://github.com/shellcheck-py/shellcheck-py/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/shellcheck-py/shellcheck-py/main.svg)](https://results.pre-commit.ci/latest/github/shellcheck-py/shellcheck-py/main)
 
 # shellcheck-py
 
 A python wrapper to provide a pip-installable [shellcheck] binary.
 
 Internally this package provides a convenient way to download the pre-built
@@ -40,14 +40,14 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.2
+    rev: v0.9.0.3
     hooks:
     -   id: shellcheck
 ```
 
 [shellcheck]: https://shellcheck.net
 [pre-commit]: https://pre-commit.com
```

