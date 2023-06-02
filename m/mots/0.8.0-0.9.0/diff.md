# Comparing `tmp/mots-0.8.0.tar.gz` & `tmp/mots-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mots-0.8.0.tar", last modified: Tue Apr 18 15:00:12 2023, max compression
+gzip compressed data, was "mots-0.9.0.tar", last modified: Fri Jun  2 18:07:40 2023, max compression
```

## Comparing `mots-0.8.0.tar` & `mots-0.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.531195 mots-0.8.0/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3101 2023-04-18 14:59:25.000000 mots-0.8.0/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-18 14:59:25.000000 mots-0.8.0/.coveragerc
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-04-18 14:59:25.000000 mots-0.8.0/.flake8
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-18 14:59:25.000000 mots-0.8.0/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2023-04-18 14:59:25.000000 mots-0.8.0/.readthedocs.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-04-18 14:59:25.000000 mots-0.8.0/AUTHORS
--rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2023-04-18 14:59:25.000000 mots-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16727 2023-04-18 14:59:25.000000 mots-0.8.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3813 2023-04-18 14:59:25.000000 mots-0.8.0/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-04-18 15:00:12.535194 mots-0.8.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      984 2023-04-18 14:59:25.000000 mots-0.8.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-04-18 14:59:25.000000 mots-0.8.0/docker-compose.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.531195 mots-0.8.0/documentation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-04-18 14:59:25.000000 mots-0.8.0/documentation/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2153 2023-04-18 14:59:25.000000 mots-0.8.0/documentation/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13728 2023-04-18 14:59:25.000000 mots-0.8.0/documentation/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-04-18 14:59:25.000000 mots-0.8.0/mots.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      795 2023-04-18 14:59:25.000000 mots-0.8.0/mots.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-04-18 14:59:25.000000 mots-0.8.0/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.531195 mots-0.8.0/requirements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/base.in
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      159 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/get_filename
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33052 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/python3.10.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35675 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/python3.7.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33297 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/python3.8.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33276 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/python3.9.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1053 2023-04-18 15:00:12.535194 mots-0.8.0/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.527194 mots-0.8.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/src/mots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2489 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/bmo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      808 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/ci.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15263 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14341 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7732 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6454 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/export.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/logging.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/mach_interface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6937 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/module.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/pmo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2748 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/src/mots/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/templates/directory.template.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2381 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/templates/directory.template.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2952 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/yaml.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/src/mots.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4618 2023-04-18 14:59:25.000000 mots-0.8.0/tests/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9829 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6862 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5225 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_export.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5727 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_module.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_style.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4489 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.488805 mots-0.9.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.480805 mots-0.9.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3101 2023-06-02 18:07:00.000000 mots-0.9.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-02 18:07:00.000000 mots-0.9.0/.coveragerc
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-06-02 18:07:00.000000 mots-0.9.0/.flake8
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-06-02 18:07:00.000000 mots-0.9.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2023-06-02 18:07:00.000000 mots-0.9.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-06-02 18:07:00.000000 mots-0.9.0/AUTHORS
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2023-06-02 18:07:00.000000 mots-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16727 2023-06-02 18:07:00.000000 mots-0.9.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3813 2023-06-02 18:07:00.000000 mots-0.9.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-06-02 18:07:40.488805 mots-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      984 2023-06-02 18:07:00.000000 mots-0.9.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-06-02 18:07:00.000000 mots-0.9.0/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.480805 mots-0.9.0/documentation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-06-02 18:07:00.000000 mots-0.9.0/documentation/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2153 2023-06-02 18:07:00.000000 mots-0.9.0/documentation/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13728 2023-06-02 18:07:00.000000 mots-0.9.0/documentation/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-06-02 18:07:00.000000 mots-0.9.0/mots.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      795 2023-06-02 18:07:00.000000 mots-0.9.0/mots.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-06-02 18:07:00.000000 mots-0.9.0/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.484805 mots-0.9.0/requirements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/base.in
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      159 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/get_filename
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33052 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/python3.10.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35675 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/python3.7.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33297 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/python3.8.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33276 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/python3.9.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1053 2023-06-02 18:07:40.488805 mots-0.9.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.480805 mots-0.9.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.484805 mots-0.9.0/src/mots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/bmo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      808 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/ci.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15263 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14341 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6454 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/export.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/logging.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/mach_interface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6937 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/module.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/pmo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2748 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.484805 mots-0.9.0/src/mots/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/templates/directory.template.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2381 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/templates/directory.template.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.484805 mots-0.9.0/src/mots.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.488805 mots-0.9.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4618 2023-06-02 18:07:00.000000 mots-0.9.0/tests/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9829 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7046 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5225 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_export.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5727 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_module.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_style.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4489 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_utils.py
```

### Comparing `mots-0.8.0/.circleci/config.yml` & `mots-0.9.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/LICENSE` & `mots-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/Makefile` & `mots-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/PKG-INFO` & `mots-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mots
-Version: 0.8.0
+Version: 0.9.0
 Summary: Module Ownership in Tree System
 Home-page: https://github.com/mozilla-conduit/mots
 Author: Zeid Zabaneh
 Author-email: zeid@mozilla.com
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mots-0.8.0/README.md` & `mots-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/docker-compose.yml` & `mots-0.9.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/documentation/Makefile` & `mots-0.9.0/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/documentation/conf.py` & `mots-0.9.0/documentation/conf.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/documentation/index.rst` & `mots-0.9.0/documentation/index.rst`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/mots.yaml` & `mots-0.9.0/mots.yaml`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/requirements/python3.10.txt` & `mots-0.9.0/requirements/python3.10.txt`

 * *Files 1% similar despite different names*

```diff
@@ -379,17 +379,17 @@
     --hash=sha256:222439474e9c98fced559f1709d89e6c9cbf8d79c794ff3eb9f8800064291427 \
     --hash=sha256:e89512406b793ca39f5971bc999cc538ce125c0e51c27941bef4568b460095e2
     # via babel
 readme-renderer==37.3 \
     --hash=sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273 \
     --hash=sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343
     # via twine
-requests==2.28.1 \
-    --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
-    --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   requests-toolbelt
     #   sphinx
     #   twine
 requests-toolbelt==0.10.1 \
     --hash=sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7 \
     --hash=sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d
```

### Comparing `mots-0.8.0/requirements/python3.7.txt` & `mots-0.9.0/requirements/python3.7.txt`

 * *Files 1% similar despite different names*

```diff
@@ -385,17 +385,17 @@
     --hash=sha256:222439474e9c98fced559f1709d89e6c9cbf8d79c794ff3eb9f8800064291427 \
     --hash=sha256:e89512406b793ca39f5971bc999cc538ce125c0e51c27941bef4568b460095e2
     # via babel
 readme-renderer==37.3 \
     --hash=sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273 \
     --hash=sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343
     # via twine
-requests==2.28.1 \
-    --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
-    --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   requests-toolbelt
     #   sphinx
     #   twine
 requests-toolbelt==0.10.1 \
     --hash=sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7 \
     --hash=sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d
```

### Comparing `mots-0.8.0/requirements/python3.8.txt` & `mots-0.9.0/requirements/python3.8.txt`

 * *Files 1% similar despite different names*

```diff
@@ -380,17 +380,17 @@
     --hash=sha256:222439474e9c98fced559f1709d89e6c9cbf8d79c794ff3eb9f8800064291427 \
     --hash=sha256:e89512406b793ca39f5971bc999cc538ce125c0e51c27941bef4568b460095e2
     # via babel
 readme-renderer==37.3 \
     --hash=sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273 \
     --hash=sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343
     # via twine
-requests==2.28.1 \
-    --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
-    --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   requests-toolbelt
     #   sphinx
     #   twine
 requests-toolbelt==0.10.1 \
     --hash=sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7 \
     --hash=sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d
```

### Comparing `mots-0.8.0/requirements/python3.9.txt` & `mots-0.9.0/requirements/python3.9.txt`

 * *Files 1% similar despite different names*

```diff
@@ -380,17 +380,17 @@
     --hash=sha256:222439474e9c98fced559f1709d89e6c9cbf8d79c794ff3eb9f8800064291427 \
     --hash=sha256:e89512406b793ca39f5971bc999cc538ce125c0e51c27941bef4568b460095e2
     # via babel
 readme-renderer==37.3 \
     --hash=sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273 \
     --hash=sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343
     # via twine
-requests==2.28.1 \
-    --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
-    --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   requests-toolbelt
     #   sphinx
     #   twine
 requests-toolbelt==0.10.1 \
     --hash=sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7 \
     --hash=sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d
```

### Comparing `mots-0.8.0/setup.cfg` & `mots-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/bmo.py` & `mots-0.9.0/src/mots/bmo.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/ci.py` & `mots-0.9.0/src/mots/ci.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/cli.py` & `mots-0.9.0/src/mots/cli.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/config.py` & `mots-0.9.0/src/mots/config.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/directory.py` & `mots-0.9.0/src/mots/directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """Directory classes for mots."""
 from __future__ import annotations
 
 import copy
 from collections import defaultdict
 from dataclasses import asdict
 from dataclasses import dataclass
+from itertools import chain
 import logging
 from mots.module import Module
 from mots.utils import parse_real_name
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -114,14 +115,28 @@
                 rejected.append(path)
                 continue
             result[path] = self.index.get(self.repo_path / path, list())
         logger.debug(f"Query {paths} resolved to {result}.")
 
         return QueryResult(result, rejected)
 
+    @property
+    def peers_and_owners(self):
+        """Return a sorted list of all peers and owners."""
+        all_modules = self.modules
+        all_submodules = list(chain(*[module.submodules for module in all_modules]))
+        modules_and_submodules = all_modules + all_submodules
+
+        peers_and_owners = set()
+        for module in modules_and_submodules:
+            peers_and_owners.update(
+                [person["bmo_id"] for person in module.peers + module.owners]
+            )
+        return sorted(list(peers_and_owners))
+
 
 class QueryResult:
     """Helper class to simplify query result interpretation."""
 
     data_keys = {
         "paths",
         "rejected_paths",
```

### Comparing `mots-0.8.0/src/mots/export.py` & `mots-0.9.0/src/mots/export.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/logging.py` & `mots-0.9.0/src/mots/logging.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/mach_interface.py` & `mots-0.9.0/src/mots/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/module.py` & `mots-0.9.0/src/mots/module.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/pmo.py` & `mots-0.9.0/src/mots/pmo.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/settings.py` & `mots-0.9.0/src/mots/settings.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/templates/directory.template.md` & `mots-0.9.0/src/mots/templates/directory.template.md`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/templates/directory.template.rst` & `mots-0.9.0/src/mots/templates/directory.template.rst`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/utils.py` & `mots-0.9.0/src/mots/utils.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots/yaml.py` & `mots-0.9.0/src/mots/yaml.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/src/mots.egg-info/PKG-INFO` & `mots-0.9.0/src/mots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mots
-Version: 0.8.0
+Version: 0.9.0
 Summary: Module Ownership in Tree System
 Home-page: https://github.com/mozilla-conduit/mots
 Author: Zeid Zabaneh
 Author-email: zeid@mozilla.com
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mots-0.8.0/src/mots.egg-info/SOURCES.txt` & `mots-0.9.0/src/mots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/tests/conftest.py` & `mots-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/tests/test_config.py` & `mots-0.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/tests/test_directory.py` & `mots-0.9.0/tests/test_directory.py`

 * *Files 7% similar despite different names*

```diff
@@ -180,7 +180,13 @@
     assert empty_result
 
 
 def test_directory__QueryResult_empty_addition():
     empty_result = QueryResult()
     other_empty_result = QueryResult()
     assert not (empty_result + other_empty_result)
+
+
+def test_directory__peers_and_owners(repo):
+    file_config = FileConfig(repo / "mots.yml")
+    directory = Directory(file_config)
+    assert directory.peers_and_owners == [0, 1, 2]
```

### Comparing `mots-0.8.0/tests/test_export.py` & `mots-0.9.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/tests/test_module.py` & `mots-0.9.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/tests/test_settings.py` & `mots-0.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/tests/test_style.py` & `mots-0.9.0/tests/test_style.py`

 * *Files identical despite different names*

### Comparing `mots-0.8.0/tests/test_utils.py` & `mots-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

