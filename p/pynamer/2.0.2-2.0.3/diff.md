# Comparing `tmp/pynamer-2.0.2.tar.gz` & `tmp/pynamer-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.0.2.tar", last modified: Wed May 31 14:21:50 2023, max compression
+gzip compressed data, was "pynamer-2.0.3.tar", last modified: Fri Jun  2 19:53:05 2023, max compression
```

## Comparing `pynamer-2.0.2.tar` & `pynamer-2.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.394847 pynamer-2.0.2/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.0.2/AUTHORS.md
--rw-rw-rw-   0        0        0     9954 2023-05-31 14:21:35.000000 pynamer-2.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.0.2/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    18786 2023-05-31 14:21:50.394847 pynamer-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    17203 2023-05-29 12:32:43.000000 pynamer-2.0.2/README.md
--rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1818 2023-05-31 14:21:50.394847 pynamer-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.067667 pynamer-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.131705 pynamer-2.0.2/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.0.2/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1853 2023-05-31 14:21:35.000000 pynamer-2.0.2/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.0.2/src/pynamer/builder.py
--rw-rw-rw-   0        0        0     2210 2023-05-28 18:04:31.000000 pynamer-2.0.2/src/pynamer/cli.py
--rw-rw-rw-   0        0        0      726 2023-05-25 17:08:55.000000 pynamer-2.0.2/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.147333 pynamer-2.0.2/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.0.2/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     7524 2023-05-31 13:31:21.000000 pynamer-2.0.2/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-05-24 15:24:28.000000 pynamer-2.0.2/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.0.2/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0     9587 2023-05-31 14:18:45.000000 pynamer-2.0.2/src/pynamer/utils.py
--rw-rw-rw-   0        0        0     7788 2023-05-31 13:49:32.000000 pynamer-2.0.2/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.147333 pynamer-2.0.2/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    18786 2023-05-31 14:21:49.000000 pynamer-2.0.2/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1130 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.394847 pynamer-2.0.2/tests/
--rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1541 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     1721 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.0.2/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.269421 pynamer-2.0.3/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.0.3/AUTHORS.md
+-rw-rw-rw-   0        0        0    10114 2023-06-02 19:52:49.000000 pynamer-2.0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    18796 2023-06-02 19:53:05.270421 pynamer-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    17213 2023-06-02 18:15:07.000000 pynamer-2.0.3/README.md
+-rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1818 2023-06-02 19:53:05.272434 pynamer-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:04.933347 pynamer-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.017348 pynamer-2.0.3/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.0.3/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1929 2023-06-02 19:52:50.000000 pynamer-2.0.3/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.0.3/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2210 2023-05-28 18:04:31.000000 pynamer-2.0.3/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      726 2023-05-25 17:08:55.000000 pynamer-2.0.3/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.027346 pynamer-2.0.3/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.0.3/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7524 2023-05-31 13:31:21.000000 pynamer-2.0.3/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-05-24 15:24:28.000000 pynamer-2.0.3/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.0.3/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0     9587 2023-05-31 14:18:45.000000 pynamer-2.0.3/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0     8280 2023-06-02 19:50:27.000000 pynamer-2.0.3/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.025348 pynamer-2.0.3/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    18796 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1130 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.267449 pynamer-2.0.3/tests/
+-rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1541 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     1700 2023-06-02 19:42:16.000000 pynamer-2.0.3/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.0.3/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_write_output_file.py
```

### Comparing `pynamer-2.0.2/CHANGELOG.md` & `pynamer-2.0.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.0.3 (2023-06-02)
+### Fix
+* Json formatting ([`892a454`](https://github.com/Stephen-RA-King/pynamer/commit/892a454d47c868973978e54be89f472ae351b455))
+
 ## v2.0.2 (2023-05-31)
 ### Fix
 * Account for nonetype returned in json data ([`39f245c`](https://github.com/Stephen-RA-King/pynamer/commit/39f245c41b17add26ed9399dbb3c376cd395d79b))
 
 ## v2.0.1 (2023-05-29)
 ### Documentation
 * Final updates ([`6c85802`](https://github.com/Stephen-RA-King/pynamer/commit/6c85802a132e91586d8d21c0ceb6dcf8f011264d))
```

### Comparing `pynamer-2.0.2/LICENSE` & `pynamer-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/PKG-INFO` & `pynamer-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.0.2
-Summary: Utility to find an available package name on the PyPI repository and register it
+Version: 2.0.3
+Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
-_**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
+_**Utility to find an available package name in the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
@@ -45,15 +45,15 @@
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
 
-As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' on PyPI.
+As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' in PyPI.
 
 ![](assets/pynamer.png)
 
 # Contents
 
 -   [tl;dr](#TLDR)
 -   [Introduction](#Introduction)
@@ -157,15 +157,15 @@
 The following are optional but required for 'registering' a project name on PyPI
 
 -   [x] An account on PyPI (and generate a PyPI API token).
 -   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
 
     or
 
--   [x] [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
+-   [x] Configure [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
 
 Your .pypirc file should contain the following and be on your PATH:
 
 ```file
 [distutils]
 index-servers =
     pypi
```

### Comparing `pynamer-2.0.2/README.md` & `pynamer-2.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
+_**Utility to find an available package name in the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
@@ -16,15 +16,15 @@
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
 
-As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' on PyPI.
+As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' in PyPI.
 
 ![](assets/pynamer.png)
 
 # Contents
 
 -   [tl;dr](#TLDR)
 -   [Introduction](#Introduction)
@@ -128,15 +128,15 @@
 The following are optional but required for 'registering' a project name on PyPI
 
 -   [x] An account on PyPI (and generate a PyPI API token).
 -   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
 
     or
 
--   [x] [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
+-   [x] Configure [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
 
 Your .pypirc file should contain the following and be on your PATH:
 
 ```file
 [distutils]
 index-servers =
     pypi
```

### Comparing `pynamer-2.0.2/pyproject.toml` & `pynamer-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/setup.cfg` & `pynamer-2.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 5374 6570 6865 6e20 5220 4120 4b69 6e67  Stephen R A King
 000000a0: 0d0a 6d61 696e 7461 696e 6572 5f65 6d61  ..maintainer_ema
 000000b0: 696c 203d 2073 6b69 6e67 2e67 6974 6875  il = sking.githu
 000000c0: 6240 676d 6169 6c2e 636f 6d0d 0a64 6573  b@gmail.com..des
 000000d0: 6372 6970 7469 6f6e 203d 2055 7469 6c69  cription = Utili
 000000e0: 7479 2074 6f20 6669 6e64 2061 6e20 6176  ty to find an av
 000000f0: 6169 6c61 626c 6520 7061 636b 6167 6520  ailable package 
-00000100: 6e61 6d65 206f 6e20 7468 6520 5079 5049  name on the PyPI
+00000100: 6e61 6d65 2069 6e20 7468 6520 5079 5049  name in the PyPI
 00000110: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
 00000120: 7265 6769 7374 6572 2069 740d 0a6c 6f6e  register it..lon
 00000130: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
 00000140: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
 00000150: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000160: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 00000170: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
```

### Comparing `pynamer-2.0.2/src/pynamer/__init__.py` & `pynamer-2.0.3/src/pynamer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
 
+__all__ = ["builder", "cli", "config", "pynamer", "utils", "validators"]
+
 
 LOGGING_CONFIG = """
 version: 1
 disable_existing_loggers: True
 handlers:
   console:
     class: logging.StreamHandler
```

### Comparing `pynamer-2.0.2/src/pynamer/builder.py` & `pynamer-2.0.3/src/pynamer/builder.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/src/pynamer/cli.py` & `pynamer-2.0.3/src/pynamer/cli.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/src/pynamer/config.py` & `pynamer-2.0.3/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/src/pynamer/pynamer.py` & `pynamer-2.0.3/src/pynamer/pynamer.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/src/pynamer/utils.py` & `pynamer-2.0.3/src/pynamer/utils.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/src/pynamer/validators.py` & `pynamer-2.0.3/src/pynamer/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,19 +77,35 @@
     try:
         project_json_raw = requests.get(url_json, timeout=5)
     except requests.RequestException as e:
         logger.error("An error occurred: %s", e)
         raise SystemExit("An error occurred with an HTTP request")
     if project_json_raw.status_code == 200:
         project_json = json.loads(project_json_raw.content)
-        author = project_json["info"]["author"] or ""
-        email = project_json["info"]["author_email"] or ""
-        version = project_json["info"]["version"] or ""
-        summary = project_json["info"]["summary"] or ""
-        result = "".join([author, "\n", email, "\n", version, "\n", summary])
+        author = (
+            "".join(["Author:  ", project_json["info"]["author"]])
+            if project_json["info"]["author"]
+            else "Author:  None"
+        )
+        version = (
+            "".join(["Version: ", project_json["info"]["version"]])
+            if project_json["info"]["version"]
+            else "Version: None"
+        )
+        email = (
+            "".join(["Email:   ", project_json["info"]["author_email"]])
+            if project_json["info"]["author_email"]
+            else "Email:   None"
+        )
+        summary = (
+            "".join(["Summary: ", project_json["info"]["summary"]])
+            if project_json["info"]["summary"]
+            else "Summary: None"
+        )
+        result = "".join([summary, "\n", author, "\n", email, "\n", version])
         return result
     logger.debug("No response from JSON URL")
     return ""
 
 
 def _pypi_search_index(project_name: str) -> bool:
     """Open the generated index file and search for the project name.
```

### Comparing `pynamer-2.0.2/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.0.3/src/pynamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.0.2
-Summary: Utility to find an available package name on the PyPI repository and register it
+Version: 2.0.3
+Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
-_**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
+_**Utility to find an available package name in the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
@@ -45,15 +45,15 @@
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
 
-As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' on PyPI.
+As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' in PyPI.
 
 ![](assets/pynamer.png)
 
 # Contents
 
 -   [tl;dr](#TLDR)
 -   [Introduction](#Introduction)
@@ -157,15 +157,15 @@
 The following are optional but required for 'registering' a project name on PyPI
 
 -   [x] An account on PyPI (and generate a PyPI API token).
 -   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
 
     or
 
--   [x] [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
+-   [x] Configure [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
 
 Your .pypirc file should contain the following and be on your PATH:
 
 ```file
 [distutils]
 index-servers =
     pypi
```

### Comparing `pynamer-2.0.2/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.0.3/src/pynamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_args.py` & `pynamer-2.0.3/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_build_dist.py` & `pynamer-2.0.3/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_cleanup.py` & `pynamer-2.0.3/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_create_setup_file.py` & `pynamer-2.0.3/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_defaults.py` & `pynamer-2.0.3/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_delete_director.py` & `pynamer-2.0.3/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_feedback.py` & `pynamer-2.0.3/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_final_analysis.py` & `pynamer-2.0.3/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_find_pypirc_file.py` & `pynamer-2.0.3/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_generate_pypi_index.py` & `pynamer-2.0.3/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_ping_json.py` & `pynamer-2.0.3/tests/test_ping_json.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!/usr/bin/env python3
-# Core Library modules
-import pickle
-from pathlib import Path
-
-# Third party modules
-import pytest
-import requests
-from requests.exceptions import ConnectTimeout
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-expected_response_found = """Stephen R A King
-sking.github@gmail.com
-1.5.5
-Utility command line tool to manage python versions"""
-
-
-def my_custom_get_found(url, **kwargs):
-    # Implement your custom logic here
-    _pickle_file = BASE_DIR / "resources" / "requests_get_json_pynball.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def my_custom_get_not_found(url, **kwargs):
-    _pickle_file = BASE_DIR / "resources" / "requests_get_json_zeedonk.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def test_ping_json_found(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_found)
-    result = pynamer._ping_json("pynball")
-    assert result == expected_response_found
-
-
-def test_ping_json_not_found(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_not_found)
-    result = pynamer._ping_json("zeedonk")
-    assert result == ""
-
-
-def test_ping_json_error(monkeypatch):
-    def mock_requests_error(*args, **kwargs):
-        raise ConnectTimeout("Connection timed out")
-
-    monkeypatch.setattr(requests, "get", mock_requests_error)
-
-    with pytest.raises(SystemExit) as excinfo:
-        pynamer._ping_json("pynball")
-    assert str(excinfo.value) == "An error occurred with an HTTP request"
+#!/usr/bin/env python3
+# Core Library modules
+import pickle
+from pathlib import Path
+
+# Third party modules
+import pytest
+import requests
+from requests.exceptions import ConnectTimeout
+
+# First party modules
+from pynamer import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+expected_response_found = """Summary: Utility command line tool to manage python versions
+Author:  Stephen R A King
+Email:   sking.github@gmail.com
+Version: 1.5.5"""
+
+
+def my_custom_get_found(url, **kwargs):
+    # Implement your custom logic here
+    _pickle_file = BASE_DIR / "resources" / "requests_get_json_pynball.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def my_custom_get_not_found(url, **kwargs):
+    _pickle_file = BASE_DIR / "resources" / "requests_get_json_zeedonk.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def test_ping_json_found(monkeypatch):
+    monkeypatch.setattr(requests, "get", my_custom_get_found)
+    result = pynamer._ping_json("pynball")
+    assert result == expected_response_found
+
+
+def test_ping_json_not_found(monkeypatch):
+    monkeypatch.setattr(requests, "get", my_custom_get_not_found)
+    result = pynamer._ping_json("zeedonk")
+    assert result == ""
+
+
+def test_ping_json_error(monkeypatch):
+    def mock_requests_error(*args, **kwargs):
+        raise ConnectTimeout("Connection timed out")
+
+    monkeypatch.setattr(requests, "get", mock_requests_error)
+
+    with pytest.raises(SystemExit) as excinfo:
+        pynamer._ping_json("pynball")
+    assert str(excinfo.value) == "An error occurred with an HTTP request"
```

### Comparing `pynamer-2.0.2/tests/test_ping_project.py` & `pynamer-2.0.3/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_process_input_file.py` & `pynamer-2.0.3/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_pypi_search.py` & `pynamer-2.0.3/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_pypi_search_index.py` & `pynamer-2.0.3/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_rename_project_dir.py` & `pynamer-2.0.3/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_upload_dist.py` & `pynamer-2.0.3/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_utils_version.py` & `pynamer-2.0.3/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.2/tests/test_write_output_file.py` & `pynamer-2.0.3/tests/test_write_output_file.py`

 * *Files identical despite different names*

