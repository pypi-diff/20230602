# Comparing `tmp/autora-3.0.0rc2.tar.gz` & `tmp/autora-3.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-3.0.0rc2.tar", last modified: Fri Jun  2 14:13:40 2023, max compression
+gzip compressed data, was "autora-3.0.0rc3.tar", last modified: Fri Jun  2 14:33:59 2023, max compression
```

## Comparing `autora-3.0.0rc2.tar` & `autora-3.0.0rc3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.681956 autora-3.0.0rc2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.681956 autora-3.0.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/publish-documentation-gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/test-pre-commit-hooks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/test-pypi-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/autora.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-02 14:13:27.000000 autora-3.0.0rc2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-02 14:13:27.000000 autora-3.0.0rc2/MAINTAINING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-02 14:13:40.689956 autora-3.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-02 14:13:27.000000 autora-3.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/docs/contribute/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/core.md
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/module.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/pre-commit-hooks.md
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/setup.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/docs/experiment-runner/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/experiment-runner/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/docs/experimentalist/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/experimentalist/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   189630 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/img/experimentalist.png
--rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/img/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/docs/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/theorist/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/tutorials/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.677956 autora-3.0.0rc2/mkdocs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/mkdocs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-02 14:13:27.000000 autora-3.0.0rc2/mkdocs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-02 14:13:27.000000 autora-3.0.0rc2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-02 14:13:27.000000 autora-3.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:13:40.689956 autora-3.0.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/src/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 14:13:27.000000 autora-3.0.0rc2/src/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/src/autora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 14:13:27.000000 autora-3.0.0rc2/tests/test_core_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.023544 autora-3.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.015544 autora-3.0.0rc3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.015544 autora-3.0.0rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.github/workflows/publish-documentation-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.github/workflows/test-pypi-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.015544 autora-3.0.0rc3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.idea/autora.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.015544 autora-3.0.0rc3/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.015544 autora-3.0.0rc3/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-02 14:33:48.000000 autora-3.0.0rc3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-02 14:33:48.000000 autora-3.0.0rc3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-02 14:33:48.000000 autora-3.0.0rc3/MAINTAINING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-02 14:33:59.019544 autora-3.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-02 14:33:48.000000 autora-3.0.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/docs/contribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/contribute/core.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/contribute/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/contribute/module.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/contribute/pre-commit-hooks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/contribute/setup.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/docs/experiment-runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/experiment-runner/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/docs/experimentalist/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/experimentalist/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   189630 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/img/experimentalist.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/img/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/docs/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/theorist/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 14:33:48.000000 autora-3.0.0rc3/docs/tutorials/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.015544 autora-3.0.0rc3/mkdocs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/mkdocs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-02 14:33:48.000000 autora-3.0.0rc3/mkdocs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-02 14:33:48.000000 autora-3.0.0rc3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-02 14:33:48.000000 autora-3.0.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:33:59.023544 autora-3.0.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 14:33:48.000000 autora-3.0.0rc3/src/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/src/autora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-02 14:33:58.000000 autora-3.0.0rc3/src/autora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-02 14:33:59.000000 autora-3.0.0rc3/src/autora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:33:58.000000 autora-3.0.0rc3/src/autora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-02 14:33:58.000000 autora-3.0.0rc3/src/autora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:33:58.000000 autora-3.0.0rc3/src/autora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:59.019544 autora-3.0.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 14:33:48.000000 autora-3.0.0rc3/tests/test_core_imports.py
```

### Comparing `autora-3.0.0rc2/.github/pull_request_template.md` & `autora-3.0.0rc3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/.github/workflows/publish-documentation-gh-pages.yml` & `autora-3.0.0rc3/.github/workflows/publish-documentation-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/.github/workflows/publish-package-pypi.yml` & `autora-3.0.0rc3/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/.github/workflows/test-pre-commit-hooks.yml` & `autora-3.0.0rc3/.github/workflows/test-pre-commit-hooks.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/.github/workflows/test-pytest.yml` & `autora-3.0.0rc3/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/.gitignore` & `autora-3.0.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/.idea/autora.iml` & `autora-3.0.0rc3/.idea/autora.iml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/.idea/inspectionProfiles/Project_Default.xml` & `autora-3.0.0rc3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/.pre-commit-config.yaml` & `autora-3.0.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/LICENSE.md` & `autora-3.0.0rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/MAINTAINING.md` & `autora-3.0.0rc3/MAINTAINING.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/PKG-INFO` & `autora-3.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.0rc2
+Version: 3.0.0rc3
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 Maintainer-email: Ben Andrew <benwallaceandrew@gmail.com>, George Dang <george_dang@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
@@ -60,16 +60,16 @@
 <b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Auto</b>mated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
 automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science.
 
 ![Autonomous Empirical Research Paradigm](https://github.com/AutoResearch/autora/raw/restructure/autora/docs/img/overview.png)
 
 ## Getting Started
 
-Check out the tutorials at 
-[https://autoresearch.github.io/autora/tutorials](https://autoresearch.github.io/autora/tutorials).
+Check out the documentation at 
+[https://autoresearch.github.io/autora](https://autoresearch.github.io/autora).
 
 ## About
 
 This project is in active development by 
 the [Autonomous Empirical Research Group](http://empiricalresearch.ai), 
 led by [Sebastian Musslick](https://smusslick.com), 
 in collaboration with the [Center for Computation and Visualization at Brown University](https://ccv.brown.edu).
```

### Comparing `autora-3.0.0rc2/README.md` & `autora-3.0.0rc3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 <b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Auto</b>mated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
 automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science.
 
 ![Autonomous Empirical Research Paradigm](https://github.com/AutoResearch/autora/raw/restructure/autora/docs/img/overview.png)
 
 ## Getting Started
 
-Check out the tutorials at 
-[https://autoresearch.github.io/autora/tutorials](https://autoresearch.github.io/autora/tutorials).
+Check out the documentation at 
+[https://autoresearch.github.io/autora](https://autoresearch.github.io/autora).
 
 ## About
 
 This project is in active development by 
 the [Autonomous Empirical Research Group](http://empiricalresearch.ai), 
 led by [Sebastian Musslick](https://smusslick.com), 
 in collaboration with the [Center for Computation and Visualization at Brown University](https://ccv.brown.edu).
```

### Comparing `autora-3.0.0rc2/docs/contribute/core.md` & `autora-3.0.0rc3/docs/contribute/core.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/contribute/index.md` & `autora-3.0.0rc3/docs/contribute/index.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/contribute/module.md` & `autora-3.0.0rc3/docs/contribute/module.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/contribute/pre-commit-hooks.md` & `autora-3.0.0rc3/docs/contribute/pre-commit-hooks.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/contribute/setup.md` & `autora-3.0.0rc3/docs/contribute/setup.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/experimentalist/index.md` & `autora-3.0.0rc3/docs/experimentalist/index.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/img/experimentalist.png` & `autora-3.0.0rc3/docs/img/experimentalist.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/img/logo.png` & `autora-3.0.0rc3/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/img/overview.png` & `autora-3.0.0rc3/docs/img/overview.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/index.md` & `autora-3.0.0rc3/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/docs/theorist/index.md` & `autora-3.0.0rc3/docs/theorist/index.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/mkdocs.yml` & `autora-3.0.0rc3/mkdocs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # yaml-language-server: $schema=https://squidfunk.github.io/mkdocs-material/schema.json
 
-site_name: Autonomous Empirical Research
+site_name: Automated Research Assistant
 repo_url: 'https://github.com/autoresearch/autora'
 edit_uri: 'blob/main/docs/'
 
 extra:
   colab_base_url: 'https://colab.research.google.com/github/AutoResearch/autora/blob/gh-pages'
 
 theme:
@@ -29,20 +29,18 @@
     - content.action.edit
     - content.action.view
     - navigation.indexes
 
 plugins:
   multirepo:
     nav_repos:
-      # There will be a navigation section with this section name
       - name: core
         import_url: https://github.com/autoresearch/autora-core/?branch=main&extra_imports=["mkdocs/base.yml"]
         imports: ["docs/pipeline/*",]
       - name: falsification
-        # you can define the edit uri path
         import_url: https://github.com/autoresearch/autora-experimentalist-falsification/?branch=main&extra_imports=["mkdocs/base.yml"]
         imports: ["docs/*", "docs/sampler/*", "docs/pooler/*"]
   mkdocs-jupyter: # required to convert Jupyter notebooks
     include_source: true
     execute: false
     ignore_h1_titles: true
   search: {}
@@ -62,19 +60,14 @@
   "javascripts/mathjax.js",
   "https://polyfill.io/v3/polyfill.min.js?features=es6",
   "https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"
 ]
 
 nav:
 - Introduction: 'index.md'
-#- Tutorials:
-#  - Introduction: 'tutorials/index.md'   # TODO: add tutorials
-#  - Automated Theorist                   # TODO: add tutorial from somewhere
-#  - Automated Experimentalist            # TODO: add tutorial from somewhere
-#  - Closed-Loop Discovery                # TODO: add tutorial from somewhere
 - User Guide:
   - Theorists:
     - Home: 'theorist/index.md'
     - DARTS: '!import https://github.com/autoresearch/autora-theorist-darts/?branch=main&extra_imports=["mkdocs/base.yml"]'
     - BMS: '!import https://github.com/autoresearch/autora-theorist-bms/?branch=main&extra_imports=["mkdocs/base.yml"]'
     - BSR: '!import https://github.com/autoresearch/autora-theorist-bsr/?branch=main&extra_imports=["mkdocs/base.yml"]'
   - Experimentalists:
```

### Comparing `autora-3.0.0rc2/pyproject.toml` & `autora-3.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/src/autora.egg-info/PKG-INFO` & `autora-3.0.0rc3/src/autora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.0rc2
+Version: 3.0.0rc3
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 Maintainer-email: Ben Andrew <benwallaceandrew@gmail.com>, George Dang <george_dang@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
@@ -60,16 +60,16 @@
 <b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Auto</b>mated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
 automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science.
 
 ![Autonomous Empirical Research Paradigm](https://github.com/AutoResearch/autora/raw/restructure/autora/docs/img/overview.png)
 
 ## Getting Started
 
-Check out the tutorials at 
-[https://autoresearch.github.io/autora/tutorials](https://autoresearch.github.io/autora/tutorials).
+Check out the documentation at 
+[https://autoresearch.github.io/autora](https://autoresearch.github.io/autora).
 
 ## About
 
 This project is in active development by 
 the [Autonomous Empirical Research Group](http://empiricalresearch.ai), 
 led by [Sebastian Musslick](https://smusslick.com), 
 in collaboration with the [Center for Computation and Visualization at Brown University](https://ccv.brown.edu).
```

### Comparing `autora-3.0.0rc2/src/autora.egg-info/SOURCES.txt` & `autora-3.0.0rc3/src/autora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-3.0.0rc2/src/autora.egg-info/requires.txt` & `autora-3.0.0rc3/src/autora.egg-info/requires.txt`

 * *Files identical despite different names*

