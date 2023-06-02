# Comparing `tmp/bulma_sphinx_theme-0.0.7.tar.gz` & `tmp/bulma_sphinx_theme-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.0.7.tar", last modified: Wed May 31 04:20:28 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.0.8.tar", last modified: Fri Jun  2 03:42:54 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.0.7.tar` & `bulma_sphinx_theme-0.0.8.tar`

### file list

```diff
@@ -1,195 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:28.299621 bulma_sphinx_theme-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/typography.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/mult_headers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/text-formatting.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subpage2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage3.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/navbar.md
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/sidenav.md
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/source-buttons.md
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_api.scss
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_code.scss
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_bulma.scss
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_leaflet.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/pygment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/webpack.config.js
--rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:54.791115 bulma_sphinx_theme-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/typography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/mult_headers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/text-formatting.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subpage2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/navbar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/source-buttons.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_edit-page.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_code.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_bulma.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_leaflet.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/last update.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/pygment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/webpack.config.js
+-rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.8/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.0.7/LICENSE` & `bulma_sphinx_theme-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/README.md` & `bulma_sphinx_theme-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/_static/favicon.png` & `bulma_sphinx_theme-0.0.8/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/_static/logo.svg` & `bulma_sphinx_theme-0.0.8/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/conf.py` & `bulma_sphinx_theme-0.0.8/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,21 @@
         },
     ],
     "source_repository": "https://github.com/zclab/bulma-sphinx-theme",
     "source_branch": "main",
     "source_directory": "docs/",
     "use_edit_page_button": True,
     "fix_navbar": True,
+    "information_panel": [],
     "navbar_start": [],
-    "navbar_end": ["navbar-nav.html", "header-icons.html"],
+    "navbar_end": ["navbar-nav.html", "theme-swither.html", "header-icons.html"],
     "have_top_navbar": True,
+    "light_colors": {
+        "bst-color-background-sidenav": "rgb(240, 248, 255)",
+    },
 }
 
 html_context = {"default_mode": "auto"}
 
 # blog_path = "blog"
 # blog_post_pattern = "posts/*/*"
 # blog_authors = {
```

### Comparing `bulma_sphinx_theme-0.0.7/docs/develop.md` & `bulma_sphinx_theme-0.0.8/docs/develop.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/index.md` & `bulma_sphinx_theme-0.0.8/docs/examples/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/mult_headers.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/mult_headers.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.0.8/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subpage1.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subpage2.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage1.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage2.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage3.rst` & `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage3.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/user_guide/navbar.md` & `bulma_sphinx_theme-0.0.8/docs/user_guide/navbar.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/user_guide/source-buttons.md` & `bulma_sphinx_theme-0.0.8/docs/user_guide/source-buttons.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/docs/web-components.rst` & `bulma_sphinx_theme-0.0.8/docs/web-components.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/noxfile.py` & `bulma_sphinx_theme-0.0.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/package-lock.json` & `bulma_sphinx_theme-0.0.8/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/package.json` & `bulma_sphinx_theme-0.0.8/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/pyproject.toml` & `bulma_sphinx_theme-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/__init__.py` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from . import pygment, toctree, transforms, utils
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 logger = logging.getLogger(__name__)
 MESSAGE_CATALOG_NAME = "bulmasphinxtheme"
 
 
 def _get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
@@ -46,19 +46,14 @@
     assert isinstance(app.builder, StandaloneHTMLBuilder)
 
     if "css_files" in context:
         _add_asset_hashes(
             context["css_files"],
             ["styles/bulma-sphinx-theme.css"],
         )
-    if "scripts" in context:
-        _add_asset_hashes(
-            context["scripts"],
-            ["scripts/bulma-sphinx-theme.js"],
-        )
 
     # determine the startdepth for building the theme
     theme_options = utils.get_theme_options(app)
     have_navbar = theme_options.get("have_top_navbar", True)
     if not isinstance(have_navbar, bool):
         have_navbar = True
     context["start_depth"] = int(have_navbar)
```

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/base/_typography.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/_typography.scss`

 * *Files 22% similar despite different names*

```diff
@@ -106,46 +106,31 @@
     &::before {
       margin-right: 0.25rem;
       vertical-align: middle;
     }
   }
 
   &.reference.download::before {
-    content: url("data:image/svg+xml;charset=utf-8,%3Csvg width='16' height='16' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2 -2v-2'/%3E%3Cpath d='M7 11l5 5l5 -5'/%3E%3Cpath d='M12 4l0 12'/%3E%3C/svg%3E");
+    content: "";
+    mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' width='16' height='16'%3E%3Cpath d='M2.75 14A1.75 1.75 0 0 1 1 12.25v-2.5a.75.75 0 0 1 1.5 0v2.5c0 .138.112.25.25.25h10.5a.25.25 0 0 0 .25-.25v-2.5a.75.75 0 0 1 1.5 0v2.5A1.75 1.75 0 0 1 13.25 14Z'%3E%3C/path%3E%3Cpath d='M7.25 7.689V2a.75.75 0 0 1 1.5 0v5.689l1.97-1.969a.749.749 0 1 1 1.06 1.06l-3.25 3.25a.749.749 0 0 1-1.06 0L4.22 6.78a.749.749 0 1 1 1.06-1.06l1.97 1.969Z'%3E%3C/path%3E%3C/svg%3E");
+    width: 1.1rem;
+    height: 1.1rem;
+    background-color: var(--bst-color-text-base);
+    display: inline-block;
+    mask-repeat: no-repeat;
   }
-}
-
-svg {
-  &.svg-bulma,
-  &.svg-github,
-  &.svg-gitlab,
-  &.svg-home,
-  &.svg-pencil,
-  &.svg-file-description,
-  &.svg-clock-edit,
-  &.svg-search,
-  &.svg-package,
-  &.svg-sun,
-  &.svg-sunset,
-  &.svg-moon {
-    width: 100%;
-    height: 100%;
-  }
-}
 
-html[data-theme="dark"] {
-  svg {
-    &.svg-github,
-    &.svg-gitlab,
-    &.svg-home,
-    &.svg-pencil,
-    &.svg-file-description,
-    &.svg-clock-edit,
-    &.svg-search,
-    &.svg-package,
-    &.svg-sun,
-    &.svg-sunset,
-    &.svg-moon {
-      filter: hue-rotate(40deg) saturate(0.5) brightness(390%) saturate(4);
+  &.github,
+  &.gitlab {
+    &::before {
+      vertical-align: middle;
+      margin-right: 0.25rem;
+      content: "";
+      mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' width='16' height='16'%3E%3Cpath d='M2 2.5A2.5 2.5 0 0 1 4.5 0h8.75a.75.75 0 0 1 .75.75v12.5a.75.75 0 0 1-.75.75h-2.5a.75.75 0 0 1 0-1.5h1.75v-2h-8a1 1 0 0 0-.714 1.7.75.75 0 1 1-1.072 1.05A2.495 2.495 0 0 1 2 11.5Zm10.5-1h-8a1 1 0 0 0-1 1v6.708A2.486 2.486 0 0 1 4.5 9h8ZM5 12.25a.25.25 0 0 1 .25-.25h3.5a.25.25 0 0 1 .25.25v3.25a.25.25 0 0 1-.4.2l-1.45-1.087a.249.249 0 0 0-.3 0L5.4 15.7a.25.25 0 0 1-.4-.2Z'%3E%3C/path%3E%3C/svg%3E");
+      width: 1.1rem;
+      height: 1.1rem;
+      background-color: var(--bst-color-text-base);
+      display: inline-block;
+      mask-repeat: no-repeat;
     }
   }
 }
```

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_api.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_api.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_code.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_code.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss`

 * *Files 6% similar despite different names*

```diff
@@ -123,13 +123,18 @@
       height: 100%;
       width: 100%;
     }
   }
 
   .reference {
     &.external:after {
-      content: url("data:image/svg+xml;charset=utf-8,%3Csvg width='16' height='16' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M11 7H6a2 2 0 0 0-2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2-2v-5M10 14 20 4M15 4h5v5'/%3E%3C/svg%3E");
+      content: "";
       margin-left: 0.3rem;
-      vertical-align: middle;
+      mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='13.5' height='13.5' aria-hidden='true' viewBox='0 0 24 24' class='iconExternalLink_Rdzz'%3E%3Cpath fill='currentColor' d='M21 13v10h-21v-19h12v2h-10v15h17v-8h2zm3-12h-10.988l4.035 4-6.977 7.07 2.828 2.828 6.977-7.07 4.125 4.172v-11z'%3E%3C/path%3E%3C/svg%3E");
+      width: 0.8rem;
+      height: 0.8rem;
+      background-color: var(--bst-color-text-base);
+      display: inline-block;
+      mask-repeat: no-repeat;
     }
   }
 }
```

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .bulma-tocnav {
-  width: var(--tocnav-width);
   padding: 0 1rem;
   word-break: break-word;
 
   .toc-wrapper {
     position: sticky;
     top: calc(var(--navbar-height) + var(--top-content-to-navbar-gap));
     overflow-y: auto;
```

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_color.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_color.scss`

 * *Files 2% similar despite different names*

```diff
@@ -76,18 +76,14 @@
     ),
   // on_surface: object on top of surface object (without shadows)
   "on-surface":
     (
       "light": rgb(225, 225, 225),
       "dark": rgb(55, 55, 55),
     ),
-  "background-sidenav": (
-    "light": rgb(240, 248, 255),
-    "dark": rgb(18, 18, 18),
-  ),
   "background-info-panel": (
     "light": linear-gradient(0.25turn, #e3e5f7, #d9e1ef, #e8ebfb),
     "dark": linear-gradient(0.25turn, #5e605a, #51544e, #5a5c58),
   ),
   "canvas": (
     "light": rgb(246, 248, 250),
     "dark": rgb(22, 27, 34),
@@ -115,14 +111,15 @@
       --bst-color-#{$name}: #{$value};
     }
   }
 
   // assign the "duplicate" colors (ones that just reference other variables)
   & {
     --bst-color-link-hover: var(--bst-color-warning);
+    --bst-color-background-sidenav: var(--bst-color-background);
   }
 
   // adapt to light/dark-specific content
   @if $mode == "light" {
     .only-dark,
     .only-dark ~ figcaption {
       display: none !important;
```

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/pygment.py` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/pygment.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 
 {#- Hide breadcrumbs on the home page #}
 {% if title and pagename != root_doc %}
 <nav class="breadcrumb" aria-label="breadcrumbs">
     <ul>
         <li>
             <a href="{{ pathto(root_doc) }}" title="home">
-                <svg class="svg-home">
-                    <use href="#svg-home"></use>
-                </svg>
+                <span class="icon">
+                    <svg class="svg-home">
+                        <use href="#svg-home"></use>
+                    </svg>
+                </span>
             </a>
         </li>
         {%- for doc in parents %}
         {% if doc.link %}
         <li><a href="{{ doc.link|e }}">{{ doc.title }}</a></li>
         {% else %}
         <li><a href="#">{{ doc.title }}</a></li>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 {%- block breadcrumbs %} {# If we have more than 3 parents (excluding the home
 page) then we remove The ones in the middle and add an ellipsis. This code is
 from https://github.com/pydata/pydata-sphinx-theme/blob/main/src/
 pydata_sphinx_theme/theme/pydata_sphinx_theme/components/breadcrumbs.html #} {#
 djlint:off #} {% if parents|length>2 %} {% set parents=[parents[0], {"title":
 '•••'}, parents[-1]] %} {% endif %} {# djlint:on #} {#- Hide breadcrumbs on the
 home page #} {% if title and pagename != root_doc %}
-    * __
+    * ____
     * {%- for doc in parents %} {% if doc.link %}
     * {{_doc.title_}}
     * {% else %}
     * {{_doc.title_}}
     * {% endif %} {%- endfor %}
     * {{ title }}
  {% endif %} {%- endblock %}
```

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf`

 * *Files 25% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 show_nav_level = 1
 show_toc_level = 1
 header_links_before_dropdown = 4
 external_links =
 header_icons =
 logo =
 fix_navbar =
+# see https://pygments.org/styles/ for more styles
 pygment_light_style = manni
 pygment_dark_style = material
 
-# see navbar color styles: https://bulma.io/documentation/components/navbar/#colors
+# see https://bulma.io/documentation/components/navbar/#colors for more navbar color styles
 navbar_color_style = is-white
 navbar_start = navbar-nav.html
 navbar_end = header-icons.html
 navbar_include_directly = navbar-nav.html, header-icons.html
 analytics =
 footer = copyright.html, sphinx-version.html
 toc_title = On this page
@@ -38,10 +39,12 @@
 article_bottom_right = sourcelink.html
 use_edit_page_button =
 source_repository =
 source_branch =
 source_directory =
 source_edit_link =
 show_prev_next = True
-css_variables =
-dark_css_variables =
 information_panel = theme-swither.html
+# define css variables
+light_colors =
+dark_colors =
+css_variables =
```

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/toctree.py` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/toctree.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/transforms.py` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/transforms.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/translations.py` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/translations.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.7/webpack.config.js` & `bulma_sphinx_theme-0.0.8/webpack.config.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -14,39 +14,29 @@
     exec
 } = require("child_process");
 exec("python src/bulma_sphinx_theme/translations.py");
 
 const scriptPath = resolve(__dirname, "src/bulma_sphinx_theme/assets/scripts");
 const stylePath = resolve(__dirname, "src/bulma_sphinx_theme/assets/styles");
 const staticPath = resolve(__dirname, "src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static");
-const vendorPath = resolve(staticPath, "vendor");
 
 /*******************************************************************************
  * functions to load the assets in the html head
  * the css, and js (preload/scripts) are digested for cache busting
  * the fonts are loaded from vendors
  */
 
-function stylesheet(css) {
-    return `<link href="{{ pathto('_static/${css}', 1) }}?digest=${this.hash}" rel="stylesheet" />`;
-}
-
 function preload(js) {
     return `<link rel="preload" as="script" href="{{ pathto('_static/${js}', 1) }}?digest=${this.hash}" />`;
 }
 
 function script(js) {
     return `<script src="{{ pathto('_static/${js}', 1) }}?digest=${this.hash}"></script>`;
 }
 
-function font(woff2) {
-    return `<link rel="preload" as="font" type="font/woff2" crossorigin href="{{ pathto('_static/${woff2}', 1) }}" />`;
-}
-
-
 /*******************************************************************************
  * the assets to load in the macro
  */
 const theme_scripts = [
     "scripts/bulma-sphinx-theme.js",
 ];
```

### Comparing `bulma_sphinx_theme-0.0.7/PKG-INFO` & `bulma_sphinx_theme-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulma-sphinx-theme
-Version: 0.0.7
+Version: 0.0.8
 Summary: A sphinx theme based on bulma.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.7 Summary: A sphinx
+Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.8 Summary: A sphinx
 theme based on bulma. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

