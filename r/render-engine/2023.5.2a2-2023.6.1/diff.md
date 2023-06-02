# Comparing `tmp/render_engine-2023.5.2a2.tar.gz` & `tmp/render_engine-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.5.2a2.tar", last modified: Thu May 18 14:36:44 2023, max compression
+gzip compressed data, was "render_engine-2023.6.1.tar", last modified: Fri Jun  2 06:02:09 2023, max compression
```

## Comparing `render_engine-2023.5.2a2.tar` & `render_engine-2023.6.1.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.664371 render_engine-2023.5.2a2/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.664371 render_engine-2023.5.2a2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/assets/render-engine-init-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/building-your-site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/creating-your-app.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.672371 render_engine-2023.5.2a2/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.672371 render_engine-2023.5.2a2/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.672371 render_engine-2023.5.2a2/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.672371 render_engine-2023.5.2a2/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/create_app_check_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/create_app_check_file_no_site_vars.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-02 06:01:54.000000 render_engine-2023.6.1/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-02 06:02:09.176831 render_engine-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-02 06:01:54.000000 render_engine-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-06-02 06:01:54.000000 render_engine-2023.6.1/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-02 06:01:54.000000 render_engine-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-02 06:01:54.000000 render_engine-2023.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 06:02:09.176831 render_engine-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_site.py
```

### Comparing `render_engine-2023.5.2a2/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.6.1/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/.devcontainer/devcontainer.json` & `render_engine-2023.6.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.6.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/.github/CONTRIBUTION.md` & `render_engine-2023.6.1/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/.github/FUNDING.yml` & `render_engine-2023.6.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/.github/LICENSE` & `render_engine-2023.6.1/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/.github/dependabot.yml` & `render_engine-2023.6.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/.github/workflows/publish.yml` & `render_engine-2023.6.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/.gitignore` & `render_engine-2023.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/PKG-INFO` & `render_engine-2023.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.5.2a2
+Version: 2023.6.1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.5.2a2/README.md` & `render_engine-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/changelog.md` & `render_engine-2023.6.1/changelog.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/archive.md` & `render_engine-2023.6.1/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/assets/create-app-help.png` & `render_engine-2023.6.1/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/assets/render-engine-init-help.png` & `render_engine-2023.6.1/docs/docs/assets/render-engine-init-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/assets/render-engine-init.png` & `render_engine-2023.6.1/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/cli.md` & `render_engine-2023.6.1/docs/docs/cli.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/contributing/pages.md` & `render_engine-2023.6.1/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/custom_collections.md` & `render_engine-2023.6.1/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/getting-started/building-your-site.md` & `render_engine-2023.6.1/docs/docs/getting-started/building-your-site.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.6.1/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.6.1/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/getting-started/installation.md` & `render_engine-2023.6.1/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/getting-started/layout.md` & `render_engine-2023.6.1/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/index.md` & `render_engine-2023.6.1/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/page.md` & `render_engine-2023.6.1/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/parsers.md` & `render_engine-2023.6.1/docs/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/docs/templates.md` & `render_engine-2023.6.1/docs/docs/templates.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/docs/mkdocs.yml` & `render_engine-2023.6.1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/pyproject.toml` & `render_engine-2023.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/requirements.txt` & `render_engine-2023.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/.DS_Store` & `render_engine-2023.6.1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/.DS_Store` & `render_engine-2023.6.1/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/_base_object.py` & `render_engine-2023.6.1/src/render_engine/_base_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Shared Properties and methods across render_engine objects."""
 
 from slugify import slugify
 
+from .hookspecs import register_plugins
+
 
 class BaseObject:
     """
     Shared properties for render_engine objects.
 
     This ensures that the behavior around the title, slug, and path_name are consistent
 
     This is not intended to be used directly.
     """
 
     title: str
     template_vars: dict
+    plugins: list
 
     @property
     def _title(self) -> str:
         """
         The title of the Page
         If no title is provided, use the class name.
         """
@@ -67,11 +70,20 @@
             "url": self.url_for(),
         }
 
         # Pull out template_vars
         if hasattr(self, "template_vars"):
             for key, value in self.template_vars.items():
                 base_dict[key] = value
-
-            base_dict.pop("template_vars")
         
         return base_dict
+
+
+    def register_plugins(self, plugins):
+        """Creates the plugin manager and registers plugins"""
+
+        if getattr('self', 'plugins', None):
+            self.plugins.extend(plugins)
+        else:
+            self.plugins = plugins
+
+        self._pm = register_plugins(self.plugins)
```

### Comparing `render_engine-2023.5.2a2/src/render_engine/archive.py` & `render_engine-2023.6.1/src/render_engine/archive.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/blog.py` & `render_engine-2023.6.1/src/render_engine/blog.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from .collection import Collection
 from .feeds import RSSFeed
-from .page import Page
 from .parsers.markdown import MarkdownPageParser
 
 
-class BlogPost(Page):
-    """Page Like object with slight modifications to work with BlogPosts."""
-    invalid_attrs = ["slug"]
-
-
 class Blog(Collection):
     """
     Custom :py:class:`collection.Collection` class with archiving enabled, sort by `date` by default.
 
-    Todos:
+    TODOS:
         - Add Support for JSON Feeds
         - Rename the archive items so they are not private
     """
 
     BasePageParser = MarkdownPageParser
-    content_type: BlogPost = BlogPost
     sort_reverse: bool = True
     sort_by = "date"
     has_archive = True
     Feed = RSSFeed
+
+    def latest(self, count: int = 1):
+        """Get the latest post from the collection."""
+        latest_pages = list(sorted(
+            self.__iter__(),
+            key=lambda x:getattr(x, self.sort_by),
+            reverse=self.sort_reverse))[0:count]
+        return latest_pages
```

### Comparing `render_engine-2023.5.2a2/src/render_engine/cli.py` & `render_engine-2023.6.1/src/render_engine/cli.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/collection.py` & `render_engine-2023.6.1/src/render_engine/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,25 +68,22 @@
     sort_by: str = "title"
     sort_reverse: bool = False
     template: str | None
     plugins: list[typing.Callable] | None
 
     def __init__(
         self,
-        plugins: list[typing.Callable] = [],
     ) -> None:
 
         self.has_archive = any(
             [
                 hasattr(self, "archive_template"),
                 getattr(self, "items_per_page", None),
             ]
         )
-        self.plugins = [*getattr(self, "plugins", []), *plugins]
-        self.PM = register_plugins(plugins=self.plugins)
         self.title = self._title
 
     def iter_content_path(self):
         """Iterate through in the collection's content path."""
 
         return flatten(
             [
@@ -118,16 +115,18 @@
             self,
             content_path:str|None=None,
     ) -> type[Page]:
         """Returns the page Object for the specified Content Path"""
         _page = self.content_type(
             content_path=content_path,
             Parser=self.PageParser,
-            plugins=self.plugins,
         )
+
+        if getattr(self, '_pm', None):
+            _page.register_plugins(self.plugins)
         _page.parser_extras = getattr(self, "parser_extras", {})
         _page.routes = self.routes
         _page.template = getattr(self, "template", None)
         _page.collection_vars = self.to_dict()
         return _page
 
     @property
```

### Comparing `render_engine-2023.5.2a2/src/render_engine/engine.py` & `render_engine-2023.6.1/src/render_engine/engine.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/feeds.py` & `render_engine-2023.6.1/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/hookspecs.py` & `render_engine-2023.6.1/src/render_engine/hookspecs.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/links.py` & `render_engine-2023.6.1/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/page.py` & `render_engine-2023.6.1/src/render_engine/page.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any, Type, Callable
 
 import jinja2
 
 from ._base_object import BaseObject
-from .hookspecs import register_plugins
 from .parsers.base_parsers import BasePageParser
 
 
 class BasePage(BaseObject):
     """
     This is the Base Page object.
 
@@ -122,17 +121,14 @@
         reference: 
             Used to determine how to reference the page in the `Site`'s route_list.
             Defaults to `slug`.
         routes: The routes to use for the page. Defaults to `["./"]`.
         template: 
             The template used to render the page.
             If not provided, the `Site`'s `content` will be used.
-        invalid_attrs: 
-            A list of attributes that are not valid for the page.
-            Defaults to `["slug", "content"]`. See [Invalid Attrs][invalid-attrs].
         Parser: 
             The parser to generate the page's `raw_content`.
             Defaults to `BasePageParser`.
         title: The title of the page. Defaults to the class name.
 
     """
 
@@ -165,16 +161,11 @@
             attrs = {}
             self.content = None
 
         # Set the attributes
         for key, val in attrs.items():
             setattr(self, key.lower(), val)
 
-        # Set the plugins
-        self.plugins = [*getattr(self, "plugins", []), *plugins]
-        self.PM = register_plugins(self.plugins)
-        self.PM.hook.render_content(Page=self) # type: ignore pluggy doesn't expose hook
-
     @property
     def _content(self):
         """Returns the content of the page."""
         return self.Parser.parse(self.content, page=self)
```

### Comparing `render_engine-2023.5.2a2/src/render_engine/parsers/.DS_Store` & `render_engine-2023.6.1/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.6.1/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.6.1/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.6.1/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/plugins.py` & `render_engine-2023.6.1/src/render_engine/plugins.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.6.1/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.6.1/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.6.1/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.6.1/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/src/render_engine/site.py` & `render_engine-2023.6.1/src/render_engine/site.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     engine: Environment = engine
 
 
     def __init__(
         self,
         plugins: list[str] = [],
     ) -> None:
-        self._route_list = dict()
+        self.route_list = dict()
         self.subcollections = defaultdict(lambda: {"pages": []})
         self.engine.globals.update(self.site_vars)
         self.plugins = [*plugins, *getattr(self, "plugins", [])]
         self._pm = register_plugins(plugins=self.plugins)
 
     def collection(self, Collection: type[Collection]) -> Collection:
         """
@@ -78,17 +78,18 @@
 
         class Posts(Collection):
             pass
 
         site.collection(Posts) # also works
         ```
         """
-        _Collection = Collection(plugins=self.plugins)
+        _Collection = Collection()
+        _Collection.register_plugins(self.plugins)
         self._pm.hook.pre_build_collection(collection=_Collection) #type: ignore
-        self._route_list[_Collection._slug] = _Collection
+        self.route_list[_Collection._slug] = _Collection
         return _Collection
 
     def page(self, Page: Page) -> Page:
         """
         Add the page to the route list to be rendered later.
         Also remaps `title` in case the user wants to use it in the template rendering.
 
@@ -109,18 +110,18 @@
 
         class About(Page):
             pass
 
         site.page(About) # also works
         ```
         """
-        page = Page(plugins=self.plugins)
+        page = Page()
         page.title = page._title # Expose _title to the user through `title`
-        self._route_list[getattr(page, page._reference)] = page
-        return page
+        page.register_plugins(self.plugins)
+        self.route_list[getattr(page, page._reference)] = page
 
     def _render_static(self) -> None:
         """Copies a Static Directory to the output folder"""
         shutil.copytree(
             self.static_path,
             pathlib.Path(self.output_path) / pathlib.Path(self.static_path).name,
             dirs_exist_ok=True
@@ -137,14 +138,15 @@
         return path.write_text(
             page._render_content(engine=self.engine)
         )
 
     def _render_partial_collection(self, collection: Collection) -> None:
         """Iterate through the Changed Pages and Check for Collections and Feeds"""
         for entry in collection._generate_content_from_modified_pages():
+            entry._pm.hook.render_content(Page=entry)
             for route in collection.routes:
                 self._render_output(route, entry)
 
         if collection.has_archive:
             for archive in collection.archives:
                 logging.debug("Adding Archive: %s", archive.__class__.__name__)
 
@@ -153,14 +155,15 @@
         if hasattr(collection, "Feed"):
             self._render_output("./", collection._feed)
 
     def _render_full_collection(self, collection: Collection) -> None:
         """Iterate through Pages and Check for Collections and Feeds"""
 
         for entry in collection:
+            entry._pm.hook.render_content(Page=entry)
             for route in collection.routes:
                 self._render_output(route, entry)
 
         if collection.has_archive:
             for archive in collection.archives:
                 logging.debug("Adding Archive: %s", archive.__class__.__name__)
 
@@ -186,27 +189,29 @@
         with Progress() as progress:
 
             pre_build_task = progress.add_task("Loading Pre-Build Plugins", total=1)
             self._pm.hook.pre_build_site(site=self)
 
             # Parse Route List
             task_add_route = progress.add_task(
-                "[blue]Adding Routes", total=len(self._route_list)
+                "[blue]Adding Routes", total=len(self.route_list)
             )
 
             if pathlib.Path(self.static_path).exists():
                 self._render_static()
             self.engine.globals["site"] = self
-            self.engine.globals["routes"] = self._route_list
+            self.engine.globals["routes"] = self.route_list
 
-            for slug, entry in self._route_list.items():
+            for slug, entry in self.route_list.items():
                 progress.update(
                     task_add_route, description=f"[blue]Adding[gold]Route: [blue]{slug}"
                 )
                 if isinstance(entry, Page):
+                    if getattr(entry, "collection", None):
+                        entry._pm.hook.render_content(Page=entry)
                     for route in entry.routes:
                         progress.update(
                             task_add_route,
                             description=f"[blue]Adding[gold]Route: [blue]{entry._slug}",
                         )
                         self._render_output(route, entry)
```

### Comparing `render_engine-2023.5.2a2/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.6.1/src/render_engine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine
-Version: 2023.5.2a2
+Version: 2023.6.1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.5.2a2/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.6.1/src/render_engine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -91,11 +91,12 @@
 tests/test_base_parser.py
 tests/test_blog.py
 tests/test_collections.py
 tests/test_create_app.py
 tests/test_feeds.py
 tests/test_page.py
 tests/test_parser_markdown_parser.py
+tests/test_plugins.py
 tests/test_site.py
 tests/site_test/build.py
 tests/site_test/blog/test_blog_content.md
 tests/site_test/templates/index.html
```

### Comparing `render_engine-2023.5.2a2/tests/conftest.py` & `render_engine-2023.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/tests/create_app_check_file.txt` & `render_engine-2023.6.1/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/tests/test_base_object.py` & `render_engine-2023.6.1/tests/test_base_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,10 +56,11 @@
         self.test_object.template_vars = {"test": "test"}
 
         assert self.test_object.to_dict() == {
             "title": "TestObject",
             "slug": "testobject",
             "url": None,
             "test": "test",
+            'template_vars': {'test': 'test'},
         }
 
         assert self.test_object.template_vars == {"test": "test"}
```

### Comparing `render_engine-2023.5.2a2/tests/test_base_parser.py` & `render_engine-2023.6.1/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/tests/test_collections.py` & `render_engine-2023.6.1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/tests/test_create_app.py` & `render_engine-2023.6.1/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/tests/test_feeds.py` & `render_engine-2023.6.1/tests/test_feeds.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,21 +53,21 @@
     collection = BasicCollection()
 
     assert collection._feed.title == "BasicCollection"
 
 
 def test_rss_feed_item_url(site):
     """Test that the feed item url is set correctly"""
-    assert "<link>http://localhost:8000/page.html</link>" in site._route_list['testcollection']._feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
+    assert "<link>http://localhost:8000/page.html</link>" in site.route_list['testcollection']._feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
 
 
 
 def test_rss_feed_item_has_guid(site):
     """Test that the feed item url is set correctly"""
-    assert '<guid isPermaLink="true">http://localhost:8000/page.html</guid>' in site._route_list['testcollection']._feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
+    assert '<guid isPermaLink="true">http://localhost:8000/page.html</guid>' in site.route_list['testcollection']._feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
 
 
 @pytest.mark.skip("Invalid Test")
 def test_rss_feed_template_with_strictundefined(engine, tmp_path):
     """Test that the RSS feed template works with the StrictUndefined undefined handler."""
     tmp_dir = tmp_path / "content"
     tmp_dir.mkdir()
```

### Comparing `render_engine-2023.5.2a2/tests/test_page.py` & `render_engine-2023.6.1/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a2/tests/test_site.py` & `render_engine-2023.6.1/tests/test_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,60 +47,60 @@
     tmp_dir.mkdir()
     file = tmp_dir / "test.md"
     file.write_text("test")
 
     site = Site()
 
     # assert that the route list is empty
-    assert len(site._route_list) == 0
+    assert len(site.route_list) == 0
 
     class CustomPage(Page):
         test_value = "test"
         content_path = file.absolute()
 
     site.page(CustomPage)
 
-    assert site._route_list["custompage"].test_value == "test"
+    assert site.route_list["custompage"].test_value == "test"
 
 
 def test_site_collection_in_route_list():
     """Tests that when a collection is added to the route_list it is only the colleciton"""
     site = Site()
 
     # assert that the route list is empty
-    assert len(site._route_list) == 0
+    assert len(site.route_list) == 0
 
     class CustomPage1(Page):
         pass
 
 
     class CustomPage2(Page):
         pass
 
     class collection(Collection):
         pages = [CustomPage1(), CustomPage2()]
 
     collection = site.collection(collection)
 
-    assert site._route_list["collection"] == collection
-    assert len(site._route_list) == 1
-    assert 'custompage1' in [getattr(page, page._reference) for page in site._route_list["collection"]]
+    assert site.route_list["collection"] == collection
+    assert len(site.route_list) == 1
+    assert 'custompage1' in [getattr(page, page._reference) for page in site.route_list["collection"]]
 
 
 def test_site_page_with_multiple_routes_has_one_entry_in_routes_list():
     """Tests a page with multiple routes only has one entry in the routes list"""
     site = Site()
 
     class CustomPage(Page):
         test_value = "test"
         routes = ["customroute", "customroute2"]
 
     site.page(CustomPage)
 
-    assert len(site._route_list) == 1
+    assert len(site.route_list) == 1
 
 def test_url_for_Page_in_site(tmp_path):
     """Tests that url_for a page is added to a template"""
     test_template = pathlib.Path(tmp_path / "template.html")
     test_template.write_text("The URL is '{{ 'custompage'|url_for }}'")
     site = Site()
     site.engine.loader.loaders.insert(0, FileSystemLoader(tmp_path))
@@ -135,15 +135,15 @@
 
     @site.collection
     class CustomCollection(Collection):
         archive_template = test_collection_archive_template.name
         has_archive = True
         pages = [CustomCollectionPage()]
 
-    print(site._route_list)
+    print(site.route_list)
 
     site.render()
     print(list(tmp_path.iterdir()))
     assert pathlib.Path(tmp_path / "customcollection.html").exists()
     assert pathlib.Path(tmp_path / "customcollectionpage.html").exists()
     assert pathlib.Path(tmp_path / "customcollection.html").read_text() == "This is the collection archive"
     assert pathlib.Path(tmp_path / "customcollectionpage.html").read_text() == "The collection archive route is at '/customcollection.html'"
```

