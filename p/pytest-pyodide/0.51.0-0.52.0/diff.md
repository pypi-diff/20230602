# Comparing `tmp/pytest-pyodide-0.51.0.tar.gz` & `tmp/pytest-pyodide-0.52.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-pyodide-0.51.0.tar", last modified: Wed May 10 01:27:35 2023, max compression
+gzip compressed data, was "pytest-pyodide-0.52.0.tar", last modified: Fri Jun  2 01:02:27 2023, max compression
```

## Comparing `pytest-pyodide-0.51.0.tar` & `pytest-pyodide-0.52.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.899367 pytest-pyodide-0.51.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/workflows/filtermatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/workflows/testall.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3384 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/COMPATIBILITY.md
--rw-r--r--   0 runner    (1001) docker     (122)    10400 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9771 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/examples/test_install_package.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/examples/wheels/
--rw-r--r--   0 runner    (1001) docker     (122)    93002 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.899367 pytest-pyodide-0.51.0/pytest_pyodide/
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/_decorator_in_pyodide.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.899367 pytest-pyodide-0.51.0/pytest_pyodide/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/_templates/module_test.html
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/_templates/test.html
--rw-r--r--   0 runner    (1001) docker     (122)     5403 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/copy_files_to_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)    13997 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8300 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/fixture.py
--rw-r--r--   0 runner    (1001) docker     (122)     9186 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/node_test_driver.js
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)     5171 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/run_tests_inside_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)    16829 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10400 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/tests/datafiles/
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/datafiles/in_pyodide_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     9613 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_copy_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     6204 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_fixture.py
--rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_jsassert.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_marker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_run_in_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/workflows/filtermatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/workflows/testall.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/COMPATIBILITY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10398 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9769 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/examples/test_install_package.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/examples/wheels/
+-rw-r--r--   0 runner    (1001) docker     (122)    93002 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/pytest_pyodide/
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/_decorator_in_pyodide.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/pytest_pyodide/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/_templates/module_test.html
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/_templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5403 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/copy_files_to_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13591 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8300 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9186 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/node_test_driver.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5171 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/run_tests_inside_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16829 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10398 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/tests/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/datafiles/in_pyodide_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9613 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_copy_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_jsassert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_marker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_run_in_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_testing.py
```

### Comparing `pytest-pyodide-0.51.0/.github/workflows/build.yaml` & `pytest-pyodide-0.52.0/.github/workflows/build.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
   test:
       uses: ./.github/workflows/testall.yaml
       with:
         build-artifact-name: none
         build-artifact-path: none
-        pyodide-versions: "[0.23.2,0.22.0,0.21.3]"
+        pyodide-versions: "[0.23.2,0.22.0]"
 
   deploy:
     runs-on: ubuntu-20.04
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     environment: PyPi-deploy
     steps:
       - uses: actions/checkout@v3
```

### Comparing `pytest-pyodide-0.51.0/.github/workflows/filtermatrix.py` & `pytest-pyodide-0.52.0/.github/workflows/filtermatrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import yaml
 
 # pyodide versions is a set of versions to test
 # as opposed to other parameters which just filter
 # the configs below
 pyodide_versions = sys.argv[1]
 if pyodide_versions == "*":
-    pyodide_versions = "[0.22.0,0.21.0]"
+    pyodide_versions = "[0.23.2,0.22.0]"
 
 matrix = yaml.safe_load(
     """
 os: [ubuntu-20.04]
 pyodide-version: """
     + pyodide_versions
     + """
@@ -29,23 +29,23 @@
     {runner: selenium, browser: host},
     # playwright browser versions are pinned to playwright version
     {runner: playwright, browser: firefox, runner-version: 1.22.0, driver-version: 18},
     {runner: playwright, browser: chrome, runner-version: 1.22.0, driver-version: 18},
 ]
 include:
     - os: macos-11
-      pyodide-version: 0.21.0
+      pyodide-version: 0.23.2
       test-config: {runner: selenium, browser: safari}
       # the following two tests check that the fallback browser behaviour works
       # okay (this is because ubuntu 22.04 doesn't support getting python 3.10.2)
     - os: ubuntu-latest
-      pyodide-version: 0.21.0
+      pyodide-version: 0.23.2
       test-config: {runner: selenium, browser: node, browser-version: 18}
     - os: ubuntu-22.04
-      pyodide-version: 0.21.0
+      pyodide-version: 0.23.2
       test-config: {runner: selenium, browser: node, browser-version: 18}
 """
 )
 
 ranges: "dict[str, list[tuple[str, str]]]" = {}
 for key in matrix.keys():
     if key != "include":
```

### Comparing `pytest-pyodide-0.51.0/.github/workflows/main.yaml` & `pytest-pyodide-0.52.0/.github/workflows/main.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         type: string
       build-artifact-path:
         required: true
         type: string
       pyodide-version:
         required: false
         type: string
-        default: "0.21.0"
+        default: "0.23.2"
       runner:
         required: false
         type: string
         default: "selenium"
       runner-version:
         required: false
         type: string
@@ -128,14 +128,20 @@
       - name: Download build artifacts from calling package
         if: ${{ inputs.build-artifact-name != 'none' }}
         uses: actions/download-artifact@v3
         with:
           name: ${{ inputs.build-artifact-name }}
           path: ${{ inputs.build-artifact-path }}
 
+      - name: install pyodide-py
+        shell: bash -l {0}
+        run: |
+          ${{needs.get_versions.outputs.pythonexec}} -m pip install pyodide-py==${{inputs.pyodide-version}}
+
+
       - name: Install pytest-pyodide
         shell: bash -l {0}
         run: |
           if [ -d "pytest_pyodide" ]; then
             # Currently we only install the package for dependencies.
             # We then uninstall it otherwise tests fails due to pytest hook being
             # registered twice.
```

### Comparing `pytest-pyodide-0.51.0/.github/workflows/testall.yaml` & `pytest-pyodide-0.52.0/.github/workflows/testall.yaml`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/.pre-commit-config.yaml` & `pytest-pyodide-0.52.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/CHANGELOG.md` & `pytest-pyodide-0.52.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## [0.52.0] - 2023-06-01
+
+- Removed `JsException` unpickle special case. This was fixed by
+  [pyodide/pyodide#3387](https://github.com/pyodide/pyodide/pull/3387).
+  [#91](https://github.com/pyodide/pytest-pyodide/pull/91)
+
+- Dropped support for Pyodide version `0.21.x`.
+  [#91](https://github.com/pyodide/pytest-pyodide/pull/91)
+
 ## [0.51.0] - 2023-05-10
 
 - Added test templates files in the package.
   [#87](https://github.com/pyodide/pytest-pyodide/pull/87)
 
 ## [0.50.0] - 2023-01-05
```

### Comparing `pytest-pyodide-0.51.0/PKG-INFO` & `pytest-pyodide-0.52.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pyodide
-Version: 0.51.0
+Version: 0.52.0
 Summary: "Pytest plugin for testing applications that use Pyodide"
 Home-page: https://github.com/pyodide/pytest-pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pytest-pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -41,63 +41,63 @@
 
 In your github actions workflow, call it with as a aseparate job. To pass in your build wheel use an upload-artifact step in your build step.
 
 This will run your tests on the given browser/pyodide version/OS configuration. It runs pytest in the root of your repo, which should catch any test_\*.py files in subfolders.
 
 ```
 jobs:
-  # Build for pyodide 0.21.0
+  # Build for pyodide 0.23.2
   build:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
-        python-version: 3.10.2
+        python-version: 3.11
     - uses: mymindstorm/setup-emsdk@v11
       with:
-        version: 3.1.14
-    - run: pip install pyodide-build==0.21.0
+        version: 3.1.32
+    - run: pip install pyodide-build==0.23.2
     - run: pyodide build
     - uses: actions/upload-artifact@v3
       with:
         name: pyodide wheel
         path: dist
   # this is the job which you add to run pyodide-test
   test:
     needs: build
     uses: pyodide/pytest-pyodide/.github/workflows/main.yaml@main
     with:
       build-artifact-name: pyodide wheel
       build-artifact-path: dist
       browser: firefox
       runner: selenium
-      pyodide-version: 0.21.0
+      pyodide-version: 0.23.2
 ```
 
 If you want to run on multiple browsers / pyodide versions etc., you can either use a matrix strategy and run main.yaml as above, or you can use testall.yaml. This by default tests on all browsers (and node) with multiple configurations. If you want to reduce the configurations you can filter with lists of browsers, runners, pyodide-versions as shown below.
 ```
   test:
     needs: build
     uses: pyodide/pytest-pyodide/.github/workflows/testall.yaml@main
     with:
       build-artifact-name: pyodide wheel
       build-artifact-path: dist
-      pyodide-versions: [0.21.0,0.23.0]
+      pyodide-versions: [0.22.0,0.23.2]
       runners: [selenium,playwright]
       browsers: [firefox,chrome,node]
       os: [ubuntu-latest,macos-latest]
 ```
 
 ## Usage
 
 1. First you need a compatible version of Pyodide. You can download the Pyodide build artifacts from releases with,
    ```bash
-   wget https://github.com/pyodide/pyodide/releases/download/0.21.0/pyodide-build-0.21.0.tar.bz2
-   tar xjf pyodide-build-0.21.0.tar.bz2
+   wget https://github.com/pyodide/pyodide/releases/download/0.23.2/pyodide-build-0.23.2.tar.bz2
+   tar xjf pyodide-build-0.23.2.tar.bz2
    mv pyodide dist/
    ```
 
 2. You can then use the provided fixtures (`selenium`, `selenium_standalone`) in tests,
    ```py
    def test_a(selenium):
        selenium.run("assert 1+1 == 2")   # run Python with Pyodide
```

### Comparing `pytest-pyodide-0.51.0/README.md` & `pytest-pyodide-0.52.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,63 +25,63 @@
 
 In your github actions workflow, call it with as a aseparate job. To pass in your build wheel use an upload-artifact step in your build step.
 
 This will run your tests on the given browser/pyodide version/OS configuration. It runs pytest in the root of your repo, which should catch any test_\*.py files in subfolders.
 
 ```
 jobs:
-  # Build for pyodide 0.21.0
+  # Build for pyodide 0.23.2
   build:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
-        python-version: 3.10.2
+        python-version: 3.11
     - uses: mymindstorm/setup-emsdk@v11
       with:
-        version: 3.1.14
-    - run: pip install pyodide-build==0.21.0
+        version: 3.1.32
+    - run: pip install pyodide-build==0.23.2
     - run: pyodide build
     - uses: actions/upload-artifact@v3
       with:
         name: pyodide wheel
         path: dist
   # this is the job which you add to run pyodide-test
   test:
     needs: build
     uses: pyodide/pytest-pyodide/.github/workflows/main.yaml@main
     with:
       build-artifact-name: pyodide wheel
       build-artifact-path: dist
       browser: firefox
       runner: selenium
-      pyodide-version: 0.21.0
+      pyodide-version: 0.23.2
 ```
 
 If you want to run on multiple browsers / pyodide versions etc., you can either use a matrix strategy and run main.yaml as above, or you can use testall.yaml. This by default tests on all browsers (and node) with multiple configurations. If you want to reduce the configurations you can filter with lists of browsers, runners, pyodide-versions as shown below.
 ```
   test:
     needs: build
     uses: pyodide/pytest-pyodide/.github/workflows/testall.yaml@main
     with:
       build-artifact-name: pyodide wheel
       build-artifact-path: dist
-      pyodide-versions: [0.21.0,0.23.0]
+      pyodide-versions: [0.22.0,0.23.2]
       runners: [selenium,playwright]
       browsers: [firefox,chrome,node]
       os: [ubuntu-latest,macos-latest]
 ```
 
 ## Usage
 
 1. First you need a compatible version of Pyodide. You can download the Pyodide build artifacts from releases with,
    ```bash
-   wget https://github.com/pyodide/pyodide/releases/download/0.21.0/pyodide-build-0.21.0.tar.bz2
-   tar xjf pyodide-build-0.21.0.tar.bz2
+   wget https://github.com/pyodide/pyodide/releases/download/0.23.2/pyodide-build-0.23.2.tar.bz2
+   tar xjf pyodide-build-0.23.2.tar.bz2
    mv pyodide dist/
    ```
 
 2. You can then use the provided fixtures (`selenium`, `selenium_standalone`) in tests,
    ```py
    def test_a(selenium):
        selenium.run("assert 1+1 == 2")   # run Python with Pyodide
```

### Comparing `pytest-pyodide-0.51.0/examples/test_install_package.py` & `pytest-pyodide-0.52.0/examples/test_install_package.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl` & `pytest-pyodide-0.52.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pyproject.toml` & `pytest-pyodide-0.52.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/__init__.py` & `pytest-pyodide-0.52.0/pytest_pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/_decorator_in_pyodide.py` & `pytest-pyodide-0.52.0/pytest_pyodide/_decorator_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/_templates/module_test.html` & `pytest-pyodide-0.52.0/pytest_pyodide/_templates/module_test.html`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/_templates/test.html` & `pytest-pyodide-0.52.0/pytest_pyodide/_templates/test.html`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/copy_files_to_pyodide.py` & `pytest-pyodide-0.52.0/pytest_pyodide/copy_files_to_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/decorator.py` & `pytest-pyodide-0.52.0/pytest_pyodide/decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from io import BytesIO
 from typing import Any, Protocol
 
 import pytest
 
 from .copy_files_to_pyodide import copy_files_to_emscripten_fs
 from .hook import ORIGINAL_MODULE_ASTS, REWRITTEN_MODULE_ASTS
-from .pyodide import JsException
 from .runner import _BrowserBaseRunner
 from .utils import package_is_built as _package_is_built
 
 
 def package_is_built(package_name: str):
     return _package_is_built(package_name, pytest.pyodide_dist_dir)  # type: ignore[arg-type]
 
@@ -52,24 +51,14 @@
         if not isinstance(pid, tuple) or len(pid) != 2 or pid[0] != "PyodideHandle":
             raise pickle.UnpicklingError("unsupported persistent object")
         ptr = pid[1]
         # the PyodideHandle needs access to selenium in order to free the
         # reference count.
         return PyodideHandle(self.selenium, ptr)
 
-    def find_class(self, module: str, name: str) -> Any:
-        """
-        Catch exceptions that only exist in the pyodide environment and
-        convert them to exception in the host.
-        """
-        if module in ("pyodide", "pyodide.ffi") and name == "JsException":
-            return JsException
-        else:
-            return super().find_class(module, name)
-
 
 class Pickler(pickle.Pickler):
     def persistent_id(self, obj: Any) -> Any:
         if not isinstance(obj, PyodideHandle):
             return None
         return ("PyodideHandle", obj.ptr)
```

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/fixture.py` & `pytest-pyodide-0.52.0/pytest_pyodide/fixture.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/hook.py` & `pytest-pyodide-0.52.0/pytest_pyodide/hook.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/hypothesis.py` & `pytest-pyodide-0.52.0/pytest_pyodide/hypothesis.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/node_test_driver.js` & `pytest-pyodide-0.52.0/pytest_pyodide/node_test_driver.js`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/run_tests_inside_pyodide.py` & `pytest-pyodide-0.52.0/pytest_pyodide/run_tests_inside_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/runner.py` & `pytest-pyodide-0.52.0/pytest_pyodide/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/server.py` & `pytest-pyodide-0.52.0/pytest_pyodide/server.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide/utils.py` & `pytest-pyodide-0.52.0/pytest_pyodide/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide.egg-info/PKG-INFO` & `pytest-pyodide-0.52.0/pytest_pyodide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pyodide
-Version: 0.51.0
+Version: 0.52.0
 Summary: "Pytest plugin for testing applications that use Pyodide"
 Home-page: https://github.com/pyodide/pytest-pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pytest-pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -41,63 +41,63 @@
 
 In your github actions workflow, call it with as a aseparate job. To pass in your build wheel use an upload-artifact step in your build step.
 
 This will run your tests on the given browser/pyodide version/OS configuration. It runs pytest in the root of your repo, which should catch any test_\*.py files in subfolders.
 
 ```
 jobs:
-  # Build for pyodide 0.21.0
+  # Build for pyodide 0.23.2
   build:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
-        python-version: 3.10.2
+        python-version: 3.11
     - uses: mymindstorm/setup-emsdk@v11
       with:
-        version: 3.1.14
-    - run: pip install pyodide-build==0.21.0
+        version: 3.1.32
+    - run: pip install pyodide-build==0.23.2
     - run: pyodide build
     - uses: actions/upload-artifact@v3
       with:
         name: pyodide wheel
         path: dist
   # this is the job which you add to run pyodide-test
   test:
     needs: build
     uses: pyodide/pytest-pyodide/.github/workflows/main.yaml@main
     with:
       build-artifact-name: pyodide wheel
       build-artifact-path: dist
       browser: firefox
       runner: selenium
-      pyodide-version: 0.21.0
+      pyodide-version: 0.23.2
 ```
 
 If you want to run on multiple browsers / pyodide versions etc., you can either use a matrix strategy and run main.yaml as above, or you can use testall.yaml. This by default tests on all browsers (and node) with multiple configurations. If you want to reduce the configurations you can filter with lists of browsers, runners, pyodide-versions as shown below.
 ```
   test:
     needs: build
     uses: pyodide/pytest-pyodide/.github/workflows/testall.yaml@main
     with:
       build-artifact-name: pyodide wheel
       build-artifact-path: dist
-      pyodide-versions: [0.21.0,0.23.0]
+      pyodide-versions: [0.22.0,0.23.2]
       runners: [selenium,playwright]
       browsers: [firefox,chrome,node]
       os: [ubuntu-latest,macos-latest]
 ```
 
 ## Usage
 
 1. First you need a compatible version of Pyodide. You can download the Pyodide build artifacts from releases with,
    ```bash
-   wget https://github.com/pyodide/pyodide/releases/download/0.21.0/pyodide-build-0.21.0.tar.bz2
-   tar xjf pyodide-build-0.21.0.tar.bz2
+   wget https://github.com/pyodide/pyodide/releases/download/0.23.2/pyodide-build-0.23.2.tar.bz2
+   tar xjf pyodide-build-0.23.2.tar.bz2
    mv pyodide dist/
    ```
 
 2. You can then use the provided fixtures (`selenium`, `selenium_standalone`) in tests,
    ```py
    def test_a(selenium):
        selenium.run("assert 1+1 == 2")   # run Python with Pyodide
```

### Comparing `pytest-pyodide-0.51.0/pytest_pyodide.egg-info/SOURCES.txt` & `pytest-pyodide-0.52.0/pytest_pyodide.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 ./pytest_pyodide/_decorator_in_pyodide.py
 ./pytest_pyodide/copy_files_to_pyodide.py
 ./pytest_pyodide/decorator.py
 ./pytest_pyodide/fixture.py
 ./pytest_pyodide/hook.py
 ./pytest_pyodide/hypothesis.py
 ./pytest_pyodide/node_test_driver.js
-./pytest_pyodide/pyodide.py
 ./pytest_pyodide/run_tests_inside_pyodide.py
 ./pytest_pyodide/runner.py
 ./pytest_pyodide/server.py
 ./pytest_pyodide/utils.py
 ./pytest_pyodide/_templates/__init__.py
 ./pytest_pyodide/_templates/module_test.html
 ./pytest_pyodide/_templates/test.html
@@ -35,15 +34,14 @@
 pytest_pyodide/_decorator_in_pyodide.py
 pytest_pyodide/copy_files_to_pyodide.py
 pytest_pyodide/decorator.py
 pytest_pyodide/fixture.py
 pytest_pyodide/hook.py
 pytest_pyodide/hypothesis.py
 pytest_pyodide/node_test_driver.js
-pytest_pyodide/pyodide.py
 pytest_pyodide/run_tests_inside_pyodide.py
 pytest_pyodide/runner.py
 pytest_pyodide/server.py
 pytest_pyodide/utils.py
 pytest_pyodide.egg-info/PKG-INFO
 pytest_pyodide.egg-info/SOURCES.txt
 pytest_pyodide.egg-info/dependency_links.txt
```

### Comparing `pytest-pyodide-0.51.0/setup.cfg` & `pytest-pyodide-0.52.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/tests/datafiles/in_pyodide_tests.py` & `pytest-pyodide-0.52.0/tests/datafiles/in_pyodide_tests.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl` & `pytest-pyodide-0.52.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/tests/test_copy_files.py` & `pytest-pyodide-0.52.0/tests/test_copy_files.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/tests/test_decorator.py` & `pytest-pyodide-0.52.0/tests/test_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from hypothesis import given, settings
 
+from pyodide.ffi import JsException
 from pytest_pyodide.decorator import run_in_pyodide
 from pytest_pyodide.hypothesis import any_strategy, std_hypothesis_settings
-from pytest_pyodide.pyodide import JsException
 from pytest_pyodide.utils import parse_driver_timeout
 
 
 @run_in_pyodide
 def example_func(selenium):
     pass
```

### Comparing `pytest-pyodide-0.51.0/tests/test_jsassert.py` & `pytest-pyodide-0.52.0/tests/test_jsassert.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/tests/test_options.py` & `pytest-pyodide-0.52.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/tests/test_run_in_pyodide.py` & `pytest-pyodide-0.52.0/tests/test_run_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/tests/test_server.py` & `pytest-pyodide-0.52.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.51.0/tests/test_testing.py` & `pytest-pyodide-0.52.0/tests/test_testing.py`

 * *Files identical despite different names*

