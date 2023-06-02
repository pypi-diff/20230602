# Comparing `tmp/geocat.viz-2023.5.0.tar.gz` & `tmp/geocat.viz-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocat.viz-2023.5.0.tar", last modified: Fri May  5 15:41:39 2023, max compression
+gzip compressed data, was "geocat.viz-2023.6.0.tar", last modified: Fri Jun  2 04:18:53 2023, max compression
```

## Comparing `geocat.viz-2023.5.0.tar` & `geocat.viz-2023.6.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/ISSUE_TEMPLATE/plot-type-request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.github/workflows/upstream-examples-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/build_envs/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/build_envs/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/build_envs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/build_envs/upstream-dev-environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/docs/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/icons/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/icons/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/icons/notpublic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/icons/public.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/_static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (123)   171533 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/logos/GeoCAT_long.svg
--rw-r--r--   0 runner    (1001) docker     (123)   291776 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/logos/GeoCAT_nsf.svg
--rw-r--r--   0 runner    (1001) docker     (123)   180376 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/logos/GeoCAT_square.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/images/logos/nsf.png
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/internal_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/docs/user_api/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/docs/user_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.731566 geocat.viz-2023.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.735566 geocat.viz-2023.5.0/src/geocat/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/src/geocat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/src/geocat/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/src/geocat/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30219 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/src/geocat/viz/taylor.py
--rw-r--r--   0 runner    (1001) docker     (123)    51827 2023-05-05 15:41:24.000000 geocat.viz-2023.5.0/src/geocat/viz/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:39.739567 geocat.viz-2023.5.0/src/geocat.viz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 15:41:39.000000 geocat.viz-2023.5.0/src/geocat.viz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.931011 geocat.viz-2023.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/ISSUE_TEMPLATE/plot-type-request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/workflows/upstream-examples-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/build_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/build_envs/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/build_envs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/build_envs/upstream-dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.931011 geocat.viz-2023.6.0/docs/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/docs/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/icons/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/icons/notpublic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/icons/public.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/docs/_static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)   171533 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_long.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   291776 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_nsf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   180376 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_square.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/logos/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.931011 geocat.viz-2023.6.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/docs/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/internal_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/docs/user_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/user_api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.931011 geocat.viz-2023.6.0/gallery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/gallery/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/gallery/util/add_height_from_pressure_axis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/src/geocat/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/src/geocat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/src/geocat/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/src/geocat/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/src/geocat/viz/taylor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62471 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/src/geocat/viz/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/src/geocat.viz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/top_level.txt
```

### Comparing `geocat.viz-2023.5.0/.github/workflows/ci.yml` & `geocat.viz-2023.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/.github/workflows/pypi.yaml` & `geocat.viz-2023.6.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/.github/workflows/upstream-examples-ci.yml` & `geocat.viz-2023.6.0/.github/workflows/upstream-examples-ci.yml`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/.pre-commit-config.yaml` & `geocat.viz-2023.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/CONTRIBUTING.md` & `geocat.viz-2023.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/LICENSE` & `geocat.viz-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/PKG-INFO` & `geocat.viz-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocat.viz
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: GeoCAT-viz is vizualization component of the GeoCAT project and
 Home-page: https://geocat-viz.readthedocs.io
 Author: GeoCAT Team
 Author-email: geocat@ucar.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `geocat.viz-2023.5.0/README.md` & `geocat.viz-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/build_envs/upstream-dev-environment.yml` & `geocat.viz-2023.6.0/build_envs/upstream-dev-environment.yml`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/Makefile` & `geocat.viz-2023.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/_static/images/icons/code.svg` & `geocat.viz-2023.6.0/docs/_static/images/icons/code.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/_static/images/icons/notpublic.svg` & `geocat.viz-2023.6.0/docs/_static/images/icons/notpublic.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/_static/images/icons/public.svg` & `geocat.viz-2023.6.0/docs/_static/images/icons/public.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/_static/images/logos/GeoCAT_long.svg` & `geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_long.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/_static/images/logos/GeoCAT_nsf.svg` & `geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_nsf.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/_static/images/logos/GeoCAT_square.svg` & `geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_square.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/_static/images/logos/nsf.png` & `geocat.viz-2023.6.0/docs/_static/images/logos/nsf.png`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/_templates/autosummary/class.rst` & `geocat.viz-2023.6.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/api.rst` & `geocat.viz-2023.6.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/citation.rst` & `geocat.viz-2023.6.0/docs/citation.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/conf.py` & `geocat.viz-2023.6.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # -- Project information -----------------------------------------------------
 
+import datetime
+import geocat.viz as gv
 import os
 import sys
 import pathlib
 import yaml
 from sphinx.application import Sphinx
 from sphinx.util import logging
 from textwrap import dedent, indent
 
 print("sys.path:", sys.path)
 
-import geocat.viz as gv
-
 LOGGER = logging.getLogger("conf")
 
 try:
     from unittest.mock import MagicMock
 except ImportError:
     from mock import Mock as MagicMock
 
@@ -124,15 +124,15 @@
 autosummary_generate = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
-# source_suffix = ['.rst', '.md']
+#source_suffix = ['.rst', '.md']
 source_suffix = {
     '.rst': 'restructuredtext',
     '.ipynb': 'myst-nb',
     '.myst': 'myst-nb',
 }
 
 # The encoding of source files.
@@ -140,16 +140,14 @@
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'GeoCAT-viz'
 
-import datetime
-
 current_year = datetime.datetime.now().year
 copyright = u'{}, University Corporation for Atmospheric Research'.format(
     current_year)
 author = u'GeoCAT'
 
 # The version info for the project being documented
 version = gv.__version__.split("+")[0]
@@ -322,13 +320,13 @@
 autodoc_typehints = 'none'
 
 # turn off notebook execution
 # set to "auto" for default behavior
 nb_execution_mode = "off"
 
 # generate warning for all invalid links
-# nitpicky = True
+#nitpicky = True
 
 
 # Allow for changes to be made to the css in the theme_overrides file
 def setup(app):
     app.add_css_file('theme_overrides.css')
```

### Comparing `geocat.viz-2023.5.0/docs/index.rst` & `geocat.viz-2023.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/installation.rst` & `geocat.viz-2023.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/make.bat` & `geocat.viz-2023.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/support.rst` & `geocat.viz-2023.6.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/docs/user_api/index.rst` & `geocat.viz-2023.6.0/docs/user_api/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -38,16 +38,29 @@
 
    truncate_colormap
 
    xr_add_cyclic_longitudes
 
    set_map_boundary
 
-   findLocalExtrema
+   find_local_extrema
 
-   plotCLabels
+   plot_contour_labels
 
-   plotELabels
+   plot_extrema_labels
 
    set_vector_density
 
    get_skewt_vars
+
+Deprecated Functions
+--------------------
+Util
+^^^^^^^^^^^^^
+.. currentmodule:: geocat.viz.util
+.. autosummary::
+   :nosignatures:
+   :toctree: ./generated/
+
+   findLocalExtrema
+   plotCLabels
+   plotELabels
```

### Comparing `geocat.viz-2023.5.0/setup.cfg` & `geocat.viz-2023.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.5.0/src/geocat/viz/taylor.py` & `geocat.viz-2023.6.0/src/geocat/viz/taylor.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,28 +155,28 @@
         # Bottom axis is not needed
         ax.axis["bottom"].set_visible(False)
 
         self._ax = ax  # Graphical axes
         self.ax = ax.get_aux_axes(tr)  # Polar coordinates
 
         # Add reference point stddev contour
-        t = np.linspace(0, np.pi / 2)
-        r = np.zeros_like(t) + self.refstd
-        h, = self.ax.plot(t,
-                          r,
-                          linewidth=1,
-                          linestyle=(0, (9, 5)),
-                          color='black',
-                          zorder=1)
+        t_array = np.linspace(0, np.pi / 2)
+        r_array = np.zeros_like(t_array) + self.refstd
+        h_plot, = self.ax.plot(t_array,
+                               r_array,
+                               linewidth=1,
+                               linestyle=(0, (9, 5)),
+                               color='black',
+                               zorder=1)
 
         # Set aspect ratio
         self.ax.set_aspect('equal')
 
         # Store the reference line
-        self.referenceLine = h
+        self.referenceLine = h_plot
 
         # Collect sample points for latter use (e.g. legend)
         self.modelMarkerSet = []
 
         # Set number for models outside axes
         self.modelOutside = -1
 
@@ -313,16 +313,16 @@
 
         # Add modelset to modelMarkerSet for legend handles
         if not percent_bias_on:
             self.modelMarkerSet.append(modelset)
         else:
             label = kwargs.get('label')
             if percent_bias_on:
-                handle = plt.scatter(1, 2, color=color, label=label)
-                self.modelMarkerSet.append(handle)
+                plot_handle = plt.scatter(1, 2, color=color, label=label)
+                self.modelMarkerSet.append(plot_handle)
 
         # Annotate model markers if annotate_on is True
         if annotate_on:
             # Initialize empty array that will be filled with model label text objects and returned
             modelTexts = []
 
             for std, corr in zip(std_plot, corr_plot):
@@ -457,23 +457,23 @@
         Examples
         --------
         All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
          - `NCL_taylor_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/TaylorDiagrams/NCL_taylor_2.html?highlight=add_ygrid>`_
         """
 
-        t = np.linspace(0, np.pi / 2)
+        t_array = np.linspace(0, np.pi / 2)
         for value in arr:
-            r = np.zeros_like(t) + value
-            h, = self.ax.plot(t,
-                              r,
-                              color=color,
-                              linestyle=linestyle,
-                              linewidth=linewidth,
-                              **kwargs)
+            r_array = np.zeros_like(t_array) + value
+            h_plot, = self.ax.plot(t_array,
+                                   r_array,
+                                   color=color,
+                                   linestyle=linestyle,
+                                   linewidth=linewidth,
+                                   **kwargs)
 
     def add_grid(self, *args, **kwargs):
         """Add a grid.
 
         Notes
         -----
         *args* and *kwargs* are propagated to `matplotlib.axes.Axes.grid`
```

### Comparing `geocat.viz-2023.5.0/src/geocat/viz/util.py` & `geocat.viz-2023.6.0/src/geocat/viz/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from sklearn.cluster import DBSCAN
 
 import matplotlib as mpl
 import matplotlib.axes
 import matplotlib.path as mpath
 import matplotlib.pyplot as plt
 import matplotlib.ticker as tic
-import matplotlib.cm as cm
 
 import cartopy.crs as ccrs
 import cartopy.util as cutil
 import cartopy.mpl.geoaxes
 from cartopy.mpl.ticker import LongitudeFormatter, LatitudeFormatter
 
 import metpy.calc as mpcalc
@@ -635,39 +634,45 @@
     if ylim is not None:
         ax.set_ylim(ylim)
 
 
 def truncate_colormap(cmap: matplotlib.colors.Colormap,
                       minval: typing.Union[int, float] = 0.0,
                       maxval: typing.Union[int, float] = 1.0,
-                      n: int = 100,
-                      name: str = None):
+                      n: int = 256,
+                      name: str = None,
+                      force: bool = True):
     """Utility function that truncates a colormap. Registers the new colormap
-    by name in plt.cm, and also returns the updated map.
+    by name and returns the corresponding colormap object.
 
     `Copied from Stack Overflow <https://stackoverflow.com/questions/18926031/how-to-extract-a-subset-of-a-colormap-as-a-new-colormap-in-matplotlib>`_
 
     Parameters
     ----------
     cmap : :class:`matplotlib.colors.Colormap`
         Colormap to be truncated.
 
     minval : int, float
-        Minimum value to be used for truncation of the color map.
+        Minimum normalized value to be used for truncation of the color map.
 
     maxval : int, float
-        Maximum value to be used for truncation of the color map.
+        Maximum normalized value to be used for truncation of the color map.
 
     n : int
         Number of color values in the new color map.
 
     name : str
         Optional name of the new color map. If not set, a new name is generated by using the name of the input
         colormap as well as min and max values.
 
+    force : bool, default = True
+        If False, a ValueError is raised if trying to overwrite an already registered name. True supports
+        overwriting registered colormaps other than the builtin colormaps.
+
+
     Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the
     `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_dev_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Panels/NCL_dev_2.html?highlight=truncate_colormap>`_
 
@@ -677,18 +682,21 @@
     """
 
     if not name:
         name = "trunc({n},{a:.2f},{b:.2f})".format(n=cmap.name,
                                                    a=minval,
                                                    b=maxval)
     new_cmap = mpl.colors.LinearSegmentedColormap.from_list(
-        name=name,
-        colors=cmap(np.linspace(minval, maxval, n)),
-    )
-    cm.register_cmap(name, new_cmap)
+        name=name, colors=cmap(np.linspace(minval, maxval)), N=n)
+
+    try:
+        mpl.colormaps.register(new_cmap, force=force)
+    except AttributeError:
+        mpl.cm.register_cmap(name=name, cmap=new_cmap)
+
     return new_cmap
 
 
 def xr_add_cyclic_longitudes(da: xr.DataArray, coord: str):
     """Utility function to handle the no-shown-data artifact of 0 and
     360-degree longitudes.
 
@@ -829,25 +837,27 @@
     # west and continuing anticlockwise creating a point every `res` degree
     if lon_range[0] >= 0 >= lon_range[1]:  # Case when range crosses antimeridian
         vertices = [(lon, lat_range[0]) for lon in range(lon_range[0], 180 + 1, res)] + \
                    [(lon, lat_range[0]) for lon in range(-180, lon_range[1] + 1, res)] + \
                    [(lon_range[1], lat) for lat in range(lat_range[0], lat_range[1] + 1, res)] + \
                    [(lon, lat_range[1]) for lon in range(lon_range[1], -180 - 1, -res)] + \
                    [(lon, lat_range[1]) for lon in range(180, lon_range[0] - 1, -res)] + \
-                   [(lon_range[0], lat) for lat in range(lat_range[1], lat_range[0] - 1, -res)]
+                   [(lon_range[0], lat)
+                    for lat in range(lat_range[1], lat_range[0] - 1, -res)]
         path = mpath.Path(vertices)
     elif ((lon_range[0] == 180 or lon_range[0] == -180) and
           (lon_range[1] == 180 or lon_range[1] == -180)):
         vertices = [(lon, lat_range[0]) for lon in range(0, 360 + 1, res)]
         path = mpath.Path(vertices)
     else:
         vertices = [(lon, lat_range[0]) for lon in range(lon_range[0], lon_range[1] + 1, res)] + \
                    [(lon_range[1], lat) for lat in range(lat_range[0], lat_range[1] + 1, res)] + \
                    [(lon, lat_range[1]) for lon in range(lon_range[1], lon_range[0] - 1, -res)] + \
-                   [(lon_range[0], lat) for lat in range(lat_range[1], lat_range[0] - 1, -res)]
+                   [(lon_range[0], lat)
+                    for lat in range(lat_range[1], lat_range[0] - 1, -res)]
         path = mpath.Path(vertices)
 
     proj_to_data = ccrs.PlateCarree()._as_mpl_transform(ax) - ax.transData
     ax.set_boundary(proj_to_data.transform_path(path))
 
     ax.set_extent([
         lon_range[0] - west_pad, lon_range[1] + east_pad,
@@ -857,14 +867,71 @@
 
 
 def findLocalExtrema(da: xr.DataArray,
                      highVal: int = 0,
                      lowVal: int = 1000,
                      eType: str = 'Low',
                      eps: float = 10) -> list:
+    r""".. deprecated:: 2023.02.0 The ``findLocalExtrema`` function is deprecated due to naming conventions. Use :func:`find_local_extrema` instead.
+
+    Utility function to find local low/high field variable coordinates on a
+    contour map. To classify as a local high, the data point must be greater
+    than highval, and to classify as a local low, the data point must be less
+    than lowVal.
+
+    Parameters
+    ----------
+    da : :class:`xarray.DataArray`
+        Xarray data array containing the lat, lon, and field variable (ex. pressure) data values
+
+    highVal : int
+        Data value that the local high must be greater than to qualify as a "local high" location.
+        Default highVal is 0.
+
+    lowVal : int
+        Data value that the local low must be less than to qualify as a "local low" location.
+        Default lowVal is 1000.
+
+    eType : str
+        'Low' or 'High'
+        Determines which extrema are being found- minimum or maximum, respectively.
+        Default eType is 'Low'.
+
+    eps : float
+            Parameter supplied to sklearn.cluster.DBSCAN determining the maximum distance between two samples
+            for one to be considered as in the neighborhood of the other.
+            Default eps is 10.
+
+    Returns
+    -------
+    clusterExtremas : list
+        List of coordinate tuples in GPS form (lon in degrees, lat in degrees)
+        that specify local low/high locations
+
+    Examples
+    --------
+    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+    - `NCL_sat_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_1.html?highlight=findlocalextrema>`_
+
+    - `NCL_sat_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_2.html?highlight=findlocalextrema>`_
+    """
+
+    warnings.warn(
+        'This function is deprecated. Call `find_local_extrema` instead.',
+        PendingDeprecationWarning)
+
+    return find_local_extrema(da, highVal, lowVal, eType, eps)
+
+
+def find_local_extrema(da: xr.DataArray,
+                       highVal: int = 0,
+                       lowVal: int = 1000,
+                       eType: str = 'Low',
+                       eps: float = 10) -> list:
     """Utility function to find local low/high field variable coordinates on a
     contour map. To classify as a local high, the data point must be greater
     than highval, and to classify as a local low, the data point must be less
     than lowVal.
 
     Parameters
     ----------
@@ -950,27 +1017,27 @@
     # Initialize array of coordinates to be returned
     clusterExtremas = []
 
     # Iterate through the coordinates in each cluster
     for key in coordsAndLabels:
 
         # Create array to hold all the field variable values for that cluster
-        datavals = []
+        data_vals = []
         for coord in coordsAndLabels[key]:
             # Find pressure data at that coordinate
             cond = np.logical_and(coordarr[:, :, 0] == coord[0],
                                   coordarr[:, :, 1] == coord[1])
             x, y = np.where(cond)
-            datavals.append(da.data[x[0]][y[0]])
+            data_vals.append(da.data[x[0]][y[0]])
 
         # Find the index of the smallest/greatest field variable value of each cluster
         if eType == 'Low':
-            index = np.argmin(np.array(datavals))
+            index = np.argmin(np.array(data_vals))
         if eType == 'High':
-            index = np.argmax(np.array(datavals))
+            index = np.argmax(np.array(data_vals))
 
         # Append the coordinate corresponding to that index to the array to be returned
         clusterExtremas.append(
             (coordsAndLabels[key][index][0], coordsAndLabels[key][index][1]))
 
     return clusterExtremas
 
@@ -979,14 +1046,80 @@
                 contours,
                 transform: cartopy.crs.CRS,
                 proj: cartopy.crs.CRS,
                 clabel_locations: list = [],
                 fontsize: int = 12,
                 whitebbox: bool = False,
                 horizontal: bool = False) -> list:
+    r""".. deprecated:: 2023.02.0 The ``plotCLabels`` function is deprecated due to naming conventions. Use :func:`plot_contour_levels` instead.
+
+    Utility function to plot contour labels by passing in a coordinate to
+    the clabel function.
+
+    This allows the user to specify the exact locations of the labels, rather than having matplotlib
+    plot them automatically.
+
+
+    Parameters
+    ----------
+    ax : :class:`matplotlib.axes.Axes`
+        Axis containing the contour set.
+
+    contours : :class:`matplotlib.contour.QuadContourSet`
+        Contour set that is being labeled.
+
+    transform : :class:`cartopy.crs.CRS`
+        Instance of CRS that represents the source coordinate system of coordinates.
+        (ex. ccrs.Geodetic()).
+
+    proj : :class:`cartopy.crs.CRS`
+        Projection 'ax' is defined by.
+        This is the instance of CRS that the coordinates will be transformed to.
+
+    clabel_locations : list
+        List of coordinate tuples in GPS form (lon in degrees, lat in degrees)
+        that specify where the contours with regular field variable values should be plotted.
+
+    fontsize : int
+        Font size of contour labels.
+
+    whitebbox : bool
+        Setting this to "True" will cause all labels to be plotted with white backgrounds
+
+    horizontal : bool
+        Setting this to "True" will cause the contour labels to be horizontal.
+
+    Returns
+    -------
+    cLabels : list
+        List of text instances of all contour labels
+
+    Examples
+    --------
+    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+    - `NCL_sat_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_1.html?highlight=plotCLabels>`_
+    """
+
+    warnings.warn(
+        'This function is  deprecated. Call `plot_contour_labels` instead.',
+        PendingDeprecationWarning)
+
+    return plot_contour_labels(ax, contours, transform, proj, clabel_locations,
+                               fontsize, whitebbox, horizontal)
+
+
+def plot_contour_labels(ax: matplotlib.axes.Axes,
+                        contours,
+                        transform: cartopy.crs.CRS,
+                        proj: cartopy.crs.CRS,
+                        clabel_locations: list = [],
+                        fontsize: int = 12,
+                        whitebbox: bool = False,
+                        horizontal: bool = False) -> list:
     """Utility function to plot contour labels by passing in a coordinate to
     the clabel function.
 
     This allows the user to specify the exact locations of the labels, rather than having matplotlib
     plot them automatically.
 
 
@@ -1041,15 +1174,15 @@
             np.array([x[1] for x in clabel_locations]))
         transformed_locations = [(x[0], x[1]) for x in clevelpoints]
         ax.clabel(contours,
                   manual=transformed_locations,
                   inline=True,
                   fontsize=fontsize,
                   colors='black',
-                  fmt="%.0f")
+                  fmt='%.0f')
         [cLabels.append(txt) for txt in contours.labelTexts]
 
         if horizontal is True:
             [txt.set_rotation('horizontal') for txt in contours.labelTexts]
 
     if whitebbox is True:
         [
@@ -1064,14 +1197,82 @@
                 transform: cartopy.crs.CRS,
                 proj: cartopy.crs.CRS,
                 clabel_locations: list = [],
                 label: str = 'L',
                 fontsize: int = 22,
                 whitebbox: bool = False,
                 horizontal: bool = True) -> list:
+    r""".. deprecated:: 2023.02.0 The ``plotELabels`` function is deprecated due to naming conventions. Use :func:`plot_extrema_labels` instead.
+
+    Utility function to plot high/low contour labels.
+
+    High/Low contour labels will be plotted using text boxes for more accurate label values
+    and placement.
+    This function is exemplified in the python version of `sat_1_lg <https://www.ncl.ucar.edu/Applications/Images/sat_1_lg.png>`__
+
+    Parameters
+    ----------
+    da : :class:`xarray.DataArray`
+        Xarray data array containing the lat, lon, and field variable data values.
+
+    transform : :class:`cartopy.crs.CRS`
+        Instance of CRS that represents the source coordinate system of coordinates.
+        (ex. ccrs.Geodetic()).
+
+    proj : :class:`cartopy.crs.CRS`
+        Projection 'ax' is defined by.
+        This is the instance of CRS that the coordinates will be transformed to.
+
+    clabel_locations : list
+        List of coordinate tuples in GPS form (lon in degrees, lat in degrees)
+        that specify where the contour labels should be plotted.
+
+    label : str
+        ex. 'L' or 'H'
+        The data value will be plotted as a subscript of this label.
+
+    fontsize : int
+        Font size of regular contour labels.
+
+    horizontal : bool
+        Setting this to "True" will cause the contour labels to be horizontal.
+
+    whitebbox : bool
+        Setting this to "True" will cause all labels to be plotted with white backgrounds
+
+    Returns
+    -------
+    extremaLabels : list
+        List of text instances of all contour labels
+
+    Examples
+    --------
+    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+
+    - `NCL_sat_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_1.html?highlight=plotELabels>`_
+
+    - `NCL_sat_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_sat_2.html?highlight=plotELabels>`_
+    """
+
+    warnings.warn(
+        'This function is deprecated. Please use `plot_extrema_labels` instead.',
+        PendingDeprecationWarning)
+
+    return plot_extrema_labels(da, transform, proj, clabel_locations, label,
+                               fontsize, whitebbox, horizontal)
+
+
+def plot_extrema_labels(da: xr.DataArray,
+                        transform: cartopy.crs.CRS,
+                        proj: cartopy.crs.CRS,
+                        label_locations: list = [],
+                        label: str = 'L',
+                        fontsize: int = 22,
+                        whitebbox: bool = False,
+                        horizontal: bool = True) -> list:
     """Utility function to plot contour labels.
 
     High/Low contour labels will be plotted using text boxes for more accurate label values
     and placement.
     This function is exemplified in the python version of https://www.ncl.ucar.edu/Applications/Images/sat_1_lg.png
 
     Parameters
@@ -1083,15 +1284,15 @@
         Instance of CRS that represents the source coordinate system of coordinates.
         (ex. ccrs.Geodetic()).
 
     proj : :class:`cartopy.crs.CRS`
         Projection 'ax' is defined by.
         This is the instance of CRS that the coordinates will be transformed to.
 
-    clabel_locations : list
+    label_locations : list
         List of coordinate tuples in GPS form (lon in degrees, lat in degrees)
         that specify where the contour labels should be plotted.
 
     label : str
         ex. 'L' or 'H'
         The data value will be plotted as a subscript of this label.
 
@@ -1128,31 +1329,31 @@
     coordarr = np.dstack((lons, lats))
 
     # Initialize empty array that will be filled with contour label text objects and returned
     extremaLabels = []
 
     # Plot any low contour levels
     clabel_points = proj.transform_points(
-        transform, np.array([x[0] for x in clabel_locations]),
-        np.array([x[1] for x in clabel_locations]))
+        transform, np.array([x[0] for x in label_locations]),
+        np.array([x[1] for x in label_locations]))
     transformed_locations = [(x[0], x[1]) for x in clabel_points]
 
-    for x in range(len(transformed_locations)):
+    for loc in range(len(transformed_locations)):
 
         try:
             # Find field variable data at that coordinate
-            coord = clabel_locations[x]
+            coord = label_locations[loc]
             cond = np.logical_and(coordarr[:, :, 0] == coord[0],
                                   coordarr[:, :, 1] == coord[1])
-            z, y = np.where(cond)
-            p = int(round(da.data[z[0]][y[0]]))
+            z_loc, y_loc = np.where(cond)
+            p_loc = int(round(da.data[z_loc[0]][y_loc[0]]))
 
-            lab = plt.text(transformed_locations[x][0],
-                           transformed_locations[x][1],
-                           label + "$_{" + str(p) + "}$",
+            lab = plt.text(transformed_locations[loc][0],
+                           transformed_locations[loc][1],
+                           label + '$_{' + str(p_loc) + '}$',
                            fontsize=fontsize,
                            horizontalalignment='center',
                            verticalalignment='center')
 
             if horizontal is True:
                 lab.set_rotation('horizontal')
 
@@ -1194,15 +1395,15 @@
 
     - `NCL_vector_3.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Vectors/NCL_vector_3.html?highlight=set_vector_density>`_
     """
     import math
     import warnings
 
     if minDistance <= 0:
-        raise Exception("minDistance cannot be negative or zero.")
+        raise Exception('minDistance cannot be negative or zero.')
     else:
         lat_every = 1
         lon_every = 1
 
         # Get distance between points in latitude (y axis)
         lat = data['lat']
         latdifference = float(lat[1] - lat[0])
@@ -1236,30 +1437,67 @@
         # Slice data arrays
         ds = data.isel(lat=slice(None, None, lat_every),
                        lon=slice(None, None, lon_every))
 
         return ds
 
 
-def get_skewt_vars(p: Quantity, tc: Quantity, tdc: Quantity,
-                   pro: Quantity) -> str:
+def get_skewt_vars(pressure: Quantity = None,
+                   temperature: Quantity = None,
+                   dewpoint: Quantity = None,
+                   profile: Quantity = None,
+                   p: Quantity = None,
+                   tc: Quantity = None,
+                   tdc: Quantity = None,
+                   pro: Quantity = None) -> str:
     """This function processes the dataset values and returns a string element
     which can be used as a subtitle to replicate the styles of NCL Skew-T
     Diagrams.
 
     Parameters
     ----------
+    pressure : :class:`pint.Quantity`
+        Pressure level input from dataset. Renamed from deprecated kwarg `p`.
+    temperature : :class:`pint.Quantity`
+        Temperature for parcel from dataset. Renamed from deprecated kwarg `tc`.
+    dewpoint : :class:`pint.Quantity`
+        Dew point temperature for parcel from dataset. Renamed from deprecated kwarg `tdc`.
+    profile : :class:`pint.Quantity`
+        Parcel profile temperature converted to degC. Renamed from deprecated kwarg `pro`.
     p : :class:`pint.Quantity`
-        Pressure level input from dataset
+        Pressure level input from dataset.
+
+        .. deprecated:: 2023.06.0
+            In an effort to refactor the codebase to follow naming conventions,
+            keyword arguments have been renamed to more meaningful values.
+            ``p`` parameter has been deprecated in favor of ``pressure`.
+
     tc : :class:`pint.Quantity`
-        Temperature for parcel from dataset
+        Temperature for parcel from dataset.
+
+        .. deprecated:: 2023.06.0
+            In an effort to refactor the codebase to follow naming conventions,
+            keyword arguments have been renamed to more meaningful values.
+            ``tc`` parameter has been deprecated in favor of ``temperature``.
+
     tdc : :class:`pint.Quantity`
-        Dew point temperature for parcel from dataset
+        Dew point temperature for parcel from dataset.
+
+        .. deprecated:: 2023.06.0
+            In an effort to refactor the codebase to follow naming conventions,
+            keyword arguments have been renamed to more meaningful values.
+            ``tdc`` parameter has been deprecated in favor of ``dewpoint``.
+
     pro : :class:`pint.Quantity`
-        Parcel profile temperature converted to degC
+        Parcel profile temperature converted to degC.
+
+        .. deprecated:: 2023.06.0
+            In an effort to refactor the codebase to follow naming conventions,
+            keyword arguments have been renamed to more meaningful values.
+            ``pro`` parameter has been deprecated in favor of ``profile``.
 
     Returns
     -------
     joined : str
         A string element with the format "Plcl=<value> Tlcl[C]=<value> Shox=<value> Pwat[cm]=<value> Cape[J]=<value>" where:
         - Cape  -  Convective Available Potential Energy [J]
         - Pwat  -  Precipitable Water [cm]
@@ -1269,47 +1507,68 @@
 
     See Also
     --------
     Related NCL Functions:
         `skewT_PlotData <https://www.ncl.ucar.edu/Document/Functions/Skewt_func/skewT_PlotData.shtml>`_,
         `skewt_BackGround <https://www.ncl.ucar.edu/Document/Functions/Skewt_func/skewT_BackGround.shtml>`_
 
-     Examples
+    Examples
     --------
     All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_skewt_2_2 <https://geocat-examples.readthedocs.io/en/latest/gallery/Skew-T/NCL_skewt_2_2.html?highlight=get_skewt_vars>`_
     """
+    # Support for deprecating kwargs
+    if p:
+        pressure = p
+        warnings.warn(
+            'The keyword argument `p` is deprecated. Use `pressure` instead.',
+            PendingDeprecationWarning)
+    if tc:
+        temperature = tc
+        warnings.warn(
+            'The keyword argument `tc` is deprecated. Use `temperature` instead.',
+            PendingDeprecationWarning)
+    if tdc:
+        dewpoint = tdc
+        warnings.warn(
+            'The keyword argument `tdc` is deprecated. Use `dewpoint` instead.',
+            PendingDeprecationWarning)
+    if pro:
+        profile = pro
+        warnings.warn(
+            'The keyword argument `pro` is deprecated. Use `profile` instead.',
+            PendingDeprecationWarning)
 
     # CAPE
-    cape = mpcalc.cape_cin(p, tc, tdc, pro)
+    cape = mpcalc.cape_cin(pressure, temperature, dewpoint, profile)
     cape = cape[0].magnitude
 
     # Precipitable Water
-    pwat = mpcalc.precipitable_water(p, tdc)
+    pwat = mpcalc.precipitable_water(pressure, dewpoint)
     pwat = (pwat.magnitude / 10) * units.cm  # Convert mm to cm
     pwat = pwat.magnitude
 
     # Pressure and temperature of lcl
-    lcl = mpcalc.lcl(p[0], tc[0], tdc[0])
+    lcl = mpcalc.lcl(pressure[0], temperature[0], dewpoint[0])
     plcl = lcl[0].magnitude
     tlcl = lcl[1].magnitude
 
     # Showalter index
-    shox = mpcalc.showalter_index(p, tc, tdc)
+    shox = mpcalc.showalter_index(pressure, temperature, dewpoint)
     shox = shox[0].magnitude
 
     # Place calculated values in iterable list
-    vals = [plcl, tlcl, shox, pwat, cape]
-    vals = np.round(vals).astype(int)
+    val_list = [plcl, tlcl, shox, pwat, cape]
+    val_ints = np.round(val_list).astype(int)
 
     # Define variable names for calculated values
     names = ['Plcl=', 'Tlcl[C]=', 'Shox=', 'Pwat[cm]=', 'Cape[J]=']
 
     # Combine the list of values with their corresponding labels
-    lst = list(chain.from_iterable(zip(names, vals)))
+    lst = list(chain.from_iterable(zip(names, val_ints)))
     lst = map(str, lst)
 
     # Create one large string for later plotting use
     joined = ' '.join(lst)
 
     return joined
```

### Comparing `geocat.viz-2023.5.0/src/geocat.viz.egg-info/PKG-INFO` & `geocat.viz-2023.6.0/src/geocat.viz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocat.viz
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: GeoCAT-viz is vizualization component of the GeoCAT project and
 Home-page: https://geocat-viz.readthedocs.io
 Author: GeoCAT Team
 Author-email: geocat@ucar.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `geocat.viz-2023.5.0/src/geocat.viz.egg-info/SOURCES.txt` & `geocat.viz-2023.6.0/src/geocat.viz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 docs/_static/images/logos/GeoCAT_long.svg
 docs/_static/images/logos/GeoCAT_nsf.svg
 docs/_static/images/logos/GeoCAT_square.svg
 docs/_static/images/logos/nsf.png
 docs/_templates/autosummary/class.rst
 docs/internal_api/index.rst
 docs/user_api/index.rst
+gallery/util/add_height_from_pressure_axis.ipynb
 src/geocat/__init__.py
 src/geocat.viz.egg-info/PKG-INFO
 src/geocat.viz.egg-info/SOURCES.txt
 src/geocat.viz.egg-info/dependency_links.txt
 src/geocat.viz.egg-info/not-zip-safe
 src/geocat.viz.egg-info/requires.txt
 src/geocat.viz.egg-info/top_level.txt
```

