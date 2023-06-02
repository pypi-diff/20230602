# Comparing `tmp/autora-3.0.0a9.tar.gz` & `tmp/autora-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-3.0.0a9.tar", last modified: Fri May  5 13:20:41 2023, max compression
+gzip compressed data, was "autora-3.0.0rc2.tar", last modified: Fri Jun  2 14:13:40 2023, max compression
```

## Comparing `autora-3.0.0a9.tar` & `autora-3.0.0rc2.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.009979 autora-3.0.0a9/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 13:20:29.000000 autora-3.0.0a9/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:40.997979 autora-3.0.0a9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:40.997979 autora-3.0.0a9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/publish-documentation-gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/publish-package-anaconda-org.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/test-conda-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/test-poetry-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/test-pre-commit-hooks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-05 13:20:29.000000 autora-3.0.0a9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/autora.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-05 13:20:29.000000 autora-3.0.0a9/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:29.000000 autora-3.0.0a9/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:20:29.000000 autora-3.0.0a9/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 13:20:29.000000 autora-3.0.0a9/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 13:20:29.000000 autora-3.0.0a9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-05 13:20:41.009979 autora-3.0.0a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-05-05 13:20:29.000000 autora-3.0.0a9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:40.989979 autora-3.0.0a9/conda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/conda/autora/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-05 13:20:29.000000 autora-3.0.0a9/conda/autora/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 13:20:29.000000 autora-3.0.0a9/conda/autora/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/docs/experiment-runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/experiment-runner/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/docs/experimentalists/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/experimentalists/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/img/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/docs/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/theorist/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-05 13:20:29.000000 autora-3.0.0a9/mkdocs/base.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/mkdocs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-05 13:20:29.000000 autora-3.0.0a9/mkdocs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-05 13:20:29.000000 autora-3.0.0a9/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-05 13:20:29.000000 autora-3.0.0a9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:20:41.009979 autora-3.0.0a9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/src/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 13:20:29.000000 autora-3.0.0a9/src/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.009979 autora-3.0.0a9/src/autora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.681956 autora-3.0.0rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.681956 autora-3.0.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/publish-documentation-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/test-pypi-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/autora.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-02 14:13:27.000000 autora-3.0.0rc2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-02 14:13:27.000000 autora-3.0.0rc2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-02 14:13:27.000000 autora-3.0.0rc2/MAINTAINING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-02 14:13:40.689956 autora-3.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-02 14:13:27.000000 autora-3.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/docs/contribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/core.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/module.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/pre-commit-hooks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/contribute/setup.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/docs/experiment-runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/experiment-runner/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.685956 autora-3.0.0rc2/docs/experimentalist/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/experimentalist/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   189630 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/img/experimentalist.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/img/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/docs/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/theorist/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 14:13:27.000000 autora-3.0.0rc2/docs/tutorials/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.677956 autora-3.0.0rc2/mkdocs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/mkdocs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-02 14:13:27.000000 autora-3.0.0rc2/mkdocs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-02 14:13:27.000000 autora-3.0.0rc2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-02 14:13:27.000000 autora-3.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:13:40.689956 autora-3.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 14:13:27.000000 autora-3.0.0rc2/src/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/src/autora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:13:40.000000 autora-3.0.0rc2/src/autora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:40.689956 autora-3.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 14:13:27.000000 autora-3.0.0rc2/tests/test_core_imports.py
```

### Comparing `autora-3.0.0a9/.github/pull_request_template.md` & `autora-3.0.0rc2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a9/.github/workflows/publish-package-pypi.yml` & `autora-3.0.0rc2/.github/workflows/publish-package-pypi.yml`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,22 @@
     types: [published]
 
 permissions:
   contents: read
 
 jobs:
   deploy:
-
     runs-on: ubuntu-latest
-
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
+        cache: 'pip'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
```

### Comparing `autora-3.0.0a9/.github/workflows/test-pre-commit-hooks.yml` & `autora-3.0.0rc2/.github/workflows/test-pre-commit-hooks.yml`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 on:
   pull_request:
   merge_group:
 
 jobs:
   build:
     runs-on: ubuntu-latest
-
     steps:
     - uses: actions/checkout@v3
-    - run: pipx install poetry
-    - uses: actions/setup-python@v4
+    - name: Set up Python
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.8
-        cache: "poetry"
-    - run: poetry install --only pre-commit
+        python-version: '3.8'
+        cache: 'pip'
+    - run: pip install pre-commit
     - uses: actions/cache@v3
       with:
         path: ~/.cache/pre-commit
         key: pre-commit-3|${{ env.pythonLocation }}|${{ runner.os }}|${{ hashFiles('.pre-commit-config.yaml') }}
-    - run: poetry run pre-commit run --all-files --show-diff-on-failure --color=always
+    - run: pre-commit run --all-files --show-diff-on-failure --color=always
```

### Comparing `autora-3.0.0a9/.github/workflows/test-pytest.yml` & `autora-3.0.0rc2/.github/workflows/test-pytest.yml`

 * *Files 24% similar despite different names*

```diff
@@ -8,19 +8,19 @@
   merge_group:
 
 jobs:
   test:
     strategy:
       fail-fast: true
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
         os: [ubuntu-latest, macos-latest, windows-latest]
     runs-on: ${{ matrix.os }}
     steps:
-    - uses: actions/checkout@v3
-    - run: pipx install poetry
-    - uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python-version }}
-        cache: "poetry"
-    - run: poetry install --only main,test
-    - run: poetry run pytest
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+          cache: 'pip'
+      - name: Install dependencies
+        run: pip install -U ".[test]"
+      - run: pytest
```

### Comparing `autora-3.0.0a9/.gitignore` & `autora-3.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a9/.idea/autora.iml` & `autora-3.0.0rc2/.idea/autora.iml`

 * *Files 19% similar despite different names*

#### Comparing `autora-3.0.0a9/.idea/autora.iml` & `autora-3.0.0rc2/.idea/autora.iml`

```diff
@@ -9,16 +9,14 @@
       <excludeFolder url="file://$MODULE_DIR$/.venv"/>
       <excludeFolder url="file://$MODULE_DIR$/.vscode"/>
       <excludeFolder url="file://$MODULE_DIR$/site"/>
       <excludeFolder url="file://$MODULE_DIR$/venv"/>
     </content>
     <orderEntry type="jdk" jdkName="Python 3.8 (autora)" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
-    <orderEntry type="module" module-name="autora-darts"/>
-    <orderEntry type="module" module-name="autora-core"/>
   </component>
   <component name="PackageRequirementsSettings">
     <option name="requirementsPath" value=""/>
   </component>
   <component name="PyDocumentationSettings">
     <option name="format" value="GOOGLE"/>
     <option name="myDocStringFormat" value="Google"/>
```

### Comparing `autora-3.0.0a9/.idea/inspectionProfiles/Project_Default.xml` & `autora-3.0.0rc2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a9/.pre-commit-config.yaml` & `autora-3.0.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a9/LICENSE.md` & `autora-3.0.0rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a9/docs/experimentalists/index.md` & `autora-3.0.0rc2/docs/experimentalist/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 ![Overview](../img/experimentalist.png)
 
 Experimentalists may use information about candidate models $M$ obtained from a theorist, 
 experiment conditions that have already been probed $\vec{x}' \in X'$, or 
 respective dependent measures $\vec{y}' \in Y'$. The following table includes the experimentalists currently implemented
  in AutoRA.
 
-| Experimentalist  | Function                                                                                                                      | Arguments  |
-|------------------|-------------------------------------------------------------------------------------------------------------------------------|------------|
-| Random           | $\vec{x_i} \sim U[a_i,b_i]$                                                                                                   |            |
-| Novelty          | $\underset{\vec{x}}{\arg\max}~\min(d(\vec{x}, \vec{x}'))$                                                                     | $X'$       |
-| Least Confident  | $\underset{\vec{x}}{\arg\max}~1 - P_M(\hat{y}^*, \vec{x})$, $\hat{y}^* = \underset{\hat{y}}{\arg\max}~P_M(\hat{y}_i \vec{x})$ | $M$        |
-| Model Comparison | $\underset{\vec{x}}{\argmax}~(P_{M_1}(\hat{y}, \vec{x}) - P_{M_2}(\hat{y} \vec{x}))^2$                                        | $M$        |
-| Falsification    | $\underset{\vec{x}}{\argmax}~\hat{\mathcal{L}}(M,X',Y',\vec{x})$                                                              | $M, X', Y'$ |
+| Experimentalist  | Function                                                                                                                      | Arguments   |
+|------------------|-------------------------------------------------------------------------------------------------------------------------------|-------------|
+| Random           | $\vec{x_i} \sim U[a_i,b_i]$                                                                                                   |             |
+| Novelty          | $\underset{\vec{x}}{\arg\max}~\min(d(\vec{x}, \vec{x}'))$                                                                     | $X'$        |
+| Least Confident  | $\underset{\vec{x}}{\arg\max}~1 - P_M(\hat{y}^*, \vec{x})$, $\hat{y}^* = \underset{\hat{y}}{\arg\max}~P_M(\hat{y}_i \vec{x})$ | $M$         |
+| Model Comparison | $\underset{\vec{x}}{\arg\max}~(P_{M_1}(\hat{y}, \vec{x}) - P_{M_2}(\hat{y} \vec{x}))^2$                                       | $M$         |
+| Falsification    | $\underset{\vec{x}}{\arg\max}~\hat{\mathcal{L}}(M,X',Y',\vec{x})$                                                             | $M, X', Y'$ |
```

### Comparing `autora-3.0.0a9/docs/img/logo.png` & `autora-3.0.0rc2/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a9/docs/img/overview.png` & `autora-3.0.0rc2/docs/img/overview.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a9/docs/index.md` & `autora-3.0.0rc2/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a9/docs/theorist/index.md` & `autora-3.0.0rc2/docs/theorist/index.md`

 * *Files identical despite different names*

