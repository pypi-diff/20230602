# Comparing `tmp/plopp-23.4.0.tar.gz` & `tmp/plopp-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plopp-23.4.0.tar", last modified: Tue Apr 11 12:29:14 2023, max compression
+gzip compressed data, was "plopp-23.5.0.tar", last modified: Fri Jun  2 13:20:16 2023, max compression
```

## Comparing `plopp-23.4.0.tar` & `plopp-23.5.0.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.617212 plopp-23.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.577211 plopp-23.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-11 12:28:58.000000 plopp-23.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-11 12:28:58.000000 plopp-23.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-11 12:28:58.000000 plopp-23.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-04-11 12:28:58.000000 plopp-23.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-04-11 12:28:58.000000 plopp-23.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-11 12:28:58.000000 plopp-23.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-11 12:28:58.000000 plopp-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-04-11 12:29:14.617212 plopp-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-04-11 12:28:58.000000 plopp-23.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-04-11 12:28:58.000000 plopp-23.4.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/_static/gallery/
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/gallery/README.txt
--rw-r--r--   0 runner    (1001) docker     (122)    18766 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (122)    66718 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (122)    76253 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/_templates/sections/header-article.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.581211 plopp-23.4.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/faq.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/about/reference/
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/reference/matplotlib.rst
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/reference/plotly.rst
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/reference/pythreejs.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/about/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/basics/
--rw-r--r--   0 runner    (1001) docker     (122)     5402 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/image-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4446 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/inspector-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/line-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/saving-figures.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/scatter3d-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/slicer-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2984 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/basics/super-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     9238 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/customization/
--rw-r--r--   0 runner    (1001) docker     (122)     5080 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/customization/subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/customization/tweaking-figures.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (122)    19809 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/custom-interfaces.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/examples/gallery/
--rw-r--r--   0 runner    (1001) docker     (122)     4574 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/masking-a-range.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/nyc-taxi.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     6988 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/rectangle-selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/scatter3d-with-slider.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery/scatter3d-with-threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/examples/gallery.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.585211 plopp-23.4.0/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/getting-started/numpy-pandas-xarray.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     8677 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/getting-started/overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-04-11 12:28:58.000000 plopp-23.4.0/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-04-11 12:28:58.000000 plopp-23.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.589211 plopp-23.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/mini.in
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/mini.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/noplotly.in
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/noplotly.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-04-11 12:28:58.000000 plopp-23.4.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.589211 plopp-23.4.0/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    53363 2023-04-11 12:28:58.000000 plopp-23.4.0/resources/logo-plopp-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-11 12:29:14.617212 plopp-23.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.573211 plopp-23.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.589211 plopp-23.4.0/src/plopp/
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.593212 plopp-23.4.0/src/plopp/backends/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.593212 plopp-23.4.0/src/plopp/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12570 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     5557 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2586 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/interactive.py
--rw-r--r--   0 runner    (1001) docker     (122)     8124 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/line.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/static.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/matplotlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.593212 plopp-23.4.0/src/plopp/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/plotly/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/plotly/figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/plotly/line.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.597211 plopp-23.4.0/src/plopp/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8089 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/outline.py
--rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/backends/pythreejs/point_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.597211 plopp-23.4.0/src/plopp/core/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/limits.py
--rw-r--r--   0 runner    (1001) docker     (122)     7013 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/node.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/system.py
--rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/core/view.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.601211 plopp-23.4.0/src/plopp/data/
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/data/examples.py
--rw-r--r--   0 runner    (1001) docker     (122)     6098 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/data/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/data/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.601211 plopp-23.4.0/src/plopp/functions/
--rw-r--r--   0 runner    (1001) docker     (122)      284 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6627 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3566 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/inspector.py
--rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     4517 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/slicer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6129 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/functions/superplot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.605212 plopp-23.4.0/src/plopp/graphics/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/basefig.py
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/camera.py
--rw-r--r--   0 runner    (1001) docker     (122)     9762 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/colormapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/figimage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/figline.py
--rw-r--r--   0 runner    (1001) docker     (122)     6637 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/figscatter3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/graphics/figure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.609212 plopp-23.4.0/src/plopp/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1830 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/checkboxes.py
--rw-r--r--   0 runner    (1001) docker     (122)    11209 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/cut3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/drawing.py
--rw-r--r--   0 runner    (1001) docker     (122)     3619 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/slice.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/style.py
--rw-r--r--   0 runner    (1001) docker     (122)     3935 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-04-11 12:28:58.000000 plopp-23.4.0/src/plopp/widgets/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.593212 plopp-23.4.0/src/plopp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-11 12:29:14.000000 plopp-23.4.0/src/plopp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.609212 plopp-23.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.577211 plopp-23.4.0/tests/backends/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.609212 plopp-23.4.0/tests/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (122)     2745 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_figimage_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_figline_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_image_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_interactive_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/matplotlib/mpl_line_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.609212 plopp-23.4.0/tests/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/plotly/plotly_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      649 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/plotly/plotly_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/plotly/plotly_line_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.613211 plopp-23.4.0/tests/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (122)     8670 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/pythreejs/pythreejs_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/pythreejs/pythreejs_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.613211 plopp-23.4.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/graph_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2675 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/limits_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5717 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/node_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.613211 plopp-23.4.0/tests/functions/
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/common_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/inspector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     9973 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/plot_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/scatter3d_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/slicer_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/functions/superplot_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.617212 plopp-23.4.0/tests/graphics/
--rw-r--r--   0 runner    (1001) docker     (122)     5308 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/graphics/colormapper_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4461 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/graphics/figimage_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5911 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/graphics/figline_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/graphics/figscatter3d_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/high_level_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/minimal_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:29:14.617212 plopp-23.4.0/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     2602 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/widgets/box_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/widgets/checkboxes_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/widgets/cut3d_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-04-11 12:28:58.000000 plopp-23.4.0/tests/widgets/slice_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-04-11 12:28:58.000000 plopp-23.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-02 13:20:03.000000 plopp-23.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-02 13:20:03.000000 plopp-23.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-06-02 13:20:03.000000 plopp-23.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-06-02 13:20:03.000000 plopp-23.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-02 13:20:03.000000 plopp-23.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-06-02 13:20:03.000000 plopp-23.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-06-02 13:20:03.000000 plopp-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-06-02 13:20:16.969053 plopp-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-06-02 13:20:03.000000 plopp-23.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-02 13:20:03.000000 plopp-23.5.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/_static/gallery/
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/gallery/README.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    18766 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (122)    66718 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (122)    76253 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_templates/sections/header-article.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/faq.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/about/reference/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/reference/matplotlib.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/reference/plotly.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/reference/pythreejs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/basics/
+-rw-r--r--   0 runner    (1001) docker     (122)     5402 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/image-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4446 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/inspector-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/line-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/saving-figures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/scatter3d-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/slicer-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2984 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/super-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/customization/
+-rw-r--r--   0 runner    (1001) docker     (122)     5080 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/customization/subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/customization/tweaking-figures.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)    19809 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/custom-interfaces.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/examples/gallery/
+-rw-r--r--   0 runner    (1001) docker     (122)     4574 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/masking-a-range.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/nyc-taxi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     7022 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/rectangle-selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/scatter3d-with-slider.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/scatter3d-with-threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/getting-started/numpy-pandas-xarray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     8677 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/getting-started/overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-06-02 13:20:03.000000 plopp-23.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/mini.in
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/mini.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/noplotly.in
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/noplotly.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    53363 2023-06-02 13:20:03.000000 plopp-23.5.0/resources/logo-plopp-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-06-02 13:20:16.973053 plopp-23.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.945051 plopp-23.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/src/plopp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/src/plopp/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/src/plopp/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15050 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7828 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/plotly/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/plotly/figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/plotly/line.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8550 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/outline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/point_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/limits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7013 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/system.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/view.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/data/examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6098 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/data/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)      284 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6624 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3566 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4895 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7017 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6129 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/superplot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.965052 plopp-23.5.0/src/plopp/graphics/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/basefig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/camera.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10419 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/colormapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/figimage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5760 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/figline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6224 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/figscatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/figure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.965052 plopp-23.5.0/src/plopp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1830 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/checkboxes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11209 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/cut3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3619 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/slice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/style.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3935 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/src/plopp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.965052 plopp-23.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.945051 plopp-23.5.0/tests/backends/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.965052 plopp-23.5.0/tests/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_figimage_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_figline_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_interactive_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_line_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (122)     2308 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/plotly/plotly_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/plotly/plotly_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/plotly/plotly_line_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/pythreejs/pythreejs_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/pythreejs/pythreejs_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2675 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/limits_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5717 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/inspector_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10161 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/plot_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/scatter3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4027 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/slicer_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/superplot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/graphics/
+-rw-r--r--   0 runner    (1001) docker     (122)     8472 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/graphics/colormapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4461 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/graphics/figimage_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6317 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/graphics/figline_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/graphics/figscatter3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/high_level_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/minimal_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     2602 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/widgets/box_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/widgets/checkboxes_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/widgets/cut3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/widgets/slice_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-06-02 13:20:03.000000 plopp-23.5.0/tox.ini
```

### Comparing `plopp-23.4.0/.github/workflows/ci.yml` & `plopp-23.5.0/.github/workflows/ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   formatting:
     name: Formatting and static analysis
     runs-on: ubuntu-20.04
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.9
+          python-version: '3.10'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e static
       - uses: stefanzweifel/git-auto-commit-action@v4
         with:
           commit_message: Apply automatic formatting
 
@@ -33,16 +33,20 @@
     name: Tests
     needs: formatting
     runs-on: ubuntu-20.04
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.9
+          python-version: '3.10'
       - run: sudo apt install --yes graphviz graphviz-dev
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox
 
   docs:
     needs: tests
     uses: ./.github/workflows/docs.yml
+    with:
+      publish: false
+      version: ${{ github.ref_name }}
+      branch: ${{ github.head_ref == '' && github.ref_name || github.head_ref }}
```

### Comparing `plopp-23.4.0/.github/workflows/docs.yml` & `plopp-23.5.0/.github/workflows/docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -9,54 +9,65 @@
       publish:
         default: false
         type: boolean
       version:
         default: ''
         required: false
         type: string
+      branch:
+        description: 'Branch/tag with documentation source. If not set, the current branch will be used.'
+        default: ''
+        required: false
+        type: string
   workflow_call:
     inputs:
       publish:
         default: false
         type: boolean
       version:
         default: ''
         required: false
         type: string
+      branch:
+        description: 'Branch/tag with documentation source. If not set, the current branch will be used.'
+        default: ''
+        required: false
+        type: string
 
 env:
   VERSION: ${{ inputs.version }}
 
 jobs:
   docs:
     name: Build documentation
     runs-on: ubuntu-20.04
     steps:
       - run: sudo apt install --yes graphviz pandoc
       - uses: actions/checkout@v3
         with:
-          ref: ${{ inputs.version }}
+          ref: ${{ inputs.branch == '' && github.ref_name || inputs.branch }}
           fetch-depth: 0  # history required so setuptools_scm can determine version
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.9
+          python-version: '3.10'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: |
+          python -m pip cache remove plopp
           tox --skip-pkg-install -e docs -- plopp==${VERSION}
-          echo "target=$(python docs/version.py --repo=plopp --version=${VERSION} --action=get-target)" >> $GITHUB_ENV
+          echo "target=$(python docs/version.py --version=${VERSION} --action=get-target)" >> $GITHUB_ENV
         if: ${{ inputs.publish }}
       - run: tox -e docs
         if: ${{ !inputs.publish }}
       - uses: actions/upload-artifact@v3
         with:
           name: html
           path: html/
 
-      - uses: JamesIves/github-pages-deploy-action@v4.4.1
+      - uses: JamesIves/github-pages-deploy-action@v4.4.2
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
           target-folder: ${{ env.target }}
           single-commit: true
           clean-exclude: release
```

### Comparing `plopp-23.4.0/.github/workflows/release.yml` & `plopp-23.5.0/.github/workflows/release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -14,97 +14,100 @@
 
 jobs:
   build_conda:
     name: Conda build
     runs-on: ubuntu-20.04
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           submodules: true
           fetch-depth: 0  # history required so cmake can determine version
 
       - uses: conda-incubator/setup-miniconda@v2
       - run: conda install -c conda-forge --yes conda-build boa
       - run: conda mambabuild --channel conda-forge --channel scipp --python=3.8 --no-anaconda-upload --override-channels --output-folder conda/package conda
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         with:
           name: conda-package-noarch
           path: conda/package/*/plopp*.tar.bz2
 
   build_wheels:
     name: Wheels
     runs-on: ubuntu-20.04
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.9
+          python-version: '3.10'
 
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/wheels.txt
 
       - name: Build wheels
         run: python -m build
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: dist
           path: dist
 
   upload_packages:
     name: Deploy packages
     needs: [build_conda, build_wheels]
     runs-on: ubuntu-20.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
       - uses: conda-incubator/setup-miniconda@v2
+        with:
+          python-version: '3.10'
       - run: conda install -c conda-forge --yes anaconda-client
       - run: anaconda --token ${{ secrets.ANACONDATOKEN }} upload --user scipp --label main $(ls conda-package-*/*/*.tar.bz2)
       - uses: actions/setup-python@v3
 
-      - uses: pypa/gh-action-pypi-publish@v1.8.5
+      - uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
 
   manage-versions:
     name: Manage Versions
     runs-on: ubuntu-20.04
     outputs:
       version-new: ${{ steps.version.outputs.new }}
       version-replaced: ${{ steps.version.outputs.replaced }}
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.9
+          python-version: '3.10'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - name: Set outputs
         id: version
         run: |
-          echo "::set-output name=new::$(python docs/version.py --repo=plopp --version=${GITHUB_REF_NAME} --action=is-new)"
-          echo "::set-output name=replaced::$(python docs/version.py --repo=plopp --version=${GITHUB_REF_NAME} --action=get-replaced)"
+          echo "new=$(python docs/version.py --version=${GITHUB_REF_NAME} --action=is-new)" >> $GITHUB_OUTPUT
+          echo "replaced=$(python docs/version.py --version=${GITHUB_REF_NAME} --action=get-replaced)" >> $GITHUB_OUTPUT
 
   replaced-docs:
     needs: [upload_packages, manage-versions]
     if: github.event_name == 'release' && github.event.action == 'published' && needs.manage-versions.outputs.version-new == 'True'
     uses: ./.github/workflows/docs.yml
     with:
       publish: true
       version: ${{ needs.manage-versions.outputs.version-replaced }}
+      branch: ${{ needs.manage-versions.outputs.version-replaced }}
     secrets: inherit
 
   docs:
     needs: upload_packages
     uses: ./.github/workflows/docs.yml
     with:
       publish: ${{ github.event_name == 'release' && github.event.action == 'published' }}
```

### Comparing `plopp-23.4.0/.pre-commit-config.yaml` & `plopp-23.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/LICENSE` & `plopp-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/PKG-INFO` & `plopp-23.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 23.4.0
+Version: 23.5.0
 Summary: Plotting library based on scipp
 Home-page: https://scipp.github.io/plopp
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/plopp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `plopp-23.4.0/README.md` & `plopp-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/conda/meta.yaml` & `plopp-23.5.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/_static/favicon.ico` & `plopp-23.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png` & `plopp-23.5.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png` & `plopp-23.5.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/_static/logo.svg` & `plopp-23.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/_templates/scipp-class-template.rst` & `plopp-23.5.0/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/_templates/scipp-module-template.rst` & `plopp-23.5.0/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/_templates/sections/header-article.html` & `plopp-23.5.0/docs/_templates/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/about/about.rst` & `plopp-23.5.0/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/about/faq.ipynb` & `plopp-23.5.0/docs/about/faq.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/about/reference.rst` & `plopp-23.5.0/docs/about/reference.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/basics/image-plot.ipynb` & `plopp-23.5.0/docs/basics/image-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/basics/inspector-plot.ipynb` & `plopp-23.5.0/docs/basics/inspector-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/basics/line-plot.ipynb` & `plopp-23.5.0/docs/basics/line-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/basics/saving-figures.ipynb` & `plopp-23.5.0/docs/basics/saving-figures.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/basics/scatter3d-plot.ipynb` & `plopp-23.5.0/docs/basics/scatter3d-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/basics/slicer-plot.ipynb` & `plopp-23.5.0/docs/basics/slicer-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/basics/super-plot.ipynb` & `plopp-23.5.0/docs/basics/super-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/conf.py` & `plopp-23.5.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         {
             "type": "group",
             "buttons": l1,
             "icon": "fa fa-caret-down",
             "text": "Related projects",
         }
     )
-    releases = version_info.minor_releases(first='0.1')
+    releases = version_info.minor_releases(first='23.3')
     if outdated:
         current = f"{long_version} (outdated)"
         latest = "latest"
         entries = ['.'.join(long_version.split('.')[:2])]
     else:
         current = f"{long_version} (latest)"
         latest = f"{releases[0]} (latest)"
```

### Comparing `plopp-23.4.0/docs/customization/subplots.ipynb` & `plopp-23.5.0/docs/customization/subplots.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/customization/tweaking-figures.ipynb` & `plopp-23.5.0/docs/customization/tweaking-figures.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/examples/custom-interfaces.ipynb` & `plopp-23.5.0/docs/examples/custom-interfaces.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/examples/gallery/masking-a-range.ipynb` & `plopp-23.5.0/docs/examples/gallery/masking-a-range.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/examples/gallery/nyc-taxi.ipynb` & `plopp-23.5.0/docs/examples/gallery/nyc-taxi.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/examples/gallery/rectangle-selection.ipynb` & `plopp-23.5.0/docs/examples/gallery/rectangle-selection.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997829861111112%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(27, "            \'dim\': '*

 * *            'figure.canvas.dims[\'x\'],\\n"), (28, "            \'left\': sc.scalar(artist.xy[0], '*

 * *            'unit=figure.canvas.units[\'x\']),\\n"), (29, "            \'right\': '*

 * *            'sc.scalar(artist.xy[0] + artist.width, unit=figure.canvas.units[\'x\']),\\n"), (32, '*

 * *            '"            \'dim\': figure.canvas.dims[\'y\'],\\n"), (33, "            \'bottom\': '*

 * *            'sc.scalar(artist.xy[1], unit=figure.canvas.unit […]*

```diff
@@ -109,22 +109,22 @@
                 "def _get_rect_info(artist, figure):\n",
                 "    \"\"\"\n",
                 "    Convert the raw rectangle info to a dict containing the dimensions of\n",
                 "    each axis, and values with units.\n",
                 "    \"\"\"\n",
                 "    return lambda: {\n",
                 "        'x': {\n",
-                "            'dim': figure.dims['x'],\n",
-                "            'left': sc.scalar(artist.xy[0], unit=figure.canvas.xunit),\n",
-                "            'right': sc.scalar(artist.xy[0] + artist.width, unit=figure.canvas.xunit),\n",
+                "            'dim': figure.canvas.dims['x'],\n",
+                "            'left': sc.scalar(artist.xy[0], unit=figure.canvas.units['x']),\n",
+                "            'right': sc.scalar(artist.xy[0] + artist.width, unit=figure.canvas.units['x']),\n",
                 "        },\n",
                 "        'y': {\n",
-                "            'dim': figure.dims['y'],\n",
-                "            'bottom': sc.scalar(artist.xy[1], unit=figure.canvas.yunit),\n",
-                "            'top': sc.scalar(artist.xy[1] + artist.height, unit=figure.canvas.yunit),\n",
+                "            'dim': figure.canvas.dims['y'],\n",
+                "            'bottom': sc.scalar(artist.xy[1], unit=figure.canvas.units['y']),\n",
+                "            'top': sc.scalar(artist.xy[1] + artist.height, unit=figure.canvas.units['y']),\n",
                 "        },\n",
                 "    }\n",
                 "\n",
                 "\n",
                 "RectangleTool = partial(\n",
                 "    DrawingTool, tool=Rectangles, get_artist_info=_get_rect_info, icon='vector-square'\n",
                 ")"
```

### Comparing `plopp-23.4.0/docs/examples/gallery/scatter3d-with-slider.ipynb` & `plopp-23.5.0/docs/examples/gallery/scatter3d-with-slider.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/examples/gallery/scatter3d-with-threshold.ipynb` & `plopp-23.5.0/docs/examples/gallery/scatter3d-with-threshold.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/examples/gallery.ipynb` & `plopp-23.5.0/docs/examples/gallery.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/getting-started/numpy-pandas-xarray.ipynb` & `plopp-23.5.0/docs/getting-started/numpy-pandas-xarray.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/getting-started/overview.ipynb` & `plopp-23.5.0/docs/getting-started/overview.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/index.rst` & `plopp-23.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/docs/version.py` & `plopp-23.5.0/docs/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import git
 from packaging.version import InvalidVersion, Version, parse
 
 
 def _get_releases() -> List[Version]:
     """Return reversed sorted list of release tag names."""
-    tags = git.Repo('..').tags
+    tags = git.Repo(search_parent_directories=True).tags
     versions = []
     for t in tags:
         try:
             versions.append(parse(t.name))
         except InvalidVersion:
             pass
     return sorted(versions, reverse=True)
```

### Comparing `plopp-23.4.0/pyproject.toml` & `plopp-23.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,8 +38,9 @@
 filterwarnings = [
   "error",
   "ignore::UserWarning",
   'ignore:\n            Sentinel is not a public part of the traitlets API:DeprecationWarning',
   'ignore:Auto-removal of grids by pcolor:matplotlib._api.deprecation.MatplotlibDeprecationWarning',
   'ignore:Jupyter is migrating its paths:DeprecationWarning',
   'ignore:Passing unrecognized arguments to super:DeprecationWarning',
-  'ignore:distutils Version classes are deprecated:DeprecationWarning',]
+  'ignore:distutils Version classes are deprecated:DeprecationWarning',
+  'ignore:setDaemon\(\) is deprecated, set the daemon attribute instead:DeprecationWarning',]
```

### Comparing `plopp-23.4.0/requirements/base.txt` & `plopp-23.5.0/requirements/base.txt`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     # via -r requirements/base.in
 pyyaml==6.0
     # via confuse
 pyzmq==25.0.2
     # via
     #   ipykernel
     #   jupyter-client
-scipp==23.3.1
+scipp==23.3.2
     # via -r requirements/base.in
 six==1.16.0
     # via
     #   asttokens
     #   python-dateutil
 stack-data==0.6.2
     # via ipython
```

### Comparing `plopp-23.4.0/requirements/ci.txt` & `plopp-23.5.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/requirements/docs.txt` & `plopp-23.5.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/requirements/mini.txt` & `plopp-23.5.0/requirements/mini.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     # via pytest
 pluggy==1.0.0
     # via pytest
 pytest==7.2.2
     # via -r requirements/mini.in
 pyyaml==6.0
     # via confuse
-scipp==23.3.1
+scipp==23.3.2
     # via -r requirements/mini.in
 tomli==2.0.1
     # via pytest
```

### Comparing `plopp-23.4.0/requirements/static.txt` & `plopp-23.5.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/requirements/test.txt` & `plopp-23.5.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/resources/logo-plopp-2022.svg` & `plopp-23.5.0/resources/logo-plopp-2022.svg`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/setup.cfg` & `plopp-23.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/__init__.py` & `plopp-23.5.0/src/plopp/__init__.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/manager.py` & `plopp-23.5.0/src/plopp/backends/manager.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/matplotlib/__init__.py` & `plopp-23.5.0/src/plopp/backends/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/matplotlib/canvas.py` & `plopp-23.5.0/src/plopp/backends/matplotlib/canvas.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import scipp as sc
 from matplotlib.collections import QuadMesh
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 from ...core.limits import find_limits, fix_empty_range
-from ...core.utils import maybe_variable_to_number
+from ...core.utils import maybe_variable_to_number, scalar_to_string
 from .utils import fig_to_bytes, is_sphinx_build, silent_mpl_figure
 
 
 def _none_if_not_finite(x):
     return x if np.isfinite(x) else None
 
 
@@ -42,14 +42,18 @@
         The minimum value for the vertical axis. If a number (without a unit) is
         supplied, it is assumed that the unit is the same as the current vertical axis
         unit.
     vmax:
         The maximum value for the vertical axis. If a number (without a unit) is
         supplied, it is assumed that the unit is the same as the current vertical axis
         unit.
+    autoscale:
+        The behavior of the axis limits. If ``auto``, the limits automatically
+        adjusts every time the data changes. If ``grow``, the limits are allowed to
+        grow with time but they do not shrink.
     aspect:
         The aspect ratio for the axes.
     cbar:
         Add axes to host a colorbar if ``True``.
     """
 
     def __init__(
@@ -57,14 +61,15 @@
         ax: plt.Axes = None,
         cax: plt.Axes = None,
         figsize: Optional[Tuple[float, float]] = None,
         title: str = None,
         grid: bool = False,
         vmin: Union[sc.Variable, int, float] = None,
         vmax: Union[sc.Variable, int, float] = None,
+        autoscale: Literal['auto', 'grow'] = 'auto',
         aspect: Literal['auto', 'equal'] = 'auto',
         cbar: bool = False,
         **ignored,
     ):
         # Note on the `**ignored`` keyword arguments: the figure which owns the canvas
         # creates both the canvas and an artist object (Line or Image). The figure
         # accepts keyword arguments, and has to somehow forward them to the canvas and
@@ -75,17 +80,18 @@
         # artist, and filter out the artist kwargs with `**ignored`.
 
         self.fig = None
         self.ax = ax
         self.cax = cax
         self._user_vmin = vmin
         self._user_vmax = vmax
-        self.xunit = None
-        self.yunit = None
+        self.units = {}
+        self.dims = {}
         self._own_axes = False
+        self._autoscale = autoscale
 
         if self.ax is None:
             self._own_axes = True
             with silent_mpl_figure():
                 self.fig, self.ax = plt.subplots(
                     figsize=(6.0, 4.0) if figsize is None else figsize
                 )
@@ -98,14 +104,15 @@
         if cbar and self.cax is None:
             divider = make_axes_locatable(self.ax)
             self.cax = divider.append_axes("right", "4%", pad="5%")
 
         self.ax.set_aspect(aspect)
         self.ax.set_title(title)
         self.ax.grid(grid)
+        self._coord_formatters = []
 
         self._xmin = np.inf
         self._xmax = np.NINF
         self._ymin = np.inf
         self._ymax = np.NINF
 
     def is_widget(self):
@@ -136,18 +143,19 @@
             Make a draw call to the figure if ``True``.
         """
         if self.ax.lines:
             self.ax.relim()
             self.ax.autoscale()
             xmin, xmax = self.ax.get_xlim()
             ymin, ymax = self.ax.get_ylim()
-            self._xmin = min(self._xmin, xmin)
-            self._xmax = max(self._xmax, xmax)
-            self._ymin = min(self._ymin, ymin)
-            self._ymax = max(self._ymax, ymax)
+        else:
+            xmin = np.inf
+            xmax = np.NINF
+            ymin = np.inf
+            ymax = np.NINF
         for c in self.ax.collections:
             if isinstance(c, QuadMesh):
                 coords = c.get_coordinates()
                 left, right = fix_empty_range(
                     find_limits(
                         sc.array(dims=['x', 'y'], values=coords[..., 0]),
                         scale=self.xscale,
@@ -155,22 +163,32 @@
                 )
                 bottom, top = fix_empty_range(
                     find_limits(
                         sc.array(dims=['x', 'y'], values=coords[..., 1]),
                         scale=self.yscale,
                     )
                 )
-                self._xmin = min(self._xmin, left.value)
-                self._xmax = max(self._xmax, right.value)
-                self._ymin = min(self._ymin, bottom.value)
-                self._ymax = max(self._ymax, top.value)
+                xmin = min(xmin, left.value)
+                xmax = max(xmax, right.value)
+                ymin = min(ymin, bottom.value)
+                ymax = max(ymax, top.value)
+        if self._autoscale == 'grow':
+            self._xmin = min(self._xmin, xmin)
+            self._xmax = max(self._xmax, xmax)
+            self._ymin = min(self._ymin, ymin)
+            self._ymax = max(self._ymax, ymax)
+        else:
+            self._xmin = xmin
+            self._xmax = xmax
+            self._ymin = ymin
+            self._ymax = ymax
         if self._user_vmin is not None:
-            self._ymin = maybe_variable_to_number(self._user_vmin, unit=self.yunit)
+            self._ymin = maybe_variable_to_number(self._user_vmin, unit=self.units['y'])
         if self._user_vmax is not None:
-            self._ymax = maybe_variable_to_number(self._user_vmax, unit=self.yunit)
+            self._ymax = maybe_variable_to_number(self._user_vmax, unit=self.units['y'])
 
         self.ax.set_xlim(
             _none_if_not_finite(self._xmin), _none_if_not_finite(self._xmax)
         )
         self.ax.set_ylim(
             _none_if_not_finite(self._ymin), _none_if_not_finite(self._ymax)
         )
@@ -210,20 +228,79 @@
         ----------
         **limits:
             Min and max limits for each dimension to be cropped.
         """
         for xy, lims in limits.items():
             getattr(self.ax, f'set_{xy}lim')(
                 *[
-                    maybe_variable_to_number(lims[m], unit=getattr(self, f'{xy}unit'))
+                    maybe_variable_to_number(lims[m], unit=self.units[xy])
                     for m in ('min', 'max')
                     if m in lims
                 ]
             )
 
+    def set_axes(self, dims, units):
+        """
+        Set the axes dimensions and units.
+
+        Parameters
+        ----------
+        dims:
+            The dimensions of the data.
+        units:
+            The units of the data.
+        """
+        self.units = units
+        self.dims = dims
+        self._cursor_x_placeholder = sc.scalar(0.0, unit=self.units['x'])
+        self._cursor_y_placeholder = sc.scalar(0.0, unit=self.units['y'])
+        self._cursor_x_prefix = ''
+        self._cursor_y_prefix = ''
+        if 'y' in self.dims:
+            self._cursor_x_prefix = self.dims['x'] + '='
+            self._cursor_y_prefix = self.dims['y'] + '='
+        self.ax.format_coord = self.format_coord
+
+    def register_format_coord(self, formatter):
+        """
+        Register a custom axis formatter for the x-axis.
+        """
+        self._coord_formatters.append(formatter)
+
+    def format_coord(self, x: float, y: float) -> str:
+        """
+        Format the coordinates of the mouse pointer to show the value of the
+        data at that point.
+
+        Parameters
+        ----------
+        x:
+            The x coordinate of the mouse pointer.
+        y:
+            The y coordinate of the mouse pointer.
+        """
+        self._cursor_x_placeholder.value = x
+        self._cursor_y_placeholder.value = y
+        out = (
+            f"({self._cursor_x_prefix}{scalar_to_string(self._cursor_x_placeholder)}, "
+            f"{self._cursor_y_prefix}{scalar_to_string(self._cursor_y_placeholder)})"
+        )
+        extra = [formatter(x, y) for formatter in self._coord_formatters]
+        extra = [e for e in extra if e is not None]
+        if extra:
+            out += ": {" + ", ".join(extra) + "}"
+        return out
+
+    @property
+    def empty(self) -> bool:
+        """
+        Check if the canvas is empty.
+        """
+        return not self.dims
+
     @property
     def title(self) -> str:
         """
         Get or set the title of the plot.
         """
         return self.ax.get_title()
```

### Comparing `plopp-23.4.0/src/plopp/backends/matplotlib/image.py` & `plopp-23.5.0/src/plopp/backends/matplotlib/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
 
 import numpy as np
 import scipp as sc
 
-from ...core.utils import coord_as_bin_edges, merge_masks, repeat
+from ...core.utils import coord_as_bin_edges, merge_masks, repeat, scalar_to_string
 from .canvas import Canvas
 
 
 def _find_dim_of_2d_coord(coords):
     for xy, coord in coords.items():
         if coord['var'].ndim == 2:
             return (xy, coord['dim'])
@@ -91,20 +91,22 @@
         # call pcolormesh, because that turns the grid off automatically.
         # See https://github.com/matplotlib/matplotlib/issues/15600.
         need_grid = self._ax.xaxis.get_gridlines()[0].get_visible()
 
         to_dim_search = {}
         string_labels = {}
         bin_edge_coords = {}
+        self._data_with_bin_edges = sc.DataArray(data=self._data.data)
         for i, k in enumerate('yx'):
             to_dim_search[k] = {
                 'dim': self._data.dims[i],
                 'var': self._data.meta[self._data.dims[i]],
             }
             bin_edge_coords[k] = coord_as_bin_edges(self._data, self._data.dims[i])
+            self._data_with_bin_edges.coords[self._data.dims[i]] = bin_edge_coords[k]
             if self._data.meta[self._data.dims[i]].dtype == str:
                 string_labels[k] = self._data.meta[self._data.dims[i]]
 
         self._dim_1d, self._dim_2d = _get_dims_of_1d_and_2d_coords(to_dim_search)
         self._mesh = None
 
         x, y, z = _from_data_array_to_pcolormesh(
@@ -126,14 +128,39 @@
         for xy, var in string_labels.items():
             getattr(self._ax, f'set_{xy}ticks')(np.arange(float(var.shape[0])))
             getattr(self._ax, f'set_{xy}ticklabels')(var.values)
 
         if need_grid:
             self._ax.grid(True)
 
+        # Cache slicing order for hover values
+        if self._dim_1d is not None:
+            # If there is a 2d coord, we first slice the 1d coord, and then the
+            # dimension that is left should also be 1d, making value-based slicing
+            # possible.
+            self._hover_slicing = {
+                'dir': (self._dim_1d[0], self._dim_2d[0]),
+                'dim': (self._dim_1d[1], self._dim_2d[1]),
+                'unit': (
+                    self._data.coords[self._dim_1d[1]].unit,
+                    self._data.coords[self._dim_2d[1]].unit,
+                ),
+            }
+        else:
+            self._hover_slicing = {
+                'dir': ('y', 'x'),
+                'dim': (self._data.dims[0], self._data.dims[1]),
+                'unit': (
+                    self._data.coords[self._data.dims[0]].unit,
+                    self._data.coords[self._data.dims[1]].unit,
+                ),
+            }
+
+        self._canvas.register_format_coord(self.format_coord)
+
     @property
     def data(self):
         """
         Get the Mesh's data in a form that may have been tweaked, compared to the
         original data, in the case of a two-dimensional coordinate.
         """
         out = sc.DataArray(
@@ -171,7 +198,42 @@
 
         Parameters
         ----------
         new_values:
             New data to update the mesh values from.
         """
         self._data = new_values
+
+    def format_coord(self, x: float, y: float) -> str:
+        """
+        Format the coordinates of the mouse pointer to show the value of the
+        data at that point.
+
+        Parameters
+        ----------
+        x:
+            The x coordinate of the mouse pointer.
+        y:
+            The y coordinate of the mouse pointer.
+        """
+        xy = {'x': x, 'y': y}
+        try:
+            val = self._data_with_bin_edges[
+                self._hover_slicing['dim'][0],
+                sc.scalar(
+                    xy[self._hover_slicing['dir'][0]],
+                    unit=self._hover_slicing['unit'][0],
+                ),
+            ]
+            val = val[
+                self._hover_slicing['dim'][1],
+                sc.scalar(
+                    xy[self._hover_slicing['dir'][1]],
+                    unit=self._hover_slicing['unit'][1],
+                ),
+            ]
+            prefix = self._data.name
+            if prefix:
+                prefix += ': '
+            return prefix + scalar_to_string(val)
+        except IndexError:
+            return None
```

### Comparing `plopp-23.4.0/src/plopp/backends/matplotlib/interactive.py` & `plopp-23.5.0/src/plopp/backends/matplotlib/interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,18 +55,14 @@
         return self._fig.canvas
 
     @property
     def artists(self):
         return self._fig.artists
 
     @property
-    def dims(self):
-        return self._fig.dims
-
-    @property
     def graph_nodes(self):
         return self._fig.graph_nodes
 
     @property
     def id(self):
         return self._fig.id
```

### Comparing `plopp-23.4.0/src/plopp/backends/matplotlib/line.py` & `plopp-23.5.0/src/plopp/backends/matplotlib/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,16 +201,16 @@
         new_values:
             New data to update the line values, masks, errorbars from.
         """
         self._data = new_values
         new_values = self._make_data()
 
         self._line.set_data(new_values['values']['x'], new_values['values']['y'])
+        self._mask.set_data(new_values['mask']['x'], new_values['mask']['y'])
         if new_values['mask']['visible']:
-            self._mask.set_data(new_values['mask']['x'], new_values['mask']['y'])
             self._mask.set_visible(True)
         else:
             self._mask.set_visible(False)
 
         if (self._error is not None) and (new_values['stddevs'] is not None):
             coll = self._error.get_children()[0]
             coll.set_segments(
```

### Comparing `plopp-23.4.0/src/plopp/backends/matplotlib/static.py` & `plopp-23.5.0/src/plopp/backends/matplotlib/static.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/matplotlib/utils.py` & `plopp-23.5.0/src/plopp/backends/matplotlib/utils.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/plotly/__init__.py` & `plopp-23.5.0/src/plopp/backends/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/plotly/canvas.py` & `plopp-23.5.0/src/plopp/backends/plotly/canvas.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/plotly/figure.py` & `plopp-23.5.0/src/plopp/backends/plotly/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/plotly/line.py` & `plopp-23.5.0/src/plopp/backends/plotly/line.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/pythreejs/__init__.py` & `plopp-23.5.0/src/plopp/backends/pythreejs/__init__.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/pythreejs/canvas.py` & `plopp-23.5.0/src/plopp/backends/pythreejs/canvas.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,17 +34,16 @@
         self,
         figsize: Tuple[int, int] = (600, 400),
         title: Optional[str] = None,
         camera: Optional[Camera] = None,
     ):
         import pythreejs as p3
 
-        self.xunit = None
-        self.yunit = None
-        self.zunit = None
+        self.dims = {}
+        self.units = {}
         self.outline = None
         self.axticks = None
         self.figsize = np.asarray(figsize)
         self._title_text = title
         self._title = self._make_title()
         width, height = self.figsize
         self._user_camera = Camera() if camera is None else camera
@@ -63,14 +62,28 @@
             width=width,
             height=height,
         )
 
     def to_widget(self):
         return self.renderer
 
+    def set_axes(self, dims, units):
+        """
+        Set the axes dimensions and units.
+
+        Parameters
+        ----------
+        dims:
+            The dimensions of the data.
+        units:
+            The units of the data.
+        """
+        self.units = units
+        self.dims = dims
+
     def make_outline(self, limits: Tuple[sc.Variable, sc.Variable, sc.Variable]):
         """
         Create an outline box with ticklabels, given a range in the XYZ directions.
         """
         from .outline import Outline
 
         if self.outline is not None:
@@ -85,15 +98,17 @@
         Update the camera position when a new object is added to the canvas.
         The camera will look at the mean position of all the objects, and its position
         will be far enough from the center to see all the objects.
         This 'Home' position will be backed up so it can be used when resetting the
         camera via the ``home`` function.
         """
         if not self._user_camera.has_units():
-            self._user_camera.set_units(self.xunit, self.yunit, self.zunit)
+            self._user_camera.set_units(
+                self.units.get('x'), self.units.get('y'), self.units.get('z')
+            )
 
         center = [var.mean().value for var in limits]
         distance_fudge_factor = 1.2
         box_size = np.array([(limits[i][1] - limits[i][0]).value for i in range(3)])
         self.camera.position = self._user_camera.get(
             'position', list(np.array(center) + distance_fudge_factor * box_size)
         )
@@ -128,14 +143,21 @@
         ]
         self.camera_backup["z_normal"] = [
             center[0],
             center[1],
             center[2] - distance_fudge_factor * box_mean_size,
         ]
 
+    @property
+    def empty(self) -> bool:
+        """
+        Check if the canvas is empty.
+        """
+        return not self.dims
+
     def home(self):
         """
         Reset the camera position.
         """
         self.move_camera(
             position=self.camera_backup["reset"], look_at=self.camera_backup["look_at"]
         )
```

### Comparing `plopp-23.4.0/src/plopp/backends/pythreejs/figure.py` & `plopp-23.5.0/src/plopp/backends/pythreejs/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/pythreejs/outline.py` & `plopp-23.5.0/src/plopp/backends/pythreejs/outline.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/backends/pythreejs/point_cloud.py` & `plopp-23.5.0/src/plopp/backends/pythreejs/point_cloud.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/core/graph.py` & `plopp-23.5.0/src/plopp/core/graph.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/core/helpers.py` & `plopp-23.5.0/src/plopp/core/helpers.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/core/limits.py` & `plopp-23.5.0/src/plopp/core/limits.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         finite_min = np.amin(finite_vals, initial=initial, where=finite_vals > 0)
     else:
         finite_min = np.amin(finite_vals)
     finite_max = np.amax(finite_vals)
     return (scalar(finite_min, unit=x.unit), scalar(finite_max, unit=x.unit))
 
 
-def fix_empty_range(lims: Tuple[Variable, ...]) -> Tuple[Variable, ...]:
+def fix_empty_range(lims: Tuple[Variable, Variable]) -> Tuple[Variable, Variable]:
     """
     Range correction in case xmin == xmax
     """
     if lims[0].value != lims[1].value:
         return lims
     if lims[0].value == 0.0:
         dx = scalar(0.5, unit=lims[0].unit)
```

### Comparing `plopp-23.4.0/src/plopp/core/node.py` & `plopp-23.5.0/src/plopp/core/node.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/core/utils.py` & `plopp-23.5.0/src/plopp/core/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         The input number or variable.
     unit:
         Convert the input to that unit if not ``None``.
     """
     if hasattr(x, 'unit'):
         if unit is not None:
             x = x.to(unit=unit)
-        x = x.values
+        x = x.values if x.dims else x.value
     return x
 
 
 def name_with_unit(var: sc.Variable, name: str = None) -> str:
     """
     Make a string from a variable dimension and its unit.
     The variable dimension can be overridden by specifying the ``name`` directly.
@@ -155,14 +155,30 @@
     else:
         text = "{}".format(val)
         if len(text) > precision + 2 + (text[0] == '-'):
             text = "{val:.{prec}f}".format(val=val, prec=precision)
     return text
 
 
+def scalar_to_string(var: sc.Variable, precision: int = 3) -> str:
+    """
+    Convert a scalar to a human readable string.
+
+    Parameters
+    ----------
+    var:
+        The input scalar.
+    precision:
+        The number of decimal places to use for the string output.
+    """
+    return value_to_string(var.value, precision=precision) + (
+        f" {var.unit}" if var.unit not in (None, "") else ""
+    )
+
+
 def merge_masks(masks: Dict[str, sc.Variable]) -> sc.Variable:
     """
     Combine all masks into a single one using the OR operation.
 
     Parameters
     ----------
     masks:
@@ -177,19 +193,17 @@
     case of a bin-edge coordinate) to a string.
 
     Parameters
     ----------
     x:
         The input variable (of length 1 or 2).
     """
-    vals = x.values
-    if vals.shape:
-        out = ':'.join([value_to_string(v) for v in vals])
-    else:
-        out = value_to_string(float(vals))
+    if not x.shape:
+        return value_to_string(x.value) + (f" [{x.unit}]" if x.unit is not None else "")
+    out = ':'.join([value_to_string(v) for v in x.values])
     if x.unit is not None:
         out += f" [{x.unit}]"
     return out
 
 
 def make_compatible(
     x: sc.Variable, *, unit: Union[str, None], dim: Optional[str] = None
```

### Comparing `plopp-23.4.0/src/plopp/core/view.py` & `plopp-23.5.0/src/plopp/core/view.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/data/examples.py` & `plopp-23.5.0/src/plopp/data/examples.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/data/factory.py` & `plopp-23.5.0/src/plopp/data/factory.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/functions/common.py` & `plopp-23.5.0/src/plopp/functions/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,29 +151,30 @@
         if isinstance(coords, str):
             coords = [coords]
         for dim in coords:
             underlying = out.meta[dim].dims[-1]
             renamed_dims[underlying] = dim
         out = out.rename_dims(**renamed_dims)
     for name, coord in out.coords.items():
-        if coord.ndim > 0:
-            try:
-                if not (
-                    _all_dims_sorted(coord, order='ascending')
-                    or _all_dims_sorted(coord, order='descending')
-                ):
-                    warnings.warn(
-                        'The input contains a coordinate with unsorted values '
-                        f'({name}). The results may be unpredictable. '
-                        'Coordinates can be sorted using '
-                        '`scipp.sort(data, dim="to_be_sorted", order="ascending")`.',
-                        UserWarning,
-                    )
-            except sc.DTypeError:
-                pass
+        if (coord.ndim == 0) or (name not in out.dims):
+            continue
+        try:
+            if not (
+                _all_dims_sorted(coord, order='ascending')
+                or _all_dims_sorted(coord, order='descending')
+            ):
+                warnings.warn(
+                    'The input contains a coordinate with unsorted values '
+                    f'({name}). The results may be unpredictable. '
+                    'Coordinates can be sorted using '
+                    '`scipp.sort(data, dim="to_be_sorted", order="ascending")`.',
+                    RuntimeWarning,
+                )
+        except sc.DTypeError:
+            pass
     return out
 
 
 def preprocess_multi(obj, **kwargs) -> List[sc.DataArray]:
     """
     Pre-process potentially multiple input data for plotting.
     See :func:`preprocess` for details.
```

### Comparing `plopp-23.4.0/src/plopp/functions/inspector.py` & `plopp-23.5.0/src/plopp/functions/inspector.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/functions/plot.py` & `plopp-23.5.0/src/plopp/functions/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ignore_size: bool = False,
     mask_color: str = 'black',
     norm: Literal['linear', 'log'] = 'linear',
     scale: Optional[Dict[str, str]] = None,
     title: Optional[str] = None,
     vmin: Optional[Union[Variable, int, float]] = None,
     vmax: Optional[Union[Variable, int, float]] = None,
+    autoscale: Literal['auto', 'grow'] = 'auto',
     **kwargs,
 ):
     """Plot a Scipp object.
 
     Parameters
     ----------
     obj:
@@ -69,14 +70,18 @@
         The figure title.
     vmin:
         Lower bound for data to be displayed (y-axis for 1d plots, colorscale for
         2d plots).
     vmax:
         Upper bound for data to be displayed (y-axis for 1d plots, colorscale for
         2d plots).
+    autoscale:
+        The behavior of the axis (1d plots) or the color range limits (2d plots).
+        If ``auto``, the limits automatically adjusts every time the data changes.
+        If ``grow``, the limits are allowed to grow with time but they do not shrink.
     **kwargs:
         All other kwargs are directly forwarded to Matplotlib, the underlying plotting
         library. The underlying functions called are the following:
 
         - 1d data with a non bin-edge coordinate: ``plot``
         - 1d data with a bin-edge coordinate: ``step``
         - 2d data: ``pcolormesh``
@@ -91,14 +96,15 @@
         'crop': crop,
         'grid': grid,
         'norm': norm,
         'scale': scale,
         'title': title,
         'vmin': vmin,
         'vmax': vmax,
+        'autoscale': autoscale,
         'figsize': figsize,
         **kwargs,
     }
 
     data_arrays = preprocess_multi(
         obj, crop=crop, ignore_size=ignore_size, coords=coords
     )
```

### Comparing `plopp-23.4.0/src/plopp/functions/scatter3d.py` & `plopp-23.5.0/src/plopp/functions/scatter3d.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/functions/superplot.py` & `plopp-23.5.0/src/plopp/functions/superplot.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/graphics/basefig.py` & `plopp-23.5.0/src/plopp/graphics/basefig.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     *nodes:
         The nodes that are attached to the view.
     """
 
     def __init__(self, *nodes):
         super().__init__(*nodes)
         self.artists = {}
-        self.dims = {}
 
     def notify_view(self, message: Dict[str, Any]):
         """
         When a notification is received, request data from the corresponding parent node
         and update the relevant artist.
 
         Parameters
```

### Comparing `plopp-23.4.0/src/plopp/graphics/camera.py` & `plopp-23.5.0/src/plopp/graphics/camera.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/graphics/colormapper.py` & `plopp-23.5.0/src/plopp/graphics/colormapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+from collections.abc import Iterable
 from copy import copy
+from functools import reduce
 from typing import Any, Literal, Optional, Tuple, Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import scipp as sc
 from matplotlib.colorbar import ColorbarBase
@@ -51,16 +53,14 @@
 
 
 class ColorMapper:
     """
     A class that handles conversion between data values and RGBA colors.
     It controls the normalization (linear or log), as well as the min and max limits
     for the color range.
-    If the min and max values are not set manually by the user, they are allowed to grow
-    with time but they do not shrink.
 
     Parameters
     ----------
     cax:
         The axes to use for the colorbar. If none are supplied, the ColorMapper will
         create its own axes.
     cbar:
@@ -71,14 +71,18 @@
         (see https://matplotlib.org/stable/tutorials/colors/colormaps.html).
         In addition to the Matplotlib docs, if the name is just a single html color,
         a colormap with that single color will be used.
     mask_cmap:
         The name of the colormap for masked data.
     norm:
         The colorscale normalization.
+    autoscale:
+        The behavior of the color range limits. If ``auto``, the limits automatically
+        adjusts every time the data changes. If ``grow``, the limits are allowed to
+        grow with time but they do not shrink.
     vmin:
         The minimum value for the colorscale range. If a number (without a unit) is
         supplied, it is assumed that the unit is the same as the data unit.
     vmax:
         The maximum value for the colorscale range. If a number (without a unit) is
         supplied, it is assumed that the unit is the same as the data unit.
     nan_color:
@@ -90,33 +94,36 @@
     def __init__(
         self,
         canvas: Optional[Any] = None,
         cbar: bool = True,
         cmap: str = 'viridis',
         mask_cmap: str = 'gray',
         norm: Literal['linear', 'log'] = 'linear',
+        autoscale: Literal['auto', 'grow'] = 'auto',
         vmin: Optional[Union[sc.Variable, int, float]] = None,
         vmax: Optional[Union[sc.Variable, int, float]] = None,
         nan_color: Optional[str] = None,
         figsize: Optional[Tuple[float, float]] = None,
     ):
         self.cax = canvas.cax if canvas is not None else None
         self.cmap = _get_cmap(cmap, nan_color=nan_color)
         self.mask_cmap = _get_cmap(mask_cmap, nan_color=nan_color)
         self.user_vmin = vmin
         self.user_vmax = vmax
         self.vmin = np.inf
         self.vmax = np.NINF
         self.norm = norm
+        self._autoscale = autoscale
 
         # Note that we need to set vmin/vmax for the LogNorm, if not an error is
         # raised when making the colorbar before any call to update is made.
         self.normalizer = _get_normalizer(self.norm)
         self.colorbar = None
         self.unit = None
+
         self.name = None
         self.changed = False
         self.artists = {}
         self.widget = None
 
         if cbar:
             if self.cax is None:
@@ -124,18 +131,18 @@
                 height_inches = (figsize[1] / dpi) if figsize is not None else 6
                 with silent_mpl_figure():
                     fig = plt.figure(figsize=(height_inches * 0.2, height_inches))
                 self.cax = fig.add_axes([0.05, 0.02, 0.2, 0.98])
             self.colorbar = ColorbarBase(self.cax, cmap=self.cmap, norm=self.normalizer)
             self.cax.yaxis.set_label_coords(-0.9, 0.5)
 
-    def __setitem__(self, key, val):
-        self.artists[key] = val
+    def __setitem__(self, key: str, artist: Any):
+        self.artists[key] = artist
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> Any:
         return self.artists[key]
 
     def to_widget(self):
         """
         Convert the colorbar into a widget for use with other ``ipywidgets``.
         """
         import ipywidgets as ipw
@@ -162,47 +169,53 @@
         """
         colors = self.cmap(self.normalizer(data.values))
         if data.masks:
             one_mask = merge_masks(data.masks).values
             colors[one_mask] = self.mask_cmap(self.normalizer(data.values[one_mask]))
         return colors
 
-    def autoscale(self, data: sc.DataArray):
-        """
-        Re-compute the min and max range of values, given new values.
-        The current range can grow but not shrink.
-
-        Parameters
-        ----------
-        data:
-            The data array containing the values to update the current range.
+    def autoscale(self):
         """
-        vmin, vmax = fix_empty_range(find_limits(data, scale=self.norm))
+        Re-compute the global min and max range of values by iterating over all the
+        artists. If autoscale is set to ``'auto'``, the limits adjust to he current
+        range. If it is set to ``'grow'``, limits can grow but not shrink.
+        """
+        limits = [
+            fix_empty_range(find_limits(artist._data, scale=self.norm))
+            for artist in self.artists.values()
+        ]
+        vmin = reduce(min, [v[0] for v in limits])
+        vmax = reduce(max, [v[1] for v in limits])
         if self.user_vmin is not None:
-            self.vmin = maybe_variable_to_number(self.user_vmin, unit=self.unit)
-        elif vmin.value < self.vmin:
+            self.vmin = self.user_vmin
+        elif (vmin.value < self.vmin) or (self._autoscale == 'auto'):
             self.vmin = vmin.value
         if self.user_vmax is not None:
-            self.vmax = maybe_variable_to_number(self.user_vmax, unit=self.unit)
-        elif vmax.value > self.vmax:
+            self.vmax = self.user_vmax
+        elif (vmax.value > self.vmax) or (self._autoscale == 'auto'):
             self.vmax = vmax.value
 
-    def _set_artists_colors(self, key: str = None):
+        if self.vmin >= self.vmax:
+            if self.user_vmax is not None:
+                self.vmax = self.user_vmax
+                self.vmin = self.user_vmax - abs(self.user_vmax) * 0.1
+            else:
+                self.vmin = self.user_vmin
+                self.vmax = self.user_vmin + abs(self.user_vmin) * 0.1
+
+    def _set_artists_colors(self, keys: Iterable):
         """
         Update the colors of all the artists apart from the one that triggered the
         update, as those get updated by the figure.
 
         Parameters
         ----------
-        key:
-            Update all connected artists, apart from the one whose id is ``key``.
+        keys:
+            List of artists to update.
         """
-        keys = set(self.artists.keys())
-        if key is not None:
-            keys -= {key}
         for k in keys:
             self.artists[k].set_colors(self.rgba(self.artists[k].data))
 
     def _set_normalizer_limits(self):
         """
         Synchronize the underlying normalizer limits to the current state.
         """
@@ -211,61 +224,62 @@
         if self.vmin >= self.normalizer.vmax:
             self.normalizer.vmax = self.vmax
             self.normalizer.vmin = self.vmin
         else:
             self.normalizer.vmin = self.vmin
             self.normalizer.vmax = self.vmax
 
-    def update(self, data: sc.DataArray, key: str):
+    def update(self, key: str, data: sc.DataArray):
         """
         Update the colorscale bounds taking into account new values.
-        If the bounds have changed, we update all the colors in the artists that depend
-        on this ColorMapper. We also update the colorbar widget if it exists.
+        We also update the colorbar widget if it exists.
 
         Parameters
         ----------
         data:
             The data array to use to update the colorscale range.
         key:
             The id of the node that provided this data.
         """
-        if self.unit is None:
-            self.unit = data.unit
-        elif data.unit != self.unit:
-            raise ValueError(
-                f'Incompatible unit: colormapper has unit {self.unit}, '
-                f'new data has unit {data.unit}.'
-            )
-
         if self.name is None:
             self.name = data.name
+            # If name is None, this is the first time update is called
+            if self.user_vmin is not None:
+                self.user_vmin = maybe_variable_to_number(
+                    self.user_vmin, unit=self.unit
+                )
+            if self.user_vmax is not None:
+                self.user_vmax = maybe_variable_to_number(
+                    self.user_vmax, unit=self.unit
+                )
         elif data.name != self.name:
             self.name = ''
         if self.cax is not None:
             text = self.name
             if self.unit is not None:
                 text += f'{" " if self.name else ""}[{self.unit}]'
             self.cax.set_ylabel(text)
-
         old_bounds = np.array([self.vmin, self.vmax])
-        self.autoscale(data=data)
+        self.autoscale()
         self._set_normalizer_limits()
 
         if not np.allclose(old_bounds, np.array([self.vmin, self.vmax])):
-            self._set_artists_colors(key=key)
             self._update_colorbar_widget()
+            keys = self.artists.keys()
+        else:
+            keys = [key]
+        self._set_artists_colors(keys)
 
     def toggle_norm(self):
         """
         Toggle the norm flag, between `linear` and `log`.
         """
         self.norm = "log" if self.norm == 'linear' else 'linear'
         self.normalizer = _get_normalizer(self.norm)
         self.vmin = np.inf
         self.vmax = np.NINF
-        for artist in self.artists.values():
-            self.autoscale(data=artist._data)
+        self.autoscale()
         self._set_normalizer_limits()
-        self._set_artists_colors()
+        self._set_artists_colors(self.artists.keys())
         if self.colorbar is not None:
             self.colorbar.mappable.norm = self.normalizer
             self._update_colorbar_widget()
```

### Comparing `plopp-23.4.0/src/plopp/graphics/figimage.py` & `plopp-23.5.0/src/plopp/graphics/figimage.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         Control the scaling on the vertical axis.
     vmin:
         Lower bound for the colorbar. If a number (without a unit) is supplied, it is
         assumed that the unit is the same as the data unit.
     vmax:
         Upper bound for the colorbar. If a number (without a unit) is supplied, it is
         assumed that the unit is the same as the data unit.
+    autoscale:
+        The behavior of the color range limits. If ``auto``, the limits automatically
+        adjusts every time the data changes. If ``grow``, the limits are allowed to
+        grow with time but they do not shrink.
     scale:
         Control the scaling of the horizontal axis. For example, specify
         ``scale={'tof': 'log'}`` if you want log-scale for the ``tof`` dimension.
     aspect:
         Aspect ratio for the axes.
     grid:
         Show grid if ``True``.
@@ -70,14 +74,15 @@
         self,
         *nodes,
         cmap: str = 'viridis',
         mask_cmap: str = 'gray',
         norm: Literal['linear', 'log'] = 'linear',
         vmin: Optional[Union[sc.Variable, int, float]] = None,
         vmax: Optional[Union[sc.Variable, int, float]] = None,
+        autoscale: Literal['auto', 'grow'] = 'auto',
         scale: Optional[Dict[str, str]] = None,
         aspect: Literal['auto', 'equal'] = 'auto',
         grid: bool = False,
         crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
         cbar: bool = True,
         title: Optional[str] = None,
         figsize: Optional[Tuple[float, float]] = None,
@@ -95,14 +100,15 @@
         self.colormapper = ColorMapper(
             cmap=cmap,
             cbar=cbar,
             mask_cmap=mask_cmap,
             norm=norm,
             vmin=vmin,
             vmax=vmax,
+            autoscale=autoscale,
             canvas=self.canvas,
         )
 
         self.render()
         self.canvas.autoscale()
         if crop is not None:
             self.crop(**crop)
@@ -122,54 +128,47 @@
         if new_values.ndim != 2:
             raise ValueError("FigImage can only be used to plot 2-D data.")
 
         xdim = new_values.dims[1]
         xcoord = new_values.coords[xdim]
         ydim = new_values.dims[0]
         ycoord = new_values.coords[ydim]
-        if not self.dims:
-            self.dims.update({"x": xdim, "y": ydim})
-            self.canvas.xunit = xcoord.unit
-            self.canvas.yunit = ycoord.unit
+        if self.canvas.empty:
+            self.canvas.set_axes(
+                dims={'x': xdim, 'y': ydim}, units={'x': xcoord.unit, 'y': ycoord.unit}
+            )
+            self.canvas.xlabel = name_with_unit(var=xcoord)
+            self.canvas.ylabel = name_with_unit(var=ycoord)
             self.colormapper.unit = new_values.unit
+            if xdim in self._scale:
+                self.canvas.xscale = self._scale[xdim]
+            if ydim in self._scale:
+                self.canvas.yscale = self._scale[ydim]
         else:
             new_values.data = make_compatible(
                 new_values.data, unit=self.colormapper.unit
             )
-            new_values.coords[xdim] = make_compatible(
-                xcoord, dim=self.dims['x'], unit=self.canvas.xunit
-            )
-            new_values.coords[ydim] = make_compatible(
-                ycoord, dim=self.dims['y'], unit=self.canvas.yunit
-            )
-
-        self.colormapper.update(data=new_values, key=key)
+            for xyz, dim in {'x': xdim, 'y': ydim}.items():
+                new_values.coords[dim] = make_compatible(
+                    new_values.coords[dim],
+                    dim=self.canvas.dims[xyz],
+                    unit=self.canvas.units[xyz],
+                )
 
         if key not in self.artists:
             image = backends.image(canvas=self.canvas, data=new_values, **self._kwargs)
             self.artists[key] = image
             self.colormapper[key] = image
-            self.dims.update({"x": new_values.dims[1], "y": new_values.dims[0]})
-
-            self.canvas.xunit = new_values.meta[new_values.dims[1]].unit
-            self.canvas.yunit = new_values.meta[new_values.dims[0]].unit
-
-            self.canvas.xlabel = name_with_unit(var=new_values.meta[self.dims['x']])
-            self.canvas.ylabel = name_with_unit(var=new_values.meta[self.dims['y']])
-            if self.dims['x'] in self._scale:
-                self.canvas.xscale = self._scale[self.dims['x']]
-            if self.dims['y'] in self._scale:
-                self.canvas.yscale = self._scale[self.dims['y']]
 
         self.artists[key].update(new_values=new_values)
-        self.artists[key].set_colors(self.colormapper.rgba(self.artists[key].data))
+        self.colormapper.update(key=key, data=new_values)
 
     def crop(self, **limits):
         """
         Set the axes limits according to the crop parameters.
 
         Parameters
         ----------
         **limits:
             Min and max limits for each dimension to be cropped.
         """
-        self.canvas.crop(**{xy: limits[self.dims[xy]] for xy in 'xy'})
+        self.canvas.crop(**{xy: limits[self.canvas.dims[xy]] for xy in 'xy'})
```

### Comparing `plopp-23.4.0/src/plopp/graphics/figline.py` & `plopp-23.5.0/src/plopp/graphics/figline.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         Control the scaling on the vertical axis.
     vmin:
         Lower bound for the vertical axis. If a number (without a unit) is supplied,
         it is assumed that the unit is the same as the current vertical axis unit.
     vmax:
         Upper bound for the vertical axis. If a number (without a unit) is supplied,
         it is assumed that the unit is the same as the current vertical axis unit.
+    autoscale:
+        The behavior of the axis limits. If ``auto``, the limits automatically
+        adjusts every time the data changes. If ``grow``, the limits are allowed to
+        grow with time but they do not shrink.
     scale:
         Control the scaling of the horizontal axis. For example, specify
         ``scale={'tof': 'log'}`` if you want log-scale for the ``tof`` dimension.
     errorbars:
         Hide errorbars if ``False``.
     mask_color:
         The color of the masks.
@@ -62,14 +66,15 @@
 
     def __init__(
         self,
         *nodes,
         norm: Literal['linear', 'log'] = 'linear',
         vmin: Optional[Union[sc.Variable, int, float]] = None,
         vmax: Optional[Union[sc.Variable, int, float]] = None,
+        autoscale: Literal['auto', 'grow'] = 'auto',
         scale: Optional[Dict[str, str]] = None,
         errorbars: bool = True,
         mask_color: str = 'black',
         aspect: Literal['auto', 'equal'] = 'auto',
         grid: bool = False,
         crop: Optional[Dict[str, Dict[str, sc.Variable]]] = None,
         title: Optional[str] = None,
@@ -88,14 +93,15 @@
             cbar=False,
             aspect=aspect,
             grid=grid,
             figsize=figsize,
             title=title,
             vmin=vmin,
             vmax=vmax,
+            autoscale=autoscale,
             **kwargs
         )
         self.canvas.yscale = norm
 
         self.render()
         self.canvas.autoscale()
         if crop is not None:
@@ -112,51 +118,51 @@
             New data to create or update a :class:`Line` object from.
         key:
             The id of the node that sent the new data.
         """
         if new_values.ndim != 1:
             raise ValueError("FigLine can only be used to plot 1-D data.")
 
-        dim = new_values.dim
-        coord = new_values.coords[dim]
-        if not self.dims:
-            self.dims['x'] = dim
-            self.canvas.xunit = coord.unit
-            self.canvas.yunit = new_values.unit
+        xdim = new_values.dim
+        xcoord = new_values.coords[xdim]
+        if self.canvas.empty:
+            self.canvas.set_axes(
+                dims={'x': xdim}, units={'x': xcoord.unit, 'y': new_values.unit}
+            )
+            self.canvas.xlabel = name_with_unit(var=xcoord)
+            self.canvas.ylabel = name_with_unit(var=new_values.data, name="")
+            if xdim in self._scale:
+                self.canvas.xscale = self._scale[xdim]
         else:
-            new_values.data = make_compatible(new_values.data, unit=self.canvas.yunit)
-            new_values.coords[dim] = make_compatible(
-                coord, dim=self.dims['x'], unit=self.canvas.xunit
+            new_values.data = make_compatible(
+                new_values.data, unit=self.canvas.units['y']
+            )
+            new_values.coords[xdim] = make_compatible(
+                xcoord, dim=self.canvas.dims['x'], unit=self.canvas.units['x']
             )
 
         if key not in self.artists:
             line = backends.line(
                 canvas=self.canvas,
                 data=new_values,
                 number=len(self.artists),
                 errorbars=self._errorbars,
                 mask_color=self._mask_color,
                 **self._kwargs
             )
             self.artists[key] = line
 
-            self.canvas.xlabel = name_with_unit(var=new_values.meta[self.dims['x']])
-            self.canvas.ylabel = name_with_unit(var=new_values.data, name="")
-
-            if self.dims['x'] in self._scale:
-                self.canvas.xscale = self._scale[self.dims['x']]
-
         else:
             self.artists[key].update(new_values=new_values)
 
         self.canvas.autoscale()
 
     def crop(self, **limits):
         """
         Set the axes limits according to the crop parameters.
 
         Parameters
         ----------
         **limits:
             Min and max limits for each dimension to be cropped.
         """
-        self.canvas.crop(x=limits[self.dims['x']])
+        self.canvas.crop(x=limits[self.canvas.dims['x']])
```

### Comparing `plopp-23.4.0/src/plopp/graphics/figscatter3d.py` & `plopp-23.5.0/src/plopp/graphics/figscatter3d.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,51 +99,42 @@
         new_values:
             New data to create or update a :class:`PointCloud` object from.
         key:
             The id of the node that sent the new data.
         draw:
             This argument is ignored for the 3d figure update.
         """
-        xcoord = new_values.coords[self._x]
-        ycoord = new_values.coords[self._y]
-        zcoord = new_values.coords[self._z]
-        if not self.dims:
-            self.dims.update({'x': self._x, 'y': self._y, 'z': self._z})
-            self.canvas.xunit = xcoord.unit
-            self.canvas.yunit = ycoord.unit
-            self.canvas.zunit = zcoord.unit
+        mapping = {'x': self._x, 'y': self._y, 'z': self._z}
+        if self.canvas.empty:
+            self.canvas.set_axes(
+                dims=mapping,
+                units={x: new_values.coords[dim].unit for x, dim in mapping.items()},
+            )
             self.colormapper.unit = new_values.unit
         else:
             new_values.data = make_compatible(
                 new_values.data, unit=self.colormapper.unit
             )
-            new_values.coords[self._x] = new_values.coords[self._x].to(
-                unit=self.canvas.xunit, copy=False
-            )
-            new_values.coords[self._y] = new_values.coords[self._y].to(
-                unit=self.canvas.yunit, copy=False
-            )
-            new_values.coords[self._z] = new_values.coords[self._z].to(
-                unit=self.canvas.zunit, copy=False
-            )
-
-        self.colormapper.update(data=new_values, key=key)
+            for xyz, dim in mapping.items():
+                new_values.coords[dim] = new_values.coords[dim].to(
+                    unit=self.canvas.units[xyz], copy=False
+                )
 
         if key not in self.artists:
             pts = backends.point_cloud(
                 data=new_values, x=self._x, y=self._y, z=self._z, **self._kwargs
             )
             self.artists[key] = pts
             self.colormapper[key] = pts
             self.canvas.add(pts.points)
             if key in self._original_artists:
                 self.canvas.make_outline(limits=self.get_limits())
 
         self.artists[key].update(new_values=new_values)
-        self.artists[key].set_colors(self.colormapper.rgba(self.artists[key].data))
+        self.colormapper.update(key=key, data=new_values)
 
     def get_limits(self) -> Tuple[sc.Variable, sc.Variable, sc.Variable]:
         """
         Get global limits for all the point clouds in the scene.
         """
         xmin = None
         xmax = None
```

### Comparing `plopp-23.4.0/src/plopp/graphics/figure.py` & `plopp-23.5.0/src/plopp/graphics/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/widgets/box.py` & `plopp-23.5.0/src/plopp/widgets/box.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/widgets/checkboxes.py` & `plopp-23.5.0/src/plopp/widgets/checkboxes.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/widgets/cut3d.py` & `plopp-23.5.0/src/plopp/widgets/cut3d.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/widgets/drawing.py` & `plopp-23.5.0/src/plopp/widgets/drawing.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,20 +115,20 @@
 def _get_points_info(artist, figure):
     """
     Convert the raw (x, y) position of a point to a dict containing the dimensions of
     each axis, and scalar values with units.
     """
     return lambda: {
         'x': {
-            'dim': figure.dims['x'],
-            'value': sc.scalar(artist.x, unit=figure.canvas.xunit),
+            'dim': figure.canvas.dims['x'],
+            'value': sc.scalar(artist.x, unit=figure.canvas.units['x']),
         },
         'y': {
-            'dim': figure.dims['y'],
-            'value': sc.scalar(artist.y, unit=figure.canvas.yunit),
+            'dim': figure.canvas.dims['y'],
+            'value': sc.scalar(artist.y, unit=figure.canvas.units['y']),
         },
     }
 
 
 def _make_points(**kwargs):
     """
     Intermediate function needed for giving to `partial` to avoid making mpltoolbox a
```

### Comparing `plopp-23.4.0/src/plopp/widgets/slice.py` & `plopp-23.5.0/src/plopp/widgets/slice.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/widgets/toolbar.py` & `plopp-23.5.0/src/plopp/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp/widgets/tools.py` & `plopp-23.5.0/src/plopp/widgets/tools.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/src/plopp.egg-info/PKG-INFO` & `plopp-23.5.0/src/plopp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 23.4.0
+Version: 23.5.0
 Summary: Plotting library based on scipp
 Home-page: https://scipp.github.io/plopp
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/plopp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `plopp-23.4.0/src/plopp.egg-info/SOURCES.txt` & `plopp-23.5.0/src/plopp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/matplotlib/mpl_canvas_test.py` & `plopp-23.5.0/tests/backends/matplotlib/mpl_canvas_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,16 +40,15 @@
     canvas.logy()
     assert canvas.ax.get_yscale() == 'linear'
     assert canvas.yscale == 'linear'
 
 
 def test_crop():
     canvas = Canvas()
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
+    canvas.units.update(x='m', y='m')
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(102.0, unit='m')
     ymin = sc.scalar(5.5, unit='m')
     ymax = sc.scalar(22.3, unit='m')
     canvas.crop(
         x={
             'min': xmin,
@@ -62,26 +61,24 @@
     )
     assert canvas.ax.get_xlim() == (xmin.value, xmax.value)
     assert canvas.ax.get_ylim() == (ymin.value, ymax.value)
 
 
 def test_crop_unit_conversion():
     canvas = Canvas()
-    canvas.xunit = 'cm'
-    canvas.yunit = 'cm'
+    canvas.units.update(x='cm', y='cm')
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(3.3, unit='m')
     canvas.crop(x={'min': xmin, 'max': xmax})
     assert canvas.ax.get_xlim() == (210.0, 330.0)
 
 
 def test_crop_no_variable():
     canvas = Canvas()
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
+    canvas.units.update(x='m', y='m')
     xmin = 2.1
     xmax = 102.0
     ymin = 5.5
     ymax = 22.3
     canvas.crop(
         x={
             'min': xmin,
```

### Comparing `plopp-23.4.0/tests/backends/matplotlib/mpl_figimage_test.py` & `plopp-23.5.0/tests/backends/matplotlib/mpl_figimage_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     da1 = data_array(ndim=2)
     da2 = 3.0 * data_array(ndim=2)
     da2.coords['xx'] += sc.scalar(50.0, unit='m')
     a = Node(da1)
     b = Node(da2)
     f = FigImage(a, b)
     old_b_colors = f.artists[b.id]._mesh.get_facecolors()
-    a.func = lambda: da1 * 1.1
+    a.func = lambda: da1 * 2.1
     a.notify_children('updated a')
     # No change because the update did not change the colorbar limits
     assert np.allclose(old_b_colors, f.artists[b.id]._mesh.get_facecolors())
     a.func = lambda: da1 * 5.0
     a.notify_children('updated a')
     assert not np.allclose(old_b_colors, f.artists[b.id]._mesh.get_facecolors())
```

### Comparing `plopp-23.4.0/tests/backends/matplotlib/mpl_figline_test.py` & `plopp-23.5.0/tests/backends/matplotlib/mpl_figline_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/matplotlib/mpl_figure_test.py` & `plopp-23.5.0/tests/backends/matplotlib/mpl_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/matplotlib/mpl_image_test.py` & `plopp-23.5.0/tests/backends/matplotlib/mpl_image_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/matplotlib/mpl_interactive_test.py` & `plopp-23.5.0/tests/backends/matplotlib/mpl_interactive_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/matplotlib/mpl_line_test.py` & `plopp-23.5.0/tests/backends/matplotlib/mpl_line_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/plotly/plotly_canvas_test.py` & `plopp-23.5.0/tests/backends/plotly/plotly_canvas_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/plotly/plotly_figure_test.py` & `plopp-23.5.0/tests/backends/plotly/plotly_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/plotly/plotly_line_test.py` & `plopp-23.5.0/tests/backends/plotly/plotly_line_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/pythreejs/pythreejs_canvas_test.py` & `plopp-23.5.0/tests/backends/pythreejs/pythreejs_canvas_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -111,95 +111,81 @@
 
 
 @pytest.mark.parametrize('key', ['position', 'look_at'])
 def test_camera_user_vector(key):
     pos = (0, 1, 2)
     vec = sc.vector(pos, unit='m')
     canvas = Canvas(camera=Camera(**{key: vec}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 'm'
+    canvas.units.update(x='m', y='m', z='m')
     canvas._update_camera(limits=_make_limits())
     _assert_pos(pos, canvas, key)
 
 
 @pytest.mark.parametrize('key', ['position', 'look_at'])
 def test_camera_user_vector_unit_conversion(key):
     vec = sc.vector([0, 1, 2], unit='cm')
     canvas = Canvas(camera=Camera(**{key: vec}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 'm'
+    canvas.units.update(x='m', y='m', z='m')
     canvas._update_camera(limits=_make_limits())
     _assert_pos((0, 0.01, 0.02), canvas, key)
 
 
 @pytest.mark.parametrize('key', ['position', 'look_at'])
 def test_camera_user_vector_bad_unit_raises(key):
     vec = sc.vector([0, 1, 2], unit='s')
     canvas = Canvas(camera=Camera(**{key: vec}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 'm'
+    canvas.units.update(x='m', y='m', z='m')
     with pytest.raises(sc.UnitError):
         canvas._update_camera(limits=_make_limits())
 
 
 @pytest.mark.parametrize('key', ['position', 'look_at'])
 def test_camera_user_vector_can_convert_a_single_field(key):
     vec = sc.vector([0, 1, 2], unit='m')
     canvas = Canvas(camera=Camera(**{key: vec}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 'cm'
+    canvas.units.update(x='m', y='m', z='cm')
     canvas._update_camera(limits=_make_limits())
     _assert_pos((0, 1, 200), canvas, key)
 
 
 @pytest.mark.parametrize('key', ['position', 'look_at'])
 def test_camera_user_tuple_of_variables(key):
     pos = [
         sc.scalar(2.0, unit='m'),
         sc.scalar(-12.0, unit='m'),
         sc.scalar(44.0, unit='m'),
     ]
     canvas = Canvas(camera=Camera(**{key: pos}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 'm'
+    canvas.units.update(x='m', y='m', z='m')
     canvas._update_camera(limits=_make_limits())
     _assert_pos((2.0, -12.0, 44.0), canvas, key)
 
 
 @pytest.mark.parametrize('key', ['position', 'look_at'])
 def test_camera_user_tuple_of_variables_unit_conversion(key):
     pos = [
         sc.scalar(2.0, unit='m'),
         sc.scalar(-12.0, unit='cm'),
         sc.scalar(44.0, unit='mm'),
     ]
     canvas = Canvas(camera=Camera(**{key: pos}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 'm'
+    canvas.units.update(x='m', y='m', z='m')
     canvas._update_camera(limits=_make_limits())
     _assert_pos((2.0, -0.12, 0.044), canvas, key)
 
 
 @pytest.mark.parametrize('key', ['position', 'look_at'])
 def test_camera_user_tuple_of_variables_bad_unit_raises(key):
     pos = [
         sc.scalar(2.0, unit='m'),
         sc.scalar(-12.0, unit='m'),
         sc.scalar(44.0, unit='m'),
     ]
     canvas = Canvas(camera=Camera(**{key: pos}))
-    canvas.xunit = 's'
-    canvas.yunit = 's'
-    canvas.zunit = 's'
+    canvas.units.update(x='s', y='s', z='s')
     with pytest.raises(sc.UnitError):
         canvas._update_camera(limits=_make_limits())
 
 
 @pytest.mark.parametrize('key', ['near', 'far'])
 def test_camera_user_float(key):
     value = 6.8
@@ -208,50 +194,42 @@
     assert getattr(canvas.camera, key) == value
 
 
 @pytest.mark.parametrize('key', ['near', 'far'])
 def test_camera_user_variable(key):
     value = sc.scalar(15.1, unit='m')
     canvas = Canvas(camera=Camera(**{key: value}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 'm'
+    canvas.units.update(x='m', y='m', z='m')
     canvas._update_camera(limits=_make_limits())
     assert getattr(canvas.camera, key) == value.value
 
 
 @pytest.mark.parametrize('key', ['near', 'far'])
 def test_camera_user_variable_unit_conversion(key):
     value = sc.scalar(33.0, unit='cm')
     canvas = Canvas(camera=Camera(**{key: value}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 'm'
+    canvas.units.update(x='m', y='m', z='m')
     canvas._update_camera(limits=_make_limits())
     assert getattr(canvas.camera, key) == 0.33
 
 
 @pytest.mark.parametrize('key', ['near', 'far'])
 def test_camera_user_variable_bad_unit_raises(key):
     value = sc.scalar(6.6, unit='s')
     canvas = Canvas(camera=Camera(**{key: value}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 'm'
+    canvas.units.update(x='m', y='m', z='m')
     with pytest.raises(sc.UnitError):
         canvas._update_camera(limits=_make_limits())
 
 
 @pytest.mark.parametrize('key', ['near', 'far'])
 def test_camera_user_variable_raises_when_axes_units_are_different(key):
     value = sc.scalar(5.66, unit='m')
     canvas = Canvas(camera=Camera(**{key: value}))
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
-    canvas.zunit = 's'
+    canvas.units.update(x='m', y='m', z='s')
     with pytest.raises(sc.UnitError, match='All axes must have the same unit'):
         canvas._update_camera(limits=_make_limits())
 
 
 def test_toggle_axes_3d():
     canvas = Canvas()
     assert canvas.axes_3d.visible
```

### Comparing `plopp-23.4.0/tests/backends/pythreejs/pythreejs_figure_test.py` & `plopp-23.5.0/tests/backends/pythreejs/pythreejs_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py` & `plopp-23.5.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/conftest.py` & `plopp-23.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/core/graph_test.py` & `plopp-23.5.0/tests/core/graph_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/core/limits_test.py` & `plopp-23.5.0/tests/core/limits_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/core/node_test.py` & `plopp-23.5.0/tests/core/node_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/core/views.py` & `plopp-23.5.0/tests/core/views.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/functions/common_test.py` & `plopp-23.5.0/tests/functions/common_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     assert out.coords['yy2'].max() == 3.3 * da.coords['yy'].max()
 
 
 def test_preprocess_warns_when_coordinate_is_not_sorted():
     da = data_array(ndim=1)
     unsorted = sc.concat([da['xx', 20:], da['xx', :20]], dim='xx')
     with pytest.warns(
-        UserWarning, match='The input contains a coordinate with unsorted values'
+        RuntimeWarning, match='The input contains a coordinate with unsorted values'
     ):
         preprocess(unsorted)
 
 
 def test_preprocess_no_warning_if_dtype_cannot_be_sorted():
     da = data_array(ndim=1)
     da.coords['vecs'] = sc.vectors(
```

### Comparing `plopp-23.4.0/tests/functions/plot_test.py` & `plopp-23.5.0/tests/functions/plot_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,14 +79,20 @@
         pp.plot(np.random.random((3000, 2500)))
 
 
 def test_plot_ignore_size_disables_size_check():
     pp.plot(np.random.random(1_100_000), ignore_size=True)
 
 
+def test_plot_with_non_dimensional_unsorted_coord_does_not_warn():
+    da = data_array(ndim=1)
+    da.coords['aux'] = sc.sin(sc.arange(da.dim, 50.0, unit='rad'))
+    pp.plot(da)
+
+
 def test_plot_2d_coord():
     da = data_array(ndim=2, ragged=True)
     pp.plot(da)
     pp.plot(da.transpose())
 
 
 def test_plot_2d_coord_with_mask():
@@ -101,18 +107,14 @@
     return artists[keys[n]]
 
 
 def _get_line(fig, n=0):
     return _get_artist(fig=fig, n=n)._line
 
 
-def _get_mesh(fig):
-    return _get_artist(fig=fig)._mesh
-
-
 def test_kwarg_linecolor():
     da = data_array(ndim=1)
     p = pp.plot(da, color='r')
     assert _get_line(p).get_color() == 'r'
     p = pp.plot(da, c='b')
     assert _get_line(p).get_color() == 'b'
 
@@ -242,25 +244,25 @@
 
 
 def test_use_non_dimension_coords():
     da = data_array(ndim=2, binedges=True)
     da.coords['xx2'] = 7.5 * da.coords['xx']
     da.coords['yy2'] = 3.3 * da.coords['yy']
     p = pp.plot(da, coords=['xx2', 'yy2'])
-    assert p._fig.dims['x'] == 'xx2'
-    assert p._fig.dims['y'] == 'yy2'
+    assert p.canvas.dims['x'] == 'xx2'
+    assert p.canvas.dims['y'] == 'yy2'
     assert p.canvas._xmax == 7.5 * da.coords['xx'].max().value
     assert p.canvas._ymax == 3.3 * da.coords['yy'].max().value
 
 
 def test_use_non_dimension_coords_dataset():
     ds = dataset(ndim=1)
     ds.coords['xx2'] = 6.6 * ds.coords['xx']
     p = pp.plot(ds, coords=['xx2'])
-    assert p._fig.dims['x'] == 'xx2'
+    assert p.canvas.dims['x'] == 'xx2'
     assert p.canvas._xmax > 6.6 * ds.coords['xx'].max().value
 
 
 @pytest.mark.parametrize('ext', ['jpg', 'png', 'pdf', 'svg'])
 def test_save_to_disk_1d(ext):
     da = data_array(ndim=1)
     fig = pp.plot(da)
@@ -300,35 +302,35 @@
     import xarray as xr
 
     N = 50
     data = np.random.random(N)
     time = np.arange(float(N))
     da = xr.DataArray(data, coords={'time': time}, dims=['time'])
     p = pp.plot(da)
-    assert p._fig.dims['x'] == 'time'
-    assert p.canvas.xunit == 'dimensionless'
-    assert p.canvas.yunit == 'dimensionless'
+    assert p.canvas.dims['x'] == 'time'
+    assert p.canvas.units['x'] == 'dimensionless'
+    assert p.canvas.units['y'] == 'dimensionless'
 
 
 def test_plot_xarray_data_array_2d():
     import xarray as xr
 
     N = 50
     M = 40
     data = np.random.random([M, N])
     time = np.arange(float(N))
     space = np.arange(float(M))
     da = xr.DataArray(
         data, coords={'space': space, 'time': time}, dims=['space', 'time']
     )
     p = pp.plot(da)
-    assert p._fig.dims['x'] == 'time'
-    assert p._fig.dims['y'] == 'space'
-    assert p.canvas.xunit == 'dimensionless'
-    assert p.canvas.yunit == 'dimensionless'
+    assert p.canvas.dims['x'] == 'time'
+    assert p.canvas.dims['y'] == 'space'
+    assert p.canvas.units['x'] == 'dimensionless'
+    assert p.canvas.units['y'] == 'dimensionless'
 
 
 def test_plot_xarray_dataset():
     import xarray as xr
 
     N = 50
     temp = 15 + 8 * np.random.random(N)
@@ -337,28 +339,28 @@
         {
             "temperature": (["time"], temp),
             "precipitation": (["time"], precip),
         },
         coords={"time": np.arange(50)},
     )
     p = pp.plot(ds)
-    assert p._fig.dims['x'] == 'time'
-    assert p.canvas.xunit == 'dimensionless'
-    assert p.canvas.yunit == 'dimensionless'
+    assert p.canvas.dims['x'] == 'time'
+    assert p.canvas.units['x'] == 'dimensionless'
+    assert p.canvas.units['y'] == 'dimensionless'
     assert len(p._fig.artists) == 2
 
 
 def test_plot_pandas_series():
     import pandas as pd
 
     s = pd.Series(np.arange(100.0), name='MyDataSeries')
     p = pp.plot(s)
-    assert p._fig.dims['x'] == 'row'
-    assert p.canvas.xunit == 'dimensionless'
-    assert p.canvas.yunit == 'dimensionless'
+    assert p.canvas.dims['x'] == 'row'
+    assert p.canvas.units['x'] == 'dimensionless'
+    assert p.canvas.units['y'] == 'dimensionless'
     assert list(p._fig.artists.values())[0].label == 'MyDataSeries'
 
 
 def test_plot_pandas_dataframe():
     import pandas as pd
 
     df = pd.DataFrame(
@@ -366,11 +368,11 @@
             'A': np.arange(50.0),
             'B': 1.5 * np.arange(50),
             'C': np.random.random(50),
             'D': np.random.normal(size=50),
         }
     )
     p = pp.plot(df)
-    assert p._fig.dims['x'] == 'row'
-    assert p.canvas.xunit == 'dimensionless'
-    assert p.canvas.yunit == 'dimensionless'
+    assert p.canvas.dims['x'] == 'row'
+    assert p.canvas.units['x'] == 'dimensionless'
+    assert p.canvas.units['y'] == 'dimensionless'
     assert len(p._fig.artists) == 4
```

### Comparing `plopp-23.4.0/tests/functions/scatter3d_test.py` & `plopp-23.5.0/tests/functions/scatter3d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/functions/slicer_test.py` & `plopp-23.5.0/tests/functions/slicer_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -93,7 +93,19 @@
 
 def test_raises_when_requested_keep_dims_do_not_exist():
     da = data_array(ndim=3)
     with pytest.raises(
         ValueError, match='Slicer plot: one or more of the requested dims to be kept'
     ):
         Slicer(da, keep=['time'])
+
+
+def test_autoscale_fixed():
+    da = sc.DataArray(
+        data=sc.arange('x', 5 * 10 * 20).fold(dim='x', sizes={'z': 20, 'y': 10, 'x': 5})
+    )
+    sl = Slicer(da, keep=['y', 'x'], autoscale='fixed')
+    assert sl.figure._fig.colormapper.vmin == 0
+    assert sl.figure._fig.colormapper.vmax == 5 * 10 * 20 - 1
+    sl.slider.controls['z']['slider'].value = 5
+    assert sl.figure._fig.colormapper.vmin == 0
+    assert sl.figure._fig.colormapper.vmax == 5 * 10 * 20 - 1
```

### Comparing `plopp-23.4.0/tests/functions/superplot_test.py` & `plopp-23.5.0/tests/functions/superplot_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/graphics/colormapper_test.py` & `plopp-23.5.0/tests/graphics/colormapper_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     def __init__(self, data):
         self._data = data
         self._colors = None
 
     def set_colors(self, colors):
         self._colors = colors
 
+    def update(self, data):
+        self._data = data
+
     @property
     def data(self):
         return self._data
 
 
 def test_creation():
     mapper = ColorMapper(
@@ -43,82 +46,111 @@
     mapper = ColorMapper(norm='log')
     assert mapper.norm == 'log'
 
 
 def test_autoscale():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper()
+    artist = DummyChild(da)
+    mapper['data'] = artist
 
-    mapper.autoscale(data=da)
+    mapper.update(key='data', data=da)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
 
     const = 2.3
-    mapper.autoscale(data=da * const)
+    artist.update(da * const)
+    mapper.update(key='data', data=da * const)
     assert mapper.vmin == (da.min() * const).value
     assert mapper.vmax == (da.max() * const).value
 
 
-def test_rescale_limits_do_not_shrink():
+def test_auto_rescale_limits_can_shrink():
     da = data_array(ndim=2, unit='K')
-    mapper = ColorMapper()
+    mapper = ColorMapper(autoscale='auto')
+    artist = DummyChild(da)
+    mapper['data'] = artist
+
+    mapper.update(key='data', data=da)
+    assert mapper.vmin == da.min().value
+    assert mapper.vmax == da.max().value
+
+    const = 0.5
+    artist.update(da * const)
+    mapper.update(key='data', data=da * const)
+    assert mapper.vmin == da.min().value * const
+    assert mapper.vmax == da.max().value * const
+
+
+def test_grow_rescale_limits_do_not_shrink():
+    da = data_array(ndim=2, unit='K')
+    mapper = ColorMapper(autoscale='grow')
+    artist = DummyChild(da)
+    mapper['data'] = artist
 
-    mapper.autoscale(data=da)
+    mapper.update(key='data', data=da)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
 
     const = 0.5
-    mapper.autoscale(data=da * const)
+    artist.update(da * const)
+    mapper.update(key='data', data=da * const)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
 
 
 def test_correct_normalizer_limits():
     da = sc.DataArray(data=sc.array(dims=['y', 'x'], values=[[1, 2], [3, 4]]))
     mapper = ColorMapper()
-    mapper.update(data=da, key=None)
+    artist = DummyChild(da)
+    mapper['data'] = artist
+    mapper.update(key='data', data=da)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
     # The normalizer initially has limits [0, 1].
     # In Matplotlib, if we set the normalizer vmin value (1) equal to the current vmax,
     # it will silently set it to something smaller, e.g. 0.9.
     # Our implementation needs to work around this.
     assert mapper.normalizer.vmin == da.min().value
     assert mapper.normalizer.vmax == da.max().value
 
 
 def test_vmin_vmax():
-    da = data_array(ndim=2, unit='K')
+    da = data_array(ndim=2, unit='K') * 100.0
     vmin = sc.scalar(-0.1, unit='K')
     vmax = sc.scalar(3.5, unit='K')
     mapper = ColorMapper(vmin=vmin, vmax=vmax)
-    mapper.update(data=da * 100.0, key=None)
-    assert sc.identical(mapper.user_vmin, vmin)
-    assert sc.identical(mapper.user_vmax, vmax)
+    artist = DummyChild(da)
+    mapper['data'] = artist
+    mapper.update(key='data', data=da)
+    assert mapper.user_vmin == vmin.value
+    assert mapper.user_vmax == vmax.value
     assert mapper.vmin == vmin.value
     assert mapper.vmax == vmax.value
 
 
 def test_vmin_vmax_no_variable():
-    da = data_array(ndim=2, unit='K')
+    da = data_array(ndim=2, unit='K') * 100.0
     vmin = -0.1
     vmax = 3.5
     mapper = ColorMapper(vmin=vmin, vmax=vmax)
-    mapper.update(data=da * 100.0, key=None)
+    artist = DummyChild(da)
+    mapper['data'] = artist
+    mapper.update(key='data', data=da)
     assert mapper.user_vmin == vmin
     assert mapper.user_vmax == vmax
     assert mapper.vmin == vmin
     assert mapper.vmax == vmax
 
 
 def test_toggle_norm():
     mapper = ColorMapper()
     da = data_array(ndim=2, unit='K')
     mapper['child1'] = DummyChild(da)
-    mapper.autoscale(da)
+    mapper.update(key='child1', data=da)
     assert mapper.norm == 'linear'
     assert isinstance(mapper.normalizer, Normalize)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
 
     mapper.toggle_norm()
     assert mapper.norm == 'log'
@@ -126,20 +158,23 @@
     assert mapper.vmin > 0
     assert mapper.vmax == da.max().value
 
 
 def test_update_changes_limits():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper()
+    artist = DummyChild(da)
+    mapper['data'] = artist
 
     mapper.update(data=da, key=None)
     assert mapper.normalizer.vmin == da.min().value
     assert mapper.normalizer.vmax == da.max().value
 
     const = 2.3
+    artist.update(da * const)
     mapper.update(data=da * const, key=None)
     assert mapper.normalizer.vmin == (da.min() * const).value
     assert mapper.normalizer.vmax == (da.max() * const).value
 
 
 def test_rgba():
     da = data_array(ndim=2, unit='K')
@@ -154,26 +189,62 @@
     mapper = ColorMapper()
     assert not np.allclose(mapper.rgba(da1), mapper.rgba(da2))
 
 
 def test_colorbar_updated_on_rescale():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper()
+    artist = DummyChild(da)
+    key = 'data'
+    mapper[key] = artist
 
-    mapper.update(data=da, key=None)
+    mapper.update(data=da, key=key)
     _ = mapper.to_widget()
     old_image = mapper.widget.value
     old_image_array = old_image
 
     # Update with the same values should not make a new colorbar image
-    mapper.update(data=da, key=None)
+    artist.update(da)
+    mapper.update(data=da, key=key)
     assert old_image is mapper.widget.value
 
+    # Update with new values should make a new colorbar image
     const = 2.3
-    mapper.update(data=da * const, key=None)
+    artist.update(da * const)
+    mapper.update(data=da * const, key=key)
+    assert old_image_array != mapper.widget.value
+
+
+def test_colorbar_does_not_update_on_rescale_if_limits_can_only_grow():
+    da = data_array(ndim=2, unit='K')
+    mapper = ColorMapper(autoscale='grow')
+    artist = DummyChild(da)
+    key = 'data'
+    mapper[key] = artist
+
+    mapper.update(data=da, key=key)
+    _ = mapper.to_widget()
+    old_image = mapper.widget.value
+    old_image_array = old_image
+
+    # Update with the same values should not make a new colorbar image
+    artist.update(da)
+    mapper.update(data=da, key=key)
+    assert old_image is mapper.widget.value
+
+    # Update with a smaller range should not make a new colorbar image
+    const = 0.8
+    artist.update(da * const)
+    mapper.update(data=da * const, key=key)
+    assert old_image is mapper.widget.value
+
+    # Update with new values should make a new colorbar image
+    const = 2.3
+    artist.update(da * const)
+    mapper.update(data=da * const, key=key)
     assert old_image_array != mapper.widget.value
 
 
 def test_colorbar_is_not_created_if_cbar_false():
     mapper = ColorMapper(cbar=False)
     assert mapper.colorbar is None
     assert mapper.cax is None
@@ -182,7 +253,37 @@
 def test_colorbar_cbar_false_overrides_cax():
     @dataclass
     class Canvas:
         cax: int
 
     mapper = ColorMapper(cbar=False, canvas=Canvas(cax=0))
     assert mapper.colorbar is None
+
+
+def test_autoscale_auto_vmin_set():
+    da = data_array(ndim=2, unit='K')
+    mapper = ColorMapper(autoscale='auto', vmin=-0.5)
+    artist = DummyChild(da)
+    key = 'data'
+    mapper[key] = artist
+    mapper.update(data=da, key=key)
+    assert mapper.vmin == -0.5
+    assert mapper.vmax == da.max().value
+    # Make sure it handles when da.max() is greater than vmin
+    mapper.update(data=da - sc.scalar(5.0, unit='K'), key=key)
+    assert mapper.vmin == -0.5
+    assert mapper.vmin < mapper.vmax
+
+
+def test_autoscale_auto_vmax_set():
+    da = data_array(ndim=2, unit='K')
+    mapper = ColorMapper(autoscale='auto', vmax=0.5)
+    artist = DummyChild(da)
+    key = 'data'
+    mapper[key] = artist
+    mapper.update(data=da, key=key)
+    assert mapper.vmax == 0.5
+    assert mapper.vmin == da.min().value
+    # Make sure it handles when da.min() is greater than vmax
+    mapper.update(data=da + sc.scalar(5.0, unit='K'), key=key)
+    assert mapper.vmax == 0.5
+    assert mapper.vmin < mapper.vmax
```

### Comparing `plopp-23.4.0/tests/graphics/figimage_test.py` & `plopp-23.5.0/tests/graphics/figimage_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/graphics/figline_test.py` & `plopp-23.5.0/tests/graphics/figline_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,17 +98,29 @@
     key = list(fig.artists.keys())[0]
     fig.update(da * 2.5, key=key)
     new_lims = fig.canvas.yrange
     assert new_lims[0] < old_lims[0]
     assert new_lims[1] > old_lims[1]
 
 
-def test_update_does_not_shrink_limits():
+def test_update_does_shrink_limits_if_auto_mode():
     da = data_array(ndim=1)
-    fig = FigLine(Node(da))
+    fig = FigLine(Node(da), autoscale='auto')
+    old_lims = fig.canvas.yrange
+    key = list(fig.artists.keys())[0]
+    const = 0.5
+    fig.update(da * const, key=key)
+    new_lims = fig.canvas.yrange
+    assert new_lims[0] == old_lims[0] * const
+    assert new_lims[1] == old_lims[1] * const
+
+
+def test_update_does_not_shrink_limits_if_grow_mode():
+    da = data_array(ndim=1)
+    fig = FigLine(Node(da), autoscale='grow')
     old_lims = fig.canvas.yrange
     key = list(fig.artists.keys())[0]
     fig.update(da * 0.5, key=key)
     new_lims = fig.canvas.yrange
     assert new_lims[0] == old_lims[0]
     assert new_lims[1] == old_lims[1]
```

### Comparing `plopp-23.4.0/tests/graphics/figscatter3d_test.py` & `plopp-23.5.0/tests/graphics/figscatter3d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/high_level_test.py` & `plopp-23.5.0/tests/high_level_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/widgets/box_test.py` & `plopp-23.5.0/tests/widgets/box_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/widgets/checkboxes_test.py` & `plopp-23.5.0/tests/widgets/checkboxes_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/widgets/cut3d_test.py` & `plopp-23.5.0/tests/widgets/cut3d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tests/widgets/slice_test.py` & `plopp-23.5.0/tests/widgets/slice_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.4.0/tox.ini` & `plopp-23.5.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 [tox]
-envlist = minimal,noplotly,py39
+envlist = minimal,noplotly,py310
 isolated_build = true
 
 [testenv]
 deps = -r requirements/test.txt
 commands = pytest
 
 [testenv:minimal]
 description = Test if plopp can plot when installed with only base dependencies
-basepython = python3.9
+basepython = python3.10
 deps = -r requirements/mini.txt
 commands = pytest tests/minimal_plot.py
 
 [testenv:noplotly]
 description = Test that plotly tests are skipped if plotly is not installed
-basepython = python3.9
+basepython = python3.10
 deps = -r requirements/noplotly.txt
 commands = pytest tests/backends/plotly
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
-basepython = python3.9
+basepython = python3.10
 deps = {posargs:}
        -r requirements/docs.txt
 allowlist_externals=find
 commands = python -m sphinx -j2 -v -b html -d {toxworkdir}/docs_doctrees docs html
            find html -type f -name "*.ipynb" -not -path "html/_sources/*" -delete
 
 [testenv:linkcheck]
 description = Run Sphinx linkcheck
 deps = -r requirements/docs.txt
 commands = python -m sphinx -j2 -v -b linkcheck -d {toxworkdir}/docs_doctrees docs html
 
 [testenv:static]
 description = Code formatting and static analysis
-basepython = python3.9
+basepython = python3.10
 skip_install = true
 deps = -r requirements/static.txt
 allowlist_externals = sh
 # The first run of pre-commit may reformat files. If this happens, it returns 1 but this
 # should not fail the job. So just run again if it fails. A second failure means that
 # either the different formatters can't agree on a format or that static analysis failed.
 commands = sh -c 'pre-commit run -a || (echo "" && pre-commit run -a)'
```

