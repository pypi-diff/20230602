# Comparing `tmp/pydash-7.0.3.tar.gz` & `tmp/pydash-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash-7.0.3.tar", last modified: Thu May  4 14:18:50 2023, max compression
+gzip compressed data, was "pydash-7.0.4.tar", last modified: Fri Jun  2 14:03:15 2023, max compression
```

## Comparing `pydash-7.0.3.tar` & `pydash-7.0.4.tar`

### file list

```diff
@@ -1,633 +1,633 @@
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.327670 pydash-7.0.3/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.275059 pydash-7.0.3/.tox/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261449 pydash-7.0.3/.tox/.package/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261507 pydash-7.0.3/.tox/.package/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261558 pydash-7.0.3/.tox/.package/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261598 pydash-7.0.3/.tox/.package/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.281661 pydash-7.0.3/.tox/.package/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.3/.tox/.package/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261706 pydash-7.0.3/.tox/.pkg/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261748 pydash-7.0.3/.tox/.pkg/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261795 pydash-7.0.3/.tox/.pkg/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261844 pydash-7.0.3/.tox/.pkg/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.281909 pydash-7.0.3/.tox/.pkg/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.3/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261952 pydash-7.0.3/.tox/3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261999 pydash-7.0.3/.tox/3.11/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.262051 pydash-7.0.3/.tox/3.11/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.264530 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282129 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282233 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282329 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282427 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282694 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282808 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282902 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282998 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283109 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283206 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283292 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283543 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283633 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283720 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283804 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283901 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.263151 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283986 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284333 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284456 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284546 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284798 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284888 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285106 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285202 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285431 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285512 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285705 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285906 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285999 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286094 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286227 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286332 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286425 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286692 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286785 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286873 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286958 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287045 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287139 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287223 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.264646 pydash-7.0.3/.tox/py310/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.264687 pydash-7.0.3/.tox/py310/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.264726 pydash-7.0.3/.tox/py310/lib/python3.10/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.267143 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287322 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287412 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287498 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287584 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287834 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287932 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288031 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288125 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288220 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288317 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288404 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288625 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288727 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288816 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288895 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288978 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289070 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.265843 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289168 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289415 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289502 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289579 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289756 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289835 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290068 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290161 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290363 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290438 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290647 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290850 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290943 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291041 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291133 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291229 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291329 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291577 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291658 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291737 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291819 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291903 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292219 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292320 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292429 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.267244 pydash-7.0.3/.tox/py311/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.267286 pydash-7.0.3/.tox/py311/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.267326 pydash-7.0.3/.tox/py311/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.269736 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292534 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292621 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292709 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292788 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293041 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293132 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293229 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293328 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293433 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293522 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293606 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293861 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293959 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294047 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294135 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294215 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.268465 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294309 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294550 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294630 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294714 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294918 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295229 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295316 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295568 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295664 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295902 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296176 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296283 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296377 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296461 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296547 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296645 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296903 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297024 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297136 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297240 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297335 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297429 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297524 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.269839 pydash-7.0.3/.tox/py37/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.269879 pydash-7.0.3/.tox/py37/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.269919 pydash-7.0.3/.tox/py37/lib/python3.7/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.272326 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297626 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297722 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297832 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297943 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298197 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298301 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298393 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298482 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298578 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298663 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298919 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299007 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299102 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299199 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299295 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299395 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.270870 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299493 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299766 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299873 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299980 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300245 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300340 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300575 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300660 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300873 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300953 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301177 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301395 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301487 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301582 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.271765 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301666 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301749 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301845 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301946 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302173 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302270 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302373 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302475 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302576 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302902 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303021 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.272423 pydash-7.0.3/.tox/py38/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.272459 pydash-7.0.3/.tox/py38/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.272494 pydash-7.0.3/.tox/py38/lib/python3.8/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.274981 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303133 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303245 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303351 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303436 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303711 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303819 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303927 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304042 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304157 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304264 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304373 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304653 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304771 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304884 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304998 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305122 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/importlib_resources/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305233 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305344 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.273504 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305462 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305738 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305858 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305973 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.306241 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.306355 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.306623 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.306778 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307019 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307132 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307396 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307668 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307789 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307900 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308008 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308122 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308235 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308515 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308630 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308741 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308858 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308972 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309214 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309321 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309424 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.275111 pydash-7.0.3/.tox/py39/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.275161 pydash-7.0.3/.tox/py39/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.275213 pydash-7.0.3/.tox/py39/lib/python3.9/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.278550 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309536 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309641 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309749 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309848 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310119 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310232 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310326 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310430 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310536 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310629 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310723 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310989 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311102 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311206 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311302 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311395 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311491 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.276652 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311595 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311848 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311954 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312061 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312292 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312388 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312590 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312673 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312872 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312954 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313182 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313383 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313477 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313572 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313659 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313743 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313835 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314043 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314125 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314210 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314287 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314370 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314581 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314669 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314759 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/twine/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)     1257 2021-06-27 18:15:07.000000 pydash-7.0.3/AUTHORS.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    40554 2023-05-04 14:14:49.000000 pydash-7.0.3/CHANGELOG.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.3/CONTRIBUTING.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.3/LICENSE.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.3/MANIFEST.in
--rw-r--r--   0 dgilland   (501) staff       (20)    44029 2023-05-04 14:18:50.327762 pydash-7.0.3/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.3/README.rst
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.317511 pydash-7.0.3/docs/
--rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/Makefile
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.317729 pydash-7.0.3/docs/_static/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.3/docs/_static/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)      137 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/_static/theme_override.css
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.317934 pydash-7.0.3/docs/_templates/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.3/docs/_templates/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/api.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.3/docs/authors.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/callbacks.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.3/docs/chaining.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/changelog.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     5733 2022-09-23 13:07:13.000000 pydash-7.0.3/docs/conf.py
--rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.3/docs/contributing.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/deeppath.rst
--rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.3/docs/devguide.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/differences.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.3/docs/index.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.3/docs/installation.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/kudos.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.3/docs/license.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/quickstart.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/templating.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/upgrading.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.3/docs/versioning.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.3/pylintrc
--rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.3/pyproject.toml
--rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.3/requirements.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     2528 2023-05-04 14:18:50.328144 pydash-7.0.3/setup.cfg
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.278985 pydash-7.0.3/src/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.321462 pydash-7.0.3/src/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)    11148 2023-05-04 14:14:07.000000 pydash-7.0.3/src/pydash/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    69733 2023-05-04 14:12:08.000000 pydash-7.0.3/src/pydash/arrays.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.322716 pydash-7.0.3/src/pydash/chaining/
--rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.3/src/pydash/chaining/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.3/src/pydash/chaining/all_funcs.py
--rw-r--r--   0 dgilland   (501) staff       (20)   123215 2023-05-04 14:12:08.000000 pydash-7.0.3/src/pydash/chaining/all_funcs.pyi
--rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.3/src/pydash/chaining/chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.3/src/pydash/exceptions.py
--rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/helpers.py
--rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.3/src/pydash/predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.3/src/pydash/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)      690 2023-04-27 16:14:56.000000 pydash-7.0.3/src/pydash/types.py
--rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/utilities.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.322059 pydash-7.0.3/src/pydash.egg-info/
--rw-r--r--   0 dgilland   (501) staff       (20)    44029 2023-05-04 14:18:48.000000 pydash-7.0.3/src/pydash.egg-info/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)    16310 2023-05-04 14:18:50.000000 pydash-7.0.3/src/pydash.egg-info/SOURCES.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-05-04 14:18:48.000000 pydash-7.0.3/src/pydash.egg-info/dependency_links.txt
--rw-r--r--   0 dgilland   (501) staff       (20)      293 2023-05-04 14:18:48.000000 pydash-7.0.3/src/pydash.egg-info/requires.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-05-04 14:18:48.000000 pydash-7.0.3/src/pydash.egg-info/top_level.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.3/tasks.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.325235 pydash-7.0.3/tests/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.3/tests/__init__.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.279251 pydash-7.0.3/tests/build/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.325386 pydash-7.0.3/tests/build/testresults/
--rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.3/tests/build/testresults/junit.xml
--rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.3/tests/conftest.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.3/tests/helpers.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.327555 pydash-7.0.3/tests/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.3/tests/pytest_mypy_testing/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    16882 2023-05-04 14:12:08.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.3/tests/test_annotations.py
--rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.3/tests/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.3/tests/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.3/tests/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.3/tests/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.3/tests/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.3/tests/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.3/tests/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.3/tests/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.3/tests/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.3/tox.ini
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.498645 pydash-7.0.4/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446816 pydash-7.0.4/.tox/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.432870 pydash-7.0.4/.tox/.package/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.432916 pydash-7.0.4/.tox/.package/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.432956 pydash-7.0.4/.tox/.package/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.432995 pydash-7.0.4/.tox/.package/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.453302 pydash-7.0.4/.tox/.package/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.4/.tox/.package/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433102 pydash-7.0.4/.tox/.pkg/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433144 pydash-7.0.4/.tox/.pkg/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433184 pydash-7.0.4/.tox/.pkg/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433224 pydash-7.0.4/.tox/.pkg/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.453573 pydash-7.0.4/.tox/.pkg/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.4/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433329 pydash-7.0.4/.tox/3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433371 pydash-7.0.4/.tox/3.11/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433420 pydash-7.0.4/.tox/3.11/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.435972 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.453838 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.453937 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454021 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454109 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454395 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454484 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454581 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454675 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454772 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454872 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454974 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455267 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455367 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455470 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455558 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455643 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.434504 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455743 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456011 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456087 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456165 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456374 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456469 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456709 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456802 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457049 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457129 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457346 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457552 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457633 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457731 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457828 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457926 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458022 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458270 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458348 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458427 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458506 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458588 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458673 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458766 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.436064 pydash-7.0.4/.tox/py310/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.436101 pydash-7.0.4/.tox/py310/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.436138 pydash-7.0.4/.tox/py310/lib/python3.10/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.438506 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458860 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458938 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459028 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459124 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459371 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459455 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459534 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459608 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459689 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459769 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459867 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460099 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460175 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460252 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460332 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460408 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460494 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.437195 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460587 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460844 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460923 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461005 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461205 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461281 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461504 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461596 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461823 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461908 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462128 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462346 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462430 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462510 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462594 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462677 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462767 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463092 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463205 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463313 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463417 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463518 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463791 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463885 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463978 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.438600 pydash-7.0.4/.tox/py311/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.438636 pydash-7.0.4/.tox/py311/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.438672 pydash-7.0.4/.tox/py311/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.441148 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464085 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464183 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464285 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464390 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464671 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464773 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464873 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464965 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465052 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465142 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465225 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465551 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465666 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465777 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465876 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465968 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.439678 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466056 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466334 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466412 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466495 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466764 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466849 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467089 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467173 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467378 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467462 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467716 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467926 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468010 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468159 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468288 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468387 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468491 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468748 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468855 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468944 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469031 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469118 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469206 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469296 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.441270 pydash-7.0.4/.tox/py37/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.441321 pydash-7.0.4/.tox/py37/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.441370 pydash-7.0.4/.tox/py37/lib/python3.7/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443706 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469383 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469467 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469550 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469634 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469869 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469964 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470049 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470135 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470214 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470294 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470545 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470628 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470720 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470825 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470925 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471020 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.442412 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471114 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471349 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471439 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471526 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471775 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471850 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472085 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472178 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472389 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472482 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472680 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472885 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472965 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473044 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443162 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473126 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473208 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473296 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473386 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473624 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473725 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473815 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473908 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474025 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474301 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474417 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443799 pydash-7.0.4/.tox/py38/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443836 pydash-7.0.4/.tox/py38/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443874 pydash-7.0.4/.tox/py38/lib/python3.8/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446715 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474531 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474640 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474746 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474857 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475153 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475254 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475357 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475467 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475571 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475658 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475760 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476049 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476211 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476307 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476419 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476523 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476634 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476740 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.445199 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476849 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477128 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477239 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477358 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477625 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477732 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477990 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478092 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478311 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478412 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478668 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478924 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479028 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479121 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479219 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479307 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479409 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479675 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479781 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479894 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479996 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480106 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480352 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480464 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480578 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446870 pydash-7.0.4/.tox/py39/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446923 pydash-7.0.4/.tox/py39/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446976 pydash-7.0.4/.tox/py39/lib/python3.9/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.450126 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480687 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480796 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480901 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481009 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481270 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481373 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481474 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481572 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481674 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481775 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481877 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482144 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482253 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482358 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482452 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482545 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482636 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.448391 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482745 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483007 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483109 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483209 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483425 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483509 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483704 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483781 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483972 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484065 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484298 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484486 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484562 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484638 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484716 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484829 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484923 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485170 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485257 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485335 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485416 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485510 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485725 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485820 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485898 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/twine/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)     1396 2023-06-02 13:53:01.000000 pydash-7.0.4/AUTHORS.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    40727 2023-06-02 13:50:44.000000 pydash-7.0.4/CHANGELOG.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.4/LICENSE.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.4/MANIFEST.in
+-rw-r--r--   0 dgilland   (501) staff       (20)    44202 2023-06-02 14:03:15.498748 pydash-7.0.4/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.4/README.rst
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.488634 pydash-7.0.4/docs/
+-rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/Makefile
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.488880 pydash-7.0.4/docs/_static/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.4/docs/_static/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)      137 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/_static/theme_override.css
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.489010 pydash-7.0.4/docs/_templates/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.4/docs/_templates/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/api.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.4/docs/authors.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/callbacks.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.4/docs/chaining.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/changelog.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     5733 2022-09-23 13:07:13.000000 pydash-7.0.4/docs/conf.py
+-rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.4/docs/contributing.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/deeppath.rst
+-rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.4/docs/devguide.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/differences.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.4/docs/index.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.4/docs/installation.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/kudos.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.4/docs/license.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/quickstart.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/templating.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/upgrading.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.4/docs/versioning.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.4/pylintrc
+-rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.4/pyproject.toml
+-rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.4/requirements.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     2536 2023-06-02 14:03:15.499134 pydash-7.0.4/setup.cfg
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.450516 pydash-7.0.4/src/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.492402 pydash-7.0.4/src/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)    11148 2023-06-02 13:50:23.000000 pydash-7.0.4/src/pydash/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    69733 2023-05-04 14:12:08.000000 pydash-7.0.4/src/pydash/arrays.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.493676 pydash-7.0.4/src/pydash/chaining/
+-rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.4/src/pydash/chaining/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.4/src/pydash/chaining/all_funcs.py
+-rw-r--r--   0 dgilland   (501) staff       (20)   123215 2023-05-04 14:12:08.000000 pydash-7.0.4/src/pydash/chaining/all_funcs.pyi
+-rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.4/src/pydash/chaining/chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.4/src/pydash/exceptions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/helpers.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.4/src/pydash/predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.4/src/pydash/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      690 2023-04-27 16:14:56.000000 pydash-7.0.4/src/pydash/types.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/utilities.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.492982 pydash-7.0.4/src/pydash.egg-info/
+-rw-r--r--   0 dgilland   (501) staff       (20)    44202 2023-06-02 14:03:13.000000 pydash-7.0.4/src/pydash.egg-info/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)    16310 2023-06-02 14:03:15.000000 pydash-7.0.4/src/pydash.egg-info/SOURCES.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-06-02 14:03:13.000000 pydash-7.0.4/src/pydash.egg-info/dependency_links.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)      301 2023-06-02 14:03:13.000000 pydash-7.0.4/src/pydash.egg-info/requires.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-06-02 14:03:13.000000 pydash-7.0.4/src/pydash.egg-info/top_level.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.4/tasks.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.496277 pydash-7.0.4/tests/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.4/tests/__init__.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.450764 pydash-7.0.4/tests/build/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.496439 pydash-7.0.4/tests/build/testresults/
+-rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.4/tests/build/testresults/junit.xml
+-rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.4/tests/conftest.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.4/tests/helpers.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.498515 pydash-7.0.4/tests/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.4/tests/pytest_mypy_testing/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    16882 2023-05-04 14:12:08.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.4/tests/test_annotations.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.4/tests/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.4/tests/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.4/tests/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.4/tests/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.4/tests/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.4/tests/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.4/tests/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.4/tests/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.4/tests/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.4/tox.ini
```

### Comparing `pydash-7.0.3/AUTHORS.rst` & `pydash-7.0.4/AUTHORS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -21,7 +21,9 @@
 - Frank Epperlein, `efenka@github <https://github.com/efenka>`_
 - Joshua Wilson, `jwilson8767@github <https://github.com/jwilson8767>`_
 - Eli Jose, `elijose55@github <https://github.com/elijose55>`_
 - Gonzalo Naveira, `gonzalonaveira@github <https://github.com/gonzalonaveira>`_
 - Wenbo Zhao, zhaowb@gmail.com, `zhaowb@github <https://github.com/zhaowb>`_
 - Mervyn Lee, `mervynlee94@github <https://github.com/mervynlee94>`_
 - Weineel Lee, `weineel@github <https://github.com/weineel>`_
+- bl4ckst0ne@github `bl4ckst0ne@github <https://github.com/bl4ckst0ne>`_
+- Thomas `DeviousStoat@github <https://github.com/DeviousStoat>`_
```

### Comparing `pydash-7.0.3/CHANGELOG.rst` & `pydash-7.0.4/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.4 (2023-06-02)
+-------------------
+
+- Exclude incompatible ``typing-extensions`` version ``4.6.0`` from install requirements. Incompatibility was fixed in ``4.6.1``.
+
+
 v7.0.3 (2023-05-04)
 -------------------
 
 - Fix typing for ``difference_by``, ``intersection_by``, ``union_by``, ``uniq_by``, and ``xor_by`` by allowing ``iteratee`` argument to be `Any`.  Thanks DeviousStoat_!
 
 
 v7.0.2 (2023-04-27)
```

### Comparing `pydash-7.0.3/CONTRIBUTING.rst` & `pydash-7.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/LICENSE.rst` & `pydash-7.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/PKG-INFO` & `pydash-7.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.3
+Version: 7.0.4
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,20 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.4 (2023-06-02)
+-------------------
+
+- Exclude incompatible ``typing-extensions`` version ``4.6.0`` from install requirements. Incompatibility was fixed in ``4.6.1``.
+
+
 v7.0.3 (2023-05-04)
 -------------------
 
 - Fix typing for ``difference_by``, ``intersection_by``, ``union_by``, ``uniq_by``, and ``xor_by`` by allowing ``iteratee`` argument to be `Any`.  Thanks DeviousStoat_!
 
 
 v7.0.2 (2023-04-27)
```

### Comparing `pydash-7.0.3/README.rst` & `pydash-7.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/Makefile` & `pydash-7.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/api.rst` & `pydash-7.0.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/callbacks.rst` & `pydash-7.0.4/docs/callbacks.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/chaining.rst` & `pydash-7.0.4/docs/chaining.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/conf.py` & `pydash-7.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/deeppath.rst` & `pydash-7.0.4/docs/deeppath.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/differences.rst` & `pydash-7.0.4/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/index.rst` & `pydash-7.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/quickstart.rst` & `pydash-7.0.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/templating.rst` & `pydash-7.0.4/docs/templating.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/docs/upgrading.rst` & `pydash-7.0.4/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/pylintrc` & `pydash-7.0.4/pylintrc`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/setup.cfg` & `pydash-7.0.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 include_package_data = True
 install_requires = 
-	typing-extensions>=3.10
+	typing-extensions>=3.10,!=4.6.0
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	black
```

### Comparing `pydash-7.0.3/src/pydash/__init__.py` & `pydash-7.0.4/src/pydash/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python port of Lo-Dash."""
 
-__version__ = "7.0.3"
+__version__ = "7.0.4"
 
 from .arrays import (
     chunk,
     compact,
     concat,
     difference,
     difference_by,
```

### Comparing `pydash-7.0.3/src/pydash/arrays.py` & `pydash-7.0.4/src/pydash/arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/chaining/all_funcs.py` & `pydash-7.0.4/src/pydash/chaining/all_funcs.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/chaining/all_funcs.pyi` & `pydash-7.0.4/src/pydash/chaining/all_funcs.pyi`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/chaining/chaining.py` & `pydash-7.0.4/src/pydash/chaining/chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/collections.py` & `pydash-7.0.4/src/pydash/collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/functions.py` & `pydash-7.0.4/src/pydash/functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/helpers.py` & `pydash-7.0.4/src/pydash/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/numerical.py` & `pydash-7.0.4/src/pydash/numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/objects.py` & `pydash-7.0.4/src/pydash/objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/predicates.py` & `pydash-7.0.4/src/pydash/predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/strings.py` & `pydash-7.0.4/src/pydash/strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/types.py` & `pydash-7.0.4/src/pydash/types.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash/utilities.py` & `pydash-7.0.4/src/pydash/utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/src/pydash.egg-info/PKG-INFO` & `pydash-7.0.4/src/pydash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.3
+Version: 7.0.4
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,20 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.4 (2023-06-02)
+-------------------
+
+- Exclude incompatible ``typing-extensions`` version ``4.6.0`` from install requirements. Incompatibility was fixed in ``4.6.1``.
+
+
 v7.0.3 (2023-05-04)
 -------------------
 
 - Fix typing for ``difference_by``, ``intersection_by``, ``union_by``, ``uniq_by``, and ``xor_by`` by allowing ``iteratee`` argument to be `Any`.  Thanks DeviousStoat_!
 
 
 v7.0.2 (2023-04-27)
```

### Comparing `pydash-7.0.3/src/pydash.egg-info/SOURCES.txt` & `pydash-7.0.4/src/pydash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tasks.py` & `pydash-7.0.4/tasks.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/build/testresults/junit.xml` & `pydash-7.0.4/tests/build/testresults/junit.xml`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/helpers.py` & `pydash-7.0.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/pytest_mypy_testing/test_arrays.py` & `pydash-7.0.4/tests/pytest_mypy_testing/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/pytest_mypy_testing/test_chaining.py` & `pydash-7.0.4/tests/pytest_mypy_testing/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/pytest_mypy_testing/test_collections.py` & `pydash-7.0.4/tests/pytest_mypy_testing/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/pytest_mypy_testing/test_functions.py` & `pydash-7.0.4/tests/pytest_mypy_testing/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/pytest_mypy_testing/test_numerical.py` & `pydash-7.0.4/tests/pytest_mypy_testing/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/pytest_mypy_testing/test_objects.py` & `pydash-7.0.4/tests/pytest_mypy_testing/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/pytest_mypy_testing/test_predicates.py` & `pydash-7.0.4/tests/pytest_mypy_testing/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/pytest_mypy_testing/test_strings.py` & `pydash-7.0.4/tests/pytest_mypy_testing/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/pytest_mypy_testing/test_utilities.py` & `pydash-7.0.4/tests/pytest_mypy_testing/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/test_arrays.py` & `pydash-7.0.4/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/test_chaining.py` & `pydash-7.0.4/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/test_collections.py` & `pydash-7.0.4/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/test_functions.py` & `pydash-7.0.4/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/test_numerical.py` & `pydash-7.0.4/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/test_objects.py` & `pydash-7.0.4/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/test_predicates.py` & `pydash-7.0.4/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/test_strings.py` & `pydash-7.0.4/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.3/tests/test_utilities.py` & `pydash-7.0.4/tests/test_utilities.py`

 * *Files identical despite different names*

