# Comparing `tmp/rlstack-0.1.0.tar.gz` & `tmp/rlstack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlstack-0.1.0.tar", last modified: Wed May 31 21:48:08 2023, max compression
+gzip compressed data, was "rlstack-0.1.1.tar", last modified: Thu Jun  1 22:13:19 2023, max compression
```

## Comparing `rlstack-0.1.0.tar` & `rlstack-0.1.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.500000 rlstack-0.1.0/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.480000 rlstack-0.1.0/.github/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/.github/workflows/
--rw-r--r--   0 berger    (1000) berger    (1000)      916 2023-04-26 21:08:56.000000 rlstack-0.1.0/.github/workflows/build-docs.yml
--rw-r--r--   0 berger    (1000) berger    (1000)      745 2023-04-26 21:09:13.000000 rlstack-0.1.0/.github/workflows/test-and-publish.yml
--rw-r--r--   0 berger    (1000) berger    (1000)      551 2023-04-26 21:10:03.000000 rlstack-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 berger    (1000) berger    (1000)     1887 2023-04-28 20:49:45.000000 rlstack-0.1.0/.gitignore
--rw-r--r--   0 berger    (1000) berger    (1000)      694 2023-05-03 00:17:18.000000 rlstack-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 berger    (1000) berger    (1000)    11357 2023-02-10 22:26:37.000000 rlstack-0.1.0/LICENSE
--rw-r--r--   0 berger    (1000) berger    (1000)    25248 2023-05-31 21:48:08.500000 rlstack-0.1.0/PKG-INFO
--rw-r--r--   0 berger    (1000) berger    (1000)    11488 2023-05-31 21:17:24.000000 rlstack-0.1.0/README.rst
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/docs/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/.nojekyll
--rw-r--r--   0 berger    (1000) berger    (1000)      635 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/Makefile
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/docs/_static/
--rw-r--r--   0 berger    (1000) berger    (1000)      480 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/_static/custom.css
--rw-r--r--   0 berger    (1000) berger    (1000)     4234 2023-05-04 01:02:37.000000 rlstack-0.1.0/docs/conf.py
--rw-r--r--   0 berger    (1000) berger    (1000)       71 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/index.html
--rw-r--r--   0 berger    (1000) berger    (1000)      188 2023-05-04 20:56:47.000000 rlstack-0.1.0/docs/index.rst
--rw-r--r--   0 berger    (1000) berger    (1000)      799 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/make.bat
--rw-r--r--   0 berger    (1000) berger    (1000)       75 2023-04-30 23:31:03.000000 rlstack-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.480000 rlstack-0.1.0/examples/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/examples/algotrading/
--rw-r--r--   0 berger    (1000) berger    (1000)     2134 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/README.rst
--rw-r--r--   0 berger    (1000) berger    (1000)     1705 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/__main__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     7276 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/env.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/examples/algotrading/models/
--rw-r--r--   0 berger    (1000) berger    (1000)      102 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/models/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     3955 2023-05-31 21:42:40.000000 rlstack-0.1.0/examples/algotrading/models/lstm.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4874 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/models/mlp.py
--rw-r--r--   0 berger    (1000) berger    (1000)     5613 2023-05-31 21:35:47.000000 rlstack-0.1.0/examples/algotrading/models/transformer.py
--rw-r--r--   0 berger    (1000) berger    (1000)     3776 2023-05-31 21:17:24.000000 rlstack-0.1.0/pyproject.toml
--rw-r--r--   0 berger    (1000) berger    (1000)       38 2023-05-31 21:48:08.500000 rlstack-0.1.0/setup.cfg
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.480000 rlstack-0.1.0/src/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/
--rw-r--r--   0 berger    (1000) berger    (1000)      644 2023-05-15 21:11:00.000000 rlstack-0.1.0/src/rlstack/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4685 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/_utils.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/algorithms/
--rw-r--r--   0 berger    (1000) berger    (1000)      834 2023-05-15 21:16:46.000000 rlstack-0.1.0/src/rlstack/algorithms/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)    27138 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/algorithms/_feedforward.py
--rw-r--r--   0 berger    (1000) berger    (1000)    29353 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/algorithms/_recurrent.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4415 2023-05-21 00:35:52.000000 rlstack-0.1.0/src/rlstack/conditions.py
--rw-r--r--   0 berger    (1000) berger    (1000)    13633 2023-05-19 02:41:20.000000 rlstack-0.1.0/src/rlstack/data.py
--rw-r--r--   0 berger    (1000) berger    (1000)     6021 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/distributions.py
--rw-r--r--   0 berger    (1000) berger    (1000)     6629 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/env.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/models/
--rw-r--r--   0 berger    (1000) berger    (1000)     1126 2023-05-15 21:11:00.000000 rlstack-0.1.0/src/rlstack/models/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)    14331 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/models/_feedforward.py
--rw-r--r--   0 berger    (1000) berger    (1000)    13255 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/models/_recurrent.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/nn/
--rw-r--r--   0 berger    (1000) berger    (1000)      568 2023-05-17 21:40:38.000000 rlstack-0.1.0/src/rlstack/nn/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)    13184 2023-05-22 21:34:03.000000 rlstack-0.1.0/src/rlstack/nn/functional.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/nn/modules/
--rw-r--r--   0 berger    (1000) berger    (1000)      348 2023-02-08 23:39:43.000000 rlstack-0.1.0/src/rlstack/nn/modules/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1061 2023-05-02 01:12:30.000000 rlstack-0.1.0/src/rlstack/nn/modules/activations.py
--rw-r--r--   0 berger    (1000) berger    (1000)    12068 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/nn/modules/attention.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1740 2023-05-02 00:38:37.000000 rlstack-0.1.0/src/rlstack/nn/modules/embeddings.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1749 2023-02-09 01:31:09.000000 rlstack-0.1.0/src/rlstack/nn/modules/mlp.py
--rw-r--r--   0 berger    (1000) berger    (1000)      586 2023-05-04 01:01:58.000000 rlstack-0.1.0/src/rlstack/nn/modules/module.py
--rw-r--r--   0 berger    (1000) berger    (1000)     8138 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/nn/modules/perceiver.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4601 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/nn/modules/skip.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2791 2023-05-21 20:55:43.000000 rlstack-0.1.0/src/rlstack/optimizer.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/policies/
--rw-r--r--   0 berger    (1000) berger    (1000)      509 2023-05-15 21:17:42.000000 rlstack-0.1.0/src/rlstack/policies/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     8036 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/policies/_feedforward.py
--rw-r--r--   0 berger    (1000) berger    (1000)     8237 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/policies/_recurrent.py
--rw-r--r--   0 berger    (1000) berger    (1000)     7532 2023-05-21 15:13:57.000000 rlstack-0.1.0/src/rlstack/schedulers.py
--rw-r--r--   0 berger    (1000) berger    (1000)    72012 2023-05-03 00:17:58.000000 rlstack-0.1.0/src/rlstack/specs.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4120 2023-05-22 22:09:36.000000 rlstack-0.1.0/src/rlstack/trainer.py
--rw-r--r--   0 berger    (1000) berger    (1000)    18782 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/views.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack.egg-info/
--rw-r--r--   0 berger    (1000) berger    (1000)    25248 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/PKG-INFO
--rw-r--r--   0 berger    (1000) berger    (1000)     1819 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/SOURCES.txt
--rw-r--r--   0 berger    (1000) berger    (1000)        1 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/dependency_links.txt
--rw-r--r--   0 berger    (1000) berger    (1000)      159 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/requires.txt
--rw-r--r--   0 berger    (1000) berger    (1000)        8 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/top_level.txt
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/tests/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-02-10 22:22:48.000000 rlstack-0.1.0/tests/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1751 2023-05-21 20:54:04.000000 rlstack-0.1.0/tests/test_algorithms.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1033 2023-05-21 00:35:52.000000 rlstack-0.1.0/tests/test_conditions.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/tests/test_nn/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-05-21 00:35:52.000000 rlstack-0.1.0/tests/test_nn/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2536 2023-05-21 14:55:57.000000 rlstack-0.1.0/tests/test_nn/test_functional.py
--rw-r--r--   0 berger    (1000) berger    (1000)     3124 2023-05-21 00:35:52.000000 rlstack-0.1.0/tests/test_policies.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1402 2023-05-21 00:35:52.000000 rlstack-0.1.0/tests/test_schedulers.py
--rw-r--r--   0 berger    (1000) berger    (1000)    12184 2023-05-31 21:17:24.000000 rlstack-0.1.0/tests/test_views.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.660000 rlstack-0.1.1/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/.github/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/.github/workflows/
+-rw-r--r--   0 berger    (1000) berger    (1000)      916 2023-04-26 21:08:56.000000 rlstack-0.1.1/.github/workflows/build-docs.yml
+-rw-r--r--   0 berger    (1000) berger    (1000)      738 2023-06-01 22:10:56.000000 rlstack-0.1.1/.github/workflows/test-and-publish.yml
+-rw-r--r--   0 berger    (1000) berger    (1000)      568 2023-06-01 21:51:37.000000 rlstack-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0 berger    (1000) berger    (1000)     1887 2023-04-28 20:49:45.000000 rlstack-0.1.1/.gitignore
+-rw-r--r--   0 berger    (1000) berger    (1000)      694 2023-05-03 00:17:18.000000 rlstack-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 berger    (1000) berger    (1000)    11357 2023-02-10 22:26:37.000000 rlstack-0.1.1/LICENSE
+-rw-r--r--   0 berger    (1000) berger    (1000)    25248 2023-06-01 22:13:19.660000 rlstack-0.1.1/PKG-INFO
+-rw-r--r--   0 berger    (1000) berger    (1000)    11488 2023-05-31 21:17:24.000000 rlstack-0.1.1/README.rst
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/docs/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-04-26 22:09:05.000000 rlstack-0.1.1/docs/.nojekyll
+-rw-r--r--   0 berger    (1000) berger    (1000)      635 2023-04-26 22:09:05.000000 rlstack-0.1.1/docs/Makefile
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/docs/_static/
+-rw-r--r--   0 berger    (1000) berger    (1000)      480 2023-04-26 22:09:05.000000 rlstack-0.1.1/docs/_static/custom.css
+-rw-r--r--   0 berger    (1000) berger    (1000)     4234 2023-05-04 01:02:37.000000 rlstack-0.1.1/docs/conf.py
+-rw-r--r--   0 berger    (1000) berger    (1000)       71 2023-04-26 22:09:05.000000 rlstack-0.1.1/docs/index.html
+-rw-r--r--   0 berger    (1000) berger    (1000)      188 2023-05-04 20:56:47.000000 rlstack-0.1.1/docs/index.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)      799 2023-04-26 22:09:05.000000 rlstack-0.1.1/docs/make.bat
+-rw-r--r--   0 berger    (1000) berger    (1000)       75 2023-04-30 23:31:03.000000 rlstack-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/examples/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/examples/algotrading/
+-rw-r--r--   0 berger    (1000) berger    (1000)     2134 2023-05-31 21:17:24.000000 rlstack-0.1.1/examples/algotrading/README.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)     1705 2023-06-01 02:06:40.000000 rlstack-0.1.1/examples/algotrading/__main__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     7276 2023-05-31 21:17:24.000000 rlstack-0.1.1/examples/algotrading/env.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/examples/algotrading/models/
+-rw-r--r--   0 berger    (1000) berger    (1000)      102 2023-05-31 21:17:24.000000 rlstack-0.1.1/examples/algotrading/models/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3955 2023-05-31 21:42:40.000000 rlstack-0.1.1/examples/algotrading/models/lstm.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4874 2023-05-31 21:17:24.000000 rlstack-0.1.1/examples/algotrading/models/mlp.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     5613 2023-05-31 21:35:47.000000 rlstack-0.1.1/examples/algotrading/models/transformer.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3776 2023-05-31 21:17:24.000000 rlstack-0.1.1/pyproject.toml
+-rw-r--r--   0 berger    (1000) berger    (1000)       38 2023-06-01 22:13:19.660000 rlstack-0.1.1/setup.cfg
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/src/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/src/rlstack/
+-rw-r--r--   0 berger    (1000) berger    (1000)      644 2023-05-15 21:11:00.000000 rlstack-0.1.1/src/rlstack/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4685 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/_utils.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/src/rlstack/algorithms/
+-rw-r--r--   0 berger    (1000) berger    (1000)      834 2023-05-15 21:16:46.000000 rlstack-0.1.1/src/rlstack/algorithms/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    27138 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/algorithms/_feedforward.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    29353 2023-06-01 02:10:44.000000 rlstack-0.1.1/src/rlstack/algorithms/_recurrent.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4415 2023-05-21 00:35:52.000000 rlstack-0.1.1/src/rlstack/conditions.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    14089 2023-06-01 02:13:44.000000 rlstack-0.1.1/src/rlstack/data.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     6021 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/distributions.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     6629 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/env.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.660000 rlstack-0.1.1/src/rlstack/models/
+-rw-r--r--   0 berger    (1000) berger    (1000)     1126 2023-05-15 21:11:00.000000 rlstack-0.1.1/src/rlstack/models/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    14331 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/models/_feedforward.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    13255 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/models/_recurrent.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.660000 rlstack-0.1.1/src/rlstack/nn/
+-rw-r--r--   0 berger    (1000) berger    (1000)      568 2023-05-17 21:40:38.000000 rlstack-0.1.1/src/rlstack/nn/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    13184 2023-05-22 21:34:03.000000 rlstack-0.1.1/src/rlstack/nn/functional.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.660000 rlstack-0.1.1/src/rlstack/nn/modules/
+-rw-r--r--   0 berger    (1000) berger    (1000)      348 2023-02-08 23:39:43.000000 rlstack-0.1.1/src/rlstack/nn/modules/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1061 2023-05-02 01:12:30.000000 rlstack-0.1.1/src/rlstack/nn/modules/activations.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    12068 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/nn/modules/attention.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1740 2023-05-02 00:38:37.000000 rlstack-0.1.1/src/rlstack/nn/modules/embeddings.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1749 2023-02-09 01:31:09.000000 rlstack-0.1.1/src/rlstack/nn/modules/mlp.py
+-rw-r--r--   0 berger    (1000) berger    (1000)      586 2023-05-04 01:01:58.000000 rlstack-0.1.1/src/rlstack/nn/modules/module.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     8138 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/nn/modules/perceiver.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4601 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/nn/modules/skip.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2791 2023-05-21 20:55:43.000000 rlstack-0.1.1/src/rlstack/optimizer.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.660000 rlstack-0.1.1/src/rlstack/policies/
+-rw-r--r--   0 berger    (1000) berger    (1000)      509 2023-05-15 21:17:42.000000 rlstack-0.1.1/src/rlstack/policies/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     8036 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/policies/_feedforward.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     8237 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/policies/_recurrent.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     7532 2023-05-21 15:13:57.000000 rlstack-0.1.1/src/rlstack/schedulers.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    72012 2023-05-03 00:17:58.000000 rlstack-0.1.1/src/rlstack/specs.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4120 2023-05-22 22:09:36.000000 rlstack-0.1.1/src/rlstack/trainer.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    18782 2023-05-31 21:17:24.000000 rlstack-0.1.1/src/rlstack/views.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.650000 rlstack-0.1.1/src/rlstack.egg-info/
+-rw-r--r--   0 berger    (1000) berger    (1000)    25248 2023-06-01 22:13:19.000000 rlstack-0.1.1/src/rlstack.egg-info/PKG-INFO
+-rw-r--r--   0 berger    (1000) berger    (1000)     1819 2023-06-01 22:13:19.000000 rlstack-0.1.1/src/rlstack.egg-info/SOURCES.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)        1 2023-06-01 22:13:19.000000 rlstack-0.1.1/src/rlstack.egg-info/dependency_links.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)      159 2023-06-01 22:13:19.000000 rlstack-0.1.1/src/rlstack.egg-info/requires.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)        8 2023-06-01 22:13:19.000000 rlstack-0.1.1/src/rlstack.egg-info/top_level.txt
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.660000 rlstack-0.1.1/tests/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-02-10 22:22:48.000000 rlstack-0.1.1/tests/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3090 2023-06-01 02:30:50.000000 rlstack-0.1.1/tests/test_algorithms.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1033 2023-05-21 00:35:52.000000 rlstack-0.1.1/tests/test_conditions.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-06-01 22:13:19.660000 rlstack-0.1.1/tests/test_nn/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-05-21 00:35:52.000000 rlstack-0.1.1/tests/test_nn/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2536 2023-05-21 14:55:57.000000 rlstack-0.1.1/tests/test_nn/test_functional.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3124 2023-05-21 00:35:52.000000 rlstack-0.1.1/tests/test_policies.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1402 2023-05-21 00:35:52.000000 rlstack-0.1.1/tests/test_schedulers.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    12184 2023-05-31 21:17:24.000000 rlstack-0.1.1/tests/test_views.py
```

### Comparing `rlstack-0.1.0/.github/workflows/build-docs.yml` & `rlstack-0.1.1/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/.github/workflows/test-and-publish.yml` & `rlstack-0.1.1/.github/workflows/test-and-publish.yml`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     secrets: inherit
 
   publish:
     needs: test
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10", "3.11"]
+        python-version: ["3.10"]
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install tox
@@ -27,8 +27,8 @@
       - name: Build
         run: tox -e build
       - name: Publish
         run: tox -e publish
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
-          TWIN_REPOSITORY: pypi
+          TWINE_REPOSITORY: pypi
```

### Comparing `rlstack-0.1.0/.github/workflows/test.yml` & `rlstack-0.1.1/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 name: Test
 
 on:
   push:
     branches:
       - main
+  workflow_call:
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.10"]
```

### Comparing `rlstack-0.1.0/.gitignore` & `rlstack-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/.pre-commit-config.yaml` & `rlstack-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/LICENSE` & `rlstack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/PKG-INFO` & `rlstack-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlstack
-Version: 0.1.0
+Version: 0.1.1
 Summary: A minimal RL library for infinite horizon tasks.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rlstack-0.1.0/README.rst` & `rlstack-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/docs/Makefile` & `rlstack-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/docs/conf.py` & `rlstack-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/docs/make.bat` & `rlstack-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/examples/algotrading/README.rst` & `rlstack-0.1.1/examples/algotrading/README.rst`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/examples/algotrading/__main__.py` & `rlstack-0.1.1/examples/algotrading/__main__.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/examples/algotrading/env.py` & `rlstack-0.1.1/examples/algotrading/env.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/examples/algotrading/models/lstm.py` & `rlstack-0.1.1/examples/algotrading/models/lstm.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/examples/algotrading/models/mlp.py` & `rlstack-0.1.1/examples/algotrading/models/mlp.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/examples/algotrading/models/transformer.py` & `rlstack-0.1.1/examples/algotrading/models/transformer.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/pyproject.toml` & `rlstack-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/__init__.py` & `rlstack-0.1.1/src/rlstack/__init__.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/_utils.py` & `rlstack-0.1.1/src/rlstack/_utils.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/algorithms/__init__.py` & `rlstack-0.1.1/src/rlstack/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/algorithms/_feedforward.py` & `rlstack-0.1.1/src/rlstack/algorithms/_feedforward.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/algorithms/_recurrent.py` & `rlstack-0.1.1/src/rlstack/algorithms/_recurrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
                 ]
                 self.buffer[DataKeys.LOGP][:, t, ...] = sample_batch[DataKeys.LOGP]
                 self.buffer[DataKeys.VALUES][:, t, ...] = sample_batch[DataKeys.VALUES]
                 self.buffer[DataKeys.REWARDS][:, t, ...] = out_batch[DataKeys.REWARDS]
                 self.buffer[DataKeys.OBS][:, t + 1, ...] = out_batch[DataKeys.OBS]
                 self.buffer[DataKeys.STATES][:, t + 1, ...] = sample_states
 
-                if t and not (t % self.hparams.seq_len):
+                if not ((t + 1) % self.hparams.seq_len):
                     self.state.seqs += 1
 
             # Sample features and value function at last observation.
             in_batch = self.buffer[:, -1:, ...]
             in_states = self.buffer[DataKeys.STATES][:, -1:, ...]
             sample_batch, _ = self.policy.sample(
                 in_batch,
```

### Comparing `rlstack-0.1.0/src/rlstack/conditions.py` & `rlstack-0.1.1/src/rlstack/conditions.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/data.py` & `rlstack-0.1.1/src/rlstack/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,24 @@
         super().__post_init__()
         if not (self.seq_len > 0):
             raise ValueError("`seq_len` must be > 0.")
 
         if self.horizon % self.seq_len:
             raise ValueError("`seq_len` must be a factor of `horizon`.")
 
+        if (self.horizon * self.horizons_per_env_reset) % (
+            self.seq_len * self.seqs_per_state_reset
+        ):
+            raise ValueError(
+                "`seq_len * seqs_per_state_reset` must be a factor of `horizon *"
+                " horizons_per_env_reset`. As an example, if `horizon=8`,"
+                " `horizons_per_env_reset=1`, and `seq_len=2`, then"
+                " `seqs_per_state_reset` can be 1, 2, or 4."
+            )
+
         if self.seqs_per_state_reset == 0:
             raise ValueError("`seqs_per_state_reset` must be nonzero.")
 
     @property
     def num_minibatches(self) -> int:
         """Return the number of minibatches for convenience."""
         return (
```

### Comparing `rlstack-0.1.0/src/rlstack/distributions.py` & `rlstack-0.1.1/src/rlstack/distributions.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/env.py` & `rlstack-0.1.1/src/rlstack/env.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/models/__init__.py` & `rlstack-0.1.1/src/rlstack/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/models/_feedforward.py` & `rlstack-0.1.1/src/rlstack/models/_feedforward.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/models/_recurrent.py` & `rlstack-0.1.1/src/rlstack/models/_recurrent.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/nn/__init__.py` & `rlstack-0.1.1/src/rlstack/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/nn/functional.py` & `rlstack-0.1.1/src/rlstack/nn/functional.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/nn/modules/activations.py` & `rlstack-0.1.1/src/rlstack/nn/modules/activations.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/nn/modules/attention.py` & `rlstack-0.1.1/src/rlstack/nn/modules/attention.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/nn/modules/embeddings.py` & `rlstack-0.1.1/src/rlstack/nn/modules/embeddings.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/nn/modules/mlp.py` & `rlstack-0.1.1/src/rlstack/nn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/nn/modules/module.py` & `rlstack-0.1.1/src/rlstack/nn/modules/module.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/nn/modules/perceiver.py` & `rlstack-0.1.1/src/rlstack/nn/modules/perceiver.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/nn/modules/skip.py` & `rlstack-0.1.1/src/rlstack/nn/modules/skip.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/optimizer.py` & `rlstack-0.1.1/src/rlstack/optimizer.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/policies/_feedforward.py` & `rlstack-0.1.1/src/rlstack/policies/_feedforward.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/policies/_recurrent.py` & `rlstack-0.1.1/src/rlstack/policies/_recurrent.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/schedulers.py` & `rlstack-0.1.1/src/rlstack/schedulers.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/specs.py` & `rlstack-0.1.1/src/rlstack/specs.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/trainer.py` & `rlstack-0.1.1/src/rlstack/trainer.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack/views.py` & `rlstack-0.1.1/src/rlstack/views.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/src/rlstack.egg-info/PKG-INFO` & `rlstack-0.1.1/src/rlstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlstack
-Version: 0.1.0
+Version: 0.1.1
 Summary: A minimal RL library for infinite horizon tasks.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rlstack-0.1.0/src/rlstack.egg-info/SOURCES.txt` & `rlstack-0.1.1/src/rlstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/tests/test_conditions.py` & `rlstack-0.1.1/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/tests/test_nn/test_functional.py` & `rlstack-0.1.1/tests/test_nn/test_functional.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/tests/test_policies.py` & `rlstack-0.1.1/tests/test_policies.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/tests/test_schedulers.py` & `rlstack-0.1.1/tests/test_schedulers.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.1.0/tests/test_views.py` & `rlstack-0.1.1/tests/test_views.py`

 * *Files identical despite different names*

