# Comparing `tmp/xsarslc-2023.6.1.tar.gz` & `tmp/xsarslc-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsarslc-2023.6.1.tar", last modified: Thu Jun  1 08:11:40 2023, max compression
+gzip compressed data, was "xsarslc-2023.6.2.tar", last modified: Fri Jun  2 08:40:32 2023, max compression
```

## Comparing `xsarslc-2023.6.1.tar` & `xsarslc-2023.6.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.587534 xsarslc-2023.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.587534 xsarslc-2023.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.591534 xsarslc-2023.6.1/auxdata/
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/auxdata/S1B_IRs_IW3_VV.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.587534 xsarslc-2023.6.1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.591534 xsarslc-2023.6.1/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.591534 xsarslc-2023.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/ATBD.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/ATBD_L1BSLC.tex
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.587534 xsarslc-2023.6.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.591534 xsarslc-2023.6.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/_static/css/xsarslc.css
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/crossspectra.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/cutoff.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.595534 xsarslc-2023.6.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/default_impulseResponse_files_IW.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/examples/xspec_WV_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.595534 xsarslc-2023.6.1/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/NIRAN_NRCS_VH.png
--rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/NIRAN_NRCS_vv.png
--rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/S1_azimuth_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/S1_azimuth_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/S1_range_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/S1_range_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/figures/index
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/normalizedvariance.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/docs/sigma0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.595534 xsarslc-2023.6.1/xsarslc/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/get_config_infos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/get_test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/xsarslc/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/HR_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/deramping.py
--rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/impulseResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/interburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    30553 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/intraburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    31595 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/processing/xspectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.599534 xsarslc-2023.6.1/xsarslc/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-06-01 08:11:25.000000 xsarslc-2023.6.1/xsarslc/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:40.595534 xsarslc-2023.6.1/xsarslc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 08:11:40.000000 xsarslc-2023.6.1/xsarslc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.449012 xsarslc-2023.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.449012 xsarslc-2023.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/auxdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW3_VV.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.445012 xsarslc-2023.6.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/ATBD.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/ATBD_L1BSLC.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.445012 xsarslc-2023.6.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/_static/css/xsarslc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/crossspectra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/cutoff.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/default_impulseResponse_files_IW.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/xspec_WV_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/NIRAN_NRCS_VH.png
+-rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/NIRAN_NRCS_vv.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/S1_azimuth_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/S1_azimuth_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/S1_range_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/S1_range_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/index
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/normalizedvariance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/sigma0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/xsarslc/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/get_config_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/get_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/xsarslc/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/HR_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/deramping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/impulseResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/interburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30553 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/intraburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31595 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/xspectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/xsarslc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/xsarslc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/top_level.txt
```

### Comparing `xsarslc-2023.6.1/.github/workflows/publish.yml` & `xsarslc-2023.6.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/.gitignore` & `xsarslc-2023.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/.pre-commit-config.yaml` & `xsarslc-2023.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/LICENSE` & `xsarslc-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/PKG-INFO` & `xsarslc-2023.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_HH.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_HV.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_VH.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW1_VV.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW2_VH.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW2_VV.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_HH.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_HV.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_VH.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1A_IRs_IW3_VV.nc` & `xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_HH.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_HV.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_VH.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW1_VV.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_HH.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_HV.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_VH.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW2_VV.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW3_VH.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/auxdata/S1B_IRs_IW3_VV.nc` & `xsarslc-2023.6.2/auxdata/S1B_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/ATBD.rst` & `xsarslc-2023.6.2/docs/ATBD.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/ATBD_L1BSLC.tex` & `xsarslc-2023.6.2/docs/ATBD_L1BSLC.tex`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/Makefile` & `xsarslc-2023.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/basic_api.rst` & `xsarslc-2023.6.2/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/conf.py` & `xsarslc-2023.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/crossspectra.rst` & `xsarslc-2023.6.2/docs/crossspectra.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/cutoff.rst` & `xsarslc-2023.6.2/docs/cutoff.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/examples/default_impulseResponse_files_IW.ipynb` & `xsarslc-2023.6.2/docs/examples/default_impulseResponse_files_IW.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.6.2/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.6.2/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/examples/xspec_IW_intra_and_inter_burst.ipynb` & `xsarslc-2023.6.2/docs/examples/xspec_IW_intra_and_inter_burst.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/examples/xspec_WV_example.ipynb` & `xsarslc-2023.6.2/docs/examples/xspec_WV_example.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/figures/NIRAN_NRCS_VH.png` & `xsarslc-2023.6.2/docs/figures/NIRAN_NRCS_VH.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/figures/NIRAN_NRCS_vv.png` & `xsarslc-2023.6.2/docs/figures/NIRAN_NRCS_vv.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/figures/S1_azimuth_IR_IW_VV.png` & `xsarslc-2023.6.2/docs/figures/S1_azimuth_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/figures/S1_azimuth_IR_WV_VV.png` & `xsarslc-2023.6.2/docs/figures/S1_azimuth_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/figures/S1_range_IR_IW_VV.png` & `xsarslc-2023.6.2/docs/figures/S1_range_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/figures/S1_range_IR_WV_VV.png` & `xsarslc-2023.6.2/docs/figures/S1_range_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/index.rst` & `xsarslc-2023.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/installing.rst` & `xsarslc-2023.6.2/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/normalizedvariance.rst` & `xsarslc-2023.6.2/docs/normalizedvariance.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/oceanspectrumSAR.png` & `xsarslc-2023.6.2/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/docs/sigma0.rst` & `xsarslc-2023.6.2/docs/sigma0.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/pyproject.toml` & `xsarslc-2023.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/burst.py` & `xsarslc-2023.6.2/xsarslc/burst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/config.yml` & `xsarslc-2023.6.2/xsarslc/config.yml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/get_config_infos.py` & `xsarslc-2023.6.2/xsarslc/get_config_infos.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/get_test_files.py` & `xsarslc-2023.6.2/xsarslc/get_test_files.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/interface.py` & `xsarslc-2023.6.2/xsarslc/interface.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/processing/HR_tiles.py` & `xsarslc-2023.6.2/xsarslc/processing/HR_tiles.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/processing/deramping.py` & `xsarslc-2023.6.2/xsarslc/processing/deramping.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/processing/impulseResponse.py` & `xsarslc-2023.6.2/xsarslc/processing/impulseResponse.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/processing/interburst.py` & `xsarslc-2023.6.2/xsarslc/processing/interburst.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,24 +207,27 @@
 
         mod0 = compute_modulation(np.abs(sub0['digital_number']), lowpass_width=lowpass_width,
                                   spacing={'sample': ground_spacing, 'line': azimuth_spacing})
         # ------------- nv ------------
         nv = compute_normalized_variance(mod0)
         # ------------- mean sigma0 and nesz ------------
         sigma0, nesz = compute_mean_sigma0_interp(sub0['digital_number'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+        sigma0_overlap, _ = compute_mean_sigma0_interp(sub1['digital_number'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+        sigma0_overlap = sigma0_overlap.rename(sigma0_overlap.name+'_overlap').drop('burst')
+        sigma0_overlap.attrs.update({'long_name':sigma0_overlap.attrs['long_name']+' (latest burst overlap)'})
         if not np.isfinite(sigma0): # should only append in IW mode. Case when line are badly indexed in noise-range LUT
             sigma0, nesz = compute_mean_sigma0_closest(sub0['digital_number'], burst['linesPerBurst'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
         # ------------- mean incidence ------------
         mean_incidence = xr.DataArray(mean_incidence, name='incidence', attrs={'long_name':'incidence at tile middle', 'units':'degree'})
         # ------------- heading ------------
         _,heading = haversine(float(corner_lons.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lons.sel(mytile)[{'c_line': 1, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 1, 'c_sample': 0}]))
         ground_heading = xr.DataArray(float(heading), name='ground_heading', attrs={'long_name':'ground heading', 'units':'degree', 'convention':'from North clockwise'})
 
         # ---------------- part of the variables to be added to the final dataset ----------------------
-        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), nesz.to_dataset(), ground_heading.to_dataset()]
+        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), sigma0_overlap.to_dataset(), nesz.to_dataset(), ground_heading.to_dataset()]
 
         if water_only:
 
             periodo_spacing = {'sample': ground_spacing, 'line': azimuth_spacing}
             nperseg_periodo = {d: int(np.rint(periodo_width[d] / periodo_spacing[d])) for d in tile_width.keys()}
             noverlap_periodo = {d: int(np.rint(periodo_overlap[d] / periodo_spacing[d])) for d in tile_width.keys()}
```

### Comparing `xsarslc-2023.6.1/xsarslc/processing/intraburst.py` & `xsarslc-2023.6.2/xsarslc/processing/intraburst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/processing/xspectra.py` & `xsarslc-2023.6.2/xsarslc/processing/xspectra.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py` & `xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py` & `xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py` & `xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc/tools.py` & `xsarslc-2023.6.2/xsarslc/tools.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.1/xsarslc.egg-info/PKG-INFO` & `xsarslc-2023.6.2/xsarslc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `xsarslc-2023.6.1/xsarslc.egg-info/SOURCES.txt` & `xsarslc-2023.6.2/xsarslc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

