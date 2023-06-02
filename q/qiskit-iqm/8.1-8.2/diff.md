# Comparing `tmp/qiskit-iqm-8.1.tar.gz` & `tmp/qiskit-iqm-8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-iqm-8.1.tar", last modified: Mon May 29 08:27:56 2023, max compression
+gzip compressed data, was "qiskit-iqm-8.2.tar", last modified: Fri Jun  2 08:10:11 2023, max compression
```

## Comparing `qiskit-iqm-8.1.tar` & `qiskit-iqm-8.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.722275 qiskit-iqm-8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/examples/bell_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.722275 qiskit-iqm-8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.730276 qiskit-iqm-8.1/src/qiskit_iqm/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.730276 qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/qiskit_to_iqm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.730276 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/tests/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/fake_backends/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/fake_backends/test_fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/fake_backends/test_iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_iqm_facade_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_qiskit_to_iqm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.762906 qiskit-iqm-8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-02 08:10:11.762906 qiskit-iqm-8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/examples/bell_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:10:11.762906 qiskit-iqm-8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/src/qiskit_iqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/qiskit_to_iqm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/tests/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/fake_backends/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/fake_backends/test_fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/fake_backends/test_iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_iqm_facade_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_qiskit_to_iqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tox.ini
```

### Comparing `qiskit-iqm-8.1/.github/workflows/ci.yml` & `qiskit-iqm-8.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/.github/workflows/publish.yml` & `qiskit-iqm-8.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/.github/workflows/tag_and_release.yml` & `qiskit-iqm-8.2/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/CHANGELOG.rst` & `qiskit-iqm-8.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+Version 8.2
+============
+
+* Add ``heralding`` option to ``IQMBackend``. `#63 <https://github.com/iqm-finland/qiskit-on-iqm/pull/63>`_
+* Upgrade to ``IQMClient`` version 12.5. `#63 <https://github.com/iqm-finland/qiskit-on-iqm/pull/63>`_
+
 Version 8.1
 ===========
 
 * Upgrade to IQMClient version 12.4 `#61 <https://github.com/iqm-finland/qiskit-on-iqm/pull/61>`_
 * Add parameter ``circuit_duration_check`` allowing to control server-side maximum circuit duration check `#61 <https://github.com/iqm-finland/qiskit-on-iqm/pull/61>`_
 
 Version 8.0
```

### Comparing `qiskit-iqm-8.1/CONTRIBUTING.rst` & `qiskit-iqm-8.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/LICENSE` & `qiskit-iqm-8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/PKG-INFO` & `qiskit-iqm-8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 8.1
+Version: 8.2
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-8.1/README.rst` & `qiskit-iqm-8.2/README.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/docs/Makefile` & `qiskit-iqm-8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/docs/_static/images/favicon.ico` & `qiskit-iqm-8.2/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/docs/_static/images/logo.png` & `qiskit-iqm-8.2/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/docs/_templates/autosummary-class-template.rst` & `qiskit-iqm-8.2/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/docs/_templates/autosummary-module-template.rst` & `qiskit-iqm-8.2/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/docs/_templates/page.html` & `qiskit-iqm-8.2/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/docs/_templates/versioning.html` & `qiskit-iqm-8.2/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/docs/conf.py` & `qiskit-iqm-8.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 default_py_root = os.path.join(os.getcwd(), os.path.dirname(__file__))
 py_path = os.path.join(os.getenv("SPHINX_MULTIVERSION_SOURCEDIR", default=default_py_root), "../src")
 sys.path.insert(0, os.path.abspath(py_path))
 
 # -- Project information -----------------------------------------------------
 
 project = 'Qiskit on IQM'
-copyright = '2022, Qiskit on IQM developers'
+copyright = '2022-2023, Qiskit on IQM developers'
 author = 'Qiskit on IQM developers'
 
 # The short X.Y version.
 version = ''
 # The full version, including alpha/beta/rc tags.
 release = ''
 try:
@@ -149,14 +149,16 @@
 python_version = '.'.join(map(str, sys.version_info[0:2]))
 intersphinx_mapping = {
     'sphinx': ('https://www.sphinx-doc.org/en/master', None),
     'python': ('https://docs.python.org/' + python_version, None),
     'matplotlib': ('https://matplotlib.org/stable', None),
     'numpy': ('https://numpy.org/doc/stable', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/reference', None),
+    'qiskit': ('https://qiskit.org/documentation', None),
+    'iqm_client': ('https://iqm-finland.github.io/iqm-client', None),
 }
 
 extlinks = {
     'issue': ('https://github.com/iqm-finland/qiskit-on-iqm/issues/%s', 'issue '),
     'mr': ('https://github.com/iqm-finland/qiskit-on-iqm/pull/%s', 'MR '),
 }
```

### Comparing `qiskit-iqm-8.1/docs/index.rst` & `qiskit-iqm-8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/docs/user_guide.rst` & `qiskit-iqm-8.2/docs/user_guide.rst`

 * *Files 6% similar despite different names*

```diff
@@ -93,33 +93,55 @@
 
     job = execute(qc, backend, shots=1000)
 
     print(job.result().get_counts())
 
 Note that the code snippet above assumes that you have set the variable ``iqm_server_url``.
 
-You can optionally set IQM backend specific settings as additional keyword arguments to the ``execute`` method (which
-passes the values down to :meth:`.IQMBackend.run`). For example, an IQM server uses the best available calibration set
-automatically; however, if you know an ID (UUID4) of a specific calibration set that you want to use, you can provide it
-as follows:
+You can optionally set IQM backend specific options as additional keyword arguments to the ``execute`` method (which
+passes the values down to :meth:`.IQMBackend.run`). For example, if you know an ID of a specific calibration set that
+you want to use, you can provide it as follows:
 
 .. code-block:: python
 
     job = execute(circuit, backend, shots=1000, calibration_set_id="f7d9642e-b0ca-4f2d-af2a-30195bd7a76d")
 
-Another example is disabling the server-side circuit duration check. If any circuit in a job would take too long to
-execute compared to the coherence time of the QPU, the server will disqualify the job and not execute any circuits.
-In some special cases, you may want to disable this as follows:
 
-.. code-block:: python
-
-    job = execute(circuit, backend, shots=1000, circuit_duration_check=False)
-
-Disabling the circuit duration check may be limited to certain users or groups, depending on the server settings.
-In normal use, the circuit duration check should always remain enabled.
+Alternatively, you can update the values of the options directly on the backend instance using the :meth:`.IQMBackend.set_options`
+and then call execution methods without specifying additional keyword arguments. You can view all available options and
+their current values using `backend.options`. Below table summarizes currently available options:
+
+.. list-table::
+   :widths: 25 20 25 100
+   :header-rows: 1
+
+   * - Name
+     - Type
+     - Example value
+     - Description
+   * - `shots`
+     - int
+     - 1207
+     - Number of shots.
+   * - `calibration_set_id`
+     - str
+     - "f7d9642e-b0ca-4f2d-af2a-30195bd7a76d"
+     - Indicates the calibration set to use. By default it is `None`, which means an IQM server will use the best
+       available calibration set automatically. The value is string representation of a UUID.
+   * - `circuit_duration_check`
+     - bool
+     - False
+     - Enable/Disable server-side circuit duration check. The default value is `True`, which means if any job is
+       estimated to take unreasonably long compared to the coherence time of the QPU, or too long in wall-clock time,
+       the server will reject it. This option can be used to consciously disable this behaviour. Disabling may be
+       limited to certain users or groups. In normal use, the circuit duration check should always remain enabled.
+   * - `heralding_mode`
+     - :py:class:`~iqm_client.iqm_client.HeraldingMode`
+     - "zeros"
+     - Heralding mode to use during execution. The default value is "none".
 
 If the IQM server you are connecting to requires authentication, you will also have to use
 `Cortex CLI <https://github.com/iqm-finland/cortex-cli>`_ to retrieve and automatically refresh access tokens,
 then set the ``IQM_TOKENS_FILE`` environment variable to use those tokens.
 See Cortex CLI's `documentation <https://iqm-finland.github.io/cortex-cli/readme.html>`__ for details.
 Alternatively, authorize with the IQM_AUTH_SERVER, IQM_AUTH_USERNAME and IQM_AUTH_PASSWORD environment variables
 or pass them as arguments to the constructor of :class:`.IQMProvider`, however this approach is less secure
```

### Comparing `qiskit-iqm-8.1/examples/bell_measure.py` & `qiskit-iqm-8.2/examples/bell_measure.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/pyproject.toml` & `qiskit-iqm-8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License"
 ]
 requires-python = ">=3.9, <3.11"
 dependencies = [
     "numpy",
     "qiskit ~= 0.42.1",
-    "iqm-client >= 12.4, < 13.0"
+    "iqm-client >= 12.5, < 13.0"
 ]
 
 [project.urls]
 homepage = "https://github.com/iqm-finland/qiskit-on-iqm"
 documentation = "https://iqm-finland.github.io/qiskit-on-iqm"
 repository = "https://github.com/iqm-finland/qiskit-on-iqm.git"
 changelog = "https://github.com/iqm-finland/qiskit-on-iqm/blob/main/CHANGELOG.rst"
```

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm/__init__.py` & `qiskit-iqm-8.2/src/qiskit_iqm/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/__init__.py` & `qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/fake_adonis.py` & `qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/iqm_fake_backend.py` & `qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm/iqm_backend.py` & `qiskit-iqm-8.2/src/qiskit_iqm/iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm/iqm_job.py` & `qiskit-iqm-8.2/src/qiskit_iqm/iqm_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 from collections import Counter
 from datetime import date
 from typing import Optional, Union
 import uuid
 
-from iqm_client import CircuitMeasurementResults, IQMClient, RunRequest, RunResult, Status
+from iqm_client import CircuitMeasurementResults, HeraldingMode, IQMClient, RunRequest, RunResult, Status
 import numpy as np
 from qiskit.providers import JobStatus, JobV1
 from qiskit.result import Counts, Result
 
 from qiskit_iqm.qiskit_to_iqm import MeasurementKey
 
 
@@ -46,45 +46,50 @@
         self.circuit_metadata: Optional[list] = None  # Metadata that was originally associated with circuits by user
 
     def _format_iqm_results(self, iqm_result: RunResult) -> list[tuple[str, list[str]]]:
         """Convert the measurement results from a circuit(s) run into the Qiskit format."""
         if iqm_result.measurements is None:
             raise ValueError(f'Cannot format IQM result without measurements. Job status is ${iqm_result.status}')
 
-        shots = self.metadata.get('shots', iqm_result.metadata.request.shots)
-        shape = (shots, 1)  # only one qubit is measured per measurement op
+        requested_shots = self.metadata.get('shots', iqm_result.metadata.request.shots)
+        # If no heralding, for all circuits we expect the same number of shots which is the shots requested by user.
+        expect_exact_shots = iqm_result.metadata.request.heralding_mode == HeraldingMode.NONE
 
         return [
-            (circuit.name, self._format_measurement_results(measurements, shape))
+            (circuit.name, self._format_measurement_results(measurements, requested_shots, expect_exact_shots))
             for measurements, circuit in zip(iqm_result.measurements, iqm_result.metadata.request.circuits)
         ]
 
     @staticmethod
     def _format_measurement_results(
-        measurement_results: CircuitMeasurementResults, shape: tuple[int, int]
+        measurement_results: CircuitMeasurementResults, requested_shots: int, expect_exact_shots: bool = True
     ) -> list[str]:
         formatted_results: dict[int, np.ndarray] = {}
-        shots = shape[0]
         for k, v in measurement_results.items():
             mk = MeasurementKey.from_string(k)
             res = np.array(v, dtype=int)
-
-            if res.shape != shape:
-                raise ValueError(f'Measurement result {mk} has the wrong shape {res.shape}, expected {shape}')
+            # in Qiskit each measurement is a separate single-qubit instruction. qiskit-iqm assigns unique measurement
+            # key to each such instruction, so only one column is expected per measurement key.
+            if res.shape[1] != 1:
+                raise ValueError(f'Measurement result {mk} has the wrong shape {res.shape}, expected (*, 1)')
             res = res[:, 0]
 
+            shots = len(res)
+            if expect_exact_shots and shots != requested_shots:
+                raise ValueError(f'Expected {requested_shots} shots but got {shots} for measurement result {mk}')
+
             # group the measurements into cregs, fill in zeros for unused bits
             creg = formatted_results.setdefault(mk.creg_idx, np.zeros((shots, mk.creg_len), dtype=int))
             creg[:, mk.clbit_idx] = res
 
         # 1. Loop over the registers in the reverse order they were added to the circuit.
         # 2. Within each register the highest index is the most significant, so it goes to the leftmost position.
         return [
             ' '.join(''.join(map(str, res[s, ::-1])) for _, res in sorted(formatted_results.items(), reverse=True))
-            for s in range(shots)
+            for s in range(len(res))
         ]
 
     def submit(self):
         raise NotImplementedError(
             'You should never have to submit jobs by calling this method. When running circuits through '
             'RemoteIQMBackend, the submission will happen under the hood. The job instance that you get is only for '
             'checking the progress and retrieving the results of the submitted job.'
```

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm/iqm_provider.py` & `qiskit-iqm-8.2/src/qiskit_iqm/iqm_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Qiskit Backend Provider for IQM backends.
 """
 from importlib.metadata import version
 from functools import reduce
 from typing import Optional, Union
+from uuid import UUID
 import warnings
 
-from iqm_client import Circuit, Instruction, IQMClient
+from iqm_client import Circuit, HeraldingMode, Instruction, IQMClient
 from iqm_client.util import to_json_dict
 import numpy as np
 from qiskit import QuantumCircuit
 from qiskit.providers import JobStatus, JobV1, Options
 
 from qiskit_iqm.fake_backends import IQMFakeAdonis
 from qiskit_iqm.iqm_backend import IQMBackendBase
@@ -40,15 +41,17 @@
 
     def __init__(self, client: IQMClient, **kwargs):
         super().__init__(client.get_quantum_architecture(), **kwargs)
         self.client = client
 
     @classmethod
     def _default_options(cls) -> Options:
-        return Options(shots=1024, calibration_set_id=None, circuit_duration_check=True)
+        return Options(
+            shots=1024, calibration_set_id=None, circuit_duration_check=True, heralding_mode=HeraldingMode.NONE
+        )
 
     @property
     def max_circuits(self) -> Optional[int]:
         return None
 
     def run(self, run_input: Union[QuantumCircuit, list[QuantumCircuit]], **options) -> IQMJob:
         if self.client is None:
@@ -58,28 +61,30 @@
 
         if len(circuits) == 0:
             raise ValueError('Empty list of circuits submitted for execution.')
 
         shots = options.get('shots', self.options.shots)
         calibration_set_id = options.get('calibration_set_id', self.options.calibration_set_id)
         circuit_duration_check = options.get('circuit_duration_check', self.options.circuit_duration_check)
+        heralding_mode = options.get('heralding_mode', self.options.heralding_mode)
 
         circuits_serialized: list[Circuit] = [self.serialize_circuit(circuit) for circuit in circuits]
         used_indices: set[int] = reduce(
             lambda qubits, circuit: qubits.union(set(int(q) for q in circuit.all_qubits())), circuits_serialized, set()
         )
         qubit_mapping = {str(idx): qb for idx, qb in self._idx_to_qb.items() if idx in used_indices}
-        uuid = self.client.submit_circuits(
+        job_id = self.client.submit_circuits(
             circuits_serialized,
             qubit_mapping=qubit_mapping,
-            calibration_set_id=calibration_set_id,
+            calibration_set_id=UUID(calibration_set_id) if calibration_set_id else None,
             shots=shots,
             circuit_duration_check=circuit_duration_check,
+            heralding_mode=heralding_mode,
         )
-        job = IQMJob(self, str(uuid), shots=shots)
+        job = IQMJob(self, str(job_id), shots=shots)
         job.circuit_metadata = [c.metadata for c in circuits]
         return job
 
     def retrieve_job(self, job_id: str) -> IQMJob:
         """Create and return an IQMJob instance associated with this backend with given job id."""
         return IQMJob(self, job_id)
```

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm/qiskit_to_iqm.py` & `qiskit-iqm-8.2/src/qiskit_iqm/qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm.egg-info/PKG-INFO` & `qiskit-iqm-8.2/src/qiskit_iqm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 8.1
+Version: 8.2
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-8.1/src/qiskit_iqm.egg-info/SOURCES.txt` & `qiskit-iqm-8.2/src/qiskit_iqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tag-from-pipeline.sh` & `qiskit-iqm-8.2/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tests/conftest.py` & `qiskit-iqm-8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tests/fake_backends/conftest.py` & `qiskit-iqm-8.2/tests/fake_backends/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tests/fake_backends/test_fake_adonis.py` & `qiskit-iqm-8.2/tests/fake_backends/test_fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tests/fake_backends/test_iqm_fake_backend.py` & `qiskit-iqm-8.2/tests/fake_backends/test_iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tests/test_iqm_backend.py` & `qiskit-iqm-8.2/tests/test_iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tests/test_iqm_facade_backend.py` & `qiskit-iqm-8.2/tests/test_iqm_facade_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tests/test_iqm_job.py` & `qiskit-iqm-8.2/tests/test_iqm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tests/test_iqm_provider.py` & `qiskit-iqm-8.2/tests/test_iqm_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """Testing IQM provider.
 """
 from importlib.metadata import version
 from numbers import Number
 import uuid
 
-from iqm_client import IQMClient, RunResult, RunStatus
+from iqm_client import HeraldingMode, IQMClient, RunResult, RunStatus
 from mockito import ANY, mock, patch, when
 import numpy as np
 import pytest
 from qiskit import QuantumCircuit, execute
 from qiskit.circuit import Parameter, ParameterExpression
 from qiskit.circuit.library import RGate
 from qiskit.compiler import transpile
@@ -46,14 +46,30 @@
 @pytest.fixture
 def circuit_2() -> QuantumCircuit:
     circuit = QuantumCircuit(5)
     circuit.cz(0, 1)
     return circuit
 
 
+@pytest.fixture
+def submit_circuits_default_kwargs() -> dict:
+    return {
+        'qubit_mapping': None,
+        'calibration_set_id': None,
+        'shots': 1024,
+        'circuit_duration_check': True,
+        'heralding_mode': HeraldingMode.NONE,
+    }
+
+
+@pytest.fixture
+def job_id():
+    return uuid.uuid4()
+
+
 def test_default_options(backend):
     assert backend.options.shots == 1024
     assert backend.options.calibration_set_id is None
 
 
 def test_retrieve_job(backend):
     job = backend.retrieve_job('a job id')
@@ -221,30 +237,27 @@
 
     patch(backend.run, run_mock)
     execute(
         circuit, backend, shots=10, calibration_set_id='92d8dd9a-2678-467e-a20b-ef9c1a594d1f', something_else=[1, 2, 3]
     )
 
 
-def test_run_single_circuit(backend, circuit):
+def test_run_single_circuit(backend, circuit, submit_circuits_default_kwargs, job_id):
     circuit.measure(0, 0)
     circuit_ser = backend.serialize_circuit(circuit)
-    some_id = uuid.uuid4()
-    shots = 10
-    when(backend.client).submit_circuits(
-        [circuit_ser], qubit_mapping={'0': 'QB1'}, calibration_set_id=None, shots=shots, circuit_duration_check=True
-    ).thenReturn(some_id)
-    job = backend.run(circuit, shots=shots)
+    kwargs = submit_circuits_default_kwargs | {'qubit_mapping': {'0': 'QB1'}}
+    when(backend.client).submit_circuits([circuit_ser], **kwargs).thenReturn(job_id)
+    job = backend.run(circuit)
     assert isinstance(job, IQMJob)
-    assert job.job_id() == str(some_id)
+    assert job.job_id() == str(job_id)
 
     # Should also work if the circuit is passed inside a list
-    job = backend.run([circuit], shots=shots)
+    job = backend.run([circuit])
     assert isinstance(job, IQMJob)
-    assert job.job_id() == str(some_id)
+    assert job.job_id() == str(job_id)
 
 
 def test_run_sets_circuit_metadata_to_the_job(backend):
     circuit_1 = QuantumCircuit(3)
     circuit_1.cz(0, 1)
     circuit_1.metadata = {'key1': 'value1', 'key2': 'value2'}
     circuit_2 = QuantumCircuit(3)
@@ -254,64 +267,66 @@
     backend.client.submit_circuits = lambda *args, **kwargs: some_id
     job = backend.run([circuit_1, circuit_2], shots=10)
     assert isinstance(job, IQMJob)
     assert job.job_id() == str(some_id)
     assert job.circuit_metadata == [circuit_1.metadata, circuit_2.metadata]
 
 
-def test_run_with_custom_calibration_set_id(backend, circuit):
+def test_run_with_custom_calibration_set_id(backend, circuit, submit_circuits_default_kwargs, job_id):
     circuit.measure(0, 0)
     circuit_ser = backend.serialize_circuit(circuit)
-    some_id = uuid.uuid4()
-    shots = 10
     calibration_set_id = '67e77465-d90e-4839-986e-9270f952b743'
-    when(backend.client).submit_circuits(
-        [circuit_ser],
-        qubit_mapping={'0': 'QB1'},
-        calibration_set_id=calibration_set_id,
-        shots=shots,
-        circuit_duration_check=True,
-    ).thenReturn(some_id)
+    kwargs = submit_circuits_default_kwargs | {
+        'calibration_set_id': uuid.UUID(calibration_set_id),
+        'qubit_mapping': {'0': 'QB1'},
+    }
+    when(backend.client).submit_circuits([circuit_ser], **kwargs).thenReturn(job_id)
 
-    backend.run([circuit], calibration_set_id=calibration_set_id, shots=shots)
+    backend.run([circuit], calibration_set_id=calibration_set_id)
 
 
-def test_run_with_duration_check_disabled(backend, circuit):
+def test_run_with_duration_check_disabled(backend, circuit, submit_circuits_default_kwargs, job_id):
     circuit.measure(0, 0)
     circuit_ser = backend.serialize_circuit(circuit)
-    some_id = uuid.uuid4()
-    shots = 10
-    when(backend.client).submit_circuits(
-        [circuit_ser], qubit_mapping={'0': 'QB1'}, calibration_set_id=None, shots=shots, circuit_duration_check=False
-    ).thenReturn(some_id)
+    kwargs = submit_circuits_default_kwargs | {'qubit_mapping': {'0': 'QB1'}, 'circuit_duration_check': False}
+    when(backend.client).submit_circuits([circuit_ser], **kwargs).thenReturn(job_id)
+
+    backend.run([circuit], circuit_duration_check=False)
+
 
-    backend.run([circuit], shots=shots, circuit_duration_check=False)
+def test_run_uses_heralding_mode_none_by_default(backend, circuit, submit_circuits_default_kwargs, job_id):
+    circuit.measure(0, 0)
+    circuit_ser = backend.serialize_circuit(circuit)
+    kwargs = submit_circuits_default_kwargs | {'heralding_mode': HeraldingMode.NONE, 'qubit_mapping': {'0': 'QB1'}}
+    when(backend.client).submit_circuits([circuit_ser], **kwargs).thenReturn(job_id)
+    backend.run([circuit])
 
 
-def test_run_batch_of_circuits(backend, circuit):
+def test_run_with_heralding_mode_zeros(backend, circuit, submit_circuits_default_kwargs, job_id):
+    circuit.measure(0, 0)
+    circuit_ser = backend.serialize_circuit(circuit)
+    kwargs = submit_circuits_default_kwargs | {'heralding_mode': HeraldingMode.ZEROS, 'qubit_mapping': {'0': 'QB1'}}
+    when(backend.client).submit_circuits([circuit_ser], **kwargs).thenReturn(job_id)
+    backend.run([circuit], heralding_mode='zeros')
+
+
+def test_run_batch_of_circuits(backend, circuit, submit_circuits_default_kwargs, job_id):
     theta = Parameter('theta')
     theta_range = np.linspace(0, 2 * np.pi, 3)
-    shots = 10
-    some_id = uuid.uuid4()
     circuit.cz(0, 1)
     circuit.r(theta, 0, 0)
     circuit.cz(0, 1)
     circuits = [circuit.bind_parameters({theta: t}) for t in theta_range]
     circuits_serialized = [backend.serialize_circuit(circuit) for circuit in circuits]
-    when(backend.client).submit_circuits(
-        circuits_serialized,
-        qubit_mapping={'0': 'QB1', '1': 'QB2'},
-        calibration_set_id=None,
-        shots=shots,
-        circuit_duration_check=True,
-    ).thenReturn(some_id)
+    kwargs = submit_circuits_default_kwargs | {'qubit_mapping': {'0': 'QB1', '1': 'QB2'}}
+    when(backend.client).submit_circuits(circuits_serialized, **kwargs).thenReturn(job_id)
 
-    job = backend.run(circuits, shots=shots)
+    job = backend.run(circuits)
     assert isinstance(job, IQMJob)
-    assert job.job_id() == str(some_id)
+    assert job.job_id() == str(job_id)
 
 
 def test_error_on_empty_circuit_list(backend):
     with pytest.raises(ValueError, match='Empty list of circuits submitted for execution.'):
         backend.run([], shots=42)
 
 
@@ -382,18 +397,16 @@
                 ],
             }
         },
     }
     result_status = {'status': 'failed'}
 
     when(IQMClient).get_quantum_architecture().thenReturn(adonis_architecture)
-    when(IQMClient).submit_circuits(
-        ANY, qubit_mapping=ANY, calibration_set_id=ANY, shots=ANY, circuit_duration_check=ANY
-    ).thenReturn(uuid.uuid4())
-    when(IQMClient).get_run(ANY).thenReturn(RunResult.from_dict(result))
-    when(IQMClient).get_run_status(ANY).thenReturn(RunStatus.from_dict(result_status))
+    when(IQMClient).submit_circuits(...).thenReturn(uuid.uuid4())
+    when(IQMClient).get_run(ANY(uuid.UUID)).thenReturn(RunResult.from_dict(result))
+    when(IQMClient).get_run_status(ANY(uuid.UUID)).thenReturn(RunStatus.from_dict(result_status))
 
     provider = IQMProvider(url)
     backend = provider.get_backend('facade_adonis')
 
-    with pytest.raises(RuntimeError):
+    with pytest.raises(RuntimeError, match='Remote execution did not succeed'):
         backend.run(circuit_2)
```

### Comparing `qiskit-iqm-8.1/tests/test_qiskit_to_iqm.py` & `qiskit-iqm-8.2/tests/test_qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.1/tox.ini` & `qiskit-iqm-8.2/tox.ini`

 * *Files identical despite different names*

