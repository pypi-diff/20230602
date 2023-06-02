# Comparing `tmp/gwpy-3.0.4.tar.gz` & `tmp/gwpy-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwpy-3.0.4.tar", last modified: Wed Apr 12 12:14:41 2023, max compression
+gzip compressed data, was "gwpy-3.0.5.tar", last modified: Fri Jun  2 08:36:27 2023, max compression
```

## Comparing `gwpy-3.0.4.tar` & `gwpy-3.0.5.tar`

### file list

```diff
@@ -1,441 +1,442 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      524 2023-04-06 10:37:11.000000 gwpy-3.0.4/.codeclimate.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      498 2023-04-06 10:37:11.000000 gwpy-3.0.4/.codecov.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      483 2023-04-06 10:37:11.000000 gwpy-3.0.4/.flake8
--rw-r--r--   0 duncan    (1000) duncan    (1000)       30 2023-04-06 10:37:11.000000 gwpy-3.0.4/.gitattributes
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.958642 gwpy-3.0.4/.github/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.978642 gwpy-3.0.4/.github/workflows/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5119 2023-04-12 09:57:39.000000 gwpy-3.0.4/.github/workflows/conda.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2920 2023-04-06 10:37:11.000000 gwpy-3.0.4/.github/workflows/dependencies.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3119 2023-04-06 10:37:11.000000 gwpy-3.0.4/.github/workflows/dist.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1415 2023-04-12 09:57:39.000000 gwpy-3.0.4/.github/workflows/lint.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      726 2023-04-06 10:37:11.000000 gwpy-3.0.4/.gitignore
--rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2023-04-06 10:37:11.000000 gwpy-3.0.4/.pep8speaks.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      133 2023-04-06 10:37:11.000000 gwpy-3.0.4/CODE_OF_CONDUCT.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4481 2023-04-06 10:37:11.000000 gwpy-3.0.4/CONTRIBUTING.md
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2023-04-06 10:37:11.000000 gwpy-3.0.4/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2023-04-06 10:37:11.000000 gwpy-3.0.4/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-04-12 12:14:41.108642 gwpy-3.0.4/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1800 2023-04-06 10:37:11.000000 gwpy-3.0.4/README.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      788 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/Makefile
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/_static/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/_static/css/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_static/css/gwpy-sphinx.css
--rw-r--r--   0 duncan    (1000) duncan    (1000)    19634 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_static/favicon.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)    15166 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_static/gwpy_white_24.png
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.958642 gwpy-3.0.4/docs/_templates/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/_templates/autoclass/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      860 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_templates/autoclass/class.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/_templates/autosummary/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      170 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_templates/autosummary/base.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1145 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      703 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/astro/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      735 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/astro/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2653 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/citing.rst.in
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/cli/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5295 2023-04-09 14:36:48.000000 gwpy-3.0.4/docs/cli/examples.ini
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2879 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/cli/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13301 2023-04-09 14:36:48.000000 gwpy-3.0.4/docs/conf.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/detector/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3245 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/detector/channel.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/dev/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3787 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/dev/release.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1624 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/env.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.958642 gwpy-3.0.4/docs/examples/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/examples/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/external/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1162 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/external/framecpp.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      990 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/external/framel.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3134 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/external/lalsuite.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1025 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/external/nds2.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    52297 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/gwpy-docs-logo.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2491 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1300 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/install.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2694 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/overview.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/plot/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/colorbars.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2985 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/colors.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      772 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/filter.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2514 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/gps.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1838 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/legend.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1363 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/log.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5072 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/references.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/segments/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1513 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/segments/dqsegdb.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6818 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/segments/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6756 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/segments/io.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2124 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/segments/thresholding.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/signal/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4369 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/signal/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/spectrogram/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3771 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/spectrogram/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/spectrum/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      505 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/spectrum/filtering.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3732 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/spectrum/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4986 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/spectrum/io.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7364 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/filter.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      955 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/histogram.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1500 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    30445 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/table/io.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1756 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/plot.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2142 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/rate.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/time/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1085 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/time/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/timeseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11634 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/timeseries/datafind.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2722 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/timeseries/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10656 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/timeseries/io.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2744 2023-04-12 12:10:00.000000 gwpy-3.0.4/docs/timeseries/opendata.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3032 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/timeseries/plot.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8470 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/timeseries/statevector.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/examples/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/frequencyseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2584 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2065 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/hoff.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      258 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2585 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/inject.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/percentiles.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/rayleigh.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2203 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/transfer_function.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2630 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/variance.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/miscellaneous/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      216 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/miscellaneous/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3354 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/miscellaneous/open-data-spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2366 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/miscellaneous/range-spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2490 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/miscellaneous/range-timeseries.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/segments/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      158 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/segments/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2411 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/segments/open-data.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/signal/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5642 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/signal/gw150914.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      179 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/signal/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3139 2023-04-09 14:36:48.000000 gwpy-3.0.4/examples/signal/qscan.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/spectrogram/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2387 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2627 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2581 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/ratio.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2125 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/rayleigh.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2885 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/spectrogram2.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1597 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/histogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      198 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2317 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/rate.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2460 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/rate_binned.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2018 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/scatter.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2287 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/tiles.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3734 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/test_examples.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/timeseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2644 2023-04-12 12:10:00.000000 gwpy-3.0.4/examples/timeseries/blrms.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4204 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/correlate.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2797 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/filter.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      246 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2641 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/inject.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2466 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/public.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3788 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/pycbc-snr.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/qscan.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2202 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/statevector.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2476 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/whiten.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/gwpy/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1533 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy/_version.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy/astro/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1909 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/astro/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    24880 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/astro/range.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy/astro/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/astro/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6032 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/astro/tests/test_range.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy/cli/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1404 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    34269 2023-04-12 12:10:00.000000 gwpy-3.0.4/gwpy/cli/cliproduct.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4048 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3353 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/coherencegram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5121 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/gwpy_plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9140 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/qtransform.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7131 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4899 2023-04-12 12:10:00.000000 gwpy-3.0.4/gwpy/cli/spectrum.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy/cli/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      744 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10831 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/base.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1353 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1580 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_coherencegram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1718 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_gwpy_plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2899 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_qtransform.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1509 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1416 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_spectrum.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1279 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_timeseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1999 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_transferfunction.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3891 2023-04-12 12:10:00.000000 gwpy-3.0.4/gwpy/cli/timeseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9784 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/transferfunction.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1639 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/conftest.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/detector/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2252 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    26901 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/channel.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/detector/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1037 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3184 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/io/cis.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5689 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/io/clf.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5939 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/io/omega.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/detector/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    18473 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/detector/tests/test_channel.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2548 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/tests/test_units.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7113 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/units.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/frequencyseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      995 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1943 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/_fdcommon.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14328 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/frequencyseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11947 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/hist.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/frequencyseries/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      907 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1071 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/io/ascii.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1036 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1149 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/io/ligolw.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/frequencyseries/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      756 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11033 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/frequencyseries/tests/test_frequencyseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4005 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/frequencyseries/tests/test_hist.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.038642 gwpy-3.0.4/gwpy/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      831 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4250 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/io/_framecpp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14662 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/cache.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18462 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/datafind.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8399 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/ffldatafind.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18966 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/io/gwf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5257 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6928 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    22182 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4116 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    19331 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/nds2.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3518 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/registry.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.038642 gwpy-3.0.4/gwpy/io/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      743 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8567 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_cache.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10606 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_datafind.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6277 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/tests/test_ffldatafind.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4228 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_gwf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10701 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3293 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12185 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_nds2.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3971 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7341 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.048642 gwpy-3.0.4/gwpy/plot/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1641 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    23094 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/axes.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8733 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/bode.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7041 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/plot/colorbar.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3367 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/colors.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    16720 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/plot/gps.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1635 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/legend.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5030 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/plot/log.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    21766 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4816 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/rc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    16943 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/segments.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.048642 gwpy-3.0.4/gwpy/plot/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      740 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11542 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/plot/tests/test_axes.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3351 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_bode.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1881 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_colors.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5456 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_gps.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2652 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_log.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4398 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1252 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_rc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5442 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_segments.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2318 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/plot/tests/test_tex.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_text.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1615 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1925 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4783 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/plot/tex.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1989 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/text.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1383 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/units.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1670 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.048642 gwpy-3.0.4/gwpy/segments/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1194 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    52670 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/flag.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/segments/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1005 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11048 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3036 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/json.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4907 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5007 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/segwizard.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9042 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/segments.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/segments/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    29683 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/segments/tests/test_flag.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5360 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/tests/test_segments.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/signal/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      972 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1189 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/fft.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    20270 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/signal/filter_design.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    24471 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/signal/qtransform.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/signal/spectral/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1818 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12000 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1851 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_median_mean.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3577 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2346 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_registry.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_scipy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14241 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_ui.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1669 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/signal/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      747 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4349 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_filter_design.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4017 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_qtransform.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3543 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2195 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_median_mean.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2249 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1446 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_registry.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1874 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_scipy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3045 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_ui.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1453 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2726 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/signal/tests/test_window.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5927 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/signal/window.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/spectrogram/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      919 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5742 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/coherence.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/spectrogram/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      846 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      963 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    22206 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/spectrogram.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/spectrogram/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      752 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6590 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/spectrogram/tests/test_spectrogram.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1418 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7918 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/filter.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2645 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/filters.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8173 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/gravityspy.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/table/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1564 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3809 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/cwb.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/fetch.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4663 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/gravityspy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8390 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/gstlal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5433 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/gwf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5205 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/hacr.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13590 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4434 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/losc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2604 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/omega.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1333 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/omicron.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8894 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3318 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/root.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3857 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/snax.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3067 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/sql.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3183 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    26330 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/table.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.078642 gwpy-3.0.4/gwpy/table/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3392 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/table/tests/test_gravityspy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7979 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/tests/test_io_gstlal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2848 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/tests/test_io_ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8313 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/table/tests/test_io_pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    30399 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/table/tests/test_table.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.078642 gwpy-3.0.4/gwpy/testing/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/__init__.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.088642 gwpy-3.0.4/gwpy/testing/data/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)   377295 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/HLV-HW100916-968654552-1.gwf
--rw-r--r--   0 duncan    (1000) duncan    (1000)   382679 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/HLV-HW100916-968654552-1.hdf
--rw-r--r--   0 duncan    (1000) duncan    (1000)       59 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      564 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2783 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/testing/errors.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3772 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/fixtures.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1480 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/marks.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4131 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/mocks.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11726 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.088642 gwpy-3.0.4/gwpy/time/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1812 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/time/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2285 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/time/__main__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8975 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/time/_tconvert.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.088642 gwpy-3.0.4/gwpy/time/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/time/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1362 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/time/tests/test_main.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5728 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/time/tests/test_time.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.088642 gwpy-3.0.4/gwpy/timeseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1134 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    56990 2023-04-12 12:10:02.000000 gwpy-3.0.4/gwpy/timeseries/core.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/timeseries/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      938 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1185 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/ascii.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/cache.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/core.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/timeseries/io/gwf/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13156 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/gwf/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    17130 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/gwf/framecpp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4776 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/gwf/framel.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6828 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/gwf/lalframe.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4214 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9334 2023-04-12 12:10:02.000000 gwpy-3.0.4/gwpy/timeseries/io/losc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7811 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/nds2.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3595 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/wav.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35787 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/statevector.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/timeseries/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      751 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    18215 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_core.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2265 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_io_gwf_framecpp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4969 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_io_gwf_lalframe.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1833 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_io_losc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12356 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_statevector.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    55164 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_timeseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    87612 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/timeseries.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/types/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1159 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    15282 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/array.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12367 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/array2d.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3074 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/types/index.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/types/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      905 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2872 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/io/ascii.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8002 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7267 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    36772 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/series.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3567 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/sliceutils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/gwpy/types/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8608 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/tests/test_array.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9081 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/types/tests/test_array2d.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2044 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/types/tests/test_index.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14762 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/types/tests/test_series.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/gwpy/utils/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      933 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3723 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/decorators.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1490 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/enum.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1911 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8507 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3284 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/misc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5057 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1367 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/progress.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3396 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/shell.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/gwpy/utils/sphinx/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      770 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/sphinx/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3559 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/sphinx/epydoc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4763 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/sphinx/ex2rst.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3425 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/sphinx/zenodo.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/gwpy/utils/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2209 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_decorators.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2185 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_enum.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2000 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/tests/test_env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3478 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2610 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_misc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2062 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2367 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/tests/test_shell.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2263 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/tests/test_sphinx_ex2rst.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10040 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       54 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/entry_points.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      793 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        5 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4844 2023-04-12 10:27:17.000000 gwpy-3.0.4/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)       38 2023-04-12 12:14:41.108642 gwpy-3.0.4/setup.cfg
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)     2989 2023-04-06 10:37:11.000000 gwpy-3.0.4/setup_utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.297606 gwpy-3.0.5/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      524 2023-04-06 10:37:11.000000 gwpy-3.0.5/.codeclimate.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      498 2023-04-06 10:37:11.000000 gwpy-3.0.5/.codecov.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      483 2023-04-06 10:37:11.000000 gwpy-3.0.5/.flake8
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       30 2023-04-06 10:37:11.000000 gwpy-3.0.5/.gitattributes
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.007606 gwpy-3.0.5/.github/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.097606 gwpy-3.0.5/.github/workflows/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5119 2023-04-14 15:14:06.000000 gwpy-3.0.5/.github/workflows/conda.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2920 2023-04-06 10:37:11.000000 gwpy-3.0.5/.github/workflows/dependencies.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3119 2023-04-06 10:37:11.000000 gwpy-3.0.5/.github/workflows/dist.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1415 2023-04-14 15:14:06.000000 gwpy-3.0.5/.github/workflows/lint.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      726 2023-04-06 10:37:11.000000 gwpy-3.0.5/.gitignore
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2023-04-06 10:37:11.000000 gwpy-3.0.5/.pep8speaks.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      133 2023-04-06 10:37:11.000000 gwpy-3.0.5/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4481 2023-04-06 10:37:11.000000 gwpy-3.0.5/CONTRIBUTING.md
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2023-04-06 10:37:11.000000 gwpy-3.0.5/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2023-04-06 10:37:11.000000 gwpy-3.0.5/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-06-02 08:36:27.297606 gwpy-3.0.5/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1800 2023-04-06 10:37:11.000000 gwpy-3.0.5/README.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.097606 gwpy-3.0.5/docs/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      788 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/Makefile
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.097606 gwpy-3.0.5/docs/_static/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.097606 gwpy-3.0.5/docs/_static/css/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/_static/css/gwpy-sphinx.css
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    19634 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/_static/favicon.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    15166 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/_static/gwpy_white_24.png
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.017606 gwpy-3.0.5/docs/_templates/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.097606 gwpy-3.0.5/docs/_templates/autoclass/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      860 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/_templates/autoclass/class.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.107606 gwpy-3.0.5/docs/_templates/autosummary/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      170 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1145 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      703 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.107606 gwpy-3.0.5/docs/astro/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      735 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/astro/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2653 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/citing.rst.in
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.107606 gwpy-3.0.5/docs/cli/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5295 2023-04-14 15:14:06.000000 gwpy-3.0.5/docs/cli/examples.ini
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2879 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/cli/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13301 2023-04-14 15:14:06.000000 gwpy-3.0.5/docs/conf.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.107606 gwpy-3.0.5/docs/detector/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3245 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/detector/channel.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.107606 gwpy-3.0.5/docs/dev/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3787 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/dev/release.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1624 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/env.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.027606 gwpy-3.0.5/docs/examples/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.107606 gwpy-3.0.5/docs/examples/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.107606 gwpy-3.0.5/docs/external/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1162 2023-04-14 15:14:06.000000 gwpy-3.0.5/docs/external/framecpp.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      990 2023-04-14 15:14:06.000000 gwpy-3.0.5/docs/external/framel.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3134 2023-04-14 15:14:06.000000 gwpy-3.0.5/docs/external/lalsuite.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1025 2023-04-14 15:14:06.000000 gwpy-3.0.5/docs/external/nds2.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    52297 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/gwpy-docs-logo.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2491 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1300 2023-06-02 08:29:18.000000 gwpy-3.0.5/docs/install.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2694 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/overview.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.117606 gwpy-3.0.5/docs/plot/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/plot/colorbars.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2985 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/plot/colors.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      772 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/plot/filter.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2514 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/plot/gps.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/plot/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1838 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/plot/legend.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1363 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/plot/log.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4903 2023-06-02 08:29:18.000000 gwpy-3.0.5/docs/references.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.117606 gwpy-3.0.5/docs/segments/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1513 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/segments/dqsegdb.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6818 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/segments/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6756 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/segments/io.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2124 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/segments/thresholding.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.117606 gwpy-3.0.5/docs/signal/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4369 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/signal/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.117606 gwpy-3.0.5/docs/spectrogram/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3771 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/spectrogram/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.117606 gwpy-3.0.5/docs/spectrum/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      505 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/spectrum/filtering.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3732 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/spectrum/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4986 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/spectrum/io.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.127606 gwpy-3.0.5/docs/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7364 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/table/filter.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      955 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/table/histogram.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1500 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/table/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    30432 2023-06-02 08:29:18.000000 gwpy-3.0.5/docs/table/io.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1756 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/table/plot.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2142 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/table/rate.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.127606 gwpy-3.0.5/docs/time/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1085 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/time/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.127606 gwpy-3.0.5/docs/timeseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11634 2023-04-14 15:14:06.000000 gwpy-3.0.5/docs/timeseries/datafind.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2722 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/timeseries/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10656 2023-04-14 15:14:06.000000 gwpy-3.0.5/docs/timeseries/io.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2731 2023-06-02 08:29:18.000000 gwpy-3.0.5/docs/timeseries/opendata.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3032 2023-04-06 10:37:11.000000 gwpy-3.0.5/docs/timeseries/plot.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8457 2023-06-02 08:29:18.000000 gwpy-3.0.5/docs/timeseries/statevector.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.127606 gwpy-3.0.5/examples/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.127606 gwpy-3.0.5/examples/frequencyseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2584 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/frequencyseries/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2065 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/frequencyseries/hoff.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      258 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/frequencyseries/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2585 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/frequencyseries/inject.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/frequencyseries/percentiles.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/frequencyseries/rayleigh.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2203 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/frequencyseries/transfer_function.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2630 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/frequencyseries/variance.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.127606 gwpy-3.0.5/examples/miscellaneous/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      216 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/miscellaneous/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3328 2023-06-02 08:29:18.000000 gwpy-3.0.5/examples/miscellaneous/open-data-spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2353 2023-06-02 08:29:18.000000 gwpy-3.0.5/examples/miscellaneous/range-spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2477 2023-06-02 08:29:18.000000 gwpy-3.0.5/examples/miscellaneous/range-timeseries.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.137606 gwpy-3.0.5/examples/segments/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      158 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/segments/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2398 2023-06-02 08:29:18.000000 gwpy-3.0.5/examples/segments/open-data.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.137606 gwpy-3.0.5/examples/signal/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5642 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/signal/gw150914.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      179 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/signal/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3139 2023-04-14 15:14:06.000000 gwpy-3.0.5/examples/signal/qscan.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.137606 gwpy-3.0.5/examples/spectrogram/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2387 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/spectrogram/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/spectrogram/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2627 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/spectrogram/plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2581 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/spectrogram/ratio.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2125 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/spectrogram/rayleigh.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2885 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/spectrogram/spectrogram2.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.137606 gwpy-3.0.5/examples/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1597 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/table/histogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      198 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/table/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2317 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/table/rate.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2460 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/table/rate_binned.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2018 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/table/scatter.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2287 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/table/tiles.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3734 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/test_examples.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.137606 gwpy-3.0.5/examples/timeseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2644 2023-05-30 16:45:11.000000 gwpy-3.0.5/examples/timeseries/blrms.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4204 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/timeseries/correlate.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2797 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/timeseries/filter.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      246 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/timeseries/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2628 2023-06-02 08:29:18.000000 gwpy-3.0.5/examples/timeseries/inject.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2466 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/timeseries/public.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3788 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/timeseries/pycbc-snr.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/timeseries/qscan.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2202 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/timeseries/statevector.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2476 2023-04-06 10:37:11.000000 gwpy-3.0.5/examples/timeseries/whiten.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.147606 gwpy-3.0.5/gwpy/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1533 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-06-02 08:36:26.000000 gwpy-3.0.5/gwpy/_version.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.147606 gwpy-3.0.5/gwpy/astro/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1909 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/astro/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    24880 2023-05-23 15:12:46.000000 gwpy-3.0.5/gwpy/astro/range.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.147606 gwpy-3.0.5/gwpy/astro/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/astro/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6032 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/astro/tests/test_range.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.157606 gwpy-3.0.5/gwpy/cli/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1404 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    34269 2023-05-30 16:45:11.000000 gwpy-3.0.5/gwpy/cli/cliproduct.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4048 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3353 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/coherencegram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5121 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/gwpy_plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9140 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/qtransform.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7131 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4899 2023-05-30 16:45:11.000000 gwpy-3.0.5/gwpy/cli/spectrum.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.157606 gwpy-3.0.5/gwpy/cli/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      744 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10831 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/base.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1353 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/test_coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1580 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/test_coherencegram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1718 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/test_gwpy_plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2899 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/test_qtransform.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1509 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/test_spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1416 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/test_spectrum.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1279 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/test_timeseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1999 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/tests/test_transferfunction.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3891 2023-05-30 16:45:11.000000 gwpy-3.0.5/gwpy/cli/timeseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9784 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/cli/transferfunction.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1639 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/conftest.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.157606 gwpy-3.0.5/gwpy/detector/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2252 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/detector/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    26901 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/detector/channel.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.167606 gwpy-3.0.5/gwpy/detector/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1037 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/detector/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3184 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/detector/io/cis.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5689 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/detector/io/clf.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5939 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/detector/io/omega.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.167606 gwpy-3.0.5/gwpy/detector/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/detector/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    18473 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/detector/tests/test_channel.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2548 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/detector/tests/test_units.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7113 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/detector/units.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.167606 gwpy-3.0.5/gwpy/frequencyseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      995 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/frequencyseries/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1943 2023-05-30 15:01:02.000000 gwpy-3.0.5/gwpy/frequencyseries/_fdcommon.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14328 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/frequencyseries/frequencyseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11947 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/frequencyseries/hist.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.167606 gwpy-3.0.5/gwpy/frequencyseries/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      907 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/frequencyseries/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1071 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/frequencyseries/io/ascii.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1036 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/frequencyseries/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1149 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/frequencyseries/io/ligolw.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.167606 gwpy-3.0.5/gwpy/frequencyseries/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      756 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/frequencyseries/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11033 2023-05-30 15:01:02.000000 gwpy-3.0.5/gwpy/frequencyseries/tests/test_frequencyseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4126 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/frequencyseries/tests/test_hist.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.177606 gwpy-3.0.5/gwpy/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      831 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4250 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/io/_framecpp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14662 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/cache.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18462 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/datafind.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8399 2023-05-05 11:11:46.000000 gwpy-3.0.5/gwpy/io/ffldatafind.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18966 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/io/gwf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5257 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6928 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    22182 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4116 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    19331 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/nds2.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3518 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/registry.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.187606 gwpy-3.0.5/gwpy/io/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      743 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8567 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/io/tests/test_cache.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10597 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/io/tests/test_datafind.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6277 2023-05-05 11:11:46.000000 gwpy-3.0.5/gwpy/io/tests/test_ffldatafind.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4228 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/io/tests/test_gwf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/io/tests/test_kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10701 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/io/tests/test_ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3293 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/io/tests/test_mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12185 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/io/tests/test_nds2.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3971 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/io/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7341 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/io/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.187606 gwpy-3.0.5/gwpy/plot/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1641 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    23094 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/axes.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8733 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/bode.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7041 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/plot/colorbar.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3367 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/colors.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    16720 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/plot/gps.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1635 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/legend.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5030 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/plot/log.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    21766 2023-04-24 12:31:10.000000 gwpy-3.0.5/gwpy/plot/plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4816 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/rc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    16943 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.197606 gwpy-3.0.5/gwpy/plot/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      740 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11542 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/plot/tests/test_axes.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3351 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/test_bode.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1881 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/test_colors.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5456 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/test_gps.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2652 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/test_log.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4398 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/test_plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1252 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/test_rc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5442 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/test_segments.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2318 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/plot/tests/test_tex.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/test_text.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1615 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1925 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/tests/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4783 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/plot/tex.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1989 2023-05-12 13:04:55.000000 gwpy-3.0.5/gwpy/plot/text.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1825 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/plot/units.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1670 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/plot/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.197606 gwpy-3.0.5/gwpy/segments/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1194 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/segments/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    52661 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/segments/flag.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.207606 gwpy-3.0.5/gwpy/segments/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1005 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/segments/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11048 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/segments/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3036 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/segments/io/json.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4907 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/segments/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5007 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/segments/io/segwizard.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9042 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/segments/segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.207606 gwpy-3.0.5/gwpy/segments/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/segments/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    29683 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/segments/tests/test_flag.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5360 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/segments/tests/test_segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.207606 gwpy-3.0.5/gwpy/signal/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      972 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1189 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/fft.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    20270 2023-05-30 15:01:02.000000 gwpy-3.0.5/gwpy/signal/filter_design.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    24471 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/signal/qtransform.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.217606 gwpy-3.0.5/gwpy/signal/spectral/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1818 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/spectral/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12000 2023-04-26 20:12:51.000000 gwpy-3.0.5/gwpy/signal/spectral/_lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1851 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/spectral/_median_mean.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3577 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/spectral/_pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2346 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/spectral/_registry.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7711 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/signal/spectral/_scipy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14241 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/spectral/_ui.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1669 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/spectral/_utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.217606 gwpy-3.0.5/gwpy/signal/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      747 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5088 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/signal/tests/test_coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4349 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/test_filter_design.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4017 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/test_qtransform.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3543 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/test_spectral_lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2195 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/test_spectral_median_mean.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2249 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/test_spectral_pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1446 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/test_spectral_registry.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1874 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/test_spectral_scipy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3045 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/test_spectral_ui.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1453 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/signal/tests/test_spectral_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2726 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/signal/tests/test_window.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5927 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/signal/window.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.227606 gwpy-3.0.5/gwpy/spectrogram/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      919 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/spectrogram/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5742 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/spectrogram/coherence.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.227606 gwpy-3.0.5/gwpy/spectrogram/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      846 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/spectrogram/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      963 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/spectrogram/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    22206 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/spectrogram/spectrogram.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.227606 gwpy-3.0.5/gwpy/spectrogram/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      752 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/spectrogram/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6590 2023-05-30 15:01:02.000000 gwpy-3.0.5/gwpy/spectrogram/tests/test_spectrogram.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.227606 gwpy-3.0.5/gwpy/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1418 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7918 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/filter.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2645 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/filters.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8173 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/gravityspy.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.237606 gwpy-3.0.5/gwpy/table/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1564 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3809 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/cwb.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/fetch.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4663 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/gravityspy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8390 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/gstlal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5433 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/gwf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5205 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/hacr.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13590 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4434 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/losc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2604 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/omega.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1333 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/omicron.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8894 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3318 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/root.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3857 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/snax.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3067 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/sql.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3183 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/io/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    26330 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/table.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.237606 gwpy-3.0.5/gwpy/table/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3392 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/table/tests/test_gravityspy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7979 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/tests/test_io_gstlal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2848 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/table/tests/test_io_ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8313 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/table/tests/test_io_pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    30399 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/table/tests/test_table.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.237606 gwpy-3.0.5/gwpy/testing/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/__init__.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.267606 gwpy-3.0.5/gwpy/testing/data/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)   377295 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/data/HLV-HW100916-968654552-1.gwf
+-rw-r--r--   0 duncan    (1000) duncan    (1000)   382679 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/data/HLV-HW100916-968654552-1.hdf
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       59 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      564 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2783 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/testing/errors.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3772 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/fixtures.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1480 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/marks.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4131 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/mocks.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11726 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/testing/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.267606 gwpy-3.0.5/gwpy/time/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1812 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/time/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2285 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/time/__main__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8975 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/time/_tconvert.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.267606 gwpy-3.0.5/gwpy/time/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/time/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1362 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/time/tests/test_main.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5728 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/time/tests/test_time.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.267606 gwpy-3.0.5/gwpy/timeseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1134 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    57425 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/timeseries/core.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.277606 gwpy-3.0.5/gwpy/timeseries/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      938 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1185 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/ascii.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/cache.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/core.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.277606 gwpy-3.0.5/gwpy/timeseries/io/gwf/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13156 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/gwf/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    17130 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/gwf/framecpp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4776 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/gwf/framel.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6828 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/gwf/lalframe.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4214 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9334 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/timeseries/io/losc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7811 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/nds2.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3595 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/io/wav.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35811 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/timeseries/statevector.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.277606 gwpy-3.0.5/gwpy/timeseries/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      751 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    18934 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/timeseries/tests/test_core.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2265 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/tests/test_io_gwf_framecpp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4969 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/timeseries/tests/test_io_gwf_lalframe.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1833 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/timeseries/tests/test_io_losc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12935 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/timeseries/tests/test_statevector.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    55461 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/timeseries/tests/test_timeseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    87809 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/timeseries/timeseries.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.287606 gwpy-3.0.5/gwpy/types/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1159 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/types/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    15282 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/types/array.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12367 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/types/array2d.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3074 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/types/index.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.287606 gwpy-3.0.5/gwpy/types/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      905 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/types/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2872 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/types/io/ascii.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8019 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/types/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7267 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/types/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    36535 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/types/series.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3567 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/types/sliceutils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.287606 gwpy-3.0.5/gwpy/types/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/types/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8608 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/types/tests/test_array.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9081 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/types/tests/test_array2d.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2044 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/types/tests/test_index.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    15551 2023-06-02 08:29:18.000000 gwpy-3.0.5/gwpy/types/tests/test_series.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.297606 gwpy-3.0.5/gwpy/utils/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      933 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3723 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/decorators.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1490 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/enum.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1911 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8507 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3284 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/misc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5057 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1367 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/progress.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3396 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/shell.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.297606 gwpy-3.0.5/gwpy/utils/sphinx/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      770 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/sphinx/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3559 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/sphinx/epydoc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4763 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/sphinx/ex2rst.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3425 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/sphinx/zenodo.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.297606 gwpy-3.0.5/gwpy/utils/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2209 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/utils/tests/test_decorators.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2185 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/utils/tests/test_enum.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2000 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/tests/test_env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3478 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/utils/tests/test_lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2610 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/utils/tests/test_misc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2062 2023-04-14 15:14:06.000000 gwpy-3.0.5/gwpy/utils/tests/test_mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2367 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/tests/test_shell.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2263 2023-04-06 10:37:11.000000 gwpy-3.0.5/gwpy/utils/tests/test_sphinx_ex2rst.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-02 08:36:27.147606 gwpy-3.0.5/gwpy.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-06-02 08:36:26.000000 gwpy-3.0.5/gwpy.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10076 2023-06-02 08:36:26.000000 gwpy-3.0.5/gwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-06-02 08:36:26.000000 gwpy-3.0.5/gwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       54 2023-06-02 08:36:26.000000 gwpy-3.0.5/gwpy.egg-info/entry_points.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      793 2023-06-02 08:36:26.000000 gwpy-3.0.5/gwpy.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        5 2023-06-02 08:36:26.000000 gwpy-3.0.5/gwpy.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4844 2023-06-02 08:29:18.000000 gwpy-3.0.5/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       38 2023-06-02 08:36:27.297606 gwpy-3.0.5/setup.cfg
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)     2989 2023-04-06 10:37:11.000000 gwpy-3.0.5/setup_utils.py
```

### Comparing `gwpy-3.0.4/.codeclimate.yml` & `gwpy-3.0.5/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/.github/workflows/conda.yml` & `gwpy-3.0.5/.github/workflows/conda.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/.github/workflows/dependencies.yml` & `gwpy-3.0.5/.github/workflows/dependencies.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/.github/workflows/dist.yml` & `gwpy-3.0.5/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/.github/workflows/lint.yml` & `gwpy-3.0.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/.gitignore` & `gwpy-3.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/CONTRIBUTING.md` & `gwpy-3.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/LICENSE` & `gwpy-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/PKG-INFO` & `gwpy-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpy
-Version: 3.0.4
+Version: 3.0.5
 Summary: A python package for gravitational-wave astrophysics
 Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwpy/gwpy/issues
 Project-URL: Discussion Forum, https://gwpy.slack.com
 Project-URL: Documentation, https://gwpy.github.io/docs/
 Project-URL: Source Code, https://github.com/gwpy/gwpy
```

### Comparing `gwpy-3.0.4/README.md` & `gwpy-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/Makefile` & `gwpy-3.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/_static/css/gwpy-sphinx.css` & `gwpy-3.0.5/docs/_static/css/gwpy-sphinx.css`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/_static/favicon.png` & `gwpy-3.0.5/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/_static/gwpy_white_24.png` & `gwpy-3.0.5/docs/_static/gwpy_white_24.png`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/_templates/autoclass/class.rst` & `gwpy-3.0.5/docs/_templates/autoclass/class.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/_templates/autosummary/class.rst` & `gwpy-3.0.5/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/_templates/autosummary/module.rst` & `gwpy-3.0.5/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/astro/index.rst` & `gwpy-3.0.5/docs/astro/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/citing.rst.in` & `gwpy-3.0.5/docs/citing.rst.in`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/cli/examples.ini` & `gwpy-3.0.5/docs/cli/examples.ini`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/cli/index.rst` & `gwpy-3.0.5/docs/cli/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/conf.py` & `gwpy-3.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/detector/channel.rst` & `gwpy-3.0.5/docs/detector/channel.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/dev/release.rst` & `gwpy-3.0.5/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/env.rst` & `gwpy-3.0.5/docs/env.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.5/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/external/framecpp.rst` & `gwpy-3.0.5/docs/external/framecpp.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/external/framel.rst` & `gwpy-3.0.5/docs/external/framel.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/external/lalsuite.rst` & `gwpy-3.0.5/docs/external/lalsuite.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/external/nds2.rst` & `gwpy-3.0.5/docs/external/nds2.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/gwpy-docs-logo.png` & `gwpy-3.0.5/docs/gwpy-docs-logo.png`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/index.rst` & `gwpy-3.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/install.rst` & `gwpy-3.0.5/docs/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
    ==================  ===========================
    Name                Constraints
    ==================  ===========================
    |astropy|_          ``>=4.0``
    |dqsegdb2|_
    |gwdatafind|_       ``>=1.1.0``
    |gwosc-mod|_        ``>=0.5.3``
-   |h5py|_             ``>=2.8.0``
+   |h5py|_             ``>=3.0.0``
    |ligo-segments|_    ``>=1.0.0``
    |ligotimegps|_      ``>=1.2.1``
    |matplotlib|_       ``>=3.1.0``
    |numpy|_            ``>=1.16.0``
    |dateutil|_
    |scipy|_            ``>=1.2.0``
    |tqdm|_             ``>=4.10.0``
```

### Comparing `gwpy-3.0.4/docs/overview.rst` & `gwpy-3.0.5/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/plot/colorbars.rst` & `gwpy-3.0.5/docs/plot/colorbars.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/plot/colors.rst` & `gwpy-3.0.5/docs/plot/colors.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/plot/filter.rst` & `gwpy-3.0.5/docs/plot/filter.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/plot/gps.rst` & `gwpy-3.0.5/docs/plot/gps.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/plot/index.rst` & `gwpy-3.0.5/docs/plot/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/plot/legend.rst` & `gwpy-3.0.5/docs/plot/legend.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/plot/log.rst` & `gwpy-3.0.5/docs/plot/log.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/references.rst` & `gwpy-3.0.5/docs/references.rst`

 * *Files 12% similar despite different names*

```diff
@@ -99,58 +99,58 @@
 
 .. -- Other references --------------------------
 
 .. |GravitySpy| replace:: Gravity Spy
 .. _GravitySpy: https://gravityspy.org
 
 .. |GWOSCl| replace:: The Gravitational-Wave Open Science Centre (GWOSC)
-.. _GWOSCl: https://www.gw-openscience.org/
+.. _GWOSCl: https://gwosc.org/
 
 .. |GWOSC| replace:: GWOSC
-.. _GWOSC: https://www.gw-openscience.org/
+.. _GWOSC: https://gwosc.org/
 
 .. |GWOSC_AUX_RELEASE| replace:: Auxiliary Channel Three Hour Release
-.. _GWOSC_AUX_RELEASE: https://www.gw-openscience.org/auxiliary/GW170814/
+.. _GWOSC_AUX_RELEASE: https://gwosc.org/auxiliary/GW170814/
 
 .. |LIGO-T050017| replace:: LIGO-T050017
 .. _LIGO-T050017: https://dcc.ligo.org/LIGO-T050017/public
 
 .. -- Event science summaries -------------------
 
 .. catalogues
 
 .. |GWTCl| replace:: Gravitational-Wave Transient Catalogue (GWTC)
-.. _GWTCl: https://www.gw-openscience.org/eventapi/html/GWTC/
+.. _GWTCl: https://gwosc.org/eventapi/html/GWTC/
 
 .. |GWTC| replace:: GWTC
-.. _GWTC: https://www.gw-openscience.org/eventapi/html/GWTC/
+.. _GWTC: https://gwosc.org/eventapi/html/GWTC/
 
 .. |GWTC-1l| replace:: Gravitational-Wave Transient Catalogue (GWTC) 1
-.. _GWTC-1l: https://www.gw-openscience.org/GWTC-1/
+.. _GWTC-1l: https://gwosc.org/GWTC-1/
 
 .. |GWTC-1| replace:: GWTC-1
-.. _GWTC-1: https://www.gw-openscience.org/GWTC-1/
+.. _GWTC-1: https://gwosc.org/GWTC-1/
 
 .. |GWTC-2l| replace:: Gravitational-Wave Transient Catalogue (GWTC) 2
-.. _GWTC-2l: https://www.gw-openscience.org/GWTC-2/
+.. _GWTC-2l: https://gwosc.org/GWTC-2/
 
 .. |GWTC-2| replace:: GWTC-2
-.. _GWTC-2: https://www.gw-openscience.org/GWTC-2/
+.. _GWTC-2: https://gwosc.org/GWTC-2/
 
 .. |GWTC-2.1l| replace:: Gravitational-Wave Transient Catalogue (GWTC) 2.1
-.. _GWTC-2.1l: https://www.gw-openscience.org/GWTC-2.1/
+.. _GWTC-2.1l: https://gwosc.org/GWTC-2.1/
 
 .. |GWTC-2.1| replace:: GWTC-2.1
-.. _GWTC-2.1: https://www.gw-openscience.org/GWTC-2.1/
+.. _GWTC-2.1: https://gwosc.org/GWTC-2.1/
 
 .. |GWTC-3l| replace:: Gravitational-Wave Transient Catalogue (GWTC) 3
-.. _GWTC-3l: https://www.gw-openscience.org/GWTC-3/
+.. _GWTC-3l: https://gwosc.org/GWTC-3/
 
 .. |GWTC-3| replace:: GWTC-3
-.. _GWTC-3: https://www.gw-openscience.org/GWTC-3/
+.. _GWTC-3: https://gwosc.org/GWTC-3/
 
 .. events
 
 .. |GW150914| replace:: GW150914
 .. _GW150914: https://www.ligo.org/science/Publication-GW150914/
 
 .. |GW170814| replace:: GW170814
```

### Comparing `gwpy-3.0.4/docs/segments/dqsegdb.rst` & `gwpy-3.0.5/docs/segments/dqsegdb.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/segments/index.rst` & `gwpy-3.0.5/docs/segments/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/segments/io.rst` & `gwpy-3.0.5/docs/segments/io.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/segments/thresholding.rst` & `gwpy-3.0.5/docs/segments/thresholding.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/signal/index.rst` & `gwpy-3.0.5/docs/signal/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/spectrogram/index.rst` & `gwpy-3.0.5/docs/spectrogram/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/spectrum/index.rst` & `gwpy-3.0.5/docs/spectrum/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/spectrum/io.rst` & `gwpy-3.0.5/docs/spectrum/io.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.5/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/table/filter.rst` & `gwpy-3.0.5/docs/table/filter.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/table/histogram.rst` & `gwpy-3.0.5/docs/table/histogram.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/table/index.rst` & `gwpy-3.0.5/docs/table/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/table/io.rst` & `gwpy-3.0.5/docs/table/io.rst`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             chirp_mass_source_lower float64                  chirp_mass_source_lower
             total_mass_source_upper float64                  total_mass_source_upper
                    chirp_mass_lower float64                         chirp_mass_lower
    ...
 
 .. admonition:: GWOSC catalogues
 
-   For more details on the GWOSC catalogues, see https://www.gw-openscience.org/eventapi/html/.
+   For more details on the GWOSC catalogues, see https://gwosc.org/eventapi/html/.
 
 .. _gwpy-table-gwosc-filter:
 
 ================
 Filtered queries
 ================
```

### Comparing `gwpy-3.0.4/docs/table/plot.rst` & `gwpy-3.0.5/docs/table/plot.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/table/rate.rst` & `gwpy-3.0.5/docs/table/rate.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/time/index.rst` & `gwpy-3.0.5/docs/time/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/timeseries/datafind.rst` & `gwpy-3.0.5/docs/timeseries/datafind.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/timeseries/index.rst` & `gwpy-3.0.5/docs/timeseries/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/timeseries/io.rst` & `gwpy-3.0.5/docs/timeseries/io.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/timeseries/opendata.rst` & `gwpy-3.0.5/docs/timeseries/opendata.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 public use, including small datasets around each GW event detection,
 and bulk datasets covering entire observing epochs.
 
 .. note::
 
    For full details of the available data, please see
 
-   https://www.gw-openscience.org/data/
+   https://gwosc.org/data/
 
 .. _gwpy-timeseries-fetchopendata:
 
 **********************************
 :meth:`TimeSeries.fetch_open_data`
 **********************************
```

### Comparing `gwpy-3.0.4/docs/timeseries/plot.rst` & `gwpy-3.0.5/docs/timeseries/plot.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/docs/timeseries/statevector.rst` & `gwpy-3.0.5/docs/timeseries/statevector.rst`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 Each |GWOSC|_ data release includes a bit vector that describes the
 data-quality states of the detector.
 
 .. admonition:: GWOSC data usage notes
 
    Refer to the GWOSC
-   `data usage notes <https://www.gw-openscience.org/yellow_box/>`__
+   `data usage notes <https://gwosc.org/yellow_box/>`__
    page for details of the various bits (states) in the state vectors.
 
 To demonstate, we can download the `StateVector` associated with
 |GW200105|_, the first detection of a mixed black hole/neutron star
 binary system:
 
 .. plot::
```

### Comparing `gwpy-3.0.4/examples/frequencyseries/coherence.py` & `gwpy-3.0.5/examples/frequencyseries/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/frequencyseries/hoff.py` & `gwpy-3.0.5/examples/frequencyseries/hoff.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/frequencyseries/inject.py` & `gwpy-3.0.5/examples/frequencyseries/inject.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/frequencyseries/percentiles.py` & `gwpy-3.0.5/examples/frequencyseries/percentiles.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/frequencyseries/rayleigh.py` & `gwpy-3.0.5/examples/frequencyseries/rayleigh.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/frequencyseries/transfer_function.py` & `gwpy-3.0.5/examples/frequencyseries/transfer_function.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/frequencyseries/variance.py` & `gwpy-3.0.5/examples/frequencyseries/variance.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/miscellaneous/open-data-spectrogram.py` & `gwpy-3.0.5/examples/miscellaneous/open-data-spectrogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """Plotting a spectrogram of all open data for 1 day
 
 In order to study interferometer performance, it is common in LIGO to plot
 all of the data for a day, in order to determine trends, and see data-quality
 issues.
 
 This is done for the LIGO-Virgo detector network, with
-`up-to-date plots <https://www.gw-openscience.org/detector_status/>`__
+`up-to-date plots <https://gwosc.org/detector_status/>`__
 available from |GWOSC|.
 
 This example demonstrates how to download data segments from GWOSC, then
 use those to build a day-timescale spectrogram plot of LIGO-Hanford strain
 data.
 """
 
@@ -38,15 +38,15 @@
 #
 # Getting the segments
 # --------------------
 #
 # First, we need to fetch the Open Data timeline segments from GWOSC.
 # To do that we can call the :meth:`DataQualityFlag.fetch_open_data` method
 # using ``'H1_DATA'`` as the flag (for an explanation of what this means,
-# read up on `The S6 Data Release <https://www.gw-openscience.org/S6/>`__).
+# read up on `The S6 Data Release <https://gwosc.org/S6/>`__).
 
 from gwpy.segments import DataQualityFlag
 h1segs = DataQualityFlag.fetch_open_data('H1_DATA',
                                          'Sep 16 2010', 'Sep 17 2010')
 
 # For sanity, lets plot these segments:
```

### Comparing `gwpy-3.0.4/examples/miscellaneous/range-spectrogram.py` & `gwpy-3.0.5/examples/miscellaneous/range-spectrogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 contribution to BNS range from the strain record surrounding GW170817
 using :func:`gwpy.astro.range_spectrogram`.
 """
 
 __author__ = 'Alex Urban <alexander.urban@ligo.org>'
 
 # First, we need to load some data. As before we can `fetch` the
-# `public data <https://www.gw-openscience.org/catalog/>`__
+# `public data <https://gwosc.org/catalog/>`__
 # around the GW170817 BNS merger:
 
 from gwpy.timeseries import TimeSeries
 l1 = TimeSeries.fetch_open_data('L1', 1187006834, 1187010930)
 
 # Then, we can calculate a `Spectrogram` of the inspiral range
 # amplitude spectrum:
```

### Comparing `gwpy-3.0.4/examples/miscellaneous/range-timeseries.py` & `gwpy-3.0.5/examples/miscellaneous/range-timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 a detector.
 """
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 __credits__ = 'Alex Urban <alexander.urban@ligo.org>'
 
 # First, we need to load some data. We can `fetch` the
-# `public data <https://www.gw-openscience.org/catalog/>`__
+# `public data <https://gwosc.org/catalog/>`__
 # around the GW170817 BNS merger:
 
 from gwpy.timeseries import TimeSeries
 h1 = TimeSeries.fetch_open_data('H1', 1187006834, 1187010930)
 l1 = TimeSeries.fetch_open_data('L1', 1187006834, 1187010930)
 
 # Then, we can measure the inspiral range directly:
```

### Comparing `gwpy-3.0.4/examples/segments/open-data.py` & `gwpy-3.0.5/examples/segments/open-data.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GWpy.  If not, see <http://www.gnu.org/licenses/>.
 
 """Plotting observing segments for O1
 
 The data from the full
-`Observing Run 1 (O1) <https://www.gw-openscience.org/O1/>`__
+`Observing Run 1 (O1) <https://gwosc.org/O1/>`__
 have been released by |GWOSC|_.
 
 This example demonstrates how to download segment information into a
 :class:`~gwpy.segments.DataQualityFlag`, and then plot them.
 """
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
```

### Comparing `gwpy-3.0.4/examples/signal/gw150914.py` & `gwpy-3.0.5/examples/signal/gw150914.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/signal/qscan.py` & `gwpy-3.0.5/examples/signal/qscan.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/spectrogram/coherence.py` & `gwpy-3.0.5/examples/spectrogram/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/spectrogram/plot.py` & `gwpy-3.0.5/examples/spectrogram/plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/spectrogram/ratio.py` & `gwpy-3.0.5/examples/spectrogram/ratio.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/spectrogram/rayleigh.py` & `gwpy-3.0.5/examples/spectrogram/rayleigh.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/spectrogram/spectrogram2.py` & `gwpy-3.0.5/examples/spectrogram/spectrogram2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.5/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/table/histogram.py` & `gwpy-3.0.5/examples/table/histogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/table/rate.py` & `gwpy-3.0.5/examples/table/rate.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/table/rate_binned.py` & `gwpy-3.0.5/examples/table/rate_binned.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/table/scatter.py` & `gwpy-3.0.5/examples/table/scatter.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/table/tiles.py` & `gwpy-3.0.5/examples/table/tiles.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/test_examples.py` & `gwpy-3.0.5/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/timeseries/blrms.py` & `gwpy-3.0.5/examples/timeseries/blrms.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/timeseries/correlate.py` & `gwpy-3.0.5/examples/timeseries/correlate.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/timeseries/filter.py` & `gwpy-3.0.5/examples/timeseries/filter.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/timeseries/inject.py` & `gwpy-3.0.5/examples/timeseries/inject.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from numpy import random
 from gwpy.timeseries import TimeSeries
 noise = TimeSeries(random.normal(scale=.1, size=16384), sample_rate=16384)
 
 # Then we can download a simulation of the GW150914 signal from GWOSC:
 
 from astropy.utils.data import get_readable_fileobj
-url = ("https://www.gw-openscience.org/s/events/GW150914/P150914/"
+url = ("https://gwosc.org/s/events/GW150914/P150914/"
        "fig2-unfiltered-waveform-H.txt")
 with get_readable_fileobj(url) as f:
     signal = TimeSeries.read(f, format='txt')
 signal.t0 = .5  # make sure this intersects with noise time samples
 
 # Note, since this simulation cuts off before a certain time, it is
 # important to taper its ends to zero to avoid ringing artifacts.
```

### Comparing `gwpy-3.0.4/examples/timeseries/public.py` & `gwpy-3.0.5/examples/timeseries/public.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/timeseries/pycbc-snr.py` & `gwpy-3.0.5/examples/timeseries/pycbc-snr.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/timeseries/qscan.py` & `gwpy-3.0.5/examples/timeseries/qscan.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/timeseries/statevector.py` & `gwpy-3.0.5/examples/timeseries/statevector.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/examples/timeseries/whiten.py` & `gwpy-3.0.5/examples/timeseries/whiten.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/__init__.py` & `gwpy-3.0.5/gwpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/astro/__init__.py` & `gwpy-3.0.5/gwpy/astro/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/astro/range.py` & `gwpy-3.0.5/gwpy/astro/range.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/astro/tests/__init__.py` & `gwpy-3.0.5/gwpy/astro/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/astro/tests/test_range.py` & `gwpy-3.0.5/gwpy/astro/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/__init__.py` & `gwpy-3.0.5/gwpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/cliproduct.py` & `gwpy-3.0.5/gwpy/cli/cliproduct.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/coherence.py` & `gwpy-3.0.5/gwpy/cli/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/coherencegram.py` & `gwpy-3.0.5/gwpy/cli/coherencegram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/gwpy_plot.py` & `gwpy-3.0.5/gwpy/cli/gwpy_plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/qtransform.py` & `gwpy-3.0.5/gwpy/cli/qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/spectrogram.py` & `gwpy-3.0.5/gwpy/cli/spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/spectrum.py` & `gwpy-3.0.5/gwpy/cli/spectrum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/__init__.py` & `gwpy-3.0.5/gwpy/cli/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/base.py` & `gwpy-3.0.5/gwpy/cli/tests/base.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/test_coherence.py` & `gwpy-3.0.5/gwpy/cli/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/test_coherencegram.py` & `gwpy-3.0.5/gwpy/cli/tests/test_coherencegram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/test_gwpy_plot.py` & `gwpy-3.0.5/gwpy/cli/tests/test_gwpy_plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/test_qtransform.py` & `gwpy-3.0.5/gwpy/cli/tests/test_qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/test_spectrogram.py` & `gwpy-3.0.5/gwpy/cli/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/test_spectrum.py` & `gwpy-3.0.5/gwpy/cli/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/test_timeseries.py` & `gwpy-3.0.5/gwpy/cli/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/tests/test_transferfunction.py` & `gwpy-3.0.5/gwpy/cli/tests/test_transferfunction.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/timeseries.py` & `gwpy-3.0.5/gwpy/cli/timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/cli/transferfunction.py` & `gwpy-3.0.5/gwpy/cli/transferfunction.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/conftest.py` & `gwpy-3.0.5/gwpy/conftest.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/__init__.py` & `gwpy-3.0.5/gwpy/detector/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/channel.py` & `gwpy-3.0.5/gwpy/detector/channel.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/io/__init__.py` & `gwpy-3.0.5/gwpy/detector/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/io/cis.py` & `gwpy-3.0.5/gwpy/detector/io/cis.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/io/clf.py` & `gwpy-3.0.5/gwpy/detector/io/clf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/io/omega.py` & `gwpy-3.0.5/gwpy/detector/io/omega.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/tests/__init__.py` & `gwpy-3.0.5/gwpy/detector/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/tests/test_channel.py` & `gwpy-3.0.5/gwpy/detector/tests/test_channel.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/tests/test_units.py` & `gwpy-3.0.5/gwpy/detector/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/detector/units.py` & `gwpy-3.0.5/gwpy/detector/units.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/__init__.py` & `gwpy-3.0.5/gwpy/frequencyseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/_fdcommon.py` & `gwpy-3.0.5/gwpy/frequencyseries/_fdcommon.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/frequencyseries.py` & `gwpy-3.0.5/gwpy/frequencyseries/frequencyseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/hist.py` & `gwpy-3.0.5/gwpy/frequencyseries/hist.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/io/__init__.py` & `gwpy-3.0.5/gwpy/frequencyseries/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/io/ascii.py` & `gwpy-3.0.5/gwpy/frequencyseries/io/ascii.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/io/hdf5.py` & `gwpy-3.0.5/gwpy/frequencyseries/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/io/ligolw.py` & `gwpy-3.0.5/gwpy/frequencyseries/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/tests/__init__.py` & `gwpy-3.0.5/gwpy/frequencyseries/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/tests/test_frequencyseries.py` & `gwpy-3.0.5/gwpy/frequencyseries/tests/test_frequencyseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/frequencyseries/tests/test_hist.py` & `gwpy-3.0.5/gwpy/frequencyseries/tests/test_hist.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,17 @@
         utils.assert_array_equal(array.value, self.data)
         utils.assert_array_equal(array.bins.value, self.bins)
         assert array.x0 == 0 * units.Hertz
         assert array.df == 1 * units.Hertz
         assert array.y0 == self.bins[0]
         assert array.dy == self.bins[1] - self.bins[0]
 
+    def test_crop_float_precision(self):
+        pytest.skip("float precision test not supported for SpectralVariance")
+
     def test_is_compatible_yindex(self, array):
         return NotImplemented
 
     def test_is_compatible_error_yindex(self, array):
         return NotImplemented
 
     def test_plot(self, array):
```

### Comparing `gwpy-3.0.4/gwpy/io/__init__.py` & `gwpy-3.0.5/gwpy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/_framecpp.py` & `gwpy-3.0.5/gwpy/io/_framecpp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/cache.py` & `gwpy-3.0.5/gwpy/io/cache.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/datafind.py` & `gwpy-3.0.5/gwpy/io/datafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/ffldatafind.py` & `gwpy-3.0.5/gwpy/io/ffldatafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/gwf.py` & `gwpy-3.0.5/gwpy/io/gwf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/hdf5.py` & `gwpy-3.0.5/gwpy/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/kerberos.py` & `gwpy-3.0.5/gwpy/io/kerberos.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/ligolw.py` & `gwpy-3.0.5/gwpy/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/mp.py` & `gwpy-3.0.5/gwpy/io/mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/nds2.py` & `gwpy-3.0.5/gwpy/io/nds2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/registry.py` & `gwpy-3.0.5/gwpy/io/registry.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/tests/__init__.py` & `gwpy-3.0.5/gwpy/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/tests/test_cache.py` & `gwpy-3.0.5/gwpy/io/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/tests/test_datafind.py` & `gwpy-3.0.5/gwpy/io/tests/test_datafind.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """Decorate a function to use the GWOSC GWDataFind server.
 
     That server returns paths from CVMFS (``/cvmfs/gwosc.osgstorage.org``) so
     we need to add various protections.
     """
     @mock.patch.dict(  # point GWDataFind at GWOSC server
         "os.environ",
-        {"GWDATAFIND_SERVER": "datafind.gw-openscience.org:80"},
+        {"GWDATAFIND_SERVER": "datafind.gwosc.org:80"},
     )
     @pytest_skip_cvmfs_read_error  # skip CVMFS problems
     @pytest_skip_network_error  # skip network problems
     @pytest.mark.skipif(  # skip missing CVMFS repo
         not os.path.isdir('/cvmfs/gwosc.osgstorage.org/'),
         reason="GWOSC CVMFS repository not available",
     )
```

### Comparing `gwpy-3.0.4/gwpy/io/tests/test_ffldatafind.py` & `gwpy-3.0.5/gwpy/io/tests/test_ffldatafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/tests/test_gwf.py` & `gwpy-3.0.5/gwpy/io/tests/test_gwf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/tests/test_kerberos.py` & `gwpy-3.0.5/gwpy/io/tests/test_kerberos.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/tests/test_ligolw.py` & `gwpy-3.0.5/gwpy/io/tests/test_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/tests/test_mp.py` & `gwpy-3.0.5/gwpy/io/tests/test_mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/tests/test_nds2.py` & `gwpy-3.0.5/gwpy/io/tests/test_nds2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/tests/test_utils.py` & `gwpy-3.0.5/gwpy/io/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/io/utils.py` & `gwpy-3.0.5/gwpy/io/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/__init__.py` & `gwpy-3.0.5/gwpy/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/axes.py` & `gwpy-3.0.5/gwpy/plot/axes.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/bode.py` & `gwpy-3.0.5/gwpy/plot/bode.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/colorbar.py` & `gwpy-3.0.5/gwpy/plot/colorbar.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/colors.py` & `gwpy-3.0.5/gwpy/plot/colors.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/gps.py` & `gwpy-3.0.5/gwpy/plot/gps.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/legend.py` & `gwpy-3.0.5/gwpy/plot/legend.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/log.py` & `gwpy-3.0.5/gwpy/plot/log.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/plot.py` & `gwpy-3.0.5/gwpy/plot/plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/rc.py` & `gwpy-3.0.5/gwpy/plot/rc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/segments.py` & `gwpy-3.0.5/gwpy/plot/segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/__init__.py` & `gwpy-3.0.5/gwpy/plot/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_axes.py` & `gwpy-3.0.5/gwpy/plot/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_bode.py` & `gwpy-3.0.5/gwpy/plot/tests/test_bode.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_colors.py` & `gwpy-3.0.5/gwpy/plot/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_gps.py` & `gwpy-3.0.5/gwpy/plot/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_log.py` & `gwpy-3.0.5/gwpy/plot/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_plot.py` & `gwpy-3.0.5/gwpy/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_rc.py` & `gwpy-3.0.5/gwpy/plot/tests/test_rc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_segments.py` & `gwpy-3.0.5/gwpy/plot/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_tex.py` & `gwpy-3.0.5/gwpy/plot/tests/test_tex.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_text.py` & `gwpy-3.0.5/gwpy/plot/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/test_utils.py` & `gwpy-3.0.5/gwpy/plot/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tests/utils.py` & `gwpy-3.0.5/gwpy/plot/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/tex.py` & `gwpy-3.0.5/gwpy/plot/tex.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/text.py` & `gwpy-3.0.5/gwpy/plot/text.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/plot/units.py` & `gwpy-3.0.5/gwpy/plot/units.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,21 +20,35 @@
 """Support for plotting with units
 """
 
 from astropy.units.format import LatexInline
 
 
 class LatexInlineDimensional(LatexInline):
-    """Custom LaTeX formatter that includes physical type (if available)
+    r"""Custom LaTeX formatter that includes physical type (if available)
 
-    Mainly for auto-labelling `Axes` in matplotlib figures
+    Mainly for auto-labelling `Axes` in matplotlib figures.
+
+    Examples
+    --------
+    The built-in astropy ``latex_inline`` formatter gives this:
+
+    >>> Unit('m/s').to_string(format='latex_inline')
+    '$\mathrm{m\,s^{-1}}$'
+
+    This custom 'dimensional' formatter gives:
+
+    >>> Unit('m/s').to_string(format='latex_inline_dimensional')
+    'Speed [$\mathrm{m\,s^{-1}}$]'
     """
     name = 'latex_inline_dimensional'
 
     @classmethod
-    def to_string(cls, unit):
-        u = f"[{super().to_string(unit)}]"
+    def to_string(cls, unit, *args, **kwargs):
+        u = f"[{super().to_string(unit, *args, **kwargs)}]"
 
         if unit.physical_type not in {None, 'unknown', 'dimensionless'}:
-            ptype = str(unit.physical_type).split('/', 1)[0].title()
-            return f"{cls._latex_escape(ptype)} {u}"
+            # format physical type of unit for LaTeX
+            ptype = str(unit.physical_type).title().replace("_", r"\_")
+            # return '<Physical type> [<unit>]'
+            return f"{ptype} {u}"
         return u
```

### Comparing `gwpy-3.0.4/gwpy/plot/utils.py` & `gwpy-3.0.5/gwpy/plot/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/__init__.py` & `gwpy-3.0.5/gwpy/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/flag.py` & `gwpy-3.0.5/gwpy/segments/flag.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,15 +439,15 @@
         verbose : `bool`, optional
             show verbose download progress, default: `False`
 
         timeout : `int`, optional
             timeout for download (seconds)
 
         host : `str`, optional
-            URL of GWOSC host, default: ``'https://gw-openscience.org'``
+            URL of GWOSC host, default: ``'https://gwosc.org'``
 
         Returns
         -------
         flag : `DataQualityFlag`
             a new flag with `active` segments filled from Open Data
 
         Examples
```

### Comparing `gwpy-3.0.4/gwpy/segments/io/__init__.py` & `gwpy-3.0.5/gwpy/segments/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/io/hdf5.py` & `gwpy-3.0.5/gwpy/segments/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/io/json.py` & `gwpy-3.0.5/gwpy/segments/io/json.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/io/ligolw.py` & `gwpy-3.0.5/gwpy/segments/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/io/segwizard.py` & `gwpy-3.0.5/gwpy/segments/io/segwizard.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/segments.py` & `gwpy-3.0.5/gwpy/segments/segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/tests/__init__.py` & `gwpy-3.0.5/gwpy/segments/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/tests/test_flag.py` & `gwpy-3.0.5/gwpy/segments/tests/test_flag.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/segments/tests/test_segments.py` & `gwpy-3.0.5/gwpy/segments/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/__init__.py` & `gwpy-3.0.5/gwpy/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/fft.py` & `gwpy-3.0.5/gwpy/signal/fft.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/filter_design.py` & `gwpy-3.0.5/gwpy/signal/filter_design.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/qtransform.py` & `gwpy-3.0.5/gwpy/signal/qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/spectral/__init__.py` & `gwpy-3.0.5/gwpy/signal/spectral/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/spectral/_lal.py` & `gwpy-3.0.5/gwpy/signal/spectral/_lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/spectral/_median_mean.py` & `gwpy-3.0.5/gwpy/signal/spectral/_median_mean.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/spectral/_pycbc.py` & `gwpy-3.0.5/gwpy/signal/spectral/_pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/spectral/_registry.py` & `gwpy-3.0.5/gwpy/signal/spectral/_registry.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/spectral/_scipy.py` & `gwpy-3.0.5/gwpy/signal/spectral/_scipy.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # You should have received a copy of the GNU General Public License
 # along with GWpy.  If not, see <http://www.gnu.org/licenses/>.
 
 """GWpy API to the scipy.signal FFT routines
 """
 
 import numpy
+import warnings
 
 import scipy.signal
 
 from ...frequencyseries import FrequencySeries
 from ._utils import scale_timeseries_unit
 from . import _registry as fft_registry
 
@@ -167,15 +168,16 @@
     kwargs.setdefault('y', other.value)
     return _spectral_density(
         timeseries, segmentlength, noverlap=noverlap,
         name=str(timeseries.name)+'---'+str(other.name),
         sdfunc=scipy.signal.csd, **kwargs)
 
 
-def coherence(timeseries, other, segmentlength, noverlap=None, **kwargs):
+def coherence(timeseries, other, segmentlength, downsample=None,
+              noverlap=None, **kwargs):
     """Calculate the coherence between two `TimeSeries` using Welch's method
 
     Parameters
     ----------
     timeseries : `~gwpy.timeseries.TimeSeries`
         time-series of data
 
@@ -184,26 +186,57 @@
 
     segmentlength : `int`
         number of samples in single average.
 
     noverlap : `int`
         number of samples to overlap between segments, defaults to 50%.
 
+    downsample : `bool`
+        Downsample the series with higher sampling frequency? SciPy assumes
+        that both TimeSeries have the same rate.
+
     **kwargs
         other keyword arguments are passed to :meth:`scipy.signal.coherence`
 
     Returns
     -------
     spectrum : `~gwpy.frequencyseries.FrequencySeries`
         average power `FrequencySeries`
 
     See also
     --------
     scipy.signal.coherence
     """
+
+    # Should we warn about unequal sampling frequencies?
+    warn_fs = False
+
+    if downsample is None:
+        warn_fs = True
+        downsample = True
+
+    if timeseries.sample_rate != other.sample_rate:
+        # scipy assumes a single sampling frequency
+        if not downsample:
+            raise ValueError("Cannot calculate coherence when sampling "
+                             "frequencies are unequal")
+        if warn_fs:
+            warnings.warn("Sampling frequencies are unequal. Higher "
+                          "frequency series will be downsampled before "
+                          "coherence is calculated",
+                          category=UserWarning)
+        # downsample the one with the higher rate
+        if timeseries.sample_rate > other.sample_rate:
+            timeseries = timeseries.resample(other.sample_rate)
+        else:
+            other = other.resample(timeseries.sample_rate)
+
+    # should never be unequal from here on
+    assert timeseries.sample_rate == other.sample_rate
+
     # calculate CSD
     kwargs.setdefault('y', other.value)
     out = _spectral_density(
         timeseries,
         segmentlength,
         noverlap=noverlap,
         name="Coherence between {} and {}".format(timeseries.name, other.name),
```

### Comparing `gwpy-3.0.4/gwpy/signal/spectral/_ui.py` & `gwpy-3.0.5/gwpy/signal/spectral/_ui.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/spectral/_utils.py` & `gwpy-3.0.5/gwpy/signal/spectral/_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/__init__.py` & `gwpy-3.0.5/gwpy/signal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_filter_design.py` & `gwpy-3.0.5/gwpy/signal/tests/test_filter_design.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_qtransform.py` & `gwpy-3.0.5/gwpy/signal/tests/test_qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_spectral_lal.py` & `gwpy-3.0.5/gwpy/signal/tests/test_spectral_lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_spectral_median_mean.py` & `gwpy-3.0.5/gwpy/signal/tests/test_spectral_median_mean.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_spectral_pycbc.py` & `gwpy-3.0.5/gwpy/signal/tests/test_spectral_pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_spectral_registry.py` & `gwpy-3.0.5/gwpy/signal/tests/test_spectral_registry.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_spectral_scipy.py` & `gwpy-3.0.5/gwpy/signal/tests/test_spectral_scipy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_spectral_ui.py` & `gwpy-3.0.5/gwpy/signal/tests/test_spectral_ui.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_spectral_utils.py` & `gwpy-3.0.5/gwpy/signal/tests/test_spectral_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/tests/test_window.py` & `gwpy-3.0.5/gwpy/signal/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/signal/window.py` & `gwpy-3.0.5/gwpy/signal/window.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/spectrogram/__init__.py` & `gwpy-3.0.5/gwpy/spectrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/spectrogram/coherence.py` & `gwpy-3.0.5/gwpy/spectrogram/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/spectrogram/io/__init__.py` & `gwpy-3.0.5/gwpy/spectrogram/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/spectrogram/io/hdf5.py` & `gwpy-3.0.5/gwpy/spectrogram/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/spectrogram/spectrogram.py` & `gwpy-3.0.5/gwpy/spectrogram/spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/spectrogram/tests/__init__.py` & `gwpy-3.0.5/gwpy/spectrogram/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/spectrogram/tests/test_spectrogram.py` & `gwpy-3.0.5/gwpy/spectrogram/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/__init__.py` & `gwpy-3.0.5/gwpy/table/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/filter.py` & `gwpy-3.0.5/gwpy/table/filter.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/filters.py` & `gwpy-3.0.5/gwpy/table/filters.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/gravityspy.py` & `gwpy-3.0.5/gwpy/table/gravityspy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/__init__.py` & `gwpy-3.0.5/gwpy/table/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/cwb.py` & `gwpy-3.0.5/gwpy/table/io/cwb.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/fetch.py` & `gwpy-3.0.5/gwpy/table/io/fetch.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/gravityspy.py` & `gwpy-3.0.5/gwpy/table/io/gravityspy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/gstlal.py` & `gwpy-3.0.5/gwpy/table/io/gstlal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/gwf.py` & `gwpy-3.0.5/gwpy/table/io/gwf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/hacr.py` & `gwpy-3.0.5/gwpy/table/io/hacr.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/ligolw.py` & `gwpy-3.0.5/gwpy/table/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/losc.py` & `gwpy-3.0.5/gwpy/table/io/losc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/omega.py` & `gwpy-3.0.5/gwpy/table/io/omega.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/omicron.py` & `gwpy-3.0.5/gwpy/table/io/omicron.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/pycbc.py` & `gwpy-3.0.5/gwpy/table/io/pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/root.py` & `gwpy-3.0.5/gwpy/table/io/root.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/snax.py` & `gwpy-3.0.5/gwpy/table/io/snax.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/sql.py` & `gwpy-3.0.5/gwpy/table/io/sql.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/io/utils.py` & `gwpy-3.0.5/gwpy/table/io/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/table.py` & `gwpy-3.0.5/gwpy/table/table.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/tests/__init__.py` & `gwpy-3.0.5/gwpy/table/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/tests/test_gravityspy.py` & `gwpy-3.0.5/gwpy/table/tests/test_gravityspy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/tests/test_io_gstlal.py` & `gwpy-3.0.5/gwpy/table/tests/test_io_gstlal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/tests/test_io_ligolw.py` & `gwpy-3.0.5/gwpy/table/tests/test_io_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/tests/test_io_pycbc.py` & `gwpy-3.0.5/gwpy/table/tests/test_io_pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/table/tests/test_table.py` & `gwpy-3.0.5/gwpy/table/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/__init__.py` & `gwpy-3.0.5/gwpy/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.5/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/data/HLV-HW100916-968654552-1.gwf` & `gwpy-3.0.5/gwpy/testing/data/HLV-HW100916-968654552-1.gwf`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/data/HLV-HW100916-968654552-1.hdf` & `gwpy-3.0.5/gwpy/testing/data/HLV-HW100916-968654552-1.hdf`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz` & `gwpy-3.0.5/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/errors.py` & `gwpy-3.0.5/gwpy/testing/errors.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/fixtures.py` & `gwpy-3.0.5/gwpy/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/marks.py` & `gwpy-3.0.5/gwpy/testing/marks.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/mocks.py` & `gwpy-3.0.5/gwpy/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/testing/utils.py` & `gwpy-3.0.5/gwpy/testing/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/time/__init__.py` & `gwpy-3.0.5/gwpy/time/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/time/__main__.py` & `gwpy-3.0.5/gwpy/time/__main__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/time/_tconvert.py` & `gwpy-3.0.5/gwpy/time/_tconvert.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/time/tests/__init__.py` & `gwpy-3.0.5/gwpy/time/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/time/tests/test_main.py` & `gwpy-3.0.5/gwpy/time/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/time/tests/test_time.py` & `gwpy-3.0.5/gwpy/time/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/__init__.py` & `gwpy-3.0.5/gwpy/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/core.py` & `gwpy-3.0.5/gwpy/timeseries/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,17 @@
     return gps
 
 
 def _dynamic_scaled(scaled, channel):
     """Determine default for scaled based on channel name
 
     This is mainly to work around LIGO not correctly recording ADC
-    scaling parameters for most of Advanced LIGO (through 2019).
+    scaling parameters for most of Advanced LIGO (through 2023).
+    Scaling parameters for H0 and L0 data are also not correct
+    starting in mid-2020.
 
     Parameters
     ----------
     scaled : `bool`, `None`
         the scaled argument as given by the user
 
     channel : `str`
@@ -104,15 +106,15 @@
     >>> _dynamic_scaled(None, "H1:channel")
     False
     >>> _dynamic_scaled(None, "V1:channel")
     True
     """
     if scaled is not None:
         return scaled
-    return not str(channel).startswith(("H1", "L1"))
+    return not str(channel).startswith(("H0", "L0", "H1", "L1"))
 
 
 # -- TimeSeriesBase------------------------------------------------------------
 
 class TimeSeriesBase(Series):
     """An `Array` with time-domain metadata.
 
@@ -989,29 +991,33 @@
             if key in self:
                 self[key].prepend(series, **kwargs)
             else:
                 self[key] = series
         return self
 
     def crop(self, start=None, end=None, copy=False):
-        """Crop each entry of this `dict`
+        """Crop each entry of this `dict`.
 
         This method calls the :meth:`crop` method of all entries and
         modifies this dict in place.
 
         Parameters
         ----------
         start : `~gwpy.time.LIGOTimeGPS`, `float`, `str`
             GPS start time of required data,
             any input parseable by `~gwpy.time.to_gps` is fine
 
         end : `~gwpy.time.LIGOTimeGPS`, `float`, `str`, optional
             GPS end time of required data, defaults to end of data found;
             any input parseable by `~gwpy.time.to_gps` is fine
 
+        copy : `bool`, optional, default: `False`
+            If `True` copy the data for each entry to fresh memory,
+            otherwise return a view.
+
         See also
         --------
         TimeSeries.crop
             for more details
         """
         for key, val in self.items():
             self[key] = val.crop(start=start, end=end, copy=copy)
@@ -1437,17 +1443,26 @@
 
             If anything else, that fixed label will be used for all lines.
 
         **kwargs
             all other keyword arguments are passed to the plotter as
             appropriate
         """
+        kwargs.update({
+            "method": method,
+            "label": label,
+        })
+
         # make plot
         from ..plot import Plot
-        plot = Plot(self.values(), method=method, label=label, **kwargs)
+
+        if kwargs.get("separate", False):
+            plot = Plot(*self.values(), **kwargs)
+        else:
+            plot = Plot(self.values(), **kwargs)
 
         # update labels
         artmap = {'plot': 'lines', 'scatter': 'collections'}
         artists = [x for ax in plot.axes for
                    x in getattr(ax, artmap.get(method, 'lines'))]
         for key, artist in zip(self, artists):
             if label.lower() == 'name':
```

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/__init__.py` & `gwpy-3.0.5/gwpy/timeseries/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/ascii.py` & `gwpy-3.0.5/gwpy/timeseries/io/ascii.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/cache.py` & `gwpy-3.0.5/gwpy/timeseries/io/cache.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/core.py` & `gwpy-3.0.5/gwpy/timeseries/io/core.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/gwf/__init__.py` & `gwpy-3.0.5/gwpy/timeseries/io/gwf/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/gwf/framecpp.py` & `gwpy-3.0.5/gwpy/timeseries/io/gwf/framecpp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/gwf/framel.py` & `gwpy-3.0.5/gwpy/timeseries/io/gwf/framel.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/gwf/lalframe.py` & `gwpy-3.0.5/gwpy/timeseries/io/gwf/lalframe.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/hdf5.py` & `gwpy-3.0.5/gwpy/timeseries/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/losc.py` & `gwpy-3.0.5/gwpy/timeseries/io/losc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/nds2.py` & `gwpy-3.0.5/gwpy/timeseries/io/nds2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/io/wav.py` & `gwpy-3.0.5/gwpy/timeseries/io/wav.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/statevector.py` & `gwpy-3.0.5/gwpy/timeseries/statevector.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,16 +423,16 @@
         mask = ('\n%s' % indent).join(['%d: %s' % (idx, bit) for
                                        idx, bit in enumerate(self)
                                        if bit])
         return ("{1}({2},\n{0}channel={3},\n{0}epoch={4})".format(
             indent, self.__class__.__name__,
             mask, str(self.channel), str(self.epoch)))
 
-    def __array__(self):
-        return numpy.array([b or '' for b in self])
+    def __array__(self, dtype="U"):
+        return numpy.array([b or '' for b in self], dtype=dtype)
 
 
 # -- StateVector --------------------------------------------------------------
 
 class StateVector(TimeSeriesBase):
     """Binary array representing good/bad state determinations of some data.
```

### Comparing `gwpy-3.0.4/gwpy/timeseries/tests/__init__.py` & `gwpy-3.0.5/gwpy/timeseries/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/tests/test_core.py` & `gwpy-3.0.5/gwpy/timeseries/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,14 +416,30 @@
                 utils.assert_array_equal(line.get_xdata(),
                                          instance[key].xindex.value)
                 utils.assert_array_equal(line.get_ydata(),
                                          instance[key].value)
             plot.save(BytesIO(), format='png')
             plot.close()
 
+    def test_plot_separate(self, instance):
+        """Test plotting `TimeSeriesDict` on separate axes.
+
+        See https://github.com/gwpy/gwpy/issues/1609
+        """
+        with rc_context(rc={'text.usetex': False}):
+            plot = instance.plot(separate=True)
+            assert len(plot.axes) == len(instance.keys())
+            for ax, key in zip(plot.axes, instance):
+                utils.assert_array_equal(ax.lines[-1].get_xdata(),
+                                         instance[key].xindex.value)
+                utils.assert_array_equal(ax.lines[-1].get_ydata(),
+                                         instance[key].value)
+            plot.save(BytesIO(), format='png')
+            plot.close()
+
 
 # -- TimeSeriesBaseList -------------------------------------------------------
 
 class TestTimeSeriesBaseList(object):
     TEST_CLASS = TimeSeriesBaseList
     ENTRY_CLASS = TimeSeriesBase
     DTYPE = None
```

### Comparing `gwpy-3.0.4/gwpy/timeseries/tests/test_io_gwf_framecpp.py` & `gwpy-3.0.5/gwpy/timeseries/tests/test_io_gwf_framecpp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/tests/test_io_gwf_lalframe.py` & `gwpy-3.0.5/gwpy/timeseries/tests/test_io_gwf_lalframe.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/tests/test_io_losc.py` & `gwpy-3.0.5/gwpy/timeseries/tests/test_io_losc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/timeseries/tests/test_statevector.py` & `gwpy-3.0.5/gwpy/timeseries/tests/test_statevector.py`

 * *Files 3% similar despite different names*

```diff
@@ -366,14 +366,30 @@
             self.data.shape[0],
             '',
             name='test',
         )
         array = self.TEST_CLASS.from_nds2_buffer(nds_buffer)
         assert array.unit is units.dimensionless_unscaled
 
+    @pytest.mark.parametrize('ext', ('hdf5', 'h5'))
+    def test_read_write_hdf5(self, tmp_path, array, ext):
+        array.bits = ["a", "b", "c", "d"]
+        array.name = "test"
+
+        tmp = tmp_path / "test.{}".format(ext)
+
+        # write array (with auto-identify)
+        array.write(tmp, overwrite=True)
+
+        # check reading gives the same data (with/without auto-identify)
+        new = type(array).read(tmp, format='hdf5')
+        utils.assert_quantity_sub_equal(array, new)
+        new = type(array).read(tmp)
+        utils.assert_quantity_sub_equal(array, new)
+
 
 # -- StateVectorDict ----------------------------------------------------------
 
 class TestStateVectorDict(_TestTimeSeriesBaseDict):
     TEST_CLASS = StateVectorDict
     ENTRY_CLASS = StateVector
     DTYPE = 'uint32'
```

### Comparing `gwpy-3.0.4/gwpy/timeseries/tests/test_timeseries.py` & `gwpy-3.0.5/gwpy/timeseries/tests/test_timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         Segment(0, 32),
         Segment(34, 34.5),
     ]),
     known=SegmentList([Segment(0, 64)]),
     isgood=True,
 )
 
-GWOSC_DATAFIND_SERVER = "datafind.gw-openscience.org"
+GWOSC_DATAFIND_SERVER = "datafind.gwosc.org"
 GWOSC_GW150914_IFO = "L1"
 GWOSC_GW150914_CHANNEL = "L1:GWOSC-16KHZ_R1_STRAIN"
 NDS2_GW150914_CHANNEL = "L1:DCS-CALIB_STRAIN_C02"
 GWOSC_GW150914_FRAMETYPE = "L1_LOSC_16_V1"
 GWOSC_GW150914 = 1126259462
 GWOSC_GW150914_SEGMENT = Segment(GWOSC_GW150914-2, GWOSC_GW150914+2)
 GWOSC_GW150914_DQ_BITS = {
@@ -830,31 +830,40 @@
             "method": "median",
         }
         utils.assert_quantity_sub_equal(
             gw150914.asd(1, **kw),
             gw150914.psd(1, **kw) ** (1/2.),
         )
 
-    def test_csd(self, noisy_sinusoid, corrupt_noisy_sinusoid):
-        # test that csd(self) is the same as psd()
-        fs = noisy_sinusoid.csd(noisy_sinusoid)
+    def test_csd(self, noisy_sinusoid):
+        """Test that `TimeSeries.csd(self)` is the same as `psd()`.
+        """
+        fs = noisy_sinusoid.csd(noisy_sinusoid, average="mean")
         utils.assert_quantity_sub_equal(
-            fs,
+            fs.abs(),
             noisy_sinusoid.psd(method="welch"),
             exclude=['name'],
         )
 
-        # test fftlength
+    def test_csd_fftlength(self, noisy_sinusoid, corrupt_noisy_sinusoid):
+        """Test that `TimeSeries.csd` uses the ``fftlength`` keyword properly.
+        """
+        # test fftlength is used
         fs = noisy_sinusoid.csd(corrupt_noisy_sinusoid, fftlength=0.5)
         assert fs.size == 0.5 * noisy_sinusoid.sample_rate.value // 2 + 1
         assert fs.df == 2 * units.Hertz
+
+        # test that the default overlap works (by comparing to explicit)
         utils.assert_quantity_sub_equal(
             fs,
-            noisy_sinusoid.csd(corrupt_noisy_sinusoid, fftlength=0.5,
-                               overlap=0.25),
+            noisy_sinusoid.csd(
+                corrupt_noisy_sinusoid,
+                fftlength=0.5,
+                overlap=0.25,
+            ),
         )
 
     @staticmethod
     def _window_helper(series, fftlength, window='hamming'):
         nfft = int(series.sample_rate.value * fftlength)
         return signal.get_window(window, nfft)
```

### Comparing `gwpy-3.0.4/gwpy/timeseries/timeseries.py` & `gwpy-3.0.5/gwpy/timeseries/timeseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1103,15 +1103,15 @@
         # format as type(self)
         new = out.view(type(self))
         new.__metadata_finalize__(self)
         new._unit = self.unit
         return new
 
     def transfer_function(self, other, fftlength=None, overlap=None,
-                          window='hann', **kwargs):
+                          window='hann', average='mean', **kwargs):
         """Calculate the transfer function between this `TimeSeries` and
         another.
 
         This `TimeSeries` is the 'A-channel', serving as the reference
         (denominator) while the other time series is the test (numerator)
 
         Parameters
@@ -1128,14 +1128,18 @@
             recommended overlap for the given window (if given), or 0
 
         window : `str`, `numpy.ndarray`, optional
             window function to apply to timeseries prior to FFT,
             see :func:`scipy.signal.get_window` for details on acceptable
             formats
 
+        average : `str`, optional
+            FFT-averaging method (default: ``'mean'``) passed to
+            underlying csd() and psd() methods
+
         **kwargs
             any other keyword arguments accepted by
             :meth:`TimeSeries.csd` or :meth:`TimeSeries.psd`
 
         Returns
         -------
         transfer_function : `~gwpy.frequencyseries.FrequencySeries`
@@ -1145,17 +1149,17 @@
         Notes
         -----
         If `self` and `other` have difference
         :attr:`TimeSeries.sample_rate` values, the higher sampled
         `TimeSeries` will be down-sampled to match the lower.
         """
         csd = self.csd(other, fftlength=fftlength, overlap=overlap,
-                       window=window, **kwargs)
+                       window=window, average=average, **kwargs)
         psd = self.psd(fftlength=fftlength, overlap=overlap, window=window,
-                       **kwargs)
+                       average=average, **kwargs)
 
         # Take the minimum of the frequencyseries csd and psd because the
         # sample rate of different channels might yield different length
         # objects
         size = min(csd.size, psd.size)
 
         return csd[:size] / psd[:size]
```

### Comparing `gwpy-3.0.4/gwpy/types/__init__.py` & `gwpy-3.0.5/gwpy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/array.py` & `gwpy-3.0.5/gwpy/types/array.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/array2d.py` & `gwpy-3.0.5/gwpy/types/array2d.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/index.py` & `gwpy-3.0.5/gwpy/types/index.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/io/__init__.py` & `gwpy-3.0.5/gwpy/types/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/io/ascii.py` & `gwpy-3.0.5/gwpy/types/io/ascii.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/io/hdf5.py` & `gwpy-3.0.5/gwpy/types/io/hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,16 +121,18 @@
         except IgnoredAttribute:
             continue
 
         # store attribute
         try:
             dataset.attrs[attr] = value
         except (TypeError, ValueError, RuntimeError) as exc:
-            exc.args = ("Failed to store {} ({}) for {}: {}".format(
-                attr, type(value).__name__, type(array).__name__, str(exc)))
+            exc.args = (
+                f"Failed to store {attr} ({type(value).__name__}) "
+                f"for {type(array).__name__}: '{exc}'",
+            )
             raise
 
 
 @io_hdf5.with_write_hdf5
 def write_hdf5_array(array, h5g, path=None, attrs=None,
                      append=False, overwrite=False,
                      compression='gzip', **kwargs):
```

### Comparing `gwpy-3.0.4/gwpy/types/io/ligolw.py` & `gwpy-3.0.5/gwpy/types/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/series.py` & `gwpy-3.0.5/gwpy/types/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -943,95 +943,93 @@
 
     def crop(self, start=None, end=None, copy=False):
         """Crop this series to the given x-axis extent.
 
         Parameters
         ----------
         start : `float`, optional
-            lower limit of x-axis to crop to, defaults to
-            current `~Series.x0`
+            Lower limit of x-axis to crop to, defaults to
+            :attr:`~Series.x0`.
 
         end : `float`, optional
-            upper limit of x-axis to crop to, defaults to current series end
+            Upper limit of x-axis to crop to, defaults to series end.
 
-        copy : `bool`, optional, default: `False`
-            copy the input data to fresh memory, otherwise return a view
+        copy : `bool`, optional
+            Copy the input data to fresh memory,
+            otherwise return a view (default).
 
         Returns
         -------
         series : `Series`
-            A new series with a sub-set of the input data
+            A new series with a sub-set of the input data.
 
         Notes
         -----
         If either ``start`` or ``end`` are outside of the original
         `Series` span, warnings will be printed and the limits will
-        be restricted to the :attr:`~Series.xspan`
+        be restricted to the :attr:`~Series.xspan`.
         """
         x0, x1 = self.xspan
         xtype = type(x0)
         if isinstance(start, Quantity):
             start = start.to(self.xunit).value
         if isinstance(end, Quantity):
             end = end.to(self.xunit).value
 
         # pin early starts to time-series start
         if start == x0:
             start = None
         elif start is not None and xtype(start) < x0:
-            warn('%s.crop given start smaller than current start, '
-                 'crop will begin when the Series actually starts.'
-                 % type(self).__name__)
+            warn(
+                f"{type(self).__name__}.crop given start smaller than current "
+                "start, crop will begin when the Series actually starts.",
+            )
             start = None
 
         # pin late ends to time-series end
         if end == x1:
             end = None
         if end is not None and xtype(end) > x1:
-            warn('%s.crop given end larger than current end, '
-                 'crop will end when the Series actually ends.'
-                 % type(self).__name__)
+            warn(
+                f"{type(self).__name__}.crop given end larger than current "
+                "end, crop will begin when the Series actually ends.",
+            )
             end = None
 
         # check if series is irregular
         try:
             self.dx
         except AttributeError:
             irregular = True
         else:
             irregular = False
 
         # find start index
         if start is None:
             idx0 = None
+        elif irregular:
+            idx0 = numpy.searchsorted(
+                self.xindex.value,
+                xtype(start),
+                side="left",
+            )
         else:
-            if not irregular:
-                idx0 = int((xtype(start) - x0) // self.dx.value)
-            else:
-                idx0 = numpy.searchsorted(
-                    self.xindex.value, xtype(start), side="left"
-                )
+            idx0 = floor((xtype(start) - x0) / self.dx.value)
 
         # find end index
         if end is None:
             idx1 = None
+        elif irregular:
+            idx1 = numpy.searchsorted(
+                self.xindex.value,
+                xtype(end),
+                side="left",
+            )
         else:
-            if not irregular:
-                idx1 = int((xtype(end) - x0) // self.dx.value)
-                if idx1 >= self.size:
-                    idx1 = None
-            else:
-                if xtype(end) >= self.xindex.value[-1]:
-                    idx1 = None
-                else:
-                    idx1 = (
-                        numpy.searchsorted(
-                            self.xindex.value, xtype(end), side="left"
-                        )
-                    )
+            idx1 = floor((xtype(end) - x0) / self.dx.value)
 
         # crop
         if copy:
             return self[idx0:idx1].copy()
         return self[idx0:idx1]
 
     def pad(self, pad_width, **kwargs):
```

### Comparing `gwpy-3.0.4/gwpy/types/sliceutils.py` & `gwpy-3.0.5/gwpy/types/sliceutils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/tests/__init__.py` & `gwpy-3.0.5/gwpy/types/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/tests/test_array.py` & `gwpy-3.0.5/gwpy/types/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/tests/test_array2d.py` & `gwpy-3.0.5/gwpy/types/tests/test_array2d.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/tests/test_index.py` & `gwpy-3.0.5/gwpy/types/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/types/tests/test_series.py` & `gwpy-3.0.5/gwpy/types/tests/test_series.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,24 +181,33 @@
 
     def test_zip(self, array):
         z = array.zip()
         utils.assert_array_equal(
             z, numpy.column_stack((array.xindex.value, array.value)))
 
     def test_crop(self, array):
+        """Test basic functionality of `Series.crop`.
+        """
+        # all defaults
+        utils.assert_quantity_equal(array, array.crop())
+
+        # normal operation
         a2 = array.crop(10, 20)
         utils.assert_quantity_equal(array[10:20], a2)
-        # check that warnings are printed for out-of-bounds
+
+    def test_crop_warnings(self, array):
+        """Test that `Series.crop` emits warnings when it is supposed to.
+        """
         with pytest.warns(UserWarning):
             array.crop(array.xspan[0]-1, array.xspan[1])
         with pytest.warns(UserWarning):
             array.crop(array.xspan[0], array.xspan[1]+1)
 
     def test_crop_irregular(self):
-        """The cropping on an irregularly spaced series.
+        """Test `Series.crop` with an irregular index.
         """
         x = numpy.linspace(0, 100, num=self.data.shape[0])
 
         # add shift to second half of times to create irregular space
         x[x > 50] += 1
 
         series = self.create(xindex=x)
@@ -208,14 +217,27 @@
 
         cropped = series.crop(start=25)
         utils.assert_quantity_equal(series[x > 25], cropped)
 
         cropped = series.crop(start=25, end=75)
         utils.assert_quantity_equal(series[(x > 25) & (x < 75)], cropped)
 
+    def test_crop_float_precision(self):
+        """Verify the float precision of the crop function.
+
+        This tests regression against https://github.com/gwpy/gwpy/issues/1601.
+        """
+        # construct empty data array with the right shape for this array object
+        shape = (101,) * self.TEST_CLASS._ndim
+        series = self.TEST_CLASS(numpy.empty(shape), dx=0.01)
+
+        # assert that when we crop it, we only crop a single sample
+        cropped = series.crop(end=1.)
+        utils.assert_quantity_equal(series[:-1], cropped)
+
     def test_is_compatible(self, array):
         """Test the `Series.is_compatible` method
         """
         other = self.create(name='TEST CASE 2')
         assert array.is_compatible(other)
 
     def test_is_compatible_error_dx(self, array):
```

### Comparing `gwpy-3.0.4/gwpy/utils/__init__.py` & `gwpy-3.0.5/gwpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/decorators.py` & `gwpy-3.0.5/gwpy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/enum.py` & `gwpy-3.0.5/gwpy/utils/enum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/env.py` & `gwpy-3.0.5/gwpy/utils/env.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/lal.py` & `gwpy-3.0.5/gwpy/utils/lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/misc.py` & `gwpy-3.0.5/gwpy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/mp.py` & `gwpy-3.0.5/gwpy/utils/mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/progress.py` & `gwpy-3.0.5/gwpy/utils/progress.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/shell.py` & `gwpy-3.0.5/gwpy/utils/shell.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/sphinx/__init__.py` & `gwpy-3.0.5/gwpy/utils/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/sphinx/epydoc.py` & `gwpy-3.0.5/gwpy/utils/sphinx/epydoc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/sphinx/ex2rst.py` & `gwpy-3.0.5/gwpy/utils/sphinx/ex2rst.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/sphinx/zenodo.py` & `gwpy-3.0.5/gwpy/utils/sphinx/zenodo.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/tests/__init__.py` & `gwpy-3.0.5/gwpy/utils/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/tests/test_decorators.py` & `gwpy-3.0.5/gwpy/utils/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/tests/test_enum.py` & `gwpy-3.0.5/gwpy/utils/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/tests/test_env.py` & `gwpy-3.0.5/gwpy/utils/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/tests/test_lal.py` & `gwpy-3.0.5/gwpy/utils/tests/test_lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/tests/test_misc.py` & `gwpy-3.0.5/gwpy/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/tests/test_mp.py` & `gwpy-3.0.5/gwpy/utils/tests/test_mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/tests/test_shell.py` & `gwpy-3.0.5/gwpy/utils/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy/utils/tests/test_sphinx_ex2rst.py` & `gwpy-3.0.5/gwpy/utils/tests/test_sphinx_ex2rst.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.4/gwpy.egg-info/PKG-INFO` & `gwpy-3.0.5/gwpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpy
-Version: 3.0.4
+Version: 3.0.5
 Summary: A python package for gravitational-wave astrophysics
 Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwpy/gwpy/issues
 Project-URL: Discussion Forum, https://gwpy.slack.com
 Project-URL: Documentation, https://gwpy.github.io/docs/
 Project-URL: Source Code, https://github.com/gwpy/gwpy
```

### Comparing `gwpy-3.0.4/gwpy.egg-info/SOURCES.txt` & `gwpy-3.0.5/gwpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,15 @@
 gwpy/signal/spectral/_median_mean.py
 gwpy/signal/spectral/_pycbc.py
 gwpy/signal/spectral/_registry.py
 gwpy/signal/spectral/_scipy.py
 gwpy/signal/spectral/_ui.py
 gwpy/signal/spectral/_utils.py
 gwpy/signal/tests/__init__.py
+gwpy/signal/tests/test_coherence.py
 gwpy/signal/tests/test_filter_design.py
 gwpy/signal/tests/test_qtransform.py
 gwpy/signal/tests/test_spectral_lal.py
 gwpy/signal/tests/test_spectral_median_mean.py
 gwpy/signal/tests/test_spectral_pycbc.py
 gwpy/signal/tests/test_spectral_registry.py
 gwpy/signal/tests/test_spectral_scipy.py
```

### Comparing `gwpy-3.0.4/gwpy.egg-info/requires.txt` & `gwpy-3.0.5/gwpy.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 astropy>=4.3.0
 dqsegdb2
 gwdatafind>=1.1.0
 gwosc>=0.5.3
-h5py>=2.8.0
+h5py>=3.0.0
 ligo-segments>=1.0.0
 ligotimegps>=1.2.1
 matplotlib>=3.3.0
 numpy>=1.17
 python-dateutil
 requests
 scipy>=1.2.0
```

### Comparing `gwpy-3.0.4/pyproject.toml` & `gwpy-3.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # requirements
 requires-python = ">=3.7"
 dependencies = [
   "astropy >=4.3.0",
   "dqsegdb2",
   "gwdatafind >=1.1.0",
   "gwosc >=0.5.3",
-  "h5py >=2.8.0",
+  "h5py >=3.0.0",
   "ligo-segments >=1.0.0",
   "ligotimegps >=1.2.1",
   "matplotlib >=3.3.0",
   "numpy >=1.17",
   "python-dateutil",
   "requests",
   "scipy >=1.2.0",
```

### Comparing `gwpy-3.0.4/setup_utils.py` & `gwpy-3.0.5/setup_utils.py`

 * *Files identical despite different names*

