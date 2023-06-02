# Comparing `tmp/greatday-1.0.0.tar.gz` & `tmp/greatday-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatday-1.0.0.tar", last modified: Wed Jun  8 16:31:04 2022, max compression
+gzip compressed data, was "greatday-1.1.0.tar", last modified: Fri Jun  2 02:20:59 2023, max compression
```

## Comparing `greatday-1.0.0.tar` & `greatday-1.1.0.tar`

### file list

```diff
@@ -1,117 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.557731 greatday-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-06-08 16:30:33.000000 greatday-1.0.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-06-08 16:30:33.000000 greatday-1.0.0/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-06-08 16:30:33.000000 greatday-1.0.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 16:30:33.000000 greatday-1.0.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.533729 greatday-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.537730 greatday-1.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.537730 greatday-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-06-08 16:30:33.000000 greatday-1.0.0/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-06-08 16:30:33.000000 greatday-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-08 16:30:33.000000 greatday-1.0.0/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8952 2022-06-08 16:30:33.000000 greatday-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-06-08 16:30:33.000000 greatday-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-06-08 16:30:33.000000 greatday-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-06-08 16:30:33.000000 greatday-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     9769 2022-06-08 16:30:33.000000 greatday-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-06-08 16:30:33.000000 greatday-1.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-06-08 16:30:33.000000 greatday-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     8362 2022-06-08 16:31:04.557731 greatday-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7669 2022-06-08 16:30:33.000000 greatday-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.537730 greatday-1.0.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1245 2022-06-08 16:30:33.000000 greatday-1.0.0/bin/check_cc
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-06-08 16:30:33.000000 greatday-1.0.0/bin/file_repo_to_sql_repo.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1158 2022-06-08 16:30:33.000000 greatday-1.0.0/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (121)      681 2022-06-08 16:30:33.000000 greatday-1.0.0/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (121)     3403 2022-06-08 16:30:33.000000 greatday-1.0.0/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-06-08 16:30:33.000000 greatday-1.0.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.537730 greatday-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/GreatLang.ebnf
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.541730 greatday-1.0.0/docs/design/
--rw-r--r--   0 runner    (1001) docker     (121)    17217 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/design/design-1.svg
--rw-r--r--   0 runner    (1001) docker     (121)    15974 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/design/design-2.svg
--rw-r--r--   0 runner    (1001) docker     (121)    19850 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/design/design-3.svg
--rw-r--r--   0 runner    (1001) docker     (121)    23241 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/design/design-4.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (121)     6432 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.545730 greatday-1.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.545730 greatday-1.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.545730 greatday-1.0.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/greatday.cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/greatday.db.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/greatday.models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/greatday.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/greatday.types.rst
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-08 16:30:33.000000 greatday-1.0.0/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 16:30:33.000000 greatday-1.0.0/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.545730 greatday-1.0.0/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     7833 2022-06-08 16:30:33.000000 greatday-1.0.0/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-06-08 16:30:33.000000 greatday-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-06-08 16:30:33.000000 greatday-1.0.0/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (121)     6401 2022-06-08 16:30:33.000000 greatday-1.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-06-08 16:30:33.000000 greatday-1.0.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-06-08 16:30:33.000000 greatday-1.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.545730 greatday-1.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-08 16:30:33.000000 greatday-1.0.0/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-06-08 16:31:04.557731 greatday-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-06-08 16:30:33.000000 greatday-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.525729 greatday-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.549730 greatday-1.0.0/src/greatday/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2455 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5399 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_dates.py
--rw-r--r--   0 runner    (1001) docker     (121)    14537 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_runners.py
--rw-r--r--   0 runner    (1001) docker     (121)     6197 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_session.py
--rw-r--r--   0 runner    (1001) docker     (121)    10252 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_spells.py
--rw-r--r--   0 runner    (1001) docker     (121)    10655 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     5075 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_todo.py
--rw-r--r--   0 runner    (1001) docker     (121)    12964 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/_tui.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/models.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-06-08 16:30:33.000000 greatday-1.0.0/src/greatday/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.553731 greatday-1.0.0/src/greatday.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8362 2022-06-08 16:31:04.000000 greatday-1.0.0/src/greatday.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-06-08 16:31:04.000000 greatday-1.0.0/src/greatday.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 16:31:04.000000 greatday-1.0.0/src/greatday.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-06-08 16:31:04.000000 greatday-1.0.0/src/greatday.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 16:30:47.000000 greatday-1.0.0/src/greatday.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-06-08 16:31:04.000000 greatday-1.0.0/src/greatday.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-08 16:31:04.000000 greatday-1.0.0/src/greatday.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6189 2022-06-08 16:30:33.000000 greatday-1.0.0/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 16:31:04.557731 greatday-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-08 16:30:33.000000 greatday-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-06-08 16:30:33.000000 greatday-1.0.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-06-08 16:30:33.000000 greatday-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-06-08 16:30:33.000000 greatday-1.0.0/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-06-08 16:30:33.000000 greatday-1.0.0/tests/test_file_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-06-08 16:30:33.000000 greatday-1.0.0/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-06-08 16:30:33.000000 greatday-1.0.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-06-08 16:30:33.000000 greatday-1.0.0/tests/test_spells.py
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-06-08 16:30:33.000000 greatday-1.0.0/tests/test_sql_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-06-08 16:30:33.000000 greatday-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.037448 greatday-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-02 02:20:36.000000 greatday-1.1.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-02 02:20:36.000000 greatday-1.1.0/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-02 02:20:36.000000 greatday-1.1.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:36.000000 greatday-1.1.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.025448 greatday-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.029448 greatday-1.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.029448 greatday-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-02 02:20:36.000000 greatday-1.1.0/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-02 02:20:36.000000 greatday-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 02:20:36.000000 greatday-1.1.0/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-06-02 02:20:36.000000 greatday-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-02 02:20:36.000000 greatday-1.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-02 02:20:36.000000 greatday-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-02 02:20:36.000000 greatday-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-02 02:20:36.000000 greatday-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-02 02:20:36.000000 greatday-1.1.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-02 02:20:36.000000 greatday-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-02 02:20:59.041448 greatday-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-02 02:20:36.000000 greatday-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.029448 greatday-1.1.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1245 2023-06-02 02:20:36.000000 greatday-1.1.0/bin/check_cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-02 02:20:36.000000 greatday-1.1.0/bin/file_repo_to_sql_repo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-06-02 02:20:36.000000 greatday-1.1.0/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-06-02 02:20:36.000000 greatday-1.1.0/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3403 2023-06-02 02:20:36.000000 greatday-1.1.0/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 02:20:36.000000 greatday-1.1.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.029448 greatday-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/GreatLang.ebnf
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.033448 greatday-1.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.033448 greatday-1.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.033448 greatday-1.1.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.common.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.dates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.db.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.runners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.session.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.spells.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.tag.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.todo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.tui.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/greatday.types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 02:20:36.000000 greatday-1.1.0/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:36.000000 greatday-1.1.0/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.033448 greatday-1.1.0/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-02 02:20:36.000000 greatday-1.1.0/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-02 02:20:36.000000 greatday-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-02 02:20:36.000000 greatday-1.1.0/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-02 02:20:36.000000 greatday-1.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-02 02:20:36.000000 greatday-1.1.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-02 02:20:36.000000 greatday-1.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.033448 greatday-1.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-02 02:20:36.000000 greatday-1.1.0/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-02 02:20:59.041448 greatday-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-02 02:20:36.000000 greatday-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.025448 greatday-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.037448 greatday-1.1.0/src/greatday/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12697 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/spells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/todo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/tui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-02 02:20:36.000000 greatday-1.1.0/src/greatday/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.037448 greatday-1.1.0/src/greatday.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-02 02:20:58.000000 greatday-1.1.0/src/greatday.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-02 02:20:59.000000 greatday-1.1.0/src/greatday.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:20:58.000000 greatday-1.1.0/src/greatday.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 02:20:58.000000 greatday-1.1.0/src/greatday.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:20:47.000000 greatday-1.1.0/src/greatday.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 02:20:58.000000 greatday-1.1.0/src/greatday.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 02:20:58.000000 greatday-1.1.0/src/greatday.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-02 02:20:36.000000 greatday-1.1.0/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:20:59.037448 greatday-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 02:20:36.000000 greatday-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-02 02:20:36.000000 greatday-1.1.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-02 02:20:36.000000 greatday-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-02 02:20:36.000000 greatday-1.1.0/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-02 02:20:36.000000 greatday-1.1.0/tests/test_file_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-02 02:20:36.000000 greatday-1.1.0/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-02 02:20:36.000000 greatday-1.1.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-02 02:20:36.000000 greatday-1.1.0/tests/test_spells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-02 02:20:36.000000 greatday-1.1.0/tests/test_sql_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-02 02:20:36.000000 greatday-1.1.0/tox.ini
```

### Comparing `greatday-1.0.0/.cruft.json` & `greatday-1.1.0/.cruft.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'0e7235f0fd512a44d9a9c423183aa15fb7c3c2c9'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "4e0a8f622f41f01ab28a11d155a6706761a62165",
+    "commit": "0e7235f0fd512a44d9a9c423183aa15fb7c3c2c9",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/python-boltons/cc-python",
             "author": "Bryan M Bugyi",
             "email": "bryanbugyi34@gmail.com",
             "git_org_name": "bbugyi200",
             "git_repo_name": "greatday",
```

### Comparing `greatday-1.0.0/.github/labels.yml` & `greatday-1.1.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/.github/workflows/ci.yml` & `greatday-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/.gitignore` & `greatday-1.1.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -114,9 +114,12 @@
 
 # Project docker switch file
 .lcldev
 
 # git conflict files
 *.rej
 
+# pyright config file
+pyrightconfig.json
+
 # local sqlite databases
 *.db
```

### Comparing `greatday-1.0.0/.pylintrc` & `greatday-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/CHANGELOG.md` & `greatday-1.1.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,27 @@
 
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
+## [Unreleased](https://github.com/bbugyi200/greatday/compare/1.1.0...HEAD)
 
-## [Unreleased](https://github.com/bbugyi200/greatday/compare/1.0.0...HEAD)
+Not much to talk about yet...
 
-No notable changes have been made.
+## [1.1.0](https://github.com/bbugyi200/greatday/compare/1.1.0...1.0.0)
+
+### Added
+
+* New `default_query_group` configuration option for 'tui` CLI command.
+
+### Miscellaneous
+
+* Lots of other stuff probably...
 
 
 ## [1.0.0](https://github.com/bbugyi200/greatday/compare/0.4.0...1.0.0) - 2022-06-08
 
 ### Changed
 
 * Multiple significant optimizations (e.g. caching `GreatTag.from_line()` calls).
```

### Comparing `greatday-1.0.0/CONTRIBUTING.md` & `greatday-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/Dockerfile` & `greatday-1.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/Makefile` & `greatday-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/PKG-INFO` & `greatday-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: greatday
-Version: 1.0.0
+Version: 1.1.0
 Summary: Don't have a good day. Have a great day.
 Home-page: https://github.com/bbugyi200/greatday
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -117,76 +116,22 @@
                         This is the default command.
 ```
 <!-- [[[[[end]]]]] -->
 
 <!-- [[[[[kooky.cog
 from pathlib import Path
 
-lines = Path("./docs/design/design.md").read_text().split("\n")
-if any(L.strip() for L in lines):
-    fixed_lines = [L.replace("(.", "(./docs/design") if L.startswith("![") else L for L in lines]
-    print("## Design Diagrams\n")
-    print("\n".join(fixed_lines))
+design_md = Path("./docs/design/design.md")
+if design_md.exists():
+    lines = design_md.read_text().split("\n")
+    if any(L.strip() for L in lines):
+        fixed_lines = [L.replace("(.", "(./docs/design") if L.startswith("![") else L for L in lines]
+        print("## Design Diagrams\n")
+        print("\n".join(fixed_lines))
 ]]]]] -->
-## Design Diagrams
-
-### State Diagrams
-
-#### State Diagram for the `greatday start` Command
-
-The below state diagram is kicked off when a user runs the `greatday start`
-command.
-
-Keep in mind the following notes while reviewing this diagram:
-
-* We assume that it has been `N` days since your tickler Todos were last processed.
-
-![diagram](./docs/design/design-1.svg)
-
-#### State Diagram for Processing Todos
-
-![diagram](./docs/design/design-2.svg)
-
-### Class Diagrams
-
-This section contains class diagrams used to help design / document greatday.
-
-#### Class Diagram for `Todo` Classes
-
-The following diagram illustrates how the various [magodo] `Todo` classes
-interact.
-
-Keep in mind the following notes while reviewing this diagram:
-
-* The type variable `Self` is implicit and is always bound by the current class.
-* The type variable `T` is bound by the `AbstractTodo` protocol.
-
-![diagram](./docs/design/design-3.svg)
-
-#### Class Diagram for `Repo` and `UnitOfWork` Classes
-
-The following diagram illustrates how the various [potoroo] `Repo` and `UnitOfWork`
-classes interact.
-
-Keep in mind the following notes while reviewing this diagram:
-
-* `V_or_None` is meant to be `Optional[V]`. There seems to be a bug in
-  [mermaid], however, that prevents us from using `Optional[V]` as a generic
-  type.
-* Similarly, `VList` is meant to be `List[V]`.
-* The type variable `Self` is implicit and is always bound by the current class.
-* The type variable `R` is bound by the `BasicRepo` class.
-* The type variables `K`, `V`, and `T` are all unbound.
-
-![diagram](./docs/design/design-4.svg)
-
-[magodo]: https://github.com/bbugyi200/magodo
-[potoroo]: https://github.com/bbugyi200/potoroo
-[mermaid]: https://github.com/mermaid-js/mermaid
-
 <!-- [[[[[end]]]]] -->
 
 
 ## Useful Links 🔗
 
 * [API Reference][3]: A developer's reference of the API exposed by this
   project.
@@ -210,9 +155,7 @@
 [7]: https://github.com/bbugyi200/greatday/blob/master/CONTRIBUTING.md
 [8]: https://github.com/bbugyi200/greatday
 [9]: https://pip.pypa.io
 [10]: http://docs.python-guide.org/en/latest/starting/installation/
 [11]: https://github.com/pypa/pipx
 [12]: https://github.com/cruft/cruft
 [13]: https://github.com/bbugyi200/greatday/issues/new/choose
-
-
```

### Comparing `greatday-1.0.0/README.md` & `greatday-1.1.0/src/greatday.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: greatday
+Version: 1.1.0
+Summary: Don't have a good day. Have a great day.
+Home-page: https://github.com/bbugyi200/greatday
+Author: Bryan M Bugyi
+Author-email: bryanbugyi34@gmail.com
+License: MIT license
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # greatday
 
 **Don't have a good day. Have a great day.**
 
 _project status badges:_
 
 [![CI Workflow](https://github.com/bbugyi200/greatday/actions/workflows/ci.yml/badge.svg)](https://github.com/bbugyi200/greatday/actions/workflows/ci.yml)
@@ -97,76 +116,22 @@
                         This is the default command.
 ```
 <!-- [[[[[end]]]]] -->
 
 <!-- [[[[[kooky.cog
 from pathlib import Path
 
-lines = Path("./docs/design/design.md").read_text().split("\n")
-if any(L.strip() for L in lines):
-    fixed_lines = [L.replace("(.", "(./docs/design") if L.startswith("![") else L for L in lines]
-    print("## Design Diagrams\n")
-    print("\n".join(fixed_lines))
+design_md = Path("./docs/design/design.md")
+if design_md.exists():
+    lines = design_md.read_text().split("\n")
+    if any(L.strip() for L in lines):
+        fixed_lines = [L.replace("(.", "(./docs/design") if L.startswith("![") else L for L in lines]
+        print("## Design Diagrams\n")
+        print("\n".join(fixed_lines))
 ]]]]] -->
-## Design Diagrams
-
-### State Diagrams
-
-#### State Diagram for the `greatday start` Command
-
-The below state diagram is kicked off when a user runs the `greatday start`
-command.
-
-Keep in mind the following notes while reviewing this diagram:
-
-* We assume that it has been `N` days since your tickler Todos were last processed.
-
-![diagram](./docs/design/design-1.svg)
-
-#### State Diagram for Processing Todos
-
-![diagram](./docs/design/design-2.svg)
-
-### Class Diagrams
-
-This section contains class diagrams used to help design / document greatday.
-
-#### Class Diagram for `Todo` Classes
-
-The following diagram illustrates how the various [magodo] `Todo` classes
-interact.
-
-Keep in mind the following notes while reviewing this diagram:
-
-* The type variable `Self` is implicit and is always bound by the current class.
-* The type variable `T` is bound by the `AbstractTodo` protocol.
-
-![diagram](./docs/design/design-3.svg)
-
-#### Class Diagram for `Repo` and `UnitOfWork` Classes
-
-The following diagram illustrates how the various [potoroo] `Repo` and `UnitOfWork`
-classes interact.
-
-Keep in mind the following notes while reviewing this diagram:
-
-* `V_or_None` is meant to be `Optional[V]`. There seems to be a bug in
-  [mermaid], however, that prevents us from using `Optional[V]` as a generic
-  type.
-* Similarly, `VList` is meant to be `List[V]`.
-* The type variable `Self` is implicit and is always bound by the current class.
-* The type variable `R` is bound by the `BasicRepo` class.
-* The type variables `K`, `V`, and `T` are all unbound.
-
-![diagram](./docs/design/design-4.svg)
-
-[magodo]: https://github.com/bbugyi200/magodo
-[potoroo]: https://github.com/bbugyi200/potoroo
-[mermaid]: https://github.com/mermaid-js/mermaid
-
 <!-- [[[[[end]]]]] -->
 
 
 ## Useful Links 🔗
 
 * [API Reference][3]: A developer's reference of the API exposed by this
   project.
```

### Comparing `greatday-1.0.0/bin/check_cc` & `greatday-1.1.0/bin/check_cc`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/bin/file_repo_to_sql_repo.py` & `greatday-1.1.0/bin/file_repo_to_sql_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This script migrates all greatday todos from text files to SQLite DB."""
 
 from __future__ import annotations
 
 import sys
 
-from greatday._common import drop_word_if_startswith
-from greatday._repo import FileRepo, SQLRepo
+from greatday.common import drop_word_if_startswith
+from greatday.repo import FileRepo, SQLRepo
 
 
 def main() -> int:
     """Main entry point for this script."""
     if len(sys.argv) != 3:
         print(
             "usage: file_repo_to_sql_repo DATA_DIR SQLITEDB", file=sys.stderr
```

### Comparing `greatday-1.0.0/bin/publish_docs` & `greatday-1.1.0/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/bin/quick-lints` & `greatday-1.1.0/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/bin/render_all_cogs` & `greatday-1.1.0/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/docs/GreatLang.ebnf` & `greatday-1.1.0/docs/GreatLang.ebnf`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/docs/Makefile` & `greatday-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/docs/make.bat` & `greatday-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/docs/source/conf.py` & `greatday-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/lib/bugyi.sh` & `greatday-1.1.0/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/requirements-dev.in` & `greatday-1.1.0/requirements-dev.in`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 ### Tests
 freezegun
 pytest
 pytest-cov
 pytest-mock
 syrupy
-tox
+tox < 4  # workaround for github.com/tox-dev/tox-pyenv/issues/21
 tox-pyenv
 -e file:.#egg=greatday>=0.dev
 
 ### Lint
 black
 cogapp ~= 3.3
 flake8
 isort
-mypy != 0.920, != 0.921, != 0.930  # workaround for https://github.com/samuelcolvin/pydantic/pull/3175
+mypy != 0.920, != 0.921, != 0.930  # workaround for github.com/samuelcolvin/pydantic/pull/3175
 pydocstyle[toml]
 pylint
 
 ### TYPES
 types-python-dateutil
 
 ### Docs
-m2r2
+m2r2 != 0.3.3.*  # since this version requires docutils>=0.19 (see github.com/CrossNox/m2r2/compare/v0.3.2...v0.3.3)
 sphinx ~= 4.3.1  # ATTOW, 'sphinx>=4.4.0' requires a 'importlib-metadata' version that conflicts with what 'cruft' requires.
 sphinx-rtd-theme
 sphinx-autodoc-typehints ~= 1.17.1  # since >=1.18 requires sphinx >=4.5
 
 ### Misc
 bump2version
 cruft[pyproject]
```

### Comparing `greatday-1.0.0/requirements-dev.txt` & `greatday-1.1.0/requirements-dev.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    "make update-requirements"
 #
 -e file:.#egg=greatday>=0.dev
     # via -r requirements-dev.in
-alabaster==0.7.12
+aiohttp==3.8.4
+    # via textual
+aiosignal==1.3.1
+    # via aiohttp
+alabaster==0.7.13
     # via sphinx
-arrow==1.2.2
+arrow==1.2.3
     # via jinja2-time
-astroid==2.11.5
+astroid==2.15.4
     # via pylint
-attrs==21.4.0
-    # via pytest
-babel==2.10.1
+async-timeout==4.0.2
+    # via aiohttp
+attrs==23.1.0
+    # via aiohttp
+babel==2.12.1
     # via sphinx
 binaryornot==0.4.4
     # via cookiecutter
-black==22.3.0
+black==23.3.0
     # via -r requirements-dev.in
 bolton-clack==0.3.4
     # via
     #   -r requirements.in
     #   greatday
 bolton-eris==0.2.3
     # via
@@ -52,294 +58,322 @@
     # via
     #   -r requirements.in
     #   bolton-clack
     #   bolton-eris
     #   greatday
     #   magodo
     #   vimala
+build==0.10.0
+    # via pip-tools
 bump2version==1.0.1
     # via -r requirements-dev.in
-certifi==2022.5.18.1
+certifi==2023.5.7
     # via requests
-chardet==4.0.0
+chardet==5.1.0
     # via binaryornot
-charset-normalizer==2.0.12
-    # via requests
+charset-normalizer==3.1.0
+    # via
+    #   aiohttp
+    #   requests
 click==8.1.3
     # via
     #   black
     #   cookiecutter
     #   cruft
     #   pip-tools
+    #   textual
     #   typer
 cogapp==3.3.0
     # via -r requirements-dev.in
-colored==1.4.3
+colored==1.4.4
     # via syrupy
-commonmark==0.9.1
-    # via rich
-cookiecutter==1.7.3
+cookiecutter==2.1.1
     # via cruft
-coverage[toml]==6.4.1
+coverage[toml]==7.2.5
     # via pytest-cov
-cruft[pyproject]==2.10.2
+cruft[pyproject]==2.15.0
     # via -r requirements-dev.in
-dill==0.3.5.1
+dill==0.3.6
     # via pylint
-distlib==0.3.4
+distlib==0.3.6
     # via virtualenv
 docutils==0.17.1
     # via
     #   m2r2
     #   sphinx
     #   sphinx-rtd-theme
-filelock==3.7.1
+exceptiongroup==1.1.1
+    # via pytest
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
-flake8==4.0.1
+flake8==6.0.0
     # via -r requirements-dev.in
-freezegun==1.2.1
+freezegun==1.2.2
     # via -r requirements-dev.in
-gitdb==4.0.9
+frozenlist==1.3.3
+    # via
+    #   aiohttp
+    #   aiosignal
+gitdb==4.0.10
     # via gitpython
-gitpython==3.1.27
+gitpython==3.1.31
     # via cruft
-greenlet==1.1.2
+greenlet==2.0.2
     # via sqlalchemy
-idna==3.3
-    # via requests
-imagesize==1.3.0
+idna==3.4
+    # via
+    #   requests
+    #   yarl
+imagesize==1.4.1
     # via sphinx
-iniconfig==1.1.1
+importlib-metadata==6.6.0
+    # via textual
+iniconfig==2.0.0
     # via pytest
-isort==5.10.1
+isort==5.12.0
     # via
     #   -r requirements-dev.in
     #   pylint
 jinja2==3.1.2
     # via
     #   cookiecutter
     #   jinja2-time
     #   sphinx
 jinja2-time==0.2.0
     # via cookiecutter
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
     # via astroid
+linkify-it-py==2.0.2
+    # via markdown-it-py
 m2r2==0.3.2
     # via -r requirements-dev.in
-magodo==1.1.0
+magodo==1.1.1
     # via
     #   -r requirements.in
     #   greatday
-markupsafe==2.1.1
+markdown-it-py[linkify,plugins]==2.2.0
+    # via
+    #   mdit-py-plugins
+    #   rich
+    #   textual
+markupsafe==2.1.2
     # via jinja2
-mccabe==0.6.1
+mccabe==0.7.0
     # via
     #   flake8
     #   pylint
+mdit-py-plugins==0.3.5
+    # via markdown-it-py
+mdurl==0.1.2
+    # via markdown-it-py
 mistune==0.8.4
     # via m2r2
-mypy==0.961
+msgpack==1.0.5
+    # via textual
+multidict==6.0.4
+    # via
+    #   aiohttp
+    #   yarl
+mypy==1.3.0
     # via -r requirements-dev.in
-mypy-extensions==0.4.3
+mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==21.3
+packaging==23.1
     # via
+    #   black
+    #   build
     #   pytest
     #   setuptools-scm
     #   sphinx
     #   tox
-pathspec==0.9.0
+pathspec==0.11.1
     # via black
-pep517==0.12.0
-    # via pip-tools
-pip-tools==6.6.2
+pip-tools==6.13.0
     # via -r requirements-dev.in
-platformdirs==2.5.2
+platformdirs==3.5.1
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 potoroo==0.4.1
     # via
     #   -r requirements.in
     #   greatday
-poyo==0.5.0
-    # via cookiecutter
 py==1.11.0
-    # via
-    #   pytest
-    #   tox
-pycodestyle==2.8.0
+    # via tox
+pycodestyle==2.10.0
     # via flake8
-pydantic==1.9.1
+pydantic==1.10.7
     # via
     #   bolton-clack
     #   sqlmodel
-pydocstyle[toml]==6.1.1
+pydocstyle[toml]==6.3.0
     # via -r requirements-dev.in
-pyflakes==2.4.0
+pyflakes==3.0.1
     # via flake8
-pygments==2.12.0
+pygments==2.15.1
     # via
     #   rich
     #   sphinx
-pylint==2.14.1
+pylint==2.17.4
     # via -r requirements-dev.in
-pyparsing==3.0.9
-    # via packaging
-pytest==7.1.2
+pyproject-hooks==1.0.0
+    # via build
+pytest==7.3.1
     # via
     #   -r requirements-dev.in
     #   pytest-cov
     #   pytest-mock
     #   syrupy
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via -r requirements-dev.in
-pytest-mock==3.7.0
+pytest-mock==3.10.0
     # via -r requirements-dev.in
 python-dateutil==2.8.2
     # via
     #   -r requirements.in
     #   freezegun
     #   greatday
-python-slugify==6.1.2
+python-slugify==8.0.1
     # via cookiecutter
-pytz==2022.1
+pytz==2023.3
     # via babel
 pyyaml==6.0
-    # via bolton-clack
-requests==2.27.1
     # via
+    #   bolton-clack
     #   cookiecutter
-    #   sphinx
-rich==12.4.4
+requests==2.30.0
     # via
-    #   -r requirements.in
-    #   greatday
-    #   textual
-setuptools-scm==6.4.2
+    #   cookiecutter
+    #   sphinx
+rich==13.3.5
+    # via textual
+setuptools-scm==7.1.0
     # via -r requirements-dev.in
 six==1.16.0
     # via
-    #   cookiecutter
     #   python-dateutil
     #   tox
-    #   virtualenv
 smmap==5.0.0
     # via gitdb
 snowballstemmer==2.2.0
     # via
     #   pydocstyle
     #   sphinx
 sphinx==4.3.2
     # via
     #   -r requirements-dev.in
     #   sphinx-autodoc-typehints
     #   sphinx-rtd-theme
+    #   sphinxcontrib-jquery
 sphinx-autodoc-typehints==1.17.1
     # via -r requirements-dev.in
-sphinx-rtd-theme==1.0.0
+sphinx-rtd-theme==1.2.0
     # via -r requirements-dev.in
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
+sphinxcontrib-jquery==4.1
+    # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 sqlalchemy==1.4.35
     # via
     #   -r requirements.in
     #   greatday
     #   sqlmodel
-sqlalchemy2-stubs==0.0.2a23
+sqlalchemy2-stubs==0.0.2a34
     # via sqlmodel
-sqlmodel==0.0.6
+sqlmodel==0.0.8
     # via
     #   -r requirements.in
     #   greatday
-structlog==21.5.0
+structlog==23.1.0
     # via bolton-logrus
-syrupy==2.3.0
+syrupy==4.0.2
     # via -r requirements-dev.in
 text-unidecode==1.3
     # via python-slugify
-textual==0.1.18
-    # via
-    #   -r requirements.in
-    #   greatday
-    #   textual-inputs
-textual-inputs==0.2.5
+textual[dev]==0.24.1
     # via
     #   -r requirements.in
     #   greatday
 toml==0.10.2
-    # via
-    #   cruft
-    #   pydocstyle
-    #   tox
+    # via cruft
 tomli==2.0.1
     # via
     #   black
+    #   build
     #   coverage
     #   mypy
-    #   pep517
+    #   pydocstyle
     #   pylint
+    #   pyproject-hooks
     #   pytest
     #   setuptools-scm
-tomlkit==0.11.0
+    #   tox
+tomlkit==0.11.8
     # via pylint
-tox==3.25.0
+tox==3.28.0
     # via
     #   -r requirements-dev.in
     #   tox-pyenv
 tox-pyenv==1.1.0
     # via -r requirements-dev.in
-typer==0.4.1
+typer==0.9.0
     # via cruft
-types-python-dateutil==2.8.17
+types-python-dateutil==2.8.19.13
     # via -r requirements-dev.in
-typing-extensions==4.2.0
+typing-extensions==4.5.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pylint
     #   rich
+    #   setuptools-scm
     #   sqlalchemy2-stubs
     #   textual
-urllib3==1.26.9
+    #   typer
+uc-micro-py==1.0.2
+    # via linkify-it-py
+urllib3==2.0.2
     # via requests
 vimala==0.1.2
     # via
     #   -r requirements.in
     #   greatday
-virtualenv==20.14.1
+virtualenv==20.23.0
     # via tox
-wheel==0.37.1
+wheel==0.40.0
     # via pip-tools
-wrapt==1.14.1
+wrapt==1.15.0
     # via astroid
+yarl==1.9.2
+    # via aiohttp
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==22.1.2
+pip==23.1.2
     # via pip-tools
-setuptools==62.3.3
+setuptools==67.7.2
     # via
-    #   astroid
     #   pip-tools
     #   setuptools-scm
     #   sphinx
```

### Comparing `greatday-1.0.0/requirements.txt` & `greatday-1.1.0/requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    "make update-requirements"
 #
+aiohttp==3.8.4
+    # via textual
+aiosignal==1.3.1
+    # via aiohttp
+async-timeout==4.0.2
+    # via aiohttp
+attrs==23.1.0
+    # via aiohttp
 bolton-clack==0.3.4
     # via -r requirements.in
 bolton-eris==0.2.3
     # via
     #   -r requirements.in
     #   bolton-clack
     #   bolton-proctor
@@ -30,55 +38,82 @@
 bolton-typist==0.2.0
     # via
     #   -r requirements.in
     #   bolton-clack
     #   bolton-eris
     #   magodo
     #   vimala
-commonmark==0.9.1
-    # via rich
-greenlet==1.1.2
+charset-normalizer==3.1.0
+    # via aiohttp
+click==8.1.3
+    # via textual
+frozenlist==1.3.3
+    # via
+    #   aiohttp
+    #   aiosignal
+greenlet==2.0.2
     # via sqlalchemy
-magodo==1.1.0
+idna==3.4
+    # via yarl
+importlib-metadata==6.6.0
+    # via textual
+linkify-it-py==2.0.2
+    # via markdown-it-py
+magodo==1.1.1
     # via -r requirements.in
+markdown-it-py[linkify,plugins]==2.2.0
+    # via
+    #   mdit-py-plugins
+    #   rich
+    #   textual
+mdit-py-plugins==0.3.5
+    # via markdown-it-py
+mdurl==0.1.2
+    # via markdown-it-py
+msgpack==1.0.5
+    # via textual
+multidict==6.0.4
+    # via
+    #   aiohttp
+    #   yarl
 potoroo==0.4.1
     # via -r requirements.in
-pydantic==1.9.1
+pydantic==1.10.7
     # via
     #   bolton-clack
     #   sqlmodel
-pygments==2.12.0
+pygments==2.15.1
     # via rich
 python-dateutil==2.8.2
     # via -r requirements.in
 pyyaml==6.0
     # via bolton-clack
-rich==12.4.4
-    # via
-    #   -r requirements.in
-    #   textual
+rich==13.3.5
+    # via textual
 six==1.16.0
     # via python-dateutil
 sqlalchemy==1.4.35
     # via
     #   -r requirements.in
     #   sqlmodel
-sqlalchemy2-stubs==0.0.2a23
+sqlalchemy2-stubs==0.0.2a34
     # via sqlmodel
-sqlmodel==0.0.6
+sqlmodel==0.0.8
     # via -r requirements.in
-structlog==21.5.0
+structlog==23.1.0
     # via bolton-logrus
-textual==0.1.18
-    # via
-    #   -r requirements.in
-    #   textual-inputs
-textual-inputs==0.2.5
+textual[dev]==0.24.1
     # via -r requirements.in
-typing-extensions==4.2.0
+typing-extensions==4.5.0
     # via
     #   pydantic
     #   rich
     #   sqlalchemy2-stubs
     #   textual
+uc-micro-py==1.0.2
+    # via linkify-it-py
 vimala==0.1.2
     # via -r requirements.in
+yarl==1.9.2
+    # via aiohttp
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `greatday-1.0.0/setup.cfg` & `greatday-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/setup.py` & `greatday-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ###############################################################################
 DESCRIPTION = "Don't have a good day. Have a great day."
 SUPPORTED_PYTHON_VERSIONS = [
     (3, 8),
     (3, 9),
     (3, 10),
 ]
-USE_SCM_VERSION = {"fallback_version": "1.0.0"}
+USE_SCM_VERSION = {"fallback_version": "1.1.0"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `greatday-1.0.0/src/greatday/_common.py` & `greatday-1.1.0/src/greatday/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from typing import Callable, Final, List, cast
 
 from magodo.types import Priority
 from typist import literal_to_list
 
 
 # special contexts
-CTX_FIRST: Final = "FIRST"
 CTX_INBOX: Final = "INBOX"
-CTX_LAST: Final = "LAST"
 
 # special ID type (assigned when no real ID exists)
 NULL_ID: Final = "null"
 
 # all valid todo lines must start with one of...
 TODO_PREFIXES: Final = ("x ", "x:", "o ")
```

### Comparing `greatday-1.0.0/src/greatday/_config.py` & `greatday-1.1.0/src/greatday/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from typing import Any, Literal, Optional, Sequence
 
 import clack
 from clack import xdg
 
 from . import APP_NAME
-from .types import YesNoDefault
+from .types import SavedQueryGroupMap, YesNoDefault
 
 
 Command = Literal["add", "list", "tui"]
 
 DEFAULT_DATA_DIR = xdg.get_full_dir("data", APP_NAME)
 
 
@@ -50,14 +50,18 @@
 
 
 class TUIConfig(Config):
     """Config for the 'tui' subcommand."""
 
     command: Literal["tui"]
 
+    # ----- CONFIG
+    default_query_group: str
+    saved_query_groups: SavedQueryGroupMap = {}
+
 
 def clack_parser(argv: Sequence[str]) -> dict[str, Any]:
     """Parser we pass to the `main_factory()` `parser` kwarg."""
     # HACK: Make 'tui' the default sub-command.
     if not list(it.dropwhile(lambda x: x.startswith("-"), argv[1:])):
         argv = list(argv) + ["tui"]
```

### Comparing `greatday-1.0.0/src/greatday/_repo.py` & `greatday-1.1.0/src/greatday/repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,66 +6,67 @@
 import operator
 from pathlib import Path
 from typing import Any, Callable, TypeVar
 
 from eris import ErisResult, Err, Ok
 from logrus import Logger
 import magodo
+import metaman
 from potoroo import Repo, TaggedRepo
 from sqlalchemy import func
-from sqlmodel import Integer, Session, or_, select
+from sqlmodel import Integer, Session, and_, or_, select
 from sqlmodel.sql.expression import SelectOfScalar
 from typist import PathLike
 
 from . import db, models
-from ._common import NULL_ID
-from ._tag import (
+from .common import NULL_ID
+from .tag import GreatTag, Tag
+from .todo import GreatTodo
+from .types import (
+    CreateEngineType,
     DescOperator,
-    GreatTag,
     MetatagOperator,
     MetatagValueType,
-    Tag,
 )
-from ._todo import GreatTodo
-from .types import CreateEngineType
 
 
 logger = Logger(__name__)
 
 SelectOfTodo = SelectOfScalar[models.Todo]
 SQLStatementParser = Callable[["SQLTag", SelectOfTodo], SelectOfTodo]
 T = TypeVar("T")
 
-# will be populated by the @sql_stmt_parser decorator
-SQL_STMT_PARSERS: list[SQLStatementParser] = []
-
-
-def sql_stmt_parser(parser: SQLStatementParser) -> SQLStatementParser:
-    """Decorator that registers statement parsers for SQLTag class."""
-    SQL_STMT_PARSERS.append(parser)
-    return parser
+# the @sql_tag_parser decorator should be used to mark a SQLTag parser
+_SQL_TAG_PARSERS: list[SQLStatementParser] = []
+sql_tag_parser = metaman.register_function_factory(_SQL_TAG_PARSERS)
 
 
 class SQLRepo(TaggedRepo[str, GreatTodo, GreatTag]):
     """Repo that stores Todos in sqlite database."""
 
     def __init__(
         self,
         url: str,
         *,
         engine_factory: CreateEngineType = db.create_cached_engine,
         verbose: int = 0,
     ) -> None:
+        # echo SQL statements to console if -vvv or greater is specified on the
+        # command-line
+        engine_kwargs = {}
+        if verbose > 2:
+            engine_kwargs["echo"] = True
+
+        # public SQLRepo attributes
         self.url = url
+        self.engine = engine_factory(url, **engine_kwargs)
 
-        # create the Engine object
-        kwargs = {}
-        if verbose > 2:
-            kwargs["echo"] = True
-        self.engine = engine_factory(url, **kwargs)
+        # private SQLRepo attributes
+        self._verbose = verbose
+        self._engine_factory = engine_factory
 
     def add(self, todo: GreatTodo, /, *, key: str = None) -> ErisResult[str]:
         """Adds a new Todo to the DB.
 
         Returns a unique identifier that has been associated with this Todo.
         """
         with Session(self.engine) as session:
@@ -165,60 +166,72 @@
 
     session: Session
     tag: Tag
 
     def to_stmt(self) -> SelectOfTodo:
         """Constructs a SQL statement from the provided Tag object."""
         stmt = select(models.Todo)
-        for parse_stmt in SQL_STMT_PARSERS:
+        for parse_stmt in _SQL_TAG_PARSERS:
             stmt = parse_stmt(self, stmt)
         return stmt
 
-    @sql_stmt_parser
+    @sql_tag_parser
     def done_parser(self, stmt: SelectOfTodo) -> SelectOfTodo:
         """Parser for done status (i.e. 'x' or 'o')."""
         if self.tag.done is not None:
             stmt = stmt.where(models.Todo.done == self.tag.done)
         return stmt
 
-    @sql_stmt_parser
+    @sql_tag_parser
     def prefix_tag_parser(self, stmt: SelectOfTodo) -> SelectOfTodo:
         """Parser for prefix tags (e.g. '@home' or '+greatday')."""
         for prefix_tag_list, link_model, model in [
             (self.tag.contexts, models.ContextLink, models.Context),
             (self.tag.epics, models.EpicLink, models.Epic),
             (self.tag.projects, models.ProjectLink, models.Project),
         ]:
+            base_subquery = select(models.Todo.id).join(link_model).join(model)
             for prefix_tag in prefix_tag_list:
-                if prefix_tag.startswith("-"):
-                    name = prefix_tag[1:]
-                    op = models.Todo.id.not_in  # type: ignore[union-attr]
+                name = prefix_tag
+
+                if name.startswith("-"):
+                    # remove '-' from name
+                    name = name[1:]
+
+                    in_op = models.Todo.id.not_in  # type: ignore[union-attr]
+                    or_and = and_
                 else:
-                    name = prefix_tag
-                    op = models.Todo.id.in_  # type: ignore[union-attr]
+                    in_op = models.Todo.id.in_  # type: ignore[union-attr]
+                    or_and = or_
 
-                subquery = (
-                    select(models.Todo.id)
-                    .join(link_model)
-                    .join(model)
-                    .where(model.name == name)
-                )
-                stmt = stmt.where(op(subquery))
+                subqueries = []
+                if name.endswith(".*"):
+                    name = name[:-2]
+
+                    like_op = model.name.ilike  # type: ignore[attr-defined]
+                    like_arg = f"{name}.%"
+
+                    subquery = base_subquery.where(like_op(like_arg))
+                    subqueries.append(subquery)
+
+                subquery = base_subquery.where(model.name == name)
+                subqueries.append(subquery)
+                stmt = stmt.where(or_and(in_op(subq) for subq in subqueries))
         return stmt
 
-    @sql_stmt_parser
+    @sql_tag_parser
     def priority_range_parser(self, stmt: SelectOfTodo) -> SelectOfTodo:
         """Parser for priority range (e.g. '(a-c)')."""
         if self.tag.priorities:
             stmt = stmt.where(
                 or_(models.Todo.priority == p for p in self.tag.priorities)
             )
         return stmt
 
-    @sql_stmt_parser
+    @sql_tag_parser
     def desc_parser(self, stmt: SelectOfTodo) -> SelectOfTodo:
         """Parser for todo description (e.g. '"foo"' or '!"bar"')"""
         for desc_filter in self.tag.desc_filters:
             case_sensitive = desc_filter.case_sensitive
             if case_sensitive is None:
                 case_sensitive = not bool(desc_filter.value.islower())
 
@@ -247,15 +260,15 @@
                 }
                 op = op_map[desc_filter.op]
                 op_arg = like_arg
 
             stmt = stmt.where(op(op_arg))
         return stmt
 
-    @sql_stmt_parser
+    @sql_tag_parser
     def date_range_parser(self, stmt: SelectOfTodo) -> SelectOfTodo:
         """Parser for create/done dates (e.g. '^2000-01-01' or '$5d:0d')."""
         for date_range_list, model_date in [
             (self.tag.create_date_ranges, models.Todo.create_date),
             (self.tag.done_date_ranges, models.Todo.done_date),
         ]:
             for date_range in date_range_list:
@@ -263,26 +276,28 @@
                 stmt = (
                     stmt.where(model_date is not None)
                     .where(model_date >= date_range.start)  # type: ignore[operator]
                     .where(model_date <= end_date)  # type: ignore[operator]
                 )
         return stmt
 
-    @sql_stmt_parser
+    @sql_tag_parser
     def metatag_parser(self, stmt: SelectOfTodo) -> SelectOfTodo:
         """Parser for metatags (e.g. 'due<=0d')."""
         comp_op_map = {
             MetatagOperator.EQ: operator.eq,
             MetatagOperator.NE: operator.ne,
             MetatagOperator.LT: operator.lt,
             MetatagOperator.GT: operator.gt,
             MetatagOperator.LE: operator.le,
             MetatagOperator.GE: operator.ge,
         }
         for mfilter in self.tag.metatag_filters:
+            # special logic is need to handle the 'id' metatag since we don't
+            # store the ID as a metatag in the SQL DB
             if mfilter.key == "id" and mfilter.op not in [
                 MetatagOperator.EXISTS,
                 MetatagOperator.NOT_EXISTS,
             ]:
                 comp_op = comp_op_map[mfilter.op]
                 stmt = stmt.where(
                     comp_op(_col_to_int(models.Todo.id), int(mfilter.value))
```

### Comparing `greatday-1.0.0/src/greatday/_runners.py` & `greatday-1.1.0/src/greatday/runners.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from __future__ import annotations
 
 from typing import Final, List
 
 from clack.types import ClackRunner
 from logrus import Logger
 import metaman
+from vimala import vim
 
-from ._common import CTX_INBOX, drop_words
-from ._config import AddConfig, ListConfig, TUIConfig
-from ._repo import SQLRepo
-from ._tag import GreatTag
-from ._todo import GreatTodo
-from ._tui import start_textual_app
+from . import tui
+from .common import CTX_INBOX, drop_words
+from .config import AddConfig, ListConfig, TUIConfig
+from .repo import SQLRepo
+from .session import GreatSession
+from .tag import GreatTag
+from .todo import GreatTodo
 
 
-ALL_RUNNERS: List[ClackRunner] = []
-runner = metaman.register_function_factory(ALL_RUNNERS)
+RUNNERS: List[ClackRunner] = []
+runner = metaman.register_function_factory(RUNNERS)
 
 logger = Logger(__name__)
 
 CTX_X: Final = "x"
 
 
 @runner
@@ -73,9 +75,36 @@
 
     return 0
 
 
 @runner
 def run_tui(cfg: TUIConfig) -> int:
     """Runer for the 'tui' subcommand."""
-    start_textual_app(cfg.database_url, verbose=cfg.verbose)
+    repo = SQLRepo(cfg.database_url)
+
+    # get default active query
+    query = tui.get_default_query(
+        cfg.saved_query_groups, cfg.default_query_group
+    )
+
+    ctx = tui.Context(query, cfg.default_query_group)
+
+    def run_app() -> None:
+        app = tui.GreatApp(
+            repo=repo, ctx=ctx, saved_query_group_map=cfg.saved_query_groups
+        )
+        app.run()
+
+    run_app()
+
+    while ctx.edit_todos:
+        tag = GreatTag.from_query(ctx.query)
+        with GreatSession(
+            cfg.database_url, tag, verbose=cfg.verbose
+        ) as session:
+            vim(session.path).unwrap()
+            session.commit()
+
+        ctx.edit_todos = False
+        run_app()
+
     return 0
```

### Comparing `greatday-1.0.0/src/greatday/_session.py` & `greatday-1.1.0/src/greatday/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,53 +11,61 @@
 from typing import Type, cast
 
 from logrus import Logger
 import magodo
 from magodo.types import Priority
 from potoroo import Repo, UnitOfWork
 
-from ._common import NULL_ID
-from ._dates import get_relative_date
-from ._repo import FileRepo, SQLRepo
-from ._tag import GreatTag
-from ._todo import GreatTodo
+from .common import NULL_ID
+from .dates import get_relative_date
+from .repo import FileRepo, SQLRepo
+from .tag import GreatTag
+from .todo import GreatTodo
 
 
 logger = Logger(__name__)
 
 
 class GreatSession(UnitOfWork[FileRepo]):
     """Each time todos are opened in an editor, a new session is created."""
 
     def __init__(
         self,
         db_url: str,
-        tag: GreatTag = None,
+        tag: GreatTag,
         *,
         name: str = None,
         verbose: int = 0,
     ) -> None:
-        self.db_url = db_url
-
         prefix = None if name is None else f"{name}."
         _, temp_path = tempfile.mkstemp(prefix=prefix, suffix=".txt")
+
+        # --- public attributes
+        self.db_url = db_url
         self.path = Path(temp_path)
 
+        # --- private attributes
+        self._tag = tag
+        self._name = name
+        self._verbose = verbose
         self._master_repo = SQLRepo(self.db_url, verbose=verbose)
         self._key_to_old_todo = {}
-        if tag is not None:
-            self.path.parent.mkdir(parents=True, exist_ok=True)
-            with self.path.open("a+") as f:
-                for todo in sorted(self._master_repo.get_by_tag(tag).unwrap()):
-                    f.write(todo.to_line() + "\n")
-                    self._key_to_old_todo[todo.ident] = todo
-
         # will be accessed via `self.repo` from this point forward
         self._repo = FileRepo(self.path)
 
+        # init SQL repo and file repo + populate file repo's text file with
+        # todos which match `tag`
+        #
+        # we also populate the `self._key_to_old_todo` dict here
+        self.path.parent.mkdir(parents=True, exist_ok=True)
+        with self.path.open("a+") as f:
+            for todo in sorted(self._master_repo.get_by_tag(tag).unwrap()):
+                f.write(todo.to_line() + "\n")
+                self._key_to_old_todo[todo.ident] = todo
+
     def __enter__(self) -> GreatSession:
         """Called before entering a GreatSession with-block."""
         return self
 
     def __exit__(
         self,
         exc_type: Type[BaseException] | None,
@@ -68,19 +76,15 @@
         del exc_type
         del exc_value
         del traceback
 
         os.unlink(self.path)
 
     def commit(self) -> None:
-        """Commit our changes.
-
-        We achieve this by copying the contents of the backup file created on
-        instantiation back to the original.
-        """
+        """Commit our changes."""
         removed_todo_keys = list(self._key_to_old_todo.keys())
         new_todos = {}
         for todo in self.repo.all().unwrap():
             key = todo.ident
             if key in removed_todo_keys:
                 removed_todo_keys.remove(key)
 
@@ -161,28 +165,32 @@
 
         # set creation date + clear creation/done time for next todo...
         next_create_date = dt.date.today()
         for key in ["ctime", "dtime"]:
             if key in next_metadata:
                 del next_metadata[key]
 
+        # clear out contexts we don't want to roll over to the next todo...
+        contexts = [ctx for ctx in todo.contexts if ctx not in ["D"]]
+
         # set priority for next todo...
         priority = todo.metadata.get("priority")
         next_priority = magodo.DEFAULT_PRIORITY
         if (
             priority
             and len(priority) == 1
             and priority.upper() in string.ascii_uppercase
         ):
             next_priority = cast(Priority, priority.upper())
         elif priority:
             logger.warning("Bad 'priority' metatag value?", priority=priority)
 
         # add next todo to repo...
         next_todo = todo.new(
+            contexts=contexts,
             create_date=next_create_date,
             done=False,
             done_date=None,
             metadata=next_metadata,
             priority=next_priority,
         )
         next_key = repo.add(next_todo).unwrap()
```

### Comparing `greatday-1.0.0/src/greatday/_spells.py` & `greatday-1.1.0/src/greatday/spells.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """Contains custom magodo Todo spells used by greatday."""
 
 from __future__ import annotations
 
 import datetime as dt
-from typing import Final, Iterable, List
+from typing import Callable, Final, Iterable, List
 
 from logrus import Logger
 import magodo
-from magodo.types import LineSpell, T, TodoSpell
+from magodo.types import LineSpell, Metadata, T, TodoSpell
 from metaman import register_function_factory
 
-from ._common import drop_word_if_startswith, drop_words, todo_prefixes
-from ._dates import (
+from .common import drop_word_if_startswith, drop_words, todo_prefixes
+from .dates import (
     RELATIVE_DATE_METATAGS,
+    SUNDAY,
     dt_from_date_and_hhmm,
+    get_all_days,
+    get_month_days,
+    get_next_day,
+    get_quarter_days,
     get_relative_date,
     matches_date_fmt,
     matches_relative_date_fmt,
 )
 
 
 logger = Logger(__name__)
@@ -113,28 +118,33 @@
 def render_relative_dates(todo: T) -> T:
     """Renders metatags that support relative dates.
 
     (e.g. 'due:1d' -> 'due:2022-02-16')
     """
     found_tag = False
     desc = todo.desc
-    metadata = dict(todo.metadata.items())
+    metadata: Metadata | None = {}
 
     for key in RELATIVE_DATE_METATAGS:
         value = todo.metadata.get(key)
         if not value:
             continue
 
         if not matches_relative_date_fmt(value):
             continue
 
-        found_tag = True
+        # we only create a new dict of metadata if we have to
+        if not found_tag:
+            found_tag = True
+            metadata = dict(todo.metadata.items())
 
         value_date = get_relative_date(value)
         new_value = magodo.dates.from_date(value_date)
+
+        assert metadata is not None
         metadata[key] = new_value
 
         desc = drop_word_if_startswith(desc, key + ":")
 
     if not found_tag:
         return todo
 
@@ -175,46 +185,131 @@
 
     today = dt.date.today()
     if magodo.dates.to_date(due) > today:
         return todo
 
     now = dt.datetime.now()
     appt_dt = dt_from_date_and_hhmm(today, appt)
-    if appt_dt < now + dt.timedelta(minutes=30):
+    if appt_dt < now + dt.timedelta(hours=1):
         priority = "C"
     else:
         priority = "T"
 
     return todo.new(priority=priority)
 
 
 @todo_spell
-def in_progress_priority_spell(todo: T) -> T:
-    """Handles todos with the in-prigress priority."""
-    start = todo.metadata.get("start")
-    if todo.priority != IN_PROGRESS_PRIORITY:
-        if start:
-            metadata = dict(todo.metadata.items())
-            del metadata["start"]
-            desc = drop_word_if_startswith(todo.desc, "start:")
-            return todo.new(desc=desc, metadata=metadata)
-        else:
-            return todo
+def inbox_spell(todo: T) -> T:
+    """Converts @i into @INBOX."""
+    if "i" not in todo.contexts:
+        return todo
+    contexts = [ctx for ctx in todo.contexts if ctx != "i"]
+    contexts.append("INBOX")
+    return todo.new(contexts=contexts)
+
+
+@todo_spell
+def scope_spell(todo: T) -> T:
+    """Spell that handles @w/@m/@q/@y/@o/@t/@s contexts.
 
-    if start:
+    Adds appropriate 'scope' metatag and 'due' date.
+    """
+    day_of_week = SUNDAY
+
+    def get_w_due() -> dt.date:
+        return get_next_day(day_of_week=day_of_week)
+
+    def get_m_due() -> dt.date:
+        return get_next_day(day_of_week=day_of_week, day_maker=get_month_days)
+
+    def get_q_due() -> dt.date:
+        return get_next_day(
+            day_of_week=day_of_week, day_maker=get_quarter_days
+        )
+
+    def get_y_due() -> dt.date:
+        year = dt.date.today().year + 1
+        return get_all_days(day_of_week=day_of_week, year=year)[0]
+
+    def get_o_due() -> dt.date:
+        return get_next_nth_year_day(4)
+
+    def get_t_due() -> dt.date:
+        return get_next_nth_year_day(20)
+
+    def get_next_nth_year_day(n: int) -> dt.date:
+        d = dt.date.today()
+        y = d.year + 1
+        while y % n != 0:
+            y += 1
+        return get_all_days(day_of_week=day_of_week, year=y)[0]
+
+    scope_contexts = ["w", "m", "q", "y", "o", "t", "s"]
+    get_due_funcs: list[Callable[[], dt.date | None]] = [
+        get_w_due,
+        get_m_due,
+        get_q_due,
+        get_y_due,
+        get_o_due,
+        get_t_due,
+        lambda: None,
+    ]
+
+    scope: int | None = None
+    due: dt.date | None = None
+    for i, (ctx, get_due) in enumerate(
+        zip(
+            scope_contexts,
+            get_due_funcs,
+        )
+    ):
+        if ctx in todo.contexts:
+            scope = i + 1
+            due = get_due()
+            break
+    else:
         return todo
 
-    now = dt.datetime.now()
-    start = f"{now.hour:0>2}{now.minute:0>2}"
+    assert scope is not None
+
+    todo = reopen_if_closed(todo)
+    bad_contexts = scope_contexts + ["INBOX"]
+    contexts = [ctx for ctx in todo.contexts if ctx not in bad_contexts]
 
     metadata = dict(todo.metadata.items())
-    metadata["start"] = start
-    desc = todo.desc + f" start:{start}"
+    metadata["scope"] = str(scope)
+    if due is not None:
+        metadata["due"] = magodo.dates.from_date(due)
+    elif "due" in metadata:
+        del metadata["due"]
 
-    return todo.new(desc=desc, metadata=metadata)
+    return todo.new(contexts=contexts, metadata=metadata)
+
+
+@todo_spell
+def reopen_todo_spell(todo: T) -> T:
+    """Spell that re-opens todos when the '@x' context is found."""
+    if "x" not in todo.contexts:
+        return todo
+
+    todo = reopen_if_closed(todo)
+    contexts = [ctx for ctx in todo.contexts if ctx != "x"]
+    return todo.new(contexts=contexts)
+
+
+def reopen_if_closed(todo: T) -> T:
+    """Re-opens a closed todo."""
+    if not todo.done:
+        return todo
+
+    metadata = dict(todo.metadata.items())
+    if "dtime" in metadata:
+        del metadata["dtime"]
+
+    return todo.new(done=False, done_date=None, metadata=metadata)
 
 
 ###############################################################################
 # post-todo spells | Lastly, all POST todo spells are cast...
 ###############################################################################
 @post_todo_spell
 def remove_priorities(todo: T) -> T:
```

### Comparing `greatday-1.0.0/src/greatday/_tag.py` & `greatday-1.1.0/src/greatday/tag.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,84 +1,40 @@
 """Contains the Tag class."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-import enum
 import string
 from typing import Callable, Iterable, cast
 
 from eris import ErisResult, Err, Ok
 from logrus import Logger
 import magodo
 from magodo.types import Priority
 
-from ._dates import (
+from .dates import (
     RELATIVE_DATE_METATAGS,
     DateRange,
     get_date_range,
     get_relative_date,
     matches_date_fmt,
     matches_relative_date_fmt,
 )
+from .types import (
+    DescFilter,
+    DescOperator,
+    MetatagFilter,
+    MetatagOperator,
+    MetatagValueType,
+)
 
 
 logger = Logger(__name__)
 
-QueryParser = Callable[[str], ErisResult[str]]
-
-
-class MetatagOperator(enum.Enum):
-    """Used to determine what kind of metatag constraint has been specified."""
-
-    # exists / not exists
-    EXISTS = enum.auto()
-    NOT_EXISTS = enum.auto()
-
-    # comparison operators
-    EQ = enum.auto()
-    NE = enum.auto()
-    LT = enum.auto()
-    LE = enum.auto()
-    GT = enum.auto()
-    GE = enum.auto()
-
-
-class MetatagValueType(enum.Enum):
-    """Specifies the data type of a MetatagFilter's value."""
-
-    DATE = enum.auto()
-    INTEGER = enum.auto()
-    STRING = enum.auto()
-
-
-@dataclass(frozen=True)
-class MetatagFilter:
-    """Represents a single metatag filter (e.g. 'due<=0d' or '!recur')."""
-
-    key: str
-    value: str = ""
-    op: MetatagOperator = MetatagOperator.EXISTS
-    value_type: MetatagValueType = MetatagValueType.STRING
-
-
-class DescOperator(enum.Enum):
-    """Used to determine the type of description constraint specified."""
-
-    CONTAINS = enum.auto()
-    NOT_CONTAINS = enum.auto()
-
-
-@dataclass(frozen=True)
-class DescFilter:
-    """Represents a description query filter (e.g. '"foo"' or '!"bar"')."""
-
-    value: str
-    case_sensitive: bool | None = None
-    op: DescOperator = DescOperator.CONTAINS
+TagParser = Callable[[str], ErisResult[str]]
 
 
 @dataclass(frozen=True)
 class GreatTag:
     """A collection of `Tag`s that have been ORed together."""
 
     tags: Iterable[Tag]
@@ -142,31 +98,33 @@
                 raise RuntimeError(
                     "No parsers are able to parse this query. |"
                     f" query={query!r}"
                 )
 
         return tag
 
-    def prefix_tag_parser_factory(self, ch: str, attr: str) -> QueryParser:
+    def prefix_tag_parser_factory(self, ch: str, attr: str) -> TagParser:
         """Factory for parsers that handle normal tags (e.g. project tags)."""
 
         def parser(query: str) -> ErisResult[str]:
             prop_list = getattr(self, attr)
             word, *rest = query.split(" ")
 
             if word.startswith(ch):
                 logger.debug("Filter on property.", word=word)
                 prop_list.append(word[1:])
             elif word.startswith(f"!{ch}"):
                 logger.debug("Filter on negative property.", word=word)
                 prop_list.append(f"-{word[2:]}")
             else:
                 return Err(
-                    "First word of query does not match required tag prefix."
-                    f" | prefix={ch} word={word}",
+                    (
+                        "First word of query does not match required tag"
+                        f" prefix. | prefix={ch} word={word}"
+                    ),
                 )
 
             return Ok(" ".join(rest))
 
         return parser
 
     def done_parser(self, query: str) -> ErisResult[str]:
@@ -177,15 +135,15 @@
         elif word.lower() == "x":
             self.done = True
         else:
             return Err("Next token is not 'o' or 'x'.")
 
         return Ok(" ".join(rest))
 
-    def date_range_parser_factory(self, ch: str, attr: str) -> QueryParser:
+    def date_range_parser_factory(self, ch: str, attr: str) -> TagParser:
         """Factory for create/done date range tokens."""
 
         def parser(query: str) -> ErisResult[str]:
             word, *rest = query.split(" ")
             if not word.startswith(ch):
                 return Err("Next token is not a date range.")
 
@@ -255,15 +213,15 @@
                 )
                 break
             else:
                 return Err("Next token is not a metadata check.")
 
         return Ok(" ".join(rest))
 
-    def desc_parser_factory(self, quote: str) -> QueryParser:
+    def desc_parser_factory(self, quote: str) -> TagParser:
         """Factory for parser that handles description tokens."""
 
         def parser(query: str) -> ErisResult[str]:
             desc_op = DescOperator.CONTAINS
             q = query
             if q.startswith(f"!{quote}") or q.startswith(f"!c{quote}"):
                 q = q[1:]
```

### Comparing `greatday-1.0.0/src/greatday/_todo.py` & `greatday-1.1.0/src/greatday/todo.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 from eris import ErisResult, Err, Ok
 import magodo
 from magodo import MagicTodoMixin
 from magodo.types import Priority
 from sqlmodel import Session, select
 
-from . import _spells as spells, models
-from ._common import NULL_ID, drop_word_if_startswith
+from . import models, spells
+from .common import NULL_ID, drop_word_if_startswith
 
 
+# cache used to optimize the `GreatTodo.from_line()` constructor method
 _LINE_TO_TODO_CACHE: dict[str, "GreatTodo"] = {}
 
 
 class GreatTodo(MagicTodoMixin):
     """Custom MagicTodo type used when working with Todos in the daily file."""
 
     pre_todo_spells = spells.GREAT_PRE_TODO_SPELLS
@@ -83,21 +84,21 @@
             # have the same value)
             del metadata["id"]
 
         if key is None and id_metatag is not None:
             key = id_metatag
 
         desc = drop_word_if_startswith(self.desc, "id:")
-        mtodo_kwargs: dict[str, Any] = dict(
-            create_date=self.create_date,
-            desc=desc,
-            done=self.done,
-            done_date=self.done_date,
-            priority=self.priority,
-        )
+        mtodo_kwargs: dict[str, Any] = {
+            "create_date": self.create_date,
+            "desc": desc,
+            "done": self.done,
+            "done_date": self.done_date,
+            "priority": self.priority,
+        }
 
         stmt: Any
         if key is None:
             mtodo = models.Todo(**mtodo_kwargs)
         else:
             stmt = select(models.Todo).where(models.Todo.id == int(key))
             results = session.exec(stmt)
```

### Comparing `greatday-1.0.0/src/greatday/db.py` & `greatday-1.1.0/src/greatday/db.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Contains all database utilities."""
 
 from __future__ import annotations
 
 from functools import lru_cache as cache
-import os
 from typing import Any
 
 from sqlalchemy.future import Engine
 from sqlmodel import SQLModel, create_engine as sqlmodel_create_engine
 
 
 @cache
@@ -15,13 +14,10 @@
     """Helper function for creating a new (if necessary) sqlalchemy engine."""
     engine = create_engine(url, **kwargs)
     return engine
 
 
 def create_engine(url: str, /, **kwargs: Any) -> Engine:
     """Wrapper around sqlmodel.create_engine() that makes sure tables exist."""
-    if "echo" not in kwargs and "ECHO_SQL_QUERIES" in os.environ:
-        kwargs["echo"] = True
-
     engine = sqlmodel_create_engine(url, **kwargs)
     SQLModel.metadata.create_all(engine)
     return engine
```

### Comparing `greatday-1.0.0/src/greatday/models.py` & `greatday-1.1.0/src/greatday/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import List, Optional
 
 from sqlmodel import Column, Field, Relationship, SQLModel, String
 from sqlmodel.sql.expression import Select, SelectOfScalar
 
 
 # HACK: see https://github.com/tiangolo/sqlmodel/issues/189
-Select.inherit_cache = True  # type: ignore[attr-defined]
-SelectOfScalar.inherit_cache = True  # type: ignore[attr-defined]
+Select.inherit_cache = True
+SelectOfScalar.inherit_cache = True
 
 
 ###############################################################################
 # abstract model classes
 ###############################################################################
 class Base(SQLModel):
     """Abstract base model class."""
```

### Comparing `greatday-1.0.0/src/greatday.egg-info/SOURCES.txt` & `greatday-1.1.0/src/greatday.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -40,51 +40,55 @@
 bin/file_repo_to_sql_repo.py
 bin/publish_docs
 bin/quick-lints
 bin/render_all_cogs
 docs/GreatLang.ebnf
 docs/Makefile
 docs/make.bat
-docs/design/design-1.svg
-docs/design/design-2.svg
-docs/design/design-3.svg
-docs/design/design-4.svg
-docs/design/design.md
-docs/design/design.template.md
 docs/source/changelog.rst
 docs/source/conf.py
 docs/source/contributing.rst
 docs/source/greatday.cli.rst
+docs/source/greatday.common.rst
+docs/source/greatday.config.rst
+docs/source/greatday.dates.rst
 docs/source/greatday.db.rst
 docs/source/greatday.models.rst
+docs/source/greatday.repo.rst
 docs/source/greatday.rst
+docs/source/greatday.runners.rst
+docs/source/greatday.session.rst
+docs/source/greatday.spells.rst
+docs/source/greatday.tag.rst
+docs/source/greatday.todo.rst
+docs/source/greatday.tui.rst
 docs/source/greatday.types.rst
 docs/source/index.rst
 docs/source/modules.rst
 docs/source/readme.rst
 docs/source/_static/README.md
 docs/source/_templates/README.md
 docs/source/_templates/footer.html
 lib/bugyi.sh
 scripts/README.md
 src/greatday/__init__.py
 src/greatday/__main__.py
-src/greatday/_common.py
-src/greatday/_config.py
-src/greatday/_dates.py
-src/greatday/_repo.py
-src/greatday/_runners.py
-src/greatday/_session.py
-src/greatday/_spells.py
-src/greatday/_tag.py
-src/greatday/_todo.py
-src/greatday/_tui.py
+src/greatday/common.py
+src/greatday/config.py
+src/greatday/dates.py
 src/greatday/db.py
 src/greatday/models.py
 src/greatday/py.typed
+src/greatday/repo.py
+src/greatday/runners.py
+src/greatday/session.py
+src/greatday/spells.py
+src/greatday/tag.py
+src/greatday/todo.py
+src/greatday/tui.py
 src/greatday/types.py
 src/greatday.egg-info/PKG-INFO
 src/greatday.egg-info/SOURCES.txt
 src/greatday.egg-info/dependency_links.txt
 src/greatday.egg-info/entry_points.txt
 src/greatday.egg-info/not-zip-safe
 src/greatday.egg-info/requires.txt
```

### Comparing `greatday-1.0.0/targets.mk` & `greatday-1.1.0/targets.mk`

 * *Files identical despite different names*

### Comparing `greatday-1.0.0/tests/common.py` & `greatday-1.1.0/tests/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,78 +8,85 @@
 # datetime info used by freezegun (and tests)
 hh: Final = "00"
 mm: Final = "00"
 hhmm: Final = f"{hh}{mm}"
 
 YYYY: Final = "2000"
 MM: Final = "01"
-DD: Final = "01"
+DD: Final = "03"
 TODAY: Final = f"{YYYY}-{MM}-{DD}"
 
-TOMORROW: Final = f"{YYYY}-{MM}-02"
+TOMORROW: Final = f"{YYYY}-{MM}-04"
 
 # dummy todo lines.. used as test data
 TODO_LINES = (
     # ID #1
     "o 2000-01-01 Do some Laundry | @home @boring foo:bar",
     # ID #2
     "(B) 2000-02-03 Buy groceries | @out @boring +buy foo:bar due:2000-02-03",
     # ID #3
-    "x 2010-01-02 2010-01-01 Finish greatday tests | @dev +greatday"
-    " mile:2 p:0",
+    (
+        "x 2010-01-02 2010-01-01 Finish greatday tests | @dev +greatday"
+        " mile:2 p:0"
+    ),
     # ID #4
     "o 1900-01-01 Finish greatday tests | @dev +greatday due:2000-01-01",
     # ID #5
-    "x 2022-06-05 Some other todo | @misc p:1",
+    "x 2022-06-05 Some misc greatday todo | @misc +greatday.misc p:1",
+    # ID #6
+    "x 2022-06-05 FOO greatday todo | +greatday.misc.foo",
 )
 
 # the database IDs that should be associated with each of the todo lines above
 TODO_LINE_IDS = tuple(str(n) for n in range(1, len(TODO_LINES) + 1))
 
 # Parameters used by test_get_by_tag() test function.
 #
 # query -> ids
 #
 # query: used to construct GreatTag objects
 # ids: iist of todo line IDs that this query should match
 QUERY_TO_TODO_IDS: list[tuple[str, list[int]]] = [
-    ("", [1, 2, 3, 4, 5]),
-    ("o", [1, 2, 4]),
-    ("x", [3, 5]),
+    ("", list(int(n) for n in TODO_LINE_IDS)),
+    ("o id<6", [1, 2, 4]),
+    ("x id<6", [3, 5]),
     ("@home", [1]),
-    ("!@home", [2, 3, 4, 5]),
+    ("!@home id<6", [2, 3, 4, 5]),
     ("!@home @boring", [2]),
     ("@home @boring", [1]),
     ("@boring", [1, 2]),
-    ("+greatday", [3, 4]),
     ("+buy @boring", [2]),
     ("(a)", []),
     ("(b)", [2]),
     ("(a-b)", [2]),
     ("(a,b)", [2]),
     ("due", [2, 4]),
-    ("!due", [1, 3, 5]),
+    ("!due id<6", [1, 3, 5]),
     ("due=2000-01-01", [4]),
     ("due>=2000-01-01", [2, 4]),
     ("due>2000-01-01", [2]),
     ("p", [3, 5]),
     ("p>0", [5]),
     ("^2000-01-01", [1]),
     ("^2000-01-01:2010-12-31", [1, 2, 3]),
     ("^2000-01-01:2010-12-31 $2010-01-01", []),
     ("^2000-01-01:2010-12-31 $2010-01-02", [3]),
     ('"some"', [1, 5]),
-    ('!"some"', [2, 3, 4]),
+    ('!"some"', [2, 3, 4, 6]),
     ('"Some"', [5]),
-    ('!"Some"', [1, 2, 3, 4]),
+    ('!"Some"', [1, 2, 3, 4, 6]),
     ('c"some"', [1]),
-    ('!c"some"', [2, 3, 4, 5]),
+    ('!c"some"', [2, 3, 4, 5, 6]),
     ("id=2", [2]),
-    ("id>2", [3, 4, 5]),
+    ("id>2 id<6", [3, 4, 5]),
     ("@home | @out", [1, 2]),
+    ("+greatday", [3, 4]),
+    ("+greatday.*", [3, 4, 5, 6]),
+    ("+greatday.* !+greatday", [5, 6]),
+    ("+greatday.* !+greatday.misc.*", [3, 4]),
 ]
 
 
 class MainType(Protocol):
     """Type returned by main() fixture."""
 
     def __call__(self, *args: str, **kwargs: Any) -> int:
```

### Comparing `greatday-1.0.0/tests/conftest.py` & `greatday-1.1.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from typing import TYPE_CHECKING, Any, Final, Iterator
 
 from freezegun import freeze_time
 from pytest import fixture
 
 from greatday import db
 from greatday.__main__ import main as gtd_main
-from greatday._repo import SQLRepo
-from greatday._todo import GreatTodo
+from greatday.repo import SQLRepo
+from greatday.todo import GreatTodo
 
 from . import common as c
 
 
 if TYPE_CHECKING:  # fixes pytest warning
     from clack.pytest_plugin import MakeConfigFile
```

### Comparing `greatday-1.0.0/tests/test_file_repo.py` & `greatday-1.1.0/tests/test_file_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from __future__ import annotations
 
 from pathlib import Path
 
 from pytest import fixture
 
-from greatday._repo import FileRepo
-from greatday._todo import GreatTodo
+from greatday.repo import FileRepo
+from greatday.todo import GreatTodo
 
 
 TODO_LINES: list[str] = [
     "o foo | id:1",
     "o bar | id:2",
     "o baz | id:3",
 ]
```

### Comparing `greatday-1.0.0/tests/test_list.py` & `greatday-1.1.0/tests/test_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Test for greatday's 'list' subcommand."""
 
 from __future__ import annotations
 
 from _pytest.capture import CaptureFixture
 from pytest import mark
 
-from greatday._repo import SQLRepo
+from greatday.repo import SQLRepo
 
-from . import common
+from . import common as c
 
 
 params = mark.parametrize
 
 
-@params("query,expected_ids", common.QUERY_TO_TODO_IDS)
+@params("query,expected_ids", c.QUERY_TO_TODO_IDS)
 def test_list(
     capsys: CaptureFixture,
-    main: common.MainType,
+    main: c.MainType,
     sql_repo: SQLRepo,
     query: str,
     expected_ids: list[int],
 ) -> None:
     """Tests the 'list' subcommand."""
     del sql_repo
```

### Comparing `greatday-1.0.0/tests/test_session.py` & `greatday-1.1.0/tests/test_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from pathlib import Path
 from typing import Callable, Final
 
 import metaman
 from pytest import mark
 
-from greatday._repo import SQLRepo
-from greatday._session import GreatSession
-from greatday._tag import GreatTag
+from greatday.repo import SQLRepo
+from greatday.session import GreatSession
+from greatday.tag import GreatTag
 
 from . import common as c
 
 
 params = mark.parametrize
 
 FakeUserValidator = Callable[[SQLRepo], bool]
@@ -49,15 +49,17 @@
     with path.open("a") as f:
         f.write(f"o {DESC}\n")
 
     def validator(repo: SQLRepo) -> bool:
         assert len(repo.all().unwrap()) == len(c.TODO_LINES) + 1
         todo = repo.get(ID).unwrap()
         assert todo is not None
-        assert DESC in todo.to_line()
+        todo_line = todo.to_line()
+        assert DESC in todo_line
+        assert " id:" in todo_line
         return True
 
     return validator
 
 
 @fake_editor_user
 def edit_one_todo(path: Path) -> FakeUserValidator:
```

### Comparing `greatday-1.0.0/tests/test_sql_repo.py` & `greatday-1.1.0/tests/test_sql_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Tests for greatday's SQLRepo class."""
 
 from __future__ import annotations
 
 from pytest import mark
 
-from greatday._repo import SQLRepo
-from greatday._tag import GreatTag
-from greatday._todo import GreatTodo
+from greatday.repo import SQLRepo
+from greatday.tag import GreatTag
+from greatday.todo import GreatTodo
 
 from . import common
 
 
 params = mark.parametrize
```

