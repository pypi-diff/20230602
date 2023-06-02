# Comparing `tmp/pyerrors-2.8.1.tar.gz` & `tmp/pyerrors-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerrors-2.8.1.tar", last modified: Thu Jun  1 12:41:28 2023, max compression
+gzip compressed data, was "pyerrors-2.8.2.tar", last modified: Fri Jun  2 14:10:51 2023, max compression
```

## Comparing `pyerrors-2.8.1.tar` & `pyerrors-2.8.2.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.620364 pyerrors-2.8.1/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/.github/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      113 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/CODEOWNERS
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1051 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/ISSUE_TEMPLATE/bug-report.yml
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/.github/workflows/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      386 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/binder.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      737 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/codeql.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1012 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/docs.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1022 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/examples.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      547 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/flake8.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1043 2023-06-01 12:28:18.000000 pyerrors-2.8.1/.github/workflows/pytest.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      211 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.gitignore
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16778 2023-06-01 12:32:58.000000 pyerrors-2.8.1/CHANGELOG.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1278 2023-05-21 16:06:57.000000 pyerrors-2.8.1/CITATION.cff
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1842 2023-03-21 12:48:56.000000 pyerrors-2.8.1/CONTRIBUTING.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1070 2023-03-11 21:38:08.000000 pyerrors-2.8.1/LICENSE
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-06-01 12:41:28.620364 pyerrors-2.8.1/PKG-INFO
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1610 2023-06-01 12:28:18.000000 pyerrors-2.8.1/README.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        0 2023-03-11 21:38:08.000000 pyerrors-2.8.1/conftest.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.608364 pyerrors-2.8.1/examples/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87858 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/01_basic_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    62623 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/02_correlators.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    97653 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/03_pcac_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   129847 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/04_fit_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9053 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/05_matrix_operations.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30851 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/06_gevp.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10604 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/07_data_management.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    21826 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/08_combined_fit_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      757 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/base_style.mplstyle
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.612364 pyerrors-2.8.1/examples/data/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7407 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/correlator_test.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15009 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/f_A.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15072 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/f_P.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266539 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/matrix_correlator.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266778 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/matrix_correlator_V1V1.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266803 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/matrix_correlator_V2V2.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266702 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/matrix_correlator_V3V3.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8575 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/json_schema.json
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.612364 pyerrors-2.8.1/pyerrors/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    29950 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/__init__.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    57481 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/correlators.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3609 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/covobs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2909 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/dirac.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30996 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/fits.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/pyerrors/input/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      579 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/__init__.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    25145 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/input/bdio.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30920 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/input/dobs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    19262 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/hadrons.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    26602 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/json.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8064 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/misc.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    50595 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/input/openQCD.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6691 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/input/pandas.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16290 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/input/sfcf.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2257 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/utils.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10177 2023-03-11 21:38:08.000000 pyerrors-2.8.1/pyerrors/linalg.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     5381 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/misc.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2273 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/mpm.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    67930 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/obs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1466 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/roots.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       22 2023-06-01 12:33:26.000000 pyerrors-2.8.1/pyerrors/version.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/pyerrors.egg-info/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/PKG-INFO
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2700 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/SOURCES.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        1 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/dependency_links.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      202 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/requires.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        9 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/top_level.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      100 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyproject.toml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       38 2023-06-01 12:41:28.620364 pyerrors-2.8.1/setup.cfg
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1888 2023-06-01 12:34:43.000000 pyerrors-2.8.1/setup.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1159 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/benchmark_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    17752 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/correlators_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3470 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/covobs_test.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/data/openqcd_test/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87320 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/openqcd_test/openqcd2r1.ms.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2076 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/openqcd_test/openqcd2r1.ms1.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   157504 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/openqcd_test/sfqcdr1.gfms.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      252 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/openqcd_test/sfqcdr1.rwms.dat
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/broken_data_c/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/data/sfcf_test/broken_data_c/data_c_r0/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8712 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/data/sfcf_test/data_a/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    24665 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.F_V0
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14670 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.f_1
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9090 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.f_A
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/data_c/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/data/sfcf_test/data_c/data_c_r0/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8918 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/data_o/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.620364 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     4926 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2927 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1811 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.620364 pyerrors-2.8.1/tests/data/sfcf_test/param/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   142045 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/param/out.out
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_a
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_c
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_o
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1885 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/dirac_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    44785 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/fits_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15556 2023-05-21 16:06:57.000000 pyerrors-2.8.1/tests/json_io_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14226 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/linalg_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      543 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/misc_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      314 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/mpm_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    46296 2023-06-01 12:29:24.000000 pyerrors-2.8.1/tests/obs_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9253 2023-06-01 12:29:24.000000 pyerrors-2.8.1/tests/openQCD_in_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    11768 2023-06-01 12:29:24.000000 pyerrors-2.8.1/tests/pandas_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1262 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/roots_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6431 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/sfcf_in_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1415 2023-05-21 16:06:57.000000 pyerrors-2.8.1/tests/utils_in_test.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/.github/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      113 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/CODEOWNERS
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1051 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/ISSUE_TEMPLATE/bug-report.yml
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/.github/workflows/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      386 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/binder.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      737 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/codeql.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1012 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/docs.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1022 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/examples.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      547 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/flake8.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1043 2023-06-02 14:05:30.000000 pyerrors-2.8.2/.github/workflows/pytest.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      211 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.gitignore
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16879 2023-06-02 14:06:35.000000 pyerrors-2.8.2/CHANGELOG.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1278 2023-06-02 10:22:14.000000 pyerrors-2.8.2/CITATION.cff
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1842 2023-03-21 12:48:56.000000 pyerrors-2.8.2/CONTRIBUTING.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1070 2023-03-11 21:38:08.000000 pyerrors-2.8.2/LICENSE
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-06-02 14:10:51.055575 pyerrors-2.8.2/PKG-INFO
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1610 2023-06-02 14:05:30.000000 pyerrors-2.8.2/README.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        0 2023-03-11 21:38:08.000000 pyerrors-2.8.2/conftest.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.043575 pyerrors-2.8.2/examples/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87858 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/01_basic_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    62623 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/02_correlators.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    97653 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/03_pcac_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   129847 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/04_fit_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9053 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/05_matrix_operations.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30851 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/06_gevp.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10604 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/07_data_management.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    21826 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/08_combined_fit_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      757 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/base_style.mplstyle
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.047575 pyerrors-2.8.2/examples/data/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7407 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/correlator_test.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15009 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/f_A.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15072 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/f_P.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266539 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/matrix_correlator.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266778 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/matrix_correlator_V1V1.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266803 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/matrix_correlator_V2V2.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266702 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/matrix_correlator_V3V3.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8575 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/json_schema.json
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.047575 pyerrors-2.8.2/pyerrors/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    29950 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/__init__.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    57481 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/correlators.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3609 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/covobs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2909 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/dirac.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30996 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/fits.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.051575 pyerrors-2.8.2/pyerrors/input/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      579 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/__init__.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    25145 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/input/bdio.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30920 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/dobs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    19262 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/hadrons.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    26602 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/json.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8064 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/misc.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    50595 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/openQCD.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6691 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/pandas.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16290 2023-06-01 13:18:57.000000 pyerrors-2.8.2/pyerrors/input/sfcf.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2257 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/utils.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10177 2023-03-11 21:38:08.000000 pyerrors-2.8.2/pyerrors/linalg.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     5381 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/misc.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2273 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/mpm.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    67936 2023-06-02 14:05:35.000000 pyerrors-2.8.2/pyerrors/obs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1466 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/roots.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       22 2023-06-02 14:06:00.000000 pyerrors-2.8.2/pyerrors/version.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.047575 pyerrors-2.8.2/pyerrors.egg-info/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/PKG-INFO
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2700 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/SOURCES.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        1 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/dependency_links.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      202 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/requires.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        9 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/top_level.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      100 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyproject.toml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       38 2023-06-02 14:10:51.055575 pyerrors-2.8.2/setup.cfg
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1888 2023-06-02 14:05:30.000000 pyerrors-2.8.2/setup.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.051575 pyerrors-2.8.2/tests/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1159 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/benchmark_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    17752 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/correlators_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3470 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/covobs_test.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/openqcd_test/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87320 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/openqcd_test/openqcd2r1.ms.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2076 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/openqcd_test/openqcd2r1.ms1.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   157504 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/openqcd_test/sfqcdr1.gfms.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      252 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/openqcd_test/sfqcdr1.rwms.dat
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/broken_data_c/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/broken_data_c/data_c_r0/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8712 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/data_a/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    24665 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.F_V0
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14670 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.f_1
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9090 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.f_A
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/data_c/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/data_c/data_c_r0/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8918 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/data_o/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     4926 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2927 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1811 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/param/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   142045 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/param/out.out
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_a
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_c
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_o
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1885 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/dirac_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    44785 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/fits_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15556 2023-06-02 10:22:14.000000 pyerrors-2.8.2/tests/json_io_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14226 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/linalg_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      543 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/misc_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      314 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/mpm_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    46473 2023-06-02 14:05:35.000000 pyerrors-2.8.2/tests/obs_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9253 2023-06-02 10:22:14.000000 pyerrors-2.8.2/tests/openQCD_in_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    11768 2023-06-02 14:05:30.000000 pyerrors-2.8.2/tests/pandas_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1262 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/roots_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6431 2023-06-01 13:14:45.000000 pyerrors-2.8.2/tests/sfcf_in_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1415 2023-06-02 10:22:14.000000 pyerrors-2.8.2/tests/utils_in_test.py
```

### Comparing `pyerrors-2.8.1/.github/ISSUE_TEMPLATE/bug-report.yml` & `pyerrors-2.8.2/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/.github/workflows/codeql.yml` & `pyerrors-2.8.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/.github/workflows/docs.yml` & `pyerrors-2.8.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/.github/workflows/examples.yml` & `pyerrors-2.8.2/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/.github/workflows/flake8.yml` & `pyerrors-2.8.2/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/.github/workflows/pytest.yml` & `pyerrors-2.8.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/CHANGELOG.md` & `pyerrors-2.8.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [2.8.2] - 2023-06-02
+### Fixed
+- Another bug appearing in an edge case of `_compute_drho` fixed.
+
 ## [2.8.1] - 2023-06-01
 ### Fixed
 - `input.pandas` can now deal with columns that only have `None` entries.
 - Bug in f-string conversion of `Obs` fixed.
 - Bug in edge case of `_compute_drho` fixed.
 - Several numpy 1.25 deprecations fixed.
```

### Comparing `pyerrors-2.8.1/CITATION.cff` & `pyerrors-2.8.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/CONTRIBUTING.md` & `pyerrors-2.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/LICENSE` & `pyerrors-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/PKG-INFO` & `pyerrors-2.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerrors
-Version: 2.8.1
+Version: 2.8.2
 Summary: Error propagation and statistical analysis for Monte Carlo simulations
 Home-page: https://github.com/fjosw/pyerrors
 Author: Fabian Joswig
 Author-email: fabian.joswig@ed.ac.uk
 License: MIT
 Project-URL: Documentation, https://fjosw.github.io/pyerrors/pyerrors.html
 Project-URL: Bug Tracker, https://github.com/fjosw/pyerrors/issues
```

### Comparing `pyerrors-2.8.1/README.md` & `pyerrors-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/01_basic_example.ipynb` & `pyerrors-2.8.2/examples/01_basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/02_correlators.ipynb` & `pyerrors-2.8.2/examples/02_correlators.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/03_pcac_example.ipynb` & `pyerrors-2.8.2/examples/03_pcac_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/04_fit_example.ipynb` & `pyerrors-2.8.2/examples/04_fit_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/05_matrix_operations.ipynb` & `pyerrors-2.8.2/examples/05_matrix_operations.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/06_gevp.ipynb` & `pyerrors-2.8.2/examples/06_gevp.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/07_data_management.ipynb` & `pyerrors-2.8.2/examples/07_data_management.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/08_combined_fit_example.ipynb` & `pyerrors-2.8.2/examples/08_combined_fit_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/base_style.mplstyle` & `pyerrors-2.8.2/examples/base_style.mplstyle`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/data/correlator_test.json.gz` & `pyerrors-2.8.2/examples/data/correlator_test.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/data/f_A.json.gz` & `pyerrors-2.8.2/examples/data/f_A.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/data/f_P.json.gz` & `pyerrors-2.8.2/examples/data/f_P.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/data/matrix_correlator.json.gz` & `pyerrors-2.8.2/examples/data/matrix_correlator.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/data/matrix_correlator_V1V1.json.gz` & `pyerrors-2.8.2/examples/data/matrix_correlator_V1V1.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/data/matrix_correlator_V2V2.json.gz` & `pyerrors-2.8.2/examples/data/matrix_correlator_V2V2.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/data/matrix_correlator_V3V3.json.gz` & `pyerrors-2.8.2/examples/data/matrix_correlator_V3V3.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/examples/json_schema.json` & `pyerrors-2.8.2/examples/json_schema.json`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/__init__.py` & `pyerrors-2.8.2/pyerrors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/correlators.py` & `pyerrors-2.8.2/pyerrors/correlators.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/covobs.py` & `pyerrors-2.8.2/pyerrors/covobs.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/dirac.py` & `pyerrors-2.8.2/pyerrors/dirac.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/fits.py` & `pyerrors-2.8.2/pyerrors/fits.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/__init__.py` & `pyerrors-2.8.2/pyerrors/input/__init__.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/bdio.py` & `pyerrors-2.8.2/pyerrors/input/bdio.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/dobs.py` & `pyerrors-2.8.2/pyerrors/input/dobs.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/hadrons.py` & `pyerrors-2.8.2/pyerrors/input/hadrons.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/json.py` & `pyerrors-2.8.2/pyerrors/input/json.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/misc.py` & `pyerrors-2.8.2/pyerrors/input/misc.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/openQCD.py` & `pyerrors-2.8.2/pyerrors/input/openQCD.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/pandas.py` & `pyerrors-2.8.2/pyerrors/input/pandas.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/sfcf.py` & `pyerrors-2.8.2/pyerrors/input/sfcf.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/input/utils.py` & `pyerrors-2.8.2/pyerrors/input/utils.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/linalg.py` & `pyerrors-2.8.2/pyerrors/linalg.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/misc.py` & `pyerrors-2.8.2/pyerrors/misc.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/mpm.py` & `pyerrors-2.8.2/pyerrors/mpm.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors/obs.py` & `pyerrors-2.8.2/pyerrors/obs.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             self.e_n_tauint[e_name][self.e_n_tauint[e_name] <= 0.5] = 0.5 + np.finfo(np.float64).eps
             # hep-lat/0306017 eq. (42)
             self.e_n_dtauint[e_name] = self.e_n_tauint[e_name] * 2 * np.sqrt(np.abs(np.arange(w_max) + 0.5 - self.e_n_tauint[e_name]) / e_N)
             self.e_n_dtauint[e_name][0] = 0.0
 
             def _compute_drho(i):
                 tmp = (self.e_rho[e_name][i + 1:w_max]
-                       + np.concatenate([self.e_rho[e_name][i - 1:None if i - w_max // 2 <= 0 else (2 * i - (2 * w_max) // 2):-1],
+                       + np.concatenate([self.e_rho[e_name][i - 1:None if i - (w_max - 1) // 2 <= 0 else (2 * i - (2 * w_max) // 2):-1],
                                          self.e_rho[e_name][1:max(1, w_max - 2 * i)]])
                        - 2 * self.e_rho[e_name][i] * self.e_rho[e_name][1:w_max - i])
                 self.e_drho[e_name][i] = np.sqrt(np.sum(tmp ** 2) / e_N)
 
             if self.tau_exp[e_name] > 0:
                 _compute_drho(1)
                 texp = self.tau_exp[e_name]
```

### Comparing `pyerrors-2.8.1/pyerrors/roots.py` & `pyerrors-2.8.2/pyerrors/roots.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/pyerrors.egg-info/PKG-INFO` & `pyerrors-2.8.2/pyerrors.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerrors
-Version: 2.8.1
+Version: 2.8.2
 Summary: Error propagation and statistical analysis for Monte Carlo simulations
 Home-page: https://github.com/fjosw/pyerrors
 Author: Fabian Joswig
 Author-email: fabian.joswig@ed.ac.uk
 License: MIT
 Project-URL: Documentation, https://fjosw.github.io/pyerrors/pyerrors.html
 Project-URL: Bug Tracker, https://github.com/fjosw/pyerrors/issues
```

### Comparing `pyerrors-2.8.1/pyerrors.egg-info/SOURCES.txt` & `pyerrors-2.8.2/pyerrors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/setup.py` & `pyerrors-2.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/benchmark_test.py` & `pyerrors-2.8.2/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/correlators_test.py` & `pyerrors-2.8.2/tests/correlators_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/covobs_test.py` & `pyerrors-2.8.2/tests/covobs_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat` & `pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat` & `pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat` & `pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/openqcd_test/openqcd2r1.ms.dat` & `pyerrors-2.8.2/tests/data/openqcd_test/openqcd2r1.ms.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/openqcd_test/openqcd2r1.ms1.dat` & `pyerrors-2.8.2/tests/data/openqcd_test/openqcd2r1.ms1.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/openqcd_test/sfqcdr1.gfms.dat` & `pyerrors-2.8.2/tests/data/openqcd_test/sfqcdr1.gfms.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1` & `pyerrors-2.8.2/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.F_V0` & `pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.F_V0`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.f_1` & `pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.f_1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.f_A` & `pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.f_A`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1` & `pyerrors-2.8.2/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0` & `pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1` & `pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A` & `pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/param/out.out` & `pyerrors-2.8.2/tests/data/sfcf_test/param/out.out`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_a` & `pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_a`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_c` & `pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_c`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_o` & `pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_o`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/dirac_test.py` & `pyerrors-2.8.2/tests/dirac_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/fits_test.py` & `pyerrors-2.8.2/tests/fits_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/json_io_test.py` & `pyerrors-2.8.2/tests/json_io_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/linalg_test.py` & `pyerrors-2.8.2/tests/linalg_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/misc_test.py` & `pyerrors-2.8.2/tests/misc_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/obs_test.py` & `pyerrors-2.8.2/tests/obs_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1278,7 +1278,12 @@
 def test_f_string_obs():
     o1 = pe.pseudo_Obs(0.348, 0.0123, "test")
     print(f"{o1}")
     print(f"{o1:3}")
     print(f"{o1:+3}")
     print(f"{o1:-1}")
     print(f"{o1: 8}")
+
+def test_compute_drho_fails():
+    obs = pe.input.json.load_json("tests/data/compute_drho_fails.json.gz")
+    obs.gm()
+    assert np.isclose(obs.dvalue, 0.0022150779611891094)
```

### Comparing `pyerrors-2.8.1/tests/openQCD_in_test.py` & `pyerrors-2.8.2/tests/openQCD_in_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/pandas_test.py` & `pyerrors-2.8.2/tests/pandas_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/roots_test.py` & `pyerrors-2.8.2/tests/roots_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/sfcf_in_test.py` & `pyerrors-2.8.2/tests/sfcf_in_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.1/tests/utils_in_test.py` & `pyerrors-2.8.2/tests/utils_in_test.py`

 * *Files identical despite different names*

