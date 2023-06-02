# Comparing `tmp/pytaser-0.1.0.tar.gz` & `tmp/pytaser-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytaser-0.1.0.tar", last modified: Sat Mar  5 01:08:18 2022, max compression
+gzip compressed data, was "pytaser-1.0.0.tar", last modified: Fri Jun  2 14:37:03 2023, max compression
```

## Comparing `pytaser-0.1.0.tar` & `pytaser-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,132 @@
-drwxr-xr-x   0 savyaaggarwal   (501) staff       (20)        0 2022-03-05 01:08:18.525117 pytaser-0.1.0/
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)     1077 2022-01-24 02:45:49.000000 pytaser-0.1.0/LICENSE
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)     3896 2022-03-05 01:08:18.524947 pytaser-0.1.0/PKG-INFO
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)     2965 2022-03-04 01:47:35.000000 pytaser-0.1.0/README.md
-drwxr-xr-x   0 savyaaggarwal   (501) staff       (20)        0 2022-03-05 01:08:18.524025 pytaser-0.1.0/pytaser/
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)        0 2022-01-24 01:39:46.000000 pytaser-0.1.0/pytaser/__init__.py
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)    13296 2022-03-03 15:00:33.000000 pytaser-0.1.0/pytaser/generator.py
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)     5695 2022-01-29 12:41:58.000000 pytaser-0.1.0/pytaser/kpoints.py
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)     8472 2022-03-04 01:02:54.000000 pytaser-0.1.0/pytaser/plotter.py
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)     1415 2022-01-28 17:00:25.000000 pytaser-0.1.0/pytaser/tas.py
-drwxr-xr-x   0 savyaaggarwal   (501) staff       (20)        0 2022-03-05 01:08:18.524764 pytaser-0.1.0/pytaser.egg-info/
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)     3896 2022-03-05 01:08:18.000000 pytaser-0.1.0/pytaser.egg-info/PKG-INFO
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)      274 2022-03-05 01:08:18.000000 pytaser-0.1.0/pytaser.egg-info/SOURCES.txt
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)        1 2022-03-05 01:08:18.000000 pytaser-0.1.0/pytaser.egg-info/dependency_links.txt
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)       44 2022-03-05 01:08:18.000000 pytaser-0.1.0/pytaser.egg-info/requires.txt
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)        8 2022-03-05 01:08:18.000000 pytaser-0.1.0/pytaser.egg-info/top_level.txt
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)       38 2022-03-05 01:08:18.525167 pytaser-0.1.0/setup.cfg
--rw-r--r--   0 savyaaggarwal   (501) staff       (20)     1369 2022-01-29 12:41:58.000000 pytaser-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.032993 pytaser-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.968988 pytaser-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.972989 pytaser-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-02 14:32:02.000000 pytaser-1.0.0/.github/workflows/build_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-02 14:32:02.000000 pytaser-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-02 14:32:02.000000 pytaser-1.0.0/.github/workflows/pip_install_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-02 14:32:02.000000 pytaser-1.0.0/.github/workflows/releasing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-02 14:32:02.000000 pytaser-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-02 14:32:02.000000 pytaser-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-02 14:32:02.000000 pytaser-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-02 14:32:02.000000 pytaser-1.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-02 14:32:02.000000 pytaser-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-02 14:37:03.032993 pytaser-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35468 2023-06-02 14:32:02.000000 pytaser-1.0.0/PyTASER.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-02 14:32:02.000000 pytaser-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.972989 pytaser-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.976989 pytaser-1.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.976989 pytaser-1.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   213708 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/_static/PyTASER.png
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/_static/orcid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/changelog_link.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/dft_examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/jdos_examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-02 14:32:02.000000 pytaser-1.0.0/docs/source/pytaser.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.976989 pytaser-1.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.968988 pytaser-1.0.0/examples/CdTe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.980989 pytaser-1.0.0/examples/CdTe/k666_Optics/
+-rw-r--r--   0 runner    (1001) docker     (123)   497792 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/CdTe/k666_Optics/WAVEDER
+-rw-r--r--   0 runner    (1001) docker     (123)  1912548 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/CdTe/k666_Optics/vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  1742322 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/PyTASER_DFT_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1071895 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/PyTASER_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.980989 pytaser-1.0.0/examples/TiO2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.980989 pytaser-1.0.0/examples/TiO2/band/
+-rw-r--r--   0 runner    (1001) docker     (123)    55292 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/band/band.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.980989 pytaser-1.0.0/examples/TiO2/band/split-01/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/band/split-01/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (123)   541483 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/band/split-01/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.984990 pytaser-1.0.0/examples/TiO2/band/split-02/
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/band/split-02/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (123)   541483 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/band/split-02/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.984990 pytaser-1.0.0/examples/TiO2/band/split-03/
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/band/split-03/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (123)   541483 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/band/split-03/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.984990 pytaser-1.0.0/examples/TiO2/band/split-04/
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/band/split-04/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (123)   491167 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/band/split-04/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.972989 pytaser-1.0.0/examples/TiO2/dostest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.984990 pytaser-1.0.0/examples/TiO2/dostest/101015/
+-rw-r--r--   0 runner    (1001) docker     (123)  5350889 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/dostest/101015/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:02.992990 pytaser-1.0.0/examples/TiO2/dostest/121218/
+-rw-r--r--   0 runner    (1001) docker     (123)  7825310 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/dostest/121218/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.000991 pytaser-1.0.0/examples/TiO2/dostest/669/
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/dostest/669/dos.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)  2740916 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/dostest/669/vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   148387 2023-06-02 14:32:02.000000 pytaser-1.0.0/examples/TiO2/vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-02 14:32:02.000000 pytaser-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.004991 pytaser-1.0.0/pytaser/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-02 14:32:02.000000 pytaser-1.0.0/pytaser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26460 2023-06-02 14:32:02.000000 pytaser-1.0.0/pytaser/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-02 14:32:02.000000 pytaser-1.0.0/pytaser/kpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30107 2023-06-02 14:32:02.000000 pytaser-1.0.0/pytaser/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-02 14:32:02.000000 pytaser-1.0.0/pytaser/tas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.004991 pytaser-1.0.0/pytaser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-02 14:37:02.000000 pytaser-1.0.0/pytaser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-02 14:37:02.000000 pytaser-1.0.0/pytaser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:37:02.000000 pytaser-1.0.0/pytaser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-02 14:37:02.000000 pytaser-1.0.0/pytaser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 14:37:02.000000 pytaser-1.0.0/pytaser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 14:32:02.000000 pytaser-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:37:03.032993 pytaser-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-02 14:32:02.000000 pytaser-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.004991 pytaser-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.004991 pytaser-1.0.0/tests/data_cdte/
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/cdte_444_bs.json
+-rw-r--r--   0 runner    (1001) docker     (123)   436124 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/cdte_444_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/cdte_444_kweights.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100019 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/cdte_k666_sumo_absorption.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.008991 pytaser-1.0.0/tests/data_cdte/error_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)   373376 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/error_testing/CdTe_LVEL_False_WAVEDER
+-rw-r--r--   0 runner    (1001) docker     (123)  1814177 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/error_testing/CdTe_LVEL_False_vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    83072 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/error_testing/CdTe_symmetry_on_WAVEDER
+-rw-r--r--   0 runner    (1001) docker     (123)  1610189 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/error_testing/CdTe_symmetry_on_vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.016992 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)   163896 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/alpha_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   185164 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/jdos_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146975 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/jdos_diff_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   185103 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/jdos_ev_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)    82714 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/jdos_ev_gaas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   310184 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/jdos_lambda_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83992 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/jdos_lambda_gaas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   122510 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/tas_absorption_only_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130977 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/tas_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118022 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/tas_cdte_custom_legend.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146982 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/tas_ev_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80671 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/tas_ev_gaas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   210858 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/tas_lambda_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)    89661 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_cdte/remote_baseline_plots/tas_lambda_gaas.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.028993 pytaser-1.0.0/tests/data_gaas/
+-rw-r--r--   0 runner    (1001) docker     (123)  5766722 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/gaas_2534_bs.json
+-rw-r--r--   0 runner    (1001) docker     (123)   499747 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/gaas_2534_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25346 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/gaas_kweights.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/gaussian_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5921615 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/new_gaas_2534_bs.json
+-rw-r--r--   0 runner    (1001) docker     (123)   499729 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/new_gaas_2534_dos.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:37:03.032993 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)   163896 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/alpha_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   185164 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/jdos_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146975 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/jdos_diff_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   185103 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/jdos_ev_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)    82714 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/jdos_ev_gaas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   310184 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/jdos_lambda_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83992 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/jdos_lambda_gaas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   122510 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/tas_absorption_only_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130977 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/tas_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118022 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/tas_cdte_custom_legend.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146982 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/tas_ev_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80671 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/tas_ev_gaas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   210858 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/tas_lambda_cdte.png
+-rw-r--r--   0 runner    (1001) docker     (123)    89661 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/data_gaas/remote_baseline_plots/tas_lambda_gaas.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-06-02 14:32:02.000000 pytaser-1.0.0/tests/test_plotter.py
```

### Comparing `pytaser-0.1.0/LICENSE` & `pytaser-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytaser-0.1.0/PKG-INFO` & `pytaser-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pytaser
-Version: 0.1.0
-Summary: Post-DFT TAS spectrum classification tool
-Home-page: https://github.com/WMD-group/PyTASER
+Version: 1.0.0
+Summary: TAS prediction tool
+Home-page: https://pytaser.readthedocs.io/en/latest/
 Author: Savyasanchi Aggarwal
-Author-email: sa13018@ic.ac.uk
+Author-email: savya10@gmail.com
 License: MIT
 Keywords: dft tas semiconductor-physics solar-fuel materials-project metal-oxides
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
@@ -16,66 +16,104 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: docs
 License-File: LICENSE
 
+[![Documentation Status](https://readthedocs.org/projects/pytaser/badge/?version=latest)](https://pytaser.readthedocs.io/en/latest/?badge=latest)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://github.com/WMD-Group/PyTASER/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/WMD-Group/PyTASER/actions)
+[![pypi](https://img.shields.io/pypi/v/pytaser)](https://pypi.org/project/pytaser)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://img.shields.io/badge/code%20style-black-000000.svg)
+
 # PyTASER
 
-PyTASER is a Python (3.9+) library and set of command-line tools for classifying spectral features in bulk materials, post-DFT. The goal of this library is to provide simulated TAS spectra, for qualitative comparison with experimental spectra. This will simplify the complex and tedious processes of TAS prep and analysis, especially for pristine materials. The main features include:
+![](PyTASER.png)
+
+***The library is undergoing changes before it is released*** 
+
+[Official Documentation](https://pytaser.readthedocs.io/en/latest/)
 
-* An interactive TAS spectrum for a pristine semiconducting material
-* Isolated spectra for individual band transitions from the overall TAS spectrum for the material.
-* Spectra in different conditions: temperature, carrier concentrations (analogous to pump-probe time delay) 
-* Partial occupancies of valence and conduction bands, using the Fermi-Dirac distribution for different Quasi-Fermi levels. 
-* Consideration of both non-magnetic and magnetic materials. 
-* Capability to input DFT-calculated bandstructure and dos inputs, with primary support for the [Materials Project](https://materialsproject.org/).
+PyTASER is a Python (3.9+) library built for simulating transient absorption spectroscopy (TAS) features from 
+DFT calculations. The goal of this library is to simulate TAS spectra for comparison with and interpretation of 
+experimental spectra. The main features include:
+
+* A TAS spectrum for a pristine semiconducting crystal
+* Components from individual band-to-band transitions
+* Spectra for different conditions: temperature and carrier concentrations
+* Consideration of non-magnetic and magnetic materials
+* Capability to input calculated bandstructure and density of states inputs with support for the [Materials Project](https://materialsproject.org)
 
 # Installation
 
-The recommended way to install PyTASER is in a conda environment. 
+To install the module with pip (recommended): 
 
 ```
-Installation method to be updated here
+pip install --user pytaser
+```
+To install directly from the git repository:
+```
+pip install --user git+https://github.com/WMD-group/PyTASER
 ```
+To do a manual build and installation:
+```
+python3 setup.py build
+python3 setup.py install --user
+```
+
 PyTASER is currently compatible with Python 3.9+ and relies on a number of open-source python packages, specifically:
 
 * [pymatgen](https://pymatgen.org/index.html) 
 * [numpy](https://numpy.org/), [scipy](https://scipy.org/) for data structures and unit conversion
 * [matplotlib](https://matplotlib.org/) for plotting the spectra
 
-# Visualisation 
+# Developer’s installation (optional)
+
+For development work, PyTASER can also be installed from a copy of the source directory:
 
-Once the library is installed, please setup a file as done in the examples provided. Then just run it as a python file:
+Download PyTASER source code using the command:
 ```
-python3 filename.py
+git clone https://github.com/WMD-group/PyTASER
 ```
+Navigate to root directory:
+```
+cd PyTASER
+```
+Install the code with the command:
+```
+pip install -e .
+```
+This command tries to obtain the required packages and their dependencies and install them automatically.
 
-# Contributing
-
-***The library is currently undergoing some final changes before it is finalised.*** However, once it is completed, we would greatly appreciate any contributions in the form of a pull request. 
-Additionally, any test cases/example spectra performed with PyTASER would be welcomed. Please feel free to reach out to us if there are any questions or suggestions. 
+# Visualisation 
 
-Future topics we'd like to build on:
+The preferred method is to generate a Jupyter Notebook, as shown in the [examples](https://github.com/WMD-group/PyTASER/blob/main/examples) folder.
+Alternatively, you can set up a file in Python to run it in the command line of the terminal:
+```
+python3 <filename.py>
+```
 
-* Direct conversion between carrier concentrations and pump-probe time delay (for more quantitative simulated-experimental comparisons)
-* Incorporating spin-change processes (e.g. moving from Spin.up to Spin.down and vice-versa) for spin-polarised systems
-* Incorporating finite-temperature effects (particularly indirect bandgaps & phonons, and defects)
-* Incorporating more complex optical processes (e.g. Stimulated Emission)
-* Cleaning regions further away from the bandgap
-* Implementing optical transition probabilities alongside the JDOS
-* Creating a similarly-obtained kinetics plot for TAS analysis.
-* Relating spectral features with associated optical processes
+# Contributing
 
+We appreciate any contributions in the form of a pull request. 
+Additional test cases/example spectra performed with PyTASER would be welcomed. 
+Please feel free to reach out to us if there are any questions or suggestions. 
+
+Future topics we plan to build on:
+
+* Incorporating finite-temperature effects (particularly for indirect bandgaps)
+* Description of more complex optical processes (e.g. stimulated emission)
+* Direct treatment of pump-probe time delay
+* Incorporating spin-flip processes for spin-polarised systems
+* Description of defective crystals 
 
 # Acknowledgements
 
-Developed by Savyasanchi Aggarwal, Alex Ganose and Liam Harnett-Caulfield. Aron Walsh designed and led the project. 
-
-Thanks to the WMD group @ Imperial/Yonsei for all the interesting discussions and improvements!
-
-
+The project was the focus of a [UROP](https://www.imperial.ac.uk/urop/) by @savya10, supervised by @utf and @aronwalsh, with on-going developments and testing from @kavanase and @youngwonwoo.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytaser-0.1.0/pytaser/kpoints.py` & `pytaser-1.0.0/pytaser/kpoints.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import numpy as np
 from pymatgen.core import Structure
+from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
 
 
 def get_kpoint_weights(bandstructure, time_reversal=True, symprec=0.1):
     """
     Function to calculate the kpoint_weights for non-magnetic materials (non-metals).
 
     Args:
         bandstructure: PMG bandstructure object
         time_reversal:
         symprec: Symmetry precision in Angstrom.(Lower value is more precise, but
             computationally more expensive)
     Returns:
         k-point_weights
     """
+    if isinstance(bandstructure, BandStructureSymmLine):
+        raise TypeError(
+            "This bandstructure object uses a line-mode kpoint mesh instead of a uniform mesh. Kpoint "
+            "weighting is not possible"
+        )
 
     kpoints = get_kpoints_from_bandstructure(bandstructure)
     _, _, _, _, _, kp_mapping = expand_kpoints(
         bandstructure.structure,
         kpoints,
         symprec=symprec,
         time_reversal=time_reversal,
@@ -147,15 +153,17 @@
     time_reversal: bool = True,
 ):
     from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
     sga = SpacegroupAnalyzer(structure, symprec=symprec)
     if sga.get_symmetry_dataset() is None:
         # sometimes default angle tolerance doesn't work as expected
-        sga = SpacegroupAnalyzer(structure, symprec=symprec, angle_tolerance=-1)
+        sga = SpacegroupAnalyzer(
+            structure, symprec=symprec, angle_tolerance=-1
+        )
 
     rotations = sga.get_symmetry_dataset()["rotations"].transpose((0, 2, 1))
     translations = sga.get_symmetry_dataset()["translations"]
     is_tr = np.full(len(rotations), False, dtype=bool)
 
     if time_reversal:
         rotations = np.concatenate([rotations, -rotations])
@@ -163,10 +171,12 @@
         is_tr = np.concatenate([is_tr, ~is_tr])
 
         rotations, unique_ops = np.unique(rotations, axis=0, return_index=True)
         translations = translations[unique_ops]
         is_tr = is_tr[unique_ops]
 
     # put identity first and time-reversal last
-    sort_idx = np.argsort(np.abs(rotations - np.eye(3)).sum(axis=(1, 2)) + is_tr * 10)
+    sort_idx = np.argsort(
+        np.abs(rotations - np.eye(3)).sum(axis=(1, 2)) + is_tr * 10
+    )
 
     return rotations[sort_idx], translations[sort_idx], is_tr[sort_idx]
```

### Comparing `pytaser-0.1.0/pytaser.egg-info/PKG-INFO` & `pytaser-1.0.0/pytaser.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pytaser
-Version: 0.1.0
-Summary: Post-DFT TAS spectrum classification tool
-Home-page: https://github.com/WMD-group/PyTASER
+Version: 1.0.0
+Summary: TAS prediction tool
+Home-page: https://pytaser.readthedocs.io/en/latest/
 Author: Savyasanchi Aggarwal
-Author-email: sa13018@ic.ac.uk
+Author-email: savya10@gmail.com
 License: MIT
 Keywords: dft tas semiconductor-physics solar-fuel materials-project metal-oxides
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
@@ -16,66 +16,104 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: docs
 License-File: LICENSE
 
+[![Documentation Status](https://readthedocs.org/projects/pytaser/badge/?version=latest)](https://pytaser.readthedocs.io/en/latest/?badge=latest)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://github.com/WMD-Group/PyTASER/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/WMD-Group/PyTASER/actions)
+[![pypi](https://img.shields.io/pypi/v/pytaser)](https://pypi.org/project/pytaser)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://img.shields.io/badge/code%20style-black-000000.svg)
+
 # PyTASER
 
-PyTASER is a Python (3.9+) library and set of command-line tools for classifying spectral features in bulk materials, post-DFT. The goal of this library is to provide simulated TAS spectra, for qualitative comparison with experimental spectra. This will simplify the complex and tedious processes of TAS prep and analysis, especially for pristine materials. The main features include:
+![](PyTASER.png)
+
+***The library is undergoing changes before it is released*** 
+
+[Official Documentation](https://pytaser.readthedocs.io/en/latest/)
 
-* An interactive TAS spectrum for a pristine semiconducting material
-* Isolated spectra for individual band transitions from the overall TAS spectrum for the material.
-* Spectra in different conditions: temperature, carrier concentrations (analogous to pump-probe time delay) 
-* Partial occupancies of valence and conduction bands, using the Fermi-Dirac distribution for different Quasi-Fermi levels. 
-* Consideration of both non-magnetic and magnetic materials. 
-* Capability to input DFT-calculated bandstructure and dos inputs, with primary support for the [Materials Project](https://materialsproject.org/).
+PyTASER is a Python (3.9+) library built for simulating transient absorption spectroscopy (TAS) features from 
+DFT calculations. The goal of this library is to simulate TAS spectra for comparison with and interpretation of 
+experimental spectra. The main features include:
+
+* A TAS spectrum for a pristine semiconducting crystal
+* Components from individual band-to-band transitions
+* Spectra for different conditions: temperature and carrier concentrations
+* Consideration of non-magnetic and magnetic materials
+* Capability to input calculated bandstructure and density of states inputs with support for the [Materials Project](https://materialsproject.org)
 
 # Installation
 
-The recommended way to install PyTASER is in a conda environment. 
+To install the module with pip (recommended): 
 
 ```
-Installation method to be updated here
+pip install --user pytaser
+```
+To install directly from the git repository:
+```
+pip install --user git+https://github.com/WMD-group/PyTASER
 ```
+To do a manual build and installation:
+```
+python3 setup.py build
+python3 setup.py install --user
+```
+
 PyTASER is currently compatible with Python 3.9+ and relies on a number of open-source python packages, specifically:
 
 * [pymatgen](https://pymatgen.org/index.html) 
 * [numpy](https://numpy.org/), [scipy](https://scipy.org/) for data structures and unit conversion
 * [matplotlib](https://matplotlib.org/) for plotting the spectra
 
-# Visualisation 
+# Developer’s installation (optional)
+
+For development work, PyTASER can also be installed from a copy of the source directory:
 
-Once the library is installed, please setup a file as done in the examples provided. Then just run it as a python file:
+Download PyTASER source code using the command:
 ```
-python3 filename.py
+git clone https://github.com/WMD-group/PyTASER
 ```
+Navigate to root directory:
+```
+cd PyTASER
+```
+Install the code with the command:
+```
+pip install -e .
+```
+This command tries to obtain the required packages and their dependencies and install them automatically.
 
-# Contributing
-
-***The library is currently undergoing some final changes before it is finalised.*** However, once it is completed, we would greatly appreciate any contributions in the form of a pull request. 
-Additionally, any test cases/example spectra performed with PyTASER would be welcomed. Please feel free to reach out to us if there are any questions or suggestions. 
+# Visualisation 
 
-Future topics we'd like to build on:
+The preferred method is to generate a Jupyter Notebook, as shown in the [examples](https://github.com/WMD-group/PyTASER/blob/main/examples) folder.
+Alternatively, you can set up a file in Python to run it in the command line of the terminal:
+```
+python3 <filename.py>
+```
 
-* Direct conversion between carrier concentrations and pump-probe time delay (for more quantitative simulated-experimental comparisons)
-* Incorporating spin-change processes (e.g. moving from Spin.up to Spin.down and vice-versa) for spin-polarised systems
-* Incorporating finite-temperature effects (particularly indirect bandgaps & phonons, and defects)
-* Incorporating more complex optical processes (e.g. Stimulated Emission)
-* Cleaning regions further away from the bandgap
-* Implementing optical transition probabilities alongside the JDOS
-* Creating a similarly-obtained kinetics plot for TAS analysis.
-* Relating spectral features with associated optical processes
+# Contributing
 
+We appreciate any contributions in the form of a pull request. 
+Additional test cases/example spectra performed with PyTASER would be welcomed. 
+Please feel free to reach out to us if there are any questions or suggestions. 
+
+Future topics we plan to build on:
+
+* Incorporating finite-temperature effects (particularly for indirect bandgaps)
+* Description of more complex optical processes (e.g. stimulated emission)
+* Direct treatment of pump-probe time delay
+* Incorporating spin-flip processes for spin-polarised systems
+* Description of defective crystals 
 
 # Acknowledgements
 
-Developed by Savyasanchi Aggarwal, Alex Ganose and Liam Harnett-Caulfield. Aron Walsh designed and led the project. 
-
-Thanks to the WMD group @ Imperial/Yonsei for all the interesting discussions and improvements!
-
-
+The project was the focus of a [UROP](https://www.imperial.ac.uk/urop/) by @savya10, supervised by @utf and @aronwalsh, with on-going developments and testing from @kavanase and @youngwonwoo.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

