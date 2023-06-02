# Comparing `tmp/python-arango-7.5.7.tar.gz` & `tmp/python-arango-7.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-arango-7.5.7.tar", last modified: Tue Feb 21 10:23:42 2023, max compression
+gzip compressed data, was "python-arango-7.5.8.tar", last modified: Fri Jun  2 15:44:35 2023, max compression
```

## Comparing `python-arango-7.5.7.tar` & `python-arango-7.5.8.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:23:42.359583 python-arango-7.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:23:42.339583 python-arango-7.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:23:42.343583 python-arango-7.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-21 10:23:31.000000 python-arango-7.5.7/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-21 10:23:31.000000 python-arango-7.5.7/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-21 10:23:31.000000 python-arango-7.5.7/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-02-21 10:23:31.000000 python-arango-7.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-21 10:23:31.000000 python-arango-7.5.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-21 10:23:31.000000 python-arango-7.5.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-21 10:23:31.000000 python-arango-7.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-21 10:23:31.000000 python-arango-7.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-02-21 10:23:42.359583 python-arango-7.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-02-21 10:23:31.000000 python-arango-7.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:23:42.351583 python-arango-7.5.7/arango/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26767 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/aql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   122525 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)    99686 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    34373 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/errno.py
--rw-r--r--   0 runner    (1001) docker     (123)    22468 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    38482 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/foxx.py
--rw-r--r--   0 runner    (1001) docker     (123)    35862 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/pregel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33852 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-21 10:23:42.000000 python-arango-7.5.7/arango/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-02-21 10:23:31.000000 python-arango-7.5.7/arango/wal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:23:42.359583 python-arango-7.5.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/admin.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/analyzer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/aql.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/async.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/backup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/batch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/certificates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/cluster.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/collection.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/cursor.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/document.rst
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/errno.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/foxx.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/graph.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/http.rst
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/indexes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/pregel.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/replication.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/serializer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/simple.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/specs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:23:42.359583 python-arango-7.5.7/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/task.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/threading.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/transaction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/user.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/view.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-02-21 10:23:31.000000 python-arango-7.5.7/docs/wal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-21 10:23:31.000000 python-arango-7.5.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:23:42.359583 python-arango-7.5.7/python_arango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-02-21 10:23:42.000000 python-arango-7.5.7/python_arango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-21 10:23:42.000000 python-arango-7.5.7/python_arango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 10:23:42.000000 python-arango-7.5.7/python_arango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-21 10:23:42.000000 python-arango-7.5.7/python_arango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-21 10:23:42.000000 python-arango-7.5.7/python_arango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-21 10:23:42.359583 python-arango-7.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-02-21 10:23:31.000000 python-arango-7.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.190516 python-arango-7.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.182516 python-arango-7.5.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.182516 python-arango-7.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-02 15:44:21.000000 python-arango-7.5.8/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-02 15:44:21.000000 python-arango-7.5.8/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-02 15:44:21.000000 python-arango-7.5.8/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-02 15:44:21.000000 python-arango-7.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-02 15:44:21.000000 python-arango-7.5.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-02 15:44:21.000000 python-arango-7.5.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 15:44:21.000000 python-arango-7.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 15:44:21.000000 python-arango-7.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-02 15:44:35.190516 python-arango-7.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-02 15:44:21.000000 python-arango-7.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.186516 python-arango-7.5.8/arango/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26767 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/aql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122524 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99686 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34373 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/errno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22468 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39554 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/foxx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35862 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/pregel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33852 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 15:44:34.000000 python-arango-7.5.8/arango/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/wal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.186516 python-arango-7.5.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/analyzer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/aql.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/async.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/backup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/batch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/certificates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/collection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/cursor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/document.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/errno.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/foxx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/http.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/indexes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/pregel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/replication.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/serializer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/simple.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/specs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.190516 python-arango-7.5.8/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/task.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/threading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/view.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/wal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-02 15:44:21.000000 python-arango-7.5.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.190516 python-arango-7.5.8/python_arango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-02 15:44:35.190516 python-arango-7.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-02 15:44:21.000000 python-arango-7.5.8/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4068 2023-06-02 15:44:21.000000 python-arango-7.5.8/tester.sh
```

### Comparing `python-arango-7.5.7/.github/workflows/build.yaml` & `python-arango-7.5.8/.github/workflows/build.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -9,37 +9,31 @@
         type: boolean
         description: Debug with tmate
         required: false
         default: false
 
 jobs:
   build:
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-22.04
 
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11.1"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
 
       - name: Fetch all tags and branches
         run: git fetch --prune --unshallow
 
       - name: Create ArangoDB Docker container
         run: >
-          docker create --name arango -p 8529:8529 -e ARANGO_ROOT_PASSWORD=passwd
-          arangodb/arangodb:3.7.7 --server.jwt-secret-keyfile=/tmp/keyfile
-
-      - name: Copy Foxx service zip into ArangoDB Docker container
-        run: docker cp tests/static/service.zip arango:/tmp/service.zip
-
-      - name: Copy keyfile into ArangoDB Docker container
-        run: docker cp tests/static/keyfile arango:/tmp/keyfile
+          docker create --name arango -p 8529:8529 -e ARANGO_ROOT_PASSWORD=passwd -v "$(pwd)/tests/static/":/tests/static
+          arangodb/arangodb:3.10.6 --server.jwt-secret-keyfile=/tests/static/keyfile
 
       - name: Start ArangoDB Docker container
         run: docker start arango
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
```

### Comparing `python-arango-7.5.7/.github/workflows/pypi.yaml` & `python-arango-7.5.8/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/.gitignore` & `python-arango-7.5.8/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -117,7 +117,10 @@
 
 # direnv
 .envrc
 .direnv/
 
 # setuptools_scm
 arango/version.py
+
+# test results
+*_results.txt
```

### Comparing `python-arango-7.5.7/.pre-commit-config.yaml` & `python-arango-7.5.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/CONTRIBUTING.md` & `python-arango-7.5.8/CONTRIBUTING.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 Run unit tests with coverage:
 
 ```shell
 py.test --cov=arango --cov-report=html  # Open htmlcov/index.html in your browser
 ```
 
+For a more comprehensive test suite, run:
+
+```shell
+./tester.sh  # Requires docker
+```
+
 Build and test documentation:
 
 ```shell
 python -m sphinx docs docs/_build  # Open docs/_build/index.html in your browser
 ```
 
 Thank you for your contribution!
```

### Comparing `python-arango-7.5.7/LICENSE` & `python-arango-7.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/PKG-INFO` & `python-arango-7.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-arango
-Version: 7.5.7
+Version: 7.5.8
 Summary: Python Driver for ArangoDB
 Home-page: https://github.com/ArangoDB-Community/python-arango
 Author: Joohwan Oh
 Author-email: joohwan.oh@outlook.com
 License: MIT
 Keywords: arangodb,python,driver
 Classifier: Intended Audience :: Developers
```

### Comparing `python-arango-7.5.7/README.md` & `python-arango-7.5.8/README.md`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/api.py` & `python-arango-7.5.8/arango/api.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/aql.py` & `python-arango-7.5.8/arango/aql.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/backup.py` & `python-arango-7.5.8/arango/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         :return: Backup details.
         :rtype: dict
         :raise arango.exceptions.BackupGetError: If delete fails.
         """
         request = Request(
             method="post",
             endpoint="/_admin/backup/list",
-            data={} if backup_id is None else {"id": backup_id},
+            data=None if backup_id is None else {"id": backup_id},
         )
 
         def response_handler(resp: Response) -> Json:
             if resp.is_success:
                 return format_backups(resp.body["result"])
             raise BackupGetError(resp, request)
```

### Comparing `python-arango-7.5.7/arango/client.py` & `python-arango-7.5.8/arango/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __all__ = ["ArangoClient"]
 
 from json import dumps, loads
 from typing import Any, Callable, Optional, Sequence, Union
 
-from pkg_resources import get_distribution
+import importlib_metadata
 
 from arango.connection import (
     BasicConnection,
     Connection,
     JwtConnection,
     JwtSuperuserConnection,
 )
@@ -123,15 +123,15 @@
     @property
     def version(self) -> str:
         """Return the client version.
 
         :return: Client version.
         :rtype: str
         """
-        version: str = get_distribution("python-arango").version
+        version: str = importlib_metadata.version("python-arango")
         return version
 
     @property
     def request_timeout(self) -> Any:
         """Return the request timeout of the http client.
 
         :return: Request timeout.
```

### Comparing `python-arango-7.5.7/arango/cluster.py` & `python-arango-7.5.8/arango/cluster.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/collection.py` & `python-arango-7.5.8/arango/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -859,15 +859,15 @@
         longitude1: Number,
         latitude2: Number,
         longitude2: Number,
         skip: Optional[int] = None,
         limit: Optional[int] = None,
         index: Optional[str] = None,
     ) -> Result[Cursor]:
-        """Return all documents in an rectangular area.
+        """Return all documents in a rectangular area.
 
         :param latitude1: First latitude.
         :type latitude1: int | float
         :param longitude1: First longitude.
         :type longitude1: int | float
         :param latitude2: Second latitude.
         :type latitude2: int | float
```

### Comparing `python-arango-7.5.7/arango/connection.py` & `python-arango-7.5.8/arango/connection.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/cursor.py` & `python-arango-7.5.8/arango/cursor.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/database.py` & `python-arango-7.5.8/arango/database.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/errno.py` & `python-arango-7.5.8/arango/errno.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/exceptions.py` & `python-arango-7.5.8/arango/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/executor.py` & `python-arango-7.5.8/arango/executor.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/formatter.py` & `python-arango-7.5.8/arango/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
         result["max_num_cover_cells"] = body["maxNumCoverCells"]
     if "storedValues" in body:
         result["storedValues"] = body["storedValues"]
     if "cacheEnabled" in body:
         result["cacheEnabled"] = body["cacheEnabled"]
     if "legacyPolygons" in body:
         result["legacyPolygons"] = body["legacyPolygons"]
+    if "estimates" in body:
+        result["estimates"] = body["estimates"]
 
     return verify_format(body, result)
 
 
 def format_key_options(body: Json) -> Json:
     """Format collection key options data.
 
@@ -223,14 +225,16 @@
                 "overwrite": cv["overwrite"],
                 "computedOn": cv["computedOn"],
                 "keepNull": cv["keepNull"],
                 "failOnWarning": cv["failOnWarning"],
             }
             for cv in body["computedValues"]
         ]
+    if "internalValidatorType" in body:
+        result["internal_validator_type"] = body["internalValidatorType"]
 
     return verify_format(body, result)
 
 
 def format_aql_cache(body: Json) -> Json:
     """Format AQL cache data.
 
@@ -389,14 +393,18 @@
     :param body: Input body.
     :type body: dict
     :return: Formatted body.
     :rtype: dict
     """
     result: Json = {}
 
+    if "agency" in body:
+        result["agency"] = body["agency"]
+    if "coordinator" in body:
+        result["coordinator"] = body["coordinator"]
     if "foxxApi" in body:
         result["foxx_api"] = body["foxxApi"]
     if "host" in body:
         result["host"] = body["host"]
     if "hostname" in body:
         result["hostname"] = body["hostname"]
     if "license" in body:
@@ -981,14 +989,17 @@
     if "version" in body:
         result["version"] = body["version"]
     if "keys" in body:
         result["keys"] = body["keys"]
     if "nrPiecesPresent" in body:
         result["pieces_present"] = body["nrPiecesPresent"]
 
+    if "countIncludesFilesOnly" in body:
+        result["count_includes_files_only"] = body["countIncludesFilesOnly"]
+
     return verify_format(body, result)
 
 
 def format_backups(body: Json) -> Json:
     """Format backup entries.
 
     :param body: Input body.
@@ -1131,14 +1142,22 @@
         result["received_count"] = body["receivedCount"]
     if "sendCount" in body:
         result["send_count"] = body["sendCount"]
 
     # The detail element was introduced in 3.10
     if "detail" in body:
         result["detail"] = body["detail"]
+    if "database" in body:
+        result["database"] = body["database"]
+    if "masterContext" in body:
+        result["master_context"] = body["masterContext"]
+    if "parallelism" in body:
+        result["parallelism"] = body["parallelism"]
+    if "useMemoryMaps" in body:
+        result["use_memory_maps"] = body["useMemoryMaps"]
 
     return verify_format(body, result)
 
 
 def format_pregel_job_list(body: Sequence[Json]) -> Json:
     """Format Pregel job list data.
 
@@ -1173,20 +1192,26 @@
                 "to_vertex_collections": edge_definition["to"],
             }
             for edge_definition in body["edgeDefinitions"]
         ],
     }
     if "isSmart" in body:
         result["smart"] = body["isSmart"]
+    if "isSatellite" in body:
+        result["is_satellite"] = body["isSatellite"]
     if "smartGraphAttribute" in body:
         result["smart_field"] = body["smartGraphAttribute"]
     if "numberOfShards" in body:
         result["shard_count"] = body["numberOfShards"]
     if "replicationFactor" in body:
         result["replication_factor"] = body["replicationFactor"]
+    if "minReplicationFactor" in body:
+        result["min_replication_factor"] = body["minReplicationFactor"]
+    if "writeConcern" in body:
+        result["write_concern"] = body["writeConcern"]
 
     return verify_format(body, result)
 
 
 def format_query_cache_entry(body: Json) -> Json:
     """Format AQL query cache entry.
```

### Comparing `python-arango-7.5.7/arango/foxx.py` & `python-arango-7.5.8/arango/foxx.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/graph.py` & `python-arango-7.5.8/arango/graph.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/http.py` & `python-arango-7.5.8/arango/http.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/job.py` & `python-arango-7.5.8/arango/job.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/pregel.py` & `python-arango-7.5.8/arango/pregel.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/replication.py` & `python-arango-7.5.8/arango/replication.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/request.py` & `python-arango-7.5.8/arango/request.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/resolver.py` & `python-arango-7.5.8/arango/resolver.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/response.py` & `python-arango-7.5.8/arango/response.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/utils.py` & `python-arango-7.5.8/arango/utils.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/arango/wal.py` & `python-arango-7.5.8/arango/wal.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/Makefile` & `python-arango-7.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/admin.rst` & `python-arango-7.5.8/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/analyzer.rst` & `python-arango-7.5.8/docs/analyzer.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/aql.rst` & `python-arango-7.5.8/docs/aql.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/async.rst` & `python-arango-7.5.8/docs/async.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/auth.rst` & `python-arango-7.5.8/docs/auth.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/backup.rst` & `python-arango-7.5.8/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/batch.rst` & `python-arango-7.5.8/docs/batch.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/certificates.rst` & `python-arango-7.5.8/docs/certificates.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/cluster.rst` & `python-arango-7.5.8/docs/cluster.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/collection.rst` & `python-arango-7.5.8/docs/collection.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/conf.py` & `python-arango-7.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/contributing.rst` & `python-arango-7.5.8/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/cursor.rst` & `python-arango-7.5.8/docs/cursor.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/database.rst` & `python-arango-7.5.8/docs/database.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/document.rst` & `python-arango-7.5.8/docs/document.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/errors.rst` & `python-arango-7.5.8/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/foxx.rst` & `python-arango-7.5.8/docs/foxx.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,37 +27,37 @@
 
     # List services.
     foxx.services()
 
     # Create a service using source on server.
     foxx.create_service(
         mount=service_mount,
-        source='/tmp/service.zip',
+        source='/tests/static/service.zip',
         config={},
         dependencies={},
         development=True,
         setup=True,
         legacy=True
     )
 
     # Update (upgrade) a service.
     service = db.foxx.update_service(
         mount=service_mount,
-        source='/tmp/service.zip',
+        source='/tests/static/service.zip',
         config={},
         dependencies={},
         teardown=True,
         setup=True,
         legacy=False
     )
 
     # Replace (overwrite) a service.
     service = db.foxx.replace_service(
         mount=service_mount,
-        source='/tmp/service.zip',
+        source='/tests/static/service.zip',
         config={},
         dependencies={},
         teardown=True,
         setup=True,
         legacy=True,
         force=False
     )
```

### Comparing `python-arango-7.5.7/docs/graph.rst` & `python-arango-7.5.8/docs/graph.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/http.rst` & `python-arango-7.5.8/docs/http.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/index.rst` & `python-arango-7.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/indexes.rst` & `python-arango-7.5.8/docs/indexes.rst`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     # Add a new geo-spatial index on field 'coordinates'.
     index = cities.add_geo_index(fields=['coordinates'])
 
     # Add a new persistent index on field 'currency'.
     index = cities.add_persistent_index(fields=['currency'], sparse=True)
 
     # Add a new TTL (time-to-live) index on field 'currency'.
-    index = cities.add_ttl_index(fields=['ttl'], expiry_time=200)
+    index = cities.add_ttl_index(fields=['currency'], expiry_time=200)
 
     # Indexes may be added with a name that can be referred to in AQL queries.
     index = cities.add_hash_index(fields=['country'], name='my_hash_index')
 
     # Delete the last index from the collection.
     cities.delete_index(index['id'])
```

### Comparing `python-arango-7.5.7/docs/logging.rst` & `python-arango-7.5.8/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/make.bat` & `python-arango-7.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/overview.rst` & `python-arango-7.5.8/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/pregel.rst` & `python-arango-7.5.8/docs/pregel.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/replication.rst` & `python-arango-7.5.8/docs/replication.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/schema.rst` & `python-arango-7.5.8/docs/schema.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/serializer.rst` & `python-arango-7.5.8/docs/serializer.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/simple.rst` & `python-arango-7.5.8/docs/simple.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/specs.rst` & `python-arango-7.5.8/docs/specs.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/static/logo.png` & `python-arango-7.5.8/docs/static/logo.png`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/task.rst` & `python-arango-7.5.8/docs/task.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/threading.rst` & `python-arango-7.5.8/docs/threading.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/transaction.rst` & `python-arango-7.5.8/docs/transaction.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/user.rst` & `python-arango-7.5.8/docs/user.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/view.rst` & `python-arango-7.5.8/docs/view.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/docs/wal.rst` & `python-arango-7.5.8/docs/wal.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/pyproject.toml` & `python-arango-7.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.7/python_arango.egg-info/PKG-INFO` & `python-arango-7.5.8/python_arango.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-arango
-Version: 7.5.7
+Version: 7.5.8
 Summary: Python Driver for ArangoDB
 Home-page: https://github.com/ArangoDB-Community/python-arango
 Author: Joohwan Oh
 Author-email: joohwan.oh@outlook.com
 License: MIT
 Keywords: arangodb,python,driver
 Classifier: Intended Audience :: Developers
```

### Comparing `python-arango-7.5.7/python_arango.egg-info/SOURCES.txt` & `python-arango-7.5.8/python_arango.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+tester.sh
 .github/workflows/build.yaml
 .github/workflows/codeql.yaml
 .github/workflows/pypi.yaml
 arango/__init__.py
 arango/api.py
 arango/aql.py
 arango/backup.py
```

### Comparing `python-arango-7.5.7/setup.py` & `python-arango-7.5.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     license="MIT",
     install_requires=[
         "urllib3>=1.26.0",
         "requests",
         "requests_toolbelt",
         "PyJWT",
         "setuptools>=42",
+        "importlib_metadata>=4.7.1",
     ],
     extras_require={
         "dev": [
             "black>=22.3.0",
             "flake8>=4.0.1",
             "isort>=5.10.1",
             "mypy>=0.942",
```

